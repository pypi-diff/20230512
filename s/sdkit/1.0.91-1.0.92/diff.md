# Comparing `tmp/sdkit-1.0.91.tar.gz` & `tmp/sdkit-1.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkit-1.0.91.tar", last modified: Thu May 11 10:58:56 2023, max compression
+gzip compressed data, was "sdkit-1.0.92.tar", last modified: Fri May 12 11:18:35 2023, max compression
```

## Comparing `sdkit-1.0.91.tar` & `sdkit-1.0.92.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:56.629815 sdkit-1.0.91/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.91/LICENSE
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.91/MANIFEST.in
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-11 10:58:56.625815 sdkit-1.0.91/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.91/README.md
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-11 10:58:32.000000 sdkit-1.0.91/pyproject.toml
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:54.369663 sdkit-1.0.91/sdkit/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3522 2023-04-22 10:04:42.000000 sdkit-1.0.91/sdkit/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:54.651669 sdkit-1.0.91/sdkit/filter/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.91/sdkit/filter/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1141 2023-02-18 09:02:00.000000 sdkit-1.0.91/sdkit/filter/apply_filters.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/filter/gfpgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.91/sdkit/filter/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.91/sdkit/filter/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:54.768813 sdkit-1.0.91/sdkit/generate/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.91/sdkit/generate/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9985 2023-05-10 14:40:47.000000 sdkit-1.0.91/sdkit/generate/image_generator.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.91/sdkit/generate/prompt_parser.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:54.952925 sdkit-1.0.91/sdkit/generate/sampler/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.91/sdkit/generate/sampler/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.91/sdkit/generate/sampler/default_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3456 2023-04-29 08:59:57.000000 sdkit-1.0.91/sdkit/generate/sampler/diffusers_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/generate/sampler/k_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.91/sdkit/generate/sampler/sampler_main.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:55.062927 sdkit-1.0.91/sdkit/generate/sampler/unipc_samplers/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.91/sdkit/generate/sampler/unipc_samplers/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.91/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:55.162925 sdkit-1.0.91/sdkit/models/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.91/sdkit/models/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/models/model_downloader.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:55.391312 sdkit-1.0.91/sdkit/models/model_loader/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1687 2023-04-28 10:51:00.000000 sdkit-1.0.91/sdkit/models/model_loader/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/models/model_loader/gfpgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:55.491310 sdkit-1.0.91/sdkit/models/model_loader/hypernetwork/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/models/model_loader/hypernetwork/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/models/model_loader/hypernetwork/hypernetwork.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-10 14:38:42.000000 sdkit-1.0.91/sdkit/models/model_loader/lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.91/sdkit/models/model_loader/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.91/sdkit/models/model_loader/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:55.636313 sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11103 2023-05-11 10:57:44.000000 sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10003 2023-05-03 09:32:43.000000 sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/optimizations.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.91/sdkit/models/model_loader/vae.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:55.855623 sdkit-1.0.91/sdkit/models/models_db/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.91/sdkit/models/models_db/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:56.291553 sdkit-1.0.91/sdkit/models/models_db/configs/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v2-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v2-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v2-midas-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v2.1-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.91/sdkit/models/models_db/configs/v2.1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.91/sdkit/models/models_db/configs/x4-upscaling.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.91/sdkit/models/models_db/gfpgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.91/sdkit/models/models_db/realesrgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.91/sdkit/models/models_db/stable_diffusion.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.91/sdkit/models/models_db/vae.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/models/scan_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:56.360553 sdkit-1.0.91/sdkit/train/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.91/sdkit/train/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/train/merge_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:56.596815 sdkit-1.0.91/sdkit/utils/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-04-29 09:01:32.000000 sdkit-1.0.91/sdkit/utils/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.91/sdkit/utils/file_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.91/sdkit/utils/hash_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.91/sdkit/utils/http_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-04-28 10:51:00.000000 sdkit-1.0.91/sdkit/utils/image_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.91/sdkit/utils/latent_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.91/sdkit/utils/memory_utils.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-11 10:58:54.488664 sdkit-1.0.91/sdkit.egg-info/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-11 10:58:53.000000 sdkit-1.0.91/sdkit.egg-info/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2240 2023-05-11 10:58:54.000000 sdkit-1.0.91/sdkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-11 10:58:53.000000 sdkit-1.0.91/sdkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-11 10:58:53.000000 sdkit-1.0.91/sdkit.egg-info/requires.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-11 10:58:53.000000 sdkit-1.0.91/sdkit.egg-info/top_level.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-11 10:58:56.630815 sdkit-1.0.91/setup.cfg
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-03 10:25:33.000000 sdkit-1.0.91/setup.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:35.195855 sdkit-1.0.92/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.92/LICENSE
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.92/MANIFEST.in
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-12 11:18:35.180220 sdkit-1.0.92/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.92/README.md
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-12 11:17:42.000000 sdkit-1.0.92/pyproject.toml
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:32.868178 sdkit-1.0.92/sdkit/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3522 2023-04-22 10:04:42.000000 sdkit-1.0.92/sdkit/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:33.144144 sdkit-1.0.92/sdkit/filter/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.92/sdkit/filter/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1141 2023-02-18 09:02:00.000000 sdkit-1.0.92/sdkit/filter/apply_filters.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/filter/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.92/sdkit/filter/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.92/sdkit/filter/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:33.228315 sdkit-1.0.92/sdkit/generate/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.92/sdkit/generate/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9985 2023-05-10 14:40:47.000000 sdkit-1.0.92/sdkit/generate/image_generator.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.92/sdkit/generate/prompt_parser.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:33.449751 sdkit-1.0.92/sdkit/generate/sampler/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.92/sdkit/generate/sampler/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.92/sdkit/generate/sampler/default_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3456 2023-04-29 08:59:57.000000 sdkit-1.0.92/sdkit/generate/sampler/diffusers_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/generate/sampler/k_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.92/sdkit/generate/sampler/sampler_main.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:33.553422 sdkit-1.0.92/sdkit/generate/sampler/unipc_samplers/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.92/sdkit/generate/sampler/unipc_samplers/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.92/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:33.667056 sdkit-1.0.92/sdkit/models/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.92/sdkit/models/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/models/model_downloader.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:33.928462 sdkit-1.0.92/sdkit/models/model_loader/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1687 2023-04-28 10:51:00.000000 sdkit-1.0.92/sdkit/models/model_loader/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/models/model_loader/gfpgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:34.038251 sdkit-1.0.92/sdkit/models/model_loader/hypernetwork/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/models/model_loader/hypernetwork/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/models/model_loader/hypernetwork/hypernetwork.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-10 14:38:42.000000 sdkit-1.0.92/sdkit/models/model_loader/lora.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.92/sdkit/models/model_loader/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.92/sdkit/models/model_loader/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:34.201472 sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11299 2023-05-12 11:10:54.000000 sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11003 2023-05-12 11:15:35.000000 sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/optimizations.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.92/sdkit/models/model_loader/vae.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:34.398767 sdkit-1.0.92/sdkit/models/models_db/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.92/sdkit/models/models_db/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:34.868135 sdkit-1.0.92/sdkit/models/models_db/configs/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v2-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v2-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v2-midas-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v2.1-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.92/sdkit/models/models_db/configs/v2.1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.92/sdkit/models/models_db/configs/x4-upscaling.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.92/sdkit/models/models_db/gfpgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.92/sdkit/models/models_db/realesrgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.92/sdkit/models/models_db/stable_diffusion.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.92/sdkit/models/models_db/vae.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/models/scan_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:34.930646 sdkit-1.0.92/sdkit/train/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.92/sdkit/train/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/train/merge_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:35.164581 sdkit-1.0.92/sdkit/utils/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-04-29 09:01:32.000000 sdkit-1.0.92/sdkit/utils/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.92/sdkit/utils/file_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.92/sdkit/utils/hash_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.92/sdkit/utils/http_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-04-28 10:51:00.000000 sdkit-1.0.92/sdkit/utils/image_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.92/sdkit/utils/latent_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.92/sdkit/utils/memory_utils.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-12 11:18:32.993624 sdkit-1.0.92/sdkit.egg-info/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-12 11:18:31.000000 sdkit-1.0.92/sdkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2240 2023-05-12 11:18:32.000000 sdkit-1.0.92/sdkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-12 11:18:31.000000 sdkit-1.0.92/sdkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-12 11:18:31.000000 sdkit-1.0.92/sdkit.egg-info/requires.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-12 11:18:31.000000 sdkit-1.0.92/sdkit.egg-info/top_level.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-12 11:18:35.195855 sdkit-1.0.92/setup.cfg
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-03 10:25:33.000000 sdkit-1.0.92/setup.py
```

### Comparing `sdkit-1.0.91/LICENSE` & `sdkit-1.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/PKG-INFO` & `sdkit-1.0.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.91
+Version: 1.0.92
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-1.0.91/README.md` & `sdkit-1.0.92/README.md`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/pyproject.toml` & `sdkit-1.0.92/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdkit"
-version = "1.0.91"
+version = "1.0.92"
 authors = [
   {name="cmdr2", email="secondary.cmdr2@gmail.com"},
 ]
 description = "sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!"
 readme = "README.md"
 requires-python = ">=3.8.5"
 classifiers = [
```

