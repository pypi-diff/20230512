# Comparing `tmp/redcat-0.0.1a165.tar.gz` & `tmp/redcat-0.0.1a182.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.1a165.tar", max compression
+gzip compressed data, was "redcat-0.0.1a182.tar", max compression
```

## Comparing `redcat-0.0.1a165.tar` & `redcat-0.0.1a182.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1501 2023-05-09 06:36:50.921476 redcat-0.0.1a165/LICENSE
--rw-r--r--   0        0        0     1457 2023-05-09 06:36:50.921476 redcat-0.0.1a165/README.md
--rw-r--r--   0        0        0     3670 2023-05-09 06:36:50.925476 redcat-0.0.1a165/pyproject.toml
--rw-r--r--   0        0        0      227 2023-05-09 06:36:50.925476 redcat-0.0.1a165/src/redcat/__init__.py
--rw-r--r--   0        0        0    18686 2023-05-09 06:36:50.925476 redcat-0.0.1a165/src/redcat/base.py
--rw-r--r--   0        0        0     2428 2023-05-09 06:36:50.925476 redcat-0.0.1a165/src/redcat/comparators.py
--rw-r--r--   0        0        0   123157 2023-05-09 06:36:50.925476 redcat-0.0.1a165/src/redcat/tensor.py
--rw-r--r--   0        0        0    47982 2023-05-09 06:36:50.925476 redcat-0.0.1a165/src/redcat/tensorseq.py
--rw-r--r--   0        0        0    12060 2023-05-09 06:36:50.925476 redcat-0.0.1a165/src/redcat/utils.py
--rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 redcat-0.0.1a165/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-12 13:45:55.644109 redcat-0.0.1a182/LICENSE
+-rw-r--r--   0        0        0     1594 2023-05-12 13:45:55.648110 redcat-0.0.1a182/README.md
+-rw-r--r--   0        0        0     4382 2023-05-12 13:45:55.648110 redcat-0.0.1a182/pyproject.toml
+-rw-r--r--   0        0        0      227 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/__init__.py
+-rw-r--r--   0        0        0    18686 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/base.py
+-rw-r--r--   0        0        0     2428 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/comparators.py
+-rw-r--r--   0        0        0   128571 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/tensor.py
+-rw-r--r--   0        0        0    51342 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0    12134 2023-05-12 13:45:55.648110 redcat-0.0.1a182/src/redcat/utils.py
+-rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 redcat-0.0.1a182/PKG-INFO
```

### Comparing `redcat-0.0.1a165/LICENSE` & `redcat-0.0.1a182/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a165/README.md` & `redcat-0.0.1a182/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,7 +27,15 @@
         <img  alt="Downloads" src="https://static.pepy.tech/badge/redcat">
     </a>
     <a href="https://pepy.tech/project/redcat">
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/redcat/month">
     </a>
     <br/>
 </p>
+
+<p align="center">
+<img height="242" src="assets/redcat.png" alt="logo"/>
+</p>
+
+---
+
+*The logo was generated with Stable Diffusion 2.1*
```

#### html2text {}

```diff
@@ -1,4 +1,6 @@
 # redcat
 [CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
                                 style:_google]
                        [Downloads] [Monthly_downloads]
