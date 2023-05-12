# Comparing `tmp/pybatfish-2022.9.7.77-py2.py3-none-any.whl.zip` & `tmp/pybatfish-2023.5.12.784-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,64 +1,42 @@
-Zip file size: 135515 bytes, number of entries: 62
--rw-r--r--  2.0 unx      962 b- defN 22-Sep-07 15:03 pybatfish/__init__.py
--rw-r--r--  2.0 unx     1297 b- defN 22-Sep-07 15:03 pybatfish/exception.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-07 15:03 pybatfish/py.typed
--rw-r--r--  2.0 unx     7411 b- defN 22-Sep-07 15:03 pybatfish/util.py
--rw-r--r--  2.0 unx      615 b- defN 22-Sep-07 15:03 pybatfish/client/__init__.py
--rw-r--r--  2.0 unx    11725 b- defN 22-Sep-07 15:03 pybatfish/client/_diagnostics.py
--rw-r--r--  2.0 unx    15608 b- defN 22-Sep-07 15:03 pybatfish/client/_facts.py
--rw-r--r--  2.0 unx    26831 b- defN 22-Sep-07 15:03 pybatfish/client/asserts.py
--rw-r--r--  2.0 unx     8235 b- defN 22-Sep-07 15:03 pybatfish/client/capirca.py
--rw-r--r--  2.0 unx    19048 b- defN 22-Sep-07 15:03 pybatfish/client/commands.py
--rw-r--r--  2.0 unx    10789 b- defN 22-Sep-07 15:03 pybatfish/client/consts.py
--rw-r--r--  2.0 unx     3820 b- defN 22-Sep-07 15:03 pybatfish/client/extended.py
--rw-r--r--  2.0 unx     2376 b- defN 22-Sep-07 15:03 pybatfish/client/internal.py
--rw-r--r--  2.0 unx     2386 b- defN 22-Sep-07 15:03 pybatfish/client/options.py
--rw-r--r--  2.0 unx     4591 b- defN 22-Sep-07 15:03 pybatfish/client/resthelper.py
--rw-r--r--  2.0 unx    27994 b- defN 22-Sep-07 15:03 pybatfish/client/restv2helper.py
--rw-r--r--  2.0 unx    57342 b- defN 22-Sep-07 15:03 pybatfish/client/session.py
--rw-r--r--  2.0 unx    15098 b- defN 22-Sep-07 15:03 pybatfish/client/workhelper.py
--rw-r--r--  2.0 unx     1703 b- defN 22-Sep-07 15:03 pybatfish/client/workitem.py
--rw-r--r--  2.0 unx      829 b- defN 22-Sep-07 15:03 pybatfish/datamodel/__init__.py
--rw-r--r--  2.0 unx     6682 b- defN 22-Sep-07 15:03 pybatfish/datamodel/acl.py
--rw-r--r--  2.0 unx    57572 b- defN 22-Sep-07 15:03 pybatfish/datamodel/flow.py
--rw-r--r--  2.0 unx    12680 b- defN 22-Sep-07 15:03 pybatfish/datamodel/primitives.py
--rw-r--r--  2.0 unx    10651 b- defN 22-Sep-07 15:03 pybatfish/datamodel/referencelibrary.py
--rw-r--r--  2.0 unx    14571 b- defN 22-Sep-07 15:03 pybatfish/datamodel/route.py
--rw-r--r--  2.0 unx      776 b- defN 22-Sep-07 15:03 pybatfish/datamodel/answer/__init__.py
--rw-r--r--  2.0 unx     4498 b- defN 22-Sep-07 15:03 pybatfish/datamodel/answer/base.py
--rw-r--r--  2.0 unx     5190 b- defN 22-Sep-07 15:03 pybatfish/datamodel/answer/table.py
--rw-r--r--  2.0 unx      797 b- defN 22-Sep-07 15:03 pybatfish/question/__init__.py
--rw-r--r--  2.0 unx      798 b- defN 22-Sep-07 15:03 pybatfish/question/bfq.py
--rw-r--r--  2.0 unx    43964 b- defN 22-Sep-07 15:03 pybatfish/question/question.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-07 15:03 pybatfish/question/questionutil.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-07 15:03 pybatfish/settings/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 22-Sep-07 15:03 pybatfish/settings/issues.py
--rw-r--r--  2.0 unx      615 b- defN 22-Sep-07 15:03 tests/datamodel/__init__.py
--rw-r--r--  2.0 unx     5690 b- defN 22-Sep-07 15:03 tests/datamodel/test_acltrace.py
--rw-r--r--  2.0 unx     1795 b- defN 22-Sep-07 15:03 tests/datamodel/test_auto_complete_suggestion.py
--rw-r--r--  2.0 unx     1608 b- defN 22-Sep-07 15:03 tests/datamodel/test_datamodel_element.py
--rw-r--r--  2.0 unx     1389 b- defN 22-Sep-07 15:03 tests/datamodel/test_filelines.py
--rw-r--r--  2.0 unx    39235 b- defN 22-Sep-07 15:03 tests/datamodel/test_flow.py
--rw-r--r--  2.0 unx     2678 b- defN 22-Sep-07 15:03 tests/datamodel/test_flowtracehop.py
--rw-r--r--  2.0 unx     1414 b- defN 22-Sep-07 15:03 tests/datamodel/test_interface.py
--rw-r--r--  2.0 unx     2071 b- defN 22-Sep-07 15:03 tests/datamodel/test_issue.py
--rw-r--r--  2.0 unx     1016 b- defN 22-Sep-07 15:03 tests/datamodel/test_primitives.py
--rw-r--r--  2.0 unx    16178 b- defN 22-Sep-07 15:03 tests/datamodel/test_referencelibrary.py
--rw-r--r--  2.0 unx     8668 b- defN 22-Sep-07 15:03 tests/datamodel/test_route.py
--rw-r--r--  2.0 unx     1917 b- defN 22-Sep-07 15:03 tests/datamodel/test_session.py
--rw-r--r--  2.0 unx     2830 b- defN 22-Sep-07 15:03 tests/datamodel/test_traceelement.py
--rw-r--r--  2.0 unx     1402 b- defN 22-Sep-07 15:03 tests/datamodel/test_traceevent.py
--rw-r--r--  2.0 unx      615 b- defN 22-Sep-07 15:03 tests/datamodel/answer/__init__.py
--rw-r--r--  2.0 unx     1501 b- defN 22-Sep-07 15:03 tests/datamodel/answer/test_answer.py
--rw-r--r--  2.0 unx     3074 b- defN 22-Sep-07 15:03 tests/datamodel/answer/test_base.py
--rw-r--r--  2.0 unx     1879 b- defN 22-Sep-07 15:03 tests/datamodel/answer/test_columnmetadata.py
--rw-r--r--  2.0 unx     5384 b- defN 22-Sep-07 15:03 tests/datamodel/answer/test_tableanswerelement.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-07 15:03 tests/settings/__init__.py
--rw-r--r--  2.0 unx     1357 b- defN 22-Sep-07 15:03 tests/settings/test_issues.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Sep-07 15:03 pybatfish-2022.9.7.77.dist-info/LICENSE
--rw-r--r--  2.0 unx     6457 b- defN 22-Sep-07 15:03 pybatfish-2022.9.7.77.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Sep-07 15:03 pybatfish-2022.9.7.77.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 22-Sep-07 15:03 pybatfish-2022.9.7.77.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 22-Sep-07 15:03 pybatfish-2022.9.7.77.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5454 b- defN 22-Sep-07 15:03 pybatfish-2022.9.7.77.dist-info/RECORD
-62 files, 504413 bytes uncompressed, 126815 bytes compressed:  74.9%
+Zip file size: 107409 bytes, number of entries: 40
+-rw-r--r--  2.0 unx      963 b- defN 23-May-12 09:05 pybatfish/__init__.py
+-rw-r--r--  2.0 unx     1297 b- defN 23-May-12 09:05 pybatfish/exception.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 09:05 pybatfish/py.typed
+-rw-r--r--  2.0 unx     7411 b- defN 23-May-12 09:05 pybatfish/util.py
+-rw-r--r--  2.0 unx      615 b- defN 23-May-12 09:05 pybatfish/client/__init__.py
+-rw-r--r--  2.0 unx    11723 b- defN 23-May-12 09:05 pybatfish/client/_diagnostics.py
+-rw-r--r--  2.0 unx    15608 b- defN 23-May-12 09:05 pybatfish/client/_facts.py
+-rw-r--r--  2.0 unx    31138 b- defN 23-May-12 09:05 pybatfish/client/asserts.py
+-rw-r--r--  2.0 unx     8235 b- defN 23-May-12 09:05 pybatfish/client/capirca.py
+-rw-r--r--  2.0 unx    19048 b- defN 23-May-12 09:05 pybatfish/client/commands.py
+-rw-r--r--  2.0 unx    10789 b- defN 23-May-12 09:05 pybatfish/client/consts.py
+-rw-r--r--  2.0 unx     3820 b- defN 23-May-12 09:05 pybatfish/client/extended.py
+-rw-r--r--  2.0 unx     2376 b- defN 23-May-12 09:05 pybatfish/client/internal.py
+-rw-r--r--  2.0 unx     2386 b- defN 23-May-12 09:05 pybatfish/client/options.py
+-rw-r--r--  2.0 unx     4589 b- defN 23-May-12 09:05 pybatfish/client/resthelper.py
+-rw-r--r--  2.0 unx    27990 b- defN 23-May-12 09:05 pybatfish/client/restv2helper.py
+-rw-r--r--  2.0 unx    57596 b- defN 23-May-12 09:05 pybatfish/client/session.py
+-rw-r--r--  2.0 unx    15098 b- defN 23-May-12 09:05 pybatfish/client/workhelper.py
+-rw-r--r--  2.0 unx     1703 b- defN 23-May-12 09:05 pybatfish/client/workitem.py
+-rw-r--r--  2.0 unx      829 b- defN 23-May-12 09:05 pybatfish/datamodel/__init__.py
+-rw-r--r--  2.0 unx     6682 b- defN 23-May-12 09:05 pybatfish/datamodel/acl.py
+-rw-r--r--  2.0 unx    57572 b- defN 23-May-12 09:05 pybatfish/datamodel/flow.py
+-rw-r--r--  2.0 unx    12680 b- defN 23-May-12 09:05 pybatfish/datamodel/primitives.py
+-rw-r--r--  2.0 unx    10651 b- defN 23-May-12 09:05 pybatfish/datamodel/referencelibrary.py
+-rw-r--r--  2.0 unx    14571 b- defN 23-May-12 09:05 pybatfish/datamodel/route.py
+-rw-r--r--  2.0 unx      776 b- defN 23-May-12 09:05 pybatfish/datamodel/answer/__init__.py
+-rw-r--r--  2.0 unx     4498 b- defN 23-May-12 09:05 pybatfish/datamodel/answer/base.py
+-rw-r--r--  2.0 unx     5190 b- defN 23-May-12 09:05 pybatfish/datamodel/answer/table.py
+-rw-r--r--  2.0 unx      797 b- defN 23-May-12 09:05 pybatfish/question/__init__.py
+-rw-r--r--  2.0 unx      798 b- defN 23-May-12 09:05 pybatfish/question/bfq.py
+-rw-r--r--  2.0 unx    43964 b- defN 23-May-12 09:05 pybatfish/question/question.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 09:05 pybatfish/question/questionutil.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 09:05 pybatfish/settings/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-May-12 09:05 pybatfish/settings/issues.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-12 09:05 pybatfish-2023.5.12.784.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6461 b- defN 23-May-12 09:05 pybatfish-2023.5.12.784.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 09:05 pybatfish-2023.5.12.784.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-May-12 09:05 pybatfish-2023.5.12.784.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-12 09:05 pybatfish-2023.5.12.784.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3448 b- defN 23-May-12 09:05 pybatfish-2023.5.12.784.dist-info/RECORD
+40 files, 404624 bytes uncompressed, 101889 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -96,92 +96,26 @@
 
 Filename: pybatfish/settings/__init__.py
 Comment: 
 
 Filename: pybatfish/settings/issues.py
 Comment: 
 
