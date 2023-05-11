# Comparing `tmp/configparserc-1.3.4.tar.gz` & `tmp/configparserc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/configparserc-1.3.4.tar", last modified: Fri Jan 27 07:29:47 2023, max compression
+gzip compressed data, was "dist/configparserc-1.4.0.tar", last modified: Thu May 11 22:04:25 2023, max compression
```

## Comparing `configparserc-1.3.4.tar` & `configparserc-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 07:29:47.000000 configparserc-1.3.4/
--rw-rw-rw-   0 root         (0) root         (0)    11363 2023-01-27 07:29:14.000000 configparserc-1.3.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      187 2023-01-27 07:29:14.000000 configparserc-1.3.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-01-27 07:29:14.000000 configparserc-1.3.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5253 2023-01-27 07:29:47.000000 configparserc-1.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3636 2023-01-27 07:29:14.000000 configparserc-1.3.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc/
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-01-27 07:29:14.000000 configparserc-1.3.4/configparserc/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1394112 2023-01-27 07:29:46.000000 configparserc-1.3.4/configparserc/config.c
--rw-rw-rw-   0 root         (0) root         (0)     3082 2023-01-27 07:29:14.000000 configparserc-1.3.4/configparserc/config.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc/include/
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-01-27 07:29:14.000000 configparserc-1.3.4/configparserc/include/_config.h
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-27 07:29:14.000000 configparserc-1.3.4/configparserc/py.typed
--rw-r--r--   0 root         (0) root         (0)   341217 2023-01-27 07:29:45.000000 configparserc-1.3.4/configparserc/tools.c
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-01-27 07:29:14.000000 configparserc-1.3.4/configparserc/tools.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5253 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-27 07:29:47.000000 configparserc-1.3.4/configparserc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-01-27 07:29:47.000000 configparserc-1.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    14447 2023-01-27 07:29:14.000000 configparserc-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11363 2023-05-11 22:03:49.000000 configparserc-1.4.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      187 2023-05-11 22:03:49.000000 configparserc-1.4.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-05-11 22:03:49.000000 configparserc-1.4.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-05-11 22:04:25.000000 configparserc-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2023-05-11 22:03:49.000000 configparserc-1.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/configparserc/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1435996 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc/config.c
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/config.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/configparserc/include/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/include/_config.h
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/py.typed
+-rw-r--r--   0 root         (0) root         (0)   341280 2023-05-11 22:04:21.000000 configparserc-1.4.0/configparserc/tools.c
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/tools.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/configparserc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-11 22:04:25.000000 configparserc-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    14643 2023-05-11 22:03:49.000000 configparserc-1.4.0/setup.py
```

### Comparing `configparserc-1.3.4/LICENSE` & `configparserc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configparserc-1.3.4/NOTICE` & `configparserc-1.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `configparserc-1.3.4/PKG-INFO` & `configparserc-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configparserc
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python (Cython) based implementation of ConfigParser based on POSIX and stdlib functions.
 Home-page: https://gitlab.com/onegreyonewhite/configparserc
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: Apache Software License
 Project-URL: Issue Tracker, https://gitlab.com/onegreyonewhite/configparserc/-/issues
 Project-URL: Source Code, https://gitlab.com/onegreyonewhite/configparserc.git
@@ -54,14 +54,15 @@
 Support converting values in formats:
 
 *  `StrType` - force convert to string all values (defaults too).
 *  `IntType` - convert values to integer (include suffixes 'K', 'M' and 'G' multiples of 1000).
 *  `BytesSizeType` - convert values to integer size of bytes (include suffixes 'K', 'M' and 'G' multiples of 1024).
 *  `BoolType` - convert 'False', 'false', 'True' and 'true' to valid Python bool type.
 *  `IntSecondsType` - convert time to seconds. Uses 'pytimeparse' python package.
+*  `TimedeltaType` - convert time to timdelta/relativedelta(if installed). Uses 'pytimeparse' python package.
 *  `ListType` - convert separated by symbol (default is comma) string to list of values.
 *  `JsonType` - convert json value to python value.
 
 
 Usage
 -----
```

### Comparing `configparserc-1.3.4/README.rst` & `configparserc-1.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Support converting values in formats:
 
 *  `StrType` - force convert to string all values (defaults too).
 *  `IntType` - convert values to integer (include suffixes 'K', 'M' and 'G' multiples of 1000).
 *  `BytesSizeType` - convert values to integer size of bytes (include suffixes 'K', 'M' and 'G' multiples of 1024).
 *  `BoolType` - convert 'False', 'false', 'True' and 'true' to valid Python bool type.
 *  `IntSecondsType` - convert time to seconds. Uses 'pytimeparse' python package.
+*  `TimedeltaType` - convert time to timdelta/relativedelta(if installed). Uses 'pytimeparse' python package.
 *  `ListType` - convert separated by symbol (default is comma) string to list of values.
 *  `JsonType` - convert json value to python value.
 
 
 Usage
 -----
