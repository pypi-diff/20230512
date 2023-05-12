# Comparing `tmp/neurotune-0.2.5.tar.gz` & `tmp/neurotune-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurotune-0.2.5.tar", last modified: Fri May 12 16:56:14 2023, max compression
+gzip compressed data, was "neurotune-0.2.6.tar", last modified: Fri May 12 17:09:39 2023, max compression
```

## Comparing `neurotune-0.2.5.tar` & `neurotune-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:56:14.032921 neurotune-0.2.5/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      125 2016-03-08 13:39:46.000000 neurotune-0.2.5/AUTHORS
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1500 2023-05-12 16:55:05.000000 neurotune-0.2.5/LICENSE
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      836 2023-05-12 16:56:14.032921 neurotune-0.2.5/PKG-INFO
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     2141 2023-05-12 16:55:09.000000 neurotune-0.2.5/README.md
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:56:14.028921 neurotune-0.2.5/neurotune/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       22 2023-05-12 16:55:09.000000 neurotune-0.2.5/neurotune/__init__.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    18183 2021-12-09 16:25:49.000000 neurotune-0.2.5/neurotune/controllers.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    30113 2023-05-12 16:55:09.000000 neurotune-0.2.5/neurotune/evaluators.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     5637 2023-05-12 16:55:09.000000 neurotune-0.2.5/neurotune/optimizers.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     7794 2023-05-12 16:55:09.000000 neurotune-0.2.5/neurotune/utils.py
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 16:56:14.028921 neurotune-0.2.5/neurotune.egg-info/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      836 2023-05-12 16:56:13.000000 neurotune-0.2.5/neurotune.egg-info/PKG-INFO
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      322 2023-05-12 16:56:13.000000 neurotune-0.2.5/neurotune.egg-info/SOURCES.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)        1 2023-05-12 16:56:13.000000 neurotune-0.2.5/neurotune.egg-info/dependency_links.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       25 2023-05-12 16:56:13.000000 neurotune-0.2.5/neurotune.egg-info/requires.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       10 2023-05-12 16:56:13.000000 neurotune-0.2.5/neurotune.egg-info/top_level.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       80 2023-05-12 16:56:14.032921 neurotune-0.2.5/setup.cfg
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1107 2023-05-12 16:55:09.000000 neurotune-0.2.5/setup.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 17:09:39.485545 neurotune-0.2.6/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)      125 2016-03-08 13:39:46.000000 neurotune-0.2.6/AUTHORS
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1500 2023-05-12 17:09:28.000000 neurotune-0.2.6/LICENSE
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     3070 2023-05-12 17:09:39.485545 neurotune-0.2.6/PKG-INFO
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     2141 2023-05-12 16:57:44.000000 neurotune-0.2.6/README.md
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 17:09:39.485545 neurotune-0.2.6/neurotune/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       22 2023-05-12 17:09:28.000000 neurotune-0.2.6/neurotune/__init__.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)    18183 2021-12-09 16:25:49.000000 neurotune-0.2.6/neurotune/controllers.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)    30113 2023-05-12 16:57:44.000000 neurotune-0.2.6/neurotune/evaluators.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     5637 2023-05-12 16:57:44.000000 neurotune-0.2.6/neurotune/optimizers.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     7736 2023-05-12 17:09:28.000000 neurotune-0.2.6/neurotune/utils.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-05-12 17:09:39.485545 neurotune-0.2.6/neurotune.egg-info/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     3070 2023-05-12 17:09:39.000000 neurotune-0.2.6/neurotune.egg-info/PKG-INFO
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)      322 2023-05-12 17:09:39.000000 neurotune-0.2.6/neurotune.egg-info/SOURCES.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)        1 2023-05-12 17:09:39.000000 neurotune-0.2.6/neurotune.egg-info/dependency_links.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       25 2023-05-12 17:09:39.000000 neurotune-0.2.6/neurotune.egg-info/requires.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       10 2023-05-12 17:09:39.000000 neurotune-0.2.6/neurotune.egg-info/top_level.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       80 2023-05-12 17:09:39.485545 neurotune-0.2.6/setup.cfg
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1293 2023-05-12 17:09:28.000000 neurotune-0.2.6/setup.py
```

### Comparing `neurotune-0.2.5/LICENSE` & `neurotune-0.2.6/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2014, Neurotune authors and contributors
+Copyright (c) 2023, Neurotune authors and contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 Neither the names of the copyright holders nor the names of the contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

### Comparing `neurotune-0.2.5/README.md` & `neurotune-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `neurotune-0.2.5/neurotune/controllers.py` & `neurotune-0.2.6/neurotune/controllers.py`

 * *Files identical despite different names*

### Comparing `neurotune-0.2.5/neurotune/evaluators.py` & `neurotune-0.2.6/neurotune/evaluators.py`

 * *Files identical despite different names*

### Comparing `neurotune-0.2.5/neurotune/optimizers.py` & `neurotune-0.2.6/neurotune/optimizers.py`

 * *Files identical despite different names*

