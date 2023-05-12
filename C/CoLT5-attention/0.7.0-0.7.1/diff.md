# Comparing `tmp/CoLT5-attention-0.7.0.tar.gz` & `tmp/CoLT5-attention-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.7.0.tar", last modified: Wed May 10 20:49:10 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.7.1.tar", last modified: Fri May 12 17:15:30 2023, max compression
```

## Comparing `CoLT5-attention-0.7.0.tar` & `CoLT5-attention-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    35401 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35723 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/setup.py
```

### Comparing `CoLT5-attention-0.7.0/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.7.1/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.7.0
+Version: 0.7.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.7.0/LICENSE` & `CoLT5-attention-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.0/PKG-INFO` & `CoLT5-attention-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.7.0
+Version: 0.7.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.7.0/README.md` & `CoLT5-attention-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.0/colt5_attention/attend.py` & `CoLT5-attention-0.7.1/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.0/colt5_attention/coor_descent.py` & `CoLT5-attention-0.7.1/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.0/colt5_attention/transformer_block.py` & `CoLT5-attention-0.7.1/colt5_attention/transformer_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,16 @@
         return src
 
     def forward(
         self,
         x,
         *,
         num_tokens,
-        mask = None
+        mask = None,
+        random_route = False
     ):
         n, device, eps, num_routes, route_block_size = x.shape[-2], x.device, self.eps, self.num_routing_tokens, self.route_block_size
 
         # whether to route even amounts from blocks of the sequence
 
         if exists(route_block_size):
             num_blocks = n // route_block_size
@@ -334,14 +335,20 @@
             s,
             n_iters = self.n_iters,
             mask = mask,
             k = k,
             eps = eps
         )
 
+        # force random routing, if negative control
+
+        if random_route:
+            scores = torch.randn_like(scores)
+            scores = scores.masked_fill(~mask, -torch.finfo(scores.dtype).max)
+
         # get the topk scores and indices from the sparse matrix
 
         selected_scores, selected_indices = scores.topk(num_tokens, dim = -1)
 
         if self.straight_through:
             # this would make sure all normalized scores returned are 1., but still differentiable using straight-through trick
             selected_scores = selected_scores + (1. - selected_scores).detach()
@@ -770,15 +777,16 @@
         )
 
     def forward(
         self,
         x,
         *,
         num_heavy_tokens_q = None,
-        num_heavy_tokens_kv = None
+        num_heavy_tokens_kv = None,
+        random_route = False
     ):
         batch, device = x.shape[0], x.device
 
         num_heavy_tokens_q = default(num_heavy_tokens_q, self.num_heavy_tokens_q)
         num_heavy_tokens_kv = default(num_heavy_tokens_kv, self.num_heavy_tokens_kv)
 
         # light local attention sees all tokens in a limited context
@@ -823,23 +831,23 @@
 
         # route tokens appropriately for heavy branch, if need be
 
         should_route_q = q.shape[-2] > num_heavy_tokens_q
         should_route_kv = kv.shape[-2] > num_heavy_tokens_kv
 
         if should_route_q:
-            normalized_scores_q, indices_q = self.q_router(q, num_tokens = num_heavy_tokens_q, mask = q_mask)
+            normalized_scores_q, indices_q = self.q_router(q, num_tokens = num_heavy_tokens_q, mask = q_mask, random_route = random_route)
 
             routed_tokens_q = batched_gather(q, indices_q)
         else:
             normalized_scores_q = 1.
             routed_tokens_q = q
 
         if should_route_kv:
-            normalized_scores_kv, indices_kv = self.kv_router(kv, num_tokens = num_heavy_tokens_kv, mask = kv_mask)
+            normalized_scores_kv, indices_kv = self.kv_router(kv, num_tokens = num_heavy_tokens_kv, mask = kv_mask, random_route = random_route)
 
             routed_tokens_kv = batched_gather(kv, indices_kv)
             routed_tokens_kv_mask = batched_gather(kv_mask, indices_kv)
         else:
             normalized_scores_kv = 1.
             routed_tokens_kv = kv
             routed_tokens_kv_mask = kv_mask
```

### Comparing `CoLT5-attention-0.7.0/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.7.1/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.0/setup.py` & `CoLT5-attention-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.7.0',
+  version = '0.7.1',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

