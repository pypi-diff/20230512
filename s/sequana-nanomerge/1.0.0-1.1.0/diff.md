# Comparing `tmp/sequana_nanomerge-1.0.0.tar.gz` & `tmp/sequana_nanomerge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequana_nanomerge-1.0.0.tar", last modified: Mon Apr 17 13:32:43 2023, max compression
+gzip compressed data, was "dist/sequana_nanomerge-1.1.0.tar", last modified: Fri May 12 09:47:21 2023, max compression
```

## Comparing `sequana_nanomerge-1.0.0.tar` & `sequana_nanomerge-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-17 13:32:43.899558 sequana_nanomerge-1.0.0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/LICENSE
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5894 2023-04-17 13:32:43.899558 sequana_nanomerge-1.0.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4566 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       25 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-17 13:32:43.899558 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5894 2023-04-17 13:32:43.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      635 2023-04-17 13:32:43.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-04-17 13:32:43.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       76 2023-04-17 13:32:43.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-04-17 13:32:33.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      118 2023-04-17 13:32:43.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2023-04-17 13:32:43.000000 sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-17 13:32:43.898558 sequana_nanomerge-1.0.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-17 13:32:43.899558 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1727 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13153 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/dag.png
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4538 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4892 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/nanomerge.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        7 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      457 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      255 2023-04-17 13:32:43.900558 sequana_nanomerge-1.0.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3557 2023-04-17 13:29:35.000000 sequana_nanomerge-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5383 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4538 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5191 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/nanomerge.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-12 09:47:21.000000 sequana_nanomerge-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-05-12 09:47:17.000000 sequana_nanomerge-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sequana_nanomerge-1.0.0/PKG-INFO` & `sequana_nanomerge-1.1.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,30 @@
-Metadata-Version: 2.1
-Name: sequana_nanomerge
-Version: 1.0.0
-Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
-Home-page: https://github.com/sequana/
-Author: thomas cokelaer
-Author-email: thomas.cokelaer@pasteur.fr
-Maintainer: thomas cokelaer
-Maintainer-email: thomas.cokelaer@pasteur.fr
-License: new BSD
-Keywords: nanopore, fastq, merge
-Platform: Linux
-Platform: Unix
-Platform: MacOsX
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
-License-File: LICENSE
-
 
 .. image:: https://badge.fury.io/py/sequana-nanomerge.svg
      :target: https://pypi.python.org/pypi/sequana_nanomerge
 
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
     :target: http://joss.theoj.org/papers/10.21105/joss.00352
     :alt: JOSS (journal of open source software) DOI
 
 .. image:: https://github.com/sequana/nanomerge/actions/workflows/main.yml/badge.svg
    :target: https://github.com/sequana/nanomerge/actions/workflows
 
+.. image:: https://coveralls.io/repos/github/sequana/nanomerge/badge.svg?branch=main
+   :target: https://coveralls.io/github/sequana/nanomerge?branch=main
+
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+   :target: http://joss.theoj.org/papers/10.21105/joss.00352
+   :alt: JOSS (journal of open source software) DOI
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
 
 
 
 This is is the **nanomerge** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
 
 :Overview: merge fastq files generated by Nanopore run and generated raw data QC.
 :Input: individual fastq files generated by nanopore demultiplexing
@@ -58,17 +36,19 @@
 Installation
 ~~~~~~~~~~~~
 
 You can install the packages using pip::
 
     pip install sequana_nanomerge --upgrade
 
-An optional requirements is pycoQC, which can be install with conda/mamba using e.g.:
+An optional requirements is pycoQC, which can be install with conda/mamba using e.g.::
+
+    conda install pycoQC
 
-    conda install pycoQC.
+you will also need graphviz installed.
 
 Usage
 ~~~~~
 
 ::
 
     sequana_nanomerge --help
@@ -79,43 +59,43 @@
         --summary summary.txt --input-pattern '*/*fastq.gz'
 
 otherwise all fastq files are in DATAPATH/::
 
     sequana_nanomerge --input-directory DATAPATH --samplesheet samplesheet.csv
         --summary summary.txt --input-pattern '*fastq.gz'
 
-The --summary is optional and takes as input the output of albacore demultiplexing. usually a file called sequencing_summary.txt
+The --summary is optional and takes as input the output of albacore/guppy demultiplexing. usually a file called sequencing_summary.txt
 
