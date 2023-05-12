# Comparing `tmp/proteinTools-1.5.2.tar.gz` & `tmp/proteinTools-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.5.2.tar", last modified: Wed May 10 05:32:10 2023, max compression
+gzip compressed data, was "proteinTools-1.5.3.tar", last modified: Fri May 12 21:10:13 2023, max compression
```

## Comparing `proteinTools-1.5.2.tar` & `proteinTools-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:32:10.105996 proteinTools-1.5.2/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.5.2/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:32:10.103589 proteinTools-1.5.2/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.5.2/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:32:10.001361 proteinTools-1.5.2/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    53429 2023-05-10 05:31:56.000000 proteinTools-1.5.2/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.5.2/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:32:10.082657 proteinTools-1.5.2/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-10 05:32:10.111572 proteinTools-1.5.2/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-05-10 05:31:29.000000 proteinTools-1.5.2/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-12 21:10:13.122485 proteinTools-1.5.3/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.5.3/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      491 2023-05-12 21:10:13.118540 proteinTools-1.5.3/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.5.3/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-12 21:10:12.960438 proteinTools-1.5.3/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    53429 2023-05-12 21:08:35.000000 proteinTools-1.5.3/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.5.3/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-12 21:10:13.082201 proteinTools-1.5.3/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      491 2023-05-12 21:10:12.000000 proteinTools-1.5.3/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-12 21:10:12.000000 proteinTools-1.5.3/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-12 21:10:12.000000 proteinTools-1.5.3/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-12 21:10:12.000000 proteinTools-1.5.3/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-12 21:10:12.000000 proteinTools-1.5.3/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-12 21:10:13.134162 proteinTools-1.5.3/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      563 2023-05-12 21:09:24.000000 proteinTools-1.5.3/setup.py
```

### Comparing `proteinTools-1.5.2/LICENSE` & `proteinTools-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.5.2/proteinTools/PT.py` & `proteinTools-1.5.3/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -1072,15 +1072,15 @@
         df
             A pandas dataframe containing the primary ligand IDs and cofactor IDs within the protein structural file.
         """
         ligs = []
         for ligand in self.ligand_list:
             if ligand.ID not in ligs:
                 ligs.append(ligand.ID)
-            ligand = ligs[1]
+            ligand = ligs[0]
             cofactors = ligs[1:]
         ligands = pd.DataFrame.from_dict({'Primary Ligand':ligand, 'Cofactors':cofactors})
         return ligands
     
     @cached_property   
     def interactions(self):
         """
```

