# Comparing `tmp/rai_toolbox-0.2.1.tar.gz` & `tmp/rai_toolbox-0.3.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai_toolbox-0.2.1.tar", last modified: Thu Jun 16 17:59:19 2022, max compression
+gzip compressed data, was "rai_toolbox-0.3.1rc2.tar", last modified: Fri May 12 13:00:03 2023, max compression
```

## Comparing `rai_toolbox-0.2.1.tar` & `rai_toolbox-0.3.1rc2.tar`

### file list

```diff
@@ -1,72 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-06-16 17:59:19.121362 rai_toolbox-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.109362 rai_toolbox-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.121362 rai_toolbox-0.2.1/src/rai_toolbox/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3330 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox/_utils/
--rw-r--r--   0 runner    (1001) docker     (121)     7617 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/_utils/itertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     6746 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/_utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/_utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-16 17:59:19.121362 rai_toolbox-0.2.1/src/rai_toolbox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/augmix/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6439 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/augmix/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/augmix/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6054 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/_fourier_basis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/_implementations.py
--rw-r--r--   0 runner    (1001) docker     (121)     9452 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/datasets/_cifar10_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6205 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/datasets/_imagenet_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/datasets/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/datasets/cifar10_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11568 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/datasets/cifar_corruptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox/losses/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/losses/_jensen_shannon_divergence.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/losses/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/src/rai_toolbox/mushin/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     4058 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/hydra.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/_pl_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)    14127 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/launchers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/src/rai_toolbox/mushin/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/testing/lightning.py
--rw-r--r--   0 runner    (1001) docker     (121)    45967 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/mushin/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/src/rai_toolbox/optim/
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22478 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/optim/frank_wolfe.py
--rw-r--r--   0 runner    (1001) docker     (121)    26882 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/optim/lp_space.py
--rw-r--r--   0 runner    (1001) docker     (121)    13969 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/optim/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    33304 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/optim/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.117362 rai_toolbox-0.2.1/src/rai_toolbox/perturbations/
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/perturbations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9115 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/perturbations/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     8827 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/perturbations/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    15833 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/perturbations/solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/src/rai_toolbox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:59:19.113362 rai_toolbox-0.2.1/src/rai_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-06-16 17:59:19.000000 rai_toolbox-0.2.1/src/rai_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-06-16 17:59:19.000000 rai_toolbox-0.2.1/src/rai_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 17:59:19.000000 rai_toolbox-0.2.1/src/rai_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-06-16 17:59:19.000000 rai_toolbox-0.2.1/src/rai_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-16 17:59:19.000000 rai_toolbox-0.2.1/src/rai_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    78194 2022-06-16 17:59:09.000000 rai_toolbox-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.408277 rai_toolbox-0.3.1rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/publish_rai_experiments.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/tox_run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/SPDX.spdx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/brand/
+-rw-r--r--   0 runner    (1001) docker     (123)    39824 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/brand/logo_no_text.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/brand/logo_no_text_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/deps/requirements-pyright.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/conda_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.416277 rai_toolbox-0.3.1rc2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.416277 rai_toolbox-0.3.1rc2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.416277 rai_toolbox-0.3.1rc2/docs/source/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/explanation/perturbations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/explanation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.428277 rai_toolbox-0.3.1rc2/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.augmix.AugMix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.augmix.Fork.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.augmix.augment_and_mix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.fourier.FourierBasis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.fourier.create_heatmaps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.fourier.generate_fourier_bases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.CIFAR100C.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.CIFAR10C.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.CIFAR10P1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.ImageNet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.ImageNetM10.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.RestrictedImageNet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.evaluating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.freeze.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.frozen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.losses.jensen_shannon_divergence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.BaseWorkflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.HydraDDP.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.MetricsCallback.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.MultiRunMetricsWorkflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.RobustnessCurve.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.negate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ChainedParamTransformingOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ClampedGradientOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ClampedParameterOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.FrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1FrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1NormedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1qFrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1qNormedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L2FrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L2NormedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L2ProjectedOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.LinfFrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.LinfProjectedOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ParamTransformingOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.SignedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.TopQGradientOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.AdditivePerturbation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.PerturbationModel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.gradient_ascent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.random_restart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.uniform_like_l1_n_ball_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.uniform_like_l2_n_ball_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.uniform_like_linf_n_ball_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.to_batch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.428277 rai_toolbox-0.3.1rc2/docs/source/how_to/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/custom_optim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/deterministic_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/hydraddp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/univ_adv_pert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_augmentations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_losses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_mushin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_optim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_perturbation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.432277 rai_toolbox-0.3.1rc2/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   253710 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials/Building-Workflows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1202618 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials/CIFAR10-Adversarial-Perturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   462921 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials/ImageNet-Concept-Probing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.436277 rai_toolbox-0.3.1rc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  1196382 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/CIFAR10-Adversarial-Perturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2042525 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/ImageNet-Concept-Probing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   194591 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/MNIST-Translation-Robustness.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.440277 rai_toolbox-0.3.1rc2/examples/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)  1489515 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/fourier/FourierBasisPerturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/fourier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.440277 rai_toolbox-0.3.1rc2/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.444277 rai_toolbox-0.3.1rc2/experiments/adversarial_training/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    84317 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/TestRobustness.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.444277 rai_toolbox-0.3.1rc2/experiments/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/benchmarking/benchmarks.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/madry/
+-rw-r--r--   0 runner    (1001) docker     (123)   138231 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/Experiments.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   508348 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/Visualizations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.404277 rai_toolbox-0.3.1rc2/experiments/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/_resnet_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/small_resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/imagenet_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/tests/test_rai_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.452278 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   248742 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/UniversalPerturbation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/experiments/xai/
+-rw-r--r--   0 runner    (1001) docker     (123)   788118 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.404277 rai_toolbox-0.3.1rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_fourier_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_cifar10_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_imagenet_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar10_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar_corruptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_jensen_shannon_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.464278 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/_pl_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/launchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.464278 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45121 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.464278 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/frank_wolfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/lp_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/top_level.txt
```

### Comparing `rai_toolbox-0.2.1/LICENSE.txt` & `rai_toolbox-0.3.1rc2/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Massachusetts Institute of Technology
+Copyright (c) 2023 Massachusetts Institute of Technology
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rai_toolbox-0.2.1/README.md` & `rai_toolbox-0.3.1rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 </p>
 
 <p align="center">
   <a href="https://pypi.org/project/rai-toolbox/">
     <img src="https://img.shields.io/pypi/v/rai-toolbox.svg" alt="PyPI" />
   </a>
   <a>
-    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.9-blue.svg" alt="Python version support" />
+    <img src="https://img.shields.io/badge/python-3.7%20&#8208;%203.10-blue.svg" alt="Python version support" />
   </a>
   <a href="https://github.com/mit-ll-responsible-ai/responsible-ai-toolbox/actions?query=workflow%3ATests+branch%3Amain">
     <img src="https://github.com/mit-ll-responsible-ai/responsible-ai-toolbox/workflows/Tests/badge.svg" alt="GitHub Actions" />
   <a href="https://hypothesis.readthedocs.io/">
     <img src="https://img.shields.io/badge/hypothesis-tested-brightgreen.svg" alt="Tested with Hypothesis" />
   </a>
 
