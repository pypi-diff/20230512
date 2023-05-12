# Comparing `tmp/fastfft-0.1.7.tar.gz` & `tmp/fastfft-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.1.7.tar", last modified: Fri May 12 14:51:37 2023, max compression
+gzip compressed data, was "fastfft-0.1.8.tar", last modified: Fri May 12 16:21:10 2023, max compression
```

## Comparing `fastfft-0.1.7.tar` & `fastfft-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.925797 fastfft-0.1.7/
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-05-12 12:16:40.000000 fastfft-0.1.7/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)       45 2023-05-12 12:16:40.000000 fastfft-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 14:51:37.925797 fastfft-0.1.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-12 12:16:40.000000 fastfft-0.1.7/README.md
--rw-rw-r--   0 root         (0) root         (0)       27 2023-05-12 12:16:40.000000 fastfft-0.1.7/requirements-dev.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-05-12 12:16:40.000000 fastfft-0.1.7/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)     1543 2023-05-12 14:51:37.925797 fastfft-0.1.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1397 2023-05-12 12:22:07.000000 fastfft-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.921797 fastfft-0.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.921797 fastfft-0.1.7/src/fastfft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-12 14:51:37.000000 fastfft-0.1.7/src/fastfft.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.921797 fastfft-0.1.7/src/fft2/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-12 12:16:40.000000 fastfft-0.1.7/src/fft2/__init__.py
--rw-r--r--   0 root         (0) root         (0)   222791 2023-05-12 14:51:29.000000 fastfft-0.1.7/src/fft2/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:51:37.925797 fastfft-0.1.7/tests/
--rw-rw-r--   0 root         (0) root         (0)      131 2023-05-12 12:16:40.000000 fastfft-0.1.7/tests/test_fft2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:10.406489 fastfft-0.1.8/
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-05-12 16:19:20.000000 fastfft-0.1.8/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       45 2023-05-12 16:19:20.000000 fastfft-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 16:21:10.406489 fastfft-0.1.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-12 16:19:20.000000 fastfft-0.1.8/README.md
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-05-12 16:19:20.000000 fastfft-0.1.8/requirements-dev.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-05-12 16:19:20.000000 fastfft-0.1.8/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)     1543 2023-05-12 16:21:10.406489 fastfft-0.1.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1339 2023-05-12 16:19:20.000000 fastfft-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:10.402489 fastfft-0.1.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:10.402489 fastfft-0.1.8/src/fastfft/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-12 16:19:20.000000 fastfft-0.1.8/src/fastfft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222908 2023-05-12 16:21:01.000000 fastfft-0.1.8/src/fastfft/fft.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:10.402489 fastfft-0.1.8/src/fastfft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-12 16:21:10.000000 fastfft-0.1.8/src/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-12 16:21:10.000000 fastfft-0.1.8/src/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:21:10.000000 fastfft-0.1.8/src/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:21:10.000000 fastfft-0.1.8/src/fastfft.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-12 16:21:10.000000 fastfft-0.1.8/src/fastfft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 16:21:10.000000 fastfft-0.1.8/src/fastfft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:10.406489 fastfft-0.1.8/tests/
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-05-12 16:19:20.000000 fastfft-0.1.8/tests/test_fft2.py
```

### Comparing `fastfft-0.1.7/LICENSE.txt` & `fastfft-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastfft-0.1.7/PKG-INFO` & `fastfft-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.1.7
+Version: 0.1.8
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.1.7/setup.cfg` & `fastfft-0.1.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fastfft
-version = 0.1.7
+version = 0.1.8
 description = Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = Maxim Movshin
 author_email = maxim-movshin@yandex.ru
 url = https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.1.7/setup.py` & `fastfft-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 
 import os
-from setuptools import setup, find_packages, Extension
+from setuptools import setup, Extension
 
 try:
     from Cython.Build import cythonize
 except ImportError:
     cythonize = None
 
 
@@ -20,15 +20,15 @@
                 sfile = path + ext
             sources.append(sfile)
         extension.sources[:] = sources
     return extensions
 
 
 extensions = [
-    Extension("fft2.main", ["src/fft2/main.pyx"]),
+    Extension("fastfft.main", ["src/fastfft/fft.pyx"]),
 ]
 
 CYTHONIZE = bool(int(os.getenv("CYTHONIZE", 0))) and cythonize is not None
 
 if CYTHONIZE:
     compiler_directives = {"language_level": 3, "embedsignature": True}
     extensions = cythonize(extensions, compiler_directives=compiler_directives)
@@ -42,10 +42,9 @@
     dev_requires = fp.read().strip().split("\n")
 
 setup(
     ext_modules=extensions,
     install_requires=install_requires,
     extras_require={
         "dev": dev_requires,
-        #"docs": ["sphinx", "sphinx-rtd-theme"]
     },
 )
```

### Comparing `fastfft-0.1.7/src/fastfft.egg-info/PKG-INFO` & `fastfft-0.1.8/src/fastfft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.1.7
+Version: 0.1.8
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.1.7/src/fft2/main.cpp` & `fastfft-0.1.8/src/fastfft/fft.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
             [
                 "CYTHON_CCOMPLEX",
                 "0"
             ]
         ],
         "depends": [],
         "language": "c++",
-        "name": "fft2.main",
+        "name": "fastfft.main",
         "sources": [
-            "src/fft2/main.pyx"
+            "src/fastfft/fft.pyx"
         ]
     },
-    "module_name": "fft2.main"
+    "module_name": "fastfft.main"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -768,16 +768,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__fft2__main
-#define __PYX_HAVE_API__fft2__main
+#define __PYX_HAVE__fastfft__main
+#define __PYX_HAVE_API__fastfft__main
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include <complex>
@@ -1008,15 +1008,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "src/fft2/main.pyx",
+  "src/fastfft/fft.pyx",
   "stringsource",
 };
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
@@ -1441,182 +1441,182 @@
 
 /* Module declarations from 'libcpp.vector' */
 
 /* Module declarations from 'libcpp.complex' */
 
 /* Module declarations from 'libcpp' */
 