-Filename: tests/datamodel/__init__.py
+Filename: pybatfish-2023.5.12.784.dist-info/LICENSE
 Comment: 
 
-Filename: tests/datamodel/test_acltrace.py
+Filename: pybatfish-2023.5.12.784.dist-info/METADATA
 Comment: 
 
-Filename: tests/datamodel/test_auto_complete_suggestion.py
+Filename: pybatfish-2023.5.12.784.dist-info/WHEEL
 Comment: 
 
-Filename: tests/datamodel/test_datamodel_element.py
+Filename: pybatfish-2023.5.12.784.dist-info/entry_points.txt
 Comment: 
 
-Filename: tests/datamodel/test_filelines.py
+Filename: pybatfish-2023.5.12.784.dist-info/top_level.txt
 Comment: 
 
-Filename: tests/datamodel/test_flow.py
-Comment: 
-
-Filename: tests/datamodel/test_flowtracehop.py
-Comment: 
-
-Filename: tests/datamodel/test_interface.py
-Comment: 
-
-Filename: tests/datamodel/test_issue.py
-Comment: 
-
-Filename: tests/datamodel/test_primitives.py
-Comment: 
-
-Filename: tests/datamodel/test_referencelibrary.py
-Comment: 
-
-Filename: tests/datamodel/test_route.py
-Comment: 
-
-Filename: tests/datamodel/test_session.py
-Comment: 
-
-Filename: tests/datamodel/test_traceelement.py
-Comment: 
-
-Filename: tests/datamodel/test_traceevent.py
-Comment: 
-
-Filename: tests/datamodel/answer/__init__.py
-Comment: 
-
-Filename: tests/datamodel/answer/test_answer.py
-Comment: 
-
-Filename: tests/datamodel/answer/test_base.py
-Comment: 
-
-Filename: tests/datamodel/answer/test_columnmetadata.py
-Comment: 
-
-Filename: tests/datamodel/answer/test_tableanswerelement.py
-Comment: 
-
-Filename: tests/settings/__init__.py
-Comment: 
-
-Filename: tests/settings/test_issues.py
-Comment: 
-
-Filename: pybatfish-2022.9.7.77.dist-info/LICENSE
-Comment: 
-
-Filename: pybatfish-2022.9.7.77.dist-info/METADATA
-Comment: 
-
-Filename: pybatfish-2022.9.7.77.dist-info/WHEEL
-Comment: 
-
-Filename: pybatfish-2022.9.7.77.dist-info/entry_points.txt
-Comment: 
-
-Filename: pybatfish-2022.9.7.77.dist-info/top_level.txt
-Comment: 
-
-Filename: pybatfish-2022.9.7.77.dist-info/RECORD
+Filename: pybatfish-2023.5.12.784.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybatfish/__init__.py

