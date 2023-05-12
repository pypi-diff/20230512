# Comparing `tmp/picachooser-1.4.1.tar.gz` & `tmp/picachooser-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picachooser-1.4.1.tar", last modified: Tue Feb 14 18:50:35 2023, max compression
+gzip compressed data, was "dist/picachooser-1.4.2.tar", last modified: Fri May 12 02:36:13 2023, max compression
```

## Comparing `picachooser-1.4.1.tar` & `picachooser-1.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:50:35.000000 picachooser-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-14 18:50:23.000000 picachooser-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-02-14 18:50:35.000000 picachooser-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-02-14 18:50:23.000000 picachooser-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser/
--rw-r--r--   0 runner    (1001) docker     (123)    35229 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/LightboxItem.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27498 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    47120 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/graderTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    37677 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/melodicompTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/picachooserTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/picachooser_imonlyTemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    46949 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/scripts/PICAchooser
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/scripts/PICAchooser_dispatcher
--rwxr-xr-x   0 runner    (1001) docker     (123)    17102 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/scripts/grader
--rwxr-xr-x   0 runner    (1001) docker     (123)    21947 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/scripts/melodicomp
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-14 18:50:23.000000 picachooser-1.4.1/picachooser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-14 18:50:35.000000 picachooser-1.4.1/picachooser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-14 18:50:23.000000 picachooser-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-14 18:50:35.000000 picachooser-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-02-14 18:50:23.000000 picachooser-1.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-02-14 18:50:23.000000 picachooser-1.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:36:13.000000 picachooser-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-12 02:36:00.000000 picachooser-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-12 02:36:13.000000 picachooser-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-12 02:36:00.000000 picachooser-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser/
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/LightboxItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27498 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47072 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/graderTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/melodicompTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/picachooserTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/picachooser_imonlyTemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47206 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/scripts/PICAchooser
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/scripts/PICAchooser_dispatcher
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17053 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/scripts/grader
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21898 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/scripts/melodicomp
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-12 02:36:00.000000 picachooser-1.4.2/picachooser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 02:36:13.000000 picachooser-1.4.2/picachooser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-12 02:36:00.000000 picachooser-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-12 02:36:13.000000 picachooser-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-12 02:36:00.000000 picachooser-1.4.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-12 02:36:00.000000 picachooser-1.4.2/versioneer.py
```

### Comparing `picachooser-1.4.1/PKG-INFO` & `picachooser-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picachooser
-Version: 1.4.1
+Version: 1.4.2
 Summary: Lightweight GUI for sorting, classifying, and matching MELODIC ICA components.
 Home-page: https://github.com/bbfrederick/picachooser
 Author: Blaise Frederick
 Author-email: bbfrederick@mclean.harvard.edu
 License: Apache Software License
 Description: PICAchooser (the package)
         =========================
```

### Comparing `picachooser-1.4.1/README.rst` & `picachooser-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/picachooser/LightboxItem.py` & `picachooser-1.4.2/picachooser/LightboxItem.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 #
 # -*- coding: utf-8 -*-
 
 """
 A widget for displaying 3 and 4 dimensional data in a lightbox
 """
 
-from __future__ import division, print_function
-
 import os
 
 import numpy as np
 import pyqtgraph as pg
 from nibabel.affines import apply_affine
 from pyqtgraph.Qt import QtCore, QtWidgets
 