+                                    [logo]
+--- *The logo was generated with Stable Diffusion 2.1*
```

### Comparing `redcat-0.0.1a165/pyproject.toml` & `redcat-0.0.1a182/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.1a165"
+version = "0.0.1a182"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
-keywords = ["redcat"]
+keywords = ["batch"]
+license = "BSD-3-Clause"
+
+classifiers = [
+    "Development Status :: 2 - Pre-Alpha",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
 
 packages = [
     { include = "redcat", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
 coola = "^0.0.6"
 python = "^3.9"
-torch = "^2.0"
+torch = "^2.0"  # make optional
 numpy = "^1.24"  # make optional
+polars = { version = "^0.17", optional = true }
+
+[tool.poetry.extras]
+all = [
+    "polars",
+]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
 coverage = { extras = ["toml"], version = "^6.5" }
 pre-commit = "^2.21"
 pylint = "^2.17"
 pytest = "^7.3"
```

### Comparing `redcat-0.0.1a165/src/redcat/base.py` & `redcat-0.0.1a182/src/redcat/base.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a165/src/redcat/comparators.py` & `redcat-0.0.1a182/src/redcat/comparators.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1a165/src/redcat/tensor.py` & `redcat-0.0.1a182/src/redcat/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1864,165 +1864,61 @@
             >>> batch.log1p_()
             >>> batch
             tensor([[0.0000, 0.6931, 1.0986, 1.3863, 1.6094],
                     [1.7918, 1.9459, 2.0794, 2.1972, 2.3026]], batch_dim=0)
         """
         self._data.log1p_()
 
-    @overload
-    def max(self) -> bool | int | float:
-        r"""Finds the maximum value in the batch.
-
-        Returns:
-            The maximum value in the batch.
-
-        Example usage:
-
-        .. code-block:: python
-
-            >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
-            >>> batch.max()
-            5
-            >>> batch = BatchedTensor(torch.tensor([[False, True, True], [True, False, True]]))
-            >>> batch.max()
-            True
-        """
-
-    @overload
-    def max(self, other: BatchedTensor) -> TBatchedTensor:
+    def maximum(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise maximum of ``self`` and ``other``.
 
         Args:
-            other (``BatchedTensor``): Specifies a batch.
+            other (``BatchedTensor`` or ``torch.Tensor``): Specifies
+                a batch.
 
         Returns:
             ``BatchedTensor``: The batch with the element-wise
                 maximum of ``self`` and ``other``
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
-            >>> batch.max(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
-            tensor([[1, 1, 2],
-                    [4, 5, 5]], batch_dim=0)
-        """
-
-    def max(
-        self, other: BatchedTensor | Tensor | None = None
-    ) -> bool | int | float | TBatchedTensor:
-        r"""If ``other`` is None, this method finds the maximum value in the
-        batch, otherwise it computes the element-wise maximum of ``self`` and
-        ``other``.
-
-        Args:
-            other (``BatchedTensor`` or ``None``, optional):
-                Specifies a batch. Default: ``None``
-
-        Returns:
-            The maximum value in the batch or the element-wise maximum
-                of ``self`` and ``other``.
-
-        Example usage:
-
-        .. code-block:: python
-
-            >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
-            >>> batch.max()
-            5
-            >>> batch.max(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
+            >>> batch.maximum(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
             tensor([[1, 1, 2],
                     [4, 5, 5]], batch_dim=0)
         """
-        if other is None:
-            return torch.max(self._data)
-        return torch.max(self, other)
-
-    @overload
-    def min(self) -> bool | int | float:
-        r"""Finds the minimum value in the batch.
-
-        Returns:
-            The minimum value in the batch.
-
-        Example usage:
-
-        .. code-block:: python
+        return torch.maximum(self, other)
 
-            >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
-            >>> batch.min()
-            0
-            >>> batch = BatchedTensor(torch.tensor([[False, True, True], [True, False, True]]))
-            >>> batch.min()
-            False
-        """
-
-    @overload
-    def min(self, other: BatchedTensor) -> TBatchedTensor:
+    def minimum(self, other: BatchedTensor | Tensor) -> TBatchedTensor:
         r"""Computes the element-wise minimum of ``self`` and ``other``.
 
         Args:
-            other (``BatchedTensor``): Specifies a batch.
+            other (``BatchedTensor`` or ``torch.Tensor``): Specifies
+                a batch.
 
         Returns:
             ``BatchedTensor``: The batch with the element-wise
                 minimum of ``self`` and ``other``
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
-            >>> batch.min(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
+            >>> batch.minimum(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
             tensor([[0, 0, 2],
                     [3, 4, 3]], batch_dim=0)
         """
-
-    def min(
-        self, other: BatchedTensor | Tensor | None = None
-    ) -> bool | int | float | TBatchedTensor:
-        r"""If ``other`` is None, this method finds the minimum value in the
-        batch, otherwise it computes the element-wise minimum of ``self`` and
-        ``other``.
-
-        Args:
-            other (``BatchedTensor`` or ``None``, optional):
-                Specifies a batch. Default: ``None``
-
-        Returns:
-            The minimum value in the batch or the element-wise minimum
-                of ``self`` and ``other``.
-
-        Example usage:
-
-        .. code-block:: python
-
-            >>> import torch
-            >>> from redcat import BatchedTensor
-            >>> batch = BatchedTensor(torch.arange(6).view(2, 3))
-            >>> batch.min()
-            0
-            >>> batch.min(BatchedTensor(torch.tensor([[1, 0, 2], [4, 5, 3]])))
-            tensor([[0, 0, 2],
-                    [3, 4, 3]], batch_dim=0)
-        """
-        if other is None:
-            return torch.min(self._data)
-        return torch.min(self, other)
+        return torch.minimum(self, other)
 
     def pow(self, exponent: int | float | BatchedTensor) -> TBatchedTensor:
         r"""Computes the power of each element with the given exponent.
 
         Args:
             exponent (int or float or ``BatchedTensor``): Specifies
                 the exponent value. ``exponent`` can be either a single
@@ -2149,14 +2045,163 @@
         """
         self._data.sqrt_()
 
     ################################
     #     Reduction operations     #
     ################################
 
+    def mean(self, *args, **kwargs) -> Tensor:
+        r"""Computes the mean of all elements.
+
+        Args:
+            *args: See the documentation of ``torch.Tensor.mean``
+            **kwargs: See the documentation of ``torch.Tensor.mean``
+
+        Returns:
+            ``torch.Tensor``: The mean of all elements.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean()
+            tensor(4.5)
+            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean(dim=1)
+            tensor([2.0, 7.0])
+            >>> BatchedTensor(torch.arange(10).view(2, 5).float()).mean(dim=1, keepdim=True)
+            tensor([[2.0], [7.0]])
+        """
+        return torch.mean(self, *args, **kwargs)
+
+    def mean_along_batch(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the mean values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the batch dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A batch with
+                the mean values along the batch dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_seq()
+            tensor([4.0, 5.0])
+            >>> BatchedTensor(torch.arange(10).view(5, 2).float()).mean_along_seq(keepdim=True)
+            tensor([[4.0], [5.0]])
+        """
+        return self.mean(dim=self._batch_dim, keepdim=keepdim)
+
+    def nanmean(self, *args, **kwargs) -> Tensor:
+        r"""Computes the mean of all elements.
+
+        Args:
+            *args: See the documentation of ``torch.Tensor.nanmean``
+            **kwargs: See the documentation of ``torch.Tensor.nanmean``
+
+        Returns:
+            ``torch.Tensor``: The mean of all elements.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmean()
+            tensor(4.0)
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmean(dim=1)
+            tensor([2.0, 6.5])
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmean(dim=1, keepdim=True)
+            tensor([[2.0], [6.5]])
+        """
+        return torch.nanmean(self, *args, **kwargs)
+
+    def nanmedian(self, *args, **kwargs) -> Tensor | torch.return_types.nanmedian:
+        r"""Computes the median of all elements.
+
+        Args:
+            *args: See the documentation of ``torch.Tensor.nanmedian``
+            **kwargs: See the documentation of ``torch.Tensor.nanmedian``
+
+        Returns:
+            ``torch.Tensor`` or ``torch.return_types.nanmedian``:
+                The median of all elements or per dimension.
+                The first tensor will be populated with the median
+                values and the second tensor, which must have dtype
+                long, with their indices in the dimension dim of input.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmedian()
+            tensor(4.0)
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmedian(dim=1)
+            torch.return_types.nanmedian(
+            values=tensor([2., 6.]),
+            indices=tensor([2, 1]))
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmedian(dim=1, keepdim=True)
+            torch.return_types.nanmedian(
+            values=tensor([[2.], [6.]]),
+            indices=tensor([[2], [1]]))
+        """
+        return torch.nanmedian(self, *args, **kwargs)
+
+    def nanmedian_along_batch(self, keepdim: bool = False) -> torch.return_types.nanmedian:
+        r"""Computes the median values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the sequence dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.return_types.nanmedian``:  The first tensor will
+                be populated with the median values and the second
+                tensor, which must have dtype long, with their indices
+                in the batch dimension of input.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ... ).nanmedian_along_batch()
+            torch.return_types.nanmedian(
+            values=tensor([2., 6.]),
+            indices=tensor([2, 1]))
+        """
+        return self.nanmedian(dim=self._batch_dim, keepdim=keepdim)
+
     def nansum(self, *args, **kwargs) -> Tensor:
         r"""Computes the sum of all elements.
 
         Args:
             *args: See the documentation of ``torch.Tensor.nansum``
             **kwargs: See the documentation of ``torch.Tensor.nansum``
 
@@ -2168,26 +2213,51 @@
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nansum()
-            tensor(36)
+            tensor(36.)
             >>> BatchedTensor(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nansum(dim=1)
-            tensor([10, 26])
+            tensor([10., 26.])
             >>> BatchedTensor(
             ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
             ... ).nansum(dim=1, keepdim=True)
-            tensor([[10], [26]])
+            tensor([[10.], [26.]])
         """
         return torch.nansum(self, *args, **kwargs)
 
+    def nansum_along_batch(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the sum values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the sequence dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A tensor with the sum values along the
+                batch dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0., 5.], [1., 6.], [2., 7.], [3., 8.], [4., float("nan")]])
+            ... ).nansum_along_batch()
+            tensor([20., 26.])
+        """
+        return self.nansum(dim=self._batch_dim, keepdim=keepdim)
+
     def prod(self, *args, **kwargs) -> Tensor:
         r"""Computes the product of all elements.
 
         Args:
             *args: See the documentation of ``torch.Tensor.nansum``
             **kwargs: See the documentation of ``torch.Tensor.nansum``
 
@@ -2211,14 +2281,43 @@
             >>> BatchedTensor(
             ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
             ... ).prod(dim=1, keepdim=True)
             tensor([[ 120], [3024]])
         """
         return torch.prod(self, *args, **kwargs)
 
+    def prod_along_batch(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the product values along the batch dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the batch dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A batch with
+                the product values along the batch dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])
+            ... ).prod_along_batch()
+            tensor([ 120, 3024])
+            >>> BatchedTensor(
+            ...     torch.tensor([[1, 6], [2, 7], [3, 8], [4, 9], [5, 1]])
+            ... ).prod_along_batch(keepdim=True)
+            tensor([[ 120, 3024]])
+        """
+        return self.prod(dim=self._batch_dim, keepdim=keepdim)
+
     def sum(self, *args, **kwargs) -> Tensor:
         r"""Computes the sum of all elements.
 
         Args:
             *args: See the documentation of ``torch.Tensor.sum``
             **kwargs: See the documentation of ``torch.Tensor.sum``
 
@@ -2241,32 +2340,31 @@
         return torch.sum(self, *args, **kwargs)
 
     def sum_along_batch(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the batch dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
-                the sequence dimension retained or not. If ``False``
-                the returned type is ``BatchedTensor``, otherwise it
-                is ``BatchedTensorSeq``. Default: ``False``
+                the sequence dimension retained or not.
+                Default: ``False``
 
         Returns:
             ``torch.Tensor``: A tensor with the sum values along the
                 batch dimension.
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensor
             >>> BatchedTensor(torch.arange(10).view(5, 2)).sum_along_batch()
             tensor([20, 25])
         """
-        return torch.sum(self._data, dim=self._batch_dim, keepdim=keepdim)
+        return self.sum(dim=self._batch_dim, keepdim=keepdim)
 
     ###########################################
     #     Mathematical | trigo operations     #
     ###########################################
 
     def acos(self) -> TBatchedTensor:
         r"""Computes the inverse cosine (arccos) of each element.
@@ -3601,28 +3699,64 @@
     r"""See ``torch.chunk`` documentation."""
     return tuple(
         BatchedTensor(chunk, batch_dim=tensor.batch_dim)
         for chunk in tensor.data.chunk(chunks, dim=dim)
     )
 
 
+# Use the name `torchmax` to avoid shadowing `max` python builtin.
+@implements(torch.max)
+def torchmax(
+    input: BatchedTensor, *args, **kwargs  # noqa: A002
+) -> Tensor | torch.return_types.max:
+    r"""See ``torch.max`` documentation."""
+    return torch.max(input.data, *args, **kwargs)
+
+
+@implements(torch.maximum)
+def maximum(input: BatchedTensor, other: BatchedTensor | Tensor) -> BatchedTensor:  # noqa: A002
+    r"""See ``torch.maximum`` documentation."""
+    check_batch_dims(get_batch_dims((input, other)))
+    if isinstance(other, BatchedTensor):
+        other = other.data
+    return BatchedTensor(torch.maximum(input.data, other), batch_dim=input.batch_dim)
+
+
 @implements(torch.mean)
 def mean(input: BatchedTensor, *args, **kwargs) -> Tensor:  # noqa: A002
     r"""See ``torch.mean`` documentation."""
     return torch.mean(input.data, *args, **kwargs)
 
 
 @implements(torch.median)
 def median(
     input: BatchedTensor, *args, **kwargs  # noqa: A002
 ) -> Tensor | torch.return_types.median:
     r"""See ``torch.median`` documentation."""
     return torch.median(input.data, *args, **kwargs)
 
 
+# Use the name `torchmin` to avoid shadowing `min` python builtin.
+@implements(torch.min)
+def torchmin(
+    input: BatchedTensor, *args, **kwargs  # noqa: A002
+) -> Tensor | torch.return_types.min:
+    r"""See ``torch.min`` documentation."""
+    return torch.min(input.data, *args, **kwargs)
+
+
+@implements(torch.minimum)
+def minimum(input: BatchedTensor, other: BatchedTensor | Tensor) -> BatchedTensor:  # noqa: A002
+    r"""See ``torch.minimum`` documentation."""
+    check_batch_dims(get_batch_dims((input, other)))
+    if isinstance(other, BatchedTensor):
+        other = other.data
+    return BatchedTensor(torch.minimum(input.data, other), batch_dim=input.batch_dim)
+
+
 @implements(torch.nanmean)
 def nanmean(input: BatchedTensor, *args, **kwargs) -> Tensor:  # noqa: A002
     r"""See ``torch.nanmean`` documentation."""
     return torch.nanmean(input.data, *args, **kwargs)
 
 
 @implements(torch.nanmedian)
```

### Comparing `redcat-0.0.1a165/src/redcat/tensorseq.py` & `redcat-0.0.1a182/src/redcat/tensorseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     check_seq_dims,
     compute_batch_seq_permutation,
     get_batch_dims,
     get_seq_dims,
 )
 
 HANDLED_FUNCTIONS = {
+    torch.max: tensor.torchmax,
     torch.mean: tensor.mean,
     torch.median: tensor.median,
+    torch.min: tensor.torchmin,
     torch.nanmean: tensor.nanmean,
     torch.nanmedian: tensor.nanmedian,
     torch.nansum: tensor.nansum,
     torch.prod: tensor.prod,
     torch.sum: tensor.torchsum,
 }
 
@@ -639,31 +641,20 @@
 
         Example usage:
 
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
-            >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).mean_along_seq()
-            (tensor([2, 7], batch_dim=0), tensor([2, 2], batch_dim=0))
-            >>> BatchedTensorSeq(torch.arange(30).view(2, 5, 3)).mean_along_seq(keepdim=True)
-            (tensor([[[12, 13, 14]], [[27, 28, 29]]], batch_dim=0, seq_dim=1),
-             tensor([[[4, 4, 4]], [[4, 4, 4]]], batch_dim=0, seq_dim=1))
+            >>> BatchedTensorSeq(torch.arange(10).view(5, 2).float()).mean_along_seq()
+            tensor([2.0, 7.0])
+            >>> BatchedTensorSeq(torch.arange(10).view(5, 2).float()).mean_along_seq(keepdim=True)
+            tensor([[2.0], [7.0]])
         """
-        values = torch.mean(
-            self._data if self._data.is_floating_point() else self._data.float(),
-            dim=self._seq_dim,
-            keepdim=keepdim,
-        )
-        if keepdim:
-            return BatchedTensorSeq(data=values, **self._get_kwargs())
-        return BatchedTensor(
-            data=values,
-            batch_dim=self._batch_dim if self._seq_dim > self._batch_dim else self._batch_dim - 1,
-        )
+        return self.mean(dim=self._seq_dim, keepdim=keepdim)
 
     def median_along_seq(
         self, keepdim: bool = False
     ) -> tuple[BatchedTensor | BatchedTensorSeq, BatchedTensor | BatchedTensorSeq]:
         r"""Computes the median values along the sequence dimension.
 
         Args:
@@ -735,14 +726,95 @@
             )
         batch_dim = self._batch_dim if self._seq_dim > self._batch_dim else self._batch_dim - 1
         return (
             BatchedTensor(data=values, batch_dim=batch_dim),
             BatchedTensor(data=indices, batch_dim=batch_dim),
         )
 
