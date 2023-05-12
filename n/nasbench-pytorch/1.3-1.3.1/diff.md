# Comparing `tmp/nasbench_pytorch-1.3.tar.gz` & `tmp/nasbench_pytorch-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasbench_pytorch-1.3.tar", last modified: Mon Dec  5 10:56:00 2022, max compression
+gzip compressed data, was "nasbench_pytorch-1.3.1.tar", last modified: Fri May 12 12:03:18 2023, max compression
```

## Comparing `nasbench_pytorch-1.3.tar` & `nasbench_pytorch-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxr-xr-x   0 gabi      (1000) gabi      (1000)        0 2022-12-05 10:56:00.867383 nasbench_pytorch-1.3/
--rw-r--r--   0 gabi      (1000) gabi      (1000)     2594 2022-11-25 10:07:58.000000 nasbench_pytorch-1.3/.gitignore
--rw-r--r--   0 gabi      (1000) gabi      (1000)      549 2022-12-05 10:36:57.000000 nasbench_pytorch-1.3/Contributors.md
--rw-r--r--   0 gabi      (1000) gabi      (1000)    11357 2022-06-30 11:52:44.000000 nasbench_pytorch-1.3/LICENSE.txt
--rw-r--r--   0 gabi      (1000) gabi      (1000)     4258 2022-12-05 10:56:00.867383 nasbench_pytorch-1.3/PKG-INFO
--rw-r--r--   0 gabi      (1000) gabi      (1000)     4063 2022-12-05 10:53:39.000000 nasbench_pytorch-1.3/README.md
-drwxr-xr-x   0 gabi      (1000) gabi      (1000)        0 2022-12-05 10:56:00.857383 nasbench_pytorch-1.3/assets/
--rw-r--r--   0 gabi      (1000) gabi      (1000)    40780 2022-06-30 11:47:23.000000 nasbench_pytorch-1.3/assets/architecture.png
--rw-r--r--   0 gabi      (1000) gabi      (1000)   127555 2022-06-30 11:47:23.000000 nasbench_pytorch-1.3/assets/param_time_acc.png
--rw-r--r--   0 gabi      (1000) gabi      (1000)     6340 2022-12-05 10:09:51.000000 nasbench_pytorch-1.3/main.py
-drwxr-xr-x   0 gabi      (1000) gabi      (1000)        0 2022-12-05 10:56:00.857383 nasbench_pytorch-1.3/nasbench_pytorch/
--rw-r--r--   0 gabi      (1000) gabi      (1000)        0 2022-06-30 11:47:23.000000 nasbench_pytorch-1.3/nasbench_pytorch/__init__.py
-drwxr-xr-x   0 gabi      (1000) gabi      (1000)        0 2022-12-05 10:56:00.867383 nasbench_pytorch-1.3/nasbench_pytorch/datasets/
--rw-r--r--   0 gabi      (1000) gabi      (1000)        0 2022-06-30 11:47:23.000000 nasbench_pytorch-1.3/nasbench_pytorch/datasets/__init__.py
--rw-r--r--   0 gabi      (1000) gabi      (1000)     5809 2022-12-05 10:27:42.000000 nasbench_pytorch-1.3/nasbench_pytorch/datasets/cifar10.py
-drwxr-xr-x   0 gabi      (1000) gabi      (1000)        0 2022-12-05 10:56:00.867383 nasbench_pytorch-1.3/nasbench_pytorch/model/
--rw-r--r--   0 gabi      (1000) gabi      (1000)       93 2022-06-30 11:47:23.000000 nasbench_pytorch-1.3/nasbench_pytorch/model/__init__.py
--rw-r--r--   0 gabi      (1000) gabi      (1000)     1941 2022-11-10 12:47:05.000000 nasbench_pytorch-1.3/nasbench_pytorch/model/base_ops.py
--rw-r--r--   0 gabi      (1000) gabi      (1000)     5533 2022-06-30 11:47:23.000000 nasbench_pytorch-1.3/nasbench_pytorch/model/graph_util.py
--rw-r--r--   0 gabi      (1000) gabi      (1000)    10443 2022-12-05 10:26:58.000000 nasbench_pytorch-1.3/nasbench_pytorch/model/model.py
--rw-r--r--   0 gabi      (1000) gabi      (1000)     5819 2022-10-10 12:08:07.000000 nasbench_pytorch-1.3/nasbench_pytorch/model/model_spec.py
--rw-r--r--   0 gabi      (1000) gabi      (1000)     5465 2022-12-05 10:02:26.000000 nasbench_pytorch-1.3/nasbench_pytorch/trainer.py
-drwxr-xr-x   0 gabi      (1000) gabi      (1000)        0 2022-12-05 10:56:00.867383 nasbench_pytorch-1.3/nasbench_pytorch.egg-info/
--rw-r--r--   0 gabi      (1000) gabi      (1000)     4258 2022-12-05 10:56:00.000000 nasbench_pytorch-1.3/nasbench_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 gabi      (1000) gabi      (1000)      593 2022-12-05 10:56:00.000000 nasbench_pytorch-1.3/nasbench_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 gabi      (1000) gabi      (1000)        1 2022-12-05 10:56:00.000000 nasbench_pytorch-1.3/nasbench_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 gabi      (1000) gabi      (1000)       17 2022-12-05 10:56:00.000000 nasbench_pytorch-1.3/nasbench_pytorch.egg-info/top_level.txt
--rw-r--r--   0 gabi      (1000) gabi      (1000)      159 2022-12-05 10:56:00.867383 nasbench_pytorch-1.3/setup.cfg
--rw-r--r--   0 gabi      (1000) gabi      (1000)      209 2022-12-05 09:52:23.000000 nasbench_pytorch-1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 12:03:18.254732 nasbench_pytorch-1.3.1/
+-rwxrwxrwx   0 root         (0) root         (0)    11357 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)     4260 2023-05-12 12:03:18.254806 nasbench_pytorch-1.3.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4063 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 12:03:18.252144 nasbench_pytorch-1.3.1/nasbench_pytorch/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 12:03:18.253351 nasbench_pytorch-1.3.1/nasbench_pytorch/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5834 2023-05-12 09:34:28.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/datasets/cifar10.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 12:03:18.254545 nasbench_pytorch-1.3.1/nasbench_pytorch/model/
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/model/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1941 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/model/base_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     5533 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/model/graph_util.py
+-rwxrwxrwx   0 root         (0) root         (0)    10443 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/model/model.py
+-rwxrwxrwx   0 root         (0) root         (0)     5819 2023-05-12 09:27:20.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/model/model_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     5474 2023-05-12 11:55:46.000000 nasbench_pytorch-1.3.1/nasbench_pytorch/trainer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 12:03:18.252979 nasbench_pytorch-1.3.1/nasbench_pytorch.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4260 2023-05-12 12:03:18.000000 nasbench_pytorch-1.3.1/nasbench_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-05-12 12:03:18.000000 nasbench_pytorch-1.3.1/nasbench_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-12 12:03:18.000000 nasbench_pytorch-1.3.1/nasbench_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-05-12 12:03:18.000000 nasbench_pytorch-1.3.1/nasbench_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      159 2023-05-12 12:03:18.255082 nasbench_pytorch-1.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      211 2023-05-12 12:02:53.000000 nasbench_pytorch-1.3.1/setup.py
```

### Comparing `nasbench_pytorch-1.3/LICENSE.txt` & `nasbench_pytorch-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nasbench_pytorch-1.3/PKG-INFO` & `nasbench_pytorch-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasbench_pytorch
-Version: 1.3
+Version: 1.3.1
 Author: Romulus Hong, Gabriela Kadlecová
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NASBench-PyTorch
 NASBench-PyTorch is a PyTorch implementation of the search space
