# Comparing `tmp/fal-0.8.6.tar.gz` & `tmp/fal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-0.8.6.tar", max compression
+gzip compressed data, was "fal-0.9.0.tar", max compression
```

## Comparing `fal-0.8.6.tar` & `fal-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0    11804 2023-04-25 13:28:20.723917 fal-0.8.6/README.md
--rw-r--r--   0        0        0     2627 2023-04-25 13:28:30.203974 fal-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      221 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/__init__.py
--rw-r--r--   0        0        0       21 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/__init__.py
--rw-r--r--   0        0        0     8470 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/args.py
--rw-r--r--   0        0        0     2120 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/cli.py
--rw-r--r--   0        0        0     5243 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/dbt_runner.py
--rw-r--r--   0        0        0     6045 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/fal_runner.py
--rw-r--r--   0        0        0     4473 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/flow_runner.py
--rw-r--r--   0        0        0       56 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/model_generator/__init__.py
--rw-r--r--   0        0        0     5505 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/model_generator/model_generator.py
--rw-r--r--   0        0        0     3180 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/model_generator/module_check.py
--rw-r--r--   0        0        0     9707 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/cli/selectors.py
--rw-r--r--   0        0        0    12440 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/fal_script.py
--rw-r--r--   0        0        0        0 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/feature_store/__init__.py
--rw-r--r--   0        0        0      401 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/feature_store/feature.py
--rw-r--r--   0        0        0     8394 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/node_graph.py
--rw-r--r--   0        0        0        0 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/bridge.py
--rw-r--r--   0        0        0     5332 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/dependency_analysis.py
--rw-r--r--   0        0        0      793 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/environments/__init__.py
--rw-r--r--   0        0        0     9482 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/environments/base.py
--rw-r--r--   0        0        0     4395 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/environments/conda.py
--rw-r--r--   0        0        0     3369 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/environments/virtual_env.py
--rw-r--r--   0        0        0     4776 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/packages/isolated_runner.py
--rw-r--r--   0        0        0        0 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/planner/__init__.py
--rw-r--r--   0        0        0     5635 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/planner/executor.py
--rw-r--r--   0        0        0     6475 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/planner/plan.py
--rw-r--r--   0        0        0     6761 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/planner/schedule.py
--rw-r--r--   0        0        0     9041 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/planner/tasks.py
--rw-r--r--   0        0        0        0 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/telemetry/__init__.py
--rw-r--r--   0        0        0    11416 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/telemetry/telemetry.py
--rw-r--r--   0        0        0     3043 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/typing.py
--rw-r--r--   0        0        0     1654 2023-04-25 13:28:20.739917 fal-0.8.6/src/fal/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/__init__.py
--rw-r--r--   0        0        0    24315 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/lib.py
--rw-r--r--   0        0        0     3273 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/logger.py
--rw-r--r--   0        0        0     1850 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/magics.py
--rw-r--r--   0        0        0     8935 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/parse.py
--rw-r--r--   0        0        0    25871 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/project.py
--rw-r--r--   0        0        0        0 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/utils/__init__.py
--rw-r--r--   0        0        0     1970 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/utils/yaml_helper.py
--rw-r--r--   0        0        0      317 2023-04-25 13:28:20.739917 fal-0.8.6/src/faldbt/version.py
--rw-r--r--   0        0        0       33 2023-04-25 13:28:20.743917 fal-0.8.6/tests/_fal_testing/__init__.py
--rw-r--r--   0        0        0     1782 2023-04-25 13:28:20.743917 fal-0.8.6/tests/_fal_testing/utils.py
--rw-r--r--   0        0        0    14134 2023-04-25 13:28:32.000357 fal-0.8.6/setup.py
--rw-r--r--   0        0        0    13983 2023-04-25 13:28:32.001269 fal-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    11804 2023-05-12 18:03:34.238037 fal-0.9.0/README.md
+-rw-r--r--   0        0        0     2617 2023-05-12 18:03:45.242026 fal-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-05-12 18:03:34.246038 fal-0.9.0/src/fal/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-12 18:03:34.246038 fal-0.9.0/src/fal/cli/__init__.py
+-rw-r--r--   0        0        0     8499 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/args.py
+-rw-r--r--   0        0        0     2120 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/cli.py
+-rw-r--r--   0        0        0     5469 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/dbt_runner.py
+-rw-r--r--   0        0        0     6159 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/fal_runner.py
+-rw-r--r--   0        0        0     4430 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/flow_runner.py
+-rw-r--r--   0        0        0       56 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/model_generator/__init__.py
+-rw-r--r--   0        0        0     5505 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/model_generator/model_generator.py
+-rw-r--r--   0        0        0     3180 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/model_generator/module_check.py
+-rw-r--r--   0        0        0     9742 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/cli/selectors.py
+-rw-r--r--   0        0        0    12306 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/fal_script.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/feature_store/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/feature_store/feature.py
+-rw-r--r--   0        0        0     8394 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/node_graph.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/bridge.py
+-rw-r--r--   0        0        0     5332 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/dependency_analysis.py
+-rw-r--r--   0        0        0      793 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/__init__.py
+-rw-r--r--   0        0        0     9482 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/base.py
+-rw-r--r--   0        0        0     4395 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/conda.py
+-rw-r--r--   0        0        0     3369 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/environments/virtual_env.py
+-rw-r--r--   0        0        0     4776 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/packages/isolated_runner.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/__init__.py
+-rw-r--r--   0        0        0     5635 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/executor.py
+-rw-r--r--   0        0        0     6475 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/plan.py
+-rw-r--r--   0        0        0     6761 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/schedule.py
+-rw-r--r--   0        0        0     9041 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/planner/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/telemetry/__init__.py
+-rw-r--r--   0        0        0    11416 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/telemetry/telemetry.py
+-rw-r--r--   0        0        0     3043 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/typing.py
+-rw-r--r--   0        0        0     1711 2023-05-12 18:03:34.250038 fal-0.9.0/src/fal/utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/__init__.py
+-rw-r--r--   0        0        0    24156 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/lib.py
+-rw-r--r--   0        0        0     3273 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/logger.py
+-rw-r--r--   0        0        0     1850 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/magics.py
+-rw-r--r--   0        0        0     8806 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/parse.py
+-rw-r--r--   0        0        0    26552 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/project.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/utils/__init__.py
+-rw-r--r--   0        0        0     1970 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/utils/yaml_helper.py
+-rw-r--r--   0        0        0      317 2023-05-12 18:03:34.250038 fal-0.9.0/src/faldbt/version.py
+-rw-r--r--   0        0        0       33 2023-05-12 18:03:34.250038 fal-0.9.0/tests/_fal_testing/__init__.py
+-rw-r--r--   0        0        0     1786 2023-05-12 18:03:34.250038 fal-0.9.0/tests/_fal_testing/utils.py
+-rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 fal-0.9.0/PKG-INFO
```

### Comparing `fal-0.8.6/README.md` & `fal-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/pyproject.toml` & `fal-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fal"
-version = "0.8.6"
+version = "0.9.0"
 description = "fal allows you to run python scripts directly from your dbt project."
 homepage = "https://github.com/fal-ai/fal/blob/-/projects/fal"
 documentation = "https://docs.fal.ai"
 repository = "https://github.com/fal-ai/fal"
 readme = "README.md"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
@@ -17,15 +17,15 @@
 classifiers = [
     "Development Status :: 4 - Beta"
 ]
 
 [tool.poetry.dependencies]
 # TODO: Python 3.11 after dill>0.3.6 version
 python = ">=3.7.2, <3.11"
-dbt-core = ">=1.4,<1.5"
+dbt-core = ">=1.5,<1.6"
 pandas = "^1.3.4"
 PyYAML = "^6.0"
 agate-sql = "^0.5.8"
 requests = "^2.27.1"
 posthog = "^1.4.5"
 astor = "^0.8.1"
 deprecation = "^2.1.0"
@@ -37,15 +37,15 @@
 dill = "^0.3.5.1, <0.3.6"
 importlib-metadata = ">=4.12.0"
 packaging = "<22"
 
 # Adapters
 
 ## snowflake
-snowflake-connector-python = { version = ">=2.8.0, <2.8.2", extras = ["pandas"], optional = true }
+snowflake-connector-python = { version = "~=3.0", extras = ["pandas"], optional = true }
 
 ## bigquery
 ### version defined by dbt-bigquery, installs pyarrow<8
 google-cloud-bigquery = { version = "~3.5.0", extras = ["pandas"], optional = true }
 
 ## redshift
 sqlalchemy-redshift = { version = "^0.8.9", optional = true }
