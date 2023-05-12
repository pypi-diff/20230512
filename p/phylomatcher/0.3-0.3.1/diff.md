# Comparing `tmp/phylomatcher-0.3.tar.gz` & `tmp/phylomatcher-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylomatcher-0.3.tar", last modified: Fri May 12 17:56:30 2023, max compression
+gzip compressed data, was "phylomatcher-0.3.1.tar", last modified: Fri May 12 18:00:42 2023, max compression
```

## Comparing `phylomatcher-0.3.tar` & `phylomatcher-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-12 17:56:30.349999 phylomatcher-0.3/
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     1073 2023-05-08 14:56:28.000000 phylomatcher-0.3/LICENSE
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     3709 2023-05-12 17:56:30.349999 phylomatcher-0.3/PKG-INFO
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     3109 2023-05-08 14:56:28.000000 phylomatcher-0.3/README.md
-drwxr-xr-x   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-12 17:56:30.349999 phylomatcher-0.3/phylomatcher/
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-08 14:56:28.000000 phylomatcher-0.3/phylomatcher/__init__.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-08 14:56:28.000000 phylomatcher-0.3/phylomatcher/__main__.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     5040 2023-05-11 15:30:51.000000 phylomatcher-0.3/phylomatcher/entrez_matcher.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     2202 2023-05-12 17:54:13.000000 phylomatcher-0.3/phylomatcher/gbif_matcher.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)    17483 2023-05-12 17:54:13.000000 phylomatcher-0.3/phylomatcher/gui.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)    25134 2023-05-12 17:54:13.000000 phylomatcher-0.3/phylomatcher/merged_gui.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     2359 2023-05-11 15:37:51.000000 phylomatcher-0.3/phylomatcher/taxomatcher.py
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     1458 2023-05-11 15:43:23.000000 phylomatcher-0.3/phylomatcher/trait_matcher.py
-drwxr-xr-x   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-12 17:56:30.349999 phylomatcher-0.3/phylomatcher.egg-info/
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     3709 2023-05-12 17:56:30.000000 phylomatcher-0.3/phylomatcher.egg-info/PKG-INFO
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)      469 2023-05-12 17:56:30.000000 phylomatcher-0.3/phylomatcher.egg-info/SOURCES.txt
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)        1 2023-05-12 17:56:30.000000 phylomatcher-0.3/phylomatcher.egg-info/dependency_links.txt
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)       64 2023-05-12 17:56:30.000000 phylomatcher-0.3/phylomatcher.egg-info/entry_points.txt
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)       29 2023-05-12 17:56:30.000000 phylomatcher-0.3/phylomatcher.egg-info/requires.txt
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)       13 2023-05-12 17:56:30.000000 phylomatcher-0.3/phylomatcher.egg-info/top_level.txt
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)      768 2023-05-12 17:56:30.349999 phylomatcher-0.3/setup.cfg
--rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)      225 2023-05-08 14:56:28.000000 phylomatcher-0.3/setup.py
+drwxr-xr-x   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-12 18:00:42.029999 phylomatcher-0.3.1/
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     1073 2023-05-08 14:56:28.000000 phylomatcher-0.3.1/LICENSE
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     3721 2023-05-12 18:00:42.029999 phylomatcher-0.3.1/PKG-INFO
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     3119 2023-05-12 17:59:30.000000 phylomatcher-0.3.1/README.md
+drwxr-xr-x   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-12 18:00:42.029999 phylomatcher-0.3.1/phylomatcher/
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-08 14:56:28.000000 phylomatcher-0.3.1/phylomatcher/__init__.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-08 14:56:28.000000 phylomatcher-0.3.1/phylomatcher/__main__.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     5040 2023-05-11 15:30:51.000000 phylomatcher-0.3.1/phylomatcher/entrez_matcher.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     2202 2023-05-12 17:54:13.000000 phylomatcher-0.3.1/phylomatcher/gbif_matcher.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)    17483 2023-05-12 17:54:13.000000 phylomatcher-0.3.1/phylomatcher/gui.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)    25134 2023-05-12 17:54:13.000000 phylomatcher-0.3.1/phylomatcher/merged_gui.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     2360 2023-05-12 17:59:01.000000 phylomatcher-0.3.1/phylomatcher/phylomatcher.py
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     1458 2023-05-11 15:43:23.000000 phylomatcher-0.3.1/phylomatcher/trait_matcher.py
+drwxr-xr-x   0 lswhiteh  (1000) lswhiteh  (1000)        0 2023-05-12 18:00:42.029999 phylomatcher-0.3.1/phylomatcher.egg-info/
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)     3721 2023-05-12 18:00:42.000000 phylomatcher-0.3.1/phylomatcher.egg-info/PKG-INFO
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)      470 2023-05-12 18:00:42.000000 phylomatcher-0.3.1/phylomatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)        1 2023-05-12 18:00:42.000000 phylomatcher-0.3.1/phylomatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)       64 2023-05-12 18:00:42.000000 phylomatcher-0.3.1/phylomatcher.egg-info/entry_points.txt
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)       29 2023-05-12 18:00:42.000000 phylomatcher-0.3.1/phylomatcher.egg-info/requires.txt
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)       13 2023-05-12 18:00:42.000000 phylomatcher-0.3.1/phylomatcher.egg-info/top_level.txt
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)      770 2023-05-12 18:00:42.029999 phylomatcher-0.3.1/setup.cfg
+-rw-r--r--   0 lswhiteh  (1000) lswhiteh  (1000)      225 2023-05-08 14:56:28.000000 phylomatcher-0.3.1/setup.py
```

### Comparing `phylomatcher-0.3/LICENSE` & `phylomatcher-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phylomatcher-0.3/PKG-INFO` & `phylomatcher-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: phylomatcher
-Version: 0.3
+Version: 0.3.1
 Summary: A tool for parsing and extracting taxon synonyms.
 Home-page: https://github.com/Lswhiteh/phylomatcher
 Author: Logan Whitehouse
 Author-email: lswhiteh@unc.edu
 License: MIT
 Project-URL: Issues, https://github.com/Lswhiteh/phylomatcher/issues
 Project-URL: GitHub, https://github.com/Lswhiteh/phylomatcher
 Keywords: population genetics,phylogenetics,taxonomy
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Taxomatcher
+# PhyloMatcher
 
 Python modules to query the GFIB or NCBI Taxonomy databases for synonym names of target species.
 
 ## Installation
 
 Required packages:
 