-/* Module declarations from 'fft2.main' */
-static std::complex<double>  __pyx_v_4fft2_4main_PI;
-static std::complex<double>  __pyx_v_4fft2_4main_I;
-static std::complex<double>  __pyx_v_4fft2_4main_MINUS_PI_2I;
-static std::complex<double>  __pyx_v_4fft2_4main_PI_I;
-static void __pyx_f_4fft2_4main_base2x2fft2(std::vector<std::vector<std::complex<double> > >  &); /*proto*/
-static std::complex<double>  __pyx_f_4fft2_4main_W_MINUS_PI_2I(double, double); /*proto*/
-static void __pyx_f_4fft2_4main_fft2_square(std::vector<std::vector<std::complex<double> > >  &); /*proto*/
+/* Module declarations from 'fastfft.main' */
+static std::complex<double>  __pyx_v_7fastfft_4main_PI;
+static std::complex<double>  __pyx_v_7fastfft_4main_I;
+static std::complex<double>  __pyx_v_7fastfft_4main_MINUS_PI_2I;
+static std::complex<double>  __pyx_v_7fastfft_4main_PI_I;
+static void __pyx_f_7fastfft_4main__base2x2fft2(std::vector<std::vector<std::complex<double> > >  &); /*proto*/
+static std::complex<double>  __pyx_f_7fastfft_4main_W(double, double); /*proto*/
+static void __pyx_f_7fastfft_4main__fft2_square(std::vector<std::vector<std::complex<double> > >  &); /*proto*/
 static std::complex<double>  __pyx_convert_complex_from_py_double(PyObject *); /*proto*/
 static std::vector<std::complex<double> >  __pyx_convert_vector_from_py_std_3a__3a_complex_3c_double_3e___(PyObject *); /*proto*/
 static PyObject *__pyx_convert_complex_to_py_double(std::complex<double>  const &); /*proto*/
 static PyObject *__pyx_convert_vector_to_py_std_3a__3a_complex_3c_double_3e___(const std::vector<std::complex<double> >  &); /*proto*/
 static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_complex_3c_double_3e____3e___(const std::vector<std::vector<std::complex<double> > >  &); /*proto*/
-#define __Pyx_MODULE_NAME "fft2.main"
-extern int __pyx_module_is_main_fft2__main;
-int __pyx_module_is_main_fft2__main = 0;
+#define __Pyx_MODULE_NAME "fastfft.main"
+extern int __pyx_module_is_main_fastfft__main;
+int __pyx_module_is_main_fastfft__main = 0;
 
-/* Implementation of 'fft2.main' */
+/* Implementation of 'fastfft.main' */
 static PyObject *__pyx_builtin_range;
+static const char __pyx_k_fft2[] = "fft2";
 static const char __pyx_k_line[] = "line";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_matrix[] = "matrix";
-static const char __pyx_k_fft2_main[] = "fft2.main";
 static const char __pyx_k_cpp_matrix[] = "cpp_matrix";
-static const char __pyx_k_py_fft2_square[] = "py_fft2_square";
-static const char __pyx_k_src_fft2_main_pyx[] = "src/fft2/main.pyx";
+static const char __pyx_k_fastfft_main[] = "fastfft.main";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_src_fastfft_fft_pyx[] = "src/fastfft/fft.pyx";
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_cpp_matrix;
-static PyObject *__pyx_n_s_fft2_main;
+static PyObject *__pyx_n_s_fastfft_main;
+static PyObject *__pyx_n_s_fft2;
 static PyObject *__pyx_n_s_line;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_matrix;
 static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_py_fft2_square;
 static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_kp_s_src_fft2_main_pyx;
+static PyObject *__pyx_kp_s_src_fastfft_fft_pyx;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_pf_4fft2_4main_py_fft2_square(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_matrix); /* proto */
+static PyObject *__pyx_pf_7fastfft_4main_fft2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_matrix); /* proto */
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_codeobj__2;
 /* Late includes */
 
-/* "fft2/main.pyx":17
+/* "src/fastfft/fft.pyx":17
  * 
  * 
- * cdef void base2x2fft2(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
+ * cdef void _base2x2fft2(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
  *     matrix[0][0], matrix[0][1] = matrix[0][0] + matrix[0][1], matrix[0][0] - matrix[0][1]
  *     matrix[1][0], matrix[1][1] = matrix[1][0] + matrix[1][1], matrix[1][0] - matrix[1][1]
  */
 