```

### Comparing `fal-0.8.6/src/fal/cli/args.py` & `fal-0.9.0/src/fal/cli/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         defined in your dbt_project.yml file. This argument should be a YAML
         string, eg. '{my_variable: my_value}'
         """,
     )
 
 
 def _build_dbt_selectors(sub: argparse.ArgumentParser):
-
     # fmt: off
     sub.add_argument(
         "-s", "--select",
         nargs="+",
         dest="select",
         help="Specify the nodes to include.",
     )
@@ -141,21 +140,21 @@
         nargs="+",
         help="Specify the nodes to exclude.",
     )
     # fmt: on
 
 
 def _build_run_parser(sub: argparse.ArgumentParser):
-
     # fmt: off
     _build_dbt_selectors(sub)
     _build_dbt_common_options(sub)
     _build_fal_common_options(sub)
     _add_threads_option(sub)
     _add_target_option(sub)
+    _add_vars_option(sub)
 
     sub.add_argument(
         "--all",
         action="store_true",
         help="Run scripts for all models. By default, fal runs scripts for models that ran in the last dbt run.",
     )
     sub.add_argument(
@@ -176,15 +175,14 @@
         default=False,
         help="Run global scripts along with selected scripts",
     )
     # fmt: on
 
 
 def _build_flow_parser(sub: argparse.ArgumentParser):
-
     flow_command_parsers = sub.add_subparsers(
         title="flow commands",
         dest="flow_command",
         metavar="COMMAND",
         required=True,
     )
     _build_dbt_common_options(sub)
@@ -210,41 +208,42 @@
         dest="cloud_command",
         metavar="COMMAND",
         required=True,
     )
 
     cloud_command_parsers.add_parser(
         name="login",
-        help="Login to fal cloud"
+        help="Login to fal cloud",
     )
 
     cloud_command_parsers.add_parser(
         name="logout",
-        help="Logout of fal cloud"
+        help="Logout of fal cloud",
     )
 
     generator_parser = cloud_command_parsers.add_parser(
         name="key-generate",
-        help="Generate a secret key for fal cloud"
+        help="Generate a secret key for fal cloud",
     )
 
     generator_parser.add_argument(
         "--host",
         type=str,
         default="api.alpha.fal.ai",
-        help="Specify fal cloud host instance URL"
+        help="Specify fal cloud host instance URL",
     )
 
     generator_parser.add_argument(
         "--port",
         type=str,
         default="443",
-        help="Specify fal cloud host instance PORT"
+        help="Specify fal cloud host instance PORT",
     )
 
+
 def _build_cli_parser():
     parser = argparse.ArgumentParser(
         prog="fal",
         description="Run Python scripts on dbt models",
     )
 
     version = pkg_resources.get_distribution("fal").version
```

### Comparing `fal-0.8.6/src/fal/cli/cli.py` & `fal-0.9.0/src/fal/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/cli/dbt_runner.py` & `fal-0.9.0/src/fal/cli/dbt_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,32 +99,38 @@
     # a crash. We'll mirror the solution from DBT, until it is fixed on
     # upstream.
     #
     # PR from dbt-core: https://github.com/dbt-labs/dbt-core/pull/4866
 
     warnings.filterwarnings("ignore", category=DeprecationWarning, module="logbook")
 
-    from dbt.main import handle_and_check
+    from dbt.cli.main import dbtRunner
+    from dbt.contracts.results import RunExecutionResult
 
-    run_results = exc = None
+    runner = dbtRunner()
+
+    run_results: Optional[RunExecutionResult] = None
+    exc = None
     try:
-        run_results, success = handle_and_check(args)
+        runner_run_results = runner.invoke(args)
+        run_results = runner_run_results.result
     except BaseException as _exc:
-        return_code = getattr(exc, "code", 1)
+        return_code = getattr(_exc, "code", 1)
         exc = _exc
     else:
-        return_code = 0 if success else 1
+        return_code = 0 if runner_run_results.success else 1
 
     LOGGER.debug(f"dbt exited with return code {return_code}")
 
     # The 'run_results' object has a 'write()' method which is basically json.dump().
     # We'll dump it directly to the fal results file (instead of first dumping it to
     # run results and then copying it over).
     if run_results is not None:
-        run_results.write(os.path.join(target_path, f"fal_results_{run_index}.json"))
+        run_results_path = os.path.join(target_path, f"fal_results_{run_index}.json")
+        run_results.write(run_results_path)
     else:
         connection.send(exc)
         return
 
     connection.send(return_code)
```

### Comparing `fal-0.8.6/src/fal/cli/fal_runner.py` & `fal-0.9.0/src/fal/cli/fal_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import argparse
 from pathlib import Path
 from typing import Any, Dict, List
 
-from dbt.flags import PROFILES_DIR
+from dbt.flags import get_flags, set_from_args
 from fal.planner.executor import parallel_executor
 from fal.planner.schedule import Scheduler
 from fal.planner.tasks import FalLocalHookTask, Status, TaskGroup
+from dbt.cli.resolvers import default_profiles_dir
 
 from fal.fal_script import FalScript, TimingType
 from faldbt.project import FAL, DbtModel, FalDbt, FalGeneralException
 
 
 def create_fal_dbt(
     args: argparse.Namespace, generated_models: Dict[str, Path] = {}
 ) -> FalDbt:
-    profiles_dir = PROFILES_DIR
-    if args.profiles_dir is not None:
-        profiles_dir = args.profiles_dir
+    if args.profiles_dir is None:
+        args.profiles_dir = default_profiles_dir()
+
+    set_from_args(args, None)
+    flags = get_flags()
+    profiles_dir = flags.PROFILES_DIR
 
     real_state = None
     if hasattr(args, "state") and args.state is not None:
         real_state = args.state
 
     return FalDbt(
         args.project_dir,
         profiles_dir,
         args.select,
         args.exclude,
         args.selector,
         args.threads,
         real_state,
         args.target,
-        getattr(args, "vars", "{}"),
+        args.vars,
         generated_models,
     )
 
 
 def fal_run(args: argparse.Namespace):
     "Runs the fal run command in a subprocess"
 
@@ -150,15 +154,15 @@
     selected_ids = _models_ids(faldbt._compile_task._flattened_nodes)
     filtered_models: List[DbtModel] = []
 
     if (
         not all
         and not selected
         and not before
-        and faldbt._run_results.nativeRunResult is None
+        and faldbt._run_results.native_run_result is None
     ):
         from faldbt.parse import FalParseError
 
         raise FalParseError(
             "Cannot define models to run without selection flags or dbt run_results artifact or --before flag"
         )
```

### Comparing `fal-0.8.6/src/fal/cli/flow_runner.py` & `fal-0.9.0/src/fal/cli/flow_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,16 @@
         connected_graph, enable_chunking=False
     )
     scheduler = schedule_graph(planned_graph.graph, node_graph)
     return parallel_executor(parsed, fal_dbt, scheduler)
 
 
 def fal_flow_run(parsed: argparse.Namespace) -> int:
-    arg_vars = getattr(parsed, "vars", "{}")
-
     # fal-format Python models
-    generated_models = generate_python_dbt_models(parsed.project_dir, arg_vars)
+    generated_models = generate_python_dbt_models(parsed.project_dir, parsed.vars)
 
     fal_dbt = create_fal_dbt(parsed, generated_models)
     _mark_dbt_nodes_status(fal_dbt, NodeStatus.Skipped)
 
     node_graph = NodeGraph.from_fal_dbt(fal_dbt)
     exit_code = run_threaded(fal_dbt=fal_dbt, parsed=parsed, node_graph=node_graph)
```

### Comparing `fal-0.8.6/src/fal/cli/model_generator/model_generator.py` & `fal-0.9.0/src/fal/cli/model_generator/model_generator.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/cli/model_generator/module_check.py` & `fal-0.9.0/src/fal/cli/model_generator/module_check.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/cli/selectors.py` & `fal-0.9.0/src/fal/cli/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             if self.children_with_parents:
                 ids = _get_children_with_parents(id, nodeGraph)
                 yield from ids
 
 
 def unique_ids_from_complex_selector(select, fal_dbt: FalDbt) -> List[str]:
     args = CompileArgs(None, [select], [select], tuple(), fal_dbt._state, None)
-    compile_task = CompileTask(args, fal_dbt._config)
+    compile_task = CompileTask(args, fal_dbt._config, fal_dbt._manifest.native_manifest)
     compile_task._runtime_initialize()
     spec = compile_task.get_selection_spec()
     graph = compile_task.get_node_selector().get_graph_queue(spec)
     return list(graph.queued)
 
 def unique_ids_from_tag_selector(selector: str, fal_dbt: FalDbt) -> List[str]:
     parts = selector.split(":")
```

### Comparing `fal-0.8.6/src/fal/fal_script.py` & `fal-0.9.0/src/fal/fal_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,16 @@
 from faldbt.project import DbtModel, FalDbt, FAL
 
 from dbt.contracts.results import RunStatus
 from dbt.config.runtime import RuntimeConfig
 from faldbt.logger import LOGGER
 
 from fal.telemetry import telemetry
-import faldbt.version as version
 
-if version.is_version_plus("1.4.0"):
-    from dbt.contracts.graph.nodes import ColumnInfo
-else:
-    from dbt.contracts.graph.parsed import ColumnInfo
+from dbt.contracts.graph.nodes import ColumnInfo
 
 
 class TimingType(Enum):
     PRE = "pre"
     POST = "post"
 
     def for_script(self):
```

### Comparing `fal-0.8.6/src/fal/node_graph.py` & `fal-0.9.0/src/fal/node_graph.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/bridge.py` & `fal-0.9.0/src/fal/packages/bridge.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/dependency_analysis.py` & `fal-0.9.0/src/fal/packages/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/environments/__init__.py` & `fal-0.9.0/src/fal/packages/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/environments/base.py` & `fal-0.9.0/src/fal/packages/environments/base.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/environments/conda.py` & `fal-0.9.0/src/fal/packages/environments/conda.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/environments/virtual_env.py` & `fal-0.9.0/src/fal/packages/environments/virtual_env.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/packages/isolated_runner.py` & `fal-0.9.0/src/fal/packages/isolated_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/planner/executor.py` & `fal-0.9.0/src/fal/planner/executor.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/planner/plan.py` & `fal-0.9.0/src/fal/planner/plan.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/planner/schedule.py` & `fal-0.9.0/src/fal/planner/schedule.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/planner/tasks.py` & `fal-0.9.0/src/fal/planner/tasks.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/telemetry/telemetry.py` & `fal-0.9.0/src/fal/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/typing.py` & `fal-0.9.0/src/fal/typing.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/fal/utils.py` & `fal-0.9.0/src/fal/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Fal utilities."""
 import copy
 from faldbt.logger import LOGGER