@@ -29,15 +29,15 @@
 - tqdm
 
 Easiest installation using a conda environment and pip:
 
 ```{bash}
 conda create -n tm-env -c conda-forge python
 conda activate tm-env
-pip install taxomatcher
+pip install PhyloMatcher
 ```
 
 ---
 
 ## Modes
 
 ### GBIF
@@ -49,16 +49,16 @@
 Sphenodon_punctatus
 Gonyosoma_prasinus
 ```
 
 Usage:
 
 ```{bash}
-$ taxomatcher gbif -h
-usage: taxomatcher gbif [-h] -i INPUT_CSV -o OUTFILE [-t THREADS]
+$ PhyloMatcher gbif -h
+usage: PhyloMatcher gbif [-h] -i INPUT_CSV -o OUTFILE [-t THREADS]
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_CSV, --csv INPUT_CSV
                         CSV where first column is a list of target species names to look up.
   -o OUTFILE, --outfile OUTFILE
                         Path to output.
@@ -77,35 +77,35 @@
 Sphenodon_punctatus,Hatteria_punctata
 Gonyosoma_prasinus,Coluber_prasinus,Elaphe_prasina,Rhadinophis_prasinus,Rhadinophis_prasina
 ```
 
 Usage:
 
 ```{bash}
-$ taxomatcher ncbi -h
-usage: taxomatcher ncbi [-h] -i INPUT_CSV -o OUTFILE -e EMAIL
+$ PhyloMatcher ncbi -h
+usage: PhyloMatcher ncbi [-h] -i INPUT_CSV -o OUTFILE -e EMAIL
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_CSV, --csv INPUT_CSV
                         CSV where first column is a list of target species names to look up.
   -o OUTFILE, --outfile OUTFILE
                         Path to output.
   -e EMAIL, --email EMAIL
 ```
 
-### Matching trait files to taxomatcher output
+### Matching trait files to PhyloMatcher output
 
-Once you have found synonyms from tree output you can match that to any phenotypic/trait data you have. Similar to the other inputs the first column must contain the species names you're targeting, and they should be formatted identically to how the taxomatcher output looks (case-sensitive and separated by underscores.)
+Once you have found synonyms from tree output you can match that to any phenotypic/trait data you have. Similar to the other inputs the first column must contain the species names you're targeting, and they should be formatted identically to how the PhyloMatcher output looks (case-sensitive and separated by underscores.)
 
 Usage:
 
 ```{bash}
-$ taxomatcher trait -h
-usage: taxomatcher trait [-h] -t TRAITFILE -s SPECIESFILE -o OUTFILE
+$ PhyloMatcher trait -h
+usage: PhyloMatcher trait [-h] -t TRAITFILE -s SPECIESFILE -o OUTFILE
 
 options:
   -h, --help            show this help message and exit
   -t TRAITFILE, --traitfile TRAITFILE
                         CSV of trait values, first column must be species names.
   -s SPECIESFILE, --speciesfile SPECIESFILE
                         CSV of species synonyms output by the gbif or ncbi modules.