```

### Comparing `configparserc-1.3.4/configparserc/__init__.py` & `configparserc-1.4.0/configparserc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 """
 
-__version__ = '1.3.4'
+__version__ = '1.4.0'
```

### Comparing `configparserc-1.3.4/configparserc/config.c` & `configparserc-1.4.0/configparserc/config.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "configparserc/include/_config.h"
         ],
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1009,14 +1009,15 @@
 struct __pyx_obj_13configparserc_6config_ParseError;
 struct __pyx_obj_13configparserc_6config_BaseType;
 struct __pyx_obj_13configparserc_6config_StrType;
 struct __pyx_obj_13configparserc_6config_IntType;
 struct __pyx_obj_13configparserc_6config_BytesSizeType;
 struct __pyx_obj_13configparserc_6config_BoolType;
 struct __pyx_obj_13configparserc_6config_IntSecondsType;
+struct __pyx_obj_13configparserc_6config_TimedeltaType;
 struct __pyx_obj_13configparserc_6config_ListType;
 struct __pyx_obj_13configparserc_6config_JsonType;
 struct __pyx_obj_13configparserc_6config___BaseDict;
 struct __pyx_obj_13configparserc_6config_ConfigParserC;
 struct __pyx_obj_13configparserc_6config_Section;
 struct __pyx_obj_13configparserc_6config_AppendSection;
 struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py;
@@ -1034,27 +1035,27 @@
  *         str key
  */
 struct __pyx_opt_args_13configparserc_6config___get_or_create_section_recursive {
   int __pyx_n;
   int carret_pos;
 };
 
-/* "configparserc/config.pyx":585
+/* "configparserc/config.pyx":590
  *         return key
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):             # <<<<<<<<<<<<<<
  *         if PyDict_Contains(self.__type_map, key) == 1:
  *             return <object>PyDict_GetItem(self.__type_map, key)
  */
 struct __pyx_opt_args_13configparserc_6config_7Section_get_type_conversation_instance {
   int __pyx_n;
   PyObject *__pyx_default;
 };
 
-/* "configparserc/config.pyx":590
+/* "configparserc/config.pyx":595
  *         return getattr(self, 'type_'+key, default)
  * 
  *     cdef object type_conversation(self, str key, object value, BaseType conv_class=None):             # <<<<<<<<<<<<<<
  *         cdef BaseType conversation_cls
  * 
  */
 struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation {
@@ -1169,49 +1170,61 @@
   struct __pyx_obj_13configparserc_6config_BaseType __pyx_base;
 };
 
 
 /* "configparserc/config.pyx":175
  * 
  * 
+ * cdef class TimedeltaType(BaseType):             # <<<<<<<<<<<<<<
+ *     def convert(self, value):
+ *         return pytimeparse2.parse(str(value), raise_exception=True, as_timedelta=True)
+ */
+struct __pyx_obj_13configparserc_6config_TimedeltaType {
+  struct __pyx_obj_13configparserc_6config_BaseType __pyx_base;
+};
+
+
+/* "configparserc/config.pyx":180
+ * 
+ * 
  * cdef class ListType(BaseType):             # <<<<<<<<<<<<<<
  *     cdef str separator
  * 
  */
 struct __pyx_obj_13configparserc_6config_ListType {
   struct __pyx_obj_13configparserc_6config_BaseType __pyx_base;
   PyObject *separator;
 };
 
 
-/* "configparserc/config.pyx":192
+/* "configparserc/config.pyx":197
  * 
  * 
  * cdef class JsonType(BaseType):             # <<<<<<<<<<<<<<
  *     def convert(self, value):
  *         if not isinstance(value, str):
  */
 struct __pyx_obj_13configparserc_6config_JsonType {
   struct __pyx_obj_13configparserc_6config_BaseType __pyx_base;
 };
 
 
-/* "configparserc/config.pyx":202
+/* "configparserc/config.pyx":207
  * 
  * 
  * cdef class __BaseDict(dict):             # <<<<<<<<<<<<<<
  * 
  *     def __eq__(self, other):
  */
 struct __pyx_obj_13configparserc_6config___BaseDict {
   PyDictObject __pyx_base;
 };
 
 
-/* "configparserc/config.pyx":218
+/* "configparserc/config.pyx":223
  * 
  * 
  * cdef class ConfigParserC(__BaseDict):             # <<<<<<<<<<<<<<
  * 
  *     section_regex = re.compile(r"^\[(?P<section>(.+))\].*$", re.MULTILINE)
  */
 struct __pyx_obj_13configparserc_6config_ConfigParserC {
@@ -1220,15 +1233,15 @@
   PyObject *__pyx___sections_map;
   PyObject *section_defaults;
   PyObject *__pyx___format_kwargs;
   PyObject *__pyx___format_exclude_sections;
 };
 
 
-/* "configparserc/config.pyx":436
+/* "configparserc/config.pyx":441
  * 
  * 
  * cdef class Section(__BaseDict):             # <<<<<<<<<<<<<<
  *     cdef:
  *         str name
  */
 struct __pyx_obj_13configparserc_6config_Section {
@@ -1236,15 +1249,15 @@
   struct __pyx_vtabstruct_13configparserc_6config_Section *__pyx_vtab;
   PyObject *name;
   struct __pyx_obj_13configparserc_6config_ConfigParserC *config;
   PyObject *__pyx___type_map;
 };
 
 
-/* "configparserc/config.pyx":640
+/* "configparserc/config.pyx":645
  * 
  * 
  * cdef class AppendSection(Section):             # <<<<<<<<<<<<<<
  *     def __init__(self, *args, **kwargs):
  *         super().__init__(*args, **kwargs)
  */
 struct __pyx_obj_13configparserc_6config_AppendSection {
@@ -1272,15 +1285,15 @@
 struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_unicode____Section___to_py {
   PyObject_HEAD
   PyObject *(*__pyx_v_f)(struct __pyx_obj_13configparserc_6config_Section *);
 };
 
 
 
-/* "configparserc/config.pyx":218
+/* "configparserc/config.pyx":223
  * 
  * 
  * cdef class ConfigParserC(__BaseDict):             # <<<<<<<<<<<<<<
  * 
  *     section_regex = re.compile(r"^\[(?P<section>(.+))\].*$", re.MULTILINE)
  */
 
@@ -1292,15 +1305,15 @@
   int (*_parse_file)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, FILE *, unsigned PY_LONG_LONG);
   PyObject *(*_parse_file_by_name)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, char *);
   PyObject *(*_parse_text)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, char *);
 };
 static struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *__pyx_vtabptr_13configparserc_6config_ConfigParserC;
 
 
-/* "configparserc/config.pyx":436
+/* "configparserc/config.pyx":441
  * 
  * 
  * cdef class Section(__BaseDict):             # <<<<<<<<<<<<<<
  *     cdef:
  *         str name
  */
 
@@ -1313,15 +1326,15 @@
   PyObject *(*__pyx___get_default_value)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *);
   PyObject *(*get_type_conversation_instance)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *, struct __pyx_opt_args_13configparserc_6config_7Section_get_type_conversation_instance *__pyx_optional_args);
   PyObject *(*type_conversation)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *, PyObject *, struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation *__pyx_optional_args);
 };
 static struct __pyx_vtabstruct_13configparserc_6config_Section *__pyx_vtabptr_13configparserc_6config_Section;
 
 
-/* "configparserc/config.pyx":640
+/* "configparserc/config.pyx":645
  * 
  * 
  * cdef class AppendSection(Section):             # <<<<<<<<<<<<<<
  *     def __init__(self, *args, **kwargs):
  *         super().__init__(*args, **kwargs)
  */
 
@@ -2175,20 +2188,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetNameInClass.proto */
 #define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
 static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
 
 /* CLineInTraceback.proto */
@@ -2302,14 +2323,15 @@
 static PyTypeObject *__pyx_ptype_13configparserc_6config_ParseError = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_BaseType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_StrType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_IntType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_BytesSizeType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_BoolType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_IntSecondsType = 0;
+static PyTypeObject *__pyx_ptype_13configparserc_6config_TimedeltaType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_ListType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_JsonType = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config___BaseDict = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_ConfigParserC = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_Section = 0;
 static PyTypeObject *__pyx_ptype_13configparserc_6config_AppendSection = 0;
 static PyTypeObject *__pyx_ptype___pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py = 0;
@@ -2324,14 +2346,15 @@
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_ParseError__set_state(struct __pyx_obj_13configparserc_6config_ParseError *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_BaseType__set_state(struct __pyx_obj_13configparserc_6config_BaseType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_StrType__set_state(struct __pyx_obj_13configparserc_6config_StrType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_IntType__set_state(struct __pyx_obj_13configparserc_6config_IntType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_BytesSizeType__set_state(struct __pyx_obj_13configparserc_6config_BytesSizeType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_BoolType__set_state(struct __pyx_obj_13configparserc_6config_BoolType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_IntSecondsType__set_state(struct __pyx_obj_13configparserc_6config_IntSecondsType *, PyObject *); /*proto*/
+static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_TimedeltaType__set_state(struct __pyx_obj_13configparserc_6config_TimedeltaType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_JsonType__set_state(struct __pyx_obj_13configparserc_6config_JsonType *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle___BaseDict__set_state(struct __pyx_obj_13configparserc_6config___BaseDict *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_ConfigParserC__set_state(struct __pyx_obj_13configparserc_6config_ConfigParserC *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_Section__set_state(struct __pyx_obj_13configparserc_6config_Section *, PyObject *); /*proto*/
 static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_AppendSection__set_state(struct __pyx_obj_13configparserc_6config_AppendSection *, PyObject *); /*proto*/
 static PyObject *__Pyx_CFunc_dict____dict____unicode___to_py(PyObject *(*)(PyObject *, PyObject *)); /*proto*/
 static PyObject *__Pyx_CFunc_bint____object___to_py(int (*)(PyObject *)); /*proto*/
@@ -2475,21 +2498,23 @@
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_CSafeLoader[] = "CSafeLoader";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_YAML_LOADER[] = "YAML_LOADER";
 static const char __pyx_k_cfunc_to_py[] = "cfunc.to_py";
 static const char __pyx_k_str_convert[] = "str_convert";
 static const char __pyx_k_subsections[] = "subsections";
+static const char __pyx_k_as_timedelta[] = "as_timedelta";
 static const char __pyx_k_pytimeparse2[] = "pytimeparse2";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_section_name[] = "section_name";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_AppendSection[] = "AppendSection";
 static const char __pyx_k_BytesSizeType[] = "BytesSizeType";
 static const char __pyx_k_ConfigParserC[] = "ConfigParserC";
+static const char __pyx_k_TimedeltaType[] = "TimedeltaType";
 static const char __pyx_k_format_kwargs[] = "format_kwargs";
 static const char __pyx_k_format_string[] = "format_string";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_section_class[] = "section_class_";
 static const char __pyx_k_section_regex[] = "section_regex";
 static const char __pyx_k_IntSecondsType[] = "IntSecondsType";
 static const char __pyx_k_parse_yaml_file[] = "parse_yaml_file";
@@ -2517,14 +2542,15 @@
 static const char __pyx_k_format_exclude_sections[] = "format_exclude_sections";
 static const char __pyx_k_generate_section_string[] = "generate_section_string";
 static const char __pyx_k_pyx_unpickle_ParseError[] = "__pyx_unpickle_ParseError";
 static const char __pyx_k_pyx_unpickle___BaseDict[] = "__pyx_unpickle___BaseDict";
 static const char __pyx_k_pyx_unpickle_AppendSection[] = "__pyx_unpickle_AppendSection";
 static const char __pyx_k_pyx_unpickle_BytesSizeType[] = "__pyx_unpickle_BytesSizeType";
 static const char __pyx_k_pyx_unpickle_ConfigParserC[] = "__pyx_unpickle_ConfigParserC";
+static const char __pyx_k_pyx_unpickle_TimedeltaType[] = "__pyx_unpickle_TimedeltaType";
 static const char __pyx_k_P_key_s_s_0_s_0_P_value_s_0[] = "^(?P<key>([^\\s]+?))[\\s]{0,}=[\\s]{0,}(?P<value>(.*?))[\\s]{0,}$";
 static const char __pyx_k_pyx_unpickle_IntSecondsType[] = "__pyx_unpickle_IntSecondsType";
 static const char __pyx_k_Pyx_CFunc_unicode____Section[] = "__Pyx_CFunc_unicode____Section___to_py.<locals>.wrap";
 static const char __pyx_k_Pyx_CFunc_bint____object___to[] = "__Pyx_CFunc_bint____object___to_py.<locals>.wrap";
 static const char __pyx_k_Pyx_CFunc_dict____dict____unic[] = "__Pyx_CFunc_dict____dict____unicode___to_py.<locals>.wrap";
 static const char __pyx_k_pyx_unpickle_ConfigParserExcep[] = "__pyx_unpickle_ConfigParserException";
 static const char __pyx_k_P_val_d_P_mul_KMGTkmgt_0_1_bB_0[] = "(?P<val>[\\d\\.]+)(?P<mul>[KMGTkmgt]{0,1})[bB]{0,1}";
@@ -2572,14 +2598,15 @@
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_Pyx_CFunc_bint____object___to;
 static PyObject *__pyx_n_s_Pyx_CFunc_dict____dict____unic;
 static PyObject *__pyx_n_s_Pyx_CFunc_unicode____Section;
 static PyObject *__pyx_n_s_SafeLoader;
 static PyObject *__pyx_n_s_Section;
 static PyObject *__pyx_n_s_StrType;
+static PyObject *__pyx_n_s_TimedeltaType;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_YAML_LOADER;
 static PyObject *__pyx_kp_u__10;
 static PyObject *__pyx_kp_u__11;
 static PyObject *__pyx_kp_u__12;
 static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_kp_u__20;
@@ -2588,14 +2615,15 @@
 static PyObject *__pyx_kp_u__23;
 static PyObject *__pyx_kp_u__24;
 static PyObject *__pyx_n_u__3;
 static PyObject *__pyx_kp_u__4;
 static PyObject *__pyx_kp_u__8;
 static PyObject *__pyx_kp_u__9;
 static PyObject *__pyx_n_s_all;
+static PyObject *__pyx_n_s_as_timedelta;
 static PyObject *__pyx_n_u_b;
 static PyObject *__pyx_n_s_cfunc_to_py;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_collect;
 static PyObject *__pyx_n_s_compile;
 static PyObject *__pyx_n_s_config;
@@ -2676,14 +2704,15 @@
 static PyObject *__pyx_n_s_pyx_unpickle_Empty;
 static PyObject *__pyx_n_s_pyx_unpickle_IntSecondsType;
 static PyObject *__pyx_n_s_pyx_unpickle_IntType;
 static PyObject *__pyx_n_s_pyx_unpickle_JsonType;
 static PyObject *__pyx_n_s_pyx_unpickle_ParseError;
 static PyObject *__pyx_n_s_pyx_unpickle_Section;
 static PyObject *__pyx_n_s_pyx_unpickle_StrType;
+static PyObject *__pyx_n_s_pyx_unpickle_TimedeltaType;
 static PyObject *__pyx_n_s_pyx_unpickle___BaseDict;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_raise_exception;
 static PyObject *__pyx_n_s_re;
 static PyObject *__pyx_n_s_re_size;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_2;
@@ -2752,14 +2781,17 @@
 static PyObject *__pyx_pf_13configparserc_6config_13BytesSizeType_4__setstate_cython__(struct __pyx_obj_13configparserc_6config_BytesSizeType *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8BoolType_convert(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_BoolType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8BoolType_2__reduce_cython__(struct __pyx_obj_13configparserc_6config_BoolType *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8BoolType_4__setstate_cython__(struct __pyx_obj_13configparserc_6config_BoolType *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_14IntSecondsType_convert(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_IntSecondsType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_14IntSecondsType_2__reduce_cython__(struct __pyx_obj_13configparserc_6config_IntSecondsType *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_14IntSecondsType_4__setstate_cython__(struct __pyx_obj_13configparserc_6config_IntSecondsType *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_13TimedeltaType_convert(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_13TimedeltaType_2__reduce_cython__(struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_13TimedeltaType_4__setstate_cython__(struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_13configparserc_6config_8ListType___cinit__(struct __pyx_obj_13configparserc_6config_ListType *__pyx_v_self, PyObject *__pyx_v_separator); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8ListType_2convert(struct __pyx_obj_13configparserc_6config_ListType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8ListType_4str_convert(struct __pyx_obj_13configparserc_6config_ListType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8ListType_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_ListType *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8ListType_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_ListType *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8JsonType_convert(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_JsonType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8JsonType_2str_convert(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_JsonType *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
@@ -2818,31 +2850,33 @@
 static PyObject *__pyx_pf_13configparserc_6config_4__pyx_unpickle_ParseError(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_6__pyx_unpickle_BaseType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_8__pyx_unpickle_StrType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_10__pyx_unpickle_IntType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_12__pyx_unpickle_BytesSizeType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_14__pyx_unpickle_BoolType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_13configparserc_6config_16__pyx_unpickle_IntSecondsType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_13configparserc_6config_18__pyx_unpickle_JsonType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_13configparserc_6config_20__pyx_unpickle___BaseDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_13configparserc_6config_22__pyx_unpickle_ConfigParserC(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_13configparserc_6config_24__pyx_unpickle_Section(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_13configparserc_6config_26__pyx_unpickle_AppendSection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_18__pyx_unpickle_TimedeltaType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_20__pyx_unpickle_JsonType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_22__pyx_unpickle___BaseDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_24__pyx_unpickle_ConfigParserC(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_26__pyx_unpickle_Section(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13configparserc_6config_28__pyx_unpickle_AppendSection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_11cfunc_dot_to_py_43__Pyx_CFunc_dict____dict____unicode___to_py_wrap(PyObject *__pyx_self, PyObject *__pyx_v_collect, PyObject *__pyx_v_key); /* proto */
 static PyObject *__pyx_pf_11cfunc_dot_to_py_34__Pyx_CFunc_bint____object___to_py_wrap(PyObject *__pyx_self, PyObject *__pyx_v_obj); /* proto */
 static PyObject *__pyx_pf_11cfunc_dot_to_py_38__Pyx_CFunc_unicode____Section___to_py_wrap(PyObject *__pyx_self, struct __pyx_obj_13configparserc_6config_Section *__pyx_v_section); /* proto */
 static PyObject *__pyx_tp_new_13configparserc_6config_Empty(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_ConfigParserException(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_ParseError(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_BaseType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_StrType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_IntType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_BytesSizeType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_BoolType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_IntSecondsType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_13configparserc_6config_TimedeltaType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_ListType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_JsonType(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config___BaseDict(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_ConfigParserC(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_Section(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_13configparserc_6config_AppendSection(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -2868,50 +2902,52 @@
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_slice__14;
 static PyObject *__pyx_slice__17;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__38;
-static PyObject *__pyx_tuple__40;
-static PyObject *__pyx_tuple__42;
-static PyObject *__pyx_tuple__44;
-static PyObject *__pyx_tuple__46;
-static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__45;
+static PyObject *__pyx_tuple__47;
 static PyObject *__pyx_tuple__49;
 static PyObject *__pyx_tuple__50;
 static PyObject *__pyx_tuple__51;
 static PyObject *__pyx_tuple__52;
 static PyObject *__pyx_tuple__53;
 static PyObject *__pyx_tuple__54;
 static PyObject *__pyx_tuple__55;
 static PyObject *__pyx_tuple__56;
 static PyObject *__pyx_tuple__57;
 static PyObject *__pyx_tuple__58;
 static PyObject *__pyx_tuple__59;
 static PyObject *__pyx_tuple__60;
 static PyObject *__pyx_tuple__61;
+static PyObject *__pyx_tuple__62;
+static PyObject *__pyx_tuple__63;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__27;
 static PyObject *__pyx_codeobj__28;
 static PyObject *__pyx_codeobj__29;
 static PyObject *__pyx_codeobj__30;
 static PyObject *__pyx_codeobj__31;
 static PyObject *__pyx_codeobj__32;
 static PyObject *__pyx_codeobj__33;
 static PyObject *__pyx_codeobj__34;
 static PyObject *__pyx_codeobj__35;
 static PyObject *__pyx_codeobj__36;
 static PyObject *__pyx_codeobj__37;
-static PyObject *__pyx_codeobj__39;
-static PyObject *__pyx_codeobj__41;
-static PyObject *__pyx_codeobj__43;
-static PyObject *__pyx_codeobj__45;
-static PyObject *__pyx_codeobj__47;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_codeobj__44;
+static PyObject *__pyx_codeobj__46;
+static PyObject *__pyx_codeobj__48;
 /* Late includes */
 
 /* "configparserc/config.pyx":45
  * 
  * 
  * cdef dict __get_dict_from_dict_for_reduce(dict collect, str key):             # <<<<<<<<<<<<<<
  *     if PyDict_Contains(collect, key) == 1:
@@ -7128,15 +7164,399 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":178
+/* "configparserc/config.pyx":176
+ * 
+ * cdef class TimedeltaType(BaseType):
+ *     def convert(self, value):             # <<<<<<<<<<<<<<
+ *         return pytimeparse2.parse(str(value), raise_exception=True, as_timedelta=True)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13configparserc_6config_13TimedeltaType_1convert(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_13configparserc_6config_13TimedeltaType_1convert(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("convert (wrapper)", 0);
+  __pyx_r = __pyx_pf_13configparserc_6config_13TimedeltaType_convert(((struct __pyx_obj_13configparserc_6config_TimedeltaType *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13configparserc_6config_13TimedeltaType_convert(CYTHON_UNUSED struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v_self, PyObject *__pyx_v_value) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("convert", 0);
+  __Pyx_TraceCall("convert", __pyx_f[0], 176, 0, __PYX_ERR(0, 176, __pyx_L1_error));
+
+  /* "configparserc/config.pyx":177
+ * cdef class TimedeltaType(BaseType):
+ *     def convert(self, value):
+ *         return pytimeparse2.parse(str(value), raise_exception=True, as_timedelta=True)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pytimeparse2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_parse); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_raise_exception, Py_True) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_as_timedelta, Py_True) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
+  goto __pyx_L0;
+
+  /* "configparserc/config.pyx":176
+ * 
+ * cdef class TimedeltaType(BaseType):
+ *     def convert(self, value):             # <<<<<<<<<<<<<<
+ *         return pytimeparse2.parse(str(value), raise_exception=True, as_timedelta=True)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("configparserc.config.TimedeltaType.convert", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13configparserc_6config_13TimedeltaType_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_13configparserc_6config_13TimedeltaType_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_13configparserc_6config_13TimedeltaType_2__reduce_cython__(((struct __pyx_obj_13configparserc_6config_TimedeltaType *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13configparserc_6config_13TimedeltaType_2__reduce_cython__(struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
+
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = ()             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ */
+  __Pyx_INCREF(__pyx_empty_tuple);
+  __pyx_v_state = __pyx_empty_tuple;
+
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = ()
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
+ */
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v__dict = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":7
+ *     state = ()
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
+
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = False
+ */
+    __pyx_v_use_setstate = 1;
+
+    /* "(tree fragment)":7
+ *     state = ()
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+    goto __pyx_L3;
+  }
+
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = False             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, None), state
+ */
+  /*else*/ {
+    __pyx_v_use_setstate = 0;
+  }
+  __pyx_L3:;
+
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = False
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, None), state
+ *     else:
+ */
+  __pyx_t_3 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = False
+ *     if use_setstate:
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, state)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_TimedeltaType); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_222419149);
+    __Pyx_GIVEREF(__pyx_int_222419149);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_222419149);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
+    goto __pyx_L0;
+
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = False
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, None), state
+ *     else:
+ */
+  }
+
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, None), state
+ *     else:
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_TimedeltaType__set_state(self, __pyx_state)
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_TimedeltaType); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_222419149);
+    __Pyx_GIVEREF(__pyx_int_222419149);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_222419149);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_5 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
+  }
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("configparserc.config.TimedeltaType.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_TimedeltaType__set_state(self, __pyx_state)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13configparserc_6config_13TimedeltaType_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_13configparserc_6config_13TimedeltaType_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_13configparserc_6config_13TimedeltaType_4__setstate_cython__(((struct __pyx_obj_13configparserc_6config_TimedeltaType *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13configparserc_6config_13TimedeltaType_4__setstate_cython__(struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
+
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, state)
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_TimedeltaType__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
+ */
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_13configparserc_6config___pyx_unpickle_TimedeltaType__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_TimedeltaType, (type(self), 0xd41d8cd, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_TimedeltaType__set_state(self, __pyx_state)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("configparserc.config.TimedeltaType.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "configparserc/config.pyx":183
  *     cdef str separator
  * 
  *     def __cinit__(self, separator=','):             # <<<<<<<<<<<<<<
  *         self.separator = separator
  * 
  */
 
@@ -7168,29 +7588,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separator);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 178, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_separator = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 178, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.ListType.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_8ListType___cinit__(((struct __pyx_obj_13configparserc_6config_ListType *)__pyx_v_self), __pyx_v_separator);
 
@@ -7204,33 +7624,33 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
-  __Pyx_TraceCall("__cinit__", __pyx_f[0], 178, 0, __PYX_ERR(0, 178, __pyx_L1_error));
+  __Pyx_TraceCall("__cinit__", __pyx_f[0], 183, 0, __PYX_ERR(0, 183, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":179
+  /* "configparserc/config.pyx":184
  * 
  *     def __cinit__(self, separator=','):
  *         self.separator = separator             # <<<<<<<<<<<<<<
  * 
  *     def convert(self, value):
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_separator))||((__pyx_v_separator) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_separator)->tp_name), 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_separator))||((__pyx_v_separator) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_separator)->tp_name), 0))) __PYX_ERR(0, 184, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_separator;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->separator);
   __Pyx_DECREF(__pyx_v_self->separator);
   __pyx_v_self->separator = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":178
+  /* "configparserc/config.pyx":183
  *     cdef str separator
  * 
  *     def __cinit__(self, separator=','):             # <<<<<<<<<<<<<<
  *         self.separator = separator
  * 
  */
 
@@ -7243,15 +7663,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":181
+/* "configparserc/config.pyx":186
  *         self.separator = separator
  * 
  *     def convert(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, (str, bytes)):
  *             value = filter(bool, value.split(self.separator))
  */
 
@@ -7278,18 +7698,18 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert", 0);
-  __Pyx_TraceCall("convert", __pyx_f[0], 181, 0, __PYX_ERR(0, 181, __pyx_L1_error));
+  __Pyx_TraceCall("convert", __pyx_f[0], 186, 0, __PYX_ERR(0, 186, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "configparserc/config.pyx":182
+  /* "configparserc/config.pyx":187
  * 
  *     def convert(self, value):
  *         if isinstance(value, (str, bytes)):             # <<<<<<<<<<<<<<
  *             value = filter(bool, value.split(self.separator))
  *         elif isinstance(value, (int, float)):
  */
   __pyx_t_2 = PyUnicode_Check(__pyx_v_value); 
@@ -7302,63 +7722,63 @@
   __pyx_t_3 = PyBytes_Check(__pyx_v_value); 
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":183
+    /* "configparserc/config.pyx":188
  *     def convert(self, value):
  *         if isinstance(value, (str, bytes)):
  *             value = filter(bool, value.split(self.separator))             # <<<<<<<<<<<<<<
  *         elif isinstance(value, (int, float)):
  *             return value,
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_split); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_split); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_self->separator) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_self->separator);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(((PyObject*)&PyBool_Type));
     __Pyx_GIVEREF(((PyObject*)&PyBool_Type));
     PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject*)&PyBool_Type));
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":182
+    /* "configparserc/config.pyx":187
  * 
  *     def convert(self, value):
  *         if isinstance(value, (str, bytes)):             # <<<<<<<<<<<<<<
  *             value = filter(bool, value.split(self.separator))
  *         elif isinstance(value, (int, float)):
  */
     goto __pyx_L3;
   }
 
-  /* "configparserc/config.pyx":184
+  /* "configparserc/config.pyx":189
  *         if isinstance(value, (str, bytes)):
  *             value = filter(bool, value.split(self.separator))
  *         elif isinstance(value, (int, float)):             # <<<<<<<<<<<<<<
  *             return value,
  *         return tuple(value)
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_value); 
@@ -7371,56 +7791,56 @@
   __pyx_t_3 = PyFloat_Check(__pyx_v_value); 
   __pyx_t_1 = (__pyx_t_3 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L6_bool_binop_done:;
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":185
+    /* "configparserc/config.pyx":190
  *             value = filter(bool, value.split(self.separator))
  *         elif isinstance(value, (int, float)):
  *             return value,             # <<<<<<<<<<<<<<
  *         return tuple(value)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_value);
     __Pyx_GIVEREF(__pyx_v_value);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_value);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":184
+    /* "configparserc/config.pyx":189
  *         if isinstance(value, (str, bytes)):
  *             value = filter(bool, value.split(self.separator))
  *         elif isinstance(value, (int, float)):             # <<<<<<<<<<<<<<
  *             return value,
  *         return tuple(value)
  */
   }
   __pyx_L3:;
 
-  /* "configparserc/config.pyx":186
+  /* "configparserc/config.pyx":191
  *         elif isinstance(value, (int, float)):
  *             return value,
  *         return tuple(value)             # <<<<<<<<<<<<<<
  * 
  *     def str_convert(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":181
+  /* "configparserc/config.pyx":186
  *         self.separator = separator
  * 
  *     def convert(self, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, (str, bytes)):
  *             value = filter(bool, value.split(self.separator))
  */
 
@@ -7435,15 +7855,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":188
+/* "configparserc/config.pyx":193
  *         return tuple(value)
  * 
  *     def str_convert(self, value):             # <<<<<<<<<<<<<<
  *         return self.separator.join(value)
  * 
  */
 
@@ -7465,35 +7885,35 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("str_convert", 0);
-  __Pyx_TraceCall("str_convert", __pyx_f[0], 188, 0, __PYX_ERR(0, 188, __pyx_L1_error));
+  __Pyx_TraceCall("str_convert", __pyx_f[0], 193, 0, __PYX_ERR(0, 193, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":189
+  /* "configparserc/config.pyx":194
  * 
  *     def str_convert(self, value):
  *         return self.separator.join(value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_self->separator == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "join");
-    __PYX_ERR(0, 189, __pyx_L1_error)
+    __PYX_ERR(0, 194, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_Join(__pyx_v_self->separator, __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_v_self->separator, __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":188
+  /* "configparserc/config.pyx":193
  *         return tuple(value)
  * 
  *     def str_convert(self, value):             # <<<<<<<<<<<<<<
  *         return self.separator.join(value)
  * 
  */
 
@@ -7624,15 +8044,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":193
+/* "configparserc/config.pyx":198
  * 
  * cdef class JsonType(BaseType):
  *     def convert(self, value):             # <<<<<<<<<<<<<<
  *         if not isinstance(value, str):
  *             value = json.dumps(value)
  */
 
@@ -7658,100 +8078,100 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert", 0);
-  __Pyx_TraceCall("convert", __pyx_f[0], 193, 0, __PYX_ERR(0, 193, __pyx_L1_error));
+  __Pyx_TraceCall("convert", __pyx_f[0], 198, 0, __PYX_ERR(0, 198, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "configparserc/config.pyx":194
+  /* "configparserc/config.pyx":199
  * cdef class JsonType(BaseType):
  *     def convert(self, value):
  *         if not isinstance(value, str):             # <<<<<<<<<<<<<<
  *             value = json.dumps(value)
  *         return json.loads(value)
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_value); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":195
+    /* "configparserc/config.pyx":200
  *     def convert(self, value):
  *         if not isinstance(value, str):
  *             value = json.dumps(value)             # <<<<<<<<<<<<<<
  *         return json.loads(value)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_json); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_json); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dumps); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dumps); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "configparserc/config.pyx":194
+    /* "configparserc/config.pyx":199
  * cdef class JsonType(BaseType):
  *     def convert(self, value):
  *         if not isinstance(value, str):             # <<<<<<<<<<<<<<
  *             value = json.dumps(value)
  *         return json.loads(value)
  */
   }
 
-  /* "configparserc/config.pyx":196
+  /* "configparserc/config.pyx":201
  *         if not isinstance(value, str):
  *             value = json.dumps(value)
  *         return json.loads(value)             # <<<<<<<<<<<<<<
  * 
  *     def str_convert(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_loads); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_loads); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":193
+  /* "configparserc/config.pyx":198
  * 
  * cdef class JsonType(BaseType):
  *     def convert(self, value):             # <<<<<<<<<<<<<<
  *         if not isinstance(value, str):
  *             value = json.dumps(value)
  */
 
@@ -7766,15 +8186,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":198
+/* "configparserc/config.pyx":203
  *         return json.loads(value)
  * 
  *     def str_convert(self, value):             # <<<<<<<<<<<<<<
  *         return json.dumps(value)
  * 
  */
 
@@ -7798,49 +8218,49 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("str_convert", 0);
-  __Pyx_TraceCall("str_convert", __pyx_f[0], 198, 0, __PYX_ERR(0, 198, __pyx_L1_error));
+  __Pyx_TraceCall("str_convert", __pyx_f[0], 203, 0, __PYX_ERR(0, 203, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":199
+  /* "configparserc/config.pyx":204
  * 
  *     def str_convert(self, value):
  *         return json.dumps(value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_value);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":198
+  /* "configparserc/config.pyx":203
  *         return json.loads(value)
  * 
  *     def str_convert(self, value):             # <<<<<<<<<<<<<<
  *         return json.dumps(value)
  * 
  */
 
@@ -8147,15 +8567,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":204
+/* "configparserc/config.pyx":209
  * cdef class __BaseDict(dict):
  * 
  *     def __eq__(self, other):             # <<<<<<<<<<<<<<
  *         if not isinstance(other, dict):
  *             return False
  */
 
@@ -8185,229 +8605,229 @@
   PyObject *__pyx_t_6 = NULL;
   Py_ssize_t __pyx_t_7;
   PyObject *(*__pyx_t_8)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 0);
-  __Pyx_TraceCall("__eq__", __pyx_f[0], 204, 0, __PYX_ERR(0, 204, __pyx_L1_error));
+  __Pyx_TraceCall("__eq__", __pyx_f[0], 209, 0, __PYX_ERR(0, 209, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":205
+  /* "configparserc/config.pyx":210
  * 
  *     def __eq__(self, other):
  *         if not isinstance(other, dict):             # <<<<<<<<<<<<<<
  *             return False
  *         if self.keys() != other.keys():
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_other); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":206
+    /* "configparserc/config.pyx":211
  *     def __eq__(self, other):
  *         if not isinstance(other, dict):
  *             return False             # <<<<<<<<<<<<<<
  *         if self.keys() != other.keys():
  *             return False
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":205
+    /* "configparserc/config.pyx":210
  * 
  *     def __eq__(self, other):
  *         if not isinstance(other, dict):             # <<<<<<<<<<<<<<
  *             return False
  *         if self.keys() != other.keys():
  */
   }
 
-  /* "configparserc/config.pyx":207
+  /* "configparserc/config.pyx":212
  *         if not isinstance(other, dict):
  *             return False
  *         if self.keys() != other.keys():             # <<<<<<<<<<<<<<
  *             return False
  *         for key in self:
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_keys); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_keys); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":208
+    /* "configparserc/config.pyx":213
  *             return False
  *         if self.keys() != other.keys():
  *             return False             # <<<<<<<<<<<<<<
  *         for key in self:
  *             if self[key] != other[key]:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":207
+    /* "configparserc/config.pyx":212
  *         if not isinstance(other, dict):
  *             return False
  *         if self.keys() != other.keys():             # <<<<<<<<<<<<<<
  *             return False
  *         for key in self:
  */
   }
 
-  /* "configparserc/config.pyx":209
+  /* "configparserc/config.pyx":214
  *         if self.keys() != other.keys():
  *             return False
  *         for key in self:             # <<<<<<<<<<<<<<
  *             if self[key] != other[key]:
  *                 return False
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
     __pyx_t_5 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_5); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 214, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 214, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 214, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_8(__pyx_t_5);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 209, __pyx_L1_error)
+          else __PYX_ERR(0, 214, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":210
+    /* "configparserc/config.pyx":215
  *             return False
  *         for key in self:
  *             if self[key] != other[key]:             # <<<<<<<<<<<<<<
  *                 return False
  *         return True
  */
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_other, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_other, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__pyx_t_2) {
 
-      /* "configparserc/config.pyx":211
+      /* "configparserc/config.pyx":216
  *         for key in self:
  *             if self[key] != other[key]:
  *                 return False             # <<<<<<<<<<<<<<
  *         return True
  * 
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_False);
       __pyx_r = Py_False;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L0;
 
-      /* "configparserc/config.pyx":210
+      /* "configparserc/config.pyx":215
  *             return False
  *         for key in self:
  *             if self[key] != other[key]:             # <<<<<<<<<<<<<<
  *                 return False
  *         return True
  */
     }
 
-    /* "configparserc/config.pyx":209
+    /* "configparserc/config.pyx":214
  *         if self.keys() != other.keys():
  *             return False
  *         for key in self:             # <<<<<<<<<<<<<<
  *             if self[key] != other[key]:
  *                 return False
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "configparserc/config.pyx":212
+  /* "configparserc/config.pyx":217
  *             if self[key] != other[key]:
  *                 return False
  *         return True             # <<<<<<<<<<<<<<
  * 
  *     def __ne__(self, other):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(Py_True);
   __pyx_r = Py_True;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":204
+  /* "configparserc/config.pyx":209
  * cdef class __BaseDict(dict):
  * 
  *     def __eq__(self, other):             # <<<<<<<<<<<<<<
  *         if not isinstance(other, dict):
  *             return False
  */
 
@@ -8423,15 +8843,15 @@
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":214
+/* "configparserc/config.pyx":219
  *         return True
  * 
  *     def __ne__(self, other):             # <<<<<<<<<<<<<<
  *         return not self == other
  * 
  */
 
@@ -8454,34 +8874,34 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__ne__", 0);
-  __Pyx_TraceCall("__ne__", __pyx_f[0], 214, 0, __PYX_ERR(0, 214, __pyx_L1_error));
+  __Pyx_TraceCall("__ne__", __pyx_f[0], 219, 0, __PYX_ERR(0, 219, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":215
+  /* "configparserc/config.pyx":220
  * 
  *     def __ne__(self, other):
  *         return not self == other             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyObject_RichCompare(((PyObject *)__pyx_v_self), __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(((PyObject *)__pyx_v_self), __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":214
+  /* "configparserc/config.pyx":219
  *         return True
  * 
  *     def __ne__(self, other):             # <<<<<<<<<<<<<<
  *         return not self == other
  * 
  */
 
@@ -8786,15 +9206,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":229
+/* "configparserc/config.pyx":234
  *         tuple __format_exclude_sections
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             dict section_overload = None,
  */
 
@@ -8811,42 +9231,42 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_section_overload,&__pyx_n_s_section_defaults,&__pyx_n_s_format_kwargs,&__pyx_n_s_format_exclude_sections,0};
     PyObject* values[4] = {0,0,0,0};
 
-    /* "configparserc/config.pyx":231
+    /* "configparserc/config.pyx":236
  *     def __init__(
  *             self,
  *             dict section_overload = None,             # <<<<<<<<<<<<<<
  *             dict section_defaults = None,
  *             dict format_kwargs = None,
  */
     values[0] = ((PyObject*)Py_None);
 
-    /* "configparserc/config.pyx":232
+    /* "configparserc/config.pyx":237
  *             self,
  *             dict section_overload = None,
  *             dict section_defaults = None,             # <<<<<<<<<<<<<<
  *             dict format_kwargs = None,
  *             tuple format_exclude_sections = (),
  */
     values[1] = ((PyObject*)Py_None);
 
-    /* "configparserc/config.pyx":233
+    /* "configparserc/config.pyx":238
  *             dict section_overload = None,
  *             dict section_defaults = None,
  *             dict format_kwargs = None,             # <<<<<<<<<<<<<<
  *             tuple format_exclude_sections = (),
  *     ):
  */
     values[2] = ((PyObject*)Py_None);
 
-    /* "configparserc/config.pyx":234
+    /* "configparserc/config.pyx":239
  *             dict section_defaults = None,
  *             dict format_kwargs = None,
  *             tuple format_exclude_sections = (),             # <<<<<<<<<<<<<<
  *     ):
  *         self.__sections_map = {}
  */
     values[3] = ((PyObject*)__pyx_empty_tuple);
@@ -8888,15 +9308,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format_exclude_sections);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 229, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 234, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -8911,27 +9331,27 @@
     __pyx_v_section_overload = ((PyObject*)values[0]);
     __pyx_v_section_defaults = ((PyObject*)values[1]);
     __pyx_v_format_kwargs = ((PyObject*)values[2]);
     __pyx_v_format_exclude_sections = ((PyObject*)values[3]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 229, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 234, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.ConfigParserC.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_section_overload), (&PyDict_Type), 1, "section_overload", 1))) __PYX_ERR(0, 231, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_section_defaults), (&PyDict_Type), 1, "section_defaults", 1))) __PYX_ERR(0, 232, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_format_kwargs), (&PyDict_Type), 1, "format_kwargs", 1))) __PYX_ERR(0, 233, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_format_exclude_sections), (&PyTuple_Type), 1, "format_exclude_sections", 1))) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_section_overload), (&PyDict_Type), 1, "section_overload", 1))) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_section_defaults), (&PyDict_Type), 1, "section_defaults", 1))) __PYX_ERR(0, 237, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_format_kwargs), (&PyDict_Type), 1, "format_kwargs", 1))) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_format_exclude_sections), (&PyTuple_Type), 1, "format_exclude_sections", 1))) __PYX_ERR(0, 239, __pyx_L1_error)
   __pyx_r = __pyx_pf_13configparserc_6config_13ConfigParserC___init__(((struct __pyx_obj_13configparserc_6config_ConfigParserC *)__pyx_v_self), __pyx_v_section_overload, __pyx_v_section_defaults, __pyx_v_format_kwargs, __pyx_v_format_exclude_sections);
 
-  /* "configparserc/config.pyx":229
+  /* "configparserc/config.pyx":234
  *         tuple __format_exclude_sections
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             dict section_overload = None,
  */
 
@@ -8960,372 +9380,372 @@
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 229, 0, __PYX_ERR(0, 229, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 234, 0, __PYX_ERR(0, 234, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":236
+  /* "configparserc/config.pyx":241
  *             tuple format_exclude_sections = (),
  *     ):
  *         self.__sections_map = {}             # <<<<<<<<<<<<<<
  *         self.section_defaults = getattr(self, 'defaults', section_defaults or {}).copy()
  *         self.__format_kwargs = getattr(self, 'format_kwargs', {}).copy()
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->__pyx___sections_map);
   __Pyx_DECREF(__pyx_v_self->__pyx___sections_map);
   __pyx_v_self->__pyx___sections_map = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":237
+  /* "configparserc/config.pyx":242
  *     ):
  *         self.__sections_map = {}
  *         self.section_defaults = getattr(self, 'defaults', section_defaults or {}).copy()             # <<<<<<<<<<<<<<
  *         self.__format_kwargs = getattr(self, 'format_kwargs', {}).copy()
  *         self.__format_exclude_sections = format_exclude_sections
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_section_defaults); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_section_defaults); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 242, __pyx_L1_error)
   if (!__pyx_t_3) {
   } else {
     __Pyx_INCREF(__pyx_v_section_defaults);
     __pyx_t_2 = __pyx_v_section_defaults;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_2 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
-  __pyx_t_4 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_u_defaults, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_u_defaults, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 237, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->section_defaults);
   __Pyx_DECREF(__pyx_v_self->section_defaults);
   __pyx_v_self->section_defaults = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":238
+  /* "configparserc/config.pyx":243
  *         self.__sections_map = {}
  *         self.section_defaults = getattr(self, 'defaults', section_defaults or {}).copy()
  *         self.__format_kwargs = getattr(self, 'format_kwargs', {}).copy()             # <<<<<<<<<<<<<<
  *         self.__format_exclude_sections = format_exclude_sections
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_u_format_kwargs, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_u_format_kwargs, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->__pyx___format_kwargs);
   __Pyx_DECREF(__pyx_v_self->__pyx___format_kwargs);
   __pyx_v_self->__pyx___format_kwargs = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":239
+  /* "configparserc/config.pyx":244
  *         self.section_defaults = getattr(self, 'defaults', section_defaults or {}).copy()
  *         self.__format_kwargs = getattr(self, 'format_kwargs', {}).copy()
  *         self.__format_exclude_sections = format_exclude_sections             # <<<<<<<<<<<<<<
  * 
  *         if format_kwargs:
  */
   __Pyx_INCREF(__pyx_v_format_exclude_sections);
   __Pyx_GIVEREF(__pyx_v_format_exclude_sections);
   __Pyx_GOTREF(__pyx_v_self->__pyx___format_exclude_sections);
   __Pyx_DECREF(__pyx_v_self->__pyx___format_exclude_sections);
   __pyx_v_self->__pyx___format_exclude_sections = __pyx_v_format_exclude_sections;
 
-  /* "configparserc/config.pyx":241
+  /* "configparserc/config.pyx":246
  *         self.__format_exclude_sections = format_exclude_sections
  * 
  *         if format_kwargs:             # <<<<<<<<<<<<<<
  *             self.__format_kwargs.update(format_kwargs)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_format_kwargs); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_format_kwargs); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 246, __pyx_L1_error)
   if (__pyx_t_3) {
 
-    /* "configparserc/config.pyx":242
+    /* "configparserc/config.pyx":247
  * 
  *         if format_kwargs:
  *             self.__format_kwargs.update(format_kwargs)             # <<<<<<<<<<<<<<
  * 
  *         if hasattr(self, 'section_overload') and self.section_overload:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___format_kwargs, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___format_kwargs, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_format_kwargs) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_format_kwargs);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":241
+    /* "configparserc/config.pyx":246
  *         self.__format_exclude_sections = format_exclude_sections
  * 
  *         if format_kwargs:             # <<<<<<<<<<<<<<
  *             self.__format_kwargs.update(format_kwargs)
  * 
  */
   }
 
-  /* "configparserc/config.pyx":244
+  /* "configparserc/config.pyx":249
  *             self.__format_kwargs.update(format_kwargs)
  * 
  *         if hasattr(self, 'section_overload') and self.section_overload:             # <<<<<<<<<<<<<<
  *             self.__sections_map.update(self.section_overload)
  *         if section_overload:
  */
-  __pyx_t_5 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_section_overload); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_section_overload); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 249, __pyx_L1_error)
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
   } else {
     __pyx_t_3 = __pyx_t_6;
     goto __pyx_L7_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_section_overload); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_section_overload); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __pyx_t_6;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_3) {
 
-    /* "configparserc/config.pyx":245
+    /* "configparserc/config.pyx":250
  * 
  *         if hasattr(self, 'section_overload') and self.section_overload:
  *             self.__sections_map.update(self.section_overload)             # <<<<<<<<<<<<<<
  *         if section_overload:
  *             self.__sections_map.update(section_overload)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___sections_map, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___sections_map, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_section_overload); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_section_overload); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_7, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":244
+    /* "configparserc/config.pyx":249
  *             self.__format_kwargs.update(format_kwargs)
  * 
  *         if hasattr(self, 'section_overload') and self.section_overload:             # <<<<<<<<<<<<<<
  *             self.__sections_map.update(self.section_overload)
  *         if section_overload:
  */
   }
 
-  /* "configparserc/config.pyx":246
+  /* "configparserc/config.pyx":251
  *         if hasattr(self, 'section_overload') and self.section_overload:
  *             self.__sections_map.update(self.section_overload)
  *         if section_overload:             # <<<<<<<<<<<<<<
  *             self.__sections_map.update(section_overload)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_section_overload); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_section_overload); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 251, __pyx_L1_error)
   if (__pyx_t_3) {
 
-    /* "configparserc/config.pyx":247
+    /* "configparserc/config.pyx":252
  *             self.__sections_map.update(self.section_overload)
  *         if section_overload:
  *             self.__sections_map.update(section_overload)             # <<<<<<<<<<<<<<
  * 
  *         super().__init__()
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___sections_map, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___sections_map, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_section_overload) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_section_overload);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":246
+    /* "configparserc/config.pyx":251
  *         if hasattr(self, 'section_overload') and self.section_overload:
  *             self.__sections_map.update(self.section_overload)
  *         if section_overload:             # <<<<<<<<<<<<<<
  *             self.__sections_map.update(section_overload)
  * 
  */
   }
 
-  /* "configparserc/config.pyx":249
+  /* "configparserc/config.pyx":254
  *             self.__sections_map.update(section_overload)
  * 
  *         super().__init__()             # <<<<<<<<<<<<<<
  * 
  *         for key in self.section_defaults:
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":251
+  /* "configparserc/config.pyx":256
  *         super().__init__()
  * 
  *         for key in self.section_defaults:             # <<<<<<<<<<<<<<
  *             self[key] = self.get_section_instance(key)
  * 
  */
   __pyx_t_8 = 0;
   if (unlikely(__pyx_v_self->section_defaults == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 251, __pyx_L1_error)
+    __PYX_ERR(0, 256, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_self->section_defaults, 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_self->section_defaults, 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_2;
   __pyx_t_2 = 0;
   while (1) {
     __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_9, &__pyx_t_8, &__pyx_t_2, NULL, NULL, __pyx_t_10);
     if (unlikely(__pyx_t_11 == 0)) break;
-    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 251, __pyx_L1_error)
+    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "configparserc/config.pyx":252
+    /* "configparserc/config.pyx":257
  * 
  *         for key in self.section_defaults:
  *             self[key] = self.get_section_instance(key)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_key);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_t_2) < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_t_2) < 0)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":229
+  /* "configparserc/config.pyx":234
  *         tuple __format_exclude_sections
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *             self,
  *             dict section_overload = None,
  */
 
@@ -9342,15 +9762,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":254
+/* "configparserc/config.pyx":259
  *             self[key] = self.get_section_instance(key)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         if item not in self:
  *             section = self.get_section_instance(item)
  */
 
@@ -9388,146 +9808,146 @@
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
-  __Pyx_TraceCall("__getitem__", __pyx_f[0], 254, 0, __PYX_ERR(0, 254, __pyx_L1_error));
+  __Pyx_TraceCall("__getitem__", __pyx_f[0], 259, 0, __PYX_ERR(0, 259, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":255
+  /* "configparserc/config.pyx":260
  * 
  *     def __getitem__(self, item):
  *         if item not in self:             # <<<<<<<<<<<<<<
  *             section = self.get_section_instance(item)
  *         else:
  */
-  __pyx_t_1 = (__Pyx_PySequence_ContainsTF(__pyx_v_item, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PySequence_ContainsTF(__pyx_v_item, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 260, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":256
+    /* "configparserc/config.pyx":261
  *     def __getitem__(self, item):
  *         if item not in self:
  *             section = self.get_section_instance(item)             # <<<<<<<<<<<<<<
  *         else:
  *             section = super().__getitem__(item)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_item) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_item);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_section = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "configparserc/config.pyx":255
+    /* "configparserc/config.pyx":260
  * 
  *     def __getitem__(self, item):
  *         if item not in self:             # <<<<<<<<<<<<<<
  *             section = self.get_section_instance(item)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "configparserc/config.pyx":258
+  /* "configparserc/config.pyx":263
  *             section = self.get_section_instance(item)
  *         else:
  *             section = super().__getitem__(item)             # <<<<<<<<<<<<<<
  * 
  *             subsections_names = list(section.subsections_names)
  */
   /*else*/ {
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC));
     __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC));
     PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC));
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_self));
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_getitem); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_getitem); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_item) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_item);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 258, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_section = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "configparserc/config.pyx":260
+    /* "configparserc/config.pyx":265
  *             section = super().__getitem__(item)
  * 
  *             subsections_names = list(section.subsections_names)             # <<<<<<<<<<<<<<
  *             only_subsections = not frozenset(subsections_names).symmetric_difference(section.keys())
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_subsections_names); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_subsections_names); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_4 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_subsections_names = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":261
+    /* "configparserc/config.pyx":266
  * 
  *             subsections_names = list(section.subsections_names)
  *             only_subsections = not frozenset(subsections_names).symmetric_difference(section.keys())             # <<<<<<<<<<<<<<
  * 
  *             if (not section or only_subsections) and isinstance(section, Section) and item in self.section_defaults:
  */
-    __pyx_t_3 = __Pyx_PyFrozenSet_New(__pyx_v_subsections_names); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFrozenSet_New(__pyx_v_subsections_names); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_symmetric_difference); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_symmetric_difference); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_keys); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_keys); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 261, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -9535,29 +9955,29 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_only_subsections = (!__pyx_t_2);
 
-    /* "configparserc/config.pyx":263
+    /* "configparserc/config.pyx":268
  *             only_subsections = not frozenset(subsections_names).symmetric_difference(section.keys())
  * 
  *             if (not section or only_subsections) and isinstance(section, Section) and item in self.section_defaults:             # <<<<<<<<<<<<<<
  *                 section = section.copy()
  *                 for key, value in self.section_defaults[item].copy().items():
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_section); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_section); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 268, __pyx_L1_error)
     __pyx_t_8 = ((!__pyx_t_1) != 0);
     if (!__pyx_t_8) {
     } else {
       goto __pyx_L6_next_and;
     }
     __pyx_t_8 = (__pyx_v_only_subsections != 0);
     if (__pyx_t_8) {
@@ -9571,157 +9991,157 @@
     if (__pyx_t_1) {
     } else {
       __pyx_t_2 = __pyx_t_1;
       goto __pyx_L5_bool_binop_done;
     }
     if (unlikely(__pyx_v_self->section_defaults == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 263, __pyx_L1_error)
+      __PYX_ERR(0, 268, __pyx_L1_error)
     }
-    __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_item, __pyx_v_self->section_defaults, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_item, __pyx_v_self->section_defaults, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 268, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_1 != 0);
     __pyx_t_2 = __pyx_t_8;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "configparserc/config.pyx":264
+      /* "configparserc/config.pyx":269
  * 
  *             if (not section or only_subsections) and isinstance(section, Section) and item in self.section_defaults:
  *                 section = section.copy()             # <<<<<<<<<<<<<<
  *                 for key, value in self.section_defaults[item].copy().items():
  *                     if key not in subsections_names:
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF_SET(__pyx_v_section, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "configparserc/config.pyx":265
+      /* "configparserc/config.pyx":270
  *             if (not section or only_subsections) and isinstance(section, Section) and item in self.section_defaults:
  *                 section = section.copy()
  *                 for key, value in self.section_defaults[item].copy().items():             # <<<<<<<<<<<<<<
  *                     if key not in subsections_names:
  *                         section[key] = value
  */
       __pyx_t_9 = 0;
       if (unlikely(__pyx_v_self->section_defaults == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 265, __pyx_L1_error)
+        __PYX_ERR(0, 270, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->section_defaults, __pyx_v_item); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->section_defaults, __pyx_v_item); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 270, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_copy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_copy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 270, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(__pyx_t_5 == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-        __PYX_ERR(0, 265, __pyx_L1_error)
+        __PYX_ERR(0, 270, __pyx_L1_error)
       }
-      __pyx_t_6 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_items, (&__pyx_t_10), (&__pyx_t_11)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_dict_iterator(__pyx_t_5, 0, __pyx_n_s_items, (&__pyx_t_10), (&__pyx_t_11)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 270, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_4);
       __pyx_t_4 = __pyx_t_6;
       __pyx_t_6 = 0;
       while (1) {
         __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_10, &__pyx_t_9, &__pyx_t_6, &__pyx_t_5, NULL, __pyx_t_11);
         if (unlikely(__pyx_t_12 == 0)) break;
-        if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 265, __pyx_L1_error)
+        if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 270, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
         __pyx_t_6 = 0;
         __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_5);
         __pyx_t_5 = 0;
 
-        /* "configparserc/config.pyx":266
+        /* "configparserc/config.pyx":271
  *                 section = section.copy()
  *                 for key, value in self.section_defaults[item].copy().items():
  *                     if key not in subsections_names:             # <<<<<<<<<<<<<<
  *                         section[key] = value
  * 
  */
-        __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, __pyx_v_subsections_names, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 266, __pyx_L1_error)
+        __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, __pyx_v_subsections_names, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 271, __pyx_L1_error)
         __pyx_t_8 = (__pyx_t_2 != 0);
         if (__pyx_t_8) {
 
-          /* "configparserc/config.pyx":267
+          /* "configparserc/config.pyx":272
  *                 for key, value in self.section_defaults[item].copy().items():
  *                     if key not in subsections_names:
  *                         section[key] = value             # <<<<<<<<<<<<<<
  * 
  *         return section
  */
-          if (unlikely(PyObject_SetItem(__pyx_v_section, __pyx_v_key, __pyx_v_value) < 0)) __PYX_ERR(0, 267, __pyx_L1_error)
+          if (unlikely(PyObject_SetItem(__pyx_v_section, __pyx_v_key, __pyx_v_value) < 0)) __PYX_ERR(0, 272, __pyx_L1_error)
 
-          /* "configparserc/config.pyx":266
+          /* "configparserc/config.pyx":271
  *                 section = section.copy()
  *                 for key, value in self.section_defaults[item].copy().items():
  *                     if key not in subsections_names:             # <<<<<<<<<<<<<<
  *                         section[key] = value
  * 
  */
         }
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "configparserc/config.pyx":263
+      /* "configparserc/config.pyx":268
  *             only_subsections = not frozenset(subsections_names).symmetric_difference(section.keys())
  * 
  *             if (not section or only_subsections) and isinstance(section, Section) and item in self.section_defaults:             # <<<<<<<<<<<<<<
  *                 section = section.copy()
  *                 for key, value in self.section_defaults[item].copy().items():
  */
     }
   }
   __pyx_L3:;
 
-  /* "configparserc/config.pyx":269
+  /* "configparserc/config.pyx":274
  *                         section[key] = value
  * 
  *         return section             # <<<<<<<<<<<<<<
  * 
  *     cdef void __set_object_item(self, str key, object value):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_section);
   __pyx_r = __pyx_v_section;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":254
+  /* "configparserc/config.pyx":259
  *             self[key] = self.get_section_instance(key)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         if item not in self:
  *             section = self.get_section_instance(item)
  */
 
@@ -9741,15 +10161,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":271
+/* "configparserc/config.pyx":276
  *         return section
  * 
  *     cdef void __set_object_item(self, str key, object value):             # <<<<<<<<<<<<<<
  *         PyDict_SetItem(self, key, value)
  * 
  */
 
@@ -9757,26 +10177,26 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set_object_item", 0);
-  __Pyx_TraceCall("__set_object_item", __pyx_f[0], 271, 0, __PYX_ERR(0, 271, __pyx_L1_error));
+  __Pyx_TraceCall("__set_object_item", __pyx_f[0], 276, 0, __PYX_ERR(0, 276, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":272
+  /* "configparserc/config.pyx":277
  * 
  *     cdef void __set_object_item(self, str key, object value):
  *         PyDict_SetItem(self, key, value)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, key, value):
  */
-  __pyx_t_1 = PyDict_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_v_value); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_1 = PyDict_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_v_value); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 277, __pyx_L1_error)
 
-  /* "configparserc/config.pyx":271
+  /* "configparserc/config.pyx":276
  *         return section
  * 
  *     cdef void __set_object_item(self, str key, object value):             # <<<<<<<<<<<<<<
  *         PyDict_SetItem(self, key, value)
  * 
  */
 
@@ -9785,15 +10205,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("configparserc.config.ConfigParserC.__set_object_item", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "configparserc/config.pyx":274
+/* "configparserc/config.pyx":279
  *         PyDict_SetItem(self, key, value)
  * 
  *     def __setitem__(self, key, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             value = self.get_section_instance(key, default=value)
  */
 
@@ -9821,18 +10241,18 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
-  __Pyx_TraceCall("__setitem__", __pyx_f[0], 274, 0, __PYX_ERR(0, 274, __pyx_L1_error));
+  __Pyx_TraceCall("__setitem__", __pyx_f[0], 279, 0, __PYX_ERR(0, 279, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "configparserc/config.pyx":275
+  /* "configparserc/config.pyx":280
  * 
  *     def __setitem__(self, key, value):
  *         if isinstance(value, dict) and not isinstance(value, Section):             # <<<<<<<<<<<<<<
  *             value = self.get_section_instance(key, default=value)
  *         self.__set_object_item(key, value)
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_value); 
@@ -9844,59 +10264,59 @@
   }
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_13configparserc_6config_Section); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":276
+    /* "configparserc/config.pyx":281
  *     def __setitem__(self, key, value):
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             value = self.get_section_instance(key, default=value)             # <<<<<<<<<<<<<<
  *         self.__set_object_item(key, value)
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_key);
     __Pyx_GIVEREF(__pyx_v_key);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_key);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default, __pyx_v_value) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default, __pyx_v_value) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "configparserc/config.pyx":275
+    /* "configparserc/config.pyx":280
  * 
  *     def __setitem__(self, key, value):
  *         if isinstance(value, dict) and not isinstance(value, Section):             # <<<<<<<<<<<<<<
  *             value = self.get_section_instance(key, default=value)
  *         self.__set_object_item(key, value)
  */
   }
 
-  /* "configparserc/config.pyx":277
+  /* "configparserc/config.pyx":282
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             value = self.get_section_instance(key, default=value)
  *         self.__set_object_item(key, value)             # <<<<<<<<<<<<<<
  * 
  *     def get(self, key, default = Empty()):
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_key)->tp_name), 0))) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_key)->tp_name), 0))) __PYX_ERR(0, 282, __pyx_L1_error)
   ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->__pyx___set_object_item(__pyx_v_self, ((PyObject*)__pyx_v_key), __pyx_v_value);
 
-  /* "configparserc/config.pyx":274
+  /* "configparserc/config.pyx":279
  *         PyDict_SetItem(self, key, value)
  * 
  *     def __setitem__(self, key, value):             # <<<<<<<<<<<<<<
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             value = self.get_section_instance(key, default=value)
  */
 
@@ -9913,15 +10333,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":279
+/* "configparserc/config.pyx":284
  *         self.__set_object_item(key, value)
  * 
  *     def get(self, key, default = Empty()):             # <<<<<<<<<<<<<<
  *         if key not in self and not isinstance(default, Empty):
  *             return self.get_section_instance(key, default=default)
  */
 
@@ -9960,15 +10380,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_default);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get") < 0)) __PYX_ERR(0, 279, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -9976,15 +10396,15 @@
       }
     }
     __pyx_v_key = values[0];
     __pyx_v_default = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 279, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 284, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.ConfigParserC.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_13ConfigParserC_6get(((struct __pyx_obj_13configparserc_6config_ConfigParserC *)__pyx_v_self), __pyx_v_key, __pyx_v_default);
 
@@ -10004,87 +10424,87 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get", 0);
-  __Pyx_TraceCall("get", __pyx_f[0], 279, 0, __PYX_ERR(0, 279, __pyx_L1_error));
+  __Pyx_TraceCall("get", __pyx_f[0], 284, 0, __PYX_ERR(0, 284, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":280
+  /* "configparserc/config.pyx":285
  * 
  *     def get(self, key, default = Empty()):
  *         if key not in self and not isinstance(default, Empty):             # <<<<<<<<<<<<<<
  *             return self.get_section_instance(key, default=default)
  *         return self[key]
  */
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_default, __pyx_ptype_13configparserc_6config_Empty); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":281
+    /* "configparserc/config.pyx":286
  *     def get(self, key, default = Empty()):
  *         if key not in self and not isinstance(default, Empty):
  *             return self.get_section_instance(key, default=default)             # <<<<<<<<<<<<<<
  *         return self[key]
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_key);
     __Pyx_GIVEREF(__pyx_v_key);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_key);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default, __pyx_v_default) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default, __pyx_v_default) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_r = __pyx_t_7;
     __pyx_t_7 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":280
+    /* "configparserc/config.pyx":285
  * 
  *     def get(self, key, default = Empty()):
  *         if key not in self and not isinstance(default, Empty):             # <<<<<<<<<<<<<<
  *             return self.get_section_instance(key, default=default)
  *         return self[key]
  */
   }
 
-  /* "configparserc/config.pyx":282
+  /* "configparserc/config.pyx":287
  *         if key not in self and not isinstance(default, Empty):
  *             return self.get_section_instance(key, default=default)
  *         return self[key]             # <<<<<<<<<<<<<<
  * 
  *     def format_string(self, value, section_name=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":279
+  /* "configparserc/config.pyx":284
  *         self.__set_object_item(key, value)
  * 
  *     def get(self, key, default = Empty()):             # <<<<<<<<<<<<<<
  *         if key not in self and not isinstance(default, Empty):
  *             return self.get_section_instance(key, default=default)
  */
 
@@ -10099,15 +10519,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":284
+/* "configparserc/config.pyx":289
  *         return self[key]
  * 
  *     def format_string(self, value, section_name=None):             # <<<<<<<<<<<<<<
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:
  *             return value.format(
  */
 
@@ -10146,15 +10566,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_section_name);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "format_string") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "format_string") < 0)) __PYX_ERR(0, 289, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -10162,15 +10582,15 @@
       }
     }
     __pyx_v_value = values[0];
     __pyx_v_section_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("format_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 284, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("format_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 289, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.ConfigParserC.format_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_13ConfigParserC_8format_string(((struct __pyx_obj_13configparserc_6config_ConfigParserC *)__pyx_v_self), __pyx_v_value, __pyx_v_section_name);
 
@@ -10192,151 +10612,151 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("format_string", 0);
-  __Pyx_TraceCall("format_string", __pyx_f[0], 284, 0, __PYX_ERR(0, 284, __pyx_L1_error));
+  __Pyx_TraceCall("format_string", __pyx_f[0], 289, 0, __PYX_ERR(0, 289, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":285
+  /* "configparserc/config.pyx":290
  * 
  *     def format_string(self, value, section_name=None):
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:             # <<<<<<<<<<<<<<
  *             return value.format(
  *                 __section=section_name,
  */
   __pyx_t_2 = PyUnicode_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__8, __pyx_v_value, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__8, __pyx_v_value, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__9, __pyx_v_value, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__9, __pyx_v_value, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_v_section_name, __pyx_v_self->__pyx___format_exclude_sections, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_v_section_name, __pyx_v_self->__pyx___format_exclude_sections, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":286
+    /* "configparserc/config.pyx":291
  *     def format_string(self, value, section_name=None):
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:
  *             return value.format(             # <<<<<<<<<<<<<<
  *                 __section=section_name,
  *                 this=self.copy(),
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
 
-    /* "configparserc/config.pyx":287
+    /* "configparserc/config.pyx":292
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:
  *             return value.format(
  *                 __section=section_name,             # <<<<<<<<<<<<<<
  *                 this=self.copy(),
  *                 **self.__format_kwargs
  */
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 287, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_section, __pyx_v_section_name) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_section, __pyx_v_section_name) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
 
-    /* "configparserc/config.pyx":288
+    /* "configparserc/config.pyx":293
  *             return value.format(
  *                 __section=section_name,
  *                 this=self.copy(),             # <<<<<<<<<<<<<<
  *                 **self.__format_kwargs
  *             )
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_copy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_copy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 293, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
     __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 288, __pyx_L1_error)
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 293, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_this, __pyx_t_7) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_this, __pyx_t_7) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_5 = __pyx_t_6;
     __pyx_t_6 = 0;
 
-    /* "configparserc/config.pyx":289
+    /* "configparserc/config.pyx":294
  *                 __section=section_name,
  *                 this=self.copy(),
  *                 **self.__format_kwargs             # <<<<<<<<<<<<<<
  *             )
  *         return value
  */
     if (unlikely(__pyx_v_self->__pyx___format_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 289, __pyx_L1_error)
+      __PYX_ERR(0, 294, __pyx_L1_error)
     }
-    if (__Pyx_MergeKeywords(__pyx_t_5, __pyx_v_self->__pyx___format_kwargs) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
+    if (__Pyx_MergeKeywords(__pyx_t_5, __pyx_v_self->__pyx___format_kwargs) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
 
-    /* "configparserc/config.pyx":286
+    /* "configparserc/config.pyx":291
  *     def format_string(self, value, section_name=None):
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:
  *             return value.format(             # <<<<<<<<<<<<<<
  *                 __section=section_name,
  *                 this=self.copy(),
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":285
+    /* "configparserc/config.pyx":290
  * 
  *     def format_string(self, value, section_name=None):
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:             # <<<<<<<<<<<<<<
  *             return value.format(
  *                 __section=section_name,
  */
   }
 
-  /* "configparserc/config.pyx":291
+  /* "configparserc/config.pyx":296
  *                 **self.__format_kwargs
  *             )
  *         return value             # <<<<<<<<<<<<<<
  * 
  *     def get_section_instance(self, section_name, *args, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_value);
   __pyx_r = __pyx_v_value;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":284
+  /* "configparserc/config.pyx":289
  *         return self[key]
  * 
  *     def format_string(self, value, section_name=None):             # <<<<<<<<<<<<<<
  *         if isinstance(value, str) and '{' in value and '}' in value and section_name not in self.__format_exclude_sections:
  *             return value.format(
  */
 
@@ -10353,15 +10773,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":293
+/* "configparserc/config.pyx":298
  *         return value
  * 
  *     def get_section_instance(self, section_name, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return self.get_section_class(section_name)(section_name, self, *args, **kwargs)
  * 
  */
 
@@ -10406,26 +10826,26 @@
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_section_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "get_section_instance") < 0)) __PYX_ERR(0, 293, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "get_section_instance") < 0)) __PYX_ERR(0, 298, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) < 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_section_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_section_instance", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 293, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_section_instance", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 298, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("configparserc.config.ConfigParserC.get_section_instance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -10446,64 +10866,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_section_instance", 0);
-  __Pyx_TraceCall("get_section_instance", __pyx_f[0], 293, 0, __PYX_ERR(0, 293, __pyx_L1_error));
+  __Pyx_TraceCall("get_section_instance", __pyx_f[0], 298, 0, __PYX_ERR(0, 298, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":294
+  /* "configparserc/config.pyx":299
  * 
  *     def get_section_instance(self, section_name, *args, **kwargs):
  *         return self.get_section_class(section_name)(section_name, self, *args, **kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def get_section_class(self, section_name):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_section_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_section_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_section_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_section_name);
   __Pyx_GIVEREF(__pyx_v_section_name);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_section_name);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":293
+  /* "configparserc/config.pyx":298
  *         return value
  * 
  *     def get_section_instance(self, section_name, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return self.get_section_class(section_name)(section_name, self, *args, **kwargs)
  * 
  */
 
@@ -10518,15 +10938,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":296
+/* "configparserc/config.pyx":301
  *         return self.get_section_class(section_name)(section_name, self, *args, **kwargs)
  * 
  *     def get_section_class(self, section_name):             # <<<<<<<<<<<<<<
  *         if section_name in self.__sections_map:
  *             return self.__sections_map[section_name]
  */
 
@@ -10551,111 +10971,111 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_section_class", 0);
-  __Pyx_TraceCall("get_section_class", __pyx_f[0], 296, 0, __PYX_ERR(0, 296, __pyx_L1_error));
+  __Pyx_TraceCall("get_section_class", __pyx_f[0], 301, 0, __PYX_ERR(0, 301, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":297
+  /* "configparserc/config.pyx":302
  * 
  *     def get_section_class(self, section_name):
  *         if section_name in self.__sections_map:             # <<<<<<<<<<<<<<
  *             return self.__sections_map[section_name]
  *         elif hasattr(self, 'section_class_' + section_name):
  */
   if (unlikely(__pyx_v_self->__pyx___sections_map == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 297, __pyx_L1_error)
+    __PYX_ERR(0, 302, __pyx_L1_error)
   }
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_section_name, __pyx_v_self->__pyx___sections_map, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_section_name, __pyx_v_self->__pyx___sections_map, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 302, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":298
+    /* "configparserc/config.pyx":303
  *     def get_section_class(self, section_name):
  *         if section_name in self.__sections_map:
  *             return self.__sections_map[section_name]             # <<<<<<<<<<<<<<
  *         elif hasattr(self, 'section_class_' + section_name):
  *             return getattr(self, 'section_class_' + section_name, Section)
  */
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_self->__pyx___sections_map == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 298, __pyx_L1_error)
+      __PYX_ERR(0, 303, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->__pyx___sections_map, __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->__pyx___sections_map, __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":297
+    /* "configparserc/config.pyx":302
  * 
  *     def get_section_class(self, section_name):
  *         if section_name in self.__sections_map:             # <<<<<<<<<<<<<<
  *             return self.__sections_map[section_name]
  *         elif hasattr(self, 'section_class_' + section_name):
  */
   }
 
-  /* "configparserc/config.pyx":299
+  /* "configparserc/config.pyx":304
  *         if section_name in self.__sections_map:
  *             return self.__sections_map[section_name]
  *         elif hasattr(self, 'section_class_' + section_name):             # <<<<<<<<<<<<<<
  *             return getattr(self, 'section_class_' + section_name, Section)
  *         return Section
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_n_u_section_class, __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_n_u_section_class, __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":300
+    /* "configparserc/config.pyx":305
  *             return self.__sections_map[section_name]
  *         elif hasattr(self, 'section_class_' + section_name):
  *             return getattr(self, 'section_class_' + section_name, Section)             # <<<<<<<<<<<<<<
  *         return Section
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyNumber_Add(__pyx_n_u_section_class, __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_n_u_section_class, __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_t_3, ((PyObject *)__pyx_ptype_13configparserc_6config_Section)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_t_3, ((PyObject *)__pyx_ptype_13configparserc_6config_Section)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":299
+    /* "configparserc/config.pyx":304
  *         if section_name in self.__sections_map:
  *             return self.__sections_map[section_name]
  *         elif hasattr(self, 'section_class_' + section_name):             # <<<<<<<<<<<<<<
  *             return getattr(self, 'section_class_' + section_name, Section)
  *         return Section
  */
   }
 
-  /* "configparserc/config.pyx":301
+  /* "configparserc/config.pyx":306
  *         elif hasattr(self, 'section_class_' + section_name):
  *             return getattr(self, 'section_class_' + section_name, Section)
  *         return Section             # <<<<<<<<<<<<<<
  * 
  *     cdef object _parse_section(self, str line):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   __pyx_r = ((PyObject *)__pyx_ptype_13configparserc_6config_Section);
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":296
+  /* "configparserc/config.pyx":301
  *         return self.get_section_class(section_name)(section_name, self, *args, **kwargs)
  * 
  *     def get_section_class(self, section_name):             # <<<<<<<<<<<<<<
  *         if section_name in self.__sections_map:
  *             return self.__sections_map[section_name]
  */
 
@@ -10668,15 +11088,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":303
+/* "configparserc/config.pyx":308
  *         return Section
  * 
  *     cdef object _parse_section(self, str line):             # <<<<<<<<<<<<<<
  *         if '[' in line and ']' in line:
  *             match = self.section_regex.match(line)
  */
 
@@ -10691,133 +11111,133 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_section", 0);
-  __Pyx_TraceCall("_parse_section", __pyx_f[0], 303, 0, __PYX_ERR(0, 303, __pyx_L1_error));
+  __Pyx_TraceCall("_parse_section", __pyx_f[0], 308, 0, __PYX_ERR(0, 308, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":304
+  /* "configparserc/config.pyx":309
  * 
  *     cdef object _parse_section(self, str line):
  *         if '[' in line and ']' in line:             # <<<<<<<<<<<<<<
  *             match = self.section_regex.match(line)
  *             if match is not None:
  */
   if (unlikely(__pyx_v_line == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 304, __pyx_L1_error)
+    __PYX_ERR(0, 309, __pyx_L1_error)
   }
-  __pyx_t_2 = (__Pyx_PyUnicode_ContainsTF(__pyx_kp_u__10, __pyx_v_line, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_ContainsTF(__pyx_kp_u__10, __pyx_v_line, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
   if (unlikely(__pyx_v_line == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 304, __pyx_L1_error)
+    __PYX_ERR(0, 309, __pyx_L1_error)
   }
-  __pyx_t_3 = (__Pyx_PyUnicode_ContainsTF(__pyx_kp_u__11, __pyx_v_line, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_ContainsTF(__pyx_kp_u__11, __pyx_v_line, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":305
+    /* "configparserc/config.pyx":310
  *     cdef object _parse_section(self, str line):
  *         if '[' in line and ']' in line:
  *             match = self.section_regex.match(line)             # <<<<<<<<<<<<<<
  *             if match is not None:
  *                 return match.group('section')
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_section_regex); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 305, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_section_regex); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_match); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 305, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_match); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_line) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_line);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 305, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_match = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":306
+    /* "configparserc/config.pyx":311
  *         if '[' in line and ']' in line:
  *             match = self.section_regex.match(line)
  *             if match is not None:             # <<<<<<<<<<<<<<
  *                 return match.group('section')
  * 
  */
     __pyx_t_1 = (__pyx_v_match != Py_None);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "configparserc/config.pyx":307
+      /* "configparserc/config.pyx":312
  *             match = self.section_regex.match(line)
  *             if match is not None:
  *                 return match.group('section')             # <<<<<<<<<<<<<<
  * 
  *     cdef object _parse_pair(self, str line):
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_group); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 307, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_group); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 312, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_n_u_section_2) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_n_u_section_2);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L0;
 
-      /* "configparserc/config.pyx":306
+      /* "configparserc/config.pyx":311
  *         if '[' in line and ']' in line:
  *             match = self.section_regex.match(line)
  *             if match is not None:             # <<<<<<<<<<<<<<
  *                 return match.group('section')
  * 
  */
     }
 
-    /* "configparserc/config.pyx":304
+    /* "configparserc/config.pyx":309
  * 
  *     cdef object _parse_section(self, str line):
  *         if '[' in line and ']' in line:             # <<<<<<<<<<<<<<
  *             match = self.section_regex.match(line)
  *             if match is not None:
  */
   }
 
-  /* "configparserc/config.pyx":303
+  /* "configparserc/config.pyx":308
  *         return Section
  * 
  *     cdef object _parse_section(self, str line):             # <<<<<<<<<<<<<<
  *         if '[' in line and ']' in line:
  *             match = self.section_regex.match(line)
  */
 
@@ -10834,15 +11254,15 @@
   __Pyx_XDECREF(__pyx_v_match);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":309
+/* "configparserc/config.pyx":314
  *                 return match.group('section')
  * 
  *     cdef object _parse_pair(self, str line):             # <<<<<<<<<<<<<<
  *         cdef:
  *             object match
  */
 
@@ -10857,121 +11277,121 @@
   int __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_pair", 0);
-  __Pyx_TraceCall("_parse_pair", __pyx_f[0], 309, 0, __PYX_ERR(0, 309, __pyx_L1_error));
+  __Pyx_TraceCall("_parse_pair", __pyx_f[0], 314, 0, __PYX_ERR(0, 314, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":313
+  /* "configparserc/config.pyx":318
  *             object match
  * 
  *         match = self.pair_regex.match(line)             # <<<<<<<<<<<<<<
  *         if match is not None:
  *             return match.group('key'), match.group('value')
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pair_regex); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_pair_regex); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_match); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_match); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_line) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_line);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_match = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":314
+  /* "configparserc/config.pyx":319
  * 
  *         match = self.pair_regex.match(line)
  *         if match is not None:             # <<<<<<<<<<<<<<
  *             return match.group('key'), match.group('value')
  * 
  */
   __pyx_t_4 = (__pyx_v_match != Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "configparserc/config.pyx":315
+    /* "configparserc/config.pyx":320
  *         match = self.pair_regex.match(line)
  *         if match is not None:
  *             return match.group('key'), match.group('value')             # <<<<<<<<<<<<<<
  * 
  *     cdef object _add_section(self, str section_name):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_group); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_group); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_key);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_group); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_group); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_n_u_value) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_value);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 315, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
     __pyx_t_1 = 0;
     __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":314
+    /* "configparserc/config.pyx":319
  * 
  *         match = self.pair_regex.match(line)
  *         if match is not None:             # <<<<<<<<<<<<<<
  *             return match.group('key'), match.group('value')
  * 
  */
   }
 
-  /* "configparserc/config.pyx":309
+  /* "configparserc/config.pyx":314
  *                 return match.group('section')
  * 
  *     cdef object _parse_pair(self, str line):             # <<<<<<<<<<<<<<
  *         cdef:
  *             object match
  */
 
@@ -10989,15 +11409,15 @@
   __Pyx_XDECREF(__pyx_v_match);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":317
+/* "configparserc/config.pyx":322
  *             return match.group('key'), match.group('value')
  * 
  *     cdef object _add_section(self, str section_name):             # <<<<<<<<<<<<<<
  *         return __get_or_create_section_recursive(section_name.split('.'), section_name, self, self)
  * 
  */
 
@@ -11007,38 +11427,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_add_section", 0);
-  __Pyx_TraceCall("_add_section", __pyx_f[0], 317, 0, __PYX_ERR(0, 317, __pyx_L1_error));
+  __Pyx_TraceCall("_add_section", __pyx_f[0], 322, 0, __PYX_ERR(0, 322, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":318
+  /* "configparserc/config.pyx":323
  * 
  *     cdef object _add_section(self, str section_name):
  *         return __get_or_create_section_recursive(section_name.split('.'), section_name, self, self)             # <<<<<<<<<<<<<<
  * 
  *     cdef int _parse_file(self, FILE *config_file, unsigned long long config_file_size):
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_section_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "split");
-    __PYX_ERR(0, 318, __pyx_L1_error)
+    __PYX_ERR(0, 323, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_Split(__pyx_v_section_name, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Split(__pyx_v_section_name, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_f_13configparserc_6config___get_or_create_section_recursive(((PyObject*)__pyx_t_1), __pyx_v_section_name, ((PyObject *)__pyx_v_self), ((PyObject *)__pyx_v_self), NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_13configparserc_6config___get_or_create_section_recursive(((PyObject*)__pyx_t_1), __pyx_v_section_name, ((PyObject *)__pyx_v_self), ((PyObject *)__pyx_v_self), NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":317
+  /* "configparserc/config.pyx":322
  *             return match.group('key'), match.group('value')
  * 
  *     cdef object _add_section(self, str section_name):             # <<<<<<<<<<<<<<
  *         return __get_or_create_section_recursive(section_name.split('.'), section_name, self, self)
  * 
  */
 
@@ -11051,15 +11471,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":320
+/* "configparserc/config.pyx":325
  *         return __get_or_create_section_recursive(section_name.split('.'), section_name, self, self)
  * 
  *     cdef int _parse_file(self, FILE *config_file, unsigned long long config_file_size):             # <<<<<<<<<<<<<<
  *         cdef:
  *             str section_name
  */
 
@@ -11076,84 +11496,84 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_file", 0);
-  __Pyx_TraceCall("_parse_file", __pyx_f[0], 320, 0, __PYX_ERR(0, 320, __pyx_L1_error));
+  __Pyx_TraceCall("_parse_file", __pyx_f[0], 325, 0, __PYX_ERR(0, 325, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":327
+  /* "configparserc/config.pyx":332
  *             object result
  *             Section current_section
  *         count = 0             # <<<<<<<<<<<<<<
  *         current_section = None
  * 
  */
   __pyx_v_count = 0;
 
-  /* "configparserc/config.pyx":328
+  /* "configparserc/config.pyx":333
  *             Section current_section
  *         count = 0
  *         current_section = None             # <<<<<<<<<<<<<<
  * 
  *         while <long>config_file_size > ftell(config_file):
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_current_section = ((struct __pyx_obj_13configparserc_6config_Section *)Py_None);
 
-  /* "configparserc/config.pyx":330
+  /* "configparserc/config.pyx":335
  *         current_section = None
  * 
  *         while <long>config_file_size > ftell(config_file):             # <<<<<<<<<<<<<<
  *             line = NULL
  *             with nogil:
  */
   while (1) {
     __pyx_t_1 = ((((long)__pyx_v_config_file_size) > ftell(__pyx_v_config_file)) != 0);
     if (!__pyx_t_1) break;
 
-    /* "configparserc/config.pyx":331
+    /* "configparserc/config.pyx":336
  * 
  *         while <long>config_file_size > ftell(config_file):
  *             line = NULL             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 if getline(&line, &count, config_file) == -1: break
  */
     __pyx_v_line = NULL;
 
-    /* "configparserc/config.pyx":332
+    /* "configparserc/config.pyx":337
  *         while <long>config_file_size > ftell(config_file):
  *             line = NULL
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 if getline(&line, &count, config_file) == -1: break
  *             if __has_only_whitespaces(line) == 1:
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "configparserc/config.pyx":333
+          /* "configparserc/config.pyx":338
  *             line = NULL
  *             with nogil:
  *                 if getline(&line, &count, config_file) == -1: break             # <<<<<<<<<<<<<<
  *             if __has_only_whitespaces(line) == 1:
  *                 continue
  */
           __pyx_t_1 = ((getline((&__pyx_v_line), (&__pyx_v_count), __pyx_v_config_file) == -1L) != 0);
           if (__pyx_t_1) {
             goto __pyx_L6_break;
           }
         }
 
-        /* "configparserc/config.pyx":332
+        /* "configparserc/config.pyx":337
  *         while <long>config_file_size > ftell(config_file):
  *             line = NULL
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 if getline(&line, &count, config_file) == -1: break
  *             if __has_only_whitespaces(line) == 1:
  */
         /*finally:*/ {
@@ -11171,43 +11591,43 @@
             #endif
             goto __pyx_L4_break;
           }
           __pyx_L9:;
         }
     }
 
-    /* "configparserc/config.pyx":334
+    /* "configparserc/config.pyx":339
  *             with nogil:
  *                 if getline(&line, &count, config_file) == -1: break
  *             if __has_only_whitespaces(line) == 1:             # <<<<<<<<<<<<<<
  *                 continue
  *             elif line[0] == b'#' or line[0] == b';':
  */
     __pyx_t_1 = ((__has_only_whitespaces(__pyx_v_line) == 1) != 0);
     if (__pyx_t_1) {
 
-      /* "configparserc/config.pyx":335
+      /* "configparserc/config.pyx":340
  *                 if getline(&line, &count, config_file) == -1: break
  *             if __has_only_whitespaces(line) == 1:
  *                 continue             # <<<<<<<<<<<<<<
  *             elif line[0] == b'#' or line[0] == b';':
  *                 continue
  */
       goto __pyx_L3_continue;
 
-      /* "configparserc/config.pyx":334
+      /* "configparserc/config.pyx":339
  *             with nogil:
  *                 if getline(&line, &count, config_file) == -1: break
  *             if __has_only_whitespaces(line) == 1:             # <<<<<<<<<<<<<<
  *                 continue
  *             elif line[0] == b'#' or line[0] == b';':
  */
     }
 
-    /* "configparserc/config.pyx":336
+    /* "configparserc/config.pyx":341
  *             if __has_only_whitespaces(line) == 1:
  *                 continue
  *             elif line[0] == b'#' or line[0] == b';':             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
     __pyx_t_2 = (((__pyx_v_line[0]) == '#') != 0);
@@ -11217,98 +11637,98 @@
       goto __pyx_L12_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_line[0]) == ';') != 0);
     __pyx_t_1 = __pyx_t_2;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "configparserc/config.pyx":337
+      /* "configparserc/config.pyx":342
  *                 continue
  *             elif line[0] == b'#' or line[0] == b';':
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             section_name = self._parse_section(line)
  */
       goto __pyx_L3_continue;
 
-      /* "configparserc/config.pyx":336
+      /* "configparserc/config.pyx":341
  *             if __has_only_whitespaces(line) == 1:
  *                 continue
  *             elif line[0] == b'#' or line[0] == b';':             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
     }
 
-    /* "configparserc/config.pyx":339
+    /* "configparserc/config.pyx":344
  *                 continue
  * 
  *             section_name = self._parse_section(line)             # <<<<<<<<<<<<<<
  *             if section_name is not None:
  *                 current_section = self._add_section(section_name)
  */
-    __pyx_t_3 = __Pyx_PyUnicode_FromString(__pyx_v_line); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_FromString(__pyx_v_line); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_section(__pyx_v_self, ((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_4 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_section(__pyx_v_self, ((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 339, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_section_name, ((PyObject*)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":340
+    /* "configparserc/config.pyx":345
  * 
  *             section_name = self._parse_section(line)
  *             if section_name is not None:             # <<<<<<<<<<<<<<
  *                 current_section = self._add_section(section_name)
  *                 with nogil:
  */
     __pyx_t_1 = (__pyx_v_section_name != ((PyObject*)Py_None));
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "configparserc/config.pyx":341
+      /* "configparserc/config.pyx":346
  *             section_name = self._parse_section(line)
  *             if section_name is not None:
  *                 current_section = self._add_section(section_name)             # <<<<<<<<<<<<<<
  *                 with nogil:
  *                     free(line)
  */
-      __pyx_t_4 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_add_section(__pyx_v_self, __pyx_v_section_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_add_section(__pyx_v_self, __pyx_v_section_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_13configparserc_6config_Section))))) __PYX_ERR(0, 341, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_13configparserc_6config_Section))))) __PYX_ERR(0, 346, __pyx_L1_error)
       __Pyx_DECREF_SET(__pyx_v_current_section, ((struct __pyx_obj_13configparserc_6config_Section *)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "configparserc/config.pyx":342
+      /* "configparserc/config.pyx":347
  *             if section_name is not None:
  *                 current_section = self._add_section(section_name)
  *                 with nogil:             # <<<<<<<<<<<<<<
  *                     free(line)
  *                 continue
  */
       {
           #ifdef WITH_THREAD
           PyThreadState *_save;
           Py_UNBLOCK_THREADS
           __Pyx_FastGIL_Remember();
           #endif
           /*try:*/ {
 
-            /* "configparserc/config.pyx":343
+            /* "configparserc/config.pyx":348
  *                 current_section = self._add_section(section_name)
  *                 with nogil:
  *                     free(line)             # <<<<<<<<<<<<<<
  *                 continue
  *             elif current_section is None:
  */
             free(__pyx_v_line);
           }
 
-          /* "configparserc/config.pyx":342
+          /* "configparserc/config.pyx":347
  *             if section_name is not None:
  *                 current_section = self._add_section(section_name)
  *                 with nogil:             # <<<<<<<<<<<<<<
  *                     free(line)
  *                 continue
  */
           /*finally:*/ {
@@ -11319,167 +11739,167 @@
               #endif
               goto __pyx_L19;
             }
             __pyx_L19:;
           }
       }
 
-      /* "configparserc/config.pyx":344
+      /* "configparserc/config.pyx":349
  *                 with nogil:
  *                     free(line)
  *                 continue             # <<<<<<<<<<<<<<
  *             elif current_section is None:
  *                 free(line)
  */
       goto __pyx_L3_continue;
 
-      /* "configparserc/config.pyx":340
+      /* "configparserc/config.pyx":345
  * 
  *             section_name = self._parse_section(line)
  *             if section_name is not None:             # <<<<<<<<<<<<<<
  *                 current_section = self._add_section(section_name)
  *                 with nogil:
  */
     }
 
-    /* "configparserc/config.pyx":345
+    /* "configparserc/config.pyx":350
  *                     free(line)
  *                 continue
  *             elif current_section is None:             # <<<<<<<<<<<<<<
  *                 free(line)
  *                 return -1
  */
     __pyx_t_2 = (((PyObject *)__pyx_v_current_section) == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "configparserc/config.pyx":346
+      /* "configparserc/config.pyx":351
  *                 continue
  *             elif current_section is None:
  *                 free(line)             # <<<<<<<<<<<<<<
  *                 return -1
  * 
  */
       free(__pyx_v_line);
 
-      /* "configparserc/config.pyx":347
+      /* "configparserc/config.pyx":352
  *             elif current_section is None:
  *                 free(line)
  *                 return -1             # <<<<<<<<<<<<<<
  * 
  *             result = self._parse_pair(line)
  */
       __pyx_r = -1;
       goto __pyx_L0;
 
-      /* "configparserc/config.pyx":345
+      /* "configparserc/config.pyx":350
  *                     free(line)
  *                 continue
  *             elif current_section is None:             # <<<<<<<<<<<<<<
  *                 free(line)
  *                 return -1
  */
     }
 
-    /* "configparserc/config.pyx":349
+    /* "configparserc/config.pyx":354
  *                 return -1
  * 
  *             result = self._parse_pair(line)             # <<<<<<<<<<<<<<
  *             if result is not None:
  *                 current_section[result[0]] = result[1]
  */
-    __pyx_t_4 = __Pyx_PyUnicode_FromString(__pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_FromString(__pyx_v_line); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_pair(__pyx_v_self, ((PyObject*)__pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_pair(__pyx_v_self, ((PyObject*)__pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_result, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "configparserc/config.pyx":350
+    /* "configparserc/config.pyx":355
  * 
  *             result = self._parse_pair(line)
  *             if result is not None:             # <<<<<<<<<<<<<<
  *                 current_section[result[0]] = result[1]
  *             else:
  */
     __pyx_t_1 = (__pyx_v_result != Py_None);
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "configparserc/config.pyx":351
+      /* "configparserc/config.pyx":356
  *             result = self._parse_pair(line)
  *             if result is not None:
  *                 current_section[result[0]] = result[1]             # <<<<<<<<<<<<<<
  *             else:
  *                 free(line)
  */
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_result, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_result, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_current_section), __pyx_t_4, __pyx_t_3) < 0)) __PYX_ERR(0, 351, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_current_section), __pyx_t_4, __pyx_t_3) < 0)) __PYX_ERR(0, 356, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "configparserc/config.pyx":350
+      /* "configparserc/config.pyx":355
  * 
  *             result = self._parse_pair(line)
  *             if result is not None:             # <<<<<<<<<<<<<<
  *                 current_section[result[0]] = result[1]
  *             else:
  */
       goto __pyx_L20;
     }
 
-    /* "configparserc/config.pyx":353
+    /* "configparserc/config.pyx":358
  *                 current_section[result[0]] = result[1]
  *             else:
  *                 free(line)             # <<<<<<<<<<<<<<
  *                 return -1
  *             free(line)
  */
     /*else*/ {
       free(__pyx_v_line);
 
-      /* "configparserc/config.pyx":354
+      /* "configparserc/config.pyx":359
  *             else:
  *                 free(line)
  *                 return -1             # <<<<<<<<<<<<<<
  *             free(line)
  *         return 0
  */
       __pyx_r = -1;
       goto __pyx_L0;
     }
     __pyx_L20:;
 
-    /* "configparserc/config.pyx":355
+    /* "configparserc/config.pyx":360
  *                 free(line)
  *                 return -1
  *             free(line)             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     free(__pyx_v_line);
     __pyx_L3_continue:;
   }
   __pyx_L4_break:;
 
-  /* "configparserc/config.pyx":356
+  /* "configparserc/config.pyx":361
  *                 return -1
  *             free(line)
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     cdef _parse_file_by_name(self, char *filename):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":320
+  /* "configparserc/config.pyx":325
  *         return __get_or_create_section_recursive(section_name.split('.'), section_name, self, self)
  * 
  *     cdef int _parse_file(self, FILE *config_file, unsigned long long config_file_size):             # <<<<<<<<<<<<<<
  *         cdef:
  *             str section_name
  */
 
@@ -11494,15 +11914,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF((PyObject *)__pyx_v_current_section);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":358
+/* "configparserc/config.pyx":363
  *         return 0
  * 
  *     cdef _parse_file_by_name(self, char *filename):             # <<<<<<<<<<<<<<
  *         cdef:
  *             FILE *fd
  */
 
@@ -11515,60 +11935,60 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_file_by_name", 0);
-  __Pyx_TraceCall("_parse_file_by_name", __pyx_f[0], 358, 0, __PYX_ERR(0, 358, __pyx_L1_error));
+  __Pyx_TraceCall("_parse_file_by_name", __pyx_f[0], 363, 0, __PYX_ERR(0, 363, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":364
+  /* "configparserc/config.pyx":369
  *             int err
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             err = 0
  *             stat(filename, &st)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "configparserc/config.pyx":365
+        /* "configparserc/config.pyx":370
  * 
  *         with nogil:
  *             err = 0             # <<<<<<<<<<<<<<
  *             stat(filename, &st)
  *             fd = fopen(filename, 'r')
  */
         __pyx_v_err = 0;
 
-        /* "configparserc/config.pyx":366
+        /* "configparserc/config.pyx":371
  *         with nogil:
  *             err = 0
  *             stat(filename, &st)             # <<<<<<<<<<<<<<
  *             fd = fopen(filename, 'r')
  *         if fd == NULL:
  */
         (void)(stat(__pyx_v_filename, (&__pyx_v_st)));
 
-        /* "configparserc/config.pyx":367
+        /* "configparserc/config.pyx":372
  *             err = 0
  *             stat(filename, &st)
  *             fd = fopen(filename, 'r')             # <<<<<<<<<<<<<<
  *         if fd == NULL:
  *             return err
  */
         __pyx_v_fd = fopen(__pyx_v_filename, ((char const *)"r"));
       }
 
-      /* "configparserc/config.pyx":364
+      /* "configparserc/config.pyx":369
  *             int err
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             err = 0
  *             stat(filename, &st)
  */
       /*finally:*/ {
@@ -11579,80 +11999,80 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "configparserc/config.pyx":368
+  /* "configparserc/config.pyx":373
  *             stat(filename, &st)
  *             fd = fopen(filename, 'r')
  *         if fd == NULL:             # <<<<<<<<<<<<<<
  *             return err
  *         err = self._parse_file(fd, st.st_size)
  */
   __pyx_t_1 = ((__pyx_v_fd == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":369
+    /* "configparserc/config.pyx":374
  *             fd = fopen(filename, 'r')
  *         if fd == NULL:
  *             return err             # <<<<<<<<<<<<<<
  *         err = self._parse_file(fd, st.st_size)
  *         fclose(fd)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":368
+    /* "configparserc/config.pyx":373
  *             stat(filename, &st)
  *             fd = fopen(filename, 'r')
  *         if fd == NULL:             # <<<<<<<<<<<<<<
  *             return err
  *         err = self._parse_file(fd, st.st_size)
  */
   }
 
-  /* "configparserc/config.pyx":370
+  /* "configparserc/config.pyx":375
  *         if fd == NULL:
  *             return err
  *         err = self._parse_file(fd, st.st_size)             # <<<<<<<<<<<<<<
  *         fclose(fd)
  *         return err
  */
   __pyx_v_err = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_file(__pyx_v_self, __pyx_v_fd, __pyx_v_st.st_size);
 
-  /* "configparserc/config.pyx":371
+  /* "configparserc/config.pyx":376
  *             return err
  *         err = self._parse_file(fd, st.st_size)
  *         fclose(fd)             # <<<<<<<<<<<<<<
  *         return err
  * 
  */
   (void)(fclose(__pyx_v_fd));
 
-  /* "configparserc/config.pyx":372
+  /* "configparserc/config.pyx":377
  *         err = self._parse_file(fd, st.st_size)
  *         fclose(fd)
  *         return err             # <<<<<<<<<<<<<<
  * 
  *     cdef _parse_text(self, char* text):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":358
+  /* "configparserc/config.pyx":363
  *         return 0
  * 
  *     cdef _parse_file_by_name(self, char *filename):             # <<<<<<<<<<<<<<
  *         cdef:
  *             FILE *fd
  */
 
@@ -11664,15 +12084,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":374
+/* "configparserc/config.pyx":379
  *         return err
  * 
  *     cdef _parse_text(self, char* text):             # <<<<<<<<<<<<<<
  *         cdef:
  *             FILE *fd
  */
 
@@ -11685,60 +12105,60 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parse_text", 0);
-  __Pyx_TraceCall("_parse_text", __pyx_f[0], 374, 0, __PYX_ERR(0, 374, __pyx_L1_error));
+  __Pyx_TraceCall("_parse_text", __pyx_f[0], 379, 0, __PYX_ERR(0, 379, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":380
+  /* "configparserc/config.pyx":385
  *             int err
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             err = 0
  *             size = strlen(text) * sizeof(char)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "configparserc/config.pyx":381
+        /* "configparserc/config.pyx":386
  * 
  *         with nogil:
  *             err = 0             # <<<<<<<<<<<<<<
  *             size = strlen(text) * sizeof(char)
  *             fd = fmemopen(text, size, 'r')
  */
         __pyx_v_err = 0;
 
-        /* "configparserc/config.pyx":382
+        /* "configparserc/config.pyx":387
  *         with nogil:
  *             err = 0
  *             size = strlen(text) * sizeof(char)             # <<<<<<<<<<<<<<
  *             fd = fmemopen(text, size, 'r')
  *         if fd == NULL:
  */
         __pyx_v_size = (strlen(__pyx_v_text) * (sizeof(char)));
 
-        /* "configparserc/config.pyx":383
+        /* "configparserc/config.pyx":388
  *             err = 0
  *             size = strlen(text) * sizeof(char)
  *             fd = fmemopen(text, size, 'r')             # <<<<<<<<<<<<<<
  *         if fd == NULL:
  *             printf('Failed to open memory stream for text - `%s`; size - %zu\n', text, size)
  */
         __pyx_v_fd = fmemopen(__pyx_v_text, __pyx_v_size, ((char const *)"r"));
       }
 
-      /* "configparserc/config.pyx":380
+      /* "configparserc/config.pyx":385
  *             int err
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             err = 0
  *             size = strlen(text) * sizeof(char)
  */
       /*finally:*/ {
@@ -11749,89 +12169,89 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "configparserc/config.pyx":384
+  /* "configparserc/config.pyx":389
  *             size = strlen(text) * sizeof(char)
  *             fd = fmemopen(text, size, 'r')
  *         if fd == NULL:             # <<<<<<<<<<<<<<
  *             printf('Failed to open memory stream for text - `%s`; size - %zu\n', text, size)
  *             return err
  */
   __pyx_t_1 = ((__pyx_v_fd == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":385
+    /* "configparserc/config.pyx":390
  *             fd = fmemopen(text, size, 'r')
  *         if fd == NULL:
  *             printf('Failed to open memory stream for text - `%s`; size - %zu\n', text, size)             # <<<<<<<<<<<<<<
  *             return err
  *         err = self._parse_file(fd, size)
  */
     (void)(printf(((char const *)"Failed to open memory stream for text - `%s`; size - %zu\n"), __pyx_v_text, __pyx_v_size));
 
-    /* "configparserc/config.pyx":386
+    /* "configparserc/config.pyx":391
  *         if fd == NULL:
  *             printf('Failed to open memory stream for text - `%s`; size - %zu\n', text, size)
  *             return err             # <<<<<<<<<<<<<<
  *         err = self._parse_file(fd, size)
  *         fclose(fd)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":384
+    /* "configparserc/config.pyx":389
  *             size = strlen(text) * sizeof(char)
  *             fd = fmemopen(text, size, 'r')
  *         if fd == NULL:             # <<<<<<<<<<<<<<
  *             printf('Failed to open memory stream for text - `%s`; size - %zu\n', text, size)
  *             return err
  */
   }
 
-  /* "configparserc/config.pyx":387
+  /* "configparserc/config.pyx":392
  *             printf('Failed to open memory stream for text - `%s`; size - %zu\n', text, size)
  *             return err
  *         err = self._parse_file(fd, size)             # <<<<<<<<<<<<<<
  *         fclose(fd)
  *         return err
  */
   __pyx_v_err = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_file(__pyx_v_self, __pyx_v_fd, __pyx_v_size);
 
-  /* "configparserc/config.pyx":388
+  /* "configparserc/config.pyx":393
  *             return err
  *         err = self._parse_file(fd, size)
  *         fclose(fd)             # <<<<<<<<<<<<<<
  *         return err
  * 
  */
   (void)(fclose(__pyx_v_fd));
 
-  /* "configparserc/config.pyx":389
+  /* "configparserc/config.pyx":394
  *         err = self._parse_file(fd, size)
  *         fclose(fd)
  *         return err             # <<<<<<<<<<<<<<
  * 
  *     def parse_file(self, filename):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_err); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":374
+  /* "configparserc/config.pyx":379
  *         return err
  * 
  *     cdef _parse_text(self, char* text):             # <<<<<<<<<<<<<<
  *         cdef:
  *             FILE *fd
  */
 
@@ -11843,15 +12263,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":391
+/* "configparserc/config.pyx":396
  *         return err
  * 
  *     def parse_file(self, filename):             # <<<<<<<<<<<<<<
  *         error = self._parse_file_by_name(filename.encode('utf-8'))
  *         if error:
  */
 
@@ -11880,103 +12300,103 @@
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   Py_UCS4 __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_file", 0);
-  __Pyx_TraceCall("parse_file", __pyx_f[0], 391, 0, __PYX_ERR(0, 391, __pyx_L1_error));
+  __Pyx_TraceCall("parse_file", __pyx_f[0], 396, 0, __PYX_ERR(0, 396, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":392
+  /* "configparserc/config.pyx":397
  * 
  *     def parse_file(self, filename):
  *         error = self._parse_file_by_name(filename.encode('utf-8'))             # <<<<<<<<<<<<<<
  *         if error:
  *             raise ParseError(f'Couldnt parse config string without section or key-value in file `{filename}`.')
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 392, __pyx_L1_error)
-  __pyx_t_2 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_file_by_name(__pyx_v_self, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_file_by_name(__pyx_v_self, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_error = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "configparserc/config.pyx":393
+  /* "configparserc/config.pyx":398
  *     def parse_file(self, filename):
  *         error = self._parse_file_by_name(filename.encode('utf-8'))
  *         if error:             # <<<<<<<<<<<<<<
  *             raise ParseError(f'Couldnt parse config string without section or key-value in file `{filename}`.')
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_error); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_error); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 398, __pyx_L1_error)
   if (unlikely(__pyx_t_5)) {
 
-    /* "configparserc/config.pyx":394
+    /* "configparserc/config.pyx":399
  *         error = self._parse_file_by_name(filename.encode('utf-8'))
  *         if error:
  *             raise ParseError(f'Couldnt parse config string without section or key-value in file `{filename}`.')             # <<<<<<<<<<<<<<
  * 
  *     def parse_yaml_file(self, filename):
  */
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Couldnt_parse_config_string_with);
     __pyx_t_6 += 66;
     __Pyx_GIVEREF(__pyx_kp_u_Couldnt_parse_config_string_with);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_Couldnt_parse_config_string_with);
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_filename, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_filename, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_kp_u__12);
     __pyx_t_6 += 2;
     __Pyx_GIVEREF(__pyx_kp_u__12);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u__12);
-    __pyx_t_1 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_13configparserc_6config_ParseError), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_13configparserc_6config_ParseError), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 394, __pyx_L1_error)
+    __PYX_ERR(0, 399, __pyx_L1_error)
 
-    /* "configparserc/config.pyx":393
+    /* "configparserc/config.pyx":398
  *     def parse_file(self, filename):
  *         error = self._parse_file_by_name(filename.encode('utf-8'))
  *         if error:             # <<<<<<<<<<<<<<
  *             raise ParseError(f'Couldnt parse config string without section or key-value in file `{filename}`.')
  * 
  */
   }
 
-  /* "configparserc/config.pyx":391
+  /* "configparserc/config.pyx":396
  *         return err
  * 
  *     def parse_file(self, filename):             # <<<<<<<<<<<<<<
  *         error = self._parse_file_by_name(filename.encode('utf-8'))
  *         if error:
  */
 
@@ -11993,15 +12413,15 @@
   __Pyx_XDECREF(__pyx_v_error);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":396
+/* "configparserc/config.pyx":401
  *             raise ParseError(f'Couldnt parse config string without section or key-value in file `{filename}`.')
  * 
  *     def parse_yaml_file(self, filename):             # <<<<<<<<<<<<<<
  *         with File(filename) as fd:
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  */
 
@@ -12044,58 +12464,58 @@
   int __pyx_t_16;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_yaml_file", 0);
-  __Pyx_TraceCall("parse_yaml_file", __pyx_f[0], 396, 0, __PYX_ERR(0, 396, __pyx_L1_error));
+  __Pyx_TraceCall("parse_yaml_file", __pyx_f[0], 401, 0, __PYX_ERR(0, 401, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":397
+  /* "configparserc/config.pyx":402
  * 
  *     def parse_yaml_file(self, filename):
  *         with File(filename) as fd:             # <<<<<<<<<<<<<<
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  *                 if not document:
  */
   /*with:*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_File); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_filename);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 397, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 397, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
@@ -12105,218 +12525,218 @@
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
           __pyx_v_fd = __pyx_t_3;
           __pyx_t_3 = 0;
 
-          /* "configparserc/config.pyx":398
+          /* "configparserc/config.pyx":403
  *     def parse_yaml_file(self, filename):
  *         with File(filename) as fd:
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):             # <<<<<<<<<<<<<<
  *                 if not document:
  *                     continue
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_yaml); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_yaml); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_load_all); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L7_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_load_all); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L7_error)
+          __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_INCREF(__pyx_v_fd);
           __Pyx_GIVEREF(__pyx_v_fd);
           PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_fd);
-          __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_YAML_LOADER); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 398, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_YAML_LOADER); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
-          if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_Loader, __pyx_t_5) < 0) __PYX_ERR(0, 398, __pyx_L7_error)
+          if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_Loader, __pyx_t_5) < 0) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 398, __pyx_L7_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
             __pyx_t_2 = __pyx_t_5; __Pyx_INCREF(__pyx_t_2); __pyx_t_9 = 0;
             __pyx_t_10 = NULL;
           } else {
-            __pyx_t_9 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L7_error)
+            __pyx_t_9 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_10 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 398, __pyx_L7_error)
+            __pyx_t_10 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 403, __pyx_L7_error)
           }
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           for (;;) {
             if (likely(!__pyx_t_10)) {
               if (likely(PyList_CheckExact(__pyx_t_2))) {
                 if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_2)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_5); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 398, __pyx_L7_error)
+                __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_5); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 403, __pyx_L7_error)
                 #else
-                __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 398, __pyx_L7_error)
+                __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_5);
                 #endif
               } else {
                 if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_5); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 398, __pyx_L7_error)
+                __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_5); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 403, __pyx_L7_error)
                 #else
-                __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 398, __pyx_L7_error)
+                __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_5);
                 #endif
               }
             } else {
               __pyx_t_5 = __pyx_t_10(__pyx_t_2);
               if (unlikely(!__pyx_t_5)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 398, __pyx_L7_error)
+                  else __PYX_ERR(0, 403, __pyx_L7_error)
                 }
                 break;
               }
               __Pyx_GOTREF(__pyx_t_5);
             }
             __Pyx_XDECREF_SET(__pyx_v_document, __pyx_t_5);
             __pyx_t_5 = 0;
 
-            /* "configparserc/config.pyx":399
+            /* "configparserc/config.pyx":404
  *         with File(filename) as fd:
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  *                 if not document:             # <<<<<<<<<<<<<<
  *                     continue
  *                 for section_name, section_data in document.items():
  */
-            __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_document); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 399, __pyx_L7_error)
+            __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_document); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 404, __pyx_L7_error)
             __pyx_t_12 = ((!__pyx_t_11) != 0);
             if (__pyx_t_12) {
 
-              /* "configparserc/config.pyx":400
+              /* "configparserc/config.pyx":405
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  *                 if not document:
  *                     continue             # <<<<<<<<<<<<<<
  *                 for section_name, section_data in document.items():
  *                     if section_name in self:
  */
               goto __pyx_L13_continue;
 
-              /* "configparserc/config.pyx":399
+              /* "configparserc/config.pyx":404
  *         with File(filename) as fd:
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  *                 if not document:             # <<<<<<<<<<<<<<
  *                     continue
  *                 for section_name, section_data in document.items():
  */
             }
 
-            /* "configparserc/config.pyx":401
+            /* "configparserc/config.pyx":406
  *                 if not document:
  *                     continue
  *                 for section_name, section_data in document.items():             # <<<<<<<<<<<<<<
  *                     if section_name in self:
  *                         self[section_name].update(section_data)
  */
             __pyx_t_13 = 0;
             if (unlikely(__pyx_v_document == Py_None)) {
               PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-              __PYX_ERR(0, 401, __pyx_L7_error)
+              __PYX_ERR(0, 406, __pyx_L7_error)
             }
-            __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_document, 0, __pyx_n_s_items, (&__pyx_t_14), (&__pyx_t_15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L7_error)
+            __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_document, 0, __pyx_n_s_items, (&__pyx_t_14), (&__pyx_t_15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_XDECREF(__pyx_t_5);
             __pyx_t_5 = __pyx_t_3;
             __pyx_t_3 = 0;
             while (1) {
               __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_5, __pyx_t_14, &__pyx_t_13, &__pyx_t_3, &__pyx_t_1, NULL, __pyx_t_15);
               if (unlikely(__pyx_t_16 == 0)) break;
-              if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 401, __pyx_L7_error)
+              if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 406, __pyx_L7_error)
               __Pyx_GOTREF(__pyx_t_3);
               __Pyx_GOTREF(__pyx_t_1);
               __Pyx_XDECREF_SET(__pyx_v_section_name, __pyx_t_3);
               __pyx_t_3 = 0;
               __Pyx_XDECREF_SET(__pyx_v_section_data, __pyx_t_1);
               __pyx_t_1 = 0;
 
-              /* "configparserc/config.pyx":402
+              /* "configparserc/config.pyx":407
  *                     continue
  *                 for section_name, section_data in document.items():
  *                     if section_name in self:             # <<<<<<<<<<<<<<
  *                         self[section_name].update(section_data)
  *                     else:
  */
-              __pyx_t_12 = (__Pyx_PySequence_ContainsTF(__pyx_v_section_name, ((PyObject *)__pyx_v_self), Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 402, __pyx_L7_error)
+              __pyx_t_12 = (__Pyx_PySequence_ContainsTF(__pyx_v_section_name, ((PyObject *)__pyx_v_self), Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 407, __pyx_L7_error)
               __pyx_t_11 = (__pyx_t_12 != 0);
               if (__pyx_t_11) {
 
-                /* "configparserc/config.pyx":403
+                /* "configparserc/config.pyx":408
  *                 for section_name, section_data in document.items():
  *                     if section_name in self:
  *                         self[section_name].update(section_data)             # <<<<<<<<<<<<<<
  *                     else:
  *                         self[section_name] = section_data
  */
-                __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L7_error)
+                __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_section_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_3);
-                __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_update); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 403, __pyx_L7_error)
+                __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_update); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 408, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_17);
                 __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
                 __pyx_t_3 = NULL;
                 if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_17))) {
                   __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_17);
                   if (likely(__pyx_t_3)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_17);
                     __Pyx_INCREF(__pyx_t_3);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_17, function);
                   }
                 }
                 __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_17, __pyx_t_3, __pyx_v_section_data) : __Pyx_PyObject_CallOneArg(__pyx_t_17, __pyx_v_section_data);
                 __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-                if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L7_error)
+                if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L7_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-                /* "configparserc/config.pyx":402
+                /* "configparserc/config.pyx":407
  *                     continue
  *                 for section_name, section_data in document.items():
  *                     if section_name in self:             # <<<<<<<<<<<<<<
  *                         self[section_name].update(section_data)
  *                     else:
  */
                 goto __pyx_L18;
               }
 
-              /* "configparserc/config.pyx":405
+              /* "configparserc/config.pyx":410
  *                         self[section_name].update(section_data)
  *                     else:
  *                         self[section_name] = section_data             # <<<<<<<<<<<<<<
  * 
  *     def parse_files(self, filename_array: _t.Sequence):
  */
               /*else*/ {
-                if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_section_name, __pyx_v_section_data) < 0)) __PYX_ERR(0, 405, __pyx_L7_error)
+                if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_section_name, __pyx_v_section_data) < 0)) __PYX_ERR(0, 410, __pyx_L7_error)
               }
               __pyx_L18:;
             }
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-            /* "configparserc/config.pyx":398
+            /* "configparserc/config.pyx":403
  *     def parse_yaml_file(self, filename):
  *         with File(filename) as fd:
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):             # <<<<<<<<<<<<<<
  *                 if not document:
  *                     continue
  */
             __pyx_L13_continue:;
           }
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "configparserc/config.pyx":397
+          /* "configparserc/config.pyx":402
  * 
  *     def parse_yaml_file(self, filename):
  *         with File(filename) as fd:             # <<<<<<<<<<<<<<
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  *                 if not document:
  */
         }
@@ -12328,36 +12748,36 @@
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("configparserc.config.ConfigParserC.parse_yaml_file", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(0, 397, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(0, 402, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_17 = PyTuple_Pack(3, __pyx_t_2, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 397, __pyx_L9_except_error)
+          __pyx_t_17 = PyTuple_Pack(3, __pyx_t_2, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 402, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_17);
           __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_17, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-          if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 397, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 402, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_18);
           __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_18);
           __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-          if (__pyx_t_11 < 0) __PYX_ERR(0, 397, __pyx_L9_except_error)
+          if (__pyx_t_11 < 0) __PYX_ERR(0, 402, __pyx_L9_except_error)
           __pyx_t_12 = ((!(__pyx_t_11 != 0)) != 0);
           if (__pyx_t_12) {
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_GIVEREF(__pyx_t_5);
             __Pyx_XGIVEREF(__pyx_t_1);
             __Pyx_ErrRestoreWithState(__pyx_t_2, __pyx_t_5, __pyx_t_1);
             __pyx_t_2 = 0; __pyx_t_5 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 397, __pyx_L9_except_error)
+            __PYX_ERR(0, 402, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -12375,30 +12795,30 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__13, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 397, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 402, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L22;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L22:;
   }
 
-  /* "configparserc/config.pyx":396
+  /* "configparserc/config.pyx":401
  *             raise ParseError(f'Couldnt parse config string without section or key-value in file `{filename}`.')
  * 
  *     def parse_yaml_file(self, filename):             # <<<<<<<<<<<<<<
  *         with File(filename) as fd:
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  */
 
@@ -12420,15 +12840,15 @@
   __Pyx_XDECREF(__pyx_v_section_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":407
+/* "configparserc/config.pyx":412
  *                         self[section_name] = section_data
  * 
  *     def parse_files(self, filename_array: _t.Sequence):             # <<<<<<<<<<<<<<
  *         for filepath in list(filter(bool, filename_array))[::-1]:
  *             if not os.path.exists(filepath):
  */
 
@@ -12457,211 +12877,211 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_files", 0);
-  __Pyx_TraceCall("parse_files", __pyx_f[0], 407, 0, __PYX_ERR(0, 407, __pyx_L1_error));
+  __Pyx_TraceCall("parse_files", __pyx_f[0], 412, 0, __PYX_ERR(0, 412, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":408
+  /* "configparserc/config.pyx":413
  * 
  *     def parse_files(self, filename_array: _t.Sequence):
  *         for filepath in list(filter(bool, filename_array))[::-1]:             # <<<<<<<<<<<<<<
  *             if not os.path.exists(filepath):
  *                 continue
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject*)&PyBool_Type));
   __Pyx_GIVEREF(((PyObject*)&PyBool_Type));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject*)&PyBool_Type));
   __Pyx_INCREF(__pyx_v_filename_array);
   __Pyx_GIVEREF(__pyx_v_filename_array);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_filename_array);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_slice__14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_slice__14); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 413, __pyx_L1_error)
     #else
-    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_filepath, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "configparserc/config.pyx":409
+    /* "configparserc/config.pyx":414
  *     def parse_files(self, filename_array: _t.Sequence):
  *         for filepath in list(filter(bool, filename_array))[::-1]:
  *             if not os.path.exists(filepath):             # <<<<<<<<<<<<<<
  *                 continue
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_filepath) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_filepath);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_7 = ((!__pyx_t_6) != 0);
     if (__pyx_t_7) {
 
-      /* "configparserc/config.pyx":410
+      /* "configparserc/config.pyx":415
  *         for filepath in list(filter(bool, filename_array))[::-1]:
  *             if not os.path.exists(filepath):
  *                 continue             # <<<<<<<<<<<<<<
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):
  *                 self.parse_yaml_file(filepath)
  */
       goto __pyx_L3_continue;
 
-      /* "configparserc/config.pyx":409
+      /* "configparserc/config.pyx":414
  *     def parse_files(self, filename_array: _t.Sequence):
  *         for filepath in list(filter(bool, filename_array))[::-1]:
  *             if not os.path.exists(filepath):             # <<<<<<<<<<<<<<
  *                 continue
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):
  */
     }
 
-    /* "configparserc/config.pyx":411
+    /* "configparserc/config.pyx":416
  *             if not os.path.exists(filepath):
  *                 continue
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):             # <<<<<<<<<<<<<<
  *                 self.parse_yaml_file(filepath)
  *             else:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filepath, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filepath, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_4, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_4, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_yaml, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_yaml, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 416, __pyx_L1_error)
     if (!__pyx_t_6) {
     } else {
       __pyx_t_7 = __pyx_t_6;
       goto __pyx_L7_bool_binop_done;
     }
-    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_yml, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_yml, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 416, __pyx_L1_error)
     __pyx_t_7 = __pyx_t_6;
     __pyx_L7_bool_binop_done:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_6 = (__pyx_t_7 != 0);
     if (__pyx_t_6) {
 
-      /* "configparserc/config.pyx":412
+      /* "configparserc/config.pyx":417
  *                 continue
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):
  *                 self.parse_yaml_file(filepath)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.parse_file(filepath)
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_yaml_file); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_yaml_file); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_filepath) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_filepath);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "configparserc/config.pyx":411
+      /* "configparserc/config.pyx":416
  *             if not os.path.exists(filepath):
  *                 continue
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):             # <<<<<<<<<<<<<<
  *                 self.parse_yaml_file(filepath)
  *             else:
  */
       goto __pyx_L6;
     }
 
-    /* "configparserc/config.pyx":414
+    /* "configparserc/config.pyx":419
  *                 self.parse_yaml_file(filepath)
  *             else:
  *                 self.parse_file(filepath)             # <<<<<<<<<<<<<<
  * 
  *     def parse_text(self, text):
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_file); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse_file); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_filepath) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_filepath);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L6:;
 
-    /* "configparserc/config.pyx":408
+    /* "configparserc/config.pyx":413
  * 
  *     def parse_files(self, filename_array: _t.Sequence):
  *         for filepath in list(filter(bool, filename_array))[::-1]:             # <<<<<<<<<<<<<<
  *             if not os.path.exists(filepath):
  *                 continue
  */
     __pyx_L3_continue:;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":407
+  /* "configparserc/config.pyx":412
  *                         self[section_name] = section_data
  * 
  *     def parse_files(self, filename_array: _t.Sequence):             # <<<<<<<<<<<<<<
  *         for filepath in list(filter(bool, filename_array))[::-1]:
  *             if not os.path.exists(filepath):
  */
 
@@ -12679,15 +13099,15 @@
   __Pyx_XDECREF(__pyx_v_filepath);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":416
+/* "configparserc/config.pyx":421
  *                 self.parse_file(filepath)
  * 
  *     def parse_text(self, text):             # <<<<<<<<<<<<<<
  *         if not text:
  *             return
  */
 
@@ -12715,111 +13135,111 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_text", 0);
-  __Pyx_TraceCall("parse_text", __pyx_f[0], 416, 0, __PYX_ERR(0, 416, __pyx_L1_error));
+  __Pyx_TraceCall("parse_text", __pyx_f[0], 421, 0, __PYX_ERR(0, 421, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":417
+  /* "configparserc/config.pyx":422
  * 
  *     def parse_text(self, text):
  *         if not text:             # <<<<<<<<<<<<<<
  *             return
  *         error = self._parse_text(text.encode('utf-8'))
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_text); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_text); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 422, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":418
+    /* "configparserc/config.pyx":423
  *     def parse_text(self, text):
  *         if not text:
  *             return             # <<<<<<<<<<<<<<
  *         error = self._parse_text(text.encode('utf-8'))
  *         if error:
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":417
+    /* "configparserc/config.pyx":422
  * 
  *     def parse_text(self, text):
  *         if not text:             # <<<<<<<<<<<<<<
  *             return
  *         error = self._parse_text(text.encode('utf-8'))
  */
   }
 
-  /* "configparserc/config.pyx":419
+  /* "configparserc/config.pyx":424
  *         if not text:
  *             return
  *         error = self._parse_text(text.encode('utf-8'))             # <<<<<<<<<<<<<<
  *         if error:
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 419, __pyx_L1_error)
-  __pyx_t_4 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_text(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC *)__pyx_v_self->__pyx_vtab)->_parse_text(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_error = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "configparserc/config.pyx":420
+  /* "configparserc/config.pyx":425
  *             return
  *         error = self._parse_text(text.encode('utf-8'))
  *         if error:             # <<<<<<<<<<<<<<
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_error); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_error); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
   if (unlikely(__pyx_t_2)) {
 
-    /* "configparserc/config.pyx":421
+    /* "configparserc/config.pyx":426
  *         error = self._parse_text(text.encode('utf-8'))
  *         if error:
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_13configparserc_6config_ParseError), __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_13configparserc_6config_ParseError), __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 421, __pyx_L1_error)
+    __PYX_ERR(0, 426, __pyx_L1_error)
 
-    /* "configparserc/config.pyx":420
+    /* "configparserc/config.pyx":425
  *             return
  *         error = self._parse_text(text.encode('utf-8'))
  *         if error:             # <<<<<<<<<<<<<<
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')
  * 
  */
   }
 
-  /* "configparserc/config.pyx":416
+  /* "configparserc/config.pyx":421
  *                 self.parse_file(filepath)
  * 
  *     def parse_text(self, text):             # <<<<<<<<<<<<<<
  *         if not text:
  *             return
  */
 
@@ -12836,15 +13256,15 @@
   __Pyx_XDECREF(__pyx_v_error);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":423
+/* "configparserc/config.pyx":428
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         return {
  *             key: self[key].all()
  */
 
@@ -12873,108 +13293,108 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("all", 0);
-  __Pyx_TraceCall("all", __pyx_f[0], 423, 0, __PYX_ERR(0, 423, __pyx_L1_error));
+  __Pyx_TraceCall("all", __pyx_f[0], 428, 0, __PYX_ERR(0, 428, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":424
+  /* "configparserc/config.pyx":429
  * 
  *     def all(self):
  *         return {             # <<<<<<<<<<<<<<
  *             key: self[key].all()
  *             for key in self
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L5_error)
+    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "configparserc/config.pyx":426
+    /* "configparserc/config.pyx":431
  *         return {
  *             key: self[key].all()
  *             for key in self             # <<<<<<<<<<<<<<
  *         }
  * 
  */
     if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
       __pyx_t_2 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 431, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 426, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 431, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 426, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 431, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 426, __pyx_L5_error)
+            else __PYX_ERR(0, 431, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_key, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "configparserc/config.pyx":425
+      /* "configparserc/config.pyx":430
  *     def all(self):
  *         return {
  *             key: self[key].all()             # <<<<<<<<<<<<<<
  *             for key in self
  *         }
  */
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_7genexpr__pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 425, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_7genexpr__pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 430, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_all); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 425, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_all); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 430, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 425, __pyx_L5_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 430, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_key, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 425, __pyx_L5_error)
+      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_key, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 430, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "configparserc/config.pyx":426
+      /* "configparserc/config.pyx":431
  *         return {
  *             key: self[key].all()
  *             for key in self             # <<<<<<<<<<<<<<
  *         }
  * 
  */
     }
@@ -12986,15 +13406,15 @@
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":423
+  /* "configparserc/config.pyx":428
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         return {
  *             key: self[key].all()
  */
 
@@ -13011,15 +13431,15 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":429
+/* "configparserc/config.pyx":434
  *         }
  * 
  *     def generate_config_string(self):             # <<<<<<<<<<<<<<
  *         return ''.join([self[key].generate_section_string() for key in self])
  * 
  */
 
@@ -13048,107 +13468,107 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_config_string", 0);
-  __Pyx_TraceCall("generate_config_string", __pyx_f[0], 429, 0, __PYX_ERR(0, 429, __pyx_L1_error));
+  __Pyx_TraceCall("generate_config_string", __pyx_f[0], 434, 0, __PYX_ERR(0, 434, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":430
+  /* "configparserc/config.pyx":435
  * 
  *     def generate_config_string(self):
  *         return ''.join([self[key].generate_section_string() for key in self])             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
       __pyx_t_2 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 435, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 430, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 435, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 430, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 435, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 430, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 435, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 430, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 435, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 430, __pyx_L5_error)
+            else __PYX_ERR(0, 435, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_key, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_8genexpr1__pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 430, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_8genexpr1__pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 435, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_generate_section_string); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 430, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_generate_section_string); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 435, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 430, __pyx_L5_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 435, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 430, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 435, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_key); __pyx_8genexpr1__pyx_v_key = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_key); __pyx_8genexpr1__pyx_v_key = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
-  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":429
+  /* "configparserc/config.pyx":434
  *         }
  * 
  *     def generate_config_string(self):             # <<<<<<<<<<<<<<
  *         return ''.join([self[key].generate_section_string() for key in self])
  * 
  */
 
@@ -13165,15 +13585,15 @@
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":432
+/* "configparserc/config.pyx":437
  *         return ''.join([self[key].generate_section_string() for key in self])
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return repr(self.all())
  * 
  */
 
@@ -13197,49 +13617,49 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
-  __Pyx_TraceCall("__repr__", __pyx_f[0], 432, 0, __PYX_ERR(0, 432, __pyx_L1_error));
+  __Pyx_TraceCall("__repr__", __pyx_f[0], 437, 0, __PYX_ERR(0, 437, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":433
+  /* "configparserc/config.pyx":438
  * 
  *     def __repr__(self):
  *         return repr(self.all())             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_all); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_all); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_Repr(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Repr(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":432
+  /* "configparserc/config.pyx":437
  *         return ''.join([self[key].generate_section_string() for key in self])
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return repr(self.all())
  * 
  */
 
@@ -13586,15 +14006,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":442
+/* "configparserc/config.pyx":447
  *         dict __type_map
  * 
  *     def __init__(self, name, config, default=None, type_map=None):             # <<<<<<<<<<<<<<
  *         self.name = name
  *         self.config = config
  */
 
@@ -13636,15 +14056,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_config)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 442, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 447, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_default);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -13652,15 +14072,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type_map);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 442, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 447, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -13673,15 +14093,15 @@
     __pyx_v_name = values[0];
     __pyx_v_config = values[1];
     __pyx_v_default = values[2];
     __pyx_v_type_map = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 442, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 447, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section___init__(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_name, __pyx_v_config, __pyx_v_default, __pyx_v_type_map);
 
@@ -13702,287 +14122,287 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 442, 0, __PYX_ERR(0, 442, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 447, 0, __PYX_ERR(0, 447, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":443
+  /* "configparserc/config.pyx":448
  * 
  *     def __init__(self, name, config, default=None, type_map=None):
  *         self.name = name             # <<<<<<<<<<<<<<
  *         self.config = config
  * 
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_name))||((__pyx_v_name) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_name)->tp_name), 0))) __PYX_ERR(0, 443, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_name))||((__pyx_v_name) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_name)->tp_name), 0))) __PYX_ERR(0, 448, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_name;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":444
+  /* "configparserc/config.pyx":449
  *     def __init__(self, name, config, default=None, type_map=None):
  *         self.name = name
  *         self.config = config             # <<<<<<<<<<<<<<
  * 
  *         self.__type_map = {}
  */
-  if (!(likely(((__pyx_v_config) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_config, __pyx_ptype_13configparserc_6config_ConfigParserC))))) __PYX_ERR(0, 444, __pyx_L1_error)
+  if (!(likely(((__pyx_v_config) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_config, __pyx_ptype_13configparserc_6config_ConfigParserC))))) __PYX_ERR(0, 449, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_config;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->config);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->config));
   __pyx_v_self->config = ((struct __pyx_obj_13configparserc_6config_ConfigParserC *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":446
+  /* "configparserc/config.pyx":451
  *         self.config = config
  * 
  *         self.__type_map = {}             # <<<<<<<<<<<<<<
  *         prefix = 'type_'
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->__pyx___type_map);
   __Pyx_DECREF(__pyx_v_self->__pyx___type_map);
   __pyx_v_self->__pyx___type_map = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":447
+  /* "configparserc/config.pyx":452
  * 
  *         self.__type_map = {}
  *         prefix = 'type_'             # <<<<<<<<<<<<<<
  * 
  *         if hasattr(self, 'types_map') and self.types_map:
  */
   __Pyx_INCREF(__pyx_n_u_type);
   __pyx_v_prefix = __pyx_n_u_type;
 
-  /* "configparserc/config.pyx":449
+  /* "configparserc/config.pyx":454
  *         prefix = 'type_'
  * 
  *         if hasattr(self, 'types_map') and self.types_map:             # <<<<<<<<<<<<<<
  *             self.__type_map.update(self.types_map)
  *         if type_map:
  */
-  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_types_map); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_types_map); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 454, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_types_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_types_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":450
+    /* "configparserc/config.pyx":455
  * 
  *         if hasattr(self, 'types_map') and self.types_map:
  *             self.__type_map.update(self.types_map)             # <<<<<<<<<<<<<<
  *         if type_map:
  *             self.__type_map.update(type_map)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___type_map, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 450, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___type_map, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 455, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_types_map); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 450, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_types_map); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 455, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":449
+    /* "configparserc/config.pyx":454
  *         prefix = 'type_'
  * 
  *         if hasattr(self, 'types_map') and self.types_map:             # <<<<<<<<<<<<<<
  *             self.__type_map.update(self.types_map)
  *         if type_map:
  */
   }
 
-  /* "configparserc/config.pyx":451
+  /* "configparserc/config.pyx":456
  *         if hasattr(self, 'types_map') and self.types_map:
  *             self.__type_map.update(self.types_map)
  *         if type_map:             # <<<<<<<<<<<<<<
  *             self.__type_map.update(type_map)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_type_map); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_type_map); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 456, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":452
+    /* "configparserc/config.pyx":457
  *             self.__type_map.update(self.types_map)
  *         if type_map:
  *             self.__type_map.update(type_map)             # <<<<<<<<<<<<<<
  * 
  *         if default and isinstance(default, dict):
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___type_map, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx___type_map, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 457, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_type_map) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_type_map);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":451
+    /* "configparserc/config.pyx":456
  *         if hasattr(self, 'types_map') and self.types_map:
  *             self.__type_map.update(self.types_map)
  *         if type_map:             # <<<<<<<<<<<<<<
  *             self.__type_map.update(type_map)
  * 
  */
   }
 
-  /* "configparserc/config.pyx":454
+  /* "configparserc/config.pyx":459
  *             self.__type_map.update(type_map)
  * 
  *         if default and isinstance(default, dict):             # <<<<<<<<<<<<<<
  *             super().__init__(default)
  *         else:
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_default); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_default); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 459, __pyx_L1_error)
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L8_bool_binop_done;
   }
   __pyx_t_4 = PyDict_Check(__pyx_v_default); 
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L8_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":455
+    /* "configparserc/config.pyx":460
  * 
  *         if default and isinstance(default, dict):
  *             super().__init__(default)             # <<<<<<<<<<<<<<
  *         else:
  *             super().__init__()
  */
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 455, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 460, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
     __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
     PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_Section));
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_self));
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 455, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 460, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 455, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 460, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_default) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_default);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":454
+    /* "configparserc/config.pyx":459
  *             self.__type_map.update(type_map)
  * 
  *         if default and isinstance(default, dict):             # <<<<<<<<<<<<<<
  *             super().__init__(default)
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "configparserc/config.pyx":457
+  /* "configparserc/config.pyx":462
  *             super().__init__(default)
  *         else:
  *             super().__init__()             # <<<<<<<<<<<<<<
  * 
  *     cdef Section get_parent(self):
  */
   /*else*/ {
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 457, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
     __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
     PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_Section));
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_self));
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 457, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 457, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L7:;
 
-  /* "configparserc/config.pyx":442
+  /* "configparserc/config.pyx":447
  *         dict __type_map
  * 
  *     def __init__(self, name, config, default=None, type_map=None):             # <<<<<<<<<<<<<<
  *         self.name = name
  *         self.config = config
  */
 
@@ -13999,15 +14419,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_prefix);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":459
+/* "configparserc/config.pyx":464
  *             super().__init__()
  * 
  *     cdef Section get_parent(self):             # <<<<<<<<<<<<<<
  *         cdef:
  *             list parent_path
  */
 
@@ -14023,138 +14443,138 @@
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_parent", 0);
-  __Pyx_TraceCall("get_parent", __pyx_f[0], 459, 0, __PYX_ERR(0, 459, __pyx_L1_error));
+  __Pyx_TraceCall("get_parent", __pyx_f[0], 464, 0, __PYX_ERR(0, 464, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":464
+  /* "configparserc/config.pyx":469
  *             Section parent
  * 
  *         parent_path = self.name.split('.')[:-1]             # <<<<<<<<<<<<<<
  *         if not parent_path:
  *             return None
  */
   if (unlikely(__pyx_v_self->name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "split");
-    __PYX_ERR(0, 464, __pyx_L1_error)
+    __PYX_ERR(0, 469, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_Split(__pyx_v_self->name, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Split(__pyx_v_self->name, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, -1L, NULL, NULL, &__pyx_slice__17, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, -1L, NULL, NULL, &__pyx_slice__17, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(PyList_CheckExact(__pyx_t_2))||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 464, __pyx_L1_error)
+  if (!(likely(PyList_CheckExact(__pyx_t_2))||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 469, __pyx_L1_error)
   __pyx_v_parent_path = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "configparserc/config.pyx":465
+  /* "configparserc/config.pyx":470
  * 
  *         parent_path = self.name.split('.')[:-1]
  *         if not parent_path:             # <<<<<<<<<<<<<<
  *             return None
  *         parent = self.config[parent_path.pop(0)]
  */
   __pyx_t_3 = (PyList_GET_SIZE(__pyx_v_parent_path) != 0);
   __pyx_t_4 = ((!__pyx_t_3) != 0);
   if (__pyx_t_4) {
 
-    /* "configparserc/config.pyx":466
+    /* "configparserc/config.pyx":471
  *         parent_path = self.name.split('.')[:-1]
  *         if not parent_path:
  *             return None             # <<<<<<<<<<<<<<
  *         parent = self.config[parent_path.pop(0)]
  *         for sub in parent_path:
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
     __pyx_r = ((struct __pyx_obj_13configparserc_6config_Section *)Py_None); __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":465
+    /* "configparserc/config.pyx":470
  * 
  *         parent_path = self.name.split('.')[:-1]
  *         if not parent_path:             # <<<<<<<<<<<<<<
  *             return None
  *         parent = self.config[parent_path.pop(0)]
  */
   }
 
-  /* "configparserc/config.pyx":467
+  /* "configparserc/config.pyx":472
  *         if not parent_path:
  *             return None
  *         parent = self.config[parent_path.pop(0)]             # <<<<<<<<<<<<<<
  *         for sub in parent_path:
  *             parent = parent[sub]
  */
-  __pyx_t_2 = __Pyx_PyList_PopIndex(__pyx_v_parent_path, __pyx_int_0, 0, 1, Py_ssize_t, PyInt_FromSsize_t); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyList_PopIndex(__pyx_v_parent_path, __pyx_int_0, 0, 1, Py_ssize_t, PyInt_FromSsize_t); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->config), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->config), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_13configparserc_6config_Section))))) __PYX_ERR(0, 467, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_13configparserc_6config_Section))))) __PYX_ERR(0, 472, __pyx_L1_error)
   __pyx_v_parent = ((struct __pyx_obj_13configparserc_6config_Section *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":468
+  /* "configparserc/config.pyx":473
  *             return None
  *         parent = self.config[parent_path.pop(0)]
  *         for sub in parent_path:             # <<<<<<<<<<<<<<
  *             parent = parent[sub]
  *         return parent
  */
   __pyx_t_1 = __pyx_v_parent_path; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
   for (;;) {
     if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 473, __pyx_L1_error)
     #else
-    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_sub, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "configparserc/config.pyx":469
+    /* "configparserc/config.pyx":474
  *         parent = self.config[parent_path.pop(0)]
  *         for sub in parent_path:
  *             parent = parent[sub]             # <<<<<<<<<<<<<<
  *         return parent
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_parent), __pyx_v_sub); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_parent), __pyx_v_sub); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 474, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_13configparserc_6config_Section))))) __PYX_ERR(0, 469, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_13configparserc_6config_Section))))) __PYX_ERR(0, 474, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_parent, ((struct __pyx_obj_13configparserc_6config_Section *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "configparserc/config.pyx":468
+    /* "configparserc/config.pyx":473
  *             return None
  *         parent = self.config[parent_path.pop(0)]
  *         for sub in parent_path:             # <<<<<<<<<<<<<<
  *             parent = parent[sub]
  *         return parent
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":470
+  /* "configparserc/config.pyx":475
  *         for sub in parent_path:
  *             parent = parent[sub]
  *         return parent             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_parent));
   __pyx_r = __pyx_v_parent;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":459
+  /* "configparserc/config.pyx":464
  *             super().__init__()
  * 
  *     cdef Section get_parent(self):             # <<<<<<<<<<<<<<
  *         cdef:
  *             list parent_path
  */
 
@@ -14170,15 +14590,15 @@
   __Pyx_XDECREF(__pyx_v_sub);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":473
+/* "configparserc/config.pyx":478
  * 
  *     @property
  *     def parent(self):             # <<<<<<<<<<<<<<
  *         return self.get_parent()
  * 
  */
 
@@ -14200,31 +14620,31 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 473, 0, __PYX_ERR(0, 473, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[0], 478, 0, __PYX_ERR(0, 478, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":474
+  /* "configparserc/config.pyx":479
  *     @property
  *     def parent(self):
  *         return self.get_parent()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->get_parent(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->get_parent(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":473
+  /* "configparserc/config.pyx":478
  * 
  *     @property
  *     def parent(self):             # <<<<<<<<<<<<<<
  *         return self.get_parent()
  * 
  */
 
@@ -14236,15 +14656,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":477
+/* "configparserc/config.pyx":482
  * 
  *     @property
  *     def main_config(self):             # <<<<<<<<<<<<<<
  *         return self.config
  * 
  */
 
@@ -14265,29 +14685,29 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 477, 0, __PYX_ERR(0, 477, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[0], 482, 0, __PYX_ERR(0, 482, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":478
+  /* "configparserc/config.pyx":483
  *     @property
  *     def main_config(self):
  *         return self.config             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->config));
   __pyx_r = ((PyObject *)__pyx_v_self->config);
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":477
+  /* "configparserc/config.pyx":482
  * 
  *     @property
  *     def main_config(self):             # <<<<<<<<<<<<<<
  *         return self.config
  * 
  */
 
@@ -14298,15 +14718,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":480
+/* "configparserc/config.pyx":485
  *         return self.config
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return json.dumps(self.all())
  * 
  */
 
@@ -14332,44 +14752,44 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
-  __Pyx_TraceCall("__repr__", __pyx_f[0], 480, 0, __PYX_ERR(0, 480, __pyx_L1_error));
+  __Pyx_TraceCall("__repr__", __pyx_f[0], 485, 0, __PYX_ERR(0, 485, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":481
+  /* "configparserc/config.pyx":486
  * 
  *     def __repr__(self):
  *         return json.dumps(self.all())             # <<<<<<<<<<<<<<
  * 
  *     cdef __set_item_value(self, str key, object value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_all); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_all); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -14377,22 +14797,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":480
+  /* "configparserc/config.pyx":485
  *         return self.config
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return json.dumps(self.all())
  * 
  */
 
@@ -14408,15 +14828,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":483
+/* "configparserc/config.pyx":488
  *         return json.dumps(self.all())
  * 
  *     cdef __set_item_value(self, str key, object value):             # <<<<<<<<<<<<<<
  *         cdef:
  *             object format_string
  */
 
@@ -14434,31 +14854,31 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set_item_value", 0);
-  __Pyx_TraceCall("__set_item_value", __pyx_f[0], 483, 0, __PYX_ERR(0, 483, __pyx_L1_error));
+  __Pyx_TraceCall("__set_item_value", __pyx_f[0], 488, 0, __PYX_ERR(0, 488, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_key);
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "configparserc/config.pyx":487
+  /* "configparserc/config.pyx":492
  *             object format_string
  * 
  *         format_string = self.config.format_string             # <<<<<<<<<<<<<<
  *         key = format_string(key, self.name)
  *         if isinstance(value, dict) and not isinstance(value, Section):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_format_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_format_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 492, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_format_string = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":488
+  /* "configparserc/config.pyx":493
  * 
  *         format_string = self.config.format_string
  *         key = format_string(key, self.name)             # <<<<<<<<<<<<<<
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             section = self.config.get_section_instance(self._get_subsection_name(key))
  */
   __Pyx_INCREF(__pyx_v_format_string);
@@ -14473,49 +14893,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_key, __pyx_v_self->name};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_key, __pyx_v_self->name};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_key);
     __Pyx_GIVEREF(__pyx_v_key);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_key);
     __Pyx_INCREF(__pyx_v_self->name);
     __Pyx_GIVEREF(__pyx_v_self->name);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_self->name);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 488, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":489
+  /* "configparserc/config.pyx":494
  *         format_string = self.config.format_string
  *         key = format_string(key, self.name)
  *         if isinstance(value, dict) and not isinstance(value, Section):             # <<<<<<<<<<<<<<
  *             section = self.config.get_section_instance(self._get_subsection_name(key))
  *             section.update(value)
  */
   __pyx_t_7 = PyDict_Check(__pyx_v_value); 
@@ -14527,102 +14947,102 @@
   }
   __pyx_t_8 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_13configparserc_6config_Section); 
   __pyx_t_7 = ((!(__pyx_t_8 != 0)) != 0);
   __pyx_t_6 = __pyx_t_7;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "configparserc/config.pyx":490
+    /* "configparserc/config.pyx":495
  *         key = format_string(key, self.name)
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             section = self.config.get_section_instance(self._get_subsection_name(key))             # <<<<<<<<<<<<<<
  *             section.update(value)
  *             value = section
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->_get_subsection_name(__pyx_v_self, __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_5 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->_get_subsection_name(__pyx_v_self, __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 495, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 490, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_section = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":491
+    /* "configparserc/config.pyx":496
  *         if isinstance(value, dict) and not isinstance(value, Section):
  *             section = self.config.get_section_instance(self._get_subsection_name(key))
  *             section.update(value)             # <<<<<<<<<<<<<<
  *             value = section
  *         elif isinstance(value, str):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_section, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 491, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":492
+    /* "configparserc/config.pyx":497
  *             section = self.config.get_section_instance(self._get_subsection_name(key))
  *             section.update(value)
  *             value = section             # <<<<<<<<<<<<<<
  *         elif isinstance(value, str):
  *             value = format_string(value, self.name)
  */
     __Pyx_INCREF(__pyx_v_section);
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_v_section);
 
-    /* "configparserc/config.pyx":489
+    /* "configparserc/config.pyx":494
  *         format_string = self.config.format_string
  *         key = format_string(key, self.name)
  *         if isinstance(value, dict) and not isinstance(value, Section):             # <<<<<<<<<<<<<<
  *             section = self.config.get_section_instance(self._get_subsection_name(key))
  *             section.update(value)
  */
     goto __pyx_L3;
   }
 
-  /* "configparserc/config.pyx":493
+  /* "configparserc/config.pyx":498
  *             section.update(value)
  *             value = section
  *         elif isinstance(value, str):             # <<<<<<<<<<<<<<
  *             value = format_string(value, self.name)
  *         PyDict_SetItem(self, key, self.type_conversation(key, value))
  */
   __pyx_t_6 = PyUnicode_Check(__pyx_v_value); 
   __pyx_t_7 = (__pyx_t_6 != 0);
   if (__pyx_t_7) {
 
-    /* "configparserc/config.pyx":494
+    /* "configparserc/config.pyx":499
  *             value = section
  *         elif isinstance(value, str):
  *             value = format_string(value, self.name)             # <<<<<<<<<<<<<<
  *         PyDict_SetItem(self, key, self.type_conversation(key, value))
  * 
  */
     __Pyx_INCREF(__pyx_v_format_string);
@@ -14637,70 +15057,70 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_value, __pyx_v_self->name};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_value, __pyx_v_self->name};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_4, __pyx_v_value);
       __Pyx_INCREF(__pyx_v_self->name);
       __Pyx_GIVEREF(__pyx_v_self->name);
       PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_4, __pyx_v_self->name);
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":493
+    /* "configparserc/config.pyx":498
  *             section.update(value)
  *             value = section
  *         elif isinstance(value, str):             # <<<<<<<<<<<<<<
  *             value = format_string(value, self.name)
  *         PyDict_SetItem(self, key, self.type_conversation(key, value))
  */
   }
   __pyx_L3:;
 
-  /* "configparserc/config.pyx":495
+  /* "configparserc/config.pyx":500
  *         elif isinstance(value, str):
  *             value = format_string(value, self.name)
  *         PyDict_SetItem(self, key, self.type_conversation(key, value))             # <<<<<<<<<<<<<<
  * 
  *     cdef object __get_item_value(self, str item):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, __pyx_v_key, __pyx_v_value, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, __pyx_v_key, __pyx_v_value, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyDict_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_4 = PyDict_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":483
+  /* "configparserc/config.pyx":488
  *         return json.dumps(self.all())
  * 
  *     cdef __set_item_value(self, str key, object value):             # <<<<<<<<<<<<<<
  *         cdef:
  *             object format_string
  */
 
@@ -14721,15 +15141,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":497
+/* "configparserc/config.pyx":502
  *         PyDict_SetItem(self, key, self.type_conversation(key, value))
  * 
  *     cdef object __get_item_value(self, str item):             # <<<<<<<<<<<<<<
  *         cdef:
  *             object value
  */
 
@@ -14743,121 +15163,121 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_item_value", 0);
-  __Pyx_TraceCall("__get_item_value", __pyx_f[0], 497, 0, __PYX_ERR(0, 497, __pyx_L1_error));
+  __Pyx_TraceCall("__get_item_value", __pyx_f[0], 502, 0, __PYX_ERR(0, 502, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":501
+  /* "configparserc/config.pyx":506
  *             object value
  * 
  *         if item not in self:             # <<<<<<<<<<<<<<
  *             value = self.__get_default_value(item)
  *         else:
  */
-  __pyx_t_1 = (__Pyx_PySequence_ContainsTF(__pyx_v_item, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PySequence_ContainsTF(__pyx_v_item, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 506, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":502
+    /* "configparserc/config.pyx":507
  * 
  *         if item not in self:
  *             value = self.__get_default_value(item)             # <<<<<<<<<<<<<<
  *         else:
  *             value = <object>PyDict_GetItem(self, item)
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_value(__pyx_v_self, __pyx_v_item); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_value(__pyx_v_self, __pyx_v_item); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "configparserc/config.pyx":501
+    /* "configparserc/config.pyx":506
  *             object value
  * 
  *         if item not in self:             # <<<<<<<<<<<<<<
  *             value = self.__get_default_value(item)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "configparserc/config.pyx":504
+  /* "configparserc/config.pyx":509
  *             value = self.__get_default_value(item)
  *         else:
  *             value = <object>PyDict_GetItem(self, item)             # <<<<<<<<<<<<<<
  *             if isinstance(value, Section) and not value:
  *                 value = self.__get_default_value(item)
  */
   /*else*/ {
     __pyx_t_4 = PyDict_GetItem(((PyObject *)__pyx_v_self), __pyx_v_item);
     __pyx_t_3 = ((PyObject *)__pyx_t_4);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_value = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "configparserc/config.pyx":505
+    /* "configparserc/config.pyx":510
  *         else:
  *             value = <object>PyDict_GetItem(self, item)
  *             if isinstance(value, Section) and not value:             # <<<<<<<<<<<<<<
  *                 value = self.__get_default_value(item)
  *         return self.type_conversation(item, value)
  */
     __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_13configparserc_6config_Section); 
     __pyx_t_5 = (__pyx_t_1 != 0);
     if (__pyx_t_5) {
     } else {
       __pyx_t_2 = __pyx_t_5;
       goto __pyx_L5_bool_binop_done;
     }
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 505, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 510, __pyx_L1_error)
     __pyx_t_1 = ((!__pyx_t_5) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "configparserc/config.pyx":506
+      /* "configparserc/config.pyx":511
  *             value = <object>PyDict_GetItem(self, item)
  *             if isinstance(value, Section) and not value:
  *                 value = self.__get_default_value(item)             # <<<<<<<<<<<<<<
  *         return self.type_conversation(item, value)
  * 
  */
-      __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_value(__pyx_v_self, __pyx_v_item); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
+      __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_value(__pyx_v_self, __pyx_v_item); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "configparserc/config.pyx":505
+      /* "configparserc/config.pyx":510
  *         else:
  *             value = <object>PyDict_GetItem(self, item)
  *             if isinstance(value, Section) and not value:             # <<<<<<<<<<<<<<
  *                 value = self.__get_default_value(item)
  *         return self.type_conversation(item, value)
  */
     }
   }
   __pyx_L3:;
 
-  /* "configparserc/config.pyx":507
+  /* "configparserc/config.pyx":512
  *             if isinstance(value, Section) and not value:
  *                 value = self.__get_default_value(item)
  *         return self.type_conversation(item, value)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, key, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, __pyx_v_item, __pyx_v_value, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, __pyx_v_item, __pyx_v_value, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":497
+  /* "configparserc/config.pyx":502
  *         PyDict_SetItem(self, key, self.type_conversation(key, value))
  * 
  *     cdef object __get_item_value(self, str item):             # <<<<<<<<<<<<<<
  *         cdef:
  *             object value
  */
 
@@ -14870,15 +15290,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":509
+/* "configparserc/config.pyx":514
  *         return self.type_conversation(item, value)
  * 
  *     def __setitem__(self, key, value):             # <<<<<<<<<<<<<<
  *         self.__set_item_value(key, value)
  * 
  */
 
@@ -14900,29 +15320,29 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
-  __Pyx_TraceCall("__setitem__", __pyx_f[0], 509, 0, __PYX_ERR(0, 509, __pyx_L1_error));
+  __Pyx_TraceCall("__setitem__", __pyx_f[0], 514, 0, __PYX_ERR(0, 514, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":510
+  /* "configparserc/config.pyx":515
  * 
  *     def __setitem__(self, key, value):
  *         self.__set_item_value(key, value)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_key)->tp_name), 0))) __PYX_ERR(0, 510, __pyx_L1_error)
-  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___set_item_value(__pyx_v_self, ((PyObject*)__pyx_v_key), __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_key)->tp_name), 0))) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___set_item_value(__pyx_v_self, ((PyObject*)__pyx_v_key), __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":509
+  /* "configparserc/config.pyx":514
  *         return self.type_conversation(item, value)
  * 
  *     def __setitem__(self, key, value):             # <<<<<<<<<<<<<<
  *         self.__set_item_value(key, value)
  * 
  */
 
@@ -14935,15 +15355,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":512
+/* "configparserc/config.pyx":517
  *         self.__set_item_value(key, value)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.__get_item_value(item)
  * 
  */
 
@@ -14965,32 +15385,32 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
-  __Pyx_TraceCall("__getitem__", __pyx_f[0], 512, 0, __PYX_ERR(0, 512, __pyx_L1_error));
+  __Pyx_TraceCall("__getitem__", __pyx_f[0], 517, 0, __PYX_ERR(0, 517, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":513
+  /* "configparserc/config.pyx":518
  * 
  *     def __getitem__(self, item):
  *         return self.__get_item_value(item)             # <<<<<<<<<<<<<<
  * 
  *     cdef str _get_subsection_name(self, str key):
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_item))||((__pyx_v_item) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_item)->tp_name), 0))) __PYX_ERR(0, 513, __pyx_L1_error)
-  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_item_value(__pyx_v_self, ((PyObject*)__pyx_v_item)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 513, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_item))||((__pyx_v_item) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_item)->tp_name), 0))) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_item_value(__pyx_v_self, ((PyObject*)__pyx_v_item)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":512
+  /* "configparserc/config.pyx":517
  *         self.__set_item_value(key, value)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.__get_item_value(item)
  * 
  */
 
@@ -15002,15 +15422,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":515
+/* "configparserc/config.pyx":520
  *         return self.__get_item_value(item)
  * 
  *     cdef str _get_subsection_name(self, str key):             # <<<<<<<<<<<<<<
  *         return self.name + '.' + key
  * 
  */
 
@@ -15020,34 +15440,34 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_subsection_name", 0);
-  __Pyx_TraceCall("_get_subsection_name", __pyx_f[0], 515, 0, __PYX_ERR(0, 515, __pyx_L1_error));
+  __Pyx_TraceCall("_get_subsection_name", __pyx_f[0], 520, 0, __PYX_ERR(0, 520, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":516
+  /* "configparserc/config.pyx":521
  * 
  *     cdef str _get_subsection_name(self, str key):
  *         return self.name + '.' + key             # <<<<<<<<<<<<<<
  * 
  *     cdef dict __get_default_data(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_self->name, __pyx_kp_u_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_self->name, __pyx_kp_u_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_1, __pyx_v_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_t_1, __pyx_v_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":515
+  /* "configparserc/config.pyx":520
  *         return self.__get_item_value(item)
  * 
  *     cdef str _get_subsection_name(self, str key):             # <<<<<<<<<<<<<<
  *         return self.name + '.' + key
  * 
  */
 
@@ -15060,15 +15480,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":518
+/* "configparserc/config.pyx":523
  *         return self.name + '.' + key
  * 
  *     cdef dict __get_default_data(self):             # <<<<<<<<<<<<<<
  *         cdef:
  *             dict section_defaults
  */
 
@@ -15085,55 +15505,55 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_default_data", 0);
-  __Pyx_TraceCall("__get_default_data", __pyx_f[0], 518, 0, __PYX_ERR(0, 518, __pyx_L1_error));
+  __Pyx_TraceCall("__get_default_data", __pyx_f[0], 523, 0, __PYX_ERR(0, 523, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":521
+  /* "configparserc/config.pyx":526
  *         cdef:
  *             dict section_defaults
  *         section_defaults = self.config.section_defaults             # <<<<<<<<<<<<<<
  * 
  *         if section_defaults:
  */
   __pyx_t_1 = __pyx_v_self->config->section_defaults;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_section_defaults = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":523
+  /* "configparserc/config.pyx":528
  *         section_defaults = self.config.section_defaults
  * 
  *         if section_defaults:             # <<<<<<<<<<<<<<
  *             return reduce(__get_dict_from_dict_for_reduce, self.name.split('.'), section_defaults)
  *         return {}
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_section_defaults); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_section_defaults); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 528, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":524
+    /* "configparserc/config.pyx":529
  * 
  *         if section_defaults:
  *             return reduce(__get_dict_from_dict_for_reduce, self.name.split('.'), section_defaults)             # <<<<<<<<<<<<<<
  *         return {}
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_reduce); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 524, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_reduce); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_CFunc_dict____dict____unicode___to_py(__pyx_f_13configparserc_6config___get_dict_from_dict_for_reduce); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 524, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_CFunc_dict____dict____unicode___to_py(__pyx_f_13configparserc_6config___get_dict_from_dict_for_reduce); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (unlikely(__pyx_v_self->name == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "split");
-      __PYX_ERR(0, 524, __pyx_L1_error)
+      __PYX_ERR(0, 529, __pyx_L1_error)
     }
-    __pyx_t_5 = PyUnicode_Split(__pyx_v_self->name, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 524, __pyx_L1_error)
+    __pyx_t_5 = PyUnicode_Split(__pyx_v_self->name, __pyx_kp_u_, -1L); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 529, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -15142,80 +15562,80 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_4, __pyx_t_5, __pyx_v_section_defaults};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 529, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_4, __pyx_t_5, __pyx_v_section_defaults};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 529, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 529, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_6) {
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
       __Pyx_INCREF(__pyx_v_section_defaults);
       __Pyx_GIVEREF(__pyx_v_section_defaults);
       PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_v_section_defaults);
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 529, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 524, __pyx_L1_error)
+    if (!(likely(PyDict_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 529, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":523
+    /* "configparserc/config.pyx":528
  *         section_defaults = self.config.section_defaults
  * 
  *         if section_defaults:             # <<<<<<<<<<<<<<
  *             return reduce(__get_dict_from_dict_for_reduce, self.name.split('.'), section_defaults)
  *         return {}
  */
   }
 
-  /* "configparserc/config.pyx":525
+  /* "configparserc/config.pyx":530
  *         if section_defaults:
  *             return reduce(__get_dict_from_dict_for_reduce, self.name.split('.'), section_defaults)
  *         return {}             # <<<<<<<<<<<<<<
  * 
  *     cdef object __get_default_value(self, str item):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":518
+  /* "configparserc/config.pyx":523
  *         return self.name + '.' + key
  * 
  *     cdef dict __get_default_data(self):             # <<<<<<<<<<<<<<
  *         cdef:
  *             dict section_defaults
  */
 
@@ -15233,15 +15653,15 @@
   __Pyx_XDECREF(__pyx_v_section_defaults);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":527
+/* "configparserc/config.pyx":532
  *         return {}
  * 
  *     cdef object __get_default_value(self, str item):             # <<<<<<<<<<<<<<
  *         cdef:
  *             dict section_defaults
  */
 
@@ -15262,91 +15682,91 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_default_value", 0);
-  __Pyx_TraceCall("__get_default_value", __pyx_f[0], 527, 0, __PYX_ERR(0, 527, __pyx_L1_error));
+  __Pyx_TraceCall("__get_default_value", __pyx_f[0], 532, 0, __PYX_ERR(0, 532, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":532
+  /* "configparserc/config.pyx":537
  *             object value
  * 
  *         section_defaults = self.__get_default_data()             # <<<<<<<<<<<<<<
  * 
  *         if section_defaults and item in section_defaults:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_data(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_data(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_section_defaults = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":534
+  /* "configparserc/config.pyx":539
  *         section_defaults = self.__get_default_data()
  * 
  *         if section_defaults and item in section_defaults:             # <<<<<<<<<<<<<<
  *             value = <object>PyDict_GetItem(section_defaults, item)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_section_defaults); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_section_defaults); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 539, __pyx_L1_error)
   if (__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
   if (unlikely(__pyx_v_section_defaults == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 534, __pyx_L1_error)
+    __PYX_ERR(0, 539, __pyx_L1_error)
   }
-  __pyx_t_3 = (__Pyx_PyDict_ContainsTF(__pyx_v_item, __pyx_v_section_defaults, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyDict_ContainsTF(__pyx_v_item, __pyx_v_section_defaults, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 539, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   __pyx_t_2 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":535
+    /* "configparserc/config.pyx":540
  * 
  *         if section_defaults and item in section_defaults:
  *             value = <object>PyDict_GetItem(section_defaults, item)             # <<<<<<<<<<<<<<
  * 
  *             if isinstance(value, dict):
  */
     __pyx_t_5 = PyDict_GetItem(__pyx_v_section_defaults, __pyx_v_item);
     __pyx_t_1 = ((PyObject *)__pyx_t_5);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_value = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":537
+    /* "configparserc/config.pyx":542
  *             value = <object>PyDict_GetItem(section_defaults, item)
  * 
  *             if isinstance(value, dict):             # <<<<<<<<<<<<<<
  *                 value = self.config.get_section_instance(self._get_subsection_name(item), section_defaults[item])
  * 
  */
     __pyx_t_2 = PyDict_Check(__pyx_v_value); 
     __pyx_t_4 = (__pyx_t_2 != 0);
     if (__pyx_t_4) {
 
-      /* "configparserc/config.pyx":538
+      /* "configparserc/config.pyx":543
  * 
  *             if isinstance(value, dict):
  *                 value = self.config.get_section_instance(self._get_subsection_name(item), section_defaults[item])             # <<<<<<<<<<<<<<
  * 
  *             return value
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 538, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_get_section_instance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 543, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->_get_subsection_name(__pyx_v_self, __pyx_v_item); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 538, __pyx_L1_error)
+      __pyx_t_7 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->_get_subsection_name(__pyx_v_self, __pyx_v_item); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 543, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (unlikely(__pyx_v_section_defaults == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 538, __pyx_L1_error)
+        __PYX_ERR(0, 543, __pyx_L1_error)
       }
-      __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_section_defaults, __pyx_v_item); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 538, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_section_defaults, __pyx_v_item); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 543, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_9 = NULL;
       __pyx_t_10 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -15355,123 +15775,123 @@
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_10 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_7, __pyx_t_8};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_7, __pyx_t_8};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       } else
       #endif
       {
-        __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 538, __pyx_L1_error)
+        __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 543, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         if (__pyx_t_9) {
           __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_9); __pyx_t_9 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_t_8);
         __pyx_t_7 = 0;
         __pyx_t_8 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "configparserc/config.pyx":537
+      /* "configparserc/config.pyx":542
  *             value = <object>PyDict_GetItem(section_defaults, item)
  * 
  *             if isinstance(value, dict):             # <<<<<<<<<<<<<<
  *                 value = self.config.get_section_instance(self._get_subsection_name(item), section_defaults[item])
  * 
  */
     }
 
-    /* "configparserc/config.pyx":540
+    /* "configparserc/config.pyx":545
  *                 value = self.config.get_section_instance(self._get_subsection_name(item), section_defaults[item])
  * 
  *             return value             # <<<<<<<<<<<<<<
  *         return super(Section, self).__getitem__(item)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_value);
     __pyx_r = __pyx_v_value;
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":534
+    /* "configparserc/config.pyx":539
  *         section_defaults = self.__get_default_data()
  * 
  *         if section_defaults and item in section_defaults:             # <<<<<<<<<<<<<<
  *             value = <object>PyDict_GetItem(section_defaults, item)
  * 
  */
   }
 
-  /* "configparserc/config.pyx":541
+  /* "configparserc/config.pyx":546
  * 
  *             return value
  *         return super(Section, self).__getitem__(item)             # <<<<<<<<<<<<<<
  * 
  *     def update(self, other = None, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_6, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_6, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_getitem); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_getitem); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_11, __pyx_v_item) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_item);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 541, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":527
+  /* "configparserc/config.pyx":532
  *         return {}
  * 
  *     cdef object __get_default_value(self, str item):             # <<<<<<<<<<<<<<
  *         cdef:
  *             dict section_defaults
  */
 
@@ -15490,15 +15910,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":543
+/* "configparserc/config.pyx":548
  *         return super(Section, self).__getitem__(item)
  * 
  *     def update(self, other = None, **kwargs):             # <<<<<<<<<<<<<<
  *         if other and isinstance(other, dict):
  *             for k, v in other.items():
  */
 
@@ -15533,29 +15953,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_other);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "update") < 0)) __PYX_ERR(0, 543, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "update") < 0)) __PYX_ERR(0, 548, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_other = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("update", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 543, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("update", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 548, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("configparserc.config.Section.update", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_8update(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_other, __pyx_v_kwargs);
@@ -15582,129 +16002,129 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update", 0);
-  __Pyx_TraceCall("update", __pyx_f[0], 543, 0, __PYX_ERR(0, 543, __pyx_L1_error));
+  __Pyx_TraceCall("update", __pyx_f[0], 548, 0, __PYX_ERR(0, 548, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":544
+  /* "configparserc/config.pyx":549
  * 
  *     def update(self, other = None, **kwargs):
  *         if other and isinstance(other, dict):             # <<<<<<<<<<<<<<
  *             for k, v in other.items():
  *                 self[k] = v
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_other); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_other); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 549, __pyx_L1_error)
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = PyDict_Check(__pyx_v_other); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":545
+    /* "configparserc/config.pyx":550
  *     def update(self, other = None, **kwargs):
  *         if other and isinstance(other, dict):
  *             for k, v in other.items():             # <<<<<<<<<<<<<<
  *                 self[k] = v
  *         if kwargs:
  */
     __pyx_t_5 = 0;
     if (unlikely(__pyx_v_other == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 545, __pyx_L1_error)
+      __PYX_ERR(0, 550, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_other, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 545, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_other, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 550, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_4);
     __pyx_t_4 = __pyx_t_8;
     __pyx_t_8 = 0;
     while (1) {
       __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_6, &__pyx_t_5, &__pyx_t_8, &__pyx_t_9, NULL, __pyx_t_7);
       if (unlikely(__pyx_t_10 == 0)) break;
-      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 545, __pyx_L1_error)
+      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 550, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "configparserc/config.pyx":546
+      /* "configparserc/config.pyx":551
  *         if other and isinstance(other, dict):
  *             for k, v in other.items():
  *                 self[k] = v             # <<<<<<<<<<<<<<
  *         if kwargs:
  *             self.update(kwargs)
  */
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v) < 0)) __PYX_ERR(0, 546, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v) < 0)) __PYX_ERR(0, 551, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":544
+    /* "configparserc/config.pyx":549
  * 
  *     def update(self, other = None, **kwargs):
  *         if other and isinstance(other, dict):             # <<<<<<<<<<<<<<
  *             for k, v in other.items():
  *                 self[k] = v
  */
   }
 
-  /* "configparserc/config.pyx":547
+  /* "configparserc/config.pyx":552
  *             for k, v in other.items():
  *                 self[k] = v
  *         if kwargs:             # <<<<<<<<<<<<<<
  *             self.update(kwargs)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 552, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "configparserc/config.pyx":548
+    /* "configparserc/config.pyx":553
  *                 self[k] = v
  *         if kwargs:
  *             self.update(kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def get_default_data(self):
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_update); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 548, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_update); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 553, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_v_kwargs) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_kwargs);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 548, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":547
+    /* "configparserc/config.pyx":552
  *             for k, v in other.items():
  *                 self[k] = v
  *         if kwargs:             # <<<<<<<<<<<<<<
  *             self.update(kwargs)
  * 
  */
   }
 
-  /* "configparserc/config.pyx":543
+  /* "configparserc/config.pyx":548
  *         return super(Section, self).__getitem__(item)
  * 
  *     def update(self, other = None, **kwargs):             # <<<<<<<<<<<<<<
  *         if other and isinstance(other, dict):
  *             for k, v in other.items():
  */
 
@@ -15722,15 +16142,15 @@
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":550
+/* "configparserc/config.pyx":555
  *             self.update(kwargs)
  * 
  *     def get_default_data(self):             # <<<<<<<<<<<<<<
  *         return self.__get_default_data()
  * 
  */
 
@@ -15752,31 +16172,31 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_default_data", 0);
-  __Pyx_TraceCall("get_default_data", __pyx_f[0], 550, 0, __PYX_ERR(0, 550, __pyx_L1_error));
+  __Pyx_TraceCall("get_default_data", __pyx_f[0], 555, 0, __PYX_ERR(0, 555, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":551
+  /* "configparserc/config.pyx":556
  * 
  *     def get_default_data(self):
  *         return self.__get_default_data()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_data(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->__pyx___get_default_data(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":550
+  /* "configparserc/config.pyx":555
  *             self.update(kwargs)
  * 
  *     def get_default_data(self):             # <<<<<<<<<<<<<<
  *         return self.__get_default_data()
  * 
  */
 
@@ -15788,15 +16208,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":554
+/* "configparserc/config.pyx":559
  * 
  *     @property
  *     def subsections(self):             # <<<<<<<<<<<<<<
  *         return filter(__is_section, self.values())
  * 
  */
 
@@ -15821,59 +16241,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 554, 0, __PYX_ERR(0, 554, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[0], 559, 0, __PYX_ERR(0, 559, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":555
+  /* "configparserc/config.pyx":560
  *     @property
  *     def subsections(self):
  *         return filter(__is_section, self.values())             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_CFunc_bint____object___to_py(__pyx_f_13configparserc_6config___is_section); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CFunc_bint____object___to_py(__pyx_f_13configparserc_6config___is_section); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":554
+  /* "configparserc/config.pyx":559
  * 
  *     @property
  *     def subsections(self):             # <<<<<<<<<<<<<<
  *         return filter(__is_section, self.values())
  * 
  */
 
@@ -15888,15 +16308,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":558
+/* "configparserc/config.pyx":563
  * 
  *     @property
  *     def subsections_names(self):             # <<<<<<<<<<<<<<
  *         return map(__get_section_subname, self.subsections)
  * 
  */
 
@@ -15920,44 +16340,44 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 558, 0, __PYX_ERR(0, 558, __pyx_L1_error));
+  __Pyx_TraceCall("__get__", __pyx_f[0], 563, 0, __PYX_ERR(0, 563, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":559
+  /* "configparserc/config.pyx":564
  *     @property
  *     def subsections_names(self):
  *         return map(__get_section_subname, self.subsections)             # <<<<<<<<<<<<<<
  * 
  *     def get_name(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_CFunc_unicode____Section___to_py(__pyx_f_13configparserc_6config___get_section_subname); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CFunc_unicode____Section___to_py(__pyx_f_13configparserc_6config___get_section_subname); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_subsections); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_subsections); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":558
+  /* "configparserc/config.pyx":563
  * 
  *     @property
  *     def subsections_names(self):             # <<<<<<<<<<<<<<
  *         return map(__get_section_subname, self.subsections)
  * 
  */
 
@@ -15971,15 +16391,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":561
+/* "configparserc/config.pyx":566
  *         return map(__get_section_subname, self.subsections)
  * 
  *     def get_name(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -16000,29 +16420,29 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_name", 0);
-  __Pyx_TraceCall("get_name", __pyx_f[0], 561, 0, __PYX_ERR(0, 561, __pyx_L1_error));
+  __Pyx_TraceCall("get_name", __pyx_f[0], 566, 0, __PYX_ERR(0, 566, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":562
+  /* "configparserc/config.pyx":567
  * 
  *     def get_name(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":561
+  /* "configparserc/config.pyx":566
  *         return map(__get_section_subname, self.subsections)
  * 
  *     def get_name(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -16033,15 +16453,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":564
+/* "configparserc/config.pyx":569
  *         return self.name
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         return self.__class__(self.name, self.config, default=super().copy())
  * 
  */
 
@@ -16068,77 +16488,77 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
-  __Pyx_TraceCall("copy", __pyx_f[0], 564, 0, __PYX_ERR(0, 564, __pyx_L1_error));
+  __Pyx_TraceCall("copy", __pyx_f[0], 569, 0, __PYX_ERR(0, 569, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":565
+  /* "configparserc/config.pyx":570
  * 
  *     def copy(self):
  *         return self.__class__(self.name, self.config, default=super().copy())             # <<<<<<<<<<<<<<
  * 
  *     def get(self, key, fallback = Empty()):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->name);
   __Pyx_GIVEREF(__pyx_v_self->name);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->name);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->config));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self->config));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_self->config));
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_Section));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_copy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 565, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_default, __pyx_t_4) < 0) __PYX_ERR(0, 565, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_default, __pyx_t_4) < 0) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":564
+  /* "configparserc/config.pyx":569
  *         return self.name
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         return self.__class__(self.name, self.config, default=super().copy())
  * 
  */
 
@@ -16155,15 +16575,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":567
+/* "configparserc/config.pyx":572
  *         return self.__class__(self.name, self.config, default=super().copy())
  * 
  *     def get(self, key, fallback = Empty()):             # <<<<<<<<<<<<<<
  *         try:
  *             return self[key]
  */
 
@@ -16202,15 +16622,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fallback);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get") < 0)) __PYX_ERR(0, 567, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get") < 0)) __PYX_ERR(0, 572, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -16218,15 +16638,15 @@
       }
     }
     __pyx_v_key = values[0];
     __pyx_v_fallback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 567, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 572, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_16get(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_key, __pyx_v_fallback);
 
@@ -16251,17 +16671,17 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get", 0);
-  __Pyx_TraceCall("get", __pyx_f[0], 567, 0, __PYX_ERR(0, 567, __pyx_L1_error));
+  __Pyx_TraceCall("get", __pyx_f[0], 572, 0, __PYX_ERR(0, 572, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":568
+  /* "configparserc/config.pyx":573
  * 
  *     def get(self, key, fallback = Empty()):
  *         try:             # <<<<<<<<<<<<<<
  *             return self[key]
  *         except KeyError:
  */
   {
@@ -16269,124 +16689,124 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "configparserc/config.pyx":569
+      /* "configparserc/config.pyx":574
  *     def get(self, key, fallback = Empty()):
  *         try:
  *             return self[key]             # <<<<<<<<<<<<<<
  *         except KeyError:
  *             if not isinstance(fallback, Empty):
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 569, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 574, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L7_try_return;
 
-      /* "configparserc/config.pyx":568
+      /* "configparserc/config.pyx":573
  * 
  *     def get(self, key, fallback = Empty()):
  *         try:             # <<<<<<<<<<<<<<
  *             return self[key]
  *         except KeyError:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":570
+    /* "configparserc/config.pyx":575
  *         try:
  *             return self[key]
  *         except KeyError:             # <<<<<<<<<<<<<<
  *             if not isinstance(fallback, Empty):
  *                 return self.config.format_string(fallback)
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_5) {
       __Pyx_AddTraceback("configparserc.config.Section.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 570, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 575, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "configparserc/config.pyx":571
+      /* "configparserc/config.pyx":576
  *             return self[key]
  *         except KeyError:
  *             if not isinstance(fallback, Empty):             # <<<<<<<<<<<<<<
  *                 return self.config.format_string(fallback)
  *             raise
  */
       __pyx_t_8 = __Pyx_TypeCheck(__pyx_v_fallback, __pyx_ptype_13configparserc_6config_Empty); 
       __pyx_t_9 = ((!(__pyx_t_8 != 0)) != 0);
       if (__pyx_t_9) {
 
-        /* "configparserc/config.pyx":572
+        /* "configparserc/config.pyx":577
  *         except KeyError:
  *             if not isinstance(fallback, Empty):
  *                 return self.config.format_string(fallback)             # <<<<<<<<<<<<<<
  *             raise
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_format_string); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 572, __pyx_L5_except_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->config), __pyx_n_s_format_string); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 577, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_v_fallback) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_fallback);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 572, __pyx_L5_except_error)
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 577, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_r = __pyx_t_10;
         __pyx_t_10 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L6_except_return;
 
-        /* "configparserc/config.pyx":571
+        /* "configparserc/config.pyx":576
  *             return self[key]
  *         except KeyError:
  *             if not isinstance(fallback, Empty):             # <<<<<<<<<<<<<<
  *                 return self.config.format_string(fallback)
  *             raise
  */
       }
 
-      /* "configparserc/config.pyx":573
+      /* "configparserc/config.pyx":578
  *             if not isinstance(fallback, Empty):
  *                 return self.config.format_string(fallback)
  *             raise             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
       __Pyx_GIVEREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_6, __pyx_t_7);
       __pyx_t_4 = 0; __pyx_t_6 = 0; __pyx_t_7 = 0; 
-      __PYX_ERR(0, 573, __pyx_L5_except_error)
+      __PYX_ERR(0, 578, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "configparserc/config.pyx":568
+    /* "configparserc/config.pyx":573
  * 
  *     def get(self, key, fallback = Empty()):
  *         try:             # <<<<<<<<<<<<<<
  *             return self[key]
  *         except KeyError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -16404,15 +16824,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "configparserc/config.pyx":567
+  /* "configparserc/config.pyx":572
  *         return self.__class__(self.name, self.config, default=super().copy())
  * 
  *     def get(self, key, fallback = Empty()):             # <<<<<<<<<<<<<<
  *         try:
  *             return self[key]
  */
 
@@ -16429,15 +16849,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":575
+/* "configparserc/config.pyx":580
  *             raise
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         data = dict()
  *         for key in self:
  */
 
@@ -16469,165 +16889,165 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("all", 0);
-  __Pyx_TraceCall("all", __pyx_f[0], 575, 0, __PYX_ERR(0, 575, __pyx_L1_error));
+  __Pyx_TraceCall("all", __pyx_f[0], 580, 0, __PYX_ERR(0, 580, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":576
+  /* "configparserc/config.pyx":581
  * 
  *     def all(self):
  *         data = dict()             # <<<<<<<<<<<<<<
  *         for key in self:
  *             value = self[key]
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":577
+  /* "configparserc/config.pyx":582
  *     def all(self):
  *         data = dict()
  *         for key in self:             # <<<<<<<<<<<<<<
  *             value = self[key]
  *             data[self.key_handler_to_all(key)] = value.all() if isinstance(value, Section) else value
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
     __pyx_t_1 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 577, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 582, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 577, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 582, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 577, __pyx_L1_error)
+          else __PYX_ERR(0, 582, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":578
+    /* "configparserc/config.pyx":583
  *         data = dict()
  *         for key in self:
  *             value = self[key]             # <<<<<<<<<<<<<<
  *             data[self.key_handler_to_all(key)] = value.all() if isinstance(value, Section) else value
  *         return data
  */
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 578, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":579
+    /* "configparserc/config.pyx":584
  *         for key in self:
  *             value = self[key]
  *             data[self.key_handler_to_all(key)] = value.all() if isinstance(value, Section) else value             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
     __pyx_t_5 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_13configparserc_6config_Section); 
     if ((__pyx_t_5 != 0)) {
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_all); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 579, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_all); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 584, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 579, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 584, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_4 = __pyx_t_6;
       __pyx_t_6 = 0;
     } else {
       __Pyx_INCREF(__pyx_v_value);
       __pyx_t_4 = __pyx_v_value;
     }
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_key_handler_to_all); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_key_handler_to_all); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_key);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 579, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_data, __pyx_t_6, __pyx_t_4) < 0)) __PYX_ERR(0, 579, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_data, __pyx_t_6, __pyx_t_4) < 0)) __PYX_ERR(0, 584, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "configparserc/config.pyx":577
+    /* "configparserc/config.pyx":582
  *     def all(self):
  *         data = dict()
  *         for key in self:             # <<<<<<<<<<<<<<
  *             value = self[key]
  *             data[self.key_handler_to_all(key)] = value.all() if isinstance(value, Section) else value
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":580
+  /* "configparserc/config.pyx":585
  *             value = self[key]
  *             data[self.key_handler_to_all(key)] = value.all() if isinstance(value, Section) else value
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def key_handler_to_all(self, key):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":575
+  /* "configparserc/config.pyx":580
  *             raise
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         data = dict()
  *         for key in self:
  */
 
@@ -16646,15 +17066,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":582
+/* "configparserc/config.pyx":587
  *         return data
  * 
  *     def key_handler_to_all(self, key):             # <<<<<<<<<<<<<<
  *         return key
  * 
  */
 
@@ -16675,29 +17095,29 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("key_handler_to_all", 0);
-  __Pyx_TraceCall("key_handler_to_all", __pyx_f[0], 582, 0, __PYX_ERR(0, 582, __pyx_L1_error));
+  __Pyx_TraceCall("key_handler_to_all", __pyx_f[0], 587, 0, __PYX_ERR(0, 587, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":583
+  /* "configparserc/config.pyx":588
  * 
  *     def key_handler_to_all(self, key):
  *         return key             # <<<<<<<<<<<<<<
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_key);
   __pyx_r = __pyx_v_key;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":582
+  /* "configparserc/config.pyx":587
  *         return data
  * 
  *     def key_handler_to_all(self, key):             # <<<<<<<<<<<<<<
  *         return key
  * 
  */
 
@@ -16708,15 +17128,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":585
+/* "configparserc/config.pyx":590
  *         return key
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):             # <<<<<<<<<<<<<<
  *         if PyDict_Contains(self.__type_map, key) == 1:
  *             return <object>PyDict_GetItem(self.__type_map, key)
  */
 
@@ -16730,36 +17150,36 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_type_conversation_instance", 0);
-  __Pyx_TraceCall("get_type_conversation_instance", __pyx_f[0], 585, 0, __PYX_ERR(0, 585, __pyx_L1_error));
+  __Pyx_TraceCall("get_type_conversation_instance", __pyx_f[0], 590, 0, __PYX_ERR(0, 590, __pyx_L1_error));
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default = __pyx_optional_args->__pyx_default;
     }
   }
 
-  /* "configparserc/config.pyx":586
+  /* "configparserc/config.pyx":591
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):
  *         if PyDict_Contains(self.__type_map, key) == 1:             # <<<<<<<<<<<<<<
  *             return <object>PyDict_GetItem(self.__type_map, key)
  *         return getattr(self, 'type_'+key, default)
  */
   __pyx_t_1 = __pyx_v_self->__pyx___type_map;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyDict_Contains(__pyx_t_1, __pyx_v_key); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Contains(__pyx_t_1, __pyx_v_key); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = ((__pyx_t_2 == 1) != 0);
   if (__pyx_t_3) {
 
-    /* "configparserc/config.pyx":587
+    /* "configparserc/config.pyx":592
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):
  *         if PyDict_Contains(self.__type_map, key) == 1:
  *             return <object>PyDict_GetItem(self.__type_map, key)             # <<<<<<<<<<<<<<
  *         return getattr(self, 'type_'+key, default)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
@@ -16767,41 +17187,41 @@
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_4 = PyDict_GetItem(__pyx_t_1, __pyx_v_key);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(((PyObject *)__pyx_t_4));
     __pyx_r = ((PyObject *)__pyx_t_4);
     goto __pyx_L0;
 
-    /* "configparserc/config.pyx":586
+    /* "configparserc/config.pyx":591
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):
  *         if PyDict_Contains(self.__type_map, key) == 1:             # <<<<<<<<<<<<<<
  *             return <object>PyDict_GetItem(self.__type_map, key)
  *         return getattr(self, 'type_'+key, default)
  */
   }
 
-  /* "configparserc/config.pyx":588
+  /* "configparserc/config.pyx":593
  *         if PyDict_Contains(self.__type_map, key) == 1:
  *             return <object>PyDict_GetItem(self.__type_map, key)
  *         return getattr(self, 'type_'+key, default)             # <<<<<<<<<<<<<<
  * 
  *     cdef object type_conversation(self, str key, object value, BaseType conv_class=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_n_u_type, __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_ConcatSafe(__pyx_n_u_type, __pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_t_1, __pyx_v_default); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_t_1, __pyx_v_default); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":585
+  /* "configparserc/config.pyx":590
  *         return key
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):             # <<<<<<<<<<<<<<
  *         if PyDict_Contains(self.__type_map, key) == 1:
  *             return <object>PyDict_GetItem(self.__type_map, key)
  */
 
@@ -16814,15 +17234,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":590
+/* "configparserc/config.pyx":595
  *         return getattr(self, 'type_'+key, default)
  * 
  *     cdef object type_conversation(self, str key, object value, BaseType conv_class=None):             # <<<<<<<<<<<<<<
  *         cdef BaseType conversation_cls
  * 
  */
 
@@ -16838,69 +17258,69 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("type_conversation", 0);
-  __Pyx_TraceCall("type_conversation", __pyx_f[0], 590, 0, __PYX_ERR(0, 590, __pyx_L1_error));
+  __Pyx_TraceCall("type_conversation", __pyx_f[0], 595, 0, __PYX_ERR(0, 595, __pyx_L1_error));
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_conv_class = __pyx_optional_args->conv_class;
     }
   }
 
-  /* "configparserc/config.pyx":593
+  /* "configparserc/config.pyx":598
  *         cdef BaseType conversation_cls
  * 
  *         if conv_class is not None:             # <<<<<<<<<<<<<<
  *             conversation_cls = conv_class
  *         else:
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_conv_class) != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "configparserc/config.pyx":594
+    /* "configparserc/config.pyx":599
  * 
  *         if conv_class is not None:
  *             conversation_cls = conv_class             # <<<<<<<<<<<<<<
  *         else:
  *            conversation_cls = self.get_type_conversation_instance(key)
  */
     __Pyx_INCREF(((PyObject *)__pyx_v_conv_class));
     __pyx_v_conversation_cls = __pyx_v_conv_class;
 
-    /* "configparserc/config.pyx":593
+    /* "configparserc/config.pyx":598
  *         cdef BaseType conversation_cls
  * 
  *         if conv_class is not None:             # <<<<<<<<<<<<<<
  *             conversation_cls = conv_class
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "configparserc/config.pyx":596
+  /* "configparserc/config.pyx":601
  *             conversation_cls = conv_class
  *         else:
  *            conversation_cls = self.get_type_conversation_instance(key)             # <<<<<<<<<<<<<<
  *         return conversation_cls(value) if conversation_cls is not None else value
  * 
  */
   /*else*/ {
-    __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->get_type_conversation_instance(__pyx_v_self, __pyx_v_key, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->get_type_conversation_instance(__pyx_v_self, __pyx_v_key, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_13configparserc_6config_BaseType))))) __PYX_ERR(0, 596, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_13configparserc_6config_BaseType))))) __PYX_ERR(0, 601, __pyx_L1_error)
     __pyx_v_conversation_cls = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_3);
     __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "configparserc/config.pyx":597
+  /* "configparserc/config.pyx":602
  *         else:
  *            conversation_cls = self.get_type_conversation_instance(key)
  *         return conversation_cls(value) if conversation_cls is not None else value             # <<<<<<<<<<<<<<
  * 
  *     def generate_section_string(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -16915,28 +17335,28 @@
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 597, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_value);
     __pyx_t_3 = __pyx_v_value;
   }
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":590
+  /* "configparserc/config.pyx":595
  *         return getattr(self, 'type_'+key, default)
  * 
  *     cdef object type_conversation(self, str key, object value, BaseType conv_class=None):             # <<<<<<<<<<<<<<
  *         cdef BaseType conversation_cls
  * 
  */
 
@@ -16952,15 +17372,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_conversation_cls);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":599
+/* "configparserc/config.pyx":604
  *         return conversation_cls(value) if conversation_cls is not None else value
  * 
  *     def generate_section_string(self):             # <<<<<<<<<<<<<<
  *         section_str = '[' + self.get_name() + ']\n'
  *         subs_names = list(self.subsections_names)
  */
 
@@ -16995,231 +17415,231 @@
   int __pyx_t_8;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_section_string", 0);
-  __Pyx_TraceCall("generate_section_string", __pyx_f[0], 599, 0, __PYX_ERR(0, 599, __pyx_L1_error));
+  __Pyx_TraceCall("generate_section_string", __pyx_f[0], 604, 0, __PYX_ERR(0, 604, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":600
+  /* "configparserc/config.pyx":605
  * 
  *     def generate_section_string(self):
  *         section_str = '[' + self.get_name() + ']\n'             # <<<<<<<<<<<<<<
  *         subs_names = list(self.subsections_names)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_kp_u__10, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_kp_u__10, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_section_str = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":601
+  /* "configparserc/config.pyx":606
  *     def generate_section_string(self):
  *         section_str = '[' + self.get_name() + ']\n'
  *         subs_names = list(self.subsections_names)             # <<<<<<<<<<<<<<
  * 
  *         for key in self.keys():
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_subsections_names); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_subsections_names); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_subs_names = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "configparserc/config.pyx":603
+  /* "configparserc/config.pyx":608
  *         subs_names = list(self.subsections_names)
  * 
  *         for key in self.keys():             # <<<<<<<<<<<<<<
  *             if key not in subs_names:
  *                 section_str += self.to_str(key) + '\n'
  */
   __pyx_t_4 = 0;
   if (unlikely(((PyObject *)__pyx_v_self) == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-    __PYX_ERR(0, 603, __pyx_L1_error)
+    __PYX_ERR(0, 608, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(((PyObject *)__pyx_v_self), 0, __pyx_n_s_keys, (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(((PyObject *)__pyx_v_self), 0, __pyx_n_s_keys, (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __pyx_t_2 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_5, &__pyx_t_4, &__pyx_t_1, NULL, NULL, __pyx_t_6);
     if (unlikely(__pyx_t_7 == 0)) break;
-    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 603, __pyx_L1_error)
+    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 608, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":604
+    /* "configparserc/config.pyx":609
  * 
  *         for key in self.keys():
  *             if key not in subs_names:             # <<<<<<<<<<<<<<
  *                 section_str += self.to_str(key) + '\n'
  * 
  */
-    __pyx_t_8 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, __pyx_v_subs_names, Py_NE)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 604, __pyx_L1_error)
+    __pyx_t_8 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, __pyx_v_subs_names, Py_NE)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 609, __pyx_L1_error)
     __pyx_t_9 = (__pyx_t_8 != 0);
     if (__pyx_t_9) {
 
-      /* "configparserc/config.pyx":605
+      /* "configparserc/config.pyx":610
  *         for key in self.keys():
  *             if key not in subs_names:
  *                 section_str += self.to_str(key) + '\n'             # <<<<<<<<<<<<<<
  * 
  *         section_str += '\n'
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_to_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_to_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_10, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_key);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__21); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_kp_u__21); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_section_str, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_section_str, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_section_str, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "configparserc/config.pyx":604
+      /* "configparserc/config.pyx":609
  * 
  *         for key in self.keys():
  *             if key not in subs_names:             # <<<<<<<<<<<<<<
  *                 section_str += self.to_str(key) + '\n'
  * 
  */
     }
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "configparserc/config.pyx":607
+  /* "configparserc/config.pyx":612
  *                 section_str += self.to_str(key) + '\n'
  * 
  *         section_str += '\n'             # <<<<<<<<<<<<<<
  *         for sub_name in subs_names:
  *             section_str += self[sub_name].generate_section_string()
  */
-  __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_section_str, __pyx_kp_u__21); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_section_str, __pyx_kp_u__21); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF_SET(__pyx_v_section_str, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "configparserc/config.pyx":608
+  /* "configparserc/config.pyx":613
  * 
  *         section_str += '\n'
  *         for sub_name in subs_names:             # <<<<<<<<<<<<<<
  *             section_str += self[sub_name].generate_section_string()
  * 
  */
   __pyx_t_2 = __pyx_v_subs_names; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
   for (;;) {
     if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 608, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 613, __pyx_L1_error)
     #else
-    __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_sub_name, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "configparserc/config.pyx":609
+    /* "configparserc/config.pyx":614
  *         section_str += '\n'
  *         for sub_name in subs_names:
  *             section_str += self[sub_name].generate_section_string()             # <<<<<<<<<<<<<<
  * 
  *         return section_str
  */
-    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_sub_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 609, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_sub_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_generate_section_string); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 609, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_generate_section_string); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_v_section_str, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 609, __pyx_L1_error)
+    __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_v_section_str, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_section_str, __pyx_t_10);
     __pyx_t_10 = 0;
 
-    /* "configparserc/config.pyx":608
+    /* "configparserc/config.pyx":613
  * 
  *         section_str += '\n'
  *         for sub_name in subs_names:             # <<<<<<<<<<<<<<
  *             section_str += self[sub_name].generate_section_string()
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "configparserc/config.pyx":611
+  /* "configparserc/config.pyx":616
  *             section_str += self[sub_name].generate_section_string()
  * 
  *         return section_str             # <<<<<<<<<<<<<<
  * 
  *     def to_str(self, key):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_section_str);
   __pyx_r = __pyx_v_section_str;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":599
+  /* "configparserc/config.pyx":604
  *         return conversation_cls(value) if conversation_cls is not None else value
  * 
  *     def generate_section_string(self):             # <<<<<<<<<<<<<<
  *         section_str = '[' + self.get_name() + ']\n'
  *         subs_names = list(self.subsections_names)
  */
 
@@ -17238,15 +17658,15 @@
   __Pyx_XDECREF(__pyx_v_sub_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":613
+/* "configparserc/config.pyx":618
  *         return section_str
  * 
  *     def to_str(self, key):             # <<<<<<<<<<<<<<
  *         conversation_class = self.get_type_conversation_instance(key)
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\
  */
 
@@ -17275,126 +17695,126 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("to_str", 0);
-  __Pyx_TraceCall("to_str", __pyx_f[0], 613, 0, __PYX_ERR(0, 613, __pyx_L1_error));
+  __Pyx_TraceCall("to_str", __pyx_f[0], 618, 0, __PYX_ERR(0, 618, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":614
+  /* "configparserc/config.pyx":619
  * 
  *     def to_str(self, key):
  *         conversation_class = self.get_type_conversation_instance(key)             # <<<<<<<<<<<<<<
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\
  *             .replace('{', '{{')\
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_key)->tp_name), 0))) __PYX_ERR(0, 614, __pyx_L1_error)
-  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->get_type_conversation_instance(__pyx_v_self, ((PyObject*)__pyx_v_key), NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_key)->tp_name), 0))) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->get_type_conversation_instance(__pyx_v_self, ((PyObject*)__pyx_v_key), NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_conversation_class = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":615
+  /* "configparserc/config.pyx":620
  *     def to_str(self, key):
  *         conversation_class = self.get_type_conversation_instance(key)
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\             # <<<<<<<<<<<<<<
  *             .replace('{', '{{')\
  *             .replace('}', '}}')
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "configparserc/config.pyx":616
+  /* "configparserc/config.pyx":621
  *         conversation_class = self.get_type_conversation_instance(key)
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\
  *             .replace('{', '{{')\             # <<<<<<<<<<<<<<
  *             .replace('}', '}}')
  * 
  */
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
 
-  /* "configparserc/config.pyx":615
+  /* "configparserc/config.pyx":620
  *     def to_str(self, key):
  *         conversation_class = self.get_type_conversation_instance(key)
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\             # <<<<<<<<<<<<<<
  *             .replace('{', '{{')\
  *             .replace('}', '}}')
  */
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_key, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_key, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__22);
   __pyx_t_2 += 3;
   __Pyx_GIVEREF(__pyx_kp_u__22);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u__22);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_conversation_class, __pyx_n_s_str_convert); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_conversation_class, __pyx_n_s_str_convert); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":616
+  /* "configparserc/config.pyx":621
  *         conversation_class = self.get_type_conversation_instance(key)
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\
  *             .replace('{', '{{')\             # <<<<<<<<<<<<<<
  *             .replace('}', '}}')
  * 
  */
-  __pyx_t_1 = PyUnicode_Replace(((PyObject*)__pyx_t_5), __pyx_kp_u__8, __pyx_kp_u__23, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Replace(((PyObject*)__pyx_t_5), __pyx_kp_u__8, __pyx_kp_u__23, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "configparserc/config.pyx":617
+  /* "configparserc/config.pyx":622
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\
  *             .replace('{', '{{')\
  *             .replace('}', '}}')             # <<<<<<<<<<<<<<
  * 
  *     def getboolean(self, option, fallback=None):
  */
-  __pyx_t_5 = PyUnicode_Replace(((PyObject*)__pyx_t_1), __pyx_kp_u__9, __pyx_kp_u__24, -1L); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 617, __pyx_L1_error)
+  __pyx_t_5 = PyUnicode_Replace(((PyObject*)__pyx_t_1), __pyx_kp_u__9, __pyx_kp_u__24, -1L); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 622, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":613
+  /* "configparserc/config.pyx":618
  *         return section_str
  * 
  *     def to_str(self, key):             # <<<<<<<<<<<<<<
  *         conversation_class = self.get_type_conversation_instance(key)
  *         return f'{key} = {conversation_class.str_convert(self[key])}'\
  */
 
@@ -17411,15 +17831,15 @@
   __Pyx_XDECREF(__pyx_v_conversation_class);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":619
+/* "configparserc/config.pyx":624
  *             .replace('}', '}}')
  * 
  *     def getboolean(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, fallback), BoolType())
  * 
  */
 
@@ -17458,15 +17878,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fallback);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getboolean") < 0)) __PYX_ERR(0, 619, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getboolean") < 0)) __PYX_ERR(0, 624, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -17474,15 +17894,15 @@
       }
     }
     __pyx_v_option = values[0];
     __pyx_v_fallback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getboolean", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 619, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getboolean", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 624, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.getboolean", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_26getboolean(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_option, __pyx_v_fallback);
 
@@ -17501,25 +17921,25 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getboolean", 0);
-  __Pyx_TraceCall("getboolean", __pyx_f[0], 619, 0, __PYX_ERR(0, 619, __pyx_L1_error));
+  __Pyx_TraceCall("getboolean", __pyx_f[0], 624, 0, __PYX_ERR(0, 624, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":620
+  /* "configparserc/config.pyx":625
  * 
  *     def getboolean(self, option, fallback=None):
  *         return self.type_conversation(None, self.get(option, fallback), BoolType())             # <<<<<<<<<<<<<<
  * 
  *     def getint(self, option, fallback=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 620, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17528,57 +17948,57 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_option, __pyx_v_fallback};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_option, __pyx_v_fallback};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 620, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 625, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_option);
     __Pyx_GIVEREF(__pyx_v_option);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_option);
     __Pyx_INCREF(__pyx_v_fallback);
     __Pyx_GIVEREF(__pyx_v_fallback);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_fallback);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_BoolType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 620, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_BoolType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.conv_class = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_2);
-  __pyx_t_5 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 620, __pyx_L1_error)
+  __pyx_t_5 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":619
+  /* "configparserc/config.pyx":624
  *             .replace('}', '}}')
  * 
  *     def getboolean(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, fallback), BoolType())
  * 
  */
 
@@ -17593,15 +18013,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":622
+/* "configparserc/config.pyx":627
  *         return self.type_conversation(None, self.get(option, fallback), BoolType())
  * 
  *     def getint(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         value = self.get(option, str(fallback))
  *         return self.type_conversation(None, value, IntType())
  */
 
@@ -17640,15 +18060,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fallback);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getint") < 0)) __PYX_ERR(0, 622, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getint") < 0)) __PYX_ERR(0, 627, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -17656,15 +18076,15 @@
       }
     }
     __pyx_v_option = values[0];
     __pyx_v_fallback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getint", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 622, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getint", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 627, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.getint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_28getint(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_option, __pyx_v_fallback);
 
@@ -17685,26 +18105,26 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getint", 0);
-  __Pyx_TraceCall("getint", __pyx_f[0], 622, 0, __PYX_ERR(0, 622, __pyx_L1_error));
+  __Pyx_TraceCall("getint", __pyx_f[0], 627, 0, __PYX_ERR(0, 627, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":623
+  /* "configparserc/config.pyx":628
  * 
  *     def getint(self, option, fallback=None):
  *         value = self.get(option, str(fallback))             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, value, IntType())
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17713,69 +18133,69 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 628, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_option);
     __Pyx_GIVEREF(__pyx_v_option);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_option);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_value = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":624
+  /* "configparserc/config.pyx":629
  *     def getint(self, option, fallback=None):
  *         value = self.get(option, str(fallback))
  *         return self.type_conversation(None, value, IntType())             # <<<<<<<<<<<<<<
  * 
  *     def getseconds(self, option, fallback=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_IntType)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 624, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_IntType)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 629, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.conv_class = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_1);
-  __pyx_t_2 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_v_value, &__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 624, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_v_value, &__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 629, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":622
+  /* "configparserc/config.pyx":627
  *         return self.type_conversation(None, self.get(option, fallback), BoolType())
  * 
  *     def getint(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         value = self.get(option, str(fallback))
  *         return self.type_conversation(None, value, IntType())
  */
 
@@ -17792,15 +18212,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":626
+/* "configparserc/config.pyx":631
  *         return self.type_conversation(None, value, IntType())
  * 
  *     def getseconds(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, str(fallback)), IntSecondsType())
  * 
  */
 
@@ -17839,15 +18259,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fallback);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getseconds") < 0)) __PYX_ERR(0, 626, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getseconds") < 0)) __PYX_ERR(0, 631, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -17855,15 +18275,15 @@
       }
     }
     __pyx_v_option = values[0];
     __pyx_v_fallback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getseconds", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 626, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getseconds", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 631, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.getseconds", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_30getseconds(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_option, __pyx_v_fallback);
 
@@ -17883,27 +18303,27 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getseconds", 0);
-  __Pyx_TraceCall("getseconds", __pyx_f[0], 626, 0, __PYX_ERR(0, 626, __pyx_L1_error));
+  __Pyx_TraceCall("getseconds", __pyx_f[0], 631, 0, __PYX_ERR(0, 631, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":627
+  /* "configparserc/config.pyx":632
  * 
  *     def getseconds(self, option, fallback=None):
  *         return self.type_conversation(None, self.get(option, str(fallback)), IntSecondsType())             # <<<<<<<<<<<<<<
  * 
  *     def getbytes(self, option, fallback=None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17912,59 +18332,59 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 627, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 632, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_option);
     __Pyx_GIVEREF(__pyx_v_option);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_option);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_IntSecondsType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_IntSecondsType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.conv_class = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_2);
-  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":626
+  /* "configparserc/config.pyx":631
  *         return self.type_conversation(None, value, IntType())
  * 
  *     def getseconds(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, str(fallback)), IntSecondsType())
  * 
  */
 
@@ -17980,15 +18400,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":629
+/* "configparserc/config.pyx":634
  *         return self.type_conversation(None, self.get(option, str(fallback)), IntSecondsType())
  * 
  *     def getbytes(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, str(fallback)), BytesSizeType())
  * 
  */
 
@@ -18027,15 +18447,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fallback);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getbytes") < 0)) __PYX_ERR(0, 629, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getbytes") < 0)) __PYX_ERR(0, 634, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -18043,15 +18463,15 @@
       }
     }
     __pyx_v_option = values[0];
     __pyx_v_fallback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getbytes", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 629, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getbytes", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 634, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.getbytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_32getbytes(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_option, __pyx_v_fallback);
 
@@ -18071,27 +18491,27 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getbytes", 0);
-  __Pyx_TraceCall("getbytes", __pyx_f[0], 629, 0, __PYX_ERR(0, 629, __pyx_L1_error));
+  __Pyx_TraceCall("getbytes", __pyx_f[0], 634, 0, __PYX_ERR(0, 634, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":630
+  /* "configparserc/config.pyx":635
  * 
  *     def getbytes(self, option, fallback=None):
  *         return self.type_conversation(None, self.get(option, str(fallback)), BytesSizeType())             # <<<<<<<<<<<<<<
  * 
  *     def getlist(self, option, fallback=None, separator=','):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 635, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -18100,59 +18520,59 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_option);
     __Pyx_GIVEREF(__pyx_v_option);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_option);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_BytesSizeType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_BytesSizeType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.conv_class = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_2);
-  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 635, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":629
+  /* "configparserc/config.pyx":634
  *         return self.type_conversation(None, self.get(option, str(fallback)), IntSecondsType())
  * 
  *     def getbytes(self, option, fallback=None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, str(fallback)), BytesSizeType())
  * 
  */
 
@@ -18168,15 +18588,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":632
+/* "configparserc/config.pyx":637
  *         return self.type_conversation(None, self.get(option, str(fallback)), BytesSizeType())
  * 
  *     def getlist(self, option, fallback=None, separator=','):             # <<<<<<<<<<<<<<
  *         fallback = fallback or ''
  *         return self.type_conversation(None, self.get(option, fallback), ListType(separator))
  */
 
@@ -18225,15 +18645,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_separator);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getlist") < 0)) __PYX_ERR(0, 632, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getlist") < 0)) __PYX_ERR(0, 637, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -18244,15 +18664,15 @@
     }
     __pyx_v_option = values[0];
     __pyx_v_fallback = values[1];
     __pyx_v_separator = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getlist", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 632, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getlist", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 637, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.getlist", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_34getlist(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_option, __pyx_v_fallback, __pyx_v_separator);
 
@@ -18272,46 +18692,46 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getlist", 0);
-  __Pyx_TraceCall("getlist", __pyx_f[0], 632, 0, __PYX_ERR(0, 632, __pyx_L1_error));
+  __Pyx_TraceCall("getlist", __pyx_f[0], 637, 0, __PYX_ERR(0, 637, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_fallback);
 
-  /* "configparserc/config.pyx":633
+  /* "configparserc/config.pyx":638
  * 
  *     def getlist(self, option, fallback=None, separator=','):
  *         fallback = fallback or ''             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, fallback), ListType(separator))
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_fallback); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_fallback); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 638, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __Pyx_INCREF(__pyx_v_fallback);
     __pyx_t_1 = __pyx_v_fallback;
     goto __pyx_L3_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_kp_u__2);
   __pyx_t_1 = __pyx_kp_u__2;
   __pyx_L3_bool_binop_done:;
   __Pyx_DECREF_SET(__pyx_v_fallback, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":634
+  /* "configparserc/config.pyx":639
  *     def getlist(self, option, fallback=None, separator=','):
  *         fallback = fallback or ''
  *         return self.type_conversation(None, self.get(option, fallback), ListType(separator))             # <<<<<<<<<<<<<<
  * 
  *     def getjson(self, option, fallback = None):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -18320,57 +18740,57 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_v_fallback};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 639, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_v_fallback};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 639, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 634, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 639, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_option);
     __Pyx_GIVEREF(__pyx_v_option);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_option);
     __Pyx_INCREF(__pyx_v_fallback);
     __Pyx_GIVEREF(__pyx_v_fallback);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_fallback);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 639, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_13configparserc_6config_ListType), __pyx_v_separator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_13configparserc_6config_ListType), __pyx_v_separator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.conv_class = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_3);
-  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":632
+  /* "configparserc/config.pyx":637
  *         return self.type_conversation(None, self.get(option, str(fallback)), BytesSizeType())
  * 
  *     def getlist(self, option, fallback=None, separator=','):             # <<<<<<<<<<<<<<
  *         fallback = fallback or ''
  *         return self.type_conversation(None, self.get(option, fallback), ListType(separator))
  */
 
@@ -18386,15 +18806,15 @@
   __Pyx_XDECREF(__pyx_v_fallback);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":636
+/* "configparserc/config.pyx":641
  *         return self.type_conversation(None, self.get(option, fallback), ListType(separator))
  * 
  *     def getjson(self, option, fallback = None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, str(fallback)), JsonType())
  * 
  */
 
@@ -18433,15 +18853,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fallback);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getjson") < 0)) __PYX_ERR(0, 636, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "getjson") < 0)) __PYX_ERR(0, 641, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -18449,15 +18869,15 @@
       }
     }
     __pyx_v_option = values[0];
     __pyx_v_fallback = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("getjson", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 636, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("getjson", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 641, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.Section.getjson", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_13configparserc_6config_7Section_36getjson(((struct __pyx_obj_13configparserc_6config_Section *)__pyx_v_self), __pyx_v_option, __pyx_v_fallback);
 
@@ -18477,27 +18897,27 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getjson", 0);
-  __Pyx_TraceCall("getjson", __pyx_f[0], 636, 0, __PYX_ERR(0, 636, __pyx_L1_error));
+  __Pyx_TraceCall("getjson", __pyx_f[0], 641, 0, __PYX_ERR(0, 641, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":637
+  /* "configparserc/config.pyx":642
  * 
  *     def getjson(self, option, fallback = None):
  *         return self.type_conversation(None, self.get(option, str(fallback)), JsonType())             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fallback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -18506,59 +18926,59 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_option, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 642, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_option);
     __Pyx_GIVEREF(__pyx_v_option);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_option);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_JsonType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_JsonType)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7.__pyx_n = 1;
   __pyx_t_7.conv_class = ((struct __pyx_obj_13configparserc_6config_BaseType *)__pyx_t_2);
-  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_13configparserc_6config_Section *)__pyx_v_self->__pyx_vtab)->type_conversation(__pyx_v_self, ((PyObject*)Py_None), __pyx_t_1, &__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "configparserc/config.pyx":636
+  /* "configparserc/config.pyx":641
  *         return self.type_conversation(None, self.get(option, fallback), ListType(separator))
  * 
  *     def getjson(self, option, fallback = None):             # <<<<<<<<<<<<<<
  *         return self.type_conversation(None, self.get(option, str(fallback)), JsonType())
  * 
  */
 
@@ -18897,15 +19317,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "configparserc/config.pyx":641
+/* "configparserc/config.pyx":646
  * 
  * cdef class AppendSection(Section):
  *     def __init__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         super().__init__(*args, **kwargs)
  *         for key, value in self.get_default_data().items():
  */
 
@@ -18947,119 +19367,119 @@
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 641, 0, __PYX_ERR(0, 641, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 646, 0, __PYX_ERR(0, 646, __pyx_L1_error));
 
-  /* "configparserc/config.pyx":642
+  /* "configparserc/config.pyx":647
  * cdef class AppendSection(Section):
  *     def __init__(self, *args, **kwargs):
  *         super().__init__(*args, **kwargs)             # <<<<<<<<<<<<<<
  *         for key, value in self.get_default_data().items():
  *             if key not in self:
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_13configparserc_6config_AppendSection));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_13configparserc_6config_AppendSection));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_ptype_13configparserc_6config_AppendSection));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "configparserc/config.pyx":643
+  /* "configparserc/config.pyx":648
  *     def __init__(self, *args, **kwargs):
  *         super().__init__(*args, **kwargs)
  *         for key, value in self.get_default_data().items():             # <<<<<<<<<<<<<<
  *             if key not in self:
  *                 self[key] = value
  */
   __pyx_t_4 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_default_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_default_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2 == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 643, __pyx_L1_error)
+    __PYX_ERR(0, 648, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(__pyx_t_2, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(__pyx_t_2, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_XDECREF(__pyx_t_3);
   __pyx_t_3 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_5, &__pyx_t_4, &__pyx_t_1, &__pyx_t_2, NULL, __pyx_t_6);
     if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 643, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "configparserc/config.pyx":644
+    /* "configparserc/config.pyx":649
  *         super().__init__(*args, **kwargs)
  *         for key, value in self.get_default_data().items():
  *             if key not in self:             # <<<<<<<<<<<<<<
  *                 self[key] = value
  */
-    __pyx_t_9 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 644, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PySequence_ContainsTF(__pyx_v_key, ((PyObject *)__pyx_v_self), Py_NE)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 649, __pyx_L1_error)
     __pyx_t_10 = (__pyx_t_9 != 0);
     if (__pyx_t_10) {
 
-      /* "configparserc/config.pyx":645
+      /* "configparserc/config.pyx":650
  *         for key, value in self.get_default_data().items():
  *             if key not in self:
  *                 self[key] = value             # <<<<<<<<<<<<<<
  */
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_v_value) < 0)) __PYX_ERR(0, 645, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_key, __pyx_v_value) < 0)) __PYX_ERR(0, 650, __pyx_L1_error)
 
-      /* "configparserc/config.pyx":644
+      /* "configparserc/config.pyx":649
  *         super().__init__(*args, **kwargs)
  *         for key, value in self.get_default_data().items():
  *             if key not in self:             # <<<<<<<<<<<<<<
  *                 self[key] = value
  */
     }
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "configparserc/config.pyx":641
+  /* "configparserc/config.pyx":646
  * 
  * cdef class AppendSection(Section):
  *     def __init__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         super().__init__(*args, **kwargs)
  *         for key, value in self.get_default_data().items():
  */
 
@@ -22902,23 +23322,412 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
+ * def __pyx_unpickle_TimedeltaType(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13configparserc_6config_19__pyx_unpickle_TimedeltaType(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_13configparserc_6config_19__pyx_unpickle_TimedeltaType = {"__pyx_unpickle_TimedeltaType", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_19__pyx_unpickle_TimedeltaType, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13configparserc_6config_19__pyx_unpickle_TimedeltaType(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__pyx_unpickle_TimedeltaType (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_TimedeltaType", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_TimedeltaType", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_TimedeltaType") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_TimedeltaType", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_TimedeltaType", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_13configparserc_6config_18__pyx_unpickle_TimedeltaType(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13configparserc_6config_18__pyx_unpickle_TimedeltaType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__35)
+  __Pyx_RefNannySetupContext("__pyx_unpickle_TimedeltaType", 0);
+  __Pyx_TraceCall("__pyx_unpickle_TimedeltaType", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__26, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *     __pyx_result = TimedeltaType.__new__(__pyx_type)
+ */
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":6
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = TimedeltaType.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ */
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_ERR(1, 6, __pyx_L1_error)
+
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ */
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *     __pyx_result = TimedeltaType.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_13configparserc_6config_TimedeltaType), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *     __pyx_result = TimedeltaType.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = TimedeltaType.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):
+ */
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_13configparserc_6config___pyx_unpickle_TimedeltaType__set_state(((struct __pyx_obj_13configparserc_6config_TimedeltaType *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ *     __pyx_result = TimedeltaType.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):
+ *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_TimedeltaType(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_TimedeltaType", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[0])
+ */
+
+static PyObject *__pyx_f_13configparserc_6config___pyx_unpickle_TimedeltaType__set_state(struct __pyx_obj_13configparserc_6config_TimedeltaType *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_TimedeltaType__set_state", 0);
+  __Pyx_TraceCall("__pyx_unpickle_TimedeltaType__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):
+ *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[0])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_2 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_3 = ((__pyx_t_2 > 0) != 0);
+  if (__pyx_t_3) {
+  } else {
+    __pyx_t_1 = __pyx_t_3;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_3 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_3 != 0);
+  __pyx_t_1 = __pyx_t_4;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_1) {
+
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):
+ *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[0])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 13, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+      }
+    }
+    __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):
+ *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[0])
+ */
+  }
+
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_TimedeltaType__set_state(<TimedeltaType> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_TimedeltaType__set_state(TimedeltaType __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[0])
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_TimedeltaType__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
  * def __pyx_unpickle_JsonType(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13configparserc_6config_19__pyx_unpickle_JsonType(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_13configparserc_6config_19__pyx_unpickle_JsonType = {"__pyx_unpickle_JsonType", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_19__pyx_unpickle_JsonType, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_13configparserc_6config_19__pyx_unpickle_JsonType(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13configparserc_6config_21__pyx_unpickle_JsonType(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_13configparserc_6config_21__pyx_unpickle_JsonType = {"__pyx_unpickle_JsonType", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_21__pyx_unpickle_JsonType, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13configparserc_6config_21__pyx_unpickle_JsonType(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -22976,37 +23785,37 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_JsonType", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_JsonType", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13configparserc_6config_18__pyx_unpickle_JsonType(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_13configparserc_6config_20__pyx_unpickle_JsonType(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13configparserc_6config_18__pyx_unpickle_JsonType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_13configparserc_6config_20__pyx_unpickle_JsonType(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__35)
+  __Pyx_TraceFrameInit(__pyx_codeobj__36)
   __Pyx_RefNannySetupContext("__pyx_unpickle_JsonType", 0);
   __Pyx_TraceCall("__pyx_unpickle_JsonType", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
@@ -23297,17 +24106,17 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle___BaseDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13configparserc_6config_21__pyx_unpickle___BaseDict(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_13configparserc_6config_21__pyx_unpickle___BaseDict = {"__pyx_unpickle___BaseDict", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_21__pyx_unpickle___BaseDict, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_13configparserc_6config_21__pyx_unpickle___BaseDict(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13configparserc_6config_23__pyx_unpickle___BaseDict(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_13configparserc_6config_23__pyx_unpickle___BaseDict = {"__pyx_unpickle___BaseDict", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_23__pyx_unpickle___BaseDict, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13configparserc_6config_23__pyx_unpickle___BaseDict(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -23365,37 +24174,37 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle___BaseDict", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.__pyx_unpickle___BaseDict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13configparserc_6config_20__pyx_unpickle___BaseDict(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_13configparserc_6config_22__pyx_unpickle___BaseDict(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13configparserc_6config_20__pyx_unpickle___BaseDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_13configparserc_6config_22__pyx_unpickle___BaseDict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__36)
+  __Pyx_TraceFrameInit(__pyx_codeobj__37)
   __Pyx_RefNannySetupContext("__pyx_unpickle___BaseDict", 0);
   __Pyx_TraceCall("__pyx_unpickle___BaseDict", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
@@ -23686,17 +24495,17 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_ConfigParserC(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13configparserc_6config_23__pyx_unpickle_ConfigParserC(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_13configparserc_6config_23__pyx_unpickle_ConfigParserC = {"__pyx_unpickle_ConfigParserC", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_23__pyx_unpickle_ConfigParserC, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_13configparserc_6config_23__pyx_unpickle_ConfigParserC(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13configparserc_6config_25__pyx_unpickle_ConfigParserC(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_13configparserc_6config_25__pyx_unpickle_ConfigParserC = {"__pyx_unpickle_ConfigParserC", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_25__pyx_unpickle_ConfigParserC, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13configparserc_6config_25__pyx_unpickle_ConfigParserC(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -23754,50 +24563,50 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ConfigParserC", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_ConfigParserC", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13configparserc_6config_22__pyx_unpickle_ConfigParserC(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_13configparserc_6config_24__pyx_unpickle_ConfigParserC(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13configparserc_6config_22__pyx_unpickle_ConfigParserC(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_13configparserc_6config_24__pyx_unpickle_ConfigParserC(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__37)
+  __Pyx_TraceFrameInit(__pyx_codeobj__38)
   __Pyx_RefNannySetupContext("__pyx_unpickle_ConfigParserC", 0);
   __Pyx_TraceCall("__pyx_unpickle_ConfigParserC", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x455c0eb, 0xea5e48a, 0x7aea40a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x455c0eb, 0xea5e48a, 0x7aea40a) = (__format_exclude_sections, __format_kwargs, __sections_map, section_defaults))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__38, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__39, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x455c0eb, 0xea5e48a, 0x7aea40a):
@@ -24131,17 +24940,17 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_Section(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13configparserc_6config_25__pyx_unpickle_Section(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_13configparserc_6config_25__pyx_unpickle_Section = {"__pyx_unpickle_Section", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_25__pyx_unpickle_Section, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_13configparserc_6config_25__pyx_unpickle_Section(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13configparserc_6config_27__pyx_unpickle_Section(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_13configparserc_6config_27__pyx_unpickle_Section = {"__pyx_unpickle_Section", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_27__pyx_unpickle_Section, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13configparserc_6config_27__pyx_unpickle_Section(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -24199,50 +25008,50 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Section", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_Section", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13configparserc_6config_24__pyx_unpickle_Section(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_13configparserc_6config_26__pyx_unpickle_Section(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13configparserc_6config_24__pyx_unpickle_Section(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_13configparserc_6config_26__pyx_unpickle_Section(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__39)
+  __Pyx_TraceFrameInit(__pyx_codeobj__40)
   __Pyx_RefNannySetupContext("__pyx_unpickle_Section", 0);
   __Pyx_TraceCall("__pyx_unpickle_Section", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf8673bb, 0xf9e5dba, 0xf3a42cf):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf8673bb, 0xf9e5dba, 0xf3a42cf) = (__type_map, config, name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__40, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__41, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf8673bb, 0xf9e5dba, 0xf3a42cf):
@@ -24564,17 +25373,17 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_AppendSection(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13configparserc_6config_27__pyx_unpickle_AppendSection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_13configparserc_6config_27__pyx_unpickle_AppendSection = {"__pyx_unpickle_AppendSection", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_27__pyx_unpickle_AppendSection, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_13configparserc_6config_27__pyx_unpickle_AppendSection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13configparserc_6config_29__pyx_unpickle_AppendSection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_13configparserc_6config_29__pyx_unpickle_AppendSection = {"__pyx_unpickle_AppendSection", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13configparserc_6config_29__pyx_unpickle_AppendSection, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_13configparserc_6config_29__pyx_unpickle_AppendSection(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -24632,50 +25441,50 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_AppendSection", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("configparserc.config.__pyx_unpickle_AppendSection", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13configparserc_6config_26__pyx_unpickle_AppendSection(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_13configparserc_6config_28__pyx_unpickle_AppendSection(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13configparserc_6config_26__pyx_unpickle_AppendSection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_13configparserc_6config_28__pyx_unpickle_AppendSection(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__41)
+  __Pyx_TraceFrameInit(__pyx_codeobj__42)
   __Pyx_RefNannySetupContext("__pyx_unpickle_AppendSection", 0);
   __Pyx_TraceCall("__pyx_unpickle_AppendSection", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf8673bb, 0xf9e5dba, 0xf3a42cf):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf8673bb, 0xf9e5dba, 0xf3a42cf) = (__type_map, config, name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__40, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__41, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf8673bb, 0xf9e5dba, 0xf3a42cf):
@@ -25156,15 +25965,15 @@
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_dict____dict____unicode___to_py")
  * cdef object __Pyx_CFunc_dict____dict____unicode___to_py(dict (*f)(dict, unicode) ):
  *     def wrap(dict collect, unicode key):             # <<<<<<<<<<<<<<
  *         """wrap(collect: dict, key: unicode) -> dict"""
  *         return f(collect, key)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_43__Pyx_CFunc_dict____dict____unicode___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_dict____dict____unic, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_43__Pyx_CFunc_dict____dict____unicode___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_dict____dict____unic, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":68
  *         """wrap(collect: dict, key: unicode) -> dict"""
  *         return f(collect, key)
@@ -25306,15 +26115,15 @@
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_bint____object___to_py")
  * cdef object __Pyx_CFunc_bint____object___to_py(bint (*f)(object) except *):
  *     def wrap(object obj):             # <<<<<<<<<<<<<<
  *         """wrap(obj) -> bool"""
  *         return f(obj)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_34__Pyx_CFunc_bint____object___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_bint____object___to, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_34__Pyx_CFunc_bint____object___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_bint____object___to, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":68
  *         """wrap(obj) -> bool"""
  *         return f(obj)
@@ -25462,15 +26271,15 @@
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_unicode____Section___to_py")
  * cdef object __Pyx_CFunc_unicode____Section___to_py(unicode (*f)(Section) ):
  *     def wrap(Section section):             # <<<<<<<<<<<<<<
  *         """wrap(section: 'Section') -> unicode"""
  *         return f(section)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_38__Pyx_CFunc_unicode____Section___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_unicode____Section, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_38__Pyx_CFunc_unicode____Section___to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_unicode____Section, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":68
  *         """wrap(section: 'Section') -> unicode"""
  *         return f(section)
@@ -26334,14 +27143,103 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
+static PyObject *__pyx_tp_new_13configparserc_6config_TimedeltaType(PyTypeObject *t, PyObject *a, PyObject *k) {
+  PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
+  if (unlikely(!o)) return 0;
+  return o;
+}
+
+static PyMethodDef __pyx_methods_13configparserc_6config_TimedeltaType[] = {
+  {"convert", (PyCFunction)__pyx_pw_13configparserc_6config_13TimedeltaType_1convert, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_13configparserc_6config_13TimedeltaType_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_13configparserc_6config_13TimedeltaType_5__setstate_cython__, METH_O, 0},
+  {0, 0, 0, 0}
+};
+
+static PyTypeObject __pyx_type_13configparserc_6config_TimedeltaType = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "configparserc.config.TimedeltaType", /*tp_name*/
+  sizeof(struct __pyx_obj_13configparserc_6config_TimedeltaType), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_13configparserc_6config_BaseType, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  #if CYTHON_COMPILING_IN_PYPY
+  __pyx_pw_13configparserc_6config_8BaseType_5__call__, /*tp_call*/
+  #else
+  0, /*tp_call*/
+  #endif
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
+  0, /*tp_doc*/
+  0, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_13configparserc_6config_TimedeltaType, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  0, /*tp_dictoffset*/
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_13configparserc_6config_TimedeltaType, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  0, /*tp_finalize*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  0, /*tp_print*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+
 static PyObject *__pyx_tp_new_13configparserc_6config_ListType(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_13configparserc_6config_ListType *p;
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_13configparserc_6config_ListType *)o);
   p->separator = ((PyObject*)Py_None); Py_INCREF(Py_None);
   if (unlikely(__pyx_pw_13configparserc_6config_8ListType_1__cinit__(o, a, k) < 0)) goto bad;
@@ -27525,14 +28423,15 @@
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_CFunc_bint____object___to, __pyx_k_Pyx_CFunc_bint____object___to, sizeof(__pyx_k_Pyx_CFunc_bint____object___to), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_CFunc_dict____dict____unic, __pyx_k_Pyx_CFunc_dict____dict____unic, sizeof(__pyx_k_Pyx_CFunc_dict____dict____unic), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_CFunc_unicode____Section, __pyx_k_Pyx_CFunc_unicode____Section, sizeof(__pyx_k_Pyx_CFunc_unicode____Section), 0, 0, 1, 1},
   {&__pyx_n_s_SafeLoader, __pyx_k_SafeLoader, sizeof(__pyx_k_SafeLoader), 0, 0, 1, 1},
   {&__pyx_n_s_Section, __pyx_k_Section, sizeof(__pyx_k_Section), 0, 0, 1, 1},
   {&__pyx_n_s_StrType, __pyx_k_StrType, sizeof(__pyx_k_StrType), 0, 0, 1, 1},
+  {&__pyx_n_s_TimedeltaType, __pyx_k_TimedeltaType, sizeof(__pyx_k_TimedeltaType), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_YAML_LOADER, __pyx_k_YAML_LOADER, sizeof(__pyx_k_YAML_LOADER), 0, 0, 1, 1},
   {&__pyx_kp_u__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 1, 0, 0},
   {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
   {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_kp_u__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 1, 0, 0},
@@ -27541,14 +28440,15 @@
   {&__pyx_kp_u__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 1, 0, 0},
   {&__pyx_kp_u__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 1, 0, 0},
   {&__pyx_n_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 1},
   {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
   {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
   {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
+  {&__pyx_n_s_as_timedelta, __pyx_k_as_timedelta, sizeof(__pyx_k_as_timedelta), 0, 0, 1, 1},
   {&__pyx_n_u_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 1, 0, 1},
   {&__pyx_n_s_cfunc_to_py, __pyx_k_cfunc_to_py, sizeof(__pyx_k_cfunc_to_py), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_collect, __pyx_k_collect, sizeof(__pyx_k_collect), 0, 0, 1, 1},
   {&__pyx_n_s_compile, __pyx_k_compile, sizeof(__pyx_k_compile), 0, 0, 1, 1},
   {&__pyx_n_s_config, __pyx_k_config, sizeof(__pyx_k_config), 0, 0, 1, 1},
@@ -27629,14 +28529,15 @@
   {&__pyx_n_s_pyx_unpickle_Empty, __pyx_k_pyx_unpickle_Empty, sizeof(__pyx_k_pyx_unpickle_Empty), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_IntSecondsType, __pyx_k_pyx_unpickle_IntSecondsType, sizeof(__pyx_k_pyx_unpickle_IntSecondsType), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_IntType, __pyx_k_pyx_unpickle_IntType, sizeof(__pyx_k_pyx_unpickle_IntType), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_JsonType, __pyx_k_pyx_unpickle_JsonType, sizeof(__pyx_k_pyx_unpickle_JsonType), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_ParseError, __pyx_k_pyx_unpickle_ParseError, sizeof(__pyx_k_pyx_unpickle_ParseError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Section, __pyx_k_pyx_unpickle_Section, sizeof(__pyx_k_pyx_unpickle_Section), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_StrType, __pyx_k_pyx_unpickle_StrType, sizeof(__pyx_k_pyx_unpickle_StrType), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_TimedeltaType, __pyx_k_pyx_unpickle_TimedeltaType, sizeof(__pyx_k_pyx_unpickle_TimedeltaType), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle___BaseDict, __pyx_k_pyx_unpickle___BaseDict, sizeof(__pyx_k_pyx_unpickle___BaseDict), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_raise_exception, __pyx_k_raise_exception, sizeof(__pyx_k_raise_exception), 0, 0, 1, 1},
   {&__pyx_n_s_re, __pyx_k_re, sizeof(__pyx_k_re), 0, 0, 1, 1},
   {&__pyx_n_s_re_size, __pyx_k_re_size, sizeof(__pyx_k_re_size), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_2, __pyx_k_reduce_2, sizeof(__pyx_k_reduce_2), 0, 0, 1, 1},
@@ -27682,19 +28583,19 @@
   {&__pyx_n_s_wrap, __pyx_k_wrap, sizeof(__pyx_k_wrap), 0, 0, 1, 1},
   {&__pyx_n_s_yaml, __pyx_k_yaml, sizeof(__pyx_k_yaml), 0, 0, 1, 1},
   {&__pyx_n_u_yaml, __pyx_k_yaml, sizeof(__pyx_k_yaml), 0, 1, 0, 1},
   {&__pyx_n_u_yml, __pyx_k_yml, sizeof(__pyx_k_yml), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 188, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 249, __pyx_L1_error)
-  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 559, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 575, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -27715,167 +28616,171 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "configparserc/config.pyx":397
+  /* "configparserc/config.pyx":402
  * 
  *     def parse_yaml_file(self, filename):
  *         with File(filename) as fd:             # <<<<<<<<<<<<<<
  *             for document in yaml.load_all(fd, Loader=YAML_LOADER):
  *                 if not document:
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "configparserc/config.pyx":408
+  /* "configparserc/config.pyx":413
  * 
  *     def parse_files(self, filename_array: _t.Sequence):
  *         for filepath in list(filter(bool, filename_array))[::-1]:             # <<<<<<<<<<<<<<
  *             if not os.path.exists(filepath):
  *                 continue
  */
-  __pyx_slice__14 = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice__14)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_slice__14 = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice__14)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__14);
   __Pyx_GIVEREF(__pyx_slice__14);
 
-  /* "configparserc/config.pyx":411
+  /* "configparserc/config.pyx":416
  *             if not os.path.exists(filepath):
  *                 continue
  *             if filepath.rsplit('.', 1)[-1] in ('yaml', 'yml'):             # <<<<<<<<<<<<<<
  *                 self.parse_yaml_file(filepath)
  *             else:
  */
-  __pyx_tuple__15 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_int_1); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_int_1); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "configparserc/config.pyx":421
+  /* "configparserc/config.pyx":426
  *         error = self._parse_text(text.encode('utf-8'))
  *         if error:
  *             raise ParseError('Couldnt parse config string without section and key-value in text.')             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_Couldnt_parse_config_string_with_2); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_Couldnt_parse_config_string_with_2); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "configparserc/config.pyx":464
+  /* "configparserc/config.pyx":469
  *             Section parent
  * 
  *         parent_path = self.name.split('.')[:-1]             # <<<<<<<<<<<<<<
  *         if not parent_path:
  *             return None
  */
-  __pyx_slice__17 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_slice__17 = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__17);
   __Pyx_GIVEREF(__pyx_slice__17);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   __pyx_tuple__26 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_int_72728811, __pyx_int_245752970, __pyx_int_128885770); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_int_260469691, __pyx_int_262036922, __pyx_int_255476431); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_int_72728811, __pyx_int_245752970, __pyx_int_128885770); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_int_260469691, __pyx_int_262036922, __pyx_int_255476431); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_dict____dict____unicode___to_py")
  * cdef object __Pyx_CFunc_dict____dict____unicode___to_py(dict (*f)(dict, unicode) ):
  *     def wrap(dict collect, unicode key):             # <<<<<<<<<<<<<<
  *         """wrap(collect: dict, key: unicode) -> dict"""
  *         return f(collect, key)
  */
-  __pyx_tuple__42 = PyTuple_Pack(2, __pyx_n_s_collect, __pyx_n_s_key); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
-  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __pyx_tuple__44 = PyTuple_Pack(1, __pyx_n_s_obj); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_n_s_section_2); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__46);
-  __Pyx_GIVEREF(__pyx_tuple__46);
-  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(2, __pyx_n_s_collect, __pyx_n_s_key); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_n_s_obj); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_n_s_section_2); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(1, 65, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Empty(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__48 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Empty, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__49 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ConfigParserExcep, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Empty, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__50 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ParseError, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ConfigParserExcep, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__51 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BaseType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ParseError, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__52 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StrType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BaseType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__53 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StrType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__54 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BytesSizeType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__55 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BoolType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BytesSizeType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__56 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__56);
   __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntSecondsType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BoolType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__57 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_JsonType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntSecondsType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__58 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle___BaseDict, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TimedeltaType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__59 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__59);
   __Pyx_GIVEREF(__pyx_tuple__59);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ConfigParserC, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_JsonType, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__60 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Section, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle___BaseDict, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__61 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__61);
   __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AppendSection, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ConfigParserC, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Section, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AppendSection, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -28031,101 +28936,112 @@
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_IntSecondsType.tp_dictoffset && __pyx_type_13configparserc_6config_IntSecondsType.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config_IntSecondsType.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_IntSecondsType, (PyObject *)&__pyx_type_13configparserc_6config_IntSecondsType) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_IntSecondsType) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config_IntSecondsType = &__pyx_type_13configparserc_6config_IntSecondsType;
+  __pyx_type_13configparserc_6config_TimedeltaType.tp_base = __pyx_ptype_13configparserc_6config_BaseType;
+  if (PyType_Ready(&__pyx_type_13configparserc_6config_TimedeltaType) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_13configparserc_6config_TimedeltaType.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_TimedeltaType.tp_dictoffset && __pyx_type_13configparserc_6config_TimedeltaType.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_13configparserc_6config_TimedeltaType.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_TimedeltaType, (PyObject *)&__pyx_type_13configparserc_6config_TimedeltaType) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_TimedeltaType) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_ptype_13configparserc_6config_TimedeltaType = &__pyx_type_13configparserc_6config_TimedeltaType;
   __pyx_type_13configparserc_6config_ListType.tp_base = __pyx_ptype_13configparserc_6config_BaseType;
-  if (PyType_Ready(&__pyx_type_13configparserc_6config_ListType) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13configparserc_6config_ListType) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13configparserc_6config_ListType.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_ListType.tp_dictoffset && __pyx_type_13configparserc_6config_ListType.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config_ListType.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ListType, (PyObject *)&__pyx_type_13configparserc_6config_ListType) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_ListType) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ListType, (PyObject *)&__pyx_type_13configparserc_6config_ListType) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_ListType) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config_ListType = &__pyx_type_13configparserc_6config_ListType;
   __pyx_type_13configparserc_6config_JsonType.tp_base = __pyx_ptype_13configparserc_6config_BaseType;
-  if (PyType_Ready(&__pyx_type_13configparserc_6config_JsonType) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13configparserc_6config_JsonType) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13configparserc_6config_JsonType.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_JsonType.tp_dictoffset && __pyx_type_13configparserc_6config_JsonType.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config_JsonType.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_JsonType, (PyObject *)&__pyx_type_13configparserc_6config_JsonType) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_JsonType) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_JsonType, (PyObject *)&__pyx_type_13configparserc_6config_JsonType) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_JsonType) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config_JsonType = &__pyx_type_13configparserc_6config_JsonType;
   __pyx_type_13configparserc_6config___BaseDict.tp_base = (&PyDict_Type);
-  if (PyType_Ready(&__pyx_type_13configparserc_6config___BaseDict) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13configparserc_6config___BaseDict) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13configparserc_6config___BaseDict.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config___BaseDict.tp_dictoffset && __pyx_type_13configparserc_6config___BaseDict.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config___BaseDict.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BaseDict, (PyObject *)&__pyx_type_13configparserc_6config___BaseDict) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config___BaseDict) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BaseDict, (PyObject *)&__pyx_type_13configparserc_6config___BaseDict) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config___BaseDict) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config___BaseDict = &__pyx_type_13configparserc_6config___BaseDict;
   __pyx_vtabptr_13configparserc_6config_ConfigParserC = &__pyx_vtable_13configparserc_6config_ConfigParserC;
   __pyx_vtable_13configparserc_6config_ConfigParserC.__pyx___set_object_item = (void (*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, PyObject *, PyObject *))__pyx_f_13configparserc_6config_13ConfigParserC___set_object_item;
   __pyx_vtable_13configparserc_6config_ConfigParserC._parse_section = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, PyObject *))__pyx_f_13configparserc_6config_13ConfigParserC__parse_section;
   __pyx_vtable_13configparserc_6config_ConfigParserC._parse_pair = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, PyObject *))__pyx_f_13configparserc_6config_13ConfigParserC__parse_pair;
   __pyx_vtable_13configparserc_6config_ConfigParserC._add_section = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, PyObject *))__pyx_f_13configparserc_6config_13ConfigParserC__add_section;
   __pyx_vtable_13configparserc_6config_ConfigParserC._parse_file = (int (*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, FILE *, unsigned PY_LONG_LONG))__pyx_f_13configparserc_6config_13ConfigParserC__parse_file;
   __pyx_vtable_13configparserc_6config_ConfigParserC._parse_file_by_name = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, char *))__pyx_f_13configparserc_6config_13ConfigParserC__parse_file_by_name;
   __pyx_vtable_13configparserc_6config_ConfigParserC._parse_text = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_ConfigParserC *, char *))__pyx_f_13configparserc_6config_13ConfigParserC__parse_text;
   __pyx_type_13configparserc_6config_ConfigParserC.tp_base = __pyx_ptype_13configparserc_6config___BaseDict;
-  if (PyType_Ready(&__pyx_type_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13configparserc_6config_ConfigParserC.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_ConfigParserC.tp_dictoffset && __pyx_type_13configparserc_6config_ConfigParserC.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config_ConfigParserC.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_13configparserc_6config_ConfigParserC.tp_dict, __pyx_vtabptr_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ConfigParserC, (PyObject *)&__pyx_type_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_13configparserc_6config_ConfigParserC.tp_dict, __pyx_vtabptr_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ConfigParserC, (PyObject *)&__pyx_type_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_ConfigParserC) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config_ConfigParserC = &__pyx_type_13configparserc_6config_ConfigParserC;
   __pyx_vtabptr_13configparserc_6config_Section = &__pyx_vtable_13configparserc_6config_Section;
   __pyx_vtable_13configparserc_6config_Section.get_parent = (struct __pyx_obj_13configparserc_6config_Section *(*)(struct __pyx_obj_13configparserc_6config_Section *))__pyx_f_13configparserc_6config_7Section_get_parent;
   __pyx_vtable_13configparserc_6config_Section.__pyx___set_item_value = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *, PyObject *))__pyx_f_13configparserc_6config_7Section___set_item_value;
   __pyx_vtable_13configparserc_6config_Section.__pyx___get_item_value = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *))__pyx_f_13configparserc_6config_7Section___get_item_value;
   __pyx_vtable_13configparserc_6config_Section._get_subsection_name = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *))__pyx_f_13configparserc_6config_7Section__get_subsection_name;
   __pyx_vtable_13configparserc_6config_Section.__pyx___get_default_data = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *))__pyx_f_13configparserc_6config_7Section___get_default_data;
   __pyx_vtable_13configparserc_6config_Section.__pyx___get_default_value = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *))__pyx_f_13configparserc_6config_7Section___get_default_value;
   __pyx_vtable_13configparserc_6config_Section.get_type_conversation_instance = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *, struct __pyx_opt_args_13configparserc_6config_7Section_get_type_conversation_instance *__pyx_optional_args))__pyx_f_13configparserc_6config_7Section_get_type_conversation_instance;
   __pyx_vtable_13configparserc_6config_Section.type_conversation = (PyObject *(*)(struct __pyx_obj_13configparserc_6config_Section *, PyObject *, PyObject *, struct __pyx_opt_args_13configparserc_6config_7Section_type_conversation *__pyx_optional_args))__pyx_f_13configparserc_6config_7Section_type_conversation;
   __pyx_type_13configparserc_6config_Section.tp_base = __pyx_ptype_13configparserc_6config___BaseDict;
-  if (PyType_Ready(&__pyx_type_13configparserc_6config_Section) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13configparserc_6config_Section) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13configparserc_6config_Section.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_Section.tp_dictoffset && __pyx_type_13configparserc_6config_Section.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config_Section.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_13configparserc_6config_Section.tp_dict, __pyx_vtabptr_13configparserc_6config_Section) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Section, (PyObject *)&__pyx_type_13configparserc_6config_Section) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_Section) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_13configparserc_6config_Section.tp_dict, __pyx_vtabptr_13configparserc_6config_Section) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Section, (PyObject *)&__pyx_type_13configparserc_6config_Section) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_Section) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config_Section = &__pyx_type_13configparserc_6config_Section;
   __pyx_vtabptr_13configparserc_6config_AppendSection = &__pyx_vtable_13configparserc_6config_AppendSection;
   __pyx_vtable_13configparserc_6config_AppendSection.__pyx_base = *__pyx_vtabptr_13configparserc_6config_Section;
   __pyx_type_13configparserc_6config_AppendSection.tp_base = __pyx_ptype_13configparserc_6config_Section;
-  if (PyType_Ready(&__pyx_type_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13configparserc_6config_AppendSection.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13configparserc_6config_AppendSection.tp_dictoffset && __pyx_type_13configparserc_6config_AppendSection.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13configparserc_6config_AppendSection.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_13configparserc_6config_AppendSection.tp_dict, __pyx_vtabptr_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AppendSection, (PyObject *)&__pyx_type_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_13configparserc_6config_AppendSection.tp_dict, __pyx_vtabptr_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AppendSection, (PyObject *)&__pyx_type_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13configparserc_6config_AppendSection) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
   __pyx_ptype_13configparserc_6config_AppendSection = &__pyx_type_13configparserc_6config_AppendSection;
   if (PyType_Ready(&__pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py) < 0) __PYX_ERR(1, 64, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py.tp_dictoffset && __pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -28162,17 +29078,17 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -28624,29 +29540,29 @@
   __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_int_1024); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_13configparserc_6config_BytesSizeType->tp_dict, __pyx_n_s_tb, __pyx_t_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_13configparserc_6config_BytesSizeType);
 
-  /* "configparserc/config.pyx":220
+  /* "configparserc/config.pyx":225
  * cdef class ConfigParserC(__BaseDict):
  * 
  *     section_regex = re.compile(r"^\[(?P<section>(.+))\].*$", re.MULTILINE)             # <<<<<<<<<<<<<<
  *     pair_regex = re.compile(r"^(?P<key>([^\s]+?))[\s]{0,}=[\s]{0,}(?P<value>(.*?))[\s]{0,}$", re.MULTILINE)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_re); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MULTILINE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MULTILINE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -28656,65 +29572,65 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_kp_u_P_section, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_kp_u_P_section, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_kp_u_P_section);
     __Pyx_GIVEREF(__pyx_kp_u_P_section);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_kp_u_P_section);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC->tp_dict, __pyx_n_s_section_regex, __pyx_t_1) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC->tp_dict, __pyx_n_s_section_regex, __pyx_t_1) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_13configparserc_6config_ConfigParserC);
 
-  /* "configparserc/config.pyx":221
+  /* "configparserc/config.pyx":226
  * 
  *     section_regex = re.compile(r"^\[(?P<section>(.+))\].*$", re.MULTILINE)
  *     pair_regex = re.compile(r"^(?P<key>([^\s]+?))[\s]{0,}=[\s]{0,}(?P<value>(.*?))[\s]{0,}$", re.MULTILINE)             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_re); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_re); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_re); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_re); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_MULTILINE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_MULTILINE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_3)) {
@@ -28724,84 +29640,84 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_kp_u_P_key_s_s_0_s_0_P_value_s_0, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_kp_u_P_key_s_s_0_s_0_P_value_s_0, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_2 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_kp_u_P_key_s_s_0_s_0_P_value_s_0);
     __Pyx_GIVEREF(__pyx_kp_u_P_key_s_s_0_s_0_P_value_s_0);
     PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_5, __pyx_kp_u_P_key_s_s_0_s_0_P_value_s_0);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_5, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC->tp_dict, __pyx_n_s_pair_regex, __pyx_t_1) < 0) __PYX_ERR(0, 221, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_13configparserc_6config_ConfigParserC->tp_dict, __pyx_n_s_pair_regex, __pyx_t_1) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_13configparserc_6config_ConfigParserC);
 
-  /* "configparserc/config.pyx":279
+  /* "configparserc/config.pyx":284
  *         self.__set_object_item(key, value)
  * 
  *     def get(self, key, default = Empty()):             # <<<<<<<<<<<<<<
  *         if key not in self and not isinstance(default, Empty):
  *             return self.get_section_instance(key, default=default)
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_Empty)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_Empty)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_k__7 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":567
+  /* "configparserc/config.pyx":572
  *         return self.__class__(self.name, self.config, default=super().copy())
  * 
  *     def get(self, key, fallback = Empty()):             # <<<<<<<<<<<<<<
  *         try:
  *             return self[key]
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_Empty)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_Empty)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_k__18 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "configparserc/config.pyx":585
+  /* "configparserc/config.pyx":590
  *         return key
  * 
  *     cdef object get_type_conversation_instance(self, str key, object default=BaseType()):             # <<<<<<<<<<<<<<
  *         if PyDict_Contains(self.__type_map, key) == 1:
  *             return <object>PyDict_GetItem(self.__type_map, key)
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_BaseType)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 585, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_13configparserc_6config_BaseType)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_k__19 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Empty(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
@@ -28904,59 +29820,69 @@
   /* "(tree fragment)":11
  *         __pyx_unpickle_IntSecondsType__set_state(<IntSecondsType> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_IntSecondsType__set_state(IntSecondsType __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[0])
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_19__pyx_unpickle_JsonType, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_19__pyx_unpickle_TimedeltaType, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_JsonType, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_TimedeltaType, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":1
- * def __pyx_unpickle___BaseDict(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ * def __pyx_unpickle_JsonType(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_21__pyx_unpickle___BaseDict, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_21__pyx_unpickle_JsonType, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle___BaseDict, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_JsonType, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
- *         __pyx_unpickle___BaseDict__set_state(<__BaseDict> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_JsonType__set_state(<JsonType> __pyx_result, __pyx_state)
  *     return __pyx_result
- * cdef __pyx_unpickle___BaseDict__set_state(__BaseDict __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_JsonType__set_state(JsonType __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 0 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[0])
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_23__pyx_unpickle_ConfigParserC, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_23__pyx_unpickle___BaseDict, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ConfigParserC, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle___BaseDict, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":1
- * def __pyx_unpickle_Section(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ * def __pyx_unpickle_ConfigParserC(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_25__pyx_unpickle_Section, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_25__pyx_unpickle_ConfigParserC, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Section, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ConfigParserC, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
- *         __pyx_unpickle_Section__set_state(<Section> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_ConfigParserC__set_state(<ConfigParserC> __pyx_result, __pyx_state)
  *     return __pyx_result
- * cdef __pyx_unpickle_Section__set_state(Section __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result.__type_map = __pyx_state[0]; __pyx_result.config = __pyx_state[1]; __pyx_result.name = __pyx_state[2]
- *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
+ * cdef __pyx_unpickle_ConfigParserC__set_state(ConfigParserC __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.__format_exclude_sections = __pyx_state[0]; __pyx_result.__format_kwargs = __pyx_state[1]; __pyx_result.__sections_map = __pyx_state[2]; __pyx_result.section_defaults = __pyx_state[3]
+ *     if len(__pyx_state) > 4 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_27__pyx_unpickle_AppendSection, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_27__pyx_unpickle_Section, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Section, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_AppendSection(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_13configparserc_6config_29__pyx_unpickle_AppendSection, NULL, __pyx_n_s_configparserc_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_AppendSection, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "configparserc/config.pyx":1
  * # cython: c_string_type=str, c_string_encoding=utf8             # <<<<<<<<<<<<<<
  * """
