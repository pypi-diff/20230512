# Comparing `tmp/gemclus-0.0.2.tar.gz` & `tmp/gemclus-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemclus-0.0.2.tar", last modified: Tue May  2 15:55:14 2023, max compression
+gzip compressed data, was "gemclus-0.1.0.tar", last modified: Fri May 12 18:02:26 2023, max compression
```

## Comparing `gemclus-0.0.2.tar` & `gemclus-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/
--rw-rw-r--   0 louis     (1000) louis     (1000)      705 2023-04-27 12:43:01.000000 gemclus-0.0.2/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-04-27 12:04:58.000000 gemclus-0.0.2/MANIFEST.in
--rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-02 15:55:14.577494 gemclus-0.0.2/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     2010 2023-05-02 09:19:29.000000 gemclus-0.0.2/README.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/
--rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-05-02 15:25:00.000000 gemclus-0.0.2/gemclus/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    20059 2023-05-02 14:58:53.000000 gemclus-0.0.2/gemclus/_base_gemini.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/_gemini_grads/
--rw-rw-r--   0 louis     (1000) louis     (1000)      300 2023-05-02 09:32:20.000000 gemclus-0.0.2/gemclus/_gemini_grads/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5568 2023-05-02 09:34:30.000000 gemclus-0.0.2/gemclus/_gemini_grads/_gemini_losses.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2406 2023-04-28 09:20:02.000000 gemclus-0.0.2/gemclus/_gemini_grads/_prox_grad.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/data/
--rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-05-02 08:01:52.000000 gemclus-0.0.2/gemclus/data/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    11872 2023-05-02 12:31:44.000000 gemclus-0.0.2/gemclus/data/synthetic_data.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/linear/
--rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/linear/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    13273 2023-05-02 13:51:33.000000 gemclus-0.0.2/gemclus/linear/_linear_geminis.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/mlp/
--rw-rw-r--   0 louis     (1000) louis     (1000)       89 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/mlp/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    11313 2023-05-02 13:51:13.000000 gemclus-0.0.2/gemclus/mlp/_mlp_geminis.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/sparse/
--rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/sparse/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    23850 2023-05-02 15:17:21.000000 gemclus-0.0.2/gemclus/sparse/_base_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5437 2023-05-02 13:46:20.000000 gemclus-0.0.2/gemclus/sparse/_linear_sparse.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5989 2023-05-02 13:50:26.000000 gemclus-0.0.2/gemclus/sparse/_mlp_sparse.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus/tests/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-03-29 14:26:07.000000 gemclus-0.0.2/gemclus/tests/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2808 2023-05-02 09:19:28.000000 gemclus-0.0.2/gemclus/tests/test_data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3331 2023-05-02 13:57:17.000000 gemclus-0.0.2/gemclus/tests/test_default.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3935 2023-05-02 09:19:29.000000 gemclus-0.0.2/gemclus/tests/test_objectives.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5548 2023-05-02 14:10:19.000000 gemclus-0.0.2/gemclus/tests/test_path.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-02 15:55:14.577494 gemclus-0.0.2/gemclus.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      851 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        8 2023-05-02 15:55:14.000000 gemclus-0.0.2/gemclus.egg-info/top_level.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       97 2023-04-27 14:33:43.000000 gemclus-0.0.2/pyproject.toml
--rw-rw-r--   0 louis     (1000) louis     (1000)       50 2023-05-02 15:54:07.000000 gemclus-0.0.2/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)      147 2023-05-02 15:55:14.577494 gemclus-0.0.2/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2023-04-27 15:56:32.000000 gemclus-0.0.2/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      705 2023-04-27 12:43:01.000000 gemclus-0.1.0/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-04-27 12:04:58.000000 gemclus-0.1.0/MANIFEST.in
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-12 18:02:26.249091 gemclus-0.1.0/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2010 2023-05-10 08:55:34.000000 gemclus-0.1.0/README.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      162 2023-05-12 18:01:12.000000 gemclus-0.1.0/gemclus/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    18744 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/_base_gemini.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus/data/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-05-10 08:55:34.000000 gemclus-0.1.0/gemclus/data/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11869 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/data/synthetic_data.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus/gemini/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      125 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/gemini/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    15507 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/gemini/_gemini_losses.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/linear/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      116 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/linear/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    12833 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/linear/_linear_geminis.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/mlp/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       89 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/mlp/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11321 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/mlp/_mlp_geminis.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/nonparametric/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      128 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/nonparametric/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     8172 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/nonparametric/_categorical_models.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/sparse/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      129 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/sparse/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    24304 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/sparse/_base_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5437 2023-05-10 08:55:34.000000 gemclus-0.1.0/gemclus/sparse/_linear_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5988 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/sparse/_mlp_sparse.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2422 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/sparse/_prox_grad.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.249091 gemclus-0.1.0/gemclus/tests/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-03-29 14:26:07.000000 gemclus-0.1.0/gemclus/tests/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2808 2023-05-10 08:55:34.000000 gemclus-0.1.0/gemclus/tests/test_data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4508 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/tests/test_default.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3248 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/tests/test_objectives.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5708 2023-05-12 18:00:55.000000 gemclus-0.1.0/gemclus/tests/test_path.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-05-12 18:02:26.245092 gemclus-0.1.0/gemclus.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3325 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      909 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      130 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        8 2023-05-12 18:02:26.000000 gemclus-0.1.0/gemclus.egg-info/top_level.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       97 2023-04-27 14:33:43.000000 gemclus-0.1.0/pyproject.toml
+-rw-rw-r--   0 louis     (1000) louis     (1000)       50 2023-05-10 08:55:34.000000 gemclus-0.1.0/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)      147 2023-05-12 18:02:26.249091 gemclus-0.1.0/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2023-04-27 15:56:32.000000 gemclus-0.1.0/setup.py
```

### Comparing `gemclus-0.0.2/LICENSE` & `gemclus-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemclus-0.0.2/PKG-INFO` & `gemclus-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemclus
-Version: 0.0.2
+Version: 0.1.0
 Summary: A package for performing discriminative clustering with gemini-trained models
 Home-page: https://github.com/gemini-clustering
 Download-URL: https://github.com/gemini-clustering
 Maintainer: Louis Ohl
 Maintainer-email: louis.ohl@inria.fr
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gemclus-0.0.2/README.md` & `gemclus-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gemclus-0.0.2/gemclus/_base_gemini.py` & `gemclus-0.1.0/gemclus/_base_gemini.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 """
 
 from abc import ABC, abstractmethod
 from numbers import Integral, Real
 
 import numpy as np
 from sklearn.base import ClusterMixin, BaseEstimator
-from sklearn.metrics.pairwise import PAIRWISE_KERNEL_FUNCTIONS, PAIRED_DISTANCES, pairwise_kernels, pairwise_distances
+from sklearn.metrics.pairwise import PAIRWISE_KERNEL_FUNCTIONS, PAIRED_DISTANCES
 from sklearn.neural_network._stochastic_optimizers import AdamOptimizer, SGDOptimizer
 from sklearn.utils import check_array, check_random_state
 from sklearn.utils._param_validation import Interval, StrOptions
 from sklearn.utils.validation import check_is_fitted
 
-from gemclus._gemini_grads import mmd_ovo, mmd_ova, wasserstein_ovo, wasserstein_ova
+from gemclus.gemini import MMDOvO, MMDOvA, WassersteinOvO, WassersteinOvA
 
 
 class _BaseGEMINI(ClusterMixin, BaseEstimator, ABC):
     """ This is the BaseGEMINI to derive to create a GEMINI MLP or linear clustering model.
      When deriving this class, there are a couple methods to override depending on the design of a discriminative model
      :math:`p(y|x)` or a specific GEMINI.
 
