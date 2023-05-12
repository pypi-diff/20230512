# Comparing `tmp/cbloss-0.1.0.tar.gz` & `tmp/cbloss-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbloss-0.1.0.tar", last modified: Thu May 11 12:26:32 2023, max compression
+gzip compressed data, was "cbloss-0.2.0.tar", last modified: Fri May 12 05:24:47 2023, max compression
```

## Comparing `cbloss-0.1.0.tar` & `cbloss-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:26:32.891887 cbloss-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 12:26:20.000000 cbloss-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 12:26:20.000000 cbloss-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-11 12:26:32.891887 cbloss-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 12:26:20.000000 cbloss-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:26:32.887886 cbloss-0.1.0/cb_loss/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 12:26:20.000000 cbloss-0.1.0/cb_loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-11 12:26:20.000000 cbloss-0.1.0/cb_loss/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:26:32.891887 cbloss-0.1.0/cbloss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-11 12:26:32.000000 cbloss-0.1.0/cbloss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 12:26:32.000000 cbloss-0.1.0/cbloss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:26:32.000000 cbloss-0.1.0/cbloss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-11 12:26:32.000000 cbloss-0.1.0/cbloss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 12:26:32.000000 cbloss-0.1.0/cbloss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 12:26:20.000000 cbloss-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 12:26:20.000000 cbloss-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 12:26:32.891887 cbloss-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-11 12:26:20.000000 cbloss-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:24:47.513677 cbloss-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 05:24:37.000000 cbloss-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 05:24:37.000000 cbloss-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-12 05:24:47.513677 cbloss-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-12 05:24:37.000000 cbloss-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:24:47.513677 cbloss-0.2.0/cbloss/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 05:24:37.000000 cbloss-0.2.0/cbloss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-12 05:24:37.000000 cbloss-0.2.0/cbloss/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:24:47.513677 cbloss-0.2.0/cbloss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-12 05:24:47.000000 cbloss-0.2.0/cbloss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-12 05:24:47.000000 cbloss-0.2.0/cbloss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:24:47.000000 cbloss-0.2.0/cbloss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 05:24:47.000000 cbloss-0.2.0/cbloss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 05:24:47.000000 cbloss-0.2.0/cbloss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 05:24:37.000000 cbloss-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 05:24:37.000000 cbloss-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-12 05:24:47.513677 cbloss-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-12 05:24:37.000000 cbloss-0.2.0/setup.py
```

### Comparing `cbloss-0.1.0/LICENSE` & `cbloss-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cbloss-0.1.0/cb_loss/loss.py` & `cbloss-0.2.0/cbloss/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     Reference:
     - Lin, T. Y., Goyal, P., Girshick, R., He, K., & Dollár, P. (2017).
       Focal loss for dense object detection. In Proceedings of the IEEE international
       conference on computer vision (pp. 2980-2988).
     - https://arxiv.org/pdf/1708.02002.pdf
 
     Args:
+        num_classes (int) : number of classes
         alpha (float): balancing parameter, default to 1.
         gamma (float): focusing parameter, default to 2.
         reduction (str): reduction method for the loss, either 'mean' or 'sum', default to 'mean'.
 
     Inputs:
         outputs (tensor): model predictions of shape (batch_size, num_classes) for multi-class,
                           or (batch_size, ) for binary-class.
```

### Comparing `cbloss-0.1.0/setup.py` & `cbloss-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def get_requirements():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 def get_version():
     current_dir = os.path.abspath(os.path.dirname(__file__))
-    version_file = os.path.join(current_dir, "cb_loss", "__init__.py")
+    version_file = os.path.join(current_dir, "cbloss", "__init__.py")
     with io.open(version_file, encoding="utf-8") as f:
         return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
 
 
 _DEV_REQUIREMENTS = [
     "black==21.7b0",
     "flake8==3.9.2",
```