-from typing import List, TYPE_CHECKING
-
+from typing import List, TYPE_CHECKING, TypeVar
 
 try:
     from functools import lru_cache
 except ImportError:
     from backports.functools_lru_cache import lru_cache
 
 if TYPE_CHECKING:
@@ -44,16 +43,17 @@
 
     def __getstate__(self):
         return self._serialization_state
 
     def __setstate__(self, state):
         super().__init__(*state["args"], **state["kwargs"])
 
+Cls = TypeVar("Cls", bound=type)
 
-def has_side_effects(cls):
+def has_side_effects(cls: "Cls") -> "Cls":
     """The given class has possible side-effects that might
     make the regular serialization problematic (e.g. registering
     adapters to DBT's global factory)."""
     return type(cls.__name__, (_ReInitialize, cls), {})
 
 
 def cache_static(func):
```

### Comparing `fal-0.8.6/src/faldbt/lib.py` & `fal-0.9.0/src/faldbt/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,20 @@
 from typing import Iterator, List, Optional, Tuple
 from urllib.parse import quote_plus
 import threading
 
 import dbt.flags as flags
 import dbt.adapters.factory as adapters_factory
 
-import faldbt.version as version
-
 from dbt.contracts.connection import AdapterResponse
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.base import BaseRelation, BaseAdapter, BaseConnectionManager
 from dbt.config import RuntimeConfig
 
-if version.is_version_plus("1.4.0"):
-    from dbt.contracts.graph.nodes import ResultNode
-else:
-    from dbt.contracts.graph.compiled import CompileResultNode as ResultNode
+from dbt.contracts.graph.nodes import ResultNode
 
 import pandas as pd
 from pandas.io import sql as pdsql
 
 import agate
 import sqlalchemy
 from sqlalchemy.sql.ddl import CreateTable
@@ -119,15 +114,14 @@
 
 def _execute_sql(
     adapter: SQLAdapter,
     sql: str,
     *,
     new_conn=True,
 ) -> Tuple[AdapterResponse, pd.DataFrame]:
-
     if adapter.type() == "bigquery":
         return _bigquery_execute_sql(adapter, sql, new_conn)
 
     if adapter.type() == "snowflake":
         return _snowflake_execute_sql(adapter, sql, new_conn)
 
     with _existing_or_new_connection(
```

### Comparing `fal-0.8.6/src/faldbt/logger.py` & `fal-0.9.0/src/faldbt/logger.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/faldbt/magics.py` & `fal-0.9.0/src/faldbt/magics.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/src/faldbt/parse.py` & `fal-0.9.0/src/faldbt/parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 from dbt.config import RuntimeConfig, Project
 from dbt.config.utils import parse_cli_vars
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.results import RunResultsArtifact, FreshnessExecutionResultArtifact
 from dbt.contracts.project import UserConfig
 from dbt.config.profile import read_user_config
 
-import faldbt.version as version
-
-if version.is_version_plus("1.4.0"):
-    from dbt.exceptions import IncompatibleSchemaError, DbtRuntimeError
-else:
-    from dbt.exceptions import IncompatibleSchemaException as IncompatibleSchemaError, RuntimeException as DbtRuntimeError
+from dbt.exceptions import IncompatibleSchemaError, DbtRuntimeError
 
 from fal.utils import cache_static
 
 from faldbt.logger import LOGGER
 from faldbt.utils.yaml_helper import load_yaml
 from fal.telemetry import telemetry
 
@@ -44,14 +39,15 @@
 class RuntimeArgs:
     project_dir: str
     profiles_dir: str
     threads: Optional[int]
     single_threaded: bool
     profile: Optional[str]
     target: Optional[str]
+    vars: Dict[str, str]
 
 
 def load_dbt_project_contract(project_dir: str) -> ProjectContract:
     partial_project = Project.partial_load(project_dir)
     contract = ProjectContract.from_dict(partial_project.project_dict)
     if not hasattr(contract, "model_paths") or contract.model_paths is None:
         setattr(contract, "model_paths", contract.source_paths)
@@ -63,36 +59,47 @@
 def get_dbt_config(
     *,
     project_dir: str,
     profiles_dir: str,
     profile_target: Optional[str] = None,
     threads: Optional[int] = None,
     profile: Optional[str] = None,
+    vars: str = "{}",
 ) -> RuntimeConfig:
     # Construct a phony config
     import os
 
+    vars_dict = parse_cli_vars(vars)
+
     args = RuntimeArgs(
         project_dir=project_dir,
         profiles_dir=profiles_dir,
         threads=threads,
         single_threaded=False,
         profile=profile,
         target=profile_target,
+        vars=vars_dict,
     )
 
     if project_dir and not "PYTEST_CURRENT_TEST" in os.environ:
         # HACK: initializing dbt-fal requires cwd to be project_dir
         # TODO: this doesn't work in pytest + Github Actions
         owd = os.getcwd()
         os.chdir(project_dir)
         config = RuntimeConfig.from_args(args)
         os.chdir(owd)
     else:
         config = RuntimeConfig.from_args(args)
+
+    # HACK: issue in dbt-core 1.5.0 https://github.com/dbt-labs/dbt-core/issues/7465
+    env_target_path = os.getenv("DBT_TARGET_PATH")
+    if env_target_path:
+        config.target_path = env_target_path
+    # TODO: should we check flags too?
+
     return config
 
 
 def get_vars_dict(project_dir: str, args_vars: str) -> Dict[str, Any]:
     project_contract = load_dbt_project_contract(project_dir)
 
     # NOTE: This happens usually inside unit tests
@@ -140,43 +147,33 @@
 def get_dbt_manifest(config) -> Manifest:
     from dbt.parser.manifest import ManifestLoader
 
     return ManifestLoader.get_full_manifest(config)
 
 
 def get_dbt_sources_artifact(project_dir: str, config: RuntimeConfig):
-    sources_path = os.path.join(project_dir, config.target_path, "sources.json")
+    # Changed in dbt 1.5.0 to use path relative to CWD instead of path relative to project_dir
+    sources_path = os.path.join(config.target_path, "sources.json")
     try:
-        # BACKWARDS: Change intorduced in 1.0.0
-        if hasattr(FreshnessExecutionResultArtifact, "read_and_check_versions"):
-            return FreshnessExecutionResultArtifact.read_and_check_versions(
-                sources_path
-            )
-        else:
-            return FreshnessExecutionResultArtifact.read(sources_path)
+        return FreshnessExecutionResultArtifact.read_and_check_versions(sources_path)
 
     except IncompatibleSchemaError as exc:
         # TODO: add test for this case
         exc.add_filename(sources_path)
         raise
     except DbtRuntimeError as exc:
         LOGGER.warn("Could not read dbt sources artifact")
         return None
 
 
-def get_dbt_results(
-    project_dir: str, config: RuntimeConfig
-) -> Optional[RunResultsArtifact]:
-    results_path = os.path.join(project_dir, config.target_path, "run_results.json")
+def get_dbt_results(project_dir: str, config: RuntimeConfig) -> Optional[RunResultsArtifact]:
+    # Changed in dbt 1.5.0 to use path relative to CWD instead of path relative to project_dir
+    results_path = os.path.join(config.target_path, "run_results.json")
     try:
-        # BACKWARDS: Change intorduced in 1.0.0
-        if hasattr(RunResultsArtifact, "read_and_check_versions"):
-            return RunResultsArtifact.read_and_check_versions(results_path)
-        else:
-            return RunResultsArtifact.read(results_path)
+        return RunResultsArtifact.read_and_check_versions(results_path)
 
     except IncompatibleSchemaError as exc:
         # TODO: add test for this case
         exc.add_filename(results_path)
         raise
     except DbtRuntimeError as exc:
         LOGGER.warn("Could not read dbt run_results artifact")
```

### Comparing `fal-0.8.6/src/faldbt/project.py` & `fal-0.9.0/src/faldbt/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 from collections import defaultdict
 import os.path
 from dataclasses import dataclass, field
-from functools import partialmethod
 from typing import (
     Dict,
     Iterable,
     List,
     Any,
     Optional,
     Tuple,
     Sequence,
     TYPE_CHECKING,
 )
 from pathlib import Path
+from deprecation import deprecated
 
 import faldbt.version as version
 
-if version.is_version_plus("1.4.0"):
-    from dbt.contracts.graph.nodes import (
-        SourceDefinition,
-        TestMetadata,
-        GenericTestNode,
-        SingularTestNode,
-    )
-    from dbt.contracts.graph.nodes import ManifestNode
-else:
-    from dbt.contracts.graph.parsed import (
-        ParsedSourceDefinition as SourceDefinition,
-        TestMetadata,
-        ParsedGenericTestNode as GenericTestNode,
-        ParsedSingularTestNode as SingularTestNode,
-    )
-    from dbt.contracts.graph.compiled import ManifestNode
+from dbt.cli.main import dbtRunner, dbtRunnerResult
+
+from dbt.contracts.graph.nodes import (
+    SourceDefinition,
+    TestMetadata,
+    GenericTestNode,
+    SingularTestNode,
+)
+from dbt.contracts.graph.nodes import ManifestNode
+
 from dbt.contracts.graph.manifest import (
     Manifest,
     MaybeNonSource,
     MaybeParsedSource,
     Disabled,
 )
 
@@ -45,15 +39,14 @@
     RunResultsArtifact,
     RunResultOutput,
     NodeStatus,
     FreshnessExecutionResultArtifact,
     FreshnessNodeOutput,
 )
 from dbt.task.compile import CompileTask