@@ -620,15 +618,15 @@
             thepos = self.zdim - 1
         if thepos < 0:
             thepos = 0
         return int(np.round(thepos))"""
 
     def optmatrix(self, horizontalmm, verticalmm, targetaspectratio, verbose=False):
         # first find all the combinations of x and y that will minimally hold all the images
-        numrows = np.arange(2, int(self.numslices // 2), 1, dtype=np.int)
+        numrows = np.arange(2, int(self.numslices // 2), 1, dtype=np.int16)
         numcols = numrows * 0
         for i in range(len(numcols)):
             numcols[i] = int(np.ceil(self.numslices / numrows[i]))
 
         # now calculate the aspect ratios of all of these combinations
         theaspectratios = (horizontalmm * numcols) / (verticalmm * numrows)
         theindex = np.argmin(np.fabs(theaspectratios - targetaspectratio))
```

### Comparing `picachooser-1.4.1/picachooser/colormaps.py` & `picachooser-1.4.2/picachooser/colormaps.py`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/picachooser/fit.py` & `picachooser-1.4.2/picachooser/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # $Author: frederic $
 # $Date: 2016/07/12 13:50:29 $
 # $Id: tide_funcs.py,v 1.4 2016/07/12 13:50:29 frederic Exp $
 #
-from __future__ import division, print_function
 
 import warnings
 
 import numpy as np
 import scipy as sp
 import scipy.special as sps
 from scipy.signal import hilbert
```

### Comparing `picachooser-1.4.1/picachooser/graderTemplate.py` & `picachooser-1.4.2/picachooser/graderTemplate.py`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/picachooser/io.py` & `picachooser-1.4.2/picachooser/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # $Author: frederic $
 # $Date: 2016/07/12 13:50:29 $
 # $Id: tide_funcs.py,v 1.4 2016/07/12 13:50:29 frederic Exp $
 #
-from __future__ import print_function, division
+import copy
+import json
+import os
+import sys
 
 import numpy as np
-import sys
-import os
 import pandas as pd
-import json
-import copy
 
 # ---------------------------------------- Global constants -------------------------------------------
 MAXLINES = 10000000
 
 # ----------------------------------------- Conditional imports ---------------------------------------
 try:
     import nibabel as nib
@@ -71,15 +70,14 @@
         nim = nib.load(inputfilename)
         nim_data = nim.get_fdata()
         nim_hdr = nim.header.copy()
         thedims = nim_hdr["dim"].copy()
         thesizes = nim_hdr["pixdim"].copy()
         return nim, nim_data, nim_hdr, thedims, thesizes
 
-    # dims are the array dimensions along each axis
     def parseniftidims(thedims):
         r"""Split the dims array into individual elements
 
         Parameters
         ----------
         thedims : int array
             The nifti dims structure
@@ -965,27 +963,29 @@
     if np.shape(inputdata)[1] > 1:
         print("specify only one column for input file 1")
         sys.exit()
     else:
         return inputdata[:, 0]
 
 
-def readvecs(inputfilename, colspec=None, numskip=0):
+def readvecs(inputfilename, colspec=None, numskip=0, debug=False):
     r"""
 
     Parameters
     ----------
     inputfilename
 
     Returns
     -------
 
     """
     with open(inputfilename, "r") as thefile:
         lines = thefile.readlines()
+    if debug:
+        print(f"readvecs: {inputfilename} has lines: {len(lines)}")
     if colspec is None:
         numvecs = len(lines[0].split())
         collist = range(0, numvecs)
     else:
         collist = colspectolist(colspec)
         if collist[-1] > len(lines[0].split()):
             print("READVECS: too many columns requested - exiting")
```

### Comparing `picachooser-1.4.1/picachooser/melodicompTemplate.py` & `picachooser-1.4.2/picachooser/melodicompTemplate.py`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/picachooser/picachooserTemplate.py` & `picachooser-1.4.2/picachooser/picachooserTemplate.py`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/picachooser/picachooser_imonlyTemplate.py` & `picachooser-1.4.2/picachooser/picachooser_imonlyTemplate.py`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/picachooser/scripts/PICAchooser` & `picachooser-1.4.2/picachooser/scripts/PICAchooser`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 #
 # -*- coding: utf-8 -*-
 
 """
 A simple GUI for rating timecoursese by whatever metric you want
 """
 
-from __future__ import division, print_function
 
 import argparse
 import os
 import sys
 
 import numpy as np
 import pyqtgraph as pg
@@ -916,14 +915,20 @@
         action="store_true",
         help=(
             "Output exhaustive amounts of information about the internal workings of PICAchooser. "
             "You almost certainly don't want this."
         ),
         default=False,
     )
+    debugging.add_argument(
+        "--debug",
+        action="store_true",
+        help=("Turn on debugging output."),
+        default=False,
+    )
 
     try:
         args = parser.parse_args()
     except SystemExit:
         print("Use --help option for detailed informtion on options.")
         raise
 
@@ -1167,35 +1172,38 @@
     else:
         tr = 1.0
     samplerate = 1.0 / tr
 
     # read in the timecourses and their current labels
     alldata = {}
     numelements = 0
-    alltcs = io.readvecs(Mixfile)
+    alltcs = io.readvecs(Mixfile, debug=args.debug)
     numelements = alltcs.shape[0]
     grades = np.ones(numelements, dtype=np.int16)
     if initfileexists:
-        print("reading initfile...")
+        print(f"reading initfile {Removefile}...")
         with open(Removefile, "r") as thefile:
             inline = thefile.readline().replace("[", "").replace("]", "")
-        inlist = inline.split(",")
+        if inline.find(",") > -1:
+            inlist = inline.split(",")
+        else:
+            inlist = inline.split()
         print(inlist)
         for component in inlist:
             print(component)
             grades[int(component) - 1] = -1
     else:
         grades = None
 
     # read in the motion timecourses
     if domotion:
         print("reading motion timecourses...")
         filebase, extension = os.path.splitext(Motionfile)
         if extension == ".par":
