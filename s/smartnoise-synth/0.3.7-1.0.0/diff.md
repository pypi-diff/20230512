# Comparing `tmp/smartnoise-synth-0.3.7.tar.gz` & `tmp/smartnoise-synth-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartnoise-synth-0.3.7.tar", max compression
+gzip compressed data, was "smartnoise-synth-1.0.0.tar", max compression
```

## Comparing `smartnoise-synth-0.3.7.tar` & `smartnoise-synth-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1842 2023-02-18 22:13:33.796789 smartnoise-synth-0.3.7/README.md
--rw-r--r--   0        0        0      638 2023-04-03 15:38:44.460851 smartnoise-synth-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      124 2023-02-18 22:13:34.053257 smartnoise-synth-0.3.7/snsynth/__init__.py
--rw-r--r--   0        0        0      256 2023-02-18 22:13:34.053546 smartnoise-synth-0.3.7/snsynth/aggregate_seeded/__init__.py
--rw-r--r--   0        0        0    12663 2023-02-18 22:13:34.053916 smartnoise-synth-0.3.7/snsynth/aggregate_seeded/aggregate_seeded.py
--rw-r--r--   0        0        0       63 2023-02-18 22:13:34.054165 smartnoise-synth-0.3.7/snsynth/aim/__init__.py
--rw-r--r--   0        0        0     8842 2023-02-19 02:22:28.642687 smartnoise-synth-0.3.7/snsynth/aim/aim.py
--rw-r--r--   0        0        0    15963 2023-02-18 22:13:34.054436 smartnoise-synth-0.3.7/snsynth/base.py
--rw-r--r--   0        0        0      115 2023-02-18 22:13:34.054909 smartnoise-synth-0.3.7/snsynth/definitions.py
--rw-r--r--   0        0        0       84 2023-02-18 22:13:34.055020 smartnoise-synth-0.3.7/snsynth/models/__init__.py
--rw-r--r--   0        0        0    16650 2023-02-18 22:13:34.055117 smartnoise-synth-0.3.7/snsynth/models/dp_covariance.py
--rw-r--r--   0        0        0     2929 2023-02-18 22:13:34.055183 smartnoise-synth-0.3.7/snsynth/models/linear_regression.py
--rw-r--r--   0        0        0    11356 2023-02-18 22:13:34.055477 smartnoise-synth-0.3.7/snsynth/mst/LICENSE
--rw-r--r--   0        0        0       63 2023-02-18 22:13:34.055673 smartnoise-synth-0.3.7/snsynth/mst/__init__.py
--rw-r--r--   0        0        0     8486 2023-02-19 02:22:28.642836 smartnoise-synth-0.3.7/snsynth/mst/mst.py
--rw-r--r--   0        0        0       65 2023-02-18 22:13:34.055850 smartnoise-synth-0.3.7/snsynth/mst/test-domain.json
--rw-r--r--   0        0        0    28241 2023-02-18 22:13:34.056031 smartnoise-synth-0.3.7/snsynth/mwem.py
--rw-r--r--   0        0        0       91 2023-02-18 22:13:34.056148 smartnoise-synth-0.3.7/snsynth/pytorch/__init__.py
--rw-r--r--   0        0        0      469 2023-02-18 22:13:34.056234 smartnoise-synth-0.3.7/snsynth/pytorch/nn/__init__.py
--rw-r--r--   0        0        0      566 2023-02-18 22:13:34.056291 smartnoise-synth-0.3.7/snsynth/pytorch/nn/_discriminator.py
--rw-r--r--   0        0        0      849 2023-02-18 22:13:34.056348 smartnoise-synth-0.3.7/snsynth/pytorch/nn/_generator.py
--rw-r--r--   0        0        0     1076 2023-02-18 22:13:34.056908 smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/LICENSE
--rw-r--r--   0        0        0      543 2023-02-18 22:13:34.058379 smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/base.py
--rw-r--r--   0        0        0    13649 2023-02-18 22:13:34.059426 smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/ctgan.py
--rw-r--r--   0        0        0     7100 2023-04-03 16:29:33.879311 smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/data_sampler.py
--rw-r--r--   0        0        0    17766 2023-02-18 22:13:34.060484 smartnoise-synth-0.3.7/snsynth/pytorch/nn/dpctgan.py
--rw-r--r--   0        0        0     6707 2023-02-18 22:13:34.061113 smartnoise-synth-0.3.7/snsynth/pytorch/nn/dpgan.py
--rw-r--r--   0        0        0    18759 2023-02-18 22:13:34.061565 smartnoise-synth-0.3.7/snsynth/pytorch/nn/patectgan.py
--rw-r--r--   0        0        0     7937 2023-02-18 22:13:34.061778 smartnoise-synth-0.3.7/snsynth/pytorch/nn/pategan.py
--rw-r--r--   0        0        0     1546 2023-02-18 22:13:34.061857 smartnoise-synth-0.3.7/snsynth/pytorch/nn/privacy_utils.py
--rw-r--r--   0        0        0     3468 2023-02-18 22:13:34.062007 smartnoise-synth-0.3.7/snsynth/pytorch/pytorch_synthesizer.py
--rw-r--r--   0        0        0     7681 2023-02-18 22:13:34.062243 smartnoise-synth-0.3.7/snsynth/quail.py
--rw-r--r--   0        0        0      796 2023-02-18 22:13:34.062500 smartnoise-synth-0.3.7/snsynth/transform/__init__.py
--rw-r--r--   0        0        0     4424 2023-02-18 22:13:34.062760 smartnoise-synth-0.3.7/snsynth/transform/anonymization.py
--rw-r--r--   0        0        0     6874 2023-02-18 22:13:34.062909 smartnoise-synth-0.3.7/snsynth/transform/base.py
--rw-r--r--   0        0        0     4593 2023-02-18 22:13:34.063210 smartnoise-synth-0.3.7/snsynth/transform/bin.py
--rw-r--r--   0        0        0     2251 2023-02-18 22:13:34.063442 smartnoise-synth-0.3.7/snsynth/transform/chain.py
--rw-r--r--   0        0        0     1191 2023-02-18 22:13:34.063558 smartnoise-synth-0.3.7/snsynth/transform/clamp.py
--rw-r--r--   0        0        0     6879 2023-02-18 22:13:34.063915 smartnoise-synth-0.3.7/snsynth/transform/datetime.py
--rw-r--r--   0        0        0      121 2023-02-18 22:13:34.064149 smartnoise-synth-0.3.7/snsynth/transform/definitions.py
--rw-r--r--   0        0        0      940 2023-02-18 22:13:34.064294 smartnoise-synth-0.3.7/snsynth/transform/drop.py
--rw-r--r--   0        0        0      515 2023-02-18 22:13:34.064415 smartnoise-synth-0.3.7/snsynth/transform/identity.py
--rw-r--r--   0        0        0     2078 2023-02-18 22:13:34.064540 smartnoise-synth-0.3.7/snsynth/transform/label.py
--rw-r--r--   0        0        0      977 2023-02-18 22:13:34.064660 smartnoise-synth-0.3.7/snsynth/transform/log.py
--rw-r--r--   0        0        0     4170 2023-02-18 22:13:34.064802 smartnoise-synth-0.3.7/snsynth/transform/minmax.py
--rw-r--r--   0        0        0     1473 2023-02-18 22:13:34.065027 smartnoise-synth-0.3.7/snsynth/transform/onehot.py
--rw-r--r--   0        0        0     5348 2023-02-18 22:13:34.065369 smartnoise-synth-0.3.7/snsynth/transform/standard.py
--rw-r--r--   0        0        0    14644 2023-02-18 22:13:34.065554 smartnoise-synth-0.3.7/snsynth/transform/table.py
--rw-r--r--   0        0        0    13268 2023-02-18 22:13:34.065827 smartnoise-synth-0.3.7/snsynth/transform/type_map.py
--rw-r--r--   0        0        0     2116 2023-02-19 02:22:28.642964 smartnoise-synth-0.3.7/snsynth/utils.py
--rw-r--r--   0        0        0     2843 2023-04-03 20:58:16.067463 smartnoise-synth-0.3.7/setup.py
--rw-r--r--   0        0        0     2734 2023-04-03 20:58:16.067713 smartnoise-synth-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1842 2023-02-18 22:13:33.796789 smartnoise-synth-1.0.0/README.md
+-rw-r--r--   0        0        0      637 2023-05-12 02:34:34.642365 smartnoise-synth-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-02-18 22:13:34.053257 smartnoise-synth-1.0.0/snsynth/__init__.py
+-rw-r--r--   0        0        0      256 2023-02-18 22:13:34.053546 smartnoise-synth-1.0.0/snsynth/aggregate_seeded/__init__.py
+-rw-r--r--   0        0        0    12663 2023-02-18 22:13:34.053916 smartnoise-synth-1.0.0/snsynth/aggregate_seeded/aggregate_seeded.py
+-rw-r--r--   0        0        0       63 2023-02-18 22:13:34.054165 smartnoise-synth-1.0.0/snsynth/aim/__init__.py
+-rw-r--r--   0        0        0     8842 2023-02-19 02:22:28.642687 smartnoise-synth-1.0.0/snsynth/aim/aim.py
+-rw-r--r--   0        0        0    15963 2023-02-18 22:13:34.054436 smartnoise-synth-1.0.0/snsynth/base.py
+-rw-r--r--   0        0        0      115 2023-02-18 22:13:34.054909 smartnoise-synth-1.0.0/snsynth/definitions.py
+-rw-r--r--   0        0        0       84 2023-02-18 22:13:34.055020 smartnoise-synth-1.0.0/snsynth/models/__init__.py
+-rw-r--r--   0        0        0    16650 2023-02-18 22:13:34.055117 smartnoise-synth-1.0.0/snsynth/models/dp_covariance.py
+-rw-r--r--   0        0        0     2929 2023-02-18 22:13:34.055183 smartnoise-synth-1.0.0/snsynth/models/linear_regression.py
+-rw-r--r--   0        0        0    11356 2023-02-18 22:13:34.055477 smartnoise-synth-1.0.0/snsynth/mst/LICENSE
+-rw-r--r--   0        0        0       63 2023-02-18 22:13:34.055673 smartnoise-synth-1.0.0/snsynth/mst/__init__.py
+-rw-r--r--   0        0        0     8486 2023-02-19 02:22:28.642836 smartnoise-synth-1.0.0/snsynth/mst/mst.py
+-rw-r--r--   0        0        0       65 2023-02-18 22:13:34.055850 smartnoise-synth-1.0.0/snsynth/mst/test-domain.json
+-rw-r--r--   0        0        0    28241 2023-02-18 22:13:34.056031 smartnoise-synth-1.0.0/snsynth/mwem.py
+-rw-r--r--   0        0        0       91 2023-02-18 22:13:34.056148 smartnoise-synth-1.0.0/snsynth/pytorch/__init__.py
+-rw-r--r--   0        0        0      469 2023-02-18 22:13:34.056234 smartnoise-synth-1.0.0/snsynth/pytorch/nn/__init__.py
+-rw-r--r--   0        0        0      566 2023-02-18 22:13:34.056291 smartnoise-synth-1.0.0/snsynth/pytorch/nn/_discriminator.py
+-rw-r--r--   0        0        0      849 2023-02-18 22:13:34.056348 smartnoise-synth-1.0.0/snsynth/pytorch/nn/_generator.py
+-rw-r--r--   0        0        0     1076 2023-02-18 22:13:34.056908 smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/LICENSE
+-rw-r--r--   0        0        0      543 2023-02-18 22:13:34.058379 smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/base.py
+-rw-r--r--   0        0        0    13649 2023-02-18 22:13:34.059426 smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/ctgan.py
+-rw-r--r--   0        0        0     7100 2023-04-12 02:24:35.799523 smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/data_sampler.py
+-rw-r--r--   0        0        0    17766 2023-02-18 22:13:34.060484 smartnoise-synth-1.0.0/snsynth/pytorch/nn/dpctgan.py
+-rw-r--r--   0        0        0     6707 2023-02-18 22:13:34.061113 smartnoise-synth-1.0.0/snsynth/pytorch/nn/dpgan.py
+-rw-r--r--   0        0        0    18759 2023-02-18 22:13:34.061565 smartnoise-synth-1.0.0/snsynth/pytorch/nn/patectgan.py
+-rw-r--r--   0        0        0     7937 2023-02-18 22:13:34.061778 smartnoise-synth-1.0.0/snsynth/pytorch/nn/pategan.py
+-rw-r--r--   0        0        0     1546 2023-02-18 22:13:34.061857 smartnoise-synth-1.0.0/snsynth/pytorch/nn/privacy_utils.py
+-rw-r--r--   0        0        0     3468 2023-02-18 22:13:34.062007 smartnoise-synth-1.0.0/snsynth/pytorch/pytorch_synthesizer.py
+-rw-r--r--   0        0        0     7681 2023-02-18 22:13:34.062243 smartnoise-synth-1.0.0/snsynth/quail.py
+-rw-r--r--   0        0        0      796 2023-02-18 22:13:34.062500 smartnoise-synth-1.0.0/snsynth/transform/__init__.py
+-rw-r--r--   0        0        0     4424 2023-02-18 22:13:34.062760 smartnoise-synth-1.0.0/snsynth/transform/anonymization.py
+-rw-r--r--   0        0        0     6874 2023-02-18 22:13:34.062909 smartnoise-synth-1.0.0/snsynth/transform/base.py
+-rw-r--r--   0        0        0     4593 2023-02-18 22:13:34.063210 smartnoise-synth-1.0.0/snsynth/transform/bin.py
+-rw-r--r--   0        0        0     2251 2023-02-18 22:13:34.063442 smartnoise-synth-1.0.0/snsynth/transform/chain.py
+-rw-r--r--   0        0        0     1191 2023-02-18 22:13:34.063558 smartnoise-synth-1.0.0/snsynth/transform/clamp.py
+-rw-r--r--   0        0        0     6879 2023-02-18 22:13:34.063915 smartnoise-synth-1.0.0/snsynth/transform/datetime.py
+-rw-r--r--   0        0        0      121 2023-02-18 22:13:34.064149 smartnoise-synth-1.0.0/snsynth/transform/definitions.py
+-rw-r--r--   0        0        0      940 2023-02-18 22:13:34.064294 smartnoise-synth-1.0.0/snsynth/transform/drop.py
+-rw-r--r--   0        0        0      515 2023-02-18 22:13:34.064415 smartnoise-synth-1.0.0/snsynth/transform/identity.py
+-rw-r--r--   0        0        0     2078 2023-02-18 22:13:34.064540 smartnoise-synth-1.0.0/snsynth/transform/label.py
+-rw-r--r--   0        0        0      977 2023-02-18 22:13:34.064660 smartnoise-synth-1.0.0/snsynth/transform/log.py
+-rw-r--r--   0        0        0     4170 2023-02-18 22:13:34.064802 smartnoise-synth-1.0.0/snsynth/transform/minmax.py
+-rw-r--r--   0        0        0     1473 2023-02-18 22:13:34.065027 smartnoise-synth-1.0.0/snsynth/transform/onehot.py
+-rw-r--r--   0        0        0     5348 2023-02-18 22:13:34.065369 smartnoise-synth-1.0.0/snsynth/transform/standard.py
+-rw-r--r--   0        0        0    14644 2023-02-18 22:13:34.065554 smartnoise-synth-1.0.0/snsynth/transform/table.py
+-rw-r--r--   0        0        0    13268 2023-02-18 22:13:34.065827 smartnoise-synth-1.0.0/snsynth/transform/type_map.py
+-rw-r--r--   0        0        0     2116 2023-02-19 02:22:28.642964 smartnoise-synth-1.0.0/snsynth/utils.py
+-rw-r--r--   0        0        0     2842 2023-05-12 02:46:21.114393 smartnoise-synth-1.0.0/setup.py
+-rw-r--r--   0        0        0     2733 2023-05-12 02:46:21.114639 smartnoise-synth-1.0.0/PKG-INFO
```

### Comparing `smartnoise-synth-0.3.7/README.md` & `smartnoise-synth-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/pyproject.toml` & `smartnoise-synth-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "smartnoise-synth"
-version = "0.3.7"
+version = "1.0.0"
 description = "Differentially Private Synthetic Data"
 authors = ["SmartNoise Team <smartnoise@opendp.org>"]
 license = "MIT"
 packages = [{include="snsynth"}]
 homepage = "https://smartnoise.org"
 repository = "https://github.com/opendp/smartnoise-sdk"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<=3.11"
 opendp = "^0.6.0"
 opacus = "^0.14.0"
 torch = "<2.0.0"
 pac-synth = "^0.0.8"