@@ -74,49 +74,37 @@
         self.learning_rate = learning_rate
         self.solver = solver
         self.batch_size = batch_size
         self.verbose = verbose
         self.random_state = random_state
 
     @abstractmethod
-    def _init_params(self, random_state):
+    def _init_params(self, random_state, X=None):
         """
         Initialise the set of parameters :math:`\theta` parameters of the model that are used to compute
         :math:`p_\theta(y|x)`.
 
         Parameters
         ----------
         random_state: RandomState instance
             Determines random number generation for weights and bias initialisation.
+
+        X: ndarray of shape (n_samples, n_features), default=None
+            The data to fit in case it is needed for a special initialisation of the weights.
         """
         pass
 
     @abstractmethod
-    def _compute_gemini(self, y_pred, K, return_grad=False):
+    def get_gemini(self):
         """
-        Compute the GEMINI objective given the predictions :math:`p_\theta(y|x)` and an affinity matrix. The computation
-        must return as well the gradients of the GEMINI w.r.t. the predictions. Depending on the context,
-        the affinity matrix :ref:`K` can be either a kernel matrix or a distance matrix resulting from the
-        :ref:`_compute_affinity` method.
-
-        Parameters
-        ----------
-        y_pred: ndarray of shape (n_samples, n_clusters)
-            The conditional distribution (prediction) of clustering assignment per sample.
-        K: ndarray of shape (n_samples, n_samples)
-            The affinity matrix resulting from the :ref:`_compute_affinity` method. The matrix must be symmetric.
-        return_grad: bool, default=False
-            If True, the method should return the gradient of the GEMINI w.r.t. the predictions :math:`p_\theta(y|x)`.
+        Initialises a :class:`gemclus.GEMINI` instance that will be used to train the model.
 
         Returns
         -------
-        gemclus: float
-            The gemclus score I of the model given the predictions and affinities.
-        gradients: ndarray of shape (n_samples, n_clusters)
-            The derivative :math:`\nabla_{p_\theta(y|x)}I` of the GEMINI.
+        gemini: :class:`gemclus.GEMINI` instance
         """
         pass
 
     @abstractmethod
     def _compute_grads(self, X, y_pred, gradient):
         """
         Compute the gradient of each parameter of the model according to the input, output and
@@ -169,34 +157,51 @@
         Returns
         -------
         y_pred:  ndarray of shape (n_samples, n_clusters)
             The prediction :math:`p_\theta(y|x)` probabilities of the model.
         """
         pass
 
-    @abstractmethod
-    def _compute_affinity(self, X, y=None):
+    def _batchify(self, X, affinity_matrix=None, random_state=None):
         """
-        Compute the affinity (kernel function or distance function_ between all samples of X.
+        Yields elements of X and its corresponding affinity matrix in batches with a uniform random sampling.
 
         Parameters
         ----------
         X: ndarray of shape (n_samples, n_features)
-            The samples between which all affinities must be compute
+            Training instances to cluster
 
-        y: ndarray of shape (n_samples, n_samples), default=None
-            Values of the affinity between samples in case of a "precomputed" affinity. Ignored if None and the affinity
-            is not precomputed.
-
-        Return
-        ------
-        K: ndarray of shape (n_samples, n_samples)
-            The symmetric affinity matrix
-        """
-        pass
+        affinity_matrix: ndarray of shape (n_samples, n_samples) or None
+            The affinity computed between all elements of `X`. Setting to None means the GEMINI doe snot need any
+            affinity.
+
+        random_state: int, RandomState instance, default=None
+
+        Returns
+        -------
+        X_batch: ndarray of shape (n_batch, n_features)
+            The batch of data elements
+
+        affinity_batch: ndarray of shape (n_batch, n_batch) or None
+            The affinity values of the corresponding elements of the data batch. If the parameter `affinity_matrix` was
+            None, then None is returned.
+        """
+        random_state = check_random_state(random_state)
+        all_indices = random_state.permutation(len(X))
+        batch_size = len(X) if self.batch_size is None else self.batch_size
+        j = 0
+        while j < len(X):
+            batch_indices = all_indices[j:j + batch_size]
+            X_batch = X[batch_indices]
+            if affinity_matrix is not None:
+                affinity_batch = affinity_matrix[batch_indices][:, batch_indices]
+            else:
+                affinity_batch = None
+            yield X_batch, affinity_batch
+            j += batch_size
 
     def fit(self, X, y=None):
         """Compute GEMINI clustering.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