@@ -50,15 +50,15 @@
 
 
 
 ## Disclaimer
 
 DISTRIBUTION STATEMENT A. Approved for public release. Distribution is unlimited.
 
-© 2022 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+© 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 
 - Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
 - SPDX-License-Identifier: MIT
 
 This material is based upon work supported by the Under Secretary of Defense for Research and Engineering under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Under Secretary of Defense for Research and Engineering.
 
 A portion of this research was sponsored by the United States Air Force Research Laboratory and the United States Air Force Artificial Intelligence Accelerator and was accomplished under Cooperative Agreement Number FA8750-19-2-1000. The views and conclusions contained in this document are those of the authors and should not be interpreted as representing the official policies, either expressed or implied, of the United States Air Force or the U.S. Government. The U.S. Government is authorized to reproduce and distribute reprints for Government purposes notwithstanding any copyright notation herein.
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 ## Citation Using `rai_toolbox` for your research? Please cite the following
 publication: ``` @article{soklaski2022tools, title={Tools and Practices for
 Responsible AI Engineering}, author={Soklaski, Ryan and Goodwin, Justin and
 Brown, Olivia and Yee, Michael and Matterer, Jason}, journal={arXiv preprint
 arXiv:2201.05647}, year={2022} } ``` ## Contributing If you would like to
 contribute to this repo, please refer to our `CONTRIBUTING.md` document. ##
 Disclaimer DISTRIBUTION STATEMENT A. Approved for public release. Distribution
-is unlimited. Â© 2022 MASSACHUSETTS INSTITUTE OF TECHNOLOGY - Subject to FAR
+is unlimited. Â© 2023 MASSACHUSETTS INSTITUTE OF TECHNOLOGY - Subject to FAR
 52.227-11 â Patent Rights â Ownership by the Contractor (May 2014) - SPDX-
 License-Identifier: MIT This material is based upon work supported by the Under
 Secretary of Defense for Research and Engineering under Air Force Contract No.
 FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations
 expressed in this material are those of the author(s) and do not necessarily
 reflect the views of the Under Secretary of Defense for Research and
 Engineering. A portion of this research was sponsored by the United States Air
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/_typing.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/_typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 # pyright: strict
 import functools
 import inspect
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     Mapping,
     Optional,
-    Sequence,
     Type,
     TypeVar,
     Union,
-    overload,
 )
 
 import numpy as np
 from torch import Tensor
