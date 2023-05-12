# Comparing `tmp/panfeed-1.3.0.tar.gz` & `tmp/panfeed-1.4.0.tar.gz`

## Comparing `panfeed-1.3.0.tar` & `panfeed-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.3.0/environment.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 panfeed-1.3.0/make_release.txt
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-get-clusters-runner.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-get-kmers-runner.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-plot-runner.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-runner.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/__init__.py
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/classes.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/colorlog.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/get_clusters.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/get_kmers.py
--rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/input.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/panfeed.py
--rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/plot.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.3.0/LICENSE
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.3.0/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.4.0/environment.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-get-clusters-runner.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-get-kmers-runner.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-plot-runner.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed-runner.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/__init__.py
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/classes.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/colorlog.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/get_clusters.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/get_kmers.py
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/input.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/panfeed.py
+-rw-r--r--   0        0        0    16450 2020-02-02 00:00:00.000000 panfeed-1.4.0/panfeed/plot.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.4.0/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.4.0/PKG-INFO
```

### Comparing `panfeed-1.3.0/panfeed/__main__.py` & `panfeed-1.4.0/panfeed/__main__.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/classes.py` & `panfeed-1.4.0/panfeed/classes.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/colorlog.py` & `panfeed-1.4.0/panfeed/colorlog.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/get_clusters.py` & `panfeed-1.4.0/panfeed/get_clusters.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/get_kmers.py` & `panfeed-1.4.0/panfeed/get_kmers.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/input.py` & `panfeed-1.4.0/panfeed/input.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/panfeed.py` & `panfeed-1.4.0/panfeed/panfeed.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/panfeed/plot.py` & `panfeed-1.4.0/panfeed/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -252,42 +252,48 @@
             logger.warning(f"Skipping {gene}")
             continue
 
         # p-value matrix
         g = cl.pivot_table(index='strain', columns='gene_start',
                            values='significance',
                            aggfunc=max)
+        # add missing positions, if any
+        g = g.reindex(columns=range(cl['gene_start'].min(), cl['gene_start'].max()+1))
         # add missing strains for which no entry is present in k-mers table
         if len(strains.difference(g.index)) > 0:
             g = g.reindex(sorted(g.index) + sorted(strains.difference(g.index)))
         if args.phenotype_column is None:
             # sort the table by p-values
             g = g.loc[g.fillna(0).T.max().sort_values(ascending=False).index]
         else:
             # sort by phenotype
             g = g.loc[p.index]
 
         # nucleotide matrix
         b = cl.pivot_table(index='strain', columns='gene_start',
                            values='scalar',
                            aggfunc=handle_paralogs)
+        # add missing positions, if any
+        b = b.reindex(columns=range(cl['gene_start'].min(), cl['gene_start'].max()+1))
         # add missing strains for which no entry is present in k-mers table
         if len(strains.difference(b.index)) > 0:
             b = b.reindex(sorted(b.index) + sorted(strains.difference(b.index)))
         if args.phenotype_column is None:
             # sort the table by p-values
             b = b.loc[g.index]
         else:
             # sort by phenotype
             b = b.loc[p.index]
         if args.nucleotides:
             # nucleotide matrix
             t = cl.pivot_table(index='strain', columns='gene_start',
                                values='base',
                                aggfunc=handle_paralogs_text)
+            # add missing positions, if any
+            t = t.reindex(columns=range(cl['gene_start'].min(), cl['gene_start'].max()+1))
             # add missing strains for which no entry is present in k-mers table
             if len(strains.difference(t.index)) > 0:
                 t = t.reindex(sorted(t.index) + sorted(strains.difference(t.index)),
                               fill_value='-')
             if args.phenotype_column is None:
                 # sort the table by p-values
                 t = t.loc[g.index]
```

### Comparing `panfeed-1.3.0/LICENSE` & `panfeed-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/README.md` & `panfeed-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/pyproject.toml` & `panfeed-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panfeed-1.3.0/PKG-INFO` & `panfeed-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panfeed
-Version: 1.3.0
+Version: 1.4.0
 Summary: Compute gene-cluster specific k-mers over a pangenome
 Project-URL: Homepage, https://github.com/microbial-pangenomes-lab/panfeed
 Project-URL: Bug Tracker, https://github.com/microbial-pangenomes-lab/panfeed/issues
 Author-email: Hannes Neubauer <neubauer.hannes@mh-hannover.de>, Marco Galardini <galardini.marco@mh-hannover.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