+    def nanmedian_along_seq(self, keepdim: bool = False) -> torch.return_types.nanmedian:
+        r"""Computes the median values along the sequence dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the sequence dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.return_types.nanmedian``:  The first tensor will
+                be populated with the median values and the second
+                tensor, which must have dtype long, with their indices
+                in the sequence dimension of input.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nanmedian_along_seq()
+            torch.return_types.nanmedian(
+            values=tensor([2., 6.]),
+            indices=tensor([2, 1]))
+        """
+        return self.nanmedian(dim=self._seq_dim, keepdim=keepdim)
+
+    def nansum_along_seq(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the sum values along the sequence dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the sequence dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A tensor with the sum values along the
+                sequence dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(
+            ...     torch.tensor([[0, 1, 2, 3, 4], [5, 6, 7, 8, float("nan")]])
+            ... ).nansum_along_seq()
+            tensor([20., 26.])
+        """
+        return self.nansum(dim=self._seq_dim, keepdim=keepdim)
+
+    def prod_along_seq(self, keepdim: bool = False) -> Tensor:
+        r"""Computes the product values along the sequence dimension.
+
+        Args:
+            keepdim (bool): Indicates whether the output tensor has
+                the sequence dimension retained or not.
+                Default: ``False``
+
+        Returns:
+            ``torch.Tensor``: A batch with
+                the product values along the sequence dimension.
+
+        Example usage:
+
+        .. code-block:: python
+
+            >>> import torch
+            >>> from redcat import BatchedTensor
+            >>> BatchedTensor(torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])).prod_along_seq()
+            tensor([ 120, 3024])
+            >>> BatchedTensor(
+            ...     torch.tensor([[1, 2, 3, 4, 5], [6, 7, 8, 9, 1]])
+            ... ).prod_along_seq(keepdim=True)
+            tensor([[ 120], [3024]])
+        """
+        return self.prod(dim=self._seq_dim, keepdim=keepdim)
+
     def sum_along_seq(self, keepdim: bool = False) -> Tensor:
         r"""Computes the sum values along the sequence dimension.
 
         Args:
             keepdim (bool): Indicates whether the output tensor has
                 the sequence dimension retained or not. If ``False``
                 the returned type is ``BatchedTensor``, otherwise it
