# Comparing `tmp/discotoolkit-1.0.4.tar.gz` & `tmp/discotoolkit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.4.tar", last modified: Thu May 11 01:55:40 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.5.tar", last modified: Fri May 12 05:32:43 2023, max compression
```

## Comparing `discotoolkit-1.0.4.tar` & `discotoolkit-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:55:29.168960 discotoolkit-1.0.4/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.4/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      729 2023-05-11 01:55:29.164960 discotoolkit-1.0.4/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     1433 2023-05-11 01:51:49.000000 discotoolkit-1.0.4/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:55:29.120961 discotoolkit-1.0.4/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-11 01:50:32.000000 discotoolkit-1.0.4/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.4/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-03 17:04:16.000000 discotoolkit-1.0.4/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     6958 2023-05-11 01:51:05.000000 discotoolkit-1.0.4/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-03 17:04:16.000000 discotoolkit-1.0.4/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.4/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      107 2023-05-10 06:00:24.000000 discotoolkit-1.0.4/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-11 01:55:29.156960 discotoolkit-1.0.4/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      729 2023-05-11 01:55:28.000000 discotoolkit-1.0.4/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-11 01:55:29.000000 discotoolkit-1.0.4/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-11 01:55:28.000000 discotoolkit-1.0.4/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      106 2023-05-11 01:55:28.000000 discotoolkit-1.0.4/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-11 01:55:28.000000 discotoolkit-1.0.4/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-11 01:55:29.168960 discotoolkit-1.0.4/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-11 01:55:08.000000 discotoolkit-1.0.4/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-12 05:32:32.440271 discotoolkit-1.0.5/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.5/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      729 2023-05-12 05:32:32.436271 discotoolkit-1.0.5/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1930 2023-05-12 05:32:16.000000 discotoolkit-1.0.5/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-12 05:32:32.412272 discotoolkit-1.0.5/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-11 01:50:32.000000 discotoolkit-1.0.5/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.5/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-12 05:20:20.000000 discotoolkit-1.0.5/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     7377 2023-05-12 05:28:51.000000 discotoolkit-1.0.5/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.5/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.5/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      130 2023-05-12 05:32:13.000000 discotoolkit-1.0.5/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-12 05:32:32.432271 discotoolkit-1.0.5/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      729 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      106 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-12 05:32:32.000000 discotoolkit-1.0.5/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-12 05:32:32.440271 discotoolkit-1.0.5/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-12 05:30:50.000000 discotoolkit-1.0.5/setup.py
```

### Comparing `discotoolkit-1.0.4/PKG-INFO` & `discotoolkit-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
-Requires-Python: >=3.8.10
+Requires-Python: >=3.8.16
 Description-Content-Type: text/markdown
 
 
     DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     
 
     Filter and download DISCO data based on sample metadata and cell type information
```

### Comparing `discotoolkit-1.0.4/README.md` & `discotoolkit-1.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,32 +2,32 @@
  * @Descripttion: 
  * @version: 
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
-# DISCOtoolkit 1.0.3
+# DISCOtoolkit 1.0.5
 
-DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). It provides the following functions:
+DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://jinmiaochenlab.github.io/DISCOtoolkit_py/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
-- CellMapper: project data into DISCO atlas
 
 Dependency Requirements:
+
 - Numpy 1.21.6
 - Pandas 1.4.2
 - Scanpy 1.9.3
 - Scipy 1.8.0
 - joblib 1.1.0
 - pandarallel 1.6.5
 
-Installation guide:
+## Installation guide:
 
 we recommend to install miniconda first and install discotoolkit in virtual env
 
 ```
 conda create --name disco python=3.8
 conda install pip
 conda install ipykernel
@@ -36,14 +36,23 @@
 
 Installation using pip:
 ``` 
 python -m pip install discotoolkit
 ```
 
 ## Basic Usage
-Example in Jupyter notebook
+Example in Jupyter notebook.
+
+<em>please select disco as the kernel for running the jupyter notebook</em>
+
+### [Filter and download DISCO data](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/docs/download_data.ipynb)
+
+### [Cell Type Annotation using CELLiD](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/docs/CELLiD_celltype_annotation.ipynb)
 
-### [Filter and download DISCO data](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/download_data.ipynb)
+### [scEnrichment](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/docs/scEnrichment.ipynb)
 
-### [Cell Type Annotation using CELLiD](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/CELLiD_celltype_annotation.ipynb)
+## Citation
+1. [Li, Mengwei, et al. "DISCO: a database of Deeply Integrated human Single-Cell Omics data." Nucleic acids research 50.D1 (2022): D596-D602.](https://academic.oup.com/nar/article/50/D1/D596/6430491)
 
-### [scEnrichment](https://github.com/JinmiaoChenLab/DISCOtoolkit_py/blob/main/scEnrichment.ipynb)
+## Follow us on our social media!
+- [HSCRM2](https://twitter.com/HSCRM2)
+- [JinmiaoChenLab Github repo](https://github.com/JinmiaoChenLab)
```