```diff
@@ -17,8 +17,8 @@
 
 __desc__ = "Python API and utilities for Batfish"
 
 __name__ = "pybatfish"
 
 __url__ = "https://github.com/batfish/pybatfish"
 
-__version__ = "2022.09.07.77"
+__version__ = "2023.05.12.784"
```

## pybatfish/client/_diagnostics.py

```diff
@@ -69,15 +69,15 @@
 _requests_session = requests.Session()
 _adapter = HTTPAdapter(
     max_retries=Retry(
         total=_UPLOAD_MAX_TRIES,
         backoff_factor=_UPLOAD_RETRY_BACKOFF,
         status_forcelist=[500, 502, 503, 504, 104],
         # Retry on all calls, including POST
-        method_whitelist=False,
+        allowed_methods=None,
     )
 )
 _requests_session.mount("https://", _adapter)
 
 
 def upload_diagnostics(
     session: "Session",
```

## pybatfish/client/asserts.py

```diff
@@ -110,42 +110,56 @@
 
 def _subdict(d, keys):
     # type: (Dict, Iterable[str]) -> Dict[str, Any]
     """Helper function that retrieves a subset of a dictionary given some keys."""
     return {k: d.get(k) for k in keys}
 
 
-def _get_duplicate_router_ids(question_name, session=None, snapshot=None):
-    # type: (str, Optional[Session], Optional[str]) -> DataFrame
+def _get_duplicate_router_ids(
+    question_name: str,
+    session: Optional["Session"] = None,
+    snapshot: Optional[str] = None,
+    ignore_same_node: bool = False,
+) -> DataFrame:
     """Helper function to get rows with duplicate router IDs for a given protocol.
 
     :param question_name: The question name to be used to fetch the protocol process configuration
     :param session: Batfish session to use for asking the question
     :param snapshot: Snapshot on which to ask the question
+    :param ignore_same_node: whether to ignore duplicate router-ids on the same node
     """
     df = (
         getattr(_get_question_object(session, question_name), question_name)()
         .answer(snapshot)
         .frame()
     )
-    df_duplicate = df[df.duplicated(["Router_ID"], keep=False)].sort_values(
-        ["Router_ID"]
-    )
-
+    if ignore_same_node:
+        # Maps Router_ID to whether multiple nodes have that Router_ID
+        router_id_on_duplicate_nodes = (
+            df.drop_duplicates(["Node", "Router_ID"])
+            .value_counts(["Router_ID"])
+            .map(lambda x: x > 1)
+        )
+        df_duplicate = df[
+            df.apply(lambda x: router_id_on_duplicate_nodes[x["Router_ID"]][0], axis=1)
+        ].sort_values(["Router_ID"])
+    else:
+        df_duplicate = df[df.duplicated(["Router_ID"], keep=False)].sort_values(
+            ["Router_ID"]
+        )
     return df_duplicate
 
 
-def _is_dict_match(actual, expected):
-    # type: (Dict, Dict) -> bool
+def _is_dict_match(actual: Dict[str, Any], expected: Dict[str, Any]) -> bool:
     """Matches two dictionaries. `expected` can be a subset of `actual`."""
     diff = DeepDiff(
         _subdict(actual, expected.keys()),
         expected,
         ignore_order=True,
-        verbose_level=0,
+        verbose_level=1,
         view="text",
     )
     return not diff
 
 
 def _raise_common(err_text, soft=False):
     # type: (str, bool) -> bool
@@ -167,76 +181,182 @@
         return str(df.to_dict(orient="records"))
     else:
         raise ValueError(
             "Unknown df_format {}. Should be 'table' or 'records'".format(df_format)
         )
 
 
-# TODO: converge on representation of routes. (Blocked on backend batfish).
-# TODO: allow this to be role-based. (Again, backend support).
-def assert_has_route(routes, expected_route, node, vrf="default", soft=False):
+def assert_has_route(
+    routes: Union[DataFrame, Dict[str, Dict[str, List[Dict[str, Any]]]]],
+    expected_route: Dict[str, Any],
+    node: str,
+    vrf: str = "default",
+    soft: bool = False,
+) -> bool:
     """Assert that a particular route is present.
 
-    :param routes: All routes returned by the Batfish routes question.
+    :param routes: Routes returned by the Batfish routes or ribs questions, either as a Pandas DataFrame or a multilevel dictionary from hostname to VRF name to list of routes, where each route is a dictionary.
+    :type routes: Union[DataFrame, Dict[str, Dict[str, List[Dict[str, any]]]]]
     :param expected_route: A dictionary describing route to match.
+    :type expected_route: Dict[str, any]
     :param node: node hostname on which to look for a route.
+    :type node: str
     :param vrf: VRF name where the route should be present. Default is `default`.
+    :type node: str
     :param soft: whether this assertion is soft (i.e., generates a warning but
         not a failure)
     :type soft: bool
     """
     __tracebackhide__ = operator.methodcaller("errisinstance", BatfishAssertException)
+
+    if isinstance(routes, DataFrame):
+        return _assert_has_route_dataframe_routes(
+            routes, expected_route, node, vrf, soft
+        )
+    elif isinstance(routes, Dict):
+        return _assert_has_route_dict_routes(routes, expected_route, node, vrf, soft)
+
+    raise TypeError("'routes' is neither a Pandas DataFrame nor a dictionary")
+
+
+def _assert_has_route_dataframe_routes(
+    routes: DataFrame, expected_route: Dict[str, Any], node: str, vrf: str, soft: bool
+) -> bool:
+    node_routes = routes[routes["Node"] == node]
+    if len(node_routes) == 0:
+        raise BatfishAssertException("No node: {}".format(node))
+
+    vrf_routes = node_routes[node_routes["VRF"] == vrf]
+    if len(vrf_routes) == 0:
+        raise BatfishAssertException("No VRF: {} on node {}".format(vrf, node))
+
+    if not any(
+        _is_dict_match(actual_route, expected_route)
+        for actual_route in vrf_routes.to_dict(orient="records")
+    ):
+        err_text = "No route matches for {} on node {}, VRF {}".format(
+            expected_route, node, vrf
+        )
+        return _raise_common(err_text, soft)
+    return True
+
+
+def _assert_has_route_dict_routes(
+    routes: Dict[str, Dict[str, List[Dict[str, Any]]]],
+    expected_route: Dict[str, Any],
+    node: str,
+    vrf: str,
+    soft: bool,
+) -> bool:
     try:
-        d = routes[node]
+        node_routes = routes[node]
     except KeyError:
         raise BatfishAssertException("No node: {}".format(node))
 
     try:
-        d = d[vrf]
+        vrf_routes = node_routes[vrf]
     except KeyError:
         raise BatfishAssertException("No VRF: {} on node {}".format(vrf, node))
 
-    if not any(_is_dict_match(actual_route, expected_route) for actual_route in d):
+    if not any(
+        _is_dict_match(actual_route, expected_route) for actual_route in vrf_routes
+    ):
         err_text = "No route matches for {} on node {}, VRF {}".format(
             expected_route, node, vrf
         )
         return _raise_common(err_text, soft)
     return True
 
 
-def assert_has_no_route(routes, expected_route, node, vrf="default", soft=False):
+def assert_has_no_route(
+    routes: Union[DataFrame, Dict[str, Dict[str, List[Dict[str, Any]]]]],
+    expected_route: Dict[str, Any],
+    node: str,
+    vrf: str = "default",
+    soft: bool = False,
+) -> bool:
     """Assert that a particular route is **NOT** present.
 
     .. note:: If a node or VRF is missing in the route answer the assertion
         will NOT fail, but a warning will be generated.
 
-    :param routes: All routes returned by the Batfish routes question.
+    :param routes: Routes returned by the Batfish routes or ribs questions, either as a Pandas DataFrame or a multilevel dictionary from hostname to VRF name to list of routes, where each route is a dictionary.
+    :type routes: Union[DataFrame, Dict[str, Dict[str, List[Dict[str, any]]]]]
     :param expected_route: A dictionary describing route to match.
-    :param node: node hostname on which to look for expected route.
-    :param vrf: VRF name to check. Default is `default`.
+    :type expected_route: Dict[str, any]
+    :param node: node hostname on which to look for a route.
+    :type node: str
+    :param vrf: VRF name where the route should be present. Default is `default`.
+    :type node: str
     :param soft: whether this assertion is soft (i.e., generates a warning but
         not a failure)
     :type soft: bool
     """
     __tracebackhide__ = operator.methodcaller("errisinstance", BatfishAssertException)
+    if isinstance(routes, DataFrame):
+        return _assert_has_no_route_dataframe_routes(
+            routes, expected_route, node, vrf, soft
+        )
+    elif isinstance(routes, Dict):
+        return _assert_has_no_route_dict_routes(routes, expected_route, node, vrf, soft)
+
+    raise TypeError("'routes' is neither a Pandas DataFrame nor a dictionary")
+
+
+def _assert_has_no_route_dataframe_routes(
+    routes: DataFrame, expected_route: Dict[str, Any], node: str, vrf: str, soft: bool
+) -> bool:
+    node_routes = routes[routes["Node"] == node]
+    if len(node_routes) == 0:
+        warnings.warn("No node: {}".format(node), category=BatfishAssertWarning)
+        return True
+
+    vrf_routes = node_routes[node_routes["VRF"] == vrf]
+    if len(vrf_routes) == 0:
+        warnings.warn(
+            "No VRF: {} on node {}".format(vrf, node), category=BatfishAssertWarning
+        )
+        return True
+
+    all_matches = [
+        route
+        for route in vrf_routes.to_dict(orient="records")
+        if _is_dict_match(route, expected_route)
+    ]
+    if all_matches:
+        err_text = "Found route(s) that match, "
+        "when none were expected:\n{}".format(all_matches)
+        return _raise_common(err_text, soft)
+    return True
+
+
+def _assert_has_no_route_dict_routes(
+    routes: Dict[str, Dict[str, List[Dict[str, Any]]]],
+    expected_route: Dict[str, Any],
+    node: str,
+    vrf: str,
+    soft: bool,
+) -> bool:
     try:
-        d = routes[node]
+        node_routes = routes[node]
     except KeyError:
         warnings.warn("No node: {}".format(node), category=BatfishAssertWarning)
         return True
 
     try:
-        d = d[vrf]
+        vrf_routes = node_routes[vrf]
     except KeyError:
         warnings.warn(
             "No VRF: {} on node {}".format(vrf, node), category=BatfishAssertWarning
         )
         return True
 
-    all_matches = [route for route in d if _is_dict_match(route, expected_route)]
+    all_matches = [
+        route for route in vrf_routes if _is_dict_match(route, expected_route)
+    ]
     if all_matches:
         err_text = "Found route(s) that match, "
         "when none were expected:\n{}".format(all_matches)
         return _raise_common(err_text, soft)
     return True
 
 
@@ -634,31 +754,32 @@
             ),
             soft,
         )
     return True
 
 
 def assert_no_duplicate_router_ids(
-    snapshot=None,
-    nodes=None,
-    protocols=None,
-    soft=False,
-    session=None,
-    df_format="table",
-):
-    # type: (Optional[str], Optional[str], Optional[List[str]], bool, Optional[Session], str) -> bool
+    snapshot: Optional[str] = None,
+    nodes: Optional[str] = None,
+    protocols: Optional[List[str]] = None,
+    soft: bool = False,
+    session: Optional["Session"] = None,
+    df_format: str = "table",
+    ignore_same_node: bool = False,
+) -> bool:
     """Assert that there are no duplicate router IDs present in the snapshot.
 
     :param snapshot: the snapshot on which to check the assertion
     :param protocols: the protocols on which to run the assertion, currently BGP and OSPF are supported
     :param soft: whether this assertion is soft (i.e., generates a warning but
         not a failure)
     :param session: Batfish session to use for the assertion
     :param df_format: How to format the Dataframe content in the output message.
         Valid options are 'table' and 'records' (each row is a key-value pairs).
+    :param ignore_same_node: whether to ignore duplicate router-ids on the same node
     """
     __tracebackhide__ = operator.methodcaller("errisinstance", BatfishAssertException)
 
     kwargs = dict()  # type: Dict
     if nodes is not None:
         kwargs.update(nodes=nodes)
 
@@ -673,15 +794,15 @@
             )
         )
     found_duplicates = False
     duplicate_results = ""
 
     for protocol in protocols_to_fetch:
         df_duplicate = _get_duplicate_router_ids(
-            protocol + "ProcessConfiguration", session, snapshot
+            protocol + "ProcessConfiguration", session, snapshot, ignore_same_node
         )
         if not df_duplicate.empty:
             found_duplicates = True
             duplicate_results += "{}: {}\n".format(
                 protocol.upper(), _format_df(df_duplicate, df_format)
             )
```