-smartnoise-sql = "^0.2.10"
+smartnoise-sql = "^1.0.0"
 Faker = "^15.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `smartnoise-synth-0.3.7/snsynth/aggregate_seeded/aggregate_seeded.py` & `smartnoise-synth-1.0.0/snsynth/aggregate_seeded/aggregate_seeded.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/aim/aim.py` & `smartnoise-synth-1.0.0/snsynth/aim/aim.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/base.py` & `smartnoise-synth-1.0.0/snsynth/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/models/dp_covariance.py` & `smartnoise-synth-1.0.0/snsynth/models/dp_covariance.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/models/linear_regression.py` & `smartnoise-synth-1.0.0/snsynth/models/linear_regression.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/mst/LICENSE` & `smartnoise-synth-1.0.0/snsynth/mst/LICENSE`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/mst/mst.py` & `smartnoise-synth-1.0.0/snsynth/mst/mst.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/mwem.py` & `smartnoise-synth-1.0.0/snsynth/mwem.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/_discriminator.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/_discriminator.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/_generator.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/_generator.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/LICENSE` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/LICENSE`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/base.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/ctgan.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/ctgan.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/ctgan/data_sampler.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/ctgan/data_sampler.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/dpctgan.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/dpctgan.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/dpgan.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/dpgan.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/patectgan.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/patectgan.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/pategan.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/pategan.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/nn/privacy_utils.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/nn/privacy_utils.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/pytorch/pytorch_synthesizer.py` & `smartnoise-synth-1.0.0/snsynth/pytorch/pytorch_synthesizer.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/quail.py` & `smartnoise-synth-1.0.0/snsynth/quail.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/__init__.py` & `smartnoise-synth-1.0.0/snsynth/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/anonymization.py` & `smartnoise-synth-1.0.0/snsynth/transform/anonymization.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/base.py` & `smartnoise-synth-1.0.0/snsynth/transform/base.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/bin.py` & `smartnoise-synth-1.0.0/snsynth/transform/bin.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/chain.py` & `smartnoise-synth-1.0.0/snsynth/transform/chain.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/clamp.py` & `smartnoise-synth-1.0.0/snsynth/transform/clamp.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/datetime.py` & `smartnoise-synth-1.0.0/snsynth/transform/datetime.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/drop.py` & `smartnoise-synth-1.0.0/snsynth/transform/drop.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/identity.py` & `smartnoise-synth-1.0.0/snsynth/transform/identity.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/label.py` & `smartnoise-synth-1.0.0/snsynth/transform/label.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/log.py` & `smartnoise-synth-1.0.0/snsynth/transform/log.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/minmax.py` & `smartnoise-synth-1.0.0/snsynth/transform/minmax.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/onehot.py` & `smartnoise-synth-1.0.0/snsynth/transform/onehot.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/standard.py` & `smartnoise-synth-1.0.0/snsynth/transform/standard.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/table.py` & `smartnoise-synth-1.0.0/snsynth/transform/table.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/transform/type_map.py` & `smartnoise-synth-1.0.0/snsynth/transform/type_map.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/snsynth/utils.py` & `smartnoise-synth-1.0.0/snsynth/utils.py`

 * *Files identical despite different names*