```

### Comparing `nasbench_pytorch-1.3/README.md` & `nasbench_pytorch-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch/datasets/cifar10.py` & `nasbench_pytorch-1.3.1/nasbench_pytorch/datasets/cifar10.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                                                    sampler=train_sampler, num_workers=num_workers,
                                                    worker_init_fn=worker_fn)
         valid_loader = torch.utils.data.DataLoader(valid_set, batch_size=batch_size, shuffle=False,
                                                    sampler=valid_sampler, num_workers=num_val_workers,
                                                    worker_init_fn=worker_fn)
     else:
         train_loader = torch.utils.data.DataLoader(train_set, batch_size=batch_size, shuffle=True,
-                                                   worker_init_fn=worker_fn)
+                                                   num_workers=num_workers, worker_init_fn=worker_fn)
         valid_loader = None
 
     test_set = torchvision.datasets.CIFAR10(root=root, train=False, download=True, transform=test_transform)
     test_loader = torch.utils.data.DataLoader(test_set, batch_size=test_batch_size, shuffle=False,
                                               num_workers=num_test_workers, worker_init_fn=worker_fn)
     test_size = len(test_set)
```

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch/model/base_ops.py` & `nasbench_pytorch-1.3.1/nasbench_pytorch/model/base_ops.py`

 * *Files identical despite different names*

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch/model/graph_util.py` & `nasbench_pytorch-1.3.1/nasbench_pytorch/model/graph_util.py`

 * *Files identical despite different names*

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch/model/model.py` & `nasbench_pytorch-1.3.1/nasbench_pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch/model/model_spec.py` & `nasbench_pytorch-1.3.1/nasbench_pytorch/model/model_spec.py`

 * *Files identical despite different names*

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch/trainer.py` & `nasbench_pytorch-1.3.1/nasbench_pytorch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 
     # defaults
     if loss is None:
         loss = nn.CrossEntropyLoss()
 
     if optimizer is not None and not isinstance(optimizer, str):
         pass
-    elif optimizer is None or optimizer.lower() == 'sgd':
+    elif optimizer is None or optimizer.lower() == 'rmsprop':
+        optimizer = torch.optim.RMSprop(net.parameters(), lr=0.2, momentum=0.9, weight_decay=1e-4, eps=1.0)
+    elif optimizer.lower() == 'sgd':
         optimizer = torch.optim.SGD(net.parameters(), lr=0.025, momentum=0.9, weight_decay=1e-4)
-    elif optimizer.lower() == 'rmsprop':
-        optimizer = torch.optim.RMSprop(net.parameters(), lr=0.2, momentum=0.9, weight_decay=1e-4)
     elif optimizer.lower() == 'adam':
         optimizer = torch.optim.Adam(net.parameters())
 
     if scheduler is None:
         scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(optimizer, num_epochs)
 
     # training
```

### Comparing `nasbench_pytorch-1.3/nasbench_pytorch.egg-info/PKG-INFO` & `nasbench_pytorch-1.3.1/nasbench_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasbench-pytorch
-Version: 1.3
+Version: 1.3.1
 Author: Romulus Hong, Gabriela Kadlecová
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NASBench-PyTorch
 NASBench-PyTorch is a PyTorch implementation of the search space
```

