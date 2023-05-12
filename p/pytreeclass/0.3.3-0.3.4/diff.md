# Comparing `tmp/pytreeclass-0.3.3.tar.gz` & `tmp/pytreeclass-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.3.tar", last modified: Tue Apr 25 07:45:16 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.4.tar", last modified: Fri May 12 18:36:35 2023, max compression
```

## Comparing `pytreeclass-0.3.3.tar` & `pytreeclass-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.437437 pytreeclass-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.437437 pytreeclass-0.3.3/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.441437 pytreeclass-0.3.3/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30880 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.441437 pytreeclass-0.3.3/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 07:45:16.000000 pytreeclass-0.3.3/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:16.445437 pytreeclass-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-25 07:45:05.000000 pytreeclass-0.3.3/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28159 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28279 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.3/LICENSE` & `pytreeclass-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.3/PKG-INFO` & `pytreeclass-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.3
+Version: 0.3.4
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -904,9 +904,10 @@
 </table>
 
 </details>
 
 ## 📙 Acknowledgements<a id="acknowledgements"></a>
 
 - [Farid Talibli (for visualization link generation backend)](https://www.linkedin.com/in/frdt98)
+- [Lenses](https://hackage.haskell.org/package/lens)
 - [Treex](https://github.com/cgarciae/treex), [Equinox](https://github.com/patrick-kidger/equinox), [tree-math](https://github.com/google/tree-math), [Flax](https://github.com/google/flax), [TensorFlow](https://www.tensorflow.org), [PyTorch](https://pytorch.org)
 - [Lovely JAX](https://github.com/xl0/lovely-jax)
```

### Comparing `pytreeclass-0.3.3/README.md` & `pytreeclass-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -881,9 +881,10 @@
 </table>
 
 </details>
 
 ## 📙 Acknowledgements<a id="acknowledgements"></a>
 
 - [Farid Talibli (for visualization link generation backend)](https://www.linkedin.com/in/frdt98)
+- [Lenses](https://hackage.haskell.org/package/lens)
 - [Treex](https://github.com/cgarciae/treex), [Equinox](https://github.com/patrick-kidger/equinox), [tree-math](https://github.com/google/tree-math), [Flax](https://github.com/google/flax), [TensorFlow](https://www.tensorflow.org), [PyTorch](https://pytorch.org)
 - [Lovely JAX](https://github.com/xl0/lovely-jax)
```

### Comparing `pytreeclass-0.3.3/docs/conf.py` & `pytreeclass-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.3/pytreeclass/__init__.py` & `pytreeclass-0.3.4/pytreeclass/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from pytreeclass._src.tree_decorator import TreeClass, field, fields
-from pytreeclass._src.tree_freeze import freeze, is_frozen, is_nondiff, unfreeze
-from pytreeclass._src.tree_indexer import bcmap, is_tree_equal, tree_indexer
+from pytreeclass._src.code_build import field, fields
+from pytreeclass._src.tree_base import AtIndexer, TreeClass
 from pytreeclass._src.tree_pprint import (
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
     tree_str,
     tree_summary,
 )
-from pytreeclass._src.tree_trace import (
+from pytreeclass._src.tree_util import (
+    Partial,
+    bcmap,
+    freeze,
+    is_frozen,
+    is_nondiff,
+    is_tree_equal,
     tree_flatten_with_trace,
     tree_leaves_with_trace,
     tree_map_with_trace,
+    unfreeze,
 )
 
 __all__ = (
     # general utils
     "TreeClass",
     "is_tree_equal",
     "field",
@@ -25,23 +31,23 @@
     # pprint utils
     "tree_diagram",
     "tree_mermaid",
     "tree_repr",
     "tree_str",
     "tree_indent",
     "tree_summary",
-    "tree_trace_summary",
     # freeze/unfreeze utils
     "is_nondiff",
     "is_frozen",
     "freeze",
     "unfreeze",
     # masking and indexing utils
     "bcmap",
-    "tree_indexer",
+    "AtIndexer",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
+    "Partial",
 )
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
```

### Comparing `pytreeclass-0.3.3/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.3.4/pytreeclass/_src/tree_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,527 +1,519 @@
 from __future__ import annotations
 
-import functools as ft
-import operator as op
+import abc
 from collections.abc import Callable
 from contextlib import contextmanager
-from math import ceil, floor, trunc
 from typing import Any, NamedTuple, TypeVar
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
+from typing_extensions import dataclass_transform
 
-from pytreeclass._src.tree_pprint import tree_repr_with_trace
-from pytreeclass._src.tree_trace import NamedSequenceKey, TraceType, tree_map_with_trace
+from pytreeclass._src.code_build import (
+    Field,
+    _build_field_map,
+    _build_init_method,
+    field,
+)
+from pytreeclass._src.tree_pprint import tree_repr, tree_str
+from pytreeclass._src.tree_util import (
+    IsLeafType,
+    NamedSequenceKey,
+    _leafwise_transform,
+    _resolve_where,
+    is_tree_equal,
+    tree_copy,
+    tree_hash,
+)
 
-T = TypeVar("T")
+"""Define a class that convert a class to a JAX compatible tree structure"""
+
+
+T = TypeVar("T", bound="TreeClass")
 PyTree = Any
 EllipsisType = type(Ellipsis)
 _no_initializer = object()
-_non_partial = object()
-
 
 # allow methods in mutable context to be called without raising `AttributeError`
-# the instances are registered  during initialization and using `at` property with `__call__
-# this is done by registering the instance id in a set before entering the
-# mutable context and removing it after exiting the context
+# the instances are registered  during initialization and using `at`  property
+# with `__call__ this is done by registering the instance id in a set before
+# entering the mutable context and removing it after exiting the context
 _mutable_instance_registry: set[int] = set()
 
 
-def _unpack_entry(entry) -> tuple[Any, ...]:
-    # define rule for indexing matching through `at` property
-    # for example `jax` internals uses `jtu.GetAttrKey` to index an attribute, however
-    # its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]` to index an attribute
-    # instead `tree.at['attr']` is more ergonomic
-    if isinstance(entry, jtu.GetAttrKey):
-        return (entry.name,)
-    if isinstance(entry, jtu.SequenceKey):
-        return (entry.idx,)
-    if isinstance(entry, (jtu.DictKey, jtu.FlattenedIndexKey)):
-        return (entry.key,)
-    if isinstance(entry, NamedSequenceKey):
-        return (entry.idx, entry.key)
-    return (entry,)
-
-
-def tree_copy(tree: T) -> T:
-    """Return a copy of the tree."""
-    leaves, treedef = jtu.tree_flatten(tree)
-    return jtu.tree_unflatten(treedef, leaves)
-
-
 @contextmanager
-def _mutable_context(tree: PyTree, *, kopy: bool = False):
+def _mutable_context(tree, *, kopy: bool = False):
     tree = tree_copy(tree) if kopy else tree
     _mutable_instance_registry.add(id(tree))
     yield tree
     _mutable_instance_registry.discard(id(tree))
 
 
-# tree indexing by boolean PyTree
+def _register_treeclass(klass: type[T]) -> type[T]:
+    # handle all registration logic for `treeclass`
+
+    def tree_unflatten(keys: tuple[str, ...], leaves: tuple[Any, ...]) -> T:
+        # unflatten rule to use with `jax.tree_unflatten`
+        tree = getattr(object, "__new__")(klass)
+        vars(tree).update(zip(keys, leaves))
+        return tree
+
+    def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
+        # flatten rule to use with `jax.tree_flatten`
+        dynamic = vars(tree)
+        return tuple(dynamic.values()), tuple(dynamic.keys())
+
+    def tree_flatten_with_keys(tree: T):
+        # flatten rule to use with `jax.tree_util.tree_flatten_with_path`
+        dynamic = dict(vars(tree))
+        for idx, key in enumerate(vars(tree)):
+            entry = NamedSequenceKey(idx, key)
+            dynamic[key] = (entry, dynamic[key])
+        return tuple(dynamic.values()), tuple(dynamic.keys())
+
+    jtu.register_pytree_with_keys(
+        nodetype=klass,
+        flatten_func=tree_flatten,
+        flatten_with_keys=tree_flatten_with_keys,
+        unflatten_func=tree_unflatten,
+    )
+    return klass
 
 
-def _get_at_mask(
-    tree: PyTree, where: PyTree, is_leaf: Callable[[Any], bool] | None
-) -> PyTree:
-    def leaf_get(leaf: Any, where: Any):
-        if isinstance(where, (jax.Array, np.ndarray)) and where.ndim != 0:
-            return leaf[jnp.where(where)]
-        return leaf if where else None
-
-    return jtu.tree_map(leaf_get, tree, where, is_leaf=is_leaf)
-
-
-def _set_at_mask(
-    tree: PyTree,
-    where: PyTree,
-    set_value: Any,
-    is_leaf: Callable[[Any], bool] | None,
-) -> PyTree:
-    def leaf_set(leaf: Any, where: Any, set_value: Any):
-        if isinstance(where, (jax.Array, np.ndarray)):
-            return jnp.where(where, set_value, leaf)
-        return set_value if where else leaf
-
-    if jtu.tree_structure(tree) == jtu.tree_structure(set_value):
-        # do not broadcast set_value if it is a pytree of same structure
-        # for example tree.at[where].set(tree2) will set all tree leaves to tree2 leaves
-        # if tree2 is a pytree of same structure as tree
-        # instead of making each leaf of tree a copy of tree2
-        # is design is similar to `numpy` design `Array.at[...].set(Array)`
-        return jtu.tree_map(leaf_set, tree, where, set_value, is_leaf=is_leaf)
-
-    # set_value is broadcasted to tree leaves
-    # for example tree.at[where].set(1) will set all tree leaves to 1
-    partial_leaf_set = lambda leaf, where: leaf_set(leaf, where, set_value)
-    return jtu.tree_map(partial_leaf_set, tree, where, is_leaf=is_leaf)
-
-
-def _apply_at_mask(
-    tree: PyTree,
-    where: PyTree,
-    func: Callable[[Any], Any],
-    is_leaf: Callable[[Any], bool] | None,
-) -> PyTree:
-    def leaf_apply(leaf: Any, where: bool):
-        if isinstance(where, (jax.Array, np.ndarray)):
-            return jnp.where(where, func(leaf), leaf)
-        return func(leaf) if where else leaf
-
-    return jtu.tree_map(leaf_apply, tree, where, is_leaf=is_leaf)
-
-
-def _reduce_at_mask(
-    tree: PyTree,
-    where: PyTree,
-    func: Callable[[Any, Any], Any],
-    initializer: Any = _no_initializer,
-    is_leaf: Callable[[Any], bool] | None = None,
-) -> Any:
-    tree = tree.at[where].get(is_leaf=is_leaf)  # type: ignore
-    if initializer is _no_initializer:
-        return jtu.tree_reduce(func, tree)
-    return jtu.tree_reduce(func, tree, initializer)
-
-
-def _generate_path_mask(
-    tree: PyTree,
-    where: tuple[int | str, ...],
-    is_leaf: Callable[[Any], bool] | None = None,
-) -> PyTree:
-    match = False
-
-    def map_func(path: TraceType, _: Any):
-        keys, _ = path
-
-        if len(where) > len(keys):
-            return False
-
-        for wi, key in zip(where, keys):
-            if wi not in (..., *_unpack_entry(key)):
-                return False
-
-        nonlocal match
-
-        return (match := True)
-
-    mask = tree_map_with_trace(map_func, tree, is_leaf=is_leaf)
-
-    if not match:
-        fmt = "/".join(map(str, where))
-        msg = f"No leaf match is found for path={fmt} for tree with trace:\n"
-        msg += f"{tree_repr_with_trace(tree)}\n"
-        msg += f"with mask={mask}"
-        raise LookupError(msg)
-
-    return mask
-
-
-def _combine_maybe_bool_masks(*masks: PyTree) -> PyTree:
-    def is_bool_leaf(leaf: Any) -> bool:
-        if hasattr(leaf, "dtype"):
-            return leaf.dtype == "bool"
-        return isinstance(leaf, bool)
-
-    def map_func(*leaves):
-        verdict = True
-        for leaf in leaves:
-            if not is_bool_leaf(leaf):
-                msg = f"Expected boolean, got {leaf=}, of type {type(leaf).__name__}."
-                raise TypeError(msg)
-            verdict &= leaf
-        return verdict
-
-    return jtu.tree_map(map_func, *masks)
-
-
-def _resolve_where(
-    tree: PyTree,
-    where: tuple[int | str | PyTree | EllipsisType, ...],
-    is_leaf: Callable[[Any], bool] | None = None,
-):
-    mask = None
-
-    if path := [i for i in where if isinstance(i, (int, str, type(...)))]:
-        mask = _generate_path_mask(tree, path, is_leaf=is_leaf)
-
-    if maybe_bool_masks := [i for i in where if isinstance(i, type(tree))]:
-        all_masks = [mask, *maybe_bool_masks] if mask else maybe_bool_masks
-        mask = _combine_maybe_bool_masks(*all_masks)
-
-    return mask
-
-
-def _recursive_getattr(tree: Any, where: tuple[str, ...]):
-    def step(tree: Any, where: tuple[str, ...]):
-        if len(where) == 1:
-            return getattr(tree, where[0])
-        return step(getattr(tree, where[0]), where[1:])
+class AtIndexer(NamedTuple):
+    """Adds `.at` indexing abilities to a PyTree.
 
-    return step(tree, where)
+    Example:
+        >>> import jax.tree_util as jtu
+        >>> import pytreeclass as pytc
+        >>> @jax.tree_util.register_pytree_with_keys_class
+        ... class Tree:
+        ...    def __init__(self, a, b):
+        ...        self.a = a
+        ...        self.b = b
+        ...    def tree_flatten_with_keys(self):
+        ...        kva = (jtu.GetAttrKey("a"), self.a)
+        ...        kvb = (jtu.GetAttrKey("b"), self.b)
+        ...        return (kva, kvb), None
+        ...    @classmethod
+        ...    def tree_unflatten(cls, aux_data, children):
+        ...        return cls(*children)
+        ...    @property
+        ...    def at(self):
+        ...        return pytc.AtIndexer(self, where=())
+        ...    def __repr__(self) -> str:
+        ...        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
 
+        >>> Tree(1, 2).at["a"].get()
+        Tree(a=1, b=None)
+    """
 
-class AtIndexer(NamedTuple):
-    # base class for indexing with `.at`
     tree: PyTree
     where: tuple[str | int] | PyTree
 
     def __getitem__(self, where: str | int | PyTree | EllipsisType) -> AtIndexer:
         if isinstance(where, (type(self.tree), str, int, EllipsisType)):
             return AtIndexer(self.tree, (*self.where, where))
 
         raise NotImplementedError(
             f"Indexing with {type(where).__name__} is not implemented.\n"
             "Example of supported indexing:\n\n"
+            ">>> import jax\n"
+            ">>> import pytreeclass as pytc\n"
             f"class {type(self.tree).__name__}:(pytc.TreeClass)\n"
             "    ...\n\n"
             f">>> tree = {type(self.tree).__name__}(...)\n"
             ">>> # indexing by boolean pytree\n"
-            ">>> tree.at[tree > 0].get()\n\n"
+            ">>> mask = jax.tree_map(lambda x: x > 0, tree)\n"
+            ">>> tree.at[mask].get()\n\n"
             ">>> # indexing by attribute name\n"
             ">>> tree.at[`attribute_name`].get()\n\n"
-            ">>> # indexing by attribute index\n"
-            ">>> tree.at[`attribute_index`].get()"
+            ">>> # indexing by leaf index\n"
+            ">>> tree.at[index].get()"
         )
 
-    def get(self, *, is_leaf: Callable[[Any], bool] | None = None) -> PyTree:
+    def get(self, *, is_leaf: IsLeafType = None) -> PyTree:
+        """Get the leaf values at the specified location.
+
+        Args:
+            is_leaf: a predicate function to determine if a value is a leaf.
+
+        Returns:
+            A PyTree of leaf values at the specified location, with the
+            non-selected leaf values set to None if the leaf is not an array.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> class Tree(pytc.TreeClass):
+            ...     a: int
+            ...     b: int
+            >>> tree = Tree(a=1, b=2)
+            >>> # get `a` and return a new instance
+            >>> # with `None` for all other leaves
+            >>> tree.at['a'].get()
+            Tree(a=1, b=None)
+        """
         where = _resolve_where(self.tree, self.where, is_leaf)
-        return _get_at_mask(self.tree, where, is_leaf)
 
-    def set(
-        self,
-        set_value: Any,
-        *,
-        is_leaf: Callable[[Any], bool] | None = None,
-    ) -> PyTree:
+        def leaf_get(leaf: Any, where: Any):
+            if isinstance(where, (jax.Array, np.ndarray)) and where.ndim != 0:
+                return leaf[jnp.where(where)]
+            return leaf if where else None
+
+        return jtu.tree_map(leaf_get, self.tree, where, is_leaf=is_leaf)
+
+    def set(self, set_value: Any, *, is_leaf: IsLeafType = None):
+        """Set the leaf values at the specified location.
+
+        Args:
+            set_value: the value to set at the specified location.
+            is_leaf: a predicate function to determine if a value is a leaf.
+
+        Returns:
+            A PyTree with the leaf values at the specified location
+            set to `set_value`.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> class Tree(pytc.TreeClass):
+            ...     a: int
+            ...     b: int
+            >>> tree = Tree(a=1, b=2)
+            >>> # set `a` and return a new instance
+            >>> # with all other leaves unchanged
+            >>> tree.at['a'].set(100)
+            Tree(a=100, b=2)
+        """
         where = _resolve_where(self.tree, self.where, is_leaf)
-        return _set_at_mask(self.tree, where, set_value, is_leaf)
 
-    def apply(
-        self,
-        func: Callable[[Any], Any],
-        *,
-        is_leaf: Callable[[Any], bool] | None = None,
-    ) -> PyTree:
+        def leaf_set(leaf: Any, where: Any, set_value: Any):
+            if isinstance(where, (jax.Array, np.ndarray)):
+                return jnp.where(where, set_value, leaf)
+            return set_value if where else leaf
+
+        if jtu.tree_structure(self.tree) == jtu.tree_structure(set_value):
+            # do not broadcast set_value if it is a pytree of same structure
+            # for example tree.at[where].set(tree2) will set all tree leaves
+            # to tree2 leaves if tree2 is a pytree of same structure as tree
+            # instead of making each leaf of tree a copy of tree2
+            # is design is similar to `numpy` design `Array.at[...].set(Array)`
+            return jtu.tree_map(leaf_set, self.tree, where, set_value, is_leaf=is_leaf)
+
+        # set_value is broadcasted to tree leaves
+        # for example tree.at[where].set(1) will set all tree leaves to 1
+        partial_leaf_set = lambda leaf, where: leaf_set(leaf, where, set_value)
+        return jtu.tree_map(partial_leaf_set, self.tree, where, is_leaf=is_leaf)
+
+    def apply(self, func: Callable[[Any], Any], *, is_leaf: IsLeafType = None):
+        """Apply a function to the leaf values at the specified location.
+
+        Args:
+            func: the function to apply to the leaf values.
+            is_leaf: a predicate function to determine if a value is a leaf.
+
+        Returns:
+            A PyTree with the leaf values at the specified location set to
+            the result of applying `func` to the leaf values.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> class Tree(pytc.TreeClass):
+            ...     a: int
+            ...     b: int
+            >>> tree = Tree(a=1, b=2)
+            >>> # apply to `a` and return a new instance
+            >>> # with all other leaves unchanged
+            >>> tree.at['a'].apply(lambda _: 100)
+            Tree(a=100, b=2)
+        """
         where = _resolve_where(self.tree, self.where, is_leaf)
-        return _apply_at_mask(self.tree, where, func, is_leaf)
+
+        def leaf_apply(leaf: Any, where: bool):
+            if isinstance(where, (jax.Array, np.ndarray)):
+                return jnp.where(where, func(leaf), leaf)
+            return func(leaf) if where else leaf
+
+        return jtu.tree_map(leaf_apply, self.tree, where, is_leaf=is_leaf)
 
     def reduce(
         self,
         func: Callable[[Any, Any], Any],
         *,
         initializer: Any = _no_initializer,
-        is_leaf: Callable[[Any], bool] | None = None,
+        is_leaf: IsLeafType = None,
     ) -> Any:
+        """Reduce the leaf values at the specified location.
+
+        Args:
+            func: the function to reduce the leaf values.
+            initializer: the initializer value for the reduction.
+            is_leaf: a predicate function to determine if a value is a leaf.
+
+        Returns:
+            The result of reducing the leaf values at the specified location.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> class Tree(pytc.TreeClass):
+            ...     a: int
+            ...     b: int
+            >>> tree = Tree(a=1, b=2)
+            >>> tree.at[...].reduce(lambda a, b: a + b, initializer=0)
+            3
+        """
         where = _resolve_where(self.tree, self.where, is_leaf)
-        return _reduce_at_mask(self.tree, where, func, initializer, is_leaf)
+        tree = self.tree.at[where].get(is_leaf=is_leaf)  # type: ignore
+        if initializer is _no_initializer:
+            return jtu.tree_reduce(func, tree)
+        return jtu.tree_reduce(func, tree, initializer)
 
     def __getattr__(self, name: str) -> AtIndexer:
-        # support nested `.at``
-        # for example `.at[A].at[B]` represents model.A.B
+        """Support nested indexing"""
         if name == "at":
             # pass the current tree and the current path to the next `.at`
             return AtIndexer(tree=self.tree, where=self.where)
 
-        msg = f"{name} is not a valid attribute of {self}\n"
-        msg += f"Did you mean to use .at[{name!r}]?"
-        raise AttributeError(msg)
+        raise AttributeError(f"`{type(self).__name__!r}` has no attribute {name!r}.")
 
     def __call__(self, *a, **k) -> tuple[Any, PyTree]:
+        """
+        Call the function at the specified location and return a **copy**
+        of the tree. with the result of the function call.
+
+        Returns:
+            A tuple of the result of the function call and a copy of the a
+            new instance of the tree with the modified values.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> class Tree(pytc.TreeClass):
+            ...     a: int
+            ...     def add(self, x:int) -> int:
+            ...         self.a += x
+            ...         return self.a
+            >>> tree = Tree(a=1)
+            >>> # call `add` and return a tuple of
+            >>> # (return value, new instance)
+            >>> tree.at['add'](99)
+            (100, Tree(a=100))
+
+        Note:
+            - `AttributeError` is raised, If the function mutates the instance.
+            - Use .at["method_name"](*, **) to call a method that mutates the instance.
+        """
+
+        def recursive_getattr(tree: Any, where: tuple[str, ...]):
+            if len(where) == 1:
+                return getattr(tree, where[0])
+            return recursive_getattr(getattr(tree, where[0]), where[1:])
+
         with _mutable_context(self.tree, kopy=True) as tree:
-            value = _recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
+            value = recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
         return value, tree
 
 
-def tree_indexer(tree: PyTree) -> AtIndexer:
-    """Adds `.at` indexing abilities to a PyTree.
+class TreeClassMeta(abc.ABCMeta):
+    def __call__(klass: type[T], *a, **k) -> T:
+        self = getattr(klass, "__new__")(klass, *a, **k)
+
+        with _mutable_context(self):
+            # initialize the instance under the mutable context
+            # to allow setting instance attributes without
+            # throwing an `AttributeError`
+            getattr(klass, "__init__")(self, *a, **k)
+
+        if len(keys := set(_build_field_map(klass)) - set(vars(self))):
+            raise AttributeError(f"Found uninitialized fields {keys}.")
+        return self
+
+
+@dataclass_transform(field_specifiers=(field, Field))
+class TreeClass(metaclass=TreeClassMeta):
+    """Convert a class to a JAX compatible tree structure.
 
     Example:
-        >>> import jax.tree_util as jtu
+        >>> import jax
         >>> import pytreeclass as pytc
-        >>> @jax.tree_util.register_pytree_with_keys_class
-        ... class Tree:
-        ...    def __init__(self, a, b):
-        ...        self.a = a
-        ...        self.b = b
-        ...    def tree_flatten_with_keys(self):
-        ...        return ((jtu.GetAttrKey("a"), self.a), (jtu.GetAttrKey("b"), self.b)), None
-        ...    @classmethod
-        ...    def tree_unflatten(cls, aux_data, children):
-        ...        return cls(*children)
-        ...    @property
-        ...    def at(self):
-        ...        return pytc.tree_indexer(self)
-        ...    def __repr__(self) -> str:
-        ...        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
 
-        >>> Tree(1, 2).at["a"].get()
+        >>> # Tree leaves are instance attributes
+        >>> class Tree(pytc.TreeClass):
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> jax.tree_util.tree_leaves(tree)
+        [1, 2.0]
+
+        >>> # Leaf-wise math operations are supported by setting `leafwise=True`
+        >>> class Tree(pytc.TreeClass, leafwise=True):
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> tree + 1
+        Tree(a=2, b=3.0)
+
+        >>> # Advanced indexing is supported using `at` property
+        >>> class Tree(pytc.TreeClass):
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> tree.at["a"].get()
+        Tree(a=1, b=None)
+        >>> tree.at[0].get()
         Tree(a=1, b=None)
-    """
-    return AtIndexer(tree=tree, where=())
-
 
-class BroadcastablePartial(ft.partial):
-    def __call__(self, *args, **keywords) -> Callable:
-        # https://stackoverflow.com/a/7811270
-        keywords = {**self.keywords, **keywords}
-        iargs = iter(args)
-        args = (next(iargs) if arg is _non_partial else arg for arg in self.args)  # type: ignore
-        return self.func(*args, *iargs, **keywords)
-
-
-def bcmap(
-    func: Callable[..., Any],
-    *,
-    is_leaf: Callable[[Any], bool] | None = None,
-) -> Callable:
-    """(map)s a function over pytrees leaves with automatic (b)road(c)asting for scalar arguments
-
-    Args:
-        func: the function to be mapped over the pytree
-        is_leaf: a function that returns True if the argument is a leaf of the pytree
+    Note:
+        ``leafwise=True`` adds the following methods to the class
 
-    Example:
-        >>> import jax
-        >>> import pytreeclass as pytc
-        >>> import functools as ft
+        ==================      ============
+        Method                  Operator
+        ==================      ============
+        ``__add__``              ``+``
+        ``__and__``              ``&``
+        ``__ceil__``             ``math.ceil``
+        ``__divmod__``           ``divmod``
+        ``__eq__``               ``==``
+        ``__floor__``            ``math.floor``
+        ``__floordiv__``         ``//``
+        ``__ge__``               ``>=``
+        ``__gt__``               ``>``
+        ``__invert__``           ``~``
+        ``__le__``               ``<=``
+        ``__lshift__``           ``<<``
+        ``__lt__``               ``<``
+        ``__matmul__``           ``@``
+        ``__mod__``              ``%``
+        ``__mul__``              ``*``
+        ``__ne__``               ``!=``
+        ``__neg__``              ``-``
+        ``__or__``               ``|``
+        ``__pos__``              ``+``
+        ``__pow__``              ``**``
+        ``__round__``            ``round``
+        ``__sub__``              ``-``
+        ``__truediv__``          ``/``
+        ``__trunc__``            ``math.trunc``
+        ``__xor__``              ``^``
+        ==================      ============
 
-        >>> class Test(pytc.TreeClass, leafwise=True):
-        ...    a: tuple[int] = (1,2,3)
-        ...    b: tuple[int] = (4,5,6)
-        ...    c: jax.Array = jnp.array([1,2,3])
-
-        >>> tree = Test()
-
-        >>> # 0 is broadcasted to all leaves of the pytree
-        >>> print(pytc.bcmap(jnp.where)(tree>1, tree, 0))
-        Test(a=(0, 2, 3), b=(4, 5, 6), c=[0 2 3])
-        >>> print(pytc.bcmap(jnp.where)(tree>1, 0, tree))
-        Test(a=(1, 0, 0), b=(0, 0, 0), c=[1 0 0])
-
-        >>> # 1 is broadcasted to all leaves of the list pytree
-        >>> pytc.bcmap(lambda x,y:x+y)([1,2,3],1)
-        [2, 3, 4]
-
-        >>> # trees are summed leaf-wise
-        >>> pytc.bcmap(lambda x,y:x+y)([1,2,3],[1,2,3])
-        [2, 4, 6]
-
-        >>> # Non scalar second args case
-        >>> try:
-        ...     pytc.bcmap(lambda x,y:x+y)([1,2,3],[[1,2,3],[1,2,3]])
-        ... except TypeError as e:
-        ...     print(e)
-        unsupported operand type(s) for +: 'int' and 'list'
-
-        >>> # using **numpy** functions on pytrees
-        >>> import jax.numpy as jnp
-        >>> pytc.bcmap(jnp.add)([1,2,3],[1,2,3]) # doctest: +SKIP
-        [2, 4, 6]
     """
 
-    @ft.wraps(func)
-    def wrapper(*args, **kwargs):
-        if len(args) > 0:
-            # positional arguments are passed the argument to be compare
-            # the tree structure with is the first argument
-            leaves0, treedef0 = jtu.tree_flatten(args[0], is_leaf=is_leaf)
-            masked_args = [_non_partial]
-            masked_kwargs = {}
-            leaves = [leaves0]
-            leaves_keys = []
-
-            for arg in args[1:]:
-                if treedef0 == jtu.tree_structure(arg):
-                    masked_args += [_non_partial]
-                    leaves += [treedef0.flatten_up_to(arg)]
-                else:
-                    masked_args += [arg]
-        else:
-            # only kwargs are passed the argument to be compare
-            # the tree structure with is the first kwarg
-            key0 = next(iter(kwargs))
-            leaves0, treedef0 = jtu.tree_flatten(kwargs.pop(key0), is_leaf=is_leaf)
-            masked_args = []
-            masked_kwargs = {key0: _non_partial}
-            leaves = [leaves0]
-            leaves_keys = [key0]
-
-        for key in kwargs:
-            if treedef0 == jtu.tree_structure(kwargs[key]):
-                masked_kwargs[key] = _non_partial
-                leaves += [treedef0.flatten_up_to(kwargs[key])]
-                leaves_keys += [key]
-            else:
-                masked_kwargs[key] = kwargs[key]
-
-        bfunc = BroadcastablePartial(func, *masked_args, **masked_kwargs)
-
-        if len(leaves_keys) == 0:
-            # no kwargs leaves are present, so we can immediately zip
-            return jtu.tree_unflatten(treedef0, [bfunc(*xs) for xs in zip(*leaves)])
-
-        # kwargs leaves are present, so we need to zip them
-        kwargnum = len(leaves) - len(leaves_keys)
-        all_leaves = []
-        for xs in zip(*leaves):
-            xs_args, xs_kwargs = xs[:kwargnum], xs[kwargnum:]
-            all_leaves += [bfunc(*xs_args, **dict(zip(leaves_keys, xs_kwargs)))]
-        return jtu.tree_unflatten(treedef0, all_leaves)
-
-    docs = f"Broadcasted version of {func.__name__}\n{func.__doc__}"
-    wrapper.__doc__ = docs
-    return wrapper
-
-
-def _unary_op(func):
-    def wrapper(self):
-        return jtu.tree_map(func, self)
-
-    return ft.wraps(func)(wrapper)
-
-
-def _binary_op(func):
-    def wrapper(leaf, rhs=None):
-        if isinstance(rhs, type(leaf)):
-            return jtu.tree_map(func, leaf, rhs)
-        return jtu.tree_map(lambda x: func(x, rhs), leaf)
-
-    return ft.wraps(func)(wrapper)
-
-
-def _swop(func):
-    # swaping the arguments of a two-arg function
-    return ft.wraps(func)(lambda leaf, rhs: func(rhs, leaf))
-
-
-def _leafwise_transform(klass: type[T]) -> type[T]:
-    # add leafwise transform methods to the class
-    # that enable the user to apply a function to
-    # all the leaves of the tree
-    for key, method in (
-        ("__abs__", _unary_op(abs)),
-        ("__add__", _binary_op(op.add)),
-        ("__and__", _binary_op(op.and_)),
-        ("__ceil__", _unary_op(ceil)),
-        ("__divmod__", _binary_op(divmod)),
-        ("__eq__", _binary_op(op.eq)),
-        ("__floor__", _unary_op(floor)),
-        ("__floordiv__", _binary_op(op.floordiv)),
-        ("__ge__", _binary_op(op.ge)),
-        ("__gt__", _binary_op(op.gt)),
-        ("__invert__", _unary_op(op.invert)),
-        ("__le__", _binary_op(op.le)),
-        ("__lshift__", _binary_op(op.lshift)),
-        ("__lt__", _binary_op(op.lt)),
-        ("__matmul__", _binary_op(op.matmul)),
-        ("__mod__", _binary_op(op.mod)),
-        ("__mul__", _binary_op(op.mul)),
-        ("__ne__", _binary_op(op.ne)),
-        ("__neg__", _unary_op(op.neg)),
-        ("__or__", _binary_op(op.or_)),
-        ("__pos__", _unary_op(op.pos)),
-        ("__pow__", _binary_op(op.pow)),
-        ("__radd__", _binary_op(_swop(op.add))),
-        ("__rand__", _binary_op(_swop(op.and_))),
-        ("__rdivmod__", _binary_op(_swop(divmod))),
-        ("__rfloordiv__", _binary_op(_swop(op.floordiv))),
-        ("__rlshift__", _binary_op(_swop(op.lshift))),
-        ("__rmatmul__", _binary_op(_swop(op.matmul))),
-        ("__rmod__", _binary_op(_swop(op.mod))),
-        ("__rmul__", _binary_op(_swop(op.mul))),
-        ("__ror__", _binary_op(_swop(op.or_))),
-        ("__round__", _binary_op(round)),
-        ("__rpow__", _binary_op(_swop(op.pow))),
-        ("__rrshift__", _binary_op(_swop(op.rshift))),
-        ("__rshift__", _binary_op(op.rshift)),
-        ("__rsub__", _binary_op(_swop(op.sub))),
-        ("__rtruediv__", _binary_op(_swop(op.truediv))),
-        ("__rxor__", _binary_op(_swop(op.xor))),
-        ("__sub__", _binary_op(op.sub)),
-        ("__truediv__", _binary_op(op.truediv)),
-        ("__trunc__", _unary_op(trunc)),
-        ("__xor__", _binary_op(op.xor)),
-    ):
-        if key not in vars(klass):
-            # do not override any user defined methods
-            # this behavior similar is to `dataclasses.dataclass`
-            setattr(klass, key, method)
-    return klass
-
-
-def _is_leaf_rhs_equal(leaf, rhs) -> bool | jax.Array:
-    if hasattr(leaf, "shape") and hasattr(leaf, "dtype"):
-        if hasattr(rhs, "shape") and hasattr(rhs, "dtype"):
-            verdict = jnp.array_equal(leaf, rhs)
-            try:
-                return bool(verdict)
-            except Exception:
-                return verdict  # fail under `jit`
-        return False
-    return leaf == rhs
-
+    def __init_subclass__(
+        klass: type[T],
+        *a,
+        leafwise: bool = False,
+        **k,
+    ) -> None:
+        if "__setattr__" in vars(klass) or "__delattr__" in vars(klass):
+            raise TypeError(
+                f"Unable to transform the class `{klass.__name__}` "
+                "with resereved methods: `__setattr__` or `__delattr__` "
+                "defined.\nReserved `setters` and `deleters` implements "
+                "the immutable functionality and cannot be overriden."
+            )
+
+        super().__init_subclass__(*a, **k)
+
+        if "__init__" not in vars(klass):
+            # generate the init method if not defined similar to `dataclass`
+            setattr(klass, "__init__", _build_init_method(klass))
+
+        if leafwise:
+            # transform the class to support leafwise operations
+            # useful to use with `bcmap` and creating masks by comparisons.
+            klass = _leafwise_transform(klass)
+
+        klass = _register_treeclass(klass)
+
+    def __setattr__(self, key: str, value: Any) -> None:
+        if id(self) not in _mutable_instance_registry:
+            raise AttributeError(
+                f"Cannot set attribute {value=} to `{key=}`  "
+                f"on an immutable instance of `{type(self).__name__}`.\n"
+                f"Use `.at['{key}'].set({value})` "
+                "to set the value immutably.\nExample:\n"
+                f">>> tree1 = {type(self).__name__}(...)\n"
+                f">>> tree2 = tree1.at['{key}'].set({value!r})\n"
+                ">>> assert not tree1 is tree2\n"
+                f">>> tree2.{key}\n{value}"
+            )
+
+        if key in (field_map := _build_field_map(type(self))):
+            for callback in field_map[key].callbacks:
+                try:
+                    value = callback(value)
+                except Exception as e:
+                    raise type(e)(f"Error for field=`{key}`:\n{e}")
+
+        getattr(object, "__setattr__")(self, key, value)
+
+    def __delattr__(self, key: str) -> None:
+        if id(self) not in _mutable_instance_registry:
+            raise AttributeError(
+                f"Cannot delete attribute `{key}` "
+                f"on immutable instance of `{type(self).__name__}`.\n"
+                f"Use `.at['{key}'].set(None)` instead."
+            )
+
+        getattr(object, "__delattr__")(self, key)
+
+    @property
+    def at(self) -> AtIndexer:
+        """Immutable out-of-place indexing
+
+        - `.at[***].get()`:
+            Return a new instance with the value at the index otherwise None.
+        - `.at[***].set(value)`:
+            Set the `value` and return a new instance with the updated value.
+        - `.at[***].apply(func)`:
+            Apply a `func` and return a new instance with the updated value.
+        - `.at['method'](*a, **k)`:
+            Call a `method` and return a (return value, new instance) tuple.
+
+        `***` acceptable index types are `str` for mapping keys or
+        class attributes, `int` for positional indexing, `...` for all leaves,
+        and a boolean mask of the same structure as the tree.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> class Tree(pytc.TreeClass):
+            ...     a:int = 1
+            ...     b:float = 2.0
+            ...     def add(self, x:int) -> int:
+            ...         self.a += x
+            ...         return self.a
+            >>> tree = Tree()
+            >>> # get `a` and return a new instance
+            >>> # with `None` for all other leaves
+            >>> tree.at["a"].get()
+            Tree(a=1, b=None)
+            >>> # set `a` and return a new instance
+            >>> # with all other leaves unchanged
+            >>> tree.at["a"].set(100)
+            Tree(a=100, b=2.0)
+            >>> # apply to `a` and return a new instance
+            >>> # with all other leaves unchanged
+            >>> tree.at["a"].apply(lambda x: 100)
+            Tree(a=100, b=2.0)
+            >>> # call `add` and return a tuple of
+            >>> # (return value, new instance)
+            >>> tree.at["add"](99)
+            (100, Tree(a=100, b=2.0))
+        """
+        return AtIndexer(self, where=())
+
+    def __repr__(self) -> str:
+        return tree_repr(self)
+
+    def __str__(self) -> str:
+        return tree_str(self)
 
-def is_tree_equal(*trees: Any) -> bool | jax.Array:
-    """Return `True` if all pytrees are equal.
+    def __copy__(self):
+        return tree_copy(self)
 
-    Note:
-        trees are compared using their leaves and treedefs.
-        For `array` leaves `jnp.array_equal` is used, for other leaves
-        method `__eq__` is used.
-
-    Note:
-        Under `jit` the return type is boolean `jax.Array` instead of python `bool`.
-    """
+    def __hash__(self) -> int:
+        return tree_hash(self)
 
-    tree0, *rest = trees
-    leaves0, treedef0 = jtu.tree_flatten(tree0)
-    verdict = True
-
-    for tree in rest:
-        leaves, treedef = jtu.tree_flatten(tree)
-        if (treedef != treedef0) or verdict is False:
-            return False
-        verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
-    return verdict
+    def __eq__(self, other: Any) -> bool | jax.Array:
+        return is_tree_equal(self, other)
```

### Comparing `pytreeclass-0.3.3/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.4/pytreeclass/_src/tree_pprint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,137 @@
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import inspect
 import math
-from collections import defaultdict
 from itertools import chain
 from types import FunctionType
 from typing import Any, Callable, Literal
 
 import jax
 import jax.tree_util as jtu
 import numpy as np
-from jax._src.custom_derivatives import custom_jvp
+from jax import custom_jvp
 from jax.util import unzip2
 from jaxlib.xla_extension import PjitFunction
 
-import pytreeclass as pytc
+from pytreeclass._src.tree_util import (
+    IsLeafType,
+    Node,
+    construct_tree,
+    tree_leaves_with_trace,
+    tree_map_with_trace,
+)
 
 PyTree = Any
 PrintKind = Literal["repr", "str"]
+from_iterable = chain.from_iterable
 
 
 def _node_pprint(
     node: Any,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int | float,
 ) -> str:
     if depth < 0:
         return "..."
+
+    # avoid circular import by importing Partial here
+    from pytreeclass import TreeClass
+
+    spec = dict(indent=indent, kind=kind, width=width, depth=depth)
+
     if isinstance(node, ft.partial):
-        return f"Partial({_func_pprint(node.func, indent,kind,width,depth)})"
-    if isinstance(node, (FunctionType, custom_jvp)):
-        return _func_pprint(node, indent, kind, width, depth)
-    if isinstance(node, PjitFunction):
-        return f"jit({_func_pprint(node, indent, kind, width,depth)})"
-    if isinstance(node, (np.ndarray, jax.Array)):
-        return _numpy_pprint(node, indent, kind, width, depth)
-    if isinstance(node, jax.ShapeDtypeStruct):
-        return _shape_dtype_pprint(node, indent, kind, width, depth)
-    if isinstance(node, tuple) and hasattr(node, "_fields"):
-        return _namedtuple_pprint(node, indent, kind, width, depth)
-    if isinstance(node, list):
-        return _list_pprint(node, indent, kind, width, depth)
-    if isinstance(node, tuple):
-        return _tuple_pprint(node, indent, kind, width, depth)
-    if isinstance(node, set):
-        return _set_pprint(node, indent, kind, width, depth)
-    if isinstance(node, dict):
-        return _dict_pprint(node, indent, kind, width, depth)
-    if dc.is_dataclass(node):
-        return _dataclass_pprint(node, indent, kind, width, depth)
-    if isinstance(node, pytc.TreeClass):
-        return _treeclass_pprint(node, indent, kind, width, depth)
-    return _general_pprint(node, indent, kind, width, depth)
+        text = f"Partial({_func_pprint(node.func, **spec)})"
+    elif isinstance(node, (FunctionType, custom_jvp)):
+        text = _func_pprint(node, **spec)
+    elif isinstance(node, PjitFunction):
+        text = f"jit({_func_pprint(node, **spec)})"
+    elif isinstance(node, jax.ShapeDtypeStruct):
+        text = _shape_dtype_pprint(node, **spec)
+    elif isinstance(node, tuple) and hasattr(node, "_fields"):
+        text = _namedtuple_pprint(node, **spec)
+    elif isinstance(node, list):
+        text = _list_pprint(node, **spec)
+    elif isinstance(node, tuple):
+        text = _tuple_pprint(node, **spec)
+    elif isinstance(node, set):
+        text = _set_pprint(node, **spec)
+    elif isinstance(node, dict):
+        text = _dict_pprint(node, **spec)
+    elif dc.is_dataclass(node):
+        text = _dataclass_pprint(node, **spec)
+    elif isinstance(node, TreeClass):
+        text = _treeclass_pprint(node, **spec)
+    elif isinstance(node, (np.ndarray, jax.Array)) and kind == "repr":
+        text = _numpy_pprint(node, **spec)
+    else:
+        text = _general_pprint(node, **spec)
+
+    return _format_width(text, width)
 
 
 def _general_pprint(
     node: Any,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
-    del depth
-
-    fmt = f"{node!r}" if kind == "repr" else f"{node!s}"
-    is_mutltiline = "\n" in fmt
+    del depth, width
 
-    # multiline repr/str case, increase indent and indent
+    text = f"{node!r}" if kind == "repr" else f"{node!s}"
+    is_mutltiline = "\n" in text
     indent = (indent + 1) if is_mutltiline else indent
-    fmt = ("\n" + "\t" * indent).join(fmt.split("\n"))
-    fmt = ("\n" + "\t" * (indent) + fmt) if is_mutltiline else fmt
-    return _format_width(fmt, width)
+    text = ("\n" + "\t" * indent).join(text.split("\n"))
+    text = ("\n" + "\t" * (indent) + text) if is_mutltiline else text
+    return text
 
 
 def _shape_dtype_pprint(
-    node: Any, indent: int, kind: PrintKind, width: int, depth: int
+    node: Any,
+    *,
+    indent: int,
+    kind: PrintKind,
+    width: int,
+    depth: int,
 ) -> str:
     """Pretty print a node with dtype and shape"""
-    del indent, kind, depth
+    del indent, kind, depth, width
 
     shape = f"{node.shape}".replace(",", "")
     shape = shape.replace("(", "[")
     shape = shape.replace(")", "]")
     shape = shape.replace(" ", ",")
     dtype = f"{node.dtype}".replace("int", "i")
     dtype = dtype.replace("float", "f")
     dtype = dtype.replace("complex", "c")
-    return _format_width(dtype + shape, width)
+    return dtype + shape
 
 
 def _numpy_pprint(
     node: np.ndarray | jax.Array,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     """Replace np.ndarray repr with short hand notation for type and shape"""
-    if kind == "str":
-        return _general_pprint(node, indent, "str", width, depth)
+    spec = dict(indent=indent, kind=kind, width=width, depth=depth)
 
-    base = _shape_dtype_pprint(node, indent, kind, width, depth)
+    base = _shape_dtype_pprint(node, **spec)
 
     if not issubclass(node.dtype.type, (np.integer, np.floating)) or node.size == 0:
-        return _format_width(base, width)
+        return base
 
     # Extended repr for numpy array, with extended information
     # this part of the function is inspired by
     # lovely-jax https://github.com/xl0/lovely-jax
 
     # handle interval
     low, high = np.min(node), np.max(node)
@@ -120,182 +140,196 @@
     interval += f"{low},{high}" if is_integer else f"{low:.2f},{high:.2f}"
     interval += ")" if math.isinf(high) else "]"  # resolve closed/open interval
     interval = interval.replace("inf", "∞")  # replace inf with infinity symbol
 
     # handle mean and std
     mean, std = f"{np.mean(node):.2f}", f"{np.std(node):.2f}"
 
-    return _format_width(f"{base}(μ={mean}, σ={std}, ∈{interval})", width)
+    return f"{base}(μ={mean}, σ={std}, ∈{interval})"
 
 
 @ft.lru_cache
 def _func_pprint(
     func: Callable,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     # Pretty print function
     # Example:
     #     >>> def example(a: int, b=1, *c, d, e=2, **f) -> str:
     #         ...
     #     >>> _func_pprint(example)
     #     "example(a, b, *c, d, e, **f)"
-    del indent, kind, depth
-
+    del indent, kind, depth, width
     args, varargs, varkw, _, kwonlyargs, _, _ = inspect.getfullargspec(func)
     args = (", ".join(args)) if len(args) > 0 else ""
     varargs = ("*" + varargs) if varargs is not None else ""
     kwonlyargs = (", ".join(kwonlyargs)) if len(kwonlyargs) > 0 else ""
     varkw = ("**" + varkw) if varkw is not None else ""
     name = "Lambda" if (func.__name__ == "<lambda>") else func.__name__
-    fmt = f"{name}("
-    fmt += ", ".join(item for item in [args, varargs, kwonlyargs, varkw] if item != "")
-    fmt += ")"
-    return _format_width(fmt, width)
+    text = f"{name}("
+    text += ", ".join(item for item in [args, varargs, kwonlyargs, varkw] if item != "")
+    text += ")"
+    return text
 
 
 def _list_pprint(
     node: list,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     if depth == 0:
-        fmt = "..."
-    else:
-        fmt = (f"{(_node_pprint(v,indent+1,kind,width,depth-1))}" for v in node)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
-
-    fmt = "[\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + "]"
-    return _format_width(fmt, width)
+        return "[...]"
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{(_node_pprint(v,**spec))}" for v in node)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
+    text = "[\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + "]"
+    return text
 
 
 def _tuple_pprint(
     node: tuple,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     if depth == 0:
-        fmt = "..."
-    else:
-        fmt = (f"{(_node_pprint(v,indent+1,kind,width,depth-1))}" for v in node)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
-    fmt = "(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
-    return _format_width(fmt, width)
+        return "(...)"
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{(_node_pprint(v,**spec))}" for v in node)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
+    text = "(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
+    return text
 
 
 def _set_pprint(
     node: set,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     if depth == 0:
-        fmt = "..."
-    else:
-        fmt = (f"{(_node_pprint(v,indent+1,kind,width,depth-1))}" for v in node)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
-    fmt = "{\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + "}"
-    return _format_width(fmt, width)
+        return "{...}"
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{(_node_pprint(v,**spec))}" for v in node)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
+    text = "{\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + "}"
+    return text
 
 
 def _dict_pprint(
     node: dict,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     if depth == 0:
-        fmt = "..."
-    else:
-        kvs = node.items()
-        fmt = (f"{k}:{_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
-    fmt = "{\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + "}"
-    return _format_width(fmt, width)
+        return "{...}"
+    kvs = node.items()
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{k}:{_node_pprint(v,**spec)}" for k, v in kvs)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
+    text = "{\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + "}"
+    return text
 
 
 def _namedtuple_pprint(
     node: Any,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
+    name = type(node).__name__
+
     if depth == 0:
-        fmt = "..."
-    else:
-        kvs = node._asdict().items()
-        fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
+        return f"{name}(...)"
+
+    kvs = node._asdict().items()
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
     name = type(node).__name__
-    fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
-    return _format_width(fmt, width)
+    text = f"{name}(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
+    return text
 
 
 def _dataclass_pprint(
     node: Any,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     name = type(node).__name__
 
     if depth == 0:
-        fmt = "..."
-    else:
-        kvs = ((f.name, vars(node)[f.name]) for f in dc.fields(node) if f.repr)
-        fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
+        return f"{name}(...)"
 
-    fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
-    return _format_width(fmt, width)
+    kvs = ((f.name, vars(node)[f.name]) for f in dc.fields(node) if f.repr)
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
+    text = f"{name}(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
+    return text
 
 
 def _treeclass_pprint(
     node: Any,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     name = type(node).__name__
     if depth == 0:
-        fmt = "..."
+        return f"{name}(...)"
 
-    else:
-        skip = [f.name for f in pytc.fields(node) if not f.repr]
-        kvs = ((k, v) for k, v in vars(node).items() if k not in skip)
-        fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
-        fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
-    fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
-    return _format_width(fmt, width)
+    # avoid circular import by importing Partial here
+    from pytreeclass import fields
+
+    skip = [f.name for f in fields(node) if not f.repr]
+    kvs = ((k, v) for k, v in vars(node).items() if k not in skip)
+    spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
+    text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
+    text = (", \n" + "\t" * (indent + 1)).join(text)
+    text = f"{name}(\n" + "\t" * (indent + 1) + (text) + "\n" + "\t" * (indent) + ")"
+    return text
 
 
 def _node_type_pprint(
     node: jax.Array | np.ndarray,
+    *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
 ) -> str:
     if isinstance(node, (jax.Array, np.ndarray)):
         shape_dype = node.shape, node.dtype
-        fmt = _node_pprint(jax.ShapeDtypeStruct(*shape_dype), indent, kind, width, depth)  # fmt: skip
+        spec = dict(indent=indent, kind=kind, width=width, depth=depth)
+        text = _node_pprint(jax.ShapeDtypeStruct(*shape_dype), **spec)
     else:
-        fmt = f"{type(node).__name__}"
-    return _format_width(fmt, width)
+        text = f"{type(node).__name__}"
+    return text
 
 
 def tree_repr(
     tree: PyTree,
     *,
     width: int = 80,
     tabwidth: int = 2,
@@ -319,15 +353,16 @@
 
         >>> print(pytc.tree_repr(tree, depth=1))
         {a:1, b:[...], c:{...}, f:i32[2](μ=6.50, σ=0.50, ∈[6,7])}
 
         >>> print(pytc.tree_repr(tree, depth=2))
         {a:1, b:[2, 3], c:{d:4, e:5}, f:i32[2](μ=6.50, σ=0.50, ∈[6,7])}
     """
-    return _node_pprint(tree, 0, "repr", width, depth).expandtabs(tabwidth)
+    text = _node_pprint(tree, indent=0, kind="repr", width=width, depth=depth)
+    return text.expandtabs(tabwidth)
 
 
 def tree_str(
     tree: PyTree,
     *,
     width: int = 80,
     tabwidth: int = 2,
@@ -347,18 +382,19 @@
 
         >>> print(pytc.tree_str(tree, depth=1))
         {a:1, b:[...], c:{...}, f:[6 7]}
 
         >>> print(pytc.tree_str(tree, depth=2))
         {a:1, b:[2, 3], c:{d:4, e:5}, f:[6 7]}
     """
-    return _node_pprint(tree, 0, "str", width, depth).expandtabs(tabwidth)
+    text = _node_pprint(tree, indent=0, kind="str", width=width, depth=depth)
+    return text.expandtabs(tabwidth)
 
 
-def _is_trace_leaf_depth_factory(depth: int):
+def _is_trace_leaf_depth_factory(depth: int | float):
     # generate `is_trace_leaf` function to stop tracing at a certain `depth`
     # in essence, depth is the length of the trace entry
     def is_trace_leaf(trace) -> bool:
         # trace is a tuple of (names, leaves, tracers, aux_data)
         # done like this to ensure 4-tuple unpacking
         keys, _ = trace
         # stop tracing if depth is reached
@@ -366,24 +402,22 @@
 
     return is_trace_leaf
 
 
 def tree_indent(
     tree: Any,
     *,
-    width: int = 60,
     depth: int | float = float("inf"),
-    is_leaf: Callable[[Any], bool] | None = None,
+    is_leaf: IsLeafType = None,
     tabwidth: int | None = 4,
 ):
     """Returns a string representation of the tree with indentation.
 
     Args:
         tree: The tree to be printed.
-        width: The maximum width of leaf nodes line.
         depth: The maximum depth of the tree to be printed.
         is_leaf: A function that takes a node and returns True if it is a leaf node.
         tabwidth: The number of spaces per indentation level. if `None` then tabs are not expanded.
 
     Example:
         >>> import pytreeclass as pytc
         >>> tree = [1, [2, 3], [4, [5, 6]]]
@@ -396,244 +430,178 @@
             [2]:list
                 [0]=4
                 [1]:list
                     [0]=5
                     [1]=6
 
     """
-    fmt = f"{type(tree).__name__}"
-    seen = set()
-
-    for trace, leaf in pytc.tree_leaves_with_trace(
-        tree=tree,
-        is_leaf=is_leaf,
-        is_trace_leaf=_is_trace_leaf_depth_factory(depth),
-    ):
-        keys, types = trace
-
-        for j, (key, type_) in enumerate(zip(keys, types)):
-            if (cur := (keys[: j + 1], types[: j + 1])) in seen:
-                # skip printing the common parent node twice
-                continue
-            seen.add(cur)
-
-            name = str(key)
-            fmt += "\n" + "\t" * (j + 1)
-            fmt += f"{_node_pprint(name,0,'str',width, depth )}"
-            fmt += (
-                f"={_node_pprint(leaf,indent=j+1,kind='repr',width=width, depth=depth-1)}"
-                if j == len(keys) - 1
-                else f":{type_.__name__}"
-            )
-    return fmt if tabwidth is None else fmt.expandtabs(tabwidth)
-
-
-def _group_by_depth(input: str) -> dict[int, list[list[int]]]:
-    # >>> out = """L2
-    # 	e=4
-    # 	f:L1
-    # 		c:L0
-    # 			a=1
-    # 			b=2
-    # 		d=3
-    # 	g:L0
-    # 		a=1
-    # 		b=2
-    # 	h=5"""
-    #
-    # >>> print(_group_by_depth(out))
-    # {
-    #   3:[[4, 5]],
-    #   2:[[3, 6], [8, 9]],
-    #   0:[[0]],
-    #   1:[[1, 2, 7, 10]]
-    # }
-    # in essence, the map key is the depth of the node, and the value is a list of line indices
-    # each list of line indices is a parent node with line indices of its children
-    depth_line_index_map = defaultdict(list)
-    stack_map = defaultdict(list)
-    prev_depth = 0
-    lines = input.splitlines()
-
-    for line_index, line in enumerate(lines):
-        cur_depth = len(line) - len(line.lstrip("\t"))
-        stack_map[cur_depth] += [line_index]
-        if cur_depth < prev_depth and prev_depth in stack_map:
-            depth_line_index_map[prev_depth] += [stack_map.pop(prev_depth)]
-        prev_depth = cur_depth
-
-    for key in stack_map:
-        depth_line_index_map[key] += [stack_map[key]]
-    del stack_map
-
-    return dict(depth_line_index_map)
-
-
-def _indent_to_diagram(input: str, tabwidth: int = 4) -> str:
-    # input is a string of tab \t indented text
-    # conversion alphabet
-    vmark = ("│\t")[:tabwidth]  # vertical mark
-    lmark = ("└" + "─" * (tabwidth - 2) + (" \t"))[:tabwidth]  # last mark
-    cmark = ("├" + "─" * (tabwidth - 2) + (" \t"))[:tabwidth]  # connector mark
     smark = (" \t")[:tabwidth]  # space mark
 
-    depth_line_index_map = _group_by_depth(input)
-    lines = input.splitlines()
-
-    for depth in depth_line_index_map:
-        # iterate over groups of line indices at this depth
-        for parent_lines_indices in depth_line_index_map[depth]:
-            # iterate over line indices groups
-            for i, line_index in enumerate(parent_lines_indices):
-                # iterate over line indices at a group at this depth
-                is_last = i == len(parent_lines_indices) - 1
-
-                marker = ""
-                for j in range(1, depth):
-                    max_line_index = depth_line_index_map.get(j, [[-1]])[-1][-1]
-                    marker += vmark if max_line_index > line_index else smark
+    def step(node: Node, depth: int = 0) -> str:
+        indent = smark * depth
 
-                if depth > 0:
-                    marker += lmark if is_last else cmark
+        if (len(node.children)) == 0:
+            ppspec = dict(indent=0, kind="repr", width=80, depth=0)
+            text = f"{indent}"
+            (key, _), value = node.data
+            text += f"{key}=" if key is not None else ""
+            text += _node_pprint(value, **ppspec)
+            return text + "\n"
+
+        (key, type), _ = node.data
+        text = f"{indent}"
+        text += f"{key}:" if key is not None else ""
+        text += f"{type.__name__}\n"
+
+        for child in node:
+            text += step(child, depth=depth + 1)
+        return text
 
-                lines[line_index] = marker + lines[line_index].lstrip("\t")
-
-    return "\n".join(lines).expandtabs(tabwidth)
+    root = construct_tree(
+        tree,
+        is_leaf=is_leaf,
+        is_trace_leaf=_is_trace_leaf_depth_factory(depth),
+    )
+    text = step(root)
+    return (text if tabwidth is None else text.expandtabs(tabwidth)).rstrip()
 
 
 def tree_diagram(
     tree: Any,
     *,
-    width: int = 60,
     depth: int | float = float("inf"),
-    is_leaf: Callable[[Any], bool] | None = None,
+    is_leaf: IsLeafType = None,
     tabwidth: int = 4,
 ):
     """Pretty print arbitrary PyTrees tree with tree structure diagram.
 
     Args:
         tree: PyTree
         depth: depth of the tree to print. default is max depth
-        width: max width of line. default is 60
         is_leaf: function to determine if a node is a leaf. default is None
 
     Example:
         >>> import pytreeclass as pytc
         >>> class A(pytc.TreeClass):
         ...        x: int = 10
         ...        y: int = (20,30)
         ...        z: int = 40
 
         >>> class B(pytc.TreeClass):
         ...     a: int = 10
         ...     b: tuple = (20,30, A())
 
         >>> print(pytc.tree_diagram(B(), depth=0))
-        B
+        B(...)
 
         >>> print(pytc.tree_diagram(B(), depth=1))
         B
         ├── .a=10
         └── .b=(...)
 
 
         >>> print(pytc.tree_diagram(B(), depth=2))
         B
         ├── .a=10
         └── .b:tuple
             ├── [0]=20
             ├── [1]=30
-            └── [2]=A(x=10, y=(...), z=40)
+            └── [2]=A(...)
     """
-    indent_repr = tree_indent(
+    vmark = ("│\t")[:tabwidth]  # vertical mark
+    lmark = ("└" + "─" * (tabwidth - 2) + (" \t"))[:tabwidth]  # last mark
+    cmark = ("├" + "─" * (tabwidth - 2) + (" \t"))[:tabwidth]  # connector mark
+    smark = (" \t")[:tabwidth]  # space mark
+
+    def step(
+        node: Node,
+        depth: int = 0,
+        is_last: bool = False,
+        is_lasts: tuple[bool, ...] = (),
+    ) -> str:
+        indent = "".join(smark if is_last else vmark for is_last in is_lasts[:-1])
+        branch = (lmark if is_last else cmark) if depth > 0 else ""
+
+        if (child_count := len(node.children)) == 0:
+            ppspec = dict(indent=0, kind="repr", width=80, depth=0)
+            (key, _), value = node.data
+            text = f"{indent}"
+            text += f"{branch}{key}=" if key is not None else ""
+            text += _node_pprint(value, **ppspec)
+            return text + "\n"
+
+        (key, type), _ = node.data
+
+        text = f"{indent}{branch}"
+        text += f"{key}:" if key is not None else ""
+        text += f"{type.__name__}\n"
+
+        for i, child in enumerate(node.children.values()):
+            text += step(
+                child,
+                depth=depth + 1,
+                is_last=(i == child_count - 1),
+                is_lasts=is_lasts + (i == child_count - 1,),
+            )
+        return text
+
+    root = construct_tree(
         tree,
-        width=width,
-        depth=depth,
         is_leaf=is_leaf,
-        tabwidth=None,
+        is_trace_leaf=_is_trace_leaf_depth_factory(depth),
     )
-
-    return _indent_to_diagram(indent_repr, tabwidth=tabwidth)
-
-
-def _indent_to_mermaid(input: str, tabwidth: int) -> str:
-    # input is a string of tab \t indented text
-
-    depth_line_index_map = _group_by_depth(input)
-    lines = input.splitlines()
-
-    output = "flowchart LR\n"
-
-    for depth in depth_line_index_map:
-        # iterate over groups of line indices at this depth
-        for parent_lines_indices in depth_line_index_map[depth]:
-            # iterate over line indices groups
-            for line_index in parent_lines_indices:
-                if depth == 0:
-                    line = "<b>" + lines[line_index].lstrip("\t") + "</b>"
-                    output += f"\tid{line_index}({line})\n"
-
-                else:
-                    # get the line indices of the previous depth (parent nodes)
-                    parent_lines = chain.from_iterable(depth_line_index_map[depth - 1])
-                    parent_line_index = [x for x in parent_lines if x < line_index][-1]
-                    line = "</b>" + lines[line_index].lstrip("\t") + "</b>"
-                    output += f'\tid{parent_line_index} --- id{line_index}("{line}")\n'
-    return output.expandtabs(tabwidth)
+    text = step(root, is_last=len(root.children) == 1)
+    return (text if tabwidth is None else text.expandtabs(tabwidth)).rstrip()
 
 
 def tree_mermaid(
     tree: PyTree,
-    width: int = 60,
     depth: int | float = float("inf"),
-    is_leaf: Callable[[Any], bool] | None = None,
+    is_leaf: IsLeafType = None,
+    tabwidth: int | None = 4,
 ) -> str:
-    # def _generate_mermaid_link(mermaid_string: str) -> str:
-    #     """generate a one-time link mermaid diagram"""
-    #     url_val = "https://pytreeclass.herokuapp.com/generateTemp"
-    #     request = requests.post(url_val, json={"description": mermaid_string})
-    #     generated_id = request.json()["id"]
-    #     generated_html = f"https://pytreeclass.herokuapp.com/temp/?id={generated_id}"
-    #     return f"Open URL in browser: {generated_html}"
-
     """generate a mermaid diagram syntax for arbitrary PyTrees.
 
-
     Args:
         tree: PyTree
-        width: max width of line. default is 60
         depth: depth of the tree to print. default is max depth
         is_leaf: function to determine if a node is a leaf. default is None
-
-    Example:
-        >>> import pytreeclass as pytc
-        >>> tree = [1, [2, 3], [4, [5, 6]]]
-        >>> print(pytc.tree_mermaid(tree, depth=1))  # doctest: +SKIP
-        flowchart LR
-            id2 --- id3("</b>[0]=2</b>")
-            id2 --- id4("</b>[1]=3</b>")
-            id5 --- id6("</b>[0]=4</b>")
-            id5 --- id7("</b>[1]:list</b>")
-            id0(<b>list</b>)
-            id0 --- id1("</b>[0]=1</b>")
-            id0 --- id2("</b>[1]:list</b>")
-            id0 --- id5("</b>[2]:list</b>")
-            id7 --- id8("</b>[0]=5</b>")
-            id7 --- id9("</b>[1]=6</b>")
     """
 
-    indent_repr = tree_indent(
+    def step(node: Node, depth: int = 0) -> str:
+        if len(node.children) == 0:
+            ppspec = dict(indent=0, kind="repr", width=80, depth=0)
+            key, _, value = node.data
+            text = f"{key}=" if key is not None else ""
+            text += _node_pprint(value, **ppspec)
+            text = "<b>" + text + "</b>"
+            return f'\tid{id(node.parent)} --- id{id(node)}("{text}")\n'
+
+        key, type, _ = node.data
+        text = f"{key}:" if key is not None else ""
+        text += f"{type.__name__}"
+        text = "<b>" + text + "</b>"
+
+        if node.parent is None:
+            text = f'\tid{id(node)}("{text}")\n'
+        else:
+            text = f'\tid{id(node.parent)} --- id{id(node)}("{text}")\n'
+
+        for child in node.children.values():
+            text += step(child, depth=depth + 1)
+        return text
+
+    root = construct_tree(
         tree,
-        width=width,
-        depth=depth,
         is_leaf=is_leaf,
-        tabwidth=None,
+        is_trace_leaf=_is_trace_leaf_depth_factory(depth),
     )
+    text = "flowchart LR\n" + step(root)
 
-    return _indent_to_mermaid(indent_repr, tabwidth=4)
+    return (text.expandtabs(tabwidth) if tabwidth is not None else text).rstrip()
 
 
 def _format_width(string, width=60):
     """strip newline/tab characters if less than max width"""
     children_length = len(string) - string.count("\n") - string.count("\t")
     if children_length > width:
         return string
@@ -679,34 +647,40 @@
     #     │a  │
     #     ├───┤
     #     │   │
     #     ├───┤
     #     │a  │
     #     └───┘
 
-    max_width = (max(chain.from_iterable([[len(t) for t in item.split("\n")] for item in text])) + 0)  # fmt: skip
+    max_width = (
+        max(from_iterable([[len(t) for t in item.split("\n")] for item in text])) + 0
+    )
 
     top = f"┌{'─'*max_width}┐"
     line = f"├{'─'*max_width}┤"
-    side = ["\n".join([f"│{t}{' '*(max_width-len(t))}│" for t in item.split("\n")]) for item in text]  # fmt: skip
+    side = [
+        "\n".join([f"│{t}{' '*(max_width-len(t))}│" for t in item.split("\n")])
+        for item in text
+    ]
+
     btm = f"└{'─'*max_width}┘"
 
-    fmt = ""
+    text = ""
 
     for i, s in enumerate(side):
         if i == 0:
-            fmt += f"{top}\n{s}\n{line if len(side)>1 else btm}"
+            text += f"{top}\n{s}\n{line if len(side)>1 else btm}"
 
         elif i == len(side) - 1:
-            fmt += f"\n{s}\n{btm}"
+            text += f"\n{s}\n{btm}"
 
         else:
-            fmt += f"\n{s}\n{line}"
+            text += f"\n{s}\n{line}"
 
-    return fmt
+    return text
 
 
 def _hstack(*boxes):
     # Create horizontally stacked text boxes
     # Example:
     #     >>> print(_hstack(_hbox("a"),_vbox("b","c")))
     #     ┌─┬─┐
@@ -715,22 +689,22 @@
     #       │c│
     #       └─┘
 
     boxes = [(box).split("\n") for box in boxes]
     max_col_height = max([len(b) for b in boxes])
     # expand height of each col before merging
     boxes = [b + [" " * len(b[0])] * (max_col_height - len(b)) for b in boxes]
-    FMT = ""
+    text = ""
 
     _cells = tuple(zip(*boxes))
 
     for i, line in enumerate(_cells):
-        FMT += _resolve_line(line) + ("\n" if i != (len(_cells) - 1) else "")
+        text += _resolve_line(line) + ("\n" if i != (len(_cells) - 1) else "")
 
-    return FMT
+    return text
 
 
 def _resolve_line(cols: list[str]) -> str:
     # Combine columns of single line by merging their borders
 
     # Args:
     #     cols (Sequence[str,...]): Sequence of single line column string
@@ -805,32 +779,33 @@
     return _hstack(*(_vbox(*col) for col in cols))
 
 
 def tree_summary(
     tree: PyTree,
     *,
     depth: int | float = float("inf"),
-    is_leaf: Callable[[Any], bool] | None = None,
+    is_leaf: IsLeafType = None,
 ) -> str:
     """Print a summary of an arbitrary PyTree.
 
     Args:
-        tree: pytree to summarize (ex. list, tuple, dict, dataclass, jax.numpy.ndarray)
-        depth: max depth to traverse the tree. defaults to maximum depth = float("inf")
+        tree: a jax registered pytree to summarize.
+        depth: max depth to traverse the tree. defaults to maximum depth.
         is_leaf: function to determine if a node is a leaf. defaults to None
 
     Returns:
         String summary of the tree structure
-        - First column: is the path to the node
-        - Second column: is the type of the node
-        - Third column: is the number of leaves in the node (1 for non-array leaves and array size for array leaves)
+        - First column: path to the node
+        - Second column: type of the node
+        - Third column: number of leaves in the node
         - Last row: type of parent, number of leaves and size of parent
 
     Note:
-        Array elements are considered as leaves, for example `jnp.array([1,2,3])` has 3 leaves
+        Array elements are considered as leaves, for example:
+        `jnp.array([1,2,3])` has 3 leaves
 
     Example:
         >>> import pytreeclass as pytc
         >>> print(pytc.tree_summary([1,[2,[3]]]))
         ┌─────────┬────┬─────┐
         │Name     │Type│Count│
         ├─────────┼────┼─────┤
@@ -845,15 +820,15 @@
     """
     ROWS = [["Name", "Type", "Count"]]
     COUNT = 0
 
     # use `unzip2` from `jax.util` to avoid [] leaves
     # based on this issue:
     traces, leaves = unzip2(
-        pytc.tree_leaves_with_trace(
+        tree_leaves_with_trace(
             tree,
             is_leaf=is_leaf,
             is_trace_leaf=_is_trace_leaf_depth_factory(depth),
         )
     )
 
     for trace, leaf in zip(traces, leaves):
@@ -876,69 +851,67 @@
     ROWS += [[paths, types, counts]]
 
     return _table(ROWS)
 
 
 def tree_repr_with_trace(
     tree: PyTree,
-    is_leaf: Callable[[Any], bool] | None = None,
+    is_leaf: IsLeafType = None,
     transpose: bool = False,
 ) -> PyTree:
-    """Return a PyTree with the same structure, but with the leaves replaced by a summary of the trace.
+    """
+    Return a PyTree with the same structure, but with the leaves replaced
+    by a summary of the trace.
 
     Args:
         tree: pytree to summarize.
         is_leaf: function to determine if a node is a leaf. defaults to None
         transpose: transpose the table. i.e. rows become cols and cols become rows
 
     Example:
         >>> import pytreeclass as pytc
         >>> class Test(pytc.TreeClass):
         ...    a:int = 1
         ...    b:float = 2.0
 
         >>> tree = Test()
-        >>> print(pytc.tree_repr_with_trace(Test()))  # doctest: +SKIP
+        >>> print(pytc.tree_repr_with_trace(Test()))  # doctest: +NORMALIZE_WHITESPACE
         Test(
           a=
-            ┌──────────┬───┐
-            │Value     │1  │
-            ├──────────┼───┤
-            │Name path │a  │
-            ├──────────┼───┤
-            │Type path │int│
-            ├──────────┼───┤
-            │Index path│0  │
-            └──────────┴───┘,
+            ┌─────────┬───┐
+            │Value    │1  │
+            ├─────────┼───┤
+            │Name path│.a │
+            ├─────────┼───┤
+            │Type path│int│
+            └─────────┴───┘,
           b=
-            ┌──────────┬─────┐
-            │Value     │2.0  │
-            ├──────────┼─────┤
-            │Name path │b    │
-            ├──────────┼─────┤
-            │Type path │float│
-            ├──────────┼─────┤
-            │Index path│1    │
-            └──────────┴─────┘
+            ┌─────────┬─────┐
+            │Value    │2.0  │
+            ├─────────┼─────┤
+            │Name path│.b   │
+            ├─────────┼─────┤
+            │Type path│float│
+            └─────────┴─────┘
         )
 
-        >>> print(pytc.tree_repr_with_trace(Test(), transpose=True))  # doctest: +SKIP
+        >>> print(pytc.tree_repr_with_trace(Test(), transpose=True)) # doctest: +NORMALIZE_WHITESPACE
         Test(
-        a=
-            ┌─────┬─────────┬─────────┬──────────┐
-            │Value│Name path│Type path│Index path│
-            ├─────┼─────────┼─────────┼──────────┤
-            │1    │a        │int      │0         │
-            └─────┴─────────┴─────────┴──────────┘,
-        b=
-            ┌─────┬─────────┬─────────┬──────────┐
-            │Value│Name path│Type path│Index path│
-            ├─────┼─────────┼─────────┼──────────┤
-            │2.0  │b        │float    │1         │
-            └─────┴─────────┴─────────┴──────────┘
+          a=
+            ┌─────┬─────────┬─────────┐
+            │Value│Name path│Type path│
+            ├─────┼─────────┼─────────┤
+            │1    │.a       │int      │
+            └─────┴─────────┴─────────┘,
+          b=
+            ┌─────┬─────────┬─────────┐
+            │Value│Name path│Type path│
+            ├─────┼─────────┼─────────┤
+            │2.0  │.b       │float    │
+            └─────┴─────────┴─────────┘
         )
 
     Note:
         This function can be useful for debugging and raising descriptive errors.
     """
 
     def leaf_trace_summary(trace, leaf) -> str:
@@ -951,8 +924,8 @@
 
         types = "->".join(i.__name__ for i in trace[1])
         ROWS += [["Type path", types]]
 
         # make a pretty table for each leaf
         return _table(ROWS, transpose=transpose)
 
-    return pytc.tree_map_with_trace(leaf_trace_summary, tree, is_leaf=is_leaf)
+    return tree_map_with_trace(leaf_trace_summary, tree, is_leaf=is_leaf)
```

### Comparing `pytreeclass-0.3.3/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.4/pytreeclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.3
+Version: 0.3.4
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -904,9 +904,10 @@
 </table>
 
 </details>
 
 ## 📙 Acknowledgements<a id="acknowledgements"></a>
 
 - [Farid Talibli (for visualization link generation backend)](https://www.linkedin.com/in/frdt98)
+- [Lenses](https://hackage.haskell.org/package/lens)
 - [Treex](https://github.com/cgarciae/treex), [Equinox](https://github.com/patrick-kidger/equinox), [tree-math](https://github.com/google/tree-math), [Flax](https://github.com/google/flax), [TensorFlow](https://www.tensorflow.org), [PyTorch](https://pytorch.org)
 - [Lovely JAX](https://github.com/xl0/lovely-jax)
```

### Comparing `pytreeclass-0.3.3/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.4/pytreeclass.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 pytreeclass.egg-info/PKG-INFO
 pytreeclass.egg-info/SOURCES.txt
 pytreeclass.egg-info/dependency_links.txt
 pytreeclass.egg-info/not-zip-safe
 pytreeclass.egg-info/requires.txt
 pytreeclass.egg-info/top_level.txt
 pytreeclass/_src/__init__.py
-pytreeclass/_src/tree_decorator.py
-pytreeclass/_src/tree_freeze.py
-pytreeclass/_src/tree_indexer.py
+pytreeclass/_src/code_build.py
+pytreeclass/_src/tree_base.py
 pytreeclass/_src/tree_pprint.py
-pytreeclass/_src/tree_trace.py
+pytreeclass/_src/tree_util.py
 tests/__init__.py
 tests/test_indexing.py
 tests/test_nn.py
 tests/test_tree_freeze.py
 tests/test_tree_operator.py
 tests/test_tree_pprint.py
 tests/test_tree_viz_util.py
```

### Comparing `pytreeclass-0.3.3/setup.py` & `pytreeclass-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.3/tests/test_indexing.py` & `pytreeclass-0.3.4/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass import TreeClass
-from pytreeclass._src.tree_indexer import _mutable_context
+from pytreeclass._src.tree_base import _mutable_context
+from pytreeclass._src.tree_util import construct_tree
 
 
 class Tree(TreeClass, leafwise=True):
     a: float
     b: float
     c: float
     d: jnp.ndarray
@@ -675,7 +676,16 @@
 
     class Tree(pytc.TreeClass, leafwise=True):
         a: Any = (1, {"b": Dict({"c": 1})})
 
     tree = Tree()
     assert jtu.tree_leaves(tree.at["a"].at[1].at["b"].get())[0] == Dict({"c": 1})
     assert jtu.tree_leaves(tree.at[0].at[1].at["b"].get())[0] == Dict({"c": 1})
+
+
+def test_construct_tree():
+    tree = construct_tree([1, 2, [3, 4]])
+
+    assert repr(tree) == "Node(data=((None, <class 'list'>), None))"
+
+    with pytest.raises(TypeError):
+        tree.add_child("a")
```

### Comparing `pytreeclass-0.3.3/tests/test_nn.py` & `pytreeclass-0.3.4/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.3/tests/test_tree_freeze.py` & `pytreeclass-0.3.4/tests/test_tree_freeze.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
-from pytreeclass._src.tree_freeze import _HashableWrapper, tree_hash
+from pytreeclass._src.tree_util import _HashableWrapper, tree_hash
 
 
 def test_freeze_unfreeze():
     class A(pytc.TreeClass, leafwise=True):
         a: int
         b: int
```

### Comparing `pytreeclass-0.3.3/tests/test_tree_operator.py` & `pytreeclass-0.3.4/tests/test_tree_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import math
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
 import pytreeclass as pytc
-from pytreeclass._src.tree_freeze import _hash_node
-from pytreeclass._src.tree_indexer import bcmap
+from pytreeclass._src.tree_util import _hash_node, bcmap
 
 
 def test_bcmap():
     class Test(pytc.TreeClass, leafwise=True):
         a: tuple[int]
         b: tuple[int]
         c: jnp.ndarray
```

### Comparing `pytreeclass-0.3.3/tests/test_tree_pprint.py` & `pytreeclass-0.3.4/tests/test_tree_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 
 def _tree_to_indent(str):
     return str.replace("├── ", "    ").replace("└── ", "    ").replace("│", " ")
 
 
 def test_tree_diagram():
-    assert tree_diagram(r1, depth=0) == tree_indent(r1, depth=0) == "Repr1"
+    assert tree_diagram(r1, depth=0) == tree_indent(r1, depth=0) == "Repr1(...)"
 
     # trunk-ignore(flake8/E501)
     out = "Repr1\n├── .a=1\n├── .b='string'\n├── .c=1.0\n├── .d='aaaaa'\n├── .e=[...]\n├── .f={...}\n├── .g={...}\n├── .h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .k=(...)\n├── .l=a(...)\n├── .m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .n=bool[]\n└── .o=c64[2]"
 
     assert tree_diagram(r1, depth=1) == out
     assert tree_indent(r1, depth=1) == _tree_to_indent(out)
 
@@ -142,24 +142,25 @@
         == "┌───────┬────┬─────┐\n│Name   │Type│Count│\n├───────┼────┼─────┤\n│.leaf_0│int │1    │\n├───────┼────┼─────┤\n│.leaf_1│int │1    │\n├───────┼────┼─────┤\n│Σ      │Test│2    │\n└───────┴────┴─────┘"
     )
 
     assert tree_repr(Test) == repr(Test)
     assert tree_str(Test) == str(Test)
 
 
+@pytest.mark.skip(reason="depends on object id")
 def test_tree_mermaid():
     assert (
         tree_mermaid(r1, depth=1)
         # trunk-ignore(flake8/E501)
         == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e=[...]</b>")\n    id0 --- id6("</b>.f={...}</b>")\n    id0 --- id7("</b>.g={...}</b>")\n    id0 --- id8("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>.k=(...)</b>")\n    id0 --- id12("</b>.l=a(...)</b>")\n    id0 --- id13("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>.n=bool[]</b>")\n    id0 --- id15("</b>.o=c64[2]</b>")\n'
     )
     assert (
         tree_mermaid(r1, depth=2)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>.b=1</b>")\n    id23 --- id25("</b>.c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e:list</b>")\n    id0 --- id11("</b>.f={1, 2, 3}</b>")\n    id0 --- id12("</b>.g:dict</b>")\n    id0 --- id16("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>.k:tuple</b>")\n    id0 --- id23("</b>.l:a</b>")\n    id0 --- id26("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>.n=bool[]</b>")\n    id0 --- id28("</b>.o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>.b=1</b>")\n    id23 --- id25("</b>.c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e:list</b>")\n    id0 --- id11("</b>.f={...}</b>")\n    id0 --- id12("</b>.g:dict</b>")\n    id0 --- id16("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>.k:tuple</b>")\n    id0 --- id23("</b>.l:a</b>")\n    id0 --- id26("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>.n=bool[]</b>")\n    id0 --- id28("</b>.o=c64[2]</b>")\n'
     )
 
 
 def test_misc():
     x = (1, 2, 3)
     assert tree_repr(x) == tree_str(x) == "(1, 2, 3)"
```

### Comparing `pytreeclass-0.3.3/tests/test_tree_viz_util.py` & `pytreeclass-0.3.4/tests/test_tree_viz_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import jax
+import jax.nn.initializers as ji
 import jax.tree_util as jtu
 
 from pytreeclass._src.tree_pprint import (
     _func_pprint,
     _hbox,
     _hstack,
     _node_pprint,
@@ -36,24 +37,36 @@
     assert _hstack(_hbox("a"), _vbox("b", "c")) == "┌─┬─┐\n│a│b│\n└─┼─┤\n  │c│\n  └─┘"
 
 
 def test_func_pprint():
     def example(a: int, b=1, *c, d, e=2, **f) -> str:
         ...  # fmt: skip
 
-    assert _func_pprint(example, 0, "str", 60, 0) == "example(a, b, *c, d, e, **f)"
-    assert _func_pprint(lambda x: x, 0, "str", 60, 0) == "Lambda(x)"
-    assert _func_pprint(jax.nn.relu, 0, "str", 60, 0) == "relu(*args, **kwargs)"
     assert (
-        _node_pprint(jtu.Partial(jax.nn.relu), 0, "str", 60, 0)
+        _func_pprint(example, indent=0, kind="str", width=60, depth=0)
+        == "example(a, b, *c, d, e, **f)"
+    )
+    assert (
+        _func_pprint(lambda x: x, indent=0, kind="str", width=60, depth=0)
+        == "Lambda(x)"
+    )
+    assert (
+        _func_pprint(jax.nn.relu, indent=0, kind="str", width=60, depth=0)
+        == "relu(*args, **kwargs)"
+    )
+    assert (
+        _node_pprint(jtu.Partial(jax.nn.relu), indent=0, kind="str", width=60, depth=0)
         == "Partial(relu(*args, **kwargs))"
     )
     assert (
-        _node_pprint(jtu.Partial(jax.nn.relu), 0, "str", 60, 0)
+        _node_pprint(jtu.Partial(jax.nn.relu), indent=0, kind="str", width=60, depth=0)
         == "Partial(relu(*args, **kwargs))"
     )
     assert (
-        _func_pprint(jax.nn.initializers.he_normal, 0, "str", 60, 0)
+        _func_pprint(ji.he_normal, indent=0, kind="str", width=60, depth=0)
         == "he_normal(in_axis, out_axis, batch_axis, dtype)"
     )
 
-    assert _node_pprint(jax.jit(lambda x: x), 0, "repr", 60, 0) == "jit(Lambda(x))"
+    assert (
+        _node_pprint(jax.jit(lambda x: x), indent=0, kind="repr", width=60, depth=0)
+        == "jit(Lambda(x))"
+    )
```

### Comparing `pytreeclass-0.3.3/tests/test_treeclass.py` & `pytreeclass-0.3.4/tests/test_treeclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,14 @@
     tree = Tree(name="test")
     assert tree._name == "test"
 
     with pytest.raises(TypeError):
         pytc.field(alias=1)
 
 
-def test_field_hash():
-    f1 = pytc.field(default=1.0, callbacks=[lambda x: x])
-    f2 = pytc.field(default=1.0)
-    hash(f1) == hash(f2)
-
-
 def test_field_nondiff():
     class Test(pytc.TreeClass):
         a: jax.Array
         b: jax.Array
 
         def __init__(
             self,
```

### Comparing `pytreeclass-0.3.3/tests/test_under_jit.py` & `pytreeclass-0.3.4/tests/test_under_jit.py`

 * *Files identical despite different names*

