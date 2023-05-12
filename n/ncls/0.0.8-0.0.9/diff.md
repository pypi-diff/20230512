# Comparing `tmp/ncls-0.0.8.tar.gz` & `tmp/ncls-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ncls-0.0.8.tar", last modified: Wed May  9 08:43:17 2018, max compression
+gzip compressed data, was "dist/ncls-0.0.9.tar", last modified: Wed May  9 08:48:21 2018, max compression
```

## Comparing `ncls-0.0.8.tar` & `ncls-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:43:17.000000 ncls-0.0.8/
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:43:16.000000 ncls-0.0.8/ncls.egg-info/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      303 2018-05-09 08:43:16.000000 ncls-0.0.8/ncls.egg-info/SOURCES.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2018-05-09 08:43:15.000000 ncls-0.0.8/ncls.egg-info/dependency_links.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        9 2018-05-09 08:43:15.000000 ncls-0.0.8/ncls.egg-info/top_level.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      785 2018-05-09 08:43:15.000000 ncls-0.0.8/ncls.egg-info/PKG-INFO
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:43:17.000000 ncls-0.0.8/src/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      581 2018-05-08 19:10:12.000000 ncls-0.0.8/src/cgraph.h
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     7744 2018-05-09 08:40:51.000000 ncls-0.0.8/src/ncls.pyx
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-08 19:10:12.000000 ncls-0.0.8/src/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1967 2018-05-08 19:10:12.000000 ncls-0.0.8/src/cgraph.c
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    34050 2018-05-08 19:10:13.000000 ncls-0.0.8/src/intervaldb.c
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4975 2018-05-08 19:10:13.000000 ncls-0.0.8/src/intervaldb.h
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4264 2018-05-08 19:10:13.000000 ncls-0.0.8/src/default.h
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   863009 2018-05-09 08:43:15.000000 ncls-0.0.8/src/ncls.c
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     3363 2018-05-08 19:10:12.000000 ncls-0.0.8/src/cncls.pxd
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:43:16.000000 ncls-0.0.8/ncls/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      211 2018-05-08 19:10:12.000000 ncls-0.0.8/ncls/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       22 2018-05-09 08:42:58.000000 ncls-0.0.8/ncls/version.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1231 2018-05-09 08:42:48.000000 ncls-0.0.8/README.md
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       41 2018-05-08 19:10:11.000000 ncls-0.0.8/MANIFEST.in
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      289 2018-05-09 08:43:17.000000 ncls-0.0.8/PKG-INFO
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1444 2018-05-08 19:10:12.000000 ncls-0.0.8/setup.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       59 2018-05-09 08:43:17.000000 ncls-0.0.8/setup.cfg
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:48:21.000000 ncls-0.0.9/
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:48:20.000000 ncls-0.0.9/ncls.egg-info/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      303 2018-05-09 08:48:20.000000 ncls-0.0.9/ncls.egg-info/SOURCES.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2018-05-09 08:48:19.000000 ncls-0.0.9/ncls.egg-info/dependency_links.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        9 2018-05-09 08:48:19.000000 ncls-0.0.9/ncls.egg-info/top_level.txt
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      785 2018-05-09 08:48:19.000000 ncls-0.0.9/ncls.egg-info/PKG-INFO
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:48:21.000000 ncls-0.0.9/src/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      581 2018-05-08 19:10:12.000000 ncls-0.0.9/src/cgraph.h
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     7744 2018-05-09 08:47:10.000000 ncls-0.0.9/src/ncls.pyx
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-08 19:10:12.000000 ncls-0.0.9/src/__init__.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1967 2018-05-08 19:10:12.000000 ncls-0.0.9/src/cgraph.c
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    34050 2018-05-08 19:10:13.000000 ncls-0.0.9/src/intervaldb.c
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4975 2018-05-08 19:10:13.000000 ncls-0.0.9/src/intervaldb.h
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4264 2018-05-08 19:10:13.000000 ncls-0.0.9/src/default.h
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   863294 2018-05-09 08:47:45.000000 ncls-0.0.9/src/ncls.c
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     3363 2018-05-08 19:10:12.000000 ncls-0.0.9/src/cncls.pxd
+drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2018-05-09 08:48:20.000000 ncls-0.0.9/ncls/
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      211 2018-05-08 19:10:12.000000 ncls-0.0.9/ncls/__init__.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       22 2018-05-09 08:47:36.000000 ncls-0.0.9/ncls/version.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1231 2018-05-09 08:47:30.000000 ncls-0.0.9/README.md
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       41 2018-05-08 19:10:11.000000 ncls-0.0.9/MANIFEST.in
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      289 2018-05-09 08:48:21.000000 ncls-0.0.9/PKG-INFO
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1444 2018-05-08 19:10:12.000000 ncls-0.0.9/setup.py
+-rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       59 2018-05-09 08:48:21.000000 ncls-0.0.9/setup.cfg
```

### Comparing `ncls-0.0.8/ncls.egg-info/PKG-INFO` & `ncls-0.0.9/ncls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ncls
-Version: 0.0.8
+Version: 0.0.9
 Summary: A wrapper for the nested containment list data structure.
 Home-page: https://github.com/endrebak/pyncls
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: New BSD License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ncls-0.0.8/src/cgraph.h` & `ncls-0.0.9/src/cgraph.h`

 * *Files identical despite different names*

### Comparing `ncls-0.0.8/src/ncls.pyx` & `ncls-0.0.9/src/ncls.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
         return None
 
     cdef check_nonempty(self):
         if self.im:
             return True
         else:
-            return ()
+            return []
 
 
     def __getstate__(self):
 
         cdef char *bp
         cdef size_t size
         cdef cn.FILE *stream
```

### Comparing `ncls-0.0.8/src/cgraph.c` & `ncls-0.0.9/src/cgraph.c`

 * *Files identical despite different names*

### Comparing `ncls-0.0.8/src/intervaldb.c` & `ncls-0.0.9/src/intervaldb.c`

 * *Files identical despite different names*

### Comparing `ncls-0.0.8/src/intervaldb.h` & `ncls-0.0.9/src/intervaldb.h`

 * *Files identical despite different names*

### Comparing `ncls-0.0.8/src/default.h` & `ncls-0.0.9/src/default.h`

 * *Files identical despite different names*

### Comparing `ncls-0.0.8/src/ncls.c` & `ncls-0.0.9/src/ncls.c`

 * *Files 0% similar despite different names*

```diff
@@ -3974,14 +3974,15 @@
  *             return True
  */
 
 static PyObject *__pyx_f_3src_4ncls_4NCLS_check_nonempty(struct __pyx_obj_3src_4ncls_NCLS *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("check_nonempty", 0);
 
   /* "src/ncls.pyx":160
  * 
  *     cdef check_nonempty(self):
  *         if self.im:             # <<<<<<<<<<<<<<
  *             return True
@@ -3991,15 +3992,15 @@
   if (__pyx_t_1) {
 
     /* "src/ncls.pyx":161
  *     cdef check_nonempty(self):
  *         if self.im:
  *             return True             # <<<<<<<<<<<<<<
  *         else:
- *             return ()
+ *             return []
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_True);
     __pyx_r = Py_True;
     goto __pyx_L0;
 
     /* "src/ncls.pyx":160
@@ -4010,34 +4011,40 @@
  *         else:
  */
   }
 
   /* "src/ncls.pyx":163
  *             return True
  *         else:
- *             return ()             # <<<<<<<<<<<<<<
+ *             return []             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_empty_tuple);
-    __pyx_r = __pyx_empty_tuple;
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
   /* "src/ncls.pyx":159
  *         return None
  * 
  *     cdef check_nonempty(self):             # <<<<<<<<<<<<<<
  *         if self.im:
  *             return True
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("src.ncls.NCLS.check_nonempty", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "src/ncls.pyx":166
```

### Comparing `ncls-0.0.8/src/cncls.pxd` & `ncls-0.0.9/src/cncls.pxd`

 * *Files identical despite different names*

### Comparing `ncls-0.0.8/README.md` & `ncls-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 Should do better timings than at first announcement. Still seems much faster (i.e. many times) than even the fastest intervaltrees for most purposes though.
 
 Paper: https://academic.oup.com/bioinformatics/article/23/11/1386/199545
 
 ## Install
 
 ```
-pip install ncls==0.0.8
+pip install ncls==0.0.9
 ```
 
 ## Changelog
 
 ```
-# 2018.05.09 (0.0.8)
-- empty NCLS returns () instead of raising IndexError
+# 2018.05.09 (0.0.9)
+- empty NCLS returns [] instead of raising IndexError
 ```
 
 ## Usage
 
 ```python
 # see the examples/ folder for more examples
 from ncls import NCLS
```

### Comparing `ncls-0.0.8/setup.py` & `ncls-0.0.9/setup.py`

 * *Files identical despite different names*

