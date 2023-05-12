# Comparing `tmp/archspec-0.2.0.tar.gz` & `tmp/archspec-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archspec-0.2.0.tar", max compression
+gzip compressed data, was "archspec-0.2.1.tar", max compression
```

## Comparing `archspec-0.2.0.tar` & `archspec-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.189003 archspec-0.2.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.189003 archspec-0.2.0/LICENSE-MIT
--rw-r--r--   0        0        0     3104 2022-10-20 07:06:28.800541 archspec-0.2.0/README.md
--rw-r--r--   0        0        0       66 2022-11-16 15:35:23.021770 archspec-0.2.0/archspec/__init__.py
--rwxr-xr-x   0        0        0      544 2021-09-03 15:23:36.193003 archspec-0.2.0/archspec/cli.py
--rw-r--r--   0        0        0      670 2021-09-03 15:23:36.193003 archspec-0.2.0/archspec/cpu/__init__.py
--rw-r--r--   0        0        0     2506 2022-11-16 15:35:23.021770 archspec-0.2.0/archspec/cpu/alias.py
--rw-r--r--   0        0        0    12718 2022-11-16 15:35:23.021770 archspec-0.2.0/archspec/cpu/detect.py
--rw-r--r--   0        0        0    13128 2022-11-16 15:35:23.021770 archspec-0.2.0/archspec/cpu/microarchitecture.py
--rw-r--r--   0        0        0     1899 2022-11-16 15:35:23.021770 archspec-0.2.0/archspec/cpu/schema.py
--rw-r--r--   0        0        0       41 2022-10-20 07:03:47.055484 archspec-0.2.0/archspec/json/.git
--rw-r--r--   0        0        0      558 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/.github/workflows/validation.yml
--rw-r--r--   0        0        0       37 2022-10-09 11:48:17.920223 archspec-0.2.0/archspec/json/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-10-09 11:48:17.920223 archspec-0.2.0/archspec/json/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-10-09 11:48:17.920223 archspec-0.2.0/archspec/json/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-10-09 11:48:17.920223 archspec-0.2.0/archspec/json/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-10-09 11:48:17.920223 archspec-0.2.0/archspec/json/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      805 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/COPYRIGHT
--rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/LICENSE-APACHE
--rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/LICENSE-MIT
--rw-r--r--   0        0        0     1167 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/NOTICE
--rw-r--r--   0        0        0     1386 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/README.md
--rw-r--r--   0        0        0    67871 2022-10-20 11:44:43.351413 archspec-0.2.0/archspec/json/cpu/microarchitectures.json
--rw-r--r--   0        0        0     2955 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/cpu/microarchitectures_schema.json
--rw-r--r--   0        0        0      116 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/bgq-rhel6-power7
--rw-r--r--   0        0        0      534 2021-10-22 10:17:21.472678 archspec-0.2.0/archspec/json/tests/targets/darwin-bigsur-m1
--rw-r--r--   0        0        0      553 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/darwin-mojave-haswell
--rw-r--r--   0        0        0     2356 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/darwin-mojave-ivybridge
--rw-r--r--   0        0        0      598 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/darwin-mojave-skylake
--rw-r--r--   0        0        0     3307 2022-06-06 17:01:35.566636 archspec-0.2.0/archspec/json/tests/targets/darwin-monterey-m1
--rw-r--r--   0        0        0     3307 2022-10-20 11:44:43.351413 archspec-0.2.0/archspec/json/tests/targets/darwin-monterey-m2
--rw-r--r--   0        0        0      221 2022-10-20 07:05:46.605297 archspec-0.2.0/archspec/json/tests/targets/linux-amazon-cortex_a72
--rw-r--r--   0        0        0      276 2022-10-20 07:05:46.605297 archspec-0.2.0/archspec/json/tests/targets/linux-amazon-neoverse_n1
--rw-r--r--   0        0        0      361 2022-10-20 07:05:46.605297 archspec-0.2.0/archspec/json/tests/targets/linux-amazon-neoverse_v1
--rw-r--r--   0        0        0      363 2022-06-06 17:01:35.566636 archspec-0.2.0/archspec/json/tests/targets/linux-asahi-m1
--rw-r--r--   0        0        0      381 2022-10-20 11:44:43.351413 archspec-0.2.0/archspec/json/tests/targets/linux-asahi-m2
--rw-r--r--   0        0        0     1408 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-centos7-cascadelake
--rw-r--r--   0        0        0      111 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-centos7-power8le
--rw-r--r--   0        0        0      238 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-centos7-thunderx2
--rw-r--r--   0        0        0     1411 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-rhel6-piledriver
--rw-r--r--   0        0        0     1187 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-broadwell
--rw-r--r--   0        0        0     1095 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-haswell
--rw-r--r--   0        0        0     1009 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-ivybridge
--rw-r--r--   0        0        0     1286 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-skylake_avx512
--rw-r--r--   0        0        0     1172 2021-10-22 10:17:21.472678 archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-x86_64_v3
--rw-r--r--   0        0        0     1319 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-zen
--rw-r--r--   0        0        0     1111 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-scientific7-k10
--rw-r--r--   0        0        0     1149 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-scientific7-piledriver
--rw-r--r--   0        0        0     1201 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-scientificfermi6-bulldozer
--rw-r--r--   0        0        0     1099 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-scientificfermi6-piledriver
--rw-r--r--   0        0        0      124 2021-10-22 10:17:21.472678 archspec-0.2.0/archspec/json/tests/targets/linux-sifive-u74mc
--rw-r--r--   0        0        0     1190 2021-09-03 15:23:36.888990 archspec-0.2.0/archspec/json/tests/targets/linux-ubuntu18.04-broadwell
--rw-r--r--   0        0        0     1531 2021-10-22 10:17:21.472678 archspec-0.2.0/archspec/json/tests/targets/linux-ubuntu20.04-zen3
--rw-r--r--   0        0        0     1400 2022-11-16 15:35:23.025770 archspec-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 archspec-0.2.0/setup.py
--rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 archspec-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.189003 archspec-0.2.1/LICENSE-APACHE
+-rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.189003 archspec-0.2.1/LICENSE-MIT
+-rw-r--r--   0        0        0     3104 2022-10-20 07:06:28.800541 archspec-0.2.1/README.md
+-rw-r--r--   0        0        0       66 2023-05-12 10:17:38.028075 archspec-0.2.1/archspec/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-12 09:53:22.723465 archspec-0.2.1/archspec/__main__.py
+-rwxr-xr-x   0        0        0     1605 2023-05-12 09:53:22.723465 archspec-0.2.1/archspec/cli.py
+-rw-r--r--   0        0        0      670 2021-09-03 15:23:36.193003 archspec-0.2.1/archspec/cpu/__init__.py
+-rw-r--r--   0        0        0     2506 2022-11-16 15:35:23.021770 archspec-0.2.1/archspec/cpu/alias.py
+-rw-r--r--   0        0        0    12718 2022-11-16 15:35:23.021770 archspec-0.2.1/archspec/cpu/detect.py
+-rw-r--r--   0        0        0    13201 2023-05-12 09:53:22.723465 archspec-0.2.1/archspec/cpu/microarchitecture.py
+-rw-r--r--   0        0        0     1899 2023-04-20 18:20:21.340475 archspec-0.2.1/archspec/cpu/schema.py
+-rw-r--r--   0        0        0       41 2022-10-20 07:03:47.055484 archspec-0.2.1/archspec/json/.git
+-rw-r--r--   0        0        0      558 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/.github/workflows/validation.yml
+-rw-r--r--   0        0        0       37 2022-10-09 11:48:17.920223 archspec-0.2.1/archspec/json/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-10-09 11:48:17.920223 archspec-0.2.1/archspec/json/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-10-09 11:48:17.920223 archspec-0.2.1/archspec/json/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2022-10-09 11:48:17.920223 archspec-0.2.1/archspec/json/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-10-09 11:48:17.920223 archspec-0.2.1/archspec/json/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      805 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/COPYRIGHT
+-rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/LICENSE-APACHE
+-rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/LICENSE-MIT
+-rw-r--r--   0        0        0     1167 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/NOTICE
+-rw-r--r--   0        0        0     1386 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/README.md
+-rw-r--r--   0        0        0    74711 2023-05-12 08:40:43.994331 archspec-0.2.1/archspec/json/cpu/microarchitectures.json
+-rw-r--r--   0        0        0     2955 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/cpu/microarchitectures_schema.json
+-rw-r--r--   0        0        0      116 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/bgq-rhel6-power7
+-rw-r--r--   0        0        0      534 2021-10-22 10:17:21.472678 archspec-0.2.1/archspec/json/tests/targets/darwin-bigsur-m1
+-rw-r--r--   0        0        0      553 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/darwin-mojave-haswell
+-rw-r--r--   0        0        0     2356 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/darwin-mojave-ivybridge
+-rw-r--r--   0        0        0      598 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/darwin-mojave-skylake
+-rw-r--r--   0        0        0     3307 2022-06-06 17:01:35.566636 archspec-0.2.1/archspec/json/tests/targets/darwin-monterey-m1
+-rw-r--r--   0        0        0     3307 2022-10-20 11:44:43.351413 archspec-0.2.1/archspec/json/tests/targets/darwin-monterey-m2
+-rw-r--r--   0        0        0      221 2022-10-20 07:05:46.605297 archspec-0.2.1/archspec/json/tests/targets/linux-amazon-cortex_a72
+-rw-r--r--   0        0        0      276 2022-10-20 07:05:46.605297 archspec-0.2.1/archspec/json/tests/targets/linux-amazon-neoverse_n1
+-rw-r--r--   0        0        0      361 2022-10-20 07:05:46.605297 archspec-0.2.1/archspec/json/tests/targets/linux-amazon-neoverse_v1
+-rw-r--r--   0        0        0      363 2022-06-06 17:01:35.566636 archspec-0.2.1/archspec/json/tests/targets/linux-asahi-m1
+-rw-r--r--   0        0        0      381 2022-10-20 11:44:43.351413 archspec-0.2.1/archspec/json/tests/targets/linux-asahi-m2
+-rw-r--r--   0        0        0     1408 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-centos7-cascadelake
+-rw-r--r--   0        0        0      111 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-centos7-power8le
+-rw-r--r--   0        0        0      238 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-centos7-thunderx2
+-rw-r--r--   0        0        0     1411 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-rhel6-piledriver
+-rw-r--r--   0        0        0     1187 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-broadwell
+-rw-r--r--   0        0        0     1095 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-haswell
+-rw-r--r--   0        0        0     1009 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-ivybridge
+-rw-r--r--   0        0        0     1286 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-skylake_avx512
+-rw-r--r--   0        0        0     1172 2021-10-22 10:17:21.472678 archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-x86_64_v3
+-rw-r--r--   0        0        0     1319 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-zen
+-rw-r--r--   0        0        0      256 2022-12-07 16:19:11.411531 archspec-0.2.1/archspec/json/tests/targets/linux-rocky8-a64fx
+-rw-r--r--   0        0        0     1750 2022-12-19 15:30:17.403229 archspec-0.2.1/archspec/json/tests/targets/linux-rocky8.5-zen4
+-rw-r--r--   0        0        0     1111 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-scientific7-k10
+-rw-r--r--   0        0        0     1149 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-scientific7-piledriver
+-rw-r--r--   0        0        0     1201 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-scientificfermi6-bulldozer
+-rw-r--r--   0        0        0     1099 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-scientificfermi6-piledriver
+-rw-r--r--   0        0        0      124 2021-10-22 10:17:21.472678 archspec-0.2.1/archspec/json/tests/targets/linux-sifive-u74mc
+-rw-r--r--   0        0        0     1190 2021-09-03 15:23:36.888990 archspec-0.2.1/archspec/json/tests/targets/linux-ubuntu18.04-broadwell
+-rw-r--r--   0        0        0     1531 2021-10-22 10:17:21.472678 archspec-0.2.1/archspec/json/tests/targets/linux-ubuntu20.04-zen3
+-rw-r--r--   0        0        0     1387 2023-05-12 10:17:38.028075 archspec-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 archspec-0.2.1/PKG-INFO
```

### Comparing `archspec-0.2.0/LICENSE-APACHE` & `archspec-0.2.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/LICENSE-MIT` & `archspec-0.2.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/README.md` & `archspec-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/cpu/__init__.py` & `archspec-0.2.1/archspec/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/cpu/alias.py` & `archspec-0.2.1/archspec/cpu/alias.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/cpu/detect.py` & `archspec-0.2.1/archspec/cpu/detect.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/cpu/microarchitecture.py` & `archspec-0.2.1/archspec/cpu/microarchitecture.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,23 +264,22 @@
                 if warning_message:
                     warnings.warn(warning_message)
 
                 flags = flags_fmt.format(**compiler_entry)
                 return flags
 
         msg = (
-            "cannot produce optimized binary for micro-architecture '{0}'"
-            " with {1}@{2} [supported compiler versions are {3}]"
-        )
-        msg = msg.format(
-            self.name,
-            compiler,
-            version,
-            ", ".join([x["versions"] for x in compiler_info]),
+            "cannot produce optimized binary for micro-architecture '{0}' with {1}@{2}"
         )