### Comparing `discotoolkit-1.0.4/discotoolkit/CELLiD.py` & `discotoolkit-1.0.5/discotoolkit/CELLiD.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.4/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.5/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.4/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.5/discotoolkit/DownloadDiscoData.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,26 +44,27 @@
 
         # getting the dataframe of the samples
         samples = metadata.sample_metadata
 
         # iterate through all the samples
         for i in range(len(samples)):
             s = list(samples["sampleId"])[i]
+            p = list(samples["projectId"])[i]
             output_file = "%s/%s.h5ad" % (output_dir, s) # getting the name of the file
 
             # condition if the file has been downloaded before
             if (os.path.exists(output_file)) and \
             hashlib.md5(open(output_file, "rb").read()).hexdigest() == list(samples["md5h5ad"])[i]:
                 logging.info(" %s has been downloaded before. Ignore ..." % (s)) # giving message to the user
             else:
                 logging.info("Downloading data of %s" % (s)) # giving message to the user
 
                 try:
                     # try to download the data as requested
-                    response = requests.get(url=prefix_disco_url + "getH5adBySample?sample=" + s)
+                    response = requests.get(url=prefix_disco_url + "getH5adBySample?project="+ p +"&sample=" + s)
 
                     # condition for error in downloading the samples
                     if response.status_code == 404:
                         error_sample.append(s) # append the error samples into a list for debugging later on
                         logging.warning("sample %s download fail" % (s)) # giving message to the user
                     else:
                         # write the file to directory
@@ -77,44 +78,47 @@
                 except:
                     # except error when the download fail
                     error_sample.append(s)
                     logging.warning("sample %s download fail" % (s))
         
         # if there are error samples, we set all the attribute for FilterData object to the error samples and return the object in FilterData object
         if len(error_sample) > 0:
-            metadata.sample_metadata.set_index("sampleId", inplace = True)
+            metadata.sample_metadata = metadata.sample_metadata.set_index("sampleId") # change from inplace to this to increase efficiency
             metadata.sample_metadata = metadata.sample_metadata.loc[error_sample]
             metadata.cell_type_metadata = metadata.cell_type_metadata.iloc[check_in_list(metadata.cell_type_metadata["sampleId"], error_sample)]
             metadata.cell_count = metadata.cell_type_metadata["cellNumber"].sum()
             metadata.sample_count = len(error_sample)
             return metadata
         
     else:
         # get the dataframe for the metadata
+        metadata.sample_metadata = metadata.sample_metadata.set_index("sampleId")
         samples = metadata.cell_type_metadata
         concat_func = lambda x,y: x + "_" + str(y)
 
         # create new element by concatenating the sampleId and cluster
         samples["sampleId"] = list(map(concat_func, list(samples["sampleId"]),
                                        list(samples["cluster"])))
         
         # similarly, iterative through all the sample for downloading
         for i in range(len(samples)):
             s = list(samples["sampleId"])[i]
+            sub_s = s.replace("_" + str(list(samples["cluster"])[i]) , "") # adding handler for celltype specific to get the data
+            p = metadata.sample_metadata.loc[sub_s]["projectId"]
             output_file = "%s/%s.h5ad" % (output_dir, s)
             
             # checking for file and ignore if it is already exist
             if (os.path.exists(output_file)) and \
             hashlib.md5(open(output_file, "rb").read()).hexdigest() == list(samples["h5adMd5"]):
                 logging.info(" %s has been downloaded before. Ignore ..." % (s)) # give message to the user
             else:
                 logging.info("Downloading data of %s" % (s)) # give message to the user
                 try:
                     # get the data from the server
-                    response = requests.get(url=prefix_disco_url + "getH5adBySampleCt?sample=" + s)
+                    response = requests.get(url=prefix_disco_url + "getH5adBySampleCt?project="+ p +"&sample=" + s)
                     if response.status_code == 404:
                         error_sample.append(s) # append error samples
                         logging.warning("sample %s download fail 1" % (s)) # give message to the user
                     else:
                         open(output_file, "wb").write(response.content)
                         
                         # condition for another error
```

### Comparing `discotoolkit-1.0.4/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.5/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.4/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.5/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.4/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.5/discotoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.4
+Version: 1.0.5
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
-Requires-Python: >=3.8.10
+Requires-Python: >=3.8.16
 Description-Content-Type: text/markdown
 
 
     DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     
 
     Filter and download DISCO data based on sample metadata and cell type information
```

### Comparing `discotoolkit-1.0.4/setup.py` & `discotoolkit-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='discotoolkit',
-    version='1.0.4',
+    version='1.0.5',
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
-    python_requires = '>=3.8.10',
+    python_requires = '>=3.8.16',
     include_package_data=True,
     long_description="""
     DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     \n
     Filter and download DISCO data based on sample metadata and cell type information
     \nCELLiD: cell type annotation
     \nscEnrichment: geneset enrichment using DISCO DEGs
```

