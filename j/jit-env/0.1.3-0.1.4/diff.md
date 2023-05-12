# Comparing `tmp/jit_env-0.1.3.tar.gz` & `tmp/jit_env-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jit_env-0.1.3.tar", last modified: Tue Apr 25 14:22:23 2023, max compression
+gzip compressed data, was "dist/jit_env-0.1.4.tar", last modified: Fri May 12 13:31:40 2023, max compression
```

## Comparing `jit_env-0.1.3.tar` & `jit_env-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-25 14:22:22.708681 jit_env-0.1.3/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.3/LICENSE
--rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.3/MANIFEST.in
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-25 14:22:22.701198 jit_env-0.1.3/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-25 14:21:51.000000 jit_env-0.1.3/README.md
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-25 14:22:22.591823 jit_env-0.1.3/jit_env/
--rwxrwxrwx   0 joery     (1000) joery     (1000)      772 2023-04-25 14:18:00.000000 jit_env-0.1.3/jit_env/__init__.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.3/jit_env/_compat_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    14702 2023-04-15 05:34:34.000000 jit_env-0.1.3/jit_env/_core.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.3/jit_env/_core_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.3/jit_env/_specs_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    15327 2023-04-25 14:18:00.000000 jit_env-0.1.3/jit_env/_wrappers_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.3/jit_env/compat.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.3/jit_env/py.typed
--rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.3/jit_env/specs.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-25 14:21:51.000000 jit_env-0.1.3/jit_env/version.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    14574 2023-04-25 14:18:00.000000 jit_env-0.1.3/jit_env/wrappers.py
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-25 14:22:22.685574 jit_env-0.1.3/jit_env.egg-info/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/SOURCES.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/dependency_links.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/requires.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-25 14:22:21.000000 jit_env-0.1.3/jit_env.egg-info/top_level.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.3/requirements.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.3/requirements_dev.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-25 14:22:22.709193 jit_env-0.1.3/setup.cfg
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.3/setup.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-05-12 13:31:40.649218 jit_env-0.1.4/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.4/LICENSE
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5676 2023-05-12 13:31:40.649218 jit_env-0.1.4/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4892 2023-05-12 13:29:10.000000 jit_env-0.1.4/README.md
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-05-12 13:31:40.539011 jit_env-0.1.4/jit_env/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      772 2023-04-25 14:18:00.000000 jit_env-0.1.4/jit_env/__init__.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    11454 2023-05-12 13:18:58.000000 jit_env-0.1.4/jit_env/_compat_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14702 2023-04-15 05:34:34.000000 jit_env-0.1.4/jit_env/_core.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.4/jit_env/_core_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    18967 2023-05-12 13:22:05.000000 jit_env-0.1.4/jit_env/_specs_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    15327 2023-04-25 14:18:00.000000 jit_env-0.1.4/jit_env/_wrappers_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     8889 2023-05-12 13:20:35.000000 jit_env-0.1.4/jit_env/compat.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.4/jit_env/py.typed
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    24006 2023-05-12 13:07:51.000000 jit_env-0.1.4/jit_env/specs.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-05-12 13:29:10.000000 jit_env-0.1.4/jit_env/version.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14574 2023-04-25 14:18:00.000000 jit_env-0.1.4/jit_env/wrappers.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-05-12 13:31:40.617961 jit_env-0.1.4/jit_env.egg-info/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5676 2023-05-12 13:31:39.000000 jit_env-0.1.4/jit_env.egg-info/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-05-12 13:31:39.000000 jit_env-0.1.4/jit_env.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-05-12 13:31:39.000000 jit_env-0.1.4/jit_env.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      175 2023-05-12 13:31:39.000000 jit_env-0.1.4/jit_env.egg-info/requires.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-05-12 13:31:39.000000 jit_env-0.1.4/jit_env.egg-info/top_level.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.4/requirements.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      134 2023-05-10 11:59:26.000000 jit_env-0.1.4/requirements_dev.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-05-12 13:31:40.649218 jit_env-0.1.4/setup.cfg
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.4/setup.py
```

### Comparing `jit_env-0.1.3/LICENSE` & `jit_env-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.3/PKG-INFO` & `jit_env-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jit_env
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.3-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.4-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
 