+        if compiler_info:
+            versions = [x["versions"] for x in compiler_info]
+            msg += f' [supported compiler versions are {", ".join(versions)}]'
+        else:
+            msg += " [no supported compiler versions]"
+        msg = msg.format(self.name, compiler, version)
         raise UnsupportedMicroarchitecture(msg)
 
 
 def generic_microarchitecture(name):
     """Returns a generic micro-architecture with no vendor and no features.
 
     Args:
```

### Comparing `archspec-0.2.0/archspec/cpu/schema.py` & `archspec-0.2.1/archspec/cpu/schema.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/.github/workflows/validation.yml` & `archspec-0.2.1/archspec/json/.github/workflows/validation.yml`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/COPYRIGHT` & `archspec-0.2.1/archspec/json/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/LICENSE-APACHE` & `archspec-0.2.1/archspec/json/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/LICENSE-MIT` & `archspec-0.2.1/archspec/json/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/NOTICE` & `archspec-0.2.1/archspec/json/NOTICE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/README.md` & `archspec-0.2.1/archspec/json/README.md`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/cpu/microarchitectures.json` & `archspec-0.2.1/archspec/json/cpu/microarchitectures.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963041485665184%*

 * *Differences: {"'microarchitectures'": "{'x86_64': {'compilers': {'nvhpc': []}}, 'x86_64_v2': {'compilers': "*

 * *                         "{'nvhpc': []}}, 'x86_64_v3': {'compilers': {'nvhpc': "*

 * *                         "[OrderedDict([('versions', ':'), ('name', 'px'), ('flags', '-tp {name} "*

 * *                         '-mpopcnt -msse3 -msse4.1 -msse4.2 -mssse3 -mavx -mavx2 -mbmi -mbmi2 '*

 * *                         "-mf16c -mfma -mlzcnt -mxsave')])]}}, 'x86_64_v4': {'compilers': "*

 * *                         "{'nvhpc': [OrderedDict […]*

```diff
@@ -135,15 +135,14 @@
                     }
                 ]
             },
             "features": [
                 "fp",
                 "asimd",
                 "evtstrm",
-                "pmull",
                 "sha1",
                 "sha2",
                 "crc32",
                 "atomics",
                 "cpuid",
                 "asimdrdm",
                 "fphp",
@@ -178,15 +177,16 @@
                     }
                 ],
                 "gcc": [
                     {
                         "flags": "-march=armv8-a -mtune=generic",
                         "versions": "4.8.0:"
                     }
-                ]
+                ],
+                "nvhpc": []
             },
             "features": [],
             "from": [],
             "vendor": "generic"
         },
         "arm": {
             "compilers": {
@@ -401,14 +401,21 @@
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "haswell",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -471,14 +478,20 @@
                 "intel": [
                     {
                         "flags": "-msse3",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-msse3",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ]
@@ -538,14 +551,21 @@
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "skylake",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -620,14 +640,21 @@
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "19.0.1:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "skylake",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -701,14 +728,15 @@
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "16.0:"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -797,14 +825,21 @@
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "piledriver",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
@@ -884,14 +919,20 @@
                         "versions": "16.0:17.9.0"
                     },
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -975,14 +1016,21 @@
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "icelake-client",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "skylake",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "icelake-client",
                         "versions": ":"
                     }
                 ]
@@ -1078,14 +1126,20 @@
                         "versions": "16.0:17.9.0"
                     },
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -1141,14 +1195,15 @@
                 "intel": [
                     {
                         "flags": "-msse2",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-msse2",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ]
@@ -1240,26 +1295,34 @@
             "compilers": {
                 "apple-clang": [
                     {
                         "flags": "-march=armv8.5-a",
                         "versions": "11.0:12.5"
                     },
                     {
-                        "flags": "-mcpu=vortex",
-                        "versions": "13.0:"
+                        "flags": "-mcpu=apple-m1",
+                        "versions": "13.0:14.0.2"
+                    },
+                    {
+                        "flags": "-mcpu=apple-m2",
+                        "versions": "14.0.2:"
                     }
                 ],
                 "clang": [
                     {
                         "flags": "-march=armv8.5-a",
                         "versions": "9.0:12.0"
                     },
                     {
                         "flags": "-mcpu=apple-m1",
                         "versions": "13.0:"
+                    },
+                    {
+                        "flags": "-mcpu=apple-m2",
+                        "versions": "16.0:"
                     }
                 ],
                 "gcc": [
                     {
                         "flags": "-march=armv8.5-a -mtune=generic",
                         "versions": "8.0:"
                     }
@@ -1331,36 +1394,36 @@
                         "versions": "3.9:"
                     }
                 ],
                 "dpcpp": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "knl",
-                        "versions": ":"
+                        "versions": ":2021.2"
                     }
                 ],
                 "gcc": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "knl",
                         "versions": "5.1:"
                     }
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "knl",
-                        "versions": "18.0:"
+                        "versions": "18.0:2021.2"
                     }
                 ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "knl",
-                        "versions": ":"
+                        "versions": ":2021.2"
                     }
                 ]
             },
             "features": [
                 "mmx",
                 "sse",
                 "sse2",
@@ -1432,14 +1495,15 @@
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "corei7",
                         "versions": "16.0:"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "corei7",
                         "versions": ":"
                     }
                 ]
@@ -1506,14 +1570,21 @@
                         "flags": "-march=armv8.2-a+fp16+rcpc+dotprod+crypto -mtune=cortex-a72",
                         "versions": "8.1:8.9"
                     },
                     {
                         "flags": "-mcpu=neoverse-n1",
                         "versions": "9.0:"
                     }
+                ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "neoverse-n1",
+                        "versions": "22.5:"
+                    }
                 ]
             },
             "features": [
                 "fp",
                 "asimd",
                 "evtstrm",
                 "aes",
@@ -1582,23 +1653,46 @@
                     },
                     {
                         "flags": "-march=armv8.2-a+crypto+fp16 -mtune=cortex-a72",
                         "versions": "7:7.9"
                     },
                     {
                         "flags": "-march=armv8.2-a+fp16+dotprod+crypto -mtune=cortex-a72",
-                        "versions": "8.0:8.9"
+                        "versions": "8.0:8.4"
+                    },
+                    {
+                        "flags": "-mcpu=neoverse-v1",
+                        "versions": "8.5:8.9"
+                    },
+                    {
+                        "flags": "-march=armv8.2-a+fp16+dotprod+crypto -mtune=cortex-a72",
+                        "versions": "9.0:9.3"
                     },
                     {
                         "flags": "-mcpu=neoverse-v1",
-                        "versions": "9.0:9.9"
+                        "versions": "9.4:9.9"
+                    },
+                    {
+                        "flags": "-march=armv8.2-a+fp16+dotprod+crypto -mtune=cortex-a72",
+                        "versions": "10.0:10.1"
+                    },
+                    {
+                        "flags": "-mcpu=zeus",
+                        "versions": "10.2"
                     },
                     {
                         "flags": "-mcpu=neoverse-v1",
-                        "versions": "10.0:"
+                        "versions": "10.3:"
+                    }
+                ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "neoverse-n1",
+                        "versions": "22.5:"
                     }
                 ]
             },
             "features": [
                 "fp",
                 "asimd",
                 "evtstrm",
@@ -1678,14 +1772,15 @@
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "16.0:"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -1763,14 +1858,20 @@
                 "intel": [
                     {
                         "flags": "-msse3",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-msse3",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ]
@@ -1867,14 +1968,21 @@
                     },
                     {
                         "flags": "-mcpu={name} -mtune={name}",
                         "name": "power8",
                         "versions": "4.8:4.8.5",
                         "warnings": "Using GCC 4.8 to optimize for Power 8 might not work if you are not on Red Hat Enterprise Linux 7, where a custom backport of the feature has been done. Upstream support from GCC starts in version 4.9"
                     }
+                ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "pwr8",
+                        "versions": ":"
+                    }
                 ]
             },
             "features": [],
             "from": [
                 "ppc64le"
             ],
             "generation": 8,
@@ -1914,14 +2022,21 @@
                 ],
                 "gcc": [
                     {
                         "flags": "-mcpu={name} -mtune={name}",
                         "name": "power9",
                         "versions": "6.0:"
                     }
+                ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "pwr9",
+                        "versions": ":"
+                    }
                 ]
             },
             "features": [],
             "from": [
                 "power8le"
             ],
             "generation": 9,
@@ -1963,15 +2078,16 @@
                 ],
                 "gcc": [
                     {
                         "flags": "-mcpu={name} -mtune={name}",
                         "name": "powerpc64le",
                         "versions": "4.8:"
                     }
-                ]
+                ],
+                "nvhpc": []
             },
             "features": [],
             "from": [],
             "vendor": "generic"
         },
         "ppcle": {
             "compilers": {},
@@ -2054,14 +2170,20 @@
                         "versions": "16.0:17.9.0"
                     },
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -2116,14 +2238,21 @@
                 ],
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "haswell",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "versions": ":"
                     }
                 ]
             },
@@ -2195,14 +2324,21 @@
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "skylake-avx512",
                         "versions": "18.0:"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "skylake",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "skylake-avx512",
                         "versions": ":"
                     }
                 ]
@@ -2288,14 +2424,21 @@
                 "intel": [
                     {
                         "flags": "-msse4.2",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "piledriver",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-msse4.2",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ]
@@ -2432,14 +2575,15 @@
                 "intel": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "corei7",
                         "versions": "16.0:"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "corei7",
                         "versions": ":"
                     }
                 ]
@@ -2510,14 +2654,15 @@
                 "intel": [
                     {
                         "flags": "-march={name} -mtune=generic",
                         "name": "pentium4",
                         "versions": ":"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune=generic",
                         "name": "x86-64",
                         "versions": ":"
                     }
                 ]
@@ -2555,14 +2700,15 @@
                     },
                     {
                         "flags": "-march={name} -mtune=generic -mcx16 -msahf -mpopcnt -msse3 -msse4.1 -msse4.2 -mssse3",
                         "name": "x86-64",
                         "versions": "4.6:11.0"
                     }
                 ],
+                "nvhpc": [],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune=generic",
                         "name": "x86-64-v2",
                         "versions": "2021.2.0:"
                     }
                 ]
@@ -2619,14 +2765,21 @@
                     },
                     {
                         "flags": "-march={name} -mtune=generic -mcx16 -msahf -mpopcnt -msse3 -msse4.1 -msse4.2 -mssse3 -mavx -mavx2 -mbmi -mbmi2 -mf16c -mfma -mlzcnt -mmovbe -mxsave",
                         "name": "x86-64",
                         "versions": "4.8:11.0"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name} -mpopcnt -msse3 -msse4.1 -msse4.2 -mssse3 -mavx -mavx2 -mbmi -mbmi2 -mf16c -mfma -mlzcnt -mxsave",
+                        "name": "px",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune=generic",
                         "name": "x86-64-v3",
                         "versions": "2021.2.0:"
                     }
                 ]
@@ -2692,14 +2845,21 @@
                     },
                     {
                         "flags": "-march={name} -mtune=generic -mcx16 -msahf -mpopcnt -msse3 -msse4.1 -msse4.2 -mssse3 -mavx -mavx2 -mbmi -mbmi2 -mf16c -mfma -mlzcnt -mmovbe -mxsave -mavx512f -mavx512bw -mavx512cd -mavx512dq -mavx512vl",
                         "name": "x86-64",
                         "versions": "6.0:11.0"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name} -mpopcnt -msse3 -msse4.1 -msse4.2 -mssse3 -mavx -mavx2 -mbmi -mbmi2 -mf16c -mfma -mlzcnt -mxsave -mavx512f -mavx512bw -mavx512cd -mavx512dq -mavx512vl",
+                        "name": "px",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune=generic",
                         "name": "x86-64-v4",
                         "versions": "2021.2.0:"
                     }
                 ]
@@ -2769,14 +2929,20 @@
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": ":"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
@@ -2849,14 +3015,20 @@
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": "20.5:"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
@@ -2930,14 +3102,20 @@
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": "16.0:",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
                 ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "versions": "21.11:"
+                    }
+                ],
                 "oneapi": [
                     {
                         "flags": "-march={name} -mtune={name}",
                         "name": "core-avx2",
                         "versions": ":",
                         "warnings": "Intel's compilers may or may not optimize to the same degree for non-Intel microprocessors for optimizations that are not unique to Intel microprocessors"
                     }
@@ -2974,10 +3152,111 @@
                 "vpclmulqdq",
                 "pku"
             ],
             "from": [
                 "zen2"
             ],
             "vendor": "AuthenticAMD"
+        },
+        "zen4": {
+            "compilers": {
+                "aocc": [
+                    {
+                        "flags": "-march={name} -mtune={name} -mavx512f -mavx512dq -mavx512ifma -mavx512cd -mavx512bw -mavx512vl -mavx512vbmi -mavx512vbmi2 -mavx512vnni -mavx512bitalg",
+                        "name": "znver3",
+                        "versions": "3.0:3.9",
+                        "warnings": "Zen4 processors are not fully supported by AOCC versions < 4.0.  For optimal performance please upgrade to a newer version of AOCC"
+                    },
+                    {
+                        "flags": "-march={name} -mtune={name}",
+                        "name": "znver4",
+                        "versions": "4.0:"
+                    }
+                ],
+                "clang": [
+                    {
+                        "flags": "-march={name} -mtune={name} -mavx512f -mavx512dq -mavx512ifma -mavx512cd -mavx512bw -mavx512vl -mavx512vbmi -mavx512vbmi2 -mavx512vnni -mavx512bitalg",
+                        "name": "znver3",
+                        "versions": "12.0:15.9"
+                    },
+                    {
+                        "flags": "-march={name} -mtune={name}",
+                        "name": "znver4",
+                        "versions": "16.0:"
+                    }
+                ],
+                "gcc": [
+                    {
+                        "flags": "-march={name} -mtune={name} -mavx512f -mavx512dq -mavx512ifma -mavx512cd -mavx512bw -mavx512vl -mavx512vbmi -mavx512vbmi2 -mavx512vnni -mavx512bitalg",
+                        "name": "znver3",
+                        "versions": "10.3:13.0"
+                    },
+                    {
+                        "flags": "-march={name} -mtune={name}",
+                        "name": "znver4",
+                        "versions": "13.1:"
+                    }
+                ],
+                "nvhpc": [
+                    {
+                        "flags": "-tp {name}",
+                        "name": "zen3",
+                        "versions": "21.11:",
+                        "warnings": "zen4 is not fully supported by nvhpc yet, falling back to zen3"
+                    }
+                ]
+            },
+            "features": [
+                "bmi1",
+                "bmi2",
+                "f16c",
+                "fma",
+                "fsgsbase",
+                "avx",
+                "avx2",
+                "rdseed",
+                "clzero",
+                "aes",
+                "pclmulqdq",
+                "cx16",
+                "movbe",
+                "mmx",
+                "sse",
+                "sse2",
+                "sse4a",
+                "ssse3",
+                "sse4_1",
+                "sse4_2",
+                "abm",
+                "xsavec",
+                "xsaveopt",
+                "clflushopt",
+                "popcnt",
+                "clwb",
+                "vaes",
+                "vpclmulqdq",
+                "pku",
+                "gfni",
+                "flush_l1d",
+                "erms",
+                "avic",
+                "avx512f",
+                "avx512dq",
+                "avx512ifma",
+                "avx512cd",
+                "avx512bw",
+                "avx512vl",
+                "avx512_bf16",
+                "avx512vbmi",
+                "avx512_vbmi2",
+                "avx512_vnni",
+                "avx512_bitalg",
+                "avx512_vpopcntdq"
+            ],
+            "from": [
+                "zen3",
+                "x86_64_v4"
+            ],
+            "vendor": "AuthenticAMD"
         }
     }
 }
```

### Comparing `archspec-0.2.0/archspec/json/cpu/microarchitectures_schema.json` & `archspec-0.2.1/archspec/json/cpu/microarchitectures_schema.json`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/darwin-bigsur-m1` & `archspec-0.2.1/archspec/json/tests/targets/darwin-bigsur-m1`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/darwin-mojave-haswell` & `archspec-0.2.1/archspec/json/tests/targets/darwin-mojave-haswell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/darwin-mojave-ivybridge` & `archspec-0.2.1/archspec/json/tests/targets/darwin-mojave-ivybridge`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/darwin-mojave-skylake` & `archspec-0.2.1/archspec/json/tests/targets/darwin-mojave-skylake`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/darwin-monterey-m1` & `archspec-0.2.1/archspec/json/tests/targets/darwin-monterey-m1`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/darwin-monterey-m2` & `archspec-0.2.1/archspec/json/tests/targets/darwin-monterey-m2`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-centos7-cascadelake` & `archspec-0.2.1/archspec/json/tests/targets/linux-centos7-cascadelake`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel6-piledriver` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel6-piledriver`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-broadwell` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-broadwell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-haswell` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-haswell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-ivybridge` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-ivybridge`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-skylake_avx512` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-skylake_avx512`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-x86_64_v3` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-x86_64_v3`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-rhel7-zen` & `archspec-0.2.1/archspec/json/tests/targets/linux-rhel7-zen`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-scientific7-k10` & `archspec-0.2.1/archspec/json/tests/targets/linux-scientific7-k10`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-scientific7-piledriver` & `archspec-0.2.1/archspec/json/tests/targets/linux-scientific7-piledriver`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-scientificfermi6-bulldozer` & `archspec-0.2.1/archspec/json/tests/targets/linux-scientificfermi6-bulldozer`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-scientificfermi6-piledriver` & `archspec-0.2.1/archspec/json/tests/targets/linux-scientificfermi6-piledriver`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-ubuntu18.04-broadwell` & `archspec-0.2.1/archspec/json/tests/targets/linux-ubuntu18.04-broadwell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/archspec/json/tests/targets/linux-ubuntu20.04-zen3` & `archspec-0.2.1/archspec/json/tests/targets/linux-ubuntu20.04-zen3`

 * *Files identical despite different names*

### Comparing `archspec-0.2.0/pyproject.toml` & `archspec-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archspec"
-version = "0.2.0"
+version = "0.2.1"
 description = "A library to query system architecture"
 license = "Apache-2.0 OR MIT"
 authors = ["archspec developers <maintainers@spack.io>"]
 maintainers = [
     "Greg Becker <maintainers@spack.io>",
     "Massimiliano Culpo <massimiliano.culpo@gmail.com>",
     "Todd Gamblin <maintainers@spack.io>",
@@ -22,15 +22,14 @@
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Unix"
 ]
 
 [tool.poetry.dependencies]
 python = "3.6.15 || ^3.7"
-click = "^8"
 
 [tool.poetry.dev-dependencies]
 pytest = { version = "^7", python = "^3.7" }
 pytest-cov = { version = "^4", python = "^3.7" }
 jsonschema = { version = "^4", python = "^3.7" }
 pylint = { version = "^2", python = "^3.7" }
 flake8 = { version = "^5", python = "^3.7" }
```

### Comparing `archspec-0.2.0/PKG-INFO` & `archspec-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archspec
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library to query system architecture
 Home-page: https://github.com/archspec/archspec
 License: Apache-2.0 OR MIT
 Author: archspec developers
 Author-email: maintainers@spack.io
 Maintainer: Greg Becker
 Maintainer-email: maintainers@spack.io
@@ -19,15 +19,14 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8,<9)
 Project-URL: Documentation, https://archspec.readthedocs.io
 Project-URL: Repository, https://github.com/archspec/archspec.git
 Description-Content-Type: text/markdown
 
 # Archspec (Python bindings)
 
 [![CI](https://github.com/archspec/archspec/workflows/Unit%20tests/badge.svg)](https://github.com/archspec/archspec/actions)
```