### Comparing `sdkit-1.0.91/sdkit/__init__.py` & `sdkit-1.0.92/sdkit/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/filter/apply_filters.py` & `sdkit-1.0.92/sdkit/filter/apply_filters.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/filter/gfpgan.py` & `sdkit-1.0.92/sdkit/filter/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/filter/nsfw_checker.py` & `sdkit-1.0.92/sdkit/filter/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/image_generator.py` & `sdkit-1.0.92/sdkit/generate/image_generator.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/prompt_parser.py` & `sdkit-1.0.92/sdkit/generate/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/sampler/default_samplers.py` & `sdkit-1.0.92/sdkit/generate/sampler/default_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/sampler/diffusers_samplers.py` & `sdkit-1.0.92/sdkit/generate/sampler/diffusers_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/sampler/k_samplers.py` & `sdkit-1.0.92/sdkit/generate/sampler/k_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/sampler/sampler_main.py` & `sdkit-1.0.92/sdkit/generate/sampler/sampler_main.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/sampler/unipc_samplers/__init__.py` & `sdkit-1.0.92/sdkit/generate/sampler/unipc_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py` & `sdkit-1.0.92/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_downloader.py` & `sdkit-1.0.92/sdkit/models/model_downloader.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/__init__.py` & `sdkit-1.0.92/sdkit/models/model_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/gfpgan.py` & `sdkit-1.0.92/sdkit/models/model_loader/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/hypernetwork/__init__.py` & `sdkit-1.0.92/sdkit/models/model_loader/hypernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/hypernetwork/hypernetwork.py` & `sdkit-1.0.92/sdkit/models/model_loader/hypernetwork/hypernetwork.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/lora.py` & `sdkit-1.0.92/sdkit/models/model_loader/lora.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/nsfw_checker.py` & `sdkit-1.0.92/sdkit/models/model_loader/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/realesrgan.py` & `sdkit-1.0.92/sdkit/models/model_loader/realesrgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/__init__.py` & `sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,20 @@
     from compel import Compel
 
     from sdkit.generate.sampler import diffusers_samplers
     from sdkit.utils import gc
 
     from .convert_from_ckpt import download_from_original_stable_diffusion_ckpt
 