+from torch.nn.parameter import Parameter
 from typing_extensions import Protocol, TypeAlias, TypeGuard
 
 T = TypeVar("T")
 T_co = TypeVar("T_co", covariant=True)
 
 __all__ = [
     "InstantiatesTo",
@@ -54,47 +53,51 @@
 
     def state_dict(self) -> Any:
         ...
 
     def load_state_dict(self, state_dict: Any) -> None:
         ...
 
-    def zero_grad(self, set_to_none: Optional[bool] = ...) -> None:
+    def zero_grad(self, set_to_none: Any = ...) -> None:
+        # In order to maintain compatibility across torch versions we
+        # annotate `set_to_none: Any`
+        # - torch 1.12 annotates `set_to_none: bool`
+        # - torch <1.12 annotates `set_to_none: Optional[bool]`
         ...
 
-    def step(self, closure: Optional[Callable[[], Any]] = ...) -> Optional[Any]:
+    def step(self, closure: Optional[Callable[[], Any]] = None) -> Optional[Any]:
         ...
 
     def add_param_group(self, param_group: Any) -> None:
         ...
 
 
 ParamGroup = Mapping[str, Any]
 
 # Needed instead of Type[Optimizer] to deal with __init__ sig mismatch
 OptimizerType: TypeAlias = Callable[..., Optimizer]
 
 
 # type for Optim(params: <>)
-OptimParams = Union[Sequence[Tensor], Iterable[ParamGroup]]
+OptimParams = Union[Iterable[Tensor], Iterable[Parameter], Iterable[ParamGroup]]
 
 
 InstantiatesTo = Union[Type[T_co], Partial[T_co]]
 
 
 def _is_protocol(cls: Any) -> bool:
     return issubclass(cls, Generic) and getattr(cls, "_is_protocol", False)
 
 
 # This should *only* be used internally and with care.
 # There are complications for using this with protocols.
 def instantiates_to(x: Any, co_var_type: Type[T]) -> TypeGuard[InstantiatesTo[T]]:
     """Checks if `x(...)` will return type `co_var_type`.
 
-    Accomodates structural subtyping via protocols.
+    Accommodates structural subtyping via protocols.
 
     Parameters
     ----------
     x : Any
 
     co_var_type : Type[T]
         A type or a protocol. Note that protocols should not
@@ -128,24 +131,10 @@
     complex,
     str,
     bytes,
     np.generic,
 ]
 
 
-class _SupportsArray(Protocol):  # pragma: no cover
-    @overload
-    def __array__(self, __dtype: Any = ...) -> np.ndarray:  # type: ignore
+class ArrayLike(Protocol):
+    def __array__(self, dtype: Any = ...) -> Any:
         ...
-
-    @overload
-    def __array__(self, dtype: Any = ...) -> np.ndarray:  # type: ignore
-        ...
-
-
-# mypy doesn't support recursive types
-ArrayLike = Union[
-    Scalar,
-    Sequence[Scalar],
-    Sequence[Sequence[Any]],
-    _SupportsArray,
-]
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/_utils/__init__.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 from numbers import Real
 from typing import Any, Iterable, Mapping, Optional, Tuple, TypeVar, Union, cast
 
 import torch as tr
 
@@ -90,15 +90,15 @@
         elif not min_ < max_:
             raise Unsatisfiable(f"{min_} < {max_}")
 
     min_satisfied = (
         (min_ <= value if incl_min else min_ < value) if min_ is not None else True
     )
     max_satisfied = (
-        (value <= max_ if incl_min else value < max_) if max_ is not None else True
+        (value <= max_ if incl_max else value < max_) if max_ is not None else True
     )
 
     if not min_satisfied or not max_satisfied:
         lsymb = "<=" if incl_min else "<"
         rsymb = "<=" if incl_max else "<"
 
         err_msg = f"`{name}` must satisfy"
@@ -191,15 +191,15 @@
     p : Tensor
 
     param_ndim: Optional[int]
         Determines the shape of the resulting parameter
 
         - A positive number determines the dimensionality of the tensor that the transformation will act on.
         - A negative number indicates the 'offset' from the dimensionality of the tensor.
-        - `None` means that the transformation will be applied to the tensor without any broadcasting.
+        - `None` means that the transformation will be applied to the tensor without any broadcasting. This is equivalent to `param_ndim=p.ndim`
 
     Returns
     -------
     reshaped_p: Tensor, shape-(N, d0, ...)
         Where
         - (d0, ...) is of length `param_ndim` for `param_ndim > 0`
         - (d0, ...) is (1,) for `param_ndim == 0`
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/_utils/itertools.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/itertools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Callable, Iterable, List, Mapping, TypeVar, Union
 
 import torch as tr
 
@@ -11,15 +11,14 @@
 
 
 def flatten_params(
     iter_params_or_groups: Union[
         tr.Tensor, Iterable[tr.Tensor], Iterable[Mapping[str, Iterable[tr.Tensor]]]
     ]
 ) -> List[tr.Tensor]:
-
     if isinstance(iter_params_or_groups, tr.Tensor):
         return [iter_params_or_groups]
 
     out = []
     for params in iter_params_or_groups:
         if isinstance(params, tr.Tensor):
             out.append(params)
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/_utils/stateful.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/stateful.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from abc import ABCMeta, abstractmethod
 from functools import wraps
 from typing import Callable, Dict, Iterable, TypeVar, Union, cast
 from weakref import WeakSet
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/_utils/tqdm.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/tqdm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Iterable, Optional, TypeVar
 
 _T = TypeVar("_T", bound=Iterable)
 
 __all__ = ["tqdm"]
 
+
 def _dummy_tqdm(
     iterable: _T,
     desc: Optional[str] = None,
     total: Optional[int] = None,
     leave=True,
     file=None,
     ncols=None,
@@ -27,13 +28,13 @@
     bar_format=None,
     initial=0,
     position=None,
     postfix=None,
     unit_divisor=1000,
 ) -> _T:
     return iterable
-        
+
+
 try:
     from tqdm.auto import tqdm
 except ImportError:  # pragma: no cover
     tqdm = _dummy_tqdm
-
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/augmentations/augmix/_implementation.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
-
+# type: ignore
 """
 An implementation of the AugMix augmentation method specified in:
 
     Hendrycks, Dan, et al. "Augmix: A simple data processing method to improve
     robustness and uncertainty." arXiv preprint arXiv:1912.02781 (2019).
 
 with reference implementation from https://github.com/google-research/augmix
 """
+
 from numbers import Real
 from typing import Callable, Optional, Sequence, Tuple, TypeVar, Union
 
 import numpy as np
 
 from rai_toolbox._typing import ArrayLike
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/augmentations/augmix/transforms.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from numbers import Integral
 from typing import Any, Callable, Optional, Sequence, Tuple, TypeVar, Union
 
-import numpy as np
 import torch as tr
 
+from rai_toolbox._typing import ArrayLike
+
 from ._implementation import augment_and_mix
 
 _T1 = TypeVar("_T1")
-_T2 = TypeVar("_T2", np.ndarray, tr.Tensor, float)
+_T2 = TypeVar("_T2", bound=ArrayLike)
 
 __all__ = ["AugMix", "Fork", "augment_and_mix"]
 
 
 def _check_non_neg_int(item, name):
     if not isinstance(item, (int, Integral)) or item < 0:
         raise ValueError(f"`{name}`` must be a non-negative integer. Got {item}")
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/_fourier_basis.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_fourier_basis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from itertools import product
 from typing import Iterable, Iterator, NamedTuple, Optional, Tuple
 
 import numpy as np
 from numpy.typing import DTypeLike
 
 
 class FourierBasis(NamedTuple):
-    """
+    r"""
     Describes a 2D planewave generated via:
 
     A * cos(2pi * freq_vector @ x + phase_shift)
 
     Where `A` normalizes the 2D array to have an :math:`L^2`-norm of 1,
     and `x` is evaluated on a grid of positions on [0, H] x [0, W].
 
@@ -47,15 +47,15 @@
     nrows: int,
     ncols: int,
     dtype: DTypeLike = np.float32,
     *,
     factor_2pi_phase_shift: float = 0,
     row_col_coords: Optional[Iterable[Tuple[int, int]]] = None,
 ) -> Iterator[FourierBasis]:
-    """Yields each unique, real-valued 2D array with unit norm, such that its Fourier
+    r"""Yields each unique, real-valued 2D array with unit norm, such that its Fourier
     transform is supported at each (i, j) and its symmetric position on a shape-(nrows, ncols)
     grid in Fourier space, where the lowest frequency component resides at the center of
     the grid.
 
     Parameters
     ----------
     nrows : int
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/_implementations.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_implementations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
-
+# type: ignore
 import random
 from collections import defaultdict
 from typing import (
     Any,
     Callable,
     Collection,
     DefaultDict,
@@ -135,15 +135,15 @@
     rand_flip_per_channel: bool,
     post_pert_batch_transform: Optional[Callable[[tr.Tensor], tr.Tensor]] = None,
     device: Optional[Union[tr.device, str, int]] = None,
     row_col_coords: Optional[Iterable[Tuple[int, int]]] = None,
     factor_2pi_phase_shift: float = 0,
 ) -> Dict[str, List[HeatMapEntry]]:
     from rai_toolbox._utils.tqdm import tqdm
-    
+
     _outer_total = (
         None if row_col_coords is not None else int(np.prod(image_height_width)) // 2
     )
 
     with evaluating(model), tr.no_grad():
         if device is not None:
             device = tr.device(device)
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/augmentations/fourier/transforms.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from numbers import Number
 from typing import List, Optional, Tuple, TypeVar, Union, cast
 
 import numpy as np
@@ -53,18 +53,18 @@
                 p=self._sample_probs,
             ).tolist()
 
         index = self._rand_index_cache.pop()
 
         if isinstance(self._norm_bnds, tuple):
             norm = np.random.uniform(*self._norm_bnds, size=1).item()
-            return self.bases[index] * norm
+            return cast(Tensor, self.bases[index] * norm)
         else:
             # norm was already applied to all bases in __init__
-            return self.bases[index]
+            return cast(Tensor, self.bases[index])
 
     def __init__(
         self,
         size: Union[int, Tuple[int, int]],
         *,
         norm_scale: Union[float, Tuple[float, float]] = 1.0,
         dtype: Union[str, tr.dtype] = "float32",
@@ -199,15 +199,15 @@
             self.bases = self._norm_bnds * self.bases
 
         # Sample probabilities are adjusted so that sampling occurs evenly
         # over basis-frequencies.
         self._sample_probs = np.concatenate([1 / _radii] * num_distinct_phases)
         self._sample_probs /= self._sample_probs.sum()
 
-    def forward(self, img: _T) -> _T:
+    def forward(self, img: _T) -> _T:  # type: ignore
         """
         Parameters
         ----------
         img: Union[Image, Tensor], shape-(C, H, W)
             Tensors are expected to have shape-(C, H, W) and to be on the domain [0, 1].
             The post-perturbation tensor is clipped to [0, 1]. PIL images are scaled
             and transposed appropriately (255 -> 1) prior to augmentation.
@@ -240,12 +240,11 @@
         if _was_pil:
             img = tr.clip_(img, min=0.0, max=1.0)
             return cast(_T, _to_pil(img))
 
         return cast(_T, img)
 
     def __repr__(self) -> str:
-
         return (
             self.__class__.__name__
             + f"(norm_scale={self._norm_bnds}, rand_flip_per_channel={self.rand_flip_per_channel}, radii_bounds={self.radii_bounds})"
         )
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/datasets/_cifar10_base.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_cifar10_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Any, Dict, Tuple
 
 import numpy as np
 from PIL import Image
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/datasets/_imagenet_base.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_imagenet_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 from torchvision.datasets import folder
@@ -36,15 +36,15 @@
             A function to load a sample given its path.
 
         is_valid_file : Optional[Callable[[str], bool]], optional (default=None)
             A function that takes path of a file
             and checks if the file is a valid file.
         """
         super().__init__(
-            root,
+            str(root),
             loader,
             folder.IMG_EXTENSIONS if is_valid_file is None else None,
             transform=transform,
             target_transform=target_transform,
             is_valid_file=is_valid_file,
         )
 
@@ -87,15 +87,15 @@
         root: Union[str, Path],
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         loader: Callable[[str], Any] = folder.default_loader,
         is_valid_file: Optional[Callable[[str], bool]] = None,
     ):
         super().__init__(
-            root=root,
+            root=str(root),
             loader=loader,
             extensions=folder.IMG_EXTENSIONS if is_valid_file is None else None,
             transform=transform,
             target_transform=target_transform,
             is_valid_file=is_valid_file,
         )
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/datasets/_utils.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from pathlib import Path
 from typing import Union
 
 PathLike = Union[str, Path]
 
 __all__ = ["md5_check"]
 
 
-def md5_check(fname: PathLike, chunksize: int = 1024 ** 2) -> str:
+def md5_check(fname: PathLike, chunksize: int = 1024**2) -> str:
     """Reads in data from disk and returns md5 hash"""
     import hashlib
 
     hash_md5 = hashlib.md5()
     with open(fname, "rb") as f:
         for chunk in iter(lambda: f.read(chunksize), b""):
             hash_md5.update(chunk)
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/datasets/cifar10_extensions.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar10_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 
 import numpy as np
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/datasets/cifar_corruptions.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar_corruptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from numbers import Integral
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional, Union
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/losses/_jensen_shannon_divergence.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_jensen_shannon_divergence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Optional
 
 import torch as tr
 import torch.nn.functional as F
 
 from rai_toolbox._typing import ArrayLike
 
 
 def jensen_shannon_divergence(
     *probs: ArrayLike, weight: Optional[float] = None
 ) -> tr.Tensor:
-    """
+    r"""
     Computes the Jensen-Shannon divergence [1]_ between n distributions:
 
     :math:`JSD(P_1, P_2, ..., P_n)`
 
     This loss is symmetric and is bounded by :math:`0 <= JSD(P_1, P_2, ..., P_n) <= \ln(n)`
 
     Parameters
@@ -56,28 +56,27 @@
     tensor(0.4621)
 
     The divergence is symmetric.
 
     >>> jensen_shannon_divergence(P1, P3, P2)
     tensor(0.4621)
     """
+    list_probs = [tr.as_tensor(p) for p in probs]
 
-    probs = tuple(tr.as_tensor(p) for p in probs)
-
-    if len(probs) < 2 or any(
-        not isinstance(p, tr.Tensor) or p.dim() != 2 for p in probs
+    if len(list_probs) < 2 or any(
+        not isinstance(p, tr.Tensor) or p.dim() != 2 for p in list_probs
     ):
         raise ValueError(
             f"*probs must consist of at least two Tensors, and each tensor must have a shape of (N, D). Got {probs}"
         )
 
-    zero = tr.tensor(0.0).type_as(probs[0])
+    zero = tr.tensor(0.0).type_as(list_probs[0])
     # Clamp mixture distribution to avoid exploding KL divergence
-    log_p_mixture = tr.clamp(sum(probs, zero) / len(probs), 1e-7, 1).log()
+    log_p_mixture = tr.clamp(sum(list_probs, zero) / len(list_probs), 1e-7, 1).log()
     loss = sum(
-        (F.kl_div(log_p_mixture, p, reduction="batchmean") for p in probs), zero
+        (F.kl_div(log_p_mixture, p, reduction="batchmean") for p in list_probs), zero
     ) / len(probs)
 
     if weight is not None:
         loss = loss * weight
 
     return loss
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/losses/_utils.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from functools import wraps
 from typing import Any, Callable, TypeVar, cast
 
 from typing_extensions import Protocol
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/__init__.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from ._utils import load_experiment, load_from_checkpoint
 from .lightning import HydraDDP, MetricsCallback
 from .workflows import (
     BaseWorkflow,
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/_compatibility.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import NamedTuple
 
 import pytorch_lightning
 from typing_extensions import Final
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/_utils.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
@@ -71,15 +71,15 @@
             k[len(weights_key_strip) :]: v
             for k, v in ckpt_data.items()
             if k.startswith(weights_key_strip)
         }
 
     if model_attr is None:
         # The weights can be loaded in directly
-        model.load_state_dict(ckpt_data)  # type: ignore
+        model.load_state_dict(ckpt_data)
 
     else:
         assert hasattr(model, model_attr)
         getattr(model, model_attr).load_state_dict(ckpt_data)
 
     return model
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/_pl_main.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/_pl_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 """
 This script is called from `rai_toolbox.mushin.lightning.launchers.HydraDDP
 """
 
 import logging
 from typing import Optional
 
 import hydra
+from hydra_zen import zen
 from pytorch_lightning import LightningDataModule, LightningModule, Trainer
 
-from ..hydra import zen
-
 log = logging.getLogger(__name__)
 
 
 def task(
     trainer: Trainer,
     module: LightningModule,
     datamodule: Optional[LightningDataModule] = None,
@@ -32,14 +31,14 @@
         log.info(f"Rank {pl_local_rank}: Launched subprocess using Trainer.predict")
         trainer.predict(module, datamodule=datamodule)
     else:
         log.info(f"Rank {pl_local_rank}: Launched subprocess using Training.fit")
         trainer.fit(module, datamodule=datamodule)
 
 
-@hydra.main(config_path=None, config_name="config")
+@hydra.main(config_path=None, config_name="config", version_base="1.1")
 def main(cfg):
     zen(task)(cfg)
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/callbacks.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from collections import defaultdict
 from pathlib import Path
 from typing import Union
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/lightning/launchers.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/launchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 import os
 import subprocess
 import sys
 from pathlib import Path
@@ -255,15 +255,15 @@
 
                 # starting all processes at once can cause issues
                 # with dataloaders delay between 1-10 seconds
                 delay = np.random.uniform(1, 5, 1)[0]
                 sleep(delay)
 
 else:  # pragma: no cover
-    from pytorch_lightning.plugins.training_type.ddp import DDPPlugin
+    from pytorch_lightning.plugins.training_type.ddp import DDPPlugin  # type: ignore
 
     class HydraDDP(DDPPlugin):
         """DDP Strategy that supports Hydra run and multirun jobs.
 
         This strategy assumes a PyTorch Lightning `Trainer.fit` or `Trainer.test` has been configured
         to execute via Hydra.  It requires that Hydra saves a `config.yaml` in the current working directory with the following keys/properties set::
 
@@ -348,19 +348,19 @@
             if self.lightning_module.trainer is None:  # pragma: no cover
                 raise TypeError("HydraDDP.lightning_module.trainer is None")
 
             if self.cluster_environment is None:  # pragma: no cover
                 raise TypeError("HydraDDP.cluster_environment is None")
 
             # bookkeeping of spawned processes
-            self._check_can_spawn_children()  # type: ignore
+            self._check_can_spawn_children()
 
             # DDP Environment variables
-            os.environ["MASTER_ADDR"] = self.cluster_environment.master_address()  # type: ignore
-            os.environ["MASTER_PORT"] = str(self.cluster_environment.master_port())  # type: ignore
+            os.environ["MASTER_ADDR"] = self.cluster_environment.master_address()
+            os.environ["MASTER_PORT"] = str(self.cluster_environment.master_port())
 
             # allow the user to pass the node rank
             os.environ["NODE_RANK"] = str(self.cluster_environment.node_rank())
             os.environ["LOCAL_RANK"] = str(self.cluster_environment.local_rank())
             os.environ["WORLD_SIZE"] = f"{self.num_processes * self.num_nodes}"
 
             self.interactive_ddp_procs = []
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/testing/lightning.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/lightning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 import torch
 from pytorch_lightning import LightningDataModule, LightningModule
 from torch.nn import functional as fnn
 from torch.utils.data import DataLoader, Dataset
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/mushin/workflows.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
-import warnings
-from collections import UserList, defaultdict
+from collections import defaultdict
 from inspect import getattr_static
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     DefaultDict,
     Dict,
@@ -22,54 +21,37 @@
     Union,
 )
 
 import numpy as np
 import torch as tr
 from hydra.core.override_parser.overrides_parser import OverridesParser
 from hydra.core.utils import JobReturn
-from hydra_zen import launch, load_from_yaml, make_config
+from hydra_zen import hydra_list, launch, load_from_yaml, make_config, multirun, zen
 from hydra_zen._compatibility import HYDRA_VERSION
 from hydra_zen._launch import _NotSet
 from typing_extensions import Self, TypeAlias, TypeGuard
 
 from rai_toolbox._utils import value_check
 
-from .hydra import zen
-
 LoadedValue: TypeAlias = Union[str, int, float, bool, List[Any], Dict[str, Any]]
 
 __all__ = [
     "BaseWorkflow",
     "RobustnessCurve",
     "MultiRunMetricsWorkflow",
-    "multirun",
-    "hydra_list",
 ]
 
 
 T = TypeVar("T", List[Any], Tuple[Any])
 T1 = TypeVar("T1")
 
 
 _VERSION_BASE_DEFAULT = _NotSet if HYDRA_VERSION < (1, 2, 0) else "1.1"
 
 
-class multirun(UserList):
-    """Signals that a sequence is to be iterated over in a multirun"""
-
-    pass
-
-
-class hydra_list(UserList):
-    """Signals that a sequence is provided as a single configured value (i.e. it is not
-    to be iterated over during a multirun)"""
-
-    pass
-
-
 def _sort_x_by_k(x: T, k: Iterable[Any]) -> T:
     k = tuple(k)
     assert len(x) == len(k)
     sorted_, _ = zip(*sorted(zip(x, k), key=lambda x: x[1]))
     return type(x)(sorted_)
 
 
@@ -135,25 +117,14 @@
         self.cfgs = []
         self.metrics = {}
         self.workflow_overrides = {}
         self._multirun_task_overrides = {}
         self.jobs = []
         self._working_dir = None
 
-        if hasattr(self, "evaluation_task"):
-            warnings.warn(
-                "The static method `evaluation_task` is deprecated in favor of the "
-                "static method  `task`. Support for `evaluation_task` will be removed "
-                "in version 0.3.0 of rai-toolbox. To fix this, simply rename "
-                "`evaluation_task` method to `task`.",
-                FutureWarning,
-                stacklevel=2,
-            )
-            self.task = self.evaluation_task  # type: ignore
-
     @property
     def working_dir(self) -> Path:
         if self._working_dir is None:
             raise ValueError("`self.working_dir` must be set.")
 
         return self._working_dir
 
@@ -217,15 +188,14 @@
         >>>
         >>> wf = WorkFlow()
         >>> wf.run(foo=hydra_list(["val"]), bar=multirun(["a", "b"]), apple=1)
         >>> wf.multirun_task_overrides
         {'foo': ['val'], 'bar': multirun(['a', 'b']), 'apple': 1}
         """
         if not self._multirun_task_overrides:
-
             overrides = load_from_yaml(
                 self.working_dir / "multirun.yaml"
             ).hydra.overrides.task
 
             output = self._parse_overrides(overrides)
             self._multirun_task_overrides = output
 
@@ -239,17 +209,17 @@
         which must occur prior to instantiating objects for the evaluation
         task.
 
         Notes
         -----
         This function is automatically wrapped by `zen`, which is responsible
         for parsing the function's signature and then extracting and instantiating
-        the correspending fields from a Hydra config object – passing them to the
-        function. This behavior can be modified by `self.run(pre_task_fn_wrapper=...)`"""
-        pass
+        the corresponding fields from a Hydra config object – passing them to the
+        function. This behavior can be modified by `self.run(pre_task_fn_wrapper=...)`
+        """
 
     @staticmethod
     def task(*args: Any, **kwargs: Any) -> Any:
         """User-defined task that is run by the workflow. This should be
         a static method.
 
         Arguments will be instantiated configuration variables.  For example,
@@ -267,21 +237,21 @@
             def task(trainer: Trainer, module: LightningModule) -> None:
                 trainer.fit(module)
 
         Notes
         -----
         This function is automatically wrapped by `zen`, which is responsible
         for parsing the function's signature and then extracting and instantiating
-        the correspending fields from a Hydra config object – passing them to the
+        the corresponding fields from a Hydra config object – passing them to the
         function. This behavior can be modified by `self.run(task_fn_wrapper=...)`
         """
         raise NotImplementedError()
 
     def validate(self, include_pre_task: bool = True):
-        """Valide the configuration will execute with the user defined evaluation task"""
+        """Validates that the configuration will execute with the user-defined evaluation task"""
         if include_pre_task:
             zen(self.pre_task).validate(self.eval_task_cfg)
 
         zen(self.task).validate(self.eval_task_cfg)
 
     def run(
         self,
@@ -301,15 +271,15 @@
         config_name: str = "rai_workflow",
         job_name: str = "rai_workflow",
         with_log_configuration: bool = True,
         **workflow_overrides: Union[str, int, float, bool, dict, multirun, hydra_list],
     ):
         """Run the experiment.
 
-        Individual workflows can expclitly define `workflow_overrides` to improve
+        Individual workflows can explicitly define `workflow_overrides` to improve
         readability and undstanding of what parameters are expected for a particular
         workflow.
 
         Parameters
         ----------
         task_fn_wrapper: Callable[[Callable[..., T1]], Callable[[Any], T1]] | None, optional (default=rai_toolbox.mushin.zen)
             A wrapper applied to `self.task` prior to launching the task.
@@ -454,15 +424,15 @@
     return v
 
 
 class MultiRunMetricsWorkflow(BaseWorkflow):
     """Abstract class for workflows that record metrics using Hydra multirun.
 
     This workflow creates subdirectories of multirun experiments using Hydra.  These directories
-    contain the Hydra YAML configuration and any saved metrics file (defined by the evaulation task)::
+    contain the Hydra YAML configuration and any saved metrics file (defined by the evaluationf task)::
 
         ├── working_dir
         │    ├── <experiment directory name: 0>
         │    |    ├── <hydra output subdirectory: (default: .hydra)>
         |    |    |    ├── config.yaml
         |    |    |    ├── hydra.yaml
         |    |    |    ├── overrides.yaml
@@ -822,15 +792,15 @@
         Parameters
         ----------
         metrics_filename : str | Sequence[str]
             The filename(s) or glob-pattern(s) uses to load the metrics.
             If `None`, the metrics stored in `self.metrics` is used.
 
         Returns
-        ------
+        -------
         metrics : Dict[str, List[Any]]
 
         Examples
         --------
         Creating a workflow that saves named metrics using `torch.save`
 
         >>> from rai_toolbox.mushin.workflows import MultiRunMetricsWorkflow, multirun
@@ -995,15 +965,14 @@
 
             v = _coerce_list_of_arraylikes(v)
 
             datum = np.asarray(v).reshape(shape + np.asarray(v[0]).shape)
 
             k_coords = list(orig_coords)
             for n in range(datum.ndim - len(orig_coords)):
-
                 if coord_from_metrics and n < len(metric_coords):
                     # Assume the first coordinate of the metric is the metric coordinate dimension
                     k_coords += list(metric_coords.keys())
                     for mk, mv in metric_coords.items():
                         coords[mk] = mv
                 else:
                     # Create additional arbitrary coordinates as-needed for non-scalar
@@ -1021,15 +990,14 @@
             coords = {}
             for k, v in self.target_dir_multirun_overrides.items():
                 if len(v) == len(exp_dir):
                     if (
                         len(set(np.unique(v))) > 1
                         or non_multirun_params_as_singleton_dims
                     ):
-
                         coords[k] = (
                             [self._JOBDIR_NAME],
                             [self._sanitize_coordinate_for_xarray(item) for item in v],
                         )
             out = out.assign_coords(coords)
         return out
 
@@ -1092,15 +1060,15 @@
             This is helpful for filtering out parameters stored in
             `self.workflow_overrides`.
 
         **workflow_overrides: dict | str | int | float | bool | multirun | hydra_list
             These parameters represent the values for configurations to use for the
             experiment.
 
-            These values will be appeneded to the `overrides` for the Hydra job.
+            These values will be appended to the `overrides` for the Hydra job.
         """
 
         if not isinstance(epsilon, str):
             epsilon = multirun(epsilon)
 
         return super().run(
             task_fn_wrapper=task_fn_wrapper,
@@ -1162,15 +1130,15 @@
             )
             .sortby("epsilon")
         )
 
     def plot(
         self,
         metric: str,
-        ax=None,
+        ax: Any = None,
         group: Optional[str] = None,
         save_filename: Optional[str] = None,
         non_multirun_params_as_singleton_dims: bool = False,
         **kwargs,
     ) -> Any:
         """Plot metrics versus `epsilon`.
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/optim/__init__.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from .frank_wolfe import (
     FrankWolfe,
     L1FrankWolfe,
     L1qFrankWolfe,
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/optim/frank_wolfe.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/frank_wolfe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Union
 
 import torch
 from torch.optim import Optimizer
@@ -129,24 +129,29 @@
     parameter's gradient. Each updated parameter is constrained to fall within an
     :math:`\epsilon`-sized ball in :math:`L^1` space, centered on the origin.
 
     The sparsification process retains only the signs (i.e., :math:`\pm 1`) of the
     gradient's elements. The transformation is applied to the gradient in accordance
     with `param_ndim`.
 
+    Notes
+    -----
+    This parameter-transforming optimizer is useful for visual concept probing [2]_.
+
     See Also
     --------
     FrankWolfe
     L1FrankWolfe
     L2FrankWolfe
     LinfFrankWolfe
 
     References
     ----------
     .. [1] https://en.wikipedia.org/wiki/Frank%E2%80%93Wolfe_algorithm#Algorithm
+    .. [2] Roberts, Jay, and Theodoros Tsiligkaridis. Controllably Sparse Perturbations of Robust Classifiers for Explaining Predictions and Probing Learned Concepts. (2021).
     """
 
     def __init__(
         self,
         params: OptimParams,
         *,
         q: float,
@@ -378,14 +383,18 @@
         param.grad[torch.arange(len(param)), argmax] = signs
 
 
 class L2FrankWolfe(L2NormedGradientOptim):
     r"""A Frank-Wolfe [1]_ optimizer that constrains each updated parameter to fall
     within an :math:`\epsilon`-sized ball in :math:`L^2` space, centered on the origin.
 
+
+    This parameter-transforming optimizer is useful for producing error counter
+    factuals and performing visual concept probing [2]_.
+
     Notes
     -----
     The method `L2NormedGradientOptim._pre_step_transform_` is responsible for
     computing the *negative* linear minimization oracle for a parameter and storing it
     on `param.grad`.
 
     See Also
@@ -394,14 +403,15 @@
     L1FrankWolfe
     LinfFrankWolfe
     L1qFrankWolfe
 
     References
     ----------
     .. [1] https://en.wikipedia.org/wiki/Frank%E2%80%93Wolfe_algorithm#Algorithm
+    .. [2] Roberts, Jay, and Theodoros Tsiligkaridis. Controllably Sparse Perturbations of Robust Classifiers for Explaining Predictions and Probing Learned Concepts. (2021).
     """
 
     def __init__(
         self,
         params: OptimParams,
         *,
         epsilon: float,
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/optim/lp_space.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/lp_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from functools import partial
 from typing import Any, Dict, Optional, Union
 
 import torch
 from torch import Generator, Tensor, default_generator
 from torch.optim import SGD
 from typing_extensions import Final
 
-from rai_toolbox._typing import Optimizer as Opt
-from rai_toolbox._typing import OptimizerType, OptimParams, Partial
+from rai_toolbox._typing import Optimizer as Opt, OptimizerType, OptimParams, Partial
 from rai_toolbox._utils import check_param_group_value, value_check
 
 from .misc import TopQGradientOptimizer
 from .optimizer import (
     REQUIRED,
     ChainedParamTransformingOptimizer,
     DatumParamGroup,
@@ -123,15 +122,15 @@
         self.div_by_zero_eps = value_check("div_by_zero_eps", div_by_zero_eps, min_=0.0)
 
     @property
     def p(self) -> Union[float, int]:
         return self._p
 
     def per_datum_norm(self, x: torch.Tensor) -> torch.Tensor:
-        return torch.norm(x, p=self.p, dim=1)  # type: ignore
+        return torch.norm(x, p=self.p, dim=1)
 
     def _pre_step_transform_(self, param: Tensor, **_unused_kwargs) -> None:
         if param.grad is None:  # pragma: no cover
             return
 
         g = param.grad.flatten(1)
         g_norm = self.per_datum_norm(g).view(-1, *([1] * (param.ndim - 1)))
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/optim/misc.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import torch
 from torch import Generator, Tensor, default_generator
 from torch.optim import SGD
 
-from rai_toolbox._typing import Optimizer as Opt
-from rai_toolbox._typing import OptimizerType, OptimParams, Partial
+from rai_toolbox._typing import Optimizer as Opt, OptimizerType, OptimParams, Partial
 from rai_toolbox._utils import check_param_group_value, value_check
 
 from .optimizer import REQUIRED, DatumParamGroup, ParamTransformingOptimizer
 
 __all__ = ["ClampedGradientOptimizer", "TopQGradientOptimizer"]
 
 
@@ -66,15 +65,15 @@
             Added to each gradient in-place after the in-place transformation is
             performed. This can be specified per param-group.
 
         defaults : Optional[Dict[str, Any]]
             Specifies default parameters for all parameter groups.
 
         param_ndim : Optional[int]
-            Controles how `_pre_step_transform_` and `_post_step_transform_`  are
+            Controls how `_pre_step_transform_` and `_post_step_transform_`  are
             broadcast onto a given parameter. This has no effect for
             `ClampedGradientOptimizer` and `ClampedParameterOptimizer`.
 
         **inner_opt_kwargs : Any
             Named arguments used to initialize `InnerOpt`.
         """
         if defaults is None:
@@ -163,15 +162,15 @@
         self, param: Tensor, optim_group: ClampedParamGroup
     ) -> None:
         param.clamp_(min=optim_group["clamp_min"], max=optim_group["clamp_max"])
 
 
 class TopQGradientOptimizer(ParamTransformingOptimizer):
     """A gradient-tranforming  optimizer that zeros the elements of a gradient whose
-    absolue magnitudes fall below the Qth percentile. `InnerOpt.step()` is then to
+    absolute magnitudes fall below the Qth percentile. `InnerOpt.step()` is then to
     update the corresponding parameter.
 
     See Also
     --------
     L1qNormedGradientOptim
     ParamTransformingOptimizer"""
 
@@ -183,15 +182,14 @@
         q: float = REQUIRED,
         dq: float = 0.0,
         param_ndim: Union[int, None] = -1,
         defaults: Optional[Dict[str, Any]] = None,
         generator: Generator = default_generator,
         **inner_opt_kwargs,
     ):
-
         r"""
         Parameters
         ----------
         params : Sequence[Tensor] | Iterable[Mapping[str, Any]]
             Iterable of parameters or dicts defining parameter groups.
 
         InnerOpt : Type[Optimizer] | Partial[Optimizer], optional (default=`torch.nn.optim.SGD`)
@@ -343,15 +341,14 @@
         )
         check_param_group_value(
             "dq", self.param_groups, optional=True, min_=0.0, max_=1.0
         )
         self._generator = value_check("generator", generator, type_=torch.Generator)
 
     def _pre_step_transform_(self, param: Tensor, optim_group: Dict[str, Any]) -> None:
-
         if param.grad is None:  # pragma: no cover
             return
 
         q = optim_group["q"]
         dq = optim_group["dq"]
 
         if dq > 0.0:
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/optim/optimizer.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 import inspect
-import warnings
 from abc import ABCMeta
 from typing import Any, Callable, Dict, List, Optional, TypeVar, Union, cast, overload
 
 import torch
 from torch import Tensor
 from torch.optim import SGD, Optimizer
 from typing_extensions import TypedDict
 
-from rai_toolbox._typing import InstantiatesTo
-from rai_toolbox._typing import Optimizer as Opt
-from rai_toolbox._typing import OptimizerType, OptimParams, Partial, instantiates_to
+from rai_toolbox._typing import (
+    InstantiatesTo,
+    Optimizer as Opt,
+    OptimizerType,
+    OptimParams,
+    Partial,
+    instantiates_to,
+)
 from rai_toolbox._utils import validate_param_ndim as _validate_param_ndim
 
 _T = TypeVar("_T", bound=Optional[Union[Tensor, float]])
 
 __all__ = ["ParamTransformingOptimizer", "ChainedParamTransformingOptimizer"]
 
 
@@ -149,15 +153,15 @@
 
     Notes
     -----
     `ParamTransformingOptimizer` mirrors state with `InnerOpt` so that their
     `param_groups`, `defaults`, and `state` are always in sync.
 
     `ParamTransformingOptimizer` is designed to be combined with other,
-    standard gradient-based optimizers (e.g., Adam) via encapsulation, rather than
+    standard gradient-based optimizers (e.g., Adam) via composition, rather than
     through inheritance. I.e., `ParamTransformingOptimizer(InnerOpt=<...>)` will apply
     `_pre_step_transform_` on a parameter, and then use `InnerOpt.step(...)` to update
     said parameter, and finally will apply `_post_step_transform_` to the parameter.
 
     If a closure is supplied to the `.step(...)` method, then the `_pre_step_transform_`
     is applied after the closure call and prior to the parameter steps.
 
@@ -520,34 +524,14 @@
         for group in self.param_groups:
             param_ndim = group["param_ndim"]
 
             for p in group["params"]:
                 p = _to_batch(p, param_ndim)
                 self._post_step_transform_(param=p, optim_group=group)
 
-    def project(self):
-        """
-        .. deprecated:: 0.2.0
-          `project` will be removed in rai-toolbox 0.3.0, it is replaced by
-          `_apply_post_step_transform_`
-
-        Update each parameter in-place by calling `_post_step_transform_` on the
-        parameter.
-
-        This is called automatically by `.step()` after `InnerOpt.step()` has been
-        called."""
-        warnings.warn(
-            FutureWarning(
-                "`project` will be removed in rai-toolbox 0.3.0, it is replaced by "
-                "`_apply_post_step_transform_`"
-            ),
-            stacklevel=2,
-        )
-        return self._apply_post_step_transform_()
-
     @torch.no_grad()
     def _apply_pre_step_transform_(self):
         """Update each parameter in-place by calling `_pre_step_transform_` on the
         parameter.
 
         This is called automatically by `.step()` before `InnerOpt.step()` has been
         called."""
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/perturbations/__init__.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
-from .models import AdditivePerturbation, PerturbationModel
 from .init import (
     uniform_like_l1_n_ball_,
     uniform_like_l2_n_ball_,
     uniform_like_linf_n_ball_,
 )
+from .models import AdditivePerturbation, PerturbationModel
 from .solvers import gradient_ascent, random_restart
 
 __all__ = [
     "AdditivePerturbation",
     "PerturbationModel",
     "gradient_ascent",
     "random_restart",
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/perturbations/init.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from typing import Optional, Union
 
 import torch
 from torch import Generator, Tensor, default_generator
 
-from rai_toolbox._utils import to_batch as _to_batch
-from rai_toolbox._utils import validate_param_ndim as _validate_param_ndim
-from rai_toolbox._utils import value_check
+from rai_toolbox._utils import (
+    to_batch as _to_batch,
+    validate_param_ndim as _validate_param_ndim,
+    value_check,
+)
 
 
 @torch.no_grad()
 def uniform_like_l1_n_ball_(
     x: Tensor,
     epsilon: float = 1.0,
     param_ndim: Union[int, None] = -1,
@@ -24,21 +26,21 @@
     Parameters
     ----------
     x: Tensor, shape-(N, D, ...)
         The tensor from which to generate a new random tensor, i.e., returns a tensor of
         similar shape and on the same device.
 
         By default, each of the `N` shape-`(D, ...)` subtensors are initialized
-        independently. See `param_ndim` to contol this behavior.
+        independently. See `param_ndim` to control this behavior.
 
     epsilon : float, optional (default=1)
         Determines the radius of the ball.
 
     param_ndim : int | None, optional (default=-1)
-        Determines the dimenionality of the subtensors that are sampled by this
+        Determines the dimensionality of the subtensors that are sampled by this
         function.
 
         - A positive number determines the dimensionality of each subtensor to be drawn and packed into the shape-`(N, D, ...)` resulting tensor.
         - A negative number determines from the dimensionality of the subtensor in terms of the offset of `x.ndim`. E.g. -1 indicates that `x` is arranged in a batch-style, and that `N` independent shape-`(D, ...)` tensors will be sampled.
         - `None` means that a single tensor of shape-`(N, D, ...)` is sampled.
 
     Returns
@@ -119,21 +121,21 @@
     Parameters
     ----------
     x: Tensor, shape-(N, D, ...)
         The tensor to generate a new random tensor from, i.e., returns a tensor of
         similar shape and on the same device.
 
         By default, each of the `N` shape-`(D, ...)` subtensors are initialized
-        independently. See `param_ndim` to contol this behavior.
+        independently. See `param_ndim` to control this behavior.
 
     epsilon : float, optional (default=1)
         Determines the radius of the ball.
 
     param_ndim : int | None, optional (default=-1)
-        Determines the dimenionality of the subtensors that are sampled by this
+        Determines the dimensionality of the subtensors that are sampled by this
         function.
 
         - A positive number determines the dimensionality of each subtensor to be drawn and packed into the shape-`(N, D, ...)` resulting tensor.
         - A negative number determines from the dimensionality of the subtensor in terms of the offset of `x.ndim`. E.g. -1 indicates that `x` is arranged in a batch-style, and that `N` independent shape-`(D, ...)` tensors will be sampled.
         - `None` means that a single tensor of shape-`(N, D, ...)` is sampled.
 
     generator : torch.Generator, optional (default=`torch.default_generator`)
@@ -183,15 +185,15 @@
     value_check("epsilon", epsilon, min_=0.0, incl_min=False)
 
     xflat = _to_batch(x, param_ndim=param_ndim).flatten(1)
     nbatch, ndim = xflat.shape
 
     z = torch.empty((nbatch, ndim + 2), dtype=xflat.dtype, device=generator.device)
     z.normal_(generator=generator)
-    r = z.norm(p=2, dim=1, keepdim=True)  # type: ignore
+    r = z.norm(p=2, dim=1, keepdim=True)
     x.copy_(epsilon * (z / r)[:, :ndim].reshape(x.shape))
 
 
 @torch.no_grad()
 def uniform_like_linf_n_ball_(
     x: Tensor,
     epsilon: float = 1.0,
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/perturbations/models.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 from abc import abstractmethod
 from typing import Any, Callable, Iterator, Optional, Sequence, Union
 
 import torch as tr
```

### Comparing `rai_toolbox-0.2.1/src/rai_toolbox/perturbations/solvers.py` & `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
+# Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
 import functools
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import torch as tr
@@ -49,30 +49,30 @@
        pert_data = perturbation_model(data)
        loss = criterion(model(pert_data), target)
        loss = (1 if targeted else -1) * loss  # default: targeted=False
        optim.step()
 
     Note that, by default, this perturbs the data away from `target` (i.e., this performs
     gradient *ascent*), given a standard loss function that seeks to minimize the
-    diffence between the model's output and the target. See `targeted` to toggle this
+    difference between the model's output and the target. See `targeted` to toggle this
     behavior.
 
     Parameters
     ----------
     model : Callable[[Tensor], Tensor]
         Differentiable function that processes the (perturbed) data prior to computing
         the loss.
 
         If `model` is a `torch.nn.Module`, then its weights will be frozen and it will
         be set to eval mode during the perturbation-solve phase.
 
-    data : Tensor, shape-(N, ...)
+    data : ArrayLike, shape-(N, ...)
         The input data to perturb.
 
-    target : Tensor, shape-(N, ...)
+    target : ArrayLike, shape-(N, ...)
         If `targeted==False` (default), then this is the target to perturb away from.
         If `targeted==True`, then this is the target to perturb toward.
 
     optimizer : Optimizer | Type[Optimizer] | Partial[Optimizer]
         The optimizer to use for updating the perturbation model.
 
         If `optimizer` is uninstantiated, it will be instantiated as
@@ -243,15 +243,15 @@
             raise TypeError(
                 f"`optimizer` must be an instance of Optimizer or must instantiate to "
                 f"Optimizer; got: {optimizer}"
             )
         if instantiates_to(perturbation_model, PerturbationModel):
             raise TypeError(
                 "An initialized optimizer can only be passed to the solver in "
-                "combination with an intialized perturbation model."
+                "combination with an initialized perturbation model."
             )
         if optim_kwargs:
             raise TypeError(
                 "**optim_kwargs were specified, but the provided `optimizer` has "
                 "already been instaniated"
             )
 
@@ -282,26 +282,26 @@
             if use_best:
                 if (
                     (losses.ndim == 0 and data.ndim > 0)
                     or losses.ndim > data.ndim
                     or losses.shape != data.shape[: losses.ndim]
                 ):
                     raise ValueError(
-                        f"`use_best=True` but `criterion` does not ouput a per-datum-loss. "
+                        f"`use_best=True` but `criterion` does not output a per-datum-loss. "
                         f"I.e. `criterion` returned a tensor of shape-{tuple(losses.shape)} for a "
                         f"batch of shape-{tuple(data.shape)}. Expected a tensor of "
                         f"shape-{(len(data),)} or greater."
                     )
 
                 best_loss, best_x = _replace_best(losses, best_loss, xadv, best_x)
 
         # free up memory
         optim.zero_grad(set_to_none=True)
 
-        # Final evalulation
+        # Final evaluation
         with tr.no_grad():
             xadv = pmodel(data)
             logits = model(xadv)
             losses = criterion(logits, target)
 
             if use_best:
                 # we negate the loss when `targeted=True` so min-loss is always best
```

