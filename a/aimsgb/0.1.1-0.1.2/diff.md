# Comparing `tmp/aimsgb-0.1.1.tar.gz` & `tmp/aimsgb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsgb-0.1.1.tar", last modified: Mon Jun 20 22:59:49 2022, max compression
+gzip compressed data, was "aimsgb-0.1.2.tar", last modified: Fri May 12 05:17:06 2023, max compression
```

## Comparing `aimsgb-0.1.1.tar` & `aimsgb-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2022-06-20 22:59:49.215598 aimsgb-0.1.1/
--rw-r--r--   0 jianli     (501) staff       (20)     5402 2022-06-20 22:59:49.215765 aimsgb-0.1.1/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)     3507 2022-02-18 17:39:30.000000 aimsgb-0.1.1/README.rst
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2022-06-20 22:59:49.213590 aimsgb-0.1.1/aimsgb/
--rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-0.1.1/aimsgb/__init__.py
--rw-r--r--   0 jianli     (501) staff       (20)     6662 2019-01-09 23:19:05.000000 aimsgb-0.1.1/aimsgb/agb.py
--rw-r--r--   0 jianli     (501) staff       (20)     7636 2022-06-20 18:42:05.000000 aimsgb-0.1.1/aimsgb/grain.py
--rw-r--r--   0 jianli     (501) staff       (20)    22413 2022-02-18 17:39:30.000000 aimsgb-0.1.1/aimsgb/grain_bound.py
--rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-0.1.1/aimsgb/utils.py
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2022-06-20 22:59:49.215302 aimsgb-0.1.1/aimsgb.egg-info/
--rw-r--r--   0 jianli     (501) staff       (20)     5402 2022-06-20 22:59:49.000000 aimsgb-0.1.1/aimsgb.egg-info/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)      298 2022-06-20 22:59:49.000000 aimsgb-0.1.1/aimsgb.egg-info/SOURCES.txt
--rw-r--r--   0 jianli     (501) staff       (20)        1 2022-06-20 22:59:49.000000 aimsgb-0.1.1/aimsgb.egg-info/dependency_links.txt
--rw-r--r--   0 jianli     (501) staff       (20)       44 2022-06-20 22:59:49.000000 aimsgb-0.1.1/aimsgb.egg-info/entry_points.txt
--rw-r--r--   0 jianli     (501) staff       (20)        9 2022-06-20 22:59:49.000000 aimsgb-0.1.1/aimsgb.egg-info/requires.txt
--rw-r--r--   0 jianli     (501) staff       (20)        7 2022-06-20 22:59:49.000000 aimsgb-0.1.1/aimsgb.egg-info/top_level.txt
--rw-r--r--   0 jianli     (501) staff       (20)       80 2022-06-20 22:59:49.216351 aimsgb-0.1.1/setup.cfg
--rw-r--r--   0 jianli     (501) staff       (20)     5211 2022-06-20 22:59:13.000000 aimsgb-0.1.1/setup.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-12 05:17:06.261973 aimsgb-0.1.2/
+-rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-0.1.2/LICENSE.txt
+-rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-12 05:17:06.262088 aimsgb-0.1.2/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)     3697 2022-06-21 05:53:18.000000 aimsgb-0.1.2/README.rst
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-12 05:17:06.259312 aimsgb-0.1.2/aimsgb/
+-rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-0.1.2/aimsgb/__init__.py
+-rw-r--r--   0 jianli     (501) staff       (20)     7367 2023-05-09 23:32:55.000000 aimsgb-0.1.2/aimsgb/agb.py
+-rw-r--r--   0 jianli     (501) staff       (20)     8833 2023-05-12 04:44:43.000000 aimsgb-0.1.2/aimsgb/grain.py
+-rw-r--r--   0 jianli     (501) staff       (20)    22091 2023-05-12 04:44:56.000000 aimsgb-0.1.2/aimsgb/grain_bound.py
+-rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-0.1.2/aimsgb/utils.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-12 05:17:06.261763 aimsgb-0.1.2/aimsgb.egg-info/
+-rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)      310 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/SOURCES.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        1 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/dependency_links.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       43 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/entry_points.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       22 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/requires.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        7 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/top_level.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       80 2023-05-12 05:17:06.262523 aimsgb-0.1.2/setup.cfg
+-rw-r--r--   0 jianli     (501) staff       (20)     5238 2023-05-10 20:13:09.000000 aimsgb-0.1.2/setup.py
```

### Comparing `aimsgb-0.1.1/PKG-INFO` & `aimsgb-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,96 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: aimsgb
-Version: 0.1.1
+Version: 0.1.2
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
-Maintainer-email: jic198@ucsd.edu, sij014@ucsd.edu, kesong@ucsd.edu
-License: UNKNOWN
-Description: 
-        Introduction
-        ============
-        aimsgb, an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
-        construct various grain boundary structures from cubic and non-cubic initial
-        configurations. A convenient command line tool has also been provided to enable
-        easy and fast construction of tilt and twist boundaries by assigining the degree
-        of fit (Σ), rotation axis, grain boundary plane and initial crystal structure.
-        aimsgb is expected to greatly accelerate the theoretical investigation of
-        grain boundary properties and facilitate the experimental analysis of grain
-        boundary structures as well.
-        
-        A reference for the usage of aimsGB software is:
-        Jianli Cheng, Jian Luo, and Kesong Yang, Aimsgb: An Algorithm and OPen-Source Python Library to Generate Periodic Grain Boundary Structures, Comput. Mater. Sci. 155, 92-103, (2018). 
-        DOI:10.1016/j.commatsci.2018.08.029  
-        
-        Install aimsgb
-        ==============
-        1. Clone the latest version from github::
-        
-            git clone git@github.com:ksyang2013/aimsgb.git
-        
-        2. Navigate to aimsgb folder::
-        
-            cd aimsgb
-        
-        3. Type in the root of the repo::
-        
-            pip install .
-        
-        4. or to install the package in development mode::
-        
-            pip install -e .
-        
-        
-        How to cite aimsgb
-        ==================
-        
-        If you use aimsgb in your research, please consider citing the following work:
-        
-            Jianli Cheng, Jian Luo, Kesong Yang. *Aimsgb: An algorithm and open-source python
-            library to generate periodic grain boundary structures.* Computational Materials
-            Science, 2018, 155, 92-103. `doi:10.1016/j.commatsci.2018.08.029
-            <https://doi.org/10.1016/j.commatsci.2018.08.029>`_
-        
-        
-        Copyright
-        =========
-        Copyright (C) 2018 The Regents of the University of California
-        
-        All Rights Reserved. Permission to copy, modify, and distribute this software and its documentation for educational, research and non-profit purposes, without fee, and without a written agreement is hereby granted, provided that the above copyright notice, this paragraph and the following three paragraphs appear in all copies. Permission to make commercial use of this software may be obtained by contacting:
-        
-        Office of Innovation and Commercialization
-        9500 Gilman Drive, Mail Code 0910
-        University of California
-        La Jolla, CA 92093-0910
-        (858) 534-5815
-        innovation@ucsd.edu
-        
-        This software program and documentation are copyrighted by The Regents of the University of California. The software program and documentation are supplied “as is”, without any accompanying services from The Regents. The Regents does not warrant that the operation of the program will be uninterrupted or error-free. The end-user understands that the program was developed for research purposes and is advised not to rely exclusively on the program for any reason.
-        
-        IN NO EVENT SHALL THE UNIVERSITY OF CALIFORNIA BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF THE UNIVERSITY OF CALIFORNIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. THE UNIVERSITY OF CALIFORNIA SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN “AS IS” BASIS, AND THE UNIVERSITY OF CALIFORNIA HAS NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
-        
-        
-        Authors
-        =======
-        Dr. Jianli Cheng (jic198@ucsd.edu)
-        New Email: jianlicheng@lbl.gov
-        
-        Prof. Kesong Yang  (kesong@ucsd.edu)
-        
-        About the aimsgb Development Team
-        =================================
-        http://materials.ucsd.edu/
-        
+Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE.txt
+
+
+Introduction
+============
+aimsgb, an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
+construct various grain boundary structures from cubic and non-cubic initial
+configurations. A convenient command line tool has also been provided to enable
+easy and fast construction of tilt and twist boundaries by assigining the degree
+of fit (Σ), rotation axis, grain boundary plane and initial crystal structure.
+aimsgb is expected to greatly accelerate the theoretical investigation of
+grain boundary properties and facilitate the experimental analysis of grain
+boundary structures as well.
+
+A reference for the usage of aimsGB software is:
+Jianli Cheng, Jian Luo, and Kesong Yang, Aimsgb: An Algorithm and OPen-Source Python Library to Generate Periodic Grain Boundary Structures, Comput. Mater. Sci. 155, 92-103, (2018). 
+DOI:10.1016/j.commatsci.2018.08.029  
+
+Install aimsgb
+==============
+1. Clone the latest version from github::
+
+    git clone git@github.com:ksyang2013/aimsgb.git
+
+2. Navigate to aimsgb folder::
+
+    cd aimsgb
+
+3. Type in the root of the repo::
+
+    pip install .
+
+4. or to install the package in development mode::
+
+    pip install -e .
+
+
+How to cite aimsgb
+==================
+
+If you use aimsgb in your research, please consider citing the following work:
+
+    Jianli Cheng, Jian Luo, Kesong Yang. *Aimsgb: An algorithm and open-source python
+    library to generate periodic grain boundary structures.* Computational Materials
+    Science, 2018, 155, 92-103. `doi:10.1016/j.commatsci.2018.08.029
+    <https://doi.org/10.1016/j.commatsci.2018.08.029>`_
+
+
+Copyright
+=========
+Copyright (C) 2018 The Regents of the University of California
+
+All Rights Reserved. Permission to copy, modify, and distribute this software and its documentation for educational, research and non-profit purposes, without fee, and without a written agreement is hereby granted, provided that the above copyright notice, this paragraph and the following three paragraphs appear in all copies. Permission to make commercial use of this software may be obtained by contacting:
+
+Office of Innovation and Commercialization
+9500 Gilman Drive, Mail Code 0910
+University of California
+La Jolla, CA 92093-0910
+(858) 534-5815
+innovation@ucsd.edu
+
+This software program and documentation are copyrighted by The Regents of the University of California. The software program and documentation are supplied “as is”, without any accompanying services from The Regents. The Regents does not warrant that the operation of the program will be uninterrupted or error-free. The end-user understands that the program was developed for research purposes and is advised not to rely exclusively on the program for any reason.
+
+IN NO EVENT SHALL THE UNIVERSITY OF CALIFORNIA BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF THE UNIVERSITY OF CALIFORNIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. THE UNIVERSITY OF CALIFORNIA SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN “AS IS” BASIS, AND THE UNIVERSITY OF CALIFORNIA HAS NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
+
+
+Authors
+=======
+Dr. Jianli Cheng (jic198@ucsd.edu)
+New Email: jianlicheng@lbl.gov
+
+Prof. Kesong Yang  (kesong@ucsd.edu)
+
+About the aimsgb Development Team
+=================================
+http://materials.ucsd.edu/
```

### Comparing `aimsgb-0.1.1/README.rst` & `aimsgb-0.1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 boundary structures as well.
 
 We also provide a web-based GUI to access aimsgb framework: `aimsgb.org
 <http://aimsgb.org/>`_
 
 Install aimsgb
 ==============