-import dbt.tracking
 
 from . import parse
 from . import lib
 from . import version
 
 from fal.feature_store.feature import Feature
 
@@ -190,15 +183,15 @@
 
 
 @dataclass
 class DbtSource(_DbtTestableNode):
     freshness: Optional[FreshnessNodeOutput] = field(default=None)
 
     def __repr__(self):
-        attrs = ["name", "tests", "status"]
+        attrs = ["name", "table_name", "tests", "status"]
         props = ", ".join([f"{item}={repr(getattr(self, item))}" for item in attrs])
         return f"DbtSource({props})"
 
     @property
     def meta(self):
         return self.node.meta
 
@@ -313,20 +306,25 @@
         meta = self.meta or {}
         fal = meta.get("fal") or {}
         return fal.get("environment")
 
 
 @dataclass
 class DbtRunResult:
-    nativeRunResult: Optional[RunResultsArtifact]
+    native_run_result: Optional[RunResultsArtifact]
+
+    @property
+    @deprecated(details="Use native_run_result instead")
+    def nativeRunResult(self):
+        return self.native_run_result
 
     @property
     def results(self) -> Sequence[RunResultOutput]:
-        if self.nativeRunResult:
-            return self.nativeRunResult.results
+        if self.native_run_result:
+            return self.native_run_result.results
         else:
             return []
 
 
 @dataclass
 class DbtFreshnessExecutionResult:
     _artifact: Optional[FreshnessExecutionResultArtifact]
@@ -337,32 +335,37 @@
             return self._artifact.results
         else:
             return []
 
 
 @dataclass
 class DbtManifest:
-    nativeManifest: Manifest
+    native_manifest: Manifest
+
+    @property
+    @deprecated(details="Use native_manifest instead")
+    def nativeManifest(self):
+        return self.native_manifest
 
     def get_model_nodes(self) -> Iterable[ManifestNode]:
         return (
             node
-            for node in self.nativeManifest.nodes.values()
+            for node in self.native_manifest.nodes.values()
             if node.resource_type == NodeType.Model
         )
 
     def get_test_nodes(self) -> Iterable[ManifestNode]:
         return (
             node
-            for node in self.nativeManifest.nodes.values()
+            for node in self.native_manifest.nodes.values()
             if node.resource_type == NodeType.Test
         )
 
     def get_source_nodes(self) -> Iterable[SourceDefinition]:
-        return self.nativeManifest.sources.values()
+        return self.native_manifest.sources.values()
 
     def _map_nodes(
         self,
         run_results: DbtRunResult,
         freshness_results: DbtFreshnessExecutionResult,
         generated_models: Dict[str, Path],
     ) -> Tuple[List[DbtModel], List[DbtSource], List[DbtTest]]:
@@ -418,15 +421,15 @@
             sources.append(source)
 
         return models, sources, tests
 
 
 @dataclass
 class CompileArgs:
-    selector_name: Optional[str]
+    selector: Optional[str]
     select: List[str]
     models: List[str]
     exclude: Tuple[str]
     state: Optional[Path]
     single_threaded: Optional[bool]
 
 
@@ -437,15 +440,15 @@
     # TODO: figure out a meaningful __repr__ for this class
     def __init__(
         self,
         project_dir: str,
         profiles_dir: str,
         select: List[str] = [],
         exclude: Tuple[str] = tuple(),
-        selector_name: Optional[str] = None,
+        selector: Optional[str] = None,
         threads: Optional[int] = None,
         state: Optional[str] = None,
         profile_target: Optional[str] = None,
         args_vars: str = "{}",
         generated_models: Dict[str, Path] = {},
     ):
         if not version.is_version_plus("1.0.0"):
@@ -465,46 +468,47 @@
 
         # Can be overwritten if profile_target is not None
         self._config = parse.get_dbt_config(
             project_dir=self.project_dir,
             profiles_dir=self.profiles_dir,
             profile_target=profile_target,
             threads=threads,
+            vars=args_vars
         )
 
         self._run_results = DbtRunResult(
             parse.get_dbt_results(self.project_dir, self._config)
         )
 
-        self.method = "run"
-
-        if self._run_results.nativeRunResult:
-            self.method = self._run_results.nativeRunResult.args["rpc_method"]
+        if self._run_results.native_run_result:
             if profile_target is None:
                 profile_target = _get_custom_target(self._run_results)
 
         if profile_target is not None:
             self._config = parse.get_dbt_config(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 threads=threads,
                 profile_target=profile_target,
             )
 
         lib.register_adapters(self._config)
 
+        parse_result = self._dbt_invoke("parse")
+        native_manifest: Manifest = parse_result.result # type: ignore
+
         # Necessary for manifest loading to not fail
-        dbt.tracking.initialize_tracking(self.profiles_dir)
+        # dbt.tracking.initialize_tracking(self.profiles_dir)
 
-        args = CompileArgs(selector_name, select, select, exclude, self._state, None)
-        self._compile_task = CompileTask(args, self._config)
+        args = CompileArgs(selector, select, select, exclude, self._state, None)
+        self._compile_task = CompileTask(args, self._config, native_manifest)
 
         self._compile_task._runtime_initialize()
 