@@ -30186,28 +31112,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -32065,44 +32991,62 @@
     return -1;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `configparserc-1.3.4/configparserc/config.pyi` & `configparserc-1.4.0/configparserc/config.pyi`

 * *Files identical despite different names*

### Comparing `configparserc-1.3.4/configparserc/include/_config.h` & `configparserc-1.4.0/configparserc/include/_config.h`

 * *Files identical despite different names*

### Comparing `configparserc-1.3.4/configparserc/tools.c` & `configparserc-1.4.0/configparserc/tools.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-g0",
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -225,15 +225,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -264,15 +264,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -6120,28 +6120,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `configparserc-1.3.4/configparserc/tools.pyi` & `configparserc-1.4.0/configparserc/tools.pyi`

 * *Files identical despite different names*

### Comparing `configparserc-1.3.4/configparserc.egg-info/PKG-INFO` & `configparserc-1.4.0/configparserc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configparserc
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python (Cython) based implementation of ConfigParser based on POSIX and stdlib functions.
 Home-page: https://gitlab.com/onegreyonewhite/configparserc
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: Apache Software License
 Project-URL: Issue Tracker, https://gitlab.com/onegreyonewhite/configparserc/-/issues
 Project-URL: Source Code, https://gitlab.com/onegreyonewhite/configparserc.git
