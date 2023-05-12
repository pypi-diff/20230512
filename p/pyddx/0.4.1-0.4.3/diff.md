# Comparing `tmp/pyddx-0.4.1.tar.gz` & `tmp/pyddx-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyddx-0.4.1.tar", last modified: Thu Apr 13 15:40:02 2023, max compression
+gzip compressed data, was "pyddx-0.4.3.tar", last modified: Fri May 12 13:05:00 2023, max compression
```

## Comparing `pyddx-0.4.1.tar` & `pyddx-0.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:02.739338 pyddx-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-13 15:37:32.000000 pyddx-0.4.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-13 15:37:32.000000 pyddx-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 15:37:32.000000 pyddx-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 15:40:02.739338 pyddx-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 15:37:32.000000 pyddx-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:02.731337 pyddx-0.4.1/pyddx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:37:44.000000 pyddx-0.4.1/pyddx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 15:37:32.000000 pyddx-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 15:40:02.739338 pyddx-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-04-13 15:37:32.000000 pyddx-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:02.739338 pyddx-0.4.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/cbessel.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx.f90
--rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx.h
--rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_cinterface.f90
--rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_constants.f90
--rw-r--r--   0 runner    (1001) docker     (123)   120346 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_cosmo.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_definitions.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_driver.f90
--rw-r--r--   0 runner    (1001) docker     (123)    82968 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_gradients.f90
--rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_harmonics.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_lpb.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_lpb_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_mkrhs.f90
--rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_multipolar_solutes.f90
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_operators.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_parameters.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_pcm.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_solvers.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_workspace.f90
--rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/llgnew.f
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/matrix_debug.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/pyddx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/pyddx_classes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/pyddx_data.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:05:00.552627 pyddx-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-12 13:02:43.000000 pyddx-0.4.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-12 13:02:43.000000 pyddx-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 13:02:43.000000 pyddx-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-12 13:05:00.552627 pyddx-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-12 13:02:43.000000 pyddx-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:05:00.548627 pyddx-0.4.3/pyddx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:02:52.000000 pyddx-0.4.3/pyddx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 13:02:43.000000 pyddx-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 13:05:00.552627 pyddx-0.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-05-12 13:02:43.000000 pyddx-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:05:00.552627 pyddx-0.4.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/cbessel.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_cinterface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_constants.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   122788 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_cosmo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_definitions.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_driver.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    73336 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_gradients.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_harmonics.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_lpb.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_lpb_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_mkrhs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_multipolar_solutes.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_operators.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_pcm.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_solvers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_workspace.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/llgnew.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/matrix_debug.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/pyddx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31313 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/pyddx_classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/pyddx_data.cpp
```

### Comparing `pyddx-0.4.1/CMakeLists.txt` & `pyddx-0.4.3/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Restrict building in top-level directory
 if("${CMAKE_CURRENT_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_BINARY_DIR}")
     message(FATAL_ERROR "In-source builds are not allowed.\nPlease create a "
         "build directory first and execute cmake configuration from this "
         "directory. Example: mkdir build && cd build && cmake ..")
 endif()
 
-project(ddX VERSION 0.4.1 LANGUAGES Fortran CXX)
+project(ddX VERSION 0.4.3 LANGUAGES Fortran CXX)
 # If ddX is a subproject, append ddx_ prefix to all targets.
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
     set(ddx_is_subproject false)
     set(ddx_ "")
 else()
     set(ddx_is_subproject true)
     set(ddx_ "ddx_")
```

### Comparing `pyddx-0.4.1/LICENSE.txt` & `pyddx-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/PKG-INFO` & `pyddx-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.1
+Version: 0.4.3
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.1/README.md` & `pyddx-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/pyddx.egg-info/PKG-INFO` & `pyddx-0.4.3/pyddx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.1
+Version: 0.4.3
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.1/pyddx.egg-info/SOURCES.txt` & `pyddx-0.4.3/pyddx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/setup.py` & `pyddx-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyddx",
     description="ddx continuum solvation library",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