-Note that the different between the two is the extra `*/` before the `*.fastq.gz` pattern since barcoded files are in individual subdirectories..
+Note that the different between the two is the extra `*/` before the `*.fastq.gz` pattern since barcoded files are in individual subdirectories.
 
 In both bases, the command creates a directory with the pipeline and configuration file. You will then need to execute the pipeline::
 
     cd nanomerge
     sh nanomerge.sh  # for a local run
 
 This launch a snakemake pipeline. If you are familiar with snakemake, you can 
 retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
 
     snakemake -s nanomerge.rules -c config.yaml --cores 4 --stats stats.txt
 
 Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
 
-COncerning the sample sheet, whther your data is barcoded or not, it should be a CSV file ::
+Concerning the sample sheet, whether your data is barcoded or not, it should be a CSV file ::
 
     barcode,project,sample
     barcode01,main,A
     barcode02,main,B
     barcode03,main,C
 
-For a non-barcoded run, you must provide a file where the barcode column can be set (empty) or just removed::
+For a non-barcoded run, you must provide a file where the barcode column can be set (empty)::
 
     barcode,project,sample
     ,main,A
 
-or::
+or just removed::
 
     project,sample
     main,A
 
 Usage with apptainer::
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -139,14 +119,15 @@
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s), which is optional:
 
 - pycoQC
+- dot
 
 .. image:: https://raw.githubusercontent.com/sequana/nanomerge/main/sequana_pipelines/nanomerge/dag.png
 
 
 Details
 ~~~~~~~~~
 
@@ -162,12 +143,16 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
+            runs such as promethion
+1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
+          * Fix the pyco file paths, update requirements and doc
 1.0.0     Stable release ready for production
 0.0.1     **First release.**
 ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.0.0/sequana_nanomerge.egg-info/SOURCES.txt` & `sequana_nanomerge-1.1.0/sequana_nanomerge.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 sequana_nanomerge.egg-info/PKG-INFO
 sequana_nanomerge.egg-info/SOURCES.txt
```

### Comparing `sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/config.yaml` & `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,41 @@
 #
 # One of input_directory, input_pattern and input_samples must be provided
 # If input_directory provided, use it otherwise if input_pattern provided,
 # use it, otherwise use input_samples.
 # ============================================================================
 
 # Keep input_readtag empty for nanopore
-#input_directory: '/home/cokelaer/TEMP/fastq_pass/barcode21'
-input_directory: '/home/cokelaer/TEMP/fastq_pass/'
+input_directory:
 input_readtag:
 input_pattern: '*/*.fastq.gz'
-summary: /home/cokelaer/TEMP/fastq_pass/sequencing_summary_AOI637_ef78de7c_aef0cc4b.txt
-#samplesheet: "samplesheet1.csv"
+summary:
 samplesheet: "samplesheet.csv"
 
 ################################################################################
 # extra_prefixes_to_strip
 #
 # In most cases, the input_directory and input_pattern (and input_read_tag for paired analysis)
 # allows us to retrieve unique sample names. We automatically removed common prefixes for you.
 #
 # Sometimes, some prefixes are not common to all samples but still need to be removed
 # to get unique sample names or better output. You can provide extra prefixes to be removed
 # by uncommenting and filling the field extra_prefixes_to_strip.
 #
 # For instance, if you have files called prefix.mess.A.fastq.gz and prefix.B.fastq.gz
-# 'prefix.' will be removed automatically because it is common, but not 'mess'. 
+# 'prefix.' will be removed automatically because it is common, but not 'mess'.
 # use thoses prefixes in the left to right order ['prefix', 'mess'] or ['prefix.mess']
 #
 # extra_prefixes_to_strip: []
 
 apptainers:
-  pycoqc: https://zenodo.org/record/7746269/files/pycoqc_2.5.2.img
+  pycoqc: "https://zenodo.org/record/7746269/files/pycoqc_2.5.2.img"
+  graphviz: "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
+
+
+###################################################################################
+#
+# subsample: If not None, N number of reads will be randomly selected instead of
+#     the entire dataset
+pycoqc:
+  subsample: 1000000
```

### Comparing `sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/dag.png` & `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/main.py` & `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/main.py`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.0.0/sequana_pipelines/nanomerge/nanomerge.rules` & `sequana_nanomerge-1.1.0/sequana_pipelines/nanomerge/nanomerge.rules`

 * *Files 16% similar despite different names*