-        self._manifest = DbtManifest(self._compile_task.manifest)
+        self._manifest = DbtManifest(native_manifest)
 
         freshness_execution_results = DbtFreshnessExecutionResult(
             parse.get_dbt_sources_artifact(self.project_dir, self._config)
         )
 
         self.models, self.sources, self.tests = self._manifest._map_nodes(
             self._run_results,
@@ -524,23 +528,42 @@
         self._environments = None
 
         telemetry.log_api(
             action="faldbt_initialized",
             dbt_config=self._config,
         )
 
+    def _dbt_invoke(
+        self, cmd: str, args: Optional[List[str]] = None
+    ) -> dbtRunnerResult:
+        runner = dbtRunner()
+
+        if args is None:
+            args = []
+
+        project_args = [
+            "--project-dir",
+            self.project_dir,
+            "--profiles-dir",
+            self.profiles_dir,
+            "--target",
+            self._profile_target,
+        ]
+
+        # TODO: Intervene the dbt logs and capture them to avoid printing them to the console
+        return runner.invoke([cmd] + project_args + args)
+
     @property
+    def model_paths(self) -> List[str]:
+        return self._config.model_paths
+
+    @property
+    @deprecated(details="Use model_paths instead")
     def source_paths(self) -> List[str]:
-        # BACKWARDS: Change intorduced in 1.0.0
-        if hasattr(self._config, "model_paths"):
-            return self._config.model_paths
-        elif hasattr(self._config, "source_paths"):
-            return self._config.source_paths  # type: ignore
-        else:
-            raise RuntimeError("No model_paths in config")
+        return self.model_paths
 
     @property
     def _profile_target(self):
         return self._config.target_name
 
     @property
     def threads(self):
@@ -622,16 +645,21 @@
                     )
                 )
         return features
 
     def _model(
         self, target_model_name: str, target_package_name: Optional[str]
     ) -> ManifestNode:
-        target_model: MaybeNonSource = self._manifest.nativeManifest.resolve_ref(
-            target_model_name, target_package_name, self.project_dir, self.project_dir
+        # HACK: always setting node package as self.project_dir
+        target_model: MaybeNonSource = self._manifest.native_manifest.resolve_ref(
+            target_model_name,
+            target_package_name,
+            None,
+            self.project_dir,
+            self.project_dir,
         )
         package_str = f"'{target_package_name}'." if target_package_name else ""
         model_str = f"{package_str}'{target_model_name}'"
         if target_model is None:
             raise Exception(f"Could not find model {model_str}")
 
         if isinstance(target_model, Disabled):
@@ -659,16 +687,22 @@
                 self._profile_target,
                 config=self._config,
             )
 
     def _source(
         self, target_source_name: str, target_table_name: str
     ) -> SourceDefinition:
-        target_source: MaybeParsedSource = self._manifest.nativeManifest.resolve_source(
-            target_source_name, target_table_name, self.project_dir, self.project_dir
+        # HACK: always setting node package as self.project_dir
+        target_source: MaybeParsedSource = (
+            self._manifest.native_manifest.resolve_source(
+                target_source_name,
+                target_table_name,
+                self.project_dir,
+                self.project_dir,
+            )
         )
 
         if target_source is None:
             raise RuntimeError(
                 f"Could not find source '{target_source_name}'.'{target_table_name}'"
             )
 
@@ -792,15 +826,14 @@
             else:
                 raise Exception(f"write_to_model mode `{mode}` not supported")
 
     def execute_sql(self, sql: str) -> pd.DataFrame:
         """Execute a sql query."""
 
         with telemetry.log_time("execute_sql", dbt_config=self._config):
-
             # HACK: we need to pass config in because of weird behavior of execute_sql when
             # ran from GitHub Actions. For some reason, it can not find the right profile.
             # Haven't been able to reproduce this behavior locally and therefore developed
             # this workaround.
             compiled_result = lib.compile_sql(
                 self.project_dir,
                 self.profiles_dir,
@@ -834,10 +867,10 @@
         """
         if self._environments is None:
             self._environments = parse.load_environments(self.project_dir)
         return self._environments[name]
 
 
 def _get_custom_target(run_results: DbtRunResult):
-    if "target" in run_results.nativeRunResult.args:
-        return run_results.nativeRunResult.args["target"]
+    if "target" in run_results.native_run_result.args:
+        return run_results.native_run_result.args["target"]
     return None
```

### Comparing `fal-0.8.6/src/faldbt/utils/yaml_helper.py` & `fal-0.9.0/src/faldbt/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.6/tests/_fal_testing/utils.py` & `fal-0.9.0/tests/_fal_testing/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if additional_data:
         output += f"\n{additional_data}"
 
     create_file(output, Path(model_name).with_suffix(suffix))
 
 
 def create_file(output, file_name):
-    temp_dir = Path(os.environ["temp_dir"])
+    temp_dir = Path(os.getenv("temp_dir", "."))
     temp_file = temp_dir / file_name
     temp_file.write_text(output)
 
 
 def create_model_artifact(context, additional_data=None):
     create_artifact(context, ".txt", additional_data)
```

### Comparing `fal-0.8.6/setup.py` & `fal-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,404 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fal
+Version: 0.9.0
+Summary: fal allows you to run python scripts directly from your dbt project.
+Home-page: https://github.com/fal-ai/fal/blob/-/projects/fal
+Keywords: dbt,pandas
+Author: Features & Labels
+Author-email: hello@fal.ai
+Requires-Python: >=3.7.2,<3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: athena
+Provides-Extra: bigquery
+Provides-Extra: cloud
+Provides-Extra: dev
+Provides-Extra: duckdb
+Provides-Extra: postgres
+Provides-Extra: redshift
+Provides-Extra: snowflake
+Provides-Extra: test
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: agate-sql (>=0.5.8,<0.6.0)
+Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: backports.functools_lru_cache (>=1.6.4,<2.0.0)
+Requires-Dist: behave (>=1.2.6,<2.0.0) ; extra == "test"
+Requires-Dist: black (>=22.3,<23.0) ; extra == "test"
+Requires-Dist: dbt-core (>=1.5,<1.6)
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: dill (>=0.3.5.1,<0.3.6)
+Requires-Dist: duckdb-engine (>=0.1.8,<0.2.0) ; extra == "duckdb"
+Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0) ; extra == "bigquery"
+Requires-Dist: importlib-metadata (>=4.12.0)
+Requires-Dist: koldstart (>=0.6.16,<0.7.0) ; extra == "cloud"
+Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "dev"
+Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "test"
+Requires-Dist: packaging (<22)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: platformdirs (>=2.5.2,<3.0.0)
+Requires-Dist: posthog (>=1.4.5,<2.0.0)
+Requires-Dist: pytest (>=5.2,<6.0) ; extra == "test"
+Requires-Dist: pytest-mock (>=3.7.0,<4.0.0) ; extra == "test"
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: snowflake-connector-python[pandas] (>=3.0,<4.0) ; extra == "snowflake"
+Requires-Dist: sqlalchemy-redshift (>=0.8.9,<0.9.0) ; extra == "redshift"
+Requires-Dist: virtualenv (>=20.16.2,<21.0.0)
+Project-URL: Documentation, https://docs.fal.ai
+Project-URL: Repository, https://github.com/fal-ai/fal
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'tests'}
+<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/fal/" target="_blank" /> -->
 
-packages = \
-['_fal_testing',
- 'fal',
- 'fal.cli',
- 'fal.cli.model_generator',
- 'fal.feature_store',
- 'fal.packages',
- 'fal.packages.environments',
- 'fal.planner',
- 'fal.telemetry',
- 'faldbt',
- 'faldbt.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'agate-sql>=0.5.8,<0.6.0',
- 'astor>=0.8.1,<0.9.0',
- 'backports.functools_lru_cache>=1.6.4,<2.0.0',
- 'dbt-core>=1.4,<1.5',
- 'deprecation>=2.1.0,<3.0.0',
- 'dill>=0.3.5.1,<0.3.6',
- 'importlib-metadata>=4.12.0',
- 'packaging<22',
- 'pandas>=1.3.4,<2.0.0',
- 'platformdirs>=2.5.2,<3.0.0',
- 'posthog>=1.4.5,<2.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'virtualenv>=20.16.2,<21.0.0']
-
-extras_require = \
-{'bigquery': ['google-cloud-bigquery[pandas]>=3.5.0,<3.6.0'],
- 'cloud': ['koldstart>=0.6.16,<0.7.0'],
- 'dev': ['matplotlib>=3.5.2,<4.0.0'],
- 'duckdb': ['duckdb-engine>=0.1.8,<0.2.0'],
- 'redshift': ['sqlalchemy-redshift>=0.8.9,<0.9.0'],
- 'snowflake': ['snowflake-connector-python[pandas]>=2.8.0,<2.8.2'],
- 'test': ['pytest>=5.2,<6.0',
-          'black>=22.3,<23.0',
-          'behave>=1.2.6,<2.0.0',
-          'mock>=4.0.3,<5.0.0',
-          'pytest-mock>=3.7.0,<4.0.0']}
-
-entry_points = \
-{'console_scripts': ['fal = fal.cli:cli']}
-
-setup_kwargs = {
-    'name': 'fal',
-    'version': '0.8.6',
-    'description': 'fal allows you to run python scripts directly from your dbt project.',
-    'long_description': '<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/fal/" target="_blank" /> -->\n\n# fal: do more with dbt\n\nfal is the easiest way to run Python with your [dbt](https://www.getdbt.com/) project.\n\n# Introduction\n\nWith the `fal` CLI, you can:\n\n- [Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example) upon dbt model success or failure.\n- [Load data from external data sources](https://blog.fal.ai/populate-dbt-models-with-csv-data/) before a model starts running.\n- [Download dbt models](https://docs.fal.ai/fal/python-package) into a Python context with a familiar syntax: `ref(\'my_dbt_model\')` using `FalDbt`\n- [Programatically access rich metadata](https://docs.fal.ai/fal/reference/variables-and-functions) about your dbt project.\n\nHead to our [documentation site](https://docs.fal.ai/) for a deeper dive or play with [in-depth examples](https://github.com/fal-ai/fal/blob/-/examples/README.md) to see how fal can help you get more done with dbt.\n\n> ❗️ If you would like to write data back to your data-warehouse, we recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter.\n\n# Getting Started\n\n## 1. Install `fal`\n\n```bash\n$ pip install fal\n```\n\n## 2. Go to your dbt project directory\n\n```bash\n$ cd ~/src/my_dbt_project\n```\n\n## 3. Create a Python script: `send_slack_message.py`\n\n```python\nimport os\nfrom slack_sdk import WebClient\nfrom slack_sdk.errors import SlackApiError\n\nCHANNEL_ID = os.getenv("SLACK_BOT_CHANNEL")\nSLACK_TOKEN = os.getenv("SLACK_BOT_TOKEN")\n\nclient = WebClient(token=SLACK_TOKEN)\nmessage_text = f"Model: {context.current_model.name}. Status: {context.current_model.status}."\n\ntry:\n    response = client.chat_postMessage(\n        channel=CHANNEL_ID,\n        text=message_text\n    )\nexcept SlackApiError as e:\n    assert e.response["error"]\n```\n\n## 4. Add a `meta` section in your `schema.yml`\n\n```yaml\nmodels:\n  - name: historical_ozone_levels\n    description: Ozone levels\n    config:\n      materialized: table\n    columns:\n      - name: ozone_level\n        description: Ozone level\n      - name: ds\n        description: Date\n    meta:\n      fal:\n        scripts:\n          - send_slack_message.py\n```\n\n## 5. Run `fal flow run`\n\n```bash\n$ fal flow run\n# both your dbt models and fal scripts are run\n```\n\n## 6. Alternatively run `dbt` and `fal` consecutively\n\n```bash\n$ dbt run\n# Your dbt models are run\n\n$ fal run\n# Your python scripts are run\n```\n\n# Examples\n\nTo explore what is possible with fal, take a look at the in-depth examples below. We will be adding more examples here over time:\n\n- [Example 1: Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example/README.md)\n- [Example 2: Use dbt from a Jupyter Notebook](https://github.com/fal-ai/fal/blob/-/examples/write_jupyter_notebook/README.md)\n- [Example 3: Read and parse dbt metadata](https://github.com/fal-ai/fal/blob/-/examples/read_dbt_metadata/README.md)\n- [Example 4: Metric forecasting](https://github.com/fal-ai/fal/blob/-/examples/metric-forecast/README.md)\n- [Example 5: Sentiment analysis on support tickets](https://github.com/fal-ai/fal/blob/-/examples/sentiment-analysis/README.md)\n- [Example 6: Anomaly Detection](https://github.com/fal-ai/fal/blob/-/examples/anomaly-detection/README.md)\n- [Example 7: Incorporate fal in CI/CD workflow](https://github.com/fal-ai/fal/blob/-/examples/ci_example/README.md)\n- [Example 8: Send events to Datadog](https://github.com/fal-ai/fal/blob/-/examples/datadog_event/README.md)\n- [Example 9: Write dbt artifacts to GCS](https://github.com/fal-ai/fal/blob/-/examples/write_to_gcs/README.md)\n- [Example 10: Write dbt artifacts to AWS S3](https://github.com/fal-ai/fal/blob/-/examples/write_to_aws/README.md)\n\n[Check out the examples directory for more](https://github.com/fal-ai/fal/blob/-/examples/README.md)\n\n# How it works?\n\n`fal` is a command line tool that can read the state of your `dbt` project and help you run Python scripts after your `dbt run`s by leveraging the [`meta` config](https://docs.getdbt.com/reference/resource-configs/meta).\n\n```yaml\nmodels:\n  - name: historical_ozone_levels\n    ...\n    meta:\n      fal:\n        post-hook:\n          # scripts will run concurrently\n          - send_slack_message.py\n          - another_python_script.py\n```\n\n`fal` also provides useful helpers within the Python context to seamlessly interact with dbt models: `ref("my_dbt_model_name")` will pull a dbt model into your Python script as a [`pandas.DataFrame`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).\n\n## Running scripts before dbt runs\n\nRun scripts before the model runs by using the `pre-hook:` configuration option.\n\nGiven the following schema.yml:\n\n```\nmodels:\n  - name: boston\n    description: Ozone levels\n    config:\n      materialized: table\n    meta:\n      owner: "@meder"\n      fal:\n        pre-hook:\n          - fal_scripts/trigger_fivetran.py\n        post-hook:\n          - fal_scripts/slack.py\n```\n\n`fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.\nIf a model is selected with a selection flag (e.g. `--select boston`), the hooks associated to the model will always run with it.\n\n```bash\n$ fal flow run --select boston\n```\n\n# Concepts\n\n## profile.yml and Credentials\n\n`fal` integrates with `dbt`\'s `profile.yml` file to access and read data from the data warehouse. Once you setup credentials in your `profile.yml` file for your existing `dbt` workflows anytime you use `ref` or `source` to create a dataframe `fal` authenticates using the credentials specified in the `profile.yml` file.\n\n## `meta` Syntax\n\n```yaml\nmodels:\n  - name: historical_ozone_levels\n    ...\n    meta:\n      owner: "@me"\n      fal:\n        post-hook:\n          - send_slack_message.py\n          - another_python_script.py\n```\n\nUse the `fal` and `post-hook` keys underneath the `meta` config to let `fal` CLI know where to look for the Python scripts. You can pass a list of scripts as shown above to run one or more scripts as a post-hook operation after a `dbt run`.\n\n## Variables and functions\n\nInside a Python script, you get access to some useful variables and functions\n\n### Variables\n\nA `context` object with information relevant to the model through which the script was run. For the [`meta` Syntax](#meta-syntax) example, we would get the following:\n\n```python\ncontext.current_model.name\n#= historical_ozone_levels\n\ncontext.current_model.meta\n#= {\'owner\': \'@me\'}\n\ncontext.current_model.meta.get("owner")\n#= \'@me\'\n\ncontext.current_model.status\n# Could be one of\n#= \'success\'\n#= \'error\'\n#= \'skipped\'\n```\n\n`context` object also has access to test information related to the current model. If the previous dbt command was either `test` or `build`, the `context.current_model.test` property is populated with a list of tests:\n\n```python\ncontext.current_model.tests\n#= [CurrentTest(name=\'not_null\', modelname=\'historical_ozone_levels, column=\'ds\', status=\'Pass\')]\n```\n\n### `ref` and `source` functions\n\nThere are also available some familiar functions from `dbt`\n\n```python\n# Refer to dbt models or sources by name and returns it as `pandas.DataFrame`\nref(\'model_name\')\nsource(\'source_name\', \'table_name\')\n\n# You can use it to get the running model data\nref(context.current_model.name)\n```\n\n### `write_to_model` function\n\n> ❗️ We recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter for writing data back to your data-warehouse.\n\nIt is also possible to send data back to your data-warehouse. This makes it easy to get the data, process it and upload it back into dbt territory.\n\nThis function is available in fal Python models only, that is a Python script inside a `fal_models` directory and add a `fal-models-paths` to your `dbt_project.yml`\n\n```yaml\nname: "jaffle_shop"\n# ...\nmodel-paths: ["models"]\n# ...\n\nvars:\n  # Add this to your dbt_project.yml\n  fal-models-paths: ["fal_models"]\n```\n\nOnce added, it will automatically be run by fal without having to add any extra configurations in the `schema.yml`.\n\n```python\nsource_df = source(\'source_name\', \'table_name\')\nref_df = ref(\'a_model\')\n\n# Your code here\ndf = ...\n\n# Upload a `pandas.DataFrame` back to the datawarehouse\nwrite_to_model(df)\n```\n\n`write_to_model` also accepts an optional `dtype` argument, which lets you specify datatypes of columns. It works the same way as `dtype` argument for [`DataFrame.to_sql` function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_sql.html).\n\n```python\nfrom sqlalchemy.types import Integer\n# Upload but specifically create the `value` column with type `integer`\n# Can be useful if data has `None` values\nwrite_to_model(df, dtype={\'value\': Integer()})\n```\n\n## Importing `fal` as a Python package\n\nYou may be interested in accessing dbt models and sources easily from a Jupyter Notebook or another Python script.\nFor that, just import the `fal` package and intantiate a FalDbt project:\n\n```py\nfrom fal import FalDbt\nfaldbt = FalDbt(profiles_dir="~/.dbt", project_dir="../my_project")\n\nfaldbt.list_sources()\n# [\n#    DbtSource(name=\'results\' ...),\n#    DbtSource(name=\'ticket_data_sentiment_analysis\' ...)\n#    ...\n# ]\n\nfaldbt.list_models()\n# [\n#    DbtModel(name=\'zendesk_ticket_data\' ...),\n#    DbtModel(name=\'agent_wait_time\' ...)\n#    ...\n# ]\n\n\nsentiments = faldbt.source(\'results\', \'ticket_data_sentiment_analysis\')\n# pandas.DataFrame\ntickets = faldbt.ref(\'stg_zendesk_ticket_data\')\n# pandas.DataFrame\n```\n\n# Supported `dbt` versions\n\nThe latest `fal` version currently supports dbt `1.4.*`.\n\nIf you need another version, [open an issue](https://github.com/fal-ai/fal/issues/new) and we will take a look!\n\n# Contributing / Development\n\nWe use Poetry for dependency management and easy development testing.\n\nUse Poetry shell to trying your changes right away:\n\n```sh\n~ $ cd fal\n\n~/fal $ poetry install\n\n~/fal $ poetry shell\nSpawning shell within [...]/fal-eFX98vrn-py3.8\n\n~/fal fal-eFX98vrn-py3.8 $ cd ../dbt_project\n\n~/dbt_project fal-eFX98vrn-py3.8 $ fal flow run\n19:27:30  Found 5 models, 0 tests, 0 snapshots, 0 analyses, 165 macros, 0 operations, 0 seed files, 1 source, 0 exposures, 0 metrics\n19:27:30 | Starting fal run for following models and scripts:\n[...]\n```\n\n## Running tests\n\nTests rely on a Postgres database to be present, this can be achieved with docker-compose:\n\n```sh\n~/fal $ docker-compose -f tests/docker-compose.yml up -d\nCreating network "tests_default" with the default driver\nCreating fal_db ... done\n\n# Necessary for the import test\n~/fal $ dbt run --profiles-dir tests/mock/mockProfile --project-dir tests/mock\nRunning with dbt=1.0.1\n[...]\nCompleted successfully\nDone. PASS=5 WARN=0 ERROR=0 SKIP=0 TOTAL=5\n\n~/fal $ pytest -s\n```\n\n# Why are we building this?\n\nWe think `dbt` is great because it empowers data people to get more done with the tools that they are already familiar with.\n\n`dbt`\'s SQL only design is powerful, but if you ever want to get out of SQL-land and connect to external services or get into Python-land for any reason, you will have a hard time. We built `fal` to enable Python workloads (sending alerts to Slack, building predictive models, pushing data to non-data-warehouse destinations and more) **right within `dbt`**.\n\nThis library will form the basis of our attempt to more comprehensively enable **data science workloads** downstream of `dbt`. And because having reliable data pipelines is the most important ingredient in building predictive analytics, we are building a library that integrates well with dbt.\n\n# Have feedback or need help?\n\n- Join us in [fal on Discord](https://discord.com/invite/Fyc9PwrccF)\n- Join the [dbt Community](http://community.getdbt.com/) and go into our [#tools-fal channel](https://getdbt.slack.com/archives/C02V8QW3Q4Q)\n',
-    'author': 'Features & Labels',
-    'author_email': 'hello@fal.ai',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/fal-ai/fal/blob/-/projects/fal',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<3.11',
-}
+# fal: do more with dbt
 
+fal is the easiest way to run Python with your [dbt](https://www.getdbt.com/) project.
+
+# Introduction
+
+With the `fal` CLI, you can:
+
+- [Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example) upon dbt model success or failure.
+- [Load data from external data sources](https://blog.fal.ai/populate-dbt-models-with-csv-data/) before a model starts running.
+- [Download dbt models](https://docs.fal.ai/fal/python-package) into a Python context with a familiar syntax: `ref('my_dbt_model')` using `FalDbt`
+- [Programatically access rich metadata](https://docs.fal.ai/fal/reference/variables-and-functions) about your dbt project.
+
+Head to our [documentation site](https://docs.fal.ai/) for a deeper dive or play with [in-depth examples](https://github.com/fal-ai/fal/blob/-/examples/README.md) to see how fal can help you get more done with dbt.
+
+> ❗️ If you would like to write data back to your data-warehouse, we recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter.
+
+# Getting Started
+
+## 1. Install `fal`
+
+```bash
+$ pip install fal
+```
+
+## 2. Go to your dbt project directory
+
+```bash
+$ cd ~/src/my_dbt_project
+```
+
+## 3. Create a Python script: `send_slack_message.py`
+
+```python
+import os
+from slack_sdk import WebClient
+from slack_sdk.errors import SlackApiError
+
+CHANNEL_ID = os.getenv("SLACK_BOT_CHANNEL")
+SLACK_TOKEN = os.getenv("SLACK_BOT_TOKEN")
+
+client = WebClient(token=SLACK_TOKEN)
+message_text = f"Model: {context.current_model.name}. Status: {context.current_model.status}."
+
+try:
+    response = client.chat_postMessage(
+        channel=CHANNEL_ID,
+        text=message_text
+    )
+except SlackApiError as e:
+    assert e.response["error"]
+```
+
+## 4. Add a `meta` section in your `schema.yml`
+
+```yaml
+models:
+  - name: historical_ozone_levels
+    description: Ozone levels
+    config:
+      materialized: table
+    columns:
+      - name: ozone_level
+        description: Ozone level
+      - name: ds
+        description: Date
+    meta:
+      fal:
+        scripts:
+          - send_slack_message.py
+```
+
+## 5. Run `fal flow run`
+
+```bash
+$ fal flow run
+# both your dbt models and fal scripts are run
+```
+
+## 6. Alternatively run `dbt` and `fal` consecutively
+
+```bash
+$ dbt run
+# Your dbt models are run
+
+$ fal run
+# Your python scripts are run
+```
+
+# Examples
+
+To explore what is possible with fal, take a look at the in-depth examples below. We will be adding more examples here over time:
+
+- [Example 1: Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example/README.md)
+- [Example 2: Use dbt from a Jupyter Notebook](https://github.com/fal-ai/fal/blob/-/examples/write_jupyter_notebook/README.md)
+- [Example 3: Read and parse dbt metadata](https://github.com/fal-ai/fal/blob/-/examples/read_dbt_metadata/README.md)
+- [Example 4: Metric forecasting](https://github.com/fal-ai/fal/blob/-/examples/metric-forecast/README.md)
+- [Example 5: Sentiment analysis on support tickets](https://github.com/fal-ai/fal/blob/-/examples/sentiment-analysis/README.md)
+- [Example 6: Anomaly Detection](https://github.com/fal-ai/fal/blob/-/examples/anomaly-detection/README.md)
+- [Example 7: Incorporate fal in CI/CD workflow](https://github.com/fal-ai/fal/blob/-/examples/ci_example/README.md)
+- [Example 8: Send events to Datadog](https://github.com/fal-ai/fal/blob/-/examples/datadog_event/README.md)
+- [Example 9: Write dbt artifacts to GCS](https://github.com/fal-ai/fal/blob/-/examples/write_to_gcs/README.md)
+- [Example 10: Write dbt artifacts to AWS S3](https://github.com/fal-ai/fal/blob/-/examples/write_to_aws/README.md)
+
+[Check out the examples directory for more](https://github.com/fal-ai/fal/blob/-/examples/README.md)
+
+# How it works?
+
+`fal` is a command line tool that can read the state of your `dbt` project and help you run Python scripts after your `dbt run`s by leveraging the [`meta` config](https://docs.getdbt.com/reference/resource-configs/meta).
+
+```yaml
+models:
+  - name: historical_ozone_levels
+    ...
+    meta:
+      fal:
+        post-hook:
+          # scripts will run concurrently
+          - send_slack_message.py
+          - another_python_script.py
+```
+
+`fal` also provides useful helpers within the Python context to seamlessly interact with dbt models: `ref("my_dbt_model_name")` will pull a dbt model into your Python script as a [`pandas.DataFrame`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
+
+## Running scripts before dbt runs
+
+Run scripts before the model runs by using the `pre-hook:` configuration option.
+
+Given the following schema.yml:
+
+```
+models:
+  - name: boston
+    description: Ozone levels
+    config:
+      materialized: table
+    meta:
+      owner: "@meder"
+      fal:
+        pre-hook:
+          - fal_scripts/trigger_fivetran.py
+        post-hook:
+          - fal_scripts/slack.py
+```
+
+`fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.
+If a model is selected with a selection flag (e.g. `--select boston`), the hooks associated to the model will always run with it.
+
+```bash
+$ fal flow run --select boston
+```
+
+# Concepts
+
+## profile.yml and Credentials
+
+`fal` integrates with `dbt`'s `profile.yml` file to access and read data from the data warehouse. Once you setup credentials in your `profile.yml` file for your existing `dbt` workflows anytime you use `ref` or `source` to create a dataframe `fal` authenticates using the credentials specified in the `profile.yml` file.
+
+## `meta` Syntax
+
+```yaml
+models:
+  - name: historical_ozone_levels
+    ...
+    meta:
+      owner: "@me"
+      fal:
+        post-hook:
+          - send_slack_message.py
+          - another_python_script.py
+```
+
+Use the `fal` and `post-hook` keys underneath the `meta` config to let `fal` CLI know where to look for the Python scripts. You can pass a list of scripts as shown above to run one or more scripts as a post-hook operation after a `dbt run`.
+
+## Variables and functions
+
+Inside a Python script, you get access to some useful variables and functions
+
+### Variables
+
+A `context` object with information relevant to the model through which the script was run. For the [`meta` Syntax](#meta-syntax) example, we would get the following:
+
+```python
+context.current_model.name
+#= historical_ozone_levels
+
+context.current_model.meta
+#= {'owner': '@me'}
+
+context.current_model.meta.get("owner")
+#= '@me'
+
+context.current_model.status
+# Could be one of
+#= 'success'
+#= 'error'
+#= 'skipped'
+```
+
+`context` object also has access to test information related to the current model. If the previous dbt command was either `test` or `build`, the `context.current_model.test` property is populated with a list of tests:
+
+```python
+context.current_model.tests
+#= [CurrentTest(name='not_null', modelname='historical_ozone_levels, column='ds', status='Pass')]
+```
+
+### `ref` and `source` functions
+
+There are also available some familiar functions from `dbt`
+
+```python
+# Refer to dbt models or sources by name and returns it as `pandas.DataFrame`
+ref('model_name')
+source('source_name', 'table_name')
+
+# You can use it to get the running model data
+ref(context.current_model.name)
+```
+
+### `write_to_model` function
+
+> ❗️ We recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter for writing data back to your data-warehouse.
+
+It is also possible to send data back to your data-warehouse. This makes it easy to get the data, process it and upload it back into dbt territory.
+
+This function is available in fal Python models only, that is a Python script inside a `fal_models` directory and add a `fal-models-paths` to your `dbt_project.yml`
+
+```yaml
+name: "jaffle_shop"
+# ...
+model-paths: ["models"]
+# ...
+
+vars:
+  # Add this to your dbt_project.yml
+  fal-models-paths: ["fal_models"]
+```
+
+Once added, it will automatically be run by fal without having to add any extra configurations in the `schema.yml`.
+
+```python
+source_df = source('source_name', 'table_name')
+ref_df = ref('a_model')
+
+# Your code here
+df = ...
+
+# Upload a `pandas.DataFrame` back to the datawarehouse
+write_to_model(df)
+```
+
+`write_to_model` also accepts an optional `dtype` argument, which lets you specify datatypes of columns. It works the same way as `dtype` argument for [`DataFrame.to_sql` function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_sql.html).
+
+```python
+from sqlalchemy.types import Integer
+# Upload but specifically create the `value` column with type `integer`
+# Can be useful if data has `None` values
+write_to_model(df, dtype={'value': Integer()})
+```
+
+## Importing `fal` as a Python package
+
+You may be interested in accessing dbt models and sources easily from a Jupyter Notebook or another Python script.
+For that, just import the `fal` package and intantiate a FalDbt project:
+
+```py
+from fal import FalDbt
+faldbt = FalDbt(profiles_dir="~/.dbt", project_dir="../my_project")
+
+faldbt.list_sources()
+# [
+#    DbtSource(name='results' ...),
+#    DbtSource(name='ticket_data_sentiment_analysis' ...)
+#    ...
+# ]
+
+faldbt.list_models()
+# [
+#    DbtModel(name='zendesk_ticket_data' ...),
+#    DbtModel(name='agent_wait_time' ...)
+#    ...
+# ]
+
+
+sentiments = faldbt.source('results', 'ticket_data_sentiment_analysis')
+# pandas.DataFrame
+tickets = faldbt.ref('stg_zendesk_ticket_data')
+# pandas.DataFrame
+```
+
+# Supported `dbt` versions
+
+The latest `fal` version currently supports dbt `1.4.*`.
+
+If you need another version, [open an issue](https://github.com/fal-ai/fal/issues/new) and we will take a look!
+
+# Contributing / Development
+
+We use Poetry for dependency management and easy development testing.
+
+Use Poetry shell to trying your changes right away:
+
+```sh
+~ $ cd fal
+
+~/fal $ poetry install
+
+~/fal $ poetry shell
+Spawning shell within [...]/fal-eFX98vrn-py3.8
+
+~/fal fal-eFX98vrn-py3.8 $ cd ../dbt_project
+
+~/dbt_project fal-eFX98vrn-py3.8 $ fal flow run
+19:27:30  Found 5 models, 0 tests, 0 snapshots, 0 analyses, 165 macros, 0 operations, 0 seed files, 1 source, 0 exposures, 0 metrics
+19:27:30 | Starting fal run for following models and scripts:
+[...]
+```
+
+## Running tests
+
+Tests rely on a Postgres database to be present, this can be achieved with docker-compose:
+
+```sh
+~/fal $ docker-compose -f tests/docker-compose.yml up -d
+Creating network "tests_default" with the default driver
+Creating fal_db ... done
+
+# Necessary for the import test
+~/fal $ dbt run --profiles-dir tests/mock/mockProfile --project-dir tests/mock
+Running with dbt=1.0.1
+[...]
+Completed successfully
+Done. PASS=5 WARN=0 ERROR=0 SKIP=0 TOTAL=5
+
+~/fal $ pytest -s
+```
+
+# Why are we building this?
+
+We think `dbt` is great because it empowers data people to get more done with the tools that they are already familiar with.
+
+`dbt`'s SQL only design is powerful, but if you ever want to get out of SQL-land and connect to external services or get into Python-land for any reason, you will have a hard time. We built `fal` to enable Python workloads (sending alerts to Slack, building predictive models, pushing data to non-data-warehouse destinations and more) **right within `dbt`**.
+
+This library will form the basis of our attempt to more comprehensively enable **data science workloads** downstream of `dbt`. And because having reliable data pipelines is the most important ingredient in building predictive analytics, we are building a library that integrates well with dbt.
+
+# Have feedback or need help?
+
+- Join us in [fal on Discord](https://discord.com/invite/Fyc9PwrccF)
+- Join the [dbt Community](http://community.getdbt.com/) and go into our [#tools-fal channel](https://getdbt.slack.com/archives/C02V8QW3Q4Q)
 
-setup(**setup_kwargs)
```