-static void __pyx_f_4fft2_4main_base2x2fft2(std::vector<std::vector<std::complex<double> > >  &__pyx_v_matrix) {
+static void __pyx_f_7fastfft_4main__base2x2fft2(std::vector<std::vector<std::complex<double> > >  &__pyx_v_matrix) {
   __Pyx_RefNannyDeclarations
   std::complex<double>  __pyx_t_1;
   std::complex<double>  __pyx_t_2;
-  __Pyx_RefNannySetupContext("base2x2fft2", 0);
+  __Pyx_RefNannySetupContext("_base2x2fft2", 0);
 
-  /* "fft2/main.pyx":18
+  /* "src/fastfft/fft.pyx":18
  * 
- * cdef void base2x2fft2(vector[vector[complex[double]]]& matrix):
+ * cdef void _base2x2fft2(vector[vector[complex[double]]]& matrix):
  *     matrix[0][0], matrix[0][1] = matrix[0][0] + matrix[0][1], matrix[0][0] - matrix[0][1]             # <<<<<<<<<<<<<<
  *     matrix[1][0], matrix[1][1] = matrix[1][0] + matrix[1][1], matrix[1][0] - matrix[1][1]
  * 
  */
   __pyx_t_1 = (((__pyx_v_matrix[0])[0]) + ((__pyx_v_matrix[0])[1]));
   __pyx_t_2 = (((__pyx_v_matrix[0])[0]) - ((__pyx_v_matrix[0])[1]));
   ((__pyx_v_matrix[0])[0]) = __pyx_t_1;
   ((__pyx_v_matrix[0])[1]) = __pyx_t_2;
 
-  /* "fft2/main.pyx":19
- * cdef void base2x2fft2(vector[vector[complex[double]]]& matrix):
+  /* "src/fastfft/fft.pyx":19
+ * cdef void _base2x2fft2(vector[vector[complex[double]]]& matrix):
  *     matrix[0][0], matrix[0][1] = matrix[0][0] + matrix[0][1], matrix[0][0] - matrix[0][1]
  *     matrix[1][0], matrix[1][1] = matrix[1][0] + matrix[1][1], matrix[1][0] - matrix[1][1]             # <<<<<<<<<<<<<<
  * 
  *     matrix[0][0], matrix[1][0] = matrix[0][0] + matrix[1][0], matrix[0][0] - matrix[1][0]
  */
   __pyx_t_2 = (((__pyx_v_matrix[1])[0]) + ((__pyx_v_matrix[1])[1]));
   __pyx_t_1 = (((__pyx_v_matrix[1])[0]) - ((__pyx_v_matrix[1])[1]));
   ((__pyx_v_matrix[1])[0]) = __pyx_t_2;
   ((__pyx_v_matrix[1])[1]) = __pyx_t_1;
 
-  /* "fft2/main.pyx":21
+  /* "src/fastfft/fft.pyx":21
  *     matrix[1][0], matrix[1][1] = matrix[1][0] + matrix[1][1], matrix[1][0] - matrix[1][1]
  * 
  *     matrix[0][0], matrix[1][0] = matrix[0][0] + matrix[1][0], matrix[0][0] - matrix[1][0]             # <<<<<<<<<<<<<<
  *     matrix[0][1], matrix[1][1] = matrix[0][1] + matrix[1][1], matrix[0][1] - matrix[1][1]
  * 
  */
   __pyx_t_1 = (((__pyx_v_matrix[0])[0]) + ((__pyx_v_matrix[1])[0]));
   __pyx_t_2 = (((__pyx_v_matrix[0])[0]) - ((__pyx_v_matrix[1])[0]));
   ((__pyx_v_matrix[0])[0]) = __pyx_t_1;
   ((__pyx_v_matrix[1])[0]) = __pyx_t_2;
 
-  /* "fft2/main.pyx":22
+  /* "src/fastfft/fft.pyx":22
  * 
  *     matrix[0][0], matrix[1][0] = matrix[0][0] + matrix[1][0], matrix[0][0] - matrix[1][0]
  *     matrix[0][1], matrix[1][1] = matrix[0][1] + matrix[1][1], matrix[0][1] - matrix[1][1]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (((__pyx_v_matrix[0])[1]) + ((__pyx_v_matrix[1])[1]));
   __pyx_t_1 = (((__pyx_v_matrix[0])[1]) - ((__pyx_v_matrix[1])[1]));
   ((__pyx_v_matrix[0])[1]) = __pyx_t_2;
   ((__pyx_v_matrix[1])[1]) = __pyx_t_1;
 
-  /* "fft2/main.pyx":17
+  /* "src/fastfft/fft.pyx":17
  * 
  * 
- * cdef void base2x2fft2(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
+ * cdef void _base2x2fft2(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
  *     matrix[0][0], matrix[0][1] = matrix[0][0] + matrix[0][1], matrix[0][0] - matrix[0][1]
  *     matrix[1][0], matrix[1][1] = matrix[1][0] + matrix[1][1], matrix[1][0] - matrix[1][1]
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "fft2/main.pyx":25
+/* "src/fastfft/fft.pyx":25
  * 
  * 
- * cdef complex[double] W_MINUS_PI_2I(double n, double m):             # <<<<<<<<<<<<<<
+ * cdef complex[double] W(double n, double m):             # <<<<<<<<<<<<<<
  *     return exp[double](MINUS_PI_2I * m / n)
  * 
  */
 
-static std::complex<double>  __pyx_f_4fft2_4main_W_MINUS_PI_2I(double __pyx_v_n, double __pyx_v_m) {
+static std::complex<double>  __pyx_f_7fastfft_4main_W(double __pyx_v_n, double __pyx_v_m) {
   std::complex<double>  __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("W_MINUS_PI_2I", 0);
+  __Pyx_RefNannySetupContext("W", 0);
 
-  /* "fft2/main.pyx":26
+  /* "src/fastfft/fft.pyx":26
  * 
- * cdef complex[double] W_MINUS_PI_2I(double n, double m):
+ * cdef complex[double] W(double n, double m):
  *     return exp[double](MINUS_PI_2I * m / n)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_r = std::exp<double>(((__pyx_v_4fft2_4main_MINUS_PI_2I * __pyx_v_m) / __pyx_v_n));
+  __pyx_r = std::exp<double>(((__pyx_v_7fastfft_4main_MINUS_PI_2I * __pyx_v_m) / __pyx_v_n));
   goto __pyx_L0;
 
-  /* "fft2/main.pyx":25
+  /* "src/fastfft/fft.pyx":25
  * 
  * 
- * cdef complex[double] W_MINUS_PI_2I(double n, double m):             # <<<<<<<<<<<<<<
+ * cdef complex[double] W(double n, double m):             # <<<<<<<<<<<<<<
  *     return exp[double](MINUS_PI_2I * m / n)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fft2/main.pyx":29
+/* "src/fastfft/fft.pyx":29
  * 
  * 
- * cdef void fft2_square(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
+ * cdef void _fft2_square(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
  *     cdef int n = matrix.size()
  *     cdef half_n = n // 2
  */
 
-static void __pyx_f_4fft2_4main_fft2_square(std::vector<std::vector<std::complex<double> > >  &__pyx_v_matrix) {
+static void __pyx_f_7fastfft_4main__fft2_square(std::vector<std::vector<std::complex<double> > >  &__pyx_v_matrix) {
   int __pyx_v_n;
   PyObject *__pyx_v_half_n = 0;
   std::vector<std::vector<std::complex<double> > >  __pyx_v_matrix00;
   std::vector<std::vector<std::complex<double> > >  __pyx_v_matrix01;
   std::vector<std::vector<std::complex<double> > >  __pyx_v_matrix10;
   std::vector<std::vector<std::complex<double> > >  __pyx_v_matrix11;
   std::vector<std::complex<double> >  __pyx_v_line0;
@@ -1641,115 +1641,115 @@
   std::vector<std::vector<std::complex<double> > > ::size_type __pyx_t_11;
   std::vector<std::complex<double> > ::size_type __pyx_t_12;
   std::vector<std::complex<double> > ::size_type __pyx_t_13;
   double __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("fft2_square", 0);
+  __Pyx_RefNannySetupContext("_fft2_square", 0);
 
-  /* "fft2/main.pyx":30
+  /* "src/fastfft/fft.pyx":30
  * 
- * cdef void fft2_square(vector[vector[complex[double]]]& matrix):
+ * cdef void _fft2_square(vector[vector[complex[double]]]& matrix):
  *     cdef int n = matrix.size()             # <<<<<<<<<<<<<<
  *     cdef half_n = n // 2
  *     if n == 2:
  */
   __pyx_v_n = __pyx_v_matrix.size();
 
-  /* "fft2/main.pyx":31
- * cdef void fft2_square(vector[vector[complex[double]]]& matrix):
+  /* "src/fastfft/fft.pyx":31
+ * cdef void _fft2_square(vector[vector[complex[double]]]& matrix):
  *     cdef int n = matrix.size()
  *     cdef half_n = n // 2             # <<<<<<<<<<<<<<
  *     if n == 2:
- *         base2x2fft2(matrix)
+ *         _base2x2fft2(matrix)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__Pyx_div_long(__pyx_v_n, 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_half_n = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fft2/main.pyx":32
+  /* "src/fastfft/fft.pyx":32
  *     cdef int n = matrix.size()
  *     cdef half_n = n // 2
  *     if n == 2:             # <<<<<<<<<<<<<<
- *         base2x2fft2(matrix)
+ *         _base2x2fft2(matrix)
  *         return
  */
   __pyx_t_2 = ((__pyx_v_n == 2) != 0);
   if (__pyx_t_2) {
 
-    /* "fft2/main.pyx":33
+    /* "src/fastfft/fft.pyx":33
  *     cdef half_n = n // 2
  *     if n == 2:
- *         base2x2fft2(matrix)             # <<<<<<<<<<<<<<
+ *         _base2x2fft2(matrix)             # <<<<<<<<<<<<<<
  *         return
  * 
  */
-    __pyx_f_4fft2_4main_base2x2fft2(__pyx_v_matrix);
+    __pyx_f_7fastfft_4main__base2x2fft2(__pyx_v_matrix);
 
-    /* "fft2/main.pyx":34
+    /* "src/fastfft/fft.pyx":34
  *     if n == 2:
- *         base2x2fft2(matrix)
+ *         _base2x2fft2(matrix)
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef vector[vector[complex[double]]] matrix00, matrix01, matrix10, matrix11
  */
     goto __pyx_L0;
 
-    /* "fft2/main.pyx":32
+    /* "src/fastfft/fft.pyx":32
  *     cdef int n = matrix.size()
  *     cdef half_n = n // 2
  *     if n == 2:             # <<<<<<<<<<<<<<
- *         base2x2fft2(matrix)
+ *         _base2x2fft2(matrix)
  *         return
  */
   }
 
-  /* "fft2/main.pyx":38
+  /* "src/fastfft/fft.pyx":38
  *     cdef vector[vector[complex[double]]] matrix00, matrix01, matrix10, matrix11
  * 
  *     matrix00.reserve(half_n)             # <<<<<<<<<<<<<<
  *     matrix01.reserve(half_n)
  *     matrix10.reserve(half_n)
  */
   __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_half_n); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_v_matrix00.reserve(__pyx_t_3);
 
-  /* "fft2/main.pyx":39
+  /* "src/fastfft/fft.pyx":39
  * 
  *     matrix00.reserve(half_n)
  *     matrix01.reserve(half_n)             # <<<<<<<<<<<<<<
  *     matrix10.reserve(half_n)
  *     matrix11.reserve(half_n)
  */
   __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_half_n); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
   __pyx_v_matrix01.reserve(__pyx_t_3);
 
-  /* "fft2/main.pyx":40
+  /* "src/fastfft/fft.pyx":40
  *     matrix00.reserve(half_n)
  *     matrix01.reserve(half_n)
  *     matrix10.reserve(half_n)             # <<<<<<<<<<<<<<
  *     matrix11.reserve(half_n)
  * 
  */
   __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_half_n); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L1_error)
   __pyx_v_matrix10.reserve(__pyx_t_3);
 
-  /* "fft2/main.pyx":41
+  /* "src/fastfft/fft.pyx":41
  *     matrix01.reserve(half_n)
  *     matrix10.reserve(half_n)
  *     matrix11.reserve(half_n)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_half_n); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L1_error)
   __pyx_v_matrix11.reserve(__pyx_t_3);
 
-  /* "fft2/main.pyx":47
+  /* "src/fastfft/fft.pyx":47
  *     cdef vector[complex[double]] line1
  *     # todo - redo
  *     for i in range(half_n):             # <<<<<<<<<<<<<<
  *         line0.push_back(I)
  *         line1.push_back(I)
  */
   __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_half_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
@@ -1793,53 +1793,53 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fft2/main.pyx":48
+    /* "src/fastfft/fft.pyx":48
  *     # todo - redo
  *     for i in range(half_n):
  *         line0.push_back(I)             # <<<<<<<<<<<<<<
  *         line1.push_back(I)
  * 
  */
     try {
-      __pyx_v_line0.push_back(__pyx_v_4fft2_4main_I);
+      __pyx_v_line0.push_back(__pyx_v_7fastfft_4main_I);
     } catch(...) {
       __Pyx_CppExn2PyErr();
       __PYX_ERR(0, 48, __pyx_L1_error)
     }
 
-    /* "fft2/main.pyx":49
+    /* "src/fastfft/fft.pyx":49
  *     for i in range(half_n):
  *         line0.push_back(I)
  *         line1.push_back(I)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
     try {
-      __pyx_v_line1.push_back(__pyx_v_4fft2_4main_I);
+      __pyx_v_line1.push_back(__pyx_v_7fastfft_4main_I);
     } catch(...) {
       __Pyx_CppExn2PyErr();
       __PYX_ERR(0, 49, __pyx_L1_error)
     }
 
-    /* "fft2/main.pyx":47
+    /* "src/fastfft/fft.pyx":47
  *     cdef vector[complex[double]] line1
  *     # todo - redo
  *     for i in range(half_n):             # <<<<<<<<<<<<<<
  *         line0.push_back(I)
  *         line1.push_back(I)
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fft2/main.pyx":51
+  /* "src/fastfft/fft.pyx":51
  *         line1.push_back(I)
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(n):
  *             if j % 2 == 0:
  */
   __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
@@ -1886,15 +1886,15 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "fft2/main.pyx":52
+    /* "src/fastfft/fft.pyx":52
  * 
  *     for i in range(n):
  *         for j in range(n):             # <<<<<<<<<<<<<<
  *             if j % 2 == 0:
  *                 line0[j // 2] = matrix[i][j]
  */
     __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
@@ -1941,15 +1941,15 @@
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_j, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "fft2/main.pyx":53
+      /* "src/fastfft/fft.pyx":53
  *     for i in range(n):
  *         for j in range(n):
  *             if j % 2 == 0:             # <<<<<<<<<<<<<<
  *                 line0[j // 2] = matrix[i][j]
  *             else:
  */
       __pyx_t_7 = __Pyx_PyInt_RemainderObjC(__pyx_v_j, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 53, __pyx_L1_error)
@@ -1957,40 +1957,40 @@
       __pyx_t_10 = __Pyx_PyInt_EqObjC(__pyx_t_7, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 53, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (__pyx_t_2) {
 
-        /* "fft2/main.pyx":54
+        /* "src/fastfft/fft.pyx":54
  *         for j in range(n):
  *             if j % 2 == 0:
  *                 line0[j // 2] = matrix[i][j]             # <<<<<<<<<<<<<<
  *             else:
  *                 line1[j // 2] = matrix[i][j]
  */
         __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
         __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
         __pyx_t_10 = __Pyx_PyInt_FloorDivideObjC(__pyx_v_j, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_t_10); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         (__pyx_v_line0[__pyx_t_13]) = ((__pyx_v_matrix[__pyx_t_11])[__pyx_t_12]);
 
-        /* "fft2/main.pyx":53
+        /* "src/fastfft/fft.pyx":53
  *     for i in range(n):
  *         for j in range(n):
  *             if j % 2 == 0:             # <<<<<<<<<<<<<<
  *                 line0[j // 2] = matrix[i][j]
  *             else:
  */
         goto __pyx_L10;
       }
 
-      /* "fft2/main.pyx":56
+      /* "src/fastfft/fft.pyx":56
  *                 line0[j // 2] = matrix[i][j]
  *             else:
  *                 line1[j // 2] = matrix[i][j]             # <<<<<<<<<<<<<<
  *         if i % 2 == 0:
  *             matrix00.push_back(line0)
  */
       /*else*/ {
@@ -2000,25 +2000,25 @@
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_t_10); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 56, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         (__pyx_v_line1[__pyx_t_13]) = ((__pyx_v_matrix[__pyx_t_11])[__pyx_t_12]);
       }
       __pyx_L10:;
 
-      /* "fft2/main.pyx":52
+      /* "src/fastfft/fft.pyx":52
  * 
  *     for i in range(n):
  *         for j in range(n):             # <<<<<<<<<<<<<<
  *             if j % 2 == 0:
  *                 line0[j // 2] = matrix[i][j]
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fft2/main.pyx":57
+    /* "src/fastfft/fft.pyx":57
  *             else:
  *                 line1[j // 2] = matrix[i][j]
  *         if i % 2 == 0:             # <<<<<<<<<<<<<<
  *             matrix00.push_back(line0)
  *             matrix01.push_back(line1)
  */
     __pyx_t_1 = __Pyx_PyInt_RemainderObjC(__pyx_v_i, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
@@ -2026,130 +2026,130 @@
     __pyx_t_10 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (__pyx_t_2) {
 
-      /* "fft2/main.pyx":58
+      /* "src/fastfft/fft.pyx":58
  *                 line1[j // 2] = matrix[i][j]
  *         if i % 2 == 0:
  *             matrix00.push_back(line0)             # <<<<<<<<<<<<<<
  *             matrix01.push_back(line1)
  *         else:
  */
       try {
         __pyx_v_matrix00.push_back(__pyx_v_line0);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 58, __pyx_L1_error)
       }
 
-      /* "fft2/main.pyx":59
+      /* "src/fastfft/fft.pyx":59
  *         if i % 2 == 0:
  *             matrix00.push_back(line0)
  *             matrix01.push_back(line1)             # <<<<<<<<<<<<<<
  *         else:
  *             matrix10.push_back(line0)
  */
       try {
         __pyx_v_matrix01.push_back(__pyx_v_line1);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 59, __pyx_L1_error)
       }
 
-      /* "fft2/main.pyx":57
+      /* "src/fastfft/fft.pyx":57
  *             else:
  *                 line1[j // 2] = matrix[i][j]
  *         if i % 2 == 0:             # <<<<<<<<<<<<<<
  *             matrix00.push_back(line0)
  *             matrix01.push_back(line1)
  */
       goto __pyx_L11;
     }
 
-    /* "fft2/main.pyx":61
+    /* "src/fastfft/fft.pyx":61
  *             matrix01.push_back(line1)
  *         else:
  *             matrix10.push_back(line0)             # <<<<<<<<<<<<<<
  *             matrix11.push_back(line1)
  * 
  */
     /*else*/ {
       try {
         __pyx_v_matrix10.push_back(__pyx_v_line0);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 61, __pyx_L1_error)
       }
 
-      /* "fft2/main.pyx":62
+      /* "src/fastfft/fft.pyx":62
  *         else:
  *             matrix10.push_back(line0)
  *             matrix11.push_back(line1)             # <<<<<<<<<<<<<<
  * 
- *     fft2_square(matrix00)
+ *     _fft2_square(matrix00)
  */
       try {
         __pyx_v_matrix11.push_back(__pyx_v_line1);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 62, __pyx_L1_error)
       }
     }
     __pyx_L11:;
 