@@ -54,14 +54,15 @@
 Support converting values in formats:
 
 *  `StrType` - force convert to string all values (defaults too).
 *  `IntType` - convert values to integer (include suffixes 'K', 'M' and 'G' multiples of 1000).
 *  `BytesSizeType` - convert values to integer size of bytes (include suffixes 'K', 'M' and 'G' multiples of 1024).
 *  `BoolType` - convert 'False', 'false', 'True' and 'true' to valid Python bool type.
 *  `IntSecondsType` - convert time to seconds. Uses 'pytimeparse' python package.
+*  `TimedeltaType` - convert time to timdelta/relativedelta(if installed). Uses 'pytimeparse' python package.
 *  `ListType` - convert separated by symbol (default is comma) string to list of values.
 *  `JsonType` - convert json value to python value.
 
 
 Usage
 -----
```

### Comparing `configparserc-1.3.4/setup.cfg` & `configparserc-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `configparserc-1.3.4/setup.py` & `configparserc-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Compilation block
 ########################################################################################
 import re
 import os
 import sys
+import subprocess
 import fnmatch
 import codecs
 import gzip
-import glob
 import shutil
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-from setuptools import find_packages, setup, Command
+from setuptools import find_packages, setup, errors, Command
 from setuptools.extension import Extension
 from setuptools.command.sdist import sdist as _sdist
 from setuptools.command.build_py import build_py as build_py_orig
 from setuptools.command.install_lib import install_lib as _install_lib
 try:
     from Cython.Build import cythonize, build_ext as _build_ext
 except ImportError:
@@ -186,18 +186,19 @@
                 if not any(filter(lambda fp: bool(fp.search(fext_file)), regex_exclude)):
                     func, subfunc = funcs
                     with codecs.open(fext_file, 'r', encoding='utf-8') as static_file_fd:
                         minified = func(static_file_fd.read(), subfunc)
                     with codecs.open(fext_file, 'w', encoding='utf-8') as static_file_fd:
                         static_file_fd.write(minified)
                     print('Minfied file {fext_file}.'.format(fext_file=fext_file))
-                with open(fext_file, 'rb') as f_in:
-                    with gzip.open("{}.gz".format(fext_file), 'wb') as f_out:
-                        shutil.copyfileobj(f_in, f_out)
-                print('Compressed file {fext_file}.'.format(fext_file=fext_file))
+                if not os.environ.get('NOT_COMPRESS', False):
+                    with open(fext_file, 'rb') as f_in:
+                        with gzip.open("{}.gz".format(fext_file), 'wb') as f_out:
+                            shutil.copyfileobj(f_in, f_out)
+                    print('Compressed file {fext_file}.'.format(fext_file=fext_file))
 
 
 def compile_py_func(fullname, compile_file_func):
     if compile_file_func(fullname, ddir=os.path.dirname(fullname), legacy=True, optimize=0):
         os.remove(fullname)
 
 
@@ -371,20 +372,19 @@
     if has_sphinx and 'build_sphinx' not in cmdclass:
         cmdclass['build_sphinx'] = BuildDoc
     cmdclass['githubrelease'] = GithubRelease
     opts['cmdclass'] = cmdclass
 
     webpack_path = os.path.join(os.getcwd(), 'webpack.config.js')
     if os.path.exists(webpack_path) and is_build and os.environ.get('DONT_YARN', "") != 'true':
-        yarn_build_command = 'devBuild' if is_develop else 'build'
         try:
-            os.system('yarn install --pure-lockfile')
-            os.system('yarn ' + yarn_build_command)
-        except Extension as err:
-            print(err)
+            subprocess.check_call(['yarn', 'install', '--pure-lockfile', '--mutex network'], stdout=sys.stdout, stderr=sys.stderr)
+            subprocess.check_call(['yarn', 'devBuild' if is_develop else 'build'], stdout=sys.stdout, stderr=sys.stderr)
+        except Exception as err:
+            raise errors.CompileError(str(err))
 
     setup(**opts)
 
 ########################################################################################
 # end block
 
 ext_list = [
@@ -396,15 +396,15 @@
     ext_list = []
 
 kwargs = dict(
     name='configparserc',
     packages=find_packages(exclude=['tests']+ext_list),
     ext_modules_list=ext_list,
     install_requires=[
-        'pytimeparse2~=1.6.0',
+        'pytimeparse2~=1.7.1',
         'pyyaml>=3.13,<5.4'
     ],
     project_urls={
         "Issue Tracker": "https://gitlab.com/onegreyonewhite/configparserc/-/issues",
         "Source Code": "https://gitlab.com/onegreyonewhite/configparserc.git",
         "Releases": "https://pypi.org/project/configparserc/#history",
     },
```