### Comparing `neurotune-0.2.5/neurotune/utils.py` & `neurotune-0.2.6/neurotune/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 
     Script to plot evolution of parameters in neurotune
 
 """
 
+from __future__ import annotations
 import math
 import numpy as np
+
 try:
-    from typing import List, Dict, Bool, Union
+    import typing
 except ImportError:
     pass
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def plot_generation_evolution(
-    sim_var_names,
-    target_values={},
-    individuals_file_name="../data/ga_individuals.csv",
-    show_plot_already=True,
-    save_to_file=False,
-    save_to_file_scatter=False,
-    save_to_file_hist=False,
-    title_prefix="",
-):
-    # type: (List, Dict, str, Bool, Union[Bool, str], Union[Bool, str], Union[Bool, str], str) -> None
+    sim_var_names: list,
+    target_values: dict = {},
+    individuals_file_name: str = "../data/ga_individuals.csv",
+    show_plot_already: bool = True,
+    save_to_file: typing.Union[bool, str] = False,
+    save_to_file_scatter: bool = False,
+    save_to_file_hist: bool = False,
+    title_prefix: str = "",
+) -> None:
     """Plot generation evolution related graphs.
 
     :param sim_var_names: names of variables
     :type sim_var_names: list
     :param target_values: target values provided for fitting
     :type target_values: dict
     :param individuals_file_name: name of file storing data from individual generation runs
@@ -141,34 +142,38 @@
         + " Evolution over %i generations of %s" % (generations_total, sim_var_names)
     )
     pyplot.subplots_adjust(hspace=0.4)
     pyplot.figtext(
         0.40,
         0.01,
         "Generation (%i individuals, offset slightly; larger circle => fitter)"
-        % (population_total)
+        % (population_total),
     )
     for i in range(val_num):
 
         var_name = sim_var_names[i]
 
-        pyplot.subplot(nrows, ncols, i + 1, xlabel="Generation",
-                       ylabel="{} ({})".format(var_name.split('/')[-2],
-                                               var_name.split('/')[-1]))
+        pyplot.subplot(
+            nrows,
+            ncols,
+            i + 1,
+            xlabel="Generation",
+            ylabel="{} ({})".format(var_name.split("/")[-2], var_name.split("/")[-1]),
+        )
         pyplot.title(var_name)
         if target_values is not None and sim_var_names[i] in target_values:
             value = target_values[sim_var_names[i]]
             x = [-1, generations_total + 1]
             y = [value, value]
             pyplot.plot(x, y, "--", color="grey")
 
         pyplot.scatter(generations_offset, vals[i], s=sizes[i], c=colours[i], alpha=0.4)
 
     if save_to_file_scatter:
-        pyplot.savefig(save_to_file_scatter, dpi=300, bbox_inches='tight')
+        pyplot.savefig(save_to_file_scatter, dpi=300, bbox_inches="tight")
 
     fig2 = pyplot.figure()
     pyplot.get_current_fig_manager().set_window_title(
         title_prefix
         + " Fitness over %i generations from %s"
         % (generations_total, individuals_file_name)
     )
@@ -179,49 +184,51 @@
     ax = fig2.add_subplot(2, 1, 2, ylabel="Fitness (log)")
     ax.set_yscale("log")
     ax.scatter(generations_offset, f, s=sizes[i], c=colours[i], alpha=0.4)
     pyplot.figtext(
         0.40,
         0.01,
         "Generation (%i individuals, offset slightly; larger circle => fitter)"
-        % (population_total)
+        % (population_total),
     )
 
     if save_to_file:
-        pyplot.savefig(save_to_file, dpi=300, bbox_inches='tight')
+        pyplot.savefig(save_to_file, dpi=300, bbox_inches="tight")
 
     fig3 = pyplot.figure()
     pyplot.get_current_fig_manager().set_window_title(
-        title_prefix + " Histograms over %i generations of %s" %
-        (generations_total, sim_var_names)
+        title_prefix
+        + " Histograms over %i generations of %s" % (generations_total, sim_var_names)
     )
 
     pyplot.subplots_adjust(hspace=0.4)
     for i in range(val_num):
 
-        var_name = (sim_var_names[i])
-        ax = pyplot.subplot(nrows, ncols, i + 1,
-                            xlabel="{} ({})".format(var_name.split('/')[-2],
-                                                    var_name.split('/')[-1])
-                            )
+        var_name = sim_var_names[i]
+        ax = pyplot.subplot(
+            nrows,
+            ncols,
+            i + 1,
+            xlabel="{} ({})".format(var_name.split("/")[-2], var_name.split("/")[-1]),
+        )
         pyplot.title(var_name)
 
         for generation in generations:
             values = ind_vals[i][generation]
 
             hist, bin_edges = np.histogram(values, bins=10)
             half_bin_width = (bin_edges[1] - bin_edges[0]) / 2
             xs = [be + half_bin_width for be in bin_edges[:-1]]
 
             shade = 1 - generation / (float(generations[-1]) + 1)
             # print("Gen: %s; shade: %s; value bins: %s; tots: %s"%(generation,shade,xs,hist))
             ax.plot(xs, hist, color=(shade, shade, shade))
 
     if save_to_file_hist:
-        pyplot.savefig(save_to_file_hist, dpi=300, bbox_inches='tight')
+        pyplot.savefig(save_to_file_hist, dpi=300, bbox_inches="tight")
 
     if show_plot_already:
         pyplot.show()
 
     individuals_file.close()
```

### Comparing `neurotune-0.2.5/setup.py` & `neurotune-0.2.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 
 from setuptools import setup
 
 for line in open("neurotune/__init__.py"):
     if line.startswith("__version__"):
         version = line.split("=")[1].strip()[1:-1]
 
+long_description = open("README.md").read()
+
 setup(
     name="neurotune",
     version=version,
     packages=["neurotune"],
     author="Michael Vella, Padraig Gleeson",
     author_email="mv333@cam.ac.uk, p.gleeson@gmail.com",
     description="A Python library for optimising neuronal models",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     license="BSD",
     install_requires=["scipy", "inspyred", "pyelectro"],
     url="https://github.com/NeuralEnsemble/neurotune",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
 )
```