## pybatfish/client/resthelper.py

```diff
@@ -41,15 +41,15 @@
 _adapter = HTTPAdapter(
     max_retries=Retry(
         total=Options.max_retries_to_connect_to_coordinator,
         connect=Options.max_retries_to_connect_to_coordinator,
         read=Options.max_retries_to_connect_to_coordinator,
         backoff_factor=Options.request_backoff_factor,
         # Retry on all calls, including POST
-        method_whitelist=False,
+        allowed_methods=None,
         status_forcelist=[429, 500, 502, 503, 504],
     )
 )
 # Configure retries for http and https requests
 _requests_session.mount("http://", _adapter)
 _requests_session.mount("https://", _adapter)
```

## pybatfish/client/restv2helper.py

```diff
@@ -59,15 +59,15 @@
 _adapter = HTTPAdapter(
     max_retries=Retry(
         total=Options.max_retries_to_connect_to_coordinator,
         connect=Options.max_retries_to_connect_to_coordinator,
         read=Options.max_retries_to_connect_to_coordinator,
         backoff_factor=Options.request_backoff_factor,
         # Retry on all calls, including POST
-        method_whitelist=False,
+        allowed_methods=None,
         status_forcelist=_STATUS_FORCELIST,
     )
 )
 # Configure retries for both http and https requests
 _requests_session.mount("http://", _adapter)
 _requests_session.mount("https://", _adapter)
 
@@ -76,15 +76,15 @@
 _adapter_fail_fast = HTTPAdapter(
     max_retries=Retry(
         total=Options.max_initial_tries_to_connect_to_coordinator,
         connect=Options.max_initial_tries_to_connect_to_coordinator,
         read=Options.max_initial_tries_to_connect_to_coordinator,
         backoff_factor=Options.request_backoff_factor,
         # Retry on all calls, including POST
-        method_whitelist=False,
+        allowed_methods=None,
         status_forcelist=_STATUS_FORCELIST,
     )
 )
 # Configure retries for both http and https requests
 _requests_session_fail_fast.mount("http://", _adapter_fail_fast)
 _requests_session_fail_fast.mount("https://", _adapter_fail_fast)
```