+    from .optimizations import optimized_get_attention_scores
+
+    from diffusers.models.attention_processor import Attention
+
+    Attention.get_attention_scores = optimized_get_attention_scores
+
     log.info("loading on diffusers")
 
     log.info(f"using config: {config_file_path}")
     config = OmegaConf.load(config_file_path)
     config.model.params.unet_config.params.use_fp16 = context.half_precision
 
     extra_config = config.get("extra", {})
```

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py` & `sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/stable_diffusion/optimizations.py` & `sdkit-1.0.92/sdkit/models/model_loader/stable_diffusion/optimizations.py`

 * *Files 12% similar despite different names*

```diff
@@ -248,7 +248,44 @@
     sizeCS = 0
     for _, val in model.cond_stage_model.state_dict().items():
         sizeCS += val.element_size() * val.nelement()
 
     log.info(f"model.cond_stage_model: {mb(sizeCS)} Mb")
 
     log.info(f"model (TOTAL): {mb(size_input + size_middle + size_output + sizeFS + sizeCS)} Mb")
+
+
+# optimized version of diffusers.models.attention_processor.Attention.get_attention_scores()
+# deletes the tensor as soon as possible
+def optimized_get_attention_scores(self, query, key, attention_mask=None):
+    dtype = query.dtype
+    if self.upcast_attention:
+        query = query.float()
+        key = key.float()
+
+    if attention_mask is None:
+        baddbmm_input = torch.empty(
+            query.shape[0], query.shape[1], key.shape[1], dtype=query.dtype, device=query.device
+        )
+        beta = 0
+    else:
+        baddbmm_input = attention_mask
+        beta = 1
+
+    attention_scores = torch.baddbmm(
+        baddbmm_input,
+        query,
+        key.transpose(-1, -2),
+        beta=beta,
+        alpha=self.scale,
+    )
+    del baddbmm_input
+
+    if self.upcast_softmax:
+        attention_scores = attention_scores.float()
+
+    attention_probs = attention_scores.softmax(dim=-1)
+    del attention_scores
+
+    attention_probs = attention_probs.to(dtype)
+
+    return attention_probs
```

### Comparing `sdkit-1.0.91/sdkit/models/model_loader/vae.py` & `sdkit-1.0.92/sdkit/models/model_loader/vae.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/__init__.py` & `sdkit-1.0.92/sdkit/models/models_db/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v1-inference.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v1-inpainting-inference.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v2-inference-v.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v2-inference.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v2-inpainting-inference.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v2-midas-inference.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v2.1-inference-v.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v2.1-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/v2.1-inference.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/v2.1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/configs/x4-upscaling.yaml` & `sdkit-1.0.92/sdkit/models/models_db/configs/x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/gfpgan.json` & `sdkit-1.0.92/sdkit/models/models_db/gfpgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/realesrgan.json` & `sdkit-1.0.92/sdkit/models/models_db/realesrgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/models/models_db/stable_diffusion.json` & `sdkit-1.0.92/sdkit/models/models_db/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/train/merge_models.py` & `sdkit-1.0.92/sdkit/train/merge_models.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/__init__.py` & `sdkit-1.0.92/sdkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/file_utils.py` & `sdkit-1.0.92/sdkit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/hash_utils.py` & `sdkit-1.0.92/sdkit/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/http_utils.py` & `sdkit-1.0.92/sdkit/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/image_utils.py` & `sdkit-1.0.92/sdkit/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/latent_utils.py` & `sdkit-1.0.92/sdkit/utils/latent_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit/utils/memory_utils.py` & `sdkit-1.0.92/sdkit/utils/memory_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.91/sdkit.egg-info/PKG-INFO` & `sdkit-1.0.92/sdkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.91
+Version: 1.0.92
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-1.0.91/sdkit.egg-info/SOURCES.txt` & `sdkit-1.0.92/sdkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