+Method 1: Use Pip
+-----------------
+The easiest way to install aimsgb is to simply run a one-liner in pip::
+
+   pip install aimsgb
+
+Method 2: Use Git to install
+----------------------------
 1. Clone the latest version from github::
 
     git clone https://github.com/ksyang2013/aimsgb.git
 
 2. Navigate to aimsgb folder::
 
     cd aimsgb
```

### Comparing `aimsgb-0.1.1/aimsgb/agb.py` & `aimsgb-0.1.2/aimsgb/agb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 from __future__ import division
 
 import sys
 import argparse
 import numpy as np
+from mp_api.client import MPRester, MPRestError
 
 from aimsgb import Grain, GBInformation, GrainBoundary
 
 __author__ = "Jianli Cheng and Kesong YANG"
 __copyright__ = "Copyright (C) 2018 The Regents of the University of California"
 __maintainer__ = "Jianli Cheng"
 __email__ = "jic198@ucsd.edu"
@@ -31,15 +32,27 @@
     sigma = args.sigma
     print(GBInformation(axis, sigma).__str__())
 
 
 def gb(args):
     axis = list(map(int, args.axis))
     plane = args.plane
-    initial_struct = Grain.from_file(args.poscar)
+    initial_struct = None
+    if args.filename:
+        initial_struct = Grain.from_file(args.filename)
+    elif args.mpid:
+        mpr = MPRester()
+        try:
+            s = mpr.get_structure_by_material_id(args.mpid)
+            initial_struct = Grain.from_dict(s.as_dict())
+        except MPRestError:
+            raise MPRestError("Please run 'export MP_API_KEY=YOUR_MAPI_KEY' to setup your api_key first.")
+    if initial_struct is None:
+        raise ValueError("Please provide either filename or mpid.")
+    
     gb = GrainBoundary(axis, args.sigma, plane, initial_struct, args.uc_a, args.uc_b)
     to_primitive = False if args.conventional else True
     gb.build_gb(args.vacuum, args.add_if_dist, to_primitive, args.delete_layer,
                 args.tol).to(filename=args.out, fmt=args.fmt)
     print("CSL Matrix (det=%.1f):\n%s" % (np.linalg.det(gb.csl), gb.csl))
     print("%s of sigma%s[%s]/(%s) is created"
           % (args.out, gb.sigma, args.axis, gb.plane_str))