-    /* "fft2/main.pyx":51
+    /* "src/fastfft/fft.pyx":51
  *         line1.push_back(I)
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         for j in range(n):
  *             if j % 2 == 0:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fft2/main.pyx":64
+  /* "src/fastfft/fft.pyx":64
  *             matrix11.push_back(line1)
  * 
- *     fft2_square(matrix00)             # <<<<<<<<<<<<<<
- *     fft2_square(matrix01)
- *     fft2_square(matrix10)
+ *     _fft2_square(matrix00)             # <<<<<<<<<<<<<<
+ *     _fft2_square(matrix01)
+ *     _fft2_square(matrix10)
  */
-  __pyx_f_4fft2_4main_fft2_square(__pyx_v_matrix00);
+  __pyx_f_7fastfft_4main__fft2_square(__pyx_v_matrix00);
 
-  /* "fft2/main.pyx":65
+  /* "src/fastfft/fft.pyx":65
  * 
- *     fft2_square(matrix00)
- *     fft2_square(matrix01)             # <<<<<<<<<<<<<<
- *     fft2_square(matrix10)
- *     fft2_square(matrix11)
+ *     _fft2_square(matrix00)
+ *     _fft2_square(matrix01)             # <<<<<<<<<<<<<<
+ *     _fft2_square(matrix10)
+ *     _fft2_square(matrix11)
  */