@@ -757,15 +829,15 @@
         .. code-block:: python
 
             >>> import torch
             >>> from redcat import BatchedTensorSeq
             >>> BatchedTensorSeq(torch.arange(10).view(2, 5)).sum_along_seq()
             tensor([10, 35])
         """
-        return torch.sum(self._data, dim=self._seq_dim, keepdim=keepdim)
+        return self.sum(dim=self._seq_dim, keepdim=keepdim)
 
     ##########################################################
     #    Indexing, slicing, joining, mutating operations     #
     ##########################################################
 
     def align_as(self, other: BatchedTensorSeq) -> BatchedTensorSeq:
         r"""Aligns the current batch with the batch ``other``.
@@ -1215,14 +1287,42 @@
     r"""See ``torch.chunk`` documentation."""
     return tuple(
         BatchedTensorSeq(chunk, batch_dim=tensor.batch_dim, seq_dim=tensor.seq_dim)
         for chunk in tensor.data.chunk(chunks, dim=dim)
     )
 
 
+@implements(torch.maximum)
+def maximum(
+    input: BatchedTensorSeq, other: BatchedTensor | Tensor  # noqa: A002
+) -> BatchedTensorSeq:
+    r"""See ``torch.maximum`` documentation."""
+    check_batch_dims(get_batch_dims((input, other)))
+    check_seq_dims(get_seq_dims((input, other)))
+    if isinstance(other, BatchedTensor):
+        other = other.data
+    return BatchedTensorSeq(
+        torch.maximum(input.data, other), batch_dim=input.batch_dim, seq_dim=input.seq_dim
+    )
+
+
+@implements(torch.minimum)
+def minimum(
+    input: BatchedTensorSeq, other: BatchedTensor | Tensor  # noqa: A002
+) -> BatchedTensorSeq:
+    r"""See ``torch.minimum`` documentation."""
+    check_batch_dims(get_batch_dims((input, other)))
+    check_seq_dims(get_seq_dims((input, other)))
+    if isinstance(other, BatchedTensor):
+        other = other.data
+    return BatchedTensorSeq(
+        torch.minimum(input.data, other), batch_dim=input.batch_dim, seq_dim=input.seq_dim
+    )
+
+
 @implements(torch.select)
 def select(input: BatchedTensorSeq, dim: int, index: int) -> Tensor:  # noqa: A002
     r"""See ``torch.select`` documentation."""
     return torch.select(input.data, dim=dim, index=index)
 
 
 @implements(torch.sort)