## pybatfish/client/session.py

```diff
@@ -195,29 +195,41 @@
         :return: True if the assertion passes
         """
         return assert_flows_succeed(
             startLocation, headers, soft, snapshot, self.session, df_format
         )
 
     def assert_no_duplicate_router_ids(
-        self, snapshot=None, nodes=None, protocols=None, soft=False, df_format="table"
-    ):
-        # type: (Optional[str], Optional[str], Optional[List[str]], bool, str) -> bool
+        self,
+        snapshot: Optional[str] = None,
+        nodes: Optional[str] = None,
+        protocols: Optional[List[str]] = None,
+        soft: bool = False,
+        df_format: str = "table",
+        ignore_same_node: bool = False,
+    ) -> bool:
         """Assert that there are no duplicate router IDs present in the snapshot.
 
         :param snapshot: the snapshot on which to check the assertion
         :param nodes: the nodes on which to run the assertion
         :param protocols: the protocol on which to use the assertion, e.g. bgp, ospf, etc.
         :param soft: whether this assertion is soft (i.e., generates a warning but
             not a failure)
         :param df_format: How to format the Dataframe content in the output message.
             Valid options are 'table' and 'records' (each row is a key-value pairs).
+        :param ignore_same_node whether to ignore duplicate router-ids on the same node
         """
         return assert_no_duplicate_router_ids(
-            snapshot, nodes, protocols, soft, self.session, df_format
+            snapshot,
+            nodes,
+            protocols,
+            soft,
+            self.session,
+            df_format,
+            ignore_same_node,
         )
 
     def assert_no_forwarding_loops(self, snapshot=None, soft=False, df_format="table"):
         # type: (Optional[str], bool, str) -> bool
         """Assert that there are no forwarding loops in the snapshot.
 
         :param snapshot: the snapshot on which to check the assertion
@@ -356,15 +368,15 @@
         self.asserts = Asserts(self)
 
         # Additional worker args
         self.additional_args = {}  # type: Dict
 
         self.elapsed_delay = 5  # type: int
         self.stale_timeout = 5  # type: int
-        self.enable_diagnostics = True  # type: bool
+        self.enable_diagnostics = False  # type: bool
 
         # Auto-load question templates
         if load_questions:
             self.q.load()
 
         self._use_deprecated_workmgr_v1 = (
             use_deprecated_workmgr_v1
```

## Comparing `pybatfish-2022.9.7.77.dist-info/LICENSE` & `pybatfish-2023.5.12.784.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pybatfish-2022.9.7.77.dist-info/METADATA` & `pybatfish-2023.5.12.784.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pybatfish
-Version: 2022.9.7.77
+Version: 2023.5.12.784
 Summary: Python API and utilities for Batfish
 Home-page: https://github.com/batfish/pybatfish
 Author: The Batfish Open Source Project
 Author-email: pybatfish-dev@intentionet.com
 License: Apache License 2.0
 Keywords: network configuration verification
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: attrs (>=18.1.0)
 Requires-Dist: deepdiff
 Requires-Dist: deprecated
 Requires-Dist: netconan (>=0.12.0)
 Requires-Dist: pandas (<1.2)
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
@@ -112,9 +112,7 @@
 ```
 
 Our notebooks provide a quick start guide for different use cases. Beyond that, the complete documentation is available on [readthedocs](https://pybatfish.readthedocs.io/en/latest/quickstart.html).
 
 ### Pybatfish documentation
 
 Complete documentation of pybatfish APIs is [here](https://pybatfish.readthedocs.io/en/latest/).
-
-
```