-  __pyx_f_4fft2_4main_fft2_square(__pyx_v_matrix01);
+  __pyx_f_7fastfft_4main__fft2_square(__pyx_v_matrix01);
 
-  /* "fft2/main.pyx":66
- *     fft2_square(matrix00)
- *     fft2_square(matrix01)
- *     fft2_square(matrix10)             # <<<<<<<<<<<<<<
- *     fft2_square(matrix11)
+  /* "src/fastfft/fft.pyx":66
+ *     _fft2_square(matrix00)
+ *     _fft2_square(matrix01)
+ *     _fft2_square(matrix10)             # <<<<<<<<<<<<<<
+ *     _fft2_square(matrix11)
  * 
  */
-  __pyx_f_4fft2_4main_fft2_square(__pyx_v_matrix10);
+  __pyx_f_7fastfft_4main__fft2_square(__pyx_v_matrix10);
 
-  /* "fft2/main.pyx":67
- *     fft2_square(matrix01)
- *     fft2_square(matrix10)
- *     fft2_square(matrix11)             # <<<<<<<<<<<<<<
+  /* "src/fastfft/fft.pyx":67
+ *     _fft2_square(matrix01)
+ *     _fft2_square(matrix10)
+ *     _fft2_square(matrix11)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_f_4fft2_4main_fft2_square(__pyx_v_matrix11);
+  __pyx_f_7fastfft_4main__fft2_square(__pyx_v_matrix11);
 
-  /* "fft2/main.pyx":72
+  /* "src/fastfft/fft.pyx":72
  *     cdef complex[double] v00, vW10, vW01, vW11
  * 
  *     for i in range(half_n):             # <<<<<<<<<<<<<<
  *         for j in range(half_n):
  *             v00 = matrix00[i][j]
  */
   __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_half_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