@@ -41,15 +41,15 @@
 
 Note that this module is only an interface and does not implement any
 Environments itself. The implementations in `examples` serve to illustrate the syntax.
 For a more thorough review of the semantics, please refer to the [dm-env](https://github.com/deepmind/dm_env/blob/master/dm_env/specs.py) 
 wiki and compare our implementation of `jit_env.Environment` with `dm_env.Environment` and the conversion as given in [`compat.py`](https://github.com/joeryjoery/jit_env/blob/main/jit_env/compat.py).
 
 ## Installation
-`jit_env` can be installed with:
+`jit_env` can be installed with (it is recommended to install `jax` first):
 
 `python -m pip install jit-env`
 
 You can also install it directly from our GitHub repository using pip:
 
 `python -m pip install git+git://github.com/joeryjoery/jit_env.git`
 
@@ -99,7 +99,8 @@
 ```
 
 ## References
 This library was heavily inspired by the following libraries:
 - dm-env: [https://github.com/deepmind/dm_env](https://github.com/deepmind/dm_env)
 - jumanji: [https://github.com/instadeepai/jumanji](https://github.com/instadeepai/jumanji)
 - gymnax: [https://github.com/RobertTLange/gymnax](https://github.com/RobertTLange/gymnax)
+- gymnasium: [https://github.com/Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium)
```

### Comparing `jit_env-0.1.3/README.md` & `jit_env-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.3-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.4-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
 
@@ -20,15 +20,15 @@
 
 Note that this module is only an interface and does not implement any
 Environments itself. The implementations in `examples` serve to illustrate the syntax.
 For a more thorough review of the semantics, please refer to the [dm-env](https://github.com/deepmind/dm_env/blob/master/dm_env/specs.py) 
 wiki and compare our implementation of `jit_env.Environment` with `dm_env.Environment` and the conversion as given in [`compat.py`](https://github.com/joeryjoery/jit_env/blob/main/jit_env/compat.py).
 
 ## Installation
-`jit_env` can be installed with:
+`jit_env` can be installed with (it is recommended to install `jax` first):
 
 `python -m pip install jit-env`
 
 You can also install it directly from our GitHub repository using pip:
 
 `python -m pip install git+git://github.com/joeryjoery/jit_env.git`
 
@@ -78,7 +78,8 @@
 ```
 
 ## References
 This library was heavily inspired by the following libraries:
 - dm-env: [https://github.com/deepmind/dm_env](https://github.com/deepmind/dm_env)
 - jumanji: [https://github.com/instadeepai/jumanji](https://github.com/instadeepai/jumanji)
 - gymnax: [https://github.com/RobertTLange/gymnax](https://github.com/RobertTLange/gymnax)
+- gymnasium: [https://github.com/Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium)
```

### Comparing `jit_env-0.1.3/jit_env/__init__.py` & `jit_env-0.1.4/jit_env/__init__.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.3/jit_env/_core.py` & `jit_env-0.1.4/jit_env/_core.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.3/jit_env/_core_test.py` & `jit_env-0.1.4/jit_env/_core_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.3/jit_env/_specs_test.py` & `jit_env-0.1.4/jit_env/_specs_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pickle
 
 import chex
 
 import jax
 from jax import numpy as jnp
 
+from jaxtyping import PyTree
+
 from jit_env import specs
 
 INT_SIZE: int = 3
 BATCH_SIZE: int = 2
 
 VEC_MIN: float = 0.0
 VEC_MAX: float = 1.0
@@ -106,14 +108,85 @@
 
     _ = jax.tree_map(check_spec, env_spec.rewards, r)
     _ = jax.tree_map(check_spec, env_spec.observations, o)
     _ = jax.tree_map(check_spec, env_spec.discounts, d)
     _ = jax.tree_map(check_spec, env_spec.actions, a)
 
 
+@pytest.mark.parametrize(
+    'in_spec, expected_tree', [
+        (
+                specs.Tuple(
+                    specs.Tuple(
+                        specs.Tuple(
+                            specs.Array((), jnp.float32)
+                        )
+                    )
+                ),
+                (((specs.Array((), jnp.float32),),),)
+        ),
+        (
+                specs.Dict(
+                    a=specs.Tuple(
+                        specs.DiscreteArray(5)
+                    ),
+                    b=specs.Tree(
+                        leaves=[
+                            specs.Array((), jnp.float32),
+                            specs.DiscreteArray(10)
+                        ],
+                        structure=jax.tree_util.tree_structure((0, dict(c=0)))
+                    )
+                ),
+                dict(
+                    a=(specs.DiscreteArray(5),),
+                    b=(specs.Array((), jnp.float32), dict(
+                        c=specs.DiscreteArray(10)
+                    ))
+                )
+        ),
+        (
+                specs.Tree(
+                    leaves=[
+                        specs.Array((), jnp.float32),
+                        specs.DiscreteArray(5),
+                        specs.DiscreteArray(10),
+                    ],
+                    structure=jax.tree_util.tree_structure(
+                        (0, dict(a=dict(b=(0, [0]))))
+                    )
+                ),
+                (specs.Array((), jnp.float32), dict(a=dict(
+                    b=(specs.DiscreteArray(5), [specs.DiscreteArray(10)])
+                )))
+        )
+
+    ]
+)
+def test_unpack_spec(in_spec: specs.Spec, expected_tree: PyTree[specs.Spec]):
+    unpacked = specs.unpack_spec(in_spec)
+    chex.assert_trees_all_equal_structs(unpacked, expected_tree)
+
+    sample_normal = in_spec.generate_value()
+    sample_tree = jax.tree_map(lambda s: s.generate_value(), unpacked)
+    sample_spec = specs.unpack_spec(
+        jax.tree_map(lambda s: s.generate_value(), in_spec)
+    )
+
+    in_spec.validate(sample_tree)
+    in_spec.validate(sample_spec)
+
+    chex.assert_trees_all_equal_shapes_and_dtypes(
+        sample_normal, sample_tree, ignore_nones=True
+    )
+    chex.assert_trees_all_equal_shapes_and_dtypes(
+        sample_normal, sample_spec, ignore_nones=True
+    )
+
+
 class TestTree:
 
     def test_serialize(self, tree_spec):
         reconstructed = pickle.loads(pickle.dumps(tree_spec))
 
         assert isinstance(reconstructed, tree_spec.__class__)
 
@@ -243,17 +316,18 @@
     def test_empty_batch(self, int_spec):
         with pytest.raises(ValueError):
             _ = specs.Batched(int_spec, 0)
 
     def test_struct(self, batch_spec: specs.Batched):
         out_dict = batch_spec.generate_value()
 
-        batched_specs = batch_spec.as_spec_struct()
+        unpacked = batch_spec.as_spec_struct()
         new_dict = jax.tree_map(
-            lambda s: s.generate_value(), batched_specs
+            lambda s: s.generate_value(), unpacked,
+            is_leaf=lambda s: isinstance(s, specs.CompositeSpec)
         )
 
         chex.assert_trees_all_equal(out_dict, new_dict)
         chex.assert_trees_all_equal_shapes_and_dtypes(out_dict, new_dict)
 
 
 class TestArray:
```

### Comparing `jit_env-0.1.3/jit_env/_wrappers_test.py` & `jit_env-0.1.4/jit_env/_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.3/jit_env/specs.py` & `jit_env-0.1.4/jit_env/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             name: Explicit string name for the array specification.
         """
         super().__init__(name)
         self._shape = tuple(shape)
         self._dtype = _jnp.zeros((), dtype).dtype  # get uniform `dtype` type
 
     @property
-    def shape(self) -> int | _typing.Sequence[int]:
+    def shape(self) -> _typing.Sequence[int]:
         return self._shape
 
     @property
     def dtype(self) -> _typing.Any:
         return self._dtype
 
 
@@ -453,26 +453,28 @@
         """Return the unflattend Spec PyTree as is."""
         return _tree_util.tree_unflatten(self.treedef, self.leave_specs)
 
     def validate(
             self,
             value: _jxtype.PyTree[_jxtype.ArrayLike | None]
     ) -> _jxtype.PyTree[_jxtype.ArrayLike | None]:
-        return _jax.tree_map(
-            lambda s, v: s.validate(v),
-            self.as_spec_struct(), value
-        )
+        leaf_values = self.treedef.flatten_up_to(value)
+        leaf_validated = [
+            s.validate(v) for s, v in zip(self.leave_specs, leaf_values)
+        ]
+        return self.treedef.unflatten(leaf_validated)
 
     def generate_value(
             self
     ) -> _jxtype.PyTree[_jxtype.Num[_jxtype.Array, '...'] | None]:
         values = [s.generate_value() for s in self.leave_specs]
         return _tree_util.tree_unflatten(self.treedef, values)
 
 
+@_tree_util.register_pytree_node_class
 class Tuple(Tree):
     """Overrides Tree as a Tuple PyTree Structure."""
     __slots__ = ()
 
     def __init__(self, *var_specs: Spec, name: str = ""):
         """Initializes a new `Tuple` spec.
 
@@ -486,19 +488,28 @@
             ValueError: If no specs are provided.
         """
         if not var_specs:
             raise ValueError("Cannot initialize an empty Spec")
 
         super().__init__(
             list(var_specs),
-            _tree_util.tree_structure(var_specs),
+            _tree_util.tree_structure((0,) * len(var_specs)),
             name
         )
 
+    @classmethod
+    def tree_unflatten(
+            cls: _typing.Type[Tuple],
+            aux: tuple[_tree_util.PyTreeDef, str],
+            children: _typing.Sequence[Spec]
+    ) -> Tuple:
+        return cls(*children, name=aux[-1])
+
 
+@_tree_util.register_pytree_node_class
 class Dict(Tree):
     """Overrides Tree as a Dictionary PyTree Structure."""
     __slots__ = ()
 
     def __init__(
             self,
             dict_spec: dict[str, Spec] | None = None,
@@ -527,18 +538,27 @@
         full_spec = dict_spec | kwarg_specs
 
         if not full_spec:
             raise ValueError("Cannot initialize an empty Spec")
 
         super().__init__(
             list(full_spec.values()),
-            _tree_util.tree_structure(full_spec),
+            _tree_util.tree_structure({k: 0 for k in full_spec.keys()}),
             name=name
         )
 
+    @classmethod
+    def tree_unflatten(
+            cls: _typing.Type[Dict],
+            aux: tuple[_tree_util.PyTreeDef, str],
+            children: _typing.Sequence[Spec]
+    ) -> Dict:
+        tree_dict = _jax.tree_util.tree_unflatten(aux[0], children)
+        return cls(tree_dict, name=aux[-1])
+
 
 class Batched(CompositeSpec, _typing.Generic[_T]):
     """A generic CompositeSpec that prepends a fixed Batch dimension.
 
     This Spec type essentially wraps the base spec with a call to jax.vmap
     inside `validate` and `generate_value`
     """
@@ -580,17 +600,15 @@
         To do this recursively, see `unpack_spec`.
         """
         base_spec = self.spec
         if isinstance(base_spec, CompositeSpec):
             base_spec = base_spec.as_spec_struct()
 
         def reshape(s: Spec):
-            if isinstance(s, PrimitiveSpec):
-                return reshape_spec(s, prepend=(self.num,))
-            return Batched(s, self.num)
+            return reshape_spec(s, prepend=(self.num,))
 
         return _jax.tree_map(reshape, base_spec)
 
     def validate(self, value: _T) -> _T:
         # jax.vmap fails as error-raising is non-homogenous.
         return _jax.lax.map(self.spec.validate, value)
 
@@ -674,15 +692,19 @@
 
 
 def unpack_spec(
         spec: Spec
 ) -> Spec:
     """Recursively unpack composite specs to a tree of Primitive Specs."""
     if isinstance(spec, CompositeSpec):
-        return _jax.tree_map(unpack_spec, spec.as_spec_struct())
+        unpacked = spec.as_spec_struct()
+        return _jax.tree_map(
+            unpack_spec, unpacked,
+            is_leaf=lambda z: z is not unpacked
+        )
     return spec
 
 
 def make_environment_spec(env: jit_env.Environment):
     return EnvironmentSpec(
         observations=env.observation_spec(),
         actions=env.action_spec(),
```

### Comparing `jit_env-0.1.3/jit_env/wrappers.py` & `jit_env-0.1.4/jit_env/wrappers.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.3/jit_env.egg-info/PKG-INFO` & `jit_env-0.1.4/jit_env.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jit-env
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.3-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.4-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
 
@@ -41,15 +41,15 @@
 
 Note that this module is only an interface and does not implement any
 Environments itself. The implementations in `examples` serve to illustrate the syntax.
 For a more thorough review of the semantics, please refer to the [dm-env](https://github.com/deepmind/dm_env/blob/master/dm_env/specs.py) 
 wiki and compare our implementation of `jit_env.Environment` with `dm_env.Environment` and the conversion as given in [`compat.py`](https://github.com/joeryjoery/jit_env/blob/main/jit_env/compat.py).
 
 ## Installation
-`jit_env` can be installed with:
+`jit_env` can be installed with (it is recommended to install `jax` first):
 
 `python -m pip install jit-env`
 
 You can also install it directly from our GitHub repository using pip:
 
 `python -m pip install git+git://github.com/joeryjoery/jit_env.git`
 
@@ -99,7 +99,8 @@
 ```
 
 ## References
 This library was heavily inspired by the following libraries:
 - dm-env: [https://github.com/deepmind/dm_env](https://github.com/deepmind/dm_env)
 - jumanji: [https://github.com/instadeepai/jumanji](https://github.com/instadeepai/jumanji)
 - gymnax: [https://github.com/RobertTLange/gymnax](https://github.com/RobertTLange/gymnax)
+- gymnasium: [https://github.com/Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium)
```

### Comparing `jit_env-0.1.3/setup.py` & `jit_env-0.1.4/setup.py`

 * *Files identical despite different names*