### Comparing `smartnoise-synth-0.3.7/setup.py` & `smartnoise-synth-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 {'': ['*']}
 
 install_requires = \
 ['Faker>=15.0.0,<16.0.0',
  'opacus>=0.14.0,<0.15.0',
  'opendp>=0.6.0,<0.7.0',
  'pac-synth>=0.0.8,<0.0.9',
- 'smartnoise-sql>=0.2.10,<0.3.0',
+ 'smartnoise-sql>=1.0.0,<2.0.0',
  'torch<2.0.0']
 
 setup_kwargs = {
     'name': 'smartnoise-synth',
-    'version': '0.3.7',
+    'version': '1.0.0',
     'description': 'Differentially Private Synthetic Data',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)\n\n<a href="https://smartnoise.org"><img src="https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg" align="left" height="65" vspace="8" hspace="18"></a>\n\n# SmartNoise Synthesizers\n\nDifferentially private synthesizers for tabular data.  Package includes:\n* MWEM\n* MST\n* QUAIL\n* DP-CTGAN\n* PATE-CTGAN\n* PATE-GAN\n* AIM\n\n## Installation\n\n```\npip install smartnoise-synth\n```\n\n## Using\n\nPlease see the [SmartNoise synthesizers documentation](https://docs.smartnoise.org/synth/index.html) for usage examples.\n\n## Note on Inputs\n\nMWEM and MST require columns to be categorical. If you have columns with continuous values, you should discretize them before fitting.  Take care to discretize in a way that does not reveal information about the distribution of the data.\n\n## Communication\n\n- You are encouraged to join us on [GitHub Discussions](https://github.com/opendp/opendp/discussions/categories/smartnoise)\n- Please use [GitHub Issues](https://github.com/opendp/smartnoise-sdk/issues) for bug reports and feature requests.\n- For other requests, including security issues, please contact us at [smartnoise@opendp.org](mailto:smartnoise@opendp.org).\n\n## Releases and Contributing\n\nPlease let us know if you encounter a bug by [creating an issue](https://github.com/opendp/smartnoise-sdk/issues).\n\nWe appreciate all contributions. Please review the [contributors guide](../contributing.rst). We welcome pull requests with bug-fixes without prior discussion.\n\nIf you plan to contribute new features, utility functions or extensions to this system, please first open an issue and discuss the feature with us.\n',
     'author': 'SmartNoise Team',
     'author_email': 'smartnoise@opendp.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://smartnoise.org',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['snsynth',
 'snsynth.aggregate_seeded', 'snsynth.aim', 'snsynth.models', 'snsynth.mst',
 'snsynth.pytorch', 'snsynth.pytorch.nn', 'snsynth.pytorch.nn.ctgan',
 'snsynth.transform'] package_data = \ {'': ['*']} install_requires = \
 ['Faker>=15.0.0,<16.0.0', 'opacus>=0.14.0,<0.15.0', 'opendp>=0.6.0,<0.7.0',
-'pac-synth>=0.0.8,<0.0.9', 'smartnoise-sql>=0.2.10,<0.3.0', 'torch<2.0.0']
-setup_kwargs = { 'name': 'smartnoise-synth', 'version': '0.3.7', 'description':
+'pac-synth>=0.0.8,<0.0.9', 'smartnoise-sql>=1.0.0,<2.0.0', 'torch<2.0.0']
+setup_kwargs = { 'name': 'smartnoise-synth', 'version': '1.0.0', 'description':
 'Differentially Private Synthetic Data', 'long_description': '[![License: MIT]
 (https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
 licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-
 blue)](https://www.python.org/)\n\n[https://github.com/opendp/smartnoise-sdk/
 raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg]\n\n# SmartNoise
 Synthesizers\n\nDifferentially private synthesizers for tabular data. Package
 includes:\n* MWEM\n* MST\n* QUAIL\n* DP-CTGAN\n* PATE-CTGAN\n* PATE-GAN\n*