@@ -63,58 +76,60 @@
                                      "EXAMPLE: aimsgb list 001 100")
     parser_gb_list.set_defaults(func=gb_list)
 
     parser_gb = subparsers.add_parser(
         "gb", help="Build grain boundary based on rotation axis, sigma, GB plane, "
                    "and input structure file.\nThe user can also specify many "
                    "optional arguments, such grain size and interface terminations."
-                   "\nEXAMPLE1: aimsgb gb 001 5 1 2 0 POSCAR"
-                   "\nEXAMPLE2: aimsgb gb 001 5 1 2 0 POSCAR -ua 2 -ub 3"
-                   "\nEXAMPLE3: aimsgb gb 001 5 1 2 0 POSCAR -ua 3 -ub 2 -dl 0b1t1b0t",
+                   "\nEXAMPLE1: aimsgb gb 001 5 1 2 0 -f POSCAR"
+                   "\nEXAMPLE2: aimsgb gb 001 5 1 2 0 -mp mp-13 -ua 2 -ub 3"
+                   "\nEXAMPLE3: aimsgb gb 001 5 1 2 0 -f POSCAR -ua 3 -ub 2 -dl 0b1t1b0t",
         formatter_class=argparse.RawTextHelpFormatter)
     parser_gb.add_argument("axis", metavar="rotation axis", type=str,
                            help="The rotation axis of GB, EXAMPLE: 110")
     parser_gb.add_argument("sigma", type=int,
                            help="The sigma value for grain boundary, EXAMPLE: 3")
     parser_gb.add_argument("plane", type=int, nargs=3,
                            help="The GB plane for grain boundary, EXAMPLE: 1 1 0")
