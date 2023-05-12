# Comparing `tmp/cuteSV-2.0.2.tar.gz` & `tmp/cuteSV-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cuteSV-2.0.2.tar", last modified: Thu Nov  3 05:38:42 2022, max compression
+gzip compressed data, was "dist/cuteSV-2.0.3.tar", last modified: Fri May 12 03:03:04 2023, max compression
```

## Comparing `cuteSV-2.0.2.tar` & `cuteSV-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:38:42.871345 cuteSV-2.0.2/
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     1065 2022-11-03 05:36:07.000000 cuteSV-2.0.2/LICENSE
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    14248 2022-11-03 05:38:42.871345 cuteSV-2.0.2/PKG-INFO
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    13943 2022-11-03 05:36:07.000000 cuteSV-2.0.2/README.md
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)       38 2022-11-03 05:38:42.871345 cuteSV-2.0.2/setup.cfg
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)      759 2022-11-03 05:36:07.000000 cuteSV-2.0.2/setup.py
-drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:38:42.867345 cuteSV-2.0.2/src/
-drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:38:42.871345 cuteSV-2.0.2/src/benchmarks/
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/__init__.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     8612 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/cmp_NA19240.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    13868 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/eval_sim.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5834 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/eval_trio.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5587 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/multi_platform.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     6919 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/sta_venn.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     2511 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/benchmarks/vcf2bedpe.py
-drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:38:42.871345 cuteSV-2.0.2/src/cuteSV/
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5159 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/CommandRunner.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/__init__.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    38706 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    11720 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_Description.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    24266 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_forcecalling.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    21077 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_genotype.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     7493 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_resolveDUP.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    20199 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_resolveINDEL.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    11687 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_resolveINV.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     8789 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/cuteSV_resolveTRA.py
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     2991 2022-11-03 05:36:07.000000 cuteSV-2.0.2/src/cuteSV/diploid_calling.py
-drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2022-11-03 05:38:42.871345 cuteSV-2.0.2/src/cuteSV.egg-info/
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    14248 2022-11-03 05:38:42.000000 cuteSV-2.0.2/src/cuteSV.egg-info/PKG-INFO
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)      754 2022-11-03 05:38:42.000000 cuteSV-2.0.2/src/cuteSV.egg-info/SOURCES.txt
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        1 2022-11-03 05:38:42.000000 cuteSV-2.0.2/src/cuteSV.egg-info/dependency_links.txt
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        1 2022-11-03 05:38:23.000000 cuteSV-2.0.2/src/cuteSV.egg-info/not-zip-safe
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)       34 2022-11-03 05:38:42.000000 cuteSV-2.0.2/src/cuteSV.egg-info/requires.txt
--rw-rw-r--   0 sqcao     (1009) sqcao     (1009)       18 2022-11-03 05:38:42.000000 cuteSV-2.0.2/src/cuteSV.egg-info/top_level.txt
+drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 03:03:04.118217 cuteSV-2.0.3/
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     1065 2023-05-12 02:13:53.000000 cuteSV-2.0.3/LICENSE
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    14544 2023-05-12 03:03:04.118217 cuteSV-2.0.3/PKG-INFO
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    14239 2023-05-12 02:13:53.000000 cuteSV-2.0.3/README.md
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)       38 2023-05-12 03:03:04.118217 cuteSV-2.0.3/setup.cfg
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)      759 2023-05-12 02:28:47.000000 cuteSV-2.0.3/setup.py
+drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 03:03:04.114217 cuteSV-2.0.3/src/
+drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 03:03:04.114217 cuteSV-2.0.3/src/benchmarks/
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/__init__.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     8612 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/cmp_NA19240.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     4349 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/eval_BND.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     2357 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/eval_generegion.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5780 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/eval_population.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    13868 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/eval_sim.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5834 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/eval_trio.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5587 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/multi_platform.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     6919 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/sta_venn.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     2511 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/benchmarks/vcf2bedpe.py
+drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 03:03:04.118217 cuteSV-2.0.3/src/cuteSV/
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     5159 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/CommandRunner.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/__init__.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    39195 2023-05-12 02:17:51.000000 cuteSV-2.0.3/src/cuteSV/cuteSV
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    11900 2023-05-12 02:21:52.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_Description.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    24266 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_forcecalling.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    24434 2023-05-12 02:24:04.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_genotype.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     8042 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_resolveDUP.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    20199 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_resolveINDEL.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    11687 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_resolveINV.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     8789 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/cuteSV_resolveTRA.py
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)     2991 2023-05-12 02:13:53.000000 cuteSV-2.0.3/src/cuteSV/diploid_calling.py
+drwxrwxr-x   0 sqcao     (1009) sqcao     (1009)        0 2023-05-12 03:03:04.118217 cuteSV-2.0.3/src/cuteSV.egg-info/
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)    14544 2023-05-12 03:03:03.000000 cuteSV-2.0.3/src/cuteSV.egg-info/PKG-INFO
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)      849 2023-05-12 03:03:03.000000 cuteSV-2.0.3/src/cuteSV.egg-info/SOURCES.txt
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        1 2023-05-12 03:03:03.000000 cuteSV-2.0.3/src/cuteSV.egg-info/dependency_links.txt
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)        1 2023-05-12 03:03:03.000000 cuteSV-2.0.3/src/cuteSV.egg-info/not-zip-safe
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)       34 2023-05-12 03:03:03.000000 cuteSV-2.0.3/src/cuteSV.egg-info/requires.txt
+-rw-rw-r--   0 sqcao     (1009) sqcao     (1009)       18 2023-05-12 03:03:03.000000 cuteSV-2.0.3/src/cuteSV.egg-info/top_level.txt
```

### Comparing `cuteSV-2.0.2/LICENSE` & `cuteSV-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/PKG-INFO` & `cuteSV-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuteSV
-Version: 2.0.2
+Version: 2.0.3
 Summary: Long-read-based human genomic structural variation detection with cuteSV
 Home-page: https://github.com/tjiangHIT/cuteSV
 Author: Jiang Tao
 Author-email: tjiang@hit.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -51,14 +51,16 @@
 
 BTW, we used [Truvari](https://github.com/spiralgenetics/truvari) to calculate the recall, precision, and f-measure.
 For more detailed implementation of SV benchmarks, we show an example [here](https://github.com/tjiangHIT/sv-benchmark).
 
 ## Notice
 A new wiki page about diploid-assembly-based SV detection using cuteSV has been established. More details please see [here](https://github.com/tjiangHIT/cuteSV/wiki/Diploid-assembly-based-SV-detection-using-cuteSV).
 
+We provided a new document for applying **force calling** (or **regenotyping**) benchmark [here](https://github.com/tjiangHIT/cuteSV/tree/master/src/documentation).
+
 ---
 ### Dependence
 	
 	1. python3
 	2. pysam
 	3. Biopython
 	4. cigar
@@ -84,14 +86,16 @@
 		--diff_ratio_merging_DEL	0.5
 
 	> For ONT data:
 		--max_cluster_bias_INS		100
 		--diff_ratio_merging_INS	0.3
 		--max_cluster_bias_DEL	100
 		--diff_ratio_merging_DEL	0.3
+	> For force calling:
+		--min_mapq 			10
 	
 | Parameter | Description | Default |
 | :------------ |:---------------|-------------:|
 |--threads|Number of threads to use.| 16 |
 |--batches| Batch of genome segmentation interval.|10,000,000|
 |--sample| Sample name/id |NULL|
 |--retain_work_dir|Enable to retain temporary folder and files.|False|
@@ -112,14 +116,15 @@
 |--max_cluster_bias_DEL|Maximum distance to cluster read together for deletion.|200|
 |--diff_ratio_merging_DEL|Do not merge breakpoints with basepair identity more than the ratio of *default* for deletion.|0.5|
 |--max_cluster_bias_INV|Maximum distance to cluster read together for inversion.|500|
 |--max_cluster_bias_DUP|Maximum distance to cluster read together for duplication.|500|
 |--max_cluster_bias_TRA|Maximum distance to cluster read together for translocation.|50|
 |--diff_ratio_filtering_TRA|Filter breakpoints with basepair identity less than the ratio of *default* for translocation.|0.6|
 |--remain_reads_ratio|The ratio of reads remained in cluster to generate the breakpoint. Set lower to get more precise breakpoint when the alignment data have high quality but recommand over 0.5.|1|
+|-include_bed|Optional given bed file. Only detect SVs in regions in the BED file.|NULL|
 
 ---
 ### Datasets generated from cuteSV
 We provided the SV callsets of the HG002 human sample produced by cuteSV form three different long-read sequencing platforms (i.e. PacBio CLR, PacBio CCS, and ONT PromethION). 
 
 You can download them at: 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783083.svg)](https://doi.org/10.5281/zenodo.3783083)
```

### Comparing `cuteSV-2.0.2/README.md` & `cuteSV-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
 BTW, we used [Truvari](https://github.com/spiralgenetics/truvari) to calculate the recall, precision, and f-measure.
 For more detailed implementation of SV benchmarks, we show an example [here](https://github.com/tjiangHIT/sv-benchmark).
 
 ## Notice
 A new wiki page about diploid-assembly-based SV detection using cuteSV has been established. More details please see [here](https://github.com/tjiangHIT/cuteSV/wiki/Diploid-assembly-based-SV-detection-using-cuteSV).
 
+We provided a new document for applying **force calling** (or **regenotyping**) benchmark [here](https://github.com/tjiangHIT/cuteSV/tree/master/src/documentation).
+
 ---
 ### Dependence
 	
 	1. python3
 	2. pysam
 	3. Biopython
 	4. cigar
@@ -73,14 +75,16 @@
 		--diff_ratio_merging_DEL	0.5
 
 	> For ONT data:
 		--max_cluster_bias_INS		100
 		--diff_ratio_merging_INS	0.3
 		--max_cluster_bias_DEL	100
 		--diff_ratio_merging_DEL	0.3
+	> For force calling:
+		--min_mapq 			10
 	
 | Parameter | Description | Default |
 | :------------ |:---------------|-------------:|
 |--threads|Number of threads to use.| 16 |
 |--batches| Batch of genome segmentation interval.|10,000,000|
 |--sample| Sample name/id |NULL|
 |--retain_work_dir|Enable to retain temporary folder and files.|False|
@@ -101,14 +105,15 @@
 |--max_cluster_bias_DEL|Maximum distance to cluster read together for deletion.|200|
 |--diff_ratio_merging_DEL|Do not merge breakpoints with basepair identity more than the ratio of *default* for deletion.|0.5|
 |--max_cluster_bias_INV|Maximum distance to cluster read together for inversion.|500|
 |--max_cluster_bias_DUP|Maximum distance to cluster read together for duplication.|500|
 |--max_cluster_bias_TRA|Maximum distance to cluster read together for translocation.|50|
 |--diff_ratio_filtering_TRA|Filter breakpoints with basepair identity less than the ratio of *default* for translocation.|0.6|
 |--remain_reads_ratio|The ratio of reads remained in cluster to generate the breakpoint. Set lower to get more precise breakpoint when the alignment data have high quality but recommand over 0.5.|1|
+|-include_bed|Optional given bed file. Only detect SVs in regions in the BED file.|NULL|
 
 ---
 ### Datasets generated from cuteSV
 We provided the SV callsets of the HG002 human sample produced by cuteSV form three different long-read sequencing platforms (i.e. PacBio CLR, PacBio CCS, and ONT PromethION). 
 
 You can download them at: 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783083.svg)](https://doi.org/10.5281/zenodo.3783083)
```

### Comparing `cuteSV-2.0.2/setup.py` & `cuteSV-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name = "cuteSV",
-    version = "2.0.2",
+    version = "2.0.3",
     description = "Long-read-based human genomic structural variation detection with cuteSV",
     author = "Jiang Tao",
     author_email = "tjiang@hit.edu.cn",
     url = "https://github.com/tjiangHIT/cuteSV",
     license = "MIT",
     packages = find_packages("src"),
     package_dir = {"": "src"},
```

### Comparing `cuteSV-2.0.2/src/benchmarks/cmp_NA19240.py` & `cuteSV-2.0.3/src/benchmarks/cmp_NA19240.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/benchmarks/eval_sim.py` & `cuteSV-2.0.3/src/benchmarks/eval_sim.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/benchmarks/eval_trio.py` & `cuteSV-2.0.3/src/benchmarks/eval_trio.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/benchmarks/multi_platform.py` & `cuteSV-2.0.3/src/benchmarks/multi_platform.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/benchmarks/sta_venn.py` & `cuteSV-2.0.3/src/benchmarks/sta_venn.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/benchmarks/vcf2bedpe.py` & `cuteSV-2.0.3/src/benchmarks/vcf2bedpe.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV/CommandRunner.py` & `cuteSV-2.0.3/src/cuteSV/CommandRunner.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV` & `cuteSV-2.0.3/src/cuteSV/cuteSV`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 
 ''' 
  * All rights Reserved, Designed By HIT-Bioinformatics   
  * @Title: cuteSV 
  * @author: tjiang & sqcao
- * @date: Sep 12th 2022
- * @version V2.0.2
+ * @date: May 12th 2023
+ * @version V2.0.3
 '''
 
 import pysam
 import cigar
 from Bio import SeqIO
 from cuteSV.cuteSV_Description import parseArgs
 from multiprocessing import Pool
 from cuteSV.CommandRunner import *
 # from resolution_type import * 
 from cuteSV.cuteSV_resolveINV import run_inv
 from cuteSV.cuteSV_resolveTRA import run_tra
 from cuteSV.cuteSV_resolveINDEL import run_ins, run_del
 from cuteSV.cuteSV_resolveDUP import run_dup
-from cuteSV.cuteSV_genotype import generate_output, generate_pvcf, load_valuable_chr
+from cuteSV.cuteSV_genotype import generate_output, generate_pvcf, load_valuable_chr, load_bed
 from cuteSV.cuteSV_forcecalling import force_calling_chrom
 import os
 import argparse
 import logging
 import sys
 import time
 import gc
@@ -606,33 +606,43 @@
             if i[0] == 'SA':
                 Supplementary_info = i[1].split(';')[:-1]
                 organize_split_signal(primary_info, Supplementary_info, read.query_length, 
                     SV_size, min_mapq, max_split_parts, read.query_name, candidate, MaxSize, read.query_sequence)
     return candidate
 
 def single_pipe(sam_path, min_length, min_mapq, max_split_parts, min_read_len, temp_dir, 
-                task, min_siglength, merge_del_threshold, merge_ins_threshold, MaxSize):
+                task, min_siglength, merge_del_threshold, merge_ins_threshold, MaxSize, bed_regions):
 
     candidate = list()
     reads_info_list = list()
     Chr_name = task[0]
     samfile = pysam.AlignmentFile(sam_path)
 
     for read in samfile.fetch(Chr_name, task[1], task[2]):
-        if read.reference_start >= task[1]:
+        pos_start = read.reference_start # 0-based
+        pos_end = read.reference_end
+        in_bed = False
+        if bed_regions != None:
+            for bed_region in bed_regions:
+                if pos_end <= bed_region[0] or pos_start >= bed_region[1]:
+                    continue
+                else:
+                    in_bed = True
+                    break
+        else:
+            in_bed = True
+        if read.reference_start >= task[1] and in_bed:
             read_candidate = parse_read(read, Chr_name, min_length, min_mapq, max_split_parts, 
                                     min_read_len, min_siglength, merge_del_threshold, 
                                     merge_ins_threshold, MaxSize)
             candidate.extend(read_candidate)
             if read.mapq >= min_mapq:
                 is_primary = 0
                 if read.flag in [0, 16]:
                     is_primary = 1
-                pos_start = read.reference_start # 0-based
-                pos_end = read.reference_end
                 reads_info_list.append([pos_start, pos_end, is_primary, read.query_name])
     samfile.close()
     # print('finish %s:%d-%d in %f seconds.'%(task[0], task[1], len(reads_info_list), time.time() - start_time))
    
     if len(candidate) == 0:
         logging.info("Skip %s:%d-%d."%(Chr_name, task[1], task[2]))
         return
@@ -657,15 +667,14 @@
     reads_file = open(reads_output, 'w')
     for ele in reads_info_list:
         reads_file.write("%s\t%d\t%d\t%d\t%s\n"%(Chr_name, ele[0], ele[1], ele[2], ele[3]))
     reads_file.close()
     logging.info("Finished %s:%d-%d."%(Chr_name, task[1], task[2]))	
     gc.collect()
 
-
 def multi_run_wrapper(args):
     return single_pipe(*args)
 
 def main_ctrl(args, argv):
     if not os.path.isfile(args.reference):
         raise FileNotFoundError("[Errno 2] No such file: '%s'"%args.reference)
     if not os.path.exists(args.work_dir):
@@ -694,29 +703,31 @@
             pos = 0
             task_round = int(local_ref_len/args.batches)
             for j in range(task_round):
                 Task_list.append([i[0], pos, pos+args.batches])
                 pos += args.batches
             if pos < local_ref_len:
                 Task_list.append([i[0], pos, local_ref_len])
+    bed_regions = load_bed(args.include_bed, Task_list)
     #'''
     analysis_pools = Pool(processes=int(args.threads))
     os.mkdir("%ssignatures"%temporary_dir)
-    for i in Task_list:
+    for i in range(len(Task_list)):
         para = [(args.input, 
                     args.min_size, 
                     args.min_mapq, 
                     args.max_split_parts, 
                     args.min_read_len, 
                     temporary_dir, 
-                    i, 
+                    Task_list[i], 
                     args.min_siglength, 
                     args.merge_del_threshold, 
                     args.merge_ins_threshold, 
-                    args.max_size)]
+                    args.max_size,
+                    None if bed_regions == None else bed_regions[i])]
         analysis_pools.map_async(multi_run_wrapper, para)
     analysis_pools.close()
     analysis_pools.join()
     #'''
     #'''
     logging.info("Rebuilding signatures of structural variants.")
     analysis_pools = Pool(processes=int(args.threads))
```

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_Description.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_Description.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ''' 
  * All rights Reserved, Designed By HIT-Bioinformatics   
  * @Title:  cuteSV_Description.py
  * @author: tjiang & sqcao
- * @date: Sep 12th 2022
- * @version V2.0.2
+ * @date: May 12th 2023
+ * @version V2.0.3
 '''
 import argparse
 
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 
 class cuteSVdp(object):
 	'''
 	Detailed descriptions of cuteSV version and its parameters.
 	'''
 
 	USAGE="""\
@@ -116,14 +116,18 @@
 		help = "Maximum distance of deletion signals to be merged. In our paper, I used -md 500 to process HG002 real human sample data.[%(default)s]", 
 		default = 0, 
 		type = int)
 	GroupSignaturesCollect.add_argument('-mi', '--merge_ins_threshold', 
 		help = "Maximum distance of insertion signals to be merged. In our paper, I used -mi 500 to process HG002 real human sample data.[%(default)s]", 
 		default = 100, 
 		type = int)
+	GroupSignaturesCollect.add_argument('-include_bed', 
+		help = "Optional given bed file. Only detect SVs in regions in the BED file. [NULL]",
+		default = None,
+        type = str)
 	# The min_read_len in last version is 2000.
 	# signatures with overlap need to be filtered
 
 	# **************Parameters in clustering******************
 	GroupSVCluster = parser.add_argument_group('Generation of SV clusters')
 	GroupSVCluster.add_argument('-s', '--min_support', 
 		help = "Minimum number of reads that support a SV to be reported.[%(default)s]",
```

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_forcecalling.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_forcecalling.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_genotype.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_genotype.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,89 +4,89 @@
 import numpy as np
 
 err = 0.1
 prior = float(1/3)
 Genotype = ["0/0", "0/1", "1/1"]
 
 def log10sumexp(log10_probs):
-	# Normalization of Genotype likelihoods
-	m = max(log10_probs)
-	return m + log10(sum(pow(10.0, x-m) for x in log10_probs))
+    # Normalization of Genotype likelihoods
+    m = max(log10_probs)
+    return m + log10(sum(pow(10.0, x-m) for x in log10_probs))
 
 def normalize_log10_probs(log10_probs):
-	# Adjust the Genotype likelihoods
-	log10_probs = np.array(log10_probs)
-	lse = log10sumexp(log10_probs)
-	return np.minimum(log10_probs - lse, 0.0)
+    # Adjust the Genotype likelihoods
+    log10_probs = np.array(log10_probs)
+    lse = log10sumexp(log10_probs)
+    return np.minimum(log10_probs - lse, 0.0)
 
 def rescale_read_counts(c0, c1, max_allowed_reads=100):
-	"""Ensures that n_total <= max_allowed_reads, rescaling if necessary."""
-	Total = c0 + c1
-	if Total > max_allowed_reads:
-		c0 = int(max_allowed_reads * float(c0/Total))
-		c1 = max_allowed_reads - c0
-	return c0, c1
+    """Ensures that n_total <= max_allowed_reads, rescaling if necessary."""
+    Total = c0 + c1
+    if Total > max_allowed_reads:
+        c0 = int(max_allowed_reads * float(c0/Total))
+        c1 = max_allowed_reads - c0
+    return c0, c1
 
 def cal_GL(c0, c1):
-	# Approximate adjustment of events with larger read depth
-	c0, c1 = rescale_read_counts(c0, c1)
-	# original genotype likelihood
-	# ori_GL00 = np.float64(pow((1-err), c0)*pow(err, c1)*comb(c0+c1,c0)*(1-prior)/2)
-	# ori_GL11 = np.float64(pow(err, c0)*pow((1-err), c1)*comb(c0+c1,c0)*(1-prior)/2)
-	# ori_GL01 = np.float64(pow(0.5, c0+c1)*comb(c0+c1,c0)*prior)
-	
-	ori_GL00 = np.float64(pow((1-err), c0)*pow(err, c1)*(1-prior)/2)
-	ori_GL11 = np.float64(pow(err, c0)*pow((1-err), c1)*(1-prior)/2)
-	ori_GL01 = np.float64(pow(0.5, c0+c1)*prior)
-
-	# normalized genotype likelihood
-	prob = list(normalize_log10_probs([log10(ori_GL00), log10(ori_GL01), log10(ori_GL11)]))
-	GL_P = [pow(10, i) for i in prob]
-	PL = [int(np.around(-10*log10(i))) for i in GL_P]
-	GQ = [int(-10*log10(GL_P[1] + GL_P[2])), int(-10*log10(GL_P[0] + GL_P[2])), int(-10*log10(GL_P[0] + GL_P[1]))]
-	QUAL = abs(np.around(-10*log10(GL_P[0]), 1))
+    # Approximate adjustment of events with larger read depth
+    c0, c1 = rescale_read_counts(c0, c1)
+    # original genotype likelihood
+    # ori_GL00 = np.float64(pow((1-err), c0)*pow(err, c1)*comb(c0+c1,c0)*(1-prior)/2)
+    # ori_GL11 = np.float64(pow(err, c0)*pow((1-err), c1)*comb(c0+c1,c0)*(1-prior)/2)
+    # ori_GL01 = np.float64(pow(0.5, c0+c1)*comb(c0+c1,c0)*prior)
+    
+    ori_GL00 = np.float64(pow((1-err), c0)*pow(err, c1)*(1-prior)/2)
+    ori_GL11 = np.float64(pow(err, c0)*pow((1-err), c1)*(1-prior)/2)
+    ori_GL01 = np.float64(pow(0.5, c0+c1)*prior)
+
+    # normalized genotype likelihood
+    prob = list(normalize_log10_probs([log10(ori_GL00), log10(ori_GL01), log10(ori_GL11)]))
+    GL_P = [pow(10, i) for i in prob]
+    PL = [int(np.around(-10*log10(i))) for i in GL_P]
+    GQ = [int(-10*log10(GL_P[1] + GL_P[2])), int(-10*log10(GL_P[0] + GL_P[2])), int(-10*log10(GL_P[0] + GL_P[1]))]
+    QUAL = abs(np.around(-10*log10(GL_P[0]), 1))
 
-	return Genotype[prob.index(max(prob))], "%d,%d,%d"%(PL[0], PL[1], PL[2]), max(GQ), QUAL
+    return Genotype[prob.index(max(prob))], "%d,%d,%d"%(PL[0], PL[1], PL[2]), max(GQ), QUAL
 
 def cal_CIPOS(std, num):
-	pos = int(1.96 * std / num ** 0.5)
-	return "-%d,%d"%(pos,pos)
+    pos = int(1.96 * std / num ** 0.5)
+    return "-%d,%d"%(pos,pos)
 
 def threshold_ref_count(num):
-	if num <= 2:
-		return 20*num
-	elif 3 <= num <= 5:
-		return 9*num 
-	elif 6 <= num <= 15:
-		return 7*num
-	else:
-		return 5*num
+    if num <= 2:
+        return 20*num
+    elif 3 <= num <= 5:
+        return 9*num 
+    elif 6 <= num <= 15:
+        return 7*num
+    else:
+        return 5*num
 
 def count_coverage(chr, s, e, f, read_count, up_bound, itround):
-	status = 0
-	iteration = 0
-	primary_num = 0
-	for i in f.fetch(chr, s, e):
-		iteration += 1
-		if i.flag not in [0,16]:
-			continue
-		primary_num += 1
-		if i.reference_start < s and i.reference_end > e:
-			read_count.add(i.query_name)
-			if len(read_count) >= up_bound:
-				status = 1
-				break
-		if iteration >= itround:
-			if float(primary_num/iteration) <= 0.2:
-				status = 1
-			else:
-				status = -1
-			break
+    status = 0
+    iteration = 0
+    primary_num = 0
+    for i in f.fetch(chr, s, e):
+        iteration += 1
+        if i.flag not in [0,16]:
+            continue
+        primary_num += 1
+        if i.reference_start < s and i.reference_end > e:
+            read_count.add(i.query_name)
+            if len(read_count) >= up_bound:
+                status = 1
+                break
+        if iteration >= itround:
+            if float(primary_num/iteration) <= 0.2:
+                status = 1
+            else:
+                status = -1
+            break
 
-	return status
+    return status
 
 def overlap_cover(svs_list, reads_list):
     # [(10024, 12024), (89258, 91258), ...]
     # [[10000, 10468, 0, 'm54238_180901_011437/52298335/ccs'], [10000, 17490, 1, 'm54238_180901_011437/44762027/ccs'], ...]
     sort_list = list()
     idx = 0
     for i in reads_list:
@@ -191,197 +191,199 @@
             print(overlap - cover2_dict[idx])
         else:
             correct_num += 1
         idx += 1
     print('Correct iteration %d'%(correct_num))
 
 def generate_output(args, semi_result, contigINFO, argv, ref_g):
-	
-	'''
-	Generation of VCF format file.
-	VCF version: 4.2
-	'''
-
-	# genotype_trigger = TriggerGT[args.genotype]
-
-	svid = dict()
-	svid["INS"] = 0
-	svid["DEL"] = 0
-	svid["BND"] = 0
-	svid["DUP"] = 0
-	svid["INV"] = 0
-
-	file = open(args.output, 'w')
-	action = args.genotype
-	Generation_VCF_header(file, contigINFO, args.sample, argv)
-	file.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t%s\n"%(args.sample))
-	for i in semi_result:
-		if i[1] in ["DEL", "INS"]:
-			if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
-				continue
-			if i[1] == "INS":
-				cal_end = int(i[2])
-			else:
-				cal_end = int(i[2]) + abs(int(float(i[3])))
-			info_list = "{PRECISION};SVTYPE={SVTYPE};SVLEN={SVLEN};END={END};CIPOS={CIPOS};CILEN={CILEN};RE={RE};RNAMES={RNAMES}".format(
-				PRECISION = "IMPRECISE" if i[8] == "0/0" else "PRECISE", 
-				SVTYPE = i[1], 
-				SVLEN = i[3], 
-				END = str(cal_end), 
-				CIPOS = i[5], 
-				CILEN = i[6], 
-				RE = i[4],
-				RNAMES = i[12] if args.report_readid else "NULL")
-			if action:
-				try:
-					info_list += ";AF=" + str(round(int(i[4]) / (int(i[4]) + int(i[7])), 4))
-				except:
-					info_list += ";AF=."
-			if i[1] =="DEL":
-				info_list += ";STRAND=+-"
-			if i[11] == "." or i[11] == None:
-				filter_lable = "PASS"
-			else:
-				filter_lable = "PASS" if float(i[11]) >= 5.0 else "q5"
-			file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
-				CHR = i[0], 
-				POS = str(int(i[2])), 
-				ID = "cuteSV.%s.%d"%(i[1], svid[i[1]]),
-				REF = str(ref_g[i[0]].seq[max(int(i[2])-1, 0)]) if i[1] == 'INS' else str(ref_g[i[0]].seq[max(int(i[2])-1, 0):int(i[2])-int(i[3])]),
-				ALT = "%s"%(str(ref_g[i[0]].seq[max(int(i[2])-1, 0)])+i[13] if i[1] == 'INS' else str(ref_g[i[0]].seq[max(int(i[2])-1, 0)])), 
-				INFO = info_list, 
-				FORMAT = "GT:DR:DV:PL:GQ", 
-				GT = i[8],
-				DR = i[7],
-				RE = i[4],
-				PL = i[9],
-				GQ = i[10],
-				QUAL = i[11],
-				PASS = filter_lable))
-			svid[i[1]] += 1
-		elif i[1] == "DUP":
-			if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
-				continue
-			cal_end = int(i[2]) + 1 + abs(int(float(i[3])))
-			info_list = "{PRECISION};SVTYPE={SVTYPE};SVLEN={SVLEN};END={END};RE={RE};STRAND=-+;RNAMES={RNAMES}".format(
-				PRECISION = "IMPRECISE" if i[6] == "0/0" else "PRECISE", 
-				SVTYPE = i[1], 
-				SVLEN = i[3], 
-				END = str(cal_end), 
-				RE = i[4],
-				RNAMES = i[10] if args.report_readid else "NULL")
-			if action:
-				try:
-					info_list += ";AF=" + str(round(int(i[4]) / (int(i[4]) + int(i[5])), 4))
-				except:
-					info_list += ";AF=."
-			if i[9] == ".":
-				filter_lable = "PASS"
-			else:
-				filter_lable = "PASS" if float(i[9]) >= 5.0 else "q5"
-			file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
-				CHR = i[0], 
-				POS = str(int(i[2]) + 1), 
-				ID = "cuteSV.%s.%d"%(i[1], svid[i[1]]),
-				REF = str(ref_g[i[0]].seq[int(i[2])]),
-				ALT = "<%s>"%(i[1]), 
-				INFO = info_list, 
-				FORMAT = "GT:DR:DV:PL:GQ", 
-				GT = i[6],
-				DR = i[5],
-				RE = i[4],
-				PL = i[7],
-				GQ = i[8],
-				QUAL = i[9],
-				PASS = filter_lable))
-			svid[i[1]] += 1
-		elif i[1] == "INV":
-			if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
-				continue
-			cal_end = int(i[2]) + 1 + abs(int(float(i[3])))
-			info_list = "{PRECISION};SVTYPE={SVTYPE};SVLEN={SVLEN};END={END};RE={RE};STRAND={STRAND};RNAMES={RNAMES}".format(
-				PRECISION = "IMPRECISE" if i[6] == "0/0" else "PRECISE", 
-				SVTYPE = i[1], 
-				SVLEN = i[3], 
-				END = str(cal_end), 
-				RE = i[4],
-				STRAND = i[7],
-				RNAMES = i[11] if args.report_readid else "NULL")
-			if action:
-				try:
-					info_list += ";AF=" + str(round(int(i[4]) / (int(i[4]) + int(i[5])), 4))
-				except:
-					info_list += ";AF=."
-			if i[10] == ".":
-				filter_lable = "PASS"
-			else:
-				filter_lable = "PASS" if float(i[10]) >= 5.0 else "q5"
-			file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
-				CHR = i[0], 
-				POS = str(int(i[2]) + 1), 
-				ID = "cuteSV.%s.%d"%(i[1], svid[i[1]]),
-				REF = str(ref_g[i[0]].seq[int(i[2])]),
-				ALT = "<%s>"%(i[1]), 
-				INFO = info_list, 
-				FORMAT = "GT:DR:DV:PL:GQ", 
-				GT = i[6],
-				DR = i[5],
-				RE = i[4],
-				PL = i[8],
-				GQ = i[9],
-				QUAL = i[10],
-				PASS = filter_lable))
-			svid[i[1]] += 1
-		else:
-			# BND
-			# info_list = "{PRECISION};SVTYPE={SVTYPE};CHR2={CHR2};END={END};RE={RE};RNAMES={RNAMES}".format(
-			info_list = "{PRECISION};SVTYPE={SVTYPE};RE={RE};RNAMES={RNAMES}".format(
-				PRECISION = "IMPRECISE" if i[7] == "0/0" else "PRECISE", 
-				SVTYPE = "BND", 
-				# CHR2 = i[3], 
-				# END = str(int(i[4]) + 1), 
-				RE = i[5],
-				RNAMES = i[11] if args.report_readid else "NULL")
-			if action:
-				try:
-					info_list += ";AF=" + str(round(int(i[5]) / (int(i[5]) + int(i[6])), 4))
-				except:
-					info_list += ";AF=."
-			if i[10] == ".":
-				filter_lable = "PASS"
-			else:
-				filter_lable = "PASS" if float(i[10]) >= 5.0 else "q5"
-			file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
-				CHR = i[0], 
-				POS = str(int(i[2]) + 1), 
-				ID = "cuteSV.%s.%d"%("BND", svid["BND"]), 
-				REF = 'N',
-				ALT = i[1], 
-				INFO = info_list, 
-				FORMAT = "GT:DR:DV:PL:GQ", 
-				GT = i[7],
-				DR = i[6],
-				RE = i[5],
-				PL = i[8],
-				GQ = i[9],
-				QUAL = i[10],
-				PASS = filter_lable))
-			svid["BND"] += 1
+    
+    '''
+    Generation of VCF format file.
+    VCF version: 4.2
+    '''
+
+    # genotype_trigger = TriggerGT[args.genotype]
+
+    svid = dict()
+    svid["INS"] = 0
+    svid["DEL"] = 0
+    svid["BND"] = 0
+    svid["DUP"] = 0
+    svid["INV"] = 0
+
+    file = open(args.output, 'w')
+    action = args.genotype
+    Generation_VCF_header(file, contigINFO, args.sample, argv)
+    file.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t%s\n"%(args.sample))
+    for i in semi_result:
+        if i[1] in ["DEL", "INS"]:
+            if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
+                continue
+            if abs(int(float(i[3]))) < args.min_size:
+                continue
+            if i[1] == "INS":
+                cal_end = int(i[2])
+            else:
+                cal_end = int(i[2]) + abs(int(float(i[3])))
+            info_list = "{PRECISION};SVTYPE={SVTYPE};SVLEN={SVLEN};END={END};CIPOS={CIPOS};CILEN={CILEN};RE={RE};RNAMES={RNAMES}".format(
+                PRECISION = "IMPRECISE" if i[8] == "0/0" else "PRECISE", 
+                SVTYPE = i[1], 
+                SVLEN = i[3], 
+                END = str(cal_end), 
+                CIPOS = i[5], 
+                CILEN = i[6], 
+                RE = i[4],
+                RNAMES = i[12] if args.report_readid else "NULL")
+            if action:
+                try:
+                    info_list += ";AF=" + str(round(int(i[4]) / (int(i[4]) + int(i[7])), 4))
+                except:
+                    info_list += ";AF=."
+            if i[1] =="DEL":
+                info_list += ";STRAND=+-"
+            if i[11] == "." or i[11] == None:
+                filter_lable = "PASS"
+            else:
+                filter_lable = "PASS" if float(i[11]) >= 5.0 else "q5"
+            file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
+                CHR = i[0], 
+                POS = str(int(i[2])), 
+                ID = "cuteSV.%s.%d"%(i[1], svid[i[1]]),
+                REF = str(ref_g[i[0]].seq[max(int(i[2])-1, 0)]) if i[1] == 'INS' else str(ref_g[i[0]].seq[max(int(i[2])-1, 0):int(i[2])-int(i[3])]),
+                ALT = "%s"%(str(ref_g[i[0]].seq[max(int(i[2])-1, 0)])+i[13] if i[1] == 'INS' else str(ref_g[i[0]].seq[max(int(i[2])-1, 0)])), 
+                INFO = info_list, 
+                FORMAT = "GT:DR:DV:PL:GQ", 
+                GT = i[8],
+                DR = i[7],
+                RE = i[4],
+                PL = i[9],
+                GQ = i[10],
+                QUAL = i[11],
+                PASS = filter_lable))
+            svid[i[1]] += 1
+        elif i[1] == "DUP":
+            if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
+                continue
+            cal_end = int(i[2]) + 1 + abs(int(float(i[3])))
+            info_list = "{PRECISION};SVTYPE={SVTYPE};SVLEN={SVLEN};END={END};RE={RE};STRAND=-+;RNAMES={RNAMES}".format(
+                PRECISION = "IMPRECISE" if i[6] == "0/0" else "PRECISE", 
+                SVTYPE = i[1], 
+                SVLEN = i[3], 
+                END = str(cal_end), 
+                RE = i[4],
+                RNAMES = i[10] if args.report_readid else "NULL")
+            if action:
+                try:
+                    info_list += ";AF=" + str(round(int(i[4]) / (int(i[4]) + int(i[5])), 4))
+                except:
+                    info_list += ";AF=."
+            if i[9] == ".":
+                filter_lable = "PASS"
+            else:
+                filter_lable = "PASS" if float(i[9]) >= 5.0 else "q5"
+            file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
+                CHR = i[0], 
+                POS = str(int(i[2]) + 1), 
+                ID = "cuteSV.%s.%d"%(i[1], svid[i[1]]),
+                REF = str(ref_g[i[0]].seq[int(i[2])]),
+                ALT = "<%s>"%(i[1]), 
+                INFO = info_list, 
+                FORMAT = "GT:DR:DV:PL:GQ", 
+                GT = i[6],
+                DR = i[5],
+                RE = i[4],
+                PL = i[7],
+                GQ = i[8],
+                QUAL = i[9],
+                PASS = filter_lable))
+            svid[i[1]] += 1
+        elif i[1] == "INV":
+            if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
+                continue
+            cal_end = int(i[2]) + 1 + abs(int(float(i[3])))
+            info_list = "{PRECISION};SVTYPE={SVTYPE};SVLEN={SVLEN};END={END};RE={RE};STRAND={STRAND};RNAMES={RNAMES}".format(
+                PRECISION = "IMPRECISE" if i[6] == "0/0" else "PRECISE", 
+                SVTYPE = i[1], 
+                SVLEN = i[3], 
+                END = str(cal_end), 
+                RE = i[4],
+                STRAND = i[7],
+                RNAMES = i[11] if args.report_readid else "NULL")
+            if action:
+                try:
+                    info_list += ";AF=" + str(round(int(i[4]) / (int(i[4]) + int(i[5])), 4))
+                except:
+                    info_list += ";AF=."
+            if i[10] == ".":
+                filter_lable = "PASS"
+            else:
+                filter_lable = "PASS" if float(i[10]) >= 5.0 else "q5"
+            file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
+                CHR = i[0], 
+                POS = str(int(i[2]) + 1), 
+                ID = "cuteSV.%s.%d"%(i[1], svid[i[1]]),
+                REF = str(ref_g[i[0]].seq[int(i[2])]),
+                ALT = "<%s>"%(i[1]), 
+                INFO = info_list, 
+                FORMAT = "GT:DR:DV:PL:GQ", 
+                GT = i[6],
+                DR = i[5],
+                RE = i[4],
+                PL = i[8],
+                GQ = i[9],
+                QUAL = i[10],
+                PASS = filter_lable))
+            svid[i[1]] += 1
+        else:
+            # BND
+            # info_list = "{PRECISION};SVTYPE={SVTYPE};CHR2={CHR2};END={END};RE={RE};RNAMES={RNAMES}".format(
+            info_list = "{PRECISION};SVTYPE={SVTYPE};RE={RE};RNAMES={RNAMES}".format(
+                PRECISION = "IMPRECISE" if i[7] == "0/0" else "PRECISE", 
+                SVTYPE = "BND", 
+                # CHR2 = i[3], 
+                # END = str(int(i[4]) + 1), 
+                RE = i[5],
+                RNAMES = i[11] if args.report_readid else "NULL")
+            if action:
+                try:
+                    info_list += ";AF=" + str(round(int(i[5]) / (int(i[5]) + int(i[6])), 4))
+                except:
+                    info_list += ";AF=."
+            if i[10] == ".":
+                filter_lable = "PASS"
+            else:
+                filter_lable = "PASS" if float(i[10]) >= 5.0 else "q5"
+            file.write("{CHR}\t{POS}\t{ID}\t{REF}\t{ALT}\t{QUAL}\t{PASS}\t{INFO}\t{FORMAT}\t{GT}:{DR}:{RE}:{PL}:{GQ}\n".format(
+                CHR = i[0], 
+                POS = str(int(i[2]) + 1), 
+                ID = "cuteSV.%s.%d"%("BND", svid["BND"]), 
+                REF = 'N',
+                ALT = i[1], 
+                INFO = info_list, 
+                FORMAT = "GT:DR:DV:PL:GQ", 
+                GT = i[7],
+                DR = i[6],
+                RE = i[5],
+                PL = i[8],
+                GQ = i[9],
+                QUAL = i[10],
+                PASS = filter_lable))
+            svid["BND"] += 1
 
 
 def generate_pvcf(args, result, contigINFO, argv, ref_g):
     file = open(args.output, 'w')
     Generation_VCF_header(file, contigINFO, args.sample, argv)
     file.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t%s\n"%(args.sample))
     # [chrom(0), sv_start, genotype(2), sv_type, sv_end(4), CIPOS, CILEN(6), [gt_re, DR, GT(new), GL, GQ, QUAL], rname(8), svid, ref(10), alts, sv_strand(12), seq]
     for i in result:
         if i == []:
             continue
-        if i[7][5] == '.,.':
-            print(i)
+        # if i[7][5] == '.,.':
+        #     print(i)
         if i[7][5] == "." or i[7][5] == None:
             filter_lable = "PASS"
         else:
             filter_lable = "PASS" if float(i[7][5]) >= 2.5 else "q5"
         if i[3] == 'INS':
             if abs(i[4]) > args.max_size and args.max_size != -1:
                 continue
@@ -554,41 +556,64 @@
                 GT = i[2],
                 DR = i[7][1],
                 RE = i[7][0],
                 PL = i[7][3],
                 GQ = i[7][4]
                 ))
 
-			
+            
 def load_valuable_chr(path):
-	valuable_chr = dict()
-	valuable_chr["DEL"] = list()
-	valuable_chr["DUP"] = list()
-	valuable_chr["INS"] = list()
-	valuable_chr["INV"] = list()
-	valuable_chr["TRA"] = dict()
-
-	for svtype in ["DEL", "DUP", "INS", "INV"]:
-		file = open("%s%s.sigs"%(path, svtype), 'r')
-		for line in file:
-			chr = line.strip('\n').split('\t')[1]
-			if chr not in valuable_chr[svtype]:
-				valuable_chr[svtype].append(chr)
-		file.close()
-		valuable_chr[svtype].sort()
-
-	file = open("%s%s.sigs"%(path, "TRA"), 'r')
-	for line in file:
-		chr1 = line.strip('\n').split('\t')[1]
-		chr2 = line.strip('\n').split('\t')[4]
-		
-		if chr1 not in valuable_chr["TRA"]:
-			valuable_chr["TRA"][chr1] = list()
-		if chr2 not in valuable_chr["TRA"][chr1]:
-			valuable_chr["TRA"][chr1].append(chr2)
-
-	file.close()
-	for chr1 in valuable_chr["TRA"]:
-		valuable_chr["TRA"][chr1].sort()
-
-	return valuable_chr
-
+    valuable_chr = dict()
+    valuable_chr["DEL"] = list()
+    valuable_chr["DUP"] = list()
+    valuable_chr["INS"] = list()
+    valuable_chr["INV"] = list()
+    valuable_chr["TRA"] = dict()
+
+    for svtype in ["DEL", "DUP", "INS", "INV"]:
+        file = open("%s%s.sigs"%(path, svtype), 'r')
+        for line in file:
+            chr = line.strip('\n').split('\t')[1]
+            if chr not in valuable_chr[svtype]:
+                valuable_chr[svtype].append(chr)
+        file.close()
+        valuable_chr[svtype].sort()
+
+    file = open("%s%s.sigs"%(path, "TRA"), 'r')
+    for line in file:
+        chr1 = line.strip('\n').split('\t')[1]
+        chr2 = line.strip('\n').split('\t')[4]
+        
+        if chr1 not in valuable_chr["TRA"]:
+            valuable_chr["TRA"][chr1] = list()
+        if chr2 not in valuable_chr["TRA"][chr1]:
+            valuable_chr["TRA"][chr1].append(chr2)
+
+    file.close()
+    for chr1 in valuable_chr["TRA"]:
+        valuable_chr["TRA"][chr1].sort()
+
+    return valuable_chr
+
+def load_bed(bed_file, Task_list):
+    # Task_list: [[chr, start, end], ...]
+    bed_regions = dict()
+    if bed_file != None:
+        # only consider regions in BED file
+        with open(bed_file, 'r') as f:
+            for line in f:
+                seq = line.strip().split('\t')
+                if seq[0] not in bed_regions:
+                    bed_regions[seq[0]] = list()
+                bed_regions[seq[0]].append((int(seq[1]) - 1000, int(seq[2]) + 1000))
+        region_list = [[] for i in range(len(Task_list))]
+        for chrom in bed_regions:
+            bed_regions[chrom].sort(key = lambda x:(x[0], x[1]))
+            for item in bed_regions[chrom]:
+                for i in range(len(Task_list)):
+                    if chrom == Task_list[i][0]:
+                        if (Task_list[i][1] <= item[0] and Task_list[i][2] > item[0]) or item[0] <= Task_list[i][1] < item[1]:
+                            region_list[i].append(item)
+        assert len(region_list) == len(Task_list), "parse bed file error"
+        return region_list
+    else:
+        return None
```

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_resolveDUP.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_resolveDUP.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         if seq[1] != chr:
             continue
 
         pos_1 = int(seq[2])
         pos_2 = int(seq[3])
         read_id = seq[4]
         
-        if pos_1 - semi_dup_cluster[-1][0] > max_cluster_bias or pos_2 - semi_dup_cluster[-1][1] > max_cluster_bias:
+        # if pos_1 - semi_dup_cluster[-1][0] > max_cluster_bias or pos_2 - semi_dup_cluster[-1][1] > max_cluster_bias:
+        if pos_1 - semi_dup_cluster[-1][0] > max_cluster_bias:
             if len(semi_dup_cluster) >= read_count:
                 if semi_dup_cluster[-1][0] == semi_dup_cluster[-1][1] == 0:
                     pass
                 else:
                     generate_dup_cluster(semi_dup_cluster, 
                                         chr, 
                                         read_count, 
@@ -77,47 +78,60 @@
 def generate_dup_cluster(semi_dup_cluster, chr, read_count, max_cluster_bias, 
     sv_size, candidate_single_SV, action, MaxSize, gt_round):
     # calculate support reads
     support_read = list(set([i[2] for i in semi_dup_cluster]))
     if len(support_read) < read_count:
         return
 
-    low_b = int(len(semi_dup_cluster)*0.4)
-    up_b = int(len(semi_dup_cluster)*0.6)
+    semi_dup_cluster.sort(key = lambda x:x[1])
+    allele_collect = []
+    allele_collect.append([semi_dup_cluster[0]])
+    last_len = semi_dup_cluster[0][1]
+    for i in semi_dup_cluster[1:]:
+        if i[1] - last_len > max_cluster_bias:
+            allele_collect.append([])
+        allele_collect[-1].append(i)
+        last_len = i[1]
+    for i in allele_collect:
+        support_read = list(set([j[2] for j in i]))
+        if len(support_read) < read_count:
+            continue
+        low_b = int(len(i)*0.4)
+        up_b = int(len(i)*0.6)
 
-    if low_b == up_b:
-        breakpoint_1 = semi_dup_cluster[low_b][0]
-        breakpoint_2 = semi_dup_cluster[low_b][1]
-    else:
-        breakpoint_1 = [i[0] for i in semi_dup_cluster[low_b:up_b]]
-        breakpoint_2 = [i[1] for i in semi_dup_cluster[low_b:up_b]]
-        breakpoint_1 = int(sum(breakpoint_1)/len(semi_dup_cluster[low_b:up_b]))
-        breakpoint_2 = int(sum(breakpoint_2)/len(semi_dup_cluster[low_b:up_b]))
+        if low_b == up_b:
+            breakpoint_1 = i[low_b][0]
+            breakpoint_2 = i[low_b][1]
+        else:
+            breakpoint_1 = [i[0] for i in i[low_b:up_b]]
+            breakpoint_2 = [i[1] for i in i[low_b:up_b]]
+            breakpoint_1 = int(sum(breakpoint_1)/len(i[low_b:up_b]))
+            breakpoint_2 = int(sum(breakpoint_2)/len(i[low_b:up_b]))
 
 
-    if sv_size <= breakpoint_2 - breakpoint_1 <= MaxSize or (sv_size <= breakpoint_2 - breakpoint_1 and MaxSize == -1):
-        if action:
-            candidate_single_SV.append([chr,
-                                        'DUP', 
-                                        breakpoint_1, 
-                                        breakpoint_2,
-                                        support_read])
-            # print("DUP", chr, int(breakpoint_1), int(breakpoint_2), DR, DV, QUAL, "%.4f"%cost_time)
-        else:
-            candidate_single_SV.append([chr,
-                                        'DUP', 
-                                        str(breakpoint_1), 
-                                        str(breakpoint_2 - breakpoint_1), 
-                                        str(len(support_read)),
-                                        '.',
-                                        './.',
-                                        '.,.,.',
-                                        '.',
-                                        '.',
-                                        str(','.join(support_read))])
+        if sv_size <= breakpoint_2 - breakpoint_1 <= MaxSize or (sv_size <= breakpoint_2 - breakpoint_1 and MaxSize == -1):
+            if action:
+                candidate_single_SV.append([chr,
+                                            'DUP', 
+                                            breakpoint_1, 
+                                            breakpoint_2,
+                                            support_read])
+                # print("DUP", chr, int(breakpoint_1), int(breakpoint_2), DR, DV, QUAL, "%.4f"%cost_time)
+            else:
+                candidate_single_SV.append([chr,
+                                            'DUP', 
+                                            str(breakpoint_1), 
+                                            str(breakpoint_2 - breakpoint_1), 
+                                            str(len(support_read)),
+                                            '.',
+                                            './.',
+                                            '.,.,.',
+                                            '.',
+                                            '.',
+                                            str(','.join(support_read))])
 
 
 def run_dup(args):
     return resolution_DUP(*args)
 
 def call_gt(temporary_dir, chr, candidate_single_SV, max_cluster_bias):
     reads_list = list() # [(10000, 10468, 0, 'm54238_180901_011437/52298335/ccs'), ...]
```

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_resolveINDEL.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_resolveINDEL.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_resolveINV.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_resolveINV.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV/cuteSV_resolveTRA.py` & `cuteSV-2.0.3/src/cuteSV/cuteSV_resolveTRA.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV/diploid_calling.py` & `cuteSV-2.0.3/src/cuteSV/diploid_calling.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.0.2/src/cuteSV.egg-info/PKG-INFO` & `cuteSV-2.0.3/src/cuteSV.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuteSV
-Version: 2.0.2
+Version: 2.0.3
 Summary: Long-read-based human genomic structural variation detection with cuteSV
 Home-page: https://github.com/tjiangHIT/cuteSV
 Author: Jiang Tao
 Author-email: tjiang@hit.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -51,14 +51,16 @@
 
 BTW, we used [Truvari](https://github.com/spiralgenetics/truvari) to calculate the recall, precision, and f-measure.
 For more detailed implementation of SV benchmarks, we show an example [here](https://github.com/tjiangHIT/sv-benchmark).
 
 ## Notice
 A new wiki page about diploid-assembly-based SV detection using cuteSV has been established. More details please see [here](https://github.com/tjiangHIT/cuteSV/wiki/Diploid-assembly-based-SV-detection-using-cuteSV).
 
+We provided a new document for applying **force calling** (or **regenotyping**) benchmark [here](https://github.com/tjiangHIT/cuteSV/tree/master/src/documentation).
+
 ---
 ### Dependence
 	
 	1. python3
 	2. pysam
 	3. Biopython
 	4. cigar
@@ -84,14 +86,16 @@
 		--diff_ratio_merging_DEL	0.5
 
 	> For ONT data:
 		--max_cluster_bias_INS		100
 		--diff_ratio_merging_INS	0.3
 		--max_cluster_bias_DEL	100
 		--diff_ratio_merging_DEL	0.3
+	> For force calling:
+		--min_mapq 			10
 	
 | Parameter | Description | Default |
 | :------------ |:---------------|-------------:|
 |--threads|Number of threads to use.| 16 |
 |--batches| Batch of genome segmentation interval.|10,000,000|
 |--sample| Sample name/id |NULL|
 |--retain_work_dir|Enable to retain temporary folder and files.|False|
@@ -112,14 +116,15 @@
 |--max_cluster_bias_DEL|Maximum distance to cluster read together for deletion.|200|
 |--diff_ratio_merging_DEL|Do not merge breakpoints with basepair identity more than the ratio of *default* for deletion.|0.5|
 |--max_cluster_bias_INV|Maximum distance to cluster read together for inversion.|500|
 |--max_cluster_bias_DUP|Maximum distance to cluster read together for duplication.|500|
 |--max_cluster_bias_TRA|Maximum distance to cluster read together for translocation.|50|
 |--diff_ratio_filtering_TRA|Filter breakpoints with basepair identity less than the ratio of *default* for translocation.|0.6|
 |--remain_reads_ratio|The ratio of reads remained in cluster to generate the breakpoint. Set lower to get more precise breakpoint when the alignment data have high quality but recommand over 0.5.|1|
+|-include_bed|Optional given bed file. Only detect SVs in regions in the BED file.|NULL|
 
 ---
 ### Datasets generated from cuteSV
 We provided the SV callsets of the HG002 human sample produced by cuteSV form three different long-read sequencing platforms (i.e. PacBio CLR, PacBio CCS, and ONT PromethION). 
 
 You can download them at: 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783083.svg)](https://doi.org/10.5281/zenodo.3783083)
```

### Comparing `cuteSV-2.0.2/src/cuteSV.egg-info/SOURCES.txt` & `cuteSV-2.0.3/src/cuteSV.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 LICENSE
 README.md
 setup.py
 src/benchmarks/__init__.py
 src/benchmarks/cmp_NA19240.py
+src/benchmarks/eval_BND.py
+src/benchmarks/eval_generegion.py
+src/benchmarks/eval_population.py
 src/benchmarks/eval_sim.py
 src/benchmarks/eval_trio.py
 src/benchmarks/multi_platform.py
 src/benchmarks/sta_venn.py
 src/benchmarks/vcf2bedpe.py
 src/cuteSV/CommandRunner.py
 src/cuteSV/__init__.py
```