@@ -2193,20 +2193,20 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "fft2/main.pyx":73
+    /* "src/fastfft/fft.pyx":73
  * 
  *     for i in range(half_n):
  *         for j in range(half_n):             # <<<<<<<<<<<<<<
  *             v00 = matrix00[i][j]
- *             vW10 = matrix10[i][j] * W_MINUS_PI_2I(n, i)
+ *             vW10 = matrix10[i][j] * W(n, i)
  */
     __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_half_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
       __pyx_t_1 = __pyx_t_4; __Pyx_INCREF(__pyx_t_1); __pyx_t_8 = 0;
       __pyx_t_9 = NULL;
     } else {
@@ -2245,104 +2245,104 @@
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v_j, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "fft2/main.pyx":74
+      /* "src/fastfft/fft.pyx":74
  *     for i in range(half_n):
  *         for j in range(half_n):
  *             v00 = matrix00[i][j]             # <<<<<<<<<<<<<<
- *             vW10 = matrix10[i][j] * W_MINUS_PI_2I(n, i)
- *             vW01 = matrix10[i][j] * W_MINUS_PI_2I(n, j)
+ *             vW10 = matrix10[i][j] * W(n, i)
+ *             vW01 = matrix10[i][j] * W(n, j)
  */
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
       __pyx_v_v00 = ((__pyx_v_matrix00[__pyx_t_11])[__pyx_t_12]);
 
-      /* "fft2/main.pyx":75
+      /* "src/fastfft/fft.pyx":75
  *         for j in range(half_n):
  *             v00 = matrix00[i][j]
- *             vW10 = matrix10[i][j] * W_MINUS_PI_2I(n, i)             # <<<<<<<<<<<<<<
- *             vW01 = matrix10[i][j] * W_MINUS_PI_2I(n, j)
- *             vW11 = matrix10[i][j] * W_MINUS_PI_2I(n, i + i)
+ *             vW10 = matrix10[i][j] * W(n, i)             # <<<<<<<<<<<<<<
+ *             vW01 = matrix10[i][j] * W(n, j)
+ *             vW11 = matrix10[i][j] * W(n, i + i)
  */
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L1_error)
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L1_error)
       __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_v_i); if (unlikely((__pyx_t_14 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L1_error)
-      __pyx_v_vW10 = (((__pyx_v_matrix10[__pyx_t_11])[__pyx_t_12]) * __pyx_f_4fft2_4main_W_MINUS_PI_2I(__pyx_v_n, __pyx_t_14));
+      __pyx_v_vW10 = (((__pyx_v_matrix10[__pyx_t_11])[__pyx_t_12]) * __pyx_f_7fastfft_4main_W(__pyx_v_n, __pyx_t_14));
 
-      /* "fft2/main.pyx":76
+      /* "src/fastfft/fft.pyx":76
  *             v00 = matrix00[i][j]
- *             vW10 = matrix10[i][j] * W_MINUS_PI_2I(n, i)
- *             vW01 = matrix10[i][j] * W_MINUS_PI_2I(n, j)             # <<<<<<<<<<<<<<
- *             vW11 = matrix10[i][j] * W_MINUS_PI_2I(n, i + i)
+ *             vW10 = matrix10[i][j] * W(n, i)
+ *             vW01 = matrix10[i][j] * W(n, j)             # <<<<<<<<<<<<<<
+ *             vW11 = matrix10[i][j] * W(n, i + i)
  * 
  */
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
       __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_v_j); if (unlikely((__pyx_t_14 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
-      __pyx_v_vW01 = (((__pyx_v_matrix10[__pyx_t_11])[__pyx_t_12]) * __pyx_f_4fft2_4main_W_MINUS_PI_2I(__pyx_v_n, __pyx_t_14));
+      __pyx_v_vW01 = (((__pyx_v_matrix10[__pyx_t_11])[__pyx_t_12]) * __pyx_f_7fastfft_4main_W(__pyx_v_n, __pyx_t_14));
 
-      /* "fft2/main.pyx":77
- *             vW10 = matrix10[i][j] * W_MINUS_PI_2I(n, i)
- *             vW01 = matrix10[i][j] * W_MINUS_PI_2I(n, j)
- *             vW11 = matrix10[i][j] * W_MINUS_PI_2I(n, i + i)             # <<<<<<<<<<<<<<
+      /* "src/fastfft/fft.pyx":77
+ *             vW10 = matrix10[i][j] * W(n, i)
+ *             vW01 = matrix10[i][j] * W(n, j)
+ *             vW11 = matrix10[i][j] * W(n, i + i)             # <<<<<<<<<<<<<<
  * 
  *             matrix[i][j] = v00 + vW10 + vW01 + vW11
  */
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       __pyx_t_4 = PyNumber_Add(__pyx_v_i, __pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_14 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_v_vW11 = (((__pyx_v_matrix10[__pyx_t_11])[__pyx_t_12]) * __pyx_f_4fft2_4main_W_MINUS_PI_2I(__pyx_v_n, __pyx_t_14));
+      __pyx_v_vW11 = (((__pyx_v_matrix10[__pyx_t_11])[__pyx_t_12]) * __pyx_f_7fastfft_4main_W(__pyx_v_n, __pyx_t_14));
 
-      /* "fft2/main.pyx":79
- *             vW11 = matrix10[i][j] * W_MINUS_PI_2I(n, i + i)
+      /* "src/fastfft/fft.pyx":79
+ *             vW11 = matrix10[i][j] * W(n, i + i)
  * 
  *             matrix[i][j] = v00 + vW10 + vW01 + vW11             # <<<<<<<<<<<<<<
  *             matrix[i + half_n][j] = v00 - vW10 + vW01 - vW11
  *             matrix[i][j + half_n] = v00 + vW10 - vW01 - vW11
  */
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
       ((__pyx_v_matrix[__pyx_t_11])[__pyx_t_12]) = (((__pyx_v_v00 + __pyx_v_vW10) + __pyx_v_vW01) + __pyx_v_vW11);
 
-      /* "fft2/main.pyx":80
+      /* "src/fastfft/fft.pyx":80
  * 
  *             matrix[i][j] = v00 + vW10 + vW01 + vW11
  *             matrix[i + half_n][j] = v00 - vW10 + vW01 - vW11             # <<<<<<<<<<<<<<
  *             matrix[i][j + half_n] = v00 + vW10 - vW01 - vW11
  *             matrix[i + half_n][j + half_n] = v00 - vW10 - vW01 + vW11
  */
       __pyx_t_4 = PyNumber_Add(__pyx_v_i, __pyx_v_half_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_t_4); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
       ((__pyx_v_matrix[__pyx_t_11])[__pyx_t_12]) = (((__pyx_v_v00 - __pyx_v_vW10) + __pyx_v_vW01) - __pyx_v_vW11);
 
-      /* "fft2/main.pyx":81
+      /* "src/fastfft/fft.pyx":81
  *             matrix[i][j] = v00 + vW10 + vW01 + vW11
  *             matrix[i + half_n][j] = v00 - vW10 + vW01 - vW11
  *             matrix[i][j + half_n] = v00 + vW10 - vW01 - vW11             # <<<<<<<<<<<<<<
  *             matrix[i + half_n][j + half_n] = v00 - vW10 - vW01 + vW11
  * 
  */
       __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
       __pyx_t_4 = PyNumber_Add(__pyx_v_j, __pyx_v_half_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_t_4); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       ((__pyx_v_matrix[__pyx_t_11])[__pyx_t_12]) = (((__pyx_v_v00 + __pyx_v_vW10) - __pyx_v_vW01) - __pyx_v_vW11);
 
-      /* "fft2/main.pyx":82
+      /* "src/fastfft/fft.pyx":82
  *             matrix[i + half_n][j] = v00 - vW10 + vW01 - vW11
  *             matrix[i][j + half_n] = v00 + vW10 - vW01 - vW11
  *             matrix[i + half_n][j + half_n] = v00 - vW10 - vW01 + vW11             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_4 = PyNumber_Add(__pyx_v_i, __pyx_v_half_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
@@ -2351,111 +2351,111 @@
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = PyNumber_Add(__pyx_v_j, __pyx_v_half_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_t_4); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 82, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       ((__pyx_v_matrix[__pyx_t_11])[__pyx_t_12]) = (((__pyx_v_v00 - __pyx_v_vW10) - __pyx_v_vW01) + __pyx_v_vW11);
 
-      /* "fft2/main.pyx":73
+      /* "src/fastfft/fft.pyx":73
  * 
  *     for i in range(half_n):
  *         for j in range(half_n):             # <<<<<<<<<<<<<<
  *             v00 = matrix00[i][j]
- *             vW10 = matrix10[i][j] * W_MINUS_PI_2I(n, i)
+ *             vW10 = matrix10[i][j] * W(n, i)
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "fft2/main.pyx":72
+    /* "src/fastfft/fft.pyx":72
  *     cdef complex[double] v00, vW10, vW01, vW11
  * 
  *     for i in range(half_n):             # <<<<<<<<<<<<<<
  *         for j in range(half_n):
  *             v00 = matrix00[i][j]
  */
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "fft2/main.pyx":29
+  /* "src/fastfft/fft.pyx":29
  * 
  * 
- * cdef void fft2_square(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
+ * cdef void _fft2_square(vector[vector[complex[double]]]& matrix):             # <<<<<<<<<<<<<<
  *     cdef int n = matrix.size()
  *     cdef half_n = n // 2
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_WriteUnraisable("fft2.main.fft2_square", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("fastfft.main._fft2_square", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_half_n);
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_j);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "fft2/main.pyx":85
+/* "src/fastfft/fft.pyx":85
  * 
  * 
- * def py_fft2_square(matrix):             # <<<<<<<<<<<<<<
+ * def fft2(matrix):             # <<<<<<<<<<<<<<
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4fft2_4main_1py_fft2_square(PyObject *__pyx_self, PyObject *__pyx_v_matrix); /*proto*/
-static char __pyx_doc_4fft2_4main_py_fft2_square[] = "py_fft2_square(matrix)";
-static PyMethodDef __pyx_mdef_4fft2_4main_1py_fft2_square = {"py_fft2_square", (PyCFunction)__pyx_pw_4fft2_4main_1py_fft2_square, METH_O, __pyx_doc_4fft2_4main_py_fft2_square};
-static PyObject *__pyx_pw_4fft2_4main_1py_fft2_square(PyObject *__pyx_self, PyObject *__pyx_v_matrix) {
+static PyObject *__pyx_pw_7fastfft_4main_1fft2(PyObject *__pyx_self, PyObject *__pyx_v_matrix); /*proto*/
+static char __pyx_doc_7fastfft_4main_fft2[] = "fft2(matrix)";
+static PyMethodDef __pyx_mdef_7fastfft_4main_1fft2 = {"fft2", (PyCFunction)__pyx_pw_7fastfft_4main_1fft2, METH_O, __pyx_doc_7fastfft_4main_fft2};
+static PyObject *__pyx_pw_7fastfft_4main_1fft2(PyObject *__pyx_self, PyObject *__pyx_v_matrix) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("py_fft2_square (wrapper)", 0);
-  __pyx_r = __pyx_pf_4fft2_4main_py_fft2_square(__pyx_self, ((PyObject *)__pyx_v_matrix));
+  __Pyx_RefNannySetupContext("fft2 (wrapper)", 0);
+  __pyx_r = __pyx_pf_7fastfft_4main_fft2(__pyx_self, ((PyObject *)__pyx_v_matrix));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4fft2_4main_py_fft2_square(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_matrix) {
+static PyObject *__pyx_pf_7fastfft_4main_fft2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_matrix) {
   std::vector<std::vector<std::complex<double> > >  __pyx_v_cpp_matrix;
   PyObject *__pyx_v_line = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   std::vector<std::complex<double> >  __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("py_fft2_square", 0);
+  __Pyx_RefNannySetupContext("fft2", 0);
 
-  /* "fft2/main.pyx":87
- * def py_fft2_square(matrix):
+  /* "src/fastfft/fft.pyx":87
+ * def fft2(matrix):
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))             # <<<<<<<<<<<<<<
  *     for line in matrix:
  *        cpp_matrix.push_back(line)
  */
   __pyx_t_1 = PyObject_Length(__pyx_v_matrix); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 87, __pyx_L1_error)
   __pyx_v_cpp_matrix.reserve(__pyx_t_1);
 
-  /* "fft2/main.pyx":88
+  /* "src/fastfft/fft.pyx":88
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))
  *     for line in matrix:             # <<<<<<<<<<<<<<
  *        cpp_matrix.push_back(line)
- *     fft2_square(cpp_matrix)
+ *     _fft2_square(cpp_matrix)
  */
   if (likely(PyList_CheckExact(__pyx_v_matrix)) || PyTuple_CheckExact(__pyx_v_matrix)) {
     __pyx_t_2 = __pyx_v_matrix; __Pyx_INCREF(__pyx_t_2); __pyx_t_1 = 0;
     __pyx_t_3 = NULL;
   } else {
     __pyx_t_1 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_matrix); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
@@ -2491,72 +2491,72 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_line, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "fft2/main.pyx":89
+    /* "src/fastfft/fft.pyx":89
  *     cpp_matrix.reserve(len(matrix))
  *     for line in matrix:
  *        cpp_matrix.push_back(line)             # <<<<<<<<<<<<<<
- *     fft2_square(cpp_matrix)
+ *     _fft2_square(cpp_matrix)
  *     return cpp_matrix
  */
     __pyx_t_5 = __pyx_convert_vector_from_py_std_3a__3a_complex_3c_double_3e___(__pyx_v_line); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L1_error)
     try {
       __pyx_v_cpp_matrix.push_back(__pyx_t_5);
     } catch(...) {
       __Pyx_CppExn2PyErr();
       __PYX_ERR(0, 89, __pyx_L1_error)
     }
 
-    /* "fft2/main.pyx":88
+    /* "src/fastfft/fft.pyx":88
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))
  *     for line in matrix:             # <<<<<<<<<<<<<<
  *        cpp_matrix.push_back(line)
- *     fft2_square(cpp_matrix)
+ *     _fft2_square(cpp_matrix)
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "fft2/main.pyx":90
+  /* "src/fastfft/fft.pyx":90
  *     for line in matrix:
  *        cpp_matrix.push_back(line)
- *     fft2_square(cpp_matrix)             # <<<<<<<<<<<<<<
+ *     _fft2_square(cpp_matrix)             # <<<<<<<<<<<<<<
  *     return cpp_matrix
  */
-  __pyx_f_4fft2_4main_fft2_square(__pyx_v_cpp_matrix);
+  __pyx_f_7fastfft_4main__fft2_square(__pyx_v_cpp_matrix);
 
-  /* "fft2/main.pyx":91
+  /* "src/fastfft/fft.pyx":91
  *        cpp_matrix.push_back(line)
- *     fft2_square(cpp_matrix)
+ *     _fft2_square(cpp_matrix)
  *     return cpp_matrix             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_complex_3c_double_3e____3e___(__pyx_v_cpp_matrix); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "fft2/main.pyx":85
+  /* "src/fastfft/fft.pyx":85
  * 
  * 
- * def py_fft2_square(matrix):             # <<<<<<<<<<<<<<
+ * def fft2(matrix):             # <<<<<<<<<<<<<<
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("fft2.main.py_fft2_square", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("fastfft.main.fft2", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_line);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -2977,47 +2977,47 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_cpp_matrix, __pyx_k_cpp_matrix, sizeof(__pyx_k_cpp_matrix), 0, 0, 1, 1},
-  {&__pyx_n_s_fft2_main, __pyx_k_fft2_main, sizeof(__pyx_k_fft2_main), 0, 0, 1, 1},
+  {&__pyx_n_s_fastfft_main, __pyx_k_fastfft_main, sizeof(__pyx_k_fastfft_main), 0, 0, 1, 1},
+  {&__pyx_n_s_fft2, __pyx_k_fft2, sizeof(__pyx_k_fft2), 0, 0, 1, 1},
   {&__pyx_n_s_line, __pyx_k_line, sizeof(__pyx_k_line), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_matrix, __pyx_k_matrix, sizeof(__pyx_k_matrix), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_py_fft2_square, __pyx_k_py_fft2_square, sizeof(__pyx_k_py_fft2_square), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_kp_s_src_fft2_main_pyx, __pyx_k_src_fft2_main_pyx, sizeof(__pyx_k_src_fft2_main_pyx), 0, 0, 1, 0},
+  {&__pyx_kp_s_src_fastfft_fft_pyx, __pyx_k_src_fastfft_fft_pyx, sizeof(__pyx_k_src_fastfft_fft_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 47, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "fft2/main.pyx":85
+  /* "src/fastfft/fft.pyx":85
  * 
  * 
- * def py_fft2_square(matrix):             # <<<<<<<<<<<<<<
+ * def fft2(matrix):             # <<<<<<<<<<<<<<
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))
  */
   __pyx_tuple_ = PyTuple_Pack(3, __pyx_n_s_matrix, __pyx_n_s_cpp_matrix, __pyx_n_s_line); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_fft2_main_pyx, __pyx_n_s_py_fft2_square, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_fastfft_fft_pyx, __pyx_n_s_fft2, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3262,22 +3262,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_fft2__main) {
+  if (__pyx_module_is_main_fastfft__main) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "fft2.main")) {
-      if (unlikely(PyDict_SetItemString(modules, "fft2.main", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "fastfft.main")) {
+      if (unlikely(PyDict_SetItemString(modules, "fastfft.main", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3290,63 +3290,63 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "fft2/main.pyx":10
+  /* "src/fastfft/fft.pyx":10
  * 
  * cdef complex[double] PI
  * PI.real(3.141592653589793238462643383279)             # <<<<<<<<<<<<<<
  * cdef complex[double] I
  * I.imag(1)
  */
-  __pyx_v_4fft2_4main_PI.real(3.141592653589793238462643383279);
+  __pyx_v_7fastfft_4main_PI.real(3.141592653589793238462643383279);
 
-  /* "fft2/main.pyx":12
+  /* "src/fastfft/fft.pyx":12
  * PI.real(3.141592653589793238462643383279)
  * cdef complex[double] I
  * I.imag(1)             # <<<<<<<<<<<<<<
  * cdef complex[double] MINUS_PI_2I = PI * I * (-2)
  * cdef complex[double] PI_I = PI * I
  */
-  __pyx_v_4fft2_4main_I.imag(1.0);
+  __pyx_v_7fastfft_4main_I.imag(1.0);
 
-  /* "fft2/main.pyx":13
+  /* "src/fastfft/fft.pyx":13
  * cdef complex[double] I
  * I.imag(1)
  * cdef complex[double] MINUS_PI_2I = PI * I * (-2)             # <<<<<<<<<<<<<<
  * cdef complex[double] PI_I = PI * I
  * 
  */
-  __pyx_v_4fft2_4main_MINUS_PI_2I = ((__pyx_v_4fft2_4main_PI * __pyx_v_4fft2_4main_I) * -2.0);
+  __pyx_v_7fastfft_4main_MINUS_PI_2I = ((__pyx_v_7fastfft_4main_PI * __pyx_v_7fastfft_4main_I) * -2.0);
 
-  /* "fft2/main.pyx":14
+  /* "src/fastfft/fft.pyx":14
  * I.imag(1)
  * cdef complex[double] MINUS_PI_2I = PI * I * (-2)
  * cdef complex[double] PI_I = PI * I             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_v_4fft2_4main_PI_I = (__pyx_v_4fft2_4main_PI * __pyx_v_4fft2_4main_I);
+  __pyx_v_7fastfft_4main_PI_I = (__pyx_v_7fastfft_4main_PI * __pyx_v_7fastfft_4main_I);
 
-  /* "fft2/main.pyx":85
+  /* "src/fastfft/fft.pyx":85
  * 
  * 
- * def py_fft2_square(matrix):             # <<<<<<<<<<<<<<
+ * def fft2(matrix):             # <<<<<<<<<<<<<<
  *     cdef vector[vector[complex[double]]] cpp_matrix
  *     cpp_matrix.reserve(len(matrix))
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4fft2_4main_1py_fft2_square, NULL, __pyx_n_s_fft2_main); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7fastfft_4main_1fft2, NULL, __pyx_n_s_fastfft_main); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_fft2_square, __pyx_t_1) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fft2, __pyx_t_1) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fft2/main.pyx":1
+  /* "src/fastfft/fft.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # distutils: define_macros=CYTHON_CCOMPLEX=0
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3363,19 +3363,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init fft2.main", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init fastfft.main", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init fft2.main");
+    PyErr_SetString(PyExc_ImportError, "init fastfft.main");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