```

### Comparing `smartnoise-synth-0.3.7/PKG-INFO` & `smartnoise-synth-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartnoise-synth
-Version: 0.3.7
+Version: 1.0.0
 Summary: Differentially Private Synthetic Data
 Home-page: https://smartnoise.org
 License: MIT
 Author: SmartNoise Team
 Author-email: smartnoise@opendp.org
 Requires-Python: >=3.7,<=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Faker (>=15.0.0,<16.0.0)
 Requires-Dist: opacus (>=0.14.0,<0.15.0)
 Requires-Dist: opendp (>=0.6.0,<0.7.0)
 Requires-Dist: pac-synth (>=0.0.8,<0.0.9)
-Requires-Dist: smartnoise-sql (>=0.2.10,<0.3.0)
+Requires-Dist: smartnoise-sql (>=1.0.0,<2.0.0)
 Requires-Dist: torch (<2.0.0)
 Project-URL: Repository, https://github.com/opendp/smartnoise-sdk
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8-blue)](https://www.python.org/)
 
 <a href="https://smartnoise.org"><img src="https://github.com/opendp/smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg" align="left" height="65" vspace="8" hspace="18"></a>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: smartnoise-synth Version: 0.3.7 Summary:
+Metadata-Version: 2.1 Name: smartnoise-synth Version: 1.0.0 Summary:
 Differentially Private Synthetic Data Home-page: https://smartnoise.org
 License: MIT Author: SmartNoise Team Author-email: smartnoise@opendp.org
 Requires-Python: >=3.7,<=3.11 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Requires-Dist: Faker (>=15.0.0,<16.0.0) Requires-
 Dist: opacus (>=0.14.0,<0.15.0) Requires-Dist: opendp (>=0.6.0,<0.7.0)
 Requires-Dist: pac-synth (>=0.0.8,<0.0.9) Requires-Dist: smartnoise-sql
-(>=0.2.10,<0.3.0) Requires-Dist: torch (<2.0.0) Project-URL: Repository, https:
-//github.com/opendp/smartnoise-sdk Description-Content-Type: text/markdown [!
+(>=1.0.0,<2.0.0) Requires-Dist: torch (<2.0.0) Project-URL: Repository, https:/
+/github.com/opendp/smartnoise-sdk Description-Content-Type: text/markdown [!
 [License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![Python](https://img.shields.io/badge/python-
 3.7%20%7C%203.8-blue)](https://www.python.org/) [https://github.com/opendp/
 smartnoise-sdk/raw/main/images/SmartNoise/SVG/Logo%20Mark_grey.svg] #
 SmartNoise Synthesizers Differentially private synthesizers for tabular data.
 Package includes: * MWEM * MST * QUAIL * DP-CTGAN * PATE-CTGAN * PATE-GAN * AIM
 ## Installation ``` pip install smartnoise-synth ``` ## Using Please see the
```

