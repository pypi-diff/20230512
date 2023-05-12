# Comparing `tmp/funasr_onnx-0.0.8.tar.gz` & `tmp/funasr_onnx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr_onnx-0.0.8.tar", last modified: Mon May  8 11:00:59 2023, max compression
+gzip compressed data, was "funasr_onnx-0.0.9.tar", last modified: Fri May 12 02:20:35 2023, max compression
```

## Comparing `funasr_onnx-0.0.8.tar` & `funasr_onnx-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 11:00:59.802449 funasr_onnx-0.0.8/
--rw-r--r--   0 zhifu      (502) staff       (20)     8882 2023-05-08 11:00:59.802146 funasr_onnx-0.0.8/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     8264 2023-04-23 09:14:56.000000 funasr_onnx-0.0.8/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 11:00:59.797955 funasr_onnx-0.0.8/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.0.8/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr_onnx-0.0.8/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12299 2023-05-08 10:59:00.000000 funasr_onnx-0.0.8/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 11:00:59.801048 funasr_onnx-0.0.8/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.0.8/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.0.8/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr_onnx-0.0.8/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.0.8/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.0.8/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr_onnx-0.0.8/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr_onnx-0.0.8/funasr_onnx/vad_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 11:00:59.799197 funasr_onnx-0.0.8/funasr_onnx.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8882 2023-05-08 11:00:59.000000 funasr_onnx-0.0.8/funasr_onnx.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)      485 2023-05-08 11:00:59.000000 funasr_onnx-0.0.8/funasr_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-08 11:00:59.000000 funasr_onnx-0.0.8/funasr_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       90 2023-05-08 11:00:59.000000 funasr_onnx-0.0.8/funasr_onnx.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-05-08 11:00:59.000000 funasr_onnx-0.0.8/funasr_onnx.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-08 11:00:59.802528 funasr_onnx-0.0.8/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-05-08 10:59:26.000000 funasr_onnx-0.0.8/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-12 02:20:35.472169 funasr_onnx-0.0.9/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8882 2023-05-12 02:20:35.471778 funasr_onnx-0.0.9/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     8264 2023-04-23 09:14:56.000000 funasr_onnx-0.0.9/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-12 02:20:35.467738 funasr_onnx-0.0.9/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.0.9/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8754 2023-05-12 02:16:09.000000 funasr_onnx-0.0.9/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12299 2023-05-08 10:59:00.000000 funasr_onnx-0.0.9/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-12 02:20:35.471237 funasr_onnx-0.0.9/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.0.9/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.0.9/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr_onnx-0.0.9/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.0.9/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.0.9/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr_onnx-0.0.9/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr_onnx-0.0.9/funasr_onnx/vad_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-12 02:20:35.468883 funasr_onnx-0.0.9/funasr_onnx.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8882 2023-05-12 02:20:35.000000 funasr_onnx-0.0.9/funasr_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)      485 2023-05-12 02:20:35.000000 funasr_onnx-0.0.9/funasr_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-12 02:20:35.000000 funasr_onnx-0.0.9/funasr_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      113 2023-05-12 02:20:35.000000 funasr_onnx-0.0.9/funasr_onnx.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-05-12 02:20:35.000000 funasr_onnx-0.0.9/funasr_onnx.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-12 02:20:35.472251 funasr_onnx-0.0.9/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 02:10:33.000000 funasr_onnx-0.0.9/setup.py
```

### Comparing `funasr_onnx-0.0.8/PKG-INFO` & `funasr_onnx-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr_onnx
-Version: 0.0.8
+Version: 0.0.9
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
```

### Comparing `funasr_onnx-0.0.8/README.md` & `funasr_onnx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.0.9/funasr_onnx/paraformer_bin.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,33 @@
     """
     def __init__(self, model_dir: Union[str, Path] = None,
                  batch_size: int = 1,
                  device_id: Union[str, int] = "-1",
                  plot_timestamp_to: str = "",
                  quantize: bool = False,
                  intra_op_num_threads: int = 4,
+                 cache_dir=None
                  ):
 
         if not Path(model_dir).exists():
-            raise FileNotFoundError(f'{model_dir} does not exist.')
+            from modelscope.hub.snapshot_download import snapshot_download
+            try:
+                model_dir = snapshot_download(model_dir, cache_dir=cache_dir)
+            except:
+                raise "model_dir must be model_name in modelscope or local path downloaded from modelscope, but is {}".format(model_dir)
+            from funasr.export.export_model import ModelExport
+            export_model = ModelExport(
+                cache_dir=cache_dir,
+                onnx=True,
+                device="cpu",
+                quant=quantize,
+            )
+            export_model.export(args.model_name)
+            
+            
 
         model_file = os.path.join(model_dir, 'model.onnx')
         if quantize:
             model_file = os.path.join(model_dir, 'model_quant.onnx')
         config_file = os.path.join(model_dir, 'config.yaml')
         cmvn_file = os.path.join(model_dir, 'am.mvn')
         config = read_yaml(config_file)
```

### Comparing `funasr_onnx-0.0.8/funasr_onnx/punc_bin.py` & `funasr_onnx-0.0.9/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/utils/e2e_vad.py` & `funasr_onnx-0.0.9/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/utils/frontend.py` & `funasr_onnx-0.0.9/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.0.9/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.0.9/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/utils/utils.py` & `funasr_onnx-0.0.9/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx/vad_bin.py` & `funasr_onnx-0.0.9/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.8/funasr_onnx.egg-info/PKG-INFO` & `funasr_onnx-0.0.9/funasr_onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr-onnx
-Version: 0.0.8
+Version: 0.0.9
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
```

### Comparing `funasr_onnx-0.0.8/setup.py` & `funasr_onnx-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,32 +9,39 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.8'
+VERSION_NUM = '0.0.9'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license='MIT',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
-    install_requires=["librosa", "onnxruntime>=1.7.0",
-                      "scipy", "numpy>=1.19.3",
-                      "typeguard", "kaldi-native-fbank",
-                      "PyYAML>=5.1.2"],
+    install_requires=["librosa",
+                      "onnxruntime>=1.7.0",
+                      "scipy",
+                      "numpy>=1.19.3",
+                      "typeguard",
+                      "kaldi-native-fbank",
+                      "PyYAML>=5.1.2",
+                      "funasr",
+                      "modelscope",
+                      "onnx"
+                      ],
     packages=[MODULE_NAME, f'{MODULE_NAME}.utils'],
     keywords=[
         'funasr,asr'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