-    version="0.4.1",
+    version="0.4.3",
     #
     author="ddx developers",
     author_email="best@ians.uni-stuttgart.de",
     license="LGPL v3",
     url="https://ddsolvation.github.io/ddX",
     project_urls={
         "Source": "https://github.com/ddsolvation/ddX",
```

### Comparing `pyddx-0.4.1/src/CMakeLists.txt` & `pyddx-0.4.3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/cbessel.f90` & `pyddx-0.4.3/src/cbessel.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx.f90` & `pyddx-0.4.3/src/ddx.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx.h` & `pyddx-0.4.3/src/ddx.h`

 * *Files 3% similar despite different names*

```diff
@@ -235,14 +235,25 @@
 /** Return the xi, the adjoint solution s projected onto the cavity points.
  *  \param state   DDX state
  *  \param ddx     DDX model
  *  \param ncav    Number of cavity points
  *  \param xi      Array to be filled with ncav
  */
 void ddx_get_xi(const void* state, const void* ddx, int ncav, double* xi);
+
+/** Return the zeta_dip, the dipolar contribution of the LPB adjoint solution,
+ *  at the cavity points.
+ *  The pointer should refer to the memory location of an array of
+ *  size (3, ncav). Data will be stored in column-major format.
+ *  \param state     DDX state
+ *  \param ddx       DDX model
+ *  \param ncav      Number of cavity points
+ *  \param zeta_dip  Array to be filled with ncav
+ */
+void ddx_get_zeta_dip(const void* state, const void* ddx, int ncav, double* zeta_dip);
 ///@}
 
 /** \name Problem setup and solution routines */
 ///@{
 
 /** Setup a COSMO problem in the passed state.
  *  \param ddx     DDX model
```

### Comparing `pyddx-0.4.1/src/ddx_cinterface.f90` & `pyddx-0.4.3/src/ddx_cinterface.f90`

 * *Files 1% similar despite different names*

```diff
@@ -505,19 +505,29 @@
     type(c_ptr), intent(in), value :: c_state, c_ddx
     type(ddx_state_type), pointer :: state
     type(ddx_setup), pointer :: ddx
     integer(c_int), intent(in), value :: ncav
     real(c_double), intent(out)  :: xi(ncav)
     call c_f_pointer(c_ddx, ddx)
     call c_f_pointer(c_state, state)
-    if (allocated(state%x_adj_lpb)) then  ! Case for ddLPB
-        ! Use only the first of the two solutions
-        call ddproject_cav(ddx%params, ddx%constants, state%x_adj_lpb(:, :, 1), xi)
+    call ddproject_cav(ddx%params, ddx%constants, state%q, xi)
+end subroutine
+
+subroutine ddx_get_zeta_dip(c_state, c_ddx, ncav, zeta_dip) bind(C)
+    type(c_ptr), intent(in), value :: c_state, c_ddx
+    type(ddx_state_type), pointer :: state
+    type(ddx_setup), pointer :: ddx
+    integer(c_int), intent(in), value :: ncav
+    real(c_double), intent(out)  :: zeta_dip(3, ncav)
+    call c_f_pointer(c_ddx, ddx)
+    call c_f_pointer(c_state, state)
+    if (allocated(state%zeta_dip)) then
+        zeta_dip(:, :) = state%zeta_dip(:, :)
     else
-        call ddproject_cav(ddx%params, ddx%constants, state%s, xi)
+        zeta_dip(:, :) = 0d0
     endif
 end subroutine
 
 
 !
 ! Cosmo
 !
```

### Comparing `pyddx-0.4.1/src/ddx_constants.f90` & `pyddx-0.4.3/src/ddx_constants.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_core.f90` & `pyddx-0.4.3/src/ddx_core.f90`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,18 @@
     !> Relative error of the iterative solver at each iteration of the adjoint
     !! ddLPB linear system, dimension (maxiter).
     !! Allocated and used only by the LPB (model=3) model.
     real(dp), allocatable :: x_adj_lpb_rel_diff(:)
     !> Zeta dipoles intermediate for the forces. Dimension (3, ncav).
     !! Allocated and used only by the LPB (model=3) model.
     real(dp), allocatable :: zeta_dip(:, :)
+    real(dp), allocatable :: x_adj_re_grid(:, :)
+    real(dp), allocatable :: x_adj_r_grid(:, :)
+    real(dp), allocatable :: x_adj_e_grid(:, :)
+    real(dp), allocatable :: phi_n(:, :)
 
 end type ddx_state_type
 
 !> Main ddX type that stores all the required information.
 !! Container for the params, contants and workspace derived types.
 type ddx_type
     !! New types inside the old one for an easier shift to the new design
@@ -333,14 +337,22 @@
     end if
     allocate(state % gradphi_cav(3, constants % ncav), stat=istatus)
     if (istatus .ne. 0) then
         state % error_flag = 1
         state % error_message = "ddinit: `gradphi_cav` allocation failed"
         return
     end if
+    allocate(state % q(constants % nbasis, &
+        & params % nsph), stat=istatus)
+    if (istatus .ne. 0) then
+        state % error_flag = 1
+        state % error_message = "ddinit: `q` " // &
+            & "allocation failed"
+        return
+    end if
 
     ! COSMO model
     if (params % model .eq. 1) then
         allocate(state % phi_grid(params % ngrid, &
             & params % nsph), stat=istatus)
         if (istatus .ne. 0) then
             state % error_flag = 1
@@ -513,22 +525,14 @@
             & params % nsph), stat=istatus)
         if (istatus .ne. 0) then
             state % error_flag = 1
             state % error_message = "ddinit: `g` " // &
                 & "allocation failed"
             return
         end if
-        allocate(state % q(constants % nbasis, &
-            & params % nsph), stat=istatus)
-        if (istatus .ne. 0) then
-            state % error_flag = 1
-            state % error_message = "ddinit: `q` " // &
-                & "allocation failed"
-            return
-        end if
         allocate(state % qgrid(params % ngrid, &
             & params % nsph), stat=istatus)
         if (istatus .ne. 0) then
             state % error_flag = 1
             state % error_message = "ddinit: `qgrid` " // &
                 & "allocation failed"
             return
@@ -636,14 +640,46 @@
         allocate(state % zeta_dip(3, constants % ncav), stat=istatus)
         if (istatus .ne. 0) then
             state % error_flag = 1
             state % error_message = "ddinit: `zeta_dip` " // &
                 & "allocation failed"
             return
         end if
+        allocate(state % x_adj_re_grid(params % ngrid, params % nsph), &
+            & stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "ddinit: `x_adj_re_grid` " // &
+                & "allocation failed"
+            return
+        end if
+        allocate(state % x_adj_r_grid(params % ngrid, params % nsph), &
+            & stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "ddinit: `x_adj_r_grid` " // &
+                & "allocation failed"
+            return
+        end if
+        allocate(state % x_adj_e_grid(params % ngrid, params % nsph), &
+            & stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "ddinit: `x_adj_e_grid` " // &
+                & "allocation failed"
+            return
+        end if
+        allocate(state % phi_n(params % ngrid, params % nsph), &
+            & stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "ddinit: `phi_n` " // &
+                & "allocation failed"
+            return
+        end if
     end if
 end subroutine ddx_init_state
 
 !------------------------------------------------------------------------------
 !> Read configuration from a file
 !!
 !! @param[in] fname: Filename containing all the required info
@@ -1108,14 +1144,42 @@
     if (allocated(state % zeta_dip)) then
         deallocate(state % zeta_dip, stat=istatus)
         if (istatus .ne. 0) then
             state % error_flag = 1
             state % error_message = "`zeta_dip` deallocation failed!"
         endif
     end if
+    if (allocated(state % x_adj_re_grid)) then
+        deallocate(state % x_adj_re_grid, stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "`x_adj_re_grid` deallocation failed!"
+        endif
+    end if
+    if (allocated(state % x_adj_r_grid)) then
+        deallocate(state % x_adj_r_grid, stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "`x_adj_r_grid` deallocation failed!"
+        endif
+    end if
+    if (allocated(state % x_adj_e_grid)) then
+        deallocate(state % x_adj_e_grid, stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "`x_adj_e_grid` deallocation failed!"
+        endif
+    end if
+    if (allocated(state % phi_n)) then
+        deallocate(state % phi_n, stat=istatus)
+        if (istatus .ne. 0) then
+            state % error_flag = 1
+            state % error_message = "`phi_n` deallocation failed!"
+        endif
+    end if
 end subroutine ddx_free_state
 
 !------------------------------------------------------------------------------
 !> Print array of spherical harmonics
 !!
 !! Prints (nbasis, ncol) array
 !!
@@ -1772,16 +1836,16 @@
     real(dp), intent(out) :: xi(constants%ncav)
     integer :: its, isph, ii
     ii = 0
     do isph = 1, params%nsph
         do its = 1, params%ngrid
             if (constants%ui(its, isph) .gt. zero) then
                 ii     = ii + 1
-                xi(ii) = constants%ui(its, isph) &
-                    &* dot_product(constants%vwgrid(:, its), s(:, isph))
+                xi(ii) = constants%ui(its, isph)*dot_product( &
+                    & constants%vwgrid(:constants % nbasis, its), s(:, isph))
             end if
         end do
     end do
 end subroutine ddproject_cav
 
 !------------------------------------------------------------------------------
 !> Transfer multipole coefficients over a tree
@@ -2957,15 +3021,15 @@
 !!
 !! @param[out] string: container for the logo
 !!
 subroutine get_banner(string)
     implicit none
     character (len=2047), intent(out) :: string
     character (len=10) :: vstr
-    write(vstr, *) "0.4.1"
+    write(vstr, *) "0.4.3"
     write(string, *) &
         & " +----------------------------------------------------------------+", &
         & NEW_LINE('a'), &
         & "  |                                                                |", &
         & NEW_LINE('a'), &
         & "  |                        888      888 Y8b    d8Y                 |", &
         & NEW_LINE('a'), &
```

### Comparing `pyddx-0.4.1/src/ddx_cosmo.f90` & `pyddx-0.4.3/src/ddx_cosmo.f90`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,18 @@
     state % s_niter = params % maxiter
     start_time = omp_get_wtime()
     call jacobi_diis(params, constants, workspace, tol, state % psi, &
         & state % s, state % s_niter, state % s_rel_diff, lstarx, ldm1x, hnorm)
     finish_time = omp_get_wtime()
     state % s_time = finish_time - start_time
 
+    state % q = state % s
+
+    call ddcosmo_derivative_setup(params, constants, workspace, state)
+
 end subroutine ddcosmo_solve_adjoint
 
 !> Compute the solvation term of the forces (solute aspecific). This must
 !> be summed to the solute specific term to get the full forces.
 !!
 !> @ingroup Fortran_interface_ddcosmo
 !! @param[in] params: User specified parameters
@@ -222,54 +226,73 @@
     implicit none
     type(ddx_params_type), intent(in) :: params
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     type(ddx_state_type), intent(inout) :: state
     real(dp), intent(inout) :: force(3, params % nsph)
     ! local variables
-    real(dp), external :: ddot
     real(dp) :: start_time, finish_time
-    integer :: icav, isph, igrid
+    integer :: isph
 
     start_time = omp_get_wtime()
-    ! Get values of S on the grid
-    call ddeval_grid_work(constants % nbasis, params % ngrid, params % nsph, &
-        & constants % vgrid, constants % vgrid_nbasis, one, state % s, zero, &
-        & state % sgrid)
-    ! Get the values of phi on the grid
-    call ddcav_to_grid_work(params % ngrid, params % nsph, constants % ncav, &
-        & constants % icav_ia, constants % icav_ja, state % phi_cav, &
-        & state % phi_grid)
 
     force = zero
     do isph = 1, params % nsph
         call contract_grad_l(params, constants, isph, state % xs, &
             & state % sgrid, workspace % tmp_vylm(:, 1), &
             & workspace % tmp_vdylm(:, :, 1), workspace % tmp_vplm(:, 1), &
             & workspace % tmp_vcos(:, 1), workspace % tmp_vsin(:, 1), &
             & force(:, isph))
         call contract_grad_u(params, constants, isph, state % sgrid, &
             & state % phi_grid, force(:, isph))
     end do
     force = - pt5 * force
 
+    finish_time = omp_get_wtime()
+    state % force_time = finish_time - start_time
+
+end subroutine ddcosmo_solvation_force_terms
+
+!> This routines precomputes the intermediates to be used in the evaluation
+!! of ddCOSMO analytical derivatives.
+!!
+!! @param[in] params: ddx parameters
+!! @param[in] constant: ddx constants
+!! @param[inout] workspace: ddx workspaces
+!! @param[inout] state: ddx state
+!!
+subroutine ddcosmo_derivative_setup(params, constants, workspace, state)
+    type(ddx_params_type), intent(in) :: params
+    type(ddx_constants_type), intent(in) :: constants
+    type(ddx_workspace_type), intent(inout) :: workspace
+    type(ddx_state_type), intent(inout) :: state
+
+    real(dp), external :: ddot
+    integer :: icav, isph, igrid
+
+    ! Get values of S on the grid
+    call ddeval_grid_work(constants % nbasis, params % ngrid, params % nsph, &
+        & constants % vgrid, constants % vgrid_nbasis, one, state % s, zero, &
+        & state % sgrid)
+    ! Get the values of phi on the grid
+    call ddcav_to_grid_work(params % ngrid, params % nsph, constants % ncav, &
+        & constants % icav_ia, constants % icav_ja, state % phi_cav, &
+        & state % phi_grid)
+
     ! assemble the intermediate zeta: S weighted by U evaluated on the
-    ! exposed grid points. This is not required here, but it is used
-    ! in later steps.
+    ! exposed grid points.
     icav = 0
     do isph = 1, params % nsph
         do igrid = 1, params % ngrid
             if (constants % ui(igrid, isph) .ne. zero) then
                 icav = icav + 1
                 state % zeta(icav) = constants % wgrid(igrid) * &
                     & constants % ui(igrid, isph) * ddot(constants % nbasis, &
                     & constants % vgrid(1, igrid), 1, state % s(1, isph), 1)
             end if
         end do
     end do
-    finish_time = omp_get_wtime()
-    state % force_time = finish_time - start_time
 
-end subroutine ddcosmo_solvation_force_terms
+end subroutine ddcosmo_derivative_setup
 
 end module ddx_cosmo
```

### Comparing `pyddx-0.4.1/src/ddx_definitions.f90` & `pyddx-0.4.3/src/ddx_definitions.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_driver.f90` & `pyddx-0.4.3/src/ddx_driver.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_gradients.f90` & `pyddx-0.4.3/src/ddx_gradients.f90`

 * *Files 14% similar despite different names*

```diff
@@ -310,31 +310,30 @@
 !! @param[in]  workspace          : Input workspace
 !! @param[in] sol_sgrid           : Solution of the Adjoint problem evaluated at the grid
 !! @param[in] sol_adj             : Adjoint solution
 !! @param[in]  normal_hessian_cav : Normal of the Hessian evaluated at cavity points
 !! @param[in]  icav_g             : Index of outside cavity point
 !! @param[out] force              : Force
 subroutine contract_grad_f(params, constants, workspace, sol_adj, sol_sgrid, &
-    & gradpsi, normal_hessian_cav, icav_g, force, state)
+    & gradpsi, normal_hessian_cav, force, state)
     type(ddx_params_type), intent(in) :: params
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     type(ddx_state_type), intent(inout) :: state
     real(dp), dimension(constants % nbasis, params % nsph), intent(in) :: sol_adj
     real(dp), dimension(params % ngrid, params % nsph), intent(in) :: sol_sgrid
     real(dp), dimension(3, constants % ncav), intent(in) :: gradpsi
     real(dp), dimension(3, constants % ncav), intent(in) :: normal_hessian_cav
-    integer, intent(inout) :: icav_g
     real(dp), dimension(3, params % nsph), intent(inout) :: force
 
     call contract_grad_f_worker1(params, constants, workspace, sol_adj, sol_sgrid, &
         & gradpsi, force)
     if (workspace % error_flag .eq. 1) return
-    call contract_grad_f_worker2(params, constants, workspace, sol_sgrid, gradpsi, &
-        & normal_hessian_cav, icav_g, force, state)
+    call contract_grad_f_worker2(params, constants, workspace, gradpsi, &
+        & normal_hessian_cav, force, state)
     if (workspace % error_flag .eq. 1) return
 
 end subroutine contract_grad_f
 
 !> Subroutine to compute K^A counterpart for the HSP equation. Similar to contract_gradi_Lik.
 !!
 !! @param[in]  params    : Input parameter file
@@ -1551,284 +1550,64 @@
         workspace % error_flag = 1
         workspace % error_message = "deallocation error in ddx_grad_f_worker1"
         return
     end if
 
 end subroutine contract_grad_f_worker1
 
-
-!> Subroutine to calculate the derivative of C_{0l0m0}^j
-!!
-!! @param[in]  params             : Input parameter file
-!! @param[in]  constants          : Input constants file
-!! @param[in]  workspace          : Input workspace
-!! @param[in]  ksph               : Derivative with respect to x_k
-!! @param[in]  sol_sgrid          : Solution of the Adjoint problem evaluated at the grid
-!! @param[in]  gradpsi            : Gradient of Psi_0
-!! @param[in]  normal_hessian_cav : Normal of the Hessian evaluated at cavity points
-!! @param[in]  icav_g             : Index of outside cavity point
-!! @param[out] force              : Force corresponding to HSP problem
-subroutine contract_grad_f_worker2(params, constants, workspace, sol_sgrid, gradpsi, &
-    & normal_hessian_cav, icav_g, force, state)
-    ! input/output
+subroutine contract_grad_f_worker2(params, constants, workspace, &
+        & gradpsi, normal_hessian_cav, force, state)
     type(ddx_params_type), intent(in) :: params
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
-    real(dp), dimension(params % ngrid, params % nsph), intent(in) :: sol_sgrid
-    real(dp), dimension(3, constants % ncav), intent(in) :: gradpsi
-    real(dp), dimension(3, constants % ncav), intent(in) :: normal_hessian_cav
-    integer, intent(inout) :: icav_g
-    real(dp), dimension(3, params % nsph), intent(inout) :: force
+    real(dp), intent(in) :: gradpsi(3, constants % ncav), &
+        & normal_hessian_cav(3, constants % ncav)
+    real(dp), intent(inout) :: force(3, params % nsph)
     type(ddx_state_type), intent(inout) :: state
 
-    ! local
-    integer :: isph, jsph, igrid, l0, m0, ind0, igrid0, icav, &
-        & indl, inode, istat
-    ! term  : SK_rijn/SK_rj
-    ! termi : DI_ri/SI_ri
-    ! termk : DK_ri/SK_ri
-    ! sum_int : Intermediate sum
-    ! hessian_contribution :
-    real(dp) :: sum_int, nderpsi
-    real(dp) :: rijn
-    real(dp)  :: vij(3), sij(3), vtij(3)
+    integer :: icav, isph, igrid, istat
+    real(dp) :: nderpsi
+    real(dp), allocatable :: gradpsi_grid(:, :)
 
-    ! local allocatable
-    ! phi_n : Phi corresponding to Laplace problem
-    ! coefY_d : sum_{l0m0} C_ik*term*Y_l0m0^j(x_in)*Y_l0m0(s_n)
-    ! gradpsi_grid : gradpsi evaluated at grid point
-    real(dp), allocatable :: phi_n(:,:), phi_n2(:,:), coefY_d(:,:,:), &
-        & gradpsi_grid(:,:)
-
-    ! vplm   : Argument to call ylmbas
-    real(dp),  dimension(constants % nbasis):: basloc, vplm
-    real(dp),  dimension(3, constants % nbasis):: dbasloc
-    ! vcos   : Argument to call ylmbas
-    ! vsin   : Argument to call ylmbas
-    real(dp),  dimension(params % lmax+1):: vcos, vsin
-    real(dp), dimension(0:params % lmax) :: SK_rijn, DK_rijn
-    real(dp) :: coef(constants % nbasis0), work(constants % lmax0+1)
-    complex(dp) :: work_complex(constants % lmax0+1)
-    real(dp), external :: dnrm2
-
-    allocate(phi_n(params % ngrid, params % nsph), &
-        & phi_n2(params % ngrid, params % nsph), &
-        & gradpsi_grid(params % ngrid, params % nsph), stat=istat)
+    allocate(gradpsi_grid(params % ngrid, params % nsph), stat=istat)
     if (istat.ne.0) then
         workspace % error_flag = 1
         workspace % error_message = "allocation error in ddx_grad_f_worker2"
         return
     end if
 
-    ! Intial allocation of vectors
-    sum_int = zero
-    phi_n = zero
-    gradpsi_grid = zero
-    basloc = zero
-    vplm = zero
-    dbasloc = zero
-    vcos = zero
-    vsin = zero
-    SK_rijn = zero
-    DK_rijn = zero
-
-    if (params % fmm .eq. 0) then
-        allocate(coefY_d(constants % ncav, params % ngrid, params % nsph), &
-            & stat=istat)
-        if (istat.ne.0) then
-            workspace % error_flag = 1
-            workspace % error_message = "allocation error in fmm ddx_grad_f_worker2"
-            return
-        end if
-        coefY_d = zero
-        ! Compute  summation over l0, m0
-        ! Loop over the sphers j
-        do jsph = 1, params % nsph
-          ! Loop over the grid points n0
-          do igrid0 = 1, params % ngrid
-            icav = zero
-            ! Loop over spheres i
-            do isph = 1, params % nsph
-              ! Loop over grid points n
-              do igrid = 1, params % ngrid
-                ! Check for U_i^{eta}(x_in)
-                if(constants % ui(igrid, isph) .gt. zero) then
-                  icav = icav + 1
-                  vij  = params % csph(:,isph) + &
-                         & params % rsph(isph)*constants % cgrid(:,igrid) - &
-                         & params % csph(:,jsph)
-                  rijn = sqrt(dot_product(vij,vij))
-                  sij = vij/rijn
-                  ! Loop over l0
-                  do l0 = 0, constants % lmax0
-      !              term = SK_rijn(l0)/constants % SK_ri(l0,jsph)
-                    ! Loop over m0
-                    do m0 = -l0,l0
-                      ind0 = l0**2 + l0 + m0 + 1
-                      coef(ind0) = constants % vgrid(ind0, igrid0) * &
-                          & constants % C_ik(l0, jsph)
-                    end do ! End of loop m0
-                  end do! End of loop l0
-                  vtij = vij*params % kappa
-                  call fmm_m2p_bessel_work(vtij, constants % lmax0, &
-                      & constants % vscales, constants % SK_ri(:, jsph), one, &
-                      & coef, zero, coefY_d(icav, igrid0, jsph), work_complex, work)
-                end if
-              end do ! End of loop igrid
-            end do! End of loop isph
-          end do ! End of loop igrid0
-        end do ! End of loop jsph
-        ! Compute phi_in
-        ! Loop over spheres j
-        do jsph = 1, params % nsph
-          ! Loop over grid points n0
-          do igrid0 = 1, params % ngrid
-            icav = zero
-            sum_int = zero
-            ! Loop over sphers i
-            do isph = 1, params % nsph
-              ! Loop over grid points n
-              do igrid = 1, params % ngrid
-                if(constants % ui(igrid, isph) .gt. zero) then
-                  icav = icav + 1
-                  sum_int = sum_int + coefY_d(icav, igrid0, jsph)*sol_sgrid(igrid, isph) &
-                          & * constants % wgrid(igrid)*constants % ui(igrid, isph)
-                end if
-              end do
-            end do
-            phi_n(igrid0, jsph) = -(params % epsp/params % eps)*sum_int
-          end do! End of loop j
-        end do ! End of loop igrid
-    else
-        ! Adjoint integration from spherical harmonics to grid points is not needed
-        ! here as ygrid already contains grid values, we just need to scale it by
-        ! weights of grid points
-        do isph = 1, params % nsph
-            workspace % tmp_grid(:, isph) = sol_sgrid(:, isph) * &
-                & constants % wgrid(:) * constants % ui(:, isph)
-        end do
-        ! Adjoint FMM
-        call tree_m2p_bessel_adj(params, constants, constants % lmax0, one, &
-            & workspace % tmp_grid, zero, params % lmax, workspace % tmp_sph)
-        call tree_l2p_bessel_adj(params, constants, one, workspace % tmp_grid, &
-            & zero, workspace % tmp_node_l)
-        call tree_l2l_bessel_rotation_adj(params, constants, &
-            & workspace % tmp_node_l)
-        call tree_m2l_bessel_rotation_adj(params, constants, &
-            & workspace % tmp_node_l, workspace % tmp_node_m)
-        call tree_m2m_bessel_rotation_adj(params, constants, &
-            & workspace % tmp_node_m)
-        ! Properly load adjoint multipole harmonics into tmp_sph
-        if(constants % lmax0 .lt. params % pm) then
-            do isph = 1, params % nsph
-                inode = constants % snode(isph)
-                workspace % tmp_sph(1:constants % nbasis0, isph) = &
-                    & workspace % tmp_sph(1:constants % nbasis0, isph) + &
-                    & workspace % tmp_node_m(1:constants % nbasis0, inode)
-            end do
-        else
-            indl = (params % pm+1)**2
-            do isph = 1, params % nsph
-                inode = constants % snode(isph)
-                workspace % tmp_sph(1:indl, isph) = &
-                    & workspace % tmp_sph(1:indl, isph) + &
-                    & workspace % tmp_node_m(:, inode)
-            end do
-        end if
-        ! Scale by C_ik
-        do isph = 1, params % nsph
-            do l0 = 0, constants % lmax0
-                ind0 = l0*l0 + l0 + 1
-                workspace % tmp_sph(ind0-l0:ind0+l0, isph) = &
-                    & workspace % tmp_sph(ind0-l0:ind0+l0, isph) * &
-                    & constants % C_ik(l0, isph)
-            end do
-        end do
-        ! Multiply by vgrid
-        call dgemm('T', 'N', params % ngrid, params % nsph, constants % nbasis0, &
-            & -params % epsp/params % eps, constants % vgrid, constants % vgrid_nbasis, &
-            & workspace % tmp_sph, constants % nbasis, zero, phi_n, params % ngrid)
-    end if
-    icav = zero
+    icav = 0
     do isph = 1, params % nsph
-      do igrid = 1, params % ngrid
-        if(constants % ui(igrid, isph) .gt. zero) then
-          icav = icav + 1
-          nderpsi = dot_product( gradpsi(:,icav),constants % cgrid(:,igrid) )
-          gradpsi_grid(igrid, isph) = nderpsi
-        end if
-      end do ! End of loop igrid
-    end do ! End of loop i
+        do igrid = 1, params % ngrid
+            if(constants % ui(igrid, isph) .gt. zero) then
+                icav = icav + 1
+                nderpsi = dot_product(gradpsi(:, icav), &
+                    & constants % cgrid(:, igrid))
+                gradpsi_grid(igrid, isph) = nderpsi
+            end if
+        end do
+    end do
 
+    icav = 0
     do isph = 1, params % nsph
-        call contract_grad_U(params, constants, isph, gradpsi_grid, phi_n, force(:, isph))
-        ! Compute the Hessian contributions
+        call contract_grad_U(params, constants, isph, gradpsi_grid, &
+            & state % phi_n, force(:, isph))
         do igrid = 1, params % ngrid
           if(constants % ui(igrid, isph) .gt. zero) then
-            icav_g = icav_g + 1
-            ! a contrib
-            force(:, isph) = force(:, isph) + constants % wgrid(igrid)*constants % ui(igrid, isph)*&
-                             & phi_n(igrid, isph)*normal_hessian_cav(:, icav_g)
+            icav = icav + 1
+            force(:, isph) = force(:, isph) &
+                & + constants % wgrid(igrid)*constants % ui(igrid, isph) &
+                & *state % phi_n(igrid, isph)*normal_hessian_cav(:, icav)
           end if
         end do
     end do
 
-    call build_zeta_dip_intermediate(params, constants, phi_n, state)
-
-    deallocate(phi_n, phi_n2, gradpsi_grid, stat=istat)
+    deallocate(gradpsi_grid, stat=istat)
     if (istat.ne.0) then
         workspace % error_flag = 1
         workspace % error_message = "deallocation error in ddx_grad_f_worker2"
         return
     end if
-    if (allocated(coefY_d)) then
-        deallocate(coefY_d, stat=istat)
-        if (istat.ne.0) then
-            workspace % error_flag = 1
-            workspace % error_message = "deallocation error in ddx_grad_f_worker2"
-            return
-        end if
-    end if
-end subroutine contract_grad_f_worker2
-
-
-!> This routines precomputes an intermediate for its later usage in the
-!! computation of the forces. The intermediate is the equivalent of
-!! zeta for the F RHS of ddLPB. In this case the intermediate has the
-!! shape of dipoles at the cavity points, in contrast to zeta, which
-!! has the shape of charges at the cavity points. This intermediate
-!! must be used later on to compute its interaction with the solute.
-!!
-!! @param[in] params: ddx parameters
-!! @param[in] constant: ddx constants
-!! @param[in] phi_n: adjoint solution contracted with other matrices,
-!!     size (ngrid, nsph)
-!! @param[inout] force: force array, size (3, nsph)
-!!
-subroutine build_zeta_dip_intermediate(params, constants, phi_n, state)
-    implicit none
-    type(ddx_params_type), intent(in) :: params
-    type(ddx_constants_type), intent(in) :: constants
-    type(ddx_state_type), intent(inout) :: state
-    real(dp), intent(in) :: phi_n(params % ngrid, params % nsph)
-
-    integer :: isph, icav, igrid
-    real(dp) :: fac
 
-    ! assemble the pseudo-dipoles
-    icav = 0
-    do isph = 1, params % nsph
-        do igrid = 1, params % ngrid
-            if (constants % ui(igrid, isph) .gt. zero) then
-                icav = icav + 1
-                fac = - constants % ui(igrid, isph)*constants % wgrid(igrid) &
-                    & *phi_n(igrid, isph)
-                state % zeta_dip(1, icav) = fac*constants % cgrid(1, igrid)
-                state % zeta_dip(2, icav) = fac*constants % cgrid(2, igrid)
-                state % zeta_dip(3, icav) = fac*constants % cgrid(3, igrid)
-            end if
-        end do
-    end do
-
-end subroutine build_zeta_dip_intermediate
+end subroutine contract_grad_f_worker2
 
 end module ddx_gradients
```

### Comparing `pyddx-0.4.1/src/ddx_harmonics.f90` & `pyddx-0.4.3/src/ddx_harmonics.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_lpb.f90` & `pyddx-0.4.3/src/ddx_lpb.f90`

 * *Files 20% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 
     ! Get forces if needed
     if(params % force .eq. 1) then
         call ddlpb_guess_adjoint(params, constants, workspace, state, tol)
         if (workspace % error_flag .eq. 1) return
         call ddlpb_solve_adjoint(params, constants, workspace, state, tol)
         if (workspace % error_flag .eq. 1) return
-        ! TODO: (if easy) remove hessianphi_cav
         call ddlpb_solvation_force_terms(params, constants, workspace, &
             & state, hessianphi_cav, force)
         if (workspace % error_flag .eq. 1) return
     endif
 
 end subroutine ddlpb
 
@@ -286,21 +285,24 @@
     if (workspace % error_flag .ne. 0) then
         workspace % error_message = 'Jacobi solver failed to ' // &
             & 'converge in ddlpb_solve_adjoint'
         return
     end if
     state % x_adj_lpb_time = omp_get_wtime() - start_time
 
+    state % q = state % x_adj_lpb(:, :, 1)
+
+    call ddlpb_derivative_setup(params, constants, workspace, state)
+
 end subroutine ddlpb_solve_adjoint
 
+!> Compute the solvation terms of the forces (solute aspecific). This
+!! must be summed to the solute specific term to get the full forces.
 !!
-!! Wrapper routine for the computation of ddPCM forces. It makes the
-!! interface easier to implement. If a fine control is needed, the
-!! worker routine should be directly called.
-!!
+!> @ingroup Fortran_interface_ddlpb
 !! @param[in] params         : General options
 !! @param[in] constants      : Precomputed constants
 !! @param[inout] workspace   : Preallocated workspaces
 !! @param[inout] state       : Solutions and relevant quantities
 !! @param[in] hessianphi_cav : Electric field gradient at the grid points
 !! @param[out] force         : Geometrical contribution to the forces
 !!
@@ -316,25 +318,23 @@
 
     ! local
     real(dp), dimension(constants % nbasis) :: basloc, vplm
     real(dp), dimension(3, constants % nbasis) :: dbasloc
     real(dp), dimension(params % lmax + 1) :: vsin, vcos
 
     ! large local are allocatable
-    real(dp), allocatable :: ef(:,:), xadj_r_sgrid(:,:), xadj_e_sgrid(:,:), &
-        & normal_hessian_cav(:,:), diff_re(:,:), scaled_xr(:,:)
-    integer :: isph, icav, icav_gr, icav_ge, igrid, istat
+    real(dp), allocatable :: ef(:,:), normal_hessian_cav(:,:), &
+        & diff_re(:,:), scaled_xr(:,:)
+    integer :: isph, icav, igrid, istat
     integer :: i
     real(dp), external :: ddot, dnrm2
     real(dp) :: start_time, finish_time
 
     start_time = omp_get_wtime()
     allocate(ef(3, params % nsph), &
-        & xadj_r_sgrid(params % ngrid, params % nsph), &
-        & xadj_e_sgrid(params % ngrid, params % nsph), &
         & normal_hessian_cav(3, constants % ncav), &
         & diff_re(constants % nbasis, params % nsph), &
         & scaled_xr(constants % nbasis, params % nsph), stat=istat)
     if (istat.ne.0) then
         workspace % error_message = 'Allocation failed in ddlpb_force_worker'
         workspace % error_flag = 1
         return
@@ -363,47 +363,37 @@
                     normal_hessian_cav(:, icav) = normal_hessian_cav(:,icav) +&
                         & hessianphi_cav(:,i,icav)*constants % cgrid(i,igrid)
                 end do
             end if
         end do
     end do
 
-    ! Call dgemm to integrate the adjoint solution on the grid points
-    call dgemm('T', 'N', params % ngrid, params % nsph, constants % nbasis, &
-        & one, constants % vgrid, constants % vgrid_nbasis, &
-        & state % x_adj_lpb(:, :, 1), constants % nbasis, zero, &
-        & Xadj_r_sgrid, params % ngrid)
-    call dgemm('T', 'N', params % ngrid, params % nsph, constants % nbasis, &
-        & one, constants % vgrid, constants % vgrid_nbasis, &
-        & state % x_adj_lpb(:,:,2), constants % nbasis, zero, &
-        & Xadj_e_sgrid, params % ngrid)
-
     ! Scale by the factor of 1/(4Pi/(2l+1))
     scaled_Xr = state % x_lpb(:,:,1)
     call convert_ddcosmo(params, constants, -1, scaled_Xr)
 
     !$omp parallel do default(none) shared(params,constants,workspace, &
-    !$omp scaled_xr,xadj_r_sgrid,state,force,xadj_e_sgrid) &
-    !$omp private(isph,basloc,dbasloc,vplm,vcos,vsin) &
+    !$omp scaled_xr,state,force) private(isph,basloc,dbasloc,vplm,vcos,vsin) &
     !$omp schedule(static,1)
     do isph = 1, params % nsph
         ! Compute A^k*Xadj_r, using Subroutine from ddCOSMO
-        call contract_grad_L(params, constants, isph, scaled_Xr, Xadj_r_sgrid, &
-            & basloc, dbasloc, vplm, vcos, vsin, force(:,isph))
+        call contract_grad_L(params, constants, isph, scaled_Xr, &
+            & state % x_adj_r_grid, basloc, dbasloc, vplm, vcos, vsin, &
+            & force(:,isph))
         ! Compute B^k*Xadj_e
-        call contract_grad_B(params, constants, isph, &
-            & state % x_lpb(:,:,2), Xadj_e_sgrid, force(:, isph))
+        call contract_grad_B(params, constants, isph, state % x_lpb(:,:,2), &
+            & state % x_adj_e_grid, force(:, isph))
         ! Computation of G0
-        call contract_grad_U(params, constants, isph, Xadj_r_sgrid, &
+        call contract_grad_U(params, constants, isph, state % x_adj_r_grid, &
             & state % phi_grid, force(:, isph))
     end do
     ! Compute C1 and C2 contributions
     diff_re = zero
     call contract_grad_C(params, constants, workspace, state % x_lpb(:,:,1), &
-        & state % x_lpb(:,:,2), Xadj_r_sgrid, Xadj_e_sgrid, &
+        & state % x_lpb(:,:,2), state % x_adj_r_grid, state % x_adj_e_grid, &
         & state % x_adj_lpb(:,:,1), state % x_adj_lpb(:,:,2), force, &
         & diff_re)
     ! Computation of G0 continued
 
     ! NOTE: contract_grad_U returns a positive summation
     if (workspace % error_flag .eq. 1) return
     force = -force
@@ -416,35 +406,207 @@
                     & constants % ui(igrid, isph) * ddot(constants % nbasis, &
                     & constants % vgrid(1, igrid), 1, &
                     & state % x_adj_lpb(1, isph, 1), 1)
             end if
         end do
     end do
 
-    icav_gr = zero
-    icav_ge = zero
     ! Computation of F0
     call contract_grad_f(params, constants, workspace, &
         & state % x_adj_lpb(:,:,1) + state % x_adj_lpb(:,:,2), &
-        & Xadj_r_sgrid + xadj_e_sgrid, state % gradphi_cav, &
-        & normal_hessian_cav, icav_gr, force, state)
+        & state % x_adj_re_grid, state % gradphi_cav, &
+        & normal_hessian_cav, force, state)
     if (workspace % error_flag .eq. 1) return
 
     force = pt5*force
 
-    deallocate(ef, xadj_r_sgrid, xadj_e_sgrid, normal_hessian_cav, &
-        & diff_re, scaled_xr, stat=istat)
+    deallocate(ef, normal_hessian_cav, diff_re, scaled_xr, stat=istat)
     if (istat.ne.0) then
         workspace % error_message = 'Deallocation failed in ddlpb_force_worker'
         workspace % error_flag = 1
         return
     end if
     finish_time = omp_get_wtime()
     state % force_time = finish_time - start_time
 
     ! and now we remove again the factor, so that the density is
     ! restored.
     call convert_ddcosmo(params, constants, -1, state % x_lpb(:, :, 1))
 
 end subroutine ddlpb_solvation_force_terms
 
+!> This routines precomputes two intermediates for its later usage in
+!! the computation of analytical derivatives (forces or other).
+!!
+!! @param[in] params: ddx parameters
+!! @param[in] constant: ddx constants
+!! @param[inout] workspace: ddx workspaces
+!! @param[inout] state: ddx state
+!!
+subroutine ddlpb_derivative_setup(params, constants, workspace, state)
+    implicit none
+    type(ddx_params_type), intent(in) :: params
+    type(ddx_constants_type), intent(in) :: constants
+    type(ddx_workspace_type), intent(inout) :: workspace
+    type(ddx_state_type), intent(inout) :: state
+
+    real(dp), allocatable :: coefy_d(:, :, :)
+    integer :: istat, jsph, igrid0, icav, isph, igrid, l0, m0, ind0, &
+        & inode, indl
+    real(dp) :: rijn, sum_int, fac
+    real(dp) :: work(constants % lmax0 + 1), coef(constants % nbasis0), &
+        & vij(3), vtij(3), sij(3)
+    complex(dp) :: work_complex(constants % lmax0 + 1)
+
+    ! expand the adjoint solutions at the Lebedev points and compute
+    ! their sum
+    call dgemm('T', 'N', params % ngrid, params % nsph, &
+        & constants % nbasis, one, constants % vgrid, &
+        & constants % vgrid_nbasis, state % x_adj_lpb(:, :, 1), &
+        & constants % nbasis, zero, state % x_adj_r_grid, params % ngrid)
+    call dgemm('T', 'N', params % ngrid, params % nsph, &
+        & constants % nbasis, one, constants % vgrid, &
+        & constants % vgrid_nbasis, state % x_adj_lpb(:, :, 2), &
+        & constants % nbasis, zero, state % x_adj_e_grid, params % ngrid)
+    state % x_adj_re_grid = state % x_adj_r_grid + state % x_adj_e_grid
+
+    if (params % fmm .eq. 0) then
+        allocate(coefy_d(constants % ncav, params % ngrid, params % nsph), &
+            & stat=istat)
+        if (istat.ne.0) then
+            workspace % error_flag = 1
+            workspace % error_message = &
+                & "allocation error in ddlpb_derivative_intermediates"
+            return
+        end if
+        coefy_d = zero
+        do jsph = 1, params % nsph
+            do igrid0 = 1, params % ngrid
+                icav = zero
+                do isph = 1, params % nsph
+                    do igrid = 1, params % ngrid
+                        if(constants % ui(igrid, isph) .gt. zero) then
+                            icav = icav + 1
+                            vij = params % csph(:,isph) + params % rsph(isph) &
+                                & *constants % cgrid(:,igrid) &
+                                & - params % csph(:,jsph)
+                            rijn = sqrt(dot_product(vij,vij))
+                            sij = vij/rijn
+                            do l0 = 0, constants % lmax0
+                                do m0 = -l0, l0
+                                    ind0 = l0**2 + l0 + m0 + 1
+                                    coef(ind0) = &
+                                        & constants % vgrid(ind0, igrid0) * &
+                                        & constants % C_ik(l0, jsph)
+                                end do
+                            end do
+                            vtij = vij*params % kappa
+                            call fmm_m2p_bessel_work(vtij, constants % lmax0, &
+                                & constants % vscales, &
+                                & constants % sk_ri(:, jsph), one, &
+                                & coef, zero, coefy_d(icav, igrid0, jsph), &
+                                & work_complex, work)
+                        end if
+                    end do
+                end do
+            end do
+        end do
+        do jsph = 1, params % nsph
+            do igrid0 = 1, params % ngrid
+                icav = zero
+                sum_int = zero
+                do isph = 1, params % nsph
+                    do igrid = 1, params % ngrid
+                        if(constants % ui(igrid, isph) .gt. zero) then
+                            icav = icav + 1
+                            sum_int = sum_int + coefy_d(icav, igrid0, jsph) &
+                                & *state % x_adj_re_grid(igrid, isph) &
+                                & *constants % wgrid(igrid) &
+                                & *constants % ui(igrid, isph)
+                        end if
+                    end do
+                end do
+                state % phi_n(igrid0, jsph) = &
+                    & - (params % epsp/params % eps)*sum_int
+            end do
+        end do
+    else
+        ! Adjoint integration from spherical harmonics to grid points is not needed
+        ! here as ygrid already contains grid values, we just need to scale it by
+        ! weights of grid points
+        do isph = 1, params % nsph
+            workspace % tmp_grid(:, isph) = state % x_adj_re_grid(:, isph) * &
+                & constants % wgrid(:) * constants % ui(:, isph)
+        end do
+        ! Adjoint FMM
+        call tree_m2p_bessel_adj(params, constants, constants % lmax0, one, &
+            & workspace % tmp_grid, zero, params % lmax, workspace % tmp_sph)
+        call tree_l2p_bessel_adj(params, constants, one, &
+            & workspace % tmp_grid, zero, workspace % tmp_node_l)
+        call tree_l2l_bessel_rotation_adj(params, constants, &
+            & workspace % tmp_node_l)
+        call tree_m2l_bessel_rotation_adj(params, constants, &
+            & workspace % tmp_node_l, workspace % tmp_node_m)
+        call tree_m2m_bessel_rotation_adj(params, constants, &
+            & workspace % tmp_node_m)
+        ! Properly load adjoint multipole harmonics into tmp_sph
+        if(constants % lmax0 .lt. params % pm) then
+            do isph = 1, params % nsph
+                inode = constants % snode(isph)
+                workspace % tmp_sph(1:constants % nbasis0, isph) = &
+                    & workspace % tmp_sph(1:constants % nbasis0, isph) + &
+                    & workspace % tmp_node_m(1:constants % nbasis0, inode)
+            end do
+        else
+            indl = (params % pm+1)**2
+            do isph = 1, params % nsph
+                inode = constants % snode(isph)
+                workspace % tmp_sph(1:indl, isph) = &
+                    & workspace % tmp_sph(1:indl, isph) + &
+                    & workspace % tmp_node_m(:, inode)
+            end do
+        end if
+        ! Scale by C_ik
+        do isph = 1, params % nsph
+            do l0 = 0, constants % lmax0
+                ind0 = l0*l0 + l0 + 1
+                workspace % tmp_sph(ind0-l0:ind0+l0, isph) = &
+                    & workspace % tmp_sph(ind0-l0:ind0+l0, isph) * &
+                    & constants % C_ik(l0, isph)
+            end do
+        end do
+        ! Multiply by vgrid
+        call dgemm('T', 'N', params % ngrid, params % nsph, &
+            & constants % nbasis0, -params % epsp/params % eps, &
+            & constants % vgrid, constants % vgrid_nbasis, &
+            & workspace % tmp_sph, constants % nbasis, zero, &
+            & state % phi_n, params % ngrid)
+    end if
+
+    ! assemble the pseudo-dipoles
+    icav = 0
+    do isph = 1, params % nsph
+        do igrid = 1, params % ngrid
+            if (constants % ui(igrid, isph) .gt. zero) then
+                icav = icav + 1
+                fac = - constants % ui(igrid, isph)*constants % wgrid(igrid) &
+                    & *state % phi_n(igrid, isph)
+                state % zeta_dip(1, icav) = fac*constants % cgrid(1, igrid)
+                state % zeta_dip(2, icav) = fac*constants % cgrid(2, igrid)
+                state % zeta_dip(3, icav) = fac*constants % cgrid(3, igrid)
+            end if
+        end do
+    end do
+
+    if (allocated(coefy_d)) then
+        deallocate(coefy_d, stat=istat)
+        if (istat.ne.0) then
+            workspace % error_flag = 1
+            workspace % error_message = &
+                & "deallocation error in ddlpb_derivative_intermediates"
+            return
+        end if
+    end if
+
+end subroutine ddlpb_derivative_setup
+
 end module ddx_lpb
```

### Comparing `pyddx-0.4.1/src/ddx_lpb_core.f90` & `pyddx-0.4.3/src/ddx_lpb_core.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_mkrhs.f90` & `pyddx-0.4.3/src/ddx_mkrhs.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_multipolar_solutes.f90` & `pyddx-0.4.3/src/ddx_multipolar_solutes.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_operators.f90` & `pyddx-0.4.3/src/ddx_operators.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_parameters.f90` & `pyddx-0.4.3/src/ddx_parameters.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_pcm.f90` & `pyddx-0.4.3/src/ddx_pcm.f90`

 * *Files 3% similar despite different names*

```diff
@@ -243,14 +243,19 @@
 
     if (workspace % error_flag .ne. 0) then
         workspace % error_message = "ddpcm_energy: solver for adjoint " // &
             & "ddPCM system did not converge"
         return
     end if
 
+    ! compute the real adjoint solution and store it in Q
+    state % q = state % s - fourpi/(params % eps - one)*state % y
+
+    call ddpcm_derivative_setup(params, constants, workspace, state)
+
 end subroutine ddpcm_solve_adjoint
 
 !> Compute the solvation contribution to the ddPCM forces
 !!
 !> @ingroup Fortran_interface_ddpcm
 !! @param[in] params       : General options
 !! @param[in] constants    : Precomputed constants
@@ -262,59 +267,81 @@
         & state, force)
     implicit none
     type(ddx_params_type), intent(in) :: params
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     type(ddx_state_type), intent(inout) :: state
     real(dp), intent(out) :: force(3, params % nsph)
-    ! local
+
     real(dp) :: start_time, finish_time
-    real(dp), external :: ddot
-    integer :: icav, isph, igrid
+    integer :: isph
 
     start_time = omp_get_wtime()
-    call ddcav_to_grid_work(params % ngrid, params % nsph, constants % ncav, &
-        & constants % icav_ia, constants % icav_ja, state % phi_cav, &
-        & state % phi_grid)
-    ! Get grid values of S and Y
-    call dgemm('T', 'N', params % ngrid, params % nsph, &
-        & constants % nbasis, one, constants % vgrid, constants % vgrid_nbasis, &
-        & state % s, constants % nbasis, zero, state % sgrid, params % ngrid)
-    call dgemm('T', 'N', params % ngrid, params % nsph, &
-        & constants % nbasis, one, constants % vgrid, constants % vgrid_nbasis, &
-        & state % y, constants % nbasis, zero, state % ygrid, params % ngrid)
-
-    state % g = - (state % phieps - state % phi)
-    state % q = state % s - fourpi/(params % eps - one)*state % y
-    state % qgrid = state % sgrid - fourpi/(params % eps - one)*state % ygrid
 
     call gradr(params, constants, workspace, state % g, state % ygrid, force)
 
     do isph = 1, params % nsph
         call contract_grad_L(params, constants, isph, state % xs, &
             & state % sgrid, workspace % tmp_vylm(:, 1), &
             & workspace % tmp_vdylm(:, :, 1), workspace % tmp_vplm(:, 1), &
             & workspace % tmp_vcos(:, 1), workspace % tmp_vsin(:, 1), &
             & force(:, isph))
         call contract_grad_U(params, constants, isph, state % qgrid, &
             & state % phi_grid, force(:, isph))
     end do
     force = - pt5 * force
 
+    finish_time = omp_get_wtime()
+    state % force_time = finish_time - start_time
+
+end subroutine ddpcm_solvation_force_terms
+
+!> This routines precomputes the intermediates to be used in the evaluation
+!! of ddCOSMO analytical derivatives.
+!!
+!! @param[in] params: ddx parameters
+!! @param[in] constant: ddx constants
+!! @param[inout] workspace: ddx workspaces
+!! @param[inout] state: ddx state
+!!
+subroutine ddpcm_derivative_setup(params, constants, workspace, state)
+    type(ddx_params_type), intent(in) :: params
+    type(ddx_constants_type), intent(in) :: constants
+    type(ddx_workspace_type), intent(inout) :: workspace
+    type(ddx_state_type), intent(inout) :: state
+
+    real(dp), external :: ddot
+    integer :: icav, isph, igrid
+
+    ! Get grid values of S and Y
+    call dgemm('T', 'N', params % ngrid, params % nsph, &
+        & constants % nbasis, one, constants % vgrid, constants % vgrid_nbasis, &
+        & state % s, constants % nbasis, zero, state % sgrid, params % ngrid)
+    call dgemm('T', 'N', params % ngrid, params % nsph, &
+        & constants % nbasis, one, constants % vgrid, constants % vgrid_nbasis, &
+        & state % y, constants % nbasis, zero, state % ygrid, params % ngrid)
+
+    ! Get the values of phi on the grid
+    call ddcav_to_grid_work(params % ngrid, params % nsph, constants % ncav, &
+        & constants % icav_ia, constants % icav_ja, state % phi_cav, &
+        & state % phi_grid)
+
+    state % g = - (state % phieps - state % phi)
+    state % qgrid = state % sgrid - fourpi/(params % eps - one)*state % ygrid
+
+    ! assemble the intermediate zeta: S weighted by U evaluated on the
+    ! exposed grid points.
     icav = 0
     do isph = 1, params % nsph
         do igrid = 1, params % ngrid
-            if(constants % ui(igrid, isph) .ne. zero) then
+            if (constants % ui(igrid, isph) .ne. zero) then
                 icav = icav + 1
                 state % zeta(icav) = constants % wgrid(igrid) * &
                     & constants % ui(igrid, isph) * ddot(constants % nbasis, &
-                    & constants % vgrid(1, igrid), 1, &
-                    & state % q(1, isph), 1)
+                    & constants % vgrid(1, igrid), 1, state % q(1, isph), 1)
             end if
         end do
     end do
-    finish_time = omp_get_wtime()
-    state % force_time = finish_time - start_time
 
-end subroutine ddpcm_solvation_force_terms
+end subroutine ddpcm_derivative_setup
 
 end module ddx_pcm
```

### Comparing `pyddx-0.4.1/src/ddx_solvers.f90` & `pyddx-0.4.3/src/ddx_solvers.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/ddx_workspace.f90` & `pyddx-0.4.3/src/ddx_workspace.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/llgnew.f` & `pyddx-0.4.3/src/llgnew.f`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/matrix_debug.f90` & `pyddx-0.4.3/src/matrix_debug.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/pyddx.cpp` & `pyddx-0.4.3/src/pyddx.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.1/src/pyddx_classes.cpp` & `pyddx-0.4.3/src/pyddx_classes.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,21 @@
   }
   array_f_t xi() const {
     check_solved_adjoint();
     array_f_t xi({m_model->n_cav()});
     ddx_get_xi(m_holder, m_model->holder(), m_model->n_cav(), xi.mutable_data());
     return xi;
   }
+  array_f_t zeta_dip() const {
+    check_solved_adjoint();
+    array_f_t zeta_dip({3, m_model->n_cav()});
+    ddx_get_zeta_dip(m_holder, m_model->holder(), m_model->n_cav(),
+                     zeta_dip.mutable_data());
+    return zeta_dip;
+  }
 
   //
   // Solving COSMO / PCM / LPB
   //
   void update_problem(array_f_t psi, array_f_t phi, py::object py_elec_field) {
     if (psi.ndim() != 2 || psi.shape(0) != model()->n_basis() ||
         psi.shape(1) != model()->n_spheres()) {
@@ -698,14 +705,15 @@
               "x_n_iter", &State::x_n_iter,
               "Number of iterations required to solve the forward problem.")
         .def_property_readonly("s", &State::s, "Solution of the adjoint problem.")
         .def_property_readonly(
               "s_n_iter", &State::s_n_iter,
               "Number of iterations required to solve the adjoint problem.")
         .def_property_readonly("xi", &State::xi)
+        .def_property_readonly("zeta_dip", &State::zeta_dip)
         .def_property_readonly("is_solved", &State::is_solved,
                                "Return whether the forward problem is solved.")
         .def_property_readonly("is_solved_adjoint", &State::is_solved_adjoint,
                                "Return whether the adjoint problem is solved.")
         //
         .def("update_problem", &State::update_problem,
              "Update the definition of of the forward and adjoint problem", "psi"_a,
```

### Comparing `pyddx-0.4.1/src/pyddx_data.cpp` & `pyddx-0.4.3/src/pyddx_data.cpp`

 * *Files identical despite different names*