```

### Comparing `phylomatcher-0.3/README.md` & `phylomatcher-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Taxomatcher
+# PhyloMatcher
 
 Python modules to query the GFIB or NCBI Taxonomy databases for synonym names of target species.
 
 ## Installation
 
 Required packages:
 
@@ -12,15 +12,15 @@
 - tqdm
 
 Easiest installation using a conda environment and pip:
 
 ```{bash}
 conda create -n tm-env -c conda-forge python
 conda activate tm-env
-pip install taxomatcher
+pip install PhyloMatcher
 ```
 
 ---
 
 ## Modes
 
 ### GBIF
@@ -32,16 +32,16 @@
 Sphenodon_punctatus
 Gonyosoma_prasinus
 ```
 
 Usage:
 
 ```{bash}
-$ taxomatcher gbif -h
-usage: taxomatcher gbif [-h] -i INPUT_CSV -o OUTFILE [-t THREADS]
+$ PhyloMatcher gbif -h
+usage: PhyloMatcher gbif [-h] -i INPUT_CSV -o OUTFILE [-t THREADS]
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_CSV, --csv INPUT_CSV
                         CSV where first column is a list of target species names to look up.
   -o OUTFILE, --outfile OUTFILE
                         Path to output.
@@ -60,35 +60,35 @@
 Sphenodon_punctatus,Hatteria_punctata
 Gonyosoma_prasinus,Coluber_prasinus,Elaphe_prasina,Rhadinophis_prasinus,Rhadinophis_prasina
 ```
 
 Usage:
 
 ```{bash}
-$ taxomatcher ncbi -h
-usage: taxomatcher ncbi [-h] -i INPUT_CSV -o OUTFILE -e EMAIL
+$ PhyloMatcher ncbi -h
+usage: PhyloMatcher ncbi [-h] -i INPUT_CSV -o OUTFILE -e EMAIL
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_CSV, --csv INPUT_CSV
                         CSV where first column is a list of target species names to look up.
   -o OUTFILE, --outfile OUTFILE
                         Path to output.
   -e EMAIL, --email EMAIL
 ```
 
-### Matching trait files to taxomatcher output
+### Matching trait files to PhyloMatcher output
 
-Once you have found synonyms from tree output you can match that to any phenotypic/trait data you have. Similar to the other inputs the first column must contain the species names you're targeting, and they should be formatted identically to how the taxomatcher output looks (case-sensitive and separated by underscores.)
+Once you have found synonyms from tree output you can match that to any phenotypic/trait data you have. Similar to the other inputs the first column must contain the species names you're targeting, and they should be formatted identically to how the PhyloMatcher output looks (case-sensitive and separated by underscores.)
 
 Usage:
 
 ```{bash}
-$ taxomatcher trait -h
-usage: taxomatcher trait [-h] -t TRAITFILE -s SPECIESFILE -o OUTFILE
+$ PhyloMatcher trait -h
+usage: PhyloMatcher trait [-h] -t TRAITFILE -s SPECIESFILE -o OUTFILE
 
 options:
   -h, --help            show this help message and exit
   -t TRAITFILE, --traitfile TRAITFILE
                         CSV of trait values, first column must be species names.
   -s SPECIESFILE, --speciesfile SPECIESFILE
                         CSV of species synonyms output by the gbif or ncbi modules.
```

### Comparing `phylomatcher-0.3/phylomatcher/entrez_matcher.py` & `phylomatcher-0.3.1/phylomatcher/entrez_matcher.py`

 * *Files identical despite different names*

### Comparing `phylomatcher-0.3/phylomatcher/gbif_matcher.py` & `phylomatcher-0.3.1/phylomatcher/gbif_matcher.py`

 * *Files identical despite different names*

### Comparing `phylomatcher-0.3/phylomatcher/gui.py` & `phylomatcher-0.3.1/phylomatcher/gui.py`

 * *Files identical despite different names*

### Comparing `phylomatcher-0.3/phylomatcher/merged_gui.py` & `phylomatcher-0.3.1/phylomatcher/merged_gui.py`

 * *Files identical despite different names*

### Comparing `phylomatcher-0.3/phylomatcher/taxomatcher.py` & `phylomatcher-0.3.1/phylomatcher/phylomatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 
 
 def main():
