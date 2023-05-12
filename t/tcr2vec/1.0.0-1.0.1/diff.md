# Comparing `tmp/tcr2vec-1.0.0.tar.gz` & `tmp/tcr2vec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcr2vec-1.0.0.tar", last modified: Tue Mar 21 03:19:43 2023, max compression
+gzip compressed data, was "tcr2vec-1.0.1.tar", last modified: Fri May 12 13:13:12 2023, max compression
```

## Comparing `tcr2vec-1.0.0.tar` & `tcr2vec-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,44 @@
-drwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)        0 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/
-drwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)        0 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec.egg-info/
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)        8 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec.egg-info/top_level.txt
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)        1 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec.egg-info/dependency_links.txt
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)       78 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec.egg-info/requires.txt
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)      900 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec.egg-info/PKG-INFO
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)      487 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec.egg-info/SOURCES.txt
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)        1 2023-03-19 14:48:47.000000 tcr2vec-1.0.0/tcr2vec.egg-info/not-zip-safe
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     1332 2023-03-19 14:48:44.000000 tcr2vec-1.0.0/setup.py
--rwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)     6107 2023-03-20 14:57:46.000000 tcr2vec-1.0.0/README.md
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)    35149 2023-03-19 13:08:16.000000 tcr2vec-1.0.0/LICENSE
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)       38 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/setup.cfg
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)      900 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/PKG-INFO
-drwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)        0 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec/
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)       50 2023-03-19 14:38:55.000000 tcr2vec-1.0.0/tcr2vec/__init__.py
--rwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)     3578 2023-03-19 13:50:27.000000 tcr2vec-1.0.0/tcr2vec/dataset.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     5755 2023-03-20 09:04:35.000000 tcr2vec-1.0.0/tcr2vec/cdr3_to_full_seq.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     8167 2023-03-20 13:40:54.000000 tcr2vec-1.0.0/tcr2vec/evaluate.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     1431 2023-03-19 15:23:27.000000 tcr2vec-1.0.0/tcr2vec/embed.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     5091 2023-03-20 13:44:29.000000 tcr2vec-1.0.0/tcr2vec/finetune.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     4705 2023-03-20 07:34:57.000000 tcr2vec-1.0.0/tcr2vec/predict.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     2655 2023-03-20 07:11:07.000000 tcr2vec-1.0.0/tcr2vec/model.py
-drwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)        0 2023-03-21 03:19:43.000000 tcr2vec-1.0.0/tcr2vec/Epi_model/
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)        0 2023-03-19 14:59:29.000000 tcr2vec-1.0.0/tcr2vec/Epi_model/__init__.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     4544 2023-03-20 08:16:43.000000 tcr2vec-1.0.0/tcr2vec/Epi_model/epi_encode_ed.py
--rw-rw-r--   0 yuepjiang3  (1000) yuepjiang3  (1000)     2596 2023-03-19 13:11:23.000000 tcr2vec-1.0.0/tcr2vec/Epi_model/epi_encode_ae.py
--rwxrwxr-x   0 yuepjiang3  (1000) yuepjiang3  (1000)     1757 2023-03-20 07:22:14.000000 tcr2vec-1.0.0/tcr2vec/utils.py
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.565219 tcr2vec-1.0.1/
+-rwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)      166 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/.gitignore
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)    35149 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/LICENSE
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)      889 2023-05-12 13:13:12.565219 tcr2vec-1.0.1/PKG-INFO
+-rwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)     6272 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/README.md
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.557219 tcr2vec-1.0.1/figures/
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)  1847578 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/figures/workflow.jpg
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)       80 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/requirements.txt
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.561219 tcr2vec-1.0.1/scripts/
+-rwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)     1944 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/scripts/run.sh
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)      891 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/scripts/test_tcr2vec.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)       38 2023-05-12 13:13:12.565219 tcr2vec-1.0.1/setup.cfg
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     1347 2023-05-12 13:11:56.000000 tcr2vec-1.0.1/setup.py
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.561219 tcr2vec-1.0.1/tcr2vec/
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.561219 tcr2vec-1.0.1/tcr2vec/Epi_model/
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)      763 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/Epi_model/Atchley_factors.csv
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/Epi_model/__init__.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)   237157 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/Epi_model/aaindex2.txt
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     2596 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/Epi_model/epi_encode_ae.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     4544 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/Epi_model/epi_encode_ed.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)   983704 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/Epi_model/ept_trained_AE.h5
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)       50 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/__init__.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     5996 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/cdr3_to_full_seq.py
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.561219 tcr2vec-1.0.1/tcr2vec/data/
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.561219 tcr2vec-1.0.1/tcr2vec/data/TCR_gene_segment_data/
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     8783 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/data/TCR_gene_segment_data/J_segment_sequences.fasta
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)    47296 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/data/TCR_gene_segment_data/V_segment_sequences.fasta
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     8223 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/data/sample.csv
+-rwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)     3578 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/dataset.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     1431 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/embed.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     8167 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/evaluate.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     5091 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/finetune.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     2655 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/model.py
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     4705 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/predict.py
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.565219 tcr2vec-1.0.1/tcr2vec/results/
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)     8224 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/results/sample_full.csv
+-rwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)     1757 2023-05-12 13:03:56.000000 tcr2vec-1.0.1/tcr2vec/utils.py
+drwxrwxr-x   0 yuepengjiang  (1000) yuepengjiang  (1000)        0 2023-05-12 13:13:12.561219 tcr2vec-1.0.1/tcr2vec.egg-info/
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)      889 2023-05-12 13:13:12.000000 tcr2vec-1.0.1/tcr2vec.egg-info/PKG-INFO
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)      858 2023-05-12 13:13:12.000000 tcr2vec-1.0.1/tcr2vec.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)        1 2023-05-12 13:13:12.000000 tcr2vec-1.0.1/tcr2vec.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)        1 2023-05-12 13:12:00.000000 tcr2vec-1.0.1/tcr2vec.egg-info/not-zip-safe
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)       78 2023-05-12 13:13:12.000000 tcr2vec-1.0.1/tcr2vec.egg-info/requires.txt
+-rw-rw-r--   0 yuepengjiang  (1000) yuepengjiang  (1000)        8 2023-05-12 13:13:12.000000 tcr2vec-1.0.1/tcr2vec.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tcr2vec-1.0.0/tcr2vec.egg-info/PKG-INFO` & `tcr2vec-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: tcr2vec
-Version: 1.0.0
+Version: 1.0.1
 Summary: TCR2vec is a deep representation learning framework of T-cell receptor sequence and function
 Home-page: https://github.com/jiangdada1221/TCR2vec
 Author: Yuepeng Jiang
 Author-email: jiangdada12344321@gmail.com
 License: GPLv3