@@ -212,60 +217,45 @@
         """
         self._validate_params()
 
         # Check that X has the correct shape
         X = check_array(X)
         X = self._validate_data(X, accept_sparse=True, dtype=np.float64, ensure_min_samples=self.n_clusters)
 
-        if self.batch_size is None:
-            batch_size = len(X)
-        else:
-            batch_size = self.batch_size
-
         # Fix the random seed
         random_state = check_random_state(self.random_state)
 
         # Initialise the weights
         if self.verbose:
             print("Initialising parameters")
-        self._init_params(random_state)
+        self._init_params(random_state, X)
         weights = self._get_weights()
+        gemini = self.get_gemini()
 
         if self.solver == "sgd":
             self.optimiser_ = SGDOptimizer(weights, self.learning_rate)
         else:
             self.optimiser_ = AdamOptimizer(weights, self.learning_rate)
 
         if self.verbose:
             print(f"Computing affinity")
 
-        affinity = self._compute_affinity(X, y)
+        affinity = gemini.compute_affinity(X, y)
 
         if self.verbose:
             print(f"Starting training over {self.max_iter} iterations.")
         # Now, iterate for gradient descent
         for i in range(self.max_iter):
             # Create batches
-            j = 0
-            all_indices = random_state.permutation(len(X))
-            while j < len(X):
-                batch_indices = all_indices[j:j + batch_size]
-                X_batch = X[batch_indices]
-                if affinity is None:
-                    affinity_batch = None  # Specific case of f-div GEMINI
-                else:
-                    affinity_batch = affinity[batch_indices][:, batch_indices]
-
+            for X_batch, affinity_batch in self._batchify(X, affinity, random_state):
                 y_pred = self._infer(X_batch)
-                _, grads = self._compute_gemini(y_pred, affinity_batch, return_grad=True)
+                _, grads = gemini(y_pred, affinity_batch, return_grad=True)
                 grads = self._compute_grads(X_batch, y_pred, grads)
                 self._update_weights(weights, grads)
 
-                j += batch_size
-
         if self.verbose:
             print("Finished")
 
         # Return the classifier
 
         # Must save the labels
         self.labels_ = self._infer(X).argmax(1)
@@ -353,17 +343,18 @@
             construction. Otherwise, it is not used and present here for API consistency by convention.
 
         Returns
         -------
         score : float
             GEMINI evaluated on the output of ``self.predict(X)``.
         """
-        K = self._compute_affinity(X, y)
+        gemini = self.get_gemini()
+        K = gemini.compute_affinity(X, y)
         y_pred = self.predict_proba(X)
-        return self._compute_gemini(y_pred, K).item()
+        return gemini(y_pred, K).item()
 
 
 class _BaseMMD(_BaseGEMINI, ABC):
     """
     Adds the MMD GEMINI to the base model.
 
     Parameters
@@ -426,27 +417,19 @@
             batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.kernel = kernel
         self.ovo = ovo
 
-    def _compute_affinity(self, X, y=None):
-        if callable(self.kernel):
-            return self.kernel(X)
-        elif self.kernel == "precomputed":
-            assert y is not None, f"Kernel should be precomputed, yet no kernel was passed as parameters: y={y}"
-            return y
-        return pairwise_kernels(X, metric=self.kernel)
-
-    def _compute_gemini(self, y_pred, K, return_grad=False):
+    def get_gemini(self):
         if self.ovo:
-            return mmd_ovo(y_pred, K, return_grad)
+            return MMDOvO(self.kernel)
         else:
-            return mmd_ova(y_pred, K, return_grad)
+            return MMDOvA(self.kernel)
 
 
 class _BaseWasserstein(_BaseGEMINI, ABC):
     """
     Adds the Wasserstein GEMINI to the base model.
 
     Parameters
@@ -509,20 +492,12 @@
             batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.metric = metric
         self.ovo = ovo
 
-    def _compute_affinity(self, X, y=None):
-        if callable(self.metric):
-            return self.metric(X)
-        elif self.metric == "precomputed":
-            assert y is not None, f"Kernel should be precomputed, yet no kernel was passed as parameters: y={y}"
-            return y
-        return pairwise_distances(X, metric=self.metric)
-
-    def _compute_gemini(self, y_pred, K, return_grad=False):
+    def get_gemini(self):
         if self.ovo:
-            return wasserstein_ovo(y_pred, K, return_grad)
+            return WassersteinOvO(self.metric)
         else:
-            return wasserstein_ova(y_pred, K, return_grad)
+            return WassersteinOvA(self.metric)
```

### Comparing `gemclus-0.0.2/gemclus/_gemini_grads/_prox_grad.py` & `gemclus-0.1.0/gemclus/sparse/_prox_grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 
-def soft_threshold(l, x):
-    return np.sign(x) * np.maximum(np.abs(x) - l, 0)
+def soft_threshold(threshold, x):
+    return np.sign(x) * np.maximum(np.abs(x) - threshold, 0)
 
 
 def mlp_prox_grad(W_skip_, W1_, alpha, M):
     v = W_skip_
     u = W1_
 
     # Contrary to the original version, here the output dimension is on the columns
```

### Comparing `gemclus-0.0.2/gemclus/data/synthetic_data.py` & `gemclus-0.1.0/gemclus/data/synthetic_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     -------
     X: ndarray
         The samples of the dataset in an array of shape n_samples x n_features
     y: ndarray
         The component of the GMM from which each sample was drawn.
 
     References
-    -----------
+    ----------
     GEMINI - Ohl, L., Mattei, P. A., Bouveyron, C., Harchaoui, W., Leclercq, M., Droit, A., & Precioso, F.
         (2022, October). Generalised Mutual Information for Discriminative Clustering. In Advances in Neural
         Information Processing Systems.
     """
     generator = check_random_state(random_state)
 
     # Build the location and scale of each distribution
@@ -220,15 +220,15 @@
     -------
     X: ndarray
         The samples of the dataset in an array of shape n_samples x n_features
     y: ndarray
         The component of the GMM from which each sample was drawn.
 
     References
-    -----------
+    ----------
     Dataset - Celeux, G., Martin-Magniette, M. L., Maugis-Rabusseau, C., & Raftery, A. E. (2014). Comparing model
         selection and regularization approaches to variable selection in model-based clustering.
         Journal de la Societe francaise de statistique, 155(2), 57-71.
     """
     generator = check_random_state(random_state)
 
     # Draw the first five variables according to a balance gaussian mixture
@@ -269,15 +269,15 @@
     -------
     X: ndarray
         The samples of the dataset in an array of shape n_samples x n_features
     y: ndarray
         The component of the GMM from which each sample was drawn.
 
     References