```diff
@@ -50,39 +50,41 @@
 barcodes = [x.name for x in input_directory.glob("*") if x.is_dir()]
 
 class Sample():
 
     def __init__(self, samplesheet, barcoded):
         self.df = pd.read_csv(samplesheet)
         self.barcoded = barcoded
+        if "sample" not in self.df.columns:
+            self.df['sample'] = self.df['samplename']
 
     def get_barcode_from_sample(self, sample):
-        if "sample" in self.df.columns:
-            candidate = self.df.query("sample==@sample")['barcode'].values[0]
-        elif "samplename" in self.df.columns:
-            candidate = self.df.query("sample==@samplename")['barcode'].values[0]
+        candidate = self.df.query("sample==@sample")['barcode'].values[0]
         return candidate
 
     def get_projects(self):
         return self.df.project.unique()
 
 
 if len(barcodes) == 0:
     samples = Sample(config['samplesheet'], barcoded=False)
 else:
     samples = Sample(config['samplesheet'], barcoded=True)
 
 
 if config["summary"]:
-    qc_file = "pyco/pyco.html"
+    qc_file = ["pyco/pyco.html"]
 else:
-    qc_file = ""
+    qc_file = []
 
 # ========================================================================= pipeline starts here
-expected_fastqs = expand("./{project}/{sample}.fastq.gz", zip, project=samples.df['project'], sample=samples.df['sample']),
+expected_fastqs = expand("./{project}/{sample}.fastq.gz", zip, project=samples.df['project'],
+        sample=samples.df['sample'])
+
+
 rule pipeline:
     input:
         expected_fastqs,
         svg = ".sequana/rulegraph.svg",
         html="summary.html"
 
 
@@ -96,75 +98,90 @@
 
 
 if config["summary"]:
     rule pyco:
         input:
             config['summary']
         output:
-            temp(qc_file)
+            "pyco/pyco.html"
         log:
-            temp(qc_file)
+            "pyco/pyco.log"
+        params:
+            sample=config["pycoqc"]["subsample"]
         container:
             config["apptainers"]["pycoqc"]
         shell:
             """
-            pycoQC --summary_file {input} -o {output} > {log} 2>&1
+            pycoQC --summary_file {input} -o {output} --sample {params.sample} > {log} 2>&1
             """
 
+
 rule merge:
     input:
         get_input_merge
     output:
         "./{project}/{sample}.fastq.gz"
-
     shell:
         """
         cat {input} > {output}
         """
 
 
 rule rulegraph:
-    input: str(manager.snakefile)
+    input:
+        workflow.snakefile
     output:
-        svg = ".sequana/rulegraph.svg"
+        "rulegraph/rulegraph.dot"
     params:
         configname = "config.yaml"
     wrapper:
         f"{sequana_wrapper_branch}/wrappers/rulegraph"
 
 
+rule dot2svg:
+    input:
+        "rulegraph/rulegraph.dot"
+    output:
+        ".sequana/rulegraph.svg"
+    container:
+        config['apptainers']['graphviz']
+    shell:
+        """dot -Tsvg {input} -o {output}"""
+
+
 rule html_report:
     input:
-        list(expected_fastqs) + [qc_file]
+        list(expected_fastqs) + qc_file
     output:
         "summary.html"
     run:
         from sequana.modules_report.summary import SummaryModule2
         from sequana_pipelines import nanomerge
         os.makedirs("images", exist_ok=True)
         data = {"name": "nanomerge",
                  "rulegraph": ".sequana/rulegraph.svg",
                  "pipeline_version": nanomerge.version}
-        manager.teardown(extra_files_to_remove=["pyco/pyco.log", qc_file])
+        manager.teardown(extra_files_to_remove=["pyco/pyco.log", "pyco/pyco.html"])
 
         dirs = ",".join([f'<a href="{x}/">{x}</a>' for x in samples.get_projects()])
         if config['summary']:
-            with open(qc_file, "r") as fout:
+            with open("pyco/pyco.html", "r") as fout:
                 pycodata = fout.read()
                 pycodata = '<div class="columns">' + pycodata.split('<div class="columns">')[-1].replace("</div>\n</body>\n</html>","")
 
             s = SummaryModule2(data, f"Your data are available in {dirs} directories" + pycodata)
         else:
             s = SummaryModule2(data, f"no summary found. Please checkout the sub directories {dirs}. They should contain your final fastq files for each project.")
 
 # ======================================================================================== rulegraph
 
 
 onsuccess:
 
     print("Once done, please clean up the directory using\n'make clean'")
     shell("chmod -R g+w .")
+    shell("rm -rf pyco rulegraph")
 
 onerror:
     from sequana_pipetools.errors import PipeError
     p = PipeError("nanomerge")
     p.status()
```

### Comparing `sequana_nanomerge-1.0.0/setup.py` & `sequana_nanomerge-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # handle sequana git link
 with open("requirements.txt", encoding='utf-8') as fh:
     requirements = [req.rstrip() if not req.startswith("git+") else req.rstrip().split("egg=")[-1] for req in fh]
 
 
 _MAJOR               = 1
-_MINOR               = 0
+_MINOR               = 1
 _MICRO               = 0
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
```

