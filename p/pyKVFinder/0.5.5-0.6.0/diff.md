# Comparing `tmp/pyKVFinder-0.5.5.tar.gz` & `tmp/pyKVFinder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKVFinder-0.5.5.tar", last modified: Wed Apr 26 19:51:03 2023, max compression
+gzip compressed data, was "pyKVFinder-0.6.0.tar", last modified: Fri May 12 19:53:35 2023, max compression
```

## Comparing `pyKVFinder-0.5.5.tar` & `pyKVFinder-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.348171 pyKVFinder-0.5.5/C/
--rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    81497 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/pyKVFinder.c
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/pyKVFinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/pyKVFinder.i
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.348171 pyKVFinder-0.5.5/pyKVFinder/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/pyKVFinder/data/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/EisenbergWeiss.toml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/HessaHeijne.toml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/KyteDoolittle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/MoonFleming.toml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/RadzickaWolfenden.toml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/WimleyWhite.toml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/ZhaoLondon.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/pyKVFinder/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/ClO4.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/PKI.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/custom-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/residues-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/vdw.dat
--rw-r--r--   0 runner    (1001) docker     (123)   110025 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    72142 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    64069 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.348171 pyKVFinder-0.5.5/pyKVFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.117694 pyKVFinder-0.6.0/C/
+-rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/pyKVFinder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/pyKVFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/pyKVFinder.i
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.121694 pyKVFinder-0.6.0/pyKVFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.121694 pyKVFinder-0.6.0/pyKVFinder/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/EisenbergWeiss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/HessaHeijne.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/KyteDoolittle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/MoonFleming.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/RadzickaWolfenden.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/WimleyWhite.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/ZhaoLondon.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/pyKVFinder/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/ClO4.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/PKI.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/custom-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/residues-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/vdw.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.121694 pyKVFinder-0.6.0/pyKVFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/setup.py
```

### Comparing `pyKVFinder-0.5.5/C/numpy.i` & `pyKVFinder-0.6.0/C/numpy.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/C/pyKVFinder.c` & `pyKVFinder-0.6.0/C/pyKVFinder.c`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
  *
  * Fill integer grid with 1
  *
  * grid: empty 3D grid
  * size: number of voxels
  *
  */
-void igrid(int *grid, int size) {
+void igrid(int *grid, int size)
+{
   int i;
 
   for (i = 0; i < size; i++)
     grid[i] = 1;
 }
 
 /*
@@ -41,15 +42,16 @@
  *
  * Fill float grid with 0.0
  *
  * grid: empty 3D grid
  * size: number of voxels
  *
  */
-void fgrid(float *grid, int size) {
+void fgrid(float *grid, int size)
+{
   int i;
 
   for (i = 0; i < size; i++)
     grid[i] = 0.0;
 }
 
 /*
@@ -58,15 +60,16 @@
  *
  * Fill double grid with 0.0
  *
  * grid: empty 3D grid
  * size: number of voxels
  *
  */
-void dgrid(double *grid, int size) {
+void dgrid(double *grid, int size)
+{
   int i;
 
   for (i = 0; i < size; i++)
     grid[i] = 0.0;
 }
 
 /*
@@ -75,15 +78,16 @@
  *
  * Fill char grid with '\0'
  *
  * grid: empty 3D grid
  * size: number of voxels
  *
  */
-void cgrid(int *grid, int size) {
+void cgrid(int *grid, int size)
+{
   int i;
 
   for (i = 0; i < size; i++)
     grid[i] = '\0';
 }
 
 /* Grid filling */
@@ -108,29 +112,31 @@
  * step: 3D grid spacing (A)
  * probe: Probe size (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void fill(int *grid, int nx, int ny, int nz, double *atoms, int natoms,
           int xyzr, double *reference, int ndims, double *sincos, int nvalues,
-          double step, double probe, int nthreads) {
+          double step, double probe, int nthreads)
+{
   int i, j, k, atom;
   double x, y, z, xaux, yaux, zaux, distance, H;
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none),                                            \
-    shared(grid, reference, step, probe, natoms, nx, ny, nz, sincos, atoms,    \
-           nthreads),                                                          \
+#pragma omp parallel default(none),                                         \
+    shared(grid, reference, step, probe, natoms, nx, ny, nz, sincos, atoms, \
+           nthreads),                                                       \
     private(atom, i, j, k, distance, H, x, y, z, xaux, yaux, zaux)
   {
 #pragma omp for schedule(dynamic) // nowait
-    for (atom = 0; atom < natoms; atom++) {
+    for (atom = 0; atom < natoms; atom++)
+    {
       // Convert atom coordinates in 3D grid coordinates
       x = (atoms[atom * 4] - reference[0]) / step;
       y = (atoms[1 + (atom * 4)] - reference[1]) / step;
       z = (atoms[2 + (atom * 4)] - reference[2]) / step;
 
       xaux = x * sincos[3] + z * sincos[2];
       yaux = y;
@@ -142,15 +148,16 @@
 
       // Create a radius (H) for space occupied by probe and atom
       H = (probe + atoms[3 + (atom * 4)]) / step;
 
       // Loop around radius from atom center
       for (i = floor(x - H); i <= ceil(x + H); i++)
         for (j = floor(y - H); j <= ceil(y + H); j++)
-          for (k = floor(z - H); k <= ceil(z + H); k++) {
+          for (k = floor(z - H); k <= ceil(z + H); k++)
+          {
             // Get distance between atom center and point inspected
             distance = sqrt(pow(i - x, 2) + pow(j - y, 2) + pow(k - z, 2));
             if (distance < H)
               if (i >= 0 && i < nx && j >= 0 && j < ny && k >= 0 && k < nz)
                 grid[k + nz * (j + (ny * i))] = 0;
           }
     }
@@ -177,29 +184,31 @@
  * step: 3D grid spacing (A)
  * probe: Probe size (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void _fill_cavity(int *cavities, int nx, int ny, int nz, double *atoms,
                   int natoms, int xyzr, double *reference, int ndims,
-                  double *sincos, int nvalues, double step, int nthreads) {
+                  double *sincos, int nvalues, double step, int nthreads)
+{
   int i, j, k, atom;
   double x, y, z, xaux, yaux, zaux;
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none),                                            \
-    shared(cavities, reference, step, natoms, nx, ny, nz, sincos, atoms,       \
-           nthreads),                                                          \
+#pragma omp parallel default(none),                                      \
+    shared(cavities, reference, step, natoms, nx, ny, nz, sincos, atoms, \
+           nthreads),                                                    \
     private(atom, i, j, k, x, y, z, xaux, yaux, zaux)
   {
 #pragma omp for schedule(dynamic) // nowait
-    for (atom = 0; atom < natoms; atom++) {
+    for (atom = 0; atom < natoms; atom++)
+    {
       // Convert atom coordinates in 3D grid coordinates
       x = (atoms[atom * 4] - reference[0]) / step;
       y = (atoms[1 + (atom * 4)] - reference[1]) / step;
       z = (atoms[2 + (atom * 4)] - reference[2]) / step;
 
       xaux = x * sincos[3] + z * sincos[2];
       yaux = y;
@@ -209,15 +218,15 @@
       j = (int)(yaux * sincos[1] - zaux * sincos[0]);
       k = (int)(yaux * sincos[0] + zaux * sincos[1]);
 
       cavities[k + nz * (j + (ny * i))] = (int)(atoms[3 + (atom * 4)]);
     }
   }
 
-#pragma omp parallel default(none), shared(cavities, nx, ny, nz),              \
+#pragma omp parallel default(none), shared(cavities, nx, ny, nz), \
     private(i, j, k)
   {
 #pragma omp for collapse(3) ordered
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
           if (cavities[k + nz * (j + (ny * i))] == 1)
@@ -248,27 +257,29 @@
  * nthreads: number of threads for OpenMP
  * verbose: print extra information to standard output
  *
  */
 void _fill_receptor(int *receptor, int size, int nx, int ny, int nz,
                     double *atoms, int natoms, int xyzr, double *reference,
                     int ndims, double *sincos, int nvalues, double step,
-                    double probe_in, int is_ses, int nthreads, int verbose) {
+                    double probe_in, int is_ses, int nthreads, int verbose)
+{
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
   if (verbose)
     fprintf(stdout, "> Creating a SAS representation of the receptor\n");
   igrid(receptor, size);
   fill(receptor, nx, ny, nz, atoms, natoms, xyzr, reference, ndims, sincos,
        nvalues, step, probe_in, nthreads);
 
-  if (is_ses) {
+  if (is_ses)
+  {
     if (verbose)
       fprintf(stdout, "> Adjusting a SES representation of the receptor\n");
     ses(receptor, nx, ny, nz, step, probe_in, nthreads);
   }
 }
 
 /* Biomolecular surface representation */
@@ -286,21 +297,23 @@
  * i: x coordinate of cavity point
  * j: y coordinate of cavity point
  * k: z coordinate of cavity point
  *
  * returns: true (int 1) or false (int 0)
  */
 int check_protein_neighbours(int *grid, int nx, int ny, int nz, int i, int j,
-                             int k) {
+                             int k)
+{
   int x, y, z;
 
   // Loop around neighboring points
   for (x = i - 1; x <= i + 1; x++)
     for (y = j - 1; y <= j + 1; y++)
-      for (z = k - 1; z <= k + 1; z++) {
+      for (z = k - 1; z <= k + 1; z++)
+      {
         // Check if point is inside 3D grid
         if (x < 0 || y < 0 || z < 0 || x > nx - 1 || y > ny - 1 || z > nz - 1)
           ;
         else if (grid[z + nz * (y + (ny * x))] == 0 ||
                  grid[z + nz * (y + (ny * x))] == -2)
           return 1;
       }
@@ -319,43 +332,48 @@
  * nz: z grid units
  * step: 3D grid spacing (A)
  * probe: Probe size (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void ses(int *grid, int nx, int ny, int nz, double step, double probe,
-         int nthreads) {
+         int nthreads)
+{
   int i, j, k, i2, j2, k2, aux;
   double distance;
 
   // Calculate sas limit in 3D grid units
   aux = ceil(probe / step);
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none),                                            \
-    shared(grid, step, probe, aux, nx, ny, nz),                                \
+#pragma omp parallel default(none),             \
+    shared(grid, step, probe, aux, nx, ny, nz), \
     private(i, j, k, i2, j2, k2, distance)
   {
 #pragma omp for schedule(dynamic) collapse(3) // nowait
     // Loop around 3D grid
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
-        for (k = 0; k < nz; k++) {
+        for (k = 0; k < nz; k++)
+        {
           // Check if a cavity point
           if (grid[k + nz * (j + (ny * i))] == 1)
-            if (check_protein_neighbours(grid, nx, ny, nz, i, j, k)) {
+            if (check_protein_neighbours(grid, nx, ny, nz, i, j, k))
+            {
               // Loop around sas limit from cavity point next to protein point
               for (i2 = i - aux; i2 <= i + aux; i2++)
                 for (j2 = j - aux; j2 <= j + aux; j2++)
-                  for (k2 = k - aux; k2 <= k + aux; k2++) {
+                  for (k2 = k - aux; k2 <= k + aux; k2++)
+                  {
                     if (i2 > 0 && j2 > 0 && k2 > 0 && i2 < nx && j2 < ny &&
-                        k2 < nz) {
+                        k2 < nz)
+                    {
                       // Get distance between point inspected and cavity point
                       distance = sqrt(pow(i - i2, 2) + pow(j - j2, 2) +
                                       pow(k - k2, 2));
                       // Check if inspected point is inside sas limit
                       if (distance < (probe / step))
                         if (grid[k2 + nz * (j2 + (ny * i2))] == 0)
                           // Mark cavity point
@@ -365,15 +383,16 @@
             }
         }
 
 #pragma omp for collapse(3)
     // Loop around 3D grid
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
-        for (k = 0; k < nz; k++) {
+        for (k = 0; k < nz; k++)
+        {
           // Mark space occupied by sas limit from protein surface
           if (grid[k + nz * (j + (ny * i))] == -2)
             grid[k + nz * (j + (ny * i))] = 1;
         }
   }
 }
 
@@ -392,35 +411,38 @@
  * nz: z grid units
  * step: 3D grid spacing (A)
  * removal_distance: Length to be removed from the cavity-bulk frontier (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void subtract(int *PI, int *PO, int nx, int ny, int nz, double step,
-              double removal_distance, int nthreads) {
+              double removal_distance, int nthreads)
+{
   int i, j, k, i2, j2, k2, rd;
 
   rd = ceil(removal_distance / step);
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
 // Create a parallel region */
-#pragma omp parallel default(none),                                            \
-    shared(PI, PO, nx, ny, nz, i, j, k, step, rd, removal_distance),           \
+#pragma omp parallel default(none),                                  \
+    shared(PI, PO, nx, ny, nz, i, j, k, step, rd, removal_distance), \
     private(j2, i2, k2)
   {
 #pragma omp for schedule(dynamic) collapse(3)
     // Loop around the search box
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
-        for (k = 0; k < nz; k++) {
+        for (k = 0; k < nz; k++)
+        {
           // Check if point is a cavity point in grid filled with PO
-          if (PO[k + nz * (j + (ny * i))]) {
+          if (PO[k + nz * (j + (ny * i))])
+          {
             // Loops around space occupied by probe from atom position
             for (i2 = i - rd; i2 <= i + rd; i2++)
               for (j2 = j - rd; j2 <= j + rd; j2++)
                 for (k2 = k - rd; k2 <= k + rd; k2++)
                   // Check if inside 3D grid
                   if (i2 >= 0 && i2 < nx && j2 >= 0 && j2 < ny && k2 >= 0 &&
                       k2 < nz)
@@ -445,27 +467,31 @@
  * grid: cavities 3D grid
  * nx: x grid units
  * ny: y grid units
  * nz: z grid units
  * nthreads: number of threads for OpenMP
  *
  */
-void filter_noise(int *grid, int nx, int ny, int nz, int nthreads) {
+void filter_noise(int *grid, int nx, int ny, int nz, int nthreads)
+{
   int i, j, k, contacts;
 
   for (i = 0; i < nx; i++)
     for (j = 0; j < ny; j++)
-      for (k = 0; k < nz; k++) {
-        if (grid[k + nz * (j + (ny * i))] == 1) {
+      for (k = 0; k < nz; k++)
+      {
+        if (grid[k + nz * (j + (ny * i))] == 1)
+        {
           contacts = 0;
 
           // Check if a protein point (0) or a medium point (-1) is next to a
           // cavity point (==1)
           if (i - 1 >= 0 && i + 1 < nx && j - 1 >= 0 && j + 1 < ny &&
-              k - 1 >= 0 && k + 1 < nz) {
+              k - 1 >= 0 && k + 1 < nz)
+          {
             if (grid[k + nz * (j + (ny * (i - 1)))] == 0 ||
                 grid[k + nz * (j + (ny * (i - 1)))] == -1)
               contacts++;
             if (grid[k + nz * (j + (ny * (i + 1)))] == 0 ||
                 grid[k + nz * (j + (ny * (i + 1)))] == -1)
               contacts++;
             if (grid[k + nz * ((j - 1) + (ny * i))] == 0 ||
@@ -511,33 +537,36 @@
  * step: 3D grid spacing (A)
  * ligand_cutoff: Radius value to limit a space around a ligand (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void adjust(int *grid, int nx, int ny, int nz, double *ligand, int lnatoms,
             int lxyzr, double *reference, int ndims, double *sincos,
-            int nvalues, double step, double ligand_cutoff, int nthreads) {
+            int nvalues, double step, double ligand_cutoff, int nthreads)
+{
   int i, j, k, atom, inside;
   double x, y, z, xaux, yaux, zaux, distance;
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none),                                            \
-    shared(grid, nx, ny, nz, step, sincos, reference, ligand, ligand_cutoff,   \
-           lnatoms),                                                           \
+#pragma omp parallel default(none),                                          \
+    shared(grid, nx, ny, nz, step, sincos, reference, ligand, ligand_cutoff, \
+           lnatoms),                                                         \
     private(inside, i, j, k, x, y, z, xaux, yaux, zaux, atom, distance)
   {
 #pragma omp for collapse(3) schedule(static) nowait
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
-        for (k = 0; k < nz; k++) {
+        for (k = 0; k < nz; k++)
+        {
           inside = 0;
-          for (atom = 0; atom < lnatoms; atom++) {
+          for (atom = 0; atom < lnatoms; atom++)
+          {
             // Get 3D grid point coordinate
             x = i * step;
             y = j * step;
             z = k * step;
 
             xaux = (x * sincos[3]) + (y * sincos[0] * sincos[2]) -
                    (z * sincos[1] * sincos[2]) + reference[0];
@@ -580,27 +609,29 @@
  * step: 3D grid spacing (A)
  * probe_in: Probe In size (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void _filter_pdb(int nx, int ny, int nz, double *atoms, int natoms, int xyzr,
                  double *reference, int ndims, double *sincos, int nvalues,
-                 double step, double probe_in, int nthreads) {
+                 double step, double probe_in, int nthreads)
+{
   int atom;
   double x, y, z, xaux, yaux, zaux;
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
 
-#pragma omp parallel default(none),                                            \
-    shared(atoms, natoms, reference, sincos, step, probe_in, nx, ny, nz),      \
+#pragma omp parallel default(none),                                       \
+    shared(atoms, natoms, reference, sincos, step, probe_in, nx, ny, nz), \
     private(atom, x, y, z, xaux, yaux, zaux)
   {
 #pragma omp for schedule(static) // nowait
-    for (atom = 0; atom < natoms; atom++) {
+    for (atom = 0; atom < natoms; atom++)
+    {
       x = (atoms[atom * 4] - reference[0]) / step;
       y = (atoms[1 + (atom * 4)] - reference[1]) / step;
       z = (atoms[2 + (atom * 4)] - reference[2]) / step;
 
       xaux = x * sincos[3] + z * sincos[2];
       yaux = y;
       zaux = (-x) * sincos[2] + z * sincos[3];
@@ -612,15 +643,16 @@
       if (x > 0.0 - (probe_in + atoms[3 + (atom * 4)]) / step &&
           x < (double)nx + (probe_in + atoms[3 + (atom * 4)]) / step &&
           y > 0.0 - (probe_in + atoms[3 + (atom * 4)]) / step &&
           y < (double)ny + (probe_in + atoms[3 + (atom * 4)]) / step &&
           z > 0.0 - (probe_in + atoms[3 + (atom * 4)]) / step &&
           z < (double)nz + (probe_in + atoms[3 + (atom * 4)]) / step)
         ;
-      else {
+      else
+      {
         atoms[atom * 4] = 0.0;
         atoms[1 + (atom * 4)] = 0.0;
         atoms[2 + (atom * 4)] = 0.0;
         atoms[3 + (atom * 4)] = 0.0;
       }
     }
   }
@@ -645,15 +677,16 @@
  * step: 3D grid spacing (A)
  * probe_out: Radius value to limit a space around a ligand (A)
  * nthreads: number of threads for OpenMP
  *
  */
 void filter(int *grid, int nx, int ny, int nz, double *P1, int ndims,
             double *P2, int nndims, double *sincos, int nvalues, double step,
-            double probe_out, int nthreads) {
+            double probe_out, int nthreads)
+{
   int i, j, k;
   double aux, normB, norm1, X1, Y1, Z1, X2, Y2, Z2;
 
   // Set number of processes in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
@@ -757,21 +790,23 @@
  * i: x coordinate of cavity point
  * j: y coordinate of cavity point
  * k: z coordinate of cavity point
  *
  * returns: true (int 1) or false (int 0)
  */
 int check_unclustered_neighbours(int *grid, int nx, int ny, int nz, int i,
-                                 int j, int k) {
+                                 int j, int k)
+{
   int x, y, z;
 
   // Loop around neighboring points
   for (x = i - 1; x <= i + 1; x++)
     for (y = j - 1; y <= j + 1; y++)
-      for (z = k - 1; z <= k + 1; z++) {
+      for (z = k - 1; z <= k + 1; z++)
+      {
         // Check if point is inside 3D grid
         if (x < 0 || y < 0 || z < 0 || x > nx - 1 || y > ny - 1 || z > nz - 1)
           ;
         else if (grid[z + nz * (y + (ny * x))] > 1)
           return grid[z + nz * (y + (ny * x))];
       }
   return 0;
@@ -789,28 +824,31 @@
  * nz: z grid units
  * i: x coordinate of cavity point
  * j: y coordinate of cavity point
  * k: z coordinate of cavity point
  * tag: cavity integer identifier
  *
  */
-void DFS(int *grid, int nx, int ny, int nz, int i, int j, int k, int tag) {
+void DFS(int *grid, int nx, int ny, int nz, int i, int j, int k, int tag)
+{
   int x, y, z;
 
   if (i == 0 || i == nx - 1 || j == 0 || j == ny - 1 || k == 0 || k == nz - 1)
     return;
 
-  if (grid[k + nz * (j + (ny * i))] == 1 && !big) {
+  if (grid[k + nz * (j + (ny * i))] == 1 && !big)
+  {
     grid[k + nz * (j + (ny * i))] = tag;
     vol++;
 
     if (vol == 10000)
       big = 1;
 
-    if (!big) {
+    if (!big)
+    {
       for (x = i - 1; x <= i + 1; x++)
         for (y = j - 1; y <= j + 1; y++)
           for (z = k - 1; z <= k + 1; z++)
             DFS(grid, nx, ny, nz, x, y, z, tag);
     }
   }
 }
@@ -825,15 +863,16 @@
  * nx: x grid units
  * ny: y grid units
  * nz: z grid units
  * tag: cavity integer identifier
  * nthreads: number of threads for OpenMP
  *
  */
-void remove_cavity(int *grid, int nx, int ny, int nz, int tag, int nthreads) {
+void remove_cavity(int *grid, int nx, int ny, int nz, int tag, int nthreads)
+{
   int i, j, k;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
 #pragma omp parallel default(shared)
@@ -858,53 +897,58 @@
  * nz: z grid units
  * step: 3D grid spacing (A)
  * volume_cutoff: Cavities volume filter (A3)
  * nthreads: number of threads for OpenMP
  *
  */
 int _cluster(int *grid, int nx, int ny, int nz, double step,
-             double volume_cutoff, int nthreads) {
+             double volume_cutoff, int nthreads)
+{
   int i, j, k, i2, j2, k2, tag, vol_aux;
 
   // Initialize variables
   tag = 1;
   vol_aux = 0;
   big = 0;
 
   for (i = 0; i < nx; i++)
     for (j = 0; j < ny; j++)
       for (k = 0; k < nz; k++)
-        if (grid[k + nz * (j + (ny * i))] == 1) {
+        if (grid[k + nz * (j + (ny * i))] == 1)
+        {
           tag++;
           vol = 0;
 
           // Clustering procedure
           DFS(grid, nx, ny, nz, i, j, k, tag);
           vol_aux = vol;
 
           // Loop for big cavities
-          while (big) {
+          while (big)
+          {
             vol_aux = 0;
 
             for (i2 = 0; i2 < nx; i2++)
               for (j2 = 0; j2 < ny; j2++)
-                for (k2 = 0; k2 < nz; k2++) {
+                for (k2 = 0; k2 < nz; k2++)
+                {
                   big = 0;
                   vol_aux += vol;
                   vol = 0;
                   if (grid[k2 + nz * (j2 + (ny * i2))] == 1 &&
                       check_unclustered_neighbours(grid, nx, ny, nz, i2, j2,
                                                    k2) == tag)
                     DFS(grid, nx, ny, nz, i2, j2, k2, tag);
                 }
           }
           vol = vol_aux;
 
           // Check if cavity reached cutoff
-          if ((double)vol * pow(step, 3) < volume_cutoff) {
+          if ((double)vol * pow(step, 3) < volume_cutoff)
+          {
             remove_cavity(grid, nx, ny, nz, tag, nthreads);
             tag--;
           }
         }
   return tag - 1;
 }
 
@@ -942,15 +986,16 @@
  *
  * returns: PI[size] (cavities 3D grid) and ncav (number of cavities)
  */
 int _detect(int *PI, int size, int nx, int ny, int nz, double *atoms,
             int natoms, int xyzr, double *reference, int ndims, double *sincos,
             int nvalues, double step, double probe_in, double probe_out,
             double removal_distance, double volume_cutoff, int box_adjustment,
-            double *P2, int nndims, int is_ses, int nthreads, int verbose) {
+            double *P2, int nndims, int is_ses, int nthreads, int verbose)
+{
   int *PO, ncav;
 
   if (verbose)
     fprintf(stdout, "> Filling grid with Probe In\n");
   igrid(PI, size);
   fill(PI, nx, ny, nz, atoms, natoms, xyzr, reference, ndims, sincos, nvalues,
        step, probe_in, nthreads);
@@ -966,15 +1011,16 @@
     ses(PI, nx, ny, nz, step, probe_in, nthreads);
   ses(PO, nx, ny, nz, step, probe_out, nthreads);
 
   if (verbose)
     fprintf(stdout, "> Defining biomolecular cavities\n");
   subtract(PI, PO, nx, ny, nz, step, removal_distance, nthreads);
 
-  if (box_adjustment) {
+  if (box_adjustment)
+  {
     if (verbose)
       fprintf(stdout, "> Adjusting biomolecular cavities to box\n");
     filter(PI, nx, ny, nz, reference, ndims, P2, nndims, sincos, nvalues, step,
            probe_out, nthreads);
   }
 
   filter_noise(PI, nx, ny, nz, nthreads);
@@ -1029,15 +1075,16 @@
 int _detect_ladj(int *PI, int size, int nx, int ny, int nz, double *atoms,
                  int natoms, int xyzr, double *ligand, int lnatoms, int lxyzr,
                  double *reference, int ndims, double *sincos, int nvalues,
                  double step, double probe_in, double probe_out,
                  double removal_distance, double volume_cutoff,
                  int ligand_adjustment, double ligand_cutoff,
                  int box_adjustment, double *P2, int nndims, int is_ses,
-                 int nthreads, int verbose) {
+                 int nthreads, int verbose)
+{
   int *PO, ncav;
 
   if (verbose)
     fprintf(stdout, "> Filling grid with Probe In\n");
   igrid(PI, size);
   fill(PI, nx, ny, nz, atoms, natoms, xyzr, reference, ndims, sincos, nvalues,
        step, probe_in, nthreads);
@@ -1053,22 +1100,24 @@
     ses(PI, nx, ny, nz, step, probe_in, nthreads);
   ses(PO, nx, ny, nz, step, probe_out, nthreads);
 
   if (verbose)
     fprintf(stdout, "> Defining biomolecular cavities\n");
   subtract(PI, PO, nx, ny, nz, step, removal_distance, nthreads);
 
-  if (ligand_adjustment) {
+  if (ligand_adjustment)
+  {
     if (verbose)
       fprintf(stdout, "> Adjusting biomolecular cavities to ligand\n");
     adjust(PI, nx, ny, nz, ligand, lnatoms, lxyzr, reference, ndims, sincos,
            nvalues, step, ligand_cutoff, nthreads);
   }
 
-  if (box_adjustment) {
+  if (box_adjustment)
+  {
     if (verbose)
       fprintf(stdout, "> Adjusting biomolecular cavities to box\n");
     filter(PI, nx, ny, nz, reference, ndims, P2, nndims, sincos, nvalues, step,
            probe_out, nthreads);
   }
 
   filter_noise(PI, nx, ny, nz, nthreads);
@@ -1098,15 +1147,16 @@
  * i: x coordinate of cavity point
  * j: y coordinate of cavity point
  * k: z coordinate of cavity point
  *
  * returns: cavity identifier (>1) or medium point (-1)
  */
 int define_surface_points(int *cavities, int nx, int ny, int nz, int i, int j,
-                          int k) {
+                          int k)
+{
   if (i - 1 >= 0)
     if (cavities[k + nz * (j + (ny * (i - 1)))] == 0)
       return cavities[k + nz * (j + (ny * i))];
   if (i + 1 < nx)
     if (cavities[k + nz * (j + (ny * (i + 1)))] == 0)
       return cavities[k + nz * (j + (ny * i))];
   if (j - 1 >= 0)
@@ -1137,33 +1187,37 @@
  * nx: x grid units
  * ny: y grid units
  * nz: z grid units
  * nthreads: number of threads for OpenMP
  *
  */
 void filter_surface(int *cavities, int *surface, int nx, int ny, int nz,
-                    int nthreads) {
+                    int nthreads)
+{
   int i, j, k;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none), shared(cavities, surface, nx, ny, nz),     \
+#pragma omp parallel default(none), shared(cavities, surface, nx, ny, nz), \
     private(i, j, k)
   {
 #pragma omp for collapse(3) schedule(static)
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
-          if (cavities[k + nz * (j + (ny * i))] > 1) {
+          if (cavities[k + nz * (j + (ny * i))] > 1)
+          {
             // Define surface cavity points
             surface[k + nz * (j + (ny * i))] =
                 define_surface_points(cavities, nx, ny, nz, i, j, k);
-          } else {
+          }
+          else
+          {
             if (cavities[k + nz * (j + (ny * i))] == 0)
               surface[k + nz * (j + (ny * i))] = 0;
             else
               surface[k + nz * (j + (ny * i))] = -1;
           }
   }
 }
@@ -1183,15 +1237,16 @@
  * i: x coordinate of cavity point
  * j: y coordinate of cavity point
  * k: z coordinate of cavity point
  *
  * returns: voxel class weight (double)
  */
 double check_voxel_class(int *surface, int nx, int ny, int nz, int i, int j,
-                         int k) {
+                         int k)
+{
   int contacts = 0;
   double weight = 1.0;
 
   // Count face contacts
   if (surface[k + nz * (j + (ny * (i - 1)))] == 0)
     contacts++;
   if (surface[k + nz * (j + (ny * (i + 1)))] == 0)
@@ -1202,15 +1257,16 @@
     contacts++;
   if (surface[(k - 1) + nz * (j + (ny * i))] == 0)
     contacts++;
   if (surface[(k + 1) + nz * (j + (ny * i))] == 0)
     contacts++;
 
   // Get weight
-  switch (contacts) {
+  switch (contacts)
+  {
   // One face in contact with biomolecule
   case 1:
     weight = 0.894;
     break;
   // Two faces in contact with biomolecule
   case 2:
     weight = 1.3409;
@@ -1218,19 +1274,21 @@
   // Three faces in contact with biomolecule
   case 3:
     if ((surface[k + nz * (j + (ny * (i - 1)))] == 0 &&
          surface[k + nz * (j + (ny * (i + 1)))] == 0) ||
         (surface[k + nz * ((j - 1) + (ny * i))] == 0 &&
          surface[k + nz * ((j + 1) + (ny * i))] == 0) ||
         (surface[(k - 1) + nz * (j + (ny * i))] == 0 &&
-         surface[(k + 1) + nz * (j + (ny * i))] == 0)) {
+         surface[(k + 1) + nz * (j + (ny * i))] == 0))
+    {
       weight = 2;
     }
 
-    else {
+    else
+    {
       weight = 1.5879;
     }
 
     break;
   // Four faces in contact with biomolecule
   case 4:
     weight = 2.6667;
@@ -1256,15 +1314,16 @@
  * step: 3D grid spacing (A)
  * areas: empty array of areas
  * narea: number of cavities
  * nthreads: number of threads for OpenMP
  *
  */
 void _area(int *surface, int nxx, int nyy, int nzz, double step, double *areas,
-           int narea, int nthreads) {
+           int narea, int nthreads)
+{
   int i, j, k;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
   for (i = 0; i < narea; i++)
@@ -1293,28 +1352,30 @@
  * step: 3D grid spacing (A)
  * volumes: empty array of volumes
  * nvol: number of cavities
  * nthreads: number of threads for OpenMP
  *
  */
 void _volume(int *cavities, int nx, int ny, int nz, double step,
-             double *volumes, int nvol, int nthreads) {
+             double *volumes, int nvol, int nthreads)
+{
   int i, j, k;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
   // Initialize volumes array
   dgrid(volumes, nvol);
 
-#pragma omp parallel default(none),                                            \
+#pragma omp parallel default(none), \
     shared(volumes, cavities, nvol, step, nx, ny, nz), private(i, j, k)
   {
-#pragma omp for collapse(3) reduction(+ : volumes[:nvol])
+#pragma omp for collapse(3) reduction(+ \
+                                      : volumes[:nvol])
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
           if (cavities[k + nz * (j + (ny * i))] > 1)
             volumes[cavities[k + nz * (j + (ny * i))] - 2] += pow(step, 3);
   }
 }
@@ -1342,15 +1403,16 @@
  * verbose: print extra information to standard output
  *
  * returns: surface (surface points 3D grid), volumes (array of volumes) and
  * area (array of areas)
  */
 void _spatial(int *cavities, int nx, int ny, int nz, int *surface, int size,
               double *volumes, int nvol, double *areas, int narea, double step,
-              int nthreads, int verbose) {
+              int nthreads, int verbose)
+{
   if (verbose)
     fprintf(stdout, "> Defining surface points\n");
   filter_surface(cavities, surface, nx, ny, nz, nthreads);
 
 #pragma omp sections
   {
 #pragma omp section
@@ -1407,15 +1469,16 @@
  * i: x coordinate of cavity point
  * j: y coordinate of cavity point
  * k: z coordinate of cavity point
  *
  * returns: cavity identifier (tag) or cavity-bulk boundary identifier (-tag)
  */
 int define_boundary_points(int *cavities, int nx, int ny, int nz, int i, int j,
-                           int k) {
+                           int k)
+{
   if (i - 1 >= 0)
     if (cavities[k + nz * (j + (ny * (i - 1)))] == -1)
       return -(cavities[k + nz * (j + (ny * i))]);
   if (i + 1 < nx)
     if (cavities[k + nz * (j + (ny * (i + 1)))] == -1)
       return -(cavities[k + nz * (j + (ny * i))]);
   if (j - 1 >= 0)
@@ -1444,30 +1507,32 @@
  * nx: x grid units
  * ny: y grid units
  * nz: z grid units
  * nthreads: number of threads for OpenMP
  *
  */
 void filter_boundary(int *cavities, int nx, int ny, int nz, pts *cavs,
-                     pts *boundaries, int nthreads) {
+                     pts *boundaries, int nthreads)
+{
   int i, j, k, tag;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none),                                            \
+#pragma omp parallel default(none), \
     shared(cavities, nx, ny, nz, cavs, boundaries), private(i, j, k, tag)
   {
 #pragma omp for collapse(3) schedule(static)
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
 #pragma omp critical
-          if (cavities[k + nz * (j + (ny * i))] > 1) {
+          if (cavities[k + nz * (j + (ny * i))] > 1)
+          {
             // Get cavity identifier
             tag = cavities[k + nz * (j + (ny * i))] - 2;
 
             // Get min and max coordinates of each cavity
             cavs[tag].X1 = min(cavs[tag].X1, i);
             cavs[tag].Y1 = min(cavs[tag].Y1, j);
             cavs[tag].Z1 = min(cavs[tag].Z1, k);
@@ -1476,15 +1541,16 @@
             cavs[tag].Z2 = max(cavs[tag].Z2, k);
 
             // Define cavity-bulk boundary points
             cavities[k + nz * (j + (ny * i))] =
                 define_boundary_points(cavities, nx, ny, nz, i, j, k);
 
             // Get min and max coordinates of each cavity-bulk boundary
-            if (cavities[k + nz * (j + (ny * i))] < -1) {
+            if (cavities[k + nz * (j + (ny * i))] < -1)
+            {
               boundaries[tag].X1 = min(boundaries[tag].X1, i);
               boundaries[tag].Y1 = min(boundaries[tag].Y1, j);
               boundaries[tag].Z1 = min(boundaries[tag].Z1, k);
               boundaries[tag].X2 = max(boundaries[tag].X2, i);
               boundaries[tag].Y2 = max(boundaries[tag].Y2, j);
               boundaries[tag].Z2 = max(boundaries[tag].Z2, k);
             }
@@ -1502,22 +1568,23 @@
  * nx: x grid units
  * ny: y grid units
  * nz: z grid units
  * nthreads: number of threads for OpenMP
  *
  */
 void remove_boundary(int *cavities, int nx, int ny, int nz, int ncav,
-                     pts *boundaries, int nthreads) {
+                     pts *boundaries, int nthreads)
+{
   int i, j, k, tag;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none),                                            \
+#pragma omp parallel default(none), \
     shared(cavities, boundaries, ncav, nx, ny, nz), private(tag, i, j, k)
 #pragma omp for schedule(dynamic)
   for (tag = 0; tag < ncav; tag++)
     for (i = boundaries[tag].X1; i <= boundaries[tag].X2; i++)
       for (j = boundaries[tag].Y1; j <= boundaries[tag].Y2; j++)
         for (k = boundaries[tag].Z1; k <= boundaries[tag].Z2; k++)
           if (cavities[k + nz * (j + (ny * i))] < -1)
@@ -1548,59 +1615,66 @@
  * boundaries: Array with minimum and maximum grid coordinates of each
  * cavity-bulk boundary step: 3D grid spacing (A) nthreads: number of threads
  * for OpenMP
  *
  */
 void estimate_depth(int *cavities, double *depths, int nx, int ny, int nz,
                     double *max_depth, double *avg_depth, int ncav, pts *cavs,
-                    pts *boundaries, double step, int nthreads) {
+                    pts *boundaries, double step, int nthreads)
+{
   int i, j, k, i2, j2, k2, count, tag;
   double distance, tmp;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
 #pragma omp parallel default(none),                                            \
     shared(cavities, depths, max_depth, avg_depth, cavs, boundaries, ncav, nx, \
            ny, nz, step),                                                      \
     private(tmp, tag, i, j, k, i2, j2, k2, distance, count)
   {
 #pragma omp for schedule(dynamic)
-    for (tag = 0; tag < ncav; tag++) {
+    for (tag = 0; tag < ncav; tag++)
+    {
       // Initialize depths for cavity tag
       max_depth[tag] = 0.0;
       avg_depth[tag] = 0.0;
 
       // Initialize number of cavity points in cavity
       count = 0;
 
       for (i = cavs[tag].X1; i <= cavs[tag].X2; i++)
         for (j = cavs[tag].Y1; j <= cavs[tag].Y2; j++)
           for (k = cavs[tag].Z1; k <= cavs[tag].Z2; k++)
-            if (abs(cavities[k + nz * (j + (ny * i))]) == (tag + 2)) {
+            if (abs(cavities[k + nz * (j + (ny * i))]) == (tag + 2))
+            {
               // Initialize tmp depth value
               tmp = sqrt(pow(nx, 2) + pow(ny, 2) + pow(nz, 2)) * step;
 
               // Count cavity point
               count++;
 
               if (boundaries[tag].X1 == nx && boundaries[tag].Y1 == ny &&
                   boundaries[tag].Z1 == nz && boundaries[tag].X2 == 0.0 &&
-                  boundaries[tag].Y2 == 0.0 && boundaries[tag].Z2 == 0.0) {
+                  boundaries[tag].Y2 == 0.0 && boundaries[tag].Z2 == 0.0)
+              {
                 // Cavity without boundary (void)
                 tmp = 0.0;
-              } else {
+              }
+              else
+              {
                 // Depth is calculate as the minimum distance between cavity
                 // point and bulk-cavity boundary
                 for (i2 = boundaries[tag].X1; i2 <= boundaries[tag].X2; i2++)
                   for (j2 = boundaries[tag].Y1; j2 <= boundaries[tag].Y2; j2++)
                     for (k2 = boundaries[tag].Z1; k2 <= boundaries[tag].Z2;
                          k2++)
-                      if (cavities[k2 + nz * (j2 + (ny * i2))] == -(tag + 2)) {
+                      if (cavities[k2 + nz * (j2 + (ny * i2))] == -(tag + 2))
+                      {
                         distance = sqrt(pow(i2 - i, 2) + pow(j2 - j, 2) +
                                         pow(k2 - k, 2)) *
                                    step;
                         if (distance < tmp)
                           tmp = distance;
                       }
               }
@@ -1646,30 +1720,32 @@
  *
  * returns: depths (3D grid with depth of cavity points), max_depth (array of
  * maximum depths) and avg_depth (array of average depths)
  *
  */
 void _depth(int *cavities, int nx, int ny, int nz, double *depths, int size,
             double *max_depth, int nmax, double *avg_depth, int navg,
-            double step, int nthreads, int verbose) {
+            double step, int nthreads, int verbose)
+{
   int i, ncav;
   pts *cavs, *boundaries;
 
   // Get number of cavities
   ncav = nmax;
 
   // Fill depth 3D grid with 0.0
   dgrid(depths, size);
 
   // Allocate memory
   cavs = (pts *)calloc(ncav, sizeof(pts));
   boundaries = (pts *)calloc(ncav, sizeof(pts));
 
   // Initialize boundaries and cavs points
-  for (i = 0; i < ncav; i++) {
+  for (i = 0; i < ncav; i++)
+  {
     boundaries[i].X1 = nx;
     boundaries[i].Y1 = ny;
     boundaries[i].Z1 = nz;
     boundaries[i].X2 = 0.0;
     boundaries[i].Y2 = 0.0;
     boundaries[i].Z2 = 0.0;
     cavs[i].X1 = nx;
@@ -1717,35 +1793,40 @@
  * nzz: z grid units (openings)
  * ncav: number of cavities
  * nthreads: number of threads for OpenMP
  *
  */
 void _openings2cavities(int *o2c, int nopenings, int *cavities, int nx, int ny,
                         int nz, int *openings, int nxx, int nyy, int nzz,
-                        int nthreads) {
+                        int nthreads)
+{
   int i, j, k, tag, stop;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-  for (tag = 0; tag < nopenings; tag++) {
-#pragma omp parallel default(none),                                            \
+  for (tag = 0; tag < nopenings; tag++)
+  {
+#pragma omp parallel default(none), \
     shared(stop, tag, o2c, cavities, openings, nx, ny, nz), private(i, j, k)
     {
       stop = 0;
 #pragma omp for collapse(3) schedule(static)
       for (i = 0; i < nx; i++)
         for (j = 0; j < ny; j++)
-          for (k = 0; k < nz; k++) {
+          for (k = 0; k < nz; k++)
+          {
             if (stop)
               continue;
-            else {
+            else
+            {
               if (openings[k + nz * (j + (ny * i))] == tag + 2 &&
-                  cavities[k + nz * (j + (ny * i))] > 1) {
+                  cavities[k + nz * (j + (ny * i))] > 1)
+              {
                 o2c[tag] = cavities[k + nz * (j + (ny * i))] - 2;
                 stop = 1;
               }
             }
           }
     }
   }
@@ -1768,33 +1849,36 @@
  * nzz: z grid units (depths)
  * ncav: number of cavities
  * nthreads: number of threads for OpenMP
  *
  */
 void remove_enclosed_cavity(int *openings, int *cavities, int nx, int ny,
                             int nz, double *depths, int nxx, int nyy, int nzz,
-                            int ncav, int nthreads) {
+                            int ncav, int nthreads)
+{
   int i, j, k, tag;
   double sum_depth;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
   // Copy cavities to openings
 #pragma omp parallel default(shared), private(i, j, k)
 #pragma omp for schedule(static)
   for (i = 0; i < (nx * ny * nz); i++)
     openings[i] = cavities[i];
 
-  for (tag = 0; tag < ncav; tag++) {
+  for (tag = 0; tag < ncav; tag++)
+  {
     sum_depth = 0.0;
 
 #pragma omp parallel default(shared), private(i, j, k)
-#pragma omp for collapse(3) schedule(static) reduction(+ : sum_depth)
+#pragma omp for collapse(3) schedule(static) reduction(+ \
+                                                       : sum_depth)
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
           if (openings[k + nz * (j + (ny * i))] == tag + 2)
             sum_depth += depths[k + nz * (j + (ny * i))];
 
     // Check if kvtag is a enclosed cavity
@@ -1814,37 +1898,42 @@
  * nx: x grid units
  * ny: y grid units
  * nz: z grid units
  * nthreads: number of threads for OpenMP
  *
  */
 void filter_openings(int *openings, double *depths, int nx, int ny, int nz,
-                     int nthreads) {
+                     int nthreads)
+{
   int i, j, k;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-#pragma omp parallel default(none), shared(openings, depths, nx, ny, nz),      \
+#pragma omp parallel default(none), shared(openings, depths, nx, ny, nz), \
     private(i, j, k)
   {
 #pragma omp for collapse(3) schedule(static)
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
-          if (openings[k + nz * (j + (ny * i))] > 1) {
+          if (openings[k + nz * (j + (ny * i))] > 1)
+          {
             if (depths[k + nz * (j + (ny * i))] == 0.0)
               openings[k + nz * (j + (ny * i))] = 1;
             else
               openings[k + nz * (j + (ny * i))] = 0;
-          } else {
+          }
+          else
+          {
             if (openings[k + nz * (j + (ny * i))] == 1)
               openings[k + nz * (j + (ny * i))] = -1;
-            else {
+            else
+            {
               if (openings[k + nz * (j + (ny * i))] == 0)
                 openings[k + nz * (j + (ny * i))] = 0;
               else
                 openings[k + nz * (j + (ny * i))] = -1;
             }
           }
   }
@@ -1873,15 +1962,16 @@
  * verbose: print extra information to standard output
  *
  * returns: surface (surface points 3D grid), volumes (array of volumes) and
  * area (array of areas)
  */
 int _openings(int *openings, int size, int *cavities, int nx, int ny, int nz,
               double *depths, int nxx, int nyy, int nzz, int ncav,
-              int openings_cutoff, double step, int nthreads, int verbose) {
+              int openings_cutoff, double step, int nthreads, int verbose)
+{
   int nopenings;
 
   if (verbose)
     fprintf(stdout, "> Removing enclosed cavities\n");
   remove_enclosed_cavity(openings, cavities, nx, ny, nz, depths, nxx, nyy, nzz,
                          ncav, nthreads);
 
@@ -1920,15 +2010,16 @@
  *
  * Create a res node
  *
  * pos: atom index in xyzr array (coordinates and radii of pdb)
  *
  * returns: res node with atom index
  */
-res *create(int pos) {
+res *create(int pos)
+{
   res *new = (res *)malloc(sizeof(res));
 
   new->pos = pos;
   new->next = NULL;
 
   return new;
 }
@@ -1939,23 +2030,28 @@
  *
  * Insert res node in linked list
  *
  * res: pointer to linked list head
  * new: res node
  *
  */
-void insert(res **head, res *new) {
+void insert(res **head, res *new)
+{
   res *current;
 
-  if (*head == NULL || (*head)->pos >= new->pos) {
+  if (*head == NULL || (*head)->pos >= new->pos)
+  {
     new->next = *head;
     *head = new;
-  } else {
+  }
+  else
+  {
     current = *head;
-    while (current->next != NULL && current->next->pos < new->pos) {
+    while (current->next != NULL && current->next->pos < new->pos)
+    {
       current = current->next;
     }
     new->next = current->next;
     current->next = new;
   }
 }
 
@@ -1984,27 +2080,29 @@
  *
  * returns: array of strings with interface residues with cavities separated by
  * '-1'
  */
 char **interface(int *cavities, int nx, int ny, int nz, char **pdb,
                  double *atoms, int natoms, int xyzr, double *reference,
                  int ndims, double *sincos, int nvalues, double step,
-                 double probe_in, int ncav, int nthreads) {
+                 double probe_in, int ncav, int nthreads)
+{
   int i, j, k, atom, tag, count = 0, old_atom = -1, old_tag = -1;
   double x, y, z, xaux, yaux, zaux, distance, H;
   char **residues;
 
   // Allocate memory for reslist structure
   res *reslist[ncav], *new, *old;
 
   // Initialize linked list
   for (i = 0; i < ncav; i++)
     reslist[i] = NULL;
 
-  for (atom = 0; atom < natoms; atom++) {
+  for (atom = 0; atom < natoms; atom++)
+  {
     // Convert atom coordinates in 3D grid coordinates
     x = (atoms[atom * 4] - reference[0]) / step;
     y = (atoms[1 + (atom * 4)] - reference[1]) / step;
     z = (atoms[2 + (atom * 4)] - reference[2]) / step;
 
     xaux = x * sincos[3] + z * sincos[2];
     yaux = y;
@@ -2016,37 +2114,43 @@
 
     // Create a radius (H) for space occupied by probe and atom
     H = (probe_in + atoms[3 + (atom * 4)]) / step;
 
     // Loop around radius from atom center
     for (i = floor(x - H); i <= ceil(x + H); i++)
       for (j = floor(y - H); j <= ceil(y + H); j++)
-        for (k = floor(z - H); k <= ceil(z + H); k++) {
+        for (k = floor(z - H); k <= ceil(z + H); k++)
+        {
           if (i < nx && i > 0 && j < ny && j > 0 && k < nz && k > 0)
-            if (abs(cavities[k + nz * (j + (ny * i))]) > 1) {
+            if (abs(cavities[k + nz * (j + (ny * i))]) > 1)
+            {
               tag = cavities[k + nz * (j + (ny * i))] - 2;
               distance = sqrt(pow(i - x, 2) + pow(j - y, 2) + pow(k - z, 2));
-              if (distance <= H) {
-                if (old_atom != atom || old_tag != tag) {
+              if (distance <= H)
+              {
+                if (old_atom != atom || old_tag != tag)
+                {
                   new = create(atom);
                   insert(&reslist[tag], new);
                   count++;
                 }
                 old_atom = atom;
                 old_tag = tag;
               }
             }
         }
   }
 
   // Pass res information to char **
   residues = calloc(count + ncav + 1, sizeof(char *));
-  for (i = 0, j = 0; i < ncav; i++) {
+  for (i = 0, j = 0; i < ncav; i++)
+  {
     new = reslist[i];
-    while (new != NULL) {
+    while (new != NULL)
+    {
       residues[j++] = pdb[new->pos];
       old = new;
       new = old->next;
       free(old);
     }
     residues[j++] = "-1";
   }
@@ -2083,15 +2187,16 @@
  * returns: array of strings with interface residues with cavities separated by
  * '-1'
  *
  */
 char **_constitutional(int *cavities, int nx, int ny, int nz, char **pdb,
                        double *atoms, int natoms, int xyzr, double *reference,
                        int ndims, double *sincos, int nvalues, double step,
-                       double probe_in, int ncav, int nthreads, int verbose) {
+                       double probe_in, int ncav, int nthreads, int verbose)
+{
   char **residues;
 
   if (verbose)
     fprintf(stdout, "> Retrieving interface residues\n");
   residues =
       interface(cavities, nx, ny, nz, pdb, atoms, natoms, xyzr, reference,
                 ndims, sincos, nvalues, step, probe_in, ncav, nthreads);
@@ -2110,15 +2215,16 @@
  * resname: target residue name
  * resn: 1D-array hydrophobicity scale residues names
  * scales: 1D-array of hydrophocity scale values
  * nscales: size of 1D-array of scales and resn
  *
  */
 double get_hydrophobicity_value(char *resname, char **resn, double *scales,
-                                int nscales) {
+                                int nscales)
+{
   int i;
 
   // Get hydrophobicity value
   for (i = 0; i < nscales; i++)
     if (strcmp(resname, resn[i]) == 0)
       return scales[i];
 
@@ -2153,25 +2259,27 @@
  *
  */
 void project_hydropathy(double *hydropathy, int *surface, int nxx, int nyy,
                         int nzz, double *atoms, int natoms, int xyzr,
                         double *reference, int ndims, double *sincos,
                         int nvalues, char **resname, char **resn,
                         double *scales, int nscales, double step,
-                        double probe_in, int nthreads) {
+                        double probe_in, int nthreads)
+{
   int i, j, k, atom;
   double x, y, z, xaux, yaux, zaux, distance, H, *ref;
 
   // Initiliaze 3D grid for residues distances
   ref = (double *)calloc(nxx * nyy * nzz, sizeof(double));
   dgrid(ref, nxx * nyy * nzz);
   dgrid(hydropathy, nxx * nyy * nzz);
 
   // Get hydrophobicity value for each surface point
-  for (atom = 0; atom < natoms; atom++) {
+  for (atom = 0; atom < natoms; atom++)
+  {
     // Convert atom coordinates in 3D grid coordinates
     x = (atoms[atom * 4] - reference[0]) / step;
     y = (atoms[1 + (atom * 4)] - reference[1]) / step;
     z = (atoms[2 + (atom * 4)] - reference[2]) / step;
 
     xaux = x * sincos[3] + z * sincos[2];
     yaux = y;
@@ -2183,29 +2291,33 @@
 
     // Create a radius (H) for space occupied by probe and atom
     H = (probe_in + atoms[3 + (atom * 4)]) / step;
 
     // Loop around radius from atom center
     for (i = floor(x - H); i <= ceil(x + H); i++)
       for (j = floor(y - H); j <= ceil(y + H); j++)
-        for (k = floor(z - H); k <= ceil(z + H); k++) {
+        for (k = floor(z - H); k <= ceil(z + H); k++)
+        {
           if (i < nxx && i > 0 && j < nyy && j > 0 && k < nzz && k > 0)
             // Found a surface point
-            if (surface[k + nzz * (j + (nyy * i))] > 1) {
+            if (surface[k + nzz * (j + (nyy * i))] > 1)
+            {
               // Calculate distance bewteen atom and surface point
               distance = sqrt(pow(i - x, 2) + pow(j - y, 2) + pow(k - z, 2));
               // Check if surface point was not checked before
-              if (ref[k + nzz * (j + (nyy * i))] == 0.0) {
+              if (ref[k + nzz * (j + (nyy * i))] == 0.0)
+              {
                 ref[k + nzz * (j + (nyy * i))] = distance;
                 hydropathy[k + nzz * (j + (nyy * i))] =
                     get_hydrophobicity_value(resname[atom], resn, scales,
                                              nscales);
               }
               // Check if this atom is closer to the previous one assigned
-              else if (ref[k + nzz * (j + (nyy * i))] > distance) {
+              else if (ref[k + nzz * (j + (nyy * i))] > distance)
+              {
                 ref[k + nzz * (j + (nyy * i))] = distance;
                 hydropathy[k + nzz * (j + (nyy * i))] =
                     get_hydrophobicity_value(resname[atom], resn, scales,
                                              nscales);
               }
             }
         }
@@ -2231,38 +2343,40 @@
  * ny: y grid units
  * nz: z grid units
  * nthreads: number of threads for OpenMP
  *
  */
 void estimate_average_hydropathy(double *avgh, int ncav, double *hydropathy,
                                  int *surface, int nx, int ny, int nz,
-                                 int nthreads) {
+                                 int nthreads)
+{
   int i, j, k, *pts;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
   // Initialize array to get number of points in each cavity
   pts = (int *)calloc(ncav, sizeof(int));
   for (i = 0; i < ncav; i++)
     pts[i] = 0;
 
   // Initialize average hydropathy array
   dgrid(avgh, ncav);
 
-#pragma omp parallel default(none),                                            \
+#pragma omp parallel default(none), \
     shared(avgh, hydropathy, surface, pts, nx, ny, nz), private(i, j, k)
   {
 #pragma omp for collapse(3) ordered
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
         for (k = 0; k < nz; k++)
 #pragma omp critical
-          if (surface[k + nz * (j + (ny * i))] > 1) {
+          if (surface[k + nz * (j + (ny * i))] > 1)
+          {
             pts[surface[k + nz * (j + (ny * i))] - 2]++;
             avgh[surface[k + nz * (j + (ny * i))] - 2] +=
                 hydropathy[k + nz * (j + (ny * i))];
           }
   }
 
   for (i = 0; i < ncav; i++)
@@ -2310,15 +2424,16 @@
  *
  */
 void _hydropathy(double *hydropathy, int size, double *avgh, int ncav,
                  int *surface, int nxx, int nyy, int nzz, double *atoms,
                  int natoms, int xyzr, double *reference, int ndims,
                  double *sincos, int nvalues, char **resname, char **resn,
                  double *scales, int nscales, double step, double probe_in,
-                 int nthreads, int verbose) {
+                 int nthreads, int verbose)
+{
   if (verbose)
     fprintf(stdout, "> Mapping hydrophobicity scale at surface points\n");
   project_hydropathy(hydropathy, surface, nxx, nyy, nzz, atoms, natoms, xyzr,
                      reference, ndims, sincos, nvalues, resname, resn, scales,
                      nscales, step, probe_in, nthreads);
 
   if (verbose)
@@ -2329,217 +2444,126 @@
 
 /* Export cavity PDB */
 
 /*
  * Function: _export
  * -----------------
  *
- * Export cavities to PDB file
- *
- * fn: cavity PDB filename
- * cavities: cavities 3D grid
- * nx: x grid units (cavities)
- * ny: y grid units (cavities)
- * nz: z grid units (cavities)
- * surface: surface points 3D grid
- * nxx: x grid units (surface)
- * nyy: y grid units (surface)
- * nzz: z grid units (surface)
- * reference: xyz coordinates of 3D grid origin
- * ndims: number of coordinates (3: xyz)
- * sincos: sin and cos of 3D grid angles
- * nvalues: number of sin and cos (sina, cosa, sinb, cosb)
- * step: 3D grid spacing (A)
- * ncav: number of cavities
- * nthreads: number of threads for OpenMP
- * append: append cavities to PDB file
- * model: model number
- *
- */
-void _export(char *fn, int *cavities, int nx, int ny, int nz, int *surface,
-             int nxx, int nyy, int nzz, double *reference, int ndims,
-             double *sincos, int nvalues, double step, int ncav, int nthreads,
-             int append, int model) {
-  int i, j, k, count, tag;
-  double x, y, z, xaux, yaux, zaux;
-  FILE *output;
-
-  // Set number of threads in OpenMP
-  omp_set_num_threads(nthreads);
-  omp_set_nested(1);
-
-  // Open cavity PDB file
-  if (append)
-    output = fopen(fn, "a+");
-  else
-    output = fopen(fn, "w");
-
-  // Write model number
-  if (abs(model) > 0)
-    fprintf(output, "MODEL     %4.d\n", model);
-
-  for (count = 1, tag = 2; tag <= ncav + 2; tag++)
-#pragma omp parallel default(none)                                             \
-    shared(cavities, surface, reference, sincos, step, ncav, tag, count, nx,   \
-           ny, nz, output),                                                    \
-    private(i, j, k, x, y, z, xaux, yaux, zaux)
-  {
-#pragma omp for schedule(static) collapse(3) ordered nowait
-    for (i = 0; i < nx; i++)
-      for (j = 0; j < ny; j++)
-        for (k = 0; k < nz; k++) {
-          // Check if cavity point with value tag
-          if (cavities[k + nz * (j + (ny * i))] == tag) {
-            // Convert 3D grid coordinates to real coordinates
-            x = i * step;
-            y = j * step;
-            z = k * step;
-
-            xaux = (x * sincos[3]) + (y * sincos[0] * sincos[2]) -
-                   (z * sincos[1] * sincos[2]) + reference[0];
-            yaux = (y * sincos[1]) + (z * sincos[0]) + reference[1];
-            zaux = (x * sincos[2]) - (y * sincos[0] * sincos[3]) +
-                   (z * sincos[1] * sincos[3]) + reference[2];
-
-// Write cavity point
-#pragma omp critical
-            if (surface[k + nz * (j + (ny * i))] == tag)
-              fprintf(output,
-                      "ATOM  %5.d  HA  K%c%c   259    %8.3lf%8.3lf%8.3lf  "
-                      "1.00%6.2lf\n",
-                      count % 100000,
-                      65 + (((surface[k + nz * (j + (ny * i))] - 2) / 26) % 26),
-                      65 + ((surface[k + nz * (j + (ny * i))] - 2) % 26), xaux,
-                      yaux, zaux, 0.0);
-            else
-              fprintf(output,
-                      "ATOM  %5.d  H   K%c%c   259    %8.3lf%8.3lf%8.3lf  "
-                      "1.00%6.2lf\n",
-                      count % 100000,
-                      65 +
-                          (((cavities[k + nz * (j + (ny * i))] - 2) / 26) % 26),
-                      65 + ((cavities[k + nz * (j + (ny * i))] - 2) % 26), xaux,
-                      yaux, zaux, 0.0);
-            count++;
-          }
-        }
-  }
-  // Write ENDMDL
-  if (abs(model) > 0)
-    fprintf(output, "ENDMDL\n");
-  // Write END
-  if (model < 0)
-    fprintf(output, "END\n");
-  // Close file
-  fclose(output);
-}
-
-/*
- * Function: _export_b
- * -------------------
- *
- * Export cavities with a variable as B-factor to PDB file
+ * Export cavities to PDB file with depth as B-factor and hydropathy as Q-factor
  *
  * fn: cavity pdb filename
  * cavities: cavities 3D grid
  * nx: x grid units (cavities)
  * ny: y grid units (cavities)
  * nz: z grid units (cavities)
  * surface: surface points 3D grid
  * nxx: x grid units (surface)
  * nyy: y grid units (surface)
  * nzz: z grid units (surface)
- * B: b-factor 3D grid (depths or hydropathy)
- * nxx: x grid units (B)
- * nyy: y grid units (B)
- * nzz: z grid units (B)
+ * B: B-factor (depth)
+ * bx: x grid units (B)
+ * by: y grid units (B)
+ * bz: z grid units (B)
+ * Q: Q-factor (hydropathy)
+ * qx: x grid units (Q)
+ * qy: y grid units (Q)
+ * qz: z grid units (Q)
  * reference: xyz coordinates of 3D grid origin
  * ndims: number of coordinates (3: xyz)
  * sincos: sin and cos of 3D grid angles
  * nvalues: number of sin and cos (sina, cosa, sinb, cosb)
  * step: 3D grid spacing (A)
  * ncav: number of cavities
  * nthreads: number of threads for OpenMP
  * append: append cavities to PDB file
  * model: model number
  *
  */
-void _export_b(char *fn, int *cavities, int nx, int ny, int nz, int *surface,
-               int nxx, int nyy, int nzz, double *B, int nxxx, int nyyy,
-               int nzzz, double *reference, int ndims, double *sincos,
-               int nvalues, double step, int ncav, int nthreads, int append,
-               int model) {
+void _export(
+    char *fn,
+    int *cavities, int nx, int ny, int nz,
+    int *surface, int nxx, int nyy, int nzz,
+    double *B, int bx, int by, int bz,
+    double *Q, int qx, int qy, int qz,
+    double *reference, int ndims,
+    double *sincos, int nvalues,
+    double step,
+    int ncav,
+    int nthreads,
+    int append, int model)
+{
   int i, j, k, count, tag;
   double x, y, z, xaux, yaux, zaux;
   FILE *output;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
 
-  // Open cavity PDB file
-  if (append)
-    output = fopen(fn, "a+");
-  else
-    output = fopen(fn, "w");
+  // Open cavity PDB file for writing and appending cavity coordinates
+  output = append ? fopen(fn, "a+") : fopen(fn, "w");
 
   // Write model number
   if (abs(model) > 0)
     fprintf(output, "MODEL     %4.d\n", model);
 
+  // Write cavity points for each cavity
   for (count = 1, tag = 2; tag <= ncav + 2; tag++)
-#pragma omp parallel default(none)                                             \
-    shared(cavities, surface, B, reference, sincos, step, ncav, tag, count,    \
-           nx, ny, nz, output),                                                \
-    private(i, j, k, x, y, z, xaux, yaux, zaux)
+#pragma omp parallel default(none) shared(cavities, surface, B, Q, reference, sincos, step, ncav, tag, count, nx, ny, nz, output), private(i, j, k, x, y, z, xaux, yaux, zaux)
   {
+    // Iterate in x, y, z coordinates from 0 to nx, ny, nz
 #pragma omp for schedule(static) collapse(3) ordered nowait
     for (i = 0; i < nx; i++)
       for (j = 0; j < ny; j++)
-        for (k = 0; k < nz; k++) {
+        for (k = 0; k < nz; k++)
           // Check if cavity point with value tag
-          if (cavities[k + nz * (j + (ny * i))] == tag) {
-            // Convert 3D grid coordinates to real coordinates
+          if (cavities[k + nz * (j + (ny * i))] == tag)
+          {
+            // Convert 3D grid coordinates to Cartesian coordinates
             x = i * step;
             y = j * step;
             z = k * step;
 
             xaux = (x * sincos[3]) + (y * sincos[0] * sincos[2]) -
                    (z * sincos[1] * sincos[2]) + reference[0];
             yaux = (y * sincos[1]) + (z * sincos[0]) + reference[1];
             zaux = (x * sincos[2]) - (y * sincos[0] * sincos[3]) +
                    (z * sincos[1] * sincos[3]) + reference[2];
 
-// Write cavity point
+// Write cavity point as a surface point or a cavity point in PDB format
+// depending on the value of the surface grid
 #pragma omp critical
             if (surface[k + nz * (j + (ny * i))] == tag)
               fprintf(output,
-                      "ATOM  %5.d  HA  K%c%c   259    %8.3lf%8.3lf%8.3lf  "
-                      "1.00%6.2lf\n",
+                      "ATOM  %5.d  HA  K%c%c   259    %8.3lf%8.3lf%8.3lf%6.2lf%6.2lf\n",
                       count % 100000,
                       65 + (((surface[k + nz * (j + (ny * i))] - 2) / 26) % 26),
-                      65 + ((surface[k + nz * (j + (ny * i))] - 2) % 26), xaux,
-                      yaux, zaux, B[k + nz * (j + (ny * i))]);
+                      65 + ((surface[k + nz * (j + (ny * i))] - 2) % 26),
+                      xaux,
+                      yaux,
+                      zaux,
+                      Q[k + nz * (j + (ny * i))],
+                      B[k + nz * (j + (ny * i))]);
             else
               fprintf(output,
-                      "ATOM  %5.d  H   K%c%c   259    %8.3lf%8.3lf%8.3lf  "
-                      "1.00%6.2lf\n",
+                      "ATOM  %5.d  H   K%c%c   259    %8.3lf%8.3lf%8.3lf%6.2lf%6.2lf\n",
                       count % 100000,
-                      65 +
-                          (((cavities[k + nz * (j + (ny * i))] - 2) / 26) % 26),
-                      65 + ((cavities[k + nz * (j + (ny * i))] - 2) % 26), xaux,
-                      yaux, zaux, B[k + nz * (j + (ny * i))]);
+                      65 + (((cavities[k + nz * (j + (ny * i))] - 2) / 26) % 26),
+                      65 + ((cavities[k + nz * (j + (ny * i))] - 2) % 26),
+                      xaux,
+                      yaux,
+                      zaux,
+                      Q[k + nz * (j + (ny * i))],
+                      B[k + nz * (j + (ny * i))]);
             count++;
           }
-        }
   }
-  // Write ENDMDL
+  // Write ENDMDL when abs(model) > 0 and END when model < 0
   if (abs(model) > 0)
     fprintf(output, "ENDMDL\n");
-  // Write END
   if (model < 0)
     fprintf(output, "END\n");
   // Close file
   fclose(output);
 }
 
 /*
@@ -2563,15 +2587,16 @@
  * append: append cavities to PDB file
  * model: model number
  *
  */
 void _export_openings(char *fn, int *openings, int nxx, int nyy, int nzz,
                       double *reference, int ndims, double *sincos, int nvalues,
                       double step, int nopenings, int nthreads, int append,
-                      int model) {
+                      int model)
+{
   int i, j, k, count, tag;
   double x, y, z, xaux, yaux, zaux;
   FILE *output;
 
   // Set number of threads in OpenMP
   omp_set_num_threads(nthreads);
   omp_set_nested(1);
@@ -2591,17 +2616,19 @@
     shared(openings, reference, sincos, step, nopenings, tag, count, nxx, nyy, \
            nzz, output),                                                       \
     private(i, j, k, x, y, z, xaux, yaux, zaux)
   {
 #pragma omp for schedule(static) collapse(3) ordered nowait
     for (i = 0; i < nxx; i++)
       for (j = 0; j < nyy; j++)
-        for (k = 0; k < nzz; k++) {
+        for (k = 0; k < nzz; k++)
+        {
           // Check if cavity point with value tag
-          if (openings[k + nzz * (j + (nyy * i))] == tag) {
+          if (openings[k + nzz * (j + (nyy * i))] == tag)
+          {
             // Convert 3D grid coordinates to real coordinates
             x = i * step;
             y = j * step;
             z = k * step;
 
             xaux = (x * sincos[3]) + (y * sincos[0] * sincos[2]) -
                    (z * sincos[1] * sincos[2]) + reference[0];
```

### Comparing `pyKVFinder-0.5.5/C/pyKVFinder.h` & `pyKVFinder-0.6.0/C/pyKVFinder.h`

 * *Files 1% similar despite different names*

```diff
@@ -98,10 +98,9 @@
                                  int *surface, int nx, int ny, int nz,
                                  int nthreads);
 
 /* Hydropathy characterization */
 void _hydropathy(double *hydropathy, int size, double *avgh, int ncav, int *surface, int nxx, int nyy, int nzz, double *atoms, int natoms, int xyzr, double *reference, int ndims, double *sincos, int nvalues, char **resname, char **resn, double *scales, int nscales, double step, double probe_in, int nthreads, int verbose);
 
 /* Export cavity PDB */
-void _export(char *fn, int *cavities, int nx, int ny, int nz, int *surface, int nxx, int nyy, int nzz, double *reference, int ndims, double *sincos, int nvalues, double step, int ncav, int nthreads, int append, int model);
-void _export_b(char *fn, int *cavities, int nx, int ny, int nz, int *surface, int nxx, int nyy, int nzz, double *B, int nxxx, int nyyy, int nzzz, double *reference, int ndims, double *sincos, int nvalues, double step, int ncav, int nthreads, int append, int model);
+void _export(char *fn, int *cavities, int nx, int ny, int nz, int *surface, int nxx, int nyy, int nzz, double *B, int bx, int by, int bz, double *Q, int qx, int qy, int qz, double *reference, int ndims, double *sincos, int nvalues, double step, int ncav, int nthreads, int append, int model);
 void _export_openings(char *fn, int *openings, int nxx, int nyy, int nzz, double *reference, int ndims, double *sincos, int nvalues, double step, int nopenings, int nthreads, int append, int model);
```

### Comparing `pyKVFinder-0.5.5/C/pyKVFinder.i` & `pyKVFinder-0.6.0/C/pyKVFinder.i`

 * *Files 5% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 %apply (double* INPLACE_ARRAY3, int DIM1, int DIM2, int DIM3) {(double* depths, int nxx, int nyy, int nzz)}
 
 /* Clustering grid */
 %apply (int* INPLACE_ARRAY3, int DIM1, int DIM2, int DIM3) {(int *grid, int nx, int ny, int nz)}
 
 /* Hydropathy grid */
 %apply (double* ARGOUT_ARRAY1, int DIM1) {(double* hydropathy, int size)}
+%apply (double* INPLACE_ARRAY3, int DIM1, int DIM2, int DIM3) {(double* Q, int qx, int qy, int qz)}
 
 /* Openings grid */
 %apply (int* ARGOUT_ARRAY1, int DIM1) {(int* openings, int size)}
 %apply (int* INPLACE_ARRAY3, int DIM1, int DIM2, int DIM3) {(int* openings, int nxx, int nyy, int nzz)}
 %apply (int* ARGOUT_ARRAY1, int DIM1) {(int* o2c, int nopenings)}
 
 /* Bfactor grid */
-%apply (double* INPLACE_ARRAY3, int DIM1, int DIM2, int DIM3) {(double* B, int nxxx, int nyyy, int nzzz)}
+%apply (double* INPLACE_ARRAY3, int DIM1, int DIM2, int DIM3) {(double* B, int bx, int by, int bz)}
 
 /* Volume array */
 %apply (double* ARGOUT_ARRAY1, int DIM1) {(double* volumes, int nvol)}
 
 /* Area array */
 %apply (double* ARGOUT_ARRAY1, int DIM1) {(double* areas, int narea)}
```

### Comparing `pyKVFinder-0.5.5/LICENSE.txt` & `pyKVFinder-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/PKG-INFO` & `pyKVFinder-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.5.5
+Version: 0.6.0
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.5.5/README.rst` & `pyKVFinder-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/__init__.py` & `pyKVFinder-0.6.0/pyKVFinder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 --------
 * GitHub repository: https://github.com/LBC-LNBio/pyKVFinder
 
 * Documentation: https://lbc-lnbio.github.io/pyKVFinder
 """
 
 __name__ = "pyKVFinder"
-__version__ = "0.5.5"
+__version__ = "0.6.0"
 license = "GNU GPL-3.0 License"
 
 from .utils import *
 from .grid import *
 from .main import *
```

### Comparing `pyKVFinder-0.5.5/pyKVFinder/argparser.py` & `pyKVFinder-0.6.0/pyKVFinder/argparser.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb` & `pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.pdb` & `pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.xyz` & `pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.pdb` & `pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.xyz` & `pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/tests/PKI.pdb` & `pyKVFinder-0.6.0/pyKVFinder/data/tests/PKI.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/data/vdw.dat` & `pyKVFinder-0.6.0/pyKVFinder/data/vdw.dat`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyKVFinder/grid.py` & `pyKVFinder-0.6.0/pyKVFinder/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -5781,1097 +5781,952 @@
 00016940: 206f 7065 6e69 6e67 3263 6176 6974 7929   opening2cavity)
 00016950: 0a0a 2020 2020 7265 7475 726e 206e 6f70  ..    return nop
 00016960: 656e 696e 6773 2c20 6f70 656e 696e 6773  enings, openings
 00016970: 2c20 616f 7065 6e69 6e67 730a 0a0a 6465  , aopenings...de
 00016980: 6620 6578 706f 7274 280a 2020 2020 666e  f export(.    fn
 00016990: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
 000169a0: 686c 6962 2e50 6174 685d 2c0a 2020 2020  hlib.Path],.    
-000169b0: 6361 7669 7469 6573 3a20 4f70 7469 6f6e  cavities: Option
-000169c0: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
-000169d0: 5d2c 0a20 2020 2073 7572 6661 6365 3a20  ],.    surface: 
-000169e0: 4f70 7469 6f6e 616c 5b6e 756d 7079 2e6e  Optional[numpy.n
-000169f0: 6461 7272 6179 5d2c 0a20 2020 2076 6572  darray],.    ver
-00016a00: 7469 6365 733a 2055 6e69 6f6e 5b6e 756d  tices: Union[num
-00016a10: 7079 2e6e 6461 7272 6179 2c20 4c69 7374  py.ndarray, List
-00016a20: 5b4c 6973 745b 666c 6f61 745d 5d5d 2c0a  [List[float]]],.
-00016a30: 2020 2020 7374 6570 3a20 556e 696f 6e5b      step: Union[
-00016a40: 666c 6f61 742c 2069 6e74 5d20 3d20 302e  float, int] = 0.
-00016a50: 362c 0a20 2020 2042 3a20 4f70 7469 6f6e  6,.    B: Option
-00016a60: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
-00016a70: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6f75  ] = None,.    ou
-00016a80: 7470 7574 5f68 7964 726f 7061 7468 793a  tput_hydropathy:
-00016a90: 2055 6e69 6f6e 5b73 7472 2c20 7061 7468   Union[str, path
-00016aa0: 6c69 622e 5061 7468 5d20 3d20 2268 7964  lib.Path] = "hyd
-00016ab0: 726f 7061 7468 792e 7064 6222 2c0a 2020  ropathy.pdb",.  
-00016ac0: 2020 7363 616c 6573 3a20 4f70 7469 6f6e    scales: Option
-00016ad0: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
-00016ae0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7365  ] = None,.    se
-00016af0: 6c65 6374 696f 6e3a 204f 7074 696f 6e61  lection: Optiona
-00016b00: 6c5b 556e 696f 6e5b 4c69 7374 5b69 6e74  l[Union[List[int
-00016b10: 5d2c 204c 6973 745b 7374 725d 5d5d 203d  ], List[str]]] =
-00016b20: 204e 6f6e 652c 0a20 2020 206e 7468 7265   None,.    nthre
-00016b30: 6164 733a 204f 7074 696f 6e61 6c5b 696e  ads: Optional[in
-00016b40: 745d 203d 204e 6f6e 652c 0a20 2020 2061  t] = None,.    a
-00016b50: 7070 656e 643a 2062 6f6f 6c20 3d20 4661  ppend: bool = Fa
-00016b60: 6c73 652c 0a20 2020 206d 6f64 656c 3a20  lse,.    model: 
-00016b70: 696e 7420 3d20 302c 0a29 202d 3e20 4e6f  int = 0,.) -> No
-00016b80: 6e65 3a0a 2020 2020 2222 2245 7870 6f72  ne:.    """Expor
-00016b90: 7420 6361 7669 7469 7920 2848 2920 616e  t cavitiy (H) an
-00016ba0: 6420 7375 7266 6163 6520 2848 4129 2070  d surface (HA) p
-00016bb0: 6f69 6e74 7320 746f 2050 4442 2d66 6f72  oints to PDB-for
-00016bc0: 6d61 7474 6564 2066 696c 6520 7769 7468  matted file with
-00016bd0: 0a20 2020 2061 2076 6172 6961 626c 6520  .    a variable 
-00016be0: 2842 3b20 6f70 7469 6f6e 616c 2920 696e  (B; optional) in
-00016bf0: 2042 2d66 6163 746f 7220 636f 6c75 6d6e   B-factor column
-00016c00: 2c20 616e 6420 6879 6472 6f70 6174 6879  , and hydropathy
-00016c10: 2074 6f0a 2020 2020 5044 422d 666f 726d   to.    PDB-form
-00016c20: 6174 7465 6420 6669 6c65 2069 6e20 422d  atted file in B-
-00016c30: 6661 6374 6f72 2063 6f6c 756d 6e20 6174  factor column at
-00016c40: 2073 7572 6661 6365 2070 6f69 6e74 7320   surface points 
-00016c50: 2848 4129 2e0a 0a20 2020 2050 6172 616d  (HA)...    Param
-00016c60: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00016c70: 2d2d 2d2d 0a20 2020 2066 6e20 3a20 556e  ----.    fn : Un
-00016c80: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-00016c90: 2e50 6174 685d 0a20 2020 2020 2020 2041  .Path].        A
-00016ca0: 2070 6174 6820 746f 2050 4442 2066 696c   path to PDB fil
-00016cb0: 6520 666f 7220 7772 6974 696e 6720 6361  e for writing ca
-00016cc0: 7669 7469 6573 2e0a 2020 2020 6361 7669  vities..    cavi
-00016cd0: 7469 6573 203a 206e 756d 7079 2e6e 6461  ties : numpy.nda
-00016ce0: 7272 6179 2c20 6f70 7469 6f6e 616c 0a20  rray, optional. 
-00016cf0: 2020 2020 2020 2043 6176 6974 7920 706f         Cavity po
-00016d00: 696e 7473 2069 6e20 7468 6520 3344 2067  ints in the 3D g
-00016d10: 7269 6420 2863 6176 6974 6965 735b 6e78  rid (cavities[nx
-00016d20: 5d5b 6e79 5d5b 6e7a 5d29 2e0a 2020 2020  ][ny][nz])..    
-00016d30: 2020 2020 4361 7669 7469 6573 2061 7272      Cavities arr
-00016d40: 6179 2068 6173 2069 6e74 6567 6572 206c  ay has integer l
-00016d50: 6162 656c 7320 696e 2065 6163 6820 706f  abels in each po
-00016d60: 7369 7469 6f6e 2c20 7468 6174 2061 7265  sition, that are
-00016d70: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
-00016d80: 202d 313a 2062 756c 6b20 706f 696e 7473   -1: bulk points
-00016d90: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
-00016da0: 2030 3a20 6269 6f6d 6f6c 6563 756c 6520   0: biomolecule 
-00016db0: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
-00016dc0: 2020 2020 202a 2031 3a20 656d 7074 7920       * 1: empty 
-00016dd0: 7370 6163 6520 706f 696e 7473 3b0a 0a20  space points;.. 
-00016de0: 2020 2020 2020 2020 2020 202a 203e 3d32             * >=2
-00016df0: 3a20 6361 7669 7479 2070 6f69 6e74 732e  : cavity points.
-00016e00: 0a0a 2020 2020 2020 2020 5468 6520 656d  ..        The em
-00016e10: 7074 7920 7370 6163 6520 706f 696e 7473  pty space points
-00016e20: 2061 7265 2072 6567 696f 6e73 2074 6861   are regions tha
-00016e30: 7420 646f 206e 6f74 206d 6565 7420 7468  t do not meet th
-00016e40: 6520 6368 6f73 656e 0a20 2020 2020 2020  e chosen.       
-00016e50: 2076 6f6c 756d 6520 6375 746f 6666 2074   volume cutoff t
-00016e60: 6f20 6265 2063 6f6e 7369 6465 7265 6420  o be considered 
-00016e70: 6120 6361 7669 7479 2e0a 2020 2020 7375  a cavity..    su
-00016e80: 7266 6163 6520 3a20 6e75 6d70 792e 6e64  rface : numpy.nd
-00016e90: 6172 7261 792c 206f 7074 696f 6e61 6c0a  array, optional.
-00016ea0: 2020 2020 2020 2020 5375 7266 6163 6520          Surface 
-00016eb0: 706f 696e 7473 2069 6e20 7468 6520 3344  points in the 3D
-00016ec0: 2067 7269 6420 2873 7572 6661 6365 5b6e   grid (surface[n
-00016ed0: 785d 5b6e 795d 5b6e 7a5d 292e 2049 6620  x][ny][nz]). If 
-00016ee0: 4e6f 6e65 2c20 7375 7266 6163 650a 2020  None, surface.  
-00016ef0: 2020 2020 2020 6973 2061 206e 756d 7079        is a numpy
-00016f00: 2e7a 6572 6f73 2061 7272 6179 2077 6974  .zeros array wit
-00016f10: 6820 7361 6d65 2073 6861 7065 206f 6620  h same shape of 
-00016f20: 6361 7669 7469 6573 2e0a 2020 2020 2020  cavities..      
-00016f30: 2020 5375 7266 6163 6520 6172 7261 7920    Surface array 
-00016f40: 6861 7320 696e 7465 6765 7220 6c61 6265  has integer labe
-00016f50: 6c73 2069 6e20 6561 6368 2070 6f73 6974  ls in each posit
-00016f60: 696f 6e2c 2074 6861 7420 6172 653a 0a0a  ion, that are:..
-00016f70: 2020 2020 2020 2020 2020 2020 2a20 2d31              * -1
-00016f80: 3a20 6275 6c6b 2070 6f69 6e74 733b 0a0a  : bulk points;..
-00016f90: 2020 2020 2020 2020 2020 2020 2a20 303a              * 0:
-00016fa0: 2062 696f 6d6f 6c65 6375 6c65 206f 7220   biomolecule or 
-00016fb0: 656d 7074 7920 7370 6163 6520 706f 696e  empty space poin
-00016fc0: 7473 3b0a 0a20 2020 2020 2020 2020 2020  ts;..           
-00016fd0: 202a 203e 3d32 3a20 7375 7266 6163 6520   * >=2: surface 
-00016fe0: 706f 696e 7473 2e0a 0a20 2020 2020 2020  points...       
-00016ff0: 2054 6865 2065 6d70 7479 2073 7061 6365   The empty space
-00017000: 2070 6f69 6e74 7320 6172 6520 7265 6769   points are regi
-00017010: 6f6e 7320 7468 6174 2064 6f20 6e6f 7420  ons that do not 
-00017020: 6d65 6574 2074 6865 2063 686f 7365 6e0a  meet the chosen.
-00017030: 2020 2020 2020 2020 766f 6c75 6d65 2063          volume c
-00017040: 7574 6f66 6620 746f 2062 6520 636f 6e73  utoff to be cons
-00017050: 6964 6572 6564 2061 2063 6176 6974 792e  idered a cavity.
-00017060: 0a20 2020 2076 6572 7469 6365 7320 3a20  .    vertices : 
-00017070: 556e 696f 6e5b 6e75 6d70 792e 6e64 6172  Union[numpy.ndar
-00017080: 7261 792c 204c 6973 745b 4c69 7374 5b66  ray, List[List[f
-00017090: 6c6f 6174 5d5d 5d0a 2020 2020 2020 2020  loat]]].        
-000170a0: 4120 6e75 6d70 792e 6e64 6172 7261 7920  A numpy.ndarray 
-000170b0: 6f72 2061 206c 6973 7420 7769 7468 2078  or a list with x
-000170c0: 797a 2076 6572 7469 6365 7320 636f 6f72  yz vertices coor
-000170d0: 6469 6e61 7465 7320 286f 7269 6769 6e2c  dinates (origin,
-000170e0: 0a20 2020 2020 2020 2058 2d61 7869 732c  .        X-axis,
-000170f0: 2059 2d61 7869 732c 205a 2d61 7869 7329   Y-axis, Z-axis)
-00017100: 2e0a 2020 2020 7374 6570 203a 2055 6e69  ..    step : Uni
-00017110: 6f6e 5b66 6c6f 6174 2c20 696e 745d 2c20  on[float, int], 
-00017120: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00017130: 2047 7269 6420 7370 6163 696e 6720 2841   Grid spacing (A
-00017140: 292c 2062 7920 6465 6661 756c 7420 302e  ), by default 0.
-00017150: 362e 0a20 2020 2042 203a 206e 756d 7079  6..    B : numpy
-00017160: 2e6e 6461 7272 6179 2c20 6f70 7469 6f6e  .ndarray, option
-00017170: 616c 0a20 2020 2020 2020 2041 206e 756d  al.        A num
-00017180: 7079 2e6e 6461 7272 6179 2077 6974 6820  py.ndarray with 
-00017190: 7661 6c75 6573 2074 6f20 6265 206d 6170  values to be map
-000171a0: 7065 6420 6f6e 2042 2d66 6163 746f 7220  ped on B-factor 
-000171b0: 636f 6c75 6d6e 2069 6e20 6361 7669 7479  column in cavity
-000171c0: 0a20 2020 2020 2020 2070 6f69 6e74 7320  .        points 
-000171d0: 2842 5b6e 785d 5b6e 795d 5b6e 7a5d 292c  (B[nx][ny][nz]),
-000171e0: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
-000171f0: 2e0a 2020 2020 6f75 7470 7574 5f68 7964  ..    output_hyd
-00017200: 726f 7061 7468 7920 3a20 556e 696f 6e5b  ropathy : Union[
-00017210: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-00017220: 685d 2c20 6f70 7469 6f6e 616c 0a20 2020  h], optional.   
-00017230: 2020 2020 2041 2070 6174 6820 746f 2068       A path to h
-00017240: 7964 726f 7061 7468 7920 5044 4220 6669  ydropathy PDB fi
-00017250: 6c65 2028 7375 7266 6163 6520 706f 696e  le (surface poin
-00017260: 7473 206d 6170 7065 6420 7769 7468 2061  ts mapped with a
-00017270: 0a20 2020 2020 2020 2068 7964 726f 7068  .        hydroph
-00017280: 6f62 6963 6974 7920 7363 616c 6529 2c20  obicity scale), 
-00017290: 6279 2064 6566 6175 6c74 2060 6879 6472  by default `hydr
-000172a0: 6f70 6174 6879 2e70 6462 602e 0a20 2020  opathy.pdb`..   
-000172b0: 2073 6361 6c65 7320 3a20 6e75 6d70 792e   scales : numpy.
-000172c0: 6e64 6172 7261 792c 206f 7074 696f 6e61  ndarray, optiona
-000172d0: 6c0a 2020 2020 2020 2020 4120 6e75 6d70  l.        A nump
-000172e0: 792e 6e64 6172 7261 7920 7769 7468 2068  y.ndarray with h
-000172f0: 7964 726f 7068 6f62 6963 6974 7920 7363  ydrophobicity sc
-00017300: 616c 6520 7661 6c75 6573 2074 6f20 6265  ale values to be
-00017310: 206d 6170 7065 6420 6f6e 0a20 2020 2020   mapped on.     
-00017320: 2020 2042 2d66 6163 746f 7220 636f 6c75     B-factor colu
-00017330: 6d6e 2069 6e20 7375 7266 6163 6520 706f  mn in surface po
-00017340: 696e 7473 2028 7363 616c 6573 5b6e 785d  ints (scales[nx]
-00017350: 5b6e 795d 5b6e 7a5d 292c 2062 7920 6465  [ny][nz]), by de
-00017360: 6661 756c 740a 2020 2020 2020 2020 4e6f  fault.        No
-00017370: 6e65 2e0a 2020 2020 7365 6c65 6374 696f  ne..    selectio
-00017380: 6e20 3a20 556e 696f 6e5b 4c69 7374 5b69  n : Union[List[i
-00017390: 6e74 5d2c 204c 6973 745b 7374 725d 5d2c  nt], List[str]],
-000173a0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000173b0: 2020 4120 6c69 7374 206f 6620 696e 7465    A list of inte
-000173c0: 6765 7220 6c61 6265 6c73 206f 7220 6120  ger labels or a 
-000173d0: 6c69 7374 206f 6620 6361 7669 7479 206e  list of cavity n
-000173e0: 616d 6573 2074 6f20 6265 2073 656c 6563  ames to be selec
-000173f0: 7465 642c 2062 7920 6465 6661 756c 7420  ted, by default 
-00017400: 4e6f 6e65 2e0a 2020 2020 6e74 6872 6561  None..    nthrea
-00017410: 6473 203a 2069 6e74 2c20 6f70 7469 6f6e  ds : int, option
-00017420: 616c 0a20 2020 2020 2020 204e 756d 6265  al.        Numbe
-00017430: 7220 6f66 2074 6872 6561 6473 2c20 6279  r of threads, by
-00017440: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
-00017450: 6620 4e6f 6e65 2c20 7468 6520 6e75 6d62  f None, the numb
-00017460: 6572 206f 6620 7468 7265 6164 7320 6973  er of threads is
-00017470: 0a20 2020 2020 2020 2060 6f73 2e63 7075  .        `os.cpu
-00017480: 5f63 6f75 6e74 2829 202d 2031 602e 0a20  _count() - 1`.. 
-00017490: 2020 2061 7070 656e 6420 3a20 626f 6f6c     append : bool
-000174a0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-000174b0: 2020 2057 6865 7468 6572 2074 6f20 6170     Whether to ap
-000174c0: 7065 6e64 2063 6176 6974 6965 7320 746f  pend cavities to
-000174d0: 2074 6865 2050 4442 2066 696c 652c 2062   the PDB file, b
-000174e0: 7920 6465 6661 756c 7420 4661 6c73 652e  y default False.
-000174f0: 0a20 2020 206d 6f64 656c 203a 2069 6e74  .    model : int
-00017500: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00017510: 2020 204d 6f64 656c 206e 756d 6265 722c     Model number,
-00017520: 2062 7920 6465 6661 756c 7420 302e 0a0a   by default 0...
-00017530: 2020 2020 5261 6973 6573 0a20 2020 202d      Raises.    -
-00017540: 2d2d 2d2d 2d0a 2020 2020 5479 7065 4572  -----.    TypeEr
-00017550: 726f 720a 2020 2020 2020 2020 6066 6e60  ror.        `fn`
-00017560: 206d 7573 7420 6265 2061 2073 7472 696e   must be a strin
-00017570: 6720 6f72 2070 6174 686c 6962 2e50 6174  g or pathlib.Pat
-00017580: 682e 0a20 2020 2054 7970 6545 7272 6f72  h..    TypeError
-00017590: 0a20 2020 2020 2020 2060 6361 7669 7469  .        `caviti
-000175a0: 6573 6020 6d75 7374 2062 6520 6120 6e75  es` must be a nu
-000175b0: 6d70 792e 6e64 6172 7261 792e 0a20 2020  mpy.ndarray..   
-000175c0: 2056 616c 7565 4572 726f 720a 2020 2020   ValueError.    
-000175d0: 2020 2020 6063 6176 6974 6965 7360 2068      `cavities` h
-000175e0: 6173 2074 6865 2069 6e63 6f72 7265 6374  as the incorrect
-000175f0: 2073 6861 7065 2e20 4974 206d 7573 7420   shape. It must 
-00017600: 6265 2028 6e78 2c20 6e79 2c20 6e7a 292e  be (nx, ny, nz).
-00017610: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
-00017620: 2020 2020 2020 2060 7375 7266 6163 6560         `surface`
-00017630: 206d 7573 7420 6265 2061 206e 756d 7079   must be a numpy
-00017640: 2e6e 6461 7272 6179 2e0a 2020 2020 5661  .ndarray..    Va
-00017650: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
-00017660: 2060 7375 7266 6163 6560 2068 6173 2074   `surface` has t
-00017670: 6865 2069 6e63 6f72 7265 6374 2073 6861  he incorrect sha
-00017680: 7065 2e20 4974 206d 7573 7420 6265 2028  pe. It must be (
-00017690: 6e78 2c20 6e79 2c20 6e7a 292e 0a20 2020  nx, ny, nz)..   
-000176a0: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-000176b0: 2020 2060 7665 7274 6963 6573 6020 6d75     `vertices` mu
-000176c0: 7374 2062 6520 6120 6c69 7374 206f 7220  st be a list or 
-000176d0: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
-000176e0: 0a20 2020 2056 616c 7565 4572 726f 720a  .    ValueError.
-000176f0: 2020 2020 2020 2020 6076 6572 7469 6365          `vertice
-00017700: 7360 2068 6173 2069 6e63 6f72 7265 6374  s` has incorrect
-00017710: 2073 6861 7065 2e20 4974 206d 7573 7420   shape. It must 
-00017720: 6265 2028 342c 2033 292e 0a20 2020 2054  be (4, 3)..    T
-00017730: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-00017740: 2060 7374 6570 6020 6d75 7374 2062 6520   `step` must be 
-00017750: 6120 706f 7369 7469 7665 2072 6561 6c20  a positive real 
-00017760: 6e75 6d62 6572 2e0a 2020 2020 5661 6c75  number..    Valu
-00017770: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
-00017780: 7374 6570 6020 6d75 7374 2062 6520 6120  step` must be a 
-00017790: 706f 7369 7469 7665 2072 6561 6c20 6e75  positive real nu
-000177a0: 6d62 6572 2e0a 2020 2020 5479 7065 4572  mber..    TypeEr
-000177b0: 726f 720a 2020 2020 2020 2020 6042 6020  ror.        `B` 
-000177c0: 6d75 7374 2062 6520 6120 6e75 6d70 792e  must be a numpy.
-000177d0: 6e64 6172 7261 792e 0a20 2020 2056 616c  ndarray..    Val
-000177e0: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
-000177f0: 6042 6020 6861 7320 7468 6520 696e 636f  `B` has the inco
-00017800: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
-00017810: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
-00017820: 206e 7a29 2e0a 2020 2020 5479 7065 4572   nz)..    TypeEr
-00017830: 726f 720a 2020 2020 2020 2020 606f 7574  ror.        `out
-00017840: 7075 745f 6879 6472 6f70 6174 6879 6020  put_hydropathy` 
-00017850: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
-00017860: 2e0a 2020 2020 5479 7065 4572 726f 720a  ..    TypeError.
-00017870: 2020 2020 2020 2020 6073 6361 6c65 7360          `scales`
-00017880: 206d 7573 7420 6265 2061 206e 756d 7079   must be a numpy
-00017890: 2e6e 6461 7272 6179 2e0a 2020 2020 5661  .ndarray..    Va
-000178a0: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
-000178b0: 2060 7363 616c 6573 6020 6861 7320 7468   `scales` has th
-000178c0: 6520 696e 636f 7272 6563 7420 7368 6170  e incorrect shap
-000178d0: 652e 2049 7420 6d75 7374 2062 6520 286e  e. It must be (n
-000178e0: 782c 206e 792c 206e 7a29 2e0a 2020 2020  x, ny, nz)..    
-000178f0: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
-00017900: 2020 6073 656c 6563 7469 6f6e 6020 6d75    `selection` mu
-00017910: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
-00017920: 7374 7269 6e67 7320 2863 6176 6974 7920  strings (cavity 
-00017930: 6e61 6d65 7329 206f 7220 696e 7465 6765  names) or intege
-00017940: 7273 2028 6361 7669 7479 206c 6162 656c  rs (cavity label
-00017950: 7329 2e0a 2020 2020 5661 6c75 6545 7272  s)..    ValueErr
-00017960: 6f72 0a20 2020 2020 2020 2049 6e76 616c  or.        Inval
-00017970: 6964 2060 7365 6c65 6374 696f 6e60 3a20  id `selection`: 
-00017980: 7b73 656c 6563 7469 6f6e 7d2e 0a20 2020  {selection}..   
-00017990: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-000179a0: 2020 2060 6e74 6872 6561 6473 6020 6d75     `nthreads` mu
-000179b0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-000179c0: 2069 6e74 6567 6572 2e0a 2020 2020 5661   integer..    Va
-000179d0: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
-000179e0: 2060 6e74 6872 6561 6473 6020 6d75 7374   `nthreads` must
-000179f0: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
-00017a00: 6e74 6567 6572 2e0a 2020 2020 5479 7065  nteger..    Type
-00017a10: 4572 726f 720a 2020 2020 2020 2020 6061  Error.        `a
-00017a20: 7070 656e 6460 206d 7573 7420 6265 2061  ppend` must be a
-00017a30: 2062 6f6f 6c65 616e 2e0a 2020 2020 5479   boolean..    Ty
-00017a40: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
-00017a50: 606d 6f64 656c 6020 6d75 7374 2062 6520  `model` must be 
-00017a60: 6120 696e 7465 6765 722e 0a20 2020 2052  a integer..    R
-00017a70: 756e 7469 6d65 4572 726f 720a 2020 2020  untimeError.    
-00017a80: 2020 2020 5573 6572 206d 7573 7420 6465      User must de
-00017a90: 6669 6e65 2060 7375 7266 6163 6560 2077  fine `surface` w
-00017aa0: 6865 6e20 6e6f 7420 6465 6669 6e69 6e67  hen not defining
-00017ab0: 2060 6361 7669 7469 6573 602e 0a0a 2020   `cavities`...  
-00017ac0: 2020 4e6f 7465 0a20 2020 202d 2d2d 2d0a    Note.    ----.
-00017ad0: 2020 2020 5468 6520 6361 7669 7479 206e      The cavity n
-00017ae0: 6f6d 656e 636c 6174 7572 6520 6973 2062  omenclature is b
-00017af0: 6173 6564 206f 6e20 7468 6520 696e 7465  ased on the inte
-00017b00: 6765 7220 6c61 6265 6c2e 2054 6865 2063  ger label. The c
-00017b10: 6176 6974 7920 6d61 726b 6564 0a20 2020  avity marked.   
-00017b20: 2077 6974 6820 322c 2074 6865 2066 6972   with 2, the fir
-00017b30: 7374 2069 6e74 6567 6572 2063 6f72 7265  st integer corre
-00017b40: 7370 6f6e 6469 6e67 2074 6f20 6120 6361  sponding to a ca
-00017b50: 7669 7479 2c20 6973 204b 4141 2c20 7468  vity, is KAA, th
-00017b60: 6520 6361 7669 7479 0a20 2020 206d 6172  e cavity.    mar
-00017b70: 6b65 6420 7769 7468 2033 2069 7320 4b41  ked with 3 is KA
-00017b80: 422c 2074 6865 2063 6176 6974 7920 6d61  B, the cavity ma
-00017b90: 726b 6564 2077 6974 6820 3420 6973 204b  rked with 4 is K
-00017ba0: 4143 2061 6e64 2073 6f20 6f6e 2e0a 0a20  AC and so on... 
-00017bb0: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
-00017bc0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6574  --------.    det
-00017bd0: 6563 740a 2020 2020 7370 6174 6961 6c0a  ect.    spatial.
-00017be0: 2020 2020 6465 7074 680a 2020 2020 6879      depth.    hy
-00017bf0: 6472 6f70 6174 6879 0a20 2020 2077 7269  dropathy.    wri
-00017c00: 7465 5f72 6573 756c 7473 0a0a 2020 2020  te_results..    
-00017c10: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
-00017c20: 2d2d 2d0a 2020 2020 5769 7468 2074 6865  ---.    With the
-00017c30: 2063 6176 6974 7920 616e 6420 7375 7266   cavity and surf
-00017c40: 6163 6520 706f 696e 7473 2069 6465 6e74  ace points ident
-00017c50: 6966 6965 6420 616e 6420 6465 7074 6820  ified and depth 
-00017c60: 616e 6420 6879 6472 6f70 686f 6269 6369  and hydrophobici
-00017c70: 7479 2073 6361 6c65 206d 6170 7065 6420  ty scale mapped 
-00017c80: 696e 2074 6865 2033 4420 6772 6964 2c20  in the 3D grid, 
-00017c90: 7765 2063 616e 3a0a 0a20 2020 202a 2045  we can:..    * E
-00017ca0: 7870 6f72 7420 6361 7669 7479 2070 6f69  xport cavity poi
-00017cb0: 6e74 730a 0a20 2020 203e 3e3e 2066 726f  nts..    >>> fro
-00017cc0: 6d20 7079 4b56 4669 6e64 6572 2069 6d70  m pyKVFinder imp
-00017cd0: 6f72 7420 6578 706f 7274 0a20 2020 203e  ort export.    >
-00017ce0: 3e3e 2065 7870 6f72 7428 2763 6176 6974  >> export('cavit
-00017cf0: 795f 776f 5f73 7572 6661 6365 2e70 6462  y_wo_surface.pdb
-00017d00: 272c 2063 6176 6974 6965 732c 204e 6f6e  ', cavities, Non
-00017d10: 652c 2076 6572 7469 6365 7329 0a0a 2020  e, vertices)..  
-00017d20: 2020 2a20 4578 706f 7274 2063 6176 6974    * Export cavit
-00017d30: 7920 616e 6420 7375 7266 6163 6520 706f  y and surface po
-00017d40: 696e 7473 0a0a 2020 2020 3e3e 3e20 6578  ints..    >>> ex
-00017d50: 706f 7274 2827 6361 7669 7469 6573 2e70  port('cavities.p
-00017d60: 6462 272c 2063 6176 6974 6965 732c 2073  db', cavities, s
-00017d70: 7572 6661 6365 2c20 7665 7274 6963 6573  urface, vertices
-00017d80: 290a 0a20 2020 202a 2045 7870 6f72 7420  )..    * Export 
-00017d90: 6361 7669 7479 2061 6e64 2073 7572 6661  cavity and surfa
-00017da0: 6365 2070 6f69 6e74 7320 7769 7468 2064  ce points with d
-00017db0: 6570 7468 206d 6170 7065 6420 6f6e 2074  epth mapped on t
-00017dc0: 6865 6d0a 0a20 2020 203e 3e3e 2065 7870  hem..    >>> exp
-00017dd0: 6f72 7428 2763 6176 6974 6965 735f 7769  ort('cavities_wi
-00017de0: 7468 5f64 6570 7468 2e70 6462 272c 2063  th_depth.pdb', c
-00017df0: 6176 6974 6965 732c 2073 7572 6661 6365  avities, surface
-00017e00: 2c20 7665 7274 6963 6573 2c20 423d 6465  , vertices, B=de
-00017e10: 7074 6873 290a 0a20 2020 202a 2045 7870  pths)..    * Exp
-00017e20: 6f72 7420 7375 7266 6163 6520 706f 696e  ort surface poin
-00017e30: 7473 2077 6974 6820 6879 6472 6f70 686f  ts with hydropho
-00017e40: 6269 6369 7479 5f73 6361 6c65 206d 6170  bicity_scale map
-00017e50: 7065 6420 6f6e 2074 6865 6d0a 0a20 2020  ped on them..   
-00017e60: 203e 3e3e 2065 7870 6f72 7428 4e6f 6e65   >>> export(None
-00017e70: 2c20 4e6f 6e65 2c20 7375 7266 6163 652c  , None, surface,
-00017e80: 2076 6572 7469 6365 732c 206f 7574 7075   vertices, outpu
-00017e90: 745f 6879 6472 6f70 6174 6879 3d27 6879  t_hydropathy='hy
-00017ea0: 6472 6f70 6174 6879 2e70 6462 272c 2073  dropathy.pdb', s
-00017eb0: 6361 6c65 733d 7363 616c 6573 290a 0a20  cales=scales).. 
-00017ec0: 2020 202a 2045 7870 6f72 7420 616c 6c0a     * Export all.
-00017ed0: 0a20 2020 203e 3e3e 2065 7870 6f72 7428  .    >>> export(
-00017ee0: 2763 6176 6974 6965 732e 7064 6227 2c20  'cavities.pdb', 
-00017ef0: 6361 7669 7469 6573 2c20 7375 7266 6163  cavities, surfac
-00017f00: 652c 2076 6572 7469 6365 732c 2042 3d64  e, vertices, B=d
-00017f10: 6570 7468 732c 206f 7574 7075 745f 6879  epths, output_hy
-00017f20: 6472 6f70 6174 6879 3d27 6879 6472 6f70  dropathy='hydrop
-00017f30: 6174 6879 2e70 6462 272c 2073 6361 6c65  athy.pdb', scale
-00017f40: 733d 7363 616c 6573 290a 0a20 2020 2022  s=scales)..    "
-00017f50: 2222 0a20 2020 2066 726f 6d20 5f70 794b  "".    from _pyK
-00017f60: 5646 696e 6465 7220 696d 706f 7274 205f  VFinder import _
-00017f70: 6578 706f 7274 2c20 5f65 7870 6f72 745f  export, _export_
-00017f80: 620a 0a20 2020 2023 2043 6865 636b 2061  b..    # Check a
-00017f90: 7267 756d 656e 7473 0a20 2020 2069 6620  rguments.    if 
-00017fa0: 666e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  fn is not None:.
-00017fb0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-00017fc0: 666e 2920 6e6f 7420 696e 205b 7374 722c  fn) not in [str,
-00017fd0: 2070 6174 686c 6962 2e50 6174 685d 3a0a   pathlib.Path]:.
-00017fe0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00017ff0: 6520 5479 7065 4572 726f 7228 2260 666e  e TypeError("`fn
-00018000: 6020 6d75 7374 2062 6520 6120 7374 7269  ` must be a stri
-00018010: 6e67 206f 7220 6120 7061 7468 6c69 622e  ng or a pathlib.
-00018020: 5061 7468 2e22 290a 2020 2020 2020 2020  Path.").        
-00018030: 6f73 2e6d 616b 6564 6972 7328 6f73 2e70  os.makedirs(os.p
-00018040: 6174 682e 6162 7370 6174 6828 6f73 2e70  ath.abspath(os.p
-00018050: 6174 682e 6469 726e 616d 6528 666e 2929  ath.dirname(fn))
-00018060: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
-00018070: 0a20 2020 2069 6620 6361 7669 7469 6573  .    if cavities
-00018080: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00018090: 2020 2020 2020 6966 2074 7970 6528 6361        if type(ca
-000180a0: 7669 7469 6573 2920 6e6f 7420 696e 205b  vities) not in [
-000180b0: 6e75 6d70 792e 6e64 6172 7261 795d 3a0a  numpy.ndarray]:.
-000180c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000180d0: 6520 5479 7065 4572 726f 7228 2260 6361  e TypeError("`ca
-000180e0: 7669 7469 6573 6020 6d75 7374 2062 6520  vities` must be 
-000180f0: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
-00018100: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-00018110: 6c65 6e28 6361 7669 7469 6573 2e73 6861  len(cavities.sha
-00018120: 7065 2920 213d 2033 3a0a 2020 2020 2020  pe) != 3:.      
-00018130: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00018140: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00018150: 2020 2020 2020 2020 2260 6361 7669 7469          "`caviti
-00018160: 6573 6020 6861 7320 7468 6520 696e 636f  es` has the inco
-00018170: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
-00018180: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
-00018190: 206e 7a29 2e22 0a20 2020 2020 2020 2020   nz).".         
-000181a0: 2020 2029 0a20 2020 2069 6620 7375 7266     ).    if surf
-000181b0: 6163 6520 6973 206e 6f74 204e 6f6e 653a  ace is not None:
-000181c0: 0a20 2020 2020 2020 2069 6620 7479 7065  .        if type
-000181d0: 2873 7572 6661 6365 2920 6e6f 7420 696e  (surface) not in
-000181e0: 205b 6e75 6d70 792e 6e64 6172 7261 795d   [numpy.ndarray]
-000181f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00018200: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-00018210: 7375 7266 6163 6560 206d 7573 7420 6265  surface` must be
-00018220: 2061 206e 756d 7079 2e6e 6461 7272 6179   a numpy.ndarray
-00018230: 2e22 290a 2020 2020 2020 2020 656c 6966  .").        elif
-00018240: 206c 656e 2873 7572 6661 6365 2e73 6861   len(surface.sha
-00018250: 7065 2920 213d 2033 3a0a 2020 2020 2020  pe) != 3:.      
-00018260: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00018270: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00018280: 2020 2020 2020 2020 2260 7375 7266 6163          "`surfac
-00018290: 6560 2068 6173 2074 6865 2069 6e63 6f72  e` has the incor
-000182a0: 7265 6374 2073 6861 7065 2e20 4974 206d  rect shape. It m
-000182b0: 7573 7420 6265 2028 6e78 2c20 6e79 2c20  ust be (nx, ny, 
-000182c0: 6e7a 292e 220a 2020 2020 2020 2020 2020  nz).".          
-000182d0: 2020 290a 2020 2020 6966 2074 7970 6528    ).    if type(
-000182e0: 7665 7274 6963 6573 2920 6e6f 7420 696e  vertices) not in
-000182f0: 205b 6e75 6d70 792e 6e64 6172 7261 792c   [numpy.ndarray,
-00018300: 206c 6973 745d 3a0a 2020 2020 2020 2020   list]:.        
-00018310: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00018320: 2260 7665 7274 6963 6573 6020 6d75 7374  "`vertices` must
-00018330: 2062 6520 6120 6c69 7374 206f 7220 6120   be a list or a 
-00018340: 6e75 6d70 792e 6e64 6172 7261 792e 2229  numpy.ndarray.")
-00018350: 0a20 2020 2065 6c69 6620 6e75 6d70 792e  .    elif numpy.
-00018360: 6173 6172 7261 7928 7665 7274 6963 6573  asarray(vertices
-00018370: 292e 7368 6170 6520 213d 2028 342c 2033  ).shape != (4, 3
-00018380: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00018390: 2056 616c 7565 4572 726f 7228 2260 7665   ValueError("`ve
-000183a0: 7274 6963 6573 6020 6861 7320 696e 636f  rtices` has inco
-000183b0: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
-000183c0: 6d75 7374 2062 6520 2834 2c20 3329 2e22  must be (4, 3)."
-000183d0: 290a 2020 2020 6966 2074 7970 6528 7374  ).    if type(st
-000183e0: 6570 2920 6e6f 7420 696e 205b 666c 6f61  ep) not in [floa
-000183f0: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
-00018400: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-00018410: 2822 6073 7465 7060 206d 7573 7420 6265  ("`step` must be
-00018420: 2061 2070 6f73 6974 6976 6520 7265 616c   a positive real
-00018430: 206e 756d 6265 722e 2229 0a20 2020 2065   number.").    e
-00018440: 6c69 6620 7374 6570 203c 3d20 302e 303a  lif step <= 0.0:
-00018450: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00018460: 616c 7565 4572 726f 7228 2260 7374 6570  alueError("`step
-00018470: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
-00018480: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
-00018490: 2e22 290a 2020 2020 6966 2042 2069 7320  .").    if B is 
-000184a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000184b0: 2020 6966 2074 7970 6528 4229 206e 6f74    if type(B) not
-000184c0: 2069 6e20 5b6e 756d 7079 2e6e 6461 7272   in [numpy.ndarr
-000184d0: 6179 5d3a 0a20 2020 2020 2020 2020 2020  ay]:.           
-000184e0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000184f0: 2822 6042 6020 6d75 7374 2062 6520 6120  ("`B` must be a 
-00018500: 6e75 6d70 792e 6e64 6172 7261 792e 2229  numpy.ndarray.")
-00018510: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
-00018520: 6e28 422e 7368 6170 6529 2021 3d20 333a  n(B.shape) != 3:
-00018530: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00018540: 7365 2056 616c 7565 4572 726f 7228 2260  se ValueError("`
-00018550: 4260 2068 6173 2074 6865 2069 6e63 6f72  B` has the incor
-00018560: 7265 6374 2073 6861 7065 2e20 4974 206d  rect shape. It m
-00018570: 7573 7420 6265 2028 6e78 2c20 6e79 2c20  ust be (nx, ny, 
-00018580: 6e7a 292e 2229 0a20 2020 2069 6620 6f75  nz).").    if ou
-00018590: 7470 7574 5f68 7964 726f 7061 7468 7920  tput_hydropathy 
-000185a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000185b0: 2020 2020 2069 6620 7479 7065 286f 7574       if type(out
-000185c0: 7075 745f 6879 6472 6f70 6174 6879 2920  put_hydropathy) 
-000185d0: 6e6f 7420 696e 205b 7374 722c 2070 6174  not in [str, pat
-000185e0: 686c 6962 2e50 6174 685d 3a0a 2020 2020  hlib.Path]:.    
-000185f0: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-00018600: 7065 4572 726f 7228 2260 6f75 7470 7574  peError("`output
-00018610: 5f68 7964 726f 7061 7468 7960 206d 7573  _hydropathy` mus
-00018620: 7420 6265 2061 2073 7472 696e 6720 6f72  t be a string or
-00018630: 2061 2070 6174 686c 6962 2e50 6174 682e   a pathlib.Path.
-00018640: 2229 0a20 2020 2020 2020 206f 732e 6d61  ").        os.ma
-00018650: 6b65 6469 7273 286f 732e 7061 7468 2e61  kedirs(os.path.a
-00018660: 6273 7061 7468 286f 732e 7061 7468 2e64  bspath(os.path.d
-00018670: 6972 6e61 6d65 286f 7574 7075 745f 6879  irname(output_hy
-00018680: 6472 6f70 6174 6879 2929 2c20 6578 6973  dropathy)), exis
-00018690: 745f 6f6b 3d54 7275 6529 0a20 2020 2069  t_ok=True).    i
-000186a0: 6620 7363 616c 6573 2069 7320 6e6f 7420  f scales is not 
-000186b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-000186c0: 2074 7970 6528 7363 616c 6573 2920 6e6f   type(scales) no
-000186d0: 7420 696e 205b 6e75 6d70 792e 6e64 6172  t in [numpy.ndar
-000186e0: 7261 795d 3a0a 2020 2020 2020 2020 2020  ray]:.          
-000186f0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-00018700: 7228 2260 7363 616c 6573 6020 6d75 7374  r("`scales` must
-00018710: 2062 6520 6120 6e75 6d70 792e 6e64 6172   be a numpy.ndar
-00018720: 7261 792e 2229 0a20 2020 2020 2020 2065  ray.").        e
-00018730: 6c69 6620 6c65 6e28 7363 616c 6573 2e73  lif len(scales.s
-00018740: 6861 7065 2920 213d 2033 3a0a 2020 2020  hape) != 3:.    
-00018750: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00018760: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00018770: 2020 2020 2020 2020 2020 2260 7363 616c            "`scal
-00018780: 6573 6020 6861 7320 7468 6520 696e 636f  es` has the inco
-00018790: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
-000187a0: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
-000187b0: 206e 7a29 2e22 0a20 2020 2020 2020 2020   nz).".         
-000187c0: 2020 2029 0a20 2020 2069 6620 7365 6c65     ).    if sele
-000187d0: 6374 696f 6e20 6973 206e 6f74 204e 6f6e  ction is not Non
-000187e0: 653a 0a20 2020 2020 2020 2023 2043 6865  e:.        # Che
-000187f0: 636b 2073 656c 6563 7469 6f6e 2074 7970  ck selection typ
-00018800: 6573 0a20 2020 2020 2020 2069 6620 616c  es.        if al
-00018810: 6c28 6973 696e 7374 616e 6365 2878 2c20  l(isinstance(x, 
-00018820: 696e 7429 2066 6f72 2078 2069 6e20 7365  int) for x in se
-00018830: 6c65 6374 696f 6e29 3a0a 2020 2020 2020  lection):.      
-00018840: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00018850: 2020 2065 6c69 6620 616c 6c28 6973 696e     elif all(isin
-00018860: 7374 616e 6365 2878 2c20 7374 7229 2066  stance(x, str) f
-00018870: 6f72 2078 2069 6e20 7365 6c65 6374 696f  or x in selectio
-00018880: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00018890: 7365 6c65 6374 696f 6e20 3d20 5b5f 6765  selection = [_ge
-000188a0: 745f 6361 7669 7479 5f6c 6162 656c 2873  t_cavity_label(s
-000188b0: 656c 6529 2066 6f72 2073 656c 6520 696e  ele) for sele in
-000188c0: 2073 656c 6563 7469 6f6e 5d0a 2020 2020   selection].    
-000188d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000188e0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-000188f0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00018900: 2020 2020 2020 2022 6073 656c 6563 7469         "`selecti
-00018910: 6f6e 6020 6d75 7374 2062 6520 6120 6c69  on` must be a li
-00018920: 7374 206f 6620 7374 7269 6e67 7320 2863  st of strings (c
-00018930: 6176 6974 7920 6e61 6d65 7329 206f 7220  avity names) or 
-00018940: 696e 7465 6765 7273 2028 6361 7669 7479  integers (cavity
-00018950: 206c 6162 656c 7329 2e22 0a20 2020 2020   labels).".     
-00018960: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018970: 2023 2043 6865 636b 2069 6620 7365 6c65   # Check if sele
-00018980: 6374 696f 6e20 696e 636c 7564 6573 2076  ction includes v
-00018990: 616c 6964 2063 6176 6974 7920 6c61 6265  alid cavity labe
-000189a0: 6c73 0a20 2020 2020 2020 2069 6620 616e  ls.        if an
-000189b0: 7928 7820 3c20 3220 666f 7220 7820 696e  y(x < 2 for x in
-000189c0: 2073 656c 6563 7469 6f6e 293a 0a20 2020   selection):.   
-000189d0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000189e0: 616c 7565 4572 726f 7228 6622 496e 7661  alueError(f"Inva
-000189f0: 6c69 6420 6073 656c 6563 7469 6f6e 603a  lid `selection`:
-00018a00: 207b 7365 6c65 6374 696f 6e7d 2e22 290a   {selection}.").
-00018a10: 2020 2020 6966 206e 7468 7265 6164 7320      if nthreads 
-00018a20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00018a30: 206e 7468 7265 6164 7320 3d20 6f73 2e63   nthreads = os.c
-00018a40: 7075 5f63 6f75 6e74 2829 202d 2031 0a20  pu_count() - 1. 
-00018a50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00018a60: 2069 6620 7479 7065 286e 7468 7265 6164   if type(nthread
-00018a70: 7329 206e 6f74 2069 6e20 5b69 6e74 5d3a  s) not in [int]:
-00018a80: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00018a90: 7365 2054 7970 6545 7272 6f72 2822 606e  se TypeError("`n
-00018aa0: 7468 7265 6164 7360 206d 7573 7420 6265  threads` must be
-00018ab0: 2061 2070 6f73 6974 6976 6520 696e 7465   a positive inte
-00018ac0: 6765 722e 2229 0a20 2020 2020 2020 2065  ger.").        e
-00018ad0: 6c69 6620 6e74 6872 6561 6473 203c 3d20  lif nthreads <= 
-00018ae0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00018af0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00018b00: 2260 6e74 6872 6561 6473 6020 6d75 7374  "`nthreads` must
-00018b10: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
-00018b20: 6e74 6567 6572 2e22 290a 2020 2020 6966  nteger.").    if
-00018b30: 2074 7970 6528 6170 7065 6e64 2920 6e6f   type(append) no
-00018b40: 7420 696e 205b 626f 6f6c 5d3a 0a20 2020  t in [bool]:.   
-00018b50: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-00018b60: 7272 6f72 2822 6061 7070 656e 6460 206d  rror("`append` m
-00018b70: 7573 7420 6265 2061 2062 6f6f 6c65 616e  ust be a boolean
-00018b80: 2e22 290a 2020 2020 6966 2074 7970 6528  .").    if type(
-00018b90: 6d6f 6465 6c29 206e 6f74 2069 6e20 5b69  model) not in [i
-00018ba0: 6e74 5d3a 0a20 2020 2020 2020 2072 6169  nt]:.        rai
-00018bb0: 7365 2054 7970 6545 7272 6f72 2822 606d  se TypeError("`m
-00018bc0: 6f64 656c 6020 6d75 7374 2062 6520 6120  odel` must be a 
-00018bd0: 696e 7465 6765 722e 2229 0a0a 2020 2020  integer.")..    
-00018be0: 2320 436f 6e76 6572 7420 7479 7065 730a  # Convert types.
-00018bf0: 2020 2020 6966 2074 7970 6528 7665 7274      if type(vert
-00018c00: 6963 6573 2920 3d3d 206c 6973 743a 0a20  ices) == list:. 
-00018c10: 2020 2020 2020 2076 6572 7469 6365 7320         vertices 
-00018c20: 3d20 6e75 6d70 792e 6173 6172 7261 7928  = numpy.asarray(
-00018c30: 7665 7274 6963 6573 290a 2020 2020 6966  vertices).    if
-00018c40: 2074 7970 6528 7374 6570 2920 3d3d 2069   type(step) == i
-00018c50: 6e74 3a0a 2020 2020 2020 2020 7374 6570  nt:.        step
-00018c60: 203d 2066 6c6f 6174 2873 7465 7029 0a0a   = float(step)..
-00018c70: 2020 2020 2320 436f 6e76 6572 7420 6e75      # Convert nu
-00018c80: 6d70 792e 6e64 6172 7261 7920 6461 7461  mpy.ndarray data
-00018c90: 2074 7970 6573 0a20 2020 2076 6572 7469   types.    verti
-00018ca0: 6365 7320 3d20 7665 7274 6963 6573 2e61  ces = vertices.a
-00018cb0: 7374 7970 6528 2266 6c6f 6174 3634 2229  stype("float64")
-00018cc0: 2069 6620 7665 7274 6963 6573 2e64 7479   if vertices.dty
-00018cd0: 7065 2021 3d20 2266 6c6f 6174 3634 2220  pe != "float64" 
-00018ce0: 656c 7365 2076 6572 7469 6365 730a 2020  else vertices.  
-00018cf0: 2020 6966 2042 2069 7320 6e6f 7420 4e6f    if B is not No
-00018d00: 6e65 3a0a 2020 2020 2020 2020 4220 3d20  ne:.        B = 
-00018d10: 422e 6173 7479 7065 2822 666c 6f61 7436  B.astype("float6
-00018d20: 3422 2920 6966 2042 2e64 7479 7065 2021  4") if B.dtype !
-00018d30: 3d20 2266 6c6f 6174 3634 2220 656c 7365  = "float64" else
-00018d40: 2042 0a20 2020 2069 6620 7363 616c 6573   B.    if scales
-00018d50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00018d60: 2020 2020 2020 7363 616c 6573 203d 2073        scales = s
-00018d70: 6361 6c65 732e 6173 7479 7065 2822 666c  cales.astype("fl
-00018d80: 6f61 7436 3422 2920 6966 2073 6361 6c65  oat64") if scale
-00018d90: 732e 6474 7970 6520 213d 2022 666c 6f61  s.dtype != "floa
-00018da0: 7436 3422 2065 6c73 6520 7363 616c 6573  t64" else scales
-00018db0: 0a0a 2020 2020 2320 4765 7420 7369 6e63  ..    # Get sinc
-00018dc0: 6f73 3a20 7369 6e65 2061 6e64 2063 6f73  os: sine and cos
-00018dd0: 7369 6e65 206f 6620 7468 6520 6772 6964  sine of the grid
-00018de0: 2072 6f74 6174 696f 6e20 616e 676c 6573   rotation angles
-00018df0: 2028 7369 6e61 2c20 636f 7361 2c20 7369   (sina, cosa, si
-00018e00: 6e62 2c20 636f 7362 290a 2020 2020 7369  nb, cosb).    si
-00018e10: 6e63 6f73 203d 205f 6765 745f 7369 6e63  ncos = _get_sinc
-00018e20: 6f73 2876 6572 7469 6365 7329 0a0a 2020  os(vertices)..  
-00018e30: 2020 2320 556e 7061 636b 2076 6572 7469    # Unpack verti
-00018e40: 6365 730a 2020 2020 5031 2c20 5032 2c20  ces.    P1, P2, 
-00018e50: 5033 2c20 5034 203d 2076 6572 7469 6365  P3, P4 = vertice
-00018e60: 730a 0a20 2020 2023 2049 6620 7375 7266  s..    # If surf
-00018e70: 6163 6520 6973 204e 6f6e 652c 2063 7265  ace is None, cre
-00018e80: 6174 6520 616e 2065 6d70 7479 2067 7269  ate an empty gri
-00018e90: 640a 2020 2020 6966 2063 6176 6974 6965  d.    if cavitie
-00018ea0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00018eb0: 2020 2020 2020 2069 6620 7375 7266 6163         if surfac
-00018ec0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00018ed0: 2020 2020 2020 2073 7572 6661 6365 203d         surface =
-00018ee0: 206e 756d 7079 2e7a 6572 6f73 2863 6176   numpy.zeros(cav
-00018ef0: 6974 6965 732e 7368 6170 652c 2064 7479  ities.shape, dty
-00018f00: 7065 3d22 696e 7433 3222 290a 2020 2020  pe="int32").    
-00018f10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00018f20: 2020 2020 2020 7375 7266 6163 6520 3d20        surface = 
-00018f30: 7375 7266 6163 652e 6173 7479 7065 2822  surface.astype("
-00018f40: 696e 7433 3222 2920 6966 2073 7572 6661  int32") if surfa
-00018f50: 6365 2e64 7479 7065 2021 3d20 2269 6e74  ce.dtype != "int
-00018f60: 3332 2220 656c 7365 2073 7572 6661 6365  32" else surface
-00018f70: 0a0a 2020 2020 2320 5365 6c65 6374 2063  ..    # Select c
-00018f80: 6176 6974 6965 730a 2020 2020 6966 2073  avities.    if s
-00018f90: 656c 6563 7469 6f6e 2069 7320 6e6f 7420  election is not 
-00018fa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7375  None:.        su
-00018fb0: 7266 6163 6520 3d20 5f73 656c 6563 745f  rface = _select_
-00018fc0: 6361 7669 7469 6573 2873 7572 6661 6365  cavities(surface
-00018fd0: 2c20 7365 6c65 6374 696f 6e29 0a20 2020  , selection).   
-00018fe0: 2020 2020 2069 6620 6361 7669 7469 6573       if cavities
-00018ff0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00019000: 2020 2020 2020 2020 2020 6361 7669 7469            caviti
-00019010: 6573 203d 205f 7365 6c65 6374 5f63 6176  es = _select_cav
-00019020: 6974 6965 7328 6361 7669 7469 6573 2c20  ities(cavities, 
-00019030: 7365 6c65 6374 696f 6e29 0a0a 2020 2020  selection)..    
-00019040: 6966 2063 6176 6974 6965 7320 6973 204e  if cavities is N
-00019050: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-00019060: 7375 7266 6163 6520 6973 204e 6f6e 653a  surface is None:
-00019070: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00019080: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-00019090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190a0: 2066 2255 7365 7220 6d75 7374 2064 6566   f"User must def
-000190b0: 696e 6520 6073 7572 6661 6365 6020 7768  ine `surface` wh
-000190c0: 656e 206e 6f74 2064 6566 696e 696e 6720  en not defining 
-000190d0: 6063 6176 6974 6965 7360 2e22 0a20 2020  `cavities`.".   
-000190e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000190f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00019100: 2020 2020 2023 2047 6574 206e 756d 6265       # Get numbe
-00019110: 7220 6f66 2063 6176 6974 6965 730a 2020  r of cavities.  
-00019120: 2020 2020 2020 2020 2020 6e63 6176 203d            ncav =
-00019130: 2069 6e74 2873 7572 6661 6365 2e6d 6178   int(surface.max
-00019140: 2829 202d 2031 290a 0a20 2020 2020 2020  () - 1)..       
-00019150: 2020 2020 2023 2045 7870 6f72 7420 6879       # Export hy
-00019160: 6472 6f70 6174 6879 0a20 2020 2020 2020  dropathy.       
-00019170: 2020 2020 205f 6578 706f 7274 5f62 280a       _export_b(.
-00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019190: 6f75 7470 7574 5f68 7964 726f 7061 7468  output_hydropath
-000191a0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-000191b0: 2020 2073 7572 6661 6365 2c0a 2020 2020     surface,.    
-000191c0: 2020 2020 2020 2020 2020 2020 7375 7266              surf
-000191d0: 6163 652c 0a20 2020 2020 2020 2020 2020  ace,.           
-000191e0: 2020 2020 2073 6361 6c65 732c 0a20 2020       scales,.   
-000191f0: 2020 2020 2020 2020 2020 2020 2050 312c               P1,
-00019200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019210: 2073 696e 636f 732c 0a20 2020 2020 2020   sincos,.       
-00019220: 2020 2020 2020 2020 2073 7465 702c 0a20           step,. 
-00019230: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00019240: 6361 762c 0a20 2020 2020 2020 2020 2020  cav,.           
-00019250: 2020 2020 206e 7468 7265 6164 732c 0a20       nthreads,. 
-00019260: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019270: 7070 656e 642c 0a20 2020 2020 2020 2020  ppend,.         
-00019280: 2020 2020 2020 206d 6f64 656c 2c0a 2020         model,.  
-00019290: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000192a0: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
-000192b0: 4368 6563 6b20 616e 6420 636f 6e76 6572  Check and conver
-000192c0: 7420 6361 7669 7469 6573 2064 7479 7065  t cavities dtype
-000192d0: 0a20 2020 2020 2020 2063 6176 6974 6965  .        cavitie
-000192e0: 7320 3d20 6361 7669 7469 6573 2e61 7374  s = cavities.ast
-000192f0: 7970 6528 2269 6e74 3332 2229 2069 6620  ype("int32") if 
-00019300: 6361 7669 7469 6573 2e64 7479 7065 2021  cavities.dtype !
-00019310: 3d20 2269 6e74 3332 2220 656c 7365 2063  = "int32" else c
-00019320: 6176 6974 6965 730a 0a20 2020 2020 2020  avities..       
-00019330: 2023 2047 6574 206e 756d 6265 7220 6f66   # Get number of
-00019340: 2063 6176 6974 6965 730a 2020 2020 2020   cavities.      
-00019350: 2020 6e63 6176 203d 2069 6e74 2863 6176    ncav = int(cav
-00019360: 6974 6965 732e 6d61 7828 2920 2d20 3129  ities.max() - 1)
-00019370: 0a0a 2020 2020 2020 2020 2320 4578 706f  ..        # Expo
-00019380: 7274 2063 6176 6974 6965 730a 2020 2020  rt cavities.    
-00019390: 2020 2020 6966 2042 2069 7320 4e6f 6e65      if B is None
-000193a0: 3a0a 2020 2020 2020 2020 2020 2020 5f65  :.            _e
-000193b0: 7870 6f72 7428 0a20 2020 2020 2020 2020  xport(.         
-000193c0: 2020 2020 2020 2066 6e2c 2063 6176 6974         fn, cavit
-000193d0: 6965 732c 2073 7572 6661 6365 2c20 5031  ies, surface, P1
-000193e0: 2c20 7369 6e63 6f73 2c20 7374 6570 2c20  , sincos, step, 
-000193f0: 6e63 6176 2c20 6e74 6872 6561 6473 2c20  ncav, nthreads, 
-00019400: 6170 7065 6e64 2c20 6d6f 6465 6c0a 2020  append, model.  
-00019410: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00019420: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00019430: 2020 2020 2020 5f65 7870 6f72 745f 6228        _export_b(
-00019440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019450: 2066 6e2c 0a20 2020 2020 2020 2020 2020   fn,.           
-00019460: 2020 2020 2063 6176 6974 6965 732c 0a20       cavities,. 
-00019470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019480: 7572 6661 6365 2c0a 2020 2020 2020 2020  urface,.        
-00019490: 2020 2020 2020 2020 422c 0a20 2020 2020          B,.     
-000194a0: 2020 2020 2020 2020 2020 2050 312c 0a20             P1,. 
-000194b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000194c0: 696e 636f 732c 0a20 2020 2020 2020 2020  incos,.         
-000194d0: 2020 2020 2020 2073 7465 702c 0a20 2020         step,.   
-000194e0: 2020 2020 2020 2020 2020 2020 206e 6361               nca
-000194f0: 762c 0a20 2020 2020 2020 2020 2020 2020  v,.             
-00019500: 2020 206e 7468 7265 6164 732c 0a20 2020     nthreads,.   
-00019510: 2020 2020 2020 2020 2020 2020 2061 7070               app
-00019520: 656e 642c 0a20 2020 2020 2020 2020 2020  end,.           
-00019530: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
-00019540: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00019550: 2020 2023 2045 7870 6f72 7420 6879 6472     # Export hydr
-00019560: 6f70 6174 6879 2073 7572 6661 6365 2070  opathy surface p
-00019570: 6f69 6e74 730a 2020 2020 2020 2020 6966  oints.        if
-00019580: 2073 6361 6c65 7320 6973 204e 6f6e 653a   scales is None:
-00019590: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-000195a0: 730a 2020 2020 2020 2020 656c 7365 3a0a  s.        else:.
-000195b0: 2020 2020 2020 2020 2020 2020 5f65 7870              _exp
-000195c0: 6f72 745f 6228 0a20 2020 2020 2020 2020  ort_b(.         
-000195d0: 2020 2020 2020 206f 7574 7075 745f 6879         output_hy
-000195e0: 6472 6f70 6174 6879 2c0a 2020 2020 2020  dropathy,.      
-000195f0: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
-00019600: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00019610: 2020 2073 7572 6661 6365 2c0a 2020 2020     surface,.    
-00019620: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-00019630: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00019640: 2020 2020 5031 2c0a 2020 2020 2020 2020      P1,.        
-00019650: 2020 2020 2020 2020 7369 6e63 6f73 2c0a          sincos,.
-00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019670: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
-00019680: 2020 2020 2020 6e63 6176 2c0a 2020 2020        ncav,.    
-00019690: 2020 2020 2020 2020 2020 2020 6e74 6872              nthr
-000196a0: 6561 6473 2c0a 2020 2020 2020 2020 2020  eads,.          
-000196b0: 2020 2020 2020 6170 7065 6e64 2c0a 2020        append,.  
-000196c0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-000196d0: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
-000196e0: 2029 0a0a 0a64 6566 2065 7870 6f72 745f   )...def export_
-000196f0: 6f70 656e 696e 6773 280a 2020 2020 666e  openings(.    fn
-00019700: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
-00019710: 686c 6962 2e50 6174 685d 2c0a 2020 2020  hlib.Path],.    
-00019720: 6f70 656e 696e 6773 3a20 6e75 6d70 792e  openings: numpy.
-00019730: 6e64 6172 7261 792c 0a20 2020 2076 6572  ndarray,.    ver
-00019740: 7469 6365 733a 2055 6e69 6f6e 5b6e 756d  tices: Union[num
-00019750: 7079 2e6e 6461 7272 6179 2c20 4c69 7374  py.ndarray, List
-00019760: 5b4c 6973 745b 666c 6f61 745d 5d5d 2c0a  [List[float]]],.
-00019770: 2020 2020 7374 6570 3a20 556e 696f 6e5b      step: Union[
-00019780: 666c 6f61 742c 2069 6e74 5d20 3d20 302e  float, int] = 0.
-00019790: 362c 0a20 2020 2073 656c 6563 7469 6f6e  6,.    selection
-000197a0: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
-000197b0: 5b4c 6973 745b 696e 745d 2c20 4c69 7374  [List[int], List
-000197c0: 5b73 7472 5d5d 5d20 3d20 4e6f 6e65 2c0a  [str]]] = None,.
-000197d0: 2020 2020 6e74 6872 6561 6473 3a20 4f70      nthreads: Op
-000197e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000197f0: 6e65 2c0a 2020 2020 6170 7065 6e64 3a20  ne,.    append: 
-00019800: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00019810: 2020 6d6f 6465 6c3a 2069 6e74 203d 2030    model: int = 0
-00019820: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-00019830: 2022 2222 4578 706f 7274 206f 7065 6e69   """Export openi
-00019840: 6e67 2070 6f69 6e74 7320 2848 2920 746f  ng points (H) to
-00019850: 2061 2050 4442 2d66 6f72 6d61 7474 6564   a PDB-formatted
-00019860: 2066 696c 652e 0a0a 2020 2020 5061 7261   file...    Para
-00019870: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00019880: 2d2d 2d2d 2d0a 2020 2020 666e 203a 2055  -----.    fn : U
-00019890: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-000198a0: 622e 5061 7468 5d0a 2020 2020 2020 2020  b.Path].        
-000198b0: 4120 7061 7468 2074 6f20 5044 4220 6669  A path to PDB fi
-000198c0: 6c65 2066 6f72 2077 7269 7469 6e67 206f  le for writing o
-000198d0: 7065 6e69 6e67 732e 0a20 2020 206f 7065  penings..    ope
-000198e0: 6e69 6e67 7320 3a20 6e75 6d70 792e 6e64  nings : numpy.nd
-000198f0: 6172 7261 790a 2020 2020 2020 2020 4f70  array.        Op
-00019900: 656e 696e 6773 2070 6f69 6e74 7320 696e  enings points in
-00019910: 2074 6865 2033 4420 6772 6964 2028 6f70   the 3D grid (op
-00019920: 656e 696e 6773 5b6e 785d 5b6e 795d 5b6e  enings[nx][ny][n
-00019930: 7a5d 292e 0a20 2020 2020 2020 204f 7065  z])..        Ope
-00019940: 6e69 6e67 7320 6172 7261 7920 6861 7320  nings array has 
-00019950: 696e 7465 6765 7220 6c61 6265 6c73 2069  integer labels i
-00019960: 6e20 6561 6368 2070 6f73 6974 696f 6e2c  n each position,
-00019970: 2074 6861 7420 6172 653a 0a0a 2020 2020   that are:..    
-00019980: 2020 2020 2020 2020 2a20 2d31 3a20 6275          * -1: bu
-00019990: 6c6b 2070 6f69 6e74 733b 0a0a 2020 2020  lk points;..    
-000199a0: 2020 2020 2020 2020 2a20 303a 2063 6176          * 0: cav
-000199b0: 6974 7920 6f72 2062 696f 6d6f 6c65 6375  ity or biomolecu
-000199c0: 6c65 2070 6f69 6e74 733b 0a0a 2020 2020  le points;..    
-000199d0: 2020 2020 2020 2020 2a20 313a 2065 6d70          * 1: emp
-000199e0: 7479 2073 7061 6365 2070 6f69 6e74 733b  ty space points;
-000199f0: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-00019a00: 3e3d 323a 204f 7065 6e69 6e67 2070 6f69  >=2: Opening poi
-00019a10: 6e74 732e 0a0a 2020 2020 2020 2020 5468  nts...        Th
-00019a20: 6520 656d 7074 7920 7370 6163 6520 706f  e empty space po
-00019a30: 696e 7473 2061 7265 2072 6567 696f 6e73  ints are regions
-00019a40: 2074 6861 7420 646f 206e 6f74 206d 6565   that do not mee
-00019a50: 7420 7468 6520 6368 6f73 656e 0a20 2020  t the chosen.   
-00019a60: 2020 2020 206f 7065 6e69 6e67 7320 6375       openings cu
-00019a70: 746f 6666 2074 6f20 6265 2063 6f6e 7369  toff to be consi
-00019a80: 6465 7265 6420 616e 206f 7065 6e69 6e67  dered an opening
-00019a90: 2e0a 2020 2020 7665 7274 6963 6573 203a  ..    vertices :
-00019aa0: 2055 6e69 6f6e 5b6e 756d 7079 2e6e 6461   Union[numpy.nda
-00019ab0: 7272 6179 2c20 4c69 7374 5b4c 6973 745b  rray, List[List[
-00019ac0: 666c 6f61 745d 5d5d 0a20 2020 2020 2020  float]]].       
-00019ad0: 2041 206e 756d 7079 2e6e 6461 7272 6179   A numpy.ndarray
-00019ae0: 206f 7220 6120 6c69 7374 2077 6974 6820   or a list with 
-00019af0: 7879 7a20 7665 7274 6963 6573 2063 6f6f  xyz vertices coo
-00019b00: 7264 696e 6174 6573 2028 6f72 6967 696e  rdinates (origin
-00019b10: 2c0a 2020 2020 2020 2020 582d 6178 6973  ,.        X-axis
-00019b20: 2c20 592d 6178 6973 2c20 5a2d 6178 6973  , Y-axis, Z-axis
-00019b30: 292e 0a20 2020 2073 7465 7020 3a20 556e  )..    step : Un
-00019b40: 696f 6e5b 666c 6f61 742c 2069 6e74 5d2c  ion[float, int],
-00019b50: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00019b60: 2020 4772 6964 2073 7061 6369 6e67 2028    Grid spacing (
-00019b70: 4129 2c20 6279 2064 6566 6175 6c74 2030  A), by default 0
-00019b80: 2e36 2e0a 2020 2020 7365 6c65 6374 696f  .6..    selectio
-00019b90: 6e20 3a20 556e 696f 6e5b 4c69 7374 5b69  n : Union[List[i
-00019ba0: 6e74 5d2c 204c 6973 745b 7374 725d 5d2c  nt], List[str]],
-00019bb0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00019bc0: 2020 4120 6c69 7374 206f 6620 696e 7465    A list of inte
-00019bd0: 6765 7220 6c61 6265 6c73 206f 7220 6120  ger labels or a 
-00019be0: 6c69 7374 206f 6620 6f70 656e 696e 6720  list of opening 
-00019bf0: 6e61 6d65 7320 746f 2062 6520 7365 6c65  names to be sele
-00019c00: 6374 6564 2c20 6279 2064 6566 6175 6c74  cted, by default
-00019c10: 204e 6f6e 652e 0a20 2020 206e 7468 7265   None..    nthre
-00019c20: 6164 7320 3a20 696e 742c 206f 7074 696f  ads : int, optio
-00019c30: 6e61 6c0a 2020 2020 2020 2020 4e75 6d62  nal.        Numb
-00019c40: 6572 206f 6620 7468 7265 6164 732c 2062  er of threads, b
-00019c50: 7920 6465 6661 756c 7420 4e6f 6e65 2e20  y default None. 
-00019c60: 4966 204e 6f6e 652c 2074 6865 206e 756d  If None, the num
-00019c70: 6265 7220 6f66 2074 6872 6561 6473 2069  ber of threads i
-00019c80: 730a 2020 2020 2020 2020 606f 732e 6370  s.        `os.cp
-00019c90: 755f 636f 756e 7428 2920 2d20 3160 2e0a  u_count() - 1`..
-00019ca0: 2020 2020 6170 7065 6e64 203a 2062 6f6f      append : boo
-00019cb0: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
-00019cc0: 2020 2020 5768 6574 6865 7220 746f 2061      Whether to a
-00019cd0: 7070 656e 6420 6f70 656e 696e 6773 2074  ppend openings t
-00019ce0: 6f20 7468 6520 5044 4220 6669 6c65 2c20  o the PDB file, 
-00019cf0: 6279 2064 6566 6175 6c74 2046 616c 7365  by default False
-00019d00: 2e0a 2020 2020 6d6f 6465 6c20 3a20 696e  ..    model : in
-00019d10: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-00019d20: 2020 2020 4d6f 6465 6c20 6e75 6d62 6572      Model number
-00019d30: 2c20 6279 2064 6566 6175 6c74 2030 2e0a  , by default 0..
-00019d40: 0a20 2020 2052 6169 7365 730a 2020 2020  .    Raises.    
-00019d50: 2d2d 2d2d 2d2d 0a20 2020 2054 7970 6545  ------.    TypeE
-00019d60: 7272 6f72 0a20 2020 2020 2020 2060 6f70  rror.        `op
-00019d70: 656e 696e 6773 6020 6d75 7374 2062 6520  enings` must be 
-00019d80: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
-00019d90: 0a20 2020 2056 616c 7565 4572 726f 720a  .    ValueError.
-00019da0: 2020 2020 2020 2020 606f 7065 6e69 6e67          `opening
-00019db0: 7360 2068 6173 2074 6865 2069 6e63 6f72  s` has the incor
-00019dc0: 7265 6374 2073 6861 7065 2e20 4974 206d  rect shape. It m
-00019dd0: 7573 7420 6265 2028 6e78 2c20 6e79 2c20  ust be (nx, ny, 
-00019de0: 6e7a 292e 0a20 2020 2054 7970 6545 7272  nz)..    TypeErr
-00019df0: 6f72 0a20 2020 2020 2020 2060 7665 7274  or.        `vert
-00019e00: 6963 6573 6020 6d75 7374 2062 6520 6120  ices` must be a 
-00019e10: 6c69 7374 206f 7220 6120 6e75 6d70 792e  list or a numpy.
-00019e20: 6e64 6172 7261 792e 0a20 2020 2056 616c  ndarray..    Val
-00019e30: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
-00019e40: 6076 6572 7469 6365 7360 2068 6173 2069  `vertices` has i
-00019e50: 6e63 6f72 7265 6374 2073 6861 7065 2e20  ncorrect shape. 
-00019e60: 4974 206d 7573 7420 6265 2028 342c 2033  It must be (4, 3
-00019e70: 292e 0a20 2020 2054 7970 6545 7272 6f72  )..    TypeError
-00019e80: 0a20 2020 2020 2020 2060 7374 6570 6020  .        `step` 
-00019e90: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-00019ea0: 7665 2072 6561 6c20 6e75 6d62 6572 2e0a  ve real number..
-00019eb0: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
-00019ec0: 2020 2020 2020 2060 7374 6570 6020 6d75         `step` mu
-00019ed0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-00019ee0: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
-00019ef0: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
-00019f00: 2020 2020 6073 656c 6563 7469 6f6e 6020      `selection` 
-00019f10: 6d75 7374 2062 6520 6120 6c69 7374 206f  must be a list o
-00019f20: 6620 7374 7269 6e67 7320 286f 7065 6e69  f strings (openi
-00019f30: 6e67 206e 616d 6573 2920 6f72 2069 6e74  ng names) or int
-00019f40: 6567 6572 7320 286f 7065 6e69 6e67 206c  egers (opening l
-00019f50: 6162 656c 7329 2e0a 2020 2020 5661 6c75  abels)..    Valu
-00019f60: 6545 7272 6f72 0a20 2020 2020 2020 2049  eError.        I
-00019f70: 6e76 616c 6964 2060 7365 6c65 6374 696f  nvalid `selectio
-00019f80: 6e60 3a20 7b73 656c 6563 7469 6f6e 7d2e  n`: {selection}.
-00019f90: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
-00019fa0: 2020 2020 2020 2060 6e74 6872 6561 6473         `nthreads
-00019fb0: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
-00019fc0: 7469 7665 2069 6e74 6567 6572 2e0a 2020  tive integer..  
-00019fd0: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
-00019fe0: 2020 2020 2060 6e74 6872 6561 6473 6020       `nthreads` 
-00019ff0: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-0001a000: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
-0001a010: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
-0001a020: 2020 6061 7070 656e 6460 206d 7573 7420    `append` must 
-0001a030: 6265 2061 2062 6f6f 6c65 616e 2e0a 2020  be a boolean..  
-0001a040: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
-0001a050: 2020 2020 606d 6f64 656c 6020 6d75 7374      `model` must
-0001a060: 2062 6520 6120 696e 7465 6765 722e 0a20   be a integer.. 
-0001a070: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
-0001a080: 2020 2020 2060 666e 6020 6d75 7374 2062       `fn` must b
-0001a090: 6520 6120 7374 7269 6e67 206f 7220 7061  e a string or pa
-0001a0a0: 7468 6c69 622e 5061 7468 2e0a 0a20 2020  thlib.Path...   
-0001a0b0: 204e 6f74 650a 2020 2020 2d2d 2d2d 0a20   Note.    ----. 
-0001a0c0: 2020 2054 6865 206f 7065 6e69 6e67 206e     The opening n
-0001a0d0: 6f6d 656e 636c 6174 7572 6520 6973 2062  omenclature is b
-0001a0e0: 6173 6564 206f 6e20 7468 6520 696e 7465  ased on the inte
-0001a0f0: 6765 7220 6c61 6265 6c2e 2054 6865 206f  ger label. The o
-0001a100: 7065 6e69 6e67 206d 6172 6b65 640a 2020  pening marked.  
-0001a110: 2020 7769 7468 2032 2c20 7468 6520 6669    with 2, the fi
-0001a120: 7273 7420 696e 7465 6765 7220 636f 7272  rst integer corr
-0001a130: 6573 706f 6e64 696e 6720 746f 2061 206f  esponding to a o
-0001a140: 7065 6e69 6e67 2c20 6973 204f 4141 2c20  pening, is OAA, 
-0001a150: 7468 6520 6f70 656e 696e 670a 2020 2020  the opening.    
-0001a160: 6d61 726b 6564 2077 6974 6820 3320 6973  marked with 3 is
-0001a170: 204f 4142 2c20 7468 6520 6f70 656e 696e   OAB, the openin
-0001a180: 6720 6d61 726b 6564 2077 6974 6820 3420  g marked with 4 
-0001a190: 6973 204f 4143 2061 6e64 2073 6f20 6f6e  is OAC and so on
-0001a1a0: 2e0a 0a20 2020 2053 6565 2041 6c73 6f0a  ...    See Also.
-0001a1b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0001a1c0: 2065 7870 6f72 740a 2020 2020 6465 7465   export.    dete
-0001a1d0: 6374 0a20 2020 2064 6570 7468 730a 2020  ct.    depths.  
-0001a1e0: 2020 6f70 656e 696e 6773 0a0a 2020 2020    openings..    
-0001a1f0: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
-0001a200: 2d2d 2d0a 2020 2020 5769 7468 2074 6865  ---.    With the
-0001a210: 206f 7065 6e69 6e67 2070 6f69 6e74 7320   opening points 
-0001a220: 6964 656e 7469 6669 6564 2077 6974 6820  identified with 
-0001a230: 6060 6f70 656e 696e 6773 6060 2c20 7765  ``openings``, we
-0001a240: 2063 616e 2065 7870 6f72 7420 7468 656d   can export them
-0001a250: 2074 6f20 6120 5044 422d 666f 726d 6174   to a PDB-format
-0001a260: 7465 6420 6669 6c65 3a0a 0a20 2020 203e  ted file:..    >
-0001a270: 3e3e 2066 726f 6d20 7079 4b56 4669 6e64  >> from pyKVFind
-0001a280: 6572 2069 6d70 6f72 7420 6578 706f 7274  er import export
-0001a290: 5f6f 7065 6e69 6e67 730a 2020 2020 3e3e  _openings.    >>
-0001a2a0: 3e20 6578 706f 7274 5f6f 7065 6e69 6e67  > export_opening
-0001a2b0: 7328 276f 7065 6e69 6e67 732e 7064 6227  s('openings.pdb'
-0001a2c0: 2c20 6f70 656e 696e 6773 2c20 7665 7274  , openings, vert
-0001a2d0: 6963 6573 290a 2020 2020 2222 220a 2020  ices).    """.  
-0001a2e0: 2020 6672 6f6d 205f 7079 4b56 4669 6e64    from _pyKVFind
-0001a2f0: 6572 2069 6d70 6f72 7420 5f65 7870 6f72  er import _expor
-0001a300: 745f 6f70 656e 696e 6773 0a0a 2020 2020  t_openings..    
-0001a310: 2320 4368 6563 6b20 6172 6775 6d65 6e74  # Check argument
-0001a320: 730a 2020 2020 6966 2074 7970 6528 6f70  s.    if type(op
-0001a330: 656e 696e 6773 2920 6e6f 7420 696e 205b  enings) not in [
-0001a340: 6e75 6d70 792e 6e64 6172 7261 795d 3a0a  numpy.ndarray]:.
-0001a350: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-0001a360: 7065 4572 726f 7228 2260 6f70 656e 696e  peError("`openin
-0001a370: 6773 6020 6d75 7374 2062 6520 6120 6e75  gs` must be a nu
-0001a380: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
-0001a390: 2020 2065 6c69 6620 6c65 6e28 6f70 656e     elif len(open
-0001a3a0: 696e 6773 2e73 6861 7065 2920 213d 2033  ings.shape) != 3
-0001a3b0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0001a3c0: 5661 6c75 6545 7272 6f72 2822 606f 7065  ValueError("`ope
-0001a3d0: 6e69 6e67 7360 2068 6173 2074 6865 2069  nings` has the i
-0001a3e0: 6e63 6f72 7265 6374 2073 6861 7065 2e20  ncorrect shape. 
-0001a3f0: 4974 206d 7573 7420 6265 2028 6e78 2c20  It must be (nx, 
-0001a400: 6e79 2c20 6e7a 292e 2229 0a20 2020 2069  ny, nz).").    i
-0001a410: 6620 7479 7065 2876 6572 7469 6365 7329  f type(vertices)
-0001a420: 206e 6f74 2069 6e20 5b6e 756d 7079 2e6e   not in [numpy.n
-0001a430: 6461 7272 6179 2c20 6c69 7374 5d3a 0a20  darray, list]:. 
-0001a440: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-0001a450: 6545 7272 6f72 2822 6076 6572 7469 6365  eError("`vertice
-0001a460: 7360 206d 7573 7420 6265 2061 206c 6973  s` must be a lis
-0001a470: 7420 6f72 2061 206e 756d 7079 2e6e 6461  t or a numpy.nda
-0001a480: 7272 6179 2e22 290a 2020 2020 656c 6966  rray.").    elif
-0001a490: 206e 756d 7079 2e61 7361 7272 6179 2876   numpy.asarray(v
-0001a4a0: 6572 7469 6365 7329 2e73 6861 7065 2021  ertices).shape !
-0001a4b0: 3d20 2834 2c20 3329 3a0a 2020 2020 2020  = (4, 3):.      
-0001a4c0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0001a4d0: 6f72 2822 6076 6572 7469 6365 7360 2068  or("`vertices` h
-0001a4e0: 6173 2069 6e63 6f72 7265 6374 2073 6861  as incorrect sha
-0001a4f0: 7065 2e20 4974 206d 7573 7420 6265 2028  pe. It must be (
-0001a500: 342c 2033 292e 2229 0a20 2020 2069 6620  4, 3).").    if 
-0001a510: 7479 7065 2873 7465 7029 206e 6f74 2069  type(step) not i
-0001a520: 6e20 5b66 6c6f 6174 2c20 696e 745d 3a0a  n [float, int]:.
-0001a530: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-0001a540: 7065 4572 726f 7228 2260 7374 6570 6020  peError("`step` 
-0001a550: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-0001a560: 7665 2072 6561 6c20 6e75 6d62 6572 2e22  ve real number."
-0001a570: 290a 2020 2020 656c 6966 2073 7465 7020  ).    elif step 
-0001a580: 3c3d 2030 2e30 3a0a 2020 2020 2020 2020  <= 0.0:.        
-0001a590: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0001a5a0: 2822 6073 7465 7060 206d 7573 7420 6265  ("`step` must be
-0001a5b0: 2061 2070 6f73 6974 6976 6520 7265 616c   a positive real
-0001a5c0: 206e 756d 6265 722e 2229 0a20 2020 2069   number.").    i
-0001a5d0: 6620 7365 6c65 6374 696f 6e20 6973 206e  f selection is n
-0001a5e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001a5f0: 2023 2043 6865 636b 2073 656c 6563 7469   # Check selecti
-0001a600: 6f6e 2074 7970 6573 0a20 2020 2020 2020  on types.       
-0001a610: 2069 6620 616c 6c28 6973 696e 7374 616e   if all(isinstan
-0001a620: 6365 2878 2c20 696e 7429 2066 6f72 2078  ce(x, int) for x
-0001a630: 2069 6e20 7365 6c65 6374 696f 6e29 3a0a   in selection):.
-0001a640: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0001a650: 0a20 2020 2020 2020 2065 6c69 6620 616c  .        elif al
-0001a660: 6c28 6973 696e 7374 616e 6365 2878 2c20  l(isinstance(x, 
-0001a670: 7374 7229 2066 6f72 2078 2069 6e20 7365  str) for x in se
-0001a680: 6c65 6374 696f 6e29 3a0a 2020 2020 2020  lection):.      
-0001a690: 2020 2020 2020 7365 6c65 6374 696f 6e20        selection 
-0001a6a0: 3d20 5b5f 6765 745f 6f70 656e 696e 675f  = [_get_opening_
-0001a6b0: 6c61 6265 6c28 7365 6c65 2920 666f 7220  label(sele) for 
-0001a6c0: 7365 6c65 2069 6e20 7365 6c65 6374 696f  sele in selectio
-0001a6d0: 6e5d 0a20 2020 2020 2020 2065 6c73 653a  n].        else:
-0001a6e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001a6f0: 7365 2054 7970 6545 7272 6f72 280a 2020  se TypeError(.  
-0001a700: 2020 2020 2020 2020 2020 2020 2020 2260                "`
-0001a710: 7365 6c65 6374 696f 6e60 206d 7573 7420  selection` must 
-0001a720: 6265 2061 206c 6973 7420 6f66 2073 7472  be a list of str
-0001a730: 696e 6773 2028 6361 7669 7479 206e 616d  ings (cavity nam
-0001a740: 6573 2920 6f72 2069 6e74 6567 6572 7320  es) or integers 
-0001a750: 2863 6176 6974 7920 6c61 6265 6c73 292e  (cavity labels).
-0001a760: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-0001a770: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-0001a780: 6966 2073 656c 6563 7469 6f6e 2069 6e63  if selection inc
-0001a790: 6c75 6465 7320 7661 6c69 6420 6361 7669  ludes valid cavi
-0001a7a0: 7479 206c 6162 656c 730a 2020 2020 2020  ty labels.      
-0001a7b0: 2020 6966 2061 6e79 2878 203c 2032 2066    if any(x < 2 f
-0001a7c0: 6f72 2078 2069 6e20 7365 6c65 6374 696f  or x in selectio
-0001a7d0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-0001a7e0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0001a7f0: 2866 2249 6e76 616c 6964 2060 7365 6c65  (f"Invalid `sele
-0001a800: 6374 696f 6e60 3a20 7b73 656c 6563 7469  ction`: {selecti
-0001a810: 6f6e 7d2e 2229 0a20 2020 2069 6620 6e74  on}.").    if nt
-0001a820: 6872 6561 6473 2069 7320 4e6f 6e65 3a0a  hreads is None:.
-0001a830: 2020 2020 2020 2020 6e74 6872 6561 6473          nthreads
-0001a840: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
-0001a850: 2920 2d20 310a 2020 2020 656c 7365 3a0a  ) - 1.    else:.
-0001a860: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0001a870: 6e74 6872 6561 6473 2920 6e6f 7420 696e  nthreads) not in
-0001a880: 205b 696e 745d 3a0a 2020 2020 2020 2020   [int]:.        
-0001a890: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-0001a8a0: 726f 7228 2260 6e74 6872 6561 6473 6020  ror("`nthreads` 
-0001a8b0: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-0001a8c0: 7665 2069 6e74 6567 6572 2e22 290a 2020  ve integer.").  
-0001a8d0: 2020 2020 2020 656c 6966 206e 7468 7265        elif nthre
-0001a8e0: 6164 7320 3c3d 2030 3a0a 2020 2020 2020  ads <= 0:.      
-0001a8f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0001a900: 6545 7272 6f72 2822 606e 7468 7265 6164  eError("`nthread
-0001a910: 7360 206d 7573 7420 6265 2061 2070 6f73  s` must be a pos
-0001a920: 6974 6976 6520 696e 7465 6765 722e 2229  itive integer.")
-0001a930: 0a20 2020 2069 6620 7479 7065 2861 7070  .    if type(app
-0001a940: 656e 6429 206e 6f74 2069 6e20 5b62 6f6f  end) not in [boo
-0001a950: 6c5d 3a0a 2020 2020 2020 2020 7261 6973  l]:.        rais
-0001a960: 6520 5479 7065 4572 726f 7228 2260 6170  e TypeError("`ap
-0001a970: 7065 6e64 6020 6d75 7374 2062 6520 6120  pend` must be a 
-0001a980: 626f 6f6c 6561 6e2e 2229 0a20 2020 2069  boolean.").    i
-0001a990: 6620 7479 7065 286d 6f64 656c 2920 6e6f  f type(model) no
-0001a9a0: 7420 696e 205b 696e 745d 3a0a 2020 2020  t in [int]:.    
-0001a9b0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-0001a9c0: 726f 7228 2260 6d6f 6465 6c60 206d 7573  ror("`model` mus
-0001a9d0: 7420 6265 2061 2069 6e74 6567 6572 2e22  t be a integer."
-0001a9e0: 290a 0a20 2020 2023 2043 6f6e 7665 7274  )..    # Convert
-0001a9f0: 2074 7970 6573 0a20 2020 2069 6620 7479   types.    if ty
-0001aa00: 7065 2876 6572 7469 6365 7329 203d 3d20  pe(vertices) == 
-0001aa10: 6c69 7374 3a0a 2020 2020 2020 2020 7665  list:.        ve
-0001aa20: 7274 6963 6573 203d 206e 756d 7079 2e61  rtices = numpy.a
-0001aa30: 7361 7272 6179 2876 6572 7469 6365 7329  sarray(vertices)
-0001aa40: 0a20 2020 2069 6620 7479 7065 2873 7465  .    if type(ste
-0001aa50: 7029 203d 3d20 696e 743a 0a20 2020 2020  p) == int:.     
-0001aa60: 2020 2073 7465 7020 3d20 666c 6f61 7428     step = float(
-0001aa70: 7374 6570 290a 0a20 2020 2023 2043 6f6e  step)..    # Con
-0001aa80: 7665 7274 206e 756d 7079 2e6e 6461 7272  vert numpy.ndarr
-0001aa90: 6179 2064 6174 6120 7479 7065 730a 2020  ay data types.  
-0001aaa0: 2020 7665 7274 6963 6573 203d 2076 6572    vertices = ver
-0001aab0: 7469 6365 732e 6173 7479 7065 2822 666c  tices.astype("fl
-0001aac0: 6f61 7436 3422 2920 6966 2076 6572 7469  oat64") if verti
-0001aad0: 6365 732e 6474 7970 6520 213d 2022 666c  ces.dtype != "fl
-0001aae0: 6f61 7436 3422 2065 6c73 6520 7665 7274  oat64" else vert
-0001aaf0: 6963 6573 0a0a 2020 2020 2320 4765 7420  ices..    # Get 
-0001ab00: 7369 6e63 6f73 3a20 7369 6e65 2061 6e64  sincos: sine and
-0001ab10: 2063 6f73 7369 6e65 206f 6620 7468 6520   cossine of the 
-0001ab20: 6772 6964 2072 6f74 6174 696f 6e20 616e  grid rotation an
-0001ab30: 676c 6573 2028 7369 6e61 2c20 636f 7361  gles (sina, cosa
-0001ab40: 2c20 7369 6e62 2c20 636f 7362 290a 2020  , sinb, cosb).  
-0001ab50: 2020 7369 6e63 6f73 203d 205f 6765 745f    sincos = _get_
-0001ab60: 7369 6e63 6f73 2876 6572 7469 6365 7329  sincos(vertices)
-0001ab70: 0a0a 2020 2020 2320 4372 6561 7465 2062  ..    # Create b
-0001ab80: 6173 6520 6469 7265 6374 6f72 6965 7320  ase directories 
-0001ab90: 6f66 2072 6573 756c 7473 0a20 2020 2069  of results.    i
-0001aba0: 6620 666e 2069 7320 6e6f 7420 4e6f 6e65  f fn is not None
-0001abb0: 3a0a 2020 2020 2020 2020 6966 2074 7970  :.        if typ
-0001abc0: 6528 666e 2920 6e6f 7420 696e 205b 7374  e(fn) not in [st
-0001abd0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
-0001abe0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0001abf0: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-0001ac00: 666e 6020 6d75 7374 2062 6520 6120 7374  fn` must be a st
-0001ac10: 7269 6e67 206f 7220 6120 7061 7468 6c69  ring or a pathli
-0001ac20: 622e 5061 7468 2e22 290a 2020 2020 2020  b.Path.").      
-0001ac30: 2020 6f73 2e6d 616b 6564 6972 7328 6f73    os.makedirs(os
-0001ac40: 2e70 6174 682e 6162 7370 6174 6828 6f73  .path.abspath(os
-0001ac50: 2e70 6174 682e 6469 726e 616d 6528 666e  .path.dirname(fn
-0001ac60: 2929 2c20 6578 6973 745f 6f6b 3d54 7275  )), exist_ok=Tru
-0001ac70: 6529 0a0a 2020 2020 2320 556e 7061 636b  e)..    # Unpack
-0001ac80: 2076 6572 7469 6365 730a 2020 2020 5031   vertices.    P1
-0001ac90: 2c20 5f2c 205f 2c20 5f20 3d20 7665 7274  , _, _, _ = vert
-0001aca0: 6963 6573 0a0a 2020 2020 2320 5365 6c65  ices..    # Sele
-0001acb0: 6374 2063 6176 6974 6965 730a 2020 2020  ct cavities.    
-0001acc0: 6966 2073 656c 6563 7469 6f6e 2069 7320  if selection is 
-0001acd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0001ace0: 2020 6f70 656e 696e 6773 203d 205f 7365    openings = _se
-0001acf0: 6c65 6374 5f63 6176 6974 6965 7328 6f70  lect_cavities(op
-0001ad00: 656e 696e 6773 2c20 7365 6c65 6374 696f  enings, selectio
-0001ad10: 6e29 0a0a 2020 2020 2320 4765 7420 6e75  n)..    # Get nu
-0001ad20: 6d62 6572 206f 6620 6f70 656e 696e 6773  mber of openings
-0001ad30: 0a20 2020 206e 6f70 656e 696e 6773 203d  .    nopenings =
-0001ad40: 2069 6e74 286f 7065 6e69 6e67 732e 6d61   int(openings.ma
-0001ad50: 7828 2920 2d20 3129 0a0a 2020 2020 2320  x() - 1)..    # 
-0001ad60: 4578 706f 7274 206f 7065 6e69 6e67 730a  Export openings.
-0001ad70: 2020 2020 5f65 7870 6f72 745f 6f70 656e      _export_open
-0001ad80: 696e 6773 2866 6e2c 206f 7065 6e69 6e67  ings(fn, opening
-0001ad90: 732c 2050 312c 2073 696e 636f 732c 2073  s, P1, sincos, s
-0001ada0: 7465 702c 206e 6f70 656e 696e 6773 2c20  tep, nopenings, 
-0001adb0: 6e74 6872 6561 6473 2c20 6170 7065 6e64  nthreads, append
-0001adc0: 2c20 6d6f 6465 6c29 0a                   , model).
+000169b0: 6361 7669 7469 6573 3a20 6e75 6d70 792e  cavities: numpy.
+000169c0: 6e64 6172 7261 792c 0a20 2020 2073 7572  ndarray,.    sur
+000169d0: 6661 6365 3a20 4f70 7469 6f6e 616c 5b6e  face: Optional[n
+000169e0: 756d 7079 2e6e 6461 7272 6179 5d2c 0a20  umpy.ndarray],. 
+000169f0: 2020 2076 6572 7469 6365 733a 2055 6e69     vertices: Uni
+00016a00: 6f6e 5b6e 756d 7079 2e6e 6461 7272 6179  on[numpy.ndarray
+00016a10: 2c20 4c69 7374 5b4c 6973 745b 666c 6f61  , List[List[floa
+00016a20: 745d 5d5d 2c0a 2020 2020 7374 6570 3a20  t]]],.    step: 
+00016a30: 556e 696f 6e5b 666c 6f61 742c 2069 6e74  Union[float, int
+00016a40: 5d20 3d20 302e 362c 0a20 2020 2042 3a20  ] = 0.6,.    B: 
+00016a50: 4f70 7469 6f6e 616c 5b6e 756d 7079 2e6e  Optional[numpy.n
+00016a60: 6461 7272 6179 5d20 3d20 4e6f 6e65 2c0a  darray] = None,.
+00016a70: 2020 2020 513a 204f 7074 696f 6e61 6c5b      Q: Optional[
+00016a80: 6e75 6d70 792e 6e64 6172 7261 795d 203d  numpy.ndarray] =
+00016a90: 204e 6f6e 652c 0a20 2020 2073 656c 6563   None,.    selec
+00016aa0: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b55  tion: Optional[U
+00016ab0: 6e69 6f6e 5b4c 6973 745b 696e 745d 2c20  nion[List[int], 
+00016ac0: 4c69 7374 5b73 7472 5d5d 5d20 3d20 4e6f  List[str]]] = No
+00016ad0: 6e65 2c0a 2020 2020 6e74 6872 6561 6473  ne,.    nthreads
+00016ae0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00016af0: 3d20 4e6f 6e65 2c0a 2020 2020 6170 7065  = None,.    appe
+00016b00: 6e64 3a20 626f 6f6c 203d 2046 616c 7365  nd: bool = False
+00016b10: 2c0a 2020 2020 6d6f 6465 6c3a 2069 6e74  ,.    model: int
+00016b20: 203d 2030 2c0a 2920 2d3e 204e 6f6e 653a   = 0,.) -> None:
+00016b30: 0a20 2020 2022 2222 4578 706f 7274 2063  .    """Export c
+00016b40: 6176 6974 6979 2028 4829 2061 6e64 2073  avitiy (H) and s
+00016b50: 7572 6661 6365 2028 4841 2920 706f 696e  urface (HA) poin
+00016b60: 7473 2074 6f20 5044 422d 666f 726d 6174  ts to PDB-format
+00016b70: 7465 6420 6669 6c65 2077 6974 680a 2020  ted file with.  
+00016b80: 2020 6120 7661 7269 6162 6c65 2028 423b    a variable (B;
+00016b90: 206f 7074 696f 6e61 6c29 2069 6e20 422d   optional) in B-
+00016ba0: 6661 6374 6f72 2063 6f6c 756d 6e2c 2061  factor column, a
+00016bb0: 6e64 2068 7964 726f 7061 7468 7920 746f  nd hydropathy to
+00016bc0: 0a20 2020 2050 4442 2d66 6f72 6d61 7474  .    PDB-formatt
+00016bd0: 6564 2066 696c 6520 696e 2042 2d66 6163  ed file in B-fac
+00016be0: 746f 7220 636f 6c75 6d6e 2061 7420 7375  tor column at su
+00016bf0: 7266 6163 6520 706f 696e 7473 2028 4841  rface points (HA
+00016c00: 292e 0a0a 2020 2020 5061 7261 6d65 7465  )...    Paramete
+00016c10: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00016c20: 2d0a 2020 2020 666e 203a 2055 6e69 6f6e  -.    fn : Union
+00016c30: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
+00016c40: 7468 5d0a 2020 2020 2020 2020 4120 7061  th].        A pa
+00016c50: 7468 2074 6f20 5044 4220 6669 6c65 2066  th to PDB file f
+00016c60: 6f72 2077 7269 7469 6e67 2063 6176 6974  or writing cavit
+00016c70: 6965 732e 0a20 2020 2063 6176 6974 6965  ies..    cavitie
+00016c80: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+00016c90: 790a 2020 2020 2020 2020 4361 7669 7479  y.        Cavity
+00016ca0: 2070 6f69 6e74 7320 696e 2074 6865 2033   points in the 3
+00016cb0: 4420 6772 6964 2028 6361 7669 7469 6573  D grid (cavities
+00016cc0: 5b6e 785d 5b6e 795d 5b6e 7a5d 292e 0a20  [nx][ny][nz]).. 
+00016cd0: 2020 2020 2020 2043 6176 6974 6965 7320         Cavities 
+00016ce0: 6172 7261 7920 6861 7320 696e 7465 6765  array has intege
+00016cf0: 7220 6c61 6265 6c73 2069 6e20 6561 6368  r labels in each
+00016d00: 2070 6f73 6974 696f 6e2c 2074 6861 7420   position, that 
+00016d10: 6172 653a 0a0a 2020 2020 2020 2020 2020  are:..          
+00016d20: 2020 2a20 2d31 3a20 6275 6c6b 2070 6f69    * -1: bulk poi
+00016d30: 6e74 733b 0a0a 2020 2020 2020 2020 2020  nts;..          
+00016d40: 2020 2a20 303a 2062 696f 6d6f 6c65 6375    * 0: biomolecu
+00016d50: 6c65 2070 6f69 6e74 733b 0a0a 2020 2020  le points;..    
+00016d60: 2020 2020 2020 2020 2a20 313a 2065 6d70          * 1: emp
+00016d70: 7479 2073 7061 6365 2070 6f69 6e74 733b  ty space points;
+00016d80: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+00016d90: 3e3d 323a 2063 6176 6974 7920 706f 696e  >=2: cavity poin
+00016da0: 7473 2e0a 0a20 2020 2020 2020 2054 6865  ts...        The
+00016db0: 2065 6d70 7479 2073 7061 6365 2070 6f69   empty space poi
+00016dc0: 6e74 7320 6172 6520 7265 6769 6f6e 7320  nts are regions 
+00016dd0: 7468 6174 2064 6f20 6e6f 7420 6d65 6574  that do not meet
+00016de0: 2074 6865 2063 686f 7365 6e0a 2020 2020   the chosen.    
+00016df0: 2020 2020 766f 6c75 6d65 2063 7574 6f66      volume cutof
+00016e00: 6620 746f 2062 6520 636f 6e73 6964 6572  f to be consider
+00016e10: 6564 2061 2063 6176 6974 792e 0a20 2020  ed a cavity..   
+00016e20: 2073 7572 6661 6365 203a 206e 756d 7079   surface : numpy
+00016e30: 2e6e 6461 7272 6179 2c20 6f70 7469 6f6e  .ndarray, option
+00016e40: 616c 0a20 2020 2020 2020 2053 7572 6661  al.        Surfa
+00016e50: 6365 2070 6f69 6e74 7320 696e 2074 6865  ce points in the
+00016e60: 2033 4420 6772 6964 2028 7375 7266 6163   3D grid (surfac
+00016e70: 655b 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e20  e[nx][ny][nz]). 
+00016e80: 4966 204e 6f6e 652c 2073 7572 6661 6365  If None, surface
+00016e90: 0a20 2020 2020 2020 2069 7320 6120 6e75  .        is a nu
+00016ea0: 6d70 792e 7a65 726f 7320 6172 7261 7920  mpy.zeros array 
+00016eb0: 7769 7468 2073 616d 6520 7368 6170 6520  with same shape 
+00016ec0: 6f66 2063 6176 6974 6965 732e 0a20 2020  of cavities..   
+00016ed0: 2020 2020 2053 7572 6661 6365 2061 7272       Surface arr
+00016ee0: 6179 2068 6173 2069 6e74 6567 6572 206c  ay has integer l
+00016ef0: 6162 656c 7320 696e 2065 6163 6820 706f  abels in each po
+00016f00: 7369 7469 6f6e 2c20 7468 6174 2061 7265  sition, that are
+00016f10: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+00016f20: 202d 313a 2062 756c 6b20 706f 696e 7473   -1: bulk points
+00016f30: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
+00016f40: 2030 3a20 6269 6f6d 6f6c 6563 756c 6520   0: biomolecule 
+00016f50: 6f72 2065 6d70 7479 2073 7061 6365 2070  or empty space p
+00016f60: 6f69 6e74 733b 0a0a 2020 2020 2020 2020  oints;..        
+00016f70: 2020 2020 2a20 3e3d 323a 2073 7572 6661      * >=2: surfa
+00016f80: 6365 2070 6f69 6e74 732e 0a0a 2020 2020  ce points...    
+00016f90: 2020 2020 5468 6520 656d 7074 7920 7370      The empty sp
+00016fa0: 6163 6520 706f 696e 7473 2061 7265 2072  ace points are r
+00016fb0: 6567 696f 6e73 2074 6861 7420 646f 206e  egions that do n
+00016fc0: 6f74 206d 6565 7420 7468 6520 6368 6f73  ot meet the chos
+00016fd0: 656e 0a20 2020 2020 2020 2076 6f6c 756d  en.        volum
+00016fe0: 6520 6375 746f 6666 2074 6f20 6265 2063  e cutoff to be c
+00016ff0: 6f6e 7369 6465 7265 6420 6120 6361 7669  onsidered a cavi
+00017000: 7479 2e0a 2020 2020 7665 7274 6963 6573  ty..    vertices
+00017010: 203a 2055 6e69 6f6e 5b6e 756d 7079 2e6e   : Union[numpy.n
+00017020: 6461 7272 6179 2c20 4c69 7374 5b4c 6973  darray, List[Lis
+00017030: 745b 666c 6f61 745d 5d5d 0a20 2020 2020  t[float]]].     
+00017040: 2020 2041 206e 756d 7079 2e6e 6461 7272     A numpy.ndarr
+00017050: 6179 206f 7220 6120 6c69 7374 2077 6974  ay or a list wit
+00017060: 6820 7879 7a20 7665 7274 6963 6573 2063  h xyz vertices c
+00017070: 6f6f 7264 696e 6174 6573 2028 6f72 6967  oordinates (orig
+00017080: 696e 2c0a 2020 2020 2020 2020 582d 6178  in,.        X-ax
+00017090: 6973 2c20 592d 6178 6973 2c20 5a2d 6178  is, Y-axis, Z-ax
+000170a0: 6973 292e 0a20 2020 2073 7465 7020 3a20  is)..    step : 
+000170b0: 556e 696f 6e5b 666c 6f61 742c 2069 6e74  Union[float, int
+000170c0: 5d2c 206f 7074 696f 6e61 6c0a 2020 2020  ], optional.    
+000170d0: 2020 2020 4772 6964 2073 7061 6369 6e67      Grid spacing
+000170e0: 2028 4129 2c20 6279 2064 6566 6175 6c74   (A), by default
+000170f0: 2030 2e36 2e0a 2020 2020 4220 3a20 6e75   0.6..    B : nu
+00017100: 6d70 792e 6e64 6172 7261 792c 206f 7074  mpy.ndarray, opt
+00017110: 696f 6e61 6c0a 2020 2020 2020 2020 4120  ional.        A 
+00017120: 6e75 6d70 792e 6e64 6172 7261 7920 7769  numpy.ndarray wi
+00017130: 7468 2076 616c 7565 7320 746f 2062 6520  th values to be 
+00017140: 6d61 7070 6564 206f 6e20 422d 6661 6374  mapped on B-fact
+00017150: 6f72 2063 6f6c 756d 6e20 696e 2063 6176  or column in cav
+00017160: 6974 790a 2020 2020 2020 2020 706f 696e  ity.        poin
+00017170: 7473 2028 425b 6e78 5d5b 6e79 5d5b 6e7a  ts (B[nx][ny][nz
+00017180: 5d29 2c20 6279 2064 6566 6175 6c74 204e  ]), by default N
+00017190: 6f6e 652e 0a20 2020 2051 203a 206e 756d  one..    Q : num
+000171a0: 7079 2e6e 6461 7272 6179 2c20 6f70 7469  py.ndarray, opti
+000171b0: 6f6e 616c 0a20 2020 2020 2020 2041 206e  onal.        A n
+000171c0: 756d 7079 2e6e 6461 7272 6179 2077 6974  umpy.ndarray wit
+000171d0: 6820 6879 6472 6f70 686f 6269 6369 7479  h hydrophobicity
+000171e0: 2073 6361 6c65 2076 616c 7565 7320 746f   scale values to
+000171f0: 2062 6520 6d61 7070 6564 206f 6e0a 2020   be mapped on.  
+00017200: 2020 2020 2020 422d 6661 6374 6f72 2063        B-factor c
+00017210: 6f6c 756d 6e20 696e 2073 7572 6661 6365  olumn in surface
+00017220: 2070 6f69 6e74 7320 2851 5b6e 785d 5b6e   points (Q[nx][n
+00017230: 795d 5b6e 7a5d 292c 2062 7920 6465 6661  y][nz]), by defa
+00017240: 756c 740a 2020 2020 2020 2020 4e6f 6e65  ult.        None
+00017250: 2e0a 2020 2020 7365 6c65 6374 696f 6e20  ..    selection 
+00017260: 3a20 556e 696f 6e5b 4c69 7374 5b69 6e74  : Union[List[int
+00017270: 5d2c 204c 6973 745b 7374 725d 5d2c 206f  ], List[str]], o
+00017280: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00017290: 4120 6c69 7374 206f 6620 696e 7465 6765  A list of intege
+000172a0: 7220 6c61 6265 6c73 206f 7220 6120 6c69  r labels or a li
+000172b0: 7374 206f 6620 6361 7669 7479 206e 616d  st of cavity nam
+000172c0: 6573 2074 6f20 6265 2073 656c 6563 7465  es to be selecte
+000172d0: 642c 2062 7920 6465 6661 756c 7420 4e6f  d, by default No
+000172e0: 6e65 2e0a 2020 2020 6e74 6872 6561 6473  ne..    nthreads
+000172f0: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+00017300: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
+00017310: 6f66 2074 6872 6561 6473 2c20 6279 2064  of threads, by d
+00017320: 6566 6175 6c74 204e 6f6e 652e 2049 6620  efault None. If 
+00017330: 4e6f 6e65 2c20 7468 6520 6e75 6d62 6572  None, the number
+00017340: 206f 6620 7468 7265 6164 7320 6973 0a20   of threads is. 
+00017350: 2020 2020 2020 2060 6f73 2e63 7075 5f63         `os.cpu_c
+00017360: 6f75 6e74 2829 202d 2031 602e 0a20 2020  ount() - 1`..   
+00017370: 2061 7070 656e 6420 3a20 626f 6f6c 2c20   append : bool, 
+00017380: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00017390: 2057 6865 7468 6572 2074 6f20 6170 7065   Whether to appe
+000173a0: 6e64 2063 6176 6974 6965 7320 746f 2074  nd cavities to t
+000173b0: 6865 2050 4442 2066 696c 652c 2062 7920  he PDB file, by 
+000173c0: 6465 6661 756c 7420 4661 6c73 652e 0a20  default False.. 
+000173d0: 2020 206d 6f64 656c 203a 2069 6e74 2c20     model : int, 
+000173e0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+000173f0: 204d 6f64 656c 206e 756d 6265 722c 2062   Model number, b
+00017400: 7920 6465 6661 756c 7420 302e 0a0a 2020  y default 0...  
+00017410: 2020 5261 6973 6573 0a20 2020 202d 2d2d    Raises.    ---
+00017420: 2d2d 2d0a 2020 2020 5479 7065 4572 726f  ---.    TypeErro
+00017430: 720a 2020 2020 2020 2020 6066 6e60 206d  r.        `fn` m
+00017440: 7573 7420 6265 2061 2073 7472 696e 6720  ust be a string 
+00017450: 6f72 2070 6174 686c 6962 2e50 6174 682e  or pathlib.Path.
+00017460: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
+00017470: 2020 2020 2020 2060 6361 7669 7469 6573         `cavities
+00017480: 6020 6d75 7374 2062 6520 6120 6e75 6d70  ` must be a nump
+00017490: 792e 6e64 6172 7261 792e 0a20 2020 2056  y.ndarray..    V
+000174a0: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
+000174b0: 2020 6063 6176 6974 6965 7360 2068 6173    `cavities` has
+000174c0: 2074 6865 2069 6e63 6f72 7265 6374 2073   the incorrect s
+000174d0: 6861 7065 2e20 4974 206d 7573 7420 6265  hape. It must be
+000174e0: 2028 6e78 2c20 6e79 2c20 6e7a 292e 0a20   (nx, ny, nz).. 
+000174f0: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
+00017500: 2020 2020 2060 7375 7266 6163 6560 206d       `surface` m
+00017510: 7573 7420 6265 2061 206e 756d 7079 2e6e  ust be a numpy.n
+00017520: 6461 7272 6179 2e0a 2020 2020 5661 6c75  darray..    Valu
+00017530: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
+00017540: 7375 7266 6163 6560 2068 6173 2074 6865  surface` has the
+00017550: 2069 6e63 6f72 7265 6374 2073 6861 7065   incorrect shape
+00017560: 2e20 4974 206d 7573 7420 6265 2028 6e78  . It must be (nx
+00017570: 2c20 6e79 2c20 6e7a 292e 0a20 2020 2054  , ny, nz)..    T
+00017580: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
+00017590: 2060 7665 7274 6963 6573 6020 6d75 7374   `vertices` must
+000175a0: 2062 6520 6120 6c69 7374 206f 7220 6120   be a list or a 
+000175b0: 6e75 6d70 792e 6e64 6172 7261 792e 0a20  numpy.ndarray.. 
+000175c0: 2020 2056 616c 7565 4572 726f 720a 2020     ValueError.  
+000175d0: 2020 2020 2020 6076 6572 7469 6365 7360        `vertices`
+000175e0: 2068 6173 2069 6e63 6f72 7265 6374 2073   has incorrect s
+000175f0: 6861 7065 2e20 4974 206d 7573 7420 6265  hape. It must be
+00017600: 2028 342c 2033 292e 0a20 2020 2054 7970   (4, 3)..    Typ
+00017610: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
+00017620: 7374 6570 6020 6d75 7374 2062 6520 6120  step` must be a 
+00017630: 706f 7369 7469 7665 2072 6561 6c20 6e75  positive real nu
+00017640: 6d62 6572 2e0a 2020 2020 5661 6c75 6545  mber..    ValueE
+00017650: 7272 6f72 0a20 2020 2020 2020 2060 7374  rror.        `st
+00017660: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
+00017670: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
+00017680: 6572 2e0a 2020 2020 5479 7065 4572 726f  er..    TypeErro
+00017690: 720a 2020 2020 2020 2020 6042 6020 6d75  r.        `B` mu
+000176a0: 7374 2062 6520 6120 6e75 6d70 792e 6e64  st be a numpy.nd
+000176b0: 6172 7261 792e 0a20 2020 2056 616c 7565  array..    Value
+000176c0: 4572 726f 720a 2020 2020 2020 2020 6042  Error.        `B
+000176d0: 6020 6861 7320 7468 6520 696e 636f 7272  ` has the incorr
+000176e0: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
+000176f0: 7374 2062 6520 286e 782c 206e 792c 206e  st be (nx, ny, n
+00017700: 7a29 2e0a 2020 2020 5479 7065 4572 726f  z)..    TypeErro
+00017710: 720a 2020 2020 2020 2020 6051 6020 6d75  r.        `Q` mu
+00017720: 7374 2062 6520 6120 6e75 6d70 792e 6e64  st be a numpy.nd
+00017730: 6172 7261 792e 0a20 2020 2056 616c 7565  array..    Value
+00017740: 4572 726f 720a 2020 2020 2020 2020 6051  Error.        `Q
+00017750: 6020 6861 7320 7468 6520 696e 636f 7272  ` has the incorr
+00017760: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
+00017770: 7374 2062 6520 286e 782c 206e 792c 206e  st be (nx, ny, n
+00017780: 7a29 2e0a 2020 2020 5479 7065 4572 726f  z)..    TypeErro
+00017790: 720a 2020 2020 2020 2020 6073 656c 6563  r.        `selec
+000177a0: 7469 6f6e 6020 6d75 7374 2062 6520 6120  tion` must be a 
+000177b0: 6c69 7374 206f 6620 7374 7269 6e67 7320  list of strings 
+000177c0: 2863 6176 6974 7920 6e61 6d65 7329 206f  (cavity names) o
+000177d0: 7220 696e 7465 6765 7273 2028 6361 7669  r integers (cavi
+000177e0: 7479 206c 6162 656c 7329 2e0a 2020 2020  ty labels)..    
+000177f0: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
+00017800: 2020 2049 6e76 616c 6964 2060 7365 6c65     Invalid `sele
+00017810: 6374 696f 6e60 3a20 7b73 656c 6563 7469  ction`: {selecti
+00017820: 6f6e 7d2e 0a20 2020 2054 7970 6545 7272  on}..    TypeErr
+00017830: 6f72 0a20 2020 2020 2020 2060 6e74 6872  or.        `nthr
+00017840: 6561 6473 6020 6d75 7374 2062 6520 6120  eads` must be a 
+00017850: 706f 7369 7469 7665 2069 6e74 6567 6572  positive integer
+00017860: 2e0a 2020 2020 5661 6c75 6545 7272 6f72  ..    ValueError
+00017870: 0a20 2020 2020 2020 2060 6e74 6872 6561  .        `nthrea
+00017880: 6473 6020 6d75 7374 2062 6520 6120 706f  ds` must be a po
+00017890: 7369 7469 7665 2069 6e74 6567 6572 2e0a  sitive integer..
+000178a0: 2020 2020 5479 7065 4572 726f 720a 2020      TypeError.  
+000178b0: 2020 2020 2020 6061 7070 656e 6460 206d        `append` m
+000178c0: 7573 7420 6265 2061 2062 6f6f 6c65 616e  ust be a boolean
+000178d0: 2e0a 2020 2020 5479 7065 4572 726f 720a  ..    TypeError.
+000178e0: 2020 2020 2020 2020 606d 6f64 656c 6020          `model` 
+000178f0: 6d75 7374 2062 6520 6120 696e 7465 6765  must be a intege
+00017900: 722e 0a20 2020 2052 756e 7469 6d65 4572  r..    RuntimeEr
+00017910: 726f 720a 2020 2020 2020 2020 5573 6572  ror.        User
+00017920: 206d 7573 7420 6465 6669 6e65 2060 7375   must define `su
+00017930: 7266 6163 6560 2077 6865 6e20 6e6f 7420  rface` when not 
+00017940: 6465 6669 6e69 6e67 2060 6361 7669 7469  defining `caviti
+00017950: 6573 602e 0a0a 2020 2020 4e6f 7465 0a20  es`...    Note. 
+00017960: 2020 202d 2d2d 2d0a 2020 2020 5468 6520     ----.    The 
+00017970: 6361 7669 7479 206e 6f6d 656e 636c 6174  cavity nomenclat
+00017980: 7572 6520 6973 2062 6173 6564 206f 6e20  ure is based on 
+00017990: 7468 6520 696e 7465 6765 7220 6c61 6265  the integer labe
+000179a0: 6c2e 2054 6865 2063 6176 6974 7920 6d61  l. The cavity ma
+000179b0: 726b 6564 0a20 2020 2077 6974 6820 322c  rked.    with 2,
+000179c0: 2074 6865 2066 6972 7374 2069 6e74 6567   the first integ
+000179d0: 6572 2063 6f72 7265 7370 6f6e 6469 6e67  er corresponding
+000179e0: 2074 6f20 6120 6361 7669 7479 2c20 6973   to a cavity, is
+000179f0: 204b 4141 2c20 7468 6520 6361 7669 7479   KAA, the cavity
+00017a00: 0a20 2020 206d 6172 6b65 6420 7769 7468  .    marked with
+00017a10: 2033 2069 7320 4b41 422c 2074 6865 2063   3 is KAB, the c
+00017a20: 6176 6974 7920 6d61 726b 6564 2077 6974  avity marked wit
+00017a30: 6820 3420 6973 204b 4143 2061 6e64 2073  h 4 is KAC and s
+00017a40: 6f20 6f6e 2e0a 0a20 2020 2053 6565 2041  o on...    See A
+00017a50: 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d  lso.    --------
+00017a60: 0a20 2020 2064 6574 6563 740a 2020 2020  .    detect.    
+00017a70: 7370 6174 6961 6c0a 2020 2020 6465 7074  spatial.    dept
+00017a80: 680a 2020 2020 6879 6472 6f70 6174 6879  h.    hydropathy
+00017a90: 0a20 2020 2077 7269 7465 5f72 6573 756c  .    write_resul
+00017aa0: 7473 0a0a 2020 2020 4578 616d 706c 650a  ts..    Example.
+00017ab0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00017ac0: 5769 7468 2074 6865 2063 6176 6974 7920  With the cavity 
+00017ad0: 616e 6420 7375 7266 6163 6520 706f 696e  and surface poin
+00017ae0: 7473 2069 6465 6e74 6966 6965 6420 616e  ts identified an
+00017af0: 6420 6465 7074 6820 616e 6420 6879 6472  d depth and hydr
+00017b00: 6f70 686f 6269 6369 7479 2073 6361 6c65  ophobicity scale
+00017b10: 206d 6170 7065 6420 696e 2074 6865 2033   mapped in the 3
+00017b20: 4420 6772 6964 2c20 7765 2063 616e 3a0a  D grid, we can:.
+00017b30: 0a20 2020 202a 2045 7870 6f72 7420 6361  .    * Export ca
+00017b40: 7669 7479 2070 6f69 6e74 730a 0a20 2020  vity points..   
+00017b50: 203e 3e3e 2066 726f 6d20 7079 4b56 4669   >>> from pyKVFi
+00017b60: 6e64 6572 2069 6d70 6f72 7420 6578 706f  nder import expo
+00017b70: 7274 0a20 2020 203e 3e3e 2065 7870 6f72  rt.    >>> expor
+00017b80: 7428 2763 6176 6974 795f 776f 5f73 7572  t('cavity_wo_sur
+00017b90: 6661 6365 2e70 6462 272c 2063 6176 6974  face.pdb', cavit
+00017ba0: 6965 732c 204e 6f6e 652c 2076 6572 7469  ies, None, verti
+00017bb0: 6365 7329 0a0a 2020 2020 2a20 4578 706f  ces)..    * Expo
+00017bc0: 7274 2063 6176 6974 7920 616e 6420 7375  rt cavity and su
+00017bd0: 7266 6163 6520 706f 696e 7473 0a0a 2020  rface points..  
+00017be0: 2020 3e3e 3e20 6578 706f 7274 2827 6361    >>> export('ca
+00017bf0: 7669 7469 6573 2e70 6462 272c 2063 6176  vities.pdb', cav
+00017c00: 6974 6965 732c 2073 7572 6661 6365 2c20  ities, surface, 
+00017c10: 7665 7274 6963 6573 290a 0a20 2020 202a  vertices)..    *
+00017c20: 2045 7870 6f72 7420 6361 7669 7479 2061   Export cavity a
+00017c30: 6e64 2073 7572 6661 6365 2070 6f69 6e74  nd surface point
+00017c40: 7320 7769 7468 2064 6570 7468 206d 6170  s with depth map
+00017c50: 7065 6420 6f6e 2074 6865 6d0a 0a20 2020  ped on them..   
+00017c60: 203e 3e3e 2065 7870 6f72 7428 2763 6176   >>> export('cav
+00017c70: 6974 6965 735f 7769 7468 5f64 6570 7468  ities_with_depth
+00017c80: 2e70 6462 272c 2063 6176 6974 6965 732c  .pdb', cavities,
+00017c90: 2073 7572 6661 6365 2c20 7665 7274 6963   surface, vertic
+00017ca0: 6573 2c20 423d 6465 7074 6873 290a 0a20  es, B=depths).. 
+00017cb0: 2020 202a 2045 7870 6f72 7420 7375 7266     * Export surf
+00017cc0: 6163 6520 706f 696e 7473 2077 6974 6820  ace points with 
+00017cd0: 6879 6472 6f70 686f 6269 6369 7479 5f73  hydrophobicity_s
+00017ce0: 6361 6c65 206d 6170 7065 6420 6f6e 2074  cale mapped on t
+00017cf0: 6865 6d0a 0a20 2020 203e 3e3e 2065 7870  hem..    >>> exp
+00017d00: 6f72 7428 2763 6176 6974 6965 735f 7769  ort('cavities_wi
+00017d10: 7468 5f68 7964 726f 7061 7468 792e 7064  th_hydropathy.pd
+00017d20: 6227 2c20 6361 7669 7469 6573 2c20 7375  b', cavities, su
+00017d30: 7266 6163 652c 2076 6572 7469 6365 732c  rface, vertices,
+00017d40: 2051 3d73 6361 6c65 7329 0a0a 2020 2020   Q=scales)..    
+00017d50: 2a20 4578 706f 7274 2061 6c6c 0a0a 2020  * Export all..  
+00017d60: 2020 3e3e 3e20 6578 706f 7274 2827 6361    >>> export('ca
+00017d70: 7669 7469 6573 2e70 6462 272c 2063 6176  vities.pdb', cav
+00017d80: 6974 6965 732c 2073 7572 6661 6365 2c20  ities, surface, 
+00017d90: 7665 7274 6963 6573 2c20 423d 6465 7074  vertices, B=dept
+00017da0: 6873 2c20 513d 7363 616c 6573 290a 0a20  hs, Q=scales).. 
+00017db0: 2020 2022 2222 0a20 2020 2066 726f 6d20     """.    from 
+00017dc0: 5f70 794b 5646 696e 6465 7220 696d 706f  _pyKVFinder impo
+00017dd0: 7274 205f 6578 706f 7274 0a0a 2020 2020  rt _export..    
+00017de0: 2320 4368 6563 6b20 6172 6775 6d65 6e74  # Check argument
+00017df0: 730a 2020 2020 6966 2066 6e20 6973 206e  s.    if fn is n
+00017e00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017e10: 2069 6620 7479 7065 2866 6e29 206e 6f74   if type(fn) not
+00017e20: 2069 6e20 5b73 7472 2c20 7061 7468 6c69   in [str, pathli
+00017e30: 622e 5061 7468 5d3a 0a20 2020 2020 2020  b.Path]:.       
+00017e40: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00017e50: 7272 6f72 2822 6066 6e60 206d 7573 7420  rror("`fn` must 
+00017e60: 6265 2061 2073 7472 696e 6720 6f72 2061  be a string or a
+00017e70: 2070 6174 686c 6962 2e50 6174 682e 2229   pathlib.Path.")
+00017e80: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
+00017e90: 6469 7273 286f 732e 7061 7468 2e61 6273  dirs(os.path.abs
+00017ea0: 7061 7468 286f 732e 7061 7468 2e64 6972  path(os.path.dir
+00017eb0: 6e61 6d65 2866 6e29 292c 2065 7869 7374  name(fn)), exist
+00017ec0: 5f6f 6b3d 5472 7565 290a 2020 2020 6966  _ok=True).    if
+00017ed0: 2074 7970 6528 6361 7669 7469 6573 2920   type(cavities) 
+00017ee0: 6e6f 7420 696e 205b 6e75 6d70 792e 6e64  not in [numpy.nd
+00017ef0: 6172 7261 795d 3a0a 2020 2020 2020 2020  array]:.        
+00017f00: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00017f10: 2260 6361 7669 7469 6573 6020 6d75 7374  "`cavities` must
+00017f20: 2062 6520 6120 6e75 6d70 792e 6e64 6172   be a numpy.ndar
+00017f30: 7261 792e 2229 0a20 2020 2065 6c69 6620  ray.").    elif 
+00017f40: 6c65 6e28 6361 7669 7469 6573 2e73 6861  len(cavities.sha
+00017f50: 7065 2920 213d 2033 3a0a 2020 2020 2020  pe) != 3:.      
+00017f60: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00017f70: 6f72 2822 6063 6176 6974 6965 7360 2068  or("`cavities` h
+00017f80: 6173 2074 6865 2069 6e63 6f72 7265 6374  as the incorrect
+00017f90: 2073 6861 7065 2e20 4974 206d 7573 7420   shape. It must 
+00017fa0: 6265 2028 6e78 2c20 6e79 2c20 6e7a 292e  be (nx, ny, nz).
+00017fb0: 2229 0a20 2020 2069 6620 7375 7266 6163  ").    if surfac
+00017fc0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00017fd0: 2020 2020 2020 2069 6620 7479 7065 2873         if type(s
+00017fe0: 7572 6661 6365 2920 6e6f 7420 696e 205b  urface) not in [
+00017ff0: 6e75 6d70 792e 6e64 6172 7261 795d 3a0a  numpy.ndarray]:.
+00018000: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00018010: 6520 5479 7065 4572 726f 7228 2260 7375  e TypeError("`su
+00018020: 7266 6163 6560 206d 7573 7420 6265 2061  rface` must be a
+00018030: 206e 756d 7079 2e6e 6461 7272 6179 2e22   numpy.ndarray."
+00018040: 290a 2020 2020 2020 2020 656c 6966 206c  ).        elif l
+00018050: 656e 2873 7572 6661 6365 2e73 6861 7065  en(surface.shape
+00018060: 2920 213d 2033 3a0a 2020 2020 2020 2020  ) != 3:.        
+00018070: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00018080: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00018090: 2020 2020 2020 2260 7375 7266 6163 6560        "`surface`
+000180a0: 2068 6173 2074 6865 2069 6e63 6f72 7265   has the incorre
+000180b0: 6374 2073 6861 7065 2e20 4974 206d 7573  ct shape. It mus
+000180c0: 7420 6265 2028 6e78 2c20 6e79 2c20 6e7a  t be (nx, ny, nz
+000180d0: 292e 220a 2020 2020 2020 2020 2020 2020  ).".            
+000180e0: 290a 2020 2020 6966 2074 7970 6528 7665  ).    if type(ve
+000180f0: 7274 6963 6573 2920 6e6f 7420 696e 205b  rtices) not in [
+00018100: 6e75 6d70 792e 6e64 6172 7261 792c 206c  numpy.ndarray, l
+00018110: 6973 745d 3a0a 2020 2020 2020 2020 7261  ist]:.        ra
+00018120: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
+00018130: 7665 7274 6963 6573 6020 6d75 7374 2062  vertices` must b
+00018140: 6520 6120 6c69 7374 206f 7220 6120 6e75  e a list or a nu
+00018150: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
+00018160: 2020 2065 6c69 6620 6e75 6d70 792e 6173     elif numpy.as
+00018170: 6172 7261 7928 7665 7274 6963 6573 292e  array(vertices).
+00018180: 7368 6170 6520 213d 2028 342c 2033 293a  shape != (4, 3):
+00018190: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+000181a0: 616c 7565 4572 726f 7228 2260 7665 7274  alueError("`vert
+000181b0: 6963 6573 6020 6861 7320 696e 636f 7272  ices` has incorr
+000181c0: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
+000181d0: 7374 2062 6520 2834 2c20 3329 2e22 290a  st be (4, 3).").
+000181e0: 2020 2020 6966 2074 7970 6528 7374 6570      if type(step
+000181f0: 2920 6e6f 7420 696e 205b 666c 6f61 742c  ) not in [float,
+00018200: 2069 6e74 5d3a 0a20 2020 2020 2020 2072   int]:.        r
+00018210: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+00018220: 6073 7465 7060 206d 7573 7420 6265 2061  `step` must be a
+00018230: 2070 6f73 6974 6976 6520 7265 616c 206e   positive real n
+00018240: 756d 6265 722e 2229 0a20 2020 2065 6c69  umber.").    eli
+00018250: 6620 7374 6570 203c 3d20 302e 303a 0a20  f step <= 0.0:. 
+00018260: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00018270: 7565 4572 726f 7228 2260 7374 6570 6020  ueError("`step` 
+00018280: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+00018290: 7665 2072 6561 6c20 6e75 6d62 6572 2e22  ve real number."
+000182a0: 290a 2020 2020 6966 2042 2069 7320 6e6f  ).    if B is no
+000182b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000182c0: 6966 2074 7970 6528 4229 206e 6f74 2069  if type(B) not i
+000182d0: 6e20 5b6e 756d 7079 2e6e 6461 7272 6179  n [numpy.ndarray
+000182e0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
+000182f0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+00018300: 6042 6020 6d75 7374 2062 6520 6120 6e75  `B` must be a nu
+00018310: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
+00018320: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
+00018330: 422e 7368 6170 6529 2021 3d20 333a 0a20  B.shape) != 3:. 
+00018340: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00018350: 2056 616c 7565 4572 726f 7228 2260 4260   ValueError("`B`
+00018360: 2068 6173 2074 6865 2069 6e63 6f72 7265   has the incorre
+00018370: 6374 2073 6861 7065 2e20 4974 206d 7573  ct shape. It mus
+00018380: 7420 6265 2028 6e78 2c20 6e79 2c20 6e7a  t be (nx, ny, nz
+00018390: 292e 2229 0a20 2020 2069 6620 5120 6973  ).").    if Q is
+000183a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000183b0: 2020 2069 6620 7479 7065 2851 2920 6e6f     if type(Q) no
+000183c0: 7420 696e 205b 6e75 6d70 792e 6e64 6172  t in [numpy.ndar
+000183d0: 7261 795d 3a0a 2020 2020 2020 2020 2020  ray]:.          
+000183e0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+000183f0: 7228 2260 5160 206d 7573 7420 6265 2061  r("`Q` must be a
+00018400: 206e 756d 7079 2e6e 6461 7272 6179 2e22   numpy.ndarray."
+00018410: 290a 2020 2020 2020 2020 656c 6966 206c  ).        elif l
+00018420: 656e 2851 2e73 6861 7065 2920 213d 2033  en(Q.shape) != 3
+00018430: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00018440: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00018450: 6051 6020 6861 7320 7468 6520 696e 636f  `Q` has the inco
+00018460: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+00018470: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
+00018480: 206e 7a29 2e22 290a 2020 2020 6966 2073   nz).").    if s
+00018490: 656c 6563 7469 6f6e 2069 7320 6e6f 7420  election is not 
+000184a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2320  None:.        # 
+000184b0: 4368 6563 6b20 7365 6c65 6374 696f 6e20  Check selection 
+000184c0: 7479 7065 730a 2020 2020 2020 2020 6966  types.        if
+000184d0: 2061 6c6c 2869 7369 6e73 7461 6e63 6528   all(isinstance(
+000184e0: 782c 2069 6e74 2920 666f 7220 7820 696e  x, int) for x in
+000184f0: 2073 656c 6563 7469 6f6e 293a 0a20 2020   selection):.   
+00018500: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00018510: 2020 2020 2020 656c 6966 2061 6c6c 2869        elif all(i
+00018520: 7369 6e73 7461 6e63 6528 782c 2073 7472  sinstance(x, str
+00018530: 2920 666f 7220 7820 696e 2073 656c 6563  ) for x in selec
+00018540: 7469 6f6e 293a 0a20 2020 2020 2020 2020  tion):.         
+00018550: 2020 2073 656c 6563 7469 6f6e 203d 205b     selection = [
+00018560: 5f67 6574 5f63 6176 6974 795f 6c61 6265  _get_cavity_labe
+00018570: 6c28 7365 6c65 2920 666f 7220 7365 6c65  l(sele) for sele
+00018580: 2069 6e20 7365 6c65 6374 696f 6e5d 0a20   in selection]. 
+00018590: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000185a0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+000185b0: 7970 6545 7272 6f72 280a 2020 2020 2020  ypeError(.      
+000185c0: 2020 2020 2020 2020 2020 2260 7365 6c65            "`sele
+000185d0: 6374 696f 6e60 206d 7573 7420 6265 2061  ction` must be a
+000185e0: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
+000185f0: 2028 6361 7669 7479 206e 616d 6573 2920   (cavity names) 
+00018600: 6f72 2069 6e74 6567 6572 7320 2863 6176  or integers (cav
+00018610: 6974 7920 6c61 6265 6c73 292e 220a 2020  ity labels).".  
+00018620: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00018630: 2020 2020 2320 4368 6563 6b20 6966 2073      # Check if s
+00018640: 656c 6563 7469 6f6e 2069 6e63 6c75 6465  election include
+00018650: 7320 7661 6c69 6420 6361 7669 7479 206c  s valid cavity l
+00018660: 6162 656c 730a 2020 2020 2020 2020 6966  abels.        if
+00018670: 2061 6e79 2878 203c 2032 2066 6f72 2078   any(x < 2 for x
+00018680: 2069 6e20 7365 6c65 6374 696f 6e29 3a0a   in selection):.
+00018690: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000186a0: 6520 5661 6c75 6545 7272 6f72 2866 2249  e ValueError(f"I
+000186b0: 6e76 616c 6964 2060 7365 6c65 6374 696f  nvalid `selectio
+000186c0: 6e60 3a20 7b73 656c 6563 7469 6f6e 7d2e  n`: {selection}.
+000186d0: 2229 0a20 2020 2069 6620 6e74 6872 6561  ").    if nthrea
+000186e0: 6473 2069 7320 4e6f 6e65 3a0a 2020 2020  ds is None:.    
+000186f0: 2020 2020 6e74 6872 6561 6473 203d 206f      nthreads = o
+00018700: 732e 6370 755f 636f 756e 7428 2920 2d20  s.cpu_count() - 
+00018710: 310a 2020 2020 656c 7365 3a0a 2020 2020  1.    else:.    
+00018720: 2020 2020 6966 2074 7970 6528 6e74 6872      if type(nthr
+00018730: 6561 6473 2920 6e6f 7420 696e 205b 696e  eads) not in [in
+00018740: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
+00018750: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00018760: 2260 6e74 6872 6561 6473 6020 6d75 7374  "`nthreads` must
+00018770: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
+00018780: 6e74 6567 6572 2e22 290a 2020 2020 2020  nteger.").      
+00018790: 2020 656c 6966 206e 7468 7265 6164 7320    elif nthreads 
+000187a0: 3c3d 2030 3a0a 2020 2020 2020 2020 2020  <= 0:.          
+000187b0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000187c0: 6f72 2822 606e 7468 7265 6164 7360 206d  or("`nthreads` m
+000187d0: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
+000187e0: 6520 696e 7465 6765 722e 2229 0a20 2020  e integer.").   
+000187f0: 2069 6620 7479 7065 2861 7070 656e 6429   if type(append)
+00018800: 206e 6f74 2069 6e20 5b62 6f6f 6c5d 3a0a   not in [bool]:.
+00018810: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00018820: 7065 4572 726f 7228 2260 6170 7065 6e64  peError("`append
+00018830: 6020 6d75 7374 2062 6520 6120 626f 6f6c  ` must be a bool
+00018840: 6561 6e2e 2229 0a20 2020 2069 6620 7479  ean.").    if ty
+00018850: 7065 286d 6f64 656c 2920 6e6f 7420 696e  pe(model) not in
+00018860: 205b 696e 745d 3a0a 2020 2020 2020 2020   [int]:.        
+00018870: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00018880: 2260 6d6f 6465 6c60 206d 7573 7420 6265  "`model` must be
+00018890: 2061 2069 6e74 6567 6572 2e22 290a 0a20   a integer.").. 
+000188a0: 2020 2023 2043 6f6e 7665 7274 2074 7970     # Convert typ
+000188b0: 6573 0a20 2020 2069 6620 7479 7065 2876  es.    if type(v
+000188c0: 6572 7469 6365 7329 203d 3d20 6c69 7374  ertices) == list
+000188d0: 3a0a 2020 2020 2020 2020 7665 7274 6963  :.        vertic
+000188e0: 6573 203d 206e 756d 7079 2e61 7361 7272  es = numpy.asarr
+000188f0: 6179 2876 6572 7469 6365 7329 0a20 2020  ay(vertices).   
+00018900: 2069 6620 7479 7065 2873 7465 7029 203d   if type(step) =
+00018910: 3d20 696e 743a 0a20 2020 2020 2020 2073  = int:.        s
+00018920: 7465 7020 3d20 666c 6f61 7428 7374 6570  tep = float(step
+00018930: 290a 0a20 2020 2023 2043 6f6e 7665 7274  )..    # Convert
+00018940: 206e 756d 7079 2e6e 6461 7272 6179 2064   numpy.ndarray d
+00018950: 6174 6120 7479 7065 730a 2020 2020 7665  ata types.    ve
+00018960: 7274 6963 6573 203d 2076 6572 7469 6365  rtices = vertice
+00018970: 732e 6173 7479 7065 2822 666c 6f61 7436  s.astype("float6
+00018980: 3422 2920 6966 2076 6572 7469 6365 732e  4") if vertices.
+00018990: 6474 7970 6520 213d 2022 666c 6f61 7436  dtype != "float6
+000189a0: 3422 2065 6c73 6520 7665 7274 6963 6573  4" else vertices
+000189b0: 0a20 2020 2069 6620 4220 6973 206e 6f74  .    if B is not
+000189c0: 204e 6f6e 653a 0a20 2020 2020 2020 2042   None:.        B
+000189d0: 203d 2042 2e61 7374 7970 6528 2266 6c6f   = B.astype("flo
+000189e0: 6174 3634 2229 2069 6620 422e 6474 7970  at64") if B.dtyp
+000189f0: 6520 213d 2022 666c 6f61 7436 3422 2065  e != "float64" e
+00018a00: 6c73 6520 420a 2020 2020 6966 2051 2069  lse B.    if Q i
+00018a10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00018a20: 2020 2020 5120 3d20 512e 6173 7479 7065      Q = Q.astype
+00018a30: 2822 666c 6f61 7436 3422 2920 6966 2051  ("float64") if Q
+00018a40: 2e64 7479 7065 2021 3d20 2266 6c6f 6174  .dtype != "float
+00018a50: 3634 2220 656c 7365 2051 0a0a 2020 2020  64" else Q..    
+00018a60: 2320 4765 7420 7369 6e63 6f73 3a20 7369  # Get sincos: si
+00018a70: 6e65 2061 6e64 2063 6f73 696e 6520 6f66  ne and cosine of
+00018a80: 2074 6865 2067 7269 6420 726f 7461 7469   the grid rotati
+00018a90: 6f6e 2061 6e67 6c65 7320 2873 696e 612c  on angles (sina,
+00018aa0: 2063 6f73 612c 2073 696e 622c 2063 6f73   cosa, sinb, cos
+00018ab0: 6229 0a20 2020 2073 696e 636f 7320 3d20  b).    sincos = 
+00018ac0: 5f67 6574 5f73 696e 636f 7328 7665 7274  _get_sincos(vert
+00018ad0: 6963 6573 290a 0a20 2020 2023 2055 6e70  ices)..    # Unp
+00018ae0: 6163 6b20 7665 7274 6963 6573 0a20 2020  ack vertices.   
+00018af0: 2050 312c 205f 2c20 5f2c 205f 203d 2076   P1, _, _, _ = v
+00018b00: 6572 7469 6365 730a 0a20 2020 2023 2049  ertices..    # I
+00018b10: 6620 7375 7266 6163 6520 6973 204e 6f6e  f surface is Non
+00018b20: 652c 2063 7265 6174 6520 6120 7a65 726f  e, create a zero
+00018b30: 7320 6772 6964 0a20 2020 2069 6620 7375  s grid.    if su
+00018b40: 7266 6163 6520 6973 204e 6f6e 653a 0a20  rface is None:. 
+00018b50: 2020 2020 2020 2073 7572 6661 6365 203d         surface =
+00018b60: 206e 756d 7079 2e7a 6572 6f73 2863 6176   numpy.zeros(cav
+00018b70: 6974 6965 732e 7368 6170 652c 2064 7479  ities.shape, dty
+00018b80: 7065 3d22 696e 7433 3222 290a 0a20 2020  pe="int32")..   
+00018b90: 2023 2049 6620 4220 6973 204e 6f6e 652c   # If B is None,
+00018ba0: 2063 7265 6174 6520 6120 7a65 726f 7320   create a zeros 
+00018bb0: 6772 6964 0a20 2020 2069 6620 4220 6973  grid.    if B is
+00018bc0: 204e 6f6e 653a 0a20 2020 2020 2020 2042   None:.        B
+00018bd0: 203d 206e 756d 7079 2e7a 6572 6f73 2863   = numpy.zeros(c
+00018be0: 6176 6974 6965 732e 7368 6170 652c 2064  avities.shape, d
+00018bf0: 7479 7065 3d22 666c 6f61 7436 3422 290a  type="float64").
+00018c00: 0a20 2020 2023 2049 6620 5120 6973 204e  .    # If Q is N
+00018c10: 6f6e 652c 2063 7265 6174 6520 616e 206f  one, create an o
+00018c20: 6e65 7320 6772 6964 0a20 2020 2069 6620  nes grid.    if 
+00018c30: 5120 6973 204e 6f6e 653a 0a20 2020 2020  Q is None:.     
+00018c40: 2020 2051 203d 206e 756d 7079 2e6f 6e65     Q = numpy.one
+00018c50: 7328 6361 7669 7469 6573 2e73 6861 7065  s(cavities.shape
+00018c60: 2c20 6474 7970 653d 2266 6c6f 6174 3634  , dtype="float64
+00018c70: 2229 0a0a 2020 2020 2320 5365 6c65 6374  ")..    # Select
+00018c80: 2063 6176 6974 6965 730a 2020 2020 6966   cavities.    if
+00018c90: 2073 656c 6563 7469 6f6e 2069 7320 6e6f   selection is no
+00018ca0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00018cb0: 6361 7669 7469 6573 203d 205f 7365 6c65  cavities = _sele
+00018cc0: 6374 5f63 6176 6974 6965 7328 6361 7669  ct_cavities(cavi
+00018cd0: 7469 6573 2c20 7365 6c65 6374 696f 6e29  ties, selection)
+00018ce0: 0a20 2020 2020 2020 2073 7572 6661 6365  .        surface
+00018cf0: 203d 205f 7365 6c65 6374 5f63 6176 6974   = _select_cavit
+00018d00: 6965 7328 7375 7266 6163 652c 2073 656c  ies(surface, sel
+00018d10: 6563 7469 6f6e 290a 0a20 2020 2023 2047  ection)..    # G
+00018d20: 6574 206e 756d 6265 7220 6f66 2063 6176  et number of cav
+00018d30: 6974 6965 730a 2020 2020 6e63 6176 203d  ities.    ncav =
+00018d40: 2069 6e74 2863 6176 6974 6965 732e 6d61   int(cavities.ma
+00018d50: 7828 2920 2d20 3129 0a0a 2020 2020 2320  x() - 1)..    # 
+00018d60: 4578 706f 7274 2063 6176 6974 6965 730a  Export cavities.
+00018d70: 2020 2020 5f65 7870 6f72 7428 0a20 2020      _export(.   
+00018d80: 2020 2020 2066 6e2c 2063 6176 6974 6965       fn, cavitie
+00018d90: 732c 2073 7572 6661 6365 2c20 422c 2051  s, surface, B, Q
+00018da0: 2c20 5031 2c20 7369 6e63 6f73 2c20 7374  , P1, sincos, st
+00018db0: 6570 2c20 6e63 6176 2c20 6e74 6872 6561  ep, ncav, nthrea
+00018dc0: 6473 2c20 6170 7065 6e64 2c20 6d6f 6465  ds, append, mode
+00018dd0: 6c0a 2020 2020 290a 0a0a 6465 6620 6578  l.    )...def ex
+00018de0: 706f 7274 5f6f 7065 6e69 6e67 7328 0a20  port_openings(. 
+00018df0: 2020 2066 6e3a 2055 6e69 6f6e 5b73 7472     fn: Union[str
+00018e00: 2c20 7061 7468 6c69 622e 5061 7468 5d2c  , pathlib.Path],
+00018e10: 0a20 2020 206f 7065 6e69 6e67 733a 206e  .    openings: n
+00018e20: 756d 7079 2e6e 6461 7272 6179 2c0a 2020  umpy.ndarray,.  
+00018e30: 2020 7665 7274 6963 6573 3a20 556e 696f    vertices: Unio
+00018e40: 6e5b 6e75 6d70 792e 6e64 6172 7261 792c  n[numpy.ndarray,
+00018e50: 204c 6973 745b 4c69 7374 5b66 6c6f 6174   List[List[float
+00018e60: 5d5d 5d2c 0a20 2020 2073 7465 703a 2055  ]]],.    step: U
+00018e70: 6e69 6f6e 5b66 6c6f 6174 2c20 696e 745d  nion[float, int]
+00018e80: 203d 2030 2e36 2c0a 2020 2020 7365 6c65   = 0.6,.    sele
+00018e90: 6374 696f 6e3a 204f 7074 696f 6e61 6c5b  ction: Optional[
+00018ea0: 556e 696f 6e5b 4c69 7374 5b69 6e74 5d2c  Union[List[int],
+00018eb0: 204c 6973 745b 7374 725d 5d5d 203d 204e   List[str]]] = N
+00018ec0: 6f6e 652c 0a20 2020 206e 7468 7265 6164  one,.    nthread
+00018ed0: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
+00018ee0: 203d 204e 6f6e 652c 0a20 2020 2061 7070   = None,.    app
+00018ef0: 656e 643a 2062 6f6f 6c20 3d20 4661 6c73  end: bool = Fals
+00018f00: 652c 0a20 2020 206d 6f64 656c 3a20 696e  e,.    model: in
+00018f10: 7420 3d20 302c 0a29 202d 3e20 4e6f 6e65  t = 0,.) -> None
+00018f20: 3a0a 2020 2020 2222 2245 7870 6f72 7420  :.    """Export 
+00018f30: 6f70 656e 696e 6720 706f 696e 7473 2028  opening points (
+00018f40: 4829 2074 6f20 6120 5044 422d 666f 726d  H) to a PDB-form
+00018f50: 6174 7465 6420 6669 6c65 2e0a 0a20 2020  atted file...   
+00018f60: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00018f70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
+00018f80: 6e20 3a20 556e 696f 6e5b 7374 722c 2070  n : Union[str, p
+00018f90: 6174 686c 6962 2e50 6174 685d 0a20 2020  athlib.Path].   
+00018fa0: 2020 2020 2041 2070 6174 6820 746f 2050       A path to P
+00018fb0: 4442 2066 696c 6520 666f 7220 7772 6974  DB file for writ
+00018fc0: 696e 6720 6f70 656e 696e 6773 2e0a 2020  ing openings..  
+00018fd0: 2020 6f70 656e 696e 6773 203a 206e 756d    openings : num
+00018fe0: 7079 2e6e 6461 7272 6179 0a20 2020 2020  py.ndarray.     
+00018ff0: 2020 204f 7065 6e69 6e67 7320 706f 696e     Openings poin
+00019000: 7473 2069 6e20 7468 6520 3344 2067 7269  ts in the 3D gri
+00019010: 6420 286f 7065 6e69 6e67 735b 6e78 5d5b  d (openings[nx][
+00019020: 6e79 5d5b 6e7a 5d29 2e0a 2020 2020 2020  ny][nz])..      
+00019030: 2020 4f70 656e 696e 6773 2061 7272 6179    Openings array
+00019040: 2068 6173 2069 6e74 6567 6572 206c 6162   has integer lab
+00019050: 656c 7320 696e 2065 6163 6820 706f 7369  els in each posi
+00019060: 7469 6f6e 2c20 7468 6174 2061 7265 3a0a  tion, that are:.
+00019070: 0a20 2020 2020 2020 2020 2020 202a 202d  .            * -
+00019080: 313a 2062 756c 6b20 706f 696e 7473 3b0a  1: bulk points;.
+00019090: 0a20 2020 2020 2020 2020 2020 202a 2030  .            * 0
+000190a0: 3a20 6361 7669 7479 206f 7220 6269 6f6d  : cavity or biom
+000190b0: 6f6c 6563 756c 6520 706f 696e 7473 3b0a  olecule points;.
+000190c0: 0a20 2020 2020 2020 2020 2020 202a 2031  .            * 1
+000190d0: 3a20 656d 7074 7920 7370 6163 6520 706f  : empty space po
+000190e0: 696e 7473 3b0a 0a20 2020 2020 2020 2020  ints;..         
+000190f0: 2020 202a 203e 3d32 3a20 4f70 656e 696e     * >=2: Openin
+00019100: 6720 706f 696e 7473 2e0a 0a20 2020 2020  g points...     
+00019110: 2020 2054 6865 2065 6d70 7479 2073 7061     The empty spa
+00019120: 6365 2070 6f69 6e74 7320 6172 6520 7265  ce points are re
+00019130: 6769 6f6e 7320 7468 6174 2064 6f20 6e6f  gions that do no
+00019140: 7420 6d65 6574 2074 6865 2063 686f 7365  t meet the chose
+00019150: 6e0a 2020 2020 2020 2020 6f70 656e 696e  n.        openin
+00019160: 6773 2063 7574 6f66 6620 746f 2062 6520  gs cutoff to be 
+00019170: 636f 6e73 6964 6572 6564 2061 6e20 6f70  considered an op
+00019180: 656e 696e 672e 0a20 2020 2076 6572 7469  ening..    verti
+00019190: 6365 7320 3a20 556e 696f 6e5b 6e75 6d70  ces : Union[nump
+000191a0: 792e 6e64 6172 7261 792c 204c 6973 745b  y.ndarray, List[
+000191b0: 4c69 7374 5b66 6c6f 6174 5d5d 5d0a 2020  List[float]]].  
+000191c0: 2020 2020 2020 4120 6e75 6d70 792e 6e64        A numpy.nd
+000191d0: 6172 7261 7920 6f72 2061 206c 6973 7420  array or a list 
+000191e0: 7769 7468 2078 797a 2076 6572 7469 6365  with xyz vertice
+000191f0: 7320 636f 6f72 6469 6e61 7465 7320 286f  s coordinates (o
+00019200: 7269 6769 6e2c 0a20 2020 2020 2020 2058  rigin,.        X
+00019210: 2d61 7869 732c 2059 2d61 7869 732c 205a  -axis, Y-axis, Z
+00019220: 2d61 7869 7329 2e0a 2020 2020 7374 6570  -axis)..    step
+00019230: 203a 2055 6e69 6f6e 5b66 6c6f 6174 2c20   : Union[float, 
+00019240: 696e 745d 2c20 6f70 7469 6f6e 616c 0a20  int], optional. 
+00019250: 2020 2020 2020 2047 7269 6420 7370 6163         Grid spac
+00019260: 696e 6720 2841 292c 2062 7920 6465 6661  ing (A), by defa
+00019270: 756c 7420 302e 362e 0a20 2020 2073 656c  ult 0.6..    sel
+00019280: 6563 7469 6f6e 203a 2055 6e69 6f6e 5b4c  ection : Union[L
+00019290: 6973 745b 696e 745d 2c20 4c69 7374 5b73  ist[int], List[s
+000192a0: 7472 5d5d 2c20 6f70 7469 6f6e 616c 0a20  tr]], optional. 
+000192b0: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
+000192c0: 2069 6e74 6567 6572 206c 6162 656c 7320   integer labels 
+000192d0: 6f72 2061 206c 6973 7420 6f66 206f 7065  or a list of ope
+000192e0: 6e69 6e67 206e 616d 6573 2074 6f20 6265  ning names to be
+000192f0: 2073 656c 6563 7465 642c 2062 7920 6465   selected, by de
+00019300: 6661 756c 7420 4e6f 6e65 2e0a 2020 2020  fault None..    
+00019310: 6e74 6872 6561 6473 203a 2069 6e74 2c20  nthreads : int, 
+00019320: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00019330: 204e 756d 6265 7220 6f66 2074 6872 6561   Number of threa
+00019340: 6473 2c20 6279 2064 6566 6175 6c74 204e  ds, by default N
+00019350: 6f6e 652e 2049 6620 4e6f 6e65 2c20 7468  one. If None, th
+00019360: 6520 6e75 6d62 6572 206f 6620 7468 7265  e number of thre
+00019370: 6164 7320 6973 0a20 2020 2020 2020 2060  ads is.        `
+00019380: 6f73 2e63 7075 5f63 6f75 6e74 2829 202d  os.cpu_count() -
+00019390: 2031 602e 0a20 2020 2061 7070 656e 6420   1`..    append 
+000193a0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+000193b0: 0a20 2020 2020 2020 2057 6865 7468 6572  .        Whether
+000193c0: 2074 6f20 6170 7065 6e64 206f 7065 6e69   to append openi
+000193d0: 6e67 7320 746f 2074 6865 2050 4442 2066  ngs to the PDB f
+000193e0: 696c 652c 2062 7920 6465 6661 756c 7420  ile, by default 
+000193f0: 4661 6c73 652e 0a20 2020 206d 6f64 656c  False..    model
+00019400: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+00019410: 0a20 2020 2020 2020 204d 6f64 656c 206e  .        Model n
+00019420: 756d 6265 722c 2062 7920 6465 6661 756c  umber, by defaul
+00019430: 7420 302e 0a0a 2020 2020 5261 6973 6573  t 0...    Raises
+00019440: 0a20 2020 202d 2d2d 2d2d 2d0a 2020 2020  .    ------.    
+00019450: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
+00019460: 2020 606f 7065 6e69 6e67 7360 206d 7573    `openings` mus
+00019470: 7420 6265 2061 206e 756d 7079 2e6e 6461  t be a numpy.nda
+00019480: 7272 6179 2e0a 2020 2020 5661 6c75 6545  rray..    ValueE
+00019490: 7272 6f72 0a20 2020 2020 2020 2060 6f70  rror.        `op
+000194a0: 656e 696e 6773 6020 6861 7320 7468 6520  enings` has the 
+000194b0: 696e 636f 7272 6563 7420 7368 6170 652e  incorrect shape.
+000194c0: 2049 7420 6d75 7374 2062 6520 286e 782c   It must be (nx,
+000194d0: 206e 792c 206e 7a29 2e0a 2020 2020 5479   ny, nz)..    Ty
+000194e0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+000194f0: 6076 6572 7469 6365 7360 206d 7573 7420  `vertices` must 
+00019500: 6265 2061 206c 6973 7420 6f72 2061 206e  be a list or a n
+00019510: 756d 7079 2e6e 6461 7272 6179 2e0a 2020  umpy.ndarray..  
+00019520: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
+00019530: 2020 2020 2060 7665 7274 6963 6573 6020       `vertices` 
+00019540: 6861 7320 696e 636f 7272 6563 7420 7368  has incorrect sh
+00019550: 6170 652e 2049 7420 6d75 7374 2062 6520  ape. It must be 
+00019560: 2834 2c20 3329 2e0a 2020 2020 5479 7065  (4, 3)..    Type
+00019570: 4572 726f 720a 2020 2020 2020 2020 6073  Error.        `s
+00019580: 7465 7060 206d 7573 7420 6265 2061 2070  tep` must be a p
+00019590: 6f73 6974 6976 6520 7265 616c 206e 756d  ositive real num
+000195a0: 6265 722e 0a20 2020 2056 616c 7565 4572  ber..    ValueEr
+000195b0: 726f 720a 2020 2020 2020 2020 6073 7465  ror.        `ste
+000195c0: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
+000195d0: 6974 6976 6520 7265 616c 206e 756d 6265  itive real numbe
+000195e0: 722e 0a20 2020 2054 7970 6545 7272 6f72  r..    TypeError
+000195f0: 0a20 2020 2020 2020 2060 7365 6c65 6374  .        `select
+00019600: 696f 6e60 206d 7573 7420 6265 2061 206c  ion` must be a l
+00019610: 6973 7420 6f66 2073 7472 696e 6773 2028  ist of strings (
+00019620: 6f70 656e 696e 6720 6e61 6d65 7329 206f  opening names) o
+00019630: 7220 696e 7465 6765 7273 2028 6f70 656e  r integers (open
+00019640: 696e 6720 6c61 6265 6c73 292e 0a20 2020  ing labels)..   
+00019650: 2056 616c 7565 4572 726f 720a 2020 2020   ValueError.    
+00019660: 2020 2020 496e 7661 6c69 6420 6073 656c      Invalid `sel
+00019670: 6563 7469 6f6e 603a 207b 7365 6c65 6374  ection`: {select
+00019680: 696f 6e7d 2e0a 2020 2020 5479 7065 4572  ion}..    TypeEr
+00019690: 726f 720a 2020 2020 2020 2020 606e 7468  ror.        `nth
+000196a0: 7265 6164 7360 206d 7573 7420 6265 2061  reads` must be a
+000196b0: 2070 6f73 6974 6976 6520 696e 7465 6765   positive intege
+000196c0: 722e 0a20 2020 2056 616c 7565 4572 726f  r..    ValueErro
+000196d0: 720a 2020 2020 2020 2020 606e 7468 7265  r.        `nthre
+000196e0: 6164 7360 206d 7573 7420 6265 2061 2070  ads` must be a p
+000196f0: 6f73 6974 6976 6520 696e 7465 6765 722e  ositive integer.
+00019700: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
+00019710: 2020 2020 2020 2060 6170 7065 6e64 6020         `append` 
+00019720: 6d75 7374 2062 6520 6120 626f 6f6c 6561  must be a boolea
+00019730: 6e2e 0a20 2020 2054 7970 6545 7272 6f72  n..    TypeError
+00019740: 0a20 2020 2020 2020 2060 6d6f 6465 6c60  .        `model`
+00019750: 206d 7573 7420 6265 2061 2069 6e74 6567   must be a integ
+00019760: 6572 2e0a 2020 2020 5479 7065 4572 726f  er..    TypeErro
+00019770: 720a 2020 2020 2020 2020 6066 6e60 206d  r.        `fn` m
+00019780: 7573 7420 6265 2061 2073 7472 696e 6720  ust be a string 
+00019790: 6f72 2070 6174 686c 6962 2e50 6174 682e  or pathlib.Path.
+000197a0: 0a0a 2020 2020 4e6f 7465 0a20 2020 202d  ..    Note.    -
+000197b0: 2d2d 2d0a 2020 2020 5468 6520 6f70 656e  ---.    The open
+000197c0: 696e 6720 6e6f 6d65 6e63 6c61 7475 7265  ing nomenclature
+000197d0: 2069 7320 6261 7365 6420 6f6e 2074 6865   is based on the
+000197e0: 2069 6e74 6567 6572 206c 6162 656c 2e20   integer label. 
+000197f0: 5468 6520 6f70 656e 696e 6720 6d61 726b  The opening mark
+00019800: 6564 0a20 2020 2077 6974 6820 322c 2074  ed.    with 2, t
+00019810: 6865 2066 6972 7374 2069 6e74 6567 6572  he first integer
+00019820: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00019830: 6f20 6120 6f70 656e 696e 672c 2069 7320  o a opening, is 
+00019840: 4f41 412c 2074 6865 206f 7065 6e69 6e67  OAA, the opening
+00019850: 0a20 2020 206d 6172 6b65 6420 7769 7468  .    marked with
+00019860: 2033 2069 7320 4f41 422c 2074 6865 206f   3 is OAB, the o
+00019870: 7065 6e69 6e67 206d 6172 6b65 6420 7769  pening marked wi
+00019880: 7468 2034 2069 7320 4f41 4320 616e 6420  th 4 is OAC and 
+00019890: 736f 206f 6e2e 0a0a 2020 2020 5365 6520  so on...    See 
+000198a0: 416c 736f 0a20 2020 202d 2d2d 2d2d 2d2d  Also.    -------
+000198b0: 2d0a 2020 2020 6578 706f 7274 0a20 2020  -.    export.   
+000198c0: 2064 6574 6563 740a 2020 2020 6465 7074   detect.    dept
+000198d0: 6873 0a20 2020 206f 7065 6e69 6e67 730a  hs.    openings.
+000198e0: 0a20 2020 2045 7861 6d70 6c65 0a20 2020  .    Example.   
+000198f0: 202d 2d2d 2d2d 2d2d 0a20 2020 2057 6974   -------.    Wit
+00019900: 6820 7468 6520 6f70 656e 696e 6720 706f  h the opening po
+00019910: 696e 7473 2069 6465 6e74 6966 6965 6420  ints identified 
+00019920: 7769 7468 2060 606f 7065 6e69 6e67 7360  with ``openings`
+00019930: 602c 2077 6520 6361 6e20 6578 706f 7274  `, we can export
+00019940: 2074 6865 6d20 746f 2061 2050 4442 2d66   them to a PDB-f
+00019950: 6f72 6d61 7474 6564 2066 696c 653a 0a0a  ormatted file:..
+00019960: 2020 2020 3e3e 3e20 6672 6f6d 2070 794b      >>> from pyK
+00019970: 5646 696e 6465 7220 696d 706f 7274 2065  VFinder import e
+00019980: 7870 6f72 745f 6f70 656e 696e 6773 0a20  xport_openings. 
+00019990: 2020 203e 3e3e 2065 7870 6f72 745f 6f70     >>> export_op
+000199a0: 656e 696e 6773 2827 6f70 656e 696e 6773  enings('openings
+000199b0: 2e70 6462 272c 206f 7065 6e69 6e67 732c  .pdb', openings,
+000199c0: 2076 6572 7469 6365 7329 0a20 2020 2022   vertices).    "
+000199d0: 2222 0a20 2020 2066 726f 6d20 5f70 794b  "".    from _pyK
+000199e0: 5646 696e 6465 7220 696d 706f 7274 205f  VFinder import _
+000199f0: 6578 706f 7274 5f6f 7065 6e69 6e67 730a  export_openings.
+00019a00: 0a20 2020 2023 2043 6865 636b 2061 7267  .    # Check arg
+00019a10: 756d 656e 7473 0a20 2020 2069 6620 7479  uments.    if ty
+00019a20: 7065 286f 7065 6e69 6e67 7329 206e 6f74  pe(openings) not
+00019a30: 2069 6e20 5b6e 756d 7079 2e6e 6461 7272   in [numpy.ndarr
+00019a40: 6179 5d3a 0a20 2020 2020 2020 2072 6169  ay]:.        rai
+00019a50: 7365 2054 7970 6545 7272 6f72 2822 606f  se TypeError("`o
+00019a60: 7065 6e69 6e67 7360 206d 7573 7420 6265  penings` must be
+00019a70: 2061 206e 756d 7079 2e6e 6461 7272 6179   a numpy.ndarray
+00019a80: 2e22 290a 2020 2020 656c 6966 206c 656e  .").    elif len
+00019a90: 286f 7065 6e69 6e67 732e 7368 6170 6529  (openings.shape)
+00019aa0: 2021 3d20 333a 0a20 2020 2020 2020 2072   != 3:.        r
+00019ab0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00019ac0: 2260 6f70 656e 696e 6773 6020 6861 7320  "`openings` has 
+00019ad0: 7468 6520 696e 636f 7272 6563 7420 7368  the incorrect sh
+00019ae0: 6170 652e 2049 7420 6d75 7374 2062 6520  ape. It must be 
+00019af0: 286e 782c 206e 792c 206e 7a29 2e22 290a  (nx, ny, nz).").
+00019b00: 2020 2020 6966 2074 7970 6528 7665 7274      if type(vert
+00019b10: 6963 6573 2920 6e6f 7420 696e 205b 6e75  ices) not in [nu
+00019b20: 6d70 792e 6e64 6172 7261 792c 206c 6973  mpy.ndarray, lis
+00019b30: 745d 3a0a 2020 2020 2020 2020 7261 6973  t]:.        rais
+00019b40: 6520 5479 7065 4572 726f 7228 2260 7665  e TypeError("`ve
+00019b50: 7274 6963 6573 6020 6d75 7374 2062 6520  rtices` must be 
+00019b60: 6120 6c69 7374 206f 7220 6120 6e75 6d70  a list or a nump
+00019b70: 792e 6e64 6172 7261 792e 2229 0a20 2020  y.ndarray.").   
+00019b80: 2065 6c69 6620 6e75 6d70 792e 6173 6172   elif numpy.asar
+00019b90: 7261 7928 7665 7274 6963 6573 292e 7368  ray(vertices).sh
+00019ba0: 6170 6520 213d 2028 342c 2033 293a 0a20  ape != (4, 3):. 
+00019bb0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00019bc0: 7565 4572 726f 7228 2260 7665 7274 6963  ueError("`vertic
+00019bd0: 6573 6020 6861 7320 696e 636f 7272 6563  es` has incorrec
+00019be0: 7420 7368 6170 652e 2049 7420 6d75 7374  t shape. It must
+00019bf0: 2062 6520 2834 2c20 3329 2e22 290a 2020   be (4, 3).").  
+00019c00: 2020 6966 2074 7970 6528 7374 6570 2920    if type(step) 
+00019c10: 6e6f 7420 696e 205b 666c 6f61 742c 2069  not in [float, i
+00019c20: 6e74 5d3a 0a20 2020 2020 2020 2072 6169  nt]:.        rai
+00019c30: 7365 2054 7970 6545 7272 6f72 2822 6073  se TypeError("`s
+00019c40: 7465 7060 206d 7573 7420 6265 2061 2070  tep` must be a p
+00019c50: 6f73 6974 6976 6520 7265 616c 206e 756d  ositive real num
+00019c60: 6265 722e 2229 0a20 2020 2065 6c69 6620  ber.").    elif 
+00019c70: 7374 6570 203c 3d20 302e 303a 0a20 2020  step <= 0.0:.   
+00019c80: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00019c90: 4572 726f 7228 2260 7374 6570 6020 6d75  Error("`step` mu
+00019ca0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+00019cb0: 2072 6561 6c20 6e75 6d62 6572 2e22 290a   real number.").
+00019cc0: 2020 2020 6966 2073 656c 6563 7469 6f6e      if selection
+00019cd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019ce0: 2020 2020 2020 2320 4368 6563 6b20 7365        # Check se
+00019cf0: 6c65 6374 696f 6e20 7479 7065 730a 2020  lection types.  
+00019d00: 2020 2020 2020 6966 2061 6c6c 2869 7369        if all(isi
+00019d10: 6e73 7461 6e63 6528 782c 2069 6e74 2920  nstance(x, int) 
+00019d20: 666f 7220 7820 696e 2073 656c 6563 7469  for x in selecti
+00019d30: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
+00019d40: 2070 6173 730a 2020 2020 2020 2020 656c   pass.        el
+00019d50: 6966 2061 6c6c 2869 7369 6e73 7461 6e63  if all(isinstanc
+00019d60: 6528 782c 2073 7472 2920 666f 7220 7820  e(x, str) for x 
+00019d70: 696e 2073 656c 6563 7469 6f6e 293a 0a20  in selection):. 
+00019d80: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+00019d90: 7469 6f6e 203d 205b 5f67 6574 5f6f 7065  tion = [_get_ope
+00019da0: 6e69 6e67 5f6c 6162 656c 2873 656c 6529  ning_label(sele)
+00019db0: 2066 6f72 2073 656c 6520 696e 2073 656c   for sele in sel
+00019dc0: 6563 7469 6f6e 5d0a 2020 2020 2020 2020  ection].        
+00019dd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00019de0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+00019df0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00019e00: 2020 2022 6073 656c 6563 7469 6f6e 6020     "`selection` 
+00019e10: 6d75 7374 2062 6520 6120 6c69 7374 206f  must be a list o
+00019e20: 6620 7374 7269 6e67 7320 2863 6176 6974  f strings (cavit
+00019e30: 7920 6e61 6d65 7329 206f 7220 696e 7465  y names) or inte
+00019e40: 6765 7273 2028 6361 7669 7479 206c 6162  gers (cavity lab
+00019e50: 656c 7329 2e22 0a20 2020 2020 2020 2020  els).".         
+00019e60: 2020 2029 0a20 2020 2020 2020 2023 2043     ).        # C
+00019e70: 6865 636b 2069 6620 7365 6c65 6374 696f  heck if selectio
+00019e80: 6e20 696e 636c 7564 6573 2076 616c 6964  n includes valid
+00019e90: 2063 6176 6974 7920 6c61 6265 6c73 0a20   cavity labels. 
+00019ea0: 2020 2020 2020 2069 6620 616e 7928 7820         if any(x 
+00019eb0: 3c20 3220 666f 7220 7820 696e 2073 656c  < 2 for x in sel
+00019ec0: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
+00019ed0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00019ee0: 4572 726f 7228 6622 496e 7661 6c69 6420  Error(f"Invalid 
+00019ef0: 6073 656c 6563 7469 6f6e 603a 207b 7365  `selection`: {se
+00019f00: 6c65 6374 696f 6e7d 2e22 290a 2020 2020  lection}.").    
+00019f10: 6966 206e 7468 7265 6164 7320 6973 204e  if nthreads is N
+00019f20: 6f6e 653a 0a20 2020 2020 2020 206e 7468  one:.        nth
+00019f30: 7265 6164 7320 3d20 6f73 2e63 7075 5f63  reads = os.cpu_c
+00019f40: 6f75 6e74 2829 202d 2031 0a20 2020 2065  ount() - 1.    e
+00019f50: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
+00019f60: 7479 7065 286e 7468 7265 6164 7329 206e  type(nthreads) n
+00019f70: 6f74 2069 6e20 5b69 6e74 5d3a 0a20 2020  ot in [int]:.   
+00019f80: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00019f90: 7970 6545 7272 6f72 2822 606e 7468 7265  ypeError("`nthre
+00019fa0: 6164 7360 206d 7573 7420 6265 2061 2070  ads` must be a p
+00019fb0: 6f73 6974 6976 6520 696e 7465 6765 722e  ositive integer.
+00019fc0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
+00019fd0: 6e74 6872 6561 6473 203c 3d20 303a 0a20  nthreads <= 0:. 
+00019fe0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00019ff0: 2056 616c 7565 4572 726f 7228 2260 6e74   ValueError("`nt
+0001a000: 6872 6561 6473 6020 6d75 7374 2062 6520  hreads` must be 
+0001a010: 6120 706f 7369 7469 7665 2069 6e74 6567  a positive integ
+0001a020: 6572 2e22 290a 2020 2020 6966 2074 7970  er.").    if typ
+0001a030: 6528 6170 7065 6e64 2920 6e6f 7420 696e  e(append) not in
+0001a040: 205b 626f 6f6c 5d3a 0a20 2020 2020 2020   [bool]:.       
+0001a050: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+0001a060: 2822 6061 7070 656e 6460 206d 7573 7420  ("`append` must 
+0001a070: 6265 2061 2062 6f6f 6c65 616e 2e22 290a  be a boolean.").
+0001a080: 2020 2020 6966 2074 7970 6528 6d6f 6465      if type(mode
+0001a090: 6c29 206e 6f74 2069 6e20 5b69 6e74 5d3a  l) not in [int]:
+0001a0a0: 0a20 2020 2020 2020 2072 6169 7365 2054  .        raise T
+0001a0b0: 7970 6545 7272 6f72 2822 606d 6f64 656c  ypeError("`model
+0001a0c0: 6020 6d75 7374 2062 6520 6120 696e 7465  ` must be a inte
+0001a0d0: 6765 722e 2229 0a0a 2020 2020 2320 436f  ger.")..    # Co
+0001a0e0: 6e76 6572 7420 7479 7065 730a 2020 2020  nvert types.    
+0001a0f0: 6966 2074 7970 6528 7665 7274 6963 6573  if type(vertices
+0001a100: 2920 3d3d 206c 6973 743a 0a20 2020 2020  ) == list:.     
+0001a110: 2020 2076 6572 7469 6365 7320 3d20 6e75     vertices = nu
+0001a120: 6d70 792e 6173 6172 7261 7928 7665 7274  mpy.asarray(vert
+0001a130: 6963 6573 290a 2020 2020 6966 2074 7970  ices).    if typ
+0001a140: 6528 7374 6570 2920 3d3d 2069 6e74 3a0a  e(step) == int:.
+0001a150: 2020 2020 2020 2020 7374 6570 203d 2066          step = f
+0001a160: 6c6f 6174 2873 7465 7029 0a0a 2020 2020  loat(step)..    
+0001a170: 2320 436f 6e76 6572 7420 6e75 6d70 792e  # Convert numpy.
+0001a180: 6e64 6172 7261 7920 6461 7461 2074 7970  ndarray data typ
+0001a190: 6573 0a20 2020 2076 6572 7469 6365 7320  es.    vertices 
+0001a1a0: 3d20 7665 7274 6963 6573 2e61 7374 7970  = vertices.astyp
+0001a1b0: 6528 2266 6c6f 6174 3634 2229 2069 6620  e("float64") if 
+0001a1c0: 7665 7274 6963 6573 2e64 7479 7065 2021  vertices.dtype !
+0001a1d0: 3d20 2266 6c6f 6174 3634 2220 656c 7365  = "float64" else
+0001a1e0: 2076 6572 7469 6365 730a 0a20 2020 2023   vertices..    #
+0001a1f0: 2047 6574 2073 696e 636f 733a 2073 696e   Get sincos: sin
+0001a200: 6520 616e 6420 636f 7373 696e 6520 6f66  e and cossine of
+0001a210: 2074 6865 2067 7269 6420 726f 7461 7469   the grid rotati
+0001a220: 6f6e 2061 6e67 6c65 7320 2873 696e 612c  on angles (sina,
+0001a230: 2063 6f73 612c 2073 696e 622c 2063 6f73   cosa, sinb, cos
+0001a240: 6229 0a20 2020 2073 696e 636f 7320 3d20  b).    sincos = 
+0001a250: 5f67 6574 5f73 696e 636f 7328 7665 7274  _get_sincos(vert
+0001a260: 6963 6573 290a 0a20 2020 2023 2043 7265  ices)..    # Cre
+0001a270: 6174 6520 6261 7365 2064 6972 6563 746f  ate base directo
+0001a280: 7269 6573 206f 6620 7265 7375 6c74 730a  ries of results.
+0001a290: 2020 2020 6966 2066 6e20 6973 206e 6f74      if fn is not
+0001a2a0: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+0001a2b0: 6620 7479 7065 2866 6e29 206e 6f74 2069  f type(fn) not i
+0001a2c0: 6e20 5b73 7472 2c20 7061 7468 6c69 622e  n [str, pathlib.
+0001a2d0: 5061 7468 5d3a 0a20 2020 2020 2020 2020  Path]:.         
+0001a2e0: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+0001a2f0: 6f72 2822 6066 6e60 206d 7573 7420 6265  or("`fn` must be
+0001a300: 2061 2073 7472 696e 6720 6f72 2061 2070   a string or a p
+0001a310: 6174 686c 6962 2e50 6174 682e 2229 0a20  athlib.Path."). 
+0001a320: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
+0001a330: 7273 286f 732e 7061 7468 2e61 6273 7061  rs(os.path.abspa
+0001a340: 7468 286f 732e 7061 7468 2e64 6972 6e61  th(os.path.dirna
+0001a350: 6d65 2866 6e29 292c 2065 7869 7374 5f6f  me(fn)), exist_o
+0001a360: 6b3d 5472 7565 290a 0a20 2020 2023 2055  k=True)..    # U
+0001a370: 6e70 6163 6b20 7665 7274 6963 6573 0a20  npack vertices. 
+0001a380: 2020 2050 312c 205f 2c20 5f2c 205f 203d     P1, _, _, _ =
+0001a390: 2076 6572 7469 6365 730a 0a20 2020 2023   vertices..    #
+0001a3a0: 2053 656c 6563 7420 6361 7669 7469 6573   Select cavities
+0001a3b0: 0a20 2020 2069 6620 7365 6c65 6374 696f  .    if selectio
+0001a3c0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+0001a3d0: 2020 2020 2020 206f 7065 6e69 6e67 7320         openings 
+0001a3e0: 3d20 5f73 656c 6563 745f 6361 7669 7469  = _select_caviti
+0001a3f0: 6573 286f 7065 6e69 6e67 732c 2073 656c  es(openings, sel
+0001a400: 6563 7469 6f6e 290a 0a20 2020 2023 2047  ection)..    # G
+0001a410: 6574 206e 756d 6265 7220 6f66 206f 7065  et number of ope
+0001a420: 6e69 6e67 730a 2020 2020 6e6f 7065 6e69  nings.    nopeni
+0001a430: 6e67 7320 3d20 696e 7428 6f70 656e 696e  ngs = int(openin
+0001a440: 6773 2e6d 6178 2829 202d 2031 290a 0a20  gs.max() - 1).. 
+0001a450: 2020 2023 2045 7870 6f72 7420 6f70 656e     # Export open
+0001a460: 696e 6773 0a20 2020 205f 6578 706f 7274  ings.    _export
+0001a470: 5f6f 7065 6e69 6e67 7328 666e 2c20 6f70  _openings(fn, op
+0001a480: 656e 696e 6773 2c20 5031 2c20 7369 6e63  enings, P1, sinc
+0001a490: 6f73 2c20 7374 6570 2c20 6e6f 7065 6e69  os, step, nopeni
+0001a4a0: 6e67 732c 206e 7468 7265 6164 732c 2061  ngs, nthreads, a
+0001a4b0: 7070 656e 642c 206d 6f64 656c 290a       ppend, model).
```

### Comparing `pyKVFinder-0.5.5/pyKVFinder/main.py` & `pyKVFinder-0.6.0/pyKVFinder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,4099 +411,4031 @@
 000019a0: 655f 6261 636b 626f 6e65 2c0a 2020 2020  e_backbone,.    
 000019b0: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
 000019c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 000019d0: 2020 6172 6773 2e6e 7468 7265 6164 732c    args.nthreads,
 000019e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000019f0: 2061 7267 732e 7665 7262 6f73 652c 0a20   args.verbose,. 
 00001a00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00001a10: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-00001a20: 6879 6472 6f70 6174 6879 203d 206f 732e  hydropathy = os.
-00001a30: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00001a40: 2020 2020 2020 2020 2020 2061 7267 732e             args.
-00001a50: 6f75 7470 7574 5f64 6972 6563 746f 7279  output_directory
-00001a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001a70: 2020 6622 7b61 7267 732e 6261 7365 5f6e    f"{args.base_n
-00001a80: 616d 657d 2e7b 6c69 7374 2861 7667 5f68  ame}.{list(avg_h
-00001a90: 7964 726f 7061 7468 792e 6b65 7973 2829  ydropathy.keys()
-00001aa0: 295b 2d31 5d7d 2e70 6462 222c 0a20 2020  )[-1]}.pdb",.   
-00001ab0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00001ac0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00001ad0: 2020 2020 2073 6361 6c65 732c 2061 7667       scales, avg
-00001ae0: 5f68 7964 726f 7061 7468 792c 206f 7574  _hydropathy, out
-00001af0: 7075 745f 6879 6472 6f70 6174 6879 203d  put_hydropathy =
-00001b00: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
-00001b10: 650a 0a20 2020 2020 2020 2023 2045 7870  e..        # Exp
-00001b20: 6f72 7420 6361 7669 7469 6573 0a20 2020  ort cavities.   
-00001b30: 2020 2020 206f 7574 7075 745f 6361 7669       output_cavi
-00001b40: 7479 203d 206f 732e 7061 7468 2e6a 6f69  ty = os.path.joi
-00001b50: 6e28 0a20 2020 2020 2020 2020 2020 2061  n(.            a
-00001b60: 7267 732e 6f75 7470 7574 5f64 6972 6563  rgs.output_direc
-00001b70: 746f 7279 2c20 6622 7b61 7267 732e 6261  tory, f"{args.ba
-00001b80: 7365 5f6e 616d 657d 2e4b 5646 696e 6465  se_name}.KVFinde
-00001b90: 722e 6f75 7470 7574 2e70 6462 220a 2020  r.output.pdb".  
-00001ba0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00001bb0: 6578 706f 7274 280a 2020 2020 2020 2020  export(.        
-00001bc0: 2020 2020 6f75 7470 7574 5f63 6176 6974      output_cavit
-00001bd0: 792c 0a20 2020 2020 2020 2020 2020 2063  y,.            c
-00001be0: 6176 6974 6965 732c 0a20 2020 2020 2020  avities,.       
-00001bf0: 2020 2020 2073 7572 6661 6365 2c0a 2020       surface,.  
-00001c00: 2020 2020 2020 2020 2020 6172 6773 2e76            args.v
-00001c10: 6572 7469 6365 732c 0a20 2020 2020 2020  ertices,.       
-00001c20: 2020 2020 2061 7267 732e 7374 6570 2c0a       args.step,.
-00001c30: 2020 2020 2020 2020 2020 2020 6465 7074              dept
-00001c40: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-00001c50: 6f75 7470 7574 5f68 7964 726f 7061 7468  output_hydropath
-00001c60: 792c 0a20 2020 2020 2020 2020 2020 2073  y,.            s
-00001c70: 6361 6c65 732c 0a20 2020 2020 2020 2020  cales,.         
-00001c80: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
-00001c90: 2020 2020 2061 7267 732e 6e74 6872 6561       args.nthrea
-00001ca0: 6473 2c0a 2020 2020 2020 2020 290a 0a20  ds,.        ).. 
-00001cb0: 2020 2020 2020 2023 2057 7269 7465 2072         # Write r
-00001cc0: 6573 756c 7473 0a20 2020 2020 2020 206f  esults.        o
-00001cd0: 7574 7075 745f 7265 7375 6c74 7320 3d20  utput_results = 
-00001ce0: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-00001cf0: 2020 2020 2020 2020 2020 6172 6773 2e6f            args.o
-00001d00: 7574 7075 745f 6469 7265 6374 6f72 792c  utput_directory,
-00001d10: 2066 227b 6172 6773 2e62 6173 655f 6e61   f"{args.base_na
-00001d20: 6d65 7d2e 4b56 4669 6e64 6572 2e72 6573  me}.KVFinder.res
-00001d30: 756c 7473 2e74 6f6d 6c22 0a20 2020 2020  ults.toml".     
-00001d40: 2020 2029 0a20 2020 2020 2020 2077 7269     ).        wri
-00001d50: 7465 5f72 6573 756c 7473 280a 2020 2020  te_results(.    
-00001d60: 2020 2020 2020 2020 6f75 7470 7574 5f72          output_r
-00001d70: 6573 756c 7473 2c0a 2020 2020 2020 2020  esults,.        
-00001d80: 2020 2020 6172 6773 2e69 6e70 7574 2c0a      args.input,.
-00001d90: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00001da0: 2e6c 6967 616e 642c 0a20 2020 2020 2020  .ligand,.       
-00001db0: 2020 2020 206f 7574 7075 745f 6361 7669       output_cavi
-00001dc0: 7479 2c0a 2020 2020 2020 2020 2020 2020  ty,.            
-00001dd0: 6f75 7470 7574 5f68 7964 726f 7061 7468  output_hydropath
-00001de0: 792c 0a20 2020 2020 2020 2020 2020 2076  y,.            v
-00001df0: 6f6c 756d 652c 0a20 2020 2020 2020 2020  olume,.         
-00001e00: 2020 2061 7265 612c 0a20 2020 2020 2020     area,.       
-00001e10: 2020 2020 206d 6178 5f64 6570 7468 2c0a       max_depth,.
-00001e20: 2020 2020 2020 2020 2020 2020 6176 675f              avg_
-00001e30: 6465 7074 682c 0a20 2020 2020 2020 2020  depth,.         
-00001e40: 2020 2061 7667 5f68 7964 726f 7061 7468     avg_hydropath
-00001e50: 792c 0a20 2020 2020 2020 2020 2020 2072  y,.            r
-00001e60: 6573 6964 7565 732c 0a20 2020 2020 2020  esidues,.       
-00001e70: 2020 2020 2066 7265 7175 656e 6369 6573       frequencies
-00001e80: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-00001e90: 6773 2e73 7465 702c 0a20 2020 2020 2020  gs.step,.       
-00001ea0: 2029 0a0a 2020 2020 2020 2020 2320 5772   )..        # Wr
-00001eb0: 6974 6520 7061 7261 6d65 7465 7273 0a20  ite parameters. 
-00001ec0: 2020 2020 2020 205f 7772 6974 655f 7061         _write_pa
-00001ed0: 7261 6d65 7465 7273 2861 7267 7329 0a20  rameters(args). 
-00001ee0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00001ef0: 2070 7269 6e74 2822 3e20 4e6f 2063 6176   print("> No cav
-00001f00: 6974 6965 7320 6465 7465 6374 6564 2122  ities detected!"
-00001f10: 290a 0a20 2020 2023 2045 6c61 7073 6564  )..    # Elapsed
-00001f20: 2074 696d 650a 2020 2020 656c 6170 7365   time.    elapse
-00001f30: 645f 7469 6d65 203d 2074 696d 652e 7469  d_time = time.ti
-00001f40: 6d65 2829 202d 2073 7461 7274 5f74 696d  me() - start_tim
-00001f50: 650a 2020 2020 7072 696e 7428 6622 5b20  e.    print(f"[ 
-00001f60: 5c30 3333 5b31 6d45 6c61 7073 6564 2074  \033[1mElapsed t
-00001f70: 696d 653a 5c30 3333 5b30 6d20 7b65 6c61  ime:\033[0m {ela
-00001f80: 7073 6564 5f74 696d 653a 2e34 667d 7320  psed_time:.4f}s 
-00001f90: 5d22 290a 2020 2020 6c6f 6767 696e 672e  ]").    logging.
-00001fa0: 696e 666f 2866 225b 2045 6c61 7073 6564  info(f"[ Elapsed
-00001fb0: 2074 696d 6520 2873 293a 207b 656c 6170   time (s): {elap
-00001fc0: 7365 645f 7469 6d65 3a2e 3466 7d73 205d  sed_time:.4f}s ]
-00001fd0: 5c6e 2229 0a0a 2020 2020 7265 7475 726e  \n")..    return
-00001fe0: 2030 0a0a 0a63 6c61 7373 2070 794b 5646   0...class pyKVF
-00001ff0: 696e 6465 7252 6573 756c 7473 286f 626a  inderResults(obj
-00002000: 6563 7429 3a0a 2020 2020 2222 2241 2063  ect):.    """A c
-00002010: 6c61 7373 2063 6f6e 7461 696e 696e 6720  lass containing 
-00002020: 7079 4b56 4669 6e64 6572 2064 6574 6563  pyKVFinder detec
-00002030: 7469 6f6e 2061 6e64 2063 6861 7261 6374  tion and charact
-00002040: 6572 697a 6174 696f 6e20 7265 7375 6c74  erization result
-00002050: 732e 0a0a 2020 2020 5061 7261 6d65 7465  s...    Paramete
-00002060: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00002070: 2d0a 2020 2020 6361 7669 7469 6573 203a  -.    cavities :
-00002080: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
-00002090: 2020 2020 2020 2043 6176 6974 7920 706f         Cavity po
-000020a0: 696e 7473 2069 6e20 7468 6520 3344 2067  ints in the 3D g
-000020b0: 7269 6420 2863 6176 6974 6965 735b 6e78  rid (cavities[nx
-000020c0: 5d5b 6e79 5d5b 6e7a 5d29 2e0a 2020 2020  ][ny][nz])..    
-000020d0: 2020 2020 4361 7669 7469 6573 2061 7272      Cavities arr
-000020e0: 6179 2068 6173 2069 6e74 6567 6572 206c  ay has integer l
-000020f0: 6162 656c 7320 696e 2065 6163 6820 706f  abels in each po
-00002100: 7369 7469 6f6e 2c20 7468 6174 2061 7265  sition, that are
-00002110: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
-00002120: 202d 313a 2062 756c 6b20 706f 696e 7473   -1: bulk points
-00002130: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
-00002140: 2030 3a20 6269 6f6d 6f6c 6563 756c 6520   0: biomolecule 
-00002150: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
-00002160: 2020 2020 202a 2031 3a20 656d 7074 7920       * 1: empty 
-00002170: 7370 6163 6520 706f 696e 7473 3b0a 0a20  space points;.. 
-00002180: 2020 2020 2020 2020 2020 202a 203e 3d32             * >=2
-00002190: 3a20 6361 7669 7479 2070 6f69 6e74 732e  : cavity points.
-000021a0: 0a0a 2020 2020 2020 2020 5468 6520 656d  ..        The em
-000021b0: 7074 7920 7370 6163 6520 706f 696e 7473  pty space points
-000021c0: 2061 7265 2072 6567 696f 6e73 2074 6861   are regions tha
-000021d0: 7420 646f 206e 6f74 206d 6565 7420 7468  t do not meet th
-000021e0: 6520 6368 6f73 656e 0a20 2020 2020 2020  e chosen.       
-000021f0: 2076 6f6c 756d 6520 6375 746f 6666 2074   volume cutoff t
-00002200: 6f20 6265 2063 6f6e 7369 6465 7265 6420  o be considered 
-00002210: 6120 6361 7669 7479 2e0a 2020 2020 7375  a cavity..    su
-00002220: 7266 6163 6520 3a20 6e75 6d70 792e 6e64  rface : numpy.nd
-00002230: 6172 7261 790a 2020 2020 2020 2020 5375  array.        Su
-00002240: 7266 6163 6520 706f 696e 7473 2069 6e20  rface points in 
-00002250: 7468 6520 3344 2067 7269 6420 2873 7572  the 3D grid (sur
-00002260: 6661 6365 5b6e 785d 5b6e 795d 5b6e 7a5d  face[nx][ny][nz]
-00002270: 292e 0a20 2020 2020 2020 2053 7572 6661  )..        Surfa
-00002280: 6365 2061 7272 6179 2068 6173 2069 6e74  ce array has int
-00002290: 6567 6572 206c 6162 656c 7320 696e 2065  eger labels in e
-000022a0: 6163 6820 706f 7369 7469 6f6e 2c20 7468  ach position, th
-000022b0: 6174 2061 7265 3a0a 0a20 2020 2020 2020  at are:..       
-000022c0: 2020 2020 202a 202d 313a 2062 756c 6b20       * -1: bulk 
-000022d0: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
-000022e0: 2020 2020 202a 2030 3a20 6269 6f6d 6f6c       * 0: biomol
-000022f0: 6563 756c 6520 6f72 2065 6d70 7479 2073  ecule or empty s
-00002300: 7061 6365 2070 6f69 6e74 733b 0a0a 2020  pace points;..  
-00002310: 2020 2020 2020 2020 2020 2a20 3e3d 323a            * >=2:
-00002320: 2073 7572 6661 6365 2070 6f69 6e74 732e   surface points.
-00002330: 0a0a 2020 2020 2020 2020 5468 6520 656d  ..        The em
-00002340: 7074 7920 7370 6163 6520 706f 696e 7473  pty space points
-00002350: 2061 7265 2072 6567 696f 6e73 2074 6861   are regions tha
-00002360: 7420 646f 206e 6f74 206d 6565 7420 7468  t do not meet th
-00002370: 6520 6368 6f73 656e 0a20 2020 2020 2020  e chosen.       
-00002380: 2076 6f6c 756d 6520 6375 746f 6666 2074   volume cutoff t
-00002390: 6f20 6265 2063 6f6e 7369 6465 7265 6420  o be considered 
-000023a0: 6120 6361 7669 7479 2e0a 2020 2020 6465  a cavity..    de
-000023b0: 7074 6873 203a 206e 756d 7079 2e6e 6461  pths : numpy.nda
-000023c0: 7272 6179 2c20 6f70 7469 6f6e 616c 0a20  rray, optional. 
-000023d0: 2020 2020 2020 2041 206e 756d 7079 2e6e         A numpy.n
-000023e0: 6461 7272 6179 2077 6974 6820 6465 7074  darray with dept
-000023f0: 6820 6f66 2063 6176 6974 7920 706f 696e  h of cavity poin
-00002400: 7473 2028 6465 7074 685b 6e78 5d5b 6e79  ts (depth[nx][ny
-00002410: 5d5b 6e7a 5d29 2e0a 2020 2020 7363 616c  ][nz])..    scal
-00002420: 6573 203a 206e 756d 7079 2e6e 6461 7272  es : numpy.ndarr
-00002430: 6179 2c20 6f70 7469 6f6e 616c 0a20 2020  ay, optional.   
-00002440: 2020 2020 2041 206e 756d 7079 2e6e 6461       A numpy.nda
-00002450: 7272 6179 2077 6974 6820 6879 6472 6f70  rray with hydrop
-00002460: 686f 6269 6369 7479 2073 6361 6c65 2076  hobicity scale v
-00002470: 616c 7565 206d 6170 7065 6420 6174 2073  alue mapped at s
-00002480: 7572 6661 6365 0a20 2020 2020 2020 2070  urface.        p
-00002490: 6f69 6e74 7320 2873 6361 6c65 735b 6e78  oints (scales[nx
-000024a0: 5d5b 6e79 5d5b 6e7a 5d29 2e0a 2020 2020  ][ny][nz])..    
-000024b0: 766f 6c75 6d65 203a 2044 6963 745b 7374  volume : Dict[st
-000024c0: 722c 2066 6c6f 6174 5d0a 2020 2020 2020  r, float].      
-000024d0: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
-000024e0: 6974 6820 766f 6c75 6d65 206f 6620 6561  ith volume of ea
-000024f0: 6368 2064 6574 6563 7465 6420 6361 7669  ch detected cavi
-00002500: 7479 2e0a 2020 2020 6172 6561 203a 2044  ty..    area : D
-00002510: 6963 745b 7374 722c 2066 6c6f 6174 5d0a  ict[str, float].
-00002520: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-00002530: 6e61 7279 2077 6974 6820 6172 6561 206f  nary with area o
-00002540: 6620 6561 6368 2064 6574 6563 7465 6420  f each detected 
-00002550: 6361 7669 7479 2e0a 2020 2020 6d61 785f  cavity..    max_
-00002560: 6465 7074 6820 3a20 4469 6374 5b73 7472  depth : Dict[str
-00002570: 2c20 666c 6f61 745d 2c20 6f70 7469 6f6e  , float], option
-00002580: 616c 0a20 2020 2020 2020 2041 2064 6963  al.        A dic
-00002590: 7469 6f6e 6172 7920 7769 7468 206d 6178  tionary with max
-000025a0: 696d 756d 2064 6570 7468 206f 6620 6561  imum depth of ea
-000025b0: 6368 2064 6574 6563 7465 6420 6361 7669  ch detected cavi
-000025c0: 7479 2e0a 2020 2020 6176 675f 6465 7074  ty..    avg_dept
-000025d0: 6820 3a20 4469 6374 5b73 7472 2c20 666c  h : Dict[str, fl
-000025e0: 6f61 745d 2c20 6f70 7469 6f6e 616c 0a20  oat], optional. 
-000025f0: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
-00002600: 6172 7920 7769 7468 2061 7665 7261 6765  ary with average
-00002610: 2064 6570 7468 206f 6620 6561 6368 2064   depth of each d
-00002620: 6574 6563 7465 6420 6361 7669 7479 2e0a  etected cavity..
-00002630: 2020 2020 6176 675f 6879 6472 6f70 6174      avg_hydropat
-00002640: 6879 203a 2044 6963 745b 7374 722c 2066  hy : Dict[str, f
-00002650: 6c6f 6174 5d2c 206f 7074 696f 6e61 6c0a  loat], optional.
-00002660: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-00002670: 6e61 7279 2077 6974 6820 6176 6572 6167  nary with averag
-00002680: 6520 6879 6472 6f70 6174 6879 2066 6f72  e hydropathy for
-00002690: 2065 6163 6820 6465 7465 6374 6564 2063   each detected c
-000026a0: 6176 6974 7920 616e 640a 2020 2020 2020  avity and.      
-000026b0: 2020 7468 6520 7261 6e67 6520 6f66 2074    the range of t
-000026c0: 6865 2068 7964 726f 7068 6f62 6963 6974  he hydrophobicit
-000026d0: 7920 7363 616c 6520 286d 696e 2c20 6d61  y scale (min, ma
-000026e0: 7829 2e0a 2020 2020 7265 7369 6475 6573  x)..    residues
-000026f0: 3a20 4469 6374 5b73 7472 2c20 4c69 7374  : Dict[str, List
-00002700: 5b4c 6973 745b 7374 725d 5d5d 0a20 2020  [List[str]]].   
-00002710: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
-00002720: 7920 7769 7468 2061 206c 6973 7420 6f66  y with a list of
-00002730: 2069 6e74 6572 6661 6365 2072 6573 6964   interface resid
-00002740: 7565 7320 666f 7220 6561 6368 2064 6574  ues for each det
-00002750: 6563 7465 640a 2020 2020 2020 2020 6361  ected.        ca
-00002760: 7669 7479 2e0a 2020 2020 6672 6571 7565  vity..    freque
-00002770: 6e63 6965 7320 3a20 4469 6374 5b73 7472  ncies : Dict[str
-00002780: 2c20 4469 6374 5b73 7472 2c20 4469 6374  , Dict[str, Dict
-00002790: 5b73 7472 2c20 696e 745d 5d5d 2c20 6f70  [str, int]]], op
-000027a0: 7469 6f6e 616c 0a20 2020 2020 2020 2041  tional.        A
-000027b0: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
-000027c0: 2066 7265 7175 656e 6369 6573 206f 6620   frequencies of 
-000027d0: 7265 7369 6475 6573 2061 6e64 2063 6c61  residues and cla
-000027e0: 7373 2066 6f72 0a20 2020 2020 2020 2072  ss for.        r
-000027f0: 6573 6964 7565 7320 6f66 2065 6163 6820  esidues of each 
-00002800: 6465 7465 6374 6564 2063 6176 6974 792e  detected cavity.
-00002810: 0a20 2020 205f 7665 7274 6963 6573 203a  .    _vertices :
-00002820: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
-00002830: 2020 2020 2020 2041 206e 756d 7079 2e6e         A numpy.n
-00002840: 6461 7272 6179 206f 7220 6120 6c69 7374  darray or a list
-00002850: 2077 6974 6820 7879 7a20 7665 7274 6963   with xyz vertic
-00002860: 6573 2063 6f6f 7264 696e 6174 6573 2028  es coordinates (
-00002870: 6f72 6967 696e 2c0a 2020 2020 2020 2020  origin,.        
-00002880: 582d 6178 6973 2c20 592d 6178 6973 2c20  X-axis, Y-axis, 
-00002890: 5a2d 6178 6973 292e 0a20 2020 205f 7374  Z-axis)..    _st
-000028a0: 6570 203a 2066 6c6f 6174 0a20 2020 2020  ep : float.     
-000028b0: 2020 2047 7269 6420 7370 6163 696e 6720     Grid spacing 
-000028c0: 2841 292e 0a20 2020 205f 696e 7075 7420  (A)..    _input 
-000028d0: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
-000028e0: 686c 6962 2e50 6174 685d 2c20 6f70 7469  hlib.Path], opti
-000028f0: 6f6e 616c 0a20 2020 2020 2020 2041 2070  onal.        A p
-00002900: 6174 6820 746f 2069 6e70 7574 2050 4442  ath to input PDB
-00002910: 206f 7220 5859 5a20 6669 6c65 2c20 6279   or XYZ file, by
-00002920: 2064 6566 6175 6c74 204e 6f6e 652e 0a20   default None.. 
-00002930: 2020 205f 6c69 6761 6e64 203a 2055 6e69     _ligand : Uni
-00002940: 6f6e 5b73 7472 2c20 7061 7468 6c69 622e  on[str, pathlib.
-00002950: 5061 7468 5d2c 206f 7074 696f 6e61 6c0a  Path], optional.
-00002960: 2020 2020 2020 2020 4120 7061 7468 2074          A path t
-00002970: 6f20 6c69 6761 6e64 2050 4442 206f 7220  o ligand PDB or 
-00002980: 5859 5a20 6669 6c65 2c20 6279 2064 6566  XYZ file, by def
-00002990: 6175 6c74 204e 6f6e 652e 0a0a 2020 2020  ault None...    
-000029a0: 4174 7472 6962 7574 6573 0a20 2020 202d  Attributes.    -
-000029b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6361  ---------.    ca
-000029c0: 7669 7469 6573 203a 206e 756d 7079 2e6e  vities : numpy.n
-000029d0: 6461 7272 6179 0a20 2020 2020 2020 2043  darray.        C
-000029e0: 6176 6974 7920 706f 696e 7473 2069 6e20  avity points in 
-000029f0: 7468 6520 3344 2067 7269 6420 2863 6176  the 3D grid (cav
-00002a00: 6974 6965 735b 6e78 5d5b 6e79 5d5b 6e7a  ities[nx][ny][nz
-00002a10: 5d29 2e0a 2020 2020 2020 2020 4361 7669  ])..        Cavi
-00002a20: 7469 6573 2061 7272 6179 2068 6173 2069  ties array has i
-00002a30: 6e74 6567 6572 206c 6162 656c 7320 696e  nteger labels in
-00002a40: 2065 6163 6820 706f 7369 7469 6f6e 2c20   each position, 
-00002a50: 7468 6174 2061 7265 3a0a 0a20 2020 2020  that are:..     
-00002a60: 2020 2020 2020 202a 202d 313a 2062 756c         * -1: bul
-00002a70: 6b20 706f 696e 7473 3b0a 0a20 2020 2020  k points;..     
-00002a80: 2020 2020 2020 202a 2030 3a20 6269 6f6d         * 0: biom
-00002a90: 6f6c 6563 756c 6520 706f 696e 7473 3b0a  olecule points;.
-00002aa0: 0a20 2020 2020 2020 2020 2020 202a 2031  .            * 1
-00002ab0: 3a20 656d 7074 7920 7370 6163 6520 706f  : empty space po
-00002ac0: 696e 7473 3b0a 0a20 2020 2020 2020 2020  ints;..         
-00002ad0: 2020 202a 203e 3d32 3a20 6361 7669 7479     * >=2: cavity
-00002ae0: 2070 6f69 6e74 732e 0a0a 2020 2020 2020   points...      
-00002af0: 2020 5468 6520 656d 7074 7920 7370 6163    The empty spac
-00002b00: 6520 706f 696e 7473 2061 7265 2072 6567  e points are reg
-00002b10: 696f 6e73 2074 6861 7420 646f 206e 6f74  ions that do not
-00002b20: 206d 6565 7420 7468 6520 6368 6f73 656e   meet the chosen
-00002b30: 0a20 2020 2020 2020 2076 6f6c 756d 6520  .        volume 
-00002b40: 6375 746f 6666 2074 6f20 6265 2063 6f6e  cutoff to be con
-00002b50: 7369 6465 7265 6420 6120 6361 7669 7479  sidered a cavity
-00002b60: 2e0a 2020 2020 7375 7266 6163 6520 3a20  ..    surface : 
-00002b70: 6e75 6d70 792e 6e64 6172 7261 790a 2020  numpy.ndarray.  
-00002b80: 2020 2020 2020 5375 7266 6163 6520 706f        Surface po
-00002b90: 696e 7473 2069 6e20 7468 6520 3344 2067  ints in the 3D g
-00002ba0: 7269 6420 2873 7572 6661 6365 5b6e 785d  rid (surface[nx]
-00002bb0: 5b6e 795d 5b6e 7a5d 292e 0a20 2020 2020  [ny][nz])..     
-00002bc0: 2020 2053 7572 6661 6365 2061 7272 6179     Surface array
-00002bd0: 2068 6173 2069 6e74 6567 6572 206c 6162   has integer lab
-00002be0: 656c 7320 696e 2065 6163 6820 706f 7369  els in each posi
-00002bf0: 7469 6f6e 2c20 7468 6174 2061 7265 3a0a  tion, that are:.
-00002c00: 0a20 2020 2020 2020 2020 2020 202a 202d  .            * -
-00002c10: 313a 2062 756c 6b20 706f 696e 7473 3b0a  1: bulk points;.
-00002c20: 0a20 2020 2020 2020 2020 2020 202a 2030  .            * 0
-00002c30: 3a20 6269 6f6d 6f6c 6563 756c 6520 6f72  : biomolecule or
-00002c40: 2065 6d70 7479 2073 7061 6365 2070 6f69   empty space poi
-00002c50: 6e74 733b 0a0a 2020 2020 2020 2020 2020  nts;..          
-00002c60: 2020 2a20 3e3d 323a 2073 7572 6661 6365    * >=2: surface
-00002c70: 2070 6f69 6e74 732e 0a0a 2020 2020 2020   points...      
-00002c80: 2020 5468 6520 656d 7074 7920 7370 6163    The empty spac
-00002c90: 6520 706f 696e 7473 2061 7265 2072 6567  e points are reg
-00002ca0: 696f 6e73 2074 6861 7420 646f 206e 6f74  ions that do not
-00002cb0: 206d 6565 7420 7468 6520 6368 6f73 656e   meet the chosen
-00002cc0: 0a20 2020 2020 2020 2076 6f6c 756d 6520  .        volume 
-00002cd0: 6375 746f 6666 2074 6f20 6265 2063 6f6e  cutoff to be con
-00002ce0: 7369 6465 7265 6420 6120 6361 7669 7479  sidered a cavity
-00002cf0: 2e0a 2020 2020 6465 7074 6873 203a 206e  ..    depths : n
-00002d00: 756d 7079 2e6e 6461 7272 6179 2c20 6f70  umpy.ndarray, op
-00002d10: 7469 6f6e 616c 0a20 2020 2020 2020 2041  tional.        A
-00002d20: 206e 756d 7079 2e6e 6461 7272 6179 2077   numpy.ndarray w
-00002d30: 6974 6820 6465 7074 6820 6f66 2063 6176  ith depth of cav
-00002d40: 6974 7920 706f 696e 7473 2028 6465 7074  ity points (dept
-00002d50: 685b 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a  h[nx][ny][nz])..
-00002d60: 2020 2020 7363 616c 6573 203a 206e 756d      scales : num
-00002d70: 7079 2e6e 6461 7272 6179 2c20 6f70 7469  py.ndarray, opti
-00002d80: 6f6e 616c 0a20 2020 2020 2020 2041 206e  onal.        A n
-00002d90: 756d 7079 2e6e 6461 7272 6179 2077 6974  umpy.ndarray wit
-00002da0: 6820 6879 6472 6f70 686f 6269 6369 7479  h hydrophobicity
-00002db0: 2073 6361 6c65 2076 616c 7565 206d 6170   scale value map
-00002dc0: 7065 6420 6174 2073 7572 6661 6365 0a20  ped at surface. 
-00002dd0: 2020 2020 2020 2070 6f69 6e74 7320 2873         points (s
-00002de0: 6361 6c65 735b 6e78 5d5b 6e79 5d5b 6e7a  cales[nx][ny][nz
-00002df0: 5d29 2e0a 2020 2020 6e63 6176 203a 2069  ])..    ncav : i
-00002e00: 6e74 0a20 2020 2020 2020 204e 756d 6265  nt.        Numbe
-00002e10: 7220 6f66 2063 6176 6974 6965 732e 0a20  r of cavities.. 
-00002e20: 2020 2076 6f6c 756d 6520 3a20 4469 6374     volume : Dict
-00002e30: 5b73 7472 2c20 666c 6f61 745d 0a20 2020  [str, float].   
-00002e40: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
-00002e50: 7920 7769 7468 2076 6f6c 756d 6520 6f66  y with volume of
-00002e60: 2065 6163 6820 6465 7465 6374 6564 2063   each detected c
-00002e70: 6176 6974 792e 0a20 2020 2061 7265 6120  avity..    area 
-00002e80: 3a20 4469 6374 5b73 7472 2c20 666c 6f61  : Dict[str, floa
-00002e90: 745d 0a20 2020 2020 2020 2041 2064 6963  t].        A dic
-00002ea0: 7469 6f6e 6172 7920 7769 7468 2061 7265  tionary with are
-00002eb0: 6120 6f66 2065 6163 6820 6465 7465 6374  a of each detect
-00002ec0: 6564 2063 6176 6974 792e 0a20 2020 206d  ed cavity..    m
-00002ed0: 6178 5f64 6570 7468 203a 2044 6963 745b  ax_depth : Dict[
-00002ee0: 7374 722c 2066 6c6f 6174 5d2c 206f 7074  str, float], opt
-00002ef0: 696f 6e61 6c0a 2020 2020 2020 2020 4120  ional.        A 
-00002f00: 6469 6374 696f 6e61 7279 2077 6974 6820  dictionary with 
-00002f10: 6d61 7869 6d75 6d20 6465 7074 6820 6f66  maximum depth of
-00002f20: 2065 6163 6820 6465 7465 6374 6564 2063   each detected c
-00002f30: 6176 6974 792e 0a20 2020 2061 7667 5f64  avity..    avg_d
-00002f40: 6570 7468 203a 2044 6963 745b 7374 722c  epth : Dict[str,
-00002f50: 2066 6c6f 6174 5d2c 206f 7074 696f 6e61   float], optiona
-00002f60: 6c0a 2020 2020 2020 2020 4120 6469 6374  l.        A dict
-00002f70: 696f 6e61 7279 2077 6974 6820 6176 6572  ionary with aver
-00002f80: 6167 6520 6465 7074 6820 6f66 2065 6163  age depth of eac
-00002f90: 6820 6465 7465 6374 6564 2063 6176 6974  h detected cavit
-00002fa0: 792e 0a20 2020 2061 7667 5f68 7964 726f  y..    avg_hydro
-00002fb0: 7061 7468 7920 3a20 4469 6374 5b73 7472  pathy : Dict[str
-00002fc0: 2c20 666c 6f61 745d 2c20 6f70 7469 6f6e  , float], option
-00002fd0: 616c 0a20 2020 2020 2020 2041 2064 6963  al.        A dic
-00002fe0: 7469 6f6e 6172 7920 7769 7468 2061 7665  tionary with ave
-00002ff0: 7261 6765 2068 7964 726f 7061 7468 7920  rage hydropathy 
-00003000: 666f 7220 6561 6368 2064 6574 6563 7465  for each detecte
-00003010: 6420 6361 7669 7479 2061 6e64 0a20 2020  d cavity and.   
-00003020: 2020 2020 2074 6865 2072 616e 6765 206f       the range o
-00003030: 6620 7468 6520 6879 6472 6f70 686f 6269  f the hydrophobi
-00003040: 6369 7479 2073 6361 6c65 2028 6d69 6e2c  city scale (min,
-00003050: 206d 6178 292e 0a20 2020 2072 6573 6964   max)..    resid
-00003060: 7565 733a 2044 6963 745b 7374 722c 204c  ues: Dict[str, L
-00003070: 6973 745b 4c69 7374 5b73 7472 5d5d 5d0a  ist[List[str]]].
-00003080: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-00003090: 6e61 7279 2077 6974 6820 6120 6c69 7374  nary with a list
-000030a0: 206f 6620 696e 7465 7266 6163 6520 7265   of interface re
-000030b0: 7369 6475 6573 2066 6f72 2065 6163 6820  sidues for each 
-000030c0: 6465 7465 6374 6564 0a20 2020 2020 2020  detected.       
-000030d0: 2063 6176 6974 792e 0a20 2020 2066 7265   cavity..    fre
-000030e0: 7175 656e 6369 6573 203a 2044 6963 745b  quencies : Dict[
-000030f0: 7374 722c 2044 6963 745b 7374 722c 2044  str, Dict[str, D
-00003100: 6963 745b 7374 722c 2069 6e74 5d5d 5d2c  ict[str, int]]],
-00003110: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00003120: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
-00003130: 6974 6820 6672 6571 7565 6e63 6965 7320  ith frequencies 
-00003140: 6f66 2072 6573 6964 7565 7320 616e 6420  of residues and 
-00003150: 636c 6173 7320 666f 720a 2020 2020 2020  class for.      
-00003160: 2020 7265 7369 6475 6573 206f 6620 6561    residues of ea
-00003170: 6368 2064 6574 6563 7465 6420 6361 7669  ch detected cavi
-00003180: 7479 2e0a 2020 2020 5f76 6572 7469 6365  ty..    _vertice
-00003190: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
-000031a0: 790a 2020 2020 2020 2020 4120 6e75 6d70  y.        A nump
-000031b0: 792e 6e64 6172 7261 7920 6f72 2061 206c  y.ndarray or a l
-000031c0: 6973 7420 7769 7468 2078 797a 2076 6572  ist with xyz ver
-000031d0: 7469 6365 7320 636f 6f72 6469 6e61 7465  tices coordinate
-000031e0: 7320 286f 7269 6769 6e2c 0a20 2020 2020  s (origin,.     
-000031f0: 2020 2058 2d61 7869 732c 2059 2d61 7869     X-axis, Y-axi
-00003200: 732c 205a 2d61 7869 7329 2e0a 2020 2020  s, Z-axis)..    
-00003210: 5f73 7465 7020 3a20 666c 6f61 740a 2020  _step : float.  
-00003220: 2020 2020 2020 4772 6964 2073 7061 6369        Grid spaci
-00003230: 6e67 2028 4129 2e0a 2020 2020 5f69 6e70  ng (A)..    _inp
-00003240: 7574 203a 2055 6e69 6f6e 5b73 7472 2c20  ut : Union[str, 
-00003250: 7061 7468 6c69 622e 5061 7468 5d2c 206f  pathlib.Path], o
-00003260: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00003270: 4120 7061 7468 2074 6f20 696e 7075 7420  A path to input 
-00003280: 5044 4220 6f72 2058 595a 2066 696c 652c  PDB or XYZ file,
-00003290: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
-000032a0: 2e0a 2020 2020 5f6c 6967 616e 6420 3a20  ..    _ligand : 
-000032b0: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-000032c0: 6962 2e50 6174 685d 2c20 6f70 7469 6f6e  ib.Path], option
-000032d0: 616c 0a20 2020 2020 2020 2041 2070 6174  al.        A pat
-000032e0: 6820 746f 206c 6967 616e 6420 5044 4220  h to ligand PDB 
-000032f0: 6f72 2058 595a 2066 696c 652c 2062 7920  or XYZ file, by 
-00003300: 6465 6661 756c 7420 4e6f 6e65 2e0a 2020  default None..  
-00003310: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-00003320: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00003330: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-00003340: 6176 6974 6965 733a 206e 756d 7079 2e6e  avities: numpy.n
-00003350: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
-00003360: 7375 7266 6163 653a 206e 756d 7079 2e6e  surface: numpy.n
-00003370: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
-00003380: 6465 7074 6873 3a20 4f70 7469 6f6e 616c  depths: Optional
-00003390: 5b6e 756d 7079 2e6e 6461 7272 6179 5d2c  [numpy.ndarray],
-000033a0: 0a20 2020 2020 2020 2073 6361 6c65 733a  .        scales:
-000033b0: 204f 7074 696f 6e61 6c5b 6e75 6d70 792e   Optional[numpy.
-000033c0: 6e64 6172 7261 795d 2c0a 2020 2020 2020  ndarray],.      
-000033d0: 2020 766f 6c75 6d65 3a20 4469 6374 5b73    volume: Dict[s
-000033e0: 7472 2c20 666c 6f61 745d 2c0a 2020 2020  tr, float],.    
-000033f0: 2020 2020 6172 6561 3a20 4469 6374 5b73      area: Dict[s
-00003400: 7472 2c20 666c 6f61 745d 2c0a 2020 2020  tr, float],.    
-00003410: 2020 2020 6d61 785f 6465 7074 683a 204f      max_depth: O
-00003420: 7074 696f 6e61 6c5b 4469 6374 5b73 7472  ptional[Dict[str
-00003430: 2c20 666c 6f61 745d 5d2c 0a20 2020 2020  , float]],.     
-00003440: 2020 2061 7667 5f64 6570 7468 3a20 4f70     avg_depth: Op
-00003450: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00003460: 2066 6c6f 6174 5d5d 2c0a 2020 2020 2020   float]],.      
-00003470: 2020 6176 675f 6879 6472 6f70 6174 6879    avg_hydropathy
-00003480: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00003490: 7374 722c 2066 6c6f 6174 5d5d 2c0a 2020  str, float]],.  
-000034a0: 2020 2020 2020 7265 7369 6475 6573 3a20        residues: 
-000034b0: 4469 6374 5b73 7472 2c20 4c69 7374 5b4c  Dict[str, List[L
-000034c0: 6973 745b 7374 725d 5d5d 2c0a 2020 2020  ist[str]]],.    
-000034d0: 2020 2020 6672 6571 7565 6e63 6965 733a      frequencies:
-000034e0: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-000034f0: 7472 2c20 4469 6374 5b73 7472 2c20 4469  tr, Dict[str, Di
-00003500: 6374 5b73 7472 2c20 696e 745d 5d5d 5d2c  ct[str, int]]]],
-00003510: 0a20 2020 2020 2020 205f 7665 7274 6963  .        _vertic
-00003520: 6573 3a20 6e75 6d70 792e 6e64 6172 7261  es: numpy.ndarra
-00003530: 792c 0a20 2020 2020 2020 205f 7374 6570  y,.        _step
-00003540: 3a20 556e 696f 6e5b 666c 6f61 742c 2069  : Union[float, i
-00003550: 6e74 5d2c 0a20 2020 2020 2020 205f 696e  nt],.        _in
-00003560: 7075 743a 204f 7074 696f 6e61 6c5b 556e  put: Optional[Un
-00003570: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-00003580: 2e50 6174 685d 5d20 3d20 4e6f 6e65 2c0a  .Path]] = None,.
-00003590: 2020 2020 2020 2020 5f6c 6967 616e 643a          _ligand:
-000035a0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000035b0: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-000035c0: 685d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  h]] = None,.    
-000035d0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000035e0: 6361 7669 7469 6573 203d 2063 6176 6974  cavities = cavit
-000035f0: 6965 730a 2020 2020 2020 2020 7365 6c66  ies.        self
-00003600: 2e73 7572 6661 6365 203d 2073 7572 6661  .surface = surfa
-00003610: 6365 0a20 2020 2020 2020 2073 656c 662e  ce.        self.
-00003620: 6465 7074 6873 203d 2064 6570 7468 730a  depths = depths.
-00003630: 2020 2020 2020 2020 7365 6c66 2e73 6361          self.sca
-00003640: 6c65 7320 3d20 7363 616c 6573 0a20 2020  les = scales.   
-00003650: 2020 2020 2073 656c 662e 766f 6c75 6d65       self.volume
-00003660: 203d 2076 6f6c 756d 650a 2020 2020 2020   = volume.      
-00003670: 2020 7365 6c66 2e6e 6361 7620 3d20 6361    self.ncav = ca
-00003680: 7669 7469 6573 2e6d 6178 2829 202d 2031  vities.max() - 1
-00003690: 0a20 2020 2020 2020 2073 656c 662e 6172  .        self.ar
-000036a0: 6561 203d 2061 7265 610a 2020 2020 2020  ea = area.      
-000036b0: 2020 7365 6c66 2e6d 6178 5f64 6570 7468    self.max_depth
-000036c0: 203d 206d 6178 5f64 6570 7468 0a20 2020   = max_depth.   
-000036d0: 2020 2020 2073 656c 662e 6176 675f 6465       self.avg_de
-000036e0: 7074 6820 3d20 6176 675f 6465 7074 680a  pth = avg_depth.
-000036f0: 2020 2020 2020 2020 7365 6c66 2e61 7667          self.avg
-00003700: 5f68 7964 726f 7061 7468 7920 3d20 6176  _hydropathy = av
-00003710: 675f 6879 6472 6f70 6174 6879 0a20 2020  g_hydropathy.   
-00003720: 2020 2020 2073 656c 662e 7265 7369 6475       self.residu
-00003730: 6573 203d 2072 6573 6964 7565 730a 2020  es = residues.  
-00003740: 2020 2020 2020 7365 6c66 2e66 7265 7175        self.frequ
-00003750: 656e 6369 6573 203d 2066 7265 7175 656e  encies = frequen
-00003760: 6369 6573 0a20 2020 2020 2020 2073 656c  cies.        sel
-00003770: 662e 5f76 6572 7469 6365 7320 3d20 5f76  f._vertices = _v
-00003780: 6572 7469 6365 730a 2020 2020 2020 2020  ertices.        
-00003790: 7365 6c66 2e5f 7374 6570 203d 205f 7374  self._step = _st
-000037a0: 6570 0a20 2020 2020 2020 2073 656c 662e  ep.        self.
-000037b0: 5f69 6e70 7574 203d 206f 732e 7061 7468  _input = os.path
-000037c0: 2e61 6273 7061 7468 285f 696e 7075 7429  .abspath(_input)
-000037d0: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
-000037e0: 6967 616e 6420 3d20 6f73 2e70 6174 682e  igand = os.path.
-000037f0: 6162 7370 6174 6828 5f6c 6967 616e 6429  abspath(_ligand)
-00003800: 2069 6620 5f6c 6967 616e 6420 656c 7365   if _ligand else
-00003810: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
-00003820: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
-00003830: 2020 2020 2020 2072 6574 7572 6e20 223c         return "<
-00003840: 7079 4b56 4669 6e64 6572 5265 7375 6c74  pyKVFinderResult
-00003850: 7320 6f62 6a65 6374 3e22 0a0a 2020 2020  s object>"..    
-00003860: 6465 6620 6578 706f 7274 280a 2020 2020  def export(.    
-00003870: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00003880: 2020 6f75 7470 7574 3a20 556e 696f 6e5b    output: Union[
-00003890: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-000038a0: 685d 203d 2022 6361 7669 7479 2e70 6462  h] = "cavity.pdb
-000038b0: 222c 0a20 2020 2020 2020 206f 7574 7075  ",.        outpu
-000038c0: 745f 6879 6472 6f70 6174 6879 3a20 556e  t_hydropathy: Un
-000038d0: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-000038e0: 2e50 6174 685d 203d 2022 6879 6472 6f70  .Path] = "hydrop
-000038f0: 6174 6879 2e70 6462 222c 0a20 2020 2020  athy.pdb",.     
-00003900: 2020 206e 7468 7265 6164 733a 204f 7074     nthreads: Opt
-00003910: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00003920: 652c 0a20 2020 2029 202d 3e20 4e6f 6e65  e,.    ) -> None
-00003930: 3a0a 2020 2020 2020 2020 2222 2245 7870  :.        """Exp
-00003940: 6f72 7473 2063 6176 6974 6979 2028 4829  orts cavitiy (H)
-00003950: 2061 6e64 2073 7572 6661 6365 2028 4841   and surface (HA
-00003960: 2920 706f 696e 7473 2074 6f20 5044 422d  ) points to PDB-
-00003970: 666f 726d 6174 7465 6420 6669 6c65 0a20  formatted file. 
-00003980: 2020 2020 2020 2077 6974 6820 6120 7661         with a va
-00003990: 7269 6162 6c65 2028 423b 206f 7074 696f  riable (B; optio
-000039a0: 6e61 6c29 2069 6e20 422d 6661 6374 6f72  nal) in B-factor
-000039b0: 2063 6f6c 756d 6e2c 2061 6e64 2068 7964   column, and hyd
-000039c0: 726f 7061 7468 7920 746f 0a20 2020 2020  ropathy to.     
-000039d0: 2020 2050 4442 2d66 6f72 6d61 7474 6564     PDB-formatted
-000039e0: 2066 696c 6520 696e 2042 2d66 6163 746f   file in B-facto
-000039f0: 7220 636f 6c75 6d6e 2061 7420 7375 7266  r column at surf
-00003a00: 6163 6520 706f 696e 7473 2028 4841 292e  ace points (HA).
-00003a10: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00003a20: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00003a30: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00003a40: 6f75 7470 7574 203a 2055 6e69 6f6e 5b73  output : Union[s
-00003a50: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
-00003a60: 5d29 2c20 6f70 7469 6f6e 616c 0a20 2020  ]), optional.   
-00003a70: 2020 2020 2020 2020 2041 2070 6174 6820           A path 
-00003a80: 746f 2050 4442 2066 696c 6520 666f 7220  to PDB file for 
-00003a90: 7772 6974 696e 6720 6361 7669 7469 6573  writing cavities
-00003aa0: 2c20 6279 2064 6566 6175 6c74 2060 6361  , by default `ca
-00003ab0: 7669 7479 2e70 6462 602e 0a20 2020 2020  vity.pdb`..     
-00003ac0: 2020 206f 7574 7075 745f 6879 6472 6f70     output_hydrop
-00003ad0: 6174 6879 203a 2055 6e69 6f6e 5b73 7472  athy : Union[str
-00003ae0: 2c20 7061 7468 6c69 622e 5061 7468 5d2c  , pathlib.Path],
-00003af0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00003b00: 2020 2020 2020 4120 7061 7468 2074 6f20        A path to 
-00003b10: 5044 4220 6669 6c65 2066 6f72 2077 7269  PDB file for wri
-00003b20: 7469 6e67 2068 7964 726f 7061 7468 7920  ting hydropathy 
-00003b30: 6174 2073 7572 6661 6365 2070 6f69 6e74  at surface point
-00003b40: 732c 2062 790a 2020 2020 2020 2020 2020  s, by.          
-00003b50: 2020 6465 6661 756c 7420 6068 7964 726f    default `hydro
-00003b60: 7061 7468 792e 7064 6260 2e0a 2020 2020  pathy.pdb`..    
-00003b70: 2020 2020 6e74 6872 6561 6473 203a 2069      nthreads : i
-00003b80: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-00003b90: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-00003ba0: 6f66 2074 6872 6561 6473 2c20 6279 2064  of threads, by d
-00003bb0: 6566 6175 6c74 204e 6f6e 652e 2049 6620  efault None. If 
-00003bc0: 4e6f 6e65 2c20 7468 6520 6e75 6d62 6572  None, the number
-00003bd0: 206f 6620 7468 7265 6164 7320 6973 0a20   of threads is. 
-00003be0: 2020 2020 2020 2020 2020 2060 6f73 2e63             `os.c
-00003bf0: 7075 5f63 6f75 6e74 2829 202d 2031 602e  pu_count() - 1`.
-00003c00: 0a0a 2020 2020 2020 2020 4e6f 7465 0a20  ..        Note. 
-00003c10: 2020 2020 2020 202d 2d2d 2d0a 2020 2020         ----.    
-00003c20: 2020 2020 5468 6520 6361 7669 7479 206e      The cavity n
-00003c30: 6f6d 656e 636c 6174 7572 6520 6973 2062  omenclature is b
-00003c40: 6173 6564 206f 6e20 7468 6520 696e 7465  ased on the inte
-00003c50: 6765 7220 6c61 6265 6c2e 2054 6865 2063  ger label. The c
-00003c60: 6176 6974 790a 2020 2020 2020 2020 6d61  avity.        ma
-00003c70: 726b 6564 2077 6974 6820 322c 2074 6865  rked with 2, the
-00003c80: 2066 6972 7374 2069 6e74 6567 6572 2063   first integer c
-00003c90: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
-00003ca0: 6120 6361 7669 7479 2c20 6973 204b 4141  a cavity, is KAA
-00003cb0: 2c0a 2020 2020 2020 2020 7468 6520 6361  ,.        the ca
-00003cc0: 7669 7479 206d 6172 6b65 6420 7769 7468  vity marked with
-00003cd0: 2033 2069 7320 4b41 422c 2074 6865 2063   3 is KAB, the c
-00003ce0: 6176 6974 7920 6d61 726b 6564 2077 6974  avity marked wit
-00003cf0: 6820 3420 6973 204b 4143 0a20 2020 2020  h 4 is KAC.     
-00003d00: 2020 2061 6e64 2073 6f20 6f6e 2e0a 0a20     and so on... 
-00003d10: 2020 2020 2020 2045 7861 6d70 6c65 0a20         Example. 
-00003d20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00003d30: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
-00003d40: 7079 4b56 4669 6e64 6572 2069 6d70 6f72  pyKVFinder impor
-00003d50: 7420 7079 4b56 4669 6e64 6572 0a20 2020  t pyKVFinder.   
-00003d60: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-00003d70: 6f73 0a20 2020 2020 2020 203e 3e3e 2070  os.        >>> p
-00003d80: 6462 203d 206f 732e 7061 7468 2e6a 6f69  db = os.path.joi
-00003d90: 6e28 6f73 2e70 6174 682e 6469 726e 616d  n(os.path.dirnam
-00003da0: 6528 7079 4b56 4669 6e64 6572 2e5f 5f66  e(pyKVFinder.__f
-00003db0: 696c 655f 5f29 2c20 2764 6174 6127 2c20  ile__), 'data', 
-00003dc0: 2774 6573 7473 272c 2027 3146 4d4f 2e70  'tests', '1FMO.p
-00003dd0: 6462 2729 0a20 2020 2020 2020 203e 3e3e  db').        >>>
-00003de0: 2072 6573 756c 7473 203d 2070 794b 5646   results = pyKVF
-00003df0: 696e 6465 7228 7064 6229 0a20 2020 2020  inder(pdb).     
-00003e00: 2020 203e 3e3e 2072 6573 756c 7473 2e65     >>> results.e
-00003e10: 7870 6f72 7428 290a 2020 2020 2020 2020  xport().        
-00003e20: 2222 220a 2020 2020 2020 2020 6578 706f  """.        expo
-00003e30: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-00003e40: 6f75 7470 7574 2c0a 2020 2020 2020 2020  output,.        
-00003e50: 2020 2020 7365 6c66 2e63 6176 6974 6965      self.cavitie
-00003e60: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
-00003e70: 656c 662e 7375 7266 6163 652c 0a20 2020  elf.surface,.   
-00003e80: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
-00003e90: 6572 7469 6365 732c 0a20 2020 2020 2020  ertices,.       
-00003ea0: 2020 2020 2073 656c 662e 5f73 7465 702c       self._step,
-00003eb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003ec0: 662e 6465 7074 6873 2c0a 2020 2020 2020  f.depths,.      
-00003ed0: 2020 2020 2020 6f75 7470 7574 5f68 7964        output_hyd
-00003ee0: 726f 7061 7468 792c 0a20 2020 2020 2020  ropathy,.       
-00003ef0: 2020 2020 2073 656c 662e 7363 616c 6573       self.scales
-00003f00: 2c0a 2020 2020 2020 2020 2020 2020 4e6f  ,.            No
-00003f10: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00003f20: 6e74 6872 6561 6473 2c0a 2020 2020 2020  nthreads,.      
-00003f30: 2020 290a 0a20 2020 2064 6566 2077 7269    )..    def wri
-00003f40: 7465 280a 2020 2020 2020 2020 7365 6c66  te(.        self
-00003f50: 2c0a 2020 2020 2020 2020 666e 3a20 556e  ,.        fn: Un
-00003f60: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-00003f70: 2e50 6174 685d 203d 2022 7265 7375 6c74  .Path] = "result
-00003f80: 732e 746f 6d6c 222c 0a20 2020 2020 2020  s.toml",.       
-00003f90: 206f 7574 7075 743a 204f 7074 696f 6e61   output: Optiona
-00003fa0: 6c5b 556e 696f 6e5b 7374 722c 2070 6174  l[Union[str, pat
-00003fb0: 686c 6962 2e50 6174 685d 5d20 3d20 4e6f  hlib.Path]] = No
-00003fc0: 6e65 2c0a 2020 2020 2020 2020 6f75 7470  ne,.        outp
-00003fd0: 7574 5f68 7964 726f 7061 7468 793a 204f  ut_hydropathy: O
-00003fe0: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
-00003ff0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
-00004000: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
-00004010: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00004020: 2022 2222 0a20 2020 2020 2020 2057 7269   """.        Wri
-00004030: 7465 7320 6669 6c65 2070 6174 6873 2061  tes file paths a
-00004040: 6e64 2063 6176 6974 7920 6368 6172 6163  nd cavity charac
-00004050: 7465 7269 7a61 7469 6f6e 2074 6f20 544f  terization to TO
-00004060: 4d4c 2d66 6f72 6d61 7474 6564 2066 696c  ML-formatted fil
-00004070: 650a 0a20 2020 2020 2020 2050 6172 616d  e..        Param
-00004080: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00004090: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-000040a0: 2066 6e20 3a20 556e 696f 6e5b 7374 722c   fn : Union[str,
-000040b0: 2070 6174 686c 6962 2e50 6174 685d 2c20   pathlib.Path], 
-000040c0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-000040d0: 2020 2020 2041 2070 6174 6820 746f 2054       A path to T
-000040e0: 4f4d 4c2d 666f 726d 6174 7465 6420 6669  OML-formatted fi
-000040f0: 6c65 2066 6f72 2077 7269 7469 6e67 2066  le for writing f
-00004100: 696c 6520 7061 7468 7320 616e 6420 6361  ile paths and ca
-00004110: 7669 7479 0a20 2020 2020 2020 2020 2020  vity.           
-00004120: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
-00004130: 6e20 2876 6f6c 756d 652c 2061 7265 612c  n (volume, area,
-00004140: 2064 6570 7468 2061 6e64 2069 6e74 6572   depth and inter
-00004150: 6661 6365 2072 6573 6964 7565 7329 0a20  face residues). 
-00004160: 2020 2020 2020 2020 2020 2070 6572 2063             per c
-00004170: 6176 6974 7920 6465 7465 6374 6564 2c20  avity detected, 
-00004180: 6279 2064 6566 6175 6c74 2060 7265 7375  by default `resu
-00004190: 6c74 732e 746f 6d6c 602e 0a20 2020 2020  lts.toml`..     
-000041a0: 2020 206f 7574 7075 7420 3a20 556e 696f     output : Unio
-000041b0: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
-000041c0: 6174 685d 2c20 6f70 7469 6f6e 616c 0a20  ath], optional. 
-000041d0: 2020 2020 2020 2020 2020 2041 2070 6174             A pat
-000041e0: 6820 746f 2061 2063 6176 6974 7920 5044  h to a cavity PD
-000041f0: 4220 6669 6c65 2c20 6279 2064 6566 6175  B file, by defau
-00004200: 6c74 204e 6f6e 652e 0a20 2020 2020 2020  lt None..       
-00004210: 206f 7574 7075 745f 6879 6472 6f70 6174   output_hydropat
-00004220: 6879 203a 2055 6e69 6f6e 5b73 7472 2c20  hy : Union[str, 
-00004230: 7061 7468 6c69 622e 5061 7468 5d2c 206f  pathlib.Path], o
-00004240: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00004250: 2020 2020 4120 7061 7468 2074 6f20 5044      A path to PD
-00004260: 4220 6669 6c65 2066 6f72 2077 7269 7469  B file for writi
-00004270: 6e67 2068 7964 726f 7061 7468 7920 6174  ng hydropathy at
-00004280: 2073 7572 6661 6365 2070 6f69 6e74 732c   surface points,
-00004290: 2062 790a 2020 2020 2020 2020 2020 2020   by.            
-000042a0: 6465 6661 756c 7420 4e6f 6e65 2e0a 0a20  default None... 
-000042b0: 2020 2020 2020 204e 6f74 650a 2020 2020         Note.    
-000042c0: 2020 2020 2d2d 2d2d 0a20 2020 2020 2020      ----.       
-000042d0: 2054 6865 2063 6176 6974 7920 6e6f 6d65   The cavity nome
-000042e0: 6e63 6c61 7475 7265 2069 7320 6261 7365  nclature is base
-000042f0: 6420 6f6e 2074 6865 2069 6e74 6567 6572  d on the integer
-00004300: 206c 6162 656c 2e20 5468 6520 6361 7669   label. The cavi
-00004310: 7479 0a20 2020 2020 2020 206d 6172 6b65  ty.        marke
-00004320: 6420 7769 7468 2032 2c20 7468 6520 6669  d with 2, the fi
-00004330: 7273 7420 696e 7465 6765 7220 636f 7272  rst integer corr
-00004340: 6573 706f 6e64 696e 6720 746f 2061 2063  esponding to a c
-00004350: 6176 6974 792c 2069 7320 4b41 412c 0a20  avity, is KAA,. 
-00004360: 2020 2020 2020 2074 6865 2063 6176 6974         the cavit
-00004370: 7920 6d61 726b 6564 2077 6974 6820 3320  y marked with 3 
-00004380: 6973 204b 4142 2c20 7468 6520 6361 7669  is KAB, the cavi
-00004390: 7479 206d 6172 6b65 6420 7769 7468 2034  ty marked with 4
-000043a0: 2069 7320 4b41 430a 2020 2020 2020 2020   is KAC.        
-000043b0: 616e 6420 736f 206f 6e2e 0a0a 2020 2020  and so on...    
-000043c0: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
-000043d0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000043e0: 2020 2020 3e3e 3e20 6672 6f6d 2070 794b      >>> from pyK
-000043f0: 5646 696e 6465 7220 696d 706f 7274 2070  VFinder import p
-00004400: 794b 5646 696e 6465 720a 2020 2020 2020  yKVFinder.      
-00004410: 2020 3e3e 3e20 696d 706f 7274 206f 730a    >>> import os.
-00004420: 2020 2020 2020 2020 3e3e 3e20 7064 6220          >>> pdb 
-00004430: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-00004440: 732e 7061 7468 2e64 6972 6e61 6d65 2870  s.path.dirname(p
-00004450: 794b 5646 696e 6465 722e 5f5f 6669 6c65  yKVFinder.__file
-00004460: 5f5f 292c 2027 6461 7461 272c 2027 7465  __), 'data', 'te
-00004470: 7374 7327 2c20 2731 464d 4f2e 7064 6227  sts', '1FMO.pdb'
-00004480: 290a 2020 2020 2020 2020 3e3e 3e20 7265  ).        >>> re
-00004490: 7375 6c74 7320 3d20 7079 4b56 4669 6e64  sults = pyKVFind
-000044a0: 6572 2870 6462 290a 2020 2020 2020 2020  er(pdb).        
-000044b0: 3e3e 3e20 7265 7375 6c74 732e 7772 6974  >>> results.writ
-000044c0: 6528 290a 2020 2020 2020 2020 2222 220a  e().        """.
-000044d0: 2020 2020 2020 2020 7772 6974 655f 7265          write_re
-000044e0: 7375 6c74 7328 0a20 2020 2020 2020 2020  sults(.         
-000044f0: 2020 2066 6e2c 0a20 2020 2020 2020 2020     fn,.         
-00004500: 2020 2073 656c 662e 5f69 6e70 7574 2c0a     self._input,.
-00004510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004520: 2e5f 6c69 6761 6e64 2c0a 2020 2020 2020  ._ligand,.      
-00004530: 2020 2020 2020 6f75 7470 7574 2c0a 2020        output,.  
-00004540: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00004550: 5f68 7964 726f 7061 7468 792c 0a20 2020  _hydropathy,.   
-00004560: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
-00004570: 6c75 6d65 2c0a 2020 2020 2020 2020 2020  lume,.          
-00004580: 2020 7365 6c66 2e61 7265 612c 0a20 2020    self.area,.   
-00004590: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-000045a0: 785f 6465 7074 682c 0a20 2020 2020 2020  x_depth,.       
-000045b0: 2020 2020 2073 656c 662e 6176 675f 6465       self.avg_de
-000045c0: 7074 682c 0a20 2020 2020 2020 2020 2020  pth,.           
-000045d0: 2073 656c 662e 6176 675f 6879 6472 6f70   self.avg_hydrop
-000045e0: 6174 6879 2c0a 2020 2020 2020 2020 2020  athy,.          
-000045f0: 2020 7365 6c66 2e72 6573 6964 7565 732c    self.residues,
-00004600: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004610: 662e 6672 6571 7565 6e63 6965 732c 0a20  f.frequencies,. 
-00004620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004630: 5f73 7465 702c 0a20 2020 2020 2020 2029  _step,.        )
-00004640: 0a0a 2020 2020 6465 6620 706c 6f74 5f66  ..    def plot_f
-00004650: 7265 7175 656e 6369 6573 2873 656c 662c  requencies(self,
-00004660: 2070 6466 3a20 556e 696f 6e5b 7374 722c   pdf: Union[str,
-00004670: 2070 6174 686c 6962 2e50 6174 685d 203d   pathlib.Path] =
-00004680: 2022 6261 7270 6c6f 7473 2e70 6466 2229   "barplots.pdf")
-00004690: 3a0a 2020 2020 2020 2020 2222 2250 6c6f  :.        """Plo
-000046a0: 7420 6261 7220 6368 6172 7473 206f 6620  t bar charts of 
-000046b0: 6672 6571 7565 6e63 6965 7320 2872 6573  frequencies (res
-000046c0: 6964 7565 7320 616e 6420 636c 6173 7365  idues and classe
-000046d0: 7320 6f66 2072 6573 6964 7565 7329 2069  s of residues) i
-000046e0: 6e0a 2020 2020 2020 2020 6120 5044 4620  n.        a PDF 
-000046f0: 6669 6c65 2e0a 0a20 2020 2020 2020 2050  file...        P
-00004700: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00004710: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00004720: 2020 2020 2070 6466 203a 2055 6e69 6f6e       pdf : Union
-00004730: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
-00004740: 7468 5d2c 206f 7074 696f 6e61 6c0a 2020  th], optional.  
-00004750: 2020 2020 2020 2020 2020 4120 7061 7468            A path
-00004760: 2074 6f20 6120 5044 4620 6669 6c65 2c20   to a PDF file, 
-00004770: 6279 2064 6566 6175 6c74 2060 6261 7270  by default `barp
-00004780: 6c6f 7473 2e70 6466 602e 0a0a 2020 2020  lots.pdf`...    
-00004790: 2020 2020 4e6f 7465 0a20 2020 2020 2020      Note.       
-000047a0: 202d 2d2d 2d0a 2020 2020 2020 2020 5468   ----.        Th
-000047b0: 6520 6361 7669 7479 206e 6f6d 656e 636c  e cavity nomencl
-000047c0: 6174 7572 6520 6973 2062 6173 6564 206f  ature is based o
-000047d0: 6e20 7468 6520 696e 7465 6765 7220 6c61  n the integer la
-000047e0: 6265 6c2e 2054 6865 2063 6176 6974 790a  bel. The cavity.
-000047f0: 2020 2020 2020 2020 6d61 726b 6564 2077          marked w
-00004800: 6974 6820 322c 2074 6865 2066 6972 7374  ith 2, the first
-00004810: 2069 6e74 6567 6572 2063 6f72 7265 7370   integer corresp
-00004820: 6f6e 6469 6e67 2074 6f20 6120 6361 7669  onding to a cavi
-00004830: 7479 2c20 6973 204b 4141 2c0a 2020 2020  ty, is KAA,.    
-00004840: 2020 2020 7468 6520 6361 7669 7479 206d      the cavity m
-00004850: 6172 6b65 6420 7769 7468 2033 2069 7320  arked with 3 is 
-00004860: 4b41 422c 2074 6865 2063 6176 6974 7920  KAB, the cavity 
-00004870: 6d61 726b 6564 2077 6974 6820 3420 6973  marked with 4 is
-00004880: 204b 4143 0a20 2020 2020 2020 2061 6e64   KAC.        and
-00004890: 2073 6f20 6f6e 2e0a 0a20 2020 2020 2020   so on...       
-000048a0: 204e 6f74 650a 2020 2020 2020 2020 2d2d   Note.        --
-000048b0: 2d2d 0a20 2020 2020 2020 2054 6865 2063  --.        The c
-000048c0: 6c61 7373 6573 206f 6620 7265 7369 6475  lasses of residu
-000048d0: 6573 2061 7265 3a0a 0a20 2020 2020 2020  es are:..       
-000048e0: 202a 2041 6c69 7068 6174 6963 2061 706f   * Aliphatic apo
-000048f0: 6c61 7220 2852 3129 3a20 416c 616e 696e  lar (R1): Alanin
-00004900: 652c 2047 6c79 6369 6e65 2c20 4973 6f6c  e, Glycine, Isol
-00004910: 6575 6369 6e65 2c20 4c65 7563 696e 652c  eucine, Leucine,
-00004920: 204d 6574 6869 6f6e 696e 652c 2056 616c   Methionine, Val
-00004930: 696e 652e 0a0a 2020 2020 2020 2020 2a20  ine...        * 
-00004940: 4172 6f6d 6174 6963 2028 5232 293a 2050  Aromatic (R2): P
-00004950: 6865 6e79 6c61 6c61 6e69 6e65 2c20 5472  henylalanine, Tr
-00004960: 7970 746f 7068 616e 2c20 5479 726f 7369  yptophan, Tyrosi
-00004970: 6e65 2e0a 0a20 2020 2020 2020 202a 2050  ne...        * P
-00004980: 6f6c 6172 2055 6e63 6861 7267 6564 2028  olar Uncharged (
-00004990: 5233 293a 2041 7370 6172 6167 696e 652c  R3): Asparagine,
-000049a0: 2043 7973 7465 696e 652c 2047 6c75 7461   Cysteine, Gluta
-000049b0: 6d69 6e65 2c20 5072 6f6c 696e 652c 2053  mine, Proline, S
-000049c0: 6572 696e 652c 2054 6872 656f 6e69 6e65  erine, Threonine
-000049d0: 2e0a 0a20 2020 2020 2020 202a 204e 6567  ...        * Neg
-000049e0: 6174 6976 656c 7920 6368 6172 6765 6420  atively charged 
-000049f0: 2852 3429 3a20 4173 7061 7274 6174 652c  (R4): Aspartate,
-00004a00: 2047 6c75 7461 6d61 7465 2e0a 0a20 2020   Glutamate...   
-00004a10: 2020 2020 202a 2050 6f73 6974 6976 656c       * Positivel
-00004a20: 7920 6368 6172 6765 6420 2852 3529 3a20  y charged (R5): 
-00004a30: 4172 6769 6e69 6e65 2c20 4869 7374 6964  Arginine, Histid
-00004a40: 696e 652c 204c 7973 696e 652e 0a0a 2020  ine, Lysine...  
-00004a50: 2020 2020 2020 2a20 4e6f 6e2d 7374 616e        * Non-stan
-00004a60: 6461 7264 2028 5258 293a 204e 6f6e 2d73  dard (RX): Non-s
-00004a70: 7461 6e64 6172 6420 7265 7369 6475 6573  tandard residues
-00004a80: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00004a90: 650a 2020 2020 2020 2020 2d2d 2d2d 2d2d  e.        ------
-00004aa0: 2d0a 2020 2020 2020 2020 3e3e 3e20 6672  -.        >>> fr
-00004ab0: 6f6d 2070 794b 5646 696e 6465 7220 696d  om pyKVFinder im
-00004ac0: 706f 7274 2070 794b 5646 696e 6465 720a  port pyKVFinder.
-00004ad0: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
-00004ae0: 7274 206f 730a 2020 2020 2020 2020 3e3e  rt os.        >>
-00004af0: 3e20 7064 6220 3d20 6f73 2e70 6174 682e  > pdb = os.path.
-00004b00: 6a6f 696e 286f 732e 7061 7468 2e64 6972  join(os.path.dir
-00004b10: 6e61 6d65 2870 794b 5646 696e 6465 722e  name(pyKVFinder.
-00004b20: 5f5f 6669 6c65 5f5f 292c 2027 6461 7461  __file__), 'data
-00004b30: 272c 2027 7465 7374 7327 2c20 2731 464d  ', 'tests', '1FM
-00004b40: 4f2e 7064 6227 290a 2020 2020 2020 2020  O.pdb').        
-00004b50: 3e3e 3e20 7265 7375 6c74 7320 3d20 7079  >>> results = py
-00004b60: 4b56 4669 6e64 6572 2870 6462 290a 2020  KVFinder(pdb).  
-00004b70: 2020 2020 2020 3e3e 3e20 7265 7375 6c74        >>> result
-00004b80: 732e 706c 6f74 5f66 7265 7175 656e 6369  s.plot_frequenci
-00004b90: 6573 2829 0a20 2020 2020 2020 2022 2222  es().        """
-00004ba0: 0a20 2020 2020 2020 2070 6c6f 745f 6672  .        plot_fr
-00004bb0: 6571 7565 6e63 6965 7328 7365 6c66 2e66  equencies(self.f
-00004bc0: 7265 7175 656e 6369 6573 2c20 7064 6629  requencies, pdf)
-00004bd0: 0a0a 2020 2020 6465 6620 6578 706f 7274  ..    def export
-00004be0: 5f61 6c6c 280a 2020 2020 2020 2020 7365  _all(.        se
-00004bf0: 6c66 2c0a 2020 2020 2020 2020 666e 3a20  lf,.        fn: 
-00004c00: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-00004c10: 6962 2e50 6174 685d 203d 2022 7265 7375  ib.Path] = "resu
-00004c20: 6c74 732e 746f 6d6c 222c 0a20 2020 2020  lts.toml",.     
-00004c30: 2020 206f 7574 7075 743a 2055 6e69 6f6e     output: Union
-00004c40: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
-00004c50: 7468 5d20 3d20 2263 6176 6974 792e 7064  th] = "cavity.pd
-00004c60: 6222 2c0a 2020 2020 2020 2020 6f75 7470  b",.        outp
-00004c70: 7574 5f68 7964 726f 7061 7468 793a 2055  ut_hydropathy: U
-00004c80: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-00004c90: 622e 5061 7468 5d20 3d20 2268 7964 726f  b.Path] = "hydro
-00004ca0: 7061 7468 792e 7064 6222 2c0a 2020 2020  pathy.pdb",.    
-00004cb0: 2020 2020 696e 636c 7564 655f 6672 6571      include_freq
-00004cc0: 7565 6e63 6965 735f 7064 663a 2062 6f6f  uencies_pdf: boo
-00004cd0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-00004ce0: 2020 2070 6466 3a20 556e 696f 6e5b 7374     pdf: Union[st
-00004cf0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
-00004d00: 203d 2022 6261 7270 6c6f 7473 2e70 6466   = "barplots.pdf
-00004d10: 222c 0a20 2020 2020 2020 206e 7468 7265  ",.        nthre
-00004d20: 6164 733a 204f 7074 696f 6e61 6c5b 696e  ads: Optional[in
-00004d30: 745d 203d 204e 6f6e 652c 0a20 2020 2029  t] = None,.    )
-00004d40: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00004d50: 2020 2222 2245 7870 6f72 7473 2063 6176    """Exports cav
-00004d60: 6974 6965 7320 616e 6420 6368 6172 6163  ities and charac
-00004d70: 7465 7269 7a61 7469 6f6e 2074 6f20 5044  terization to PD
-00004d80: 422d 666f 726d 6174 7465 6420 6669 6c65  B-formatted file
-00004d90: 732c 0a20 2020 2020 2020 2077 7269 7465  s,.        write
-00004da0: 7320 6669 6c65 2070 6174 6873 2061 6e64  s file paths and
-00004db0: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
-00004dc0: 6e20 746f 2061 2054 4f4d 4c2d 666f 726d  n to a TOML-form
-00004dd0: 6174 7465 6420 6669 6c65 2c20 616e 640a  atted file, and.
-00004de0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00004df0: 6c79 2070 6c6f 7420 6261 7220 6368 6172  ly plot bar char
-00004e00: 7473 206f 6620 6672 6571 7565 6e63 6965  ts of frequencie
-00004e10: 7320 2872 6573 6964 7565 7320 616e 6420  s (residues and 
-00004e20: 636c 6173 7365 7320 6f66 0a20 2020 2020  classes of.     
-00004e30: 2020 2072 6573 6964 7565 7329 2069 6e20     residues) in 
-00004e40: 6120 5044 4620 6669 6c65 2e0a 0a20 2020  a PDF file...   
-00004e50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00004e60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00004e70: 2d2d 0a20 2020 2020 2020 2066 6e20 3a20  --.        fn : 
-00004e80: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-00004e90: 6962 2e50 6174 685d 2c20 6f70 7469 6f6e  ib.Path], option
-00004ea0: 616c 0a20 2020 2020 2020 2020 2020 2041  al.            A
-00004eb0: 2070 6174 6820 746f 2054 4f4d 4c2d 666f   path to TOML-fo
-00004ec0: 726d 6174 7465 6420 6669 6c65 2066 6f72  rmatted file for
-00004ed0: 2077 7269 7469 6e67 2066 696c 6520 7061   writing file pa
-00004ee0: 7468 7320 616e 640a 2020 2020 2020 2020  ths and.        
-00004ef0: 2020 2020 6361 7669 7479 2063 6861 7261      cavity chara
-00004f00: 6374 6572 697a 6174 696f 6e20 2876 6f6c  cterization (vol
-00004f10: 756d 652c 2061 7265 6120 616e 6420 696e  ume, area and in
-00004f20: 7465 7266 6163 6520 7265 7369 6475 6573  terface residues
-00004f30: 290a 2020 2020 2020 2020 2020 2020 7065  ).            pe
-00004f40: 7220 6361 7669 7479 2064 6574 6563 7465  r cavity detecte
-00004f50: 642c 2062 7920 6465 6661 756c 7420 6072  d, by default `r
-00004f60: 6573 756c 7473 2e74 6f6d 6c60 2e0a 2020  esults.toml`..  
-00004f70: 2020 2020 2020 6f75 7470 7574 203a 2055        output : U
-00004f80: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-00004f90: 622e 5061 7468 5d2c 206f 7074 696f 6e61  b.Path], optiona
-00004fa0: 6c0a 2020 2020 2020 2020 2020 2020 4120  l.            A 
-00004fb0: 7061 7468 2074 6f20 5044 4220 6669 6c65  path to PDB file
-00004fc0: 2066 6f72 2077 7269 7469 6e67 2063 6176   for writing cav
-00004fd0: 6974 6965 732c 2062 7920 6465 6661 756c  ities, by defaul
-00004fe0: 7420 6063 6176 6974 792e 7064 6260 2e0a  t `cavity.pdb`..
-00004ff0: 2020 2020 2020 2020 6f75 7470 7574 5f68          output_h
-00005000: 7964 726f 7061 7468 7920 3a20 556e 696f  ydropathy : Unio
-00005010: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
-00005020: 6174 685d 2c20 6f70 7469 6f6e 616c 0a20  ath], optional. 
-00005030: 2020 2020 2020 2020 2020 2041 2070 6174             A pat
-00005040: 6820 746f 2050 4442 2066 696c 6520 666f  h to PDB file fo
-00005050: 7220 7772 6974 696e 6720 6879 6472 6f70  r writing hydrop
-00005060: 6174 6879 2061 7420 7375 7266 6163 6520  athy at surface 
-00005070: 706f 696e 7473 2c0a 2020 2020 2020 2020  points,.        
-00005080: 2020 2020 6279 2064 6566 6175 6c74 2060      by default `
-00005090: 6879 6472 6f70 6174 6879 2e70 6462 602e  hydropathy.pdb`.
-000050a0: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
-000050b0: 5f66 7265 7175 656e 6369 6573 5f70 6466  _frequencies_pdf
-000050c0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-000050d0: 6c0a 2020 2020 2020 2020 2020 2020 5768  l.            Wh
-000050e0: 6574 6865 7220 746f 2070 6c6f 7420 6672  ether to plot fr
-000050f0: 6571 7565 6e63 6965 7320 2872 6573 6964  equencies (resid
-00005100: 7565 7320 616e 6420 636c 6173 7365 7320  ues and classes 
-00005110: 6f66 2072 6573 6964 7565 7329 0a20 2020  of residues).   
-00005120: 2020 2020 2020 2020 2074 6f20 5044 4620           to PDF 
-00005130: 6669 6c65 2c20 6279 2064 6566 6175 6c74  file, by default
-00005140: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00005150: 7064 6620 3a20 556e 696f 6e5b 7374 722c  pdf : Union[str,
-00005160: 2070 6174 686c 6962 2e50 6174 685d 2c20   pathlib.Path], 
-00005170: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00005180: 2020 2020 2041 2070 6174 6820 746f 2061       A path to a
-00005190: 2050 4446 2066 696c 652c 2062 7920 6465   PDF file, by de
-000051a0: 6661 756c 7420 6062 6172 706c 6f74 732e  fault `barplots.
-000051b0: 7064 6660 2e0a 2020 2020 2020 2020 6e74  pdf`..        nt
-000051c0: 6872 6561 6473 203a 2069 6e74 2c20 6f70  hreads : int, op
-000051d0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-000051e0: 2020 204e 756d 6265 7220 6f66 2074 6872     Number of thr
-000051f0: 6561 6473 2c20 6279 2064 6566 6175 6c74  eads, by default
-00005200: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
-00005210: 7468 6520 6e75 6d62 6572 206f 6620 7468  the number of th
-00005220: 7265 6164 7320 6973 0a20 2020 2020 2020  reads is.       
-00005230: 2020 2020 2060 6f73 2e63 7075 5f63 6f75       `os.cpu_cou
-00005240: 6e74 2829 202d 2031 602e 0a0a 2020 2020  nt() - 1`...    
-00005250: 2020 2020 4e6f 7465 0a20 2020 2020 2020      Note.       
-00005260: 202d 2d2d 2d0a 2020 2020 2020 2020 5468   ----.        Th
-00005270: 6520 6361 7669 7479 206e 6f6d 656e 636c  e cavity nomencl
-00005280: 6174 7572 6520 6973 2062 6173 6564 206f  ature is based o
-00005290: 6e20 7468 6520 696e 7465 6765 7220 6c61  n the integer la
-000052a0: 6265 6c2e 2054 6865 2063 6176 6974 790a  bel. The cavity.
-000052b0: 2020 2020 2020 2020 6d61 726b 6564 2077          marked w
-000052c0: 6974 6820 322c 2074 6865 2066 6972 7374  ith 2, the first
-000052d0: 2069 6e74 6567 6572 2063 6f72 7265 7370   integer corresp
-000052e0: 6f6e 6469 6e67 2074 6f20 6120 6361 7669  onding to a cavi
-000052f0: 7479 2c20 6973 204b 4141 2c0a 2020 2020  ty, is KAA,.    
-00005300: 2020 2020 7468 6520 6361 7669 7479 206d      the cavity m
-00005310: 6172 6b65 6420 7769 7468 2033 2069 7320  arked with 3 is 
-00005320: 4b41 422c 2074 6865 2063 6176 6974 7920  KAB, the cavity 
-00005330: 6d61 726b 6564 2077 6974 6820 3420 6973  marked with 4 is
-00005340: 204b 4143 0a20 2020 2020 2020 2061 6e64   KAC.        and
-00005350: 2073 6f20 6f6e 2e0a 0a20 2020 2020 2020   so on...       
-00005360: 204e 6f74 650a 2020 2020 2020 2020 2d2d   Note.        --
-00005370: 2d2d 0a20 2020 2020 2020 2054 6865 2063  --.        The c
-00005380: 6c61 7373 6573 206f 6620 7265 7369 6475  lasses of residu
-00005390: 6573 2061 7265 3a0a 0a20 2020 2020 2020  es are:..       
-000053a0: 202a 2041 6c69 7068 6174 6963 2061 706f   * Aliphatic apo
-000053b0: 6c61 7220 2852 3129 3a20 416c 616e 696e  lar (R1): Alanin
-000053c0: 652c 2047 6c79 6369 6e65 2c20 4973 6f6c  e, Glycine, Isol
-000053d0: 6575 6369 6e65 2c20 4c65 7563 696e 652c  eucine, Leucine,
-000053e0: 204d 6574 6869 6f6e 696e 652c 2056 616c   Methionine, Val
-000053f0: 696e 652e 0a0a 2020 2020 2020 2020 2a20  ine...        * 
-00005400: 4172 6f6d 6174 6963 2028 5232 293a 2050  Aromatic (R2): P
-00005410: 6865 6e79 6c61 6c61 6e69 6e65 2c20 5472  henylalanine, Tr
-00005420: 7970 746f 7068 616e 2c20 5479 726f 7369  yptophan, Tyrosi
-00005430: 6e65 2e0a 0a20 2020 2020 2020 202a 2050  ne...        * P
-00005440: 6f6c 6172 2055 6e63 6861 7267 6564 2028  olar Uncharged (
-00005450: 5233 293a 2041 7370 6172 6167 696e 652c  R3): Asparagine,
-00005460: 2043 7973 7465 696e 652c 2047 6c75 7461   Cysteine, Gluta
-00005470: 6d69 6e65 2c20 5072 6f6c 696e 652c 2053  mine, Proline, S
-00005480: 6572 696e 652c 2054 6872 656f 6e69 6e65  erine, Threonine
-00005490: 2e0a 0a20 2020 2020 2020 202a 204e 6567  ...        * Neg
-000054a0: 6174 6976 656c 7920 6368 6172 6765 6420  atively charged 
-000054b0: 2852 3429 3a20 4173 7061 7274 6174 652c  (R4): Aspartate,
-000054c0: 2047 6c75 7461 6d61 7465 2e0a 0a20 2020   Glutamate...   
-000054d0: 2020 2020 202a 2050 6f73 6974 6976 656c       * Positivel
-000054e0: 7920 6368 6172 6765 6420 2852 3529 3a20  y charged (R5): 
-000054f0: 4172 6769 6e69 6e65 2c20 4869 7374 6964  Arginine, Histid
-00005500: 696e 652c 204c 7973 696e 652e 0a0a 2020  ine, Lysine...  
-00005510: 2020 2020 2020 2a20 4e6f 6e2d 7374 616e        * Non-stan
-00005520: 6461 7264 2028 5258 293a 204e 6f6e 2d73  dard (RX): Non-s
-00005530: 7461 6e64 6172 6420 7265 7369 6475 6573  tandard residues
-00005540: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00005550: 6c65 0a20 2020 2020 2020 202d 2d2d 2d2d  le.        -----
-00005560: 2d2d 0a20 2020 2020 2020 203e 3e3e 2066  --.        >>> f
-00005570: 726f 6d20 7079 4b56 4669 6e64 6572 2069  rom pyKVFinder i
-00005580: 6d70 6f72 7420 7079 4b56 4669 6e64 6572  mport pyKVFinder
-00005590: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
-000055a0: 6f72 7420 6f73 0a20 2020 2020 2020 203e  ort os.        >
-000055b0: 3e3e 2070 6462 203d 206f 732e 7061 7468  >> pdb = os.path
-000055c0: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
-000055d0: 726e 616d 6528 7079 4b56 4669 6e64 6572  rname(pyKVFinder
-000055e0: 2e5f 5f66 696c 655f 5f29 2c20 2764 6174  .__file__), 'dat
-000055f0: 6127 2c20 2774 6573 7473 272c 2027 3146  a', 'tests', '1F
-00005600: 4d4f 2e70 6462 2729 0a20 2020 2020 2020  MO.pdb').       
-00005610: 203e 3e3e 2072 6573 756c 7473 203d 2070   >>> results = p
-00005620: 794b 5646 696e 6465 7228 7064 6229 0a20  yKVFinder(pdb). 
-00005630: 2020 2020 2020 203e 3e3e 2072 6573 756c         >>> resul
-00005640: 7473 2e65 7870 6f72 745f 616c 6c28 290a  ts.export_all().
-00005650: 0a20 2020 2020 2020 2059 6574 2c20 7765  .        Yet, we
-00005660: 2063 616e 2073 6574 2061 2060 6069 6e63   can set a ``inc
-00005670: 6c75 6465 5f66 7265 7175 656e 6369 6573  lude_frequencies
-00005680: 5f70 6466 6060 2066 6c61 6720 746f 2054  _pdf`` flag to T
-00005690: 7275 6520 746f 2070 6c6f 7420 7468 6520  rue to plot the 
-000056a0: 6261 7220 6368 6172 7473 206f 6620 7468  bar charts of th
-000056b0: 6520 6672 6571 7565 6e63 6965 7320 696e  e frequencies in
-000056c0: 2061 2050 4446 2066 696c 652e 0a0a 2020   a PDF file...  
-000056d0: 2020 2020 2020 3e3e 3e20 7265 7375 6c74        >>> result
-000056e0: 732e 6578 706f 7274 5f61 6c6c 2869 6e63  s.export_all(inc
-000056f0: 6c75 6465 5f66 7265 7175 656e 6369 6573  lude_frequencies
-00005700: 5f70 6466 3d54 7275 6529 0a20 2020 2020  _pdf=True).     
-00005710: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00005720: 2045 7870 6f72 7420 6361 7669 7479 2050   Export cavity P
-00005730: 4442 2066 696c 650a 2020 2020 2020 2020  DB file.        
-00005740: 7365 6c66 2e65 7870 6f72 7428 6f75 7470  self.export(outp
-00005750: 7574 2c20 6f75 7470 7574 5f68 7964 726f  ut, output_hydro
-00005760: 7061 7468 792c 206e 7468 7265 6164 7329  pathy, nthreads)
-00005770: 0a20 2020 2020 2020 2023 2057 7269 7465  .        # Write
-00005780: 204b 5646 696e 6465 7220 7265 7375 6c74   KVFinder result
-00005790: 7320 544f 4d4c 0a20 2020 2020 2020 2073  s TOML.        s
-000057a0: 656c 662e 7772 6974 6528 666e 2c20 6f75  elf.write(fn, ou
-000057b0: 7470 7574 2c20 6f75 7470 7574 5f68 7964  tput, output_hyd
-000057c0: 726f 7061 7468 7929 0a20 2020 2020 2020  ropathy).       
-000057d0: 2023 2050 6c6f 7420 6261 7220 6368 6172   # Plot bar char
-000057e0: 7473 206f 6620 6672 6571 7565 6e63 6965  ts of frequencie
-000057f0: 730a 2020 2020 2020 2020 6966 2069 6e63  s.        if inc
-00005800: 6c75 6465 5f66 7265 7175 656e 6369 6573  lude_frequencies
-00005810: 5f70 6466 3a0a 2020 2020 2020 2020 2020  _pdf:.          
-00005820: 2020 7365 6c66 2e70 6c6f 745f 6672 6571    self.plot_freq
-00005830: 7565 6e63 6965 7328 7064 6629 0a0a 0a64  uencies(pdf)...d
-00005840: 6566 2072 756e 5f77 6f72 6b66 6c6f 7728  ef run_workflow(
-00005850: 0a20 2020 2069 6e70 7574 3a20 556e 696f  .    input: Unio
-00005860: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
-00005870: 6174 685d 2c0a 2020 2020 6c69 6761 6e64  ath],.    ligand
-00005880: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
-00005890: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
-000058a0: 7468 5d5d 203d 204e 6f6e 652c 0a20 2020  th]] = None,.   
-000058b0: 2076 6477 3a20 4f70 7469 6f6e 616c 5b55   vdw: Optional[U
-000058c0: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-000058d0: 622e 5061 7468 5d5d 203d 204e 6f6e 652c  b.Path]] = None,
-000058e0: 0a20 2020 2062 6f78 3a20 4f70 7469 6f6e  .    box: Option
-000058f0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 7061  al[Union[str, pa
-00005900: 7468 6c69 622e 5061 7468 5d5d 203d 204e  thlib.Path]] = N
-00005910: 6f6e 652c 0a20 2020 2073 7465 703a 2055  one,.    step: U
-00005920: 6e69 6f6e 5b66 6c6f 6174 2c20 696e 745d  nion[float, int]
-00005930: 203d 2030 2e36 2c0a 2020 2020 7072 6f62   = 0.6,.    prob
-00005940: 655f 696e 3a20 556e 696f 6e5b 666c 6f61  e_in: Union[floa
-00005950: 742c 2069 6e74 5d20 3d20 312e 342c 0a20  t, int] = 1.4,. 
-00005960: 2020 2070 726f 6265 5f6f 7574 3a20 556e     probe_out: Un
-00005970: 696f 6e5b 666c 6f61 742c 2069 6e74 5d20  ion[float, int] 
-00005980: 3d20 342e 302c 0a20 2020 2072 656d 6f76  = 4.0,.    remov
-00005990: 616c 5f64 6973 7461 6e63 653a 2055 6e69  al_distance: Uni
-000059a0: 6f6e 5b66 6c6f 6174 2c20 696e 745d 203d  on[float, int] =
-000059b0: 2032 2e34 2c0a 2020 2020 766f 6c75 6d65   2.4,.    volume
-000059c0: 5f63 7574 6f66 663a 2055 6e69 6f6e 5b66  _cutoff: Union[f
-000059d0: 6c6f 6174 2c20 696e 745d 203d 2035 2e30  loat, int] = 5.0
-000059e0: 2c0a 2020 2020 6c69 6761 6e64 5f63 7574  ,.    ligand_cut
-000059f0: 6f66 663a 2055 6e69 6f6e 5b66 6c6f 6174  off: Union[float
-00005a00: 2c20 696e 745d 203d 2035 2e30 2c0a 2020  , int] = 5.0,.  
-00005a10: 2020 696e 636c 7564 655f 6465 7074 683a    include_depth:
-00005a20: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00005a30: 2020 2069 6e63 6c75 6465 5f68 7964 726f     include_hydro
-00005a40: 7061 7468 793a 2062 6f6f 6c20 3d20 4661  pathy: bool = Fa
-00005a50: 6c73 652c 0a20 2020 2068 7964 726f 7068  lse,.    hydroph
-00005a60: 6f62 6963 6974 795f 7363 616c 653a 2055  obicity_scale: U
-00005a70: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-00005a80: 622e 5061 7468 5d20 3d20 2245 6973 656e  b.Path] = "Eisen
-00005a90: 6265 7267 5765 6973 7322 2c0a 2020 2020  bergWeiss",.    
-00005aa0: 7375 7266 6163 653a 2073 7472 203d 2022  surface: str = "
-00005ab0: 5345 5322 2c0a 2020 2020 6967 6e6f 7265  SES",.    ignore
-00005ac0: 5f62 6163 6b62 6f6e 653a 2062 6f6f 6c20  _backbone: bool 
-00005ad0: 3d20 4661 6c73 652c 0a20 2020 206d 6f64  = False,.    mod
-00005ae0: 656c 3a20 4f70 7469 6f6e 616c 5b69 6e74  el: Optional[int
-00005af0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6e74  ] = None,.    nt
-00005b00: 6872 6561 6473 3a20 4f70 7469 6f6e 616c  hreads: Optional
-00005b10: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-00005b20: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-00005b30: 3d20 4661 6c73 652c 0a29 202d 3e20 7079  = False,.) -> py
-00005b40: 4b56 4669 6e64 6572 5265 7375 6c74 733a  KVFinderResults:
-00005b50: 0a20 2020 2022 2222 4465 7465 6374 7320  .    """Detects 
-00005b60: 616e 6420 6368 6172 6163 7465 7269 7a65  and characterize
-00005b70: 7320 6361 7669 7469 6573 2028 766f 6c75  s cavities (volu
-00005b80: 6d65 2c20 6172 6561 2c20 6465 7074 6820  me, area, depth 
-00005b90: 5b6f 7074 696f 6e61 6c5d 2c0a 2020 2020  [optional],.    
-00005ba0: 6879 6472 6f70 6174 6879 205b 6f70 7469  hydropathy [opti
-00005bb0: 6f6e 616c 5d20 616e 6420 696e 7465 7266  onal] and interf
-00005bc0: 6163 6520 7265 7369 6475 6573 292e 0a0a  ace residues)...
-00005bd0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00005be0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00005bf0: 2020 696e 7075 7420 3a20 556e 696f 6e5b    input : Union[
-00005c00: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-00005c10: 685d 0a20 2020 2020 2020 2041 2070 6174  h].        A pat
-00005c20: 6820 746f 2061 2074 6172 6765 7420 7374  h to a target st
-00005c30: 7275 6374 7572 6520 6669 6c65 2c20 696e  ructure file, in
-00005c40: 2050 4442 206f 7220 5859 5a20 666f 726d   PDB or XYZ form
-00005c50: 6174 2c20 746f 2064 6574 6563 7420 616e  at, to detect an
-00005c60: 6420 6368 6172 6163 7465 7269 7a65 2063  d characterize c
-00005c70: 6176 6974 6965 732e 0a20 2020 206c 6967  avities..    lig
-00005c80: 616e 6420 3a20 556e 696f 6e5b 7374 722c  and : Union[str,
-00005c90: 2070 6174 686c 6962 2e50 6174 685d 2c20   pathlib.Path], 
-00005ca0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00005cb0: 2041 2070 6174 6820 746f 206c 6967 616e   A path to ligan
-00005cc0: 6420 6669 6c65 2c20 696e 2050 4442 206f  d file, in PDB o
-00005cd0: 7220 5859 5a20 666f 726d 6174 2c20 6279  r XYZ format, by
-00005ce0: 2064 6566 6175 6c74 204e 6f6e 652e 0a20   default None.. 
-00005cf0: 2020 2076 6477 203a 2055 6e69 6f6e 5b73     vdw : Union[s
-00005d00: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
-00005d10: 5d2c 206f 7074 696f 6e61 6c0a 2020 2020  ], optional.    
-00005d20: 2020 2020 4120 7061 7468 2074 6f20 6120      A path to a 
-00005d30: 7661 6e20 6465 7220 5761 616c 7320 7261  van der Waals ra
-00005d40: 6469 6920 6669 6c65 2c20 6279 2064 6566  dii file, by def
-00005d50: 6175 6c74 204e 6f6e 652e 2049 6620 4e6f  ault None. If No
-00005d60: 6e65 2c20 6170 706c 7920 7468 6520 6275  ne, apply the bu
-00005d70: 696c 742d 696e 2076 616e 2064 6572 0a20  ilt-in van der. 
-00005d80: 2020 2020 2020 2057 6161 6c73 2072 6164         Waals rad
-00005d90: 6969 2066 696c 653a 2060 7664 772e 6461  ii file: `vdw.da
-00005da0: 7460 2e0a 2020 2020 626f 7820 3a20 556e  t`..    box : Un
-00005db0: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-00005dc0: 2e50 6174 685d 2c20 6f70 7469 6f6e 616c  .Path], optional
-00005dd0: 0a20 2020 2020 2020 2041 2070 6174 6820  .        A path 
-00005de0: 746f 2062 6f78 2063 6f6e 6669 6775 7261  to box configura
-00005df0: 7469 6f6e 2066 696c 6520 2854 4f4d 4c2d  tion file (TOML-
-00005e00: 666f 726d 6174 7465 6429 2c20 6279 2064  formatted), by d
-00005e10: 6566 6175 6c74 204e 6f6e 652e 0a20 2020  efault None..   
-00005e20: 2073 7465 7020 3a20 556e 696f 6e5b 666c   step : Union[fl
-00005e30: 6f61 742c 2069 6e74 5d2c 206f 7074 696f  oat, int], optio
-00005e40: 6e61 6c0a 2020 2020 2020 2020 4772 6964  nal.        Grid
-00005e50: 2073 7061 6369 6e67 2028 4129 2c20 6279   spacing (A), by
-00005e60: 2064 6566 6175 6c74 2030 2e36 2e0a 2020   default 0.6..  
-00005e70: 2020 7072 6f62 655f 696e 203a 2055 6e69    probe_in : Uni
-00005e80: 6f6e 5b66 6c6f 6174 2c20 696e 745d 2c20  on[float, int], 
-00005e90: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00005ea0: 2050 726f 6265 2049 6e20 7369 7a65 2028   Probe In size (
-00005eb0: 4129 2c20 6279 2064 6566 6175 6c74 2031  A), by default 1
-00005ec0: 2e34 2e0a 2020 2020 7072 6f62 655f 6f75  .4..    probe_ou
-00005ed0: 7420 3a20 556e 696f 6e5b 666c 6f61 742c  t : Union[float,
-00005ee0: 2069 6e74 5d2c 206f 7074 696f 6e61 6c0a   int], optional.
-00005ef0: 2020 2020 2020 2020 5072 6f62 6520 4f75          Probe Ou
-00005f00: 7420 7369 7a65 2028 4129 2c20 6279 2064  t size (A), by d
-00005f10: 6566 6175 6c74 2034 2e30 2e0a 2020 2020  efault 4.0..    
-00005f20: 7265 6d6f 7661 6c5f 6469 7374 616e 6365  removal_distance
-00005f30: 203a 2055 6e69 6f6e 5b66 6c6f 6174 2c20   : Union[float, 
-00005f40: 696e 745d 2c20 6f70 7469 6f6e 616c 0a20  int], optional. 
-00005f50: 2020 2020 2020 204c 656e 6774 6820 746f         Length to
-00005f60: 2062 6520 7265 6d6f 7665 6420 6672 6f6d   be removed from
-00005f70: 2074 6865 2063 6176 6974 792d 6275 6c6b   the cavity-bulk
-00005f80: 2066 726f 6e74 6965 7220 2841 292c 2062   frontier (A), b
-00005f90: 7920 6465 6661 756c 7420 322e 342e 0a20  y default 2.4.. 
-00005fa0: 2020 2076 6f6c 756d 655f 6375 746f 6666     volume_cutoff
-00005fb0: 203a 2055 6e69 6f6e 5b66 6c6f 6174 2c20   : Union[float, 
-00005fc0: 696e 745d 2c20 6f70 7469 6f6e 616c 0a20  int], optional. 
-00005fd0: 2020 2020 2020 2043 6176 6974 6965 7320         Cavities 
-00005fe0: 766f 6c75 6d65 2066 696c 7465 7220 2841  volume filter (A
-00005ff0: 3329 2c20 6279 2064 6566 6175 6c74 2035  3), by default 5
-00006000: 2e30 2e0a 2020 2020 6c69 6761 6e64 5f63  .0..    ligand_c
-00006010: 7574 6f66 6620 3a20 556e 696f 6e5b 666c  utoff : Union[fl
-00006020: 6f61 742c 2069 6e74 5d2c 206f 7074 696f  oat, int], optio
-00006030: 6e61 6c0a 2020 2020 2020 2020 5261 6469  nal.        Radi
-00006040: 7573 2076 616c 7565 2074 6f20 6c69 6d69  us value to limi
-00006050: 7420 6120 7370 6163 6520 6172 6f75 6e64  t a space around
-00006060: 2061 206c 6967 616e 6420 2841 292c 2062   a ligand (A), b
-00006070: 7920 6465 6661 756c 7420 352e 302e 0a20  y default 5.0.. 
-00006080: 2020 2069 6e63 6c75 6465 5f64 6570 7468     include_depth
-00006090: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-000060a0: 6c0a 2020 2020 2020 2020 5768 6574 6865  l.        Whethe
-000060b0: 7220 746f 2063 6861 7261 6374 6572 697a  r to characteriz
-000060c0: 6520 7468 6520 6465 7074 6820 6f66 2074  e the depth of t
-000060d0: 6865 2064 6574 6563 7465 6420 6361 7669  he detected cavi
-000060e0: 7469 6573 2c20 6279 0a20 2020 2020 2020  ties, by.       
-000060f0: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
-00006100: 2020 2020 696e 636c 7564 655f 6879 6472      include_hydr
-00006110: 6f70 6174 6879 203a 2062 6f6f 6c2c 206f  opathy : bool, o
-00006120: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00006130: 5768 6574 6865 7220 746f 2063 6861 7261  Whether to chara
-00006140: 6374 6572 697a 6520 7468 6520 6879 6472  cterize the hydr
-00006150: 6f70 6174 6879 206f 6620 7468 6520 6465  opathy of the de
-00006160: 7465 6374 6564 2063 6176 6974 6965 732c  tected cavities,
-00006170: 2062 790a 2020 2020 2020 2020 6465 6661   by.        defa
-00006180: 756c 7420 4661 6c73 652e 0a20 2020 2068  ult False..    h
-00006190: 7964 726f 7068 6f62 6963 6974 795f 7363  ydrophobicity_sc
-000061a0: 616c 6520 3a20 556e 696f 6e5b 7374 722c  ale : Union[str,
-000061b0: 2070 6174 686c 6962 2e50 6174 685d 2c20   pathlib.Path], 
-000061c0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-000061d0: 204e 616d 6520 6f66 2061 2062 7569 6c74   Name of a built
-000061e0: 2d69 6e20 6879 6472 6f70 686f 6269 6369  -in hydrophobici
-000061f0: 7479 2073 6361 6c65 2028 4569 7365 6e62  ty scale (Eisenb
-00006200: 6572 6757 6569 7373 2c20 4865 7373 6148  ergWeiss, HessaH
-00006210: 6569 6a6e 652c 0a20 2020 2020 2020 204b  eijne,.        K
-00006220: 7974 6544 6f6f 6c69 7474 652c 204d 6f6f  yteDoolitte, Moo
-00006230: 6e46 6c65 6d69 6e67 2c20 5261 647a 6963  nFleming, Radzic
-00006240: 6b61 576f 6c66 656e 6465 6e2c 2057 696d  kaWolfenden, Wim
-00006250: 6c65 7957 6869 7465 2c20 5a68 616f 4c6f  leyWhite, ZhaoLo
-00006260: 6e64 6f6e 2920 0a20 2020 2020 2020 206f  ndon) .        o
-00006270: 7220 6120 7061 7468 2074 6f20 6120 544f  r a path to a TO
-00006280: 4d4c 2d66 6f72 6d61 7474 6564 2066 696c  ML-formatted fil
-00006290: 6520 7769 7468 2061 2063 7573 746f 6d20  e with a custom 
-000062a0: 6879 6472 6f70 686f 6269 6369 7479 2073  hydrophobicity s
-000062b0: 6361 6c65 2c0a 2020 2020 2020 2020 6279  cale,.        by
-000062c0: 2064 6566 6175 6c74 2060 4569 7365 6e62   default `Eisenb
-000062d0: 6572 6757 6569 7373 602e 0a20 2020 2073  ergWeiss`..    s
-000062e0: 7572 6661 6365 203a 2073 7472 2c20 6f70  urface : str, op
-000062f0: 7469 6f6e 616c 0a20 2020 2020 2020 204b  tional.        K
-00006300: 6579 776f 7264 7320 6f70 7469 6f6e 7320  eywords options 
-00006310: 6172 6520 5345 5320 2853 6f6c 7665 6e74  are SES (Solvent
-00006320: 2045 7863 6c75 6465 6420 5375 7266 6163   Excluded Surfac
-00006330: 6529 206f 7220 5341 5320 2853 6f6c 7665  e) or SAS (Solve
-00006340: 6e74 0a20 2020 2020 2020 2041 6363 6573  nt.        Acces
-00006350: 7369 626c 6520 5375 7266 6163 6529 2c20  sible Surface), 
-00006360: 6279 2064 6566 6175 6c74 2053 4553 2e0a  by default SES..
-00006370: 2020 2020 6967 6e6f 7265 5f62 6163 6b62      ignore_backb
-00006380: 6f6e 6520 3a20 626f 6f6c 2c20 6f70 7469  one : bool, opti
-00006390: 6f6e 616c 0a20 2020 2020 2020 2057 6865  onal.        Whe
-000063a0: 7468 6572 2074 6f20 6967 6e6f 7265 2062  ther to ignore b
-000063b0: 6163 6b62 6f6e 6520 6174 6f6d 7320 2843  ackbone atoms (C
-000063c0: 2c20 4341 2c20 4e2c 204f 2920 7768 656e  , CA, N, O) when
-000063d0: 2064 6566 696e 696e 6720 696e 7465 7266   defining interf
-000063e0: 6163 650a 2020 2020 2020 2020 7265 7369  ace.        resi
-000063f0: 6475 6573 2c20 6279 2064 6566 6175 6c74  dues, by default
-00006400: 2046 616c 7365 2e0a 2020 2020 6d6f 6465   False..    mode
-00006410: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
-00006420: 6c0a 2020 2020 2020 2020 4d6f 6465 6c20  l.        Model 
-00006430: 6e75 6d62 6572 2c20 6279 2064 6566 6175  number, by defau
-00006440: 6c74 204e 6f6e 652e 2049 6620 4e6f 6e65  lt None. If None
-00006450: 2c20 6b65 6570 2061 746f 6d73 2066 726f  , keep atoms fro
-00006460: 6d20 616c 6c20 6d6f 6465 6c73 2e0a 2020  m all models..  
-00006470: 2020 6e74 6872 6561 6473 203a 2069 6e74    nthreads : int
-00006480: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00006490: 2020 204e 756d 6265 7220 6f66 2074 6872     Number of thr
-000064a0: 6561 6473 2c20 6279 2064 6566 6175 6c74  eads, by default
-000064b0: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
-000064c0: 7468 6520 6e75 6d62 6572 206f 6620 7468  the number of th
-000064d0: 7265 6164 7320 6973 0a20 2020 2020 2020  reads is.       
-000064e0: 2060 6f73 2e63 7075 5f63 6f75 6e74 2829   `os.cpu_count()
-000064f0: 202d 2031 602e 0a20 2020 2076 6572 626f   - 1`..    verbo
-00006500: 7365 203a 2062 6f6f 6c2c 206f 7074 696f  se : bool, optio
-00006510: 6e61 6c0a 2020 2020 2020 2020 5072 696e  nal.        Prin
-00006520: 7420 6578 7472 6120 696e 666f 726d 6174  t extra informat
-00006530: 696f 6e20 746f 2073 7461 6e64 6172 6420  ion to standard 
-00006540: 6f75 7470 7574 2c20 6279 2064 6566 6175  output, by defau
-00006550: 6c74 2046 616c 7365 2e0a 0a20 2020 2052  lt False...    R
-00006560: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00006570: 2d2d 0a20 2020 2072 6573 756c 7473 203a  --.    results :
-00006580: 2070 794b 5646 696e 6465 7252 6573 756c   pyKVFinderResul
-00006590: 7473 0a20 2020 2020 2020 2041 2063 6c61  ts.        A cla
-000065a0: 7373 2077 6974 6820 7468 6520 666f 6c6c  ss with the foll
-000065b0: 6f77 696e 6720 6174 7472 6962 7574 6573  owing attributes
-000065c0: 2064 6566 696e 6564 3a0a 0a20 2020 2020   defined:..     
-000065d0: 2020 2020 2020 202a 2063 6176 6974 6965         * cavitie
-000065e0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
-000065f0: 790a 0a20 2020 2020 2020 2020 2020 2020  y..             
-00006600: 2020 2043 6176 6974 7920 706f 696e 7473     Cavity points
-00006610: 2069 6e20 7468 6520 3344 2067 7269 6420   in the 3D grid 
-00006620: 2863 6176 6974 6965 735b 6e78 5d5b 6e79  (cavities[nx][ny
-00006630: 5d5b 6e7a 5d29 2e0a 2020 2020 2020 2020  ][nz])..        
-00006640: 2020 2020 2020 2020 4361 7669 7469 6573          Cavities
-00006650: 2061 7272 6179 2068 6173 2069 6e74 6567   array has integ
-00006660: 6572 206c 6162 656c 7320 696e 2065 6163  er labels in eac
-00006670: 6820 706f 7369 7469 6f6e 2c20 7468 6174  h position, that
-00006680: 2061 7265 3a0a 0a20 2020 2020 2020 2020   are:..         
-00006690: 2020 2020 2020 202a 202d 313a 2062 756c         * -1: bul
-000066a0: 6b20 706f 696e 7473 3b0a 2020 2020 2020  k points;.      
-000066b0: 2020 2020 2020 2020 2020 2a20 303a 2062            * 0: b
-000066c0: 696f 6d6f 6c65 6375 6c65 2070 6f69 6e74  iomolecule point
-000066d0: 733b 0a20 2020 2020 2020 2020 2020 2020  s;.             
-000066e0: 2020 202a 2031 3a20 656d 7074 7920 7370     * 1: empty sp
-000066f0: 6163 6520 706f 696e 7473 3b0a 2020 2020  ace points;.    
-00006700: 2020 2020 2020 2020 2020 2020 2a20 3e3d              * >=
-00006710: 323a 2063 6176 6974 7920 706f 696e 7473  2: cavity points
-00006720: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00006730: 2020 2054 6865 2065 6d70 7479 2073 7061     The empty spa
-00006740: 6365 2070 6f69 6e74 7320 6172 6520 7265  ce points are re
-00006750: 6769 6f6e 7320 7468 6174 2064 6f20 6e6f  gions that do no
-00006760: 7420 6d65 6574 2074 6865 2063 686f 7365  t meet the chose
-00006770: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00006780: 2020 766f 6c75 6d65 2063 7574 6f66 6620    volume cutoff 
-00006790: 746f 2062 6520 636f 6e73 6964 6572 6564  to be considered
-000067a0: 2061 2063 6176 6974 792e 0a0a 2020 2020   a cavity...    
-000067b0: 2020 2020 2020 2020 2a20 7375 7266 6163          * surfac
-000067c0: 6520 3a20 6e75 6d70 792e 6e64 6172 7261  e : numpy.ndarra
-000067d0: 790a 0a20 2020 2020 2020 2020 2020 2020  y..             
-000067e0: 2020 2053 7572 6661 6365 2070 6f69 6e74     Surface point
-000067f0: 7320 696e 2074 6865 2033 4420 6772 6964  s in the 3D grid
-00006800: 2028 7375 7266 6163 655b 6e78 5d5b 6e79   (surface[nx][ny
-00006810: 5d5b 6e7a 5d29 2e0a 2020 2020 2020 2020  ][nz])..        
-00006820: 2020 2020 2020 2020 5375 7266 6163 6520          Surface 
-00006830: 6172 7261 7920 6861 7320 696e 7465 6765  array has intege
-00006840: 7220 6c61 6265 6c73 2069 6e20 6561 6368  r labels in each
-00006850: 2070 6f73 6974 696f 6e2c 2074 6861 7420   position, that 
-00006860: 6172 653a 0a0a 2020 2020 2020 2020 2020  are:..          
-00006870: 2020 2020 2020 2a20 2d31 3a20 6275 6c6b        * -1: bulk
-00006880: 2070 6f69 6e74 733b 0a20 2020 2020 2020   points;.       
-00006890: 2020 2020 2020 2020 202a 2030 3a20 6269           * 0: bi
-000068a0: 6f6d 6f6c 6563 756c 6520 6f72 2065 6d70  omolecule or emp
-000068b0: 7479 2073 7061 6365 2070 6f69 6e74 733b  ty space points;
-000068c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000068d0: 202a 203e 3d32 3a20 7375 7266 6163 6520   * >=2: surface 
-000068e0: 706f 696e 7473 2e0a 0a20 2020 2020 2020  points...       
-000068f0: 2020 2020 2020 2020 2054 6865 2065 6d70           The emp
-00006900: 7479 2073 7061 6365 2070 6f69 6e74 7320  ty space points 
-00006910: 6172 6520 7265 6769 6f6e 7320 7468 6174  are regions that
-00006920: 2064 6f20 6e6f 7420 6d65 6574 2074 6865   do not meet the
-00006930: 2063 686f 7365 6e0a 2020 2020 2020 2020   chosen.        
-00006940: 2020 2020 2020 2020 766f 6c75 6d65 2063          volume c
-00006950: 7574 6f66 6620 746f 2062 6520 636f 6e73  utoff to be cons
-00006960: 6964 6572 6564 2061 2063 6176 6974 792e  idered a cavity.
-00006970: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
-00006980: 6465 7074 6873 203a 206e 756d 7079 2e6e  depths : numpy.n
-00006990: 6461 7272 6179 2c20 6f70 7469 6f6e 616c  darray, optional
-000069a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000069b0: 2020 4120 6e75 6d70 792e 6e64 6172 7261    A numpy.ndarra
-000069c0: 7920 7769 7468 2064 6570 7468 206f 6620  y with depth of 
-000069d0: 6361 7669 7479 2070 6f69 6e74 7320 2864  cavity points (d
-000069e0: 6570 7468 5b6e 785d 5b6e 795d 5b6e 7a5d  epth[nx][ny][nz]
-000069f0: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
-00006a00: 2a20 7363 616c 6573 203a 206e 756d 7079  * scales : numpy
-00006a10: 2e6e 6461 7272 6179 2c20 6f70 7469 6f6e  .ndarray, option
-00006a20: 616c 0a0a 2020 2020 2020 2020 2020 2020  al..            
-00006a30: 2020 2020 4120 6e75 6d70 792e 6e64 6172      A numpy.ndar
-00006a40: 7261 7920 7769 7468 2068 7964 726f 7068  ray with hydroph
-00006a50: 6f62 6963 6974 7920 7363 616c 6520 7661  obicity scale va
-00006a60: 6c75 6520 6d61 7070 6564 2061 7420 7375  lue mapped at su
-00006a70: 7266 6163 650a 2020 2020 2020 2020 2020  rface.          
-00006a80: 2020 2020 2020 706f 696e 7473 2028 7363        points (sc
-00006a90: 616c 6573 5b6e 785d 5b6e 795d 5b6e 7a5d  ales[nx][ny][nz]
-00006aa0: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
-00006ab0: 2a20 6e63 6176 203a 2069 6e74 0a0a 2020  * ncav : int..  
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 4e75                Nu
-00006ad0: 6d62 6572 206f 6620 6361 7669 7469 6573  mber of cavities
-00006ae0: 2e0a 0a20 2020 2020 2020 2020 2020 202a  ...            *
-00006af0: 2076 6f6c 756d 6520 3a20 4469 6374 5b73   volume : Dict[s
-00006b00: 7472 2c20 666c 6f61 745d 0a0a 2020 2020  tr, float]..    
-00006b10: 2020 2020 2020 2020 2020 2020 4120 6469              A di
-00006b20: 6374 696f 6e61 7279 2077 6974 6820 766f  ctionary with vo
-00006b30: 6c75 6d65 206f 6620 6561 6368 2064 6574  lume of each det
-00006b40: 6563 7465 6420 6361 7669 7479 2e0a 0a20  ected cavity... 
-00006b50: 2020 2020 2020 2020 2020 202a 2061 7265             * are
-00006b60: 6120 3a20 4469 6374 5b73 7472 2c20 666c  a : Dict[str, fl
-00006b70: 6f61 745d 0a0a 2020 2020 2020 2020 2020  oat]..          
-00006b80: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
-00006b90: 7279 2077 6974 6820 6172 6561 206f 6620  ry with area of 
-00006ba0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
-00006bb0: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
-00006bc0: 2020 202a 206d 6178 5f64 6570 7468 203a     * max_depth :
-00006bd0: 2044 6963 745b 7374 722c 2066 6c6f 6174   Dict[str, float
-00006be0: 5d2c 206f 7074 696f 6e61 6c0a 0a20 2020  ], optional..   
-00006bf0: 2020 2020 2020 2020 2020 2020 2041 2064               A d
-00006c00: 6963 7469 6f6e 6172 7920 7769 7468 206d  ictionary with m
-00006c10: 6178 696d 756d 2064 6570 7468 206f 6620  aximum depth of 
-00006c20: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
-00006c30: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
-00006c40: 2020 202a 2061 7667 5f64 6570 7468 203a     * avg_depth :
-00006c50: 2044 6963 745b 7374 722c 2066 6c6f 6174   Dict[str, float
-00006c60: 5d2c 206f 7074 696f 6e61 6c0a 0a20 2020  ], optional..   
-00006c70: 2020 2020 2020 2020 2020 2020 2041 2064               A d
-00006c80: 6963 7469 6f6e 6172 7920 7769 7468 2061  ictionary with a
-00006c90: 7665 7261 6765 2064 6570 7468 206f 6620  verage depth of 
-00006ca0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
-00006cb0: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
-00006cc0: 2020 202a 2061 7667 5f68 7964 726f 7061     * avg_hydropa
-00006cd0: 7468 7920 3a20 4469 6374 5b73 7472 2c20  thy : Dict[str, 
-00006ce0: 666c 6f61 745d 2c20 6f70 7469 6f6e 616c  float], optional
-00006cf0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006d00: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
-00006d10: 6974 6820 6176 6572 6167 6520 6879 6472  ith average hydr
-00006d20: 6f70 6174 6879 2066 6f72 2065 6163 6820  opathy for each 
-00006d30: 6465 7465 6374 6564 2063 6176 6974 7920  detected cavity 
-00006d40: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00006d50: 2020 2020 7468 6520 7261 6e67 6520 6f66      the range of
-00006d60: 2074 6865 2068 7964 726f 7068 6f62 6963   the hydrophobic
-00006d70: 6974 7920 7363 616c 6520 286d 696e 2c20  ity scale (min, 
-00006d80: 6d61 7829 2e0a 0a20 2020 2020 2020 2020  max)...         
-00006d90: 2020 202a 2072 6573 6964 7565 733a 2044     * residues: D
-00006da0: 6963 745b 7374 722c 204c 6973 745b 4c69  ict[str, List[Li
-00006db0: 7374 5b73 7472 5d5d 5d0a 0a20 2020 2020  st[str]]]..     
-00006dc0: 2020 2020 2020 2020 2020 2041 2064 6963             A dic
-00006dd0: 7469 6f6e 6172 7920 7769 7468 2061 206c  tionary with a l
-00006de0: 6973 7420 6f66 2069 6e74 6572 6661 6365  ist of interface
-00006df0: 2072 6573 6964 7565 7320 666f 7220 6561   residues for ea
-00006e00: 6368 2064 6574 6563 7465 640a 2020 2020  ch detected.    
-00006e10: 2020 2020 2020 2020 2020 2020 6361 7669              cavi
-00006e20: 7479 2e0a 0a20 2020 2020 2020 2020 2020  ty...           
-00006e30: 202a 2066 7265 7175 656e 6369 6573 203a   * frequencies :
-00006e40: 2044 6963 745b 7374 722c 2044 6963 745b   Dict[str, Dict[
-00006e50: 7374 722c 2044 6963 745b 7374 722c 2069  str, Dict[str, i
-00006e60: 6e74 5d5d 5d2c 206f 7074 696f 6e61 6c0a  nt]]], optional.
-00006e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006e80: 2041 2064 6963 7469 6f6e 6172 7920 7769   A dictionary wi
-00006e90: 7468 2066 7265 7175 656e 6369 6573 206f  th frequencies o
-00006ea0: 6620 7265 7369 6475 6573 2061 6e64 2063  f residues and c
-00006eb0: 6c61 7373 2066 6f72 0a20 2020 2020 2020  lass for.       
-00006ec0: 2020 2020 2020 2020 2072 6573 6964 7565           residue
-00006ed0: 7320 6f66 2065 6163 6820 6465 7465 6374  s of each detect
-00006ee0: 6564 2063 6176 6974 792e 0a0a 2020 2020  ed cavity...    
-00006ef0: 2020 2020 2020 2020 2a20 5f76 6572 7469          * _verti
-00006f00: 6365 7320 3a20 6e75 6d70 792e 6e64 6172  ces : numpy.ndar
-00006f10: 7261 790a 0a20 2020 2020 2020 2020 2020  ray..           
-00006f20: 2020 2020 2041 206e 756d 7079 2e6e 6461       A numpy.nda
-00006f30: 7272 6179 206f 7220 6120 6c69 7374 2077  rray or a list w
-00006f40: 6974 6820 7879 7a20 7665 7274 6963 6573  ith xyz vertices
-00006f50: 2063 6f6f 7264 696e 6174 6573 2028 6f72   coordinates (or
-00006f60: 6967 696e 2c0a 2020 2020 2020 2020 2020  igin,.          
-00006f70: 2020 2020 2020 582d 6178 6973 2c20 592d        X-axis, Y-
-00006f80: 6178 6973 2c20 5a2d 6178 6973 292e 0a0a  axis, Z-axis)...
-00006f90: 2020 2020 2020 2020 2020 2020 2a20 5f73              * _s
-00006fa0: 7465 7020 3a20 666c 6f61 740a 0a20 2020  tep : float..   
-00006fb0: 2020 2020 2020 2020 2020 2020 2047 7269               Gri
-00006fc0: 6420 7370 6163 696e 6720 2841 292e 0a0a  d spacing (A)...
-00006fd0: 2020 2020 2020 2020 2020 2020 2a20 5f69              * _i
-00006fe0: 6e70 7574 203a 2055 6e69 6f6e 5b73 7472  nput : Union[str
-00006ff0: 2c20 7061 7468 6c69 622e 5061 7468 5d2c  , pathlib.Path],
-00007000: 206f 7074 696f 6e61 6c0a 0a20 2020 2020   optional..     
-00007010: 2020 2020 2020 2020 2020 2041 2070 6174             A pat
-00007020: 6820 746f 2069 6e70 7574 2050 4442 206f  h to input PDB o
-00007030: 7220 5859 5a20 6669 6c65 2e0a 0a20 2020  r XYZ file...   
-00007040: 2020 2020 2020 2020 202a 205f 6c69 6761           * _liga
-00007050: 6e64 203a 2055 6e69 6f6e 5b73 7472 2c20  nd : Union[str, 
-00007060: 7061 7468 6c69 622e 5061 7468 5d2c 206f  pathlib.Path], o
-00007070: 7074 696f 6e61 6c0a 0a20 2020 2020 2020  ptional..       
-00007080: 2020 2020 2020 2020 2041 2070 6174 6820           A path 
-00007090: 746f 206c 6967 616e 6420 5044 4220 6f72  to ligand PDB or
-000070a0: 2058 595a 2066 696c 652e 0a0a 2020 2020   XYZ file...    
-000070b0: 5261 6973 6573 0a20 2020 202d 2d2d 2d2d  Raises.    -----
-000070c0: 2d0a 2020 2020 5479 7065 4572 726f 720a  -.    TypeError.
-000070d0: 2020 2020 2020 2020 6069 6e70 7574 6020          `input` 
-000070e0: 6d75 7374 2068 6176 6520 2e70 6462 206f  must have .pdb o
-000070f0: 7220 2e78 797a 2065 7874 656e 7369 6f6e  r .xyz extension
-00007100: 2e0a 2020 2020 5479 7065 4572 726f 720a  ..    TypeError.
-00007110: 2020 2020 2020 2020 606c 6967 616e 6460          `ligand`
-00007120: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
-00007130: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
-00007140: 6e2e 0a0a 2020 2020 4e6f 7465 0a20 2020  n...    Note.   
-00007150: 202d 2d2d 2d0a 2020 2020 5468 6520 6361   ----.    The ca
-00007160: 7669 7479 206e 6f6d 656e 636c 6174 7572  vity nomenclatur
-00007170: 6520 6973 2062 6173 6564 206f 6e20 7468  e is based on th
-00007180: 6520 696e 7465 6765 7220 6c61 6265 6c2e  e integer label.
-00007190: 2054 6865 2063 6176 6974 7920 6d61 726b   The cavity mark
-000071a0: 6564 0a20 2020 2077 6974 6820 322c 2074  ed.    with 2, t
-000071b0: 6865 2066 6972 7374 2069 6e74 6567 6572  he first integer
-000071c0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
-000071d0: 6f20 6120 6361 7669 7479 2c20 6973 204b  o a cavity, is K
-000071e0: 4141 2c20 7468 6520 6361 7669 7479 0a20  AA, the cavity. 
-000071f0: 2020 206d 6172 6b65 6420 7769 7468 2033     marked with 3
-00007200: 2069 7320 4b41 422c 2074 6865 2063 6176   is KAB, the cav
-00007210: 6974 7920 6d61 726b 6564 2077 6974 6820  ity marked with 
-00007220: 3420 6973 204b 4143 2061 6e64 2073 6f20  4 is KAC and so 
-00007230: 6f6e 2e0a 0a20 2020 204e 6f74 650a 2020  on...    Note.  
-00007240: 2020 2d2d 2d2d 0a20 2020 2054 6865 2063    ----.    The c
-00007250: 6c61 7373 6573 206f 6620 7265 7369 6475  lasses of residu
-00007260: 6573 2061 7265 3a0a 0a20 2020 202a 2041  es are:..    * A
-00007270: 6c69 7068 6174 6963 2061 706f 6c61 7220  liphatic apolar 
-00007280: 2852 3129 3a20 416c 616e 696e 652c 2047  (R1): Alanine, G
-00007290: 6c79 6369 6e65 2c20 4973 6f6c 6575 6369  lycine, Isoleuci
-000072a0: 6e65 2c20 4c65 7563 696e 652c 204d 6574  ne, Leucine, Met
-000072b0: 6869 6f6e 696e 652c 2056 616c 696e 652e  hionine, Valine.
-000072c0: 0a0a 2020 2020 2a20 4172 6f6d 6174 6963  ..    * Aromatic
-000072d0: 2028 5232 293a 2050 6865 6e79 6c61 6c61   (R2): Phenylala
-000072e0: 6e69 6e65 2c20 5472 7970 746f 7068 616e  nine, Tryptophan
-000072f0: 2c20 5479 726f 7369 6e65 2e0a 0a20 2020  , Tyrosine...   
-00007300: 202a 2050 6f6c 6172 2055 6e63 6861 7267   * Polar Uncharg
-00007310: 6564 2028 5233 293a 2041 7370 6172 6167  ed (R3): Asparag
-00007320: 696e 652c 2043 7973 7465 696e 652c 2047  ine, Cysteine, G
-00007330: 6c75 7461 6d69 6e65 2c20 5072 6f6c 696e  lutamine, Prolin
-00007340: 652c 2053 6572 696e 652c 2054 6872 656f  e, Serine, Threo
-00007350: 6e69 6e65 2e0a 0a20 2020 202a 204e 6567  nine...    * Neg
-00007360: 6174 6976 656c 7920 6368 6172 6765 6420  atively charged 
-00007370: 2852 3429 3a20 4173 7061 7274 6174 652c  (R4): Aspartate,
-00007380: 2047 6c75 7461 6d61 7465 2e0a 0a20 2020   Glutamate...   
-00007390: 202a 2050 6f73 6974 6976 656c 7920 6368   * Positively ch
-000073a0: 6172 6765 6420 2852 3529 3a20 4172 6769  arged (R5): Argi
-000073b0: 6e69 6e65 2c20 4869 7374 6964 696e 652c  nine, Histidine,
-000073c0: 204c 7973 696e 652e 0a0a 2020 2020 2a20   Lysine...    * 
-000073d0: 4e6f 6e2d 7374 616e 6461 7264 2028 5258  Non-standard (RX
-000073e0: 293a 204e 6f6e 2d73 7461 6e64 6172 6420  ): Non-standard 
-000073f0: 7265 7369 6475 6573 2e0a 0a20 2020 2053  residues...    S
-00007400: 6565 2041 6c73 6f0a 2020 2020 2d2d 2d2d  ee Also.    ----
-00007410: 2d2d 2d2d 0a20 2020 2070 794b 5646 696e  ----.    pyKVFin
-00007420: 6465 7252 6573 756c 7473 0a0a 2020 2020  derResults..    
-00007430: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
-00007440: 2d2d 2d0a 2020 2020 5468 6520 2a2a 7374  ---.    The **st
-00007450: 616e 6461 7264 2077 6f72 6b66 6c6f 772a  andard workflow*
-00007460: 2a20 666f 7220 6361 7669 7479 2064 6574  * for cavity det
-00007470: 6563 7469 6f6e 2077 6974 6820 7370 6174  ection with spat
-00007480: 6961 6c20 2873 7572 6661 6365 2070 6f69  ial (surface poi
-00007490: 6e74 732c 2076 6f6c 756d 652c 2061 7265  nts, volume, are
-000074a0: 6129 2061 6e64 2063 6f6e 7374 6974 7574  a) and constitut
-000074b0: 696f 6e61 6c20 2869 6e74 6572 6661 6365  ional (interface
-000074c0: 2072 6573 6964 7565 7320 616e 6420 7468   residues and th
-000074d0: 6569 7220 6672 6571 7565 6e63 6965 7329  eir frequencies)
-000074e0: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
-000074f0: 6e20 2063 616e 2062 6520 7275 6e20 6174  n  can be run at
-00007500: 206f 6e63 6520 7769 7468 206f 6e65 2063   once with one c
-00007510: 6f6d 6d61 6e64 3a0a 0a20 2020 203e 3e3e  ommand:..    >>>
-00007520: 2069 6d70 6f72 7420 6f73 0a20 2020 203e   import os.    >
-00007530: 3e3e 2069 6d70 6f72 7420 7079 4b56 4669  >> import pyKVFi
-00007540: 6e64 6572 0a20 2020 203e 3e3e 2070 6462  nder.    >>> pdb
-00007550: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00007560: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00007570: 7079 4b56 4669 6e64 6572 2e5f 5f66 696c  pyKVFinder.__fil
-00007580: 655f 5f29 2c20 2764 6174 6127 2c20 2774  e__), 'data', 't
-00007590: 6573 7473 272c 2027 3146 4d4f 2e70 6462  ests', '1FMO.pdb
-000075a0: 2729 0a20 2020 203e 3e3e 2072 6573 756c  ').    >>> resul
-000075b0: 7473 203d 2070 794b 5646 696e 6465 722e  ts = pyKVFinder.
-000075c0: 7275 6e5f 776f 726b 666c 6f77 2870 6462  run_workflow(pdb
-000075d0: 290a 2020 2020 3e3e 3e20 7265 7375 6c74  ).    >>> result
-000075e0: 730a 2020 2020 3c70 794b 5646 696e 6465  s.    <pyKVFinde
-000075f0: 7252 6573 756c 7473 206f 626a 6563 743e  rResults object>
-00007600: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
-00007610: 2e63 6176 6974 6965 730a 2020 2020 6172  .cavities.    ar
-00007620: 7261 7928 5b5b 5b2d 312c 202d 312c 202d  ray([[[-1, -1, -
-00007630: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00007640: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00007650: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-00007660: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00007670: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00007680: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00007690: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
-000076a0: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-000076b0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-000076c0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-000076d0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-000076e0: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-000076f0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-00007700: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-00007710: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-00007720: 2d31 2c20 2d31 2c20 2d31 5d5d 2c0a 2020  -1, -1, -1]],.  
-00007730: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-00007740: 2020 2020 2020 2020 205b 5b2d 312c 202d           [[-1, -
-00007750: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00007760: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00007770: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
-00007780: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-00007790: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-000077a0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-000077b0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-000077c0: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
-000077d0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-000077e0: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-000077f0: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
-00007800: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
-00007810: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
-00007820: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
-00007830: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-00007840: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d5d  .., -1, -1, -1]]
-00007850: 5d2c 2064 7479 7065 3d69 6e74 3332 290a  ], dtype=int32).
-00007860: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-00007870: 7375 7266 6163 650a 2020 2020 6172 7261  surface.    arra
-00007880: 7928 5b5b 5b2d 312c 202d 312c 202d 312c  y([[[-1, -1, -1,
-00007890: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-000078a0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-000078b0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-000078c0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-000078d0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-000078e0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-000078f0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00007900: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-00007910: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-00007920: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00007930: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00007940: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-00007950: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00007960: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00007970: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00007980: 2c20 2d31 2c20 2d31 5d5d 2c0a 2020 2020  , -1, -1]],.    
-00007990: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-000079a0: 2020 2020 2020 205b 5b2d 312c 202d 312c         [[-1, -1,
-000079b0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-000079c0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-000079d0: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-000079e0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-000079f0: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-00007a00: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-00007a10: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
-00007a20: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-00007a30: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00007a40: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00007a50: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00007a60: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
-00007a70: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-00007a80: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-00007a90: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-00007aa0: 2c20 2d31 2c20 2d31 2c20 2d31 5d5d 5d2c  , -1, -1, -1]]],
-00007ab0: 2064 7479 7065 3d69 6e74 3332 290a 2020   dtype=int32).  
-00007ac0: 2020 3e3e 3e20 7265 7375 6c74 732e 6e63    >>> results.nc
-00007ad0: 6176 0a20 2020 203e 3e3e 2031 380a 2020  av.    >>> 18.  
-00007ae0: 2020 3e3e 3e20 7265 7375 6c74 732e 766f    >>> results.vo
-00007af0: 6c75 6d65 0a20 2020 207b 274b 4141 273a  lume.    {'KAA':
-00007b00: 2031 3337 2e31 362c 2027 4b41 4227 3a20   137.16, 'KAB': 
-00007b10: 3437 2e35 322c 2027 4b41 4327 3a20 3636  47.52, 'KAC': 66
-00007b20: 2e39 362c 2027 4b41 4427 3a20 382e 3231  .96, 'KAD': 8.21
-00007b30: 2c20 274b 4145 273a 2034 332e 3633 2c20  , 'KAE': 43.63, 
-00007b40: 274b 4146 273a 2031 322e 3533 2c20 274b  'KAF': 12.53, 'K
-00007b50: 4147 273a 2036 2e32 362c 2027 4b41 4827  AG': 6.26, 'KAH'
-00007b60: 3a20 3532 302e 3133 2c20 274b 4149 273a  : 520.13, 'KAI':
-00007b70: 2031 322e 3331 2c20 274b 414a 273a 2032   12.31, 'KAJ': 2
-00007b80: 362e 3537 2c20 274b 414b 273a 2031 322e  6.57, 'KAK': 12.
-00007b90: 3331 2c20 274b 414c 273a 2033 332e 3931  31, 'KAL': 33.91
-00007ba0: 2c20 274b 414d 273a 2032 332e 3131 2c20  , 'KAM': 23.11, 
-00007bb0: 274b 414e 273a 2031 3032 2e38 322c 2027  'KAN': 102.82, '
-00007bc0: 4b41 4f27 3a20 362e 3035 2c20 274b 4150  KAO': 6.05, 'KAP
-00007bd0: 273a 2031 352e 3535 2c20 274b 4151 273a  ': 15.55, 'KAQ':
-00007be0: 2037 2e39 392c 2027 4b41 5227 3a20 372e   7.99, 'KAR': 7.
-00007bf0: 3738 7d0a 2020 2020 3e3e 3e20 7265 7375  78}.    >>> resu
-00007c00: 6c74 732e 6172 6561 0a20 2020 207b 274b  lts.area.    {'K
-00007c10: 4141 273a 2031 3236 2e34 312c 2027 4b41  AA': 126.41, 'KA
-00007c20: 4227 3a20 3632 2e33 372c 2027 4b41 4327  B': 62.37, 'KAC'
-00007c30: 3a20 3734 2e35 372c 2027 4b41 4427 3a20  : 74.57, 'KAD': 
-00007c40: 3139 2e30 362c 2027 4b41 4527 3a20 3537  19.06, 'KAE': 57
-00007c50: 2e30 382c 2027 4b41 4627 3a20 3232 2e37  .08, 'KAF': 22.7
-00007c60: 372c 2027 4b41 4727 3a20 3135 2e33 382c  7, 'KAG': 15.38,
-00007c70: 2027 4b41 4827 3a20 3439 362e 3937 2c20   'KAH': 496.97, 
-00007c80: 274b 4149 273a 2033 302e 3538 2c20 274b  'KAI': 30.58, 'K
-00007c90: 414a 273a 2034 352e 3634 2c20 274b 414b  AJ': 45.64, 'KAK
-00007ca0: 273a 2033 302e 3538 2c20 274b 414c 273a  ': 30.58, 'KAL':
-00007cb0: 2034 352e 3538 2c20 274b 414d 273a 2034   45.58, 'KAM': 4
-00007cc0: 352e 3235 2c20 274b 414e 273a 2031 3239  5.25, 'KAN': 129
-00007cd0: 2e37 372c 2027 4b41 4f27 3a20 3132 2e32  .77, 'KAO': 12.2
-00007ce0: 382c 2027 4b41 5027 3a20 3235 2e30 342c  8, 'KAP': 25.04,
-00007cf0: 2027 4b41 5127 3a20 3133 2e34 362c 2027   'KAQ': 13.46, '
-00007d00: 4b41 5227 3a20 3136 2e36 7d0a 2020 2020  KAR': 16.6}.    
-00007d10: 3e3e 3e20 7265 7375 6c74 732e 7265 7369  >>> results.resi
-00007d20: 6475 6573 0a20 2020 207b 274b 4141 273a  dues.    {'KAA':
-00007d30: 205b 5b27 3134 272c 2027 4527 2c20 2753   [['14', 'E', 'S
-00007d40: 4552 275d 2c20 5b27 3135 272c 2027 4527  ER'], ['15', 'E'
-00007d50: 2c20 2756 414c 275d 2c20 5b27 3138 272c  , 'VAL'], ['18',
-00007d60: 2027 4527 2c20 2750 4845 275d 2c20 5b27   'E', 'PHE'], ['
-00007d70: 3139 272c 2027 4527 2c20 274c 4555 275d  19', 'E', 'LEU']
-00007d80: 2c20 5b27 3130 3027 2c20 2745 272c 2027  , ['100', 'E', '
-00007d90: 5048 4527 5d2c 205b 2731 3532 272c 2027  PHE'], ['152', '
-00007da0: 4527 2c20 274c 4555 275d 2c20 5b27 3135  E', 'LEU'], ['15
-00007db0: 3527 2c20 2745 272c 2027 474c 5527 5d2c  5', 'E', 'GLU'],
-00007dc0: 205b 2731 3536 272c 2027 4527 2c20 2754   ['156', 'E', 'T
-00007dd0: 5952 275d 2c20 5b27 3239 3227 2c20 2745  YR'], ['292', 'E
-00007de0: 272c 2027 4c59 5327 5d2c 205b 2733 3032  ', 'LYS'], ['302
-00007df0: 272c 2027 4527 2c20 2754 5250 275d 2c20  ', 'E', 'TRP'], 
-00007e00: 5b27 3330 3327 2c20 2745 272c 2027 494c  ['303', 'E', 'IL
-00007e10: 4527 5d2c 205b 2733 3036 272c 2027 4527  E'], ['306', 'E'
-00007e20: 2c20 2754 5952 275d 5d2c 2027 4b41 4227  , 'TYR']], 'KAB'
-00007e30: 3a20 5b5b 2731 3827 2c20 2745 272c 2027  : [['18', 'E', '
-00007e40: 5048 4527 5d2c 205b 2732 3227 2c20 2745  PHE'], ['22', 'E
-00007e50: 272c 2027 414c 4127 5d2c 205b 2732 3527  ', 'ALA'], ['25'
-00007e60: 2c20 2745 272c 2027 4153 5027 5d2c 205b  , 'E', 'ASP'], [
-00007e70: 2732 3627 2c20 2745 272c 2027 5048 4527  '26', 'E', 'PHE'
-00007e80: 5d2c 205b 2732 3927 2c20 2745 272c 2027  ], ['29', 'E', '
-00007e90: 4c59 5327 5d2c 205b 2739 3727 2c20 2745  LYS'], ['97', 'E
-00007ea0: 272c 2027 414c 4127 5d2c 205b 2739 3827  ', 'ALA'], ['98'
-00007eb0: 2c20 2745 272c 2027 5641 4c27 5d2c 205b  , 'E', 'VAL'], [
-00007ec0: 2739 3927 2c20 2745 272c 2027 4153 4e27  '99', 'E', 'ASN'
-00007ed0: 5d2c 205b 2731 3536 272c 2027 4527 2c20  ], ['156', 'E', 
-00007ee0: 2754 5952 275d 5d2c 2027 4b41 4327 3a20  'TYR']], 'KAC': 
-00007ef0: 5b5b 2731 3431 272c 2027 4527 2c20 2750  [['141', 'E', 'P
-00007f00: 524f 275d 2c20 5b27 3134 3227 2c20 2745  RO'], ['142', 'E
-00007f10: 272c 2027 4849 5327 5d2c 205b 2731 3434  ', 'HIS'], ['144
-00007f20: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
-00007f30: 5b27 3134 3527 2c20 2745 272c 2027 5048  ['145', 'E', 'PH
-00007f40: 4527 5d2c 205b 2731 3438 272c 2027 4527  E'], ['148', 'E'
-00007f50: 2c20 2741 4c41 275d 2c20 5b27 3239 3927  , 'ALA'], ['299'
-00007f60: 2c20 2745 272c 2027 5448 5227 5d2c 205b  , 'E', 'THR'], [
-00007f70: 2733 3030 272c 2027 4527 2c20 2754 4852  '300', 'E', 'THR
-00007f80: 275d 2c20 5b27 3330 3527 2c20 2745 272c  '], ['305', 'E',
-00007f90: 2027 494c 4527 5d2c 205b 2733 3130 272c   'ILE'], ['310',
-00007fa0: 2027 4527 2c20 2756 414c 275d 2c20 5b27   'E', 'VAL'], ['
-00007fb0: 3331 3127 2c20 2745 272c 2027 474c 5527  311', 'E', 'GLU'
-00007fc0: 5d2c 205b 2733 3133 272c 2027 4527 2c20  ], ['313', 'E', 
-00007fd0: 2750 524f 275d 5d2c 2027 4b41 4427 3a20  'PRO']], 'KAD': 
-00007fe0: 5b5b 2731 3232 272c 2027 4527 2c20 2754  [['122', 'E', 'T
-00007ff0: 5952 275d 2c20 5b27 3132 3427 2c20 2745  YR'], ['124', 'E
-00008000: 272c 2027 414c 4127 5d2c 205b 2731 3736  ', 'ALA'], ['176
-00008010: 272c 2027 4527 2c20 2747 4c4e 275d 2c20  ', 'E', 'GLN'], 
-00008020: 5b27 3331 3827 2c20 2745 272c 2027 5048  ['318', 'E', 'PH
-00008030: 4527 5d2c 205b 2733 3230 272c 2027 4527  E'], ['320', 'E'
-00008040: 2c20 2747 4c59 275d 2c20 5b27 3332 3127  , 'GLY'], ['321'
-00008050: 2c20 2745 272c 2027 5052 4f27 5d2c 205b  , 'E', 'PRO'], [
-00008060: 2733 3232 272c 2027 4527 2c20 2747 4c59  '322', 'E', 'GLY
-00008070: 275d 2c20 5b27 3332 3327 2c20 2745 272c  '], ['323', 'E',
-00008080: 2027 4153 5027 5d5d 2c20 274b 4145 273a   'ASP']], 'KAE':
-00008090: 205b 5b27 3935 272c 2027 4527 2c20 274c   [['95', 'E', 'L
-000080a0: 4555 275d 2c20 5b27 3938 272c 2027 4527  EU'], ['98', 'E'
-000080b0: 2c20 2756 414c 275d 2c20 5b27 3939 272c  , 'VAL'], ['99',
-000080c0: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
-000080d0: 3130 3027 2c20 2745 272c 2027 5048 4527  100', 'E', 'PHE'
-000080e0: 5d2c 205b 2731 3033 272c 2027 4527 2c20  ], ['103', 'E', 
-000080f0: 274c 4555 275d 2c20 5b27 3130 3427 2c20  'LEU'], ['104', 
-00008100: 2745 272c 2027 5641 4c27 5d2c 205b 2731  'E', 'VAL'], ['1
-00008110: 3035 272c 2027 4527 2c20 274c 5953 275d  05', 'E', 'LYS']
-00008120: 2c20 5b27 3130 3627 2c20 2745 272c 2027  , ['106', 'E', '
-00008130: 4c45 5527 5d5d 2c20 274b 4146 273a 205b  LEU']], 'KAF': [
-00008140: 5b27 3132 3327 2c20 2745 272c 2027 5641  ['123', 'E', 'VA
-00008150: 4c27 5d2c 205b 2731 3234 272c 2027 4527  L'], ['124', 'E'
-00008160: 2c20 2741 4c41 275d 2c20 5b27 3137 3527  , 'ALA'], ['175'
-00008170: 2c20 2745 272c 2027 4153 5027 5d2c 205b  , 'E', 'ASP'], [
-00008180: 2731 3736 272c 2027 4527 2c20 2747 4c4e  '176', 'E', 'GLN
-00008190: 275d 2c20 5b27 3138 3127 2c20 2745 272c  '], ['181', 'E',
-000081a0: 2027 474c 4e27 5d5d 2c20 274b 4147 273a   'GLN']], 'KAG':
-000081b0: 205b 5b27 3334 272c 2027 4527 2c20 2753   [['34', 'E', 'S
-000081c0: 4552 275d 2c20 5b27 3337 272c 2027 4527  ER'], ['37', 'E'
-000081d0: 2c20 2754 4852 275d 2c20 5b27 3936 272c  , 'THR'], ['96',
-000081e0: 2027 4527 2c20 2747 4c4e 275d 2c20 5b27   'E', 'GLN'], ['
-000081f0: 3130 3627 2c20 2745 272c 2027 4c45 5527  106', 'E', 'LEU'
-00008200: 5d2c 205b 2731 3037 272c 2027 4527 2c20  ], ['107', 'E', 
-00008210: 2747 4c55 275d 2c20 5b27 3130 3827 2c20  'GLU'], ['108', 
-00008220: 2745 272c 2027 5048 4527 5d2c 205b 2731  'E', 'PHE'], ['1
-00008230: 3039 272c 2027 4527 2c20 2753 4552 275d  09', 'E', 'SER']
-00008240: 5d2c 2027 4b41 4827 3a20 5b5b 2734 3927  ], 'KAH': [['49'
-00008250: 2c20 2745 272c 2027 4c45 5527 5d2c 205b  , 'E', 'LEU'], [
-00008260: 2735 3027 2c20 2745 272c 2027 474c 5927  '50', 'E', 'GLY'
-00008270: 5d2c 205b 2735 3127 2c20 2745 272c 2027  ], ['51', 'E', '
-00008280: 5448 5227 5d2c 205b 2735 3227 2c20 2745  THR'], ['52', 'E
-00008290: 272c 2027 474c 5927 5d2c 205b 2735 3327  ', 'GLY'], ['53'
-000082a0: 2c20 2745 272c 2027 5345 5227 5d2c 205b  , 'E', 'SER'], [
-000082b0: 2735 3427 2c20 2745 272c 2027 5048 4527  '54', 'E', 'PHE'
-000082c0: 5d2c 205b 2735 3527 2c20 2745 272c 2027  ], ['55', 'E', '
-000082d0: 474c 5927 5d2c 205b 2735 3627 2c20 2745  GLY'], ['56', 'E
-000082e0: 272c 2027 4152 4727 5d2c 205b 2735 3727  ', 'ARG'], ['57'
-000082f0: 2c20 2745 272c 2027 5641 4c27 5d2c 205b  , 'E', 'VAL'], [
-00008300: 2737 3027 2c20 2745 272c 2027 414c 4127  '70', 'E', 'ALA'
-00008310: 5d2c 205b 2737 3227 2c20 2745 272c 2027  ], ['72', 'E', '
-00008320: 4c59 5327 5d2c 205b 2737 3427 2c20 2745  LYS'], ['74', 'E
-00008330: 272c 2027 4c45 5527 5d2c 205b 2738 3427  ', 'LEU'], ['84'
-00008340: 2c20 2745 272c 2027 474c 4e27 5d2c 205b  , 'E', 'GLN'], [
-00008350: 2738 3727 2c20 2745 272c 2027 4849 5327  '87', 'E', 'HIS'
-00008360: 5d2c 205b 2738 3827 2c20 2745 272c 2027  ], ['88', 'E', '
-00008370: 5448 5227 5d2c 205b 2739 3127 2c20 2745  THR'], ['91', 'E
-00008380: 272c 2027 474c 5527 5d2c 205b 2731 3034  ', 'GLU'], ['104
-00008390: 272c 2027 4527 2c20 2756 414c 275d 2c20  ', 'E', 'VAL'], 
-000083a0: 5b27 3132 3027 2c20 2745 272c 2027 4d45  ['120', 'E', 'ME
-000083b0: 5427 5d2c 205b 2731 3231 272c 2027 4527  T'], ['121', 'E'
-000083c0: 2c20 2747 4c55 275d 2c20 5b27 3132 3227  , 'GLU'], ['122'
-000083d0: 2c20 2745 272c 2027 5459 5227 5d2c 205b  , 'E', 'TYR'], [
-000083e0: 2731 3233 272c 2027 4527 2c20 2756 414c  '123', 'E', 'VAL
-000083f0: 275d 2c20 5b27 3132 3727 2c20 2745 272c  '], ['127', 'E',
-00008400: 2027 474c 5527 5d2c 205b 2731 3636 272c   'GLU'], ['166',
-00008410: 2027 4527 2c20 2741 5350 275d 2c20 5b27   'E', 'ASP'], ['
-00008420: 3136 3827 2c20 2745 272c 2027 4c59 5327  168', 'E', 'LYS'
-00008430: 5d2c 205b 2731 3730 272c 2027 4527 2c20  ], ['170', 'E', 
-00008440: 2747 4c55 275d 2c20 5b27 3137 3127 2c20  'GLU'], ['171', 
-00008450: 2745 272c 2027 4153 4e27 5d2c 205b 2731  'E', 'ASN'], ['1
-00008460: 3733 272c 2027 4527 2c20 274c 4555 275d  73', 'E', 'LEU']
-00008470: 2c20 5b27 3138 3327 2c20 2745 272c 2027  , ['183', 'E', '
-00008480: 5448 5227 5d2c 205b 2731 3834 272c 2027  THR'], ['184', '
-00008490: 4527 2c20 2741 5350 275d 2c20 5b27 3138  E', 'ASP'], ['18
-000084a0: 3627 2c20 2745 272c 2027 474c 5927 5d2c  6', 'E', 'GLY'],
-000084b0: 205b 2731 3837 272c 2027 4527 2c20 2750   ['187', 'E', 'P
-000084c0: 4845 275d 2c20 5b27 3230 3127 2c20 2745  HE'], ['201', 'E
-000084d0: 272c 2027 5448 5227 5d2c 205b 2733 3237  ', 'THR'], ['327
-000084e0: 272c 2027 4527 2c20 2750 4845 275d 5d2c  ', 'E', 'PHE']],
-000084f0: 2027 4b41 4927 3a20 5b5b 2731 3331 272c   'KAI': [['131',
-00008500: 2027 4527 2c20 2748 4953 275d 2c20 5b27   'E', 'HIS'], ['
-00008510: 3133 3827 2c20 2745 272c 2027 5048 4527  138', 'E', 'PHE'
-00008520: 5d2c 205b 2731 3432 272c 2027 4527 2c20  ], ['142', 'E', 
-00008530: 2748 4953 275d 2c20 5b27 3134 3627 2c20  'HIS'], ['146', 
-00008540: 2745 272c 2027 5459 5227 5d2c 205b 2731  'E', 'TYR'], ['1
-00008550: 3734 272c 2027 4527 2c20 2749 4c45 275d  74', 'E', 'ILE']
-00008560: 2c20 5b27 3331 3427 2c20 2745 272c 2027  , ['314', 'E', '
-00008570: 5048 4527 5d5d 2c20 274b 414a 273a 205b  PHE']], 'KAJ': [
-00008580: 5b27 3333 272c 2027 4527 2c20 2750 524f  ['33', 'E', 'PRO
-00008590: 275d 2c20 5b27 3839 272c 2027 4527 2c20  '], ['89', 'E', 
-000085a0: 274c 4555 275d 2c20 5b27 3932 272c 2027  'LEU'], ['92', '
-000085b0: 4527 2c20 274c 5953 275d 2c20 5b27 3933  E', 'LYS'], ['93
-000085c0: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
-000085d0: 5b27 3936 272c 2027 4527 2c20 2747 4c4e  ['96', 'E', 'GLN
-000085e0: 275d 2c20 5b27 3334 3927 2c20 2745 272c  '], ['349', 'E',
-000085f0: 2027 474c 5527 5d2c 205b 2733 3530 272c   'GLU'], ['350',
-00008600: 2027 4527 2c20 2750 4845 275d 5d2c 2027   'E', 'PHE']], '
-00008610: 4b41 4b27 3a20 5b5b 2731 3537 272c 2027  KAK': [['157', '
-00008620: 4527 2c20 274c 4555 275d 2c20 5b27 3136  E', 'LEU'], ['16
-00008630: 3227 2c20 2745 272c 2027 4c45 5527 5d2c  2', 'E', 'LEU'],
-00008640: 205b 2731 3633 272c 2027 4527 2c20 2749   ['163', 'E', 'I
-00008650: 4c45 275d 2c20 5b27 3136 3427 2c20 2745  LE'], ['164', 'E
-00008660: 272c 2027 5459 5227 5d2c 205b 2731 3835  ', 'TYR'], ['185
-00008670: 272c 2027 4527 2c20 2750 4845 275d 2c20  ', 'E', 'PHE'], 
-00008680: 5b27 3138 3827 2c20 2745 272c 2027 414c  ['188', 'E', 'AL
-00008690: 4127 5d5d 2c20 274b 414c 273a 205b 5b27  A']], 'KAL': [['
-000086a0: 3439 272c 2027 4527 2c20 274c 4555 275d  49', 'E', 'LEU']
-000086b0: 2c20 5b27 3132 3727 2c20 2745 272c 2027  , ['127', 'E', '
-000086c0: 474c 5527 5d2c 205b 2731 3239 272c 2027  GLU'], ['129', '
-000086d0: 4527 2c20 2750 4845 275d 2c20 5b27 3133  E', 'PHE'], ['13
-000086e0: 3027 2c20 2745 272c 2027 5345 5227 5d2c  0', 'E', 'SER'],
-000086f0: 205b 2733 3236 272c 2027 4527 2c20 2741   ['326', 'E', 'A
-00008700: 534e 275d 2c20 5b27 3332 3727 2c20 2745  SN'], ['327', 'E
-00008710: 272c 2027 5048 4527 5d2c 205b 2733 3238  ', 'PHE'], ['328
-00008720: 272c 2027 4527 2c20 2741 5350 275d 2c20  ', 'E', 'ASP'], 
-00008730: 5b27 3333 3027 2c20 2745 272c 2027 5459  ['330', 'E', 'TY
-00008740: 5227 5d5d 2c20 274b 414d 273a 205b 5b27  R']], 'KAM': [['
-00008750: 3531 272c 2027 4527 2c20 2754 4852 275d  51', 'E', 'THR']
-00008760: 2c20 5b27 3535 272c 2027 4527 2c20 2747  , ['55', 'E', 'G
-00008770: 4c59 275d 2c20 5b27 3536 272c 2027 4527  LY'], ['56', 'E'
-00008780: 2c20 2741 5247 275d 2c20 5b27 3733 272c  , 'ARG'], ['73',
-00008790: 2027 4527 2c20 2749 4c45 275d 2c20 5b27   'E', 'ILE'], ['
-000087a0: 3734 272c 2027 4527 2c20 274c 4555 275d  74', 'E', 'LEU']
-000087b0: 2c20 5b27 3735 272c 2027 4527 2c20 2741  , ['75', 'E', 'A
-000087c0: 5350 275d 2c20 5b27 3131 3527 2c20 2745  SP'], ['115', 'E
-000087d0: 272c 2027 4153 4e27 5d2c 205b 2733 3335  ', 'ASN'], ['335
-000087e0: 272c 2027 4527 2c20 2749 4c45 275d 2c20  ', 'E', 'ILE'], 
-000087f0: 5b27 3333 3627 2c20 2745 272c 2027 4152  ['336', 'E', 'AR
-00008800: 4727 5d5d 2c20 274b 414e 273a 205b 5b27  G']], 'KAN': [['
-00008810: 3136 3527 2c20 2745 272c 2027 4152 4727  165', 'E', 'ARG'
-00008820: 5d2c 205b 2731 3636 272c 2027 4527 2c20  ], ['166', 'E', 
-00008830: 2741 5350 275d 2c20 5b27 3136 3727 2c20  'ASP'], ['167', 
-00008840: 2745 272c 2027 4c45 5527 5d2c 205b 2731  'E', 'LEU'], ['1
-00008850: 3939 272c 2027 4527 2c20 2743 5953 275d  99', 'E', 'CYS']
-00008860: 2c20 5b27 3230 3027 2c20 2745 272c 2027  , ['200', 'E', '
-00008870: 474c 5927 5d2c 205b 2732 3031 272c 2027  GLY'], ['201', '
-00008880: 4527 2c20 2754 4852 275d 2c20 5b27 3230  E', 'THR'], ['20
-00008890: 3427 2c20 2745 272c 2027 5459 5227 5d2c  4', 'E', 'TYR'],
-000088a0: 205b 2732 3035 272c 2027 4527 2c20 274c   ['205', 'E', 'L
-000088b0: 4555 275d 2c20 5b27 3230 3627 2c20 2745  EU'], ['206', 'E
-000088c0: 272c 2027 414c 4127 5d2c 205b 2732 3039  ', 'ALA'], ['209
-000088d0: 272c 2027 4527 2c20 2749 4c45 275d 2c20  ', 'E', 'ILE'], 
-000088e0: 5b27 3231 3927 2c20 2745 272c 2027 5641  ['219', 'E', 'VA
-000088f0: 4c27 5d2c 205b 2732 3230 272c 2027 4527  L'], ['220', 'E'
-00008900: 2c20 2741 5350 275d 2c20 5b27 3232 3327  , 'ASP'], ['223'
-00008910: 2c20 2745 272c 2027 414c 4127 5d5d 2c20  , 'E', 'ALA']], 
-00008920: 274b 414f 273a 205b 5b27 3438 272c 2027  'KAO': [['48', '
-00008930: 4527 2c20 2754 4852 275d 2c20 5b27 3531  E', 'THR'], ['51
-00008940: 272c 2027 4527 2c20 2754 4852 275d 2c20  ', 'E', 'THR'], 
-00008950: 5b27 3536 272c 2027 4527 2c20 2741 5247  ['56', 'E', 'ARG
-00008960: 275d 2c20 5b27 3333 3027 2c20 2745 272c  '], ['330', 'E',
-00008970: 2027 5459 5227 5d2c 205b 2733 3331 272c   'TYR'], ['331',
-00008980: 2027 4527 2c20 2747 4c55 275d 5d2c 2027   'E', 'GLU']], '
-00008990: 4b41 5027 3a20 5b5b 2732 3232 272c 2027  KAP': [['222', '
-000089a0: 4527 2c20 2754 5250 275d 2c20 5b27 3233  E', 'TRP'], ['23
-000089b0: 3827 2c20 2745 272c 2027 5048 4527 5d2c  8', 'E', 'PHE'],
-000089c0: 205b 2732 3533 272c 2027 4527 2c20 2747   ['253', 'E', 'G
-000089d0: 4c59 275d 2c20 5b27 3235 3427 2c20 2745  LY'], ['254', 'E
-000089e0: 272c 2027 4c59 5327 5d2c 205b 2732 3535  ', 'LYS'], ['255
-000089f0: 272c 2027 4527 2c20 2756 414c 275d 2c20  ', 'E', 'VAL'], 
-00008a00: 5b27 3237 3327 2c20 2745 272c 2027 4c45  ['273', 'E', 'LE
-00008a10: 5527 5d5d 2c20 274b 4151 273a 205b 5b27  U']], 'KAQ': [['
-00008a20: 3230 3727 2c20 2745 272c 2027 5052 4f27  207', 'E', 'PRO'
-00008a30: 5d2c 205b 2732 3038 272c 2027 4527 2c20  ], ['208', 'E', 
-00008a40: 2747 4c55 275d 2c20 5b27 3231 3127 2c20  'GLU'], ['211', 
-00008a50: 2745 272c 2027 4c45 5527 5d2c 205b 2732  'E', 'LEU'], ['2
-00008a60: 3133 272c 2027 4527 2c20 274c 5953 275d  13', 'E', 'LYS']
-00008a70: 2c20 5b27 3237 3527 2c20 2745 272c 2027  , ['275', 'E', '
-00008a80: 5641 4c27 5d2c 205b 2732 3737 272c 2027  VAL'], ['277', '
-00008a90: 4527 2c20 274c 4555 275d 5d2c 2027 4b41  E', 'LEU']], 'KA
-00008aa0: 5227 3a20 5b5b 2732 3337 272c 2027 4527  R': [['237', 'E'
-00008ab0: 2c20 2750 524f 275d 2c20 5b27 3233 3827  , 'PRO'], ['238'
-00008ac0: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
-00008ad0: 2732 3439 272c 2027 4527 2c20 274c 5953  '249', 'E', 'LYS
-00008ae0: 275d 2c20 5b27 3235 3427 2c20 2745 272c  '], ['254', 'E',
-00008af0: 2027 4c59 5327 5d2c 205b 2732 3535 272c   'LYS'], ['255',
-00008b00: 2027 4527 2c20 2756 414c 275d 2c20 5b27   'E', 'VAL'], ['
-00008b10: 3235 3627 2c20 2745 272c 2027 4152 4727  256', 'E', 'ARG'
-00008b20: 5d5d 7d0a 2020 2020 3e3e 3e20 7265 7375  ]]}.    >>> resu
-00008b30: 6c74 732e 6672 6571 7565 6e63 6965 730a  lts.frequencies.
-00008b40: 2020 2020 7b27 4b41 4127 3a20 7b27 5245      {'KAA': {'RE
-00008b50: 5349 4455 4553 273a 207b 2747 4c55 273a  SIDUES': {'GLU':
-00008b60: 2031 2c20 2749 4c45 273a 2031 2c20 274c   1, 'ILE': 1, 'L
-00008b70: 4555 273a 2032 2c20 274c 5953 273a 2031  EU': 2, 'LYS': 1
-00008b80: 2c20 2750 4845 273a 2032 2c20 2753 4552  , 'PHE': 2, 'SER
-00008b90: 273a 2031 2c20 2754 5250 273a 2031 2c20  ': 1, 'TRP': 1, 
-00008ba0: 2754 5952 273a 2032 2c20 2756 414c 273a  'TYR': 2, 'VAL':
-00008bb0: 2031 7d2c 2027 434c 4153 5327 3a20 7b27   1}, 'CLASS': {'
-00008bc0: 5231 273a 2034 2c20 2752 3227 3a20 352c  R1': 4, 'R2': 5,
-00008bd0: 2027 5233 273a 2031 2c20 2752 3427 3a20   'R3': 1, 'R4': 
-00008be0: 312c 2027 5235 273a 2031 2c20 2752 5827  1, 'R5': 1, 'RX'
-00008bf0: 3a20 307d 7d2c 2027 4b41 4227 3a20 7b27  : 0}}, 'KAB': {'
-00008c00: 5245 5349 4455 4553 273a 207b 2741 4c41  RESIDUES': {'ALA
-00008c10: 273a 2032 2c20 2741 534e 273a 2031 2c20  ': 2, 'ASN': 1, 
-00008c20: 2741 5350 273a 2031 2c20 274c 5953 273a  'ASP': 1, 'LYS':
-00008c30: 2031 2c20 2750 4845 273a 2032 2c20 2754   1, 'PHE': 2, 'T
-00008c40: 5952 273a 2031 2c20 2756 414c 273a 2031  YR': 1, 'VAL': 1
-00008c50: 7d2c 2027 434c 4153 5327 3a20 7b27 5231  }, 'CLASS': {'R1
-00008c60: 273a 2033 2c20 2752 3227 3a20 332c 2027  ': 3, 'R2': 3, '
-00008c70: 5233 273a 2031 2c20 2752 3427 3a20 312c  R3': 1, 'R4': 1,
-00008c80: 2027 5235 273a 2031 2c20 2752 5827 3a20   'R5': 1, 'RX': 
-00008c90: 307d 7d2c 2027 4b41 4327 3a20 7b27 5245  0}}, 'KAC': {'RE
-00008ca0: 5349 4455 4553 273a 207b 2741 4c41 273a  SIDUES': {'ALA':
-00008cb0: 2031 2c20 2741 5247 273a 2031 2c20 2747   1, 'ARG': 1, 'G
-00008cc0: 4c55 273a 2031 2c20 2748 4953 273a 2031  LU': 1, 'HIS': 1
-00008cd0: 2c20 2749 4c45 273a 2031 2c20 2750 4845  , 'ILE': 1, 'PHE
-00008ce0: 273a 2031 2c20 2750 524f 273a 2032 2c20  ': 1, 'PRO': 2, 
-00008cf0: 2754 4852 273a 2032 2c20 2756 414c 273a  'THR': 2, 'VAL':
-00008d00: 2031 7d2c 2027 434c 4153 5327 3a20 7b27   1}, 'CLASS': {'
-00008d10: 5231 273a 2035 2c20 2752 3227 3a20 312c  R1': 5, 'R2': 1,
-00008d20: 2027 5233 273a 2032 2c20 2752 3427 3a20   'R3': 2, 'R4': 
-00008d30: 312c 2027 5235 273a 2032 2c20 2752 5827  1, 'R5': 2, 'RX'
-00008d40: 3a20 307d 7d2c 2027 4b41 4427 3a20 7b27  : 0}}, 'KAD': {'
-00008d50: 5245 5349 4455 4553 273a 207b 2741 4c41  RESIDUES': {'ALA
-00008d60: 273a 2031 2c20 2741 5350 273a 2031 2c20  ': 1, 'ASP': 1, 
-00008d70: 2747 4c4e 273a 2031 2c20 2747 4c59 273a  'GLN': 1, 'GLY':
-00008d80: 2032 2c20 2750 4845 273a 2031 2c20 2750   2, 'PHE': 1, 'P
-00008d90: 524f 273a 2031 2c20 2754 5952 273a 2031  RO': 1, 'TYR': 1
-00008da0: 7d2c 2027 434c 4153 5327 3a20 7b27 5231  }, 'CLASS': {'R1
-00008db0: 273a 2034 2c20 2752 3227 3a20 322c 2027  ': 4, 'R2': 2, '
-00008dc0: 5233 273a 2031 2c20 2752 3427 3a20 312c  R3': 1, 'R4': 1,
-00008dd0: 2027 5235 273a 2030 2c20 2752 5827 3a20   'R5': 0, 'RX': 
-00008de0: 307d 7d2c 2027 4b41 4527 3a20 7b27 5245  0}}, 'KAE': {'RE
-00008df0: 5349 4455 4553 273a 207b 2741 534e 273a  SIDUES': {'ASN':
-00008e00: 2031 2c20 274c 4555 273a 2033 2c20 274c   1, 'LEU': 3, 'L
-00008e10: 5953 273a 2031 2c20 2750 4845 273a 2031  YS': 1, 'PHE': 1
-00008e20: 2c20 2756 414c 273a 2032 7d2c 2027 434c  , 'VAL': 2}, 'CL
-00008e30: 4153 5327 3a20 7b27 5231 273a 2035 2c20  ASS': {'R1': 5, 
-00008e40: 2752 3227 3a20 312c 2027 5233 273a 2031  'R2': 1, 'R3': 1
-00008e50: 2c20 2752 3427 3a20 302c 2027 5235 273a  , 'R4': 0, 'R5':
-00008e60: 2031 2c20 2752 5827 3a20 307d 7d2c 2027   1, 'RX': 0}}, '
-00008e70: 4b41 4627 3a20 7b27 5245 5349 4455 4553  KAF': {'RESIDUES
-00008e80: 273a 207b 2741 4c41 273a 2031 2c20 2741  ': {'ALA': 1, 'A
-00008e90: 5350 273a 2031 2c20 2747 4c4e 273a 2032  SP': 1, 'GLN': 2
-00008ea0: 2c20 2756 414c 273a 2031 7d2c 2027 434c  , 'VAL': 1}, 'CL
-00008eb0: 4153 5327 3a20 7b27 5231 273a 2032 2c20  ASS': {'R1': 2, 
-00008ec0: 2752 3227 3a20 302c 2027 5233 273a 2032  'R2': 0, 'R3': 2
-00008ed0: 2c20 2752 3427 3a20 312c 2027 5235 273a  , 'R4': 1, 'R5':
-00008ee0: 2030 2c20 2752 5827 3a20 307d 7d2c 2027   0, 'RX': 0}}, '
-00008ef0: 4b41 4727 3a20 7b27 5245 5349 4455 4553  KAG': {'RESIDUES
-00008f00: 273a 207b 2747 4c4e 273a 2031 2c20 2747  ': {'GLN': 1, 'G
-00008f10: 4c55 273a 2031 2c20 274c 4555 273a 2031  LU': 1, 'LEU': 1
-00008f20: 2c20 2750 4845 273a 2031 2c20 2753 4552  , 'PHE': 1, 'SER
-00008f30: 273a 2032 2c20 2754 4852 273a 2031 7d2c  ': 2, 'THR': 1},
-00008f40: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
-00008f50: 2031 2c20 2752 3227 3a20 312c 2027 5233   1, 'R2': 1, 'R3
-00008f60: 273a 2034 2c20 2752 3427 3a20 312c 2027  ': 4, 'R4': 1, '
-00008f70: 5235 273a 2030 2c20 2752 5827 3a20 307d  R5': 0, 'RX': 0}
-00008f80: 7d2c 2027 4b41 4827 3a20 7b27 5245 5349  }, 'KAH': {'RESI
-00008f90: 4455 4553 273a 207b 2741 4c41 273a 2031  DUES': {'ALA': 1
-00008fa0: 2c20 2741 5247 273a 2031 2c20 2741 534e  , 'ARG': 1, 'ASN
-00008fb0: 273a 2031 2c20 2741 5350 273a 2032 2c20  ': 1, 'ASP': 2, 
-00008fc0: 2747 4c4e 273a 2031 2c20 2747 4c55 273a  'GLN': 1, 'GLU':
-00008fd0: 2034 2c20 2747 4c59 273a 2034 2c20 2748   4, 'GLY': 4, 'H
-00008fe0: 4953 273a 2031 2c20 274c 4555 273a 2033  IS': 1, 'LEU': 3
-00008ff0: 2c20 274c 5953 273a 2032 2c20 274d 4554  , 'LYS': 2, 'MET
-00009000: 273a 2031 2c20 2750 4845 273a 2033 2c20  ': 1, 'PHE': 3, 
-00009010: 2753 4552 273a 2031 2c20 2754 4852 273a  'SER': 1, 'THR':
-00009020: 2034 2c20 2754 5952 273a 2031 2c20 2756   4, 'TYR': 1, 'V
-00009030: 414c 273a 2033 7d2c 2027 434c 4153 5327  AL': 3}, 'CLASS'
-00009040: 3a20 7b27 5231 273a 2031 312c 2027 5232  : {'R1': 11, 'R2
-00009050: 273a 2034 2c20 2752 3327 3a20 382c 2027  ': 4, 'R3': 8, '
-00009060: 5234 273a 2036 2c20 2752 3527 3a20 342c  R4': 6, 'R5': 4,
-00009070: 2027 5258 273a 2030 7d7d 2c20 274b 4149   'RX': 0}}, 'KAI
-00009080: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
-00009090: 7b27 4849 5327 3a20 322c 2027 494c 4527  {'HIS': 2, 'ILE'
-000090a0: 3a20 312c 2027 5048 4527 3a20 322c 2027  : 1, 'PHE': 2, '
-000090b0: 5459 5227 3a20 317d 2c20 2743 4c41 5353  TYR': 1}, 'CLASS
-000090c0: 273a 207b 2752 3127 3a20 312c 2027 5232  ': {'R1': 1, 'R2
-000090d0: 273a 2033 2c20 2752 3327 3a20 302c 2027  ': 3, 'R3': 0, '
-000090e0: 5234 273a 2030 2c20 2752 3527 3a20 322c  R4': 0, 'R5': 2,
-000090f0: 2027 5258 273a 2030 7d7d 2c20 274b 414a   'RX': 0}}, 'KAJ
-00009100: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
-00009110: 7b27 4152 4727 3a20 312c 2027 474c 4e27  {'ARG': 1, 'GLN'
-00009120: 3a20 312c 2027 474c 5527 3a20 312c 2027  : 1, 'GLU': 1, '
-00009130: 4c45 5527 3a20 312c 2027 4c59 5327 3a20  LEU': 1, 'LYS': 
-00009140: 312c 2027 5048 4527 3a20 312c 2027 5052  1, 'PHE': 1, 'PR
-00009150: 4f27 3a20 317d 2c20 2743 4c41 5353 273a  O': 1}, 'CLASS':
-00009160: 207b 2752 3127 3a20 322c 2027 5232 273a   {'R1': 2, 'R2':
-00009170: 2031 2c20 2752 3327 3a20 312c 2027 5234   1, 'R3': 1, 'R4
-00009180: 273a 2031 2c20 2752 3527 3a20 322c 2027  ': 1, 'R5': 2, '
-00009190: 5258 273a 2030 7d7d 2c20 274b 414b 273a  RX': 0}}, 'KAK':
-000091a0: 207b 2752 4553 4944 5545 5327 3a20 7b27   {'RESIDUES': {'
-000091b0: 414c 4127 3a20 312c 2027 494c 4527 3a20  ALA': 1, 'ILE': 
-000091c0: 312c 2027 4c45 5527 3a20 322c 2027 5048  1, 'LEU': 2, 'PH
-000091d0: 4527 3a20 312c 2027 5459 5227 3a20 317d  E': 1, 'TYR': 1}
-000091e0: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
-000091f0: 3a20 342c 2027 5232 273a 2032 2c20 2752  : 4, 'R2': 2, 'R
-00009200: 3327 3a20 302c 2027 5234 273a 2030 2c20  3': 0, 'R4': 0, 
-00009210: 2752 3527 3a20 302c 2027 5258 273a 2030  'R5': 0, 'RX': 0
-00009220: 7d7d 2c20 274b 414c 273a 207b 2752 4553  }}, 'KAL': {'RES
-00009230: 4944 5545 5327 3a20 7b27 4153 4e27 3a20  IDUES': {'ASN': 
-00009240: 312c 2027 4153 5027 3a20 312c 2027 474c  1, 'ASP': 1, 'GL
-00009250: 5527 3a20 312c 2027 4c45 5527 3a20 312c  U': 1, 'LEU': 1,
-00009260: 2027 5048 4527 3a20 322c 2027 5345 5227   'PHE': 2, 'SER'
-00009270: 3a20 312c 2027 5459 5227 3a20 317d 2c20  : 1, 'TYR': 1}, 
-00009280: 2743 4c41 5353 273a 207b 2752 3127 3a20  'CLASS': {'R1': 
-00009290: 312c 2027 5232 273a 2033 2c20 2752 3327  1, 'R2': 3, 'R3'
-000092a0: 3a20 322c 2027 5234 273a 2032 2c20 2752  : 2, 'R4': 2, 'R
-000092b0: 3527 3a20 302c 2027 5258 273a 2030 7d7d  5': 0, 'RX': 0}}
-000092c0: 2c20 274b 414d 273a 207b 2752 4553 4944  , 'KAM': {'RESID
-000092d0: 5545 5327 3a20 7b27 4152 4727 3a20 322c  UES': {'ARG': 2,
-000092e0: 2027 4153 4e27 3a20 312c 2027 4153 5027   'ASN': 1, 'ASP'
-000092f0: 3a20 312c 2027 474c 5927 3a20 312c 2027  : 1, 'GLY': 1, '
-00009300: 494c 4527 3a20 322c 2027 4c45 5527 3a20  ILE': 2, 'LEU': 
-00009310: 312c 2027 5448 5227 3a20 317d 2c20 2743  1, 'THR': 1}, 'C
-00009320: 4c41 5353 273a 207b 2752 3127 3a20 342c  LASS': {'R1': 4,
-00009330: 2027 5232 273a 2030 2c20 2752 3327 3a20   'R2': 0, 'R3': 
-00009340: 322c 2027 5234 273a 2031 2c20 2752 3527  2, 'R4': 1, 'R5'
-00009350: 3a20 322c 2027 5258 273a 2030 7d7d 2c20  : 2, 'RX': 0}}, 
-00009360: 274b 414e 273a 207b 2752 4553 4944 5545  'KAN': {'RESIDUE
-00009370: 5327 3a20 7b27 414c 4127 3a20 322c 2027  S': {'ALA': 2, '
-00009380: 4152 4727 3a20 312c 2027 4153 5027 3a20  ARG': 1, 'ASP': 
-00009390: 322c 2027 4359 5327 3a20 312c 2027 474c  2, 'CYS': 1, 'GL
-000093a0: 5927 3a20 312c 2027 494c 4527 3a20 312c  Y': 1, 'ILE': 1,
-000093b0: 2027 4c45 5527 3a20 322c 2027 5448 5227   'LEU': 2, 'THR'
-000093c0: 3a20 312c 2027 5459 5227 3a20 312c 2027  : 1, 'TYR': 1, '
-000093d0: 5641 4c27 3a20 317d 2c20 2743 4c41 5353  VAL': 1}, 'CLASS
-000093e0: 273a 207b 2752 3127 3a20 372c 2027 5232  ': {'R1': 7, 'R2
-000093f0: 273a 2031 2c20 2752 3327 3a20 322c 2027  ': 1, 'R3': 2, '
-00009400: 5234 273a 2032 2c20 2752 3527 3a20 312c  R4': 2, 'R5': 1,
-00009410: 2027 5258 273a 2030 7d7d 2c20 274b 414f   'RX': 0}}, 'KAO
-00009420: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
-00009430: 7b27 4152 4727 3a20 312c 2027 474c 5527  {'ARG': 1, 'GLU'
-00009440: 3a20 312c 2027 5448 5227 3a20 322c 2027  : 1, 'THR': 2, '
-00009450: 5459 5227 3a20 317d 2c20 2743 4c41 5353  TYR': 1}, 'CLASS
-00009460: 273a 207b 2752 3127 3a20 302c 2027 5232  ': {'R1': 0, 'R2
-00009470: 273a 2031 2c20 2752 3327 3a20 322c 2027  ': 1, 'R3': 2, '
-00009480: 5234 273a 2031 2c20 2752 3527 3a20 312c  R4': 1, 'R5': 1,
-00009490: 2027 5258 273a 2030 7d7d 2c20 274b 4150   'RX': 0}}, 'KAP
-000094a0: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
-000094b0: 7b27 474c 5927 3a20 312c 2027 4c45 5527  {'GLY': 1, 'LEU'
-000094c0: 3a20 312c 2027 4c59 5327 3a20 312c 2027  : 1, 'LYS': 1, '
-000094d0: 5048 4527 3a20 312c 2027 5452 5027 3a20  PHE': 1, 'TRP': 
-000094e0: 312c 2027 5641 4c27 3a20 317d 2c20 2743  1, 'VAL': 1}, 'C
-000094f0: 4c41 5353 273a 207b 2752 3127 3a20 332c  LASS': {'R1': 3,
-00009500: 2027 5232 273a 2032 2c20 2752 3327 3a20   'R2': 2, 'R3': 
-00009510: 302c 2027 5234 273a 2030 2c20 2752 3527  0, 'R4': 0, 'R5'
-00009520: 3a20 312c 2027 5258 273a 2030 7d7d 2c20  : 1, 'RX': 0}}, 
-00009530: 274b 4151 273a 207b 2752 4553 4944 5545  'KAQ': {'RESIDUE
-00009540: 5327 3a20 7b27 474c 5527 3a20 312c 2027  S': {'GLU': 1, '
-00009550: 4c45 5527 3a20 322c 2027 4c59 5327 3a20  LEU': 2, 'LYS': 
-00009560: 312c 2027 5052 4f27 3a20 312c 2027 5641  1, 'PRO': 1, 'VA
-00009570: 4c27 3a20 317d 2c20 2743 4c41 5353 273a  L': 1}, 'CLASS':
-00009580: 207b 2752 3127 3a20 342c 2027 5232 273a   {'R1': 4, 'R2':
-00009590: 2030 2c20 2752 3327 3a20 302c 2027 5234   0, 'R3': 0, 'R4
-000095a0: 273a 2031 2c20 2752 3527 3a20 312c 2027  ': 1, 'R5': 1, '
-000095b0: 5258 273a 2030 7d7d 2c20 274b 4152 273a  RX': 0}}, 'KAR':
-000095c0: 207b 2752 4553 4944 5545 5327 3a20 7b27   {'RESIDUES': {'
-000095d0: 4152 4727 3a20 312c 2027 4c59 5327 3a20  ARG': 1, 'LYS': 
-000095e0: 322c 2027 5048 4527 3a20 312c 2027 5052  2, 'PHE': 1, 'PR
-000095f0: 4f27 3a20 312c 2027 5641 4c27 3a20 317d  O': 1, 'VAL': 1}
-00009600: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
-00009610: 3a20 322c 2027 5232 273a 2031 2c20 2752  : 2, 'R2': 1, 'R
-00009620: 3327 3a20 302c 2027 5234 273a 2030 2c20  3': 0, 'R4': 0, 
-00009630: 2752 3527 3a20 332c 2027 5258 273a 2030  'R5': 3, 'RX': 0
-00009640: 7d7d 7d0a 0a20 2020 2048 6f77 6576 6572  }}}..    However
-00009650: 2c20 7573 6572 7320 6d61 7920 6f70 7420  , users may opt 
-00009660: 746f 2070 6572 666f 726d 2063 6176 6974  to perform cavit
-00009670: 7920 6465 7465 6374 696f 6e20 696e 2061  y detection in a
-00009680: 2073 6567 6d65 6e74 6564 2073 7061 6365   segmented space
-00009690: 2074 6872 6f75 6768 206c 6967 616e 6420   through ligand 
-000096a0: 6164 6a75 7374 6d65 6e74 2061 6e64 2f6f  adjustment and/o
-000096b0: 7220 626f 7820 6164 6a75 7374 6d65 6e74  r box adjustment
-000096c0: 206d 6f64 6573 2e0a 0a20 2020 2054 6865   modes...    The
-000096d0: 2063 6176 6974 7920 6465 7465 6374 696f   cavity detectio
-000096e0: 6e20 6361 6e20 6265 206c 696d 6974 6564  n can be limited
-000096f0: 2061 726f 756e 6420 7468 6520 7461 7267   around the targ
-00009700: 6574 206c 6967 616e 6428 7329 2c20 7768  et ligand(s), wh
-00009710: 6963 6820 7769 6c6c 2062 6520 7061 7373  ich will be pass
-00009720: 6564 2074 6f20 7079 4b56 4669 6e64 6572  ed to pyKVFinder
-00009730: 2074 6872 6f75 6768 2061 202a 2e70 6462   through a *.pdb
-00009740: 2a20 6f72 2061 202a 2e78 797a 2a20 6669  * or a *.xyz* fi
-00009750: 6c65 732e 2054 6875 732c 2074 6865 2064  les. Thus, the d
-00009760: 6574 6563 7465 6420 6361 7669 7469 6573  etected cavities
-00009770: 2061 7265 206c 696d 6974 6564 2077 6974   are limited wit
-00009780: 6869 6e20 6120 7261 6469 7573 2028 6060  hin a radius (``
-00009790: 6c69 6761 6e64 5f63 7574 6f66 6660 6029  ligand_cutoff``)
-000097a0: 206f 6620 7468 6520 7461 7267 6574 206c   of the target l
-000097b0: 6967 616e 6428 7329 2e0a 0a20 2020 203e  igand(s)...    >
-000097c0: 3e3e 206c 6967 616e 6420 3d20 6f73 2e70  >> ligand = os.p
-000097d0: 6174 682e 6a6f 696e 286f 732e 7061 7468  ath.join(os.path
-000097e0: 2e64 6972 6e61 6d65 2870 794b 5646 696e  .dirname(pyKVFin
-000097f0: 6465 722e 5f5f 6669 6c65 5f5f 292c 2027  der.__file__), '
-00009800: 6461 7461 272c 2027 7465 7374 7327 2c20  data', 'tests', 
-00009810: 2741 444e 2e70 6462 2729 0a20 2020 203e  'ADN.pdb').    >
-00009820: 3e3e 2072 6573 756c 7473 203d 2070 794b  >> results = pyK
-00009830: 5646 696e 6465 722e 7275 6e5f 776f 726b  VFinder.run_work
-00009840: 666c 6f77 2870 6462 2c20 6c69 6761 6e64  flow(pdb, ligand
-00009850: 290a 2020 2020 3e3e 3e20 7265 7375 6c74  ).    >>> result
-00009860: 730a 2020 2020 3c70 794b 5646 696e 6465  s.    <pyKVFinde
-00009870: 7252 6573 756c 7473 206f 626a 6563 743e  rResults object>
-00009880: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
-00009890: 2e63 6176 6974 6965 730a 2020 2020 6172  .cavities.    ar
-000098a0: 7261 7928 5b5b 5b2d 312c 202d 312c 202d  ray([[[-1, -1, -
-000098b0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-000098c0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-000098d0: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-000098e0: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-000098f0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00009900: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00009910: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
-00009920: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-00009930: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-00009940: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00009950: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-00009960: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-00009970: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-00009980: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-00009990: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-000099a0: 2d31 2c20 2d31 2c20 2d31 5d5d 2c0a 2020  -1, -1, -1]],.  
-000099b0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-000099c0: 2020 2020 2020 2020 205b 5b2d 312c 202d           [[-1, -
-000099d0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-000099e0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-000099f0: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
-00009a00: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-00009a10: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-00009a20: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-00009a30: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-00009a40: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
-00009a50: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00009a60: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00009a70: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
-00009a80: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
-00009a90: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
-00009aa0: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
-00009ab0: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-00009ac0: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d5d  .., -1, -1, -1]]
-00009ad0: 5d2c 2064 7479 7065 3d69 6e74 3332 290a  ], dtype=int32).
-00009ae0: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-00009af0: 7375 7266 6163 650a 2020 2020 6172 7261  surface.    arra
-00009b00: 7928 5b5b 5b2d 312c 202d 312c 202d 312c  y([[[-1, -1, -1,
-00009b10: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-00009b20: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00009b30: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-00009b40: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-00009b50: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00009b60: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00009b70: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00009b80: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-00009b90: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-00009ba0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00009bb0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00009bc0: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-00009bd0: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00009be0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00009bf0: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00009c00: 2c20 2d31 2c20 2d31 5d5d 2c0a 2020 2020  , -1, -1]],.    
-00009c10: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-00009c20: 2020 2020 2020 205b 5b2d 312c 202d 312c         [[-1, -1,
-00009c30: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00009c40: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-00009c50: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-00009c60: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-00009c70: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-00009c80: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-00009c90: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
-00009ca0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-00009cb0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00009cc0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00009cd0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00009ce0: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
-00009cf0: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-00009d00: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-00009d10: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-00009d20: 2c20 2d31 2c20 2d31 2c20 2d31 5d5d 5d2c  , -1, -1, -1]]],
-00009d30: 2064 7479 7065 3d69 6e74 3332 290a 2020   dtype=int32).  
-00009d40: 2020 3e3e 3e20 7265 7375 6c74 732e 6e63    >>> results.nc
-00009d50: 6176 0a20 2020 203e 3e3e 2031 380a 2020  av.    >>> 18.  
-00009d60: 2020 3e3e 3e20 7265 7375 6c74 732e 766f    >>> results.vo
-00009d70: 6c75 6d65 0a20 2020 207b 274b 4141 273a  lume.    {'KAA':
-00009d80: 2033 3635 2e30 342c 2027 4b41 4227 3a20   365.04, 'KAB': 
-00009d90: 3136 2e38 357d 0a20 2020 203e 3e3e 2072  16.85}.    >>> r
-00009da0: 6573 756c 7473 2e61 7265 610a 2020 2020  esults.area.    
-00009db0: 7b27 4b41 4127 3a20 3332 382e 3739 2c20  {'KAA': 328.79, 
-00009dc0: 274b 4142 273a 2032 332e 3135 7d0a 2020  'KAB': 23.15}.  
-00009dd0: 2020 3e3e 3e20 7265 7375 6c74 732e 7265    >>> results.re
-00009de0: 7369 6475 6573 0a20 2020 207b 274b 4141  sidues.    {'KAA
-00009df0: 273a 205b 5b27 3439 272c 2027 4527 2c20  ': [['49', 'E', 
-00009e00: 274c 4555 275d 2c20 5b27 3530 272c 2027  'LEU'], ['50', '
-00009e10: 4527 2c20 2747 4c59 275d 2c20 5b27 3531  E', 'GLY'], ['51
-00009e20: 272c 2027 4527 2c20 2754 4852 275d 2c20  ', 'E', 'THR'], 
-00009e30: 5b27 3532 272c 2027 4527 2c20 2747 4c59  ['52', 'E', 'GLY
-00009e40: 275d 2c20 5b27 3533 272c 2027 4527 2c20  '], ['53', 'E', 
-00009e50: 2753 4552 275d 2c20 5b27 3535 272c 2027  'SER'], ['55', '
-00009e60: 4527 2c20 2747 4c59 275d 2c20 5b27 3536  E', 'GLY'], ['56
-00009e70: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
-00009e80: 5b27 3537 272c 2027 4527 2c20 2756 414c  ['57', 'E', 'VAL
-00009e90: 275d 2c20 5b27 3730 272c 2027 4527 2c20  '], ['70', 'E', 
-00009ea0: 2741 4c41 275d 2c20 5b27 3732 272c 2027  'ALA'], ['72', '
-00009eb0: 4527 2c20 274c 5953 275d 2c20 5b27 3130  E', 'LYS'], ['10
-00009ec0: 3427 2c20 2745 272c 2027 5641 4c27 5d2c  4', 'E', 'VAL'],
-00009ed0: 205b 2731 3230 272c 2027 4527 2c20 274d   ['120', 'E', 'M
-00009ee0: 4554 275d 2c20 5b27 3132 3127 2c20 2745  ET'], ['121', 'E
-00009ef0: 272c 2027 474c 5527 5d2c 205b 2731 3232  ', 'GLU'], ['122
-00009f00: 272c 2027 4527 2c20 2754 5952 275d 2c20  ', 'E', 'TYR'], 
-00009f10: 5b27 3132 3327 2c20 2745 272c 2027 5641  ['123', 'E', 'VA
-00009f20: 4c27 5d2c 205b 2731 3237 272c 2027 4527  L'], ['127', 'E'
-00009f30: 2c20 2747 4c55 275d 2c20 5b27 3136 3627  , 'GLU'], ['166'
-00009f40: 2c20 2745 272c 2027 4153 5027 5d2c 205b  , 'E', 'ASP'], [
-00009f50: 2731 3638 272c 2027 4527 2c20 274c 5953  '168', 'E', 'LYS
-00009f60: 275d 2c20 5b27 3137 3027 2c20 2745 272c  '], ['170', 'E',
-00009f70: 2027 474c 5527 5d2c 205b 2731 3731 272c   'GLU'], ['171',
-00009f80: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
-00009f90: 3137 3327 2c20 2745 272c 2027 4c45 5527  173', 'E', 'LEU'
-00009fa0: 5d2c 205b 2731 3833 272c 2027 4527 2c20  ], ['183', 'E', 
-00009fb0: 2754 4852 275d 2c20 5b27 3138 3427 2c20  'THR'], ['184', 
-00009fc0: 2745 272c 2027 4153 5027 5d2c 205b 2733  'E', 'ASP'], ['3
-00009fd0: 3237 272c 2027 4527 2c20 2750 4845 275d  27', 'E', 'PHE']
-00009fe0: 5d2c 2027 4b41 4227 3a20 5b5b 2734 3927  ], 'KAB': [['49'
-00009ff0: 2c20 2745 272c 2027 4c45 5527 5d2c 205b  , 'E', 'LEU'], [
-0000a000: 2731 3237 272c 2027 4527 2c20 2747 4c55  '127', 'E', 'GLU
-0000a010: 275d 2c20 5b27 3133 3027 2c20 2745 272c  '], ['130', 'E',
-0000a020: 2027 5345 5227 5d2c 205b 2733 3236 272c   'SER'], ['326',
-0000a030: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
-0000a040: 3332 3727 2c20 2745 272c 2027 5048 4527  327', 'E', 'PHE'
-0000a050: 5d2c 205b 2733 3238 272c 2027 4527 2c20  ], ['328', 'E', 
-0000a060: 2741 5350 275d 2c20 5b27 3333 3027 2c20  'ASP'], ['330', 
-0000a070: 2745 272c 2027 5459 5227 5d5d 7d0a 2020  'E', 'TYR']]}.  
-0000a080: 2020 3e3e 3e20 7265 7375 6c74 732e 6672    >>> results.fr
-0000a090: 6571 7565 6e63 6965 730a 2020 2020 7b27  equencies.    {'
-0000a0a0: 4b41 4127 3a20 7b27 5245 5349 4455 4553  KAA': {'RESIDUES
-0000a0b0: 273a 207b 2741 4c41 273a 2031 2c20 2741  ': {'ALA': 1, 'A
-0000a0c0: 5247 273a 2031 2c20 2741 534e 273a 2031  RG': 1, 'ASN': 1
-0000a0d0: 2c20 2741 5350 273a 2032 2c20 2747 4c55  , 'ASP': 2, 'GLU
-0000a0e0: 273a 2033 2c20 2747 4c59 273a 2033 2c20  ': 3, 'GLY': 3, 
-0000a0f0: 274c 4555 273a 2032 2c20 274c 5953 273a  'LEU': 2, 'LYS':
-0000a100: 2032 2c20 274d 4554 273a 2031 2c20 2750   2, 'MET': 1, 'P
-0000a110: 4845 273a 2031 2c20 2753 4552 273a 2031  HE': 1, 'SER': 1
-0000a120: 2c20 2754 4852 273a 2032 2c20 2754 5952  , 'THR': 2, 'TYR
-0000a130: 273a 2031 2c20 2756 414c 273a 2033 7d2c  ': 1, 'VAL': 3},
-0000a140: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
-0000a150: 2039 2c20 2752 3227 3a20 322c 2027 5233   9, 'R2': 2, 'R3
-0000a160: 273a 2035 2c20 2752 3427 3a20 352c 2027  ': 5, 'R4': 5, '
-0000a170: 5235 273a 2033 2c20 2752 5827 3a20 307d  R5': 3, 'RX': 0}
-0000a180: 7d2c 2027 4b41 4227 3a20 7b27 5245 5349  }, 'KAB': {'RESI
-0000a190: 4455 4553 273a 207b 2741 534e 273a 2031  DUES': {'ASN': 1
-0000a1a0: 2c20 2741 5350 273a 2031 2c20 2747 4c55  , 'ASP': 1, 'GLU
-0000a1b0: 273a 2031 2c20 274c 4555 273a 2031 2c20  ': 1, 'LEU': 1, 
-0000a1c0: 2750 4845 273a 2031 2c20 2753 4552 273a  'PHE': 1, 'SER':
-0000a1d0: 2031 2c20 2754 5952 273a 2031 7d2c 2027   1, 'TYR': 1}, '
-0000a1e0: 434c 4153 5327 3a20 7b27 5231 273a 2031  CLASS': {'R1': 1
-0000a1f0: 2c20 2752 3227 3a20 322c 2027 5233 273a  , 'R2': 2, 'R3':
-0000a200: 2032 2c20 2752 3427 3a20 322c 2027 5235   2, 'R4': 2, 'R5
-0000a210: 273a 2030 2c20 2752 5827 3a20 307d 7d7d  ': 0, 'RX': 0}}}
-0000a220: 0a0a 2020 2020 4675 7274 6865 722c 2077  ..    Further, w
-0000a230: 6520 6361 6e20 616c 736f 2070 6572 666f  e can also perfo
-0000a240: 726d 2063 6176 6974 7920 6465 7465 6374  rm cavity detect
-0000a250: 696f 6e20 6f6e 2061 2063 7573 746f 6d20  ion on a custom 
-0000a260: 3344 2067 7269 642c 2077 6865 7265 2077  3D grid, where w
-0000a270: 6520 6361 6e20 6578 706c 6f72 6520 636c  e can explore cl
-0000a280: 6f73 6564 2072 6567 696f 6e73 2077 6974  osed regions wit
-0000a290: 6820 6120 6375 7374 6f6d 2062 6f78 2c20  h a custom box, 
-0000a2a0: 7768 6963 6820 6361 6e20 6265 2064 6566  which can be def
-0000a2b0: 696e 6564 2062 7920 6120 2a2e 746f 6d6c  ined by a *.toml
-0000a2c0: 2a20 6669 6c65 2028 7365 6520 6042 6f78  * file (see `Box
-0000a2d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-0000a2e0: 696c 6520 7465 6d70 6c61 7465 6029 2e0a  ile template`)..
-0000a2f0: 0a20 2020 203e 3e3e 2066 6e20 3d20 6f73  .    >>> fn = os
-0000a300: 2e70 6174 682e 6a6f 696e 286f 732e 7061  .path.join(os.pa
-0000a310: 7468 2e64 6972 6e61 6d65 2870 794b 5646  th.dirname(pyKVF
-0000a320: 696e 6465 722e 5f5f 6669 6c65 5f5f 292c  inder.__file__),
-0000a330: 2027 6461 7461 272c 2027 7465 7374 7327   'data', 'tests'
-0000a340: 2c20 2763 7573 746f 6d2d 626f 782e 746f  , 'custom-box.to
-0000a350: 6d6c 2729 0a20 2020 203e 3e3e 2077 6974  ml').    >>> wit
-0000a360: 6820 6f70 656e 2866 6e2c 2027 7227 2920  h open(fn, 'r') 
-0000a370: 6173 2066 3a0a 2020 2020 2e2e 2e20 2020  as f:.    ...   
-0000a380: 2020 7072 696e 7428 662e 7265 6164 2829    print(f.read()
-0000a390: 290a 2020 2020 5b62 6f78 5d0a 2020 2020  ).    [box].    
-0000a3a0: 7031 203d 205b 332e 3131 2c20 372e 3334  p1 = [3.11, 7.34
-0000a3b0: 2c20 312e 3539 5d0a 2020 2020 7032 203d  , 1.59].    p2 =
-0000a3c0: 205b 3131 2e35 312c 2037 2e33 342c 2031   [11.51, 7.34, 1
-0000a3d0: 2e35 395d 0a20 2020 2070 3320 3d20 5b33  .59].    p3 = [3
-0000a3e0: 2e31 312c 2031 302e 3734 2c20 312e 3539  .11, 10.74, 1.59
-0000a3f0: 5d0a 2020 2020 7034 203d 205b 332e 3131  ].    p4 = [3.11
-0000a400: 2c20 372e 3334 2c20 362e 3139 5d0a 2020  , 7.34, 6.19].  
-0000a410: 2020 3e3e 3e20 7265 7375 6c74 7320 3d20    >>> results = 
-0000a420: 7079 4b56 4669 6e64 6572 2e72 756e 5f77  pyKVFinder.run_w
-0000a430: 6f72 6b66 6c6f 7728 7064 622c 2062 6f78  orkflow(pdb, box
-0000a440: 3d66 6e29 0a20 2020 203e 3e3e 2072 6573  =fn).    >>> res
-0000a450: 756c 7473 0a20 2020 203c 7079 4b56 4669  ults.    <pyKVFi
-0000a460: 6e64 6572 5265 7375 6c74 7320 6f62 6a65  nderResults obje
-0000a470: 6374 3e0a 2020 2020 3e3e 3e20 7265 7375  ct>.    >>> resu
-0000a480: 6c74 732e 6361 7669 7469 6573 0a20 2020  lts.cavities.   
-0000a490: 2061 7272 6179 285b 5b5b 2d31 2c20 2d31   array([[[-1, -1
-0000a4a0: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
-0000a4b0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
-0000a4c0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-0000a4d0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-0000a4e0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000a4f0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-0000a500: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-0000a510: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
-0000a520: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-0000a530: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-0000a540: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-0000a550: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-0000a560: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-0000a570: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-0000a580: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-0000a590: 2e2c 202d 312c 202d 312c 202d 315d 5d2c  ., -1, -1, -1]],
-0000a5a0: 0a20 2020 2020 2020 2020 2020 2e2e 2e2c  .           ...,
-0000a5b0: 0a20 2020 2020 2020 2020 2020 5b5b 2d31  .           [[-1
-0000a5c0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-0000a5d0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-0000a5e0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-0000a5f0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-0000a600: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-0000a610: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-0000a620: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-0000a630: 2c0a 2020 2020 2020 2020 2020 2020 2e2e  ,.            ..
-0000a640: 2e2c 0a20 2020 2020 2020 2020 2020 205b  .,.            [
-0000a650: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-0000a660: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-0000a670: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-0000a680: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-0000a690: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-0000a6a0: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
-0000a6b0: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-0000a6c0: 315d 5d5d 2c20 6474 7970 653d 696e 7433  1]]], dtype=int3
-0000a6d0: 3229 0a20 2020 203e 3e3e 2072 6573 756c  2).    >>> resul
-0000a6e0: 7473 2e73 7572 6661 6365 0a20 2020 2061  ts.surface.    a
-0000a6f0: 7272 6179 285b 5b5b 2d31 2c20 2d31 2c20  rray([[[-1, -1, 
-0000a700: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
-0000a710: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
-0000a720: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-0000a730: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-0000a740: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-0000a750: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-0000a760: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-0000a770: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-0000a780: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
-0000a790: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
-0000a7a0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
-0000a7b0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-0000a7c0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-0000a7d0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000a7e0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-0000a7f0: 202d 312c 202d 312c 202d 315d 5d2c 0a20   -1, -1, -1]],. 
-0000a800: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
-0000a810: 2020 2020 2020 2020 2020 5b5b 2d31 2c20            [[-1, 
-0000a820: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-0000a830: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-0000a840: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-0000a850: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-0000a860: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-0000a870: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-0000a880: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-0000a890: 2020 2020 2020 2020 2020 2020 2e2e 2e2c              ...,
-0000a8a0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-0000a8b0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-0000a8c0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-0000a8d0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-0000a8e0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-0000a8f0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-0000a900: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-0000a910: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-0000a920: 5d5d 2c20 6474 7970 653d 696e 7433 3229  ]], dtype=int32)
-0000a930: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
-0000a940: 2e6e 6361 760a 2020 2020 3e3e 3e20 310a  .ncav.    >>> 1.
-0000a950: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-0000a960: 766f 6c75 6d65 0a20 2020 207b 274b 4141  volume.    {'KAA
-0000a970: 273a 2031 3135 2e37 387d 0a20 2020 203e  ': 115.78}.    >
-0000a980: 3e3e 2072 6573 756c 7473 2e61 7265 610a  >> results.area.
-0000a990: 2020 2020 7b27 4b41 4127 3a20 3333 2e39      {'KAA': 33.9
-0000a9a0: 317d 0a20 2020 203e 3e3e 2072 6573 756c  1}.    >>> resul
-0000a9b0: 7473 2e72 6573 6964 7565 730a 2020 2020  ts.residues.    
-0000a9c0: 7b27 4b41 4127 3a20 5b5b 2734 3927 2c20  {'KAA': [['49', 
-0000a9d0: 2745 272c 2027 4c45 5527 5d2c 205b 2735  'E', 'LEU'], ['5
-0000a9e0: 3027 2c20 2745 272c 2027 474c 5927 5d2c  0', 'E', 'GLY'],
-0000a9f0: 205b 2735 3127 2c20 2745 272c 2027 5448   ['51', 'E', 'TH
-0000aa00: 5227 5d2c 205b 2735 3727 2c20 2745 272c  R'], ['57', 'E',
-0000aa10: 2027 5641 4c27 5d2c 205b 2737 3027 2c20   'VAL'], ['70', 
-0000aa20: 2745 272c 2027 414c 4127 5d2c 205b 2731  'E', 'ALA'], ['1
-0000aa30: 3034 272c 2027 4527 2c20 2756 414c 275d  04', 'E', 'VAL']
-0000aa40: 2c20 5b27 3132 3127 2c20 2745 272c 2027  , ['121', 'E', '
-0000aa50: 474c 5527 5d2c 205b 2731 3232 272c 2027  GLU'], ['122', '
-0000aa60: 4527 2c20 2754 5952 275d 2c20 5b27 3132  E', 'TYR'], ['12
-0000aa70: 3327 2c20 2745 272c 2027 5641 4c27 5d2c  3', 'E', 'VAL'],
-0000aa80: 205b 2731 3237 272c 2027 4527 2c20 2747   ['127', 'E', 'G
-0000aa90: 4c55 275d 2c20 5b27 3137 3027 2c20 2745  LU'], ['170', 'E
-0000aaa0: 272c 2027 474c 5527 5d2c 205b 2731 3731  ', 'GLU'], ['171
-0000aab0: 272c 2027 4527 2c20 2741 534e 275d 2c20  ', 'E', 'ASN'], 
-0000aac0: 5b27 3137 3327 2c20 2745 272c 2027 4c45  ['173', 'E', 'LE
-0000aad0: 5527 5d2c 205b 2731 3833 272c 2027 4527  U'], ['183', 'E'
-0000aae0: 2c20 2754 4852 275d 2c20 5b27 3332 3727  , 'THR'], ['327'
-0000aaf0: 2c20 2745 272c 2027 5048 4527 5d5d 7d0a  , 'E', 'PHE']]}.
-0000ab00: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-0000ab10: 6672 6571 7565 6e63 6965 730a 2020 2020  frequencies.    
-0000ab20: 7b27 4b41 4127 3a20 7b27 5245 5349 4455  {'KAA': {'RESIDU
-0000ab30: 4553 273a 207b 2741 4c41 273a 2031 2c20  ES': {'ALA': 1, 
-0000ab40: 2741 534e 273a 2031 2c20 2747 4c55 273a  'ASN': 1, 'GLU':
-0000ab50: 2033 2c20 2747 4c59 273a 2031 2c20 274c   3, 'GLY': 1, 'L
-0000ab60: 4555 273a 2032 2c20 2750 4845 273a 2031  EU': 2, 'PHE': 1
-0000ab70: 2c20 2754 4852 273a 2032 2c20 2754 5952  , 'THR': 2, 'TYR
-0000ab80: 273a 2031 2c20 2756 414c 273a 2033 7d2c  ': 1, 'VAL': 3},
-0000ab90: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
-0000aba0: 2037 2c20 2752 3227 3a20 322c 2027 5233   7, 'R2': 2, 'R3
-0000abb0: 273a 2033 2c20 2752 3427 3a20 332c 2027  ': 3, 'R4': 3, '
-0000abc0: 5235 273a 2030 2c20 2752 5827 3a20 307d  R5': 0, 'RX': 0}
-0000abd0: 7d7d 0a0a 2020 2020 486f 7765 7665 722c  }}..    However,
-0000abe0: 2075 7365 7273 206d 6179 206f 7074 2074   users may opt t
-0000abf0: 6f20 7065 7266 6f72 6d20 7468 6520 2a2a  o perform the **
-0000ac00: 6675 6c6c 2077 6f72 6b66 6c6f 772a 2a20  full workflow** 
-0000ac10: 666f 7220 6361 7669 7479 2064 6574 6563  for cavity detec
-0000ac20: 7469 6f6e 2077 6974 6820 7370 6174 6961  tion with spatia
-0000ac30: 6c20 2873 7572 6661 6365 2070 6f69 6e74  l (surface point
-0000ac40: 732c 2076 6f6c 756d 6520 616e 6420 6172  s, volume and ar
-0000ac50: 6561 292c 2063 6f6e 7374 6974 7574 696f  ea), constitutio
-0000ac60: 6e61 6c20 2869 6e74 6572 6661 6365 2072  nal (interface r
-0000ac70: 6573 6964 7565 7320 616e 6420 7468 6569  esidues and thei
-0000ac80: 7220 6672 6571 7565 6e63 6965 7329 2c20  r frequencies), 
-0000ac90: 6879 6472 6f70 6174 6879 2061 6e64 2064  hydropathy and d
-0000aca0: 6570 7468 2063 6861 7261 6374 6572 697a  epth characteriz
-0000acb0: 6174 696f 6e2e 2054 6869 7320 6675 6c6c  ation. This full
-0000acc0: 2077 6f72 6b66 6c6f 7720 6361 6e20 6265   workflow can be
-0000acd0: 2072 756e 2077 6974 6820 6f6e 6520 636f   run with one co
-0000ace0: 6d6d 616e 6420 6279 2073 6574 7469 6e67  mmand by setting
-0000acf0: 2073 6f6d 6520 7061 7261 6d65 7465 7273   some parameters
-0000ad00: 206f 6620 6060 7275 6e5f 776f 726b 666c   of ``run_workfl
-0000ad10: 6f77 6060 2066 756e 6374 696f 6e3a 0a0a  ow`` function:..
-0000ad20: 2020 2020 3e3e 3e20 7265 7375 6c74 7320      >>> results 
-0000ad30: 3d20 7079 4b56 4669 6e64 6572 2e72 756e  = pyKVFinder.run
-0000ad40: 5f77 6f72 6b66 6c6f 7728 7064 622c 2069  _workflow(pdb, i
-0000ad50: 6e63 6c75 6465 5f64 6570 7468 3d54 7275  nclude_depth=Tru
-0000ad60: 652c 2069 6e63 6c75 6465 5f68 7964 726f  e, include_hydro
-0000ad70: 7061 7468 793d 5472 7565 2c20 6879 6472  pathy=True, hydr
-0000ad80: 6f70 686f 6269 6369 7479 5f73 6361 6c65  ophobicity_scale
-0000ad90: 3d27 4569 7365 6e62 6572 6757 6569 7373  ='EisenbergWeiss
-0000ada0: 2729 0a20 2020 203e 3e3e 2072 6573 756c  ').    >>> resul
-0000adb0: 7473 2e64 6570 7468 730a 2020 2020 6172  ts.depths.    ar
-0000adc0: 7261 7928 5b5b 5b30 2e2c 2030 2e2c 2030  ray([[[0., 0., 0
-0000add0: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
-0000ade0: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
-0000adf0: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
-0000ae00: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
-0000ae10: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-0000ae20: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-0000ae30: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-0000ae40: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-0000ae50: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
-0000ae60: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-0000ae70: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-0000ae80: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
-0000ae90: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-0000aea0: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-0000aeb0: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-0000aec0: 302e 2c20 302e 2c20 302e 5d5d 2c0a 2020  0., 0., 0.]],.  
-0000aed0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-0000aee0: 2020 2020 2020 2020 205b 5b30 2e2c 2030           [[0., 0
-0000aef0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
-0000af00: 302e 2c20 302e 5d2c 0a20 2020 2020 2020  0., 0.],.       
-0000af10: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
-0000af20: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
-0000af30: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-0000af40: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
-0000af50: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
-0000af60: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
-0000af70: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-0000af80: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-0000af90: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-0000afa0: 2020 2020 2020 205b 302e 2c20 302e 2c20         [0., 0., 
-0000afb0: 302e 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c  0., ..., 0., 0.,
-0000afc0: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
-0000afd0: 2020 5b30 2e2c 2030 2e2c 2030 2e2c 202e    [0., 0., 0., .
-0000afe0: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d5d  .., 0., 0., 0.]]
-0000aff0: 5d29 0a20 2020 203e 3e3e 2072 6573 756c  ]).    >>> resul
-0000b000: 7473 2e73 6361 6c65 730a 2020 2020 6172  ts.scales.    ar
-0000b010: 7261 7928 5b5b 5b30 2e2c 2030 2e2c 2030  ray([[[0., 0., 0
-0000b020: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
-0000b030: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
-0000b040: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
-0000b050: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
-0000b060: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-0000b070: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-0000b080: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-0000b090: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-0000b0a0: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
-0000b0b0: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-0000b0c0: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-0000b0d0: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
-0000b0e0: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-0000b0f0: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-0000b100: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-0000b110: 302e 2c20 302e 2c20 302e 5d5d 2c0a 2020  0., 0., 0.]],.  
-0000b120: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-0000b130: 2020 2020 2020 2020 205b 5b30 2e2c 2030           [[0., 0
-0000b140: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
-0000b150: 302e 2c20 302e 5d2c 0a20 2020 2020 2020  0., 0.],.       
-0000b160: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
-0000b170: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
-0000b180: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-0000b190: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
-0000b1a0: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
-0000b1b0: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
-0000b1c0: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-0000b1d0: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-0000b1e0: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-0000b1f0: 2020 2020 2020 205b 302e 2c20 302e 2c20         [0., 0., 
-0000b200: 302e 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c  0., ..., 0., 0.,
-0000b210: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
-0000b220: 2020 5b30 2e2c 2030 2e2c 2030 2e2c 202e    [0., 0., 0., .
-0000b230: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d5d  .., 0., 0., 0.]]
-0000b240: 5d29 0a20 2020 203e 3e3e 2072 6573 756c  ]).    >>> resul
-0000b250: 7473 2e61 7667 5f64 6570 7468 0a20 2020  ts.avg_depth.   
-0000b260: 207b 274b 4141 273a 2031 2e33 352c 2027   {'KAA': 1.35, '
-0000b270: 4b41 4227 3a20 302e 3931 2c20 274b 4143  KAB': 0.91, 'KAC
-0000b280: 273a 2030 2e36 382c 2027 4b41 4427 3a20  ': 0.68, 'KAD': 
-0000b290: 302e 3332 2c20 274b 4145 273a 2030 2e39  0.32, 'KAE': 0.9
-0000b2a0: 392c 2027 4b41 4627 3a20 302e 3234 2c20  9, 'KAF': 0.24, 
-0000b2b0: 274b 4147 273a 2030 2e31 2c20 274b 4148  'KAG': 0.1, 'KAH
-0000b2c0: 273a 2033 2e39 312c 2027 4b41 4927 3a20  ': 3.91, 'KAI': 
-0000b2d0: 302e 302c 2027 4b41 4a27 3a20 302e 3936  0.0, 'KAJ': 0.96
-0000b2e0: 2c20 274b 414b 273a 2030 2e30 2c20 274b  , 'KAK': 0.0, 'K
-0000b2f0: 414c 273a 2031 2e30 372c 2027 4b41 4d27  AL': 1.07, 'KAM'
-0000b300: 3a20 302e 3234 2c20 274b 414e 273a 2030  : 0.24, 'KAN': 0
-0000b310: 2e30 2c20 274b 414f 273a 2030 2e32 392c  .0, 'KAO': 0.29,
-0000b320: 2027 4b41 5027 3a20 302e 372c 2027 4b41   'KAP': 0.7, 'KA
-0000b330: 5127 3a20 302e 3232 2c20 274b 4152 273a  Q': 0.22, 'KAR':
-0000b340: 2030 2e31 327d 0a20 2020 203e 3e3e 2072   0.12}.    >>> r
-0000b350: 6573 756c 7473 2e6d 6178 5f64 6570 7468  esults.max_depth
-0000b360: 0a20 2020 207b 274b 4141 273a 2033 2e37  .    {'KAA': 3.7
-0000b370: 392c 2027 4b41 4227 3a20 322e 3638 2c20  9, 'KAB': 2.68, 
-0000b380: 274b 4143 273a 2032 2e36 322c 2027 4b41  'KAC': 2.62, 'KA
-0000b390: 4427 3a20 302e 3835 2c20 274b 4145 273a  D': 0.85, 'KAE':
-0000b3a0: 2033 2e30 2c20 274b 4146 273a 2030 2e38   3.0, 'KAF': 0.8
-0000b3b0: 352c 2027 4b41 4727 3a20 302e 362c 2027  5, 'KAG': 0.6, '
-0000b3c0: 4b41 4827 3a20 3130 2e37 332c 2027 4b41  KAH': 10.73, 'KA
-0000b3d0: 4927 3a20 302e 302c 2027 4b41 4a27 3a20  I': 0.0, 'KAJ': 
-0000b3e0: 322e 3234 2c20 274b 414b 273a 2030 2e30  2.24, 'KAK': 0.0
-0000b3f0: 2c20 274b 414c 273a 2033 2e30 2c20 274b  , 'KAL': 3.0, 'K
-0000b400: 414d 273a 2031 2e32 2c20 274b 414e 273a  AM': 1.2, 'KAN':
-0000b410: 2030 2e30 2c20 274b 414f 273a 2031 2e30   0.0, 'KAO': 1.0
-0000b420: 342c 2027 4b41 5027 3a20 322e 3038 2c20  4, 'KAP': 2.08, 
-0000b430: 274b 4151 273a 2030 2e38 352c 2027 4b41  'KAQ': 0.85, 'KA
-0000b440: 5227 3a20 302e 367d 0a20 2020 203e 3e3e  R': 0.6}.    >>>
-0000b450: 2072 6573 756c 7473 2e61 7667 5f68 7964   results.avg_hyd
-0000b460: 726f 7061 7468 790a 2020 2020 7b27 4b41  ropathy.    {'KA
-0000b470: 4127 3a20 2d30 2e37 332c 2027 4b41 4227  A': -0.73, 'KAB'
-0000b480: 3a20 2d30 2e30 352c 2027 4b41 4327 3a20  : -0.05, 'KAC': 
-0000b490: 2d30 2e30 372c 2027 4b41 4427 3a20 2d30  -0.07, 'KAD': -0
-0000b4a0: 2e36 322c 2027 4b41 4527 3a20 2d30 2e38  .62, 'KAE': -0.8
-0000b4b0: 312c 2027 4b41 4627 3a20 2d30 2e31 342c  1, 'KAF': -0.14,
-0000b4c0: 2027 4b41 4727 3a20 2d30 2e33 332c 2027   'KAG': -0.33, '
-0000b4d0: 4b41 4827 3a20 2d30 2e31 372c 2027 4b41  KAH': -0.17, 'KA
-0000b4e0: 4927 3a20 2d30 2e34 2c20 274b 414a 273a  I': -0.4, 'KAJ':
-0000b4f0: 2030 2e36 322c 2027 4b41 4b27 3a20 2d30   0.62, 'KAK': -0
-0000b500: 2e39 392c 2027 4b41 4c27 3a20 302e 3336  .99, 'KAL': 0.36
-0000b510: 2c20 274b 414d 273a 202d 302e 3333 2c20  , 'KAM': -0.33, 
-0000b520: 274b 414e 273a 2030 2e31 382c 2027 4b41  'KAN': 0.18, 'KA
-0000b530: 4f27 3a20 302e 3838 2c20 274b 4150 273a  O': 0.88, 'KAP':
-0000b540: 202d 302e 3936 2c20 274b 4151 273a 2030   -0.96, 'KAQ': 0
-0000b550: 2e34 382c 2027 4b41 5227 3a20 302e 3234  .48, 'KAR': 0.24
-0000b560: 2c20 2745 6973 656e 6265 7267 5765 6973  , 'EisenbergWeis
-0000b570: 7327 3a20 5b2d 312e 3432 2c20 322e 365d  s': [-1.42, 2.6]
-0000b580: 7d0a 2020 2020 2222 220a 2020 2020 6966  }.    """.    if
-0000b590: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-0000b5a0: 2020 7072 696e 7428 223e 204c 6f61 6469    print("> Loadi
-0000b5b0: 6e67 2061 746f 6d69 6320 6469 6374 696f  ng atomic dictio
-0000b5c0: 6e61 7279 2066 696c 6522 290a 2020 2020  nary file").    
-0000b5d0: 6966 2076 6477 2069 7320 6e6f 7420 4e6f  if vdw is not No
-0000b5e0: 6e65 3a0a 2020 2020 2020 2020 7664 7720  ne:.        vdw 
-0000b5f0: 3d20 7265 6164 5f76 6477 2876 6477 290a  = read_vdw(vdw).
-0000b600: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000b610: 2020 7664 7720 3d20 7265 6164 5f76 6477    vdw = read_vdw
-0000b620: 2856 4457 290a 0a20 2020 2069 6620 7665  (VDW)..    if ve
-0000b630: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
-0000b640: 7269 6e74 2822 3e20 5265 6164 696e 6720  rint("> Reading 
-0000b650: 5044 4220 636f 6f72 6469 6e61 7465 7322  PDB coordinates"
-0000b660: 290a 2020 2020 6966 2069 6e70 7574 2e65  ).    if input.e
-0000b670: 6e64 7377 6974 6828 222e 7064 6222 293a  ndswith(".pdb"):
-0000b680: 0a20 2020 2020 2020 2061 746f 6d69 6320  .        atomic 
-0000b690: 3d20 7265 6164 5f70 6462 2869 6e70 7574  = read_pdb(input
-0000b6a0: 2c20 7664 772c 206d 6f64 656c 290a 2020  , vdw, model).  
-0000b6b0: 2020 656c 6966 2069 6e70 7574 2e65 6e64    elif input.end
-0000b6c0: 7377 6974 6828 222e 7879 7a22 293a 0a20  swith(".xyz"):. 
-0000b6d0: 2020 2020 2020 2061 746f 6d69 6320 3d20         atomic = 
-0000b6e0: 7265 6164 5f78 797a 2869 6e70 7574 2c20  read_xyz(input, 
-0000b6f0: 7664 7729 0a20 2020 2065 6c73 653a 0a20  vdw).    else:. 
-0000b700: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-0000b710: 6545 7272 6f72 2822 6074 6172 6765 7460  eError("`target`
-0000b720: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
-0000b730: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
-0000b740: 6e2e 2229 0a0a 2020 2020 6966 206c 6967  n.")..    if lig
-0000b750: 616e 643a 0a20 2020 2020 2020 2069 6620  and:.        if 
-0000b760: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-0000b770: 2020 2020 2070 7269 6e74 2822 3e20 5265       print("> Re
-0000b780: 6164 696e 6720 6c69 6761 6e64 2063 6f6f  ading ligand coo
-0000b790: 7264 696e 6174 6573 2229 0a20 2020 2020  rdinates").     
-0000b7a0: 2020 2069 6620 6c69 6761 6e64 2e65 6e64     if ligand.end
-0000b7b0: 7377 6974 6828 222e 7064 6222 293a 0a20  swith(".pdb"):. 
-0000b7c0: 2020 2020 2020 2020 2020 206c 6174 6f6d             latom
-0000b7d0: 6963 203d 2072 6561 645f 7064 6228 6c69  ic = read_pdb(li
-0000b7e0: 6761 6e64 2c20 7664 7729 0a20 2020 2020  gand, vdw).     
-0000b7f0: 2020 2065 6c69 6620 6c69 6761 6e64 2e65     elif ligand.e
-0000b800: 6e64 7377 6974 6828 222e 7879 7a22 293a  ndswith(".xyz"):
-0000b810: 0a20 2020 2020 2020 2020 2020 206c 6174  .            lat
-0000b820: 6f6d 6963 203d 2072 6561 645f 7879 7a28  omic = read_xyz(
-0000b830: 6c69 6761 6e64 2c20 7664 7729 0a20 2020  ligand, vdw).   
-0000b840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b850: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-0000b860: 6545 7272 6f72 2822 606c 6967 616e 6460  eError("`ligand`
-0000b870: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
-0000b880: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
-0000b890: 6e2e 2229 0a20 2020 2065 6c73 653a 0a20  n.").    else:. 
-0000b8a0: 2020 2020 2020 206c 6174 6f6d 6963 203d         latomic =
-0000b8b0: 204e 6f6e 650a 0a20 2020 2069 6620 7665   None..    if ve
-0000b8c0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
-0000b8d0: 7269 6e74 2822 3e20 4361 6c63 756c 6174  rint("> Calculat
-0000b8e0: 696e 6720 3344 2067 7269 6420 6469 6d65  ing 3D grid dime
-0000b8f0: 6e73 696f 6e73 2229 0a20 2020 2069 6620  nsions").    if 
-0000b900: 626f 783a 0a20 2020 2020 2020 2023 2047  box:.        # G
-0000b910: 6574 2076 6572 7469 6365 7320 6672 6f6d  et vertices from
-0000b920: 2066 696c 650a 2020 2020 2020 2020 7665   file.        ve
-0000b930: 7274 6963 6573 2c20 6174 6f6d 6963 203d  rtices, atomic =
-0000b940: 2067 6574 5f76 6572 7469 6365 735f 6672   get_vertices_fr
-0000b950: 6f6d 5f66 696c 6528 0a20 2020 2020 2020  om_file(.       
-0000b960: 2020 2020 2062 6f78 2c20 6174 6f6d 6963       box, atomic
-0000b970: 2c20 7374 6570 2c20 7072 6f62 655f 696e  , step, probe_in
-0000b980: 2c20 7072 6f62 655f 6f75 742c 206e 7468  , probe_out, nth
-0000b990: 7265 6164 730a 2020 2020 2020 2020 290a  reads.        ).
-0000b9a0: 0a20 2020 2020 2020 2023 2053 6574 2066  .        # Set f
-0000b9b0: 6c61 6720 746f 2062 6f6f 6c65 616e 0a20  lag to boolean. 
-0000b9c0: 2020 2020 2020 2062 6f78 203d 2054 7275         box = Tru
-0000b9d0: 650a 2020 2020 656c 7365 3a0a 2020 2020  e.    else:.    
-0000b9e0: 2020 2020 2320 4765 7420 7665 7274 6963      # Get vertic
-0000b9f0: 6573 2066 726f 6d20 696e 7075 740a 2020  es from input.  
-0000ba00: 2020 2020 2020 7665 7274 6963 6573 203d        vertices =
-0000ba10: 2067 6574 5f76 6572 7469 6365 7328 6174   get_vertices(at
-0000ba20: 6f6d 6963 2c20 7072 6f62 655f 6f75 742c  omic, probe_out,
-0000ba30: 2073 7465 7029 0a0a 2020 2020 2020 2020   step)..        
-0000ba40: 2320 5365 7420 666c 6167 2074 6f20 626f  # Set flag to bo
-0000ba50: 6f6c 6561 6e0a 2020 2020 2020 2020 626f  olean.        bo
-0000ba60: 7820 3d20 4661 6c73 650a 0a20 2020 2023  x = False..    #
-0000ba70: 2043 616c 6375 6c61 7465 2064 6973 7461   Calculate dista
-0000ba80: 6e63 6520 6265 7477 6565 6e20 706f 696e  nce between poin
-0000ba90: 7473 0a20 2020 206e 782c 206e 792c 206e  ts.    nx, ny, n
-0000baa0: 7a20 3d20 5f67 6574 5f64 696d 656e 7369  z = _get_dimensi
-0000bab0: 6f6e 7328 7665 7274 6963 6573 2c20 7374  ons(vertices, st
-0000bac0: 6570 290a 2020 2020 6966 2076 6572 626f  ep).    if verbo
-0000bad0: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
-0000bae0: 7428 6622 4469 6d65 6e73 696f 6e73 3a20  t(f"Dimensions: 
-0000baf0: 286e 783a 7b6e 787d 2c20 6e79 3a7b 6e79  (nx:{nx}, ny:{ny
-0000bb00: 7d2c 206e 7a3a 7b6e 7a7d 2922 290a 0a20  }, nz:{nz})").. 
-0000bb10: 2020 2023 2043 616c 6375 6c61 7465 2073     # Calculate s
-0000bb20: 696e 2061 6e64 2063 6f73 206f 6620 616e  in and cos of an
-0000bb30: 676c 6573 2061 2061 6e64 2062 0a20 2020  gles a and b.   
-0000bb40: 2073 696e 636f 7320 3d20 5f67 6574 5f73   sincos = _get_s
-0000bb50: 696e 636f 7328 7665 7274 6963 6573 290a  incos(vertices).
-0000bb60: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-0000bb70: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-0000bb80: 7369 6e61 3a20 7b73 696e 636f 735b 305d  sina: {sincos[0]
-0000bb90: 3a2e 3266 7d5c 7473 696e 623a 207b 7369  :.2f}\tsinb: {si
-0000bba0: 6e63 6f73 5b32 5d3a 2e32 667d 2229 0a20  ncos[2]:.2f}"). 
-0000bbb0: 2020 2020 2020 2070 7269 6e74 2866 2263         print(f"c
-0000bbc0: 6f73 613a 207b 7369 6e63 6f73 5b31 5d3a  osa: {sincos[1]:
-0000bbd0: 2e32 667d 5c74 636f 7362 3a20 7b73 696e  .2f}\tcosb: {sin
-0000bbe0: 636f 735b 335d 3a2e 3266 7d22 290a 0a20  cos[3]:.2f}").. 
-0000bbf0: 2020 2023 2043 6176 6974 7920 6465 7465     # Cavity dete
-0000bc00: 6374 696f 6e0a 2020 2020 6e63 6176 2c20  ction.    ncav, 
-0000bc10: 6361 7669 7469 6573 203d 2064 6574 6563  cavities = detec
-0000bc20: 7428 0a20 2020 2020 2020 2061 746f 6d69  t(.        atomi
-0000bc30: 632c 0a20 2020 2020 2020 2076 6572 7469  c,.        verti
-0000bc40: 6365 732c 0a20 2020 2020 2020 2073 7465  ces,.        ste
-0000bc50: 702c 0a20 2020 2020 2020 2070 726f 6265  p,.        probe
-0000bc60: 5f69 6e2c 0a20 2020 2020 2020 2070 726f  _in,.        pro
-0000bc70: 6265 5f6f 7574 2c0a 2020 2020 2020 2020  be_out,.        
-0000bc80: 7265 6d6f 7661 6c5f 6469 7374 616e 6365  removal_distance
-0000bc90: 2c0a 2020 2020 2020 2020 766f 6c75 6d65  ,.        volume
-0000bca0: 5f63 7574 6f66 662c 0a20 2020 2020 2020  _cutoff,.       
-0000bcb0: 206c 6174 6f6d 6963 2c0a 2020 2020 2020   latomic,.      
-0000bcc0: 2020 6c69 6761 6e64 5f63 7574 6f66 662c    ligand_cutoff,
-0000bcd0: 0a20 2020 2020 2020 2062 6f78 2c0a 2020  .        box,.  
-0000bce0: 2020 2020 2020 7375 7266 6163 652c 0a20        surface,. 
-0000bcf0: 2020 2020 2020 206e 7468 7265 6164 732c         nthreads,
-0000bd00: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
-0000bd10: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
-0000bd20: 6e63 6176 203e 2030 3a0a 2020 2020 2020  ncav > 0:.      
-0000bd30: 2020 2320 5370 6174 6961 6c20 6368 6172    # Spatial char
-0000bd40: 6163 7465 7269 7a61 7469 6f6e 0a20 2020  acterization.   
-0000bd50: 2020 2020 2073 7572 6661 6365 2c20 766f       surface, vo
-0000bd60: 6c75 6d65 2c20 6172 6561 203d 2073 7061  lume, area = spa
-0000bd70: 7469 616c 2863 6176 6974 6965 732c 2073  tial(cavities, s
-0000bd80: 7465 702c 204e 6f6e 652c 206e 7468 7265  tep, None, nthre
-0000bd90: 6164 732c 2076 6572 626f 7365 290a 0a20  ads, verbose).. 
-0000bda0: 2020 2020 2020 2023 2043 6f6e 7374 6974         # Constit
-0000bdb0: 7574 696f 6e61 6c20 6368 6172 6163 7465  utional characte
-0000bdc0: 7269 7a61 7469 6f6e 0a20 2020 2020 2020  rization.       
-0000bdd0: 2072 6573 6964 7565 7320 3d20 636f 6e73   residues = cons
-0000bde0: 7469 7475 7469 6f6e 616c 280a 2020 2020  titutional(.    
-0000bdf0: 2020 2020 2020 2020 6361 7669 7469 6573          cavities
-0000be00: 2c0a 2020 2020 2020 2020 2020 2020 6174  ,.            at
-0000be10: 6f6d 6963 2c0a 2020 2020 2020 2020 2020  omic,.          
-0000be20: 2020 7665 7274 6963 6573 2c0a 2020 2020    vertices,.    
-0000be30: 2020 2020 2020 2020 7374 6570 2c0a 2020          step,.  
-0000be40: 2020 2020 2020 2020 2020 7072 6f62 655f            probe_
-0000be50: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
-0000be60: 6967 6e6f 7265 5f62 6163 6b62 6f6e 652c  ignore_backbone,
-0000be70: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
-0000be80: 652c 0a20 2020 2020 2020 2020 2020 206e  e,.            n
-0000be90: 7468 7265 6164 732c 0a20 2020 2020 2020  threads,.       
-0000bea0: 2020 2020 2076 6572 626f 7365 2c0a 2020       verbose,.  
-0000beb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000bec0: 6672 6571 7565 6e63 6965 7320 3d20 6361  frequencies = ca
-0000bed0: 6c63 756c 6174 655f 6672 6571 7565 6e63  lculate_frequenc
-0000bee0: 6965 7328 7265 7369 6475 6573 290a 0a20  ies(residues).. 
-0000bef0: 2020 2020 2020 2023 2044 6570 7468 2063         # Depth c
-0000bf00: 6861 7261 6374 6572 697a 6174 696f 6e0a  haracterization.
-0000bf10: 2020 2020 2020 2020 6966 2069 6e63 6c75          if inclu
-0000bf20: 6465 5f64 6570 7468 3a0a 2020 2020 2020  de_depth:.      
-0000bf30: 2020 2020 2020 6465 7074 6873 2c20 6d61        depths, ma
-0000bf40: 785f 6465 7074 682c 2061 7667 5f64 6570  x_depth, avg_dep
-0000bf50: 7468 203d 2064 6570 7468 280a 2020 2020  th = depth(.    
-0000bf60: 2020 2020 2020 2020 2020 2020 6361 7669              cavi
-0000bf70: 7469 6573 2c20 7374 6570 2c20 4e6f 6e65  ties, step, None
-0000bf80: 2c20 6e74 6872 6561 6473 2c20 7665 7262  , nthreads, verb
-0000bf90: 6f73 650a 2020 2020 2020 2020 2020 2020  ose.            
-0000bfa0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000bfb0: 2020 2020 2020 2020 2020 2020 6465 7074              dept
-0000bfc0: 6873 2c20 6d61 785f 6465 7074 682c 2061  hs, max_depth, a
-0000bfd0: 7667 5f64 6570 7468 203d 204e 6f6e 652c  vg_depth = None,
-0000bfe0: 204e 6f6e 652c 204e 6f6e 650a 0a20 2020   None, None..   
-0000bff0: 2020 2020 2023 2048 7964 726f 7061 7468       # Hydropath
-0000c000: 7920 6879 6472 6f70 686f 6269 6369 7479  y hydrophobicity
-0000c010: 2073 6361 6c65 730a 2020 2020 2020 2020   scales.        
-0000c020: 6966 2069 6e63 6c75 6465 5f68 7964 726f  if include_hydro
-0000c030: 7061 7468 793a 0a20 2020 2020 2020 2020  pathy:.         
-0000c040: 2020 2073 6361 6c65 732c 2061 7667 5f68     scales, avg_h
-0000c050: 7964 726f 7061 7468 7920 3d20 6879 6472  ydropathy = hydr
-0000c060: 6f70 6174 6879 280a 2020 2020 2020 2020  opathy(.        
-0000c070: 2020 2020 2020 2020 7375 7266 6163 652c          surface,
-0000c080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c090: 2061 746f 6d69 632c 0a20 2020 2020 2020   atomic,.       
-0000c0a0: 2020 2020 2020 2020 2076 6572 7469 6365           vertice
-0000c0b0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000c0c0: 2020 2073 7465 702c 0a20 2020 2020 2020     step,.       
-0000c0d0: 2020 2020 2020 2020 2070 726f 6265 5f69           probe_i
-0000c0e0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0000c0f0: 2020 2068 7964 726f 7068 6f62 6963 6974     hydrophobicit
-0000c100: 795f 7363 616c 652c 0a20 2020 2020 2020  y_scale,.       
-0000c110: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
-0000c120: 6261 636b 626f 6e65 2c0a 2020 2020 2020  backbone,.      
-0000c130: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 6e74 6872 6561 6473 2c0a 2020 2020 2020  nthreads,.      
-0000c160: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-0000c170: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-0000c180: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000c190: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-0000c1a0: 732c 2061 7667 5f68 7964 726f 7061 7468  s, avg_hydropath
-0000c1b0: 7920 3d20 4e6f 6e65 2c20 4e6f 6e65 0a20  y = None, None. 
-0000c1c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c1d0: 2070 7269 6e74 2822 5761 726e 696e 673a   print("Warning:
-0000c1e0: 204e 6f20 6361 7669 7469 6573 2064 6574   No cavities det
-0000c1f0: 6563 7465 642c 2072 6574 7572 6e69 6e67  ected, returning
-0000c200: 204e 6f6e 6521 2229 0a20 2020 2020 2020   None!").       
-0000c210: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-0000c220: 2020 2320 5265 7475 726e 2064 6963 740a    # Return dict.
-0000c230: 2020 2020 7265 7375 6c74 7320 3d20 7079      results = py
-0000c240: 4b56 4669 6e64 6572 5265 7375 6c74 7328  KVFinderResults(
-0000c250: 0a20 2020 2020 2020 2063 6176 6974 6965  .        cavitie
-0000c260: 732c 0a20 2020 2020 2020 2073 7572 6661  s,.        surfa
-0000c270: 6365 2c0a 2020 2020 2020 2020 6465 7074  ce,.        dept
-0000c280: 6873 2c0a 2020 2020 2020 2020 7363 616c  hs,.        scal
-0000c290: 6573 2c0a 2020 2020 2020 2020 766f 6c75  es,.        volu
-0000c2a0: 6d65 2c0a 2020 2020 2020 2020 6172 6561  me,.        area
-0000c2b0: 2c0a 2020 2020 2020 2020 6d61 785f 6465  ,.        max_de
-0000c2c0: 7074 682c 0a20 2020 2020 2020 2061 7667  pth,.        avg
-0000c2d0: 5f64 6570 7468 2c0a 2020 2020 2020 2020  _depth,.        
-0000c2e0: 6176 675f 6879 6472 6f70 6174 6879 2c0a  avg_hydropathy,.
-0000c2f0: 2020 2020 2020 2020 7265 7369 6475 6573          residues
-0000c300: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
-0000c310: 6e63 6965 732c 0a20 2020 2020 2020 2076  ncies,.        v
-0000c320: 6572 7469 6365 732c 0a20 2020 2020 2020  ertices,.       
-0000c330: 2073 7465 702c 0a20 2020 2020 2020 2069   step,.        i
-0000c340: 6e70 7574 2c0a 2020 2020 2020 2020 6c69  nput,.        li
-0000c350: 6761 6e64 2c0a 2020 2020 290a 0a20 2020  gand,.    )..   
-0000c360: 2072 6574 7572 6e20 7265 7375 6c74 730a   return results.
-0000c370: 0a0a 636c 6173 7320 4d6f 6c65 6375 6c65  ..class Molecule
-0000c380: 286f 626a 6563 7429 3a0a 2020 2020 2222  (object):.    ""
-0000c390: 2241 2063 6c61 7373 2066 6f72 2072 6570  "A class for rep
-0000c3a0: 7265 7365 6e74 696e 6720 6d6f 6c65 6375  resenting molecu
-0000c3b0: 6c61 7220 7374 7275 6374 7572 6573 2e0a  lar structures..
-0000c3c0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-0000c3d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000c3e0: 2020 206d 6f6c 6563 756c 6520 3a20 556e     molecule : Un
-0000c3f0: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-0000c400: 2e50 6174 685d 0a20 2020 2020 2020 2041  .Path].        A
-0000c410: 2066 696c 6520 7061 7468 2074 6f20 7468   file path to th
-0000c420: 6520 6d6f 6c65 6375 6c65 2069 6e20 6569  e molecule in ei
-0000c430: 7468 6572 2050 4442 206f 7220 5859 5a20  ther PDB or XYZ 
-0000c440: 666f 726d 6174 0a20 2020 2072 6164 6969  format.    radii
-0000c450: 203a 2055 6e69 6f6e 5b73 7472 2c20 7061   : Union[str, pa
-0000c460: 7468 6c69 622e 5061 7468 2c20 4469 6374  thlib.Path, Dict
-0000c470: 5b73 7472 2c20 416e 795d 5d2c 206f 7074  [str, Any]], opt
-0000c480: 696f 6e61 6c0a 2020 2020 2020 2020 4120  ional.        A 
-0000c490: 6669 6c65 2070 6174 6820 746f 2061 2076  file path to a v
-0000c4a0: 616e 2064 6572 2057 6161 6c73 2072 6164  an der Waals rad
-0000c4b0: 6969 2066 696c 6520 6f72 2061 2064 6963  ii file or a dic
-0000c4c0: 7469 6f6e 6172 7920 6f66 2056 4457 2072  tionary of VDW r
-0000c4d0: 6164 6969 2c20 6279 2064 6566 6175 6c74  adii, by default
-0000c4e0: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
-0000c4f0: 6170 706c 7920 7468 6520 6275 696c 742d  apply the built-
-0000c500: 696e 2076 616e 2064 6572 2057 6161 6c73  in van der Waals
-0000c510: 2072 6164 6969 2066 696c 653a 2060 7664   radii file: `vd
-0000c520: 772e 6461 7460 2e0a 2020 2020 6d6f 6465  w.dat`..    mode
-0000c530: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
-0000c540: 6c0a 2020 2020 2020 2020 5468 6520 6d6f  l.        The mo
-0000c550: 6465 6c20 6e75 6d62 6572 206f 6620 6120  del number of a 
-0000c560: 6d75 6c74 692d 6d6f 6465 6c20 5044 4220  multi-model PDB 
-0000c570: 6669 6c65 2c20 6279 2064 6566 6175 6c74  file, by default
-0000c580: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
-0000c590: 6b65 6570 2061 746f 6d73 2066 726f 6d20  keep atoms from 
-0000c5a0: 616c 6c20 6d6f 6465 6c73 2e0a 2020 2020  all models..    
-0000c5b0: 6e74 6872 6561 6473 203a 2069 6e74 2c20  nthreads : int, 
-0000c5c0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0000c5d0: 204e 756d 6265 7220 6f66 2074 6872 6561   Number of threa
-0000c5e0: 6473 2c20 6279 2064 6566 6175 6c74 204e  ds, by default N
-0000c5f0: 6f6e 652e 2049 6620 4e6f 6e65 2c20 7468  one. If None, th
-0000c600: 6520 6e75 6d62 6572 206f 6620 7468 7265  e number of thre
-0000c610: 6164 7320 6973 2060 6f73 2e63 7075 5f63  ads is `os.cpu_c
-0000c620: 6f75 6e74 2829 202d 2031 602e 0a20 2020  ount() - 1`..   
-0000c630: 2076 6572 626f 7365 203a 2062 6f6f 6c2c   verbose : bool,
-0000c640: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000c650: 2020 5072 696e 7420 6578 7472 6120 696e    Print extra in
-0000c660: 666f 726d 6174 696f 6e20 746f 2073 7461  formation to sta
-0000c670: 6e64 6172 6420 6f75 7470 7574 2c20 6279  ndard output, by
-0000c680: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
-0000c690: 0a20 2020 2041 7474 7269 6275 7465 730a  .    Attributes.
-0000c6a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000c6b0: 2020 205f 6174 6f6d 6963 203a 206e 756d     _atomic : num
-0000c6c0: 7079 2e6e 6461 7272 6179 0a20 2020 2020  py.ndarray.     
-0000c6d0: 2020 2041 206e 756d 7079 2061 7272 6179     A numpy array
-0000c6e0: 2077 6974 6820 6174 6f6d 6963 2064 6174   with atomic dat
-0000c6f0: 6120 2872 6573 6964 7565 206e 756d 6265  a (residue numbe
-0000c700: 722c 2063 6861 696e 2c20 7265 7369 6475  r, chain, residu
-0000c710: 6520 6e61 6d65 2c20 6174 6f6d 206e 616d  e name, atom nam
-0000c720: 652c 2078 797a 2063 6f6f 7264 696e 6174  e, xyz coordinat
-0000c730: 6573 2061 6e64 2072 6164 6975 7329 2066  es and radius) f
-0000c740: 6f72 2065 6163 6820 6174 6f6d 2e0a 2020  or each atom..  
-0000c750: 2020 5f64 696d 203a 2074 7570 6c65 0a20    _dim : tuple. 
-0000c760: 2020 2020 2020 2047 7269 6420 6469 6d65         Grid dime
-0000c770: 6e73 696f 6e73 2e0a 2020 2020 5f67 7269  nsions..    _gri
-0000c780: 6420 3a20 6e75 6d70 792e 6e64 6172 7261  d : numpy.ndarra
-0000c790: 790a 2020 2020 2020 2020 4d6f 6c65 6375  y.        Molecu
-0000c7a0: 6c65 2070 6f69 6e74 7320 696e 2074 6865  le points in the
-0000c7b0: 2033 4420 6772 6964 2028 6772 6964 5b6e   3D grid (grid[n
-0000c7c0: 785d 5b6e 795d 5b6e 7a5d 292e 0a20 2020  x][ny][nz])..   
-0000c7d0: 2020 2020 2047 7269 6420 6172 7261 7920       Grid array 
-0000c7e0: 6861 7320 696e 7465 6765 7220 6c61 6265  has integer labe
-0000c7f0: 6c73 2069 6e20 6561 6368 2070 6f73 6974  ls in each posit
-0000c800: 696f 6e2c 2074 6861 7420 6172 653a 0a0a  ion, that are:..
-0000c810: 2020 2020 2020 2020 2020 2020 2a20 303a              * 0:
-0000c820: 206d 6f6c 6563 756c 6520 706f 696e 7473   molecule points
-0000c830: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
-0000c840: 2031 3a20 736f 6c76 656e 7420 706f 696e   1: solvent poin
-0000c850: 7473 2e0a 2020 2020 5f6d 6f6c 6563 756c  ts..    _molecul
-0000c860: 6520 3a20 556e 696f 6e5b 7374 722c 2070  e : Union[str, p
-0000c870: 6174 686c 6962 2e50 6174 685d 0a20 2020  athlib.Path].   
-0000c880: 2020 2020 2041 2066 696c 6520 7061 7468       A file path
-0000c890: 2074 6f20 7468 6520 6d6f 6c65 6375 6c65   to the molecule
-0000c8a0: 2069 6e20 6569 7468 6572 2050 4442 206f   in either PDB o
-0000c8b0: 7220 5859 5a20 666f 726d 6174 2e0a 2020  r XYZ format..  
-0000c8c0: 2020 5f70 6164 6469 6e67 203a 2066 6c6f    _padding : flo
-0000c8d0: 6174 0a20 2020 2020 2020 2054 6865 206c  at.        The l
-0000c8e0: 656e 6774 6820 746f 2061 6464 2074 6f20  ength to add to 
-0000c8f0: 6561 6368 2064 6972 6563 7469 6f6e 206f  each direction o
-0000c900: 6620 7468 6520 3344 2067 7269 642e 0a20  f the 3D grid.. 
-0000c910: 2020 205f 7072 6f62 6520 3a20 666c 6f61     _probe : floa
-0000c920: 740a 2020 2020 2020 2020 5370 6865 7269  t.        Spheri
-0000c930: 6361 6c20 7072 6f62 6520 7369 7a65 2074  cal probe size t
-0000c940: 6f20 6465 6669 6e65 2074 6865 206d 6f6c  o define the mol
-0000c950: 6563 756c 6172 2073 7572 6661 6365 2062  ecular surface b
-0000c960: 6173 6564 206f 6e20 6120 6d6f 6c65 6375  ased on a molecu
-0000c970: 6c61 7220 7265 7072 6573 656e 7461 7469  lar representati
-0000c980: 6f6e 2e0a 2020 2020 5f72 6164 6969 203a  on..    _radii :
-0000c990: 2044 6963 745b 7374 722c 2041 6e79 5d0a   Dict[str, Any].
-0000c9a0: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-0000c9b0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-0000c9c0: 7261 6469 6920 7661 6c75 6573 2c20 6279  radii values, by
-0000c9d0: 2064 6566 6175 6c74 204e 6f6e 652e 0a20   default None.. 
-0000c9e0: 2020 205f 7265 7072 6573 656e 7461 7469     _representati
-0000c9f0: 6f6e 203a 2073 7472 2c20 6f70 7469 6f6e  on : str, option
-0000ca00: 616c 0a20 2020 2020 2020 204d 6f6c 6563  al.        Molec
-0000ca10: 756c 6172 2073 7572 6661 6365 2072 6570  ular surface rep
-0000ca20: 7265 7365 6e74 6174 696f 6e2e 204b 6579  resentation. Key
-0000ca30: 776f 7264 7320 6f70 7469 6f6e 7320 6172  words options ar
-0000ca40: 6520 7664 5720 2876 616e 2064 6572 2057  e vdW (van der W
-0000ca50: 6161 6c73 2073 7572 6661 6365 292c 2053  aals surface), S
-0000ca60: 4553 2028 536f 6c76 656e 7420 4578 636c  ES (Solvent Excl
-0000ca70: 7564 6564 2053 7572 6661 6365 2920 6f72  uded Surface) or
-0000ca80: 2053 4153 2028 536f 6c76 656e 7420 4163   SAS (Solvent Ac
-0000ca90: 6365 7373 6962 6c65 2053 7572 6661 6365  cessible Surface
-0000caa0: 292c 2062 7920 6465 6661 756c 7420 5345  ), by default SE
-0000cab0: 532e 0a20 2020 205f 726f 7461 7469 6f6e  S..    _rotation
-0000cac0: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-0000cad0: 0a20 2020 2020 2020 2041 206e 756d 7079  .        A numpy
-0000cae0: 2e6e 6461 7272 6179 2077 6974 6820 7369  .ndarray with si
-0000caf0: 6e65 2061 6e64 2063 6f73 7369 6e65 206f  ne and cossine o
-0000cb00: 6620 7468 6520 6772 6964 2072 6f74 6174  f the grid rotat
-0000cb10: 696f 6e20 616e 676c 6573 2028 7369 6e61  ion angles (sina
-0000cb20: 2c20 636f 7361 2c20 7369 6e62 2c20 636f  , cosa, sinb, co
-0000cb30: 7362 292e 0a20 2020 205f 7374 6570 203a  sb)..    _step :
-0000cb40: 2066 6c6f 6174 0a20 2020 2020 2020 2047   float.        G
-0000cb50: 7269 6420 7370 6163 696e 6720 2841 292e  rid spacing (A).
-0000cb60: 0a20 2020 205f 7665 7274 6963 6573 203a  .    _vertices :
-0000cb70: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
-0000cb80: 2020 2020 2020 2041 206e 756d 7079 2e6e         A numpy.n
-0000cb90: 6461 7272 6179 206f 7220 6120 6c69 7374  darray or a list
-0000cba0: 2077 6974 6820 7879 7a20 7665 7274 6963   with xyz vertic
-0000cbb0: 6573 2063 6f6f 7264 696e 6174 6573 2028  es coordinates (
-0000cbc0: 6f72 6967 696e 2c20 582d 6178 6973 2c20  origin, X-axis, 
-0000cbd0: 592d 6178 6973 2c20 5a2d 6178 6973 292e  Y-axis, Z-axis).
-0000cbe0: 0a20 2020 206e 7468 7265 6164 7320 3a20  .    nthreads : 
-0000cbf0: 696e 740a 2020 2020 2020 2020 4e75 6d62  int.        Numb
-0000cc00: 6572 206f 6620 7468 7265 6164 7320 666f  er of threads fo
-0000cc10: 7220 7061 7261 6c6c 656c 2070 726f 6365  r parallel proce
-0000cc20: 7373 696e 672e 0a20 2020 2076 6572 626f  ssing..    verbo
-0000cc30: 7365 203a 2062 6f6f 6c0a 2020 2020 2020  se : bool.      
-0000cc40: 2020 5768 6574 6865 7220 746f 2070 7269    Whether to pri
-0000cc50: 6e74 2065 7874 7261 2069 6e66 6f72 6d61  nt extra informa
-0000cc60: 7469 6f6e 2074 6f20 7374 616e 6461 7264  tion to standard
-0000cc70: 206f 7574 7075 742e 0a0a 2020 2020 4e6f   output...    No
-0000cc80: 7465 0a20 2020 202d 2d2d 2d0a 2020 2020  te.    ----.    
-0000cc90: 5468 6520 7661 6e20 6465 7220 5761 616c  The van der Waal
-0000cca0: 7320 7261 6469 6920 6669 6c65 2064 6566  s radii file def
-0000ccb0: 696e 6573 2074 6865 2072 6164 6975 7320  ines the radius 
-0000ccc0: 7661 6c75 6573 2066 6f72 2065 6163 6820  values for each 
-0000ccd0: 6174 6f6d 2062 7920 7265 7369 6475 6520  atom by residue 
-0000cce0: 616e 6420 7768 656e 206e 6f74 2064 6566  and when not def
-0000ccf0: 696e 6564 2c20 6974 2075 7365 7320 6120  ined, it uses a 
-0000cd00: 6765 6e65 7269 6320 7661 6c75 6520 6261  generic value ba
-0000cd10: 7365 6420 6f6e 2074 6865 2061 746f 6d20  sed on the atom 
-0000cd20: 7479 7065 2e20 5468 6520 6675 6e63 7469  type. The functi
-0000cd30: 6f6e 2062 7920 6465 6661 756c 7420 6c6f  on by default lo
-0000cd40: 6164 7320 7468 6520 6275 696c 742d 696e  ads the built-in
-0000cd50: 2076 616e 2064 6572 2057 6161 6c73 2072   van der Waals r
-0000cd60: 6164 6969 2066 696c 653a 2060 6076 6477  adii file: ``vdw
-0000cd70: 2e64 6174 6060 2e0a 0a20 2020 2053 6565  .dat``...    See
-0000cd80: 2041 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d   Also.    ------
-0000cd90: 2d2d 0a20 2020 2072 6561 645f 7664 770a  --.    read_vdw.
-0000cda0: 0a20 2020 2045 7861 6d70 6c65 0a20 2020  .    Example.   
-0000cdb0: 202d 2d2d 2d2d 2d2d 0a20 2020 2054 6865   -------.    The
-0000cdc0: 2060 604d 6f6c 6563 756c 6560 6020 636c   ``Molecule`` cl
-0000cdd0: 6173 7320 6c6f 6164 7320 7468 6520 7461  ass loads the ta
-0000cde0: 7267 6574 206d 6f6c 6563 756c 6172 2073  rget molecular s
-0000cdf0: 7472 7563 7475 7265 2028 436c 4f34 2920  tructure (ClO4) 
-0000ce00: 696e 746f 2070 794b 5646 696e 6465 722e  into pyKVFinder.
-0000ce10: 2063 6c61 7373 2e0a 0a20 2020 203e 3e3e   class...    >>>
-0000ce20: 2069 6d70 6f72 7420 6f73 0a20 2020 203e   import os.    >
-0000ce30: 3e3e 2066 726f 6d20 7079 4b56 4669 6e64  >> from pyKVFind
-0000ce40: 6572 2069 6d70 6f72 7420 4d6f 6c65 6375  er import Molecu
-0000ce50: 6c65 0a20 2020 203e 3e3e 2070 6462 203d  le.    >>> pdb =
-0000ce60: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
-0000ce70: 2e70 6174 682e 6469 726e 616d 6528 7079  .path.dirname(py
-0000ce80: 4b56 4669 6e64 6572 2e5f 5f66 696c 655f  KVFinder.__file_
-0000ce90: 5f29 2c20 2764 6174 6127 2c20 2774 6573  _), 'data', 'tes
-0000cea0: 7473 272c 2027 436c 4f34 2e70 6462 2729  ts', 'ClO4.pdb')
-0000ceb0: 0a20 2020 203e 3e3e 206d 6f6c 6563 756c  .    >>> molecul
-0000cec0: 6520 3d20 4d6f 6c65 6375 6c65 2870 6462  e = Molecule(pdb
-0000ced0: 290a 2020 2020 3e3e 3e20 6d6f 6c65 6375  ).    >>> molecu
-0000cee0: 6c65 0a20 2020 203e 3e3e 203c 7079 4b56  le.    >>> <pyKV
-0000cef0: 4669 6e64 6572 2e6d 6169 6e2e 4d6f 6c65  Finder.main.Mole
-0000cf00: 6375 6c65 206f 626a 6563 7420 6174 2030  cule object at 0
-0000cf10: 7837 6635 6464 6163 6632 3233 303e 0a0a  x7f5ddacf2230>..
-0000cf20: 2020 2020 5468 6520 7661 6e20 6465 7220      The van der 
-0000cf30: 5761 616c 7320 7261 6469 6920 6361 6e20  Waals radii can 
-0000cf40: 6265 2064 6566 696e 6520 6279 3a0a 0a20  be define by:.. 
-0000cf50: 2020 2020 2020 202a 2063 7265 6174 696e         * creatin
-0000cf60: 6720 6120 5079 7468 6f6e 2064 6963 7469  g a Python dicti
-0000cf70: 6f6e 6172 793a 0a0a 2020 2020 2020 2020  onary:..        
-0000cf80: 3e3e 3e20 2320 5079 4d4f 4c20 2876 322e  >>> # PyMOL (v2.
-0000cf90: 352e 3029 2076 6457 2072 6164 6969 2076  5.0) vdW radii v
-0000cfa0: 616c 7565 730a 2020 2020 2020 2020 3e3e  alues.        >>
-0000cfb0: 3e20 7664 7720 3d20 7b27 4745 4e27 3a20  > vdw = {'GEN': 
-0000cfc0: 7b27 434c 273a 2031 2e37 352c 2027 4f27  {'CL': 1.75, 'O'
-0000cfd0: 3a20 312e 3532 7d7d 0a20 2020 2020 2020  : 1.52}}.       
-0000cfe0: 203e 3e3e 206d 6f6c 6563 756c 6520 3d20   >>> molecule = 
-0000cff0: 4d6f 6c65 6375 6c65 2870 6462 2c20 7261  Molecule(pdb, ra
-0000d000: 6469 693d 7664 7729 0a20 2020 2020 2020  dii=vdw).       
-0000d010: 203e 3e3e 206d 6f6c 6563 756c 652e 7261   >>> molecule.ra
-0000d020: 6469 690a 2020 2020 2020 2020 7b27 4745  dii.        {'GE
-0000d030: 4e27 3a20 7b27 434c 273a 2031 2e37 352c  N': {'CL': 1.75,
-0000d040: 2027 4f27 3a20 312e 3532 7d7d 0a0a 2020   'O': 1.52}}..  
-0000d050: 2020 2020 2020 2a20 7370 6563 6966 7969        * specifyi
-0000d060: 6e67 2061 202a 2e64 6174 2a20 6669 6c65  ng a *.dat* file
-0000d070: 2066 6f6c 6c6f 7769 6e67 2074 656d 706c   following templ
-0000d080: 6174 6520 6f66 2060 7661 6e20 6465 7220  ate of `van der 
-0000d090: 5761 616c 7320 7261 6469 6920 6669 6c65  Waals radii file
-0000d0a0: 602e 0a0a 2020 2020 2020 2020 3e3e 3e20  `...        >>> 
-0000d0b0: 6672 6f6d 2070 794b 5646 696e 6465 7220  from pyKVFinder 
-0000d0c0: 696d 706f 7274 2072 6561 645f 7664 770a  import read_vdw.
-0000d0d0: 2020 2020 2020 2020 3e3e 3e20 2320 4368          >>> # Ch
-0000d0e0: 696d 6572 6158 2076 6457 2072 6164 6969  imeraX vdW radii
-0000d0f0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-0000d100: 3e3e 3e20 7769 7468 206f 7065 6e28 2776  >>> with open('v
-0000d110: 6477 2e64 6174 272c 2027 7727 2920 6173  dw.dat', 'w') as
-0000d120: 2066 3a0a 2020 2020 2020 2020 2e2e 2e20   f:.        ... 
-0000d130: 2020 2020 662e 7772 6974 6528 273e 4745      f.write('>GE
-0000d140: 4e5c 5c6e 434c 5c5c 745c 5c74 312e 3938  N\\nCL\\t\\t1.98
-0000d150: 5c5c 6e4f 5c5c 745c 5c74 312e 3436 5c5c  \\nO\\t\\t1.46\\
-0000d160: 6e27 290a 2020 2020 2020 2020 3e3e 3e20  n').        >>> 
-0000d170: 7664 7720 3d20 7265 6164 5f76 6477 2827  vdw = read_vdw('
-0000d180: 7664 772e 6461 7427 290a 2020 2020 2020  vdw.dat').      
-0000d190: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 203d    >>> molecule =
-0000d1a0: 204d 6f6c 6563 756c 6528 7064 622c 2072   Molecule(pdb, r
-0000d1b0: 6164 6969 3d76 6477 290a 2020 2020 2020  adii=vdw).      
-0000d1c0: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 2e72    >>> molecule.r
-0000d1d0: 6164 6969 0a20 2020 2020 2020 207b 2747  adii.        {'G
-0000d1e0: 454e 273a 207b 2743 4c27 3a20 312e 3938  EN': {'CL': 1.98
-0000d1f0: 2c20 274f 273a 2031 2e34 367d 7d0a 2020  , 'O': 1.46}}.  
-0000d200: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-0000d210: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000d220: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
-0000d230: 6f6c 6563 756c 653a 2055 6e69 6f6e 5b73  olecule: Union[s
-0000d240: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
-0000d250: 5d2c 0a20 2020 2020 2020 2072 6164 6969  ],.        radii
-0000d260: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
-0000d270: 686c 6962 2e50 6174 682c 2044 6963 745b  hlib.Path, Dict[
-0000d280: 7374 722c 2041 6e79 5d5d 203d 204e 6f6e  str, Any]] = Non
-0000d290: 652c 0a20 2020 2020 2020 206d 6f64 656c  e,.        model
-0000d2a0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0000d2b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000d2c0: 6e74 6872 6561 6473 3a20 4f70 7469 6f6e  nthreads: Option
-0000d2d0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-0000d2e0: 2020 2020 2020 2020 7665 7262 6f73 653a          verbose:
-0000d2f0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0000d300: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000d310: 2249 6e69 7469 616c 697a 6520 7468 6520  "Initialize the 
-0000d320: 4d6f 6c65 6375 6c65 206f 626a 6563 7420  Molecule object 
-0000d330: 7769 7468 206d 6f6c 6563 756c 652c 2072  with molecule, r
-0000d340: 6164 6969 2c20 6d6f 6465 6c2c 206e 7468  adii, model, nth
-0000d350: 7265 6164 7320 616e 6420 7665 7262 6f73  reads and verbos
-0000d360: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-0000d370: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000d380: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000d390: 2020 6d6f 6c65 6375 6c65 203a 2055 6e69    molecule : Uni
-0000d3a0: 6f6e 5b73 7472 2c20 7061 7468 6c69 622e  on[str, pathlib.
-0000d3b0: 5061 7468 5d0a 2020 2020 2020 2020 2020  Path].          
-0000d3c0: 2020 4120 6669 6c65 2070 6174 6820 746f    A file path to
-0000d3d0: 2074 6865 206d 6f6c 6563 756c 6520 696e   the molecule in
-0000d3e0: 2065 6974 6865 7220 5044 4220 6f72 2058   either PDB or X
-0000d3f0: 595a 2066 6f72 6d61 742e 0a20 2020 2020  YZ format..     
-0000d400: 2020 2072 6164 6969 203a 2055 6e69 6f6e     radii : Union
-0000d410: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
-0000d420: 7468 2c20 4469 6374 5b73 7472 2c20 416e  th, Dict[str, An
-0000d430: 795d 5d2c 206f 7074 696f 6e61 6c0a 2020  y]], optional.  
-0000d440: 2020 2020 2020 2020 2020 4120 6669 6c65            A file
-0000d450: 2070 6174 6820 746f 2061 2076 616e 2064   path to a van d
-0000d460: 6572 2057 6161 6c73 2072 6164 6969 2066  er Waals radii f
-0000d470: 696c 6520 6f72 2061 2064 6963 7469 6f6e  ile or a diction
-0000d480: 6172 7920 6f66 2056 4457 2072 6164 6969  ary of VDW radii
-0000d490: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-0000d4a0: 652e 2049 6620 4e6f 6e65 2c20 6170 706c  e. If None, appl
-0000d4b0: 7920 7468 6520 6275 696c 742d 696e 2076  y the built-in v
-0000d4c0: 616e 2064 6572 2057 6161 6c73 2072 6164  an der Waals rad
-0000d4d0: 6969 2066 696c 653a 2060 7664 772e 6461  ii file: `vdw.da
-0000d4e0: 7460 2e0a 2020 2020 2020 2020 6d6f 6465  t`..        mode
-0000d4f0: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
-0000d500: 6c0a 2020 2020 2020 2020 2020 2020 5468  l.            Th
-0000d510: 6520 6d6f 6465 6c20 6e75 6d62 6572 206f  e model number o
-0000d520: 6620 6120 6d75 6c74 692d 6d6f 6465 6c20  f a multi-model 
-0000d530: 5044 4220 6669 6c65 2c20 6279 2064 6566  PDB file, by def
-0000d540: 6175 6c74 204e 6f6e 652e 2049 6620 4e6f  ault None. If No
-0000d550: 6e65 2c20 6b65 6570 2061 746f 6d73 2066  ne, keep atoms f
-0000d560: 726f 6d20 616c 6c20 6d6f 6465 6c73 2e0a  rom all models..
-0000d570: 2020 2020 2020 2020 6e74 6872 6561 6473          nthreads
-0000d580: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-0000d590: 0a20 2020 2020 2020 2020 2020 204e 756d  .            Num
-0000d5a0: 6265 7220 6f66 2074 6872 6561 6473 2c20  ber of threads, 
-0000d5b0: 6279 2064 6566 6175 6c74 204e 6f6e 652e  by default None.
-0000d5c0: 2049 6620 4e6f 6e65 2c20 7468 6520 6e75   If None, the nu
-0000d5d0: 6d62 6572 206f 6620 7468 7265 6164 7320  mber of threads 
-0000d5e0: 6973 2060 6f73 2e63 7075 5f63 6f75 6e74  is `os.cpu_count
-0000d5f0: 2829 202d 2031 602e 0a20 2020 2020 2020  () - 1`..       
-0000d600: 2076 6572 626f 7365 203a 2062 6f6f 6c2c   verbose : bool,
-0000d610: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000d620: 2020 2020 2020 5072 696e 7420 6578 7472        Print extr
-0000d630: 6120 696e 666f 726d 6174 696f 6e20 746f  a information to
-0000d640: 2073 7461 6e64 6172 6420 6f75 7470 7574   standard output
-0000d650: 2c20 6279 2064 6566 6175 6c74 2046 616c  , by default Fal
-0000d660: 7365 2e0a 0a20 2020 2020 2020 2052 6169  se...        Rai
-0000d670: 7365 730a 2020 2020 2020 2020 2d2d 2d2d  ses.        ----
-0000d680: 2d2d 0a20 2020 2020 2020 2054 7970 6545  --.        TypeE
-0000d690: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-0000d6a0: 2060 6d6f 6c65 6375 6c65 6020 6d75 7374   `molecule` must
-0000d6b0: 2062 6520 6120 7374 7269 6e67 206f 7220   be a string or 
-0000d6c0: 6120 7061 7468 6c69 622e 5061 7468 2e0a  a pathlib.Path..
-0000d6d0: 2020 2020 2020 2020 5479 7065 4572 726f          TypeErro
-0000d6e0: 720a 2020 2020 2020 2020 2020 2020 606d  r.            `m
-0000d6f0: 6f6c 6563 756c 6560 206d 7573 7420 6861  olecule` must ha
-0000d700: 7665 202e 7064 6220 6f72 202e 7879 7a20  ve .pdb or .xyz 
-0000d710: 6578 7465 6e73 696f 6e2e 0a20 2020 2020  extension..     
-0000d720: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
-0000d730: 2020 2020 2020 2020 2060 6e74 6872 6561           `nthrea
-0000d740: 6473 6020 6d75 7374 2062 6520 6120 706f  ds` must be a po
-0000d750: 7369 7469 7665 2069 6e74 6567 6572 2e0a  sitive integer..
-0000d760: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-0000d770: 6f72 0a20 2020 2020 2020 2020 2020 2060  or.            `
-0000d780: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
-0000d790: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
-0000d7a0: 6567 6572 2e0a 2020 2020 2020 2020 2222  eger..        ""
-0000d7b0: 220a 0a20 2020 2020 2020 2023 2041 7474  "..        # Att
-0000d7c0: 7269 6275 7465 730a 2020 2020 2020 2020  ributes.        
-0000d7d0: 7365 6c66 2e5f 6772 6964 203d 204e 6f6e  self._grid = Non
-0000d7e0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000d7f0: 7374 6570 203d 204e 6f6e 650a 2020 2020  step = None.    
-0000d800: 2020 2020 7365 6c66 2e5f 7061 6464 696e      self._paddin
-0000d810: 6720 3d20 4e6f 6e65 0a20 2020 2020 2020  g = None.       
-0000d820: 2073 656c 662e 5f70 726f 6265 203d 204e   self._probe = N
-0000d830: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000d840: 2e5f 7265 7072 6573 656e 7461 7469 6f6e  ._representation
-0000d850: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000d860: 7365 6c66 2e5f 7665 7274 6963 6573 203d  self._vertices =
-0000d870: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-0000d880: 6c66 2e5f 6469 6d20 3d20 4e6f 6e65 0a20  lf._dim = None. 
-0000d890: 2020 2020 2020 2073 656c 662e 5f72 6f74         self._rot
-0000d8a0: 6174 696f 6e20 3d20 4e6f 6e65 0a20 2020  ation = None.   
-0000d8b0: 2020 2020 2073 656c 662e 7665 7262 6f73       self.verbos
-0000d8c0: 6520 3d20 7665 7262 6f73 650a 0a20 2020  e = verbose..   
-0000d8d0: 2020 2020 2023 204d 6f6c 6563 756c 650a       # Molecule.
-0000d8e0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0000d8f0: 6d6f 6c65 6375 6c65 2920 6e6f 7420 696e  molecule) not in
-0000d900: 205b 7374 722c 2070 6174 686c 6962 2e50   [str, pathlib.P
-0000d910: 6174 685d 3a0a 2020 2020 2020 2020 2020  ath]:.          
-0000d920: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0000d930: 7228 2260 6d6f 6c65 6375 6c65 6020 6d75  r("`molecule` mu
-0000d940: 7374 2062 6520 6120 7374 7269 6e67 206f  st be a string o
-0000d950: 7220 6120 7061 7468 6c69 622e 5061 7468  r a pathlib.Path
-0000d960: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
-0000d970: 2e5f 6d6f 6c65 6375 6c65 203d 206f 732e  ._molecule = os.
-0000d980: 7061 7468 2e72 6561 6c70 6174 6828 6d6f  path.realpath(mo
-0000d990: 6c65 6375 6c65 290a 0a20 2020 2020 2020  lecule)..       
-0000d9a0: 2023 2076 616e 2064 6572 2057 6161 6c73   # van der Waals
-0000d9b0: 2072 6164 6969 0a20 2020 2020 2020 2069   radii.        i
-0000d9c0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
-0000d9d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000d9e0: 7428 223e 204c 6f61 6469 6e67 2076 616e  t("> Loading van
-0000d9f0: 2064 6572 2057 6161 6c73 2072 6164 6969   der Waals radii
-0000da00: 2229 0a20 2020 2020 2020 2069 6620 7261  ").        if ra
-0000da10: 6469 6920 6973 204e 6f6e 653a 0a20 2020  dii is None:.   
-0000da20: 2020 2020 2020 2020 2023 2064 6566 6175           # defau
-0000da30: 6c74 0a20 2020 2020 2020 2020 2020 2073  lt.            s
-0000da40: 656c 662e 5f72 6164 6969 203d 2072 6561  elf._radii = rea
-0000da50: 645f 7664 7728 5644 5729 0a20 2020 2020  d_vdw(VDW).     
-0000da60: 2020 2065 6c69 6620 7479 7065 2872 6164     elif type(rad
-0000da70: 6969 2920 696e 205b 7374 722c 2070 6174  ii) in [str, pat
-0000da80: 686c 6962 2e50 6174 685d 3a0a 2020 2020  hlib.Path]:.    
-0000da90: 2020 2020 2020 2020 2320 7664 7720 6669          # vdw fi
-0000daa0: 6c65 0a20 2020 2020 2020 2020 2020 2073  le.            s
-0000dab0: 656c 662e 5f72 6164 6969 203d 2072 6561  elf._radii = rea
-0000dac0: 645f 7664 7728 7261 6469 6929 0a20 2020  d_vdw(radii).   
-0000dad0: 2020 2020 2065 6c69 6620 7479 7065 2872       elif type(r
-0000dae0: 6164 6969 2920 696e 205b 6469 6374 5d3a  adii) in [dict]:
-0000daf0: 0a20 2020 2020 2020 2020 2020 2023 2050  .            # P
-0000db00: 726f 6365 7373 6564 2064 6963 7469 6f6e  rocessed diction
-0000db10: 6172 790a 2020 2020 2020 2020 2020 2020  ary.            
-0000db20: 7365 6c66 2e5f 7261 6469 6920 3d20 7261  self._radii = ra
-0000db30: 6469 690a 0a20 2020 2020 2020 2023 2041  dii..        # A
-0000db40: 746f 6d69 6320 696e 666f 726d 6174 696f  tomic informatio
-0000db50: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000db60: 662e 7665 7262 6f73 653a 0a20 2020 2020  f.verbose:.     
-0000db70: 2020 2020 2020 2070 7269 6e74 2822 3e20         print("> 
-0000db80: 5265 6164 696e 6720 6d6f 6c65 6375 6c65  Reading molecule
-0000db90: 2063 6f6f 7264 696e 6174 6573 2229 0a20   coordinates"). 
-0000dba0: 2020 2020 2020 2069 6620 6d6f 6c65 6375         if molecu
-0000dbb0: 6c65 2e65 6e64 7377 6974 6828 222e 7064  le.endswith(".pd
-0000dbc0: 6222 293a 0a20 2020 2020 2020 2020 2020  b"):.           
-0000dbd0: 2073 656c 662e 5f61 746f 6d69 6320 3d20   self._atomic = 
-0000dbe0: 7265 6164 5f70 6462 286d 6f6c 6563 756c  read_pdb(molecul
-0000dbf0: 652c 2073 656c 662e 7261 6469 692c 206d  e, self.radii, m
-0000dc00: 6f64 656c 290a 2020 2020 2020 2020 656c  odel).        el
-0000dc10: 6966 206d 6f6c 6563 756c 652e 656e 6473  if molecule.ends
-0000dc20: 7769 7468 2822 2e78 797a 2229 3a0a 2020  with(".xyz"):.  
-0000dc30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000dc40: 6174 6f6d 6963 203d 2072 6561 645f 7879  atomic = read_xy
-0000dc50: 7a28 6d6f 6c65 6375 6c65 2c20 7365 6c66  z(molecule, self
-0000dc60: 2e72 6164 6969 290a 2020 2020 2020 2020  .radii).        
-0000dc70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000dc80: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0000dc90: 7228 2260 6d6f 6c65 6375 6c65 6020 6d75  r("`molecule` mu
-0000dca0: 7374 2068 6176 6520 2e70 6462 206f 7220  st have .pdb or 
-0000dcb0: 2e78 797a 2065 7874 656e 7369 6f6e 2e22  .xyz extension."
-0000dcc0: 290a 0a20 2020 2020 2020 2023 204e 756d  )..        # Num
-0000dcd0: 6265 7220 6f66 2074 6872 6561 6473 0a20  ber of threads. 
-0000dce0: 2020 2020 2020 2069 6620 6e74 6872 6561         if nthrea
-0000dcf0: 6473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ds is not None:.
-0000dd00: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000dd10: 7970 6528 6e74 6872 6561 6473 2920 6e6f  ype(nthreads) no
-0000dd20: 7420 696e 205b 696e 745d 3a0a 2020 2020  t in [int]:.    
-0000dd30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000dd40: 6520 5479 7065 4572 726f 7228 2260 6e74  e TypeError("`nt
-0000dd50: 6872 6561 6473 6020 6d75 7374 2062 6520  hreads` must be 
-0000dd60: 6120 706f 7369 7469 7665 2069 6e74 6567  a positive integ
-0000dd70: 6572 2e22 290a 2020 2020 2020 2020 2020  er.").          
-0000dd80: 2020 656c 6966 206e 7468 7265 6164 7320    elif nthreads 
-0000dd90: 3c3d 2030 3a0a 2020 2020 2020 2020 2020  <= 0:.          
-0000dda0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000ddb0: 6545 7272 6f72 2822 606e 7468 7265 6164  eError("`nthread
-0000ddc0: 7360 206d 7573 7420 6265 2061 2070 6f73  s` must be a pos
-0000ddd0: 6974 6976 6520 696e 7465 6765 722e 2229  itive integer.")
-0000dde0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000ddf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000de00: 2020 2073 656c 662e 6e74 6872 6561 6473     self.nthreads
-0000de10: 203d 206e 7468 7265 6164 730a 2020 2020   = nthreads.    
-0000de20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000de30: 2020 2020 2020 7365 6c66 2e6e 7468 7265        self.nthre
-0000de40: 6164 7320 3d20 6f73 2e63 7075 5f63 6f75  ads = os.cpu_cou
-0000de50: 6e74 2829 202d 2031 0a0a 2020 2020 4070  nt() - 1..    @p
-0000de60: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000de70: 6174 6f6d 6963 2873 656c 6629 202d 3e20  atomic(self) -> 
-0000de80: 6e75 6d70 792e 6e64 6172 7261 793a 0a20  numpy.ndarray:. 
-0000de90: 2020 2020 2020 2022 2222 4765 7420 5f61         """Get _a
-0000dea0: 746f 6d69 6320 6174 7472 6962 7574 652e  tomic attribute.
-0000deb0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-0000dec0: 726e 2073 656c 662e 5f61 746f 6d69 630a  rn self._atomic.
-0000ded0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000dee0: 2020 2064 6566 2064 696d 2873 656c 6629     def dim(self)
-0000def0: 202d 3e20 5475 706c 655b 696e 742c 2069   -> Tuple[int, i
-0000df00: 6e74 2c20 696e 745d 3a0a 2020 2020 2020  nt, int]:.      
-0000df10: 2020 2222 2247 6574 205f 6469 6d20 6174    """Get _dim at
-0000df20: 7472 6962 7574 6522 2222 0a20 2020 2020  tribute""".     
-0000df30: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000df40: 6469 6d0a 0a20 2020 2040 7072 6f70 6572  dim..    @proper
-0000df50: 7479 0a20 2020 2064 6566 2067 7269 6428  ty.    def grid(
-0000df60: 7365 6c66 2920 2d3e 206e 756d 7079 2e6e  self) -> numpy.n
-0000df70: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
-0000df80: 2222 2247 6574 205f 6772 6964 2061 7474  """Get _grid att
-0000df90: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
-0000dfa0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000dfb0: 6772 6964 0a0a 2020 2020 4070 726f 7065  grid..    @prope
-0000dfc0: 7274 790a 2020 2020 6465 6620 6d6f 6c65  rty.    def mole
-0000dfd0: 6375 6c65 2873 656c 6629 202d 3e20 556e  cule(self) -> Un
-0000dfe0: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-0000dff0: 2e50 6174 685d 3a0a 2020 2020 2020 2020  .Path]:.        
-0000e000: 2222 2247 6574 205f 6d6f 6c65 6375 6c65  """Get _molecule
-0000e010: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
-0000e020: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e030: 6c66 2e5f 6d6f 6c65 6375 6c65 0a0a 2020  lf._molecule..  
-0000e040: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000e050: 6465 6620 6e78 2873 656c 6629 202d 3e20  def nx(self) -> 
-0000e060: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-0000e070: 4765 7420 6772 6964 2075 6e69 7473 2069  Get grid units i
-0000e080: 6e20 582d 6178 6973 2e22 2222 0a20 2020  n X-axis.""".   
-0000e090: 2020 2020 2069 6620 7365 6c66 2e5f 6469       if self._di
-0000e0a0: 6d20 6973 206e 6f74 204e 6f6e 653a 0a20  m is not None:. 
-0000e0b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e0c0: 6e20 7365 6c66 2e5f 6469 6d5b 305d 0a0a  n self._dim[0]..
-0000e0d0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000e0e0: 2020 6465 6620 6e79 2873 656c 6629 202d    def ny(self) -
-0000e0f0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-0000e100: 2222 4765 7420 6772 6964 2075 6e69 7473  ""Get grid units
-0000e110: 2069 6e20 592d 6178 6973 2e22 2222 0a20   in Y-axis.""". 
-0000e120: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000e130: 6469 6d20 6973 206e 6f74 204e 6f6e 653a  dim is not None:
-0000e140: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000e150: 7572 6e20 7365 6c66 2e5f 6469 6d5b 315d  urn self._dim[1]
-0000e160: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000e170: 2020 2020 6465 6620 6e7a 2873 656c 6629      def nz(self)
-0000e180: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-0000e190: 2022 2222 4765 7420 6772 6964 2075 6e69   """Get grid uni
-0000e1a0: 7473 2069 6e20 5a2d 6178 6973 2e22 2222  ts in Z-axis."""
-0000e1b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e1c0: 2e5f 6469 6d20 6973 206e 6f74 204e 6f6e  ._dim is not Non
-0000e1d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000e1e0: 6574 7572 6e20 7365 6c66 2e5f 6469 6d5b  eturn self._dim[
-0000e1f0: 325d 0a0a 2020 2020 4070 726f 7065 7274  2]..    @propert
-0000e200: 790a 2020 2020 6465 6620 7031 2873 656c  y.    def p1(sel
-0000e210: 6629 202d 3e20 6e75 6d70 792e 6e64 6172  f) -> numpy.ndar
-0000e220: 7261 793a 0a20 2020 2020 2020 2022 2222  ray:.        """
-0000e230: 4765 7420 6f72 6967 696e 206f 6620 7468  Get origin of th
-0000e240: 6520 3344 2067 7269 642e 2222 220a 2020  e 3D grid.""".  
-0000e250: 2020 2020 2020 6966 2073 656c 662e 5f76        if self._v
-0000e260: 6572 7469 6365 7320 6973 206e 6f74 204e  ertices is not N
-0000e270: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000e280: 2072 6574 7572 6e20 7365 6c66 2e5f 7665   return self._ve
-0000e290: 7274 6963 6573 5b30 5d0a 0a20 2020 2040  rtices[0]..    @
-0000e2a0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000e2b0: 2070 3228 7365 6c66 2920 2d3e 206e 756d   p2(self) -> num
-0000e2c0: 7079 2e6e 6461 7272 6179 3a0a 2020 2020  py.ndarray:.    
-0000e2d0: 2020 2020 2222 2247 6574 2058 2d61 7869      """Get X-axi
-0000e2e0: 7320 6d61 7820 6f66 2074 6865 2033 4420  s max of the 3D 
-0000e2f0: 6772 6964 2e22 2222 0a20 2020 2020 2020  grid.""".       
-0000e300: 2069 6620 7365 6c66 2e5f 7665 7274 6963   if self._vertic
-0000e310: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-0000e320: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e330: 726e 2073 656c 662e 5f76 6572 7469 6365  rn self._vertice
-0000e340: 735b 315d 0a0a 2020 2020 4070 726f 7065  s[1]..    @prope
-0000e350: 7274 790a 2020 2020 6465 6620 7033 2873  rty.    def p3(s
-0000e360: 656c 6629 202d 3e20 6e75 6d70 792e 6e64  elf) -> numpy.nd
-0000e370: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
-0000e380: 2222 4765 7420 592d 6178 6973 206d 6178  ""Get Y-axis max
-0000e390: 206f 6620 7468 6520 3344 2067 7269 642e   of the 3D grid.
-0000e3a0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-0000e3b0: 656c 662e 5f76 6572 7469 6365 7320 6973  elf._vertices is
-0000e3c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e3d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e3e0: 6c66 2e5f 7665 7274 6963 6573 5b32 5d0a  lf._vertices[2].
-0000e3f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000e400: 2020 2064 6566 2070 3428 7365 6c66 2920     def p4(self) 
-0000e410: 2d3e 206e 756d 7079 2e6e 6461 7272 6179  -> numpy.ndarray
-0000e420: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-0000e430: 205a 2d61 7869 7320 6d61 7820 6f66 2074   Z-axis max of t
-0000e440: 6865 2033 4420 6772 6964 2e22 2222 0a20  he 3D grid.""". 
-0000e450: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000e460: 7665 7274 6963 6573 2069 7320 6e6f 7420  vertices is not 
-0000e470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000e480: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
-0000e490: 6572 7469 6365 735b 335d 0a0a 2020 2020  ertices[3]..    
-0000e4a0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000e4b0: 6620 7061 6464 696e 6728 7365 6c66 2920  f padding(self) 
-0000e4c0: 2d3e 2066 6c6f 6174 3a0a 2020 2020 2020  -> float:.      
-0000e4d0: 2020 2222 2247 6574 205f 7061 6464 696e    """Get _paddin
-0000e4e0: 6720 6174 7472 6962 7574 652e 2222 220a  g attribute.""".
-0000e4f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000e500: 656c 662e 5f70 6164 6469 6e67 0a0a 2020  elf._padding..  
-0000e510: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000e520: 6465 6620 7072 6f62 6528 7365 6c66 2920  def probe(self) 
-0000e530: 2d3e 2066 6c6f 6174 3a0a 2020 2020 2020  -> float:.      
-0000e540: 2020 2222 2247 6574 205f 7072 6f62 6520    """Get _probe 
-0000e550: 6174 7472 6962 7574 652e 2222 220a 2020  attribute.""".  
-0000e560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e570: 662e 5f70 726f 6265 0a0a 2020 2020 4070  f._probe..    @p
-0000e580: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000e590: 7261 6469 6928 7365 6c66 2920 2d3e 2044  radii(self) -> D
-0000e5a0: 6963 745b 7374 722c 2041 6e79 5d3a 0a20  ict[str, Any]:. 
-0000e5b0: 2020 2020 2020 2022 2222 4765 7420 5f72         """Get _r
-0000e5c0: 6164 6969 2061 7474 7269 6275 7465 2e22  adii attribute."
-0000e5d0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0000e5e0: 6e20 7365 6c66 2e5f 7261 6469 690a 0a20  n self._radii.. 
-0000e5f0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000e600: 2064 6566 2072 6570 7265 7365 6e74 6174   def representat
-0000e610: 696f 6e28 7365 6c66 2920 2d3e 2073 7472  ion(self) -> str
-0000e620: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-0000e630: 205f 7265 7072 6573 656e 7461 7469 6f6e   _representation
-0000e640: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
-0000e650: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e660: 6c66 2e5f 7265 7072 6573 656e 7461 7469  lf._representati
-0000e670: 6f6e 0a0a 2020 2020 4070 726f 7065 7274  on..    @propert
-0000e680: 790a 2020 2020 6465 6620 726f 7461 7469  y.    def rotati
-0000e690: 6f6e 2873 656c 6629 202d 3e20 6e75 6d70  on(self) -> nump
-0000e6a0: 792e 6e64 6172 7261 793a 0a20 2020 2020  y.ndarray:.     
-0000e6b0: 2020 2022 2222 4765 7420 5f72 6f74 6174     """Get _rotat
-0000e6c0: 696f 6e20 6174 7472 6962 7574 652e 2222  ion attribute.""
-0000e6d0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000e6e0: 2073 656c 662e 5f72 6f74 6174 696f 6e0a   self._rotation.
-0000e6f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000e700: 2020 2064 6566 2073 7465 7028 7365 6c66     def step(self
-0000e710: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
-0000e720: 2020 2020 2222 2247 6574 205f 7374 6570      """Get _step
-0000e730: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
-0000e740: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000e750: 7374 6570 2069 7320 6e6f 7420 4e6f 6e65  step is not None
-0000e760: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e770: 7475 726e 2073 656c 662e 5f73 7465 700a  turn self._step.
-0000e780: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000e790: 2020 2064 6566 2076 6572 7469 6365 7328     def vertices(
-0000e7a0: 7365 6c66 2920 2d3e 206e 756d 7079 2e6e  self) -> numpy.n
-0000e7b0: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
-0000e7c0: 2222 2247 6574 205f 7665 7274 6963 6573  """Get _vertices
-0000e7d0: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
-0000e7e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e7f0: 6c66 2e5f 7665 7274 6963 6573 0a0a 2020  lf._vertices..  
-0000e800: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000e810: 6465 6620 7879 7a72 2873 656c 6629 202d  def xyzr(self) -
-0000e820: 3e20 6e75 6d70 792e 6e64 6172 7261 793a  > numpy.ndarray:
-0000e830: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000e840: 7879 7a20 636f 6f72 6469 6e61 7465 7320  xyz coordinates 
-0000e850: 616e 6420 7261 6469 7573 206f 6620 6d6f  and radius of mo
-0000e860: 6c65 6375 6c65 2061 746f 6d73 2e22 2222  lecule atoms."""
-0000e870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e880: 7365 6c66 2e5f 6174 6f6d 6963 5b3a 2c20  self._atomic[:, 
-0000e890: 343a 5d2e 6173 7479 7065 286e 756d 7079  4:].astype(numpy
-0000e8a0: 2e66 6c6f 6174 3634 290a 0a20 2020 2064  .float64)..    d
-0000e8b0: 6566 205f 7365 745f 6772 6964 2873 656c  ef _set_grid(sel
-0000e8c0: 662c 2070 6164 6469 6e67 3a20 4f70 7469  f, padding: Opti
-0000e8d0: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-0000e8e0: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
-0000e8f0: 2020 2020 2022 2222 4465 6669 6e65 2074       """Define t
-0000e900: 6865 2033 4420 6772 6964 2066 6f72 2074  he 3D grid for t
-0000e910: 6865 2074 6172 6765 7420 6d6f 6c65 6375  he target molecu
-0000e920: 6c65 2e0a 0a20 2020 2020 2020 2050 6172  le...        Par
-0000e930: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000e940: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000e950: 2020 2070 6164 6469 6e67 203a 2066 6c6f     padding : flo
-0000e960: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
-0000e970: 2020 2020 2020 2020 2054 6865 206c 656e           The len
-0000e980: 6774 6820 746f 2061 6464 2074 6f20 6561  gth to add to ea
-0000e990: 6368 2064 6972 6563 7469 6f6e 206f 6620  ch direction of 
-0000e9a0: 7468 6520 3344 2067 7269 642c 2062 7920  the 3D grid, by 
-0000e9b0: 6465 6661 756c 7420 4e6f 6e65 2e20 4966  default None. If
-0000e9c0: 204e 6f6e 652c 2061 7574 6f6d 6174 6963   None, automatic
-0000e9d0: 616c 6c79 2064 6566 696e 6520 7468 6520  ally define the 
-0000e9e0: 6c65 6e67 7468 2062 6173 6564 206f 6e20  length based on 
-0000e9f0: 6d6f 6c65 6375 6c65 2063 6f6f 7264 696e  molecule coordin
-0000ea00: 6174 6573 2c20 7072 6f62 6520 7369 7a65  ates, probe size
-0000ea10: 2c20 6772 6964 2073 7061 6369 6e67 2061  , grid spacing a
-0000ea20: 6e64 2061 746f 6d20 7261 6469 692e 0a0a  nd atom radii...
-0000ea30: 2020 2020 2020 2020 5261 6973 6573 0a20          Raises. 
-0000ea40: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
-0000ea50: 2020 2020 2020 5479 7065 4572 726f 720a        TypeError.
-0000ea60: 2020 2020 2020 2020 2020 2020 6070 6164              `pad
-0000ea70: 6469 6e67 6020 6d75 7374 2062 6520 6120  ding` must be a 
-0000ea80: 6e6f 6e2d 6e65 6761 7469 7665 2072 6561  non-negative rea
-0000ea90: 6c20 6e75 6d62 6572 2e0a 2020 2020 2020  l number..      
-0000eaa0: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
-0000eab0: 2020 2020 2020 2020 2060 7061 6464 696e           `paddin
-0000eac0: 6760 206d 7573 7420 6265 2061 206e 6f6e  g` must be a non
-0000ead0: 2d6e 6567 6174 6976 6520 7265 616c 206e  -negative real n
-0000eae0: 756d 6265 722e 0a20 2020 2020 2020 2022  umber..        "
-0000eaf0: 2222 0a20 2020 2020 2020 2023 2050 6164  "".        # Pad
-0000eb00: 6469 6e67 0a20 2020 2020 2020 2069 6620  ding.        if 
-0000eb10: 7061 6464 696e 6720 6973 206e 6f74 204e  padding is not N
-0000eb20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000eb30: 2069 6620 7479 7065 2870 6164 6469 6e67   if type(padding
-0000eb40: 2920 6e6f 7420 696e 205b 696e 742c 2066  ) not in [int, f
-0000eb50: 6c6f 6174 5d3a 0a20 2020 2020 2020 2020  loat]:.         
-0000eb60: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-0000eb70: 6545 7272 6f72 2822 6070 6164 6469 6e67  eError("`padding
-0000eb80: 6020 6d75 7374 2062 6520 6120 6e6f 6e2d  ` must be a non-
-0000eb90: 6e65 6761 7469 7665 2072 6561 6c20 6e75  negative real nu
-0000eba0: 6d62 6572 2e22 290a 2020 2020 2020 2020  mber.").        
-0000ebb0: 2020 2020 656c 6966 2070 6164 6469 6e67      elif padding
-0000ebc0: 203c 2030 2e30 3a0a 2020 2020 2020 2020   < 0.0:.        
-0000ebd0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000ebe0: 6c75 6545 7272 6f72 2822 6070 6164 6469  lueError("`paddi
-0000ebf0: 6e67 6020 6d75 7374 2062 6520 6120 6e6f  ng` must be a no
-0000ec00: 6e2d 6e65 6761 7469 7665 2072 6561 6c20  n-negative real 
-0000ec10: 6e75 6d62 6572 2e22 290a 2020 2020 2020  number.").      
-0000ec20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ec30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ec40: 2e5f 7061 6464 696e 6720 3d20 7061 6464  ._padding = padd
-0000ec50: 696e 670a 2020 2020 2020 2020 656c 7365  ing.        else
-0000ec60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ec70: 6c66 2e5f 7061 6464 696e 6720 3d20 7365  lf._padding = se
-0000ec80: 6c66 2e5f 6765 745f 7061 6464 696e 6728  lf._get_padding(
-0000ec90: 290a 0a20 2020 2020 2020 2023 2033 4420  )..        # 3D 
-0000eca0: 6772 6964 0a20 2020 2020 2020 2069 6620  grid.        if 
-0000ecb0: 7365 6c66 2e76 6572 626f 7365 3a0a 2020  self.verbose:.  
-0000ecc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000ecd0: 223e 2043 616c 6375 6c61 7469 6e67 2033  "> Calculating 3
-0000ece0: 4420 6772 6964 2229 0a20 2020 2020 2020  D grid").       
-0000ecf0: 2073 656c 662e 5f76 6572 7469 6365 7320   self._vertices 
-0000ed00: 3d20 6765 745f 7665 7274 6963 6573 2873  = get_vertices(s
-0000ed10: 656c 662e 6174 6f6d 6963 2c20 7365 6c66  elf.atomic, self
-0000ed20: 2e70 6164 6469 6e67 2c20 7365 6c66 2e73  .padding, self.s
-0000ed30: 7465 7029 0a20 2020 2020 2020 2073 656c  tep).        sel
-0000ed40: 662e 5f64 696d 203d 205f 6765 745f 6469  f._dim = _get_di
-0000ed50: 6d65 6e73 696f 6e73 2873 656c 662e 7665  mensions(self.ve
-0000ed60: 7274 6963 6573 2c20 7365 6c66 2e73 7465  rtices, self.ste
-0000ed70: 7029 0a20 2020 2020 2020 2073 656c 662e  p).        self.
-0000ed80: 5f72 6f74 6174 696f 6e20 3d20 5f67 6574  _rotation = _get
-0000ed90: 5f73 696e 636f 7328 7365 6c66 2e76 6572  _sincos(self.ver
-0000eda0: 7469 6365 7329 0a20 2020 2020 2020 2069  tices).        i
-0000edb0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
-0000edc0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000edd0: 7428 6622 7031 3a20 7b73 656c 662e 7665  t(f"p1: {self.ve
-0000ede0: 7274 6963 6573 5b30 5d7d 2229 0a20 2020  rtices[0]}").   
-0000edf0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0000ee00: 2270 323a 207b 7365 6c66 2e76 6572 7469  "p2: {self.verti
-0000ee10: 6365 735b 315d 7d22 290a 2020 2020 2020  ces[1]}").      
-0000ee20: 2020 2020 2020 7072 696e 7428 6622 7033        print(f"p3
-0000ee30: 3a20 7b73 656c 662e 7665 7274 6963 6573  : {self.vertices
-0000ee40: 5b32 5d7d 2229 0a20 2020 2020 2020 2020  [2]}").         
-0000ee50: 2020 2070 7269 6e74 2866 2270 343a 207b     print(f"p4: {
-0000ee60: 7365 6c66 2e76 6572 7469 6365 735b 335d  self.vertices[3]
-0000ee70: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-0000ee80: 7072 696e 7428 226e 783a 207b 7d2c 206e  print("nx: {}, n
-0000ee90: 793a 207b 7d2c 206e 7a3a 207b 7d22 2e66  y: {}, nz: {}".f
-0000eea0: 6f72 6d61 7428 2a73 656c 662e 6469 6d29  ormat(*self.dim)
-0000eeb0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-0000eec0: 696e 7428 2273 696e 613a 207b 7d2c 2073  int("sina: {}, s
-0000eed0: 696e 623a 207b 7d2c 2063 6f73 613a 207b  inb: {}, cosa: {
-0000eee0: 7d2c 2063 6f73 623a 207b 7d22 2e66 6f72  }, cosb: {}".for
-0000eef0: 6d61 7428 2a73 656c 662e 726f 7461 7469  mat(*self.rotati
-0000ef00: 6f6e 2929 0a0a 2020 2020 6465 6620 5f67  on))..    def _g
-0000ef10: 6574 5f70 6164 6469 6e67 2873 656c 6629  et_padding(self)
-0000ef20: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
-0000ef30: 2020 2022 2222 4175 746f 6d61 7469 6361     """Automatica
-0000ef40: 6c6c 7920 6465 6669 6e65 2074 6865 2070  lly define the p
-0000ef50: 6164 6469 6e67 2062 6173 6564 206f 6e20  adding based on 
-0000ef60: 6d6f 6c65 6375 6c65 2063 6f6f 7264 696e  molecule coordin
-0000ef70: 6174 6573 2c20 7072 6f62 6520 7369 7a65  ates, probe size
-0000ef80: 2c20 6772 6964 2073 7061 6369 6e67 2061  , grid spacing a
-0000ef90: 6e64 2061 746f 6d20 7261 6469 692e 0a0a  nd atom radii...
-0000efa0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000efb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000efc0: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
-0000efd0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-0000efe0: 2020 2020 5468 6520 6c65 6e67 7468 2074      The length t
-0000eff0: 6f20 6164 6420 746f 2065 6163 6820 6469  o add to each di
-0000f000: 7265 6374 696f 6e20 6f66 2074 6865 2033  rection of the 3
-0000f010: 4420 6772 6964 2e0a 2020 2020 2020 2020  D grid..        
-0000f020: 2222 220a 2020 2020 2020 2020 7061 6464  """.        padd
-0000f030: 696e 6720 3d20 312e 3120 2a20 7365 6c66  ing = 1.1 * self
-0000f040: 2e78 797a 725b 3a2c 2033 5d2e 6d61 7828  .xyzr[:, 3].max(
-0000f050: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000f060: 662e 7265 7072 6573 656e 7461 7469 6f6e  f.representation
-0000f070: 2069 6e20 5b22 5345 5322 2c20 2253 4153   in ["SES", "SAS
-0000f080: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000f090: 7061 6464 696e 6720 2b3d 2073 656c 662e  padding += self.
-0000f0a0: 5f70 726f 6265 0a20 2020 2020 2020 2072  _probe.        r
-0000f0b0: 6574 7572 6e20 666c 6f61 7428 7061 6464  eturn float(padd
-0000f0c0: 696e 672e 726f 756e 6428 6465 6369 6d61  ing.round(decima
-0000f0d0: 6c73 3d31 2929 0a0a 2020 2020 6465 6620  ls=1))..    def 
-0000f0e0: 7664 7728 7365 6c66 2c20 7374 6570 3a20  vdw(self, step: 
-0000f0f0: 666c 6f61 7420 3d20 302e 362c 2070 6164  float = 0.6, pad
-0000f100: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b66  ding: Optional[f
-0000f110: 6c6f 6174 5d20 3d20 4e6f 6e65 2920 2d3e  loat] = None) ->
-0000f120: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000f130: 2222 4669 6c6c 2074 6865 2033 4420 6772  ""Fill the 3D gr
-0000f140: 6964 2077 6974 6820 7468 6520 6d6f 6c65  id with the mole
-0000f150: 6375 6c65 2061 7320 7468 6520 7661 6e20  cule as the van 
-0000f160: 6465 7220 5761 616c 7320 7375 7266 6163  der Waals surfac
-0000f170: 6520 7265 7072 6573 656e 7461 7469 6f6e  e representation
-0000f180: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0000f190: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0000f1a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000f1b0: 2073 7465 7020 3a20 666c 6f61 742c 206f   step : float, o
-0000f1c0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000f1d0: 2020 2020 4772 6964 2073 7061 6369 6e67      Grid spacing
-0000f1e0: 2028 4129 2c20 6279 2064 6566 6175 6c74   (A), by default
-0000f1f0: 2030 2e36 2e0a 2020 2020 2020 2020 7061   0.6..        pa
-0000f200: 6464 696e 6720 3a20 666c 6f61 742c 206f  dding : float, o
-0000f210: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000f220: 2020 2020 5468 6520 6c65 6e67 7468 2074      The length t
-0000f230: 6f20 6164 6420 746f 2065 6163 6820 6469  o add to each di
-0000f240: 7265 6374 696f 6e20 6f66 2074 6865 2033  rection of the 3
-0000f250: 4420 6772 6964 2c20 6279 2064 6566 6175  D grid, by defau
-0000f260: 6c74 204e 6f6e 652e 2049 6620 4e6f 6e65  lt None. If None
-0000f270: 2c20 6175 746f 6d61 7469 6361 6c6c 7920  , automatically 
-0000f280: 6465 6669 6e65 2074 6865 206c 656e 6774  define the lengt
-0000f290: 6820 6261 7365 6420 6f6e 206d 6f6c 6563  h based on molec
-0000f2a0: 756c 6520 636f 6f72 6469 6e61 7465 732c  ule coordinates,
-0000f2b0: 2070 726f 6265 2073 697a 652c 2067 7269   probe size, gri
-0000f2c0: 6420 7370 6163 696e 6720 616e 6420 6174  d spacing and at
-0000f2d0: 6f6d 2072 6164 6969 2e0a 0a20 2020 2020  om radii...     
-0000f2e0: 2020 2052 6169 7365 730a 2020 2020 2020     Raises.      
-0000f2f0: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
-0000f300: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-0000f310: 2020 2020 2020 2060 7374 6570 6020 6d75         `step` mu
-0000f320: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-0000f330: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
-0000f340: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-0000f350: 0a20 2020 2020 2020 2020 2020 2060 7374  .            `st
-0000f360: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
-0000f370: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
-0000f380: 6572 2e0a 0a20 2020 2020 2020 2045 7861  er...        Exa
-0000f390: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
-0000f3a0: 2d2d 2d2d 0a20 2020 2020 2020 2054 6865  ----.        The
-0000f3b0: 2060 604d 6f6c 6563 756c 652e 7664 7728   ``Molecule.vdw(
-0000f3c0: 2960 6020 6d65 7468 6f64 2074 616b 6573  )`` method takes
-0000f3d0: 2061 2067 7269 6420 7370 6163 696e 6720   a grid spacing 
-0000f3e0: 616e 6420 7265 7475 726e 7320 6120 4e75  and returns a Nu
-0000f3f0: 6d50 7920 6172 7261 7920 7769 7468 2074  mPy array with t
-0000f400: 6865 206d 6f6c 6563 756c 6520 706f 696e  he molecule poin
-0000f410: 7473 2072 6570 7265 7365 6e74 696e 6720  ts representing 
-0000f420: 7468 6520 7664 5720 7375 7266 6163 6520  the vdW surface 
-0000f430: 696e 2074 6865 2033 4420 6772 6964 2e0a  in the 3D grid..
-0000f440: 0a20 2020 2020 2020 203e 3e3e 2023 2047  .        >>> # G
-0000f450: 7269 6420 5370 6163 696e 6720 2873 7465  rid Spacing (ste
-0000f460: 7029 3a20 302e 310a 2020 2020 2020 2020  p): 0.1.        
-0000f470: 3e3e 3e20 7374 6570 203d 2030 2e31 0a20  >>> step = 0.1. 
-0000f480: 2020 2020 2020 203e 3e3e 206d 6f6c 6563         >>> molec
-0000f490: 756c 652e 7664 7728 7374 6570 3d73 7465  ule.vdw(step=ste
-0000f4a0: 7029 0a20 2020 2020 2020 203e 3e3e 206d  p).        >>> m
-0000f4b0: 6f6c 6563 756c 652e 6772 6964 0a20 2020  olecule.grid.   
-0000f4c0: 2020 2020 2061 7272 6179 285b 5b5b 312c       array([[[1,
-0000f4d0: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
-0000f4e0: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
-0000f4f0: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-0000f500: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-0000f510: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000f520: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
-0000f530: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
-0000f540: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-0000f550: 2020 2020 2020 2020 2020 2020 205b 312c               [1,
-0000f560: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
-0000f570: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
-0000f580: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-0000f590: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000f5b0: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
-0000f5c0: 2031 2c20 315d 5d2c 0a20 2020 2020 2020   1, 1]],.       
-0000f5d0: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-0000f5e0: 2020 2020 2020 2020 2020 2020 5b5b 312c              [[1,
-0000f5f0: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
-0000f600: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
-0000f610: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-0000f620: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-0000f630: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000f640: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
-0000f650: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
-0000f660: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-0000f670: 2020 2020 2020 2020 2020 2020 205b 312c               [1,
-0000f680: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
-0000f690: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
-0000f6a0: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-0000f6b0: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000f6d0: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
-0000f6e0: 2031 2c20 315d 5d5d 2c20 6474 7970 653d   1, 1]]], dtype=
-0000f6f0: 696e 7433 3229 0a20 2020 2020 2020 2022  int32).        "
-0000f700: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
-0000f710: 5f70 794b 5646 696e 6465 7220 696d 706f  _pyKVFinder impo
-0000f720: 7274 205f 6669 6c6c 5f72 6563 6570 746f  rt _fill_recepto
-0000f730: 720a 0a20 2020 2020 2020 2023 2043 6865  r..        # Che
-0000f740: 636b 2061 7267 756d 656e 7473 0a20 2020  ck arguments.   
-0000f750: 2020 2020 2069 6620 7479 7065 2873 7465       if type(ste
-0000f760: 7029 206e 6f74 2069 6e20 5b69 6e74 2c20  p) not in [int, 
-0000f770: 666c 6f61 745d 3a0a 2020 2020 2020 2020  float]:.        
-0000f780: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-0000f790: 726f 7228 2260 7374 6570 6020 6d75 7374  ror("`step` must
-0000f7a0: 2062 6520 6120 706f 7374 6976 6520 7265   be a postive re
-0000f7b0: 616c 206e 756d 6265 722e 2229 0a20 2020  al number.").   
-0000f7c0: 2020 2020 2065 6c69 6620 7374 6570 203c       elif step <
-0000f7d0: 3d20 302e 303a 0a20 2020 2020 2020 2020  = 0.0:.         
-0000f7e0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000f7f0: 726f 7228 2260 7374 6570 6020 6d75 7374  ror("`step` must
-0000f800: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
-0000f810: 6561 6c20 6e75 6d62 6572 2e22 290a 2020  eal number.").  
-0000f820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000f830: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-0000f840: 6570 203d 2073 7465 700a 0a20 2020 2020  ep = step..     
-0000f850: 2020 2023 2041 7474 7269 6275 7465 730a     # Attributes.
-0000f860: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-0000f870: 7072 6573 656e 7461 7469 6f6e 203d 2022  presentation = "
-0000f880: 7664 5722 0a20 2020 2020 2020 2073 656c  vdW".        sel
-0000f890: 662e 5f70 726f 6265 203d 204e 6f6e 650a  f._probe = None.
-0000f8a0: 0a20 2020 2020 2020 2023 2044 6566 696e  .        # Defin
-0000f8b0: 6520 3344 2067 7269 640a 2020 2020 2020  e 3D grid.      
-0000f8c0: 2020 7365 6c66 2e5f 7365 745f 6772 6964    self._set_grid
-0000f8d0: 2870 6164 6469 6e67 290a 0a20 2020 2020  (padding)..     
-0000f8e0: 2020 2023 2076 616e 2064 6572 2057 6161     # van der Waa
-0000f8f0: 6c73 2061 746f 6d73 2028 6861 7264 2073  ls atoms (hard s
-0000f900: 7068 6572 6520 6d6f 6465 6c29 2074 6f20  phere model) to 
-0000f910: 6772 6964 0a20 2020 2020 2020 2069 6620  grid.        if 
-0000f920: 7365 6c66 2e76 6572 626f 7365 3a0a 2020  self.verbose:.  
-0000f930: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000f940: 223e 2049 6e73 6572 7469 6e67 2061 746f  "> Inserting ato
-0000f950: 6d73 2077 6974 6820 7661 6e20 6465 7220  ms with van der 
-0000f960: 5761 616c 7320 7261 6469 6920 696e 746f  Waals radii into
-0000f970: 2033 4420 6772 6964 2229 0a20 2020 2020   3D grid").     
-0000f980: 2020 2073 656c 662e 5f67 7269 6420 3d20     self._grid = 
-0000f990: 5f66 696c 6c5f 7265 6365 7074 6f72 280a  _fill_receptor(.
-0000f9a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f9b0: 2e6e 7820 2a20 7365 6c66 2e6e 7920 2a20  .nx * self.ny * 
-0000f9c0: 7365 6c66 2e6e 7a2c 0a20 2020 2020 2020  self.nz,.       
-0000f9d0: 2020 2020 2073 656c 662e 6e78 2c0a 2020       self.nx,.  
-0000f9e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000f9f0: 792c 0a20 2020 2020 2020 2020 2020 2073  y,.            s
-0000fa00: 656c 662e 6e7a 2c0a 2020 2020 2020 2020  elf.nz,.        
-0000fa10: 2020 2020 7365 6c66 2e78 797a 722c 0a20      self.xyzr,. 
-0000fa20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fa30: 7031 2c0a 2020 2020 2020 2020 2020 2020  p1,.            
-0000fa40: 7365 6c66 2e72 6f74 6174 696f 6e2c 0a20  self.rotation,. 
-0000fa50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fa60: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
-0000fa70: 2020 302e 302c 0a20 2020 2020 2020 2020    0.0,.         
-0000fa80: 2020 2046 616c 7365 2c0a 2020 2020 2020     False,.      
-0000fa90: 2020 2020 2020 7365 6c66 2e6e 7468 7265        self.nthre
-0000faa0: 6164 732c 0a20 2020 2020 2020 2020 2020  ads,.           
-0000fab0: 2073 656c 662e 7665 7262 6f73 652c 0a20   self.verbose,. 
-0000fac0: 2020 2020 2020 2029 2e72 6573 6861 7065         ).reshape
-0000fad0: 2873 656c 662e 6e78 2c20 7365 6c66 2e6e  (self.nx, self.n
-0000fae0: 792c 2073 656c 662e 6e7a 290a 0a20 2020  y, self.nz)..   
-0000faf0: 2064 6566 2073 7572 6661 6365 280a 2020   def surface(.  
-0000fb00: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000fb10: 2020 2020 7374 6570 3a20 666c 6f61 7420      step: float 
-0000fb20: 3d20 302e 362c 0a20 2020 2020 2020 2070  = 0.6,.        p
-0000fb30: 726f 6265 3a20 666c 6f61 7420 3d20 312e  robe: float = 1.
-0000fb40: 342c 0a20 2020 2020 2020 2073 7572 6661  4,.        surfa
-0000fb50: 6365 3a20 7374 7220 3d20 2253 4553 222c  ce: str = "SES",
-0000fb60: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-0000fb70: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-0000fb80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
-0000fb90: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000fba0: 2022 2222 4669 6c6c 2074 6865 2033 4420   """Fill the 3D 
-0000fbb0: 6772 6964 2077 6974 6820 7468 6520 6d6f  grid with the mo
-0000fbc0: 6c65 6375 6c65 2061 7320 7468 6520 7661  lecule as the va
-0000fbd0: 6e20 6465 7220 5761 616c 7320 7375 7266  n der Waals surf
-0000fbe0: 6163 6520 7265 7072 6573 656e 7461 7469  ace representati
-0000fbf0: 6f6e 2e0a 0a20 2020 2020 2020 2050 6172  on...        Par
-0000fc00: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000fc10: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000fc20: 2020 2073 7465 7020 3a20 666c 6f61 742c     step : float,
-0000fc30: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000fc40: 2020 2020 2020 4772 6964 2073 7061 6369        Grid spaci
-0000fc50: 6e67 2028 4129 2c20 6279 2064 6566 6175  ng (A), by defau
-0000fc60: 6c74 2030 2e36 2e0a 2020 2020 2020 2020  lt 0.6..        
-0000fc70: 7072 6f62 6520 3a20 666c 6f61 742c 206f  probe : float, o
-0000fc80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000fc90: 2020 2020 5370 6865 7269 6361 6c20 7072      Spherical pr
-0000fca0: 6f62 6520 7369 7a65 2074 6f20 6465 6669  obe size to defi
-0000fcb0: 6e65 2074 6865 206d 6f6c 6563 756c 6172  ne the molecular
-0000fcc0: 2073 7572 6661 6365 2062 6173 6564 206f   surface based o
-0000fcd0: 6e20 6120 6d6f 6c65 6375 6c61 7220 7265  n a molecular re
-0000fce0: 7072 6573 656e 7461 7469 6f6e 2c20 6279  presentation, by
-0000fcf0: 2064 6566 6175 6c74 2031 2e34 2e0a 2020   default 1.4..  
-0000fd00: 2020 2020 2020 7375 7266 6163 6520 3a20        surface : 
-0000fd10: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
-0000fd20: 2020 2020 2020 2020 2020 4d6f 6c65 6375            Molecu
-0000fd30: 6c61 7220 7375 7266 6163 6520 7265 7072  lar surface repr
-0000fd40: 6573 656e 7461 7469 6f6e 2e20 4b65 7977  esentation. Keyw
-0000fd50: 6f72 6473 206f 7074 696f 6e73 2061 7265  ords options are
-0000fd60: 2076 6457 2028 7661 6e20 6465 7220 5761   vdW (van der Wa
-0000fd70: 616c 7320 7375 7266 6163 6529 2c20 5345  als surface), SE
-0000fd80: 5320 2853 6f6c 7665 6e74 2045 7863 6c75  S (Solvent Exclu
-0000fd90: 6465 6420 5375 7266 6163 6529 206f 7220  ded Surface) or 
-0000fda0: 5341 5320 2853 6f6c 7665 6e74 2041 6363  SAS (Solvent Acc
-0000fdb0: 6573 7369 626c 6520 5375 7266 6163 6529  essible Surface)
-0000fdc0: 2c20 6279 2064 6566 6175 6c74 2022 5345  , by default "SE
-0000fdd0: 5322 2e0a 2020 2020 2020 2020 7061 6464  S"..        padd
-0000fde0: 696e 6720 3a20 666c 6f61 742c 206f 7074  ing : float, opt
-0000fdf0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000fe00: 2020 5468 6520 6c65 6e67 7468 2074 6f20    The length to 
-0000fe10: 6164 6420 746f 2065 6163 6820 6469 7265  add to each dire
-0000fe20: 6374 696f 6e20 6f66 2074 6865 2033 4420  ction of the 3D 
-0000fe30: 6772 6964 2c20 6279 2064 6566 6175 6c74  grid, by default
-0000fe40: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
-0000fe50: 6175 746f 6d61 7469 6361 6c6c 7920 6465  automatically de
-0000fe60: 6669 6e65 2074 6865 206c 656e 6774 6820  fine the length 
-0000fe70: 6261 7365 6420 6f6e 206d 6f6c 6563 756c  based on molecul
-0000fe80: 6520 636f 6f72 6469 6e61 7465 732c 2070  e coordinates, p
-0000fe90: 726f 6265 2073 697a 652c 2067 7269 6420  robe size, grid 
-0000fea0: 7370 6163 696e 6720 616e 6420 6174 6f6d  spacing and atom
-0000feb0: 2072 6164 6969 2e0a 0a20 2020 2020 2020   radii...       
-0000fec0: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
-0000fed0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
-0000fee0: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-0000fef0: 2020 2020 2060 7374 6570 6020 6d75 7374       `step` must
-0000ff00: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
-0000ff10: 6561 6c20 6e75 6d62 6572 2e0a 2020 2020  eal number..    
-0000ff20: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
-0000ff30: 2020 2020 2020 2020 2020 2060 7374 6570             `step
-0000ff40: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
-0000ff50: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
-0000ff60: 2e0a 2020 2020 2020 2020 5479 7065 4572  ..        TypeEr
-0000ff70: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-0000ff80: 6070 726f 6265 5f6f 7574 6020 6d75 7374  `probe_out` must
-0000ff90: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
-0000ffa0: 6561 6c20 6e75 6d62 6572 2e0a 2020 2020  eal number..    
-0000ffb0: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
-0000ffc0: 2020 2020 2020 2020 2020 2060 7072 6f62             `prob
-0000ffd0: 655f 6f75 7460 206d 7573 7420 6265 2061  e_out` must be a
-0000ffe0: 2070 6f73 6974 6976 6520 7265 616c 206e   positive real n
-0000fff0: 756d 6265 722e 0a0a 2020 2020 2020 2020  umber...        
-00010000: 4578 616d 706c 650a 2020 2020 2020 2020  Example.        
-00010010: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00010020: 5468 6520 6060 4d6f 6c65 6375 6c65 2e73  The ``Molecule.s
-00010030: 7572 6661 6365 2829 6060 206d 6574 686f  urface()`` metho
-00010040: 6420 7461 6b65 7320 7468 6520 6772 6964  d takes the grid
-00010050: 2073 7061 6369 6e67 2c20 7468 6520 7370   spacing, the sp
-00010060: 6865 7269 6361 6c20 7072 6f62 6520 7369  herical probe si
-00010070: 7a65 2074 6f20 6d6f 6465 6c20 7468 6520  ze to model the 
-00010080: 7375 7266 6163 652c 2074 6865 2073 7572  surface, the sur
-00010090: 6661 6365 2072 6570 7265 7365 6e74 6174  face representat
-000100a0: 696f 6e20 616e 6420 7265 7475 726e 7320  ion and returns 
-000100b0: 6120 4e75 6d50 7920 6172 7261 7920 7769  a NumPy array wi
-000100c0: 7468 2074 6865 206d 6f6c 6563 756c 6520  th the molecule 
-000100d0: 706f 696e 7473 2072 6570 7265 7365 6e74  points represent
-000100e0: 696e 6720 7468 6520 5345 5320 696e 2074  ing the SES in t
-000100f0: 6865 2033 4420 6772 6964 2e0a 0a20 2020  he 3D grid...   
-00010100: 2020 2020 2054 6865 206d 6f6c 6563 756c       The molecul
-00010110: 6172 2073 7572 6661 6365 2063 616e 2062  ar surface can b
-00010120: 6520 6d6f 6465 6c6c 6564 2061 733a 0a0a  e modelled as:..
-00010130: 2020 2020 2020 2020 2020 2020 2a20 536f              * So
-00010140: 6c76 656e 7420 4578 636c 7564 6564 2053  lvent Excluded S
-00010150: 7572 6661 6365 2028 5345 5329 3a0a 0a20  urface (SES):.. 
-00010160: 2020 2020 2020 2020 2020 203e 3e3e 2023             >>> #
-00010170: 2053 7572 6661 6365 2052 6570 7265 7365   Surface Represe
-00010180: 6e74 6174 696f 6e3a 2053 4553 0a20 2020  ntation: SES.   
-00010190: 2020 2020 2020 2020 203e 3e3e 2073 7572           >>> sur
-000101a0: 6661 6365 203d 2027 5345 5327 0a20 2020  face = 'SES'.   
-000101b0: 2020 2020 2020 2020 203e 3e3e 2023 2047           >>> # G
-000101c0: 7269 6420 5370 6163 696e 6720 2873 7465  rid Spacing (ste
-000101d0: 7029 3a20 302e 310a 2020 2020 2020 2020  p): 0.1.        
-000101e0: 2020 2020 3e3e 3e20 7374 6570 203d 2030      >>> step = 0
-000101f0: 2e31 0a20 2020 2020 2020 2020 2020 203e  .1.            >
-00010200: 3e3e 2023 2053 7068 6572 6963 616c 2050  >> # Spherical P
-00010210: 726f 6265 2028 7072 6f62 6529 3a20 312e  robe (probe): 1.
-00010220: 340a 2020 2020 2020 2020 2020 2020 3e3e  4.            >>
-00010230: 3e20 7072 6f62 6520 3d20 312e 340a 2020  > probe = 1.4.  
-00010240: 2020 2020 2020 2020 2020 3e3e 3e20 6d6f            >>> mo
-00010250: 6c65 6375 6c65 2e73 7572 6661 6365 2873  lecule.surface(s
-00010260: 7465 703d 7374 6570 2c20 7072 6f62 653d  tep=step, probe=
-00010270: 7072 6f62 652c 2073 7572 6661 6365 3d73  probe, surface=s
-00010280: 7572 6661 6365 290a 2020 2020 2020 2020  urface).        
-00010290: 2020 2020 3e3e 3e20 6d6f 6c65 6375 6c65      >>> molecule
-000102a0: 2e67 7269 640a 2020 2020 2020 2020 2020  .grid.          
-000102b0: 2020 6172 7261 7928 5b5b 5b31 2c20 312c    array([[[1, 1,
-000102c0: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
-000102d0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-000102e0: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
-000102f0: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
-00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010310: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
-00010320: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
-00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010340: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-00010350: 2020 2020 2020 2020 2020 5b31 2c20 312c            [1, 1,
-00010360: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
-00010370: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00010380: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
-00010390: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
-000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103b0: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
-000103c0: 2e2c 2031 2c20 312c 2031 5d5d 2c0a 2020  ., 1, 1, 1]],.  
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-000103f0: 2020 2020 2020 2020 205b 5b31 2c20 312c           [[1, 1,
-00010400: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
-00010410: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00010420: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
-00010430: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
-00010460: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-00010490: 2020 2020 2020 2020 2020 5b31 2c20 312c            [1, 1,
-000104a0: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
-000104b0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-000104c0: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
-000104d0: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
-000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104f0: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
-00010500: 2e2c 2031 2c20 312c 2031 5d5d 5d2c 2064  ., 1, 1, 1]]], d
-00010510: 7479 7065 3d69 6e74 3332 290a 0a20 2020  type=int32)..   
-00010520: 2020 2020 2054 6865 206d 6f6c 6563 756c       The molecul
-00010530: 6172 2073 7572 6661 6365 2063 616e 2062  ar surface can b
-00010540: 6520 6d6f 6465 6c6c 6564 2061 733a 0a0a  e modelled as:..
-00010550: 2020 2020 2020 2020 2020 2020 2a20 536f              * So
-00010560: 6c76 656e 7420 4163 6365 7373 6962 6c65  lvent Accessible
-00010570: 2053 7572 6661 6365 2028 5341 5329 3a0a   Surface (SAS):.
-00010580: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00010590: 2023 2053 7572 6661 6365 2052 6570 7265   # Surface Repre
-000105a0: 7365 6e74 6174 696f 6e3a 2053 4153 0a20  sentation: SAS. 
-000105b0: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
-000105c0: 7572 6661 6365 203d 2027 5341 5327 0a20  urface = 'SAS'. 
-000105d0: 2020 2020 2020 2020 2020 203e 3e3e 2023             >>> #
-000105e0: 2047 7269 6420 5370 6163 696e 6720 2873   Grid Spacing (s
-000105f0: 7465 7029 3a20 302e 310a 2020 2020 2020  tep): 0.1.      
-00010600: 2020 2020 2020 3e3e 3e20 7374 6570 203d        >>> step =
-00010610: 2030 2e31 0a20 2020 2020 2020 2020 2020   0.1.           
-00010620: 203e 3e3e 2023 2053 7068 6572 6963 616c   >>> # Spherical
-00010630: 2050 726f 6265 2028 7072 6f62 6529 3a20   Probe (probe): 
-00010640: 312e 340a 2020 2020 2020 2020 2020 2020  1.4.            
-00010650: 3e3e 3e20 7072 6f62 6520 3d20 312e 340a  >>> probe = 1.4.
-00010660: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00010670: 6d6f 6c65 6375 6c65 2e73 7572 6661 6365  molecule.surface
-00010680: 2873 7465 703d 7374 6570 2c20 7072 6f62  (step=step, prob
-00010690: 653d 7072 6f62 652c 2073 7572 6661 6365  e=probe, surface
-000106a0: 3d73 7572 6661 6365 290a 2020 2020 2020  =surface).      
-000106b0: 2020 2020 2020 3e3e 3e20 6d6f 6c65 6375        >>> molecu
-000106c0: 6c65 2e67 7269 640a 2020 2020 2020 2020  le.grid.        
-000106d0: 2020 2020 6172 7261 7928 5b5b 5b31 2c20      array([[[1, 
-000106e0: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
-000106f0: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
-00010700: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
-00010710: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-00010720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010730: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-00010740: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-00010770: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
-00010780: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
-00010790: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
-000107a0: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
-000107b0: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-000107c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000107d0: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-000107e0: 2e2e 2e2c 2031 2c20 312c 2031 5d5d 2c0a  ..., 1, 1, 1]],.
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-00010810: 2020 2020 2020 2020 2020 205b 5b31 2c20             [[1, 
-00010820: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
-00010830: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
-00010840: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
-00010850: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-00010860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010870: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-00010880: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-000108b0: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
-000108c0: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
-000108d0: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
-000108e0: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
-000108f0: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-00010900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010910: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-00010920: 2e2e 2e2c 2031 2c20 312c 2031 5d5d 5d2c  ..., 1, 1, 1]]],
-00010930: 2064 7479 7065 3d69 6e74 3332 290a 2020   dtype=int32).  
-00010940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010950: 2020 6672 6f6d 205f 7079 4b56 4669 6e64    from _pyKVFind
-00010960: 6572 2069 6d70 6f72 7420 5f66 696c 6c5f  er import _fill_
-00010970: 7265 6365 7074 6f72 0a0a 2020 2020 2020  receptor..      
-00010980: 2020 2320 4368 6563 6b20 6172 6775 6d65    # Check argume
-00010990: 6e74 730a 2020 2020 2020 2020 6966 2074  nts.        if t
-000109a0: 7970 6528 7374 6570 2920 6e6f 7420 696e  ype(step) not in
-000109b0: 205b 696e 742c 2066 6c6f 6174 5d3a 0a20   [int, float]:. 
-000109c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000109d0: 2054 7970 6545 7272 6f72 2822 6073 7465   TypeError("`ste
-000109e0: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
-000109f0: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
-00010a00: 2e22 290a 2020 2020 2020 2020 656c 6966  .").        elif
-00010a10: 2073 7465 7020 3c3d 2030 2e30 3a0a 2020   step <= 0.0:.  
-00010a20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00010a30: 5661 6c75 6545 7272 6f72 2822 6073 7465  ValueError("`ste
-00010a40: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
-00010a50: 6974 6976 6520 7265 616c 206e 756d 6265  itive real numbe
-00010a60: 722e 2229 0a20 2020 2020 2020 2065 6c73  r.").        els
-00010a70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010a80: 656c 662e 5f73 7465 7020 3d20 7374 6570  elf._step = step
-00010a90: 0a0a 2020 2020 2020 2020 2320 5072 6f62  ..        # Prob
-00010aa0: 650a 2020 2020 2020 2020 6966 2074 7970  e.        if typ
-00010ab0: 6528 7072 6f62 6529 206e 6f74 2069 6e20  e(probe) not in 
-00010ac0: 5b69 6e74 2c20 666c 6f61 742c 206e 756d  [int, float, num
-00010ad0: 7079 2e66 6c6f 6174 3634 5d3a 0a20 2020  py.float64]:.   
-00010ae0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00010af0: 7970 6545 7272 6f72 2822 6070 726f 6265  ypeError("`probe
-00010b00: 5f6f 7574 6020 6d75 7374 2062 6520 6120  _out` must be a 
-00010b10: 6e6f 6e2d 6e65 6761 7469 7665 2072 6561  non-negative rea
-00010b20: 6c20 6e75 6d62 6572 2e22 290a 2020 2020  l number.").    
-00010b30: 2020 2020 656c 6966 2070 726f 6265 203c      elif probe <
-00010b40: 3d20 302e 303a 0a20 2020 2020 2020 2020  = 0.0:.         
-00010b50: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00010b60: 726f 7228 2260 7072 6f62 655f 6f75 7460  ror("`probe_out`
-00010b70: 206d 7573 7420 6265 2061 206e 6f6e 2d6e   must be a non-n
-00010b80: 6567 6174 6976 6520 7265 616c 206e 756d  egative real num
-00010b90: 6265 722e 2229 0a20 2020 2020 2020 2073  ber.").        s
-00010ba0: 656c 662e 5f70 726f 6265 203d 2070 726f  elf._probe = pro
-00010bb0: 6265 0a0a 2020 2020 2020 2020 2320 5375  be..        # Su
-00010bc0: 7266 6163 650a 2020 2020 2020 2020 6966  rface.        if
-00010bd0: 2073 7572 6661 6365 203d 3d20 2253 4553   surface == "SES
-00010be0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
-00010bf0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
-00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c10: 7072 696e 7428 223e 2053 7572 6661 6365  print("> Surface
-00010c20: 2072 6570 7265 7365 6e74 6174 696f 6e3a   representation:
-00010c30: 2053 6f6c 7665 6e74 2045 7863 6c75 6465   Solvent Exclude
-00010c40: 6420 5375 7266 6163 6520 2853 4553 292e  d Surface (SES).
-00010c50: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00010c60: 656c 662e 5f72 6570 7265 7365 6e74 6174  elf._representat
-00010c70: 696f 6e20 3d20 7375 7266 6163 650a 2020  ion = surface.  
-00010c80: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
-00010c90: 6520 3d20 5472 7565 0a20 2020 2020 2020  e = True.       
-00010ca0: 2065 6c69 6620 7375 7266 6163 6520 3d3d   elif surface ==
-00010cb0: 2022 5341 5322 3a0a 2020 2020 2020 2020   "SAS":.        
-00010cc0: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
-00010cd0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
-00010ce0: 2020 2020 2070 7269 6e74 2822 3e20 5375       print("> Su
-00010cf0: 7266 6163 6520 7265 7072 6573 656e 7461  rface representa
-00010d00: 7469 6f6e 3a20 536f 6c76 656e 7420 4163  tion: Solvent Ac
-00010d10: 6365 7373 6962 6c65 2053 7572 6661 6365  cessible Surface
-00010d20: 2028 5341 5329 2e22 290a 2020 2020 2020   (SAS).").      
-00010d30: 2020 2020 2020 7365 6c66 2e5f 7265 7072        self._repr
-00010d40: 6573 656e 7461 7469 6f6e 203d 2073 7572  esentation = sur
-00010d50: 6661 6365 0a20 2020 2020 2020 2020 2020  face.           
-00010d60: 2073 7572 6661 6365 203d 2046 616c 7365   surface = False
-00010d70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00010d80: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00010d90: 2056 616c 7565 4572 726f 7228 6622 6073   ValueError(f"`s
-00010da0: 7572 6661 6365 6020 6d75 7374 2062 6520  urface` must be 
-00010db0: 5341 5320 6f72 2053 4553 2c20 6e6f 7420  SAS or SES, not 
-00010dc0: 7b73 7572 6661 6365 7d2e 2229 0a0a 2020  {surface}.")..  
-00010dd0: 2020 2020 2020 2320 4465 6669 6e65 2033        # Define 3
-00010de0: 4420 6772 6964 0a20 2020 2020 2020 2073  D grid.        s
-00010df0: 656c 662e 5f73 6574 5f67 7269 6428 7061  elf._set_grid(pa
-00010e00: 6464 696e 6729 0a0a 2020 2020 2020 2020  dding)..        
-00010e10: 2320 4d6f 6c65 6375 6c61 7220 7375 7266  # Molecular surf
-00010e20: 6163 6520 2853 4553 206f 7220 5341 5329  ace (SES or SAS)
-00010e30: 2074 6f20 6772 6964 0a20 2020 2020 2020   to grid.       
-00010e40: 2073 656c 662e 5f67 7269 6420 3d20 5f66   self._grid = _f
-00010e50: 696c 6c5f 7265 6365 7074 6f72 280a 2020  ill_receptor(.  
-00010e60: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00010e70: 7820 2a20 7365 6c66 2e6e 7920 2a20 7365  x * self.ny * se
-00010e80: 6c66 2e6e 7a2c 0a20 2020 2020 2020 2020  lf.nz,.         
-00010e90: 2020 2073 656c 662e 6e78 2c0a 2020 2020     self.nx,.    
-00010ea0: 2020 2020 2020 2020 7365 6c66 2e6e 792c          self.ny,
-00010eb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010ec0: 662e 6e7a 2c0a 2020 2020 2020 2020 2020  f.nz,.          
-00010ed0: 2020 7365 6c66 2e78 797a 722c 0a20 2020    self.xyzr,.   
-00010ee0: 2020 2020 2020 2020 2073 656c 662e 7031           self.p1
-00010ef0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00010f00: 6c66 2e72 6f74 6174 696f 6e2c 0a20 2020  lf.rotation,.   
-00010f10: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00010f20: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
-00010f30: 7365 6c66 2e70 726f 6265 2c0a 2020 2020  self.probe,.    
-00010f40: 2020 2020 2020 2020 7375 7266 6163 652c          surface,
-00010f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010f60: 662e 6e74 6872 6561 6473 2c0a 2020 2020  f.nthreads,.    
-00010f70: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00010f80: 626f 7365 2c0a 2020 2020 2020 2020 292e  bose,.        ).
-00010f90: 7265 7368 6170 6528 7365 6c66 2e6e 782c  reshape(self.nx,
-00010fa0: 2073 656c 662e 6e79 2c20 7365 6c66 2e6e   self.ny, self.n
-00010fb0: 7a29 0a0a 2020 2020 6465 6620 766f 6c75  z)..    def volu
-00010fc0: 6d65 2873 656c 6629 202d 3e20 666c 6f61  me(self) -> floa
-00010fd0: 743a 0a20 2020 2020 2020 2022 2222 4573  t:.        """Es
-00010fe0: 7469 6d61 7465 2074 6865 2076 6f6c 756d  timate the volum
-00010ff0: 6520 6f66 2074 6865 206d 6f6c 6563 756c  e of the molecul
-00011000: 6520 6261 7365 6420 6f6e 2074 6865 206d  e based on the m
-00011010: 6f6c 6563 756c 6172 2073 7572 6661 6365  olecular surface
-00011020: 2072 6570 7265 7365 6e74 6174 696f 6e2c   representation,
-00011030: 2069 652c 2076 6457 2c20 5345 5320 6f72   ie, vdW, SES or
-00011040: 2053 4153 2072 6570 7265 7365 6e74 6174   SAS representat
-00011050: 696f 6e73 2e0a 0a20 2020 2020 2020 2052  ions...        R
-00011060: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00011070: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2076  ------.        v
-00011080: 6f6c 756d 6520 3a20 666c 6f61 740a 2020  olume : float.  
-00011090: 2020 2020 2020 2020 2020 4d6f 6c65 6375            Molecu
-000110a0: 6c61 7220 766f 6c75 6d65 2028 41c2 b329  lar volume (A..)
-000110b0: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-000110c0: 6c65 0a20 2020 2020 2020 202d 2d2d 2d2d  le.        -----
-000110d0: 2d2d 0a20 2020 2020 2020 2057 6974 6820  --.        With 
-000110e0: 7468 6520 6d6f 6c65 6375 6c61 7220 7375  the molecular su
-000110f0: 7266 6163 6520 6d6f 6465 6c6c 6564 2062  rface modelled b
-00011100: 7920 6060 4d6f 6c65 6375 6c65 2e76 6477  y ``Molecule.vdw
-00011110: 2829 6060 206f 7220 6060 4d6f 6c65 6375  ()`` or ``Molecu
-00011120: 6c65 2e73 7572 6661 6365 2829 6060 2c20  le.surface()``, 
-00011130: 7468 6520 766f 6c75 6d65 2063 616e 2062  the volume can b
-00011140: 6520 6573 7469 6d61 7465 6420 6279 2072  e estimated by r
-00011150: 756e 6e69 6e67 3a0a 0a20 2020 2020 2020  unning:..       
-00011160: 203e 3e3e 206d 6f6c 6563 756c 652e 766f   >>> molecule.vo
-00011170: 6c75 6d65 2829 0a20 2020 2020 2020 2039  lume().        9
-00011180: 302e 380a 2020 2020 2020 2020 2222 220a  0.8.        """.
-00011190: 2020 2020 2020 2020 6672 6f6d 205f 7079          from _py
-000111a0: 4b56 4669 6e64 6572 2069 6d70 6f72 7420  KVFinder import 
-000111b0: 5f76 6f6c 756d 650a 0a20 2020 2020 2020  _volume..       
-000111c0: 2069 6620 7365 6c66 2e67 7269 6420 6973   if self.grid is
-000111d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000111e0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
-000111f0: 5f76 6f6c 756d 6528 0a20 2020 2020 2020  _volume(.       
-00011200: 2020 2020 2020 2020 2028 7365 6c66 2e67           (self.g
-00011210: 7269 6420 3d3d 2030 292e 6173 7479 7065  rid == 0).astype
-00011220: 286e 756d 7079 2e69 6e74 3332 2920 2a20  (numpy.int32) * 
-00011230: 322c 2073 656c 662e 7374 6570 2c20 312c  2, self.step, 1,
-00011240: 2073 656c 662e 6e74 6872 6561 6473 0a20   self.nthreads. 
-00011250: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00011260: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011270: 666c 6f61 7428 766f 6c75 6d65 2e72 6f75  float(volume.rou
-00011280: 6e64 2864 6563 696d 616c 733d 3229 290a  nd(decimals=2)).
-00011290: 0a20 2020 2064 6566 2070 7265 7669 6577  .    def preview
-000112a0: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-000112b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000112c0: 2020 2222 2250 7265 7669 6577 2074 6865    """Preview the
-000112d0: 206d 6f6c 6563 756c 6172 2073 7572 6661   molecular surfa
-000112e0: 6365 2069 6e20 7468 6520 3344 2067 7269  ce in the 3D gri
-000112f0: 642e 0a0a 2020 2020 2020 2020 4578 616d  d...        Exam
-00011300: 706c 650a 2020 2020 2020 2020 2d2d 2d2d  ple.        ----
-00011310: 2d2d 2d0a 2020 2020 2020 2020 5769 7468  ---.        With
-00011320: 2074 6865 206d 6f6c 6563 756c 6172 2073   the molecular s
-00011330: 7572 6661 6365 206d 6f64 656c 6c65 6420  urface modelled 
-00011340: 6279 2060 604d 6f6c 6563 756c 652e 7664  by ``Molecule.vd
-00011350: 7728 2960 6020 6f72 2060 604d 6f6c 6563  w()`` or ``Molec
-00011360: 756c 652e 7375 7266 6163 6528 2960 602c  ule.surface()``,
-00011370: 2074 6865 206d 6f64 656c 6c65 6420 6d6f   the modelled mo
-00011380: 6c65 6375 6c65 2069 6e20 7468 6520 3344  lecule in the 3D
-00011390: 2067 7269 6420 6361 6e20 6265 2070 7265   grid can be pre
-000113a0: 7669 6577 6564 2062 7920 7275 6e6e 696e  viewed by runnin
-000113b0: 673a 0a0a 2020 2020 2020 2020 3e3e 3e20  g:..        >>> 
-000113c0: 6d6f 6c65 6375 6c65 2e70 7265 7669 6577  molecule.preview
-000113d0: 2829 0a20 2020 2020 2020 2022 2222 0a20  ().        """. 
-000113e0: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
-000113f0: 7269 6420 6973 206e 6f74 204e 6f6e 653a  rid is not None:
-00011400: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-00011410: 6d20 706c 6f74 6c79 2e65 7870 7265 7373  m plotly.express
-00011420: 2069 6d70 6f72 7420 7363 6174 7465 725f   import scatter_
-00011430: 3364 0a0a 2020 2020 2020 2020 2020 2020  3d..            
-00011440: 782c 2079 2c20 7a20 3d20 6e75 6d70 792e  x, y, z = numpy.
-00011450: 6e6f 6e7a 6572 6f28 7365 6c66 2e67 7269  nonzero(self.gri
-00011460: 6420 3d3d 2030 290a 2020 2020 2020 2020  d == 0).        
-00011470: 2020 2020 6669 6720 3d20 7363 6174 7465      fig = scatte
-00011480: 725f 3364 2878 3d78 2c20 793d 792c 207a  r_3d(x=x, y=y, z
-00011490: 3d7a 2c20 2a2a 6b77 6172 6773 290a 2020  =z, **kwargs).  
-000114a0: 2020 2020 2020 2020 2020 6669 672e 7570            fig.up
-000114b0: 6461 7465 5f6c 6179 6f75 7428 0a20 2020  date_layout(.   
-000114c0: 2020 2020 2020 2020 2020 2020 2073 6365               sce
-000114d0: 6e65 5f78 6178 6973 5f73 686f 7774 6963  ne_xaxis_showtic
-000114e0: 6b6c 6162 656c 733d 4661 6c73 652c 0a20  klabels=False,. 
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011500: 6365 6e65 5f79 6178 6973 5f73 686f 7774  cene_yaxis_showt
-00011510: 6963 6b6c 6162 656c 733d 4661 6c73 652c  icklabels=False,
-00011520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011530: 2073 6365 6e65 5f7a 6178 6973 5f73 686f   scene_zaxis_sho
-00011540: 7774 6963 6b6c 6162 656c 733d 4661 6c73  wticklabels=Fals
-00011550: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-00011560: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
-00011570: 2e73 686f 7728 290a 0a20 2020 2064 6566  .show()..    def
-00011580: 2065 7870 6f72 7428 0a20 2020 2020 2020   export(.       
-00011590: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
-000115a0: 6e3a 2055 6e69 6f6e 5b73 7472 2c20 7061  n: Union[str, pa
-000115b0: 7468 6c69 622e 5061 7468 5d20 3d20 226d  thlib.Path] = "m
-000115c0: 6f6c 6563 756c 652e 7064 6222 2c0a 2020  olecule.pdb",.  
-000115d0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-000115e0: 2020 2020 2022 2222 4578 706f 7274 206d       """Export m
-000115f0: 6f6c 6563 756c 6520 706f 696e 7473 2028  olecule points (
-00011600: 4829 2074 6f20 6120 5044 422d 666f 726d  H) to a PDB-form
-00011610: 6174 7465 6420 6669 6c65 2e0a 0a20 2020  atted file...   
-00011620: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00011630: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00011640: 2d2d 0a20 2020 2020 2020 2066 6e20 3a20  --.        fn : 
-00011650: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-00011660: 6962 2e50 6174 685d 2c20 6f70 7469 6f6e  ib.Path], option
-00011670: 616c 0a20 2020 2020 2020 2020 2020 2041  al.            A
-00011680: 2066 696c 6520 7061 7468 2074 6f20 7468   file path to th
-00011690: 6520 6d6f 6c65 6375 6c61 7220 766f 6c75  e molecular volu
-000116a0: 6d65 2069 6e20 7468 6520 6772 6964 2d62  me in the grid-b
-000116b0: 6173 6564 2072 6572 7065 7365 6e74 6174  ased rerpesentat
-000116c0: 696f 6e20 696e 2050 4442 2066 6f72 6d61  ion in PDB forma
-000116d0: 742c 2062 7920 6465 6661 756c 7420 226d  t, by default "m
-000116e0: 6f6c 6563 756c 652e 7064 6222 2e0a 0a20  olecule.pdb"... 
-000116f0: 2020 2020 2020 2052 6169 7365 730a 2020         Raises.  
-00011700: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-00011710: 2020 2020 2054 7970 6545 7272 6f72 0a20       TypeError. 
-00011720: 2020 2020 2020 2020 2020 2060 666e 6020             `fn` 
-00011730: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
-00011740: 206f 7220 6120 7061 7468 6c69 622e 5061   or a pathlib.Pa
-00011750: 7468 2e0a 0a20 2020 2020 2020 2045 7861  th...        Exa
-00011760: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
-00011770: 2d2d 2d2d 0a20 2020 2020 2020 2057 6974  ----.        Wit
-00011780: 6820 7468 6520 6d6f 6c65 6375 6c61 7220  h the molecular 
-00011790: 7375 7266 6163 6520 6d6f 6465 6c6c 6564  surface modelled
-000117a0: 2062 7920 6060 4d6f 6c65 6375 6c65 2e76   by ``Molecule.v
-000117b0: 6477 2829 6060 206f 7220 6060 4d6f 6c65  dw()`` or ``Mole
-000117c0: 6375 6c65 2e73 7572 6661 6365 2829 6060  cule.surface()``
-000117d0: 2c20 7468 6520 6d6f 6465 6c6c 6564 206d  , the modelled m
-000117e0: 6f6c 6563 756c 6520 696e 2074 6865 2033  olecule in the 3
-000117f0: 4420 6772 6964 2063 616e 2062 6520 6578  D grid can be ex
-00011800: 706f 7274 6564 2074 6f20 6120 5044 422d  ported to a PDB-
-00011810: 666f 726d 6174 7465 6420 6669 6c65 2062  formatted file b
-00011820: 7920 7275 6e6e 696e 673a 0a0a 2020 2020  y running:..    
-00011830: 2020 2020 3e3e 3e20 6d6f 6c65 6375 6c65      >>> molecule
-00011840: 2e65 7870 6f72 7428 276d 6f64 656c 2e70  .export('model.p
-00011850: 6462 2729 0a20 2020 2020 2020 2022 2222  db').        """
-00011860: 0a20 2020 2020 2020 2023 2046 696c 656e  .        # Filen
-00011870: 616d 6520 2866 6e29 0a20 2020 2020 2020  ame (fn).       
-00011880: 2069 6620 7479 7065 2866 6e29 206e 6f74   if type(fn) not
-00011890: 2069 6e20 5b73 7472 2c20 7061 7468 6c69   in [str, pathli
-000118a0: 622e 5061 7468 5d3a 0a20 2020 2020 2020  b.Path]:.       
-000118b0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-000118c0: 7272 6f72 2822 6066 6e60 206d 7573 7420  rror("`fn` must 
-000118d0: 6265 2061 2073 7472 696e 6720 6f72 2061  be a string or a
-000118e0: 2070 6174 686c 6962 2e50 6174 682e 2229   pathlib.Path.")
-000118f0: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
-00011900: 6469 7273 286f 732e 7061 7468 2e61 6273  dirs(os.path.abs
-00011910: 7061 7468 286f 732e 7061 7468 2e64 6972  path(os.path.dir
-00011920: 6e61 6d65 2866 6e29 292c 2065 7869 7374  name(fn)), exist
-00011930: 5f6f 6b3d 5472 7565 290a 0a20 2020 2020  _ok=True)..     
-00011940: 2020 2023 2053 6176 6520 6772 6964 2074     # Save grid t
-00011950: 6f20 5044 4220 6669 6c65 0a20 2020 2020  o PDB file.     
-00011960: 2020 2065 7870 6f72 7428 0a20 2020 2020     export(.     
-00011970: 2020 2020 2020 2066 6e2c 2028 7365 6c66         fn, (self
-00011980: 2e67 7269 6420 3d3d 2030 292e 6173 7479  .grid == 0).asty
-00011990: 7065 286e 756d 7079 2e69 6e74 3332 2920  pe(numpy.int32) 
-000119a0: 2a20 322c 204e 6f6e 652c 2073 656c 662e  * 2, None, self.
-000119b0: 7665 7274 6963 6573 2c20 7365 6c66 2e73  vertices, self.s
-000119c0: 7465 700a 2020 2020 2020 2020 290a       tep.        ).
+00001a10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00001a20: 2020 2020 2020 2073 6361 6c65 732c 2061         scales, a
+00001a30: 7667 5f68 7964 726f 7061 7468 7920 3d20  vg_hydropathy = 
+00001a40: 4e6f 6e65 2c20 4e6f 6e65 0a0a 2020 2020  None, None..    
+00001a50: 2020 2020 2320 4578 706f 7274 2063 6176      # Export cav
+00001a60: 6974 6965 730a 2020 2020 2020 2020 6f75  ities.        ou
+00001a70: 7470 7574 5f63 6176 6974 7920 3d20 6f73  tput_cavity = os
+00001a80: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
+00001a90: 2020 2020 2020 2020 6172 6773 2e6f 7574          args.out
+00001aa0: 7075 745f 6469 7265 6374 6f72 792c 2066  put_directory, f
+00001ab0: 227b 6172 6773 2e62 6173 655f 6e61 6d65  "{args.base_name
+00001ac0: 7d2e 4b56 4669 6e64 6572 2e6f 7574 7075  }.KVFinder.outpu
+00001ad0: 742e 7064 6222 0a20 2020 2020 2020 2029  t.pdb".        )
+00001ae0: 0a20 2020 2020 2020 2065 7870 6f72 7428  .        export(
+00001af0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00001b00: 7075 745f 6361 7669 7479 2c0a 2020 2020  put_cavity,.    
+00001b10: 2020 2020 2020 2020 6361 7669 7469 6573          cavities
+00001b20: 2c0a 2020 2020 2020 2020 2020 2020 7375  ,.            su
+00001b30: 7266 6163 652c 0a20 2020 2020 2020 2020  rface,.         
+00001b40: 2020 2061 7267 732e 7665 7274 6963 6573     args.vertices
+00001b50: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00001b60: 6773 2e73 7465 702c 0a20 2020 2020 2020  gs.step,.       
+00001b70: 2020 2020 2064 6570 7468 732c 0a20 2020       depths,.   
+00001b80: 2020 2020 2020 2020 2073 6361 6c65 732c           scales,
+00001b90: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
+00001ba0: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
+00001bb0: 7267 732e 6e74 6872 6561 6473 2c0a 2020  rgs.nthreads,.  
+00001bc0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00001bd0: 2023 2057 7269 7465 2072 6573 756c 7473   # Write results
+00001be0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+00001bf0: 7265 7375 6c74 7320 3d20 6f73 2e70 6174  results = os.pat
+00001c00: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
+00001c10: 2020 2020 6172 6773 2e6f 7574 7075 745f      args.output_
+00001c20: 6469 7265 6374 6f72 792c 2066 227b 6172  directory, f"{ar
+00001c30: 6773 2e62 6173 655f 6e61 6d65 7d2e 4b56  gs.base_name}.KV
+00001c40: 4669 6e64 6572 2e72 6573 756c 7473 2e74  Finder.results.t
+00001c50: 6f6d 6c22 0a20 2020 2020 2020 2029 0a20  oml".        ). 
+00001c60: 2020 2020 2020 2077 7269 7465 5f72 6573         write_res
+00001c70: 756c 7473 280a 2020 2020 2020 2020 2020  ults(.          
+00001c80: 2020 6f75 7470 7574 5f72 6573 756c 7473    output_results
+00001c90: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00001ca0: 6773 2e69 6e70 7574 2c0a 2020 2020 2020  gs.input,.      
+00001cb0: 2020 2020 2020 6172 6773 2e6c 6967 616e        args.ligan
+00001cc0: 642c 0a20 2020 2020 2020 2020 2020 206f  d,.            o
+00001cd0: 7574 7075 745f 6361 7669 7479 2c0a 2020  utput_cavity,.  
+00001ce0: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+00001cf0: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00001d00: 6561 2c0a 2020 2020 2020 2020 2020 2020  ea,.            
+00001d10: 6d61 785f 6465 7074 682c 0a20 2020 2020  max_depth,.     
+00001d20: 2020 2020 2020 2061 7667 5f64 6570 7468         avg_depth
+00001d30: 2c0a 2020 2020 2020 2020 2020 2020 6176  ,.            av
+00001d40: 675f 6879 6472 6f70 6174 6879 2c0a 2020  g_hydropathy,.  
+00001d50: 2020 2020 2020 2020 2020 7265 7369 6475            residu
+00001d60: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00001d70: 6672 6571 7565 6e63 6965 732c 0a20 2020  frequencies,.   
+00001d80: 2020 2020 2020 2020 2061 7267 732e 7374           args.st
+00001d90: 6570 2c0a 2020 2020 2020 2020 290a 0a20  ep,.        ).. 
+00001da0: 2020 2020 2020 2023 2057 7269 7465 2070         # Write p
+00001db0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00001dc0: 2020 5f77 7269 7465 5f70 6172 616d 6574    _write_paramet
+00001dd0: 6572 7328 6172 6773 290a 2020 2020 656c  ers(args).    el
+00001de0: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
+00001df0: 7428 223e 204e 6f20 6361 7669 7469 6573  t("> No cavities
+00001e00: 2064 6574 6563 7465 6421 2229 0a0a 2020   detected!")..  
+00001e10: 2020 2320 456c 6170 7365 6420 7469 6d65    # Elapsed time
+00001e20: 0a20 2020 2065 6c61 7073 6564 5f74 696d  .    elapsed_tim
+00001e30: 6520 3d20 7469 6d65 2e74 696d 6528 2920  e = time.time() 
+00001e40: 2d20 7374 6172 745f 7469 6d65 0a20 2020  - start_time.   
+00001e50: 2070 7269 6e74 2866 225b 205c 3033 335b   print(f"[ \033[
+00001e60: 316d 456c 6170 7365 6420 7469 6d65 3a5c  1mElapsed time:\
+00001e70: 3033 335b 306d 207b 656c 6170 7365 645f  033[0m {elapsed_
+00001e80: 7469 6d65 3a2e 3466 7d73 205d 2229 0a20  time:.4f}s ]"). 
+00001e90: 2020 206c 6f67 6769 6e67 2e69 6e66 6f28     logging.info(
+00001ea0: 6622 5b20 456c 6170 7365 6420 7469 6d65  f"[ Elapsed time
+00001eb0: 2028 7329 3a20 7b65 6c61 7073 6564 5f74   (s): {elapsed_t
+00001ec0: 696d 653a 2e34 667d 7320 5d5c 6e22 290a  ime:.4f}s ]\n").
+00001ed0: 0a20 2020 2072 6574 7572 6e20 300a 0a0a  .    return 0...
+00001ee0: 636c 6173 7320 7079 4b56 4669 6e64 6572  class pyKVFinder
+00001ef0: 5265 7375 6c74 7328 6f62 6a65 6374 293a  Results(object):
+00001f00: 0a20 2020 2022 2222 4120 636c 6173 7320  .    """A class 
+00001f10: 636f 6e74 6169 6e69 6e67 2070 794b 5646  containing pyKVF
+00001f20: 696e 6465 7220 6465 7465 6374 696f 6e20  inder detection 
+00001f30: 616e 6420 6368 6172 6163 7465 7269 7a61  and characteriza
+00001f40: 7469 6f6e 2072 6573 756c 7473 2e0a 0a20  tion results... 
+00001f50: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00001f60: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00001f70: 2063 6176 6974 6965 7320 3a20 6e75 6d70   cavities : nump
+00001f80: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
+00001f90: 2020 4361 7669 7479 2070 6f69 6e74 7320    Cavity points 
+00001fa0: 696e 2074 6865 2033 4420 6772 6964 2028  in the 3D grid (
+00001fb0: 6361 7669 7469 6573 5b6e 785d 5b6e 795d  cavities[nx][ny]
+00001fc0: 5b6e 7a5d 292e 0a20 2020 2020 2020 2043  [nz])..        C
+00001fd0: 6176 6974 6965 7320 6172 7261 7920 6861  avities array ha
+00001fe0: 7320 696e 7465 6765 7220 6c61 6265 6c73  s integer labels
+00001ff0: 2069 6e20 6561 6368 2070 6f73 6974 696f   in each positio
+00002000: 6e2c 2074 6861 7420 6172 653a 0a0a 2020  n, that are:..  
+00002010: 2020 2020 2020 2020 2020 2a20 2d31 3a20            * -1: 
+00002020: 6275 6c6b 2070 6f69 6e74 733b 0a0a 2020  bulk points;..  
+00002030: 2020 2020 2020 2020 2020 2a20 303a 2062            * 0: b
+00002040: 696f 6d6f 6c65 6375 6c65 2070 6f69 6e74  iomolecule point
+00002050: 733b 0a0a 2020 2020 2020 2020 2020 2020  s;..            
+00002060: 2a20 313a 2065 6d70 7479 2073 7061 6365  * 1: empty space
+00002070: 2070 6f69 6e74 733b 0a0a 2020 2020 2020   points;..      
+00002080: 2020 2020 2020 2a20 3e3d 323a 2063 6176        * >=2: cav
+00002090: 6974 7920 706f 696e 7473 2e0a 0a20 2020  ity points...   
+000020a0: 2020 2020 2054 6865 2065 6d70 7479 2073       The empty s
+000020b0: 7061 6365 2070 6f69 6e74 7320 6172 6520  pace points are 
+000020c0: 7265 6769 6f6e 7320 7468 6174 2064 6f20  regions that do 
+000020d0: 6e6f 7420 6d65 6574 2074 6865 2063 686f  not meet the cho
+000020e0: 7365 6e0a 2020 2020 2020 2020 766f 6c75  sen.        volu
+000020f0: 6d65 2063 7574 6f66 6620 746f 2062 6520  me cutoff to be 
+00002100: 636f 6e73 6964 6572 6564 2061 2063 6176  considered a cav
+00002110: 6974 792e 0a20 2020 2073 7572 6661 6365  ity..    surface
+00002120: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+00002130: 0a20 2020 2020 2020 2053 7572 6661 6365  .        Surface
+00002140: 2070 6f69 6e74 7320 696e 2074 6865 2033   points in the 3
+00002150: 4420 6772 6964 2028 7375 7266 6163 655b  D grid (surface[
+00002160: 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a 2020  nx][ny][nz])..  
+00002170: 2020 2020 2020 5375 7266 6163 6520 6172        Surface ar
+00002180: 7261 7920 6861 7320 696e 7465 6765 7220  ray has integer 
+00002190: 6c61 6265 6c73 2069 6e20 6561 6368 2070  labels in each p
+000021a0: 6f73 6974 696f 6e2c 2074 6861 7420 6172  osition, that ar
+000021b0: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
+000021c0: 2a20 2d31 3a20 6275 6c6b 2070 6f69 6e74  * -1: bulk point
+000021d0: 733b 0a0a 2020 2020 2020 2020 2020 2020  s;..            
+000021e0: 2a20 303a 2062 696f 6d6f 6c65 6375 6c65  * 0: biomolecule
+000021f0: 206f 7220 656d 7074 7920 7370 6163 6520   or empty space 
+00002200: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
+00002210: 2020 2020 202a 203e 3d32 3a20 7375 7266       * >=2: surf
+00002220: 6163 6520 706f 696e 7473 2e0a 0a20 2020  ace points...   
+00002230: 2020 2020 2054 6865 2065 6d70 7479 2073       The empty s
+00002240: 7061 6365 2070 6f69 6e74 7320 6172 6520  pace points are 
+00002250: 7265 6769 6f6e 7320 7468 6174 2064 6f20  regions that do 
+00002260: 6e6f 7420 6d65 6574 2074 6865 2063 686f  not meet the cho
+00002270: 7365 6e0a 2020 2020 2020 2020 766f 6c75  sen.        volu
+00002280: 6d65 2063 7574 6f66 6620 746f 2062 6520  me cutoff to be 
+00002290: 636f 6e73 6964 6572 6564 2061 2063 6176  considered a cav
+000022a0: 6974 792e 0a20 2020 2064 6570 7468 7320  ity..    depths 
+000022b0: 3a20 6e75 6d70 792e 6e64 6172 7261 792c  : numpy.ndarray,
+000022c0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+000022d0: 2020 4120 6e75 6d70 792e 6e64 6172 7261    A numpy.ndarra
+000022e0: 7920 7769 7468 2064 6570 7468 206f 6620  y with depth of 
+000022f0: 6361 7669 7479 2070 6f69 6e74 7320 2864  cavity points (d
+00002300: 6570 7468 5b6e 785d 5b6e 795d 5b6e 7a5d  epth[nx][ny][nz]
+00002310: 292e 0a20 2020 2073 6361 6c65 7320 3a20  )..    scales : 
+00002320: 6e75 6d70 792e 6e64 6172 7261 792c 206f  numpy.ndarray, o
+00002330: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00002340: 4120 6e75 6d70 792e 6e64 6172 7261 7920  A numpy.ndarray 
+00002350: 7769 7468 2068 7964 726f 7068 6f62 6963  with hydrophobic
+00002360: 6974 7920 7363 616c 6520 7661 6c75 6520  ity scale value 
+00002370: 6d61 7070 6564 2061 7420 7375 7266 6163  mapped at surfac
+00002380: 650a 2020 2020 2020 2020 706f 696e 7473  e.        points
+00002390: 2028 7363 616c 6573 5b6e 785d 5b6e 795d   (scales[nx][ny]
+000023a0: 5b6e 7a5d 292e 0a20 2020 2076 6f6c 756d  [nz])..    volum
+000023b0: 6520 3a20 4469 6374 5b73 7472 2c20 666c  e : Dict[str, fl
+000023c0: 6f61 745d 0a20 2020 2020 2020 2041 2064  oat].        A d
+000023d0: 6963 7469 6f6e 6172 7920 7769 7468 2076  ictionary with v
+000023e0: 6f6c 756d 6520 6f66 2065 6163 6820 6465  olume of each de
+000023f0: 7465 6374 6564 2063 6176 6974 792e 0a20  tected cavity.. 
+00002400: 2020 2061 7265 6120 3a20 4469 6374 5b73     area : Dict[s
+00002410: 7472 2c20 666c 6f61 745d 0a20 2020 2020  tr, float].     
+00002420: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00002430: 7769 7468 2061 7265 6120 6f66 2065 6163  with area of eac
+00002440: 6820 6465 7465 6374 6564 2063 6176 6974  h detected cavit
+00002450: 792e 0a20 2020 206d 6178 5f64 6570 7468  y..    max_depth
+00002460: 203a 2044 6963 745b 7374 722c 2066 6c6f   : Dict[str, flo
+00002470: 6174 5d2c 206f 7074 696f 6e61 6c0a 2020  at], optional.  
+00002480: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
+00002490: 7279 2077 6974 6820 6d61 7869 6d75 6d20  ry with maximum 
+000024a0: 6465 7074 6820 6f66 2065 6163 6820 6465  depth of each de
+000024b0: 7465 6374 6564 2063 6176 6974 792e 0a20  tected cavity.. 
+000024c0: 2020 2061 7667 5f64 6570 7468 203a 2044     avg_depth : D
+000024d0: 6963 745b 7374 722c 2066 6c6f 6174 5d2c  ict[str, float],
+000024e0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+000024f0: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
+00002500: 6974 6820 6176 6572 6167 6520 6465 7074  ith average dept
+00002510: 6820 6f66 2065 6163 6820 6465 7465 6374  h of each detect
+00002520: 6564 2063 6176 6974 792e 0a20 2020 2061  ed cavity..    a
+00002530: 7667 5f68 7964 726f 7061 7468 7920 3a20  vg_hydropathy : 
+00002540: 4469 6374 5b73 7472 2c20 666c 6f61 745d  Dict[str, float]
+00002550: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00002560: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00002570: 7769 7468 2061 7665 7261 6765 2068 7964  with average hyd
+00002580: 726f 7061 7468 7920 666f 7220 6561 6368  ropathy for each
+00002590: 2064 6574 6563 7465 6420 6361 7669 7479   detected cavity
+000025a0: 2061 6e64 0a20 2020 2020 2020 2074 6865   and.        the
+000025b0: 2072 616e 6765 206f 6620 7468 6520 6879   range of the hy
+000025c0: 6472 6f70 686f 6269 6369 7479 2073 6361  drophobicity sca
+000025d0: 6c65 2028 6d69 6e2c 206d 6178 292e 0a20  le (min, max).. 
+000025e0: 2020 2072 6573 6964 7565 733a 2044 6963     residues: Dic
+000025f0: 745b 7374 722c 204c 6973 745b 4c69 7374  t[str, List[List
+00002600: 5b73 7472 5d5d 5d0a 2020 2020 2020 2020  [str]]].        
+00002610: 4120 6469 6374 696f 6e61 7279 2077 6974  A dictionary wit
+00002620: 6820 6120 6c69 7374 206f 6620 696e 7465  h a list of inte
+00002630: 7266 6163 6520 7265 7369 6475 6573 2066  rface residues f
+00002640: 6f72 2065 6163 6820 6465 7465 6374 6564  or each detected
+00002650: 0a20 2020 2020 2020 2063 6176 6974 792e  .        cavity.
+00002660: 0a20 2020 2066 7265 7175 656e 6369 6573  .    frequencies
+00002670: 203a 2044 6963 745b 7374 722c 2044 6963   : Dict[str, Dic
+00002680: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
+00002690: 2069 6e74 5d5d 5d2c 206f 7074 696f 6e61   int]]], optiona
+000026a0: 6c0a 2020 2020 2020 2020 4120 6469 6374  l.        A dict
+000026b0: 696f 6e61 7279 2077 6974 6820 6672 6571  ionary with freq
+000026c0: 7565 6e63 6965 7320 6f66 2072 6573 6964  uencies of resid
+000026d0: 7565 7320 616e 6420 636c 6173 7320 666f  ues and class fo
+000026e0: 720a 2020 2020 2020 2020 7265 7369 6475  r.        residu
+000026f0: 6573 206f 6620 6561 6368 2064 6574 6563  es of each detec
+00002700: 7465 6420 6361 7669 7479 2e0a 2020 2020  ted cavity..    
+00002710: 5f76 6572 7469 6365 7320 3a20 6e75 6d70  _vertices : nump
+00002720: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
+00002730: 2020 4120 6e75 6d70 792e 6e64 6172 7261    A numpy.ndarra
+00002740: 7920 6f72 2061 206c 6973 7420 7769 7468  y or a list with
+00002750: 2078 797a 2076 6572 7469 6365 7320 636f   xyz vertices co
+00002760: 6f72 6469 6e61 7465 7320 286f 7269 6769  ordinates (origi
+00002770: 6e2c 0a20 2020 2020 2020 2058 2d61 7869  n,.        X-axi
+00002780: 732c 2059 2d61 7869 732c 205a 2d61 7869  s, Y-axis, Z-axi
+00002790: 7329 2e0a 2020 2020 5f73 7465 7020 3a20  s)..    _step : 
+000027a0: 666c 6f61 740a 2020 2020 2020 2020 4772  float.        Gr
+000027b0: 6964 2073 7061 6369 6e67 2028 4129 2e0a  id spacing (A)..
+000027c0: 2020 2020 5f69 6e70 7574 203a 2055 6e69      _input : Uni
+000027d0: 6f6e 5b73 7472 2c20 7061 7468 6c69 622e  on[str, pathlib.
+000027e0: 5061 7468 5d2c 206f 7074 696f 6e61 6c0a  Path], optional.
+000027f0: 2020 2020 2020 2020 4120 7061 7468 2074          A path t
+00002800: 6f20 696e 7075 7420 5044 4220 6f72 2058  o input PDB or X
+00002810: 595a 2066 696c 652c 2062 7920 6465 6661  YZ file, by defa
+00002820: 756c 7420 4e6f 6e65 2e0a 2020 2020 5f6c  ult None..    _l
+00002830: 6967 616e 6420 3a20 556e 696f 6e5b 7374  igand : Union[st
+00002840: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+00002850: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00002860: 2020 2041 2070 6174 6820 746f 206c 6967     A path to lig
+00002870: 616e 6420 5044 4220 6f72 2058 595a 2066  and PDB or XYZ f
+00002880: 696c 652c 2062 7920 6465 6661 756c 7420  ile, by default 
+00002890: 4e6f 6e65 2e0a 0a20 2020 2041 7474 7269  None...    Attri
+000028a0: 6275 7465 730a 2020 2020 2d2d 2d2d 2d2d  butes.    ------
+000028b0: 2d2d 2d2d 0a20 2020 2063 6176 6974 6965  ----.    cavitie
+000028c0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+000028d0: 790a 2020 2020 2020 2020 4361 7669 7479  y.        Cavity
+000028e0: 2070 6f69 6e74 7320 696e 2074 6865 2033   points in the 3
+000028f0: 4420 6772 6964 2028 6361 7669 7469 6573  D grid (cavities
+00002900: 5b6e 785d 5b6e 795d 5b6e 7a5d 292e 0a20  [nx][ny][nz]).. 
+00002910: 2020 2020 2020 2043 6176 6974 6965 7320         Cavities 
+00002920: 6172 7261 7920 6861 7320 696e 7465 6765  array has intege
+00002930: 7220 6c61 6265 6c73 2069 6e20 6561 6368  r labels in each
+00002940: 2070 6f73 6974 696f 6e2c 2074 6861 7420   position, that 
+00002950: 6172 653a 0a0a 2020 2020 2020 2020 2020  are:..          
+00002960: 2020 2a20 2d31 3a20 6275 6c6b 2070 6f69    * -1: bulk poi
+00002970: 6e74 733b 0a0a 2020 2020 2020 2020 2020  nts;..          
+00002980: 2020 2a20 303a 2062 696f 6d6f 6c65 6375    * 0: biomolecu
+00002990: 6c65 2070 6f69 6e74 733b 0a0a 2020 2020  le points;..    
+000029a0: 2020 2020 2020 2020 2a20 313a 2065 6d70          * 1: emp
+000029b0: 7479 2073 7061 6365 2070 6f69 6e74 733b  ty space points;
+000029c0: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+000029d0: 3e3d 323a 2063 6176 6974 7920 706f 696e  >=2: cavity poin
+000029e0: 7473 2e0a 0a20 2020 2020 2020 2054 6865  ts...        The
+000029f0: 2065 6d70 7479 2073 7061 6365 2070 6f69   empty space poi
+00002a00: 6e74 7320 6172 6520 7265 6769 6f6e 7320  nts are regions 
+00002a10: 7468 6174 2064 6f20 6e6f 7420 6d65 6574  that do not meet
+00002a20: 2074 6865 2063 686f 7365 6e0a 2020 2020   the chosen.    
+00002a30: 2020 2020 766f 6c75 6d65 2063 7574 6f66      volume cutof
+00002a40: 6620 746f 2062 6520 636f 6e73 6964 6572  f to be consider
+00002a50: 6564 2061 2063 6176 6974 792e 0a20 2020  ed a cavity..   
+00002a60: 2073 7572 6661 6365 203a 206e 756d 7079   surface : numpy
+00002a70: 2e6e 6461 7272 6179 0a20 2020 2020 2020  .ndarray.       
+00002a80: 2053 7572 6661 6365 2070 6f69 6e74 7320   Surface points 
+00002a90: 696e 2074 6865 2033 4420 6772 6964 2028  in the 3D grid (
+00002aa0: 7375 7266 6163 655b 6e78 5d5b 6e79 5d5b  surface[nx][ny][
+00002ab0: 6e7a 5d29 2e0a 2020 2020 2020 2020 5375  nz])..        Su
+00002ac0: 7266 6163 6520 6172 7261 7920 6861 7320  rface array has 
+00002ad0: 696e 7465 6765 7220 6c61 6265 6c73 2069  integer labels i
+00002ae0: 6e20 6561 6368 2070 6f73 6974 696f 6e2c  n each position,
+00002af0: 2074 6861 7420 6172 653a 0a0a 2020 2020   that are:..    
+00002b00: 2020 2020 2020 2020 2a20 2d31 3a20 6275          * -1: bu
+00002b10: 6c6b 2070 6f69 6e74 733b 0a0a 2020 2020  lk points;..    
+00002b20: 2020 2020 2020 2020 2a20 303a 2062 696f          * 0: bio
+00002b30: 6d6f 6c65 6375 6c65 206f 7220 656d 7074  molecule or empt
+00002b40: 7920 7370 6163 6520 706f 696e 7473 3b0a  y space points;.
+00002b50: 0a20 2020 2020 2020 2020 2020 202a 203e  .            * >
+00002b60: 3d32 3a20 7375 7266 6163 6520 706f 696e  =2: surface poin
+00002b70: 7473 2e0a 0a20 2020 2020 2020 2054 6865  ts...        The
+00002b80: 2065 6d70 7479 2073 7061 6365 2070 6f69   empty space poi
+00002b90: 6e74 7320 6172 6520 7265 6769 6f6e 7320  nts are regions 
+00002ba0: 7468 6174 2064 6f20 6e6f 7420 6d65 6574  that do not meet
+00002bb0: 2074 6865 2063 686f 7365 6e0a 2020 2020   the chosen.    
+00002bc0: 2020 2020 766f 6c75 6d65 2063 7574 6f66      volume cutof
+00002bd0: 6620 746f 2062 6520 636f 6e73 6964 6572  f to be consider
+00002be0: 6564 2061 2063 6176 6974 792e 0a20 2020  ed a cavity..   
+00002bf0: 2064 6570 7468 7320 3a20 6e75 6d70 792e   depths : numpy.
+00002c00: 6e64 6172 7261 792c 206f 7074 696f 6e61  ndarray, optiona
+00002c10: 6c0a 2020 2020 2020 2020 4120 6e75 6d70  l.        A nump
+00002c20: 792e 6e64 6172 7261 7920 7769 7468 2064  y.ndarray with d
+00002c30: 6570 7468 206f 6620 6361 7669 7479 2070  epth of cavity p
+00002c40: 6f69 6e74 7320 2864 6570 7468 5b6e 785d  oints (depth[nx]
+00002c50: 5b6e 795d 5b6e 7a5d 292e 0a20 2020 2073  [ny][nz])..    s
+00002c60: 6361 6c65 7320 3a20 6e75 6d70 792e 6e64  cales : numpy.nd
+00002c70: 6172 7261 792c 206f 7074 696f 6e61 6c0a  array, optional.
+00002c80: 2020 2020 2020 2020 4120 6e75 6d70 792e          A numpy.
+00002c90: 6e64 6172 7261 7920 7769 7468 2068 7964  ndarray with hyd
+00002ca0: 726f 7068 6f62 6963 6974 7920 7363 616c  rophobicity scal
+00002cb0: 6520 7661 6c75 6520 6d61 7070 6564 2061  e value mapped a
+00002cc0: 7420 7375 7266 6163 650a 2020 2020 2020  t surface.      
+00002cd0: 2020 706f 696e 7473 2028 7363 616c 6573    points (scales
+00002ce0: 5b6e 785d 5b6e 795d 5b6e 7a5d 292e 0a20  [nx][ny][nz]).. 
+00002cf0: 2020 206e 6361 7620 3a20 696e 740a 2020     ncav : int.  
+00002d00: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00002d10: 6361 7669 7469 6573 2e0a 2020 2020 766f  cavities..    vo
+00002d20: 6c75 6d65 203a 2044 6963 745b 7374 722c  lume : Dict[str,
+00002d30: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
+00002d40: 4120 6469 6374 696f 6e61 7279 2077 6974  A dictionary wit
+00002d50: 6820 766f 6c75 6d65 206f 6620 6561 6368  h volume of each
+00002d60: 2064 6574 6563 7465 6420 6361 7669 7479   detected cavity
+00002d70: 2e0a 2020 2020 6172 6561 203a 2044 6963  ..    area : Dic
+00002d80: 745b 7374 722c 2066 6c6f 6174 5d0a 2020  t[str, float].  
+00002d90: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
+00002da0: 7279 2077 6974 6820 6172 6561 206f 6620  ry with area of 
+00002db0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
+00002dc0: 7669 7479 2e0a 2020 2020 6d61 785f 6465  vity..    max_de
+00002dd0: 7074 6820 3a20 4469 6374 5b73 7472 2c20  pth : Dict[str, 
+00002de0: 666c 6f61 745d 2c20 6f70 7469 6f6e 616c  float], optional
+00002df0: 0a20 2020 2020 2020 2041 2064 6963 7469  .        A dicti
+00002e00: 6f6e 6172 7920 7769 7468 206d 6178 696d  onary with maxim
+00002e10: 756d 2064 6570 7468 206f 6620 6561 6368  um depth of each
+00002e20: 2064 6574 6563 7465 6420 6361 7669 7479   detected cavity
+00002e30: 2e0a 2020 2020 6176 675f 6465 7074 6820  ..    avg_depth 
+00002e40: 3a20 4469 6374 5b73 7472 2c20 666c 6f61  : Dict[str, floa
+00002e50: 745d 2c20 6f70 7469 6f6e 616c 0a20 2020  t], optional.   
+00002e60: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
+00002e70: 7920 7769 7468 2061 7665 7261 6765 2064  y with average d
+00002e80: 6570 7468 206f 6620 6561 6368 2064 6574  epth of each det
+00002e90: 6563 7465 6420 6361 7669 7479 2e0a 2020  ected cavity..  
+00002ea0: 2020 6176 675f 6879 6472 6f70 6174 6879    avg_hydropathy
+00002eb0: 203a 2044 6963 745b 7374 722c 2066 6c6f   : Dict[str, flo
+00002ec0: 6174 5d2c 206f 7074 696f 6e61 6c0a 2020  at], optional.  
+00002ed0: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
+00002ee0: 7279 2077 6974 6820 6176 6572 6167 6520  ry with average 
+00002ef0: 6879 6472 6f70 6174 6879 2066 6f72 2065  hydropathy for e
+00002f00: 6163 6820 6465 7465 6374 6564 2063 6176  ach detected cav
+00002f10: 6974 7920 616e 640a 2020 2020 2020 2020  ity and.        
+00002f20: 7468 6520 7261 6e67 6520 6f66 2074 6865  the range of the
+00002f30: 2068 7964 726f 7068 6f62 6963 6974 7920   hydrophobicity 
+00002f40: 7363 616c 6520 286d 696e 2c20 6d61 7829  scale (min, max)
+00002f50: 2e0a 2020 2020 7265 7369 6475 6573 3a20  ..    residues: 
+00002f60: 4469 6374 5b73 7472 2c20 4c69 7374 5b4c  Dict[str, List[L
+00002f70: 6973 745b 7374 725d 5d5d 0a20 2020 2020  ist[str]]].     
+00002f80: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00002f90: 7769 7468 2061 206c 6973 7420 6f66 2069  with a list of i
+00002fa0: 6e74 6572 6661 6365 2072 6573 6964 7565  nterface residue
+00002fb0: 7320 666f 7220 6561 6368 2064 6574 6563  s for each detec
+00002fc0: 7465 640a 2020 2020 2020 2020 6361 7669  ted.        cavi
+00002fd0: 7479 2e0a 2020 2020 6672 6571 7565 6e63  ty..    frequenc
+00002fe0: 6965 7320 3a20 4469 6374 5b73 7472 2c20  ies : Dict[str, 
+00002ff0: 4469 6374 5b73 7472 2c20 4469 6374 5b73  Dict[str, Dict[s
+00003000: 7472 2c20 696e 745d 5d5d 2c20 6f70 7469  tr, int]]], opti
+00003010: 6f6e 616c 0a20 2020 2020 2020 2041 2064  onal.        A d
+00003020: 6963 7469 6f6e 6172 7920 7769 7468 2066  ictionary with f
+00003030: 7265 7175 656e 6369 6573 206f 6620 7265  requencies of re
+00003040: 7369 6475 6573 2061 6e64 2063 6c61 7373  sidues and class
+00003050: 2066 6f72 0a20 2020 2020 2020 2072 6573   for.        res
+00003060: 6964 7565 7320 6f66 2065 6163 6820 6465  idues of each de
+00003070: 7465 6374 6564 2063 6176 6974 792e 0a20  tected cavity.. 
+00003080: 2020 205f 7665 7274 6963 6573 203a 206e     _vertices : n
+00003090: 756d 7079 2e6e 6461 7272 6179 0a20 2020  umpy.ndarray.   
+000030a0: 2020 2020 2041 206e 756d 7079 2e6e 6461       A numpy.nda
+000030b0: 7272 6179 206f 7220 6120 6c69 7374 2077  rray or a list w
+000030c0: 6974 6820 7879 7a20 7665 7274 6963 6573  ith xyz vertices
+000030d0: 2063 6f6f 7264 696e 6174 6573 2028 6f72   coordinates (or
+000030e0: 6967 696e 2c0a 2020 2020 2020 2020 582d  igin,.        X-
+000030f0: 6178 6973 2c20 592d 6178 6973 2c20 5a2d  axis, Y-axis, Z-
+00003100: 6178 6973 292e 0a20 2020 205f 7374 6570  axis)..    _step
+00003110: 203a 2066 6c6f 6174 0a20 2020 2020 2020   : float.       
+00003120: 2047 7269 6420 7370 6163 696e 6720 2841   Grid spacing (A
+00003130: 292e 0a20 2020 205f 696e 7075 7420 3a20  )..    _input : 
+00003140: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
+00003150: 6962 2e50 6174 685d 2c20 6f70 7469 6f6e  ib.Path], option
+00003160: 616c 0a20 2020 2020 2020 2041 2070 6174  al.        A pat
+00003170: 6820 746f 2069 6e70 7574 2050 4442 206f  h to input PDB o
+00003180: 7220 5859 5a20 6669 6c65 2c20 6279 2064  r XYZ file, by d
+00003190: 6566 6175 6c74 204e 6f6e 652e 0a20 2020  efault None..   
+000031a0: 205f 6c69 6761 6e64 203a 2055 6e69 6f6e   _ligand : Union
+000031b0: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
+000031c0: 7468 5d2c 206f 7074 696f 6e61 6c0a 2020  th], optional.  
+000031d0: 2020 2020 2020 4120 7061 7468 2074 6f20        A path to 
+000031e0: 6c69 6761 6e64 2050 4442 206f 7220 5859  ligand PDB or XY
+000031f0: 5a20 6669 6c65 2c20 6279 2064 6566 6175  Z file, by defau
+00003200: 6c74 204e 6f6e 652e 0a20 2020 2022 2222  lt None..    """
+00003210: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00003220: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00003230: 2c0a 2020 2020 2020 2020 6361 7669 7469  ,.        caviti
+00003240: 6573 3a20 6e75 6d70 792e 6e64 6172 7261  es: numpy.ndarra
+00003250: 792c 0a20 2020 2020 2020 2073 7572 6661  y,.        surfa
+00003260: 6365 3a20 6e75 6d70 792e 6e64 6172 7261  ce: numpy.ndarra
+00003270: 792c 0a20 2020 2020 2020 2064 6570 7468  y,.        depth
+00003280: 733a 204f 7074 696f 6e61 6c5b 6e75 6d70  s: Optional[nump
+00003290: 792e 6e64 6172 7261 795d 2c0a 2020 2020  y.ndarray],.    
+000032a0: 2020 2020 7363 616c 6573 3a20 4f70 7469      scales: Opti
+000032b0: 6f6e 616c 5b6e 756d 7079 2e6e 6461 7272  onal[numpy.ndarr
+000032c0: 6179 5d2c 0a20 2020 2020 2020 2076 6f6c  ay],.        vol
+000032d0: 756d 653a 2044 6963 745b 7374 722c 2066  ume: Dict[str, f
+000032e0: 6c6f 6174 5d2c 0a20 2020 2020 2020 2061  loat],.        a
+000032f0: 7265 613a 2044 6963 745b 7374 722c 2066  rea: Dict[str, f
+00003300: 6c6f 6174 5d2c 0a20 2020 2020 2020 206d  loat],.        m
+00003310: 6178 5f64 6570 7468 3a20 4f70 7469 6f6e  ax_depth: Option
+00003320: 616c 5b44 6963 745b 7374 722c 2066 6c6f  al[Dict[str, flo
+00003330: 6174 5d5d 2c0a 2020 2020 2020 2020 6176  at]],.        av
+00003340: 675f 6465 7074 683a 204f 7074 696f 6e61  g_depth: Optiona
+00003350: 6c5b 4469 6374 5b73 7472 2c20 666c 6f61  l[Dict[str, floa
+00003360: 745d 5d2c 0a20 2020 2020 2020 2061 7667  t]],.        avg
+00003370: 5f68 7964 726f 7061 7468 793a 204f 7074  _hydropathy: Opt
+00003380: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00003390: 666c 6f61 745d 5d2c 0a20 2020 2020 2020  float]],.       
+000033a0: 2072 6573 6964 7565 733a 2044 6963 745b   residues: Dict[
+000033b0: 7374 722c 204c 6973 745b 4c69 7374 5b73  str, List[List[s
+000033c0: 7472 5d5d 5d2c 0a20 2020 2020 2020 2066  tr]]],.        f
+000033d0: 7265 7175 656e 6369 6573 3a20 4f70 7469  requencies: Opti
+000033e0: 6f6e 616c 5b44 6963 745b 7374 722c 2044  onal[Dict[str, D
+000033f0: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
+00003400: 722c 2069 6e74 5d5d 5d5d 2c0a 2020 2020  r, int]]]],.    
+00003410: 2020 2020 5f76 6572 7469 6365 733a 206e      _vertices: n
+00003420: 756d 7079 2e6e 6461 7272 6179 2c0a 2020  umpy.ndarray,.  
+00003430: 2020 2020 2020 5f73 7465 703a 2055 6e69        _step: Uni
+00003440: 6f6e 5b66 6c6f 6174 2c20 696e 745d 2c0a  on[float, int],.
+00003450: 2020 2020 2020 2020 5f69 6e70 7574 3a20          _input: 
+00003460: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+00003470: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
+00003480: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+00003490: 2020 205f 6c69 6761 6e64 3a20 4f70 7469     _ligand: Opti
+000034a0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+000034b0: 7061 7468 6c69 622e 5061 7468 5d5d 203d  pathlib.Path]] =
+000034c0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000034d0: 2020 2020 2020 7365 6c66 2e63 6176 6974        self.cavit
+000034e0: 6965 7320 3d20 6361 7669 7469 6573 0a20  ies = cavities. 
+000034f0: 2020 2020 2020 2073 656c 662e 7375 7266         self.surf
+00003500: 6163 6520 3d20 7375 7266 6163 650a 2020  ace = surface.  
+00003510: 2020 2020 2020 7365 6c66 2e64 6570 7468        self.depth
+00003520: 7320 3d20 6465 7074 6873 0a20 2020 2020  s = depths.     
+00003530: 2020 2073 656c 662e 7363 616c 6573 203d     self.scales =
+00003540: 2073 6361 6c65 730a 2020 2020 2020 2020   scales.        
+00003550: 7365 6c66 2e76 6f6c 756d 6520 3d20 766f  self.volume = vo
+00003560: 6c75 6d65 0a20 2020 2020 2020 2073 656c  lume.        sel
+00003570: 662e 6e63 6176 203d 2063 6176 6974 6965  f.ncav = cavitie
+00003580: 732e 6d61 7828 2920 2d20 310a 2020 2020  s.max() - 1.    
+00003590: 2020 2020 7365 6c66 2e61 7265 6120 3d20      self.area = 
+000035a0: 6172 6561 0a20 2020 2020 2020 2073 656c  area.        sel
+000035b0: 662e 6d61 785f 6465 7074 6820 3d20 6d61  f.max_depth = ma
+000035c0: 785f 6465 7074 680a 2020 2020 2020 2020  x_depth.        
+000035d0: 7365 6c66 2e61 7667 5f64 6570 7468 203d  self.avg_depth =
+000035e0: 2061 7667 5f64 6570 7468 0a20 2020 2020   avg_depth.     
+000035f0: 2020 2073 656c 662e 6176 675f 6879 6472     self.avg_hydr
+00003600: 6f70 6174 6879 203d 2061 7667 5f68 7964  opathy = avg_hyd
+00003610: 726f 7061 7468 790a 2020 2020 2020 2020  ropathy.        
+00003620: 7365 6c66 2e72 6573 6964 7565 7320 3d20  self.residues = 
+00003630: 7265 7369 6475 6573 0a20 2020 2020 2020  residues.       
+00003640: 2073 656c 662e 6672 6571 7565 6e63 6965   self.frequencie
+00003650: 7320 3d20 6672 6571 7565 6e63 6965 730a  s = frequencies.
+00003660: 2020 2020 2020 2020 7365 6c66 2e5f 7665          self._ve
+00003670: 7274 6963 6573 203d 205f 7665 7274 6963  rtices = _vertic
+00003680: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+00003690: 5f73 7465 7020 3d20 5f73 7465 700a 2020  _step = _step.  
+000036a0: 2020 2020 2020 7365 6c66 2e5f 696e 7075        self._inpu
+000036b0: 7420 3d20 6f73 2e70 6174 682e 6162 7370  t = os.path.absp
+000036c0: 6174 6828 5f69 6e70 7574 290a 2020 2020  ath(_input).    
+000036d0: 2020 2020 7365 6c66 2e5f 6c69 6761 6e64      self._ligand
+000036e0: 203d 206f 732e 7061 7468 2e61 6273 7061   = os.path.abspa
+000036f0: 7468 285f 6c69 6761 6e64 2920 6966 205f  th(_ligand) if _
+00003700: 6c69 6761 6e64 2065 6c73 6520 4e6f 6e65  ligand else None
+00003710: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+00003720: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00003730: 2020 7265 7475 726e 2022 3c70 794b 5646    return "<pyKVF
+00003740: 696e 6465 7252 6573 756c 7473 206f 626a  inderResults obj
+00003750: 6563 743e 220a 0a20 2020 2064 6566 2065  ect>"..    def e
+00003760: 7870 6f72 7428 0a20 2020 2020 2020 2073  xport(.        s
+00003770: 656c 662c 0a20 2020 2020 2020 206f 7574  elf,.        out
+00003780: 7075 743a 2055 6e69 6f6e 5b73 7472 2c20  put: Union[str, 
+00003790: 7061 7468 6c69 622e 5061 7468 5d20 3d20  pathlib.Path] = 
+000037a0: 2263 6176 6974 792e 7064 6222 2c0a 2020  "cavity.pdb",.  
+000037b0: 2020 2020 2020 6e74 6872 6561 6473 3a20        nthreads: 
+000037c0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000037d0: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 204e  None,.    ) -> N
+000037e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000037f0: 4578 706f 7274 7320 6361 7669 7469 7920  Exports cavitiy 
+00003800: 2848 2920 616e 6420 7375 7266 6163 6520  (H) and surface 
+00003810: 2848 4129 2070 6f69 6e74 7320 746f 2050  (HA) points to P
+00003820: 4442 2d66 6f72 6d61 7474 6564 2066 696c  DB-formatted fil
+00003830: 650a 2020 2020 2020 2020 7769 7468 2061  e.        with a
+00003840: 2076 6172 6961 626c 6520 2842 3b20 6f70   variable (B; op
+00003850: 7469 6f6e 616c 2920 696e 2042 2d66 6163  tional) in B-fac
+00003860: 746f 7220 636f 6c75 6d6e 2c20 616e 6420  tor column, and 
+00003870: 6879 6472 6f70 6174 6879 2074 6f0a 2020  hydropathy to.  
+00003880: 2020 2020 2020 5044 422d 666f 726d 6174        PDB-format
+00003890: 7465 6420 6669 6c65 2069 6e20 422d 6661  ted file in B-fa
+000038a0: 6374 6f72 2063 6f6c 756d 6e20 6174 2073  ctor column at s
+000038b0: 7572 6661 6365 2070 6f69 6e74 7320 2848  urface points (H
+000038c0: 4129 2e0a 0a20 2020 2020 2020 2050 6172  A)...        Par
+000038d0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+000038e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+000038f0: 2020 206f 7574 7075 7420 3a20 556e 696f     output : Unio
+00003900: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
+00003910: 6174 685d 292c 206f 7074 696f 6e61 6c0a  ath]), optional.
+00003920: 2020 2020 2020 2020 2020 2020 4120 7061              A pa
+00003930: 7468 2074 6f20 5044 4220 6669 6c65 2066  th to PDB file f
+00003940: 6f72 2077 7269 7469 6e67 2063 6176 6974  or writing cavit
+00003950: 6965 732c 2062 7920 6465 6661 756c 7420  ies, by default 
+00003960: 6063 6176 6974 792e 7064 6260 2e0a 2020  `cavity.pdb`..  
+00003970: 2020 2020 2020 6e74 6872 6561 6473 203a        nthreads :
+00003980: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
+00003990: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+000039a0: 7220 6f66 2074 6872 6561 6473 2c20 6279  r of threads, by
+000039b0: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
+000039c0: 6620 4e6f 6e65 2c20 7468 6520 6e75 6d62  f None, the numb
+000039d0: 6572 206f 6620 7468 7265 6164 7320 6973  er of threads is
+000039e0: 0a20 2020 2020 2020 2020 2020 2060 6f73  .            `os
+000039f0: 2e63 7075 5f63 6f75 6e74 2829 202d 2031  .cpu_count() - 1
+00003a00: 602e 0a0a 2020 2020 2020 2020 4e6f 7465  `...        Note
+00003a10: 0a20 2020 2020 2020 202d 2d2d 2d0a 2020  .        ----.  
+00003a20: 2020 2020 2020 5468 6520 6361 7669 7479        The cavity
+00003a30: 206e 6f6d 656e 636c 6174 7572 6520 6973   nomenclature is
+00003a40: 2062 6173 6564 206f 6e20 7468 6520 696e   based on the in
+00003a50: 7465 6765 7220 6c61 6265 6c2e 2054 6865  teger label. The
+00003a60: 2063 6176 6974 790a 2020 2020 2020 2020   cavity.        
+00003a70: 6d61 726b 6564 2077 6974 6820 322c 2074  marked with 2, t
+00003a80: 6865 2066 6972 7374 2069 6e74 6567 6572  he first integer
+00003a90: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00003aa0: 6f20 6120 6361 7669 7479 2c20 6973 204b  o a cavity, is K
+00003ab0: 4141 2c0a 2020 2020 2020 2020 7468 6520  AA,.        the 
+00003ac0: 6361 7669 7479 206d 6172 6b65 6420 7769  cavity marked wi
+00003ad0: 7468 2033 2069 7320 4b41 422c 2074 6865  th 3 is KAB, the
+00003ae0: 2063 6176 6974 7920 6d61 726b 6564 2077   cavity marked w
+00003af0: 6974 6820 3420 6973 204b 4143 0a20 2020  ith 4 is KAC.   
+00003b00: 2020 2020 2061 6e64 2073 6f20 6f6e 2e0a       and so on..
+00003b10: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+00003b20: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00003b30: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
+00003b40: 6d20 7079 4b56 4669 6e64 6572 2069 6d70  m pyKVFinder imp
+00003b50: 6f72 7420 7079 4b56 4669 6e64 6572 0a20  ort pyKVFinder. 
+00003b60: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00003b70: 7420 6f73 0a20 2020 2020 2020 203e 3e3e  t os.        >>>
+00003b80: 2070 6462 203d 206f 732e 7061 7468 2e6a   pdb = os.path.j
+00003b90: 6f69 6e28 6f73 2e70 6174 682e 6469 726e  oin(os.path.dirn
+00003ba0: 616d 6528 7079 4b56 4669 6e64 6572 2e5f  ame(pyKVFinder._
+00003bb0: 5f66 696c 655f 5f29 2c20 2764 6174 6127  _file__), 'data'
+00003bc0: 2c20 2774 6573 7473 272c 2027 3146 4d4f  , 'tests', '1FMO
+00003bd0: 2e70 6462 2729 0a20 2020 2020 2020 203e  .pdb').        >
+00003be0: 3e3e 2072 6573 756c 7473 203d 2070 794b  >> results = pyK
+00003bf0: 5646 696e 6465 7228 7064 6229 0a20 2020  VFinder(pdb).   
+00003c00: 2020 2020 203e 3e3e 2072 6573 756c 7473       >>> results
+00003c10: 2e65 7870 6f72 7428 290a 2020 2020 2020  .export().      
+00003c20: 2020 2222 220a 2020 2020 2020 2020 6578    """.        ex
+00003c30: 706f 7274 280a 2020 2020 2020 2020 2020  port(.          
+00003c40: 2020 6f75 7470 7574 2c0a 2020 2020 2020    output,.      
+00003c50: 2020 2020 2020 7365 6c66 2e63 6176 6974        self.cavit
+00003c60: 6965 732c 0a20 2020 2020 2020 2020 2020  ies,.           
+00003c70: 2073 656c 662e 7375 7266 6163 652c 0a20   self.surface,. 
+00003c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003c90: 5f76 6572 7469 6365 732c 0a20 2020 2020  _vertices,.     
+00003ca0: 2020 2020 2020 2073 656c 662e 5f73 7465         self._ste
+00003cb0: 702c 0a20 2020 2020 2020 2020 2020 2073  p,.            s
+00003cc0: 656c 662e 6465 7074 6873 2c0a 2020 2020  elf.depths,.    
+00003cd0: 2020 2020 2020 2020 7365 6c66 2e73 6361          self.sca
+00003ce0: 6c65 732c 0a20 2020 2020 2020 2020 2020  les,.           
+00003cf0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00003d00: 2020 206e 7468 7265 6164 732c 0a20 2020     nthreads,.   
+00003d10: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00003d20: 7772 6974 6528 0a20 2020 2020 2020 2073  write(.        s
+00003d30: 656c 662c 0a20 2020 2020 2020 2066 6e3a  elf,.        fn:
+00003d40: 2055 6e69 6f6e 5b73 7472 2c20 7061 7468   Union[str, path
+00003d50: 6c69 622e 5061 7468 5d20 3d20 2272 6573  lib.Path] = "res
+00003d60: 756c 7473 2e74 6f6d 6c22 2c0a 2020 2020  ults.toml",.    
+00003d70: 2020 2020 6f75 7470 7574 3a20 4f70 7469      output: Opti
+00003d80: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+00003d90: 7061 7468 6c69 622e 5061 7468 5d5d 203d  pathlib.Path]] =
+00003da0: 204e 6f6e 650a 2020 2020 2920 2d3e 204e   None.    ) -> N
+00003db0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00003dc0: 0a20 2020 2020 2020 2057 7269 7465 7320  .        Writes 
+00003dd0: 6669 6c65 2070 6174 6873 2061 6e64 2063  file paths and c
+00003de0: 6176 6974 7920 6368 6172 6163 7465 7269  avity characteri
+00003df0: 7a61 7469 6f6e 2074 6f20 544f 4d4c 2d66  zation to TOML-f
+00003e00: 6f72 6d61 7474 6564 2066 696c 650a 0a20  ormatted file.. 
+00003e10: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00003e20: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00003e30: 2d2d 2d2d 0a20 2020 2020 2020 2066 6e20  ----.        fn 
+00003e40: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
+00003e50: 686c 6962 2e50 6174 685d 2c20 6f70 7469  hlib.Path], opti
+00003e60: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00003e70: 2041 2070 6174 6820 746f 2054 4f4d 4c2d   A path to TOML-
+00003e80: 666f 726d 6174 7465 6420 6669 6c65 2066  formatted file f
+00003e90: 6f72 2077 7269 7469 6e67 2066 696c 6520  or writing file 
+00003ea0: 7061 7468 7320 616e 6420 6361 7669 7479  paths and cavity
+00003eb0: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+00003ec0: 7261 6374 6572 697a 6174 696f 6e20 2876  racterization (v
+00003ed0: 6f6c 756d 652c 2061 7265 612c 2064 6570  olume, area, dep
+00003ee0: 7468 2061 6e64 2069 6e74 6572 6661 6365  th and interface
+00003ef0: 2072 6573 6964 7565 7329 0a20 2020 2020   residues).     
+00003f00: 2020 2020 2020 2070 6572 2063 6176 6974         per cavit
+00003f10: 7920 6465 7465 6374 6564 2c20 6279 2064  y detected, by d
+00003f20: 6566 6175 6c74 2060 7265 7375 6c74 732e  efault `results.
+00003f30: 746f 6d6c 602e 0a20 2020 2020 2020 206f  toml`..        o
+00003f40: 7574 7075 7420 3a20 556e 696f 6e5b 7374  utput : Union[st
+00003f50: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+00003f60: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00003f70: 2020 2020 2020 2041 2070 6174 6820 746f         A path to
+00003f80: 2061 2063 6176 6974 7920 5044 4220 6669   a cavity PDB fi
+00003f90: 6c65 2c20 6279 2064 6566 6175 6c74 204e  le, by default N
+00003fa0: 6f6e 652e 0a0a 2020 2020 2020 2020 4e6f  one...        No
+00003fb0: 7465 0a20 2020 2020 2020 202d 2d2d 2d0a  te.        ----.
+00003fc0: 2020 2020 2020 2020 5468 6520 6361 7669          The cavi
+00003fd0: 7479 206e 6f6d 656e 636c 6174 7572 6520  ty nomenclature 
+00003fe0: 6973 2062 6173 6564 206f 6e20 7468 6520  is based on the 
+00003ff0: 696e 7465 6765 7220 6c61 6265 6c2e 2054  integer label. T
+00004000: 6865 2063 6176 6974 790a 2020 2020 2020  he cavity.      
+00004010: 2020 6d61 726b 6564 2077 6974 6820 322c    marked with 2,
+00004020: 2074 6865 2066 6972 7374 2069 6e74 6567   the first integ
+00004030: 6572 2063 6f72 7265 7370 6f6e 6469 6e67  er corresponding
+00004040: 2074 6f20 6120 6361 7669 7479 2c20 6973   to a cavity, is
+00004050: 204b 4141 2c0a 2020 2020 2020 2020 7468   KAA,.        th
+00004060: 6520 6361 7669 7479 206d 6172 6b65 6420  e cavity marked 
+00004070: 7769 7468 2033 2069 7320 4b41 422c 2074  with 3 is KAB, t
+00004080: 6865 2063 6176 6974 7920 6d61 726b 6564  he cavity marked
+00004090: 2077 6974 6820 3420 6973 204b 4143 0a20   with 4 is KAC. 
+000040a0: 2020 2020 2020 2061 6e64 2073 6f20 6f6e         and so on
+000040b0: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+000040c0: 6c65 0a20 2020 2020 2020 202d 2d2d 2d2d  le.        -----
+000040d0: 2d2d 0a20 2020 2020 2020 203e 3e3e 2066  --.        >>> f
+000040e0: 726f 6d20 7079 4b56 4669 6e64 6572 2069  rom pyKVFinder i
+000040f0: 6d70 6f72 7420 7079 4b56 4669 6e64 6572  mport pyKVFinder
+00004100: 0a20 2020 2020 2020 203e 3e3e 2069 6d70  .        >>> imp
+00004110: 6f72 7420 6f73 0a20 2020 2020 2020 203e  ort os.        >
+00004120: 3e3e 2070 6462 203d 206f 732e 7061 7468  >> pdb = os.path
+00004130: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
+00004140: 726e 616d 6528 7079 4b56 4669 6e64 6572  rname(pyKVFinder
+00004150: 2e5f 5f66 696c 655f 5f29 2c20 2764 6174  .__file__), 'dat
+00004160: 6127 2c20 2774 6573 7473 272c 2027 3146  a', 'tests', '1F
+00004170: 4d4f 2e70 6462 2729 0a20 2020 2020 2020  MO.pdb').       
+00004180: 203e 3e3e 2072 6573 756c 7473 203d 2070   >>> results = p
+00004190: 794b 5646 696e 6465 7228 7064 6229 0a20  yKVFinder(pdb). 
+000041a0: 2020 2020 2020 203e 3e3e 2072 6573 756c         >>> resul
+000041b0: 7473 2e77 7269 7465 2829 0a20 2020 2020  ts.write().     
+000041c0: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
+000041d0: 7269 7465 5f72 6573 756c 7473 280a 2020  rite_results(.  
+000041e0: 2020 2020 2020 2020 2020 666e 2c0a 2020            fn,.  
+000041f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00004200: 696e 7075 742c 0a20 2020 2020 2020 2020  input,.         
+00004210: 2020 2073 656c 662e 5f6c 6967 616e 642c     self._ligand,
+00004220: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00004230: 7075 742c 0a20 2020 2020 2020 2020 2020  put,.           
+00004240: 2073 656c 662e 766f 6c75 6d65 2c0a 2020   self.volume,.  
+00004250: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00004260: 7265 612c 0a20 2020 2020 2020 2020 2020  rea,.           
+00004270: 2073 656c 662e 6d61 785f 6465 7074 682c   self.max_depth,
+00004280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004290: 662e 6176 675f 6465 7074 682c 0a20 2020  f.avg_depth,.   
+000042a0: 2020 2020 2020 2020 2073 656c 662e 6176           self.av
+000042b0: 675f 6879 6472 6f70 6174 6879 2c0a 2020  g_hydropathy,.  
+000042c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000042d0: 6573 6964 7565 732c 0a20 2020 2020 2020  esidues,.       
+000042e0: 2020 2020 2073 656c 662e 6672 6571 7565       self.freque
+000042f0: 6e63 6965 732c 0a20 2020 2020 2020 2020  ncies,.         
+00004300: 2020 2073 656c 662e 5f73 7465 702c 0a20     self._step,. 
+00004310: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00004320: 6620 706c 6f74 5f66 7265 7175 656e 6369  f plot_frequenci
+00004330: 6573 2873 656c 662c 2070 6466 3a20 556e  es(self, pdf: Un
+00004340: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
+00004350: 2e50 6174 685d 203d 2022 6261 7270 6c6f  .Path] = "barplo
+00004360: 7473 2e70 6466 2229 3a0a 2020 2020 2020  ts.pdf"):.      
+00004370: 2020 2222 2250 6c6f 7420 6261 7220 6368    """Plot bar ch
+00004380: 6172 7473 206f 6620 6672 6571 7565 6e63  arts of frequenc
+00004390: 6965 7320 2872 6573 6964 7565 7320 616e  ies (residues an
+000043a0: 6420 636c 6173 7365 7320 6f66 2072 6573  d classes of res
+000043b0: 6964 7565 7329 2069 6e0a 2020 2020 2020  idues) in.      
+000043c0: 2020 6120 5044 4620 6669 6c65 2e0a 0a20    a PDF file... 
+000043d0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000043e0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000043f0: 2d2d 2d2d 0a20 2020 2020 2020 2070 6466  ----.        pdf
+00004400: 203a 2055 6e69 6f6e 5b73 7472 2c20 7061   : Union[str, pa
+00004410: 7468 6c69 622e 5061 7468 5d2c 206f 7074  thlib.Path], opt
+00004420: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00004430: 2020 4120 7061 7468 2074 6f20 6120 5044    A path to a PD
+00004440: 4620 6669 6c65 2c20 6279 2064 6566 6175  F file, by defau
+00004450: 6c74 2060 6261 7270 6c6f 7473 2e70 6466  lt `barplots.pdf
+00004460: 602e 0a0a 2020 2020 2020 2020 4e6f 7465  `...        Note
+00004470: 0a20 2020 2020 2020 202d 2d2d 2d0a 2020  .        ----.  
+00004480: 2020 2020 2020 5468 6520 6361 7669 7479        The cavity
+00004490: 206e 6f6d 656e 636c 6174 7572 6520 6973   nomenclature is
+000044a0: 2062 6173 6564 206f 6e20 7468 6520 696e   based on the in
+000044b0: 7465 6765 7220 6c61 6265 6c2e 2054 6865  teger label. The
+000044c0: 2063 6176 6974 790a 2020 2020 2020 2020   cavity.        
+000044d0: 6d61 726b 6564 2077 6974 6820 322c 2074  marked with 2, t
+000044e0: 6865 2066 6972 7374 2069 6e74 6567 6572  he first integer
+000044f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00004500: 6f20 6120 6361 7669 7479 2c20 6973 204b  o a cavity, is K
+00004510: 4141 2c0a 2020 2020 2020 2020 7468 6520  AA,.        the 
+00004520: 6361 7669 7479 206d 6172 6b65 6420 7769  cavity marked wi
+00004530: 7468 2033 2069 7320 4b41 422c 2074 6865  th 3 is KAB, the
+00004540: 2063 6176 6974 7920 6d61 726b 6564 2077   cavity marked w
+00004550: 6974 6820 3420 6973 204b 4143 0a20 2020  ith 4 is KAC.   
+00004560: 2020 2020 2061 6e64 2073 6f20 6f6e 2e0a       and so on..
+00004570: 0a20 2020 2020 2020 204e 6f74 650a 2020  .        Note.  
+00004580: 2020 2020 2020 2d2d 2d2d 0a20 2020 2020        ----.     
+00004590: 2020 2054 6865 2063 6c61 7373 6573 206f     The classes o
+000045a0: 6620 7265 7369 6475 6573 2061 7265 3a0a  f residues are:.
+000045b0: 0a20 2020 2020 2020 202a 2041 6c69 7068  .        * Aliph
+000045c0: 6174 6963 2061 706f 6c61 7220 2852 3129  atic apolar (R1)
+000045d0: 3a20 416c 616e 696e 652c 2047 6c79 6369  : Alanine, Glyci
+000045e0: 6e65 2c20 4973 6f6c 6575 6369 6e65 2c20  ne, Isoleucine, 
+000045f0: 4c65 7563 696e 652c 204d 6574 6869 6f6e  Leucine, Methion
+00004600: 696e 652c 2056 616c 696e 652e 0a0a 2020  ine, Valine...  
+00004610: 2020 2020 2020 2a20 4172 6f6d 6174 6963        * Aromatic
+00004620: 2028 5232 293a 2050 6865 6e79 6c61 6c61   (R2): Phenylala
+00004630: 6e69 6e65 2c20 5472 7970 746f 7068 616e  nine, Tryptophan
+00004640: 2c20 5479 726f 7369 6e65 2e0a 0a20 2020  , Tyrosine...   
+00004650: 2020 2020 202a 2050 6f6c 6172 2055 6e63       * Polar Unc
+00004660: 6861 7267 6564 2028 5233 293a 2041 7370  harged (R3): Asp
+00004670: 6172 6167 696e 652c 2043 7973 7465 696e  aragine, Cystein
+00004680: 652c 2047 6c75 7461 6d69 6e65 2c20 5072  e, Glutamine, Pr
+00004690: 6f6c 696e 652c 2053 6572 696e 652c 2054  oline, Serine, T
+000046a0: 6872 656f 6e69 6e65 2e0a 0a20 2020 2020  hreonine...     
+000046b0: 2020 202a 204e 6567 6174 6976 656c 7920     * Negatively 
+000046c0: 6368 6172 6765 6420 2852 3429 3a20 4173  charged (R4): As
+000046d0: 7061 7274 6174 652c 2047 6c75 7461 6d61  partate, Glutama
+000046e0: 7465 2e0a 0a20 2020 2020 2020 202a 2050  te...        * P
+000046f0: 6f73 6974 6976 656c 7920 6368 6172 6765  ositively charge
+00004700: 6420 2852 3529 3a20 4172 6769 6e69 6e65  d (R5): Arginine
+00004710: 2c20 4869 7374 6964 696e 652c 204c 7973  , Histidine, Lys
+00004720: 696e 652e 0a0a 2020 2020 2020 2020 2a20  ine...        * 
+00004730: 4e6f 6e2d 7374 616e 6461 7264 2028 5258  Non-standard (RX
+00004740: 293a 204e 6f6e 2d73 7461 6e64 6172 6420  ): Non-standard 
+00004750: 7265 7369 6475 6573 0a0a 2020 2020 2020  residues..      
+00004760: 2020 4578 616d 706c 650a 2020 2020 2020    Example.      
+00004770: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00004780: 2020 3e3e 3e20 6672 6f6d 2070 794b 5646    >>> from pyKVF
+00004790: 696e 6465 7220 696d 706f 7274 2070 794b  inder import pyK
+000047a0: 5646 696e 6465 720a 2020 2020 2020 2020  VFinder.        
+000047b0: 3e3e 3e20 696d 706f 7274 206f 730a 2020  >>> import os.  
+000047c0: 2020 2020 2020 3e3e 3e20 7064 6220 3d20        >>> pdb = 
+000047d0: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
+000047e0: 7061 7468 2e64 6972 6e61 6d65 2870 794b  path.dirname(pyK
+000047f0: 5646 696e 6465 722e 5f5f 6669 6c65 5f5f  VFinder.__file__
+00004800: 292c 2027 6461 7461 272c 2027 7465 7374  ), 'data', 'test
+00004810: 7327 2c20 2731 464d 4f2e 7064 6227 290a  s', '1FMO.pdb').
+00004820: 2020 2020 2020 2020 3e3e 3e20 7265 7375          >>> resu
+00004830: 6c74 7320 3d20 7079 4b56 4669 6e64 6572  lts = pyKVFinder
+00004840: 2870 6462 290a 2020 2020 2020 2020 3e3e  (pdb).        >>
+00004850: 3e20 7265 7375 6c74 732e 706c 6f74 5f66  > results.plot_f
+00004860: 7265 7175 656e 6369 6573 2829 0a20 2020  requencies().   
+00004870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004880: 2070 6c6f 745f 6672 6571 7565 6e63 6965   plot_frequencie
+00004890: 7328 7365 6c66 2e66 7265 7175 656e 6369  s(self.frequenci
+000048a0: 6573 2c20 7064 6629 0a0a 2020 2020 6465  es, pdf)..    de
+000048b0: 6620 6578 706f 7274 5f61 6c6c 280a 2020  f export_all(.  
+000048c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000048d0: 2020 2020 666e 3a20 556e 696f 6e5b 7374      fn: Union[st
+000048e0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+000048f0: 203d 2022 7265 7375 6c74 732e 746f 6d6c   = "results.toml
+00004900: 222c 0a20 2020 2020 2020 206f 7574 7075  ",.        outpu
+00004910: 743a 2055 6e69 6f6e 5b73 7472 2c20 7061  t: Union[str, pa
+00004920: 7468 6c69 622e 5061 7468 5d20 3d20 2263  thlib.Path] = "c
+00004930: 6176 6974 792e 7064 6222 2c0a 2020 2020  avity.pdb",.    
+00004940: 2020 2020 696e 636c 7564 655f 6672 6571      include_freq
+00004950: 7565 6e63 6965 735f 7064 663a 2062 6f6f  uencies_pdf: boo
+00004960: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00004970: 2020 2070 6466 3a20 556e 696f 6e5b 7374     pdf: Union[st
+00004980: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+00004990: 203d 2022 6261 7270 6c6f 7473 2e70 6466   = "barplots.pdf
+000049a0: 222c 0a20 2020 2020 2020 206e 7468 7265  ",.        nthre
+000049b0: 6164 733a 204f 7074 696f 6e61 6c5b 696e  ads: Optional[in
+000049c0: 745d 203d 204e 6f6e 652c 0a20 2020 2029  t] = None,.    )
+000049d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000049e0: 2020 2222 2245 7870 6f72 7473 2063 6176    """Exports cav
+000049f0: 6974 6965 7320 616e 6420 6368 6172 6163  ities and charac
+00004a00: 7465 7269 7a61 7469 6f6e 2074 6f20 5044  terization to PD
+00004a10: 422d 666f 726d 6174 7465 6420 6669 6c65  B-formatted file
+00004a20: 732c 0a20 2020 2020 2020 2077 7269 7465  s,.        write
+00004a30: 7320 6669 6c65 2070 6174 6873 2061 6e64  s file paths and
+00004a40: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
+00004a50: 6e20 746f 2061 2054 4f4d 4c2d 666f 726d  n to a TOML-form
+00004a60: 6174 7465 6420 6669 6c65 2c20 616e 640a  atted file, and.
+00004a70: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00004a80: 6c79 2070 6c6f 7420 6261 7220 6368 6172  ly plot bar char
+00004a90: 7473 206f 6620 6672 6571 7565 6e63 6965  ts of frequencie
+00004aa0: 7320 2872 6573 6964 7565 7320 616e 6420  s (residues and 
+00004ab0: 636c 6173 7365 7320 6f66 0a20 2020 2020  classes of.     
+00004ac0: 2020 2072 6573 6964 7565 7329 2069 6e20     residues) in 
+00004ad0: 6120 5044 4620 6669 6c65 2e0a 0a20 2020  a PDF file...   
+00004ae0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00004af0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00004b00: 2d2d 0a20 2020 2020 2020 2066 6e20 3a20  --.        fn : 
+00004b10: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
+00004b20: 6962 2e50 6174 685d 2c20 6f70 7469 6f6e  ib.Path], option
+00004b30: 616c 0a20 2020 2020 2020 2020 2020 2041  al.            A
+00004b40: 2070 6174 6820 746f 2054 4f4d 4c2d 666f   path to TOML-fo
+00004b50: 726d 6174 7465 6420 6669 6c65 2066 6f72  rmatted file for
+00004b60: 2077 7269 7469 6e67 2066 696c 6520 7061   writing file pa
+00004b70: 7468 7320 616e 640a 2020 2020 2020 2020  ths and.        
+00004b80: 2020 2020 6361 7669 7479 2063 6861 7261      cavity chara
+00004b90: 6374 6572 697a 6174 696f 6e20 2876 6f6c  cterization (vol
+00004ba0: 756d 652c 2061 7265 6120 616e 6420 696e  ume, area and in
+00004bb0: 7465 7266 6163 6520 7265 7369 6475 6573  terface residues
+00004bc0: 290a 2020 2020 2020 2020 2020 2020 7065  ).            pe
+00004bd0: 7220 6361 7669 7479 2064 6574 6563 7465  r cavity detecte
+00004be0: 642c 2062 7920 6465 6661 756c 7420 6072  d, by default `r
+00004bf0: 6573 756c 7473 2e74 6f6d 6c60 2e0a 2020  esults.toml`..  
+00004c00: 2020 2020 2020 6f75 7470 7574 203a 2055        output : U
+00004c10: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
+00004c20: 622e 5061 7468 5d2c 206f 7074 696f 6e61  b.Path], optiona
+00004c30: 6c0a 2020 2020 2020 2020 2020 2020 4120  l.            A 
+00004c40: 7061 7468 2074 6f20 5044 4220 6669 6c65  path to PDB file
+00004c50: 2066 6f72 2077 7269 7469 6e67 2063 6176   for writing cav
+00004c60: 6974 6965 732c 2062 7920 6465 6661 756c  ities, by defaul
+00004c70: 7420 6063 6176 6974 792e 7064 6260 2e0a  t `cavity.pdb`..
+00004c80: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+00004c90: 6672 6571 7565 6e63 6965 735f 7064 6620  frequencies_pdf 
+00004ca0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00004cb0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00004cc0: 7468 6572 2074 6f20 706c 6f74 2066 7265  ther to plot fre
+00004cd0: 7175 656e 6369 6573 2028 7265 7369 6475  quencies (residu
+00004ce0: 6573 2061 6e64 2063 6c61 7373 6573 206f  es and classes o
+00004cf0: 6620 7265 7369 6475 6573 290a 2020 2020  f residues).    
+00004d00: 2020 2020 2020 2020 746f 2050 4446 2066          to PDF f
+00004d10: 696c 652c 2062 7920 6465 6661 756c 7420  ile, by default 
+00004d20: 4661 6c73 652e 0a20 2020 2020 2020 2070  False..        p
+00004d30: 6466 203a 2055 6e69 6f6e 5b73 7472 2c20  df : Union[str, 
+00004d40: 7061 7468 6c69 622e 5061 7468 5d2c 206f  pathlib.Path], o
+00004d50: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00004d60: 2020 2020 4120 7061 7468 2074 6f20 6120      A path to a 
+00004d70: 5044 4620 6669 6c65 2c20 6279 2064 6566  PDF file, by def
+00004d80: 6175 6c74 2060 6261 7270 6c6f 7473 2e70  ault `barplots.p
+00004d90: 6466 602e 0a20 2020 2020 2020 206e 7468  df`..        nth
+00004da0: 7265 6164 7320 3a20 696e 742c 206f 7074  reads : int, opt
+00004db0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00004dc0: 2020 4e75 6d62 6572 206f 6620 7468 7265    Number of thre
+00004dd0: 6164 732c 2062 7920 6465 6661 756c 7420  ads, by default 
+00004de0: 4e6f 6e65 2e20 4966 204e 6f6e 652c 2074  None. If None, t
+00004df0: 6865 206e 756d 6265 7220 6f66 2074 6872  he number of thr
+00004e00: 6561 6473 2069 730a 2020 2020 2020 2020  eads is.        
+00004e10: 2020 2020 606f 732e 6370 755f 636f 756e      `os.cpu_coun
+00004e20: 7428 2920 2d20 3160 2e0a 0a20 2020 2020  t() - 1`...     
+00004e30: 2020 204e 6f74 650a 2020 2020 2020 2020     Note.        
+00004e40: 2d2d 2d2d 0a20 2020 2020 2020 2054 6865  ----.        The
+00004e50: 2063 6176 6974 7920 6e6f 6d65 6e63 6c61   cavity nomencla
+00004e60: 7475 7265 2069 7320 6261 7365 6420 6f6e  ture is based on
+00004e70: 2074 6865 2069 6e74 6567 6572 206c 6162   the integer lab
+00004e80: 656c 2e20 5468 6520 6361 7669 7479 0a20  el. The cavity. 
+00004e90: 2020 2020 2020 206d 6172 6b65 6420 7769         marked wi
+00004ea0: 7468 2032 2c20 7468 6520 6669 7273 7420  th 2, the first 
+00004eb0: 696e 7465 6765 7220 636f 7272 6573 706f  integer correspo
+00004ec0: 6e64 696e 6720 746f 2061 2063 6176 6974  nding to a cavit
+00004ed0: 792c 2069 7320 4b41 412c 0a20 2020 2020  y, is KAA,.     
+00004ee0: 2020 2074 6865 2063 6176 6974 7920 6d61     the cavity ma
+00004ef0: 726b 6564 2077 6974 6820 3320 6973 204b  rked with 3 is K
+00004f00: 4142 2c20 7468 6520 6361 7669 7479 206d  AB, the cavity m
+00004f10: 6172 6b65 6420 7769 7468 2034 2069 7320  arked with 4 is 
+00004f20: 4b41 430a 2020 2020 2020 2020 616e 6420  KAC.        and 
+00004f30: 736f 206f 6e2e 0a0a 2020 2020 2020 2020  so on...        
+00004f40: 4e6f 7465 0a20 2020 2020 2020 202d 2d2d  Note.        ---
+00004f50: 2d0a 2020 2020 2020 2020 5468 6520 636c  -.        The cl
+00004f60: 6173 7365 7320 6f66 2072 6573 6964 7565  asses of residue
+00004f70: 7320 6172 653a 0a0a 2020 2020 2020 2020  s are:..        
+00004f80: 2a20 416c 6970 6861 7469 6320 6170 6f6c  * Aliphatic apol
+00004f90: 6172 2028 5231 293a 2041 6c61 6e69 6e65  ar (R1): Alanine
+00004fa0: 2c20 476c 7963 696e 652c 2049 736f 6c65  , Glycine, Isole
+00004fb0: 7563 696e 652c 204c 6575 6369 6e65 2c20  ucine, Leucine, 
+00004fc0: 4d65 7468 696f 6e69 6e65 2c20 5661 6c69  Methionine, Vali
+00004fd0: 6e65 2e0a 0a20 2020 2020 2020 202a 2041  ne...        * A
+00004fe0: 726f 6d61 7469 6320 2852 3229 3a20 5068  romatic (R2): Ph
+00004ff0: 656e 796c 616c 616e 696e 652c 2054 7279  enylalanine, Try
+00005000: 7074 6f70 6861 6e2c 2054 7972 6f73 696e  ptophan, Tyrosin
+00005010: 652e 0a0a 2020 2020 2020 2020 2a20 506f  e...        * Po
+00005020: 6c61 7220 556e 6368 6172 6765 6420 2852  lar Uncharged (R
+00005030: 3329 3a20 4173 7061 7261 6769 6e65 2c20  3): Asparagine, 
+00005040: 4379 7374 6569 6e65 2c20 476c 7574 616d  Cysteine, Glutam
+00005050: 696e 652c 2050 726f 6c69 6e65 2c20 5365  ine, Proline, Se
+00005060: 7269 6e65 2c20 5468 7265 6f6e 696e 652e  rine, Threonine.
+00005070: 0a0a 2020 2020 2020 2020 2a20 4e65 6761  ..        * Nega
+00005080: 7469 7665 6c79 2063 6861 7267 6564 2028  tively charged (
+00005090: 5234 293a 2041 7370 6172 7461 7465 2c20  R4): Aspartate, 
+000050a0: 476c 7574 616d 6174 652e 0a0a 2020 2020  Glutamate...    
+000050b0: 2020 2020 2a20 506f 7369 7469 7665 6c79      * Positively
+000050c0: 2063 6861 7267 6564 2028 5235 293a 2041   charged (R5): A
+000050d0: 7267 696e 696e 652c 2048 6973 7469 6469  rginine, Histidi
+000050e0: 6e65 2c20 4c79 7369 6e65 2e0a 0a20 2020  ne, Lysine...   
+000050f0: 2020 2020 202a 204e 6f6e 2d73 7461 6e64       * Non-stand
+00005100: 6172 6420 2852 5829 3a20 4e6f 6e2d 7374  ard (RX): Non-st
+00005110: 616e 6461 7264 2072 6573 6964 7565 732e  andard residues.
+00005120: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+00005130: 650a 2020 2020 2020 2020 2d2d 2d2d 2d2d  e.        ------
+00005140: 2d0a 2020 2020 2020 2020 3e3e 3e20 6672  -.        >>> fr
+00005150: 6f6d 2070 794b 5646 696e 6465 7220 696d  om pyKVFinder im
+00005160: 706f 7274 2070 794b 5646 696e 6465 720a  port pyKVFinder.
+00005170: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+00005180: 7274 206f 730a 2020 2020 2020 2020 3e3e  rt os.        >>
+00005190: 3e20 7064 6220 3d20 6f73 2e70 6174 682e  > pdb = os.path.
+000051a0: 6a6f 696e 286f 732e 7061 7468 2e64 6972  join(os.path.dir
+000051b0: 6e61 6d65 2870 794b 5646 696e 6465 722e  name(pyKVFinder.
+000051c0: 5f5f 6669 6c65 5f5f 292c 2027 6461 7461  __file__), 'data
+000051d0: 272c 2027 7465 7374 7327 2c20 2731 464d  ', 'tests', '1FM
+000051e0: 4f2e 7064 6227 290a 2020 2020 2020 2020  O.pdb').        
+000051f0: 3e3e 3e20 7265 7375 6c74 7320 3d20 7079  >>> results = py
+00005200: 4b56 4669 6e64 6572 2870 6462 290a 2020  KVFinder(pdb).  
+00005210: 2020 2020 2020 3e3e 3e20 7265 7375 6c74        >>> result
+00005220: 732e 6578 706f 7274 5f61 6c6c 2829 0a0a  s.export_all()..
+00005230: 2020 2020 2020 2020 5965 742c 2077 6520          Yet, we 
+00005240: 6361 6e20 7365 7420 6120 6060 696e 636c  can set a ``incl
+00005250: 7564 655f 6672 6571 7565 6e63 6965 735f  ude_frequencies_
+00005260: 7064 6660 6020 666c 6167 2074 6f20 5472  pdf`` flag to Tr
+00005270: 7565 2074 6f20 706c 6f74 2074 6865 2062  ue to plot the b
+00005280: 6172 2063 6861 7274 7320 6f66 2074 6865  ar charts of the
+00005290: 2066 7265 7175 656e 6369 6573 2069 6e20   frequencies in 
+000052a0: 6120 5044 4620 6669 6c65 2e0a 0a20 2020  a PDF file...   
+000052b0: 2020 2020 203e 3e3e 2072 6573 756c 7473       >>> results
+000052c0: 2e65 7870 6f72 745f 616c 6c28 696e 636c  .export_all(incl
+000052d0: 7564 655f 6672 6571 7565 6e63 6965 735f  ude_frequencies_
+000052e0: 7064 663d 5472 7565 290a 2020 2020 2020  pdf=True).      
+000052f0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+00005300: 4578 706f 7274 2063 6176 6974 7920 5044  Export cavity PD
+00005310: 4220 6669 6c65 0a20 2020 2020 2020 2073  B file.        s
+00005320: 656c 662e 6578 706f 7274 286f 7574 7075  elf.export(outpu
+00005330: 742c 206e 7468 7265 6164 7329 0a20 2020  t, nthreads).   
+00005340: 2020 2020 2023 2057 7269 7465 204b 5646       # Write KVF
+00005350: 696e 6465 7220 7265 7375 6c74 7320 544f  inder results TO
+00005360: 4d4c 0a20 2020 2020 2020 2073 656c 662e  ML.        self.
+00005370: 7772 6974 6528 666e 2c20 6f75 7470 7574  write(fn, output
+00005380: 290a 2020 2020 2020 2020 2320 506c 6f74  ).        # Plot
+00005390: 2062 6172 2063 6861 7274 7320 6f66 2066   bar charts of f
+000053a0: 7265 7175 656e 6369 6573 0a20 2020 2020  requencies.     
+000053b0: 2020 2069 6620 696e 636c 7564 655f 6672     if include_fr
+000053c0: 6571 7565 6e63 6965 735f 7064 663a 0a20  equencies_pdf:. 
+000053d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000053e0: 706c 6f74 5f66 7265 7175 656e 6369 6573  plot_frequencies
+000053f0: 2870 6466 290a 0a0a 6465 6620 7275 6e5f  (pdf)...def run_
+00005400: 776f 726b 666c 6f77 280a 2020 2020 696e  workflow(.    in
+00005410: 7075 743a 2055 6e69 6f6e 5b73 7472 2c20  put: Union[str, 
+00005420: 7061 7468 6c69 622e 5061 7468 5d2c 0a20  pathlib.Path],. 
+00005430: 2020 206c 6967 616e 643a 204f 7074 696f     ligand: Optio
+00005440: 6e61 6c5b 556e 696f 6e5b 7374 722c 2070  nal[Union[str, p
+00005450: 6174 686c 6962 2e50 6174 685d 5d20 3d20  athlib.Path]] = 
+00005460: 4e6f 6e65 2c0a 2020 2020 7664 773a 204f  None,.    vdw: O
+00005470: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
+00005480: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+00005490: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 626f  ] = None,.    bo
+000054a0: 783a 204f 7074 696f 6e61 6c5b 556e 696f  x: Optional[Unio
+000054b0: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
+000054c0: 6174 685d 5d20 3d20 4e6f 6e65 2c0a 2020  ath]] = None,.  
+000054d0: 2020 7374 6570 3a20 556e 696f 6e5b 666c    step: Union[fl
+000054e0: 6f61 742c 2069 6e74 5d20 3d20 302e 362c  oat, int] = 0.6,
+000054f0: 0a20 2020 2070 726f 6265 5f69 6e3a 2055  .    probe_in: U
+00005500: 6e69 6f6e 5b66 6c6f 6174 2c20 696e 745d  nion[float, int]
+00005510: 203d 2031 2e34 2c0a 2020 2020 7072 6f62   = 1.4,.    prob
+00005520: 655f 6f75 743a 2055 6e69 6f6e 5b66 6c6f  e_out: Union[flo
+00005530: 6174 2c20 696e 745d 203d 2034 2e30 2c0a  at, int] = 4.0,.
+00005540: 2020 2020 7265 6d6f 7661 6c5f 6469 7374      removal_dist
+00005550: 616e 6365 3a20 556e 696f 6e5b 666c 6f61  ance: Union[floa
+00005560: 742c 2069 6e74 5d20 3d20 322e 342c 0a20  t, int] = 2.4,. 
+00005570: 2020 2076 6f6c 756d 655f 6375 746f 6666     volume_cutoff
+00005580: 3a20 556e 696f 6e5b 666c 6f61 742c 2069  : Union[float, i
+00005590: 6e74 5d20 3d20 352e 302c 0a20 2020 206c  nt] = 5.0,.    l
+000055a0: 6967 616e 645f 6375 746f 6666 3a20 556e  igand_cutoff: Un
+000055b0: 696f 6e5b 666c 6f61 742c 2069 6e74 5d20  ion[float, int] 
+000055c0: 3d20 352e 302c 0a20 2020 2069 6e63 6c75  = 5.0,.    inclu
+000055d0: 6465 5f64 6570 7468 3a20 626f 6f6c 203d  de_depth: bool =
+000055e0: 2046 616c 7365 2c0a 2020 2020 696e 636c   False,.    incl
+000055f0: 7564 655f 6879 6472 6f70 6174 6879 3a20  ude_hydropathy: 
+00005600: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00005610: 2020 6879 6472 6f70 686f 6269 6369 7479    hydrophobicity
+00005620: 5f73 6361 6c65 3a20 556e 696f 6e5b 7374  _scale: Union[st
+00005630: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+00005640: 203d 2022 4569 7365 6e62 6572 6757 6569   = "EisenbergWei
+00005650: 7373 222c 0a20 2020 2073 7572 6661 6365  ss",.    surface
+00005660: 3a20 7374 7220 3d20 2253 4553 222c 0a20  : str = "SES",. 
+00005670: 2020 2069 676e 6f72 655f 6261 636b 626f     ignore_backbo
+00005680: 6e65 3a20 626f 6f6c 203d 2046 616c 7365  ne: bool = False
+00005690: 2c0a 2020 2020 6d6f 6465 6c3a 204f 7074  ,.    model: Opt
+000056a0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000056b0: 652c 0a20 2020 206e 7468 7265 6164 733a  e,.    nthreads:
+000056c0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+000056d0: 204e 6f6e 652c 0a20 2020 2076 6572 626f   None,.    verbo
+000056e0: 7365 3a20 626f 6f6c 203d 2046 616c 7365  se: bool = False
+000056f0: 2c0a 2920 2d3e 2070 794b 5646 696e 6465  ,.) -> pyKVFinde
+00005700: 7252 6573 756c 7473 3a0a 2020 2020 2222  rResults:.    ""
+00005710: 2244 6574 6563 7473 2061 6e64 2063 6861  "Detects and cha
+00005720: 7261 6374 6572 697a 6573 2063 6176 6974  racterizes cavit
+00005730: 6965 7320 2876 6f6c 756d 652c 2061 7265  ies (volume, are
+00005740: 612c 2064 6570 7468 205b 6f70 7469 6f6e  a, depth [option
+00005750: 616c 5d2c 0a20 2020 2068 7964 726f 7061  al],.    hydropa
+00005760: 7468 7920 5b6f 7074 696f 6e61 6c5d 2061  thy [optional] a
+00005770: 6e64 2069 6e74 6572 6661 6365 2072 6573  nd interface res
+00005780: 6964 7565 7329 2e0a 0a20 2020 2050 6172  idues)...    Par
+00005790: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+000057a0: 2d2d 2d2d 2d2d 0a20 2020 2069 6e70 7574  ------.    input
+000057b0: 203a 2055 6e69 6f6e 5b73 7472 2c20 7061   : Union[str, pa
+000057c0: 7468 6c69 622e 5061 7468 5d0a 2020 2020  thlib.Path].    
+000057d0: 2020 2020 4120 7061 7468 2074 6f20 6120      A path to a 
+000057e0: 7461 7267 6574 2073 7472 7563 7475 7265  target structure
+000057f0: 2066 696c 652c 2069 6e20 5044 4220 6f72   file, in PDB or
+00005800: 2058 595a 2066 6f72 6d61 742c 2074 6f20   XYZ format, to 
+00005810: 6465 7465 6374 2061 6e64 2063 6861 7261  detect and chara
+00005820: 6374 6572 697a 6520 6361 7669 7469 6573  cterize cavities
+00005830: 2e0a 2020 2020 6c69 6761 6e64 203a 2055  ..    ligand : U
+00005840: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
+00005850: 622e 5061 7468 5d2c 206f 7074 696f 6e61  b.Path], optiona
+00005860: 6c0a 2020 2020 2020 2020 4120 7061 7468  l.        A path
+00005870: 2074 6f20 6c69 6761 6e64 2066 696c 652c   to ligand file,
+00005880: 2069 6e20 5044 4220 6f72 2058 595a 2066   in PDB or XYZ f
+00005890: 6f72 6d61 742c 2062 7920 6465 6661 756c  ormat, by defaul
+000058a0: 7420 4e6f 6e65 2e0a 2020 2020 7664 7720  t None..    vdw 
+000058b0: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
+000058c0: 686c 6962 2e50 6174 685d 2c20 6f70 7469  hlib.Path], opti
+000058d0: 6f6e 616c 0a20 2020 2020 2020 2041 2070  onal.        A p
+000058e0: 6174 6820 746f 2061 2076 616e 2064 6572  ath to a van der
+000058f0: 2057 6161 6c73 2072 6164 6969 2066 696c   Waals radii fil
+00005900: 652c 2062 7920 6465 6661 756c 7420 4e6f  e, by default No
+00005910: 6e65 2e20 4966 204e 6f6e 652c 2061 7070  ne. If None, app
+00005920: 6c79 2074 6865 2062 7569 6c74 2d69 6e20  ly the built-in 
+00005930: 7661 6e20 6465 720a 2020 2020 2020 2020  van der.        
+00005940: 5761 616c 7320 7261 6469 6920 6669 6c65  Waals radii file
+00005950: 3a20 6076 6477 2e64 6174 602e 0a20 2020  : `vdw.dat`..   
+00005960: 2062 6f78 203a 2055 6e69 6f6e 5b73 7472   box : Union[str
+00005970: 2c20 7061 7468 6c69 622e 5061 7468 5d2c  , pathlib.Path],
+00005980: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00005990: 2020 4120 7061 7468 2074 6f20 626f 7820    A path to box 
+000059a0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000059b0: 6c65 2028 544f 4d4c 2d66 6f72 6d61 7474  le (TOML-formatt
+000059c0: 6564 292c 2062 7920 6465 6661 756c 7420  ed), by default 
+000059d0: 4e6f 6e65 2e0a 2020 2020 7374 6570 203a  None..    step :
+000059e0: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 696e   Union[float, in
+000059f0: 745d 2c20 6f70 7469 6f6e 616c 0a20 2020  t], optional.   
+00005a00: 2020 2020 2047 7269 6420 7370 6163 696e       Grid spacin
+00005a10: 6720 2841 292c 2062 7920 6465 6661 756c  g (A), by defaul
+00005a20: 7420 302e 362e 0a20 2020 2070 726f 6265  t 0.6..    probe
+00005a30: 5f69 6e20 3a20 556e 696f 6e5b 666c 6f61  _in : Union[floa
+00005a40: 742c 2069 6e74 5d2c 206f 7074 696f 6e61  t, int], optiona
+00005a50: 6c0a 2020 2020 2020 2020 5072 6f62 6520  l.        Probe 
+00005a60: 496e 2073 697a 6520 2841 292c 2062 7920  In size (A), by 
+00005a70: 6465 6661 756c 7420 312e 342e 0a20 2020  default 1.4..   
+00005a80: 2070 726f 6265 5f6f 7574 203a 2055 6e69   probe_out : Uni
+00005a90: 6f6e 5b66 6c6f 6174 2c20 696e 745d 2c20  on[float, int], 
+00005aa0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00005ab0: 2050 726f 6265 204f 7574 2073 697a 6520   Probe Out size 
+00005ac0: 2841 292c 2062 7920 6465 6661 756c 7420  (A), by default 
+00005ad0: 342e 302e 0a20 2020 2072 656d 6f76 616c  4.0..    removal
+00005ae0: 5f64 6973 7461 6e63 6520 3a20 556e 696f  _distance : Unio
+00005af0: 6e5b 666c 6f61 742c 2069 6e74 5d2c 206f  n[float, int], o
+00005b00: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00005b10: 4c65 6e67 7468 2074 6f20 6265 2072 656d  Length to be rem
+00005b20: 6f76 6564 2066 726f 6d20 7468 6520 6361  oved from the ca
+00005b30: 7669 7479 2d62 756c 6b20 6672 6f6e 7469  vity-bulk fronti
+00005b40: 6572 2028 4129 2c20 6279 2064 6566 6175  er (A), by defau
+00005b50: 6c74 2032 2e34 2e0a 2020 2020 766f 6c75  lt 2.4..    volu
+00005b60: 6d65 5f63 7574 6f66 6620 3a20 556e 696f  me_cutoff : Unio
+00005b70: 6e5b 666c 6f61 742c 2069 6e74 5d2c 206f  n[float, int], o
+00005b80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00005b90: 4361 7669 7469 6573 2076 6f6c 756d 6520  Cavities volume 
+00005ba0: 6669 6c74 6572 2028 4133 292c 2062 7920  filter (A3), by 
+00005bb0: 6465 6661 756c 7420 352e 302e 0a20 2020  default 5.0..   
+00005bc0: 206c 6967 616e 645f 6375 746f 6666 203a   ligand_cutoff :
+00005bd0: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 696e   Union[float, in
+00005be0: 745d 2c20 6f70 7469 6f6e 616c 0a20 2020  t], optional.   
+00005bf0: 2020 2020 2052 6164 6975 7320 7661 6c75       Radius valu
+00005c00: 6520 746f 206c 696d 6974 2061 2073 7061  e to limit a spa
+00005c10: 6365 2061 726f 756e 6420 6120 6c69 6761  ce around a liga
+00005c20: 6e64 2028 4129 2c20 6279 2064 6566 6175  nd (A), by defau
+00005c30: 6c74 2035 2e30 2e0a 2020 2020 696e 636c  lt 5.0..    incl
+00005c40: 7564 655f 6465 7074 6820 3a20 626f 6f6c  ude_depth : bool
+00005c50: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00005c60: 2020 2057 6865 7468 6572 2074 6f20 6368     Whether to ch
+00005c70: 6172 6163 7465 7269 7a65 2074 6865 2064  aracterize the d
+00005c80: 6570 7468 206f 6620 7468 6520 6465 7465  epth of the dete
+00005c90: 6374 6564 2063 6176 6974 6965 732c 2062  cted cavities, b
+00005ca0: 790a 2020 2020 2020 2020 6465 6661 756c  y.        defaul
+00005cb0: 7420 4661 6c73 652e 0a20 2020 2069 6e63  t False..    inc
+00005cc0: 6c75 6465 5f68 7964 726f 7061 7468 7920  lude_hydropathy 
+00005cd0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00005ce0: 0a20 2020 2020 2020 2057 6865 7468 6572  .        Whether
+00005cf0: 2074 6f20 6368 6172 6163 7465 7269 7a65   to characterize
+00005d00: 2074 6865 2068 7964 726f 7061 7468 7920   the hydropathy 
+00005d10: 6f66 2074 6865 2064 6574 6563 7465 6420  of the detected 
+00005d20: 6361 7669 7469 6573 2c20 6279 0a20 2020  cavities, by.   
+00005d30: 2020 2020 2064 6566 6175 6c74 2046 616c       default Fal
+00005d40: 7365 2e0a 2020 2020 6879 6472 6f70 686f  se..    hydropho
+00005d50: 6269 6369 7479 5f73 6361 6c65 203a 2055  bicity_scale : U
+00005d60: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
+00005d70: 622e 5061 7468 5d2c 206f 7074 696f 6e61  b.Path], optiona
+00005d80: 6c0a 2020 2020 2020 2020 4e61 6d65 206f  l.        Name o
+00005d90: 6620 6120 6275 696c 742d 696e 2068 7964  f a built-in hyd
+00005da0: 726f 7068 6f62 6963 6974 7920 7363 616c  rophobicity scal
+00005db0: 6520 2845 6973 656e 6265 7267 5765 6973  e (EisenbergWeis
+00005dc0: 732c 2048 6573 7361 4865 696a 6e65 2c0a  s, HessaHeijne,.
+00005dd0: 2020 2020 2020 2020 4b79 7465 446f 6f6c          KyteDool
+00005de0: 6974 7465 2c20 4d6f 6f6e 466c 656d 696e  itte, MoonFlemin
+00005df0: 672c 2052 6164 7a69 636b 6157 6f6c 6665  g, RadzickaWolfe
+00005e00: 6e64 656e 2c20 5769 6d6c 6579 5768 6974  nden, WimleyWhit
+00005e10: 652c 205a 6861 6f4c 6f6e 646f 6e29 0a20  e, ZhaoLondon). 
+00005e20: 2020 2020 2020 206f 7220 6120 7061 7468         or a path
+00005e30: 2074 6f20 6120 544f 4d4c 2d66 6f72 6d61   to a TOML-forma
+00005e40: 7474 6564 2066 696c 6520 7769 7468 2061  tted file with a
+00005e50: 2063 7573 746f 6d20 6879 6472 6f70 686f   custom hydropho
+00005e60: 6269 6369 7479 2073 6361 6c65 2c0a 2020  bicity scale,.  
+00005e70: 2020 2020 2020 6279 2064 6566 6175 6c74        by default
+00005e80: 2060 4569 7365 6e62 6572 6757 6569 7373   `EisenbergWeiss
+00005e90: 602e 0a20 2020 2073 7572 6661 6365 203a  `..    surface :
+00005ea0: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
+00005eb0: 2020 2020 2020 204b 6579 776f 7264 7320         Keywords 
+00005ec0: 6f70 7469 6f6e 7320 6172 6520 5345 5320  options are SES 
+00005ed0: 2853 6f6c 7665 6e74 2045 7863 6c75 6465  (Solvent Exclude
+00005ee0: 6420 5375 7266 6163 6529 206f 7220 5341  d Surface) or SA
+00005ef0: 5320 2853 6f6c 7665 6e74 0a20 2020 2020  S (Solvent.     
+00005f00: 2020 2041 6363 6573 7369 626c 6520 5375     Accessible Su
+00005f10: 7266 6163 6529 2c20 6279 2064 6566 6175  rface), by defau
+00005f20: 6c74 2053 4553 2e0a 2020 2020 6967 6e6f  lt SES..    igno
+00005f30: 7265 5f62 6163 6b62 6f6e 6520 3a20 626f  re_backbone : bo
+00005f40: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
+00005f50: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00005f60: 6967 6e6f 7265 2062 6163 6b62 6f6e 6520  ignore backbone 
+00005f70: 6174 6f6d 7320 2843 2c20 4341 2c20 4e2c  atoms (C, CA, N,
+00005f80: 204f 2920 7768 656e 2064 6566 696e 696e   O) when definin
+00005f90: 6720 696e 7465 7266 6163 650a 2020 2020  g interface.    
+00005fa0: 2020 2020 7265 7369 6475 6573 2c20 6279      residues, by
+00005fb0: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
+00005fc0: 2020 2020 6d6f 6465 6c20 3a20 696e 742c      model : int,
+00005fd0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00005fe0: 2020 4d6f 6465 6c20 6e75 6d62 6572 2c20    Model number, 
+00005ff0: 6279 2064 6566 6175 6c74 204e 6f6e 652e  by default None.
+00006000: 2049 6620 4e6f 6e65 2c20 6b65 6570 2061   If None, keep a
+00006010: 746f 6d73 2066 726f 6d20 616c 6c20 6d6f  toms from all mo
+00006020: 6465 6c73 2e0a 2020 2020 6e74 6872 6561  dels..    nthrea
+00006030: 6473 203a 2069 6e74 2c20 6f70 7469 6f6e  ds : int, option
+00006040: 616c 0a20 2020 2020 2020 204e 756d 6265  al.        Numbe
+00006050: 7220 6f66 2074 6872 6561 6473 2c20 6279  r of threads, by
+00006060: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
+00006070: 6620 4e6f 6e65 2c20 7468 6520 6e75 6d62  f None, the numb
+00006080: 6572 206f 6620 7468 7265 6164 7320 6973  er of threads is
+00006090: 0a20 2020 2020 2020 2060 6f73 2e63 7075  .        `os.cpu
+000060a0: 5f63 6f75 6e74 2829 202d 2031 602e 0a20  _count() - 1`.. 
+000060b0: 2020 2076 6572 626f 7365 203a 2062 6f6f     verbose : boo
+000060c0: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
+000060d0: 2020 2020 5072 696e 7420 6578 7472 6120      Print extra 
+000060e0: 696e 666f 726d 6174 696f 6e20 746f 2073  information to s
+000060f0: 7461 6e64 6172 6420 6f75 7470 7574 2c20  tandard output, 
+00006100: 6279 2064 6566 6175 6c74 2046 616c 7365  by default False
+00006110: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00006120: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2072     -------.    r
+00006130: 6573 756c 7473 203a 2070 794b 5646 696e  esults : pyKVFin
+00006140: 6465 7252 6573 756c 7473 0a20 2020 2020  derResults.     
+00006150: 2020 2041 2063 6c61 7373 2077 6974 6820     A class with 
+00006160: 7468 6520 666f 6c6c 6f77 696e 6720 6174  the following at
+00006170: 7472 6962 7574 6573 2064 6566 696e 6564  tributes defined
+00006180: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+00006190: 2063 6176 6974 6965 7320 3a20 6e75 6d70   cavities : nump
+000061a0: 792e 6e64 6172 7261 790a 0a20 2020 2020  y.ndarray..     
+000061b0: 2020 2020 2020 2020 2020 2043 6176 6974             Cavit
+000061c0: 7920 706f 696e 7473 2069 6e20 7468 6520  y points in the 
+000061d0: 3344 2067 7269 6420 2863 6176 6974 6965  3D grid (cavitie
+000061e0: 735b 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a  s[nx][ny][nz])..
+000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006200: 4361 7669 7469 6573 2061 7272 6179 2068  Cavities array h
+00006210: 6173 2069 6e74 6567 6572 206c 6162 656c  as integer label
+00006220: 7320 696e 2065 6163 6820 706f 7369 7469  s in each positi
+00006230: 6f6e 2c20 7468 6174 2061 7265 3a0a 0a20  on, that are:.. 
+00006240: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00006250: 202d 313a 2062 756c 6b20 706f 696e 7473   -1: bulk points
+00006260: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00006270: 2020 2a20 303a 2062 696f 6d6f 6c65 6375    * 0: biomolecu
+00006280: 6c65 2070 6f69 6e74 733b 0a20 2020 2020  le points;.     
+00006290: 2020 2020 2020 2020 2020 202a 2031 3a20             * 1: 
+000062a0: 656d 7074 7920 7370 6163 6520 706f 696e  empty space poin
+000062b0: 7473 3b0a 2020 2020 2020 2020 2020 2020  ts;.            
+000062c0: 2020 2020 2a20 3e3d 323a 2063 6176 6974      * >=2: cavit
+000062d0: 7920 706f 696e 7473 2e0a 0a20 2020 2020  y points...     
+000062e0: 2020 2020 2020 2020 2020 2054 6865 2065             The e
+000062f0: 6d70 7479 2073 7061 6365 2070 6f69 6e74  mpty space point
+00006300: 7320 6172 6520 7265 6769 6f6e 7320 7468  s are regions th
+00006310: 6174 2064 6f20 6e6f 7420 6d65 6574 2074  at do not meet t
+00006320: 6865 2063 686f 7365 6e0a 2020 2020 2020  he chosen.      
+00006330: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+00006340: 2063 7574 6f66 6620 746f 2062 6520 636f   cutoff to be co
+00006350: 6e73 6964 6572 6564 2061 2063 6176 6974  nsidered a cavit
+00006360: 792e 0a0a 2020 2020 2020 2020 2020 2020  y...            
+00006370: 2a20 7375 7266 6163 6520 3a20 6e75 6d70  * surface : nump
+00006380: 792e 6e64 6172 7261 790a 0a20 2020 2020  y.ndarray..     
+00006390: 2020 2020 2020 2020 2020 2053 7572 6661             Surfa
+000063a0: 6365 2070 6f69 6e74 7320 696e 2074 6865  ce points in the
+000063b0: 2033 4420 6772 6964 2028 7375 7266 6163   3D grid (surfac
+000063c0: 655b 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a  e[nx][ny][nz])..
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 5375 7266 6163 6520 6172 7261 7920 6861  Surface array ha
+000063f0: 7320 696e 7465 6765 7220 6c61 6265 6c73  s integer labels
+00006400: 2069 6e20 6561 6368 2070 6f73 6974 696f   in each positio
+00006410: 6e2c 2074 6861 7420 6172 653a 0a0a 2020  n, that are:..  
+00006420: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00006430: 2d31 3a20 6275 6c6b 2070 6f69 6e74 733b  -1: bulk points;
+00006440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006450: 202a 2030 3a20 6269 6f6d 6f6c 6563 756c   * 0: biomolecul
+00006460: 6520 6f72 2065 6d70 7479 2073 7061 6365  e or empty space
+00006470: 2070 6f69 6e74 733b 0a20 2020 2020 2020   points;.       
+00006480: 2020 2020 2020 2020 202a 203e 3d32 3a20           * >=2: 
+00006490: 7375 7266 6163 6520 706f 696e 7473 2e0a  surface points..
+000064a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064b0: 2054 6865 2065 6d70 7479 2073 7061 6365   The empty space
+000064c0: 2070 6f69 6e74 7320 6172 6520 7265 6769   points are regi
+000064d0: 6f6e 7320 7468 6174 2064 6f20 6e6f 7420  ons that do not 
+000064e0: 6d65 6574 2074 6865 2063 686f 7365 6e0a  meet the chosen.
+000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006500: 766f 6c75 6d65 2063 7574 6f66 6620 746f  volume cutoff to
+00006510: 2062 6520 636f 6e73 6964 6572 6564 2061   be considered a
+00006520: 2063 6176 6974 792e 0a0a 2020 2020 2020   cavity...      
+00006530: 2020 2020 2020 2a20 6465 7074 6873 203a        * depths :
+00006540: 206e 756d 7079 2e6e 6461 7272 6179 2c20   numpy.ndarray, 
+00006550: 6f70 7469 6f6e 616c 0a0a 2020 2020 2020  optional..      
+00006560: 2020 2020 2020 2020 2020 4120 6e75 6d70            A nump
+00006570: 792e 6e64 6172 7261 7920 7769 7468 2064  y.ndarray with d
+00006580: 6570 7468 206f 6620 6361 7669 7479 2070  epth of cavity p
+00006590: 6f69 6e74 7320 2864 6570 7468 5b6e 785d  oints (depth[nx]
+000065a0: 5b6e 795d 5b6e 7a5d 292e 0a0a 2020 2020  [ny][nz])...    
+000065b0: 2020 2020 2020 2020 2a20 7363 616c 6573          * scales
+000065c0: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+000065d0: 2c20 6f70 7469 6f6e 616c 0a0a 2020 2020  , optional..    
+000065e0: 2020 2020 2020 2020 2020 2020 4120 6e75              A nu
+000065f0: 6d70 792e 6e64 6172 7261 7920 7769 7468  mpy.ndarray with
+00006600: 2068 7964 726f 7068 6f62 6963 6974 7920   hydrophobicity 
+00006610: 7363 616c 6520 7661 6c75 6520 6d61 7070  scale value mapp
+00006620: 6564 2061 7420 7375 7266 6163 650a 2020  ed at surface.  
+00006630: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00006640: 696e 7473 2028 7363 616c 6573 5b6e 785d  ints (scales[nx]
+00006650: 5b6e 795d 5b6e 7a5d 292e 0a0a 2020 2020  [ny][nz])...    
+00006660: 2020 2020 2020 2020 2a20 6e63 6176 203a          * ncav :
+00006670: 2069 6e74 0a0a 2020 2020 2020 2020 2020   int..          
+00006680: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00006690: 6361 7669 7469 6573 2e0a 0a20 2020 2020  cavities...     
+000066a0: 2020 2020 2020 202a 2076 6f6c 756d 6520         * volume 
+000066b0: 3a20 4469 6374 5b73 7472 2c20 666c 6f61  : Dict[str, floa
+000066c0: 745d 0a0a 2020 2020 2020 2020 2020 2020  t]..            
+000066d0: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
+000066e0: 2077 6974 6820 766f 6c75 6d65 206f 6620   with volume of 
+000066f0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
+00006700: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
+00006710: 2020 202a 2061 7265 6120 3a20 4469 6374     * area : Dict
+00006720: 5b73 7472 2c20 666c 6f61 745d 0a0a 2020  [str, float]..  
+00006730: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+00006740: 6469 6374 696f 6e61 7279 2077 6974 6820  dictionary with 
+00006750: 6172 6561 206f 6620 6561 6368 2064 6574  area of each det
+00006760: 6563 7465 6420 6361 7669 7479 2e0a 0a20  ected cavity... 
+00006770: 2020 2020 2020 2020 2020 202a 206d 6178             * max
+00006780: 5f64 6570 7468 203a 2044 6963 745b 7374  _depth : Dict[st
+00006790: 722c 2066 6c6f 6174 5d2c 206f 7074 696f  r, float], optio
+000067a0: 6e61 6c0a 0a20 2020 2020 2020 2020 2020  nal..           
+000067b0: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
+000067c0: 7920 7769 7468 206d 6178 696d 756d 2064  y with maximum d
+000067d0: 6570 7468 206f 6620 6561 6368 2064 6574  epth of each det
+000067e0: 6563 7465 6420 6361 7669 7479 2e0a 0a20  ected cavity... 
+000067f0: 2020 2020 2020 2020 2020 202a 2061 7667             * avg
+00006800: 5f64 6570 7468 203a 2044 6963 745b 7374  _depth : Dict[st
+00006810: 722c 2066 6c6f 6174 5d2c 206f 7074 696f  r, float], optio
+00006820: 6e61 6c0a 0a20 2020 2020 2020 2020 2020  nal..           
+00006830: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
+00006840: 7920 7769 7468 2061 7665 7261 6765 2064  y with average d
+00006850: 6570 7468 206f 6620 6561 6368 2064 6574  epth of each det
+00006860: 6563 7465 6420 6361 7669 7479 2e0a 0a20  ected cavity... 
+00006870: 2020 2020 2020 2020 2020 202a 2061 7667             * avg
+00006880: 5f68 7964 726f 7061 7468 7920 3a20 4469  _hydropathy : Di
+00006890: 6374 5b73 7472 2c20 666c 6f61 745d 2c20  ct[str, float], 
+000068a0: 6f70 7469 6f6e 616c 0a0a 2020 2020 2020  optional..      
+000068b0: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
+000068c0: 696f 6e61 7279 2077 6974 6820 6176 6572  ionary with aver
+000068d0: 6167 6520 6879 6472 6f70 6174 6879 2066  age hydropathy f
+000068e0: 6f72 2065 6163 6820 6465 7465 6374 6564  or each detected
+000068f0: 2063 6176 6974 7920 616e 640a 2020 2020   cavity and.    
+00006900: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00006910: 7261 6e67 6520 6f66 2074 6865 2068 7964  range of the hyd
+00006920: 726f 7068 6f62 6963 6974 7920 7363 616c  rophobicity scal
+00006930: 6520 286d 696e 2c20 6d61 7829 2e0a 0a20  e (min, max)... 
+00006940: 2020 2020 2020 2020 2020 202a 2072 6573             * res
+00006950: 6964 7565 733a 2044 6963 745b 7374 722c  idues: Dict[str,
+00006960: 204c 6973 745b 4c69 7374 5b73 7472 5d5d   List[List[str]]
+00006970: 5d0a 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00006980: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00006990: 7769 7468 2061 206c 6973 7420 6f66 2069  with a list of i
+000069a0: 6e74 6572 6661 6365 2072 6573 6964 7565  nterface residue
+000069b0: 7320 666f 7220 6561 6368 2064 6574 6563  s for each detec
+000069c0: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+000069d0: 2020 2020 6361 7669 7479 2e0a 0a20 2020      cavity...   
+000069e0: 2020 2020 2020 2020 202a 2066 7265 7175           * frequ
+000069f0: 656e 6369 6573 203a 2044 6963 745b 7374  encies : Dict[st
+00006a00: 722c 2044 6963 745b 7374 722c 2044 6963  r, Dict[str, Dic
+00006a10: 745b 7374 722c 2069 6e74 5d5d 5d2c 206f  t[str, int]]], o
+00006a20: 7074 696f 6e61 6c0a 0a20 2020 2020 2020  ptional..       
+00006a30: 2020 2020 2020 2020 2041 2064 6963 7469           A dicti
+00006a40: 6f6e 6172 7920 7769 7468 2066 7265 7175  onary with frequ
+00006a50: 656e 6369 6573 206f 6620 7265 7369 6475  encies of residu
+00006a60: 6573 2061 6e64 2063 6c61 7373 2066 6f72  es and class for
+00006a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a80: 2072 6573 6964 7565 7320 6f66 2065 6163   residues of eac
+00006a90: 6820 6465 7465 6374 6564 2063 6176 6974  h detected cavit
+00006aa0: 792e 0a0a 2020 2020 2020 2020 2020 2020  y...            
+00006ab0: 2a20 5f76 6572 7469 6365 7320 3a20 6e75  * _vertices : nu
+00006ac0: 6d70 792e 6e64 6172 7261 790a 0a20 2020  mpy.ndarray..   
+00006ad0: 2020 2020 2020 2020 2020 2020 2041 206e               A n
+00006ae0: 756d 7079 2e6e 6461 7272 6179 206f 7220  umpy.ndarray or 
+00006af0: 6120 6c69 7374 2077 6974 6820 7879 7a20  a list with xyz 
+00006b00: 7665 7274 6963 6573 2063 6f6f 7264 696e  vertices coordin
+00006b10: 6174 6573 2028 6f72 6967 696e 2c0a 2020  ates (origin,.  
+00006b20: 2020 2020 2020 2020 2020 2020 2020 582d                X-
+00006b30: 6178 6973 2c20 592d 6178 6973 2c20 5a2d  axis, Y-axis, Z-
+00006b40: 6178 6973 292e 0a0a 2020 2020 2020 2020  axis)...        
+00006b50: 2020 2020 2a20 5f73 7465 7020 3a20 666c      * _step : fl
+00006b60: 6f61 740a 0a20 2020 2020 2020 2020 2020  oat..           
+00006b70: 2020 2020 2047 7269 6420 7370 6163 696e       Grid spacin
+00006b80: 6720 2841 292e 0a0a 2020 2020 2020 2020  g (A)...        
+00006b90: 2020 2020 2a20 5f69 6e70 7574 203a 2055      * _input : U
+00006ba0: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
+00006bb0: 622e 5061 7468 5d2c 206f 7074 696f 6e61  b.Path], optiona
+00006bc0: 6c0a 0a20 2020 2020 2020 2020 2020 2020  l..             
+00006bd0: 2020 2041 2070 6174 6820 746f 2069 6e70     A path to inp
+00006be0: 7574 2050 4442 206f 7220 5859 5a20 6669  ut PDB or XYZ fi
+00006bf0: 6c65 2e0a 0a20 2020 2020 2020 2020 2020  le...           
+00006c00: 202a 205f 6c69 6761 6e64 203a 2055 6e69   * _ligand : Uni
+00006c10: 6f6e 5b73 7472 2c20 7061 7468 6c69 622e  on[str, pathlib.
+00006c20: 5061 7468 5d2c 206f 7074 696f 6e61 6c0a  Path], optional.
+00006c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c40: 2041 2070 6174 6820 746f 206c 6967 616e   A path to ligan
+00006c50: 6420 5044 4220 6f72 2058 595a 2066 696c  d PDB or XYZ fil
+00006c60: 652e 0a0a 2020 2020 5261 6973 6573 0a20  e...    Raises. 
+00006c70: 2020 202d 2d2d 2d2d 2d0a 2020 2020 5479     ------.    Ty
+00006c80: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+00006c90: 6069 6e70 7574 6020 6d75 7374 2068 6176  `input` must hav
+00006ca0: 6520 2e70 6462 206f 7220 2e78 797a 2065  e .pdb or .xyz e
+00006cb0: 7874 656e 7369 6f6e 2e0a 2020 2020 5479  xtension..    Ty
+00006cc0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+00006cd0: 606c 6967 616e 6460 206d 7573 7420 6861  `ligand` must ha
+00006ce0: 7665 202e 7064 6220 6f72 202e 7879 7a20  ve .pdb or .xyz 
+00006cf0: 6578 7465 6e73 696f 6e2e 0a0a 2020 2020  extension...    
+00006d00: 4e6f 7465 0a20 2020 202d 2d2d 2d0a 2020  Note.    ----.  
+00006d10: 2020 5468 6520 6361 7669 7479 206e 6f6d    The cavity nom
+00006d20: 656e 636c 6174 7572 6520 6973 2062 6173  enclature is bas
+00006d30: 6564 206f 6e20 7468 6520 696e 7465 6765  ed on the intege
+00006d40: 7220 6c61 6265 6c2e 2054 6865 2063 6176  r label. The cav
+00006d50: 6974 7920 6d61 726b 6564 0a20 2020 2077  ity marked.    w
+00006d60: 6974 6820 322c 2074 6865 2066 6972 7374  ith 2, the first
+00006d70: 2069 6e74 6567 6572 2063 6f72 7265 7370   integer corresp
+00006d80: 6f6e 6469 6e67 2074 6f20 6120 6361 7669  onding to a cavi
+00006d90: 7479 2c20 6973 204b 4141 2c20 7468 6520  ty, is KAA, the 
+00006da0: 6361 7669 7479 0a20 2020 206d 6172 6b65  cavity.    marke
+00006db0: 6420 7769 7468 2033 2069 7320 4b41 422c  d with 3 is KAB,
+00006dc0: 2074 6865 2063 6176 6974 7920 6d61 726b   the cavity mark
+00006dd0: 6564 2077 6974 6820 3420 6973 204b 4143  ed with 4 is KAC
+00006de0: 2061 6e64 2073 6f20 6f6e 2e0a 0a20 2020   and so on...   
+00006df0: 204e 6f74 650a 2020 2020 2d2d 2d2d 0a20   Note.    ----. 
+00006e00: 2020 2054 6865 2063 6c61 7373 6573 206f     The classes o
+00006e10: 6620 7265 7369 6475 6573 2061 7265 3a0a  f residues are:.
+00006e20: 0a20 2020 202a 2041 6c69 7068 6174 6963  .    * Aliphatic
+00006e30: 2061 706f 6c61 7220 2852 3129 3a20 416c   apolar (R1): Al
+00006e40: 616e 696e 652c 2047 6c79 6369 6e65 2c20  anine, Glycine, 
+00006e50: 4973 6f6c 6575 6369 6e65 2c20 4c65 7563  Isoleucine, Leuc
+00006e60: 696e 652c 204d 6574 6869 6f6e 696e 652c  ine, Methionine,
+00006e70: 2056 616c 696e 652e 0a0a 2020 2020 2a20   Valine...    * 
+00006e80: 4172 6f6d 6174 6963 2028 5232 293a 2050  Aromatic (R2): P
+00006e90: 6865 6e79 6c61 6c61 6e69 6e65 2c20 5472  henylalanine, Tr
+00006ea0: 7970 746f 7068 616e 2c20 5479 726f 7369  yptophan, Tyrosi
+00006eb0: 6e65 2e0a 0a20 2020 202a 2050 6f6c 6172  ne...    * Polar
+00006ec0: 2055 6e63 6861 7267 6564 2028 5233 293a   Uncharged (R3):
+00006ed0: 2041 7370 6172 6167 696e 652c 2043 7973   Asparagine, Cys
+00006ee0: 7465 696e 652c 2047 6c75 7461 6d69 6e65  teine, Glutamine
+00006ef0: 2c20 5072 6f6c 696e 652c 2053 6572 696e  , Proline, Serin
+00006f00: 652c 2054 6872 656f 6e69 6e65 2e0a 0a20  e, Threonine... 
+00006f10: 2020 202a 204e 6567 6174 6976 656c 7920     * Negatively 
+00006f20: 6368 6172 6765 6420 2852 3429 3a20 4173  charged (R4): As
+00006f30: 7061 7274 6174 652c 2047 6c75 7461 6d61  partate, Glutama
+00006f40: 7465 2e0a 0a20 2020 202a 2050 6f73 6974  te...    * Posit
+00006f50: 6976 656c 7920 6368 6172 6765 6420 2852  ively charged (R
+00006f60: 3529 3a20 4172 6769 6e69 6e65 2c20 4869  5): Arginine, Hi
+00006f70: 7374 6964 696e 652c 204c 7973 696e 652e  stidine, Lysine.
+00006f80: 0a0a 2020 2020 2a20 4e6f 6e2d 7374 616e  ..    * Non-stan
+00006f90: 6461 7264 2028 5258 293a 204e 6f6e 2d73  dard (RX): Non-s
+00006fa0: 7461 6e64 6172 6420 7265 7369 6475 6573  tandard residues
+00006fb0: 2e0a 0a20 2020 2053 6565 2041 6c73 6f0a  ...    See Also.
+00006fc0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+00006fd0: 2070 794b 5646 696e 6465 7252 6573 756c   pyKVFinderResul
+00006fe0: 7473 0a0a 2020 2020 4578 616d 706c 650a  ts..    Example.
+00006ff0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00007000: 5468 6520 2a2a 7374 616e 6461 7264 2077  The **standard w
+00007010: 6f72 6b66 6c6f 772a 2a20 666f 7220 6361  orkflow** for ca
+00007020: 7669 7479 2064 6574 6563 7469 6f6e 2077  vity detection w
+00007030: 6974 6820 7370 6174 6961 6c20 2873 7572  ith spatial (sur
+00007040: 6661 6365 2070 6f69 6e74 732c 2076 6f6c  face points, vol
+00007050: 756d 652c 2061 7265 6129 2061 6e64 2063  ume, area) and c
+00007060: 6f6e 7374 6974 7574 696f 6e61 6c20 2869  onstitutional (i
+00007070: 6e74 6572 6661 6365 2072 6573 6964 7565  nterface residue
+00007080: 7320 616e 6420 7468 6569 7220 6672 6571  s and their freq
+00007090: 7565 6e63 6965 7329 2063 6861 7261 6374  uencies) charact
+000070a0: 6572 697a 6174 696f 6e20 2063 616e 2062  erization  can b
+000070b0: 6520 7275 6e20 6174 206f 6e63 6520 7769  e run at once wi
+000070c0: 7468 206f 6e65 2063 6f6d 6d61 6e64 3a0a  th one command:.
+000070d0: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
+000070e0: 6f73 0a20 2020 203e 3e3e 2069 6d70 6f72  os.    >>> impor
+000070f0: 7420 7079 4b56 4669 6e64 6572 0a20 2020  t pyKVFinder.   
+00007100: 203e 3e3e 2070 6462 203d 206f 732e 7061   >>> pdb = os.pa
+00007110: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
+00007120: 6469 726e 616d 6528 7079 4b56 4669 6e64  dirname(pyKVFind
+00007130: 6572 2e5f 5f66 696c 655f 5f29 2c20 2764  er.__file__), 'd
+00007140: 6174 6127 2c20 2774 6573 7473 272c 2027  ata', 'tests', '
+00007150: 3146 4d4f 2e70 6462 2729 0a20 2020 203e  1FMO.pdb').    >
+00007160: 3e3e 2072 6573 756c 7473 203d 2070 794b  >> results = pyK
+00007170: 5646 696e 6465 722e 7275 6e5f 776f 726b  VFinder.run_work
+00007180: 666c 6f77 2870 6462 290a 2020 2020 3e3e  flow(pdb).    >>
+00007190: 3e20 7265 7375 6c74 730a 2020 2020 3c70  > results.    <p
+000071a0: 794b 5646 696e 6465 7252 6573 756c 7473  yKVFinderResults
+000071b0: 206f 626a 6563 743e 0a20 2020 203e 3e3e   object>.    >>>
+000071c0: 2072 6573 756c 7473 2e63 6176 6974 6965   results.cavitie
+000071d0: 730a 2020 2020 6172 7261 7928 5b5b 5b2d  s.    array([[[-
+000071e0: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+000071f0: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+00007200: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+00007210: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+00007220: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+00007230: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+00007240: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+00007250: 5d2c 0a20 2020 2020 2020 2020 2020 202e  ],.            .
+00007260: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
+00007270: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+00007280: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+00007290: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+000072a0: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+000072b0: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+000072c0: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+000072d0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+000072e0: 2d31 5d5d 2c0a 2020 2020 2020 2020 2020  -1]],.          
+000072f0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00007300: 205b 5b2d 312c 202d 312c 202d 312c 202e   [[-1, -1, -1, .
+00007310: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+00007320: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+00007330: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+00007340: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+00007350: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+00007360: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+00007370: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+00007380: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+00007390: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+000073a0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+000073b0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+000073c0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+000073d0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+000073e0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+000073f0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00007400: 2d31 2c20 2d31 5d5d 5d2c 2064 7479 7065  -1, -1]]], dtype
+00007410: 3d69 6e74 3332 290a 2020 2020 3e3e 3e20  =int32).    >>> 
+00007420: 7265 7375 6c74 732e 7375 7266 6163 650a  results.surface.
+00007430: 2020 2020 6172 7261 7928 5b5b 5b2d 312c      array([[[-1,
+00007440: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00007450: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+00007460: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+00007470: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+00007480: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+00007490: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+000074a0: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+000074b0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+000074c0: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+000074d0: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+000074e0: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+000074f0: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+00007500: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+00007510: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+00007520: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+00007530: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+00007540: 5d5d 2c0a 2020 2020 2020 2020 2020 202e  ]],.           .
+00007550: 2e2e 2c0a 2020 2020 2020 2020 2020 205b  ..,.           [
+00007560: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+00007570: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+00007580: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+00007590: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+000075a0: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+000075b0: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+000075c0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+000075d0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+000075e0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+000075f0: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+00007600: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+00007610: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+00007620: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+00007630: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+00007640: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+00007650: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+00007660: 2c20 2d31 5d5d 5d2c 2064 7479 7065 3d69  , -1]]], dtype=i
+00007670: 6e74 3332 290a 2020 2020 3e3e 3e20 7265  nt32).    >>> re
+00007680: 7375 6c74 732e 6e63 6176 0a20 2020 203e  sults.ncav.    >
+00007690: 3e3e 2031 380a 2020 2020 3e3e 3e20 7265  >> 18.    >>> re
+000076a0: 7375 6c74 732e 766f 6c75 6d65 0a20 2020  sults.volume.   
+000076b0: 207b 274b 4141 273a 2031 3337 2e31 362c   {'KAA': 137.16,
+000076c0: 2027 4b41 4227 3a20 3437 2e35 322c 2027   'KAB': 47.52, '
+000076d0: 4b41 4327 3a20 3636 2e39 362c 2027 4b41  KAC': 66.96, 'KA
+000076e0: 4427 3a20 382e 3231 2c20 274b 4145 273a  D': 8.21, 'KAE':
+000076f0: 2034 332e 3633 2c20 274b 4146 273a 2031   43.63, 'KAF': 1
+00007700: 322e 3533 2c20 274b 4147 273a 2036 2e32  2.53, 'KAG': 6.2
+00007710: 362c 2027 4b41 4827 3a20 3532 302e 3133  6, 'KAH': 520.13
+00007720: 2c20 274b 4149 273a 2031 322e 3331 2c20  , 'KAI': 12.31, 
+00007730: 274b 414a 273a 2032 362e 3537 2c20 274b  'KAJ': 26.57, 'K
+00007740: 414b 273a 2031 322e 3331 2c20 274b 414c  AK': 12.31, 'KAL
+00007750: 273a 2033 332e 3931 2c20 274b 414d 273a  ': 33.91, 'KAM':
+00007760: 2032 332e 3131 2c20 274b 414e 273a 2031   23.11, 'KAN': 1
+00007770: 3032 2e38 322c 2027 4b41 4f27 3a20 362e  02.82, 'KAO': 6.
+00007780: 3035 2c20 274b 4150 273a 2031 352e 3535  05, 'KAP': 15.55
+00007790: 2c20 274b 4151 273a 2037 2e39 392c 2027  , 'KAQ': 7.99, '
+000077a0: 4b41 5227 3a20 372e 3738 7d0a 2020 2020  KAR': 7.78}.    
+000077b0: 3e3e 3e20 7265 7375 6c74 732e 6172 6561  >>> results.area
+000077c0: 0a20 2020 207b 274b 4141 273a 2031 3236  .    {'KAA': 126
+000077d0: 2e34 312c 2027 4b41 4227 3a20 3632 2e33  .41, 'KAB': 62.3
+000077e0: 372c 2027 4b41 4327 3a20 3734 2e35 372c  7, 'KAC': 74.57,
+000077f0: 2027 4b41 4427 3a20 3139 2e30 362c 2027   'KAD': 19.06, '
+00007800: 4b41 4527 3a20 3537 2e30 382c 2027 4b41  KAE': 57.08, 'KA
+00007810: 4627 3a20 3232 2e37 372c 2027 4b41 4727  F': 22.77, 'KAG'
+00007820: 3a20 3135 2e33 382c 2027 4b41 4827 3a20  : 15.38, 'KAH': 
+00007830: 3439 362e 3937 2c20 274b 4149 273a 2033  496.97, 'KAI': 3
+00007840: 302e 3538 2c20 274b 414a 273a 2034 352e  0.58, 'KAJ': 45.
+00007850: 3634 2c20 274b 414b 273a 2033 302e 3538  64, 'KAK': 30.58
+00007860: 2c20 274b 414c 273a 2034 352e 3538 2c20  , 'KAL': 45.58, 
+00007870: 274b 414d 273a 2034 352e 3235 2c20 274b  'KAM': 45.25, 'K
+00007880: 414e 273a 2031 3239 2e37 372c 2027 4b41  AN': 129.77, 'KA
+00007890: 4f27 3a20 3132 2e32 382c 2027 4b41 5027  O': 12.28, 'KAP'
+000078a0: 3a20 3235 2e30 342c 2027 4b41 5127 3a20  : 25.04, 'KAQ': 
+000078b0: 3133 2e34 362c 2027 4b41 5227 3a20 3136  13.46, 'KAR': 16
+000078c0: 2e36 7d0a 2020 2020 3e3e 3e20 7265 7375  .6}.    >>> resu
+000078d0: 6c74 732e 7265 7369 6475 6573 0a20 2020  lts.residues.   
+000078e0: 207b 274b 4141 273a 205b 5b27 3134 272c   {'KAA': [['14',
+000078f0: 2027 4527 2c20 2753 4552 275d 2c20 5b27   'E', 'SER'], ['
+00007900: 3135 272c 2027 4527 2c20 2756 414c 275d  15', 'E', 'VAL']
+00007910: 2c20 5b27 3138 272c 2027 4527 2c20 2750  , ['18', 'E', 'P
+00007920: 4845 275d 2c20 5b27 3139 272c 2027 4527  HE'], ['19', 'E'
+00007930: 2c20 274c 4555 275d 2c20 5b27 3130 3027  , 'LEU'], ['100'
+00007940: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
+00007950: 2731 3532 272c 2027 4527 2c20 274c 4555  '152', 'E', 'LEU
+00007960: 275d 2c20 5b27 3135 3527 2c20 2745 272c  '], ['155', 'E',
+00007970: 2027 474c 5527 5d2c 205b 2731 3536 272c   'GLU'], ['156',
+00007980: 2027 4527 2c20 2754 5952 275d 2c20 5b27   'E', 'TYR'], ['
+00007990: 3239 3227 2c20 2745 272c 2027 4c59 5327  292', 'E', 'LYS'
+000079a0: 5d2c 205b 2733 3032 272c 2027 4527 2c20  ], ['302', 'E', 
+000079b0: 2754 5250 275d 2c20 5b27 3330 3327 2c20  'TRP'], ['303', 
+000079c0: 2745 272c 2027 494c 4527 5d2c 205b 2733  'E', 'ILE'], ['3
+000079d0: 3036 272c 2027 4527 2c20 2754 5952 275d  06', 'E', 'TYR']
+000079e0: 5d2c 2027 4b41 4227 3a20 5b5b 2731 3827  ], 'KAB': [['18'
+000079f0: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
+00007a00: 2732 3227 2c20 2745 272c 2027 414c 4127  '22', 'E', 'ALA'
+00007a10: 5d2c 205b 2732 3527 2c20 2745 272c 2027  ], ['25', 'E', '
+00007a20: 4153 5027 5d2c 205b 2732 3627 2c20 2745  ASP'], ['26', 'E
+00007a30: 272c 2027 5048 4527 5d2c 205b 2732 3927  ', 'PHE'], ['29'
+00007a40: 2c20 2745 272c 2027 4c59 5327 5d2c 205b  , 'E', 'LYS'], [
+00007a50: 2739 3727 2c20 2745 272c 2027 414c 4127  '97', 'E', 'ALA'
+00007a60: 5d2c 205b 2739 3827 2c20 2745 272c 2027  ], ['98', 'E', '
+00007a70: 5641 4c27 5d2c 205b 2739 3927 2c20 2745  VAL'], ['99', 'E
+00007a80: 272c 2027 4153 4e27 5d2c 205b 2731 3536  ', 'ASN'], ['156
+00007a90: 272c 2027 4527 2c20 2754 5952 275d 5d2c  ', 'E', 'TYR']],
+00007aa0: 2027 4b41 4327 3a20 5b5b 2731 3431 272c   'KAC': [['141',
+00007ab0: 2027 4527 2c20 2750 524f 275d 2c20 5b27   'E', 'PRO'], ['
+00007ac0: 3134 3227 2c20 2745 272c 2027 4849 5327  142', 'E', 'HIS'
+00007ad0: 5d2c 205b 2731 3434 272c 2027 4527 2c20  ], ['144', 'E', 
+00007ae0: 2741 5247 275d 2c20 5b27 3134 3527 2c20  'ARG'], ['145', 
+00007af0: 2745 272c 2027 5048 4527 5d2c 205b 2731  'E', 'PHE'], ['1
+00007b00: 3438 272c 2027 4527 2c20 2741 4c41 275d  48', 'E', 'ALA']
+00007b10: 2c20 5b27 3239 3927 2c20 2745 272c 2027  , ['299', 'E', '
+00007b20: 5448 5227 5d2c 205b 2733 3030 272c 2027  THR'], ['300', '
+00007b30: 4527 2c20 2754 4852 275d 2c20 5b27 3330  E', 'THR'], ['30
+00007b40: 3527 2c20 2745 272c 2027 494c 4527 5d2c  5', 'E', 'ILE'],
+00007b50: 205b 2733 3130 272c 2027 4527 2c20 2756   ['310', 'E', 'V
+00007b60: 414c 275d 2c20 5b27 3331 3127 2c20 2745  AL'], ['311', 'E
+00007b70: 272c 2027 474c 5527 5d2c 205b 2733 3133  ', 'GLU'], ['313
+00007b80: 272c 2027 4527 2c20 2750 524f 275d 5d2c  ', 'E', 'PRO']],
+00007b90: 2027 4b41 4427 3a20 5b5b 2731 3232 272c   'KAD': [['122',
+00007ba0: 2027 4527 2c20 2754 5952 275d 2c20 5b27   'E', 'TYR'], ['
+00007bb0: 3132 3427 2c20 2745 272c 2027 414c 4127  124', 'E', 'ALA'
+00007bc0: 5d2c 205b 2731 3736 272c 2027 4527 2c20  ], ['176', 'E', 
+00007bd0: 2747 4c4e 275d 2c20 5b27 3331 3827 2c20  'GLN'], ['318', 
+00007be0: 2745 272c 2027 5048 4527 5d2c 205b 2733  'E', 'PHE'], ['3
+00007bf0: 3230 272c 2027 4527 2c20 2747 4c59 275d  20', 'E', 'GLY']
+00007c00: 2c20 5b27 3332 3127 2c20 2745 272c 2027  , ['321', 'E', '
+00007c10: 5052 4f27 5d2c 205b 2733 3232 272c 2027  PRO'], ['322', '
+00007c20: 4527 2c20 2747 4c59 275d 2c20 5b27 3332  E', 'GLY'], ['32
+00007c30: 3327 2c20 2745 272c 2027 4153 5027 5d5d  3', 'E', 'ASP']]
+00007c40: 2c20 274b 4145 273a 205b 5b27 3935 272c  , 'KAE': [['95',
+00007c50: 2027 4527 2c20 274c 4555 275d 2c20 5b27   'E', 'LEU'], ['
+00007c60: 3938 272c 2027 4527 2c20 2756 414c 275d  98', 'E', 'VAL']
+00007c70: 2c20 5b27 3939 272c 2027 4527 2c20 2741  , ['99', 'E', 'A
+00007c80: 534e 275d 2c20 5b27 3130 3027 2c20 2745  SN'], ['100', 'E
+00007c90: 272c 2027 5048 4527 5d2c 205b 2731 3033  ', 'PHE'], ['103
+00007ca0: 272c 2027 4527 2c20 274c 4555 275d 2c20  ', 'E', 'LEU'], 
+00007cb0: 5b27 3130 3427 2c20 2745 272c 2027 5641  ['104', 'E', 'VA
+00007cc0: 4c27 5d2c 205b 2731 3035 272c 2027 4527  L'], ['105', 'E'
+00007cd0: 2c20 274c 5953 275d 2c20 5b27 3130 3627  , 'LYS'], ['106'
+00007ce0: 2c20 2745 272c 2027 4c45 5527 5d5d 2c20  , 'E', 'LEU']], 
+00007cf0: 274b 4146 273a 205b 5b27 3132 3327 2c20  'KAF': [['123', 
+00007d00: 2745 272c 2027 5641 4c27 5d2c 205b 2731  'E', 'VAL'], ['1
+00007d10: 3234 272c 2027 4527 2c20 2741 4c41 275d  24', 'E', 'ALA']
+00007d20: 2c20 5b27 3137 3527 2c20 2745 272c 2027  , ['175', 'E', '
+00007d30: 4153 5027 5d2c 205b 2731 3736 272c 2027  ASP'], ['176', '
+00007d40: 4527 2c20 2747 4c4e 275d 2c20 5b27 3138  E', 'GLN'], ['18
+00007d50: 3127 2c20 2745 272c 2027 474c 4e27 5d5d  1', 'E', 'GLN']]
+00007d60: 2c20 274b 4147 273a 205b 5b27 3334 272c  , 'KAG': [['34',
+00007d70: 2027 4527 2c20 2753 4552 275d 2c20 5b27   'E', 'SER'], ['
+00007d80: 3337 272c 2027 4527 2c20 2754 4852 275d  37', 'E', 'THR']
+00007d90: 2c20 5b27 3936 272c 2027 4527 2c20 2747  , ['96', 'E', 'G
+00007da0: 4c4e 275d 2c20 5b27 3130 3627 2c20 2745  LN'], ['106', 'E
+00007db0: 272c 2027 4c45 5527 5d2c 205b 2731 3037  ', 'LEU'], ['107
+00007dc0: 272c 2027 4527 2c20 2747 4c55 275d 2c20  ', 'E', 'GLU'], 
+00007dd0: 5b27 3130 3827 2c20 2745 272c 2027 5048  ['108', 'E', 'PH
+00007de0: 4527 5d2c 205b 2731 3039 272c 2027 4527  E'], ['109', 'E'
+00007df0: 2c20 2753 4552 275d 5d2c 2027 4b41 4827  , 'SER']], 'KAH'
+00007e00: 3a20 5b5b 2734 3927 2c20 2745 272c 2027  : [['49', 'E', '
+00007e10: 4c45 5527 5d2c 205b 2735 3027 2c20 2745  LEU'], ['50', 'E
+00007e20: 272c 2027 474c 5927 5d2c 205b 2735 3127  ', 'GLY'], ['51'
+00007e30: 2c20 2745 272c 2027 5448 5227 5d2c 205b  , 'E', 'THR'], [
+00007e40: 2735 3227 2c20 2745 272c 2027 474c 5927  '52', 'E', 'GLY'
+00007e50: 5d2c 205b 2735 3327 2c20 2745 272c 2027  ], ['53', 'E', '
+00007e60: 5345 5227 5d2c 205b 2735 3427 2c20 2745  SER'], ['54', 'E
+00007e70: 272c 2027 5048 4527 5d2c 205b 2735 3527  ', 'PHE'], ['55'
+00007e80: 2c20 2745 272c 2027 474c 5927 5d2c 205b  , 'E', 'GLY'], [
+00007e90: 2735 3627 2c20 2745 272c 2027 4152 4727  '56', 'E', 'ARG'
+00007ea0: 5d2c 205b 2735 3727 2c20 2745 272c 2027  ], ['57', 'E', '
+00007eb0: 5641 4c27 5d2c 205b 2737 3027 2c20 2745  VAL'], ['70', 'E
+00007ec0: 272c 2027 414c 4127 5d2c 205b 2737 3227  ', 'ALA'], ['72'
+00007ed0: 2c20 2745 272c 2027 4c59 5327 5d2c 205b  , 'E', 'LYS'], [
+00007ee0: 2737 3427 2c20 2745 272c 2027 4c45 5527  '74', 'E', 'LEU'
+00007ef0: 5d2c 205b 2738 3427 2c20 2745 272c 2027  ], ['84', 'E', '
+00007f00: 474c 4e27 5d2c 205b 2738 3727 2c20 2745  GLN'], ['87', 'E
+00007f10: 272c 2027 4849 5327 5d2c 205b 2738 3827  ', 'HIS'], ['88'
+00007f20: 2c20 2745 272c 2027 5448 5227 5d2c 205b  , 'E', 'THR'], [
+00007f30: 2739 3127 2c20 2745 272c 2027 474c 5527  '91', 'E', 'GLU'
+00007f40: 5d2c 205b 2731 3034 272c 2027 4527 2c20  ], ['104', 'E', 
+00007f50: 2756 414c 275d 2c20 5b27 3132 3027 2c20  'VAL'], ['120', 
+00007f60: 2745 272c 2027 4d45 5427 5d2c 205b 2731  'E', 'MET'], ['1
+00007f70: 3231 272c 2027 4527 2c20 2747 4c55 275d  21', 'E', 'GLU']
+00007f80: 2c20 5b27 3132 3227 2c20 2745 272c 2027  , ['122', 'E', '
+00007f90: 5459 5227 5d2c 205b 2731 3233 272c 2027  TYR'], ['123', '
+00007fa0: 4527 2c20 2756 414c 275d 2c20 5b27 3132  E', 'VAL'], ['12
+00007fb0: 3727 2c20 2745 272c 2027 474c 5527 5d2c  7', 'E', 'GLU'],
+00007fc0: 205b 2731 3636 272c 2027 4527 2c20 2741   ['166', 'E', 'A
+00007fd0: 5350 275d 2c20 5b27 3136 3827 2c20 2745  SP'], ['168', 'E
+00007fe0: 272c 2027 4c59 5327 5d2c 205b 2731 3730  ', 'LYS'], ['170
+00007ff0: 272c 2027 4527 2c20 2747 4c55 275d 2c20  ', 'E', 'GLU'], 
+00008000: 5b27 3137 3127 2c20 2745 272c 2027 4153  ['171', 'E', 'AS
+00008010: 4e27 5d2c 205b 2731 3733 272c 2027 4527  N'], ['173', 'E'
+00008020: 2c20 274c 4555 275d 2c20 5b27 3138 3327  , 'LEU'], ['183'
+00008030: 2c20 2745 272c 2027 5448 5227 5d2c 205b  , 'E', 'THR'], [
+00008040: 2731 3834 272c 2027 4527 2c20 2741 5350  '184', 'E', 'ASP
+00008050: 275d 2c20 5b27 3138 3627 2c20 2745 272c  '], ['186', 'E',
+00008060: 2027 474c 5927 5d2c 205b 2731 3837 272c   'GLY'], ['187',
+00008070: 2027 4527 2c20 2750 4845 275d 2c20 5b27   'E', 'PHE'], ['
+00008080: 3230 3127 2c20 2745 272c 2027 5448 5227  201', 'E', 'THR'
+00008090: 5d2c 205b 2733 3237 272c 2027 4527 2c20  ], ['327', 'E', 
+000080a0: 2750 4845 275d 5d2c 2027 4b41 4927 3a20  'PHE']], 'KAI': 
+000080b0: 5b5b 2731 3331 272c 2027 4527 2c20 2748  [['131', 'E', 'H
+000080c0: 4953 275d 2c20 5b27 3133 3827 2c20 2745  IS'], ['138', 'E
+000080d0: 272c 2027 5048 4527 5d2c 205b 2731 3432  ', 'PHE'], ['142
+000080e0: 272c 2027 4527 2c20 2748 4953 275d 2c20  ', 'E', 'HIS'], 
+000080f0: 5b27 3134 3627 2c20 2745 272c 2027 5459  ['146', 'E', 'TY
+00008100: 5227 5d2c 205b 2731 3734 272c 2027 4527  R'], ['174', 'E'
+00008110: 2c20 2749 4c45 275d 2c20 5b27 3331 3427  , 'ILE'], ['314'
+00008120: 2c20 2745 272c 2027 5048 4527 5d5d 2c20  , 'E', 'PHE']], 
+00008130: 274b 414a 273a 205b 5b27 3333 272c 2027  'KAJ': [['33', '
+00008140: 4527 2c20 2750 524f 275d 2c20 5b27 3839  E', 'PRO'], ['89
+00008150: 272c 2027 4527 2c20 274c 4555 275d 2c20  ', 'E', 'LEU'], 
+00008160: 5b27 3932 272c 2027 4527 2c20 274c 5953  ['92', 'E', 'LYS
+00008170: 275d 2c20 5b27 3933 272c 2027 4527 2c20  '], ['93', 'E', 
+00008180: 2741 5247 275d 2c20 5b27 3936 272c 2027  'ARG'], ['96', '
+00008190: 4527 2c20 2747 4c4e 275d 2c20 5b27 3334  E', 'GLN'], ['34
+000081a0: 3927 2c20 2745 272c 2027 474c 5527 5d2c  9', 'E', 'GLU'],
+000081b0: 205b 2733 3530 272c 2027 4527 2c20 2750   ['350', 'E', 'P
+000081c0: 4845 275d 5d2c 2027 4b41 4b27 3a20 5b5b  HE']], 'KAK': [[
+000081d0: 2731 3537 272c 2027 4527 2c20 274c 4555  '157', 'E', 'LEU
+000081e0: 275d 2c20 5b27 3136 3227 2c20 2745 272c  '], ['162', 'E',
+000081f0: 2027 4c45 5527 5d2c 205b 2731 3633 272c   'LEU'], ['163',
+00008200: 2027 4527 2c20 2749 4c45 275d 2c20 5b27   'E', 'ILE'], ['
+00008210: 3136 3427 2c20 2745 272c 2027 5459 5227  164', 'E', 'TYR'
+00008220: 5d2c 205b 2731 3835 272c 2027 4527 2c20  ], ['185', 'E', 
+00008230: 2750 4845 275d 2c20 5b27 3138 3827 2c20  'PHE'], ['188', 
+00008240: 2745 272c 2027 414c 4127 5d5d 2c20 274b  'E', 'ALA']], 'K
+00008250: 414c 273a 205b 5b27 3439 272c 2027 4527  AL': [['49', 'E'
+00008260: 2c20 274c 4555 275d 2c20 5b27 3132 3727  , 'LEU'], ['127'
+00008270: 2c20 2745 272c 2027 474c 5527 5d2c 205b  , 'E', 'GLU'], [
+00008280: 2731 3239 272c 2027 4527 2c20 2750 4845  '129', 'E', 'PHE
+00008290: 275d 2c20 5b27 3133 3027 2c20 2745 272c  '], ['130', 'E',
+000082a0: 2027 5345 5227 5d2c 205b 2733 3236 272c   'SER'], ['326',
+000082b0: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
+000082c0: 3332 3727 2c20 2745 272c 2027 5048 4527  327', 'E', 'PHE'
+000082d0: 5d2c 205b 2733 3238 272c 2027 4527 2c20  ], ['328', 'E', 
+000082e0: 2741 5350 275d 2c20 5b27 3333 3027 2c20  'ASP'], ['330', 
+000082f0: 2745 272c 2027 5459 5227 5d5d 2c20 274b  'E', 'TYR']], 'K
+00008300: 414d 273a 205b 5b27 3531 272c 2027 4527  AM': [['51', 'E'
+00008310: 2c20 2754 4852 275d 2c20 5b27 3535 272c  , 'THR'], ['55',
+00008320: 2027 4527 2c20 2747 4c59 275d 2c20 5b27   'E', 'GLY'], ['
+00008330: 3536 272c 2027 4527 2c20 2741 5247 275d  56', 'E', 'ARG']
+00008340: 2c20 5b27 3733 272c 2027 4527 2c20 2749  , ['73', 'E', 'I
+00008350: 4c45 275d 2c20 5b27 3734 272c 2027 4527  LE'], ['74', 'E'
+00008360: 2c20 274c 4555 275d 2c20 5b27 3735 272c  , 'LEU'], ['75',
+00008370: 2027 4527 2c20 2741 5350 275d 2c20 5b27   'E', 'ASP'], ['
+00008380: 3131 3527 2c20 2745 272c 2027 4153 4e27  115', 'E', 'ASN'
+00008390: 5d2c 205b 2733 3335 272c 2027 4527 2c20  ], ['335', 'E', 
+000083a0: 2749 4c45 275d 2c20 5b27 3333 3627 2c20  'ILE'], ['336', 
+000083b0: 2745 272c 2027 4152 4727 5d5d 2c20 274b  'E', 'ARG']], 'K
+000083c0: 414e 273a 205b 5b27 3136 3527 2c20 2745  AN': [['165', 'E
+000083d0: 272c 2027 4152 4727 5d2c 205b 2731 3636  ', 'ARG'], ['166
+000083e0: 272c 2027 4527 2c20 2741 5350 275d 2c20  ', 'E', 'ASP'], 
+000083f0: 5b27 3136 3727 2c20 2745 272c 2027 4c45  ['167', 'E', 'LE
+00008400: 5527 5d2c 205b 2731 3939 272c 2027 4527  U'], ['199', 'E'
+00008410: 2c20 2743 5953 275d 2c20 5b27 3230 3027  , 'CYS'], ['200'
+00008420: 2c20 2745 272c 2027 474c 5927 5d2c 205b  , 'E', 'GLY'], [
+00008430: 2732 3031 272c 2027 4527 2c20 2754 4852  '201', 'E', 'THR
+00008440: 275d 2c20 5b27 3230 3427 2c20 2745 272c  '], ['204', 'E',
+00008450: 2027 5459 5227 5d2c 205b 2732 3035 272c   'TYR'], ['205',
+00008460: 2027 4527 2c20 274c 4555 275d 2c20 5b27   'E', 'LEU'], ['
+00008470: 3230 3627 2c20 2745 272c 2027 414c 4127  206', 'E', 'ALA'
+00008480: 5d2c 205b 2732 3039 272c 2027 4527 2c20  ], ['209', 'E', 
+00008490: 2749 4c45 275d 2c20 5b27 3231 3927 2c20  'ILE'], ['219', 
+000084a0: 2745 272c 2027 5641 4c27 5d2c 205b 2732  'E', 'VAL'], ['2
+000084b0: 3230 272c 2027 4527 2c20 2741 5350 275d  20', 'E', 'ASP']
+000084c0: 2c20 5b27 3232 3327 2c20 2745 272c 2027  , ['223', 'E', '
+000084d0: 414c 4127 5d5d 2c20 274b 414f 273a 205b  ALA']], 'KAO': [
+000084e0: 5b27 3438 272c 2027 4527 2c20 2754 4852  ['48', 'E', 'THR
+000084f0: 275d 2c20 5b27 3531 272c 2027 4527 2c20  '], ['51', 'E', 
+00008500: 2754 4852 275d 2c20 5b27 3536 272c 2027  'THR'], ['56', '
+00008510: 4527 2c20 2741 5247 275d 2c20 5b27 3333  E', 'ARG'], ['33
+00008520: 3027 2c20 2745 272c 2027 5459 5227 5d2c  0', 'E', 'TYR'],
+00008530: 205b 2733 3331 272c 2027 4527 2c20 2747   ['331', 'E', 'G
+00008540: 4c55 275d 5d2c 2027 4b41 5027 3a20 5b5b  LU']], 'KAP': [[
+00008550: 2732 3232 272c 2027 4527 2c20 2754 5250  '222', 'E', 'TRP
+00008560: 275d 2c20 5b27 3233 3827 2c20 2745 272c  '], ['238', 'E',
+00008570: 2027 5048 4527 5d2c 205b 2732 3533 272c   'PHE'], ['253',
+00008580: 2027 4527 2c20 2747 4c59 275d 2c20 5b27   'E', 'GLY'], ['
+00008590: 3235 3427 2c20 2745 272c 2027 4c59 5327  254', 'E', 'LYS'
+000085a0: 5d2c 205b 2732 3535 272c 2027 4527 2c20  ], ['255', 'E', 
+000085b0: 2756 414c 275d 2c20 5b27 3237 3327 2c20  'VAL'], ['273', 
+000085c0: 2745 272c 2027 4c45 5527 5d5d 2c20 274b  'E', 'LEU']], 'K
+000085d0: 4151 273a 205b 5b27 3230 3727 2c20 2745  AQ': [['207', 'E
+000085e0: 272c 2027 5052 4f27 5d2c 205b 2732 3038  ', 'PRO'], ['208
+000085f0: 272c 2027 4527 2c20 2747 4c55 275d 2c20  ', 'E', 'GLU'], 
+00008600: 5b27 3231 3127 2c20 2745 272c 2027 4c45  ['211', 'E', 'LE
+00008610: 5527 5d2c 205b 2732 3133 272c 2027 4527  U'], ['213', 'E'
+00008620: 2c20 274c 5953 275d 2c20 5b27 3237 3527  , 'LYS'], ['275'
+00008630: 2c20 2745 272c 2027 5641 4c27 5d2c 205b  , 'E', 'VAL'], [
+00008640: 2732 3737 272c 2027 4527 2c20 274c 4555  '277', 'E', 'LEU
+00008650: 275d 5d2c 2027 4b41 5227 3a20 5b5b 2732  ']], 'KAR': [['2
+00008660: 3337 272c 2027 4527 2c20 2750 524f 275d  37', 'E', 'PRO']
+00008670: 2c20 5b27 3233 3827 2c20 2745 272c 2027  , ['238', 'E', '
+00008680: 5048 4527 5d2c 205b 2732 3439 272c 2027  PHE'], ['249', '
+00008690: 4527 2c20 274c 5953 275d 2c20 5b27 3235  E', 'LYS'], ['25
+000086a0: 3427 2c20 2745 272c 2027 4c59 5327 5d2c  4', 'E', 'LYS'],
+000086b0: 205b 2732 3535 272c 2027 4527 2c20 2756   ['255', 'E', 'V
+000086c0: 414c 275d 2c20 5b27 3235 3627 2c20 2745  AL'], ['256', 'E
+000086d0: 272c 2027 4152 4727 5d5d 7d0a 2020 2020  ', 'ARG']]}.    
+000086e0: 3e3e 3e20 7265 7375 6c74 732e 6672 6571  >>> results.freq
+000086f0: 7565 6e63 6965 730a 2020 2020 7b27 4b41  uencies.    {'KA
+00008700: 4127 3a20 7b27 5245 5349 4455 4553 273a  A': {'RESIDUES':
+00008710: 207b 2747 4c55 273a 2031 2c20 2749 4c45   {'GLU': 1, 'ILE
+00008720: 273a 2031 2c20 274c 4555 273a 2032 2c20  ': 1, 'LEU': 2, 
+00008730: 274c 5953 273a 2031 2c20 2750 4845 273a  'LYS': 1, 'PHE':
+00008740: 2032 2c20 2753 4552 273a 2031 2c20 2754   2, 'SER': 1, 'T
+00008750: 5250 273a 2031 2c20 2754 5952 273a 2032  RP': 1, 'TYR': 2
+00008760: 2c20 2756 414c 273a 2031 7d2c 2027 434c  , 'VAL': 1}, 'CL
+00008770: 4153 5327 3a20 7b27 5231 273a 2034 2c20  ASS': {'R1': 4, 
+00008780: 2752 3227 3a20 352c 2027 5233 273a 2031  'R2': 5, 'R3': 1
+00008790: 2c20 2752 3427 3a20 312c 2027 5235 273a  , 'R4': 1, 'R5':
+000087a0: 2031 2c20 2752 5827 3a20 307d 7d2c 2027   1, 'RX': 0}}, '
+000087b0: 4b41 4227 3a20 7b27 5245 5349 4455 4553  KAB': {'RESIDUES
+000087c0: 273a 207b 2741 4c41 273a 2032 2c20 2741  ': {'ALA': 2, 'A
+000087d0: 534e 273a 2031 2c20 2741 5350 273a 2031  SN': 1, 'ASP': 1
+000087e0: 2c20 274c 5953 273a 2031 2c20 2750 4845  , 'LYS': 1, 'PHE
+000087f0: 273a 2032 2c20 2754 5952 273a 2031 2c20  ': 2, 'TYR': 1, 
+00008800: 2756 414c 273a 2031 7d2c 2027 434c 4153  'VAL': 1}, 'CLAS
+00008810: 5327 3a20 7b27 5231 273a 2033 2c20 2752  S': {'R1': 3, 'R
+00008820: 3227 3a20 332c 2027 5233 273a 2031 2c20  2': 3, 'R3': 1, 
+00008830: 2752 3427 3a20 312c 2027 5235 273a 2031  'R4': 1, 'R5': 1
+00008840: 2c20 2752 5827 3a20 307d 7d2c 2027 4b41  , 'RX': 0}}, 'KA
+00008850: 4327 3a20 7b27 5245 5349 4455 4553 273a  C': {'RESIDUES':
+00008860: 207b 2741 4c41 273a 2031 2c20 2741 5247   {'ALA': 1, 'ARG
+00008870: 273a 2031 2c20 2747 4c55 273a 2031 2c20  ': 1, 'GLU': 1, 
+00008880: 2748 4953 273a 2031 2c20 2749 4c45 273a  'HIS': 1, 'ILE':
+00008890: 2031 2c20 2750 4845 273a 2031 2c20 2750   1, 'PHE': 1, 'P
+000088a0: 524f 273a 2032 2c20 2754 4852 273a 2032  RO': 2, 'THR': 2
+000088b0: 2c20 2756 414c 273a 2031 7d2c 2027 434c  , 'VAL': 1}, 'CL
+000088c0: 4153 5327 3a20 7b27 5231 273a 2035 2c20  ASS': {'R1': 5, 
+000088d0: 2752 3227 3a20 312c 2027 5233 273a 2032  'R2': 1, 'R3': 2
+000088e0: 2c20 2752 3427 3a20 312c 2027 5235 273a  , 'R4': 1, 'R5':
+000088f0: 2032 2c20 2752 5827 3a20 307d 7d2c 2027   2, 'RX': 0}}, '
+00008900: 4b41 4427 3a20 7b27 5245 5349 4455 4553  KAD': {'RESIDUES
+00008910: 273a 207b 2741 4c41 273a 2031 2c20 2741  ': {'ALA': 1, 'A
+00008920: 5350 273a 2031 2c20 2747 4c4e 273a 2031  SP': 1, 'GLN': 1
+00008930: 2c20 2747 4c59 273a 2032 2c20 2750 4845  , 'GLY': 2, 'PHE
+00008940: 273a 2031 2c20 2750 524f 273a 2031 2c20  ': 1, 'PRO': 1, 
+00008950: 2754 5952 273a 2031 7d2c 2027 434c 4153  'TYR': 1}, 'CLAS
+00008960: 5327 3a20 7b27 5231 273a 2034 2c20 2752  S': {'R1': 4, 'R
+00008970: 3227 3a20 322c 2027 5233 273a 2031 2c20  2': 2, 'R3': 1, 
+00008980: 2752 3427 3a20 312c 2027 5235 273a 2030  'R4': 1, 'R5': 0
+00008990: 2c20 2752 5827 3a20 307d 7d2c 2027 4b41  , 'RX': 0}}, 'KA
+000089a0: 4527 3a20 7b27 5245 5349 4455 4553 273a  E': {'RESIDUES':
+000089b0: 207b 2741 534e 273a 2031 2c20 274c 4555   {'ASN': 1, 'LEU
+000089c0: 273a 2033 2c20 274c 5953 273a 2031 2c20  ': 3, 'LYS': 1, 
+000089d0: 2750 4845 273a 2031 2c20 2756 414c 273a  'PHE': 1, 'VAL':
+000089e0: 2032 7d2c 2027 434c 4153 5327 3a20 7b27   2}, 'CLASS': {'
+000089f0: 5231 273a 2035 2c20 2752 3227 3a20 312c  R1': 5, 'R2': 1,
+00008a00: 2027 5233 273a 2031 2c20 2752 3427 3a20   'R3': 1, 'R4': 
+00008a10: 302c 2027 5235 273a 2031 2c20 2752 5827  0, 'R5': 1, 'RX'
+00008a20: 3a20 307d 7d2c 2027 4b41 4627 3a20 7b27  : 0}}, 'KAF': {'
+00008a30: 5245 5349 4455 4553 273a 207b 2741 4c41  RESIDUES': {'ALA
+00008a40: 273a 2031 2c20 2741 5350 273a 2031 2c20  ': 1, 'ASP': 1, 
+00008a50: 2747 4c4e 273a 2032 2c20 2756 414c 273a  'GLN': 2, 'VAL':
+00008a60: 2031 7d2c 2027 434c 4153 5327 3a20 7b27   1}, 'CLASS': {'
+00008a70: 5231 273a 2032 2c20 2752 3227 3a20 302c  R1': 2, 'R2': 0,
+00008a80: 2027 5233 273a 2032 2c20 2752 3427 3a20   'R3': 2, 'R4': 
+00008a90: 312c 2027 5235 273a 2030 2c20 2752 5827  1, 'R5': 0, 'RX'
+00008aa0: 3a20 307d 7d2c 2027 4b41 4727 3a20 7b27  : 0}}, 'KAG': {'
+00008ab0: 5245 5349 4455 4553 273a 207b 2747 4c4e  RESIDUES': {'GLN
+00008ac0: 273a 2031 2c20 2747 4c55 273a 2031 2c20  ': 1, 'GLU': 1, 
+00008ad0: 274c 4555 273a 2031 2c20 2750 4845 273a  'LEU': 1, 'PHE':
+00008ae0: 2031 2c20 2753 4552 273a 2032 2c20 2754   1, 'SER': 2, 'T
+00008af0: 4852 273a 2031 7d2c 2027 434c 4153 5327  HR': 1}, 'CLASS'
+00008b00: 3a20 7b27 5231 273a 2031 2c20 2752 3227  : {'R1': 1, 'R2'
+00008b10: 3a20 312c 2027 5233 273a 2034 2c20 2752  : 1, 'R3': 4, 'R
+00008b20: 3427 3a20 312c 2027 5235 273a 2030 2c20  4': 1, 'R5': 0, 
+00008b30: 2752 5827 3a20 307d 7d2c 2027 4b41 4827  'RX': 0}}, 'KAH'
+00008b40: 3a20 7b27 5245 5349 4455 4553 273a 207b  : {'RESIDUES': {
+00008b50: 2741 4c41 273a 2031 2c20 2741 5247 273a  'ALA': 1, 'ARG':
+00008b60: 2031 2c20 2741 534e 273a 2031 2c20 2741   1, 'ASN': 1, 'A
+00008b70: 5350 273a 2032 2c20 2747 4c4e 273a 2031  SP': 2, 'GLN': 1
+00008b80: 2c20 2747 4c55 273a 2034 2c20 2747 4c59  , 'GLU': 4, 'GLY
+00008b90: 273a 2034 2c20 2748 4953 273a 2031 2c20  ': 4, 'HIS': 1, 
+00008ba0: 274c 4555 273a 2033 2c20 274c 5953 273a  'LEU': 3, 'LYS':
+00008bb0: 2032 2c20 274d 4554 273a 2031 2c20 2750   2, 'MET': 1, 'P
+00008bc0: 4845 273a 2033 2c20 2753 4552 273a 2031  HE': 3, 'SER': 1
+00008bd0: 2c20 2754 4852 273a 2034 2c20 2754 5952  , 'THR': 4, 'TYR
+00008be0: 273a 2031 2c20 2756 414c 273a 2033 7d2c  ': 1, 'VAL': 3},
+00008bf0: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
+00008c00: 2031 312c 2027 5232 273a 2034 2c20 2752   11, 'R2': 4, 'R
+00008c10: 3327 3a20 382c 2027 5234 273a 2036 2c20  3': 8, 'R4': 6, 
+00008c20: 2752 3527 3a20 342c 2027 5258 273a 2030  'R5': 4, 'RX': 0
+00008c30: 7d7d 2c20 274b 4149 273a 207b 2752 4553  }}, 'KAI': {'RES
+00008c40: 4944 5545 5327 3a20 7b27 4849 5327 3a20  IDUES': {'HIS': 
+00008c50: 322c 2027 494c 4527 3a20 312c 2027 5048  2, 'ILE': 1, 'PH
+00008c60: 4527 3a20 322c 2027 5459 5227 3a20 317d  E': 2, 'TYR': 1}
+00008c70: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
+00008c80: 3a20 312c 2027 5232 273a 2033 2c20 2752  : 1, 'R2': 3, 'R
+00008c90: 3327 3a20 302c 2027 5234 273a 2030 2c20  3': 0, 'R4': 0, 
+00008ca0: 2752 3527 3a20 322c 2027 5258 273a 2030  'R5': 2, 'RX': 0
+00008cb0: 7d7d 2c20 274b 414a 273a 207b 2752 4553  }}, 'KAJ': {'RES
+00008cc0: 4944 5545 5327 3a20 7b27 4152 4727 3a20  IDUES': {'ARG': 
+00008cd0: 312c 2027 474c 4e27 3a20 312c 2027 474c  1, 'GLN': 1, 'GL
+00008ce0: 5527 3a20 312c 2027 4c45 5527 3a20 312c  U': 1, 'LEU': 1,
+00008cf0: 2027 4c59 5327 3a20 312c 2027 5048 4527   'LYS': 1, 'PHE'
+00008d00: 3a20 312c 2027 5052 4f27 3a20 317d 2c20  : 1, 'PRO': 1}, 
+00008d10: 2743 4c41 5353 273a 207b 2752 3127 3a20  'CLASS': {'R1': 
+00008d20: 322c 2027 5232 273a 2031 2c20 2752 3327  2, 'R2': 1, 'R3'
+00008d30: 3a20 312c 2027 5234 273a 2031 2c20 2752  : 1, 'R4': 1, 'R
+00008d40: 3527 3a20 322c 2027 5258 273a 2030 7d7d  5': 2, 'RX': 0}}
+00008d50: 2c20 274b 414b 273a 207b 2752 4553 4944  , 'KAK': {'RESID
+00008d60: 5545 5327 3a20 7b27 414c 4127 3a20 312c  UES': {'ALA': 1,
+00008d70: 2027 494c 4527 3a20 312c 2027 4c45 5527   'ILE': 1, 'LEU'
+00008d80: 3a20 322c 2027 5048 4527 3a20 312c 2027  : 2, 'PHE': 1, '
+00008d90: 5459 5227 3a20 317d 2c20 2743 4c41 5353  TYR': 1}, 'CLASS
+00008da0: 273a 207b 2752 3127 3a20 342c 2027 5232  ': {'R1': 4, 'R2
+00008db0: 273a 2032 2c20 2752 3327 3a20 302c 2027  ': 2, 'R3': 0, '
+00008dc0: 5234 273a 2030 2c20 2752 3527 3a20 302c  R4': 0, 'R5': 0,
+00008dd0: 2027 5258 273a 2030 7d7d 2c20 274b 414c   'RX': 0}}, 'KAL
+00008de0: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
+00008df0: 7b27 4153 4e27 3a20 312c 2027 4153 5027  {'ASN': 1, 'ASP'
+00008e00: 3a20 312c 2027 474c 5527 3a20 312c 2027  : 1, 'GLU': 1, '
+00008e10: 4c45 5527 3a20 312c 2027 5048 4527 3a20  LEU': 1, 'PHE': 
+00008e20: 322c 2027 5345 5227 3a20 312c 2027 5459  2, 'SER': 1, 'TY
+00008e30: 5227 3a20 317d 2c20 2743 4c41 5353 273a  R': 1}, 'CLASS':
+00008e40: 207b 2752 3127 3a20 312c 2027 5232 273a   {'R1': 1, 'R2':
+00008e50: 2033 2c20 2752 3327 3a20 322c 2027 5234   3, 'R3': 2, 'R4
+00008e60: 273a 2032 2c20 2752 3527 3a20 302c 2027  ': 2, 'R5': 0, '
+00008e70: 5258 273a 2030 7d7d 2c20 274b 414d 273a  RX': 0}}, 'KAM':
+00008e80: 207b 2752 4553 4944 5545 5327 3a20 7b27   {'RESIDUES': {'
+00008e90: 4152 4727 3a20 322c 2027 4153 4e27 3a20  ARG': 2, 'ASN': 
+00008ea0: 312c 2027 4153 5027 3a20 312c 2027 474c  1, 'ASP': 1, 'GL
+00008eb0: 5927 3a20 312c 2027 494c 4527 3a20 322c  Y': 1, 'ILE': 2,
+00008ec0: 2027 4c45 5527 3a20 312c 2027 5448 5227   'LEU': 1, 'THR'
+00008ed0: 3a20 317d 2c20 2743 4c41 5353 273a 207b  : 1}, 'CLASS': {
+00008ee0: 2752 3127 3a20 342c 2027 5232 273a 2030  'R1': 4, 'R2': 0
+00008ef0: 2c20 2752 3327 3a20 322c 2027 5234 273a  , 'R3': 2, 'R4':
+00008f00: 2031 2c20 2752 3527 3a20 322c 2027 5258   1, 'R5': 2, 'RX
+00008f10: 273a 2030 7d7d 2c20 274b 414e 273a 207b  ': 0}}, 'KAN': {
+00008f20: 2752 4553 4944 5545 5327 3a20 7b27 414c  'RESIDUES': {'AL
+00008f30: 4127 3a20 322c 2027 4152 4727 3a20 312c  A': 2, 'ARG': 1,
+00008f40: 2027 4153 5027 3a20 322c 2027 4359 5327   'ASP': 2, 'CYS'
+00008f50: 3a20 312c 2027 474c 5927 3a20 312c 2027  : 1, 'GLY': 1, '
+00008f60: 494c 4527 3a20 312c 2027 4c45 5527 3a20  ILE': 1, 'LEU': 
+00008f70: 322c 2027 5448 5227 3a20 312c 2027 5459  2, 'THR': 1, 'TY
+00008f80: 5227 3a20 312c 2027 5641 4c27 3a20 317d  R': 1, 'VAL': 1}
+00008f90: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
+00008fa0: 3a20 372c 2027 5232 273a 2031 2c20 2752  : 7, 'R2': 1, 'R
+00008fb0: 3327 3a20 322c 2027 5234 273a 2032 2c20  3': 2, 'R4': 2, 
+00008fc0: 2752 3527 3a20 312c 2027 5258 273a 2030  'R5': 1, 'RX': 0
+00008fd0: 7d7d 2c20 274b 414f 273a 207b 2752 4553  }}, 'KAO': {'RES
+00008fe0: 4944 5545 5327 3a20 7b27 4152 4727 3a20  IDUES': {'ARG': 
+00008ff0: 312c 2027 474c 5527 3a20 312c 2027 5448  1, 'GLU': 1, 'TH
+00009000: 5227 3a20 322c 2027 5459 5227 3a20 317d  R': 2, 'TYR': 1}
+00009010: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
+00009020: 3a20 302c 2027 5232 273a 2031 2c20 2752  : 0, 'R2': 1, 'R
+00009030: 3327 3a20 322c 2027 5234 273a 2031 2c20  3': 2, 'R4': 1, 
+00009040: 2752 3527 3a20 312c 2027 5258 273a 2030  'R5': 1, 'RX': 0
+00009050: 7d7d 2c20 274b 4150 273a 207b 2752 4553  }}, 'KAP': {'RES
+00009060: 4944 5545 5327 3a20 7b27 474c 5927 3a20  IDUES': {'GLY': 
+00009070: 312c 2027 4c45 5527 3a20 312c 2027 4c59  1, 'LEU': 1, 'LY
+00009080: 5327 3a20 312c 2027 5048 4527 3a20 312c  S': 1, 'PHE': 1,
+00009090: 2027 5452 5027 3a20 312c 2027 5641 4c27   'TRP': 1, 'VAL'
+000090a0: 3a20 317d 2c20 2743 4c41 5353 273a 207b  : 1}, 'CLASS': {
+000090b0: 2752 3127 3a20 332c 2027 5232 273a 2032  'R1': 3, 'R2': 2
+000090c0: 2c20 2752 3327 3a20 302c 2027 5234 273a  , 'R3': 0, 'R4':
+000090d0: 2030 2c20 2752 3527 3a20 312c 2027 5258   0, 'R5': 1, 'RX
+000090e0: 273a 2030 7d7d 2c20 274b 4151 273a 207b  ': 0}}, 'KAQ': {
+000090f0: 2752 4553 4944 5545 5327 3a20 7b27 474c  'RESIDUES': {'GL
+00009100: 5527 3a20 312c 2027 4c45 5527 3a20 322c  U': 1, 'LEU': 2,
+00009110: 2027 4c59 5327 3a20 312c 2027 5052 4f27   'LYS': 1, 'PRO'
+00009120: 3a20 312c 2027 5641 4c27 3a20 317d 2c20  : 1, 'VAL': 1}, 
+00009130: 2743 4c41 5353 273a 207b 2752 3127 3a20  'CLASS': {'R1': 
+00009140: 342c 2027 5232 273a 2030 2c20 2752 3327  4, 'R2': 0, 'R3'
+00009150: 3a20 302c 2027 5234 273a 2031 2c20 2752  : 0, 'R4': 1, 'R
+00009160: 3527 3a20 312c 2027 5258 273a 2030 7d7d  5': 1, 'RX': 0}}
+00009170: 2c20 274b 4152 273a 207b 2752 4553 4944  , 'KAR': {'RESID
+00009180: 5545 5327 3a20 7b27 4152 4727 3a20 312c  UES': {'ARG': 1,
+00009190: 2027 4c59 5327 3a20 322c 2027 5048 4527   'LYS': 2, 'PHE'
+000091a0: 3a20 312c 2027 5052 4f27 3a20 312c 2027  : 1, 'PRO': 1, '
+000091b0: 5641 4c27 3a20 317d 2c20 2743 4c41 5353  VAL': 1}, 'CLASS
+000091c0: 273a 207b 2752 3127 3a20 322c 2027 5232  ': {'R1': 2, 'R2
+000091d0: 273a 2031 2c20 2752 3327 3a20 302c 2027  ': 1, 'R3': 0, '
+000091e0: 5234 273a 2030 2c20 2752 3527 3a20 332c  R4': 0, 'R5': 3,
+000091f0: 2027 5258 273a 2030 7d7d 7d0a 0a20 2020   'RX': 0}}}..   
+00009200: 2048 6f77 6576 6572 2c20 7573 6572 7320   However, users 
+00009210: 6d61 7920 6f70 7420 746f 2070 6572 666f  may opt to perfo
+00009220: 726d 2063 6176 6974 7920 6465 7465 6374  rm cavity detect
+00009230: 696f 6e20 696e 2061 2073 6567 6d65 6e74  ion in a segment
+00009240: 6564 2073 7061 6365 2074 6872 6f75 6768  ed space through
+00009250: 206c 6967 616e 6420 6164 6a75 7374 6d65   ligand adjustme
+00009260: 6e74 2061 6e64 2f6f 7220 626f 7820 6164  nt and/or box ad
+00009270: 6a75 7374 6d65 6e74 206d 6f64 6573 2e0a  justment modes..
+00009280: 0a20 2020 2054 6865 2063 6176 6974 7920  .    The cavity 
+00009290: 6465 7465 6374 696f 6e20 6361 6e20 6265  detection can be
+000092a0: 206c 696d 6974 6564 2061 726f 756e 6420   limited around 
+000092b0: 7468 6520 7461 7267 6574 206c 6967 616e  the target ligan
+000092c0: 6428 7329 2c20 7768 6963 6820 7769 6c6c  d(s), which will
+000092d0: 2062 6520 7061 7373 6564 2074 6f20 7079   be passed to py
+000092e0: 4b56 4669 6e64 6572 2074 6872 6f75 6768  KVFinder through
+000092f0: 2061 202a 2e70 6462 2a20 6f72 2061 202a   a *.pdb* or a *
+00009300: 2e78 797a 2a20 6669 6c65 732e 2054 6875  .xyz* files. Thu
+00009310: 732c 2074 6865 2064 6574 6563 7465 6420  s, the detected 
+00009320: 6361 7669 7469 6573 2061 7265 206c 696d  cavities are lim
+00009330: 6974 6564 2077 6974 6869 6e20 6120 7261  ited within a ra
+00009340: 6469 7573 2028 6060 6c69 6761 6e64 5f63  dius (``ligand_c
+00009350: 7574 6f66 6660 6029 206f 6620 7468 6520  utoff``) of the 
+00009360: 7461 7267 6574 206c 6967 616e 6428 7329  target ligand(s)
+00009370: 2e0a 0a20 2020 203e 3e3e 206c 6967 616e  ...    >>> ligan
+00009380: 6420 3d20 6f73 2e70 6174 682e 6a6f 696e  d = os.path.join
+00009390: 286f 732e 7061 7468 2e64 6972 6e61 6d65  (os.path.dirname
+000093a0: 2870 794b 5646 696e 6465 722e 5f5f 6669  (pyKVFinder.__fi
+000093b0: 6c65 5f5f 292c 2027 6461 7461 272c 2027  le__), 'data', '
+000093c0: 7465 7374 7327 2c20 2741 444e 2e70 6462  tests', 'ADN.pdb
+000093d0: 2729 0a20 2020 203e 3e3e 2072 6573 756c  ').    >>> resul
+000093e0: 7473 203d 2070 794b 5646 696e 6465 722e  ts = pyKVFinder.
+000093f0: 7275 6e5f 776f 726b 666c 6f77 2870 6462  run_workflow(pdb
+00009400: 2c20 6c69 6761 6e64 290a 2020 2020 3e3e  , ligand).    >>
+00009410: 3e20 7265 7375 6c74 730a 2020 2020 3c70  > results.    <p
+00009420: 794b 5646 696e 6465 7252 6573 756c 7473  yKVFinderResults
+00009430: 206f 626a 6563 743e 0a20 2020 203e 3e3e   object>.    >>>
+00009440: 2072 6573 756c 7473 2e63 6176 6974 6965   results.cavitie
+00009450: 730a 2020 2020 6172 7261 7928 5b5b 5b2d  s.    array([[[-
+00009460: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+00009470: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+00009480: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+00009490: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+000094a0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+000094b0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+000094c0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+000094d0: 5d2c 0a20 2020 2020 2020 2020 2020 202e  ],.            .
+000094e0: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
+000094f0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+00009500: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+00009510: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+00009520: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+00009530: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+00009540: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+00009550: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+00009560: 2d31 5d5d 2c0a 2020 2020 2020 2020 2020  -1]],.          
+00009570: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00009580: 205b 5b2d 312c 202d 312c 202d 312c 202e   [[-1, -1, -1, .
+00009590: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+000095a0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+000095b0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+000095c0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+000095d0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+000095e0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+000095f0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+00009600: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+00009610: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+00009620: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+00009630: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00009640: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+00009650: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+00009660: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+00009670: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00009680: 2d31 2c20 2d31 5d5d 5d2c 2064 7479 7065  -1, -1]]], dtype
+00009690: 3d69 6e74 3332 290a 2020 2020 3e3e 3e20  =int32).    >>> 
+000096a0: 7265 7375 6c74 732e 7375 7266 6163 650a  results.surface.
+000096b0: 2020 2020 6172 7261 7928 5b5b 5b2d 312c      array([[[-1,
+000096c0: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+000096d0: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+000096e0: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+000096f0: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+00009700: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+00009710: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+00009720: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+00009730: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00009740: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+00009750: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+00009760: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+00009770: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+00009780: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+00009790: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+000097a0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+000097b0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+000097c0: 5d5d 2c0a 2020 2020 2020 2020 2020 202e  ]],.           .
+000097d0: 2e2e 2c0a 2020 2020 2020 2020 2020 205b  ..,.           [
+000097e0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+000097f0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+00009800: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+00009810: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+00009820: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+00009830: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+00009840: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+00009850: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+00009860: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00009870: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+00009880: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+00009890: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+000098a0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+000098b0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+000098c0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+000098d0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+000098e0: 2c20 2d31 5d5d 5d2c 2064 7479 7065 3d69  , -1]]], dtype=i
+000098f0: 6e74 3332 290a 2020 2020 3e3e 3e20 7265  nt32).    >>> re
+00009900: 7375 6c74 732e 6e63 6176 0a20 2020 203e  sults.ncav.    >
+00009910: 3e3e 2031 380a 2020 2020 3e3e 3e20 7265  >> 18.    >>> re
+00009920: 7375 6c74 732e 766f 6c75 6d65 0a20 2020  sults.volume.   
+00009930: 207b 274b 4141 273a 2033 3635 2e30 342c   {'KAA': 365.04,
+00009940: 2027 4b41 4227 3a20 3136 2e38 357d 0a20   'KAB': 16.85}. 
+00009950: 2020 203e 3e3e 2072 6573 756c 7473 2e61     >>> results.a
+00009960: 7265 610a 2020 2020 7b27 4b41 4127 3a20  rea.    {'KAA': 
+00009970: 3332 382e 3739 2c20 274b 4142 273a 2032  328.79, 'KAB': 2
+00009980: 332e 3135 7d0a 2020 2020 3e3e 3e20 7265  3.15}.    >>> re
+00009990: 7375 6c74 732e 7265 7369 6475 6573 0a20  sults.residues. 
+000099a0: 2020 207b 274b 4141 273a 205b 5b27 3439     {'KAA': [['49
+000099b0: 272c 2027 4527 2c20 274c 4555 275d 2c20  ', 'E', 'LEU'], 
+000099c0: 5b27 3530 272c 2027 4527 2c20 2747 4c59  ['50', 'E', 'GLY
+000099d0: 275d 2c20 5b27 3531 272c 2027 4527 2c20  '], ['51', 'E', 
+000099e0: 2754 4852 275d 2c20 5b27 3532 272c 2027  'THR'], ['52', '
+000099f0: 4527 2c20 2747 4c59 275d 2c20 5b27 3533  E', 'GLY'], ['53
+00009a00: 272c 2027 4527 2c20 2753 4552 275d 2c20  ', 'E', 'SER'], 
+00009a10: 5b27 3535 272c 2027 4527 2c20 2747 4c59  ['55', 'E', 'GLY
+00009a20: 275d 2c20 5b27 3536 272c 2027 4527 2c20  '], ['56', 'E', 
+00009a30: 2741 5247 275d 2c20 5b27 3537 272c 2027  'ARG'], ['57', '
+00009a40: 4527 2c20 2756 414c 275d 2c20 5b27 3730  E', 'VAL'], ['70
+00009a50: 272c 2027 4527 2c20 2741 4c41 275d 2c20  ', 'E', 'ALA'], 
+00009a60: 5b27 3732 272c 2027 4527 2c20 274c 5953  ['72', 'E', 'LYS
+00009a70: 275d 2c20 5b27 3130 3427 2c20 2745 272c  '], ['104', 'E',
+00009a80: 2027 5641 4c27 5d2c 205b 2731 3230 272c   'VAL'], ['120',
+00009a90: 2027 4527 2c20 274d 4554 275d 2c20 5b27   'E', 'MET'], ['
+00009aa0: 3132 3127 2c20 2745 272c 2027 474c 5527  121', 'E', 'GLU'
+00009ab0: 5d2c 205b 2731 3232 272c 2027 4527 2c20  ], ['122', 'E', 
+00009ac0: 2754 5952 275d 2c20 5b27 3132 3327 2c20  'TYR'], ['123', 
+00009ad0: 2745 272c 2027 5641 4c27 5d2c 205b 2731  'E', 'VAL'], ['1
+00009ae0: 3237 272c 2027 4527 2c20 2747 4c55 275d  27', 'E', 'GLU']
+00009af0: 2c20 5b27 3136 3627 2c20 2745 272c 2027  , ['166', 'E', '
+00009b00: 4153 5027 5d2c 205b 2731 3638 272c 2027  ASP'], ['168', '
+00009b10: 4527 2c20 274c 5953 275d 2c20 5b27 3137  E', 'LYS'], ['17
+00009b20: 3027 2c20 2745 272c 2027 474c 5527 5d2c  0', 'E', 'GLU'],
+00009b30: 205b 2731 3731 272c 2027 4527 2c20 2741   ['171', 'E', 'A
+00009b40: 534e 275d 2c20 5b27 3137 3327 2c20 2745  SN'], ['173', 'E
+00009b50: 272c 2027 4c45 5527 5d2c 205b 2731 3833  ', 'LEU'], ['183
+00009b60: 272c 2027 4527 2c20 2754 4852 275d 2c20  ', 'E', 'THR'], 
+00009b70: 5b27 3138 3427 2c20 2745 272c 2027 4153  ['184', 'E', 'AS
+00009b80: 5027 5d2c 205b 2733 3237 272c 2027 4527  P'], ['327', 'E'
+00009b90: 2c20 2750 4845 275d 5d2c 2027 4b41 4227  , 'PHE']], 'KAB'
+00009ba0: 3a20 5b5b 2734 3927 2c20 2745 272c 2027  : [['49', 'E', '
+00009bb0: 4c45 5527 5d2c 205b 2731 3237 272c 2027  LEU'], ['127', '
+00009bc0: 4527 2c20 2747 4c55 275d 2c20 5b27 3133  E', 'GLU'], ['13
+00009bd0: 3027 2c20 2745 272c 2027 5345 5227 5d2c  0', 'E', 'SER'],
+00009be0: 205b 2733 3236 272c 2027 4527 2c20 2741   ['326', 'E', 'A
+00009bf0: 534e 275d 2c20 5b27 3332 3727 2c20 2745  SN'], ['327', 'E
+00009c00: 272c 2027 5048 4527 5d2c 205b 2733 3238  ', 'PHE'], ['328
+00009c10: 272c 2027 4527 2c20 2741 5350 275d 2c20  ', 'E', 'ASP'], 
+00009c20: 5b27 3333 3027 2c20 2745 272c 2027 5459  ['330', 'E', 'TY
+00009c30: 5227 5d5d 7d0a 2020 2020 3e3e 3e20 7265  R']]}.    >>> re
+00009c40: 7375 6c74 732e 6672 6571 7565 6e63 6965  sults.frequencie
+00009c50: 730a 2020 2020 7b27 4b41 4127 3a20 7b27  s.    {'KAA': {'
+00009c60: 5245 5349 4455 4553 273a 207b 2741 4c41  RESIDUES': {'ALA
+00009c70: 273a 2031 2c20 2741 5247 273a 2031 2c20  ': 1, 'ARG': 1, 
+00009c80: 2741 534e 273a 2031 2c20 2741 5350 273a  'ASN': 1, 'ASP':
+00009c90: 2032 2c20 2747 4c55 273a 2033 2c20 2747   2, 'GLU': 3, 'G
+00009ca0: 4c59 273a 2033 2c20 274c 4555 273a 2032  LY': 3, 'LEU': 2
+00009cb0: 2c20 274c 5953 273a 2032 2c20 274d 4554  , 'LYS': 2, 'MET
+00009cc0: 273a 2031 2c20 2750 4845 273a 2031 2c20  ': 1, 'PHE': 1, 
+00009cd0: 2753 4552 273a 2031 2c20 2754 4852 273a  'SER': 1, 'THR':
+00009ce0: 2032 2c20 2754 5952 273a 2031 2c20 2756   2, 'TYR': 1, 'V
+00009cf0: 414c 273a 2033 7d2c 2027 434c 4153 5327  AL': 3}, 'CLASS'
+00009d00: 3a20 7b27 5231 273a 2039 2c20 2752 3227  : {'R1': 9, 'R2'
+00009d10: 3a20 322c 2027 5233 273a 2035 2c20 2752  : 2, 'R3': 5, 'R
+00009d20: 3427 3a20 352c 2027 5235 273a 2033 2c20  4': 5, 'R5': 3, 
+00009d30: 2752 5827 3a20 307d 7d2c 2027 4b41 4227  'RX': 0}}, 'KAB'
+00009d40: 3a20 7b27 5245 5349 4455 4553 273a 207b  : {'RESIDUES': {
+00009d50: 2741 534e 273a 2031 2c20 2741 5350 273a  'ASN': 1, 'ASP':
+00009d60: 2031 2c20 2747 4c55 273a 2031 2c20 274c   1, 'GLU': 1, 'L
+00009d70: 4555 273a 2031 2c20 2750 4845 273a 2031  EU': 1, 'PHE': 1
+00009d80: 2c20 2753 4552 273a 2031 2c20 2754 5952  , 'SER': 1, 'TYR
+00009d90: 273a 2031 7d2c 2027 434c 4153 5327 3a20  ': 1}, 'CLASS': 
+00009da0: 7b27 5231 273a 2031 2c20 2752 3227 3a20  {'R1': 1, 'R2': 
+00009db0: 322c 2027 5233 273a 2032 2c20 2752 3427  2, 'R3': 2, 'R4'
+00009dc0: 3a20 322c 2027 5235 273a 2030 2c20 2752  : 2, 'R5': 0, 'R
+00009dd0: 5827 3a20 307d 7d7d 0a0a 2020 2020 4675  X': 0}}}..    Fu
+00009de0: 7274 6865 722c 2077 6520 6361 6e20 616c  rther, we can al
+00009df0: 736f 2070 6572 666f 726d 2063 6176 6974  so perform cavit
+00009e00: 7920 6465 7465 6374 696f 6e20 6f6e 2061  y detection on a
+00009e10: 2063 7573 746f 6d20 3344 2067 7269 642c   custom 3D grid,
+00009e20: 2077 6865 7265 2077 6520 6361 6e20 6578   where we can ex
+00009e30: 706c 6f72 6520 636c 6f73 6564 2072 6567  plore closed reg
+00009e40: 696f 6e73 2077 6974 6820 6120 6375 7374  ions with a cust
+00009e50: 6f6d 2062 6f78 2c20 7768 6963 6820 6361  om box, which ca
+00009e60: 6e20 6265 2064 6566 696e 6564 2062 7920  n be defined by 
+00009e70: 6120 2a2e 746f 6d6c 2a20 6669 6c65 2028  a *.toml* file (
+00009e80: 7365 6520 6042 6f78 2063 6f6e 6669 6775  see `Box configu
+00009e90: 7261 7469 6f6e 2066 696c 6520 7465 6d70  ration file temp
+00009ea0: 6c61 7465 6029 2e0a 0a20 2020 203e 3e3e  late`)...    >>>
+00009eb0: 2066 6e20 3d20 6f73 2e70 6174 682e 6a6f   fn = os.path.jo
+00009ec0: 696e 286f 732e 7061 7468 2e64 6972 6e61  in(os.path.dirna
+00009ed0: 6d65 2870 794b 5646 696e 6465 722e 5f5f  me(pyKVFinder.__
+00009ee0: 6669 6c65 5f5f 292c 2027 6461 7461 272c  file__), 'data',
+00009ef0: 2027 7465 7374 7327 2c20 2763 7573 746f   'tests', 'custo
+00009f00: 6d2d 626f 782e 746f 6d6c 2729 0a20 2020  m-box.toml').   
+00009f10: 203e 3e3e 2077 6974 6820 6f70 656e 2866   >>> with open(f
+00009f20: 6e2c 2027 7227 2920 6173 2066 3a0a 2020  n, 'r') as f:.  
+00009f30: 2020 2e2e 2e20 2020 2020 7072 696e 7428    ...     print(
+00009f40: 662e 7265 6164 2829 290a 2020 2020 5b62  f.read()).    [b
+00009f50: 6f78 5d0a 2020 2020 7031 203d 205b 332e  ox].    p1 = [3.
+00009f60: 3131 2c20 372e 3334 2c20 312e 3539 5d0a  11, 7.34, 1.59].
+00009f70: 2020 2020 7032 203d 205b 3131 2e35 312c      p2 = [11.51,
+00009f80: 2037 2e33 342c 2031 2e35 395d 0a20 2020   7.34, 1.59].   
+00009f90: 2070 3320 3d20 5b33 2e31 312c 2031 302e   p3 = [3.11, 10.
+00009fa0: 3734 2c20 312e 3539 5d0a 2020 2020 7034  74, 1.59].    p4
+00009fb0: 203d 205b 332e 3131 2c20 372e 3334 2c20   = [3.11, 7.34, 
+00009fc0: 362e 3139 5d0a 2020 2020 3e3e 3e20 7265  6.19].    >>> re
+00009fd0: 7375 6c74 7320 3d20 7079 4b56 4669 6e64  sults = pyKVFind
+00009fe0: 6572 2e72 756e 5f77 6f72 6b66 6c6f 7728  er.run_workflow(
+00009ff0: 7064 622c 2062 6f78 3d66 6e29 0a20 2020  pdb, box=fn).   
+0000a000: 203e 3e3e 2072 6573 756c 7473 0a20 2020   >>> results.   
+0000a010: 203c 7079 4b56 4669 6e64 6572 5265 7375   <pyKVFinderResu
+0000a020: 6c74 7320 6f62 6a65 6374 3e0a 2020 2020  lts object>.    
+0000a030: 3e3e 3e20 7265 7375 6c74 732e 6361 7669  >>> results.cavi
+0000a040: 7469 6573 0a20 2020 2061 7272 6179 285b  ties.    array([
+0000a050: 5b5b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e  [[-1, -1, -1, ..
+0000a060: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+0000a070: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+0000a080: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+0000a090: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+0000a0a0: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+0000a0b0: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+0000a0c0: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+0000a0d0: 2020 2e2e 2e2c 0a20 2020 2020 2020 2020    ...,.         
+0000a0e0: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+0000a0f0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+0000a100: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+0000a110: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+0000a120: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+0000a130: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+0000a140: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+0000a150: 312c 202d 315d 5d2c 0a20 2020 2020 2020  1, -1]],.       
+0000a160: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
+0000a170: 2020 2020 5b5b 2d31 2c20 2d31 2c20 2d31      [[-1, -1, -1
+0000a180: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+0000a190: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+0000a1a0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+0000a1b0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+0000a1c0: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+0000a1d0: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+0000a1e0: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+0000a1f0: 2020 2020 2020 2e2e 2e2c 0a20 2020 2020        ...,.     
+0000a200: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+0000a210: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+0000a220: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+0000a230: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+0000a240: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+0000a250: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+0000a260: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+0000a270: 312c 202d 312c 202d 315d 5d5d 2c20 6474  1, -1, -1]]], dt
+0000a280: 7970 653d 696e 7433 3229 0a20 2020 203e  ype=int32).    >
+0000a290: 3e3e 2072 6573 756c 7473 2e73 7572 6661  >> results.surfa
+0000a2a0: 6365 0a20 2020 2061 7272 6179 285b 5b5b  ce.    array([[[
+0000a2b0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+0000a2c0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+0000a2d0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+0000a2e0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+0000a2f0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+0000a300: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+0000a310: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+0000a320: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+0000a330: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
+0000a340: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+0000a350: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+0000a360: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+0000a370: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+0000a380: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+0000a390: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+0000a3a0: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+0000a3b0: 202d 315d 5d2c 0a20 2020 2020 2020 2020   -1]],.         
+0000a3c0: 2020 2e2e 2e2c 0a20 2020 2020 2020 2020    ...,.         
+0000a3d0: 2020 5b5b 2d31 2c20 2d31 2c20 2d31 2c20    [[-1, -1, -1, 
+0000a3e0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+0000a3f0: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+0000a400: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+0000a410: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+0000a420: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+0000a430: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+0000a440: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+0000a450: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
+0000a460: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+0000a470: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+0000a480: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+0000a490: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+0000a4a0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+0000a4b0: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+0000a4c0: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+0000a4d0: 202d 312c 202d 315d 5d5d 2c20 6474 7970   -1, -1]]], dtyp
+0000a4e0: 653d 696e 7433 3229 0a20 2020 203e 3e3e  e=int32).    >>>
+0000a4f0: 2072 6573 756c 7473 2e6e 6361 760a 2020   results.ncav.  
+0000a500: 2020 3e3e 3e20 310a 2020 2020 3e3e 3e20    >>> 1.    >>> 
+0000a510: 7265 7375 6c74 732e 766f 6c75 6d65 0a20  results.volume. 
+0000a520: 2020 207b 274b 4141 273a 2031 3135 2e37     {'KAA': 115.7
+0000a530: 387d 0a20 2020 203e 3e3e 2072 6573 756c  8}.    >>> resul
+0000a540: 7473 2e61 7265 610a 2020 2020 7b27 4b41  ts.area.    {'KA
+0000a550: 4127 3a20 3333 2e39 317d 0a20 2020 203e  A': 33.91}.    >
+0000a560: 3e3e 2072 6573 756c 7473 2e72 6573 6964  >> results.resid
+0000a570: 7565 730a 2020 2020 7b27 4b41 4127 3a20  ues.    {'KAA': 
+0000a580: 5b5b 2734 3927 2c20 2745 272c 2027 4c45  [['49', 'E', 'LE
+0000a590: 5527 5d2c 205b 2735 3027 2c20 2745 272c  U'], ['50', 'E',
+0000a5a0: 2027 474c 5927 5d2c 205b 2735 3127 2c20   'GLY'], ['51', 
+0000a5b0: 2745 272c 2027 5448 5227 5d2c 205b 2735  'E', 'THR'], ['5
+0000a5c0: 3727 2c20 2745 272c 2027 5641 4c27 5d2c  7', 'E', 'VAL'],
+0000a5d0: 205b 2737 3027 2c20 2745 272c 2027 414c   ['70', 'E', 'AL
+0000a5e0: 4127 5d2c 205b 2731 3034 272c 2027 4527  A'], ['104', 'E'
+0000a5f0: 2c20 2756 414c 275d 2c20 5b27 3132 3127  , 'VAL'], ['121'
+0000a600: 2c20 2745 272c 2027 474c 5527 5d2c 205b  , 'E', 'GLU'], [
+0000a610: 2731 3232 272c 2027 4527 2c20 2754 5952  '122', 'E', 'TYR
+0000a620: 275d 2c20 5b27 3132 3327 2c20 2745 272c  '], ['123', 'E',
+0000a630: 2027 5641 4c27 5d2c 205b 2731 3237 272c   'VAL'], ['127',
+0000a640: 2027 4527 2c20 2747 4c55 275d 2c20 5b27   'E', 'GLU'], ['
+0000a650: 3137 3027 2c20 2745 272c 2027 474c 5527  170', 'E', 'GLU'
+0000a660: 5d2c 205b 2731 3731 272c 2027 4527 2c20  ], ['171', 'E', 
+0000a670: 2741 534e 275d 2c20 5b27 3137 3327 2c20  'ASN'], ['173', 
+0000a680: 2745 272c 2027 4c45 5527 5d2c 205b 2731  'E', 'LEU'], ['1
+0000a690: 3833 272c 2027 4527 2c20 2754 4852 275d  83', 'E', 'THR']
+0000a6a0: 2c20 5b27 3332 3727 2c20 2745 272c 2027  , ['327', 'E', '
+0000a6b0: 5048 4527 5d5d 7d0a 2020 2020 3e3e 3e20  PHE']]}.    >>> 
+0000a6c0: 7265 7375 6c74 732e 6672 6571 7565 6e63  results.frequenc
+0000a6d0: 6965 730a 2020 2020 7b27 4b41 4127 3a20  ies.    {'KAA': 
+0000a6e0: 7b27 5245 5349 4455 4553 273a 207b 2741  {'RESIDUES': {'A
+0000a6f0: 4c41 273a 2031 2c20 2741 534e 273a 2031  LA': 1, 'ASN': 1
+0000a700: 2c20 2747 4c55 273a 2033 2c20 2747 4c59  , 'GLU': 3, 'GLY
+0000a710: 273a 2031 2c20 274c 4555 273a 2032 2c20  ': 1, 'LEU': 2, 
+0000a720: 2750 4845 273a 2031 2c20 2754 4852 273a  'PHE': 1, 'THR':
+0000a730: 2032 2c20 2754 5952 273a 2031 2c20 2756   2, 'TYR': 1, 'V
+0000a740: 414c 273a 2033 7d2c 2027 434c 4153 5327  AL': 3}, 'CLASS'
+0000a750: 3a20 7b27 5231 273a 2037 2c20 2752 3227  : {'R1': 7, 'R2'
+0000a760: 3a20 322c 2027 5233 273a 2033 2c20 2752  : 2, 'R3': 3, 'R
+0000a770: 3427 3a20 332c 2027 5235 273a 2030 2c20  4': 3, 'R5': 0, 
+0000a780: 2752 5827 3a20 307d 7d7d 0a0a 2020 2020  'RX': 0}}}..    
+0000a790: 486f 7765 7665 722c 2075 7365 7273 206d  However, users m
+0000a7a0: 6179 206f 7074 2074 6f20 7065 7266 6f72  ay opt to perfor
+0000a7b0: 6d20 7468 6520 2a2a 6675 6c6c 2077 6f72  m the **full wor
+0000a7c0: 6b66 6c6f 772a 2a20 666f 7220 6361 7669  kflow** for cavi
+0000a7d0: 7479 2064 6574 6563 7469 6f6e 2077 6974  ty detection wit
+0000a7e0: 6820 7370 6174 6961 6c20 2873 7572 6661  h spatial (surfa
+0000a7f0: 6365 2070 6f69 6e74 732c 2076 6f6c 756d  ce points, volum
+0000a800: 6520 616e 6420 6172 6561 292c 2063 6f6e  e and area), con
+0000a810: 7374 6974 7574 696f 6e61 6c20 2869 6e74  stitutional (int
+0000a820: 6572 6661 6365 2072 6573 6964 7565 7320  erface residues 
+0000a830: 616e 6420 7468 6569 7220 6672 6571 7565  and their freque
+0000a840: 6e63 6965 7329 2c20 6879 6472 6f70 6174  ncies), hydropat
+0000a850: 6879 2061 6e64 2064 6570 7468 2063 6861  hy and depth cha
+0000a860: 7261 6374 6572 697a 6174 696f 6e2e 2054  racterization. T
+0000a870: 6869 7320 6675 6c6c 2077 6f72 6b66 6c6f  his full workflo
+0000a880: 7720 6361 6e20 6265 2072 756e 2077 6974  w can be run wit
+0000a890: 6820 6f6e 6520 636f 6d6d 616e 6420 6279  h one command by
+0000a8a0: 2073 6574 7469 6e67 2073 6f6d 6520 7061   setting some pa
+0000a8b0: 7261 6d65 7465 7273 206f 6620 6060 7275  rameters of ``ru
+0000a8c0: 6e5f 776f 726b 666c 6f77 6060 2066 756e  n_workflow`` fun
+0000a8d0: 6374 696f 6e3a 0a0a 2020 2020 3e3e 3e20  ction:..    >>> 
+0000a8e0: 7265 7375 6c74 7320 3d20 7079 4b56 4669  results = pyKVFi
+0000a8f0: 6e64 6572 2e72 756e 5f77 6f72 6b66 6c6f  nder.run_workflo
+0000a900: 7728 7064 622c 2069 6e63 6c75 6465 5f64  w(pdb, include_d
+0000a910: 6570 7468 3d54 7275 652c 2069 6e63 6c75  epth=True, inclu
+0000a920: 6465 5f68 7964 726f 7061 7468 793d 5472  de_hydropathy=Tr
+0000a930: 7565 2c20 6879 6472 6f70 686f 6269 6369  ue, hydrophobici
+0000a940: 7479 5f73 6361 6c65 3d27 4569 7365 6e62  ty_scale='Eisenb
+0000a950: 6572 6757 6569 7373 2729 0a20 2020 203e  ergWeiss').    >
+0000a960: 3e3e 2072 6573 756c 7473 2e64 6570 7468  >> results.depth
+0000a970: 730a 2020 2020 6172 7261 7928 5b5b 5b30  s.    array([[[0
+0000a980: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
+0000a990: 302e 2c20 302e 2c20 302e 5d2c 0a20 2020  0., 0., 0.],.   
+0000a9a0: 2020 2020 2020 2020 205b 302e 2c20 302e           [0., 0.
+0000a9b0: 2c20 302e 2c20 2e2e 2e2c 2030 2e2c 2030  , 0., ..., 0., 0
+0000a9c0: 2e2c 2030 2e5d 2c0a 2020 2020 2020 2020  ., 0.],.        
+0000a9d0: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
+0000a9e0: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
+0000a9f0: 5d2c 0a20 2020 2020 2020 2020 2020 202e  ],.            .
+0000aa00: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
+0000aa10: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
+0000aa20: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
+0000aa30: 2020 2020 2020 2020 2020 205b 302e 2c20             [0., 
+0000aa40: 302e 2c20 302e 2c20 2e2e 2e2c 2030 2e2c  0., 0., ..., 0.,
+0000aa50: 2030 2e2c 2030 2e5d 2c0a 2020 2020 2020   0., 0.],.      
+0000aa60: 2020 2020 2020 5b30 2e2c 2030 2e2c 2030        [0., 0., 0
+0000aa70: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+0000aa80: 302e 5d5d 2c0a 2020 2020 2020 2020 2020  0.]],.          
+0000aa90: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+0000aaa0: 205b 5b30 2e2c 2030 2e2c 2030 2e2c 202e   [[0., 0., 0., .
+0000aab0: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d2c  .., 0., 0., 0.],
+0000aac0: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
+0000aad0: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
+0000aae0: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
+0000aaf0: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+0000ab00: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+0000ab10: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
+0000ab20: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+0000ab30: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
+0000ab40: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
+0000ab50: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+0000ab60: 302e 2c20 302e 2c20 302e 2c20 2e2e 2e2c  0., 0., 0., ...,
+0000ab70: 2030 2e2c 2030 2e2c 2030 2e5d 2c0a 2020   0., 0., 0.],.  
+0000ab80: 2020 2020 2020 2020 2020 5b30 2e2c 2030            [0., 0
+0000ab90: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
+0000aba0: 302e 2c20 302e 5d5d 5d29 0a20 2020 203e  0., 0.]]]).    >
+0000abb0: 3e3e 2072 6573 756c 7473 2e73 6361 6c65  >> results.scale
+0000abc0: 730a 2020 2020 6172 7261 7928 5b5b 5b30  s.    array([[[0
+0000abd0: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
+0000abe0: 302e 2c20 302e 2c20 302e 5d2c 0a20 2020  0., 0., 0.],.   
+0000abf0: 2020 2020 2020 2020 205b 302e 2c20 302e           [0., 0.
+0000ac00: 2c20 302e 2c20 2e2e 2e2c 2030 2e2c 2030  , 0., ..., 0., 0
+0000ac10: 2e2c 2030 2e5d 2c0a 2020 2020 2020 2020  ., 0.],.        
+0000ac20: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
+0000ac30: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
+0000ac40: 5d2c 0a20 2020 2020 2020 2020 2020 202e  ],.            .
+0000ac50: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
+0000ac60: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
+0000ac70: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
+0000ac80: 2020 2020 2020 2020 2020 205b 302e 2c20             [0., 
+0000ac90: 302e 2c20 302e 2c20 2e2e 2e2c 2030 2e2c  0., 0., ..., 0.,
+0000aca0: 2030 2e2c 2030 2e5d 2c0a 2020 2020 2020   0., 0.],.      
+0000acb0: 2020 2020 2020 5b30 2e2c 2030 2e2c 2030        [0., 0., 0
+0000acc0: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+0000acd0: 302e 5d5d 2c0a 2020 2020 2020 2020 2020  0.]],.          
+0000ace0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+0000acf0: 205b 5b30 2e2c 2030 2e2c 2030 2e2c 202e   [[0., 0., 0., .
+0000ad00: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d2c  .., 0., 0., 0.],
+0000ad10: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
+0000ad20: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
+0000ad30: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
+0000ad40: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+0000ad50: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+0000ad60: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
+0000ad70: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+0000ad80: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
+0000ad90: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
+0000ada0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+0000adb0: 302e 2c20 302e 2c20 302e 2c20 2e2e 2e2c  0., 0., 0., ...,
+0000adc0: 2030 2e2c 2030 2e2c 2030 2e5d 2c0a 2020   0., 0., 0.],.  
+0000add0: 2020 2020 2020 2020 2020 5b30 2e2c 2030            [0., 0
+0000ade0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
+0000adf0: 302e 2c20 302e 5d5d 5d29 0a20 2020 203e  0., 0.]]]).    >
+0000ae00: 3e3e 2072 6573 756c 7473 2e61 7667 5f64  >> results.avg_d
+0000ae10: 6570 7468 0a20 2020 207b 274b 4141 273a  epth.    {'KAA':
+0000ae20: 2031 2e33 352c 2027 4b41 4227 3a20 302e   1.35, 'KAB': 0.
+0000ae30: 3931 2c20 274b 4143 273a 2030 2e36 382c  91, 'KAC': 0.68,
+0000ae40: 2027 4b41 4427 3a20 302e 3332 2c20 274b   'KAD': 0.32, 'K
+0000ae50: 4145 273a 2030 2e39 392c 2027 4b41 4627  AE': 0.99, 'KAF'
+0000ae60: 3a20 302e 3234 2c20 274b 4147 273a 2030  : 0.24, 'KAG': 0
+0000ae70: 2e31 2c20 274b 4148 273a 2033 2e39 312c  .1, 'KAH': 3.91,
+0000ae80: 2027 4b41 4927 3a20 302e 302c 2027 4b41   'KAI': 0.0, 'KA
+0000ae90: 4a27 3a20 302e 3936 2c20 274b 414b 273a  J': 0.96, 'KAK':
+0000aea0: 2030 2e30 2c20 274b 414c 273a 2031 2e30   0.0, 'KAL': 1.0
+0000aeb0: 372c 2027 4b41 4d27 3a20 302e 3234 2c20  7, 'KAM': 0.24, 
+0000aec0: 274b 414e 273a 2030 2e30 2c20 274b 414f  'KAN': 0.0, 'KAO
+0000aed0: 273a 2030 2e32 392c 2027 4b41 5027 3a20  ': 0.29, 'KAP': 
+0000aee0: 302e 372c 2027 4b41 5127 3a20 302e 3232  0.7, 'KAQ': 0.22
+0000aef0: 2c20 274b 4152 273a 2030 2e31 327d 0a20  , 'KAR': 0.12}. 
+0000af00: 2020 203e 3e3e 2072 6573 756c 7473 2e6d     >>> results.m
+0000af10: 6178 5f64 6570 7468 0a20 2020 207b 274b  ax_depth.    {'K
+0000af20: 4141 273a 2033 2e37 392c 2027 4b41 4227  AA': 3.79, 'KAB'
+0000af30: 3a20 322e 3638 2c20 274b 4143 273a 2032  : 2.68, 'KAC': 2
+0000af40: 2e36 322c 2027 4b41 4427 3a20 302e 3835  .62, 'KAD': 0.85
+0000af50: 2c20 274b 4145 273a 2033 2e30 2c20 274b  , 'KAE': 3.0, 'K
+0000af60: 4146 273a 2030 2e38 352c 2027 4b41 4727  AF': 0.85, 'KAG'
+0000af70: 3a20 302e 362c 2027 4b41 4827 3a20 3130  : 0.6, 'KAH': 10
+0000af80: 2e37 332c 2027 4b41 4927 3a20 302e 302c  .73, 'KAI': 0.0,
+0000af90: 2027 4b41 4a27 3a20 322e 3234 2c20 274b   'KAJ': 2.24, 'K
+0000afa0: 414b 273a 2030 2e30 2c20 274b 414c 273a  AK': 0.0, 'KAL':
+0000afb0: 2033 2e30 2c20 274b 414d 273a 2031 2e32   3.0, 'KAM': 1.2
+0000afc0: 2c20 274b 414e 273a 2030 2e30 2c20 274b  , 'KAN': 0.0, 'K
+0000afd0: 414f 273a 2031 2e30 342c 2027 4b41 5027  AO': 1.04, 'KAP'
+0000afe0: 3a20 322e 3038 2c20 274b 4151 273a 2030  : 2.08, 'KAQ': 0
+0000aff0: 2e38 352c 2027 4b41 5227 3a20 302e 367d  .85, 'KAR': 0.6}
+0000b000: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
+0000b010: 2e61 7667 5f68 7964 726f 7061 7468 790a  .avg_hydropathy.
+0000b020: 2020 2020 7b27 4b41 4127 3a20 2d30 2e37      {'KAA': -0.7
+0000b030: 332c 2027 4b41 4227 3a20 2d30 2e30 352c  3, 'KAB': -0.05,
+0000b040: 2027 4b41 4327 3a20 2d30 2e30 372c 2027   'KAC': -0.07, '
+0000b050: 4b41 4427 3a20 2d30 2e36 322c 2027 4b41  KAD': -0.62, 'KA
+0000b060: 4527 3a20 2d30 2e38 312c 2027 4b41 4627  E': -0.81, 'KAF'
+0000b070: 3a20 2d30 2e31 342c 2027 4b41 4727 3a20  : -0.14, 'KAG': 
+0000b080: 2d30 2e33 332c 2027 4b41 4827 3a20 2d30  -0.33, 'KAH': -0
+0000b090: 2e31 372c 2027 4b41 4927 3a20 2d30 2e34  .17, 'KAI': -0.4
+0000b0a0: 2c20 274b 414a 273a 2030 2e36 322c 2027  , 'KAJ': 0.62, '
+0000b0b0: 4b41 4b27 3a20 2d30 2e39 392c 2027 4b41  KAK': -0.99, 'KA
+0000b0c0: 4c27 3a20 302e 3336 2c20 274b 414d 273a  L': 0.36, 'KAM':
+0000b0d0: 202d 302e 3333 2c20 274b 414e 273a 2030   -0.33, 'KAN': 0
+0000b0e0: 2e31 382c 2027 4b41 4f27 3a20 302e 3838  .18, 'KAO': 0.88
+0000b0f0: 2c20 274b 4150 273a 202d 302e 3936 2c20  , 'KAP': -0.96, 
+0000b100: 274b 4151 273a 2030 2e34 382c 2027 4b41  'KAQ': 0.48, 'KA
+0000b110: 5227 3a20 302e 3234 2c20 2745 6973 656e  R': 0.24, 'Eisen
+0000b120: 6265 7267 5765 6973 7327 3a20 5b2d 312e  bergWeiss': [-1.
+0000b130: 3432 2c20 322e 365d 7d0a 2020 2020 2222  42, 2.6]}.    ""
+0000b140: 220a 2020 2020 6966 2076 6572 626f 7365  ".    if verbose
+0000b150: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+0000b160: 223e 204c 6f61 6469 6e67 2061 746f 6d69  "> Loading atomi
+0000b170: 6320 6469 6374 696f 6e61 7279 2066 696c  c dictionary fil
+0000b180: 6522 290a 2020 2020 6966 2076 6477 2069  e").    if vdw i
+0000b190: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b1a0: 2020 2020 7664 7720 3d20 7265 6164 5f76      vdw = read_v
+0000b1b0: 6477 2876 6477 290a 2020 2020 656c 7365  dw(vdw).    else
+0000b1c0: 3a0a 2020 2020 2020 2020 7664 7720 3d20  :.        vdw = 
+0000b1d0: 7265 6164 5f76 6477 2856 4457 290a 0a20  read_vdw(VDW).. 
+0000b1e0: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0000b1f0: 2020 2020 2020 2070 7269 6e74 2822 3e20         print("> 
+0000b200: 5265 6164 696e 6720 5044 4220 636f 6f72  Reading PDB coor
+0000b210: 6469 6e61 7465 7322 290a 2020 2020 6966  dinates").    if
+0000b220: 2069 6e70 7574 2e65 6e64 7377 6974 6828   input.endswith(
+0000b230: 222e 7064 6222 293a 0a20 2020 2020 2020  ".pdb"):.       
+0000b240: 2061 746f 6d69 6320 3d20 7265 6164 5f70   atomic = read_p
+0000b250: 6462 2869 6e70 7574 2c20 7664 772c 206d  db(input, vdw, m
+0000b260: 6f64 656c 290a 2020 2020 656c 6966 2069  odel).    elif i
+0000b270: 6e70 7574 2e65 6e64 7377 6974 6828 222e  nput.endswith(".
+0000b280: 7879 7a22 293a 0a20 2020 2020 2020 2061  xyz"):.        a
+0000b290: 746f 6d69 6320 3d20 7265 6164 5f78 797a  tomic = read_xyz
+0000b2a0: 2869 6e70 7574 2c20 7664 7729 0a20 2020  (input, vdw).   
+0000b2b0: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+0000b2c0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+0000b2d0: 6074 6172 6765 7460 206d 7573 7420 6861  `target` must ha
+0000b2e0: 7665 202e 7064 6220 6f72 202e 7879 7a20  ve .pdb or .xyz 
+0000b2f0: 6578 7465 6e73 696f 6e2e 2229 0a0a 2020  extension.")..  
+0000b300: 2020 6966 206c 6967 616e 643a 0a20 2020    if ligand:.   
+0000b310: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
+0000b320: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000b330: 6e74 2822 3e20 5265 6164 696e 6720 6c69  nt("> Reading li
+0000b340: 6761 6e64 2063 6f6f 7264 696e 6174 6573  gand coordinates
+0000b350: 2229 0a20 2020 2020 2020 2069 6620 6c69  ").        if li
+0000b360: 6761 6e64 2e65 6e64 7377 6974 6828 222e  gand.endswith(".
+0000b370: 7064 6222 293a 0a20 2020 2020 2020 2020  pdb"):.         
+0000b380: 2020 206c 6174 6f6d 6963 203d 2072 6561     latomic = rea
+0000b390: 645f 7064 6228 6c69 6761 6e64 2c20 7664  d_pdb(ligand, vd
+0000b3a0: 7729 0a20 2020 2020 2020 2065 6c69 6620  w).        elif 
+0000b3b0: 6c69 6761 6e64 2e65 6e64 7377 6974 6828  ligand.endswith(
+0000b3c0: 222e 7879 7a22 293a 0a20 2020 2020 2020  ".xyz"):.       
+0000b3d0: 2020 2020 206c 6174 6f6d 6963 203d 2072       latomic = r
+0000b3e0: 6561 645f 7879 7a28 6c69 6761 6e64 2c20  ead_xyz(ligand, 
+0000b3f0: 7664 7729 0a20 2020 2020 2020 2065 6c73  vdw).        els
+0000b400: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000b410: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+0000b420: 606c 6967 616e 6460 206d 7573 7420 6861  `ligand` must ha
+0000b430: 7665 202e 7064 6220 6f72 202e 7879 7a20  ve .pdb or .xyz 
+0000b440: 6578 7465 6e73 696f 6e2e 2229 0a20 2020  extension.").   
+0000b450: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
+0000b460: 6174 6f6d 6963 203d 204e 6f6e 650a 0a20  atomic = None.. 
+0000b470: 2020 2069 6620 7665 7262 6f73 653a 0a20     if verbose:. 
+0000b480: 2020 2020 2020 2070 7269 6e74 2822 3e20         print("> 
+0000b490: 4361 6c63 756c 6174 696e 6720 3344 2067  Calculating 3D g
+0000b4a0: 7269 6420 6469 6d65 6e73 696f 6e73 2229  rid dimensions")
+0000b4b0: 0a20 2020 2069 6620 626f 783a 0a20 2020  .    if box:.   
+0000b4c0: 2020 2020 2023 2047 6574 2076 6572 7469       # Get verti
+0000b4d0: 6365 7320 6672 6f6d 2066 696c 650a 2020  ces from file.  
+0000b4e0: 2020 2020 2020 7665 7274 6963 6573 2c20        vertices, 
+0000b4f0: 6174 6f6d 6963 203d 2067 6574 5f76 6572  atomic = get_ver
+0000b500: 7469 6365 735f 6672 6f6d 5f66 696c 6528  tices_from_file(
+0000b510: 0a20 2020 2020 2020 2020 2020 2062 6f78  .            box
+0000b520: 2c20 6174 6f6d 6963 2c20 7374 6570 2c20  , atomic, step, 
+0000b530: 7072 6f62 655f 696e 2c20 7072 6f62 655f  probe_in, probe_
+0000b540: 6f75 742c 206e 7468 7265 6164 730a 2020  out, nthreads.  
+0000b550: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000b560: 2023 2053 6574 2066 6c61 6720 746f 2062   # Set flag to b
+0000b570: 6f6f 6c65 616e 0a20 2020 2020 2020 2062  oolean.        b
+0000b580: 6f78 203d 2054 7275 650a 2020 2020 656c  ox = True.    el
+0000b590: 7365 3a0a 2020 2020 2020 2020 2320 4765  se:.        # Ge
+0000b5a0: 7420 7665 7274 6963 6573 2066 726f 6d20  t vertices from 
+0000b5b0: 696e 7075 740a 2020 2020 2020 2020 7665  input.        ve
+0000b5c0: 7274 6963 6573 203d 2067 6574 5f76 6572  rtices = get_ver
+0000b5d0: 7469 6365 7328 6174 6f6d 6963 2c20 7072  tices(atomic, pr
+0000b5e0: 6f62 655f 6f75 742c 2073 7465 7029 0a0a  obe_out, step)..
+0000b5f0: 2020 2020 2020 2020 2320 5365 7420 666c          # Set fl
+0000b600: 6167 2074 6f20 626f 6f6c 6561 6e0a 2020  ag to boolean.  
+0000b610: 2020 2020 2020 626f 7820 3d20 4661 6c73        box = Fals
+0000b620: 650a 0a20 2020 2023 2043 616c 6375 6c61  e..    # Calcula
+0000b630: 7465 2064 6973 7461 6e63 6520 6265 7477  te distance betw
+0000b640: 6565 6e20 706f 696e 7473 0a20 2020 206e  een points.    n
+0000b650: 782c 206e 792c 206e 7a20 3d20 5f67 6574  x, ny, nz = _get
+0000b660: 5f64 696d 656e 7369 6f6e 7328 7665 7274  _dimensions(vert
+0000b670: 6963 6573 2c20 7374 6570 290a 2020 2020  ices, step).    
+0000b680: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+0000b690: 2020 2020 7072 696e 7428 6622 4469 6d65      print(f"Dime
+0000b6a0: 6e73 696f 6e73 3a20 286e 783a 7b6e 787d  nsions: (nx:{nx}
+0000b6b0: 2c20 6e79 3a7b 6e79 7d2c 206e 7a3a 7b6e  , ny:{ny}, nz:{n
+0000b6c0: 7a7d 2922 290a 0a20 2020 2023 2043 616c  z})")..    # Cal
+0000b6d0: 6375 6c61 7465 2073 696e 2061 6e64 2063  culate sin and c
+0000b6e0: 6f73 206f 6620 616e 676c 6573 2061 2061  os of angles a a
+0000b6f0: 6e64 2062 0a20 2020 2073 696e 636f 7320  nd b.    sincos 
+0000b700: 3d20 5f67 6574 5f73 696e 636f 7328 7665  = _get_sincos(ve
+0000b710: 7274 6963 6573 290a 2020 2020 6966 2076  rtices).    if v
+0000b720: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+0000b730: 7072 696e 7428 6622 7369 6e61 3a20 7b73  print(f"sina: {s
+0000b740: 696e 636f 735b 305d 3a2e 3266 7d5c 7473  incos[0]:.2f}\ts
+0000b750: 696e 623a 207b 7369 6e63 6f73 5b32 5d3a  inb: {sincos[2]:
+0000b760: 2e32 667d 2229 0a20 2020 2020 2020 2070  .2f}").        p
+0000b770: 7269 6e74 2866 2263 6f73 613a 207b 7369  rint(f"cosa: {si
+0000b780: 6e63 6f73 5b31 5d3a 2e32 667d 5c74 636f  ncos[1]:.2f}\tco
+0000b790: 7362 3a20 7b73 696e 636f 735b 335d 3a2e  sb: {sincos[3]:.
+0000b7a0: 3266 7d22 290a 0a20 2020 2023 2043 6176  2f}")..    # Cav
+0000b7b0: 6974 7920 6465 7465 6374 696f 6e0a 2020  ity detection.  
+0000b7c0: 2020 6e63 6176 2c20 6361 7669 7469 6573    ncav, cavities
+0000b7d0: 203d 2064 6574 6563 7428 0a20 2020 2020   = detect(.     
+0000b7e0: 2020 2061 746f 6d69 632c 0a20 2020 2020     atomic,.     
+0000b7f0: 2020 2076 6572 7469 6365 732c 0a20 2020     vertices,.   
+0000b800: 2020 2020 2073 7465 702c 0a20 2020 2020       step,.     
+0000b810: 2020 2070 726f 6265 5f69 6e2c 0a20 2020     probe_in,.   
+0000b820: 2020 2020 2070 726f 6265 5f6f 7574 2c0a       probe_out,.
+0000b830: 2020 2020 2020 2020 7265 6d6f 7661 6c5f          removal_
+0000b840: 6469 7374 616e 6365 2c0a 2020 2020 2020  distance,.      
+0000b850: 2020 766f 6c75 6d65 5f63 7574 6f66 662c    volume_cutoff,
+0000b860: 0a20 2020 2020 2020 206c 6174 6f6d 6963  .        latomic
+0000b870: 2c0a 2020 2020 2020 2020 6c69 6761 6e64  ,.        ligand
+0000b880: 5f63 7574 6f66 662c 0a20 2020 2020 2020  _cutoff,.       
+0000b890: 2062 6f78 2c0a 2020 2020 2020 2020 7375   box,.        su
+0000b8a0: 7266 6163 652c 0a20 2020 2020 2020 206e  rface,.        n
+0000b8b0: 7468 7265 6164 732c 0a20 2020 2020 2020  threads,.       
+0000b8c0: 2076 6572 626f 7365 2c0a 2020 2020 290a   verbose,.    ).
+0000b8d0: 0a20 2020 2069 6620 6e63 6176 203e 2030  .    if ncav > 0
+0000b8e0: 3a0a 2020 2020 2020 2020 2320 5370 6174  :.        # Spat
+0000b8f0: 6961 6c20 6368 6172 6163 7465 7269 7a61  ial characteriza
+0000b900: 7469 6f6e 0a20 2020 2020 2020 2073 7572  tion.        sur
+0000b910: 6661 6365 2c20 766f 6c75 6d65 2c20 6172  face, volume, ar
+0000b920: 6561 203d 2073 7061 7469 616c 2863 6176  ea = spatial(cav
+0000b930: 6974 6965 732c 2073 7465 702c 204e 6f6e  ities, step, Non
+0000b940: 652c 206e 7468 7265 6164 732c 2076 6572  e, nthreads, ver
+0000b950: 626f 7365 290a 0a20 2020 2020 2020 2023  bose)..        #
+0000b960: 2043 6f6e 7374 6974 7574 696f 6e61 6c20   Constitutional 
+0000b970: 6368 6172 6163 7465 7269 7a61 7469 6f6e  characterization
+0000b980: 0a20 2020 2020 2020 2072 6573 6964 7565  .        residue
+0000b990: 7320 3d20 636f 6e73 7469 7475 7469 6f6e  s = constitution
+0000b9a0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+0000b9b0: 6361 7669 7469 6573 2c0a 2020 2020 2020  cavities,.      
+0000b9c0: 2020 2020 2020 6174 6f6d 6963 2c0a 2020        atomic,.  
+0000b9d0: 2020 2020 2020 2020 2020 7665 7274 6963            vertic
+0000b9e0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0000b9f0: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
+0000ba00: 2020 7072 6f62 655f 696e 2c0a 2020 2020    probe_in,.    
+0000ba10: 2020 2020 2020 2020 6967 6e6f 7265 5f62          ignore_b
+0000ba20: 6163 6b62 6f6e 652c 0a20 2020 2020 2020  ackbone,.       
+0000ba30: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
+0000ba40: 2020 2020 2020 206e 7468 7265 6164 732c         nthreads,
+0000ba50: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
+0000ba60: 626f 7365 2c0a 2020 2020 2020 2020 290a  bose,.        ).
+0000ba70: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+0000ba80: 6965 7320 3d20 6361 6c63 756c 6174 655f  ies = calculate_
+0000ba90: 6672 6571 7565 6e63 6965 7328 7265 7369  frequencies(resi
+0000baa0: 6475 6573 290a 0a20 2020 2020 2020 2023  dues)..        #
+0000bab0: 2044 6570 7468 2063 6861 7261 6374 6572   Depth character
+0000bac0: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
+0000bad0: 6966 2069 6e63 6c75 6465 5f64 6570 7468  if include_depth
+0000bae0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+0000baf0: 7074 6873 2c20 6d61 785f 6465 7074 682c  pths, max_depth,
+0000bb00: 2061 7667 5f64 6570 7468 203d 2064 6570   avg_depth = dep
+0000bb10: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+0000bb20: 2020 2020 6361 7669 7469 6573 2c20 7374      cavities, st
+0000bb30: 6570 2c20 4e6f 6e65 2c20 6e74 6872 6561  ep, None, nthrea
+0000bb40: 6473 2c20 7665 7262 6f73 650a 2020 2020  ds, verbose.    
+0000bb50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000bb60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000bb70: 2020 2020 6465 7074 6873 2c20 6d61 785f      depths, max_
+0000bb80: 6465 7074 682c 2061 7667 5f64 6570 7468  depth, avg_depth
+0000bb90: 203d 204e 6f6e 652c 204e 6f6e 652c 204e   = None, None, N
+0000bba0: 6f6e 650a 0a20 2020 2020 2020 2023 2048  one..        # H
+0000bbb0: 7964 726f 7061 7468 7920 6879 6472 6f70  ydropathy hydrop
+0000bbc0: 686f 6269 6369 7479 2073 6361 6c65 730a  hobicity scales.
+0000bbd0: 2020 2020 2020 2020 6966 2069 6e63 6c75          if inclu
+0000bbe0: 6465 5f68 7964 726f 7061 7468 793a 0a20  de_hydropathy:. 
+0000bbf0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+0000bc00: 732c 2061 7667 5f68 7964 726f 7061 7468  s, avg_hydropath
+0000bc10: 7920 3d20 6879 6472 6f70 6174 6879 280a  y = hydropathy(.
+0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc30: 7375 7266 6163 652c 0a20 2020 2020 2020  surface,.       
+0000bc40: 2020 2020 2020 2020 2061 746f 6d69 632c           atomic,
+0000bc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc60: 2076 6572 7469 6365 732c 0a20 2020 2020   vertices,.     
+0000bc70: 2020 2020 2020 2020 2020 2073 7465 702c             step,
+0000bc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc90: 2070 726f 6265 5f69 6e2c 0a20 2020 2020   probe_in,.     
+0000bca0: 2020 2020 2020 2020 2020 2068 7964 726f             hydro
+0000bcb0: 7068 6f62 6963 6974 795f 7363 616c 652c  phobicity_scale,
+0000bcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bcd0: 2069 676e 6f72 655f 6261 636b 626f 6e65   ignore_backbone
+0000bce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bcf0: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
+0000bd00: 2020 2020 2020 2020 6e74 6872 6561 6473          nthreads
+0000bd10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bd20: 2020 7665 7262 6f73 652c 0a20 2020 2020    verbose,.     
+0000bd30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000bd40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000bd50: 2020 2073 6361 6c65 732c 2061 7667 5f68     scales, avg_h
+0000bd60: 7964 726f 7061 7468 7920 3d20 4e6f 6e65  ydropathy = None
+0000bd70: 2c20 4e6f 6e65 0a20 2020 2065 6c73 653a  , None.    else:
+0000bd80: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000bd90: 5761 726e 696e 673a 204e 6f20 6361 7669  Warning: No cavi
+0000bda0: 7469 6573 2064 6574 6563 7465 642c 2072  ties detected, r
+0000bdb0: 6574 7572 6e69 6e67 204e 6f6e 6521 2229  eturning None!")
+0000bdc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bdd0: 4e6f 6e65 0a0a 2020 2020 2320 5265 7475  None..    # Retu
+0000bde0: 726e 2064 6963 740a 2020 2020 7265 7375  rn dict.    resu
+0000bdf0: 6c74 7320 3d20 7079 4b56 4669 6e64 6572  lts = pyKVFinder
+0000be00: 5265 7375 6c74 7328 0a20 2020 2020 2020  Results(.       
+0000be10: 2063 6176 6974 6965 732c 0a20 2020 2020   cavities,.     
+0000be20: 2020 2073 7572 6661 6365 2c0a 2020 2020     surface,.    
+0000be30: 2020 2020 6465 7074 6873 2c0a 2020 2020      depths,.    
+0000be40: 2020 2020 7363 616c 6573 2c0a 2020 2020      scales,.    
+0000be50: 2020 2020 766f 6c75 6d65 2c0a 2020 2020      volume,.    
+0000be60: 2020 2020 6172 6561 2c0a 2020 2020 2020      area,.      
+0000be70: 2020 6d61 785f 6465 7074 682c 0a20 2020    max_depth,.   
+0000be80: 2020 2020 2061 7667 5f64 6570 7468 2c0a       avg_depth,.
+0000be90: 2020 2020 2020 2020 6176 675f 6879 6472          avg_hydr
+0000bea0: 6f70 6174 6879 2c0a 2020 2020 2020 2020  opathy,.        
+0000beb0: 7265 7369 6475 6573 2c0a 2020 2020 2020  residues,.      
+0000bec0: 2020 6672 6571 7565 6e63 6965 732c 0a20    frequencies,. 
+0000bed0: 2020 2020 2020 2076 6572 7469 6365 732c         vertices,
+0000bee0: 0a20 2020 2020 2020 2073 7465 702c 0a20  .        step,. 
+0000bef0: 2020 2020 2020 2069 6e70 7574 2c0a 2020         input,.  
+0000bf00: 2020 2020 2020 6c69 6761 6e64 2c0a 2020        ligand,.  
+0000bf10: 2020 290a 0a20 2020 2072 6574 7572 6e20    )..    return 
+0000bf20: 7265 7375 6c74 730a 0a0a 636c 6173 7320  results...class 
+0000bf30: 4d6f 6c65 6375 6c65 286f 626a 6563 7429  Molecule(object)
+0000bf40: 3a0a 2020 2020 2222 2241 2063 6c61 7373  :.    """A class
+0000bf50: 2066 6f72 2072 6570 7265 7365 6e74 696e   for representin
+0000bf60: 6720 6d6f 6c65 6375 6c61 7220 7374 7275  g molecular stru
+0000bf70: 6374 7572 6573 2e0a 0a20 2020 2050 6172  ctures...    Par
+0000bf80: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0000bf90: 2d2d 2d2d 2d2d 0a20 2020 206d 6f6c 6563  ------.    molec
+0000bfa0: 756c 6520 3a20 556e 696f 6e5b 7374 722c  ule : Union[str,
+0000bfb0: 2070 6174 686c 6962 2e50 6174 685d 0a20   pathlib.Path]. 
+0000bfc0: 2020 2020 2020 2041 2066 696c 6520 7061         A file pa
+0000bfd0: 7468 2074 6f20 7468 6520 6d6f 6c65 6375  th to the molecu
+0000bfe0: 6c65 2069 6e20 6569 7468 6572 2050 4442  le in either PDB
+0000bff0: 206f 7220 5859 5a20 666f 726d 6174 0a20   or XYZ format. 
+0000c000: 2020 2072 6164 6969 203a 2055 6e69 6f6e     radii : Union
+0000c010: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
+0000c020: 7468 2c20 4469 6374 5b73 7472 2c20 416e  th, Dict[str, An
+0000c030: 795d 5d2c 206f 7074 696f 6e61 6c0a 2020  y]], optional.  
+0000c040: 2020 2020 2020 4120 6669 6c65 2070 6174        A file pat
+0000c050: 6820 746f 2061 2076 616e 2064 6572 2057  h to a van der W
+0000c060: 6161 6c73 2072 6164 6969 2066 696c 6520  aals radii file 
+0000c070: 6f72 2061 2064 6963 7469 6f6e 6172 7920  or a dictionary 
+0000c080: 6f66 2056 4457 2072 6164 6969 2c20 6279  of VDW radii, by
+0000c090: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
+0000c0a0: 6620 4e6f 6e65 2c20 6170 706c 7920 7468  f None, apply th
+0000c0b0: 6520 6275 696c 742d 696e 2076 616e 2064  e built-in van d
+0000c0c0: 6572 2057 6161 6c73 2072 6164 6969 2066  er Waals radii f
+0000c0d0: 696c 653a 2060 7664 772e 6461 7460 2e0a  ile: `vdw.dat`..
+0000c0e0: 2020 2020 6d6f 6465 6c20 3a20 696e 742c      model : int,
+0000c0f0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000c100: 2020 5468 6520 6d6f 6465 6c20 6e75 6d62    The model numb
+0000c110: 6572 206f 6620 6120 6d75 6c74 692d 6d6f  er of a multi-mo
+0000c120: 6465 6c20 5044 4220 6669 6c65 2c20 6279  del PDB file, by
+0000c130: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
+0000c140: 6620 4e6f 6e65 2c20 6b65 6570 2061 746f  f None, keep ato
+0000c150: 6d73 2066 726f 6d20 616c 6c20 6d6f 6465  ms from all mode
+0000c160: 6c73 2e0a 2020 2020 6e74 6872 6561 6473  ls..    nthreads
+0000c170: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+0000c180: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
+0000c190: 6f66 2074 6872 6561 6473 2c20 6279 2064  of threads, by d
+0000c1a0: 6566 6175 6c74 204e 6f6e 652e 2049 6620  efault None. If 
+0000c1b0: 4e6f 6e65 2c20 7468 6520 6e75 6d62 6572  None, the number
+0000c1c0: 206f 6620 7468 7265 6164 7320 6973 2060   of threads is `
+0000c1d0: 6f73 2e63 7075 5f63 6f75 6e74 2829 202d  os.cpu_count() -
+0000c1e0: 2031 602e 0a20 2020 2076 6572 626f 7365   1`..    verbose
+0000c1f0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+0000c200: 6c0a 2020 2020 2020 2020 5072 696e 7420  l.        Print 
+0000c210: 6578 7472 6120 696e 666f 726d 6174 696f  extra informatio
+0000c220: 6e20 746f 2073 7461 6e64 6172 6420 6f75  n to standard ou
+0000c230: 7470 7574 2c20 6279 2064 6566 6175 6c74  tput, by default
+0000c240: 2046 616c 7365 2e0a 0a20 2020 2041 7474   False...    Att
+0000c250: 7269 6275 7465 730a 2020 2020 2d2d 2d2d  ributes.    ----
+0000c260: 2d2d 2d2d 2d2d 0a20 2020 205f 6174 6f6d  ------.    _atom
+0000c270: 6963 203a 206e 756d 7079 2e6e 6461 7272  ic : numpy.ndarr
+0000c280: 6179 0a20 2020 2020 2020 2041 206e 756d  ay.        A num
+0000c290: 7079 2061 7272 6179 2077 6974 6820 6174  py array with at
+0000c2a0: 6f6d 6963 2064 6174 6120 2872 6573 6964  omic data (resid
+0000c2b0: 7565 206e 756d 6265 722c 2063 6861 696e  ue number, chain
+0000c2c0: 2c20 7265 7369 6475 6520 6e61 6d65 2c20  , residue name, 
+0000c2d0: 6174 6f6d 206e 616d 652c 2078 797a 2063  atom name, xyz c
+0000c2e0: 6f6f 7264 696e 6174 6573 2061 6e64 2072  oordinates and r
+0000c2f0: 6164 6975 7329 2066 6f72 2065 6163 6820  adius) for each 
+0000c300: 6174 6f6d 2e0a 2020 2020 5f64 696d 203a  atom..    _dim :
+0000c310: 2074 7570 6c65 0a20 2020 2020 2020 2047   tuple.        G
+0000c320: 7269 6420 6469 6d65 6e73 696f 6e73 2e0a  rid dimensions..
+0000c330: 2020 2020 5f67 7269 6420 3a20 6e75 6d70      _grid : nump
+0000c340: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
+0000c350: 2020 4d6f 6c65 6375 6c65 2070 6f69 6e74    Molecule point
+0000c360: 7320 696e 2074 6865 2033 4420 6772 6964  s in the 3D grid
+0000c370: 2028 6772 6964 5b6e 785d 5b6e 795d 5b6e   (grid[nx][ny][n
+0000c380: 7a5d 292e 0a20 2020 2020 2020 2047 7269  z])..        Gri
+0000c390: 6420 6172 7261 7920 6861 7320 696e 7465  d array has inte
+0000c3a0: 6765 7220 6c61 6265 6c73 2069 6e20 6561  ger labels in ea
+0000c3b0: 6368 2070 6f73 6974 696f 6e2c 2074 6861  ch position, tha
+0000c3c0: 7420 6172 653a 0a0a 2020 2020 2020 2020  t are:..        
+0000c3d0: 2020 2020 2a20 303a 206d 6f6c 6563 756c      * 0: molecul
+0000c3e0: 6520 706f 696e 7473 3b0a 0a20 2020 2020  e points;..     
+0000c3f0: 2020 2020 2020 202a 2031 3a20 736f 6c76         * 1: solv
+0000c400: 656e 7420 706f 696e 7473 2e0a 2020 2020  ent points..    
+0000c410: 5f6d 6f6c 6563 756c 6520 3a20 556e 696f  _molecule : Unio
+0000c420: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
+0000c430: 6174 685d 0a20 2020 2020 2020 2041 2066  ath].        A f
+0000c440: 696c 6520 7061 7468 2074 6f20 7468 6520  ile path to the 
+0000c450: 6d6f 6c65 6375 6c65 2069 6e20 6569 7468  molecule in eith
+0000c460: 6572 2050 4442 206f 7220 5859 5a20 666f  er PDB or XYZ fo
+0000c470: 726d 6174 2e0a 2020 2020 5f70 6164 6469  rmat..    _paddi
+0000c480: 6e67 203a 2066 6c6f 6174 0a20 2020 2020  ng : float.     
+0000c490: 2020 2054 6865 206c 656e 6774 6820 746f     The length to
+0000c4a0: 2061 6464 2074 6f20 6561 6368 2064 6972   add to each dir
+0000c4b0: 6563 7469 6f6e 206f 6620 7468 6520 3344  ection of the 3D
+0000c4c0: 2067 7269 642e 0a20 2020 205f 7072 6f62   grid..    _prob
+0000c4d0: 6520 3a20 666c 6f61 740a 2020 2020 2020  e : float.      
+0000c4e0: 2020 5370 6865 7269 6361 6c20 7072 6f62    Spherical prob
+0000c4f0: 6520 7369 7a65 2074 6f20 6465 6669 6e65  e size to define
+0000c500: 2074 6865 206d 6f6c 6563 756c 6172 2073   the molecular s
+0000c510: 7572 6661 6365 2062 6173 6564 206f 6e20  urface based on 
+0000c520: 6120 6d6f 6c65 6375 6c61 7220 7265 7072  a molecular repr
+0000c530: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
+0000c540: 5f72 6164 6969 203a 2044 6963 745b 7374  _radii : Dict[st
+0000c550: 722c 2041 6e79 5d0a 2020 2020 2020 2020  r, Any].        
+0000c560: 4120 6469 6374 696f 6e61 7279 2063 6f6e  A dictionary con
+0000c570: 7461 696e 696e 6720 7261 6469 6920 7661  taining radii va
+0000c580: 6c75 6573 2c20 6279 2064 6566 6175 6c74  lues, by default
+0000c590: 204e 6f6e 652e 0a20 2020 205f 7265 7072   None..    _repr
+0000c5a0: 6573 656e 7461 7469 6f6e 203a 2073 7472  esentation : str
+0000c5b0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000c5c0: 2020 204d 6f6c 6563 756c 6172 2073 7572     Molecular sur
+0000c5d0: 6661 6365 2072 6570 7265 7365 6e74 6174  face representat
+0000c5e0: 696f 6e2e 204b 6579 776f 7264 7320 6f70  ion. Keywords op
+0000c5f0: 7469 6f6e 7320 6172 6520 7664 5720 2876  tions are vdW (v
+0000c600: 616e 2064 6572 2057 6161 6c73 2073 7572  an der Waals sur
+0000c610: 6661 6365 292c 2053 4553 2028 536f 6c76  face), SES (Solv
+0000c620: 656e 7420 4578 636c 7564 6564 2053 7572  ent Excluded Sur
+0000c630: 6661 6365 2920 6f72 2053 4153 2028 536f  face) or SAS (So
+0000c640: 6c76 656e 7420 4163 6365 7373 6962 6c65  lvent Accessible
+0000c650: 2053 7572 6661 6365 292c 2062 7920 6465   Surface), by de
+0000c660: 6661 756c 7420 5345 532e 0a20 2020 205f  fault SES..    _
+0000c670: 726f 7461 7469 6f6e 203a 206e 756d 7079  rotation : numpy
+0000c680: 2e6e 6461 7272 6179 0a20 2020 2020 2020  .ndarray.       
+0000c690: 2041 206e 756d 7079 2e6e 6461 7272 6179   A numpy.ndarray
+0000c6a0: 2077 6974 6820 7369 6e65 2061 6e64 2063   with sine and c
+0000c6b0: 6f73 7369 6e65 206f 6620 7468 6520 6772  ossine of the gr
+0000c6c0: 6964 2072 6f74 6174 696f 6e20 616e 676c  id rotation angl
+0000c6d0: 6573 2028 7369 6e61 2c20 636f 7361 2c20  es (sina, cosa, 
+0000c6e0: 7369 6e62 2c20 636f 7362 292e 0a20 2020  sinb, cosb)..   
+0000c6f0: 205f 7374 6570 203a 2066 6c6f 6174 0a20   _step : float. 
+0000c700: 2020 2020 2020 2047 7269 6420 7370 6163         Grid spac
+0000c710: 696e 6720 2841 292e 0a20 2020 205f 7665  ing (A)..    _ve
+0000c720: 7274 6963 6573 203a 206e 756d 7079 2e6e  rtices : numpy.n
+0000c730: 6461 7272 6179 0a20 2020 2020 2020 2041  darray.        A
+0000c740: 206e 756d 7079 2e6e 6461 7272 6179 206f   numpy.ndarray o
+0000c750: 7220 6120 6c69 7374 2077 6974 6820 7879  r a list with xy
+0000c760: 7a20 7665 7274 6963 6573 2063 6f6f 7264  z vertices coord
+0000c770: 696e 6174 6573 2028 6f72 6967 696e 2c20  inates (origin, 
+0000c780: 582d 6178 6973 2c20 592d 6178 6973 2c20  X-axis, Y-axis, 
+0000c790: 5a2d 6178 6973 292e 0a20 2020 206e 7468  Z-axis)..    nth
+0000c7a0: 7265 6164 7320 3a20 696e 740a 2020 2020  reads : int.    
+0000c7b0: 2020 2020 4e75 6d62 6572 206f 6620 7468      Number of th
+0000c7c0: 7265 6164 7320 666f 7220 7061 7261 6c6c  reads for parall
+0000c7d0: 656c 2070 726f 6365 7373 696e 672e 0a20  el processing.. 
+0000c7e0: 2020 2076 6572 626f 7365 203a 2062 6f6f     verbose : boo
+0000c7f0: 6c0a 2020 2020 2020 2020 5768 6574 6865  l.        Whethe
+0000c800: 7220 746f 2070 7269 6e74 2065 7874 7261  r to print extra
+0000c810: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
+0000c820: 7374 616e 6461 7264 206f 7574 7075 742e  standard output.
+0000c830: 0a0a 2020 2020 4e6f 7465 0a20 2020 202d  ..    Note.    -
+0000c840: 2d2d 2d0a 2020 2020 5468 6520 7661 6e20  ---.    The van 
+0000c850: 6465 7220 5761 616c 7320 7261 6469 6920  der Waals radii 
+0000c860: 6669 6c65 2064 6566 696e 6573 2074 6865  file defines the
+0000c870: 2072 6164 6975 7320 7661 6c75 6573 2066   radius values f
+0000c880: 6f72 2065 6163 6820 6174 6f6d 2062 7920  or each atom by 
+0000c890: 7265 7369 6475 6520 616e 6420 7768 656e  residue and when
+0000c8a0: 206e 6f74 2064 6566 696e 6564 2c20 6974   not defined, it
+0000c8b0: 2075 7365 7320 6120 6765 6e65 7269 6320   uses a generic 
+0000c8c0: 7661 6c75 6520 6261 7365 6420 6f6e 2074  value based on t
+0000c8d0: 6865 2061 746f 6d20 7479 7065 2e20 5468  he atom type. Th
+0000c8e0: 6520 6675 6e63 7469 6f6e 2062 7920 6465  e function by de
+0000c8f0: 6661 756c 7420 6c6f 6164 7320 7468 6520  fault loads the 
+0000c900: 6275 696c 742d 696e 2076 616e 2064 6572  built-in van der
+0000c910: 2057 6161 6c73 2072 6164 6969 2066 696c   Waals radii fil
+0000c920: 653a 2060 6076 6477 2e64 6174 6060 2e0a  e: ``vdw.dat``..
+0000c930: 0a20 2020 2053 6565 2041 6c73 6f0a 2020  .    See Also.  
+0000c940: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072    --------.    r
+0000c950: 6561 645f 7664 770a 0a20 2020 2045 7861  ead_vdw..    Exa
+0000c960: 6d70 6c65 0a20 2020 202d 2d2d 2d2d 2d2d  mple.    -------
+0000c970: 0a20 2020 2054 6865 2060 604d 6f6c 6563  .    The ``Molec
+0000c980: 756c 6560 6020 636c 6173 7320 6c6f 6164  ule`` class load
+0000c990: 7320 7468 6520 7461 7267 6574 206d 6f6c  s the target mol
+0000c9a0: 6563 756c 6172 2073 7472 7563 7475 7265  ecular structure
+0000c9b0: 2028 436c 4f34 2920 696e 746f 2070 794b   (ClO4) into pyK
+0000c9c0: 5646 696e 6465 722e 2063 6c61 7373 2e0a  VFinder. class..
+0000c9d0: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
+0000c9e0: 6f73 0a20 2020 203e 3e3e 2066 726f 6d20  os.    >>> from 
+0000c9f0: 7079 4b56 4669 6e64 6572 2069 6d70 6f72  pyKVFinder impor
+0000ca00: 7420 4d6f 6c65 6375 6c65 0a20 2020 203e  t Molecule.    >
+0000ca10: 3e3e 2070 6462 203d 206f 732e 7061 7468  >> pdb = os.path
+0000ca20: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
+0000ca30: 726e 616d 6528 7079 4b56 4669 6e64 6572  rname(pyKVFinder
+0000ca40: 2e5f 5f66 696c 655f 5f29 2c20 2764 6174  .__file__), 'dat
+0000ca50: 6127 2c20 2774 6573 7473 272c 2027 436c  a', 'tests', 'Cl
+0000ca60: 4f34 2e70 6462 2729 0a20 2020 203e 3e3e  O4.pdb').    >>>
+0000ca70: 206d 6f6c 6563 756c 6520 3d20 4d6f 6c65   molecule = Mole
+0000ca80: 6375 6c65 2870 6462 290a 2020 2020 3e3e  cule(pdb).    >>
+0000ca90: 3e20 6d6f 6c65 6375 6c65 0a20 2020 203e  > molecule.    >
+0000caa0: 3e3e 203c 7079 4b56 4669 6e64 6572 2e6d  >> <pyKVFinder.m
+0000cab0: 6169 6e2e 4d6f 6c65 6375 6c65 206f 626a  ain.Molecule obj
+0000cac0: 6563 7420 6174 2030 7837 6635 6464 6163  ect at 0x7f5ddac
+0000cad0: 6632 3233 303e 0a0a 2020 2020 5468 6520  f2230>..    The 
+0000cae0: 7661 6e20 6465 7220 5761 616c 7320 7261  van der Waals ra
+0000caf0: 6469 6920 6361 6e20 6265 2064 6566 696e  dii can be defin
+0000cb00: 6520 6279 3a0a 0a20 2020 2020 2020 202a  e by:..        *
+0000cb10: 2063 7265 6174 696e 6720 6120 5079 7468   creating a Pyth
+0000cb20: 6f6e 2064 6963 7469 6f6e 6172 793a 0a0a  on dictionary:..
+0000cb30: 2020 2020 2020 2020 3e3e 3e20 2320 5079          >>> # Py
+0000cb40: 4d4f 4c20 2876 322e 352e 3029 2076 6457  MOL (v2.5.0) vdW
+0000cb50: 2072 6164 6969 2076 616c 7565 730a 2020   radii values.  
+0000cb60: 2020 2020 2020 3e3e 3e20 7664 7720 3d20        >>> vdw = 
+0000cb70: 7b27 4745 4e27 3a20 7b27 434c 273a 2031  {'GEN': {'CL': 1
+0000cb80: 2e37 352c 2027 4f27 3a20 312e 3532 7d7d  .75, 'O': 1.52}}
+0000cb90: 0a20 2020 2020 2020 203e 3e3e 206d 6f6c  .        >>> mol
+0000cba0: 6563 756c 6520 3d20 4d6f 6c65 6375 6c65  ecule = Molecule
+0000cbb0: 2870 6462 2c20 7261 6469 693d 7664 7729  (pdb, radii=vdw)
+0000cbc0: 0a20 2020 2020 2020 203e 3e3e 206d 6f6c  .        >>> mol
+0000cbd0: 6563 756c 652e 7261 6469 690a 2020 2020  ecule.radii.    
+0000cbe0: 2020 2020 7b27 4745 4e27 3a20 7b27 434c      {'GEN': {'CL
+0000cbf0: 273a 2031 2e37 352c 2027 4f27 3a20 312e  ': 1.75, 'O': 1.
+0000cc00: 3532 7d7d 0a0a 2020 2020 2020 2020 2a20  52}}..        * 
+0000cc10: 7370 6563 6966 7969 6e67 2061 202a 2e64  specifying a *.d
+0000cc20: 6174 2a20 6669 6c65 2066 6f6c 6c6f 7769  at* file followi
+0000cc30: 6e67 2074 656d 706c 6174 6520 6f66 2060  ng template of `
+0000cc40: 7661 6e20 6465 7220 5761 616c 7320 7261  van der Waals ra
+0000cc50: 6469 6920 6669 6c65 602e 0a0a 2020 2020  dii file`...    
+0000cc60: 2020 2020 3e3e 3e20 6672 6f6d 2070 794b      >>> from pyK
+0000cc70: 5646 696e 6465 7220 696d 706f 7274 2072  VFinder import r
+0000cc80: 6561 645f 7664 770a 2020 2020 2020 2020  ead_vdw.        
+0000cc90: 3e3e 3e20 2320 4368 696d 6572 6158 2076  >>> # ChimeraX v
+0000cca0: 6457 2072 6164 6969 2076 616c 7565 730a  dW radii values.
+0000ccb0: 2020 2020 2020 2020 3e3e 3e20 7769 7468          >>> with
+0000ccc0: 206f 7065 6e28 2776 6477 2e64 6174 272c   open('vdw.dat',
+0000ccd0: 2027 7727 2920 6173 2066 3a0a 2020 2020   'w') as f:.    
+0000cce0: 2020 2020 2e2e 2e20 2020 2020 662e 7772      ...     f.wr
+0000ccf0: 6974 6528 273e 4745 4e5c 5c6e 434c 5c5c  ite('>GEN\\nCL\\
+0000cd00: 745c 5c74 312e 3938 5c5c 6e4f 5c5c 745c  t\\t1.98\\nO\\t\
+0000cd10: 5c74 312e 3436 5c5c 6e27 290a 2020 2020  \t1.46\\n').    
+0000cd20: 2020 2020 3e3e 3e20 7664 7720 3d20 7265      >>> vdw = re
+0000cd30: 6164 5f76 6477 2827 7664 772e 6461 7427  ad_vdw('vdw.dat'
+0000cd40: 290a 2020 2020 2020 2020 3e3e 3e20 6d6f  ).        >>> mo
+0000cd50: 6c65 6375 6c65 203d 204d 6f6c 6563 756c  lecule = Molecul
+0000cd60: 6528 7064 622c 2072 6164 6969 3d76 6477  e(pdb, radii=vdw
+0000cd70: 290a 2020 2020 2020 2020 3e3e 3e20 6d6f  ).        >>> mo
+0000cd80: 6c65 6375 6c65 2e72 6164 6969 0a20 2020  lecule.radii.   
+0000cd90: 2020 2020 207b 2747 454e 273a 207b 2743       {'GEN': {'C
+0000cda0: 4c27 3a20 312e 3938 2c20 274f 273a 2031  L': 1.98, 'O': 1
+0000cdb0: 2e34 367d 7d0a 2020 2020 2222 220a 0a20  .46}}.    """.. 
+0000cdc0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000cdd0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000cde0: 2020 2020 2020 206d 6f6c 6563 756c 653a         molecule:
+0000cdf0: 2055 6e69 6f6e 5b73 7472 2c20 7061 7468   Union[str, path
+0000ce00: 6c69 622e 5061 7468 5d2c 0a20 2020 2020  lib.Path],.     
+0000ce10: 2020 2072 6164 6969 3a20 556e 696f 6e5b     radii: Union[
+0000ce20: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
+0000ce30: 682c 2044 6963 745b 7374 722c 2041 6e79  h, Dict[str, Any
+0000ce40: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000ce50: 2020 206d 6f64 656c 3a20 4f70 7469 6f6e     model: Option
+0000ce60: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+0000ce70: 2020 2020 2020 2020 6e74 6872 6561 6473          nthreads
+0000ce80: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+0000ce90: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000cea0: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
+0000ceb0: 4661 6c73 652c 0a20 2020 2029 3a0a 2020  False,.    ):.  
+0000cec0: 2020 2020 2020 2222 2249 6e69 7469 616c        """Initial
+0000ced0: 697a 6520 7468 6520 4d6f 6c65 6375 6c65  ize the Molecule
+0000cee0: 206f 626a 6563 7420 7769 7468 206d 6f6c   object with mol
+0000cef0: 6563 756c 652c 2072 6164 6969 2c20 6d6f  ecule, radii, mo
+0000cf00: 6465 6c2c 206e 7468 7265 6164 7320 616e  del, nthreads an
+0000cf10: 6420 7665 7262 6f73 652e 0a0a 2020 2020  d verbose...    
+0000cf20: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000cf30: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000cf40: 2d0a 2020 2020 2020 2020 6d6f 6c65 6375  -.        molecu
+0000cf50: 6c65 203a 2055 6e69 6f6e 5b73 7472 2c20  le : Union[str, 
+0000cf60: 7061 7468 6c69 622e 5061 7468 5d0a 2020  pathlib.Path].  
+0000cf70: 2020 2020 2020 2020 2020 4120 6669 6c65            A file
+0000cf80: 2070 6174 6820 746f 2074 6865 206d 6f6c   path to the mol
+0000cf90: 6563 756c 6520 696e 2065 6974 6865 7220  ecule in either 
+0000cfa0: 5044 4220 6f72 2058 595a 2066 6f72 6d61  PDB or XYZ forma
+0000cfb0: 742e 0a20 2020 2020 2020 2072 6164 6969  t..        radii
+0000cfc0: 203a 2055 6e69 6f6e 5b73 7472 2c20 7061   : Union[str, pa
+0000cfd0: 7468 6c69 622e 5061 7468 2c20 4469 6374  thlib.Path, Dict
+0000cfe0: 5b73 7472 2c20 416e 795d 5d2c 206f 7074  [str, Any]], opt
+0000cff0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000d000: 2020 4120 6669 6c65 2070 6174 6820 746f    A file path to
+0000d010: 2061 2076 616e 2064 6572 2057 6161 6c73   a van der Waals
+0000d020: 2072 6164 6969 2066 696c 6520 6f72 2061   radii file or a
+0000d030: 2064 6963 7469 6f6e 6172 7920 6f66 2056   dictionary of V
+0000d040: 4457 2072 6164 6969 2c20 6279 2064 6566  DW radii, by def
+0000d050: 6175 6c74 204e 6f6e 652e 2049 6620 4e6f  ault None. If No
+0000d060: 6e65 2c20 6170 706c 7920 7468 6520 6275  ne, apply the bu
+0000d070: 696c 742d 696e 2076 616e 2064 6572 2057  ilt-in van der W
+0000d080: 6161 6c73 2072 6164 6969 2066 696c 653a  aals radii file:
+0000d090: 2060 7664 772e 6461 7460 2e0a 2020 2020   `vdw.dat`..    
+0000d0a0: 2020 2020 6d6f 6465 6c20 3a20 696e 742c      model : int,
+0000d0b0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000d0c0: 2020 2020 2020 5468 6520 6d6f 6465 6c20        The model 
+0000d0d0: 6e75 6d62 6572 206f 6620 6120 6d75 6c74  number of a mult
+0000d0e0: 692d 6d6f 6465 6c20 5044 4220 6669 6c65  i-model PDB file
+0000d0f0: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
+0000d100: 652e 2049 6620 4e6f 6e65 2c20 6b65 6570  e. If None, keep
+0000d110: 2061 746f 6d73 2066 726f 6d20 616c 6c20   atoms from all 
+0000d120: 6d6f 6465 6c73 2e0a 2020 2020 2020 2020  models..        
+0000d130: 6e74 6872 6561 6473 203a 2069 6e74 2c20  nthreads : int, 
+0000d140: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000d150: 2020 2020 204e 756d 6265 7220 6f66 2074       Number of t
+0000d160: 6872 6561 6473 2c20 6279 2064 6566 6175  hreads, by defau
+0000d170: 6c74 204e 6f6e 652e 2049 6620 4e6f 6e65  lt None. If None
+0000d180: 2c20 7468 6520 6e75 6d62 6572 206f 6620  , the number of 
+0000d190: 7468 7265 6164 7320 6973 2060 6f73 2e63  threads is `os.c
+0000d1a0: 7075 5f63 6f75 6e74 2829 202d 2031 602e  pu_count() - 1`.
+0000d1b0: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
+0000d1c0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+0000d1d0: 6c0a 2020 2020 2020 2020 2020 2020 5072  l.            Pr
+0000d1e0: 696e 7420 6578 7472 6120 696e 666f 726d  int extra inform
+0000d1f0: 6174 696f 6e20 746f 2073 7461 6e64 6172  ation to standar
+0000d200: 6420 6f75 7470 7574 2c20 6279 2064 6566  d output, by def
+0000d210: 6175 6c74 2046 616c 7365 2e0a 0a20 2020  ault False...   
+0000d220: 2020 2020 2052 6169 7365 730a 2020 2020       Raises.    
+0000d230: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
+0000d240: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
+0000d250: 2020 2020 2020 2020 2060 6d6f 6c65 6375           `molecu
+0000d260: 6c65 6020 6d75 7374 2062 6520 6120 7374  le` must be a st
+0000d270: 7269 6e67 206f 7220 6120 7061 7468 6c69  ring or a pathli
+0000d280: 622e 5061 7468 2e0a 2020 2020 2020 2020  b.Path..        
+0000d290: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
+0000d2a0: 2020 2020 2020 606d 6f6c 6563 756c 6560        `molecule`
+0000d2b0: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
+0000d2c0: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
+0000d2d0: 6e2e 0a20 2020 2020 2020 2054 7970 6545  n..        TypeE
+0000d2e0: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
+0000d2f0: 2060 6e74 6872 6561 6473 6020 6d75 7374   `nthreads` must
+0000d300: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
+0000d310: 6e74 6567 6572 2e0a 2020 2020 2020 2020  nteger..        
+0000d320: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
+0000d330: 2020 2020 2020 2060 6e74 6872 6561 6473         `nthreads
+0000d340: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
+0000d350: 7469 7665 2069 6e74 6567 6572 2e0a 2020  tive integer..  
+0000d360: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000d370: 2020 2023 2041 7474 7269 6275 7465 730a     # Attributes.
+0000d380: 2020 2020 2020 2020 7365 6c66 2e5f 6772          self._gr
+0000d390: 6964 203d 204e 6f6e 650a 2020 2020 2020  id = None.      
+0000d3a0: 2020 7365 6c66 2e5f 7374 6570 203d 204e    self._step = N
+0000d3b0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000d3c0: 2e5f 7061 6464 696e 6720 3d20 4e6f 6e65  ._padding = None
+0000d3d0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+0000d3e0: 726f 6265 203d 204e 6f6e 650a 2020 2020  robe = None.    
+0000d3f0: 2020 2020 7365 6c66 2e5f 7265 7072 6573      self._repres
+0000d400: 656e 7461 7469 6f6e 203d 204e 6f6e 650a  entation = None.
+0000d410: 2020 2020 2020 2020 7365 6c66 2e5f 7665          self._ve
+0000d420: 7274 6963 6573 203d 204e 6f6e 650a 2020  rtices = None.  
+0000d430: 2020 2020 2020 7365 6c66 2e5f 6469 6d20        self._dim 
+0000d440: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000d450: 656c 662e 5f72 6f74 6174 696f 6e20 3d20  elf._rotation = 
+0000d460: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000d470: 662e 7665 7262 6f73 6520 3d20 7665 7262  f.verbose = verb
+0000d480: 6f73 650a 0a20 2020 2020 2020 2023 204d  ose..        # M
+0000d490: 6f6c 6563 756c 650a 2020 2020 2020 2020  olecule.        
+0000d4a0: 6966 2074 7970 6528 6d6f 6c65 6375 6c65  if type(molecule
+0000d4b0: 2920 6e6f 7420 696e 205b 7374 722c 2070  ) not in [str, p
+0000d4c0: 6174 686c 6962 2e50 6174 685d 3a0a 2020  athlib.Path]:.  
+0000d4d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d4e0: 5479 7065 4572 726f 7228 2260 6d6f 6c65  TypeError("`mole
+0000d4f0: 6375 6c65 6020 6d75 7374 2062 6520 6120  cule` must be a 
+0000d500: 7374 7269 6e67 206f 7220 6120 7061 7468  string or a path
+0000d510: 6c69 622e 5061 7468 2e22 290a 2020 2020  lib.Path.").    
+0000d520: 2020 2020 7365 6c66 2e5f 6d6f 6c65 6375      self._molecu
+0000d530: 6c65 203d 206f 732e 7061 7468 2e72 6561  le = os.path.rea
+0000d540: 6c70 6174 6828 6d6f 6c65 6375 6c65 290a  lpath(molecule).
+0000d550: 0a20 2020 2020 2020 2023 2076 616e 2064  .        # van d
+0000d560: 6572 2057 6161 6c73 2072 6164 6969 0a20  er Waals radii. 
+0000d570: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+0000d580: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+0000d590: 2020 2020 7072 696e 7428 223e 204c 6f61      print("> Loa
+0000d5a0: 6469 6e67 2076 616e 2064 6572 2057 6161  ding van der Waa
+0000d5b0: 6c73 2072 6164 6969 2229 0a20 2020 2020  ls radii").     
+0000d5c0: 2020 2069 6620 7261 6469 6920 6973 204e     if radii is N
+0000d5d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d5e0: 2023 2064 6566 6175 6c74 0a20 2020 2020   # default.     
+0000d5f0: 2020 2020 2020 2073 656c 662e 5f72 6164         self._rad
+0000d600: 6969 203d 2072 6561 645f 7664 7728 5644  ii = read_vdw(VD
+0000d610: 5729 0a20 2020 2020 2020 2065 6c69 6620  W).        elif 
+0000d620: 7479 7065 2872 6164 6969 2920 696e 205b  type(radii) in [
+0000d630: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
+0000d640: 685d 3a0a 2020 2020 2020 2020 2020 2020  h]:.            
+0000d650: 2320 7664 7720 6669 6c65 0a20 2020 2020  # vdw file.     
+0000d660: 2020 2020 2020 2073 656c 662e 5f72 6164         self._rad
+0000d670: 6969 203d 2072 6561 645f 7664 7728 7261  ii = read_vdw(ra
+0000d680: 6469 6929 0a20 2020 2020 2020 2065 6c69  dii).        eli
+0000d690: 6620 7479 7065 2872 6164 6969 2920 696e  f type(radii) in
+0000d6a0: 205b 6469 6374 5d3a 0a20 2020 2020 2020   [dict]:.       
+0000d6b0: 2020 2020 2023 2050 726f 6365 7373 6564       # Processed
+0000d6c0: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
+0000d6d0: 2020 2020 2020 2020 7365 6c66 2e5f 7261          self._ra
+0000d6e0: 6469 6920 3d20 7261 6469 690a 0a20 2020  dii = radii..   
+0000d6f0: 2020 2020 2023 2041 746f 6d69 6320 696e       # Atomic in
+0000d700: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
+0000d710: 2020 6966 2073 656c 662e 7665 7262 6f73    if self.verbos
+0000d720: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+0000d730: 7269 6e74 2822 3e20 5265 6164 696e 6720  rint("> Reading 
+0000d740: 6d6f 6c65 6375 6c65 2063 6f6f 7264 696e  molecule coordin
+0000d750: 6174 6573 2229 0a20 2020 2020 2020 2069  ates").        i
+0000d760: 6620 6d6f 6c65 6375 6c65 2e65 6e64 7377  f molecule.endsw
+0000d770: 6974 6828 222e 7064 6222 293a 0a20 2020  ith(".pdb"):.   
+0000d780: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+0000d790: 746f 6d69 6320 3d20 7265 6164 5f70 6462  tomic = read_pdb
+0000d7a0: 286d 6f6c 6563 756c 652c 2073 656c 662e  (molecule, self.
+0000d7b0: 7261 6469 692c 206d 6f64 656c 290a 2020  radii, model).  
+0000d7c0: 2020 2020 2020 656c 6966 206d 6f6c 6563        elif molec
+0000d7d0: 756c 652e 656e 6473 7769 7468 2822 2e78  ule.endswith(".x
+0000d7e0: 797a 2229 3a0a 2020 2020 2020 2020 2020  yz"):.          
+0000d7f0: 2020 7365 6c66 2e5f 6174 6f6d 6963 203d    self._atomic =
+0000d800: 2072 6561 645f 7879 7a28 6d6f 6c65 6375   read_xyz(molecu
+0000d810: 6c65 2c20 7365 6c66 2e72 6164 6969 290a  le, self.radii).
+0000d820: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000d830: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d840: 5479 7065 4572 726f 7228 2260 6d6f 6c65  TypeError("`mole
+0000d850: 6375 6c65 6020 6d75 7374 2068 6176 6520  cule` must have 
+0000d860: 2e70 6462 206f 7220 2e78 797a 2065 7874  .pdb or .xyz ext
+0000d870: 656e 7369 6f6e 2e22 290a 0a20 2020 2020  ension.")..     
+0000d880: 2020 2023 204e 756d 6265 7220 6f66 2074     # Number of t
+0000d890: 6872 6561 6473 0a20 2020 2020 2020 2069  hreads.        i
+0000d8a0: 6620 6e74 6872 6561 6473 2069 7320 6e6f  f nthreads is no
+0000d8b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000d8c0: 2020 2020 6966 2074 7970 6528 6e74 6872      if type(nthr
+0000d8d0: 6561 6473 2920 6e6f 7420 696e 205b 696e  eads) not in [in
+0000d8e0: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
+0000d8f0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+0000d900: 726f 7228 2260 6e74 6872 6561 6473 6020  ror("`nthreads` 
+0000d910: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+0000d920: 7665 2069 6e74 6567 6572 2e22 290a 2020  ve integer.").  
+0000d930: 2020 2020 2020 2020 2020 656c 6966 206e            elif n
+0000d940: 7468 7265 6164 7320 3c3d 2030 3a0a 2020  threads <= 0:.  
+0000d950: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000d960: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0000d970: 606e 7468 7265 6164 7360 206d 7573 7420  `nthreads` must 
+0000d980: 6265 2061 2070 6f73 6974 6976 6520 696e  be a positive in
+0000d990: 7465 6765 722e 2229 0a20 2020 2020 2020  teger.").       
+0000d9a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000d9b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d9c0: 6e74 6872 6561 6473 203d 206e 7468 7265  nthreads = nthre
+0000d9d0: 6164 730a 2020 2020 2020 2020 656c 7365  ads.        else
+0000d9e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000d9f0: 6c66 2e6e 7468 7265 6164 7320 3d20 6f73  lf.nthreads = os
+0000da00: 2e63 7075 5f63 6f75 6e74 2829 202d 2031  .cpu_count() - 1
+0000da10: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000da20: 2020 2020 6465 6620 6174 6f6d 6963 2873      def atomic(s
+0000da30: 656c 6629 202d 3e20 6e75 6d70 792e 6e64  elf) -> numpy.nd
+0000da40: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
+0000da50: 2222 4765 7420 5f61 746f 6d69 6320 6174  ""Get _atomic at
+0000da60: 7472 6962 7574 652e 2222 220a 2020 2020  tribute.""".    
+0000da70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000da80: 5f61 746f 6d69 630a 0a20 2020 2040 7072  _atomic..    @pr
+0000da90: 6f70 6572 7479 0a20 2020 2064 6566 2064  operty.    def d
+0000daa0: 696d 2873 656c 6629 202d 3e20 5475 706c  im(self) -> Tupl
+0000dab0: 655b 696e 742c 2069 6e74 2c20 696e 745d  e[int, int, int]
+0000dac0: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000dad0: 205f 6469 6d20 6174 7472 6962 7574 6522   _dim attribute"
+0000dae0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000daf0: 6e20 7365 6c66 2e5f 6469 6d0a 0a20 2020  n self._dim..   
+0000db00: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000db10: 6566 2067 7269 6428 7365 6c66 2920 2d3e  ef grid(self) ->
+0000db20: 206e 756d 7079 2e6e 6461 7272 6179 3a0a   numpy.ndarray:.
+0000db30: 2020 2020 2020 2020 2222 2247 6574 205f          """Get _
+0000db40: 6772 6964 2061 7474 7269 6275 7465 2e22  grid attribute."
+0000db50: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000db60: 6e20 7365 6c66 2e5f 6772 6964 0a0a 2020  n self._grid..  
+0000db70: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000db80: 6465 6620 6d6f 6c65 6375 6c65 2873 656c  def molecule(sel
+0000db90: 6629 202d 3e20 556e 696f 6e5b 7374 722c  f) -> Union[str,
+0000dba0: 2070 6174 686c 6962 2e50 6174 685d 3a0a   pathlib.Path]:.
+0000dbb0: 2020 2020 2020 2020 2222 2247 6574 205f          """Get _
+0000dbc0: 6d6f 6c65 6375 6c65 2061 7474 7269 6275  molecule attribu
+0000dbd0: 7465 2e22 2222 0a20 2020 2020 2020 2072  te.""".        r
+0000dbe0: 6574 7572 6e20 7365 6c66 2e5f 6d6f 6c65  eturn self._mole
+0000dbf0: 6375 6c65 0a0a 2020 2020 4070 726f 7065  cule..    @prope
+0000dc00: 7274 790a 2020 2020 6465 6620 6e78 2873  rty.    def nx(s
+0000dc10: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0000dc20: 2020 2020 2022 2222 4765 7420 6772 6964       """Get grid
+0000dc30: 2075 6e69 7473 2069 6e20 582d 6178 6973   units in X-axis
+0000dc40: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+0000dc50: 7365 6c66 2e5f 6469 6d20 6973 206e 6f74  self._dim is not
+0000dc60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000dc70: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000dc80: 6469 6d5b 305d 0a0a 2020 2020 4070 726f  dim[0]..    @pro
+0000dc90: 7065 7274 790a 2020 2020 6465 6620 6e79  perty.    def ny
+0000dca0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+0000dcb0: 2020 2020 2020 2022 2222 4765 7420 6772         """Get gr
+0000dcc0: 6964 2075 6e69 7473 2069 6e20 592d 6178  id units in Y-ax
+0000dcd0: 6973 2e22 2222 0a20 2020 2020 2020 2069  is.""".        i
+0000dce0: 6620 7365 6c66 2e5f 6469 6d20 6973 206e  f self._dim is n
+0000dcf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000dd00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000dd10: 2e5f 6469 6d5b 315d 0a0a 2020 2020 4070  ._dim[1]..    @p
+0000dd20: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000dd30: 6e7a 2873 656c 6629 202d 3e20 696e 743a  nz(self) -> int:
+0000dd40: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+0000dd50: 6772 6964 2075 6e69 7473 2069 6e20 5a2d  grid units in Z-
+0000dd60: 6178 6973 2e22 2222 0a20 2020 2020 2020  axis.""".       
+0000dd70: 2069 6620 7365 6c66 2e5f 6469 6d20 6973   if self._dim is
+0000dd80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000dd90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000dda0: 6c66 2e5f 6469 6d5b 325d 0a0a 2020 2020  lf._dim[2]..    
+0000ddb0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000ddc0: 6620 7031 2873 656c 6629 202d 3e20 6e75  f p1(self) -> nu
+0000ddd0: 6d70 792e 6e64 6172 7261 793a 0a20 2020  mpy.ndarray:.   
+0000dde0: 2020 2020 2022 2222 4765 7420 6f72 6967       """Get orig
+0000ddf0: 696e 206f 6620 7468 6520 3344 2067 7269  in of the 3D gri
+0000de00: 642e 2222 220a 2020 2020 2020 2020 6966  d.""".        if
+0000de10: 2073 656c 662e 5f76 6572 7469 6365 7320   self._vertices 
+0000de20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000de30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000de40: 7365 6c66 2e5f 7665 7274 6963 6573 5b30  self._vertices[0
+0000de50: 5d0a 0a20 2020 2040 7072 6f70 6572 7479  ]..    @property
+0000de60: 0a20 2020 2064 6566 2070 3228 7365 6c66  .    def p2(self
+0000de70: 2920 2d3e 206e 756d 7079 2e6e 6461 7272  ) -> numpy.ndarr
+0000de80: 6179 3a0a 2020 2020 2020 2020 2222 2247  ay:.        """G
+0000de90: 6574 2058 2d61 7869 7320 6d61 7820 6f66  et X-axis max of
+0000dea0: 2074 6865 2033 4420 6772 6964 2e22 2222   the 3D grid."""
+0000deb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000dec0: 2e5f 7665 7274 6963 6573 2069 7320 6e6f  ._vertices is no
+0000ded0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000dee0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000def0: 5f76 6572 7469 6365 735b 315d 0a0a 2020  _vertices[1]..  
+0000df00: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000df10: 6465 6620 7033 2873 656c 6629 202d 3e20  def p3(self) -> 
+0000df20: 6e75 6d70 792e 6e64 6172 7261 793a 0a20  numpy.ndarray:. 
+0000df30: 2020 2020 2020 2022 2222 4765 7420 592d         """Get Y-
+0000df40: 6178 6973 206d 6178 206f 6620 7468 6520  axis max of the 
+0000df50: 3344 2067 7269 642e 2222 220a 2020 2020  3D grid.""".    
+0000df60: 2020 2020 6966 2073 656c 662e 5f76 6572      if self._ver
+0000df70: 7469 6365 7320 6973 206e 6f74 204e 6f6e  tices is not Non
+0000df80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000df90: 6574 7572 6e20 7365 6c66 2e5f 7665 7274  eturn self._vert
+0000dfa0: 6963 6573 5b32 5d0a 0a20 2020 2040 7072  ices[2]..    @pr
+0000dfb0: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
+0000dfc0: 3428 7365 6c66 2920 2d3e 206e 756d 7079  4(self) -> numpy
+0000dfd0: 2e6e 6461 7272 6179 3a0a 2020 2020 2020  .ndarray:.      
+0000dfe0: 2020 2222 2247 6574 205a 2d61 7869 7320    """Get Z-axis 
+0000dff0: 6d61 7820 6f66 2074 6865 2033 4420 6772  max of the 3D gr
+0000e000: 6964 2e22 2222 0a20 2020 2020 2020 2069  id.""".        i
+0000e010: 6620 7365 6c66 2e5f 7665 7274 6963 6573  f self._vertices
+0000e020: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000e030: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e040: 2073 656c 662e 5f76 6572 7469 6365 735b   self._vertices[
+0000e050: 335d 0a0a 2020 2020 4070 726f 7065 7274  3]..    @propert
+0000e060: 790a 2020 2020 6465 6620 7061 6464 696e  y.    def paddin
+0000e070: 6728 7365 6c66 2920 2d3e 2066 6c6f 6174  g(self) -> float
+0000e080: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000e090: 205f 7061 6464 696e 6720 6174 7472 6962   _padding attrib
+0000e0a0: 7574 652e 2222 220a 2020 2020 2020 2020  ute.""".        
+0000e0b0: 7265 7475 726e 2073 656c 662e 5f70 6164  return self._pad
+0000e0c0: 6469 6e67 0a0a 2020 2020 4070 726f 7065  ding..    @prope
+0000e0d0: 7274 790a 2020 2020 6465 6620 7072 6f62  rty.    def prob
+0000e0e0: 6528 7365 6c66 2920 2d3e 2066 6c6f 6174  e(self) -> float
+0000e0f0: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000e100: 205f 7072 6f62 6520 6174 7472 6962 7574   _probe attribut
+0000e110: 652e 2222 220a 2020 2020 2020 2020 7265  e.""".        re
+0000e120: 7475 726e 2073 656c 662e 5f70 726f 6265  turn self._probe
+0000e130: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000e140: 2020 2020 6465 6620 7261 6469 6928 7365      def radii(se
+0000e150: 6c66 2920 2d3e 2044 6963 745b 7374 722c  lf) -> Dict[str,
+0000e160: 2041 6e79 5d3a 0a20 2020 2020 2020 2022   Any]:.        "
+0000e170: 2222 4765 7420 5f72 6164 6969 2061 7474  ""Get _radii att
+0000e180: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
+0000e190: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000e1a0: 7261 6469 690a 0a20 2020 2040 7072 6f70  radii..    @prop
+0000e1b0: 6572 7479 0a20 2020 2064 6566 2072 6570  erty.    def rep
+0000e1c0: 7265 7365 6e74 6174 696f 6e28 7365 6c66  resentation(self
+0000e1d0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+0000e1e0: 2020 2222 2247 6574 205f 7265 7072 6573    """Get _repres
+0000e1f0: 656e 7461 7469 6f6e 2061 7474 7269 6275  entation attribu
+0000e200: 7465 2e22 2222 0a20 2020 2020 2020 2072  te.""".        r
+0000e210: 6574 7572 6e20 7365 6c66 2e5f 7265 7072  eturn self._repr
+0000e220: 6573 656e 7461 7469 6f6e 0a0a 2020 2020  esentation..    
+0000e230: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000e240: 6620 726f 7461 7469 6f6e 2873 656c 6629  f rotation(self)
+0000e250: 202d 3e20 6e75 6d70 792e 6e64 6172 7261   -> numpy.ndarra
+0000e260: 793a 0a20 2020 2020 2020 2022 2222 4765  y:.        """Ge
+0000e270: 7420 5f72 6f74 6174 696f 6e20 6174 7472  t _rotation attr
+0000e280: 6962 7574 652e 2222 220a 2020 2020 2020  ibute.""".      
+0000e290: 2020 7265 7475 726e 2073 656c 662e 5f72    return self._r
+0000e2a0: 6f74 6174 696f 6e0a 0a20 2020 2040 7072  otation..    @pr
+0000e2b0: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
+0000e2c0: 7465 7028 7365 6c66 2920 2d3e 2066 6c6f  tep(self) -> flo
+0000e2d0: 6174 3a0a 2020 2020 2020 2020 2222 2247  at:.        """G
+0000e2e0: 6574 205f 7374 6570 2061 7474 7269 6275  et _step attribu
+0000e2f0: 7465 2e22 2222 0a20 2020 2020 2020 2069  te.""".        i
+0000e300: 6620 7365 6c66 2e5f 7374 6570 2069 7320  f self._step is 
+0000e310: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000e320: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000e330: 662e 5f73 7465 700a 0a20 2020 2040 7072  f._step..    @pr
+0000e340: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
+0000e350: 6572 7469 6365 7328 7365 6c66 2920 2d3e  ertices(self) ->
+0000e360: 206e 756d 7079 2e6e 6461 7272 6179 3a0a   numpy.ndarray:.
+0000e370: 2020 2020 2020 2020 2222 2247 6574 205f          """Get _
+0000e380: 7665 7274 6963 6573 2061 7474 7269 6275  vertices attribu
+0000e390: 7465 2e22 2222 0a20 2020 2020 2020 2072  te.""".        r
+0000e3a0: 6574 7572 6e20 7365 6c66 2e5f 7665 7274  eturn self._vert
+0000e3b0: 6963 6573 0a0a 2020 2020 4070 726f 7065  ices..    @prope
+0000e3c0: 7274 790a 2020 2020 6465 6620 7879 7a72  rty.    def xyzr
+0000e3d0: 2873 656c 6629 202d 3e20 6e75 6d70 792e  (self) -> numpy.
+0000e3e0: 6e64 6172 7261 793a 0a20 2020 2020 2020  ndarray:.       
+0000e3f0: 2022 2222 4765 7420 7879 7a20 636f 6f72   """Get xyz coor
+0000e400: 6469 6e61 7465 7320 616e 6420 7261 6469  dinates and radi
+0000e410: 7573 206f 6620 6d6f 6c65 6375 6c65 2061  us of molecule a
+0000e420: 746f 6d73 2e22 2222 0a20 2020 2020 2020  toms.""".       
+0000e430: 2072 6574 7572 6e20 7365 6c66 2e5f 6174   return self._at
+0000e440: 6f6d 6963 5b3a 2c20 343a 5d2e 6173 7479  omic[:, 4:].asty
+0000e450: 7065 286e 756d 7079 2e66 6c6f 6174 3634  pe(numpy.float64
+0000e460: 290a 0a20 2020 2064 6566 205f 7365 745f  )..    def _set_
+0000e470: 6772 6964 2873 656c 662c 2070 6164 6469  grid(self, paddi
+0000e480: 6e67 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ng: Optional[flo
+0000e490: 6174 5d20 3d20 4e6f 6e65 2920 2d3e 204e  at] = None) -> N
+0000e4a0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000e4b0: 4465 6669 6e65 2074 6865 2033 4420 6772  Define the 3D gr
+0000e4c0: 6964 2066 6f72 2074 6865 2074 6172 6765  id for the targe
+0000e4d0: 7420 6d6f 6c65 6375 6c65 2e0a 0a20 2020  t molecule...   
+0000e4e0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000e4f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000e500: 2d2d 0a20 2020 2020 2020 2070 6164 6469  --.        paddi
+0000e510: 6e67 203a 2066 6c6f 6174 2c20 6f70 7469  ng : float, opti
+0000e520: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0000e530: 2054 6865 206c 656e 6774 6820 746f 2061   The length to a
+0000e540: 6464 2074 6f20 6561 6368 2064 6972 6563  dd to each direc
+0000e550: 7469 6f6e 206f 6620 7468 6520 3344 2067  tion of the 3D g
+0000e560: 7269 642c 2062 7920 6465 6661 756c 7420  rid, by default 
+0000e570: 4e6f 6e65 2e20 4966 204e 6f6e 652c 2061  None. If None, a
+0000e580: 7574 6f6d 6174 6963 616c 6c79 2064 6566  utomatically def
+0000e590: 696e 6520 7468 6520 6c65 6e67 7468 2062  ine the length b
+0000e5a0: 6173 6564 206f 6e20 6d6f 6c65 6375 6c65  ased on molecule
+0000e5b0: 2063 6f6f 7264 696e 6174 6573 2c20 7072   coordinates, pr
+0000e5c0: 6f62 6520 7369 7a65 2c20 6772 6964 2073  obe size, grid s
+0000e5d0: 7061 6369 6e67 2061 6e64 2061 746f 6d20  pacing and atom 
+0000e5e0: 7261 6469 692e 0a0a 2020 2020 2020 2020  radii...        
+0000e5f0: 5261 6973 6573 0a20 2020 2020 2020 202d  Raises.        -
+0000e600: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5479  -----.        Ty
+0000e610: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+0000e620: 2020 2020 6070 6164 6469 6e67 6020 6d75      `padding` mu
+0000e630: 7374 2062 6520 6120 6e6f 6e2d 6e65 6761  st be a non-nega
+0000e640: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
+0000e650: 2e0a 2020 2020 2020 2020 5661 6c75 6545  ..        ValueE
+0000e660: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
+0000e670: 2060 7061 6464 696e 6760 206d 7573 7420   `padding` must 
+0000e680: 6265 2061 206e 6f6e 2d6e 6567 6174 6976  be a non-negativ
+0000e690: 6520 7265 616c 206e 756d 6265 722e 0a20  e real number.. 
+0000e6a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e6b0: 2020 2023 2050 6164 6469 6e67 0a20 2020     # Padding.   
+0000e6c0: 2020 2020 2069 6620 7061 6464 696e 6720       if padding 
+0000e6d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000e6e0: 2020 2020 2020 2020 2069 6620 7479 7065           if type
+0000e6f0: 2870 6164 6469 6e67 2920 6e6f 7420 696e  (padding) not in
+0000e700: 205b 696e 742c 2066 6c6f 6174 5d3a 0a20   [int, float]:. 
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000e720: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+0000e730: 6070 6164 6469 6e67 6020 6d75 7374 2062  `padding` must b
+0000e740: 6520 6120 6e6f 6e2d 6e65 6761 7469 7665  e a non-negative
+0000e750: 2072 6561 6c20 6e75 6d62 6572 2e22 290a   real number.").
+0000e760: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000e770: 2070 6164 6469 6e67 203c 2030 2e30 3a0a   padding < 0.0:.
+0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e790: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000e7a0: 2822 6070 6164 6469 6e67 6020 6d75 7374  ("`padding` must
+0000e7b0: 2062 6520 6120 6e6f 6e2d 6e65 6761 7469   be a non-negati
+0000e7c0: 7665 2072 6561 6c20 6e75 6d62 6572 2e22  ve real number."
+0000e7d0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000e7e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000e7f0: 2020 2020 7365 6c66 2e5f 7061 6464 696e      self._paddin
+0000e800: 6720 3d20 7061 6464 696e 670a 2020 2020  g = padding.    
+0000e810: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000e820: 2020 2020 2020 7365 6c66 2e5f 7061 6464        self._padd
+0000e830: 696e 6720 3d20 7365 6c66 2e5f 6765 745f  ing = self._get_
+0000e840: 7061 6464 696e 6728 290a 0a20 2020 2020  padding()..     
+0000e850: 2020 2023 2033 4420 6772 6964 0a20 2020     # 3D grid.   
+0000e860: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
+0000e870: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+0000e880: 2020 7072 696e 7428 223e 2043 616c 6375    print("> Calcu
+0000e890: 6c61 7469 6e67 2033 4420 6772 6964 2229  lating 3D grid")
+0000e8a0: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
+0000e8b0: 6572 7469 6365 7320 3d20 6765 745f 7665  ertices = get_ve
+0000e8c0: 7274 6963 6573 2873 656c 662e 6174 6f6d  rtices(self.atom
+0000e8d0: 6963 2c20 7365 6c66 2e70 6164 6469 6e67  ic, self.padding
+0000e8e0: 2c20 7365 6c66 2e73 7465 7029 0a20 2020  , self.step).   
+0000e8f0: 2020 2020 2073 656c 662e 5f64 696d 203d       self._dim =
+0000e900: 205f 6765 745f 6469 6d65 6e73 696f 6e73   _get_dimensions
+0000e910: 2873 656c 662e 7665 7274 6963 6573 2c20  (self.vertices, 
+0000e920: 7365 6c66 2e73 7465 7029 0a20 2020 2020  self.step).     
+0000e930: 2020 2073 656c 662e 5f72 6f74 6174 696f     self._rotatio
+0000e940: 6e20 3d20 5f67 6574 5f73 696e 636f 7328  n = _get_sincos(
+0000e950: 7365 6c66 2e76 6572 7469 6365 7329 0a20  self.vertices). 
+0000e960: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+0000e970: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+0000e980: 2020 2020 7072 696e 7428 6622 7031 3a20      print(f"p1: 
+0000e990: 7b73 656c 662e 7665 7274 6963 6573 5b30  {self.vertices[0
+0000e9a0: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+0000e9b0: 2070 7269 6e74 2866 2270 323a 207b 7365   print(f"p2: {se
+0000e9c0: 6c66 2e76 6572 7469 6365 735b 315d 7d22  lf.vertices[1]}"
+0000e9d0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+0000e9e0: 696e 7428 6622 7033 3a20 7b73 656c 662e  int(f"p3: {self.
+0000e9f0: 7665 7274 6963 6573 5b32 5d7d 2229 0a20  vertices[2]}"). 
+0000ea00: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000ea10: 2866 2270 343a 207b 7365 6c66 2e76 6572  (f"p4: {self.ver
+0000ea20: 7469 6365 735b 335d 7d22 290a 2020 2020  tices[3]}").    
+0000ea30: 2020 2020 2020 2020 7072 696e 7428 226e          print("n
+0000ea40: 783a 207b 7d2c 206e 793a 207b 7d2c 206e  x: {}, ny: {}, n
+0000ea50: 7a3a 207b 7d22 2e66 6f72 6d61 7428 2a73  z: {}".format(*s
+0000ea60: 656c 662e 6469 6d29 290a 2020 2020 2020  elf.dim)).      
+0000ea70: 2020 2020 2020 7072 696e 7428 2273 696e        print("sin
+0000ea80: 613a 207b 7d2c 2073 696e 623a 207b 7d2c  a: {}, sinb: {},
+0000ea90: 2063 6f73 613a 207b 7d2c 2063 6f73 623a   cosa: {}, cosb:
+0000eaa0: 207b 7d22 2e66 6f72 6d61 7428 2a73 656c   {}".format(*sel
+0000eab0: 662e 726f 7461 7469 6f6e 2929 0a0a 2020  f.rotation))..  
+0000eac0: 2020 6465 6620 5f67 6574 5f70 6164 6469    def _get_paddi
+0000ead0: 6e67 2873 656c 6629 202d 3e20 666c 6f61  ng(self) -> floa
+0000eae0: 743a 0a20 2020 2020 2020 2022 2222 4175  t:.        """Au
+0000eaf0: 746f 6d61 7469 6361 6c6c 7920 6465 6669  tomatically defi
+0000eb00: 6e65 2074 6865 2070 6164 6469 6e67 2062  ne the padding b
+0000eb10: 6173 6564 206f 6e20 6d6f 6c65 6375 6c65  ased on molecule
+0000eb20: 2063 6f6f 7264 696e 6174 6573 2c20 7072   coordinates, pr
+0000eb30: 6f62 6520 7369 7a65 2c20 6772 6964 2073  obe size, grid s
+0000eb40: 7061 6369 6e67 2061 6e64 2061 746f 6d20  pacing and atom 
+0000eb50: 7261 6469 692e 0a0a 2020 2020 2020 2020  radii...        
+0000eb60: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000eb70: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000eb80: 7061 6464 696e 6720 3a20 666c 6f61 740a  padding : float.
+0000eb90: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000eba0: 6c65 6e67 7468 2074 6f20 6164 6420 746f  length to add to
+0000ebb0: 2065 6163 6820 6469 7265 6374 696f 6e20   each direction 
+0000ebc0: 6f66 2074 6865 2033 4420 6772 6964 2e0a  of the 3D grid..
+0000ebd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000ebe0: 2020 2020 7061 6464 696e 6720 3d20 312e      padding = 1.
+0000ebf0: 3120 2a20 7365 6c66 2e78 797a 725b 3a2c  1 * self.xyzr[:,
+0000ec00: 2033 5d2e 6d61 7828 290a 2020 2020 2020   3].max().      
+0000ec10: 2020 6966 2073 656c 662e 7265 7072 6573    if self.repres
+0000ec20: 656e 7461 7469 6f6e 2069 6e20 5b22 5345  entation in ["SE
+0000ec30: 5322 2c20 2253 4153 225d 3a0a 2020 2020  S", "SAS"]:.    
+0000ec40: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
+0000ec50: 2b3d 2073 656c 662e 5f70 726f 6265 0a20  += self._probe. 
+0000ec60: 2020 2020 2020 2072 6574 7572 6e20 666c         return fl
+0000ec70: 6f61 7428 7061 6464 696e 672e 726f 756e  oat(padding.roun
+0000ec80: 6428 6465 6369 6d61 6c73 3d31 2929 0a0a  d(decimals=1))..
+0000ec90: 2020 2020 6465 6620 7664 7728 7365 6c66      def vdw(self
+0000eca0: 2c20 7374 6570 3a20 666c 6f61 7420 3d20  , step: float = 
+0000ecb0: 302e 362c 2070 6164 6469 6e67 3a20 4f70  0.6, padding: Op
+0000ecc0: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
+0000ecd0: 4e6f 6e65 2920 2d3e 204e 6f6e 653a 0a20  None) -> None:. 
+0000ece0: 2020 2020 2020 2022 2222 4669 6c6c 2074         """Fill t
+0000ecf0: 6865 2033 4420 6772 6964 2077 6974 6820  he 3D grid with 
+0000ed00: 7468 6520 6d6f 6c65 6375 6c65 2061 7320  the molecule as 
+0000ed10: 7468 6520 7661 6e20 6465 7220 5761 616c  the van der Waal
+0000ed20: 7320 7375 7266 6163 6520 7265 7072 6573  s surface repres
+0000ed30: 656e 7461 7469 6f6e 2e0a 0a20 2020 2020  entation...     
+0000ed40: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000ed50: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000ed60: 0a20 2020 2020 2020 2073 7465 7020 3a20  .        step : 
+0000ed70: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+0000ed80: 2020 2020 2020 2020 2020 2020 4772 6964              Grid
+0000ed90: 2073 7061 6369 6e67 2028 4129 2c20 6279   spacing (A), by
+0000eda0: 2064 6566 6175 6c74 2030 2e36 2e0a 2020   default 0.6..  
+0000edb0: 2020 2020 2020 7061 6464 696e 6720 3a20        padding : 
+0000edc0: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+0000edd0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000ede0: 6c65 6e67 7468 2074 6f20 6164 6420 746f  length to add to
+0000edf0: 2065 6163 6820 6469 7265 6374 696f 6e20   each direction 
+0000ee00: 6f66 2074 6865 2033 4420 6772 6964 2c20  of the 3D grid, 
+0000ee10: 6279 2064 6566 6175 6c74 204e 6f6e 652e  by default None.
+0000ee20: 2049 6620 4e6f 6e65 2c20 6175 746f 6d61   If None, automa
+0000ee30: 7469 6361 6c6c 7920 6465 6669 6e65 2074  tically define t
+0000ee40: 6865 206c 656e 6774 6820 6261 7365 6420  he length based 
+0000ee50: 6f6e 206d 6f6c 6563 756c 6520 636f 6f72  on molecule coor
+0000ee60: 6469 6e61 7465 732c 2070 726f 6265 2073  dinates, probe s
+0000ee70: 697a 652c 2067 7269 6420 7370 6163 696e  ize, grid spacin
+0000ee80: 6720 616e 6420 6174 6f6d 2072 6164 6969  g and atom radii
+0000ee90: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+0000eea0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000eeb0: 0a20 2020 2020 2020 2054 7970 6545 7272  .        TypeErr
+0000eec0: 6f72 0a20 2020 2020 2020 2020 2020 2060  or.            `
+0000eed0: 7374 6570 6020 6d75 7374 2062 6520 6120  step` must be a 
+0000eee0: 706f 7369 7469 7665 2072 6561 6c20 6e75  positive real nu
+0000eef0: 6d62 6572 2e0a 2020 2020 2020 2020 5661  mber..        Va
+0000ef00: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
+0000ef10: 2020 2020 2060 7374 6570 6020 6d75 7374       `step` must
+0000ef20: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
+0000ef30: 6561 6c20 6e75 6d62 6572 2e0a 0a20 2020  eal number...   
+0000ef40: 2020 2020 2045 7861 6d70 6c65 0a20 2020       Example.   
+0000ef50: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000ef60: 2020 2020 2054 6865 2060 604d 6f6c 6563       The ``Molec
+0000ef70: 756c 652e 7664 7728 2960 6020 6d65 7468  ule.vdw()`` meth
+0000ef80: 6f64 2074 616b 6573 2061 2067 7269 6420  od takes a grid 
+0000ef90: 7370 6163 696e 6720 616e 6420 7265 7475  spacing and retu
+0000efa0: 726e 7320 6120 4e75 6d50 7920 6172 7261  rns a NumPy arra
+0000efb0: 7920 7769 7468 2074 6865 206d 6f6c 6563  y with the molec
+0000efc0: 756c 6520 706f 696e 7473 2072 6570 7265  ule points repre
+0000efd0: 7365 6e74 696e 6720 7468 6520 7664 5720  senting the vdW 
+0000efe0: 7375 7266 6163 6520 696e 2074 6865 2033  surface in the 3
+0000eff0: 4420 6772 6964 2e0a 0a20 2020 2020 2020  D grid...       
+0000f000: 203e 3e3e 2023 2047 7269 6420 5370 6163   >>> # Grid Spac
+0000f010: 696e 6720 2873 7465 7029 3a20 302e 310a  ing (step): 0.1.
+0000f020: 2020 2020 2020 2020 3e3e 3e20 7374 6570          >>> step
+0000f030: 203d 2030 2e31 0a20 2020 2020 2020 203e   = 0.1.        >
+0000f040: 3e3e 206d 6f6c 6563 756c 652e 7664 7728  >> molecule.vdw(
+0000f050: 7374 6570 3d73 7465 7029 0a20 2020 2020  step=step).     
+0000f060: 2020 203e 3e3e 206d 6f6c 6563 756c 652e     >>> molecule.
+0000f070: 6772 6964 0a20 2020 2020 2020 2061 7272  grid.        arr
+0000f080: 6179 285b 5b5b 312c 2031 2c20 312c 202e  ay([[[1, 1, 1, .
+0000f090: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+0000f0b0: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+0000f0c0: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+0000f0d0: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+0000f0e0: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
+0000f110: 2020 2020 205b 312c 2031 2c20 312c 202e       [1, 1, 1, .
+0000f120: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
+0000f130: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+0000f140: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+0000f150: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+0000f160: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+0000f170: 202e 2e2e 2c20 312c 2031 2c20 315d 5d2c   ..., 1, 1, 1]],
+0000f180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f190: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
+0000f1a0: 2020 2020 5b5b 312c 2031 2c20 312c 202e      [[1, 1, 1, .
+0000f1b0: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
+0000f1c0: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+0000f1d0: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+0000f1e0: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+0000f1f0: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+0000f200: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
+0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f220: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
+0000f230: 2020 2020 205b 312c 2031 2c20 312c 202e       [1, 1, 1, .
+0000f240: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
+0000f250: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+0000f260: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+0000f270: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+0000f280: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+0000f290: 202e 2e2e 2c20 312c 2031 2c20 315d 5d5d   ..., 1, 1, 1]]]
+0000f2a0: 2c20 6474 7970 653d 696e 7433 3229 0a20  , dtype=int32). 
+0000f2b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f2c0: 2020 2066 726f 6d20 5f70 794b 5646 696e     from _pyKVFin
+0000f2d0: 6465 7220 696d 706f 7274 205f 6669 6c6c  der import _fill
+0000f2e0: 5f72 6563 6570 746f 720a 0a20 2020 2020  _receptor..     
+0000f2f0: 2020 2023 2043 6865 636b 2061 7267 756d     # Check argum
+0000f300: 656e 7473 0a20 2020 2020 2020 2069 6620  ents.        if 
+0000f310: 7479 7065 2873 7465 7029 206e 6f74 2069  type(step) not i
+0000f320: 6e20 5b69 6e74 2c20 666c 6f61 745d 3a0a  n [int, float]:.
+0000f330: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000f340: 6520 5479 7065 4572 726f 7228 2260 7374  e TypeError("`st
+0000f350: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
+0000f360: 7374 6976 6520 7265 616c 206e 756d 6265  stive real numbe
+0000f370: 722e 2229 0a20 2020 2020 2020 2065 6c69  r.").        eli
+0000f380: 6620 7374 6570 203c 3d20 302e 303a 0a20  f step <= 0.0:. 
+0000f390: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f3a0: 2056 616c 7565 4572 726f 7228 2260 7374   ValueError("`st
+0000f3b0: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
+0000f3c0: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
+0000f3d0: 6572 2e22 290a 2020 2020 2020 2020 656c  er.").        el
+0000f3e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000f3f0: 7365 6c66 2e5f 7374 6570 203d 2073 7465  self._step = ste
+0000f400: 700a 0a20 2020 2020 2020 2023 2041 7474  p..        # Att
+0000f410: 7269 6275 7465 730a 2020 2020 2020 2020  ributes.        
+0000f420: 7365 6c66 2e5f 7265 7072 6573 656e 7461  self._representa
+0000f430: 7469 6f6e 203d 2022 7664 5722 0a20 2020  tion = "vdW".   
+0000f440: 2020 2020 2073 656c 662e 5f70 726f 6265       self._probe
+0000f450: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0000f460: 2023 2044 6566 696e 6520 3344 2067 7269   # Define 3D gri
+0000f470: 640a 2020 2020 2020 2020 7365 6c66 2e5f  d.        self._
+0000f480: 7365 745f 6772 6964 2870 6164 6469 6e67  set_grid(padding
+0000f490: 290a 0a20 2020 2020 2020 2023 2076 616e  )..        # van
+0000f4a0: 2064 6572 2057 6161 6c73 2061 746f 6d73   der Waals atoms
+0000f4b0: 2028 6861 7264 2073 7068 6572 6520 6d6f   (hard sphere mo
+0000f4c0: 6465 6c29 2074 6f20 6772 6964 0a20 2020  del) to grid.   
+0000f4d0: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
+0000f4e0: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+0000f4f0: 2020 7072 696e 7428 223e 2049 6e73 6572    print("> Inser
+0000f500: 7469 6e67 2061 746f 6d73 2077 6974 6820  ting atoms with 
+0000f510: 7661 6e20 6465 7220 5761 616c 7320 7261  van der Waals ra
+0000f520: 6469 6920 696e 746f 2033 4420 6772 6964  dii into 3D grid
+0000f530: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000f540: 5f67 7269 6420 3d20 5f66 696c 6c5f 7265  _grid = _fill_re
+0000f550: 6365 7074 6f72 280a 2020 2020 2020 2020  ceptor(.        
+0000f560: 2020 2020 7365 6c66 2e6e 7820 2a20 7365      self.nx * se
+0000f570: 6c66 2e6e 7920 2a20 7365 6c66 2e6e 7a2c  lf.ny * self.nz,
+0000f580: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f590: 662e 6e78 2c0a 2020 2020 2020 2020 2020  f.nx,.          
+0000f5a0: 2020 7365 6c66 2e6e 792c 0a20 2020 2020    self.ny,.     
+0000f5b0: 2020 2020 2020 2073 656c 662e 6e7a 2c0a         self.nz,.
+0000f5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f5d0: 2e78 797a 722c 0a20 2020 2020 2020 2020  .xyzr,.         
+0000f5e0: 2020 2073 656c 662e 7031 2c0a 2020 2020     self.p1,.    
+0000f5f0: 2020 2020 2020 2020 7365 6c66 2e72 6f74          self.rot
+0000f600: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
+0000f610: 2020 2073 656c 662e 7374 6570 2c0a 2020     self.step,.  
+0000f620: 2020 2020 2020 2020 2020 302e 302c 0a20            0.0,. 
+0000f630: 2020 2020 2020 2020 2020 2046 616c 7365             False
+0000f640: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+0000f650: 6c66 2e6e 7468 7265 6164 732c 0a20 2020  lf.nthreads,.   
+0000f660: 2020 2020 2020 2020 2073 656c 662e 7665           self.ve
+0000f670: 7262 6f73 652c 0a20 2020 2020 2020 2029  rbose,.        )
+0000f680: 2e72 6573 6861 7065 2873 656c 662e 6e78  .reshape(self.nx
+0000f690: 2c20 7365 6c66 2e6e 792c 2073 656c 662e  , self.ny, self.
+0000f6a0: 6e7a 290a 0a20 2020 2064 6566 2073 7572  nz)..    def sur
+0000f6b0: 6661 6365 280a 2020 2020 2020 2020 7365  face(.        se
+0000f6c0: 6c66 2c0a 2020 2020 2020 2020 7374 6570  lf,.        step
+0000f6d0: 3a20 666c 6f61 7420 3d20 302e 362c 0a20  : float = 0.6,. 
+0000f6e0: 2020 2020 2020 2070 726f 6265 3a20 666c         probe: fl
+0000f6f0: 6f61 7420 3d20 312e 342c 0a20 2020 2020  oat = 1.4,.     
+0000f700: 2020 2073 7572 6661 6365 3a20 7374 7220     surface: str 
+0000f710: 3d20 2253 4553 222c 0a20 2020 2020 2020  = "SES",.       
+0000f720: 2070 6164 6469 6e67 3a20 4f70 7469 6f6e   padding: Option
+0000f730: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+0000f740: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+0000f750: 0a20 2020 2020 2020 2022 2222 4669 6c6c  .        """Fill
+0000f760: 2074 6865 2033 4420 6772 6964 2077 6974   the 3D grid wit
+0000f770: 6820 7468 6520 6d6f 6c65 6375 6c65 2061  h the molecule a
+0000f780: 7320 7468 6520 7661 6e20 6465 7220 5761  s the van der Wa
+0000f790: 616c 7320 7375 7266 6163 6520 7265 7072  als surface repr
+0000f7a0: 6573 656e 7461 7469 6f6e 2e0a 0a20 2020  esentation...   
+0000f7b0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000f7c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000f7d0: 2d2d 0a20 2020 2020 2020 2073 7465 7020  --.        step 
+0000f7e0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+0000f7f0: 6c0a 2020 2020 2020 2020 2020 2020 4772  l.            Gr
+0000f800: 6964 2073 7061 6369 6e67 2028 4129 2c20  id spacing (A), 
+0000f810: 6279 2064 6566 6175 6c74 2030 2e36 2e0a  by default 0.6..
+0000f820: 2020 2020 2020 2020 7072 6f62 6520 3a20          probe : 
+0000f830: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+0000f840: 2020 2020 2020 2020 2020 2020 5370 6865              Sphe
+0000f850: 7269 6361 6c20 7072 6f62 6520 7369 7a65  rical probe size
+0000f860: 2074 6f20 6465 6669 6e65 2074 6865 206d   to define the m
+0000f870: 6f6c 6563 756c 6172 2073 7572 6661 6365  olecular surface
+0000f880: 2062 6173 6564 206f 6e20 6120 6d6f 6c65   based on a mole
+0000f890: 6375 6c61 7220 7265 7072 6573 656e 7461  cular representa
+0000f8a0: 7469 6f6e 2c20 6279 2064 6566 6175 6c74  tion, by default
+0000f8b0: 2031 2e34 2e0a 2020 2020 2020 2020 7375   1.4..        su
+0000f8c0: 7266 6163 6520 3a20 7374 722c 206f 7074  rface : str, opt
+0000f8d0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000f8e0: 2020 4d6f 6c65 6375 6c61 7220 7375 7266    Molecular surf
+0000f8f0: 6163 6520 7265 7072 6573 656e 7461 7469  ace representati
+0000f900: 6f6e 2e20 4b65 7977 6f72 6473 206f 7074  on. Keywords opt
+0000f910: 696f 6e73 2061 7265 2076 6457 2028 7661  ions are vdW (va
+0000f920: 6e20 6465 7220 5761 616c 7320 7375 7266  n der Waals surf
+0000f930: 6163 6529 2c20 5345 5320 2853 6f6c 7665  ace), SES (Solve
+0000f940: 6e74 2045 7863 6c75 6465 6420 5375 7266  nt Excluded Surf
+0000f950: 6163 6529 206f 7220 5341 5320 2853 6f6c  ace) or SAS (Sol
+0000f960: 7665 6e74 2041 6363 6573 7369 626c 6520  vent Accessible 
+0000f970: 5375 7266 6163 6529 2c20 6279 2064 6566  Surface), by def
+0000f980: 6175 6c74 2022 5345 5322 2e0a 2020 2020  ault "SES"..    
+0000f990: 2020 2020 7061 6464 696e 6720 3a20 666c      padding : fl
+0000f9a0: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
+0000f9b0: 2020 2020 2020 2020 2020 5468 6520 6c65            The le
+0000f9c0: 6e67 7468 2074 6f20 6164 6420 746f 2065  ngth to add to e
+0000f9d0: 6163 6820 6469 7265 6374 696f 6e20 6f66  ach direction of
+0000f9e0: 2074 6865 2033 4420 6772 6964 2c20 6279   the 3D grid, by
+0000f9f0: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
+0000fa00: 6620 4e6f 6e65 2c20 6175 746f 6d61 7469  f None, automati
+0000fa10: 6361 6c6c 7920 6465 6669 6e65 2074 6865  cally define the
+0000fa20: 206c 656e 6774 6820 6261 7365 6420 6f6e   length based on
+0000fa30: 206d 6f6c 6563 756c 6520 636f 6f72 6469   molecule coordi
+0000fa40: 6e61 7465 732c 2070 726f 6265 2073 697a  nates, probe siz
+0000fa50: 652c 2067 7269 6420 7370 6163 696e 6720  e, grid spacing 
+0000fa60: 616e 6420 6174 6f6d 2072 6164 6969 2e0a  and atom radii..
+0000fa70: 0a20 2020 2020 2020 2052 6169 7365 730a  .        Raises.
+0000fa80: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
+0000fa90: 2020 2020 2020 2054 7970 6545 7272 6f72         TypeError
+0000faa0: 0a20 2020 2020 2020 2020 2020 2060 7374  .            `st
+0000fab0: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
+0000fac0: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
+0000fad0: 6572 2e0a 2020 2020 2020 2020 5661 6c75  er..        Valu
+0000fae0: 6545 7272 6f72 0a20 2020 2020 2020 2020  eError.         
+0000faf0: 2020 2060 7374 6570 6020 6d75 7374 2062     `step` must b
+0000fb00: 6520 6120 706f 7369 7469 7665 2072 6561  e a positive rea
+0000fb10: 6c20 6e75 6d62 6572 2e0a 2020 2020 2020  l number..      
+0000fb20: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
+0000fb30: 2020 2020 2020 2020 6070 726f 6265 5f6f          `probe_o
+0000fb40: 7574 6020 6d75 7374 2062 6520 6120 706f  ut` must be a po
+0000fb50: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
+0000fb60: 6572 2e0a 2020 2020 2020 2020 5661 6c75  er..        Valu
+0000fb70: 6545 7272 6f72 0a20 2020 2020 2020 2020  eError.         
+0000fb80: 2020 2060 7072 6f62 655f 6f75 7460 206d     `probe_out` m
+0000fb90: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
+0000fba0: 6520 7265 616c 206e 756d 6265 722e 0a0a  e real number...
+0000fbb0: 2020 2020 2020 2020 4578 616d 706c 650a          Example.
+0000fbc0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000fbd0: 2020 2020 2020 2020 5468 6520 6060 4d6f          The ``Mo
+0000fbe0: 6c65 6375 6c65 2e73 7572 6661 6365 2829  lecule.surface()
+0000fbf0: 6060 206d 6574 686f 6420 7461 6b65 7320  `` method takes 
+0000fc00: 7468 6520 6772 6964 2073 7061 6369 6e67  the grid spacing
+0000fc10: 2c20 7468 6520 7370 6865 7269 6361 6c20  , the spherical 
+0000fc20: 7072 6f62 6520 7369 7a65 2074 6f20 6d6f  probe size to mo
+0000fc30: 6465 6c20 7468 6520 7375 7266 6163 652c  del the surface,
+0000fc40: 2074 6865 2073 7572 6661 6365 2072 6570   the surface rep
+0000fc50: 7265 7365 6e74 6174 696f 6e20 616e 6420  resentation and 
+0000fc60: 7265 7475 726e 7320 6120 4e75 6d50 7920  returns a NumPy 
+0000fc70: 6172 7261 7920 7769 7468 2074 6865 206d  array with the m
+0000fc80: 6f6c 6563 756c 6520 706f 696e 7473 2072  olecule points r
+0000fc90: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+0000fca0: 5345 5320 696e 2074 6865 2033 4420 6772  SES in the 3D gr
+0000fcb0: 6964 2e0a 0a20 2020 2020 2020 2054 6865  id...        The
+0000fcc0: 206d 6f6c 6563 756c 6172 2073 7572 6661   molecular surfa
+0000fcd0: 6365 2063 616e 2062 6520 6d6f 6465 6c6c  ce can be modell
+0000fce0: 6564 2061 733a 0a0a 2020 2020 2020 2020  ed as:..        
+0000fcf0: 2020 2020 2a20 536f 6c76 656e 7420 4578      * Solvent Ex
+0000fd00: 636c 7564 6564 2053 7572 6661 6365 2028  cluded Surface (
+0000fd10: 5345 5329 3a0a 0a20 2020 2020 2020 2020  SES):..         
+0000fd20: 2020 203e 3e3e 2023 2053 7572 6661 6365     >>> # Surface
+0000fd30: 2052 6570 7265 7365 6e74 6174 696f 6e3a   Representation:
+0000fd40: 2053 4553 0a20 2020 2020 2020 2020 2020   SES.           
+0000fd50: 203e 3e3e 2073 7572 6661 6365 203d 2027   >>> surface = '
+0000fd60: 5345 5327 0a20 2020 2020 2020 2020 2020  SES'.           
+0000fd70: 203e 3e3e 2023 2047 7269 6420 5370 6163   >>> # Grid Spac
+0000fd80: 696e 6720 2873 7465 7029 3a20 302e 310a  ing (step): 0.1.
+0000fd90: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+0000fda0: 7374 6570 203d 2030 2e31 0a20 2020 2020  step = 0.1.     
+0000fdb0: 2020 2020 2020 203e 3e3e 2023 2053 7068         >>> # Sph
+0000fdc0: 6572 6963 616c 2050 726f 6265 2028 7072  erical Probe (pr
+0000fdd0: 6f62 6529 3a20 312e 340a 2020 2020 2020  obe): 1.4.      
+0000fde0: 2020 2020 2020 3e3e 3e20 7072 6f62 6520        >>> probe 
+0000fdf0: 3d20 312e 340a 2020 2020 2020 2020 2020  = 1.4.          
+0000fe00: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 2e73    >>> molecule.s
+0000fe10: 7572 6661 6365 2873 7465 703d 7374 6570  urface(step=step
+0000fe20: 2c20 7072 6f62 653d 7072 6f62 652c 2073  , probe=probe, s
+0000fe30: 7572 6661 6365 3d73 7572 6661 6365 290a  urface=surface).
+0000fe40: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+0000fe50: 6d6f 6c65 6375 6c65 2e67 7269 640a 2020  molecule.grid.  
+0000fe60: 2020 2020 2020 2020 2020 6172 7261 7928            array(
+0000fe70: 5b5b 5b31 2c20 312c 2031 2c20 2e2e 2e2c  [[[1, 1, 1, ...,
+0000fe80: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000fea0: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000feb0: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
+0000fec0: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+0000fed0: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+0000fee0: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
+0000fef0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+0000ff00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff10: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
+0000ff20: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
+0000ff30: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000ff40: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000ff50: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
+0000ff60: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+0000ff70: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+0000ff80: 2031 5d5d 2c0a 2020 2020 2020 2020 2020   1]],.          
+0000ff90: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+0000ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffb0: 205b 5b31 2c20 312c 2031 2c20 2e2e 2e2c   [[1, 1, 1, ...,
+0000ffc0: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
+0000ffd0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000ffe0: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000fff0: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
+00010000: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+00010010: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+00010020: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
+00010030: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010050: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
+00010060: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
+00010070: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00010080: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+00010090: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
+000100a0: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+000100b0: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+000100c0: 2031 5d5d 5d2c 2064 7479 7065 3d69 6e74   1]]], dtype=int
+000100d0: 3332 290a 0a20 2020 2020 2020 2054 6865  32)..        The
+000100e0: 206d 6f6c 6563 756c 6172 2073 7572 6661   molecular surfa
+000100f0: 6365 2063 616e 2062 6520 6d6f 6465 6c6c  ce can be modell
+00010100: 6564 2061 733a 0a0a 2020 2020 2020 2020  ed as:..        
+00010110: 2020 2020 2a20 536f 6c76 656e 7420 4163      * Solvent Ac
+00010120: 6365 7373 6962 6c65 2053 7572 6661 6365  cessible Surface
+00010130: 2028 5341 5329 3a0a 0a20 2020 2020 2020   (SAS):..       
+00010140: 2020 2020 203e 3e3e 2023 2053 7572 6661       >>> # Surfa
+00010150: 6365 2052 6570 7265 7365 6e74 6174 696f  ce Representatio
+00010160: 6e3a 2053 4153 0a20 2020 2020 2020 2020  n: SAS.         
+00010170: 2020 203e 3e3e 2073 7572 6661 6365 203d     >>> surface =
+00010180: 2027 5341 5327 0a20 2020 2020 2020 2020   'SAS'.         
+00010190: 2020 203e 3e3e 2023 2047 7269 6420 5370     >>> # Grid Sp
+000101a0: 6163 696e 6720 2873 7465 7029 3a20 302e  acing (step): 0.
+000101b0: 310a 2020 2020 2020 2020 2020 2020 3e3e  1.            >>
+000101c0: 3e20 7374 6570 203d 2030 2e31 0a20 2020  > step = 0.1.   
+000101d0: 2020 2020 2020 2020 203e 3e3e 2023 2053           >>> # S
+000101e0: 7068 6572 6963 616c 2050 726f 6265 2028  pherical Probe (
+000101f0: 7072 6f62 6529 3a20 312e 340a 2020 2020  probe): 1.4.    
+00010200: 2020 2020 2020 2020 3e3e 3e20 7072 6f62          >>> prob
+00010210: 6520 3d20 312e 340a 2020 2020 2020 2020  e = 1.4.        
+00010220: 2020 2020 3e3e 3e20 6d6f 6c65 6375 6c65      >>> molecule
+00010230: 2e73 7572 6661 6365 2873 7465 703d 7374  .surface(step=st
+00010240: 6570 2c20 7072 6f62 653d 7072 6f62 652c  ep, probe=probe,
+00010250: 2073 7572 6661 6365 3d73 7572 6661 6365   surface=surface
+00010260: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00010270: 3e20 6d6f 6c65 6375 6c65 2e67 7269 640a  > molecule.grid.
+00010280: 2020 2020 2020 2020 2020 2020 6172 7261              arra
+00010290: 7928 5b5b 5b31 2c20 312c 2031 2c20 2e2e  y([[[1, 1, 1, ..
+000102a0: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
+000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102c0: 205b 312c 2031 2c20 312c 202e 2e2e 2c20   [1, 1, 1, ..., 
+000102d0: 312c 2031 2c20 315d 2c0a 2020 2020 2020  1, 1, 1],.      
+000102e0: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+000102f0: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+00010300: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+00010310: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010330: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
+00010340: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 205b 312c 2031 2c20 312c 202e 2e2e 2c20   [1, 1, 1, ..., 
+00010370: 312c 2031 2c20 315d 2c0a 2020 2020 2020  1, 1, 1],.      
+00010380: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+00010390: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+000103a0: 312c 2031 5d5d 2c0a 2020 2020 2020 2020  1, 1]],.        
+000103b0: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103d0: 2020 205b 5b31 2c20 312c 2031 2c20 2e2e     [[1, 1, 1, ..
+000103e0: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
+000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010400: 205b 312c 2031 2c20 312c 202e 2e2e 2c20   [1, 1, 1, ..., 
+00010410: 312c 2031 2c20 315d 2c0a 2020 2020 2020  1, 1, 1],.      
+00010420: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+00010430: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+00010440: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+00010450: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010470: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
+00010480: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
+00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104a0: 205b 312c 2031 2c20 312c 202e 2e2e 2c20   [1, 1, 1, ..., 
+000104b0: 312c 2031 2c20 315d 2c0a 2020 2020 2020  1, 1, 1],.      
+000104c0: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
+000104d0: 2c20 312c 2031 2c20 2e2e 2e2c 2031 2c20  , 1, 1, ..., 1, 
+000104e0: 312c 2031 5d5d 5d2c 2064 7479 7065 3d69  1, 1]]], dtype=i
+000104f0: 6e74 3332 290a 2020 2020 2020 2020 2222  nt32).        ""
+00010500: 220a 2020 2020 2020 2020 6672 6f6d 205f  ".        from _
+00010510: 7079 4b56 4669 6e64 6572 2069 6d70 6f72  pyKVFinder impor
+00010520: 7420 5f66 696c 6c5f 7265 6365 7074 6f72  t _fill_receptor
+00010530: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
+00010540: 6b20 6172 6775 6d65 6e74 730a 2020 2020  k arguments.    
+00010550: 2020 2020 6966 2074 7970 6528 7374 6570      if type(step
+00010560: 2920 6e6f 7420 696e 205b 696e 742c 2066  ) not in [int, f
+00010570: 6c6f 6174 5d3a 0a20 2020 2020 2020 2020  loat]:.         
+00010580: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00010590: 6f72 2822 6073 7465 7060 206d 7573 7420  or("`step` must 
+000105a0: 6265 2061 2070 6f73 7469 7665 2072 6561  be a postive rea
+000105b0: 6c20 6e75 6d62 6572 2e22 290a 2020 2020  l number.").    
+000105c0: 2020 2020 656c 6966 2073 7465 7020 3c3d      elif step <=
+000105d0: 2030 2e30 3a0a 2020 2020 2020 2020 2020   0.0:.          
+000105e0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000105f0: 6f72 2822 6073 7465 7060 206d 7573 7420  or("`step` must 
+00010600: 6265 2061 2070 6f73 6974 6976 6520 7265  be a positive re
+00010610: 616c 206e 756d 6265 722e 2229 0a20 2020  al number.").   
+00010620: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010630: 2020 2020 2020 2073 656c 662e 5f73 7465         self._ste
+00010640: 7020 3d20 7374 6570 0a0a 2020 2020 2020  p = step..      
+00010650: 2020 2320 5072 6f62 650a 2020 2020 2020    # Probe.      
+00010660: 2020 6966 2074 7970 6528 7072 6f62 6529    if type(probe)
+00010670: 206e 6f74 2069 6e20 5b69 6e74 2c20 666c   not in [int, fl
+00010680: 6f61 742c 206e 756d 7079 2e66 6c6f 6174  oat, numpy.float
+00010690: 3634 5d3a 0a20 2020 2020 2020 2020 2020  64]:.           
+000106a0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000106b0: 2822 6070 726f 6265 5f6f 7574 6020 6d75  ("`probe_out` mu
+000106c0: 7374 2062 6520 6120 6e6f 6e2d 6e65 6761  st be a non-nega
+000106d0: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
+000106e0: 2e22 290a 2020 2020 2020 2020 656c 6966  .").        elif
+000106f0: 2070 726f 6265 203c 3d20 302e 303a 0a20   probe <= 0.0:. 
+00010700: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00010710: 2056 616c 7565 4572 726f 7228 2260 7072   ValueError("`pr
+00010720: 6f62 655f 6f75 7460 206d 7573 7420 6265  obe_out` must be
+00010730: 2061 206e 6f6e 2d6e 6567 6174 6976 6520   a non-negative 
+00010740: 7265 616c 206e 756d 6265 722e 2229 0a20  real number."). 
+00010750: 2020 2020 2020 2073 656c 662e 5f70 726f         self._pro
+00010760: 6265 203d 2070 726f 6265 0a0a 2020 2020  be = probe..    
+00010770: 2020 2020 2320 5375 7266 6163 650a 2020      # Surface.  
+00010780: 2020 2020 2020 6966 2073 7572 6661 6365        if surface
+00010790: 203d 3d20 2253 4553 223a 0a20 2020 2020   == "SES":.     
+000107a0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+000107b0: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+000107c0: 2020 2020 2020 2020 7072 696e 7428 223e          print(">
+000107d0: 2053 7572 6661 6365 2072 6570 7265 7365   Surface represe
+000107e0: 6e74 6174 696f 6e3a 2053 6f6c 7665 6e74  ntation: Solvent
+000107f0: 2045 7863 6c75 6465 6420 5375 7266 6163   Excluded Surfac
+00010800: 6520 2853 4553 292e 2229 0a20 2020 2020  e (SES).").     
+00010810: 2020 2020 2020 2073 656c 662e 5f72 6570         self._rep
+00010820: 7265 7365 6e74 6174 696f 6e20 3d20 7375  resentation = su
+00010830: 7266 6163 650a 2020 2020 2020 2020 2020  rface.          
+00010840: 2020 7375 7266 6163 6520 3d20 5472 7565    surface = True
+00010850: 0a20 2020 2020 2020 2065 6c69 6620 7375  .        elif su
+00010860: 7266 6163 6520 3d3d 2022 5341 5322 3a0a  rface == "SAS":.
+00010870: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010880: 656c 662e 7665 7262 6f73 653a 0a20 2020  elf.verbose:.   
+00010890: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000108a0: 6e74 2822 3e20 5375 7266 6163 6520 7265  nt("> Surface re
+000108b0: 7072 6573 656e 7461 7469 6f6e 3a20 536f  presentation: So
+000108c0: 6c76 656e 7420 4163 6365 7373 6962 6c65  lvent Accessible
+000108d0: 2053 7572 6661 6365 2028 5341 5329 2e22   Surface (SAS)."
+000108e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000108f0: 6c66 2e5f 7265 7072 6573 656e 7461 7469  lf._representati
+00010900: 6f6e 203d 2073 7572 6661 6365 0a20 2020  on = surface.   
+00010910: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+00010920: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00010930: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00010940: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00010950: 726f 7228 6622 6073 7572 6661 6365 6020  ror(f"`surface` 
+00010960: 6d75 7374 2062 6520 5341 5320 6f72 2053  must be SAS or S
+00010970: 4553 2c20 6e6f 7420 7b73 7572 6661 6365  ES, not {surface
+00010980: 7d2e 2229 0a0a 2020 2020 2020 2020 2320  }.")..        # 
+00010990: 4465 6669 6e65 2033 4420 6772 6964 0a20  Define 3D grid. 
+000109a0: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
+000109b0: 5f67 7269 6428 7061 6464 696e 6729 0a0a  _grid(padding)..
+000109c0: 2020 2020 2020 2020 2320 4d6f 6c65 6375          # Molecu
+000109d0: 6c61 7220 7375 7266 6163 6520 2853 4553  lar surface (SES
+000109e0: 206f 7220 5341 5329 2074 6f20 6772 6964   or SAS) to grid
+000109f0: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
+00010a00: 7269 6420 3d20 5f66 696c 6c5f 7265 6365  rid = _fill_rece
+00010a10: 7074 6f72 280a 2020 2020 2020 2020 2020  ptor(.          
+00010a20: 2020 7365 6c66 2e6e 7820 2a20 7365 6c66    self.nx * self
+00010a30: 2e6e 7920 2a20 7365 6c66 2e6e 7a2c 0a20  .ny * self.nz,. 
+00010a40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010a50: 6e78 2c0a 2020 2020 2020 2020 2020 2020  nx,.            
+00010a60: 7365 6c66 2e6e 792c 0a20 2020 2020 2020  self.ny,.       
+00010a70: 2020 2020 2073 656c 662e 6e7a 2c0a 2020       self.nz,.  
+00010a80: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+00010a90: 797a 722c 0a20 2020 2020 2020 2020 2020  yzr,.           
+00010aa0: 2073 656c 662e 7031 2c0a 2020 2020 2020   self.p1,.      
+00010ab0: 2020 2020 2020 7365 6c66 2e72 6f74 6174        self.rotat
+00010ac0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00010ad0: 2073 656c 662e 7374 6570 2c0a 2020 2020   self.step,.    
+00010ae0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00010af0: 6265 2c0a 2020 2020 2020 2020 2020 2020  be,.            
+00010b00: 7375 7266 6163 652c 0a20 2020 2020 2020  surface,.       
+00010b10: 2020 2020 2073 656c 662e 6e74 6872 6561       self.nthrea
+00010b20: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+00010b30: 7365 6c66 2e76 6572 626f 7365 2c0a 2020  self.verbose,.  
+00010b40: 2020 2020 2020 292e 7265 7368 6170 6528        ).reshape(
+00010b50: 7365 6c66 2e6e 782c 2073 656c 662e 6e79  self.nx, self.ny
+00010b60: 2c20 7365 6c66 2e6e 7a29 0a0a 2020 2020  , self.nz)..    
+00010b70: 6465 6620 766f 6c75 6d65 2873 656c 6629  def volume(self)
+00010b80: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
+00010b90: 2020 2022 2222 4573 7469 6d61 7465 2074     """Estimate t
+00010ba0: 6865 2076 6f6c 756d 6520 6f66 2074 6865  he volume of the
+00010bb0: 206d 6f6c 6563 756c 6520 6261 7365 6420   molecule based 
+00010bc0: 6f6e 2074 6865 206d 6f6c 6563 756c 6172  on the molecular
+00010bd0: 2073 7572 6661 6365 2072 6570 7265 7365   surface represe
+00010be0: 6e74 6174 696f 6e2c 2069 652c 2076 6457  ntation, ie, vdW
+00010bf0: 2c20 5345 5320 6f72 2053 4153 2072 6570  , SES or SAS rep
+00010c00: 7265 7365 6e74 6174 696f 6e73 2e0a 0a20  resentations... 
+00010c10: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00010c20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00010c30: 2020 2020 2020 2076 6f6c 756d 6520 3a20         volume : 
+00010c40: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
+00010c50: 2020 4d6f 6c65 6375 6c61 7220 766f 6c75    Molecular volu
+00010c60: 6d65 2028 41c2 b329 2e0a 0a20 2020 2020  me (A..)...     
+00010c70: 2020 2045 7861 6d70 6c65 0a20 2020 2020     Example.     
+00010c80: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00010c90: 2020 2057 6974 6820 7468 6520 6d6f 6c65     With the mole
+00010ca0: 6375 6c61 7220 7375 7266 6163 6520 6d6f  cular surface mo
+00010cb0: 6465 6c6c 6564 2062 7920 6060 4d6f 6c65  delled by ``Mole
+00010cc0: 6375 6c65 2e76 6477 2829 6060 206f 7220  cule.vdw()`` or 
+00010cd0: 6060 4d6f 6c65 6375 6c65 2e73 7572 6661  ``Molecule.surfa
+00010ce0: 6365 2829 6060 2c20 7468 6520 766f 6c75  ce()``, the volu
+00010cf0: 6d65 2063 616e 2062 6520 6573 7469 6d61  me can be estima
+00010d00: 7465 6420 6279 2072 756e 6e69 6e67 3a0a  ted by running:.
+00010d10: 0a20 2020 2020 2020 203e 3e3e 206d 6f6c  .        >>> mol
+00010d20: 6563 756c 652e 766f 6c75 6d65 2829 0a20  ecule.volume(). 
+00010d30: 2020 2020 2020 2039 302e 380a 2020 2020         90.8.    
+00010d40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010d50: 6672 6f6d 205f 7079 4b56 4669 6e64 6572  from _pyKVFinder
+00010d60: 2069 6d70 6f72 7420 5f76 6f6c 756d 650a   import _volume.
+00010d70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00010d80: 2e67 7269 6420 6973 206e 6f74 204e 6f6e  .grid is not Non
+00010d90: 653a 0a20 2020 2020 2020 2020 2020 2076  e:.            v
+00010da0: 6f6c 756d 6520 3d20 5f76 6f6c 756d 6528  olume = _volume(
+00010db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dc0: 2028 7365 6c66 2e67 7269 6420 3d3d 2030   (self.grid == 0
+00010dd0: 292e 6173 7479 7065 286e 756d 7079 2e69  ).astype(numpy.i
+00010de0: 6e74 3332 2920 2a20 322c 2073 656c 662e  nt32) * 2, self.
+00010df0: 7374 6570 2c20 312c 2073 656c 662e 6e74  step, 1, self.nt
+00010e00: 6872 6561 6473 0a20 2020 2020 2020 2020  hreads.         
+00010e10: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00010e20: 2072 6574 7572 6e20 666c 6f61 7428 766f   return float(vo
+00010e30: 6c75 6d65 2e72 6f75 6e64 2864 6563 696d  lume.round(decim
+00010e40: 616c 733d 3229 290a 0a20 2020 2064 6566  als=2))..    def
+00010e50: 2070 7265 7669 6577 2873 656c 662c 202a   preview(self, *
+00010e60: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
+00010e70: 3a0a 2020 2020 2020 2020 2222 2250 7265  :.        """Pre
+00010e80: 7669 6577 2074 6865 206d 6f6c 6563 756c  view the molecul
+00010e90: 6172 2073 7572 6661 6365 2069 6e20 7468  ar surface in th
+00010ea0: 6520 3344 2067 7269 642e 0a0a 2020 2020  e 3D grid...    
+00010eb0: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
+00010ec0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00010ed0: 2020 2020 5769 7468 2074 6865 206d 6f6c      With the mol
+00010ee0: 6563 756c 6172 2073 7572 6661 6365 206d  ecular surface m
+00010ef0: 6f64 656c 6c65 6420 6279 2060 604d 6f6c  odelled by ``Mol
+00010f00: 6563 756c 652e 7664 7728 2960 6020 6f72  ecule.vdw()`` or
+00010f10: 2060 604d 6f6c 6563 756c 652e 7375 7266   ``Molecule.surf
+00010f20: 6163 6528 2960 602c 2074 6865 206d 6f64  ace()``, the mod
+00010f30: 656c 6c65 6420 6d6f 6c65 6375 6c65 2069  elled molecule i
+00010f40: 6e20 7468 6520 3344 2067 7269 6420 6361  n the 3D grid ca
+00010f50: 6e20 6265 2070 7265 7669 6577 6564 2062  n be previewed b
+00010f60: 7920 7275 6e6e 696e 673a 0a0a 2020 2020  y running:..    
+00010f70: 2020 2020 3e3e 3e20 6d6f 6c65 6375 6c65      >>> molecule
+00010f80: 2e70 7265 7669 6577 2829 0a20 2020 2020  .preview().     
+00010f90: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00010fa0: 6620 7365 6c66 2e67 7269 6420 6973 206e  f self.grid is n
+00010fb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010fc0: 2020 2020 2066 726f 6d20 706c 6f74 6c79       from plotly
+00010fd0: 2e65 7870 7265 7373 2069 6d70 6f72 7420  .express import 
+00010fe0: 7363 6174 7465 725f 3364 0a0a 2020 2020  scatter_3d..    
+00010ff0: 2020 2020 2020 2020 782c 2079 2c20 7a20          x, y, z 
+00011000: 3d20 6e75 6d70 792e 6e6f 6e7a 6572 6f28  = numpy.nonzero(
+00011010: 7365 6c66 2e67 7269 6420 3d3d 2030 290a  self.grid == 0).
+00011020: 2020 2020 2020 2020 2020 2020 6669 6720              fig 
+00011030: 3d20 7363 6174 7465 725f 3364 2878 3d78  = scatter_3d(x=x
+00011040: 2c20 793d 792c 207a 3d7a 2c20 2a2a 6b77  , y=y, z=z, **kw
+00011050: 6172 6773 290a 2020 2020 2020 2020 2020  args).          
+00011060: 2020 6669 672e 7570 6461 7465 5f6c 6179    fig.update_lay
+00011070: 6f75 7428 0a20 2020 2020 2020 2020 2020  out(.           
+00011080: 2020 2020 2073 6365 6e65 5f78 6178 6973       scene_xaxis
+00011090: 5f73 686f 7774 6963 6b6c 6162 656c 733d  _showticklabels=
+000110a0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+000110b0: 2020 2020 2020 2073 6365 6e65 5f79 6178         scene_yax
+000110c0: 6973 5f73 686f 7774 6963 6b6c 6162 656c  is_showticklabel
+000110d0: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
+000110e0: 2020 2020 2020 2020 2073 6365 6e65 5f7a           scene_z
+000110f0: 6178 6973 5f73 686f 7774 6963 6b6c 6162  axis_showticklab
+00011100: 656c 733d 4661 6c73 652c 0a20 2020 2020  els=False,.     
+00011110: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011120: 2020 2020 2066 6967 2e73 686f 7728 290a       fig.show().
+00011130: 0a20 2020 2064 6566 2065 7870 6f72 7428  .    def export(
+00011140: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00011150: 2020 2020 2020 2066 6e3a 2055 6e69 6f6e         fn: Union
+00011160: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
+00011170: 7468 5d20 3d20 226d 6f6c 6563 756c 652e  th] = "molecule.
+00011180: 7064 6222 2c0a 2020 2020 2920 2d3e 204e  pdb",.    ) -> N
+00011190: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000111a0: 4578 706f 7274 206d 6f6c 6563 756c 6520  Export molecule 
+000111b0: 706f 696e 7473 2028 4829 2074 6f20 6120  points (H) to a 
+000111c0: 5044 422d 666f 726d 6174 7465 6420 6669  PDB-formatted fi
+000111d0: 6c65 2e0a 0a20 2020 2020 2020 2050 6172  le...        Par
+000111e0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+000111f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00011200: 2020 2066 6e20 3a20 556e 696f 6e5b 7374     fn : Union[st
+00011210: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+00011220: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00011230: 2020 2020 2020 2041 2066 696c 6520 7061         A file pa
+00011240: 7468 2074 6f20 7468 6520 6d6f 6c65 6375  th to the molecu
+00011250: 6c61 7220 766f 6c75 6d65 2069 6e20 7468  lar volume in th
+00011260: 6520 6772 6964 2d62 6173 6564 2072 6572  e grid-based rer
+00011270: 7065 7365 6e74 6174 696f 6e20 696e 2050  pesentation in P
+00011280: 4442 2066 6f72 6d61 742c 2062 7920 6465  DB format, by de
+00011290: 6661 756c 7420 226d 6f6c 6563 756c 652e  fault "molecule.
+000112a0: 7064 6222 2e0a 0a20 2020 2020 2020 2052  pdb"...        R
+000112b0: 6169 7365 730a 2020 2020 2020 2020 2d2d  aises.        --
+000112c0: 2d2d 2d2d 0a20 2020 2020 2020 2054 7970  ----.        Typ
+000112d0: 6545 7272 6f72 0a20 2020 2020 2020 2020  eError.         
+000112e0: 2020 2060 666e 6020 6d75 7374 2062 6520     `fn` must be 
+000112f0: 6120 7374 7269 6e67 206f 7220 6120 7061  a string or a pa
+00011300: 7468 6c69 622e 5061 7468 2e0a 0a20 2020  thlib.Path...   
+00011310: 2020 2020 2045 7861 6d70 6c65 0a20 2020       Example.   
+00011320: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00011330: 2020 2020 2057 6974 6820 7468 6520 6d6f       With the mo
+00011340: 6c65 6375 6c61 7220 7375 7266 6163 6520  lecular surface 
+00011350: 6d6f 6465 6c6c 6564 2062 7920 6060 4d6f  modelled by ``Mo
+00011360: 6c65 6375 6c65 2e76 6477 2829 6060 206f  lecule.vdw()`` o
+00011370: 7220 6060 4d6f 6c65 6375 6c65 2e73 7572  r ``Molecule.sur
+00011380: 6661 6365 2829 6060 2c20 7468 6520 6d6f  face()``, the mo
+00011390: 6465 6c6c 6564 206d 6f6c 6563 756c 6520  delled molecule 
+000113a0: 696e 2074 6865 2033 4420 6772 6964 2063  in the 3D grid c
+000113b0: 616e 2062 6520 6578 706f 7274 6564 2074  an be exported t
+000113c0: 6f20 6120 5044 422d 666f 726d 6174 7465  o a PDB-formatte
+000113d0: 6420 6669 6c65 2062 7920 7275 6e6e 696e  d file by runnin
+000113e0: 673a 0a0a 2020 2020 2020 2020 3e3e 3e20  g:..        >>> 
+000113f0: 6d6f 6c65 6375 6c65 2e65 7870 6f72 7428  molecule.export(
+00011400: 276d 6f64 656c 2e70 6462 2729 0a20 2020  'model.pdb').   
+00011410: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011420: 2023 2046 696c 656e 616d 6520 2866 6e29   # Filename (fn)
+00011430: 0a20 2020 2020 2020 2069 6620 7479 7065  .        if type
+00011440: 2866 6e29 206e 6f74 2069 6e20 5b73 7472  (fn) not in [str
+00011450: 2c20 7061 7468 6c69 622e 5061 7468 5d3a  , pathlib.Path]:
+00011460: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00011470: 7365 2054 7970 6545 7272 6f72 2822 6066  se TypeError("`f
+00011480: 6e60 206d 7573 7420 6265 2061 2073 7472  n` must be a str
+00011490: 696e 6720 6f72 2061 2070 6174 686c 6962  ing or a pathlib
+000114a0: 2e50 6174 682e 2229 0a20 2020 2020 2020  .Path.").       
+000114b0: 206f 732e 6d61 6b65 6469 7273 286f 732e   os.makedirs(os.
+000114c0: 7061 7468 2e61 6273 7061 7468 286f 732e  path.abspath(os.
+000114d0: 7061 7468 2e64 6972 6e61 6d65 2866 6e29  path.dirname(fn)
+000114e0: 292c 2065 7869 7374 5f6f 6b3d 5472 7565  ), exist_ok=True
+000114f0: 290a 0a20 2020 2020 2020 2023 2053 6176  )..        # Sav
+00011500: 6520 6772 6964 2074 6f20 5044 4220 6669  e grid to PDB fi
+00011510: 6c65 0a20 2020 2020 2020 2065 7870 6f72  le.        expor
+00011520: 7428 0a20 2020 2020 2020 2020 2020 2066  t(.            f
+00011530: 6e2c 2028 7365 6c66 2e67 7269 6420 3d3d  n, (self.grid ==
+00011540: 2030 292e 6173 7479 7065 286e 756d 7079   0).astype(numpy
+00011550: 2e69 6e74 3332 2920 2a20 322c 204e 6f6e  .int32) * 2, Non
+00011560: 652c 2073 656c 662e 7665 7274 6963 6573  e, self.vertices
+00011570: 2c20 7365 6c66 2e73 7465 700a 2020 2020  , self.step.    
+00011580: 2020 2020 290a                               ).
```

### Comparing `pyKVFinder-0.5.5/pyKVFinder/utils.py` & `pyKVFinder-0.6.0/pyKVFinder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1094,15 +1094,14 @@
 
 
 def write_results(
     fn: Union[str, pathlib.Path],
     input: Optional[Union[str, pathlib.Path]],
     ligand: Optional[Union[str, pathlib.Path]],
     output: Optional[Union[str, pathlib.Path]],
-    output_hydropathy: Optional[Union[str, pathlib.Path]] = None,
     volume: Optional[Dict[str, float]] = None,
     area: Optional[Dict[str, float]] = None,
     max_depth: Optional[Dict[str, float]] = None,
     avg_depth: Optional[Dict[str, float]] = None,
     avg_hydropathy: Optional[Dict[str, float]] = None,
     residues: Optional[Dict[str, List[List[str]]]] = None,
     frequencies: Optional[Dict[str, Dict[str, Dict[str, int]]]] = None,
@@ -1118,17 +1117,14 @@
         residues) per cavity detected.
     input : Union[str, pathlib.Path], optional
         A path to input PDB or XYZ file.
     ligand : Union[str, pathlib.Path], optional
         A path to ligand PDB or XYZ file.
     output : Union[str, pathlib.Path], optional
         A path to cavity PDB file.
-    output_hydropathy : Union[str, pathlib.Path], optional
-        A path to hydropathy PDB file (surface points mapped with a
-        hydrophobicity scale), by default None.
     volume : Dict[str, float], optional
         A dictionary with volume of each detected cavity, by default None.
     area : Dict[str, float], optional
         A dictionary with area of each detected cavity, by default None.
     max_depth : Dict[str, float], optional
         A dictionary with maximum depth of each detected cavity, by default
         None.
@@ -1154,16 +1150,14 @@
     TypeError
         `input` must be a string or a pathlib.Path.
     TypeError
         `ligand` must be a string or a pathlib.Path.
     TypeError
         `output` must be a string or a pathlib.Path.
     TypeError
-        `output_hydropathy` must be a string or a pathlib.Path.
-    TypeError
         `volume` must be a dictionary.
     TypeError
         `area` must be a dictionary.
     TypeError
         `max_depth` must be a dictionary.
     TypeError
         `avg_depth` must be a dictionary.
@@ -1228,19 +1222,19 @@
     {'KAA': 1.28, 'KAB': 0.86, 'KAC': 0.67, 'KAD': 0.29, 'KAE': 0.98, 'KAF': 0.24, 'KAG': 0.1, 'KAH': 3.75, 'KAI': 1.5, 'KAJ': 0.96, 'KAK': 0.0, 'KAL': 1.0, 'KAM': 0.24, 'KAN': 0.0, 'KAO': 0.29, 'KAP': 0.7, 'KAQ': 0.22, 'KAR': 0.12}
     >>> write_results('results.toml', input=pdb, ligand=None, output=None, max_depth=max_depth, avg_depth=avg_depth)
 
     * Write hydropathy characterization
 
     >>> avg_hydropathy
     {'KAA': -0.73, 'KAB': -0.06, 'KAC': -0.07, 'KAD': -0.62, 'KAE': -0.81, 'KAF': -0.14, 'KAG': -0.33, 'KAH': -0.16, 'KAI': -0.4, 'KAJ': 0.62, 'KAK': -0.99, 'KAL': 0.35, 'KAM': -0.33, 'KAN': 0.18, 'KAO': 0.88, 'KAP': -0.96, 'KAQ': 0.48, 'KAR': 0.24, 'EisenbergWeiss': [-1.42, 2.6]}
-    >>> write_results('results.toml', input=pdb, ligand=None, output=None, output_hydropathy='hydropathy.pdb', avg_hydropathy=avg_hydropathy)
+    >>> write_results('results.toml', input=pdb, ligand=None, output=None, avg_hydropathy=avg_hydropathy)
 
     * Write all
 
-    >>> write_results('results.toml', input=pdb, ligand=None, output='cavities.pdb', output_hydropathy='hydropathy.pdb', volume=volume, area=area, max_depth=max_depth, avg_depth=avg_depth, avg_hydropathy=avg_hydropathy, residues=residues, frequencies=frequencies)
+    >>> write_results('results.toml', input=pdb, ligand=None, output='cavities.pdb', volume=volume, area=area, max_depth=max_depth, avg_depth=avg_depth, avg_hydropathy=avg_hydropathy, residues=residues, frequencies=frequencies)
 
     """
     import toml
 
     # Check arguments
     if type(fn) not in [str, pathlib.Path]:
         raise TypeError("`fn` must be a string or a pathlib.Path.")
@@ -1249,17 +1243,14 @@
             raise TypeError("`input` must be a string or a pathlib.Path.")
     if ligand is not None:
         if type(ligand) not in [str, pathlib.Path]:
             raise TypeError("`ligand` must be a string or a pathlib.Path.")
     if output is not None:
         if type(output) not in [str, pathlib.Path]:
             raise TypeError("`output` must be a string or a pathlib.Path.")
-    if output_hydropathy is not None:
-        if type(output_hydropathy) not in [str, pathlib.Path]:
-            raise TypeError("`output_hydropathy` must be a string or a pathlib.Path.")
     if volume is not None:
         if type(volume) not in [dict]:
             raise TypeError("`volume` must be a dictionary.")
     if area is not None:
         if type(area) not in [dict]:
             raise TypeError("`area` must be a dictionary.")
     if max_depth is not None:
@@ -1291,23 +1282,20 @@
 
     # Prepare paths
     input = os.path.abspath(input)
     if ligand:
         ligand = os.path.abspath(ligand)
     if output:
         output = os.path.abspath(output)
-    if output_hydropathy:
-        output_hydropathy = os.path.abspath(output_hydropathy)
 
     # Create output dictionary for results file
     files = {
         "INPUT": input,
         "LIGAND": ligand,
         "OUTPUT": output,
-        "HYDROPATHY": output_hydropathy,
     }
     parameters = {
         "STEP": step,
     }
     results = (
         {
             "VOLUME": volume,
```

### Comparing `pyKVFinder-0.5.5/pyKVFinder.egg-info/PKG-INFO` & `pyKVFinder-0.6.0/pyKVFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.5.5
+Version: 0.6.0
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.5.5/pyKVFinder.egg-info/SOURCES.txt` & `pyKVFinder-0.6.0/pyKVFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.5/pyproject.toml` & `pyKVFinder-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -86,12 +86,12 @@
 ]
 build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
 
 [tool.cibuildwheel.linux]
 archs = ["native"]
 
 [tool.cibuildwheel.macos]
-environment = { CC = "/usr/local/bin/gcc-11" }
-before-build = ["brew install gcc@11"]
+environment = { CC = "/usr/local/bin/gcc-9", MACOS_DEVELOPMENT_TARGET = "10.9" }
+before-build = ["brew install gcc@9"]
 archs = ["native"]
 repair-wheel-command = ""
 test-skip = "*-macosx_arm64"
```

### Comparing `pyKVFinder-0.5.5/setup.py` & `pyKVFinder-0.6.0/setup.py`

 * *Files identical despite different names*