-    parser_gb.add_argument("poscar", type=str,
+    parser_gb.add_argument("-f", "--filename", type=str,
                            help="The initial structure file for grain boundary.")
-    parser_gb.add_argument("out", type=str, default="POSCAR", nargs="?",
+    parser_gb.add_argument("-mp", "--mpid", type=str,
+                           help="The mpid to get initial structure from Materials Project.")
+    parser_gb.add_argument("-o", "--out", type=str, default="POSCAR", 
                            help="The output filename. (default: %(default)s)")
     parser_gb.add_argument("-ua", "--uc_a", default=1, type=int,
                            help="The size (uc) for grain A. (default: %(default)s)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -ua 2")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -ua 2")
     parser_gb.add_argument("-ub", "--uc_b", default=1, type=int,
                            help="The size (uc) for grain B. (default: %(default)s)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -ub 2")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -ub 2")
     parser_gb.add_argument("-dl", "--delete_layer", default="0b0t0b0t", type=str,
                            help="Delete bottom or top layers for each grain. "
                                 "(default: %(default)s)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -dl 0b1t1b0t")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -dl 0b1t1b0t")
     parser_gb.add_argument("-v", "--vacuum", default=0.0, type=float,
                            help="Set vacuum thickness for grain boundary. "
                                 "(default: %(default)s angstrom)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -v 20")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -v 20")
     parser_gb.add_argument("-t", "--tol", default=0.25, type=float,
                            help="Tolerance factor to determine if two "
                                 "atoms are at the same plane. "
                                 "(default: %(default)s angstrom)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -dl 0b1t1b0t -t 0.5")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -dl 0b1t1b0t -t 0.5")
     parser_gb.add_argument("-ad", "--add_if_dist", default=0.0, type=float,
                            help="Add extra distance between two grains. "
                                 "(default: %(default)s angstrom)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -ad 0.5")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -ad 0.5")
     parser_gb.add_argument("-c", "--conventional", action="store_true",
                            help="Get conventional GB, not primitive"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -c")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -c")
     parser_gb.add_argument("-fmt", "--fmt", default="poscar", const="poscar",
                            nargs="?", choices=["poscar", "cif", "cssr", "json"],
                            help="Choose the output format. (default: %(default)s)"
-                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 POSCAR -fmt cif")
+                                "\nEXAMPLE: aimsgb gb 001 5 1 2 0 -f POSCAR -fmt cif")
     parser_gb.set_defaults(func=gb)
 
     args = parser.parse_args()
 
     try:
         getattr(args, "func")
     except AttributeError:
```

### Comparing `aimsgb-0.1.1/aimsgb/grain.py` & `aimsgb-0.1.2/aimsgb/grain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import warnings
 import numpy as np
 from functools import reduce
 from itertools import groupby
+from aimsgb.utils import reduce_vector
 from pymatgen.core.structure import Structure, Lattice, PeriodicSite
+from pymatgen.transformations.advanced_transformations import CubicSupercellTransformation
+from pymatgen.analysis.structure_matcher import StructureMatcher
 
 __author__ = "Jianli CHENG and Kesong YANG"
 __copyright__ = "Copyright 2018 University of California San Diego"
 __maintainer__ = "Jianli CHENG"
 __email__ = "jic198@ucsd.edu"
 __status__ = "Production"
 __date__ = "January 26, 2018"
@@ -33,23 +36,25 @@
         grain_b = grain_a.copy()
         csl_t = csl.transpose()
         if sum(abs(csl_t[0]) - abs(csl_t[1])) > 0:
             axis = (1, 0, 0)
         else:
             axis = (0, 1, 0)
         anchor = grain_b.lattice.get_cartesian_coords(np.array([.0, .0, .0]))
+        # print(axis, anchor)
+        # exit()
         grain_b.rotate_sites(theta=np.radians(180), axis=axis, anchor=anchor)
         return grain_b
 
     def make_supercell(self, scaling_matrix):
         """
         Create a supercell. Very similar to pymatgen's Structure.make_supercell
         However, we need to make sure that all fractional coordinates that equal
         to 1 will become 0 and the lattice are redefined so that x_c = [0, 0, c]
-
+    
         Args:
             scaling_matrix (3x3 matrix): The scaling matrix to make supercell.
         """
         s = self * scaling_matrix
         for i, site in enumerate(s):
             f_coords = np.mod(site.frac_coords, 1)
             # The following for loop is probably not necessary. But I will leave
@@ -159,23 +164,41 @@
         Returns:
             Grain objects for grain A and B
         """
         csl_t = csl.transpose()
         # rotate along a longer axis between a and b
         grain_a = self.copy()
         grain_a.make_supercell(csl_t)
+        # grain_a.to(filename='POSCAR')
+        # exit()
 
         if not all([i == 90 for i in grain_a.lattice.angles]):
-            # warnings.warn("The lattice system of the grain is not orthogonal. "
-            #               "The periodicity of the grain is most likely broken. "
-            #               "We suggest user to build a very big supercell in "
-            #               "order to minimize this effect.")
-            grain_a.set_orthogonal_grain()
+            warnings.warn("The lattice system of the grain is not orthogonal. "
+                          "aimsgb will find a supercell of the grain structure "
+                          "that is orthogonalized. This may take a while. ")
+            cst = CubicSupercellTransformation(force_90_degrees=True,
+                                               min_length=min(grain_a.lattice.abc))
+            _s = grain_a.copy()
+            _s = cst.apply_transformation(_s)
+            _matrix = [reduce_vector(i) for i in cst.transformation_matrix]
+            _s = grain_a.copy()
+            _s.make_supercell(_matrix)
+            sm = StructureMatcher(attempt_supercell=True, primitive_cell=False)
+            _matrix = sm.get_supercell_matrix(_s, self)
+            matrix = [reduce_vector(i) for i in _matrix]
+            grain_a = self.copy()
+            grain_a.make_supercell(matrix)
+            # grain_a.make_supercell(get_sc_fromstruct(grain_a, min_length=min(grain_a.lattice.abc),
+            #                                          force_diagonal=True))
+            # grain_a.make_supercell(get_sc_fromstruct(grain_a).transpose())
+            # grain_a.set_orthogonal_grain()
             # grain_b = grain_b.set_orthogonal_grain()
 
+        # grain_a.to(filename='POSCAR')
+        # exit()
         temp_a = grain_a.copy()
         scale_vector = [1, 1]
         scale_vector.insert(gb_direction, uc_b)
         temp_a.make_supercell(scale_vector)
         grain_b = self.get_b_from_a(temp_a, csl)
         # make sure that all fractional coordinates that equal to 1 will become 0
         grain_b.make_supercell([1, 1, 1])
```

### Comparing `aimsgb-0.1.1/aimsgb/grain_bound.py` & `aimsgb-0.1.2/aimsgb/grain_bound.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from fractions import Fraction
 from math import sqrt, atan, degrees, pi
 import numpy as np
 from numpy import sin, cos, ceil, radians, inner, identity
 from numpy.linalg import inv, det, norm, solve
 from pymatgen.core.lattice import Lattice
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-
 from aimsgb import Grain
 from aimsgb.utils import reduce_vector, co_prime, plus_minus_gen, \
     is_integer, get_smallest_multiplier, reduce_integer, transpose_matrix
 
 __author__ = "Jianli Cheng, Kesong Yang"
 __copyright__ = "Copyright 2018, Yanggroup"
 __maintainer__ = "Jianli Cheng"
@@ -457,22 +456,17 @@
             sigma = reduce_sigma
         self.sigma = sigma
         self.gb_info = GBInformation(self.axis, self.sigma, specific=True)
         self.gb_direction = None
         for i, v in enumerate(self.csl.transpose()):
             if self.plane == list(v):
                 self.gb_direction = i
-        abc = initial_struct.lattice.abc
-        if abc[0] != abc[1] or \
-                any([i != 90 for i in initial_struct.lattice.angles]):
-            warnings.warn("Your input structure is not a conventional standard "
-                          "structure. aimsgb will do the transformation for you.")
-            sg = SpacegroupAnalyzer(initial_struct)
-            new_s = sg.get_conventional_standard_structure()
-            initial_struct = Grain.from_sites(new_s[:])
+        sg = SpacegroupAnalyzer(initial_struct)
+        new_s = sg.get_conventional_standard_structure()
+        initial_struct = Grain.from_sites(new_s[:])
         self._grain_a, self._grain_b = initial_struct.build_grains(
             self.csl, self.gb_direction, uc_a, uc_b)
 
     @property
     def rot_matrix(self):
         """
         Rotation matrix for calculating CSL matrix
```

### Comparing `aimsgb-0.1.1/aimsgb/utils.py` & `aimsgb-0.1.2/aimsgb/utils.py`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.1/aimsgb.egg-info/PKG-INFO` & `aimsgb-0.1.2/aimsgb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,96 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: aimsgb
-Version: 0.1.1
+Version: 0.1.2
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
-Maintainer-email: jic198@ucsd.edu, sij014@ucsd.edu, kesong@ucsd.edu
-License: UNKNOWN
-Description: 
-        Introduction
-        ============
-        aimsgb, an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
-        construct various grain boundary structures from cubic and non-cubic initial
-        configurations. A convenient command line tool has also been provided to enable
-        easy and fast construction of tilt and twist boundaries by assigining the degree
-        of fit (Σ), rotation axis, grain boundary plane and initial crystal structure.
-        aimsgb is expected to greatly accelerate the theoretical investigation of
-        grain boundary properties and facilitate the experimental analysis of grain
-        boundary structures as well.
-        
-        A reference for the usage of aimsGB software is:
-        Jianli Cheng, Jian Luo, and Kesong Yang, Aimsgb: An Algorithm and OPen-Source Python Library to Generate Periodic Grain Boundary Structures, Comput. Mater. Sci. 155, 92-103, (2018). 
-        DOI:10.1016/j.commatsci.2018.08.029  
-        
-        Install aimsgb
-        ==============
-        1. Clone the latest version from github::
-        
-            git clone git@github.com:ksyang2013/aimsgb.git
-        
-        2. Navigate to aimsgb folder::
-        
-            cd aimsgb
-        
-        3. Type in the root of the repo::
-        
-            pip install .
-        
-        4. or to install the package in development mode::
-        
-            pip install -e .
-        
-        
-        How to cite aimsgb
-        ==================
-        
-        If you use aimsgb in your research, please consider citing the following work:
-        
-            Jianli Cheng, Jian Luo, Kesong Yang. *Aimsgb: An algorithm and open-source python
-            library to generate periodic grain boundary structures.* Computational Materials
-            Science, 2018, 155, 92-103. `doi:10.1016/j.commatsci.2018.08.029
-            <https://doi.org/10.1016/j.commatsci.2018.08.029>`_
-        
-        
-        Copyright
-        =========
-        Copyright (C) 2018 The Regents of the University of California
-        
-        All Rights Reserved. Permission to copy, modify, and distribute this software and its documentation for educational, research and non-profit purposes, without fee, and without a written agreement is hereby granted, provided that the above copyright notice, this paragraph and the following three paragraphs appear in all copies. Permission to make commercial use of this software may be obtained by contacting:
-        
-        Office of Innovation and Commercialization
-        9500 Gilman Drive, Mail Code 0910
-        University of California
-        La Jolla, CA 92093-0910
-        (858) 534-5815
-        innovation@ucsd.edu
-        
-        This software program and documentation are copyrighted by The Regents of the University of California. The software program and documentation are supplied “as is”, without any accompanying services from The Regents. The Regents does not warrant that the operation of the program will be uninterrupted or error-free. The end-user understands that the program was developed for research purposes and is advised not to rely exclusively on the program for any reason.
-        
-        IN NO EVENT SHALL THE UNIVERSITY OF CALIFORNIA BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF THE UNIVERSITY OF CALIFORNIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. THE UNIVERSITY OF CALIFORNIA SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN “AS IS” BASIS, AND THE UNIVERSITY OF CALIFORNIA HAS NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
-        
-        
-        Authors
-        =======
-        Dr. Jianli Cheng (jic198@ucsd.edu)
-        New Email: jianlicheng@lbl.gov
-        
-        Prof. Kesong Yang  (kesong@ucsd.edu)
-        
-        About the aimsgb Development Team
-        =================================
-        http://materials.ucsd.edu/
-        
+Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE.txt
+
+
+Introduction
+============
+aimsgb, an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
+construct various grain boundary structures from cubic and non-cubic initial
+configurations. A convenient command line tool has also been provided to enable
+easy and fast construction of tilt and twist boundaries by assigining the degree
+of fit (Σ), rotation axis, grain boundary plane and initial crystal structure.
+aimsgb is expected to greatly accelerate the theoretical investigation of
+grain boundary properties and facilitate the experimental analysis of grain
+boundary structures as well.
+
+A reference for the usage of aimsGB software is:
+Jianli Cheng, Jian Luo, and Kesong Yang, Aimsgb: An Algorithm and OPen-Source Python Library to Generate Periodic Grain Boundary Structures, Comput. Mater. Sci. 155, 92-103, (2018). 
+DOI:10.1016/j.commatsci.2018.08.029  
+
+Install aimsgb
+==============
+1. Clone the latest version from github::
+
+    git clone git@github.com:ksyang2013/aimsgb.git
+
+2. Navigate to aimsgb folder::
+
+    cd aimsgb
+
+3. Type in the root of the repo::
+
+    pip install .
+
+4. or to install the package in development mode::
+
+    pip install -e .
+
+
+How to cite aimsgb
+==================
+
+If you use aimsgb in your research, please consider citing the following work:
+
+    Jianli Cheng, Jian Luo, Kesong Yang. *Aimsgb: An algorithm and open-source python
+    library to generate periodic grain boundary structures.* Computational Materials
+    Science, 2018, 155, 92-103. `doi:10.1016/j.commatsci.2018.08.029
+    <https://doi.org/10.1016/j.commatsci.2018.08.029>`_
+
+
+Copyright
+=========
+Copyright (C) 2018 The Regents of the University of California
+
+All Rights Reserved. Permission to copy, modify, and distribute this software and its documentation for educational, research and non-profit purposes, without fee, and without a written agreement is hereby granted, provided that the above copyright notice, this paragraph and the following three paragraphs appear in all copies. Permission to make commercial use of this software may be obtained by contacting:
+
+Office of Innovation and Commercialization
+9500 Gilman Drive, Mail Code 0910
+University of California
+La Jolla, CA 92093-0910
+(858) 534-5815
+innovation@ucsd.edu
+
+This software program and documentation are copyrighted by The Regents of the University of California. The software program and documentation are supplied “as is”, without any accompanying services from The Regents. The Regents does not warrant that the operation of the program will be uninterrupted or error-free. The end-user understands that the program was developed for research purposes and is advised not to rely exclusively on the program for any reason.
+
+IN NO EVENT SHALL THE UNIVERSITY OF CALIFORNIA BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF THE UNIVERSITY OF CALIFORNIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. THE UNIVERSITY OF CALIFORNIA SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN “AS IS” BASIS, AND THE UNIVERSITY OF CALIFORNIA HAS NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
+
+
+Authors
+=======
+Dr. Jianli Cheng (jic198@ucsd.edu)
+New Email: jianlicheng@lbl.gov
+
+Prof. Kesong Yang  (kesong@ucsd.edu)
+
+About the aimsgb Development Team
+=================================
+http://materials.ucsd.edu/
```

### Comparing `aimsgb-0.1.1/setup.py` & `aimsgb-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,21 +76,21 @@
 =================================
 http://materials.ucsd.edu/
 """
 
 setup(
     name="aimsgb",
     packages=find_packages(),
-    version="0.1.1",
+    version="0.1.2",
     setup_requires=["setuptools>=18.0"],
-    install_requires=["pymatgen"],
+    install_requires=["pymatgen", "mp_api", "numpy"],
     include_package_data=True,
     author="Jianli Cheng and Kesong YANG",
     maintainer="Jianli Cheng, Sicong JIANG, and Kesong YANG",
-    maintainer_email="jic198@ucsd.edu, sij014@ucsd.edu, kesong@ucsd.edu",
+    maintainer_email="chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu",
     url="http://aimsgb.org",
     description="aimsgb is a python library for generatng the atomic "
                 "coordinates of periodic grain boundaries."
                 "Copyright © 2018 The Regents of the University of California."
                 "All Rights Reserved. See more in Copyright.",
     long_description=long_desc,
     keywords=["material science", "grain boundary", "molecular simulation"],
```