-    ap = argparse.ArgumentParser(description="Taxomatcher")
+    ap = argparse.ArgumentParser(description="PhyloMatcher")
     subparsers = ap.add_subparsers(title="mode", dest="mode")
     gbif_parser = subparsers.add_parser("gbif")
     gbif_parser.add_argument(
         "-i",
         "--csv",
         dest="input_csv",
         required=True,
```

### Comparing `phylomatcher-0.3/phylomatcher/trait_matcher.py` & `phylomatcher-0.3.1/phylomatcher/trait_matcher.py`

 * *Files identical despite different names*

### Comparing `phylomatcher-0.3/phylomatcher.egg-info/PKG-INFO` & `phylomatcher-0.3.1/phylomatcher.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: phylomatcher
-Version: 0.3
+Version: 0.3.1
 Summary: A tool for parsing and extracting taxon synonyms.
 Home-page: https://github.com/Lswhiteh/phylomatcher
 Author: Logan Whitehouse
 Author-email: lswhiteh@unc.edu
 License: MIT
 Project-URL: Issues, https://github.com/Lswhiteh/phylomatcher/issues
 Project-URL: GitHub, https://github.com/Lswhiteh/phylomatcher
 Keywords: population genetics,phylogenetics,taxonomy
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Taxomatcher
+# PhyloMatcher
 
 Python modules to query the GFIB or NCBI Taxonomy databases for synonym names of target species.
 
 ## Installation
 
 Required packages:
 
@@ -29,15 +29,15 @@
 - tqdm
 
 Easiest installation using a conda environment and pip:
 
 ```{bash}
 conda create -n tm-env -c conda-forge python
 conda activate tm-env
-pip install taxomatcher
+pip install PhyloMatcher
 ```
 
 ---
 
 ## Modes
 
 ### GBIF
@@ -49,16 +49,16 @@
 Sphenodon_punctatus
 Gonyosoma_prasinus
 ```
 
 Usage:
 
 ```{bash}
-$ taxomatcher gbif -h
-usage: taxomatcher gbif [-h] -i INPUT_CSV -o OUTFILE [-t THREADS]
+$ PhyloMatcher gbif -h
+usage: PhyloMatcher gbif [-h] -i INPUT_CSV -o OUTFILE [-t THREADS]
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_CSV, --csv INPUT_CSV
                         CSV where first column is a list of target species names to look up.
   -o OUTFILE, --outfile OUTFILE
                         Path to output.
@@ -77,35 +77,35 @@
 Sphenodon_punctatus,Hatteria_punctata
 Gonyosoma_prasinus,Coluber_prasinus,Elaphe_prasina,Rhadinophis_prasinus,Rhadinophis_prasina
 ```
 
 Usage:
 
 ```{bash}
-$ taxomatcher ncbi -h
-usage: taxomatcher ncbi [-h] -i INPUT_CSV -o OUTFILE -e EMAIL
+$ PhyloMatcher ncbi -h
+usage: PhyloMatcher ncbi [-h] -i INPUT_CSV -o OUTFILE -e EMAIL
 
 options:
   -h, --help            show this help message and exit
   -i INPUT_CSV, --csv INPUT_CSV
                         CSV where first column is a list of target species names to look up.
   -o OUTFILE, --outfile OUTFILE
                         Path to output.
   -e EMAIL, --email EMAIL
 ```
 
-### Matching trait files to taxomatcher output
+### Matching trait files to PhyloMatcher output
 
-Once you have found synonyms from tree output you can match that to any phenotypic/trait data you have. Similar to the other inputs the first column must contain the species names you're targeting, and they should be formatted identically to how the taxomatcher output looks (case-sensitive and separated by underscores.)
+Once you have found synonyms from tree output you can match that to any phenotypic/trait data you have. Similar to the other inputs the first column must contain the species names you're targeting, and they should be formatted identically to how the PhyloMatcher output looks (case-sensitive and separated by underscores.)
 
 Usage:
 
 ```{bash}
-$ taxomatcher trait -h
-usage: taxomatcher trait [-h] -t TRAITFILE -s SPECIESFILE -o OUTFILE
+$ PhyloMatcher trait -h
+usage: PhyloMatcher trait [-h] -t TRAITFILE -s SPECIESFILE -o OUTFILE
 
 options:
   -h, --help            show this help message and exit
   -t TRAITFILE, --traitfile TRAITFILE
                         CSV of trait values, first column must be species names.
   -s SPECIESFILE, --speciesfile SPECIESFILE
                         CSV of species synonyms output by the gbif or ncbi modules.
```

### Comparing `phylomatcher-0.3/setup.cfg` & `phylomatcher-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phylomatcher
-version = 0.3
+version = 0.3.1
 author = Logan Whitehouse
 author_email = lswhiteh@unc.edu
 description = A tool for parsing and extracting taxon synonyms.
 url = https://github.com/Lswhiteh/phylomatcher
 project_urls = 
 	Issues = https://github.com/Lswhiteh/phylomatcher/issues
 	GitHub = https://github.com/Lswhiteh/phylomatcher
```