```

### Comparing `redcat-0.0.1a165/src/redcat/utils.py` & `redcat-0.0.1a182/src/redcat/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,16 @@
 
         >>> from redcat.utils import get_available_devices
         >>> get_available_devices()
         ('cpu', 'cuda:0')
     """
     if torch.cuda.is_available():
         return ("cpu", "cuda:0")
+    if torch.backends.mps.is_available():
+        return ("cpu", "mps:0")
     return ("cpu",)
 
 
 def get_batch_dims(args: Iterable[Any], kwargs: Union[Mapping[str, Any], None] = None) -> set[int]:
     r"""Gets the batch dimensions from the inputs.
 
     Args:
```

### Comparing `redcat-0.0.1a165/PKG-INFO` & `redcat-0.0.1a182/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.1a165
+Version: 0.0.1a182
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
-Keywords: redcat
+License: BSD-3-Clause
+Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: all
 Requires-Dist: coola (>=0.0.6,<0.0.7)
 Requires-Dist: numpy (>=1.24,<2.0)
+Requires-Dist: polars (>=0.17,<0.18) ; extra == "all"
 Requires-Dist: torch (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/redcat
 Description-Content-Type: text/markdown
 
 # redcat
 
 <p align="center">
@@ -47,7 +62,15 @@
     </a>
     <a href="https://pepy.tech/project/redcat">
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/redcat/month">
     </a>
     <br/>
 </p>
 
+<p align="center">
+<img height="242" src="assets/redcat.png" alt="logo"/>
+</p>
+
+---
+
+*The logo was generated with Stable Diffusion 2.1*
+
```

#### html2text {}

```diff
@@ -1,12 +1,24 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.1a165 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.1a182 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
-Keywords: redcat Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
-Requires-Python: >=3.9,<4.0 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
+durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
+Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Information Technology Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: coola (>=0.0.6,<0.0.7) Requires-Dist: numpy (>=1.24,<2.0)
-Requires-Dist: torch (>=2.0,<3.0) Project-URL: Repository, https://github.com/
-durandtibo/redcat Description-Content-Type: text/markdown # redcat
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries Provides-Extra: all Requires-Dist: coola
+(>=0.0.6,<0.0.7) Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist: polars
+(>=0.17,<0.18) ; extra == "all" Requires-Dist: torch (>=2.0,<3.0) Project-URL:
+Repository, https://github.com/durandtibo/redcat Description-Content-Type:
+text/markdown # redcat
 [CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
                                 style:_google]
                        [Downloads] [Monthly_downloads]
+                                    [logo]
+--- *The logo was generated with Stable Diffusion 2.1*
```