-    -----------
+    ----------
     Dataset - Celeux, G., Martin-Magniette, M. L., Maugis-Rabusseau, C., & Raftery, A. E. (2014). Comparing model
         selection and regularization approaches to variable selection in model-based clustering.
         Journal de la Societe francaise de statistique, 155(2), 57-71.
     """
 
     generator = check_random_state(random_state)
```

### Comparing `gemclus-0.0.2/gemclus/linear/_linear_geminis.py` & `gemclus-0.1.0/gemclus/linear/_linear_geminis.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 from sklearn.neural_network._stochastic_optimizers import AdamOptimizer, SGDOptimizer
 from sklearn.utils._param_validation import Interval
 from sklearn.utils.extmath import softmax
 
 from .._base_gemini import _BaseGEMINI, _BaseMMD, _BaseWasserstein
+from ..gemini import MI
 
 
 class _LinearGEMINI(_BaseGEMINI, ABC):
     _parameter_constraints: dict = {
         **_BaseGEMINI._parameter_constraints,
     }
 
@@ -22,15 +23,15 @@
             learning_rate=learning_rate,
             solver=solver,
             batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
 
-    def _init_params(self, random_state):
+    def _init_params(self, random_state, X=None):
         in_threshold = np.sqrt(1 / self.n_features_in_)
         self.W_ = random_state.uniform(-in_threshold, in_threshold, size=(self.n_features_in_, self.n_clusters))
         self.b_ = random_state.uniform(-in_threshold, in_threshold, size=(1, self.n_clusters))
 
     def _compute_grads(self, X, y_pred, gradient):
         tau_hat_grad = y_pred * (gradient - (y_pred * gradient).sum(1, keepdims=True))  # Shape NxK
 
@@ -119,15 +120,15 @@
     >>> X,y=load_iris(return_X_y=True)
     >>> clf = LinearMMD(random_state=0).fit(X)
     >>> clf.predict(X[:2,:])
     array([0, 0])
     >>> clf.predict_proba(X[:2,:]).shape
     (2, 3)
     >>> clf.score(X)
-    1.6949190522657158
+    1.6949190522657067
     """
     _parameter_constraints: dict = {
         **_BaseMMD._parameter_constraints,
         **_LinearGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, kernel="linear", solver="adam", ovo=False,
@@ -208,19 +209,19 @@
     Examples
     --------
     >>> from sklearn.datasets import load_iris
     >>> from gemclus.linear import LinearWasserstein
     >>> X,y=load_iris(return_X_y=True)
     >>> clf = LinearWasserstein(random_state=0).fit(X)
     >>> clf.predict(X[:2,:])
-    array([2, 2])
+    array([0, 0])
     >>> clf.predict_proba(X[:2,:]).shape
     (2, 3)
     >>> clf.score(X)
-    1.6509087196143133
+    1.6993348362264595
     """
     _parameter_constraints: dict = {
         **_BaseWasserstein._parameter_constraints,
         **_LinearGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, metric="euclidean", ovo=False,
@@ -235,84 +236,86 @@
             batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
             metric=metric
         )
 
 
+# noinspection PyPep8
 class RIM(_LinearGEMINI):
+    # noinspection PyPep8
     """ Implementation of the maximisation of the classical mutual information using a logistic regression with an
-    :math:`\ell_2` penalty on the weights. This implementation follows the framework described by Krause et al. in the
-    RIM paper.
-
-    Parameters
-    ----------
-    n_clusters : int, default=3
-        The maximum number of clusters to form as well as the number of output neurons in the neural network.
-
-    max_iter: int, default=1000
-        Maximum number of epochs to perform gradient descent in a single run.
-
-    learning_rate: float, default=1e-3
-        Initial learning rate used. It controls the step-size in updating the weights.
+        :math:`\ell_2` penalty on the weights. This implementation follows the framework described by Krause et al. in the
+        RIM paper.
 
-    reg: float, default=1.0
-        Regularisation hyperparameter for the $\ell_2$ weight penalty.
-
-    solver: {'sgd','adam'}, default='adam'
-        The solver for weight optimisation.
-
-        - 'sgd' refers to stochastic gradient descent.
-        - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
-
-    batch_size: int, default=None
-        The size of batches during gradient descent training. If set to None, the whole data will be considered.
-
-    verbose: bool, default=False
-        Whether to print progress messages to stdout
-
-    random_state: int, RandomState instance, default=None
-        Determines random number generation for weights and bias initialisation.
-        Pass an int for reproducible results across multiple function calls.
-
-    Attributes
-    ----------
-    W_: ndarray of shape (n_features_in, n_clusters)
-        The linear weights of model
-    b_: ndarray of shape (1, n_clusters)
-        The biases of the model
-    optimiser_: `AdamOptimizer` or `SGDOptimizer`
-        The optimisation algorithm used for training depending on the chosen solver parameter.
-    labels_: ndarray of shape (n_samples)
-        The labels that were assigned to the samples passed to the :meth:`fit` method.
-    n_iter_: int
-        The number of iterations that the model took for converging.
-
-    References
-    ----------
-    RIM - Discriminative Clustering by Regularized Information Maximization
-        Ryan Gomes, Andreas Krause, Pietro Perona. 2010.
-
-    See Also
-    --------
-    LinearMMD: logistic regression trained for clustering with the MMD GEMINI
-
-    Examples
-    --------
-    >>> from sklearn.datasets import load_iris
-    >>> from gemclus.linear import RIM
-    >>> X,y=load_iris(return_X_y=True)
-    >>> clf = RIM(learning_rate=1e-2, random_state=0).fit(X)
-    >>> clf.predict(X[:2,:])
-    array([0, 0])
-    >>> clf.predict_proba(X[:2,:]).shape
-    (2, 3)
-    >>> clf.score(X)
-    0.00962912118121384
-    """
+        Parameters
+        ----------
+        n_clusters : int, default=3
+            The maximum number of clusters to form as well as the number of output neurons in the neural network.
+
+        max_iter: int, default=1000
+            Maximum number of epochs to perform gradient descent in a single run.
+
+        learning_rate: float, default=1e-3
+            Initial learning rate used. It controls the step-size in updating the weights.
+
+        reg: float, default=1.0
+            Regularisation hyperparameter for the $\ell_2$ weight penalty.
+
+        solver: {'sgd','adam'}, default='adam'
+            The solver for weight optimisation.
+
+            - 'sgd' refers to stochastic gradient descent.
+            - 'adam' refers to a stochastic gradient-based optimiser proposed by Kingma, Diederik and Jimmy Ba.
+
+        batch_size: int, default=None
+            The size of batches during gradient descent training. If set to None, the whole data will be considered.
+
+        verbose: bool, default=False
+            Whether to print progress messages to stdout
+
+        random_state: int, RandomState instance, default=None
+            Determines random number generation for weights and bias initialisation.
+            Pass an int for reproducible results across multiple function calls.
+
+        Attributes
+        ----------
+        W_: ndarray of shape (n_features_in, n_clusters)
+            The linear weights of model
+        b_: ndarray of shape (1, n_clusters)
+            The biases of the model
+        optimiser_: `AdamOptimizer` or `SGDOptimizer`
+            The optimisation algorithm used for training depending on the chosen solver parameter.
+        labels_: ndarray of shape (n_samples)
+            The labels that were assigned to the samples passed to the :meth:`fit` method.
+        n_iter_: int
+            The number of iterations that the model took for converging.
+
+        References
+        ----------
+        RIM - Discriminative Clustering by Regularized Information Maximization
+            Ryan Gomes, Andreas Krause, Pietro Perona. 2010.
+
+        See Also
+        --------
+        LinearMMD: logistic regression trained for clustering with the MMD GEMINI
+
+        Examples
+        --------
+        >>> from sklearn.datasets import load_iris
+        >>> from gemclus.linear import RIM
+        >>> X,y=load_iris(return_X_y=True)
+        >>> clf = RIM(learning_rate=1e-2, random_state=0).fit(X)
+        >>> clf.predict(X[:2,:])
+        array([0, 0])
+        >>> clf.predict_proba(X[:2,:]).shape
+        (2, 3)
+        >>> clf.score(X)
+        0.00962912118121384
+        """
 
     _parameter_constraints: dict = {
         **_LinearGEMINI._parameter_constraints,
         "reg": [Interval(Real, 0, None, closed="left")]
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, reg=1,
@@ -325,36 +328,14 @@
             solver=solver,
             batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.reg = reg
 
-    def _compute_affinity(self, X, y=None):
-        return None
-
-    def _compute_gemini(self, y_pred, K, return_grad=False):
-        # Start by computing mutual information
-        p_y_x = np.clip(y_pred, 1e-12, 1 - 1e-12)
-        p_y = p_y_x.mean(0)
-
-        log_p_y_x = np.log(p_y_x)
-        log_p_y = np.log(p_y)
-
-        cluster_entropy = np.sum(p_y * log_p_y)
-        prediction_entropy = np.sum(np.mean(p_y_x * log_p_y_x, axis=0))
-
-        mutual_information = prediction_entropy - cluster_entropy
-
-        if return_grad:
-            gradient_mi = -log_p_y_x / log_p_y_x.shape[0] + log_p_y
-            return mutual_information, -gradient_mi
-        else:
-            return mutual_information
-
-    def compute_penalty(self):
-        return self.reg * np.sum(self.W_ * self.W_)
+    def get_gemini(self):
+        return MI()
 
     def _update_weights(self, weights, gradients):
         # Add the regularisation gradient on the weight matrix
         gradients[0] += self.reg * 2 * self.W_
         self.optimiser_.update_params(weights, gradients)
```

### Comparing `gemclus-0.0.2/gemclus/mlp/_mlp_geminis.py` & `gemclus-0.1.0/gemclus/mlp/_mlp_geminis.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             solver=solver,
             batch_size=batch_size,
             verbose=verbose,
             random_state=random_state
         )
         self.n_hidden_dim = n_hidden_dim
 
-    def _init_params(self, random_state):
+    def _init_params(self, random_state, X=None):
         in_threshold = np.sqrt(1 / self.n_features_in_)
         hidden_threshold = np.sqrt(1 / self.n_hidden_dim)
         self.W1_ = random_state.uniform(-in_threshold, in_threshold, size=(self.n_features_in_, self.n_hidden_dim))
         self.b1_ = random_state.uniform(-in_threshold, in_threshold, size=(1, self.n_hidden_dim))
         self.W2_ = random_state.uniform(-hidden_threshold, hidden_threshold, size=(self.n_hidden_dim, self.n_clusters))
         self.b2_ = random_state.uniform(-hidden_threshold, hidden_threshold, size=(1, self.n_clusters))
 
@@ -140,15 +140,15 @@
     >>> X,y=load_iris(return_X_y=True)
     >>> clf = MLPMMD(random_state=0).fit(X)
     >>> clf.predict(X[:2,:])
     array([2, 2])
     >>> clf.predict_proba(X[:2,:]).shape
     (2, 3)
     >>> clf.score(X)
-    1.7592155845461592
+    1.7592155845461646
     """
     _parameter_constraints: dict = {
         **_BaseMMD._parameter_constraints,
         **_MLPGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, kernel="linear", ovo=False,
@@ -256,15 +256,15 @@
     >>> X,y=load_iris(return_X_y=True)
     >>> clf = MLPWasserstein(random_state=0).fit(X)
     >>> clf.predict(X[:2,:])
     array([0, 0])
     >>> clf.predict_proba(X[:2,:]).shape
     (2, 3)
     >>> clf.score(X)
-    1.7615502432434385
+    1.7636482655127903
     """
     _parameter_constraints: dict = {
         **_BaseWasserstein._parameter_constraints,
         **_MLPGEMINI._parameter_constraints
     }
 
     def __init__(self, n_clusters=3, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, metric="euclidean", ovo=False,
```

### Comparing `gemclus-0.0.2/gemclus/sparse/_base_sparse.py` & `gemclus-0.1.0/gemclus/sparse/_base_sparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 
 import numpy as np
 from sklearn.neural_network._stochastic_optimizers import SGDOptimizer
 from sklearn.utils import check_random_state
 from sklearn.utils._param_validation import Interval
 from sklearn.utils.extmath import softmax
 
-from .._gemini_grads import linear_prox_grad, group_mlp_prox_grad, group_linear_prox_grad, mlp_prox_grad
+from ._prox_grad import linear_prox_grad, group_mlp_prox_grad, group_linear_prox_grad, mlp_prox_grad
 from ..linear._linear_geminis import _LinearGEMINI
 from ..mlp._mlp_geminis import _MLPGEMINI
 
 
 def check_groups(groups, n_features_in):
     if groups is not None:
         all_indices = []
         for g in groups:
             all_indices.extend(list(g))
         assert len(all_indices) == n_features_in and set(all_indices) == set(range(n_features_in)), \
             f"Groups must form a partition of the set of variable indices"
 
-def compute_val_score(clf,X, batch_size):
+
+def compute_val_score(clf, X, batch_size):
     validation_gemini = 0  # clf.score(X)
     validation_l1 = clf._group_lasso_penalty() * clf.alpha
     j = 0
     while j < len(X):
         X_batch = X[j:j + batch_size]
         validation_gemini += clf.score(X_batch) * len(X_batch)
         j += batch_size
     validation_gemini /= len(X)
     return validation_gemini, validation_l1
 
+
 def _path(clf, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9,
           early_stopping_factor=0.99, max_patience=10):
     clf._validate_data(X)
     check_groups(clf.groups, X.shape[1])
     if alpha_multiplier <= 1:
         warnings.warn(f"The alpha multiplier is lower or equal to 1. This will not increase alpha during the path. "
                       f"Setting it again to default parameters: 1.05")
@@ -55,99 +57,106 @@
     # Start by fitting the model using all features and without regularisation
     alpha = clf.alpha
     clf.set_params(alpha=0)
 
     if clf.verbose:
         print("Starting initial training with alpha = 0")
     clf.fit(X)
-    best_gemini = clf.score(X)
-    weights = clf._get_weights()
-    best_weights = [w.copy() for w in weights]
-
-    if clf.verbose:
-        print(f"Finished initial training. GEMINI = {best_gemini}")
-
-    kernel = clf._compute_affinity(X)
 
     generator = check_random_state(clf.random_state)
     if clf.batch_size is not None:
         batch_size = clf.batch_size
     else:
         batch_size = len(X)
 
-    alphas = [0]
-    n_features = [X.shape[1]]
-    geminis = [best_gemini]
-    group_lasso_penalties = [clf._group_lasso_penalty()]
+    best_gemini_score, _ = compute_val_score(clf, X, batch_size)  # Best gemini score only when using all features
+    gemini_objective = clf.get_gemini()
+    weights = clf._get_weights()
+    best_weights = [w.copy() for w in weights]
+
+    if clf.verbose:
+        print(f"Finished initial training. GEMINI = {best_gemini_score}")
 
-    # Re-initialise the optimiser to SGD with 0.9 momentum (default option)
+    affinity = gemini_objective.compute_affinity(X)
+
+    alphas = []
+    n_features = []
+    geminis = []
+    group_lasso_penalties = []
+
+    # Re-initialise the optimiser to SGD with 0.9 momentum (default option), to follow the torch version
+    # nesterov acceleration is set to True by default
     clf.optimiser_ = SGDOptimizer(weights, clf.learning_rate)
 
     while clf._n_selected_features() > min_features:
         clf.alpha = alpha
 
         # Compute the validation scores at the beginning of this step of the path
-        validation_gemini, validation_l1 = compute_val_score(clf, X, batch_size)
+        validation_gemini_score, validation_l1 = compute_val_score(clf, X, batch_size)
 
         if clf.verbose:
-            print(f"Starting new iteration with: alpha = {clf.alpha}. Validation score is {validation_gemini}")
+            print(f"Starting new iteration with: alpha = {clf.alpha}. Validation score is {validation_gemini_score}")
 
-        gemini_score = np.array([validation_gemini])
         patience = 0
         i = 0
         while i < clf.max_iter and patience < max_patience:
             all_indices = generator.permutation(len(X))
             j = 0
             while j < len(X):
                 batch_indices = all_indices[j:j + batch_size]
                 X_batch = X[batch_indices]
-                kernel_batch = kernel[batch_indices][:, batch_indices]
+                kernel_batch = affinity[batch_indices][:, batch_indices]
                 y_pred = clf._infer(X_batch)
-                gemini_score, grads = clf._compute_gemini(y_pred, kernel_batch, return_grad=True)
+                _, grads = gemini_objective(y_pred, kernel_batch, return_grad=True)
                 grads = clf._compute_grads(X_batch, y_pred, grads)
                 clf._update_weights(weights, grads)
 
                 j += batch_size
 
-            iteration_gemini, iteration_l1 = compute_val_score(clf, X, batch_size)
+            # Epoch control
+            iteration_gemini_score, iteration_l1 = compute_val_score(clf, X, batch_size)
 
-            if iteration_gemini > (2 - early_stopping_factor) * validation_gemini \
+            if iteration_gemini_score > (2 - early_stopping_factor) * validation_gemini_score \
                     or iteration_l1 < early_stopping_factor * validation_l1:
                 validation_l1 = iteration_l1
-                validation_gemini = iteration_gemini
+                validation_gemini_score = iteration_gemini_score
                 patience = 0
             else:
                 patience += 1
-            if np.isnan(gemini_score):
+            if np.isnan(iteration_gemini_score):
                 warnings.warn(f"Unfortunately, the GEMINI converged to nan, making the entire path unsucessful."
-                              f"Please report this error. Score and gradients are: {gemini_score}, {grads}")
+                              f"Please report this error. Score and gradients are: {iteration_gemini_score}, {grads}")
                 patience = max_patience
 
             i += 1
 
+        if np.isnan(iteration_gemini_score):
+            break
+
         alphas.append(alpha)
         n_features.append(clf._n_selected_features().item())
-        geminis.append(gemini_score.item())
+        geminis.append(iteration_gemini_score)
         group_lasso_penalties.append(clf._group_lasso_penalty())
 
         if clf.verbose:
-            print(f"Finished after {i} iterations. Current iteration score is {iteration_gemini - iteration_l1}. "
-                  f"Current GEMINI score is {gemini_score}. Number of features is"
+            print(f"Finished after {i} iterations. Current iteration score is {iteration_l1 - iteration_gemini_score}. "
+                  f"\t(GEMINI: {iteration_gemini_score}, L1: {iteration_l1}). Number of features is"
                   f" {clf._n_selected_features().item()}")
 
         alpha *= alpha_multiplier
-        if gemini_score >= best_gemini:
-            best_gemini = gemini_score
+        if iteration_gemini_score >= best_gemini_score and clf._n_selected_features() == X.shape[1]:
+            best_gemini_score = iteration_gemini_score
             if clf.verbose:
-                print("Best GEMINI score so far, saving it.")
+                print("Best GEMINI score so far using all features, saving it.")
 
-        if gemini_score >= keep_threshold * best_gemini:
+        if iteration_gemini_score >= keep_threshold * best_gemini_score:
             best_weights = [w.copy() for w in weights]
             if clf.verbose:
-                print(f"This is definitely the best score so far within threshold: {gemini_score}, {best_gemini}")
+                print(f"This is definitely the best score so far within threshold: {iteration_gemini_score}, "
+                      f"{best_gemini_score}")
 
     return best_weights, geminis, group_lasso_penalties, alphas, n_features
 
 
 class _SparseMLPGEMINI(_MLPGEMINI, ABC):
     """ This is the BaseSparseGEMINI template to derive to create a Sparse GEMINI MLP clustering model.
     When deriving, the only methods to adapt is the _compute_gemini methods which
@@ -239,16 +248,16 @@
             verbose=verbose,
             random_state=random_state
         )
         self.M = M
         self.alpha = alpha
         self.groups = groups
 
-    def _init_params(self, random_state):
-        super()._init_params(random_state)
+    def _init_params(self, random_state, X=None):
+        super()._init_params(random_state, X)
         threshold = np.sqrt(1 / self.n_features_in_)
         self.W_skip_ = random_state.uniform(-threshold, threshold, size=(self.n_features_in_, self.n_clusters))
 
     def _infer(self, X, retain=True):
         H = np.maximum(X @ self.W1_ + self.b1_, 0)
         output_network = H @ self.W2_ + self.b2_
         output_skip = X @ self.W_skip_
@@ -315,15 +324,15 @@
 
     def path(self, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9, restore_best_weights=True,
              early_stopping_factor=0.99, max_patience=10):
         """
         Unfold the progressive geometric increase of the penalty weight starting from the initial alpha until
         there remains only a specified amount of features.
 
-        The history of the different gemclus scores are kept as well as the best weights with minimum of features
+        The history of the different gemini scores are kept as well as the best weights with minimum of features
         ensuring that the GEMINI score remains at a certain percentage of the maximum GEMINI score seen during the
         path.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Test samples on which the feature reduction will be made.
@@ -337,23 +346,23 @@
         restore_best_weights: bool, default=True
             After performing the path, the best weights offering simultaneously good GEMINI score and few features
             are restored to the model.
         early_stopping_factor: float, default=0.99
             The percentage factor beyond which upgrades of the GEMINI or the group-lasso penalty are considered
             too small for early stopping.
         max_patience:
-            The maximum number of iterations to wait without any improvements in either the gemclus score or the
+            The maximum number of iterations to wait without any improvements in either the gemini score or the
             group-lasso penalty before stopping the current step.
 
         Returns
         -------
         best_weights: list of ndarray of various shapes of length 5
             The list containing the best weights during the path. Sequentially: `W1_`, `W2_`, `W_skip_`, `b1_`, `b2_`
         geminis: list of float of length T
-            The history of the gemclus scores as the penalty alpha was increased.
+            The history of the gemini scores as the penalty alpha was increased.
         group_penalties: list of float of length T
             The history of the group-lasso penalties
         alphas: list of float of length T
             The history of the penalty alphas during the path.
         n_features: list of float of length T
             The number of features that were selected at step t.
         """
@@ -481,15 +490,15 @@
 
     def path(self, X, alpha_multiplier=1.05, min_features=2, keep_threshold=0.9, restore_best_weights=True,
              early_stopping_factor=0.99, max_patience=10):
         """
         Unfold the progressive geometric increase of the penalty weight starting from the initial alpha until
         there remains only a specified amount of features.
 
-        The history of the different gemclus scores are kept as well as the best weights with minimum of features
+        The history of the different gemini scores are kept as well as the best weights with minimum of features
         ensuring that the GEMINI score remains at a certain percentage of the maximum GEMINI score seen during the
         path.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Test samples on which the feature reduction will be made.
@@ -503,23 +512,23 @@
         restore_best_weights: bool, default=True
             After performing the path, the best weights offering simultaneously good GEMINI score and few features
             are restored to the model.
         early_stopping_factor: float, default=0.99
             The percentage factor beyond which upgrades of the GEMINI or the group-lasso penalty are considered
             too small for early stopping.
         max_patience:
-            The maximum number of iterations to wait without any improvements in either the gemclus score or the
+            The maximum number of iterations to wait without any improvements in either the gemini score or the
             group-lasso penalty before stopping the current step.
 
         Returns
         -------
         best_weights: list of ndarray of various shapes of length 5
             The list containing the best weights during the path. Sequentially: `W_`, `b_`
         geminis: list of float of length T
-            The history of the gemclus scores as the penalty alpha was increased.
+            The history of the gemini scores as the penalty alpha was increased.
         group_penalties: list of float of length T
             The history of the group-lasso penalties
         alphas: list of float of length T
             The history of the penalty alphas during the path.
         n_features: list of float of length T
             The number of features that were selected at step t.
         """
```

### Comparing `gemclus-0.0.2/gemclus/sparse/_linear_sparse.py` & `gemclus-0.1.0/gemclus/sparse/_linear_sparse.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.0.2/gemclus/sparse/_mlp_sparse.py` & `gemclus-0.1.0/gemclus/sparse/_mlp_sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     >>> X,y=load_iris(return_X_y=True)
     >>> clf = SparseMLPMMD(random_state=0).fit(X)
     >>> clf.predict(X[:2,:])
     array([0, 0])
     >>> clf.predict_proba(X[:2,:]).shape
     (2, 3)
     >>> clf.score(X)
-    1.7664211836410726
+    1.766421183641077
     """
     _parameter_constraints: dict = {
         **_SparseMLPGEMINI._parameter_constraints,
     }
 
     def __init__(self, n_clusters=3, groups=None, max_iter=1000, learning_rate=1e-3, n_hidden_dim=20, kernel="linear",
                  M=10, batch_size=None, alpha=1e-2, ovo=False, solver="adam", verbose=False, random_state=None):
```

### Comparing `gemclus-0.0.2/gemclus/tests/test_data.py` & `gemclus-0.1.0/gemclus/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gemclus-0.0.2/gemclus/tests/test_default.py` & `gemclus-0.1.0/gemclus/tests/test_default.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import pytest
 from sklearn.datasets import load_iris
 from sklearn.utils.estimator_checks import check_estimator
-from sklearn.utils.estimator_checks import check_clustering
+from sklearn.utils.estimator_checks import check_clustering, check_methods_sample_order_invariance,\
+    check_methods_subset_invariance
 
 from ..linear import LinearWasserstein, LinearMMD, RIM
 from ..mlp import MLPMMD, MLPWasserstein
+from ..nonparametric import CategoricalWasserstein, CategoricalMMD
+from ..nonparametric._categorical_models import _CategoricalGEMINI
 from ..sparse import SparseMLPMMD, SparseLinearMMD
 
 
 @pytest.fixture
 def data():
     X, y = load_iris(return_X_y=True)
     return X
 
 
 @pytest.mark.parametrize(
     "clf",
-    [LinearMMD(), MLPMMD(), LinearWasserstein(), MLPWasserstein(), SparseLinearMMD(), SparseMLPMMD(), RIM()]
+    [LinearMMD(), MLPMMD(), LinearWasserstein(), MLPWasserstein(), SparseLinearMMD(), SparseMLPMMD(), RIM(),
+     CategoricalMMD(), CategoricalWasserstein()]
 )
 def test_default_clf_init(clf):
     assert clf.learning_rate == 1e-3
     assert clf.n_clusters == 3
     assert clf.max_iter == 1000
     assert clf.random_state is None
     assert clf.solver == "adam"
@@ -35,14 +39,26 @@
     clf.fit(data)
     assert hasattr(clf, 'W_')
     assert hasattr(clf, 'b_')
     assert hasattr(clf, 'optimiser_')
     assert hasattr(clf, 'labels_')
     assert hasattr(clf, 'n_iter_')
 
+@pytest.mark.parametrize(
+    "clf",
+    [CategoricalMMD, CategoricalWasserstein]
+)
+def test_all_categorical_attributes(clf, data):
+    clf = clf(max_iter=1)
+    clf.fit(data)
+    assert hasattr(clf, 'logits_')
+    assert hasattr(clf, 'optimiser_')
+    assert hasattr(clf, 'labels_')
+    assert hasattr(clf, 'n_iter_')
+
 
 @pytest.mark.parametrize(
     "clf",
     [MLPMMD, MLPWasserstein, SparseMLPMMD]
 )
 def test_all_mlp_attributes(clf, data):
     clf = clf(max_iter=1)
@@ -77,24 +93,24 @@
 def test_all_sparse_linear_attributes(clf, data):
     clf = clf(max_iter=1)
     assert clf.alpha == 1e-2
 
 
 @pytest.mark.parametrize(
     "clf",
-    [LinearMMD(), MLPMMD(), SparseMLPMMD(), SparseLinearMMD()]
+    [LinearMMD(), MLPMMD(), SparseMLPMMD(), SparseLinearMMD(), CategoricalMMD()]
 )
 def test_default_mmd(clf):
     assert clf.kernel == "linear"
     assert not clf.ovo
 
 
 @pytest.mark.parametrize(
     "clf",
-    [LinearWasserstein(), MLPWasserstein()]
+    [LinearWasserstein(), MLPWasserstein(), CategoricalWasserstein()]
 )
 def test_default_wasserstein(clf):
     assert clf.metric == "euclidean"
     assert not clf.ovo
 
 
 @pytest.mark.parametrize(
@@ -105,14 +121,27 @@
 def test_all_estimators(estimator):
     check_iterator = check_estimator(estimator, generate_only=True)
     for clf, check in check_iterator:
         if check.func == check_clustering:
             # The check clustering function tests if we output as many clusters as promised,
             # But since GEMINI may have fewer clusters, this test will never be satisfied
             continue
+        if check.func == check_methods_sample_order_invariance and isinstance(estimator, _CategoricalGEMINI):
+            continue
+        check(clf)
+
+@pytest.mark.parametrize(
+    "estimator",
+    [CategoricalMMD(max_iter=5), CategoricalWasserstein(max_iter=5)]
+)
+def test_categorical_estimators(estimator):
+    check_iterator = check_estimator(estimator, generate_only=True)
+    for clf, check in check_iterator:
+        if check.func in [check_clustering, check_methods_sample_order_invariance, check_methods_subset_invariance]:
+            continue
         check(clf)
 
 @pytest.mark.parametrize(
     "estimator",
     [MLPMMD, LinearMMD, SparseMLPMMD, SparseLinearMMD, MLPWasserstein, LinearWasserstein, RIM]
 )
 @pytest.mark.parametrize(
```

### Comparing `gemclus-0.0.2/gemclus/tests/test_path.py` & `gemclus-0.1.0/gemclus/tests/test_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,18 @@
         assert np.allclose(best_weights[i], best_weights_v2[i])
     assert np.allclose(geminis, geminis_v2)
     assert np.allclose(alphas, alphas_v2)
     assert np.allclose(n_features, n_features_v2)
 
     gemini_score = clf.score(data)
 
-    assert gemini_score >= 0.9 * max(geminis)
+    # Locate the scores when using all features
+    full_feature_models = np.where(np.array(n_features) == data.shape[1])[0]
+
+    assert gemini_score >= 0.9 * max(np.array(geminis)[full_feature_models])
 
 
 def test_weights_coherence(data):
     clf = SparseMLPMMD(random_state=0)
 
     best_weights, geminis, penalties, alphas, n_features = clf.path(data, restore_best_weights=False)
 
@@ -136,16 +139,17 @@
     for i in range(len(best_weights_v1)):
         assert np.allclose(best_weights_v1[i], best_weights_v2[i])
 
     assert np.allclose(np.array(geminis_v1), np.array(geminis_v2))
     assert np.allclose(np.array(alphas_v1), np.array(alphas_v2))
     assert np.allclose(np.array(n_features_v1), np.array(n_features_v2))
 
+
 @pytest.mark.parametrize(
     "clf_class",
     [SparseMLPMMD, SparseLinearMMD]
 )
 def test_batch_path(clf_class, data):
     clf = clf_class(batch_size=50, random_state=0, max_iter=100)
 
     best_weights_v1, geminis_v1, penalties_v1, alphas_v1, n_features_v1 = clf.path(data, restore_best_weights=False,
-                                                                                   min_features=data.shape[1]-1)
+                                                                                   min_features=data.shape[1] - 1)
```

### Comparing `gemclus-0.0.2/gemclus.egg-info/PKG-INFO` & `gemclus-0.1.0/gemclus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemclus
-Version: 0.0.2
+Version: 0.1.0
 Summary: A package for performing discriminative clustering with gemini-trained models
 Home-page: https://github.com/gemini-clustering
 Download-URL: https://github.com/gemini-clustering
 Maintainer: Louis Ohl
 Maintainer-email: louis.ohl@inria.fr
 License: GPLv3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gemclus-0.0.2/gemclus.egg-info/SOURCES.txt` & `gemclus-0.1.0/gemclus.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 gemclus/_base_gemini.py
 gemclus.egg-info/PKG-INFO
 gemclus.egg-info/SOURCES.txt
 gemclus.egg-info/dependency_links.txt
 gemclus.egg-info/not-zip-safe
 gemclus.egg-info/requires.txt
 gemclus.egg-info/top_level.txt
-gemclus/_gemini_grads/__init__.py
-gemclus/_gemini_grads/_gemini_losses.py
-gemclus/_gemini_grads/_prox_grad.py
 gemclus/data/__init__.py
 gemclus/data/synthetic_data.py
+gemclus/gemini/__init__.py
+gemclus/gemini/_gemini_losses.py
 gemclus/linear/__init__.py
 gemclus/linear/_linear_geminis.py
 gemclus/mlp/__init__.py
 gemclus/mlp/_mlp_geminis.py
+gemclus/nonparametric/__init__.py
+gemclus/nonparametric/_categorical_models.py
 gemclus/sparse/__init__.py
 gemclus/sparse/_base_sparse.py
 gemclus/sparse/_linear_sparse.py
 gemclus/sparse/_mlp_sparse.py
+gemclus/sparse/_prox_grad.py
 gemclus/tests/__init__.py
 gemclus/tests/test_data.py
 gemclus/tests/test_default.py
 gemclus/tests/test_objectives.py
 gemclus/tests/test_path.py
```

### Comparing `gemclus-0.0.2/setup.py` & `gemclus-0.1.0/setup.py`

 * *Files identical despite different names*

