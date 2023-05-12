# Comparing `tmp/open-metric-learning-0.4.0.tar.gz` & `tmp/open-metric-learning-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-0.4.0.tar", last modified: Thu Apr 27 16:36:45 2023, max compression
+gzip compressed data, was "dist/open-metric-learning-0.4.1.tar", last modified: Fri May 12 16:43:31 2023, max compression
```

## Comparing `open-metric-learning-0.4.0.tar` & `open-metric-learning-0.4.1.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    25628 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24204 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.512738 open-metric-learning-0.4.0/oml/configs/extractor/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/extractor/vit_clip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.516738 open-metric-learning-0.4.0/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4428 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/ddp/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.520738 open-metric-learning-0.4.0/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8802 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/modules/pairwise_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/lightning/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/train.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/lightning/pipelines/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.524738 open-metric-learning-0.4.0/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    15976 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/models/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/models/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/meta/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/meta/siamese.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/pooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/models/vit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/vision_transformer_clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     8065 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/models/vit/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.528738 open-metric-learning-0.4.0/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    25628 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-04-27 16:36:45.000000 open-metric-learning-0.4.0/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:36:45.532738 open-metric-learning-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/tests/test_build_readme.py
--rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-04-27 16:36:23.000000 open-metric-learning-0.4.0/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    25957 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24533 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/extractor/vit_clip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.006165 open-metric-learning-0.4.1/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4428 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/datasets/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/ddp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.010165 open-metric-learning-0.4.1/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8802 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.014165 open-metric-learning-0.4.1/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15976 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/metrics/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5799 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/meta/siamese.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/models/vit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5696 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/vision_transformer_clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8065 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/models/vit/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.018165 open-metric-learning-0.4.1/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25957 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-12 16:43:30.000000 open-metric-learning-0.4.1/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 16:43:31.022165 open-metric-learning-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-05-12 16:43:10.000000 open-metric-learning-0.4.1/tests/test_imports.py
```

### Comparing `open-metric-learning-0.4.0/LICENSE` & `open-metric-learning-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/PKG-INFO` & `open-metric-learning-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 0.4.0
+Version: 0.4.1
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -248,14 +248,19 @@
 You can also read some extra materials related to OML:
 
 * Theory and practice of metric learning with the usage of OML.
 [Post in English on Medium](https://medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) |
 [Post in Russian on Habr](https://habr.com/ru/company/ods/blog/695380/) |
 [Post in Chinese on CSDN](https://blog.csdn.net/fermion0217/article/details/127932087), translated by Chia-Chen Chang.
 
+* The
+[DEMO](https://dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/)
+for our paper
+[STIR: Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/2304.13393)
+
 * The report for Berlin-based meetup: "Computer Vision in production". November, 2022.
 [Link](https://drive.google.com/drive/folders/1uHmLU8vMrMVMFodt36u0uXAgYjG_3D30?usp=share_link)
 
 ## [Installation](https://open-metric-learning.readthedocs.io/en/latest/oml/installation.html)
 
 OML is available in PyPI:
 
@@ -363,14 +368,16 @@
 ```
 [comment]:usage-retrieval-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1S2nK6KaReDm-RjjdojdId6CakhhSyvfA?usp=share_link)
 
+[**Schemas, explanations and tips**](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction)
+
 See [extra code snippets](https://open-metric-learning.readthedocs.io/en/latest/feature_extraction/python_examples.html), including:
 * Training + Validation with Lightning
 * Training + Validation with Lightning in DDP mode
 * Training with losses from PML
 * Training with losses from PML advanced (passing distance, reducer, miner)
 
 ## [Pipelines](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines)
```

### Comparing `open-metric-learning-0.4.0/README.md` & `open-metric-learning-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,19 @@
 You can also read some extra materials related to OML:
 
 * Theory and practice of metric learning with the usage of OML.
 [Post in English on Medium](https://medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) |
 [Post in Russian on Habr](https://habr.com/ru/company/ods/blog/695380/) |
 [Post in Chinese on CSDN](https://blog.csdn.net/fermion0217/article/details/127932087), translated by Chia-Chen Chang.
 
+* The
+[DEMO](https://dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/)
+for our paper
+[STIR: Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/2304.13393)
+
 * The report for Berlin-based meetup: "Computer Vision in production". November, 2022.
 [Link](https://drive.google.com/drive/folders/1uHmLU8vMrMVMFodt36u0uXAgYjG_3D30?usp=share_link)
 
 ## [Installation](https://open-metric-learning.readthedocs.io/en/latest/oml/installation.html)
 
 OML is available in PyPI:
 
@@ -334,14 +339,16 @@
 ```
 [comment]:usage-retrieval-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1S2nK6KaReDm-RjjdojdId6CakhhSyvfA?usp=share_link)
 
+[**Schemas, explanations and tips**](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction)
+
 See [extra code snippets](https://open-metric-learning.readthedocs.io/en/latest/feature_extraction/python_examples.html), including:
 * Training + Validation with Lightning
 * Training + Validation with Lightning in DDP mode
 * Training with losses from PML
 * Training with losses from PML advanced (passing distance, reducer, miner)
 
 ## [Pipelines](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines)
```

### Comparing `open-metric-learning-0.4.0/oml/const.py` & `open-metric-learning-0.4.1/oml/const.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/datasets/base.py` & `open-metric-learning-0.4.1/oml/datasets/base.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/datasets/list_dataset.py` & `open-metric-learning-0.4.1/oml/datasets/list_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/datasets/pairs.py` & `open-metric-learning-0.4.1/oml/datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/datasets/triplet.py` & `open-metric-learning-0.4.1/oml/datasets/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/ddp/patching.py` & `open-metric-learning-0.4.1/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/ddp/utils.py` & `open-metric-learning-0.4.1/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/functional/label_smoothing.py` & `open-metric-learning-0.4.1/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/functional/losses.py` & `open-metric-learning-0.4.1/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/functional/metrics.py` & `open-metric-learning-0.4.1/oml/functional/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/inference/abstract.py` & `open-metric-learning-0.4.1/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/inference/flat.py` & `open-metric-learning-0.4.1/oml/inference/flat.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/inference/pairs.py` & `open-metric-learning-0.4.1/oml/inference/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/criterions.py` & `open-metric-learning-0.4.1/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/datasets.py` & `open-metric-learning-0.4.1/oml/interfaces/datasets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/metrics.py` & `open-metric-learning-0.4.1/oml/interfaces/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/miners.py` & `open-metric-learning-0.4.1/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/models.py` & `open-metric-learning-0.4.1/oml/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/retrieval.py` & `open-metric-learning-0.4.1/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/interfaces/samplers.py` & `open-metric-learning-0.4.1/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/callbacks/metric.py` & `open-metric-learning-0.4.1/oml/lightning/callbacks/metric.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/modules/ddp.py` & `open-metric-learning-0.4.1/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/modules/extractor.py` & `open-metric-learning-0.4.1/oml/lightning/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/modules/pairwise_postprocessing.py` & `open-metric-learning-0.4.1/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/pipelines/parser.py` & `open-metric-learning-0.4.1/oml/lightning/pipelines/parser.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/pipelines/train.py` & `open-metric-learning-0.4.1/oml/lightning/pipelines/train.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/pipelines/train_postprocessor.py` & `open-metric-learning-0.4.1/oml/lightning/pipelines/train_postprocessor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/lightning/pipelines/validate.py` & `open-metric-learning-0.4.1/oml/lightning/pipelines/validate.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/losses/arcface.py` & `open-metric-learning-0.4.1/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/losses/surrogate_precision.py` & `open-metric-learning-0.4.1/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/losses/triplet.py` & `open-metric-learning-0.4.1/oml/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/metrics/accumulation.py` & `open-metric-learning-0.4.1/oml/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/metrics/embeddings.py` & `open-metric-learning-0.4.1/oml/metrics/embeddings.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/metrics/triplets.py` & `open-metric-learning-0.4.1/oml/metrics/triplets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/miners/cross_batch.py` & `open-metric-learning-0.4.1/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/miners/inbatch_all_tri.py` & `open-metric-learning-0.4.1/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/miners/inbatch_hard_cluster.py` & `open-metric-learning-0.4.1/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/miners/inbatch_hard_tri.py` & `open-metric-learning-0.4.1/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/miners/inbatch_nhard_tri.py` & `open-metric-learning-0.4.1/oml/miners/inbatch_nhard_tri.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         hardest_negative = ids_smallest_distance[idx_anch_neg_reduced, idx_neg_sorted_by_dist]
         idx_anch_neg = all_ids_reduced[idx_anch_neg_reduced]
 
         ids_a = []
         ids_p = []
         ids_n = []
 
-        for idx_anch in torch.arange(len(labels))[torch.logical_not(ignore_anchor_mask)]:
+        for idx_anch in torch.arange(len(labels), device=distmat.device)[torch.logical_not(ignore_anchor_mask)]:
             positives = hardest_positive[idx_anch_pos == idx_anch][self.positive_slice]
             negatives = hardest_negative[idx_anch_neg == idx_anch][self.negative_slice]
 
             i_pos, i_neg = list(zip(*torch.cartesian_prod(positives, negatives).tolist()))
             ids_a.extend([idx_anch.item()] * len(i_pos))
             ids_p.extend(i_pos)
             ids_n.extend(i_neg)
```

### Comparing `open-metric-learning-0.4.0/oml/miners/miner_with_bank.py` & `open-metric-learning-0.4.1/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/miners/pairs.py` & `open-metric-learning-0.4.1/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/meta/projection.py` & `open-metric-learning-0.4.1/oml/models/meta/projection.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/meta/siamese.py` & `open-metric-learning-0.4.1/oml/models/meta/siamese.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/pooling.py` & `open-metric-learning-0.4.1/oml/models/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/resnet.py` & `open-metric-learning-0.4.1/oml/models/resnet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/utils.py` & `open-metric-learning-0.4.1/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/vit/clip.py` & `open-metric-learning-0.4.1/oml/models/vit/clip.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/vit/hubconf.py` & `open-metric-learning-0.4.1/oml/models/vit/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/vit/vision_transformer.py` & `open-metric-learning-0.4.1/oml/models/vit/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/vit/vision_transformer_clip.py` & `open-metric-learning-0.4.1/oml/models/vit/vision_transformer_clip.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/models/vit/vit.py` & `open-metric-learning-0.4.1/oml/models/vit/vit.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/__init__.py` & `open-metric-learning-0.4.1/oml/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/losses.py` & `open-metric-learning-0.4.1/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/miners.py` & `open-metric-learning-0.4.1/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/models.py` & `open-metric-learning-0.4.1/oml/registry/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/optimizers.py` & `open-metric-learning-0.4.1/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/postprocessors.py` & `open-metric-learning-0.4.1/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/samplers.py` & `open-metric-learning-0.4.1/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/schedulers.py` & `open-metric-learning-0.4.1/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/registry/transforms.py` & `open-metric-learning-0.4.1/oml/registry/transforms.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/retrieval/postprocessors/pairwise.py` & `open-metric-learning-0.4.1/oml/retrieval/postprocessors/pairwise.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/samplers/balance.py` & `open-metric-learning-0.4.1/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/samplers/category_balance.py` & `open-metric-learning-0.4.1/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/samplers/distinct_category_balance.py` & `open-metric-learning-0.4.1/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/transforms/images/albumentations.py` & `open-metric-learning-0.4.1/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/transforms/images/torchvision.py` & `open-metric-learning-0.4.1/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/dataframe_format.py` & `open-metric-learning-0.4.1/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/download_mock_dataset.py` & `open-metric-learning-0.4.1/oml/utils/download_mock_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/images/images.py` & `open-metric-learning-0.4.1/oml/utils/images/images.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/images/images_resize.py` & `open-metric-learning-0.4.1/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/io.py` & `open-metric-learning-0.4.1/oml/utils/io.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/misc.py` & `open-metric-learning-0.4.1/oml/utils/misc.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/misc_torch.py` & `open-metric-learning-0.4.1/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/oml/utils/remote_storage.py` & `open-metric-learning-0.4.1/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/open_metric_learning.egg-info/PKG-INFO` & `open-metric-learning-0.4.1/open_metric_learning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 0.4.0
+Version: 0.4.1
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -248,14 +248,19 @@
 You can also read some extra materials related to OML:
 
 * Theory and practice of metric learning with the usage of OML.
 [Post in English on Medium](https://medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) |
 [Post in Russian on Habr](https://habr.com/ru/company/ods/blog/695380/) |
 [Post in Chinese on CSDN](https://blog.csdn.net/fermion0217/article/details/127932087), translated by Chia-Chen Chang.
 
+* The
+[DEMO](https://dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/)
+for our paper
+[STIR: Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/2304.13393)
+
 * The report for Berlin-based meetup: "Computer Vision in production". November, 2022.
 [Link](https://drive.google.com/drive/folders/1uHmLU8vMrMVMFodt36u0uXAgYjG_3D30?usp=share_link)
 
 ## [Installation](https://open-metric-learning.readthedocs.io/en/latest/oml/installation.html)
 
 OML is available in PyPI:
 
@@ -363,14 +368,16 @@
 ```
 [comment]:usage-retrieval-end
 </p>
 </details>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1S2nK6KaReDm-RjjdojdId6CakhhSyvfA?usp=share_link)
 
+[**Schemas, explanations and tips**](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction)
+
 See [extra code snippets](https://open-metric-learning.readthedocs.io/en/latest/feature_extraction/python_examples.html), including:
 * Training + Validation with Lightning
 * Training + Validation with Lightning in DDP mode
 * Training with losses from PML
 * Training with losses from PML advanced (passing distance, reducer, miner)
 
 ## [Pipelines](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines)
```

### Comparing `open-metric-learning-0.4.0/open_metric_learning.egg-info/SOURCES.txt` & `open-metric-learning-0.4.1/open_metric_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/setup.py` & `open-metric-learning-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/tests/test_build_readme.py` & `open-metric-learning-0.4.1/tests/test_build_readme.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.0/tests/test_imports.py` & `open-metric-learning-0.4.1/tests/test_imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import pytest
 
 from oml.const import PROJECT_ROOT
 
 LIBS_TO_IGNORE = ["torch_xla"]
 
+NEED_TO_TEST_NOTEBOOKS = False
+
 
 def get_imports_from_files() -> List[Tuple[str, str]]:
     files = get_files_with_imports()
 
     file_import_pairs = []
 
     for file in files:
@@ -28,30 +30,38 @@
 
         file_import_pairs.extend(list(zip([file] * len(imports), imports)))
 
     return file_import_pairs
 
 
 def get_files_with_imports() -> List[str]:
+    files = []
+
     folder_with_scripts = PROJECT_ROOT / "oml"
     scriptes_files = sorted(str(fname.relative_to(PROJECT_ROOT)) for fname in folder_with_scripts.rglob("*.py"))
+    files.extend(scriptes_files)
 
     folder_with_tests = PROJECT_ROOT / "tests"
     tests_files = sorted(str(fname.relative_to(PROJECT_ROOT)) for fname in folder_with_tests.rglob("*.py"))
+    files.extend(tests_files)
 
     pipelines_folder = PROJECT_ROOT / "pipelines"
     pipelines_files = sorted(str(fname.relative_to(PROJECT_ROOT)) for fname in folder_with_tests.rglob("*.py"))
+    files.extend(pipelines_files)
 
     notebooks_files = sorted(
         str(fname.relative_to(PROJECT_ROOT))
         for fname in pipelines_folder.rglob("*.ipynb")
         if fname.parent.name != ".ipynb_checkpoints"
     )
 
-    return scriptes_files + tests_files + pipelines_files + notebooks_files
+    if NEED_TO_TEST_NOTEBOOKS:
+        files.extend(notebooks_files)
+
+    return files
 
 
 def find_imports_in_script(fname: Path) -> List[str]:
     with open(fname, "r") as f:
         script_code = f.read()
 
     imports = find_imports(script_code)
```