+Description: Not applicable
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
-Not applicable
-
```

### Comparing `tcr2vec-1.0.0/setup.py` & `tcr2vec-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from setuptools import setup, find_packages
 data_files_to_include = [('', ['README.md', 'LICENSE'])]
 
-with open('requirements.txt', 'r') as reqs:
-    requirements = reqs.read().split()
-
-setup(name='tcr2vec',
-      packages=find_packages(),
-      version='1.0.0',
+setup(name='tcr2vec',      
+      version='1.0.1',
       description='TCR2vec is a deep representation learning framework of T-cell receptor sequence and function',
       long_description='Not applicable',
       url='https://github.com/jiangdada1221/TCR2vec',
       author='Yuepeng Jiang',
       author_email='jiangdada12344321@gmail.com',
-      license='GPLv3',
-      install_requires=requirements,
+      license='GPLv3',      
       classifiers=[
             'Development Status :: 3 - Alpha',
             'Intended Audience :: Developers',
             'Intended Audience :: Healthcare Industry',
             'Intended Audience :: Science/Research',
             'Topic :: Scientific/Engineering :: Bio-Informatics',
             'Topic :: Scientific/Engineering :: Artificial Intelligence',
             'Topic :: Scientific/Engineering :: Medical Science Apps.',
             'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
             'Natural Language :: English',
             'Programming Language :: Python :: 3',
             ],
+      packages = find_packages(),
+      install_requires=['numpy','torch','matplotlib','tqdm','pandas','scikit-learn','Scipy','tape_proteins','biopython'],
       data_files = data_files_to_include,
       include_package_data=True,
       zip_safe=False)
```

### Comparing `tcr2vec-1.0.0/README.md` & `tcr2vec-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TCR2vec
-TCR2vec is a python software designed for embedding TCR sequences into numerical vectors. It is a transformer-based model that pretrained with __MLM__ and __SPM__ (similarity preservation modeling). After the multi-task pretraining stage, TCR2vec is able to transform amino acid sequences of TCRs into a similarity preserved embedding space with contextual understanding of the language of TCRs. Similar TCRs in sequence space have smaller Euclidean distances in vector space while divergent TCRs have larger Euclidean distances. The workflow of the pretraining process is shown below. <br />
+TCR2vec is a python software designed for embedding TCR sequences into numerical vectors. It is a transformer-based model that pretrained with __MLM__ and __SPM__ (similarity preservation modeling). After the multi-task pretraining stage, TCR2vec is able to transform amino acid sequences of TCRs into a similarity preserved embedding space with contextual understanding of the language of TCRs. Similar TCRs in sequence space have smaller Euclidean distances in vector space while divergent TCRs have larger Euclidean distances. The workflow of the pretraining process is shown below. TCR2vec can also be finetuned for better performance on task-specific data. <br />
 
 <img src="https://github.com/jiangdada1221/TCR2vec_train/blob/main/figures/workflow.jpg" width="800"> <br />
 
 ## Dependencies
 TCR2vec is writen in Python based on the deeplearning library - Pytorch. Compared to Tensorflow, Pytorch is more user-friendly in __version compatibility__. I would strongly suggest using Pytorch as the deeplearning library so that followers can easily run the code with less pain in making Tensorflow work.  <br />
 
 The required software dependencies are listed below:
@@ -41,14 +41,16 @@
 import torch
 from tcr2vec.model import TCR2vec
 from tape import TAPETokenizer
 
 path_to_TCR2vec = 'path_to_pretrained_TCR2vec'
 emb_model = TCR2vec(path_to_TCR2vec)
 tokenizer = TAPETokenizer(vocab='iupac') 
+#by default, the device for emb_model is cpu
+#emb_model = emb_model.to('cuda:0') #to gpu
 
 #example TCR
 seq = 'NAGVTQTPKFQVLKTGQSMTLQCAQDMNHNSMYWYRQDPGMGLRLIYYSASEGTTDKGEVPNGYNVSRLNKREFSLRLESAAPSQTSVYFCASSEALGTGNTIYFGEGSWLTVV'
 token_ids = torch.tensor([tokenizer.encode(seq)])
 output = emb_model(token_ids) # shape of 1 x 120
 
 #convert to numpy array
```

### Comparing `tcr2vec-1.0.0/LICENSE` & `tcr2vec-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/PKG-INFO` & `tcr2vec-1.0.1/tcr2vec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: tcr2vec
-Version: 1.0.0
+Version: 1.0.1
 Summary: TCR2vec is a deep representation learning framework of T-cell receptor sequence and function
 Home-page: https://github.com/jiangdada1221/TCR2vec
 Author: Yuepeng Jiang
 Author-email: jiangdada12344321@gmail.com
 License: GPLv3
+Description: Not applicable
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
-Not applicable
-
```

### Comparing `tcr2vec-1.0.0/tcr2vec/dataset.py` & `tcr2vec-1.0.1/tcr2vec/dataset.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/cdr3_to_full_seq.py` & `tcr2vec-1.0.1/tcr2vec/cdr3_to_full_seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,20 @@
 
         else:
             ## Deal with inconsistent naming conventions of segments
             Vname_adapted = rename_Vseg(Vname)
             if Vname_adapted in Vrecord.id:
                 Vseq = Vrecord.seq
                 foundV = True
-
+            elif '-' in Vname_adapted:
+                Vname_adapted = Vname_adapted.split('-')[0]
+                if Vname_adapted in Vrecord.id:
+                    Vseq = Vrecord.seq
+                    foundV = True
+                    
     for Jrecord in SeqIO.parse(
         os.path.join(directory, 'J_segment_sequences.fasta'), "fasta"
     ):
         if type(Jname) != str or Jname == 'unresolved':
             print('Jname not string but ', Jname, type(Jname))
             Jseq = ''
         else:
@@ -176,8 +181,8 @@
 
 if __name__ == '__main__':
     # parse arguments
     args = parser.parse_args()
     main(
         args.directory, args.input_sequences, args.v_seg_header,
         args.j_seg_header, args.cdr3_header, args.output
-    )
+    )
```

### Comparing `tcr2vec-1.0.0/tcr2vec/evaluate.py` & `tcr2vec-1.0.1/tcr2vec/evaluate.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/embed.py` & `tcr2vec-1.0.1/tcr2vec/embed.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/finetune.py` & `tcr2vec-1.0.1/tcr2vec/finetune.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/predict.py` & `tcr2vec-1.0.1/tcr2vec/predict.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/model.py` & `tcr2vec-1.0.1/tcr2vec/model.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/Epi_model/epi_encode_ed.py` & `tcr2vec-1.0.1/tcr2vec/Epi_model/epi_encode_ed.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/Epi_model/epi_encode_ae.py` & `tcr2vec-1.0.1/tcr2vec/Epi_model/epi_encode_ae.py`

 * *Files identical despite different names*

### Comparing `tcr2vec-1.0.0/tcr2vec/utils.py` & `tcr2vec-1.0.1/tcr2vec/utils.py`

 * *Files identical despite different names*

