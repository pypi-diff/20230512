# Comparing `tmp/FLASH-pytorch-0.1.7.tar.gz` & `tmp/FLASH-pytorch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLASH-pytorch-0.1.7.tar", last modified: Sun Feb 19 04:14:35 2023, max compression
+gzip compressed data, was "FLASH-pytorch-0.1.8.tar", last modified: Fri May 12 18:10:21 2023, max compression
```

## Comparing `FLASH-pytorch-0.1.7.tar` & `FLASH-pytorch-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 04:14:35.089664 FLASH-pytorch-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 04:14:35.085664 FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-19 04:14:35.000000 FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-19 04:14:35.000000 FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 04:14:35.000000 FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-19 04:14:35.000000 FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-19 04:14:35.000000 FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-19 04:14:24.000000 FLASH-pytorch-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-19 04:14:35.089664 FLASH-pytorch-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-02-19 04:14:24.000000 FLASH-pytorch-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 04:14:35.089664 FLASH-pytorch-0.1.7/flash_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-19 04:14:24.000000 FLASH-pytorch-0.1.7/flash_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-02-19 04:14:24.000000 FLASH-pytorch-0.1.7/flash_pytorch/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-02-19 04:14:24.000000 FLASH-pytorch-0.1.7/flash_pytorch/flash_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 04:14:35.089664 FLASH-pytorch-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-19 04:14:24.000000 FLASH-pytorch-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:10:21.647240 FLASH-pytorch-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:10:21.647240 FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-12 18:10:21.000000 FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-12 18:10:21.000000 FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:10:21.000000 FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-12 18:10:21.000000 FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 18:10:21.000000 FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 18:10:10.000000 FLASH-pytorch-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-12 18:10:21.647240 FLASH-pytorch-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-12 18:10:10.000000 FLASH-pytorch-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:10:21.647240 FLASH-pytorch-0.1.8/flash_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 18:10:10.000000 FLASH-pytorch-0.1.8/flash_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-12 18:10:10.000000 FLASH-pytorch-0.1.8/flash_pytorch/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-12 18:10:10.000000 FLASH-pytorch-0.1.8/flash_pytorch/flash_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:10:21.647240 FLASH-pytorch-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-12 18:10:10.000000 FLASH-pytorch-0.1.8/setup.py
```

### Comparing `FLASH-pytorch-0.1.7/FLASH_pytorch.egg-info/PKG-INFO` & `FLASH-pytorch-0.1.8/FLASH_pytorch.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLASH-pytorch
-Version: 0.1.7
+Version: 0.1.8
 Summary: FLASH - Transformer Quality in Linear Time - Pytorch
 Home-page: https://github.com/lucidrains/FLASH-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `FLASH-pytorch-0.1.7/LICENSE` & `FLASH-pytorch-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FLASH-pytorch-0.1.7/PKG-INFO` & `FLASH-pytorch-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLASH-pytorch
-Version: 0.1.7
+Version: 0.1.8
 Summary: FLASH - Transformer Quality in Linear Time - Pytorch
 Home-page: https://github.com/lucidrains/FLASH-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `FLASH-pytorch-0.1.7/README.md` & `FLASH-pytorch-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `FLASH-pytorch-0.1.7/flash_pytorch/autoregressive_wrapper.py` & `FLASH-pytorch-0.1.8/flash_pytorch/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `FLASH-pytorch-0.1.7/flash_pytorch/flash_pytorch.py` & `FLASH-pytorch-0.1.8/flash_pytorch/flash_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,25 +139,28 @@
         dim,
         query_key_dim = 128,
         expansion_factor = 2.,
         add_residual = True,
         causal = False,
         dropout = 0.,
         laplace_attn_fn = False,
+        rel_pos_bias = False,
         norm_klass = nn.LayerNorm
     ):
         super().__init__()
         hidden_dim = int(expansion_factor * dim)
 
         self.norm = norm_klass(dim)
         self.causal = causal
         self.dropout = nn.Dropout(dropout)
 
         self.attn_fn = ReLUSquared() if not laplace_attn_fn else LaplacianAttnFn()
 
+        self.rel_pos_bias = T5RelativePositionBias(scale = dim ** 0.5, causal = causal)
+
         self.to_hidden = nn.Sequential(
             nn.Linear(dim, hidden_dim * 2),
             nn.SiLU()
         )
 
         self.to_qk = nn.Sequential(
             nn.Linear(dim, query_key_dim),
@@ -183,20 +186,23 @@
 
         normed_x = self.norm(x)
         v, gate = self.to_hidden(normed_x).chunk(2, dim = -1)
 
         qk = self.to_qk(normed_x)
         q, k = self.offsetscale(qk)
 
-        sim = einsum('b i d, b j d -> b i j', q, k) / seq_len
+        sim = einsum('b i d, b j d -> b i j', q, k)
+
+        if exists(self.rel_pos_bias):
+            sim = sim + self.rel_pos_bias(sim)
 
         if exists(rel_pos_bias):
             sim = sim + rel_pos_bias
 
-        attn = self.attn_fn(sim)
+        attn = self.attn_fn(sim / seq_len)
         attn = self.dropout(attn)
 
         if exists(mask):
             mask = rearrange(mask, 'b j -> b 1 j')
             attn = attn.masked_fill(~mask, 0.)
 
         if self.causal:
```

### Comparing `FLASH-pytorch-0.1.7/setup.py` & `FLASH-pytorch-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'FLASH-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.7',
+  version = '0.1.8',
   license='MIT',
   description = 'FLASH - Transformer Quality in Linear Time - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/FLASH-pytorch',
   keywords = [
```