-            allmotion = io.readvecs(Motionfile)
+            allmotion = io.readvecs(Motionfile, debug=args.debug)
             motion = {}
             motion["xtrans"] = allmotion[3, :] * 1.0
             motion["ytrans"] = allmotion[4, :] * 1.0
             motion["ztrans"] = allmotion[5, :] * 1.0
             motion["maxtrans"] = np.max(
                 [
                     np.max(motion["xtrans"]),
@@ -1250,15 +1258,15 @@
             )
         else:
             print("cannot read files with extension", extension)
             sys.exit()
         motionlen = motion["xtrans"].shape[0]
 
     # read in the variance percents
-    melodicICstats = io.readvecs(melodicICstatsfile)
+    melodicICstats = io.readvecs(melodicICstatsfile, debug=args.debug)
 
     namelist = []
     print("reading timecourses...")
     for idx in range(numelements):
         theIC = str(idx + 1)
         namelist.append(theIC)
         if grades is not None:
```

### Comparing `picachooser-1.4.1/picachooser/scripts/PICAchooser_dispatcher` & `picachooser-1.4.2/picachooser/scripts/PICAchooser_dispatcher`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #
 #
 # $Author: frederic $
 # $Date: 2016/07/11 14:50:43 $
 #       $Id: resamp1tc,v 1.12 2016/07/11 14:50:43 frederic Exp $
 #
 
-from __future__ import division, print_function
 
 import os
 import subprocess
 import sys
 
 
 def main():
```

### Comparing `picachooser-1.4.1/picachooser/scripts/grader` & `picachooser-1.4.2/picachooser/scripts/grader`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 #
 # -*- coding: utf-8 -*-
 
 """
 A simple GUI for rating timecoursese by whatever metric you want
 """
 
-from __future__ import division, print_function
-
 import argparse
 import glob
 import os
 import sys
 
 import numpy as np
 import pandas as pd
```

### Comparing `picachooser-1.4.1/picachooser/scripts/melodicomp` & `picachooser-1.4.2/picachooser/scripts/melodicomp`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 #
 # -*- coding: utf-8 -*-
 
 """
 A simple GUI for rating timecoursese by whatever metric you want
 """
 
-from __future__ import division, print_function
-
 import argparse
 import os
 import sys
 
 import numpy as np
 from pyqtgraph.Qt import QtCore, QtWidgets
 from scipy.stats import pearsonr
```

### Comparing `picachooser-1.4.1/picachooser/stats.py` & `picachooser-1.4.2/picachooser/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 # $Author: frederic $
 # $Date: 2016/07/12 13:50:29 $
 # $Id: tide_funcs.py,v 1.4 2016/07/12 13:50:29 frederic Exp $
 #
-from __future__ import division, print_function
 
 import numpy as np
 import scipy as sp
 from scipy.stats import johnsonsb, kurtosis, kurtosistest
 
 import picachooser.fit as fit
 import picachooser.io as io
```

### Comparing `picachooser-1.4.1/picachooser/util.py` & `picachooser-1.4.2/picachooser/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import picachooser._version as pica_versioneer
 
+
 # ------------------------------------------ Version function ----------------------------------
 def version():
     """
 
     Returns
     -------
 
@@ -41,9 +42,7 @@
     thedate = versioninfo["date"]
     if thedate is None:
         thedate = "UNKNOWN"
     isdirty = versioninfo["dirty"]
     if isdirty is None:
         isdirty = "UNKNOWN"
     return version, longgittag, thedate, isdirty
-
-
```

### Comparing `picachooser-1.4.1/picachooser.egg-info/PKG-INFO` & `picachooser-1.4.2/picachooser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picachooser
-Version: 1.4.1
+Version: 1.4.2
 Summary: Lightweight GUI for sorting, classifying, and matching MELODIC ICA components.
 Home-page: https://github.com/bbfrederick/picachooser
 Author: Blaise Frederick
 Author-email: bbfrederick@mclean.harvard.edu
 License: Apache Software License
 Description: PICAchooser (the package)
         =========================
```

### Comparing `picachooser-1.4.1/picachooser.egg-info/SOURCES.txt` & `picachooser-1.4.2/picachooser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/pyproject.toml` & `picachooser-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/setup.py` & `picachooser-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `picachooser-1.4.1/versioneer.py` & `picachooser-1.4.2/versioneer.py`

 * *Files identical despite different names*

