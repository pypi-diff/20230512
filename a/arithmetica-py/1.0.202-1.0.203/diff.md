# Comparing `tmp/arithmetica-py-1.0.202.tar.gz` & `tmp/arithmetica-py-1.0.203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.202.tar", last modified: Wed May 10 17:01:41 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.203.tar", last modified: Fri May 12 20:28:51 2023, max compression
```

## Comparing `arithmetica-py-1.0.202.tar` & `arithmetica-py-1.0.203.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 17:01:41.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:41.117672 arithmetica-py-1.0.202/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   183374 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-10 17:01:25.000000 arithmetica-py-1.0.202/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 17:01:40.000000 arithmetica-py-1.0.202/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.158313 arithmetica-py-1.0.203/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   184894 2023-05-12 20:28:50.000000 arithmetica-py-1.0.203/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-12 20:28:50.000000 arithmetica-py-1.0.203/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 20:28:50.000000 arithmetica-py-1.0.203/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.202/LICENSE` & `arithmetica-py-1.0.203/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.202/README.md` & `arithmetica-py-1.0.203/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.202/setup.py` & `arithmetica-py-1.0.203/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.202/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.203/src/python-module/libarithmetica.a`

 * *Files 4% similar despite different names*

#### nm -s {}

```diff
@@ -51,14 +51,15 @@
 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ in Fraction.cpp.o
 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE in Fraction.cpp.o
 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE in Fraction.cpp.o
 _ZN11arithmetica8FractionC2EPKc in Fraction.cpp.o
 _ZN11arithmetica8FractionC1EPKc in Fraction.cpp.o
 _ZN11arithmetica8FractionC2ERK8fraction in Fraction.cpp.o
 _ZN11arithmetica8FractionC1ERK8fraction in Fraction.cpp.o
+_ZN11arithmetica8Fraction9to_stringB5cxx11Ev in Fraction.cpp.o
 _ZN11arithmetica8FractionD2Ev in Fraction.cpp.o
 _ZN11arithmetica8FractionD1Ev in Fraction.cpp.o
 _ZN11arithmetica8FractionplERKS0_ in Fraction.cpp.o
 _ZN11arithmetica8FractionmiERKS0_ in Fraction.cpp.o
 _ZN11arithmetica8FractionmlERKS0_ in Fraction.cpp.o
 _ZN11arithmetica8FractiondvERKS0_ in Fraction.cpp.o
 _ZN11arithmetica8FractioneqERKS0_ in Fraction.cpp.o
@@ -513,19 +514,23 @@
                  U malloc
                  U memcpy
                  U memmove
                  U strlen
 0000000000000000 T terminating_decimal_to_fraction
 
 Fraction.cpp.o:
-0000000000000003 r .LC10
+0000000000000017 r .LC12
+000000000000001a r .LC13
 0000000000000000 r .LC4
-0000000000000000 r .LC9
+0000000000000000 r .LC5
+0000000000000015 r .LC6
 0000000000000000 V DW.ref.__gxx_personality_v0
                  U _Unwind_Resume
+00000000000002a0 T _ZN11arithmetica8Fraction9to_stringB5cxx11Ev
+00000000000000d0 t _ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
 0000000000000150 T _ZN11arithmetica8FractionC1EPKc
 0000000000000200 T _ZN11arithmetica8FractionC1ERK8fraction
 00000000000000a0 T _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
 0000000000000030 T _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
 0000000000000000 T _ZN11arithmetica8FractionC1Ev
 0000000000000150 T _ZN11arithmetica8FractionC2EPKc
 0000000000000068 t _ZN11arithmetica8FractionC2EPKc.cold
@@ -535,32 +540,34 @@
 0000000000000034 t _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 0000000000000030 T _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
 0000000000000000 t _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_.cold
 0000000000000000 T _ZN11arithmetica8FractionC2Ev
 0000000000000000 W _ZN11arithmetica8FractionD1Ev
 0000000000000000 W _ZN11arithmetica8FractionD2Ev
 0000000000000000 n _ZN11arithmetica8FractionD5Ev
-0000000000000bd0 T _ZN11arithmetica8FractiondvERKS0_
-000000000000019c t _ZN11arithmetica8FractiondvERKS0_.cold
-0000000000000ee0 T _ZN11arithmetica8FractioneqERKS0_
-00000000000005b0 T _ZN11arithmetica8FractionmiERKS0_
-0000000000000114 t _ZN11arithmetica8FractionmiERKS0_.cold
-00000000000008c0 T _ZN11arithmetica8FractionmlERKS0_
-0000000000000158 t _ZN11arithmetica8FractionmlERKS0_.cold
-00000000000002a0 T _ZN11arithmetica8FractionplERKS0_
-00000000000000d0 t _ZN11arithmetica8FractionplERKS0_.cold
+0000000000000da0 T _ZN11arithmetica8FractiondvERKS0_
+00000000000001bc t _ZN11arithmetica8FractiondvERKS0_.cold
+00000000000010b0 T _ZN11arithmetica8FractioneqERKS0_
+0000000000000780 T _ZN11arithmetica8FractionmiERKS0_
+0000000000000134 t _ZN11arithmetica8FractionmiERKS0_.cold
+0000000000000a90 T _ZN11arithmetica8FractionmlERKS0_
+0000000000000178 t _ZN11arithmetica8FractionmlERKS0_.cold
+0000000000000470 T _ZN11arithmetica8FractionplERKS0_
+00000000000000f0 t _ZN11arithmetica8FractionplERKS0_.cold
                  U _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
+                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
                  U _ZSt19__throw_logic_errorPKc
+                 U _ZSt20__throw_length_errorPKc
                  U _ZdlPvm
-0000000000000fb0 T _ZeqRKN11arithmetica8FractionES2_
-0000000000001080 T _ZltRKN11arithmetica8FractionES2_
-00000000000001e0 t _ZltRKN11arithmetica8FractionES2_.cold
+0000000000001180 T _ZeqRKN11arithmetica8FractionES2_
+0000000000001250 T _ZltRKN11arithmetica8FractionES2_
+0000000000000200 t _ZltRKN11arithmetica8FractionES2_.cold
                  U __gxx_personality_v0
                  U __stack_chk_fail
                  U add_fraction
                  U calloc
                  U delete_fraction
                  U memcmp
                  U memcpy
```

#### file list

```diff
@@ -1,8 +1,8 @@
-----------   0        0        0     3696 1970-01-01 00:00:00.000000 /
+----------   0        0        0     3744 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0    22216 1970-01-01 00:00:00.000000 arithmetica.cpp.o
 ?rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 arccos.c.o
 ?rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 arcsin.c.o
 ?rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 arctan.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 check_accuracy.c.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 continued_fraction_to_fraction.c.o
@@ -18,15 +18,15 @@
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18192 1970-01-01 00:00:00.000000 simplify_arithmetic_expression.c.o
 ?rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 sine.c.o
 ?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 square_root.c.o
 ?rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 tangent.c.o
 ?rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
-?rw-r--r--   0        0        0    18288 1970-01-01 00:00:00.000000 Fraction.cpp.o
+?rw-r--r--   0        0        0    19760 1970-01-01 00:00:00.000000 Fraction.cpp.o
 ?rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 fraction.c.o
 ?rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 add_fraction.c.o
 ?rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 multiply_fraction.c.o
 ?rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 parse_fraction.c.o
 ?rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 power_fraction.c.o
 ?rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 simplify_parsed_fraction.c.o
 ?rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 subtract_fraction.c.o
```

#### Fraction.cpp.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          16752 (bytes into file)
+  Start of section headers:          18224 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         24
   Section header string table index: 23
```

##### readelf --wide --sections {}

```diff
@@ -1,33 +1,33 @@
-There are 24 section headers, starting at offset 0x4170:
+There are 24 section headers, starting at offset 0x4730:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .group            GROUP           0000000000000000 000040 00000c 04     21  18  4
-  [ 2] .group            GROUP           0000000000000000 00004c 00000c 04     21  22  4
-  [ 3] .text             PROGBITS        0000000000000000 000060 0012ff 00  AX  0   0 16
-  [ 4] .rela.text        RELA            0000000000000000 002948 000ff0 18   I 21   3  8
-  [ 5] .data             PROGBITS        0000000000000000 00135f 000000 00  WA  0   0  1
-  [ 6] .bss              NOBITS          0000000000000000 00135f 000000 00  WA  0   0  1
-  [ 7] .text.unlikely    PROGBITS        0000000000000000 001360 000210 00  AX  0   0  2
-  [ 8] .rela.text.unlikely RELA            0000000000000000 003938 000300 18   I 21   7  8
-  [ 9] .gcc_except_table PROGBITS        0000000000000000 001570 000137 00   A  0   0  1
-  [10] .text._ZN11arithmetica8FractionD2Ev PROGBITS        0000000000000000 0016b0 000042 00 AXG  0   0 16
-  [11] .rela.text._ZN11arithmetica8FractionD2Ev RELA            0000000000000000 003c38 000030 18  IG 21  10  8
-  [12] .rodata.str1.8    PROGBITS        0000000000000000 0016f8 00002a 01 AMS  0   0  8
-  [13] .rodata.str1.1    PROGBITS        0000000000000000 001722 000005 01 AMS  0   0  1
-  [14] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 001728 000008 00 WAG  0   0  8
-  [15] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 003c68 000018 18  IG 21  14  8
-  [16] .comment          PROGBITS        0000000000000000 001730 00002c 01  MS  0   0  1
-  [17] .note.GNU-stack   PROGBITS        0000000000000000 00175c 000000 00      0   0  1
-  [18] .note.gnu.property NOTE            0000000000000000 001760 000020 00   A  0   0  8
-  [19] .eh_frame         PROGBITS        0000000000000000 001780 000520 00   A  0   0  8
-  [20] .rela.eh_frame    RELA            0000000000000000 003c80 0003d8 18   I 21  19  8
-  [21] .symtab           SYMTAB          0000000000000000 001ca0 000570 18     22  19  8
-  [22] .strtab           STRTAB          0000000000000000 002210 000736 00      0   0  1
-  [23] .shstrtab         STRTAB          0000000000000000 004058 000111 00      0   0  1
+  [ 1] .group            GROUP           0000000000000000 000040 00000c 04     21  21  4
+  [ 2] .group            GROUP           0000000000000000 00004c 00000c 04     21  25  4
+  [ 3] .text             PROGBITS        0000000000000000 000060 0014cf 00  AX  0   0 16
+  [ 4] .rela.text        RELA            0000000000000000 002d40 001128 18   I 21   3  8
+  [ 5] .data             PROGBITS        0000000000000000 00152f 000000 00  WA  0   0  1
+  [ 6] .bss              NOBITS          0000000000000000 00152f 000000 00  WA  0   0  1
+  [ 7] .text.unlikely    PROGBITS        0000000000000000 001530 000230 00  AX  0   0  2
+  [ 8] .rela.text.unlikely RELA            0000000000000000 003e68 000330 18   I 21   7  8
+  [ 9] .gcc_except_table PROGBITS        0000000000000000 001760 00015a 00   A  0   0  1
+  [10] .rodata.str1.8    PROGBITS        0000000000000000 0018c0 00002a 01 AMS  0   0  8
+  [11] .rodata.str1.1    PROGBITS        0000000000000000 0018ea 00001c 01 AMS  0   0  1
+  [12] .text._ZN11arithmetica8FractionD2Ev PROGBITS        0000000000000000 001910 000042 00 AXG  0   0 16
+  [13] .rela.text._ZN11arithmetica8FractionD2Ev RELA            0000000000000000 004198 000030 18  IG 21  12  8
+  [14] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 001958 000008 00 WAG  0   0  8
+  [15] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 0041c8 000018 18  IG 21  14  8
+  [16] .comment          PROGBITS        0000000000000000 001960 00002c 01  MS  0   0  1
+  [17] .note.GNU-stack   PROGBITS        0000000000000000 00198c 000000 00      0   0  1
+  [18] .note.gnu.property NOTE            0000000000000000 001990 000020 00   A  0   0  8
+  [19] .eh_frame         PROGBITS        0000000000000000 0019b0 000588 00   A  0   0  8
+  [20] .rela.eh_frame    RELA            0000000000000000 0041e0 000438 18   I 21  19  8
+  [21] .symtab           SYMTAB          0000000000000000 001f38 000600 18     22  22  8
+  [22] .strtab           STRTAB          0000000000000000 002538 000803 00      0   0  1
+  [23] .shstrtab         STRTAB          0000000000000000 004618 000111 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,61 +1,67 @@
 
-Symbol table '.symtab' contains 58 entries:
+Symbol table '.symtab' contains 64 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS Fraction.cpp
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    3 .text
      3: 0000000000000000     0 SECTION LOCAL  DEFAULT    7 .text.unlikely
      4: 0000000000000000     0 SECTION LOCAL  DEFAULT    9 .gcc_except_table
      5: 0000000000000000    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_.cold
      6: 0000000000000034    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
      7: 0000000000000068    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2EPKc.cold
      8: 000000000000009c    51 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionC2ERK8fraction.cold
-     9: 0000000000000000     0 SECTION LOCAL  DEFAULT   10 .text._ZN11arithmetica8FractionD2Ev
-    10: 00000000000000d0    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionplERKS0_.cold
-    11: 0000000000000114    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmiERKS0_.cold
-    12: 0000000000000158    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmlERKS0_.cold
-    13: 000000000000019c    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractiondvERKS0_.cold
-    14: 00000000000001e0    48 FUNC    LOCAL  DEFAULT    7 _ZltRKN11arithmetica8FractionES2_.cold
-    15: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   12 .LC4
-    16: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   13 .LC9
-    17: 0000000000000003     0 NOTYPE  LOCAL  DEFAULT   13 .LC10
-    18: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    1 _ZN11arithmetica8FractionD5Ev
-    19: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2Ev
-    20: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1Ev
-    21: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
-    22: 0000000000000000     8 OBJECT  WEAK   HIDDEN    14 DW.ref.__gxx_personality_v0
-    23: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
-    24: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __gxx_personality_v0
-    25: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZdlPvm
-    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Unwind_Resume
-    27: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
-    28: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-    29: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
-    30: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
-    31: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
-    32: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
-    33: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-    34: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2EPKc
-    35: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1EPKc
-    36: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERK8fraction
-    37: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERK8fraction
-    38: 0000000000000000    66 FUNC    WEAK   DEFAULT   10 _ZN11arithmetica8FractionD2Ev
-    39: 0000000000000000    66 FUNC    WEAK   DEFAULT   10 _ZN11arithmetica8FractionD1Ev
-    40: 00000000000002a0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionplERKS0_
-    41: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
-    42: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcpy
-    43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add_fraction
-    44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt19__throw_logic_errorPKc
-    45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
-    46: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
+     9: 00000000000000d0    32 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
+    10: 0000000000000000     0 SECTION LOCAL  DEFAULT   12 .text._ZN11arithmetica8FractionD2Ev
+    11: 00000000000000f0    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionplERKS0_.cold
+    12: 0000000000000134    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmiERKS0_.cold
+    13: 0000000000000178    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractionmlERKS0_.cold
+    14: 00000000000001bc    68 FUNC    LOCAL  DEFAULT    7 _ZN11arithmetica8FractiondvERKS0_.cold
+    15: 0000000000000200    48 FUNC    LOCAL  DEFAULT    7 _ZltRKN11arithmetica8FractionES2_.cold
+    16: 0000000000000015     0 NOTYPE  LOCAL  DEFAULT   11 .LC6
+    17: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   10 .LC4
+    18: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   11 .LC5
+    19: 0000000000000017     0 NOTYPE  LOCAL  DEFAULT   11 .LC12
+    20: 000000000000001a     0 NOTYPE  LOCAL  DEFAULT   11 .LC13
+    21: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    1 _ZN11arithmetica8FractionD5Ev
+    22: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2Ev
+    23: 0000000000000000    44 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1Ev
+    24: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
+    25: 0000000000000000     8 OBJECT  WEAK   HIDDEN    14 DW.ref.__gxx_personality_v0
+    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
+    27: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __gxx_personality_v0
+    28: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZdlPvm
+    29: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Unwind_Resume
+    30: 0000000000000030    98 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_
+    31: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    32: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
+    33: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
+    34: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
+    35: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
+    36: 00000000000000a0   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    37: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2EPKc
+    38: 0000000000000150   172 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1EPKc
+    39: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC2ERK8fraction
+    40: 0000000000000200   155 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionC1ERK8fraction
+    41: 00000000000002a0   458 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev
+    42: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
+    43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
+    44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
+    45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt19__throw_logic_errorPKc
+    46: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc
     47: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
-    48: 00000000000005b0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmiERKS0_
-    49: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract_fraction
-    50: 00000000000008c0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmlERKS0_
-    51: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply_fraction
-    52: 0000000000000bd0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractiondvERKS0_
-    53: 0000000000000ee0   207 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractioneqERKS0_
-    54: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
-    55: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcmp
-    56: 0000000000000fb0   207 FUNC    GLOBAL DEFAULT    3 _ZeqRKN11arithmetica8FractionES2_
-    57: 0000000000001080   639 FUNC    GLOBAL DEFAULT    3 _ZltRKN11arithmetica8FractionES2_
+    48: 0000000000000000    66 FUNC    WEAK   DEFAULT   12 _ZN11arithmetica8FractionD2Ev
+    49: 0000000000000000    66 FUNC    WEAK   DEFAULT   12 _ZN11arithmetica8FractionD1Ev
+    50: 0000000000000470   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionplERKS0_
+    51: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
+    52: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcpy
+    53: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add_fraction
+    54: 0000000000000780   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmiERKS0_
+    55: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract_fraction
+    56: 0000000000000a90   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractionmlERKS0_
+    57: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply_fraction
+    58: 0000000000000da0   780 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractiondvERKS0_
+    59: 00000000000010b0   207 FUNC    GLOBAL DEFAULT    3 _ZN11arithmetica8FractioneqERKS0_
+    60: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
+    61: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcmp
+    62: 0000000000001180   207 FUNC    GLOBAL DEFAULT    3 _ZeqRKN11arithmetica8FractionES2_
+    63: 0000000000001250   639 FUNC    GLOBAL DEFAULT    3 _ZltRKN11arithmetica8FractionES2_
```

##### readelf --wide --relocs {}

```diff
@@ -1,229 +1,244 @@
 
-Relocation section '.rela.text' at offset 0x2948 contains 170 entries:
+Relocation section '.rela.text' at offset 0x2d40 contains 183 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000006a  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
-0000000000000079  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
-00000000000000e0  0000001d00000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
-00000000000000ee  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000102  0000001f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-000000000000010e  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000122  0000001f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-000000000000012d  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000190  0000001d00000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
-000000000000019e  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001b2  0000001f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-00000000000001be  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001d2  0000001f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-00000000000001dd  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000246  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000258  0000001f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-0000000000000268  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000027c  0000001f00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-00000000000002dc  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000002f1  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000306  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000031b  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000032a  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000336  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000341  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000350  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000378  0000002b00000004 R_X86_64_PLT32         0000000000000000 add_fraction - 4
-0000000000000389  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000399  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000003b4  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000003fe  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000403  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000424  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000467  0000001b00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-000000000000047f  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000497  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000004a2  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000004fb  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000518  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000053b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000055a  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000056e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000575  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-000000000000057a  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000005ec  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000601  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000616  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000062b  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000063a  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000646  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000651  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000660  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000688  0000003100000004 R_X86_64_PLT32         0000000000000000 subtract_fraction - 4
-0000000000000699  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000006a9  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000006c4  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000070e  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000713  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000734  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000777  0000001b00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-000000000000078f  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000007a7  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000007b2  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-000000000000080b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000828  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000084b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000086a  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000087e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000885  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-000000000000088a  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000008fc  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000911  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000926  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000093b  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000094a  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000956  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000961  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000970  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000998  0000003300000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
-00000000000009a9  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000009b9  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000009d4  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000a1e  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000a23  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000a44  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000a87  0000001b00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-0000000000000a9f  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000ab7  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000ac2  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000b1b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000b38  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000b5b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000b7a  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000b8e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000b95  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000b9a  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000c0c  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000c21  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000c36  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000c4b  0000002900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000c5a  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000c66  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000c72  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000c80  0000002a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000000ca8  0000003300000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
-0000000000000cb9  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000cc9  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000ce4  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000d2e  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000d33  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000d54  0000001e00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000d97  0000001b00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
-0000000000000daf  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000dc7  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000dd2  0000002000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000e2b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000e48  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000e6b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000e8a  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000e9e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000ea5  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-0000000000000eaa  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000ee9  0000001000000002 R_X86_64_PC32          0000000000000000 .LC9 - 4
-0000000000000ef2  0000001100000002 R_X86_64_PC32          0000000000000003 .LC10 - 4
-0000000000000f06  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000000f15  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000000f28  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000000f5d  0000003700000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000000f85  0000003700000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000000f97  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000000fb9  0000001000000002 R_X86_64_PC32          0000000000000000 .LC9 - 4
-0000000000000fc2  0000001100000002 R_X86_64_PC32          0000000000000003 .LC10 - 4
-0000000000000fd6  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000000fe5  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000000ff8  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-000000000000102d  0000003700000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001055  0000003700000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001067  0000003600000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
-0000000000001160  0000003000000004 R_X86_64_PLT32         00000000000005b0 _ZN11arithmetica8FractionmiERKS0_ - 4
-0000000000001192  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000011af  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000011c7  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000011df  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000124d  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000126a  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000128d  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000012aa  0000002e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000012c0  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-00000000000012c5  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000012ca  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-00000000000012d1  0000000f00000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
-00000000000012d6  0000002c00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000006a  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
+0000000000000079  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
+00000000000000e0  0000002000000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
+00000000000000ee  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000102  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+000000000000010e  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000122  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+000000000000012d  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000190  0000002000000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
+000000000000019e  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000001b2  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+00000000000001be  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000001d2  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+00000000000001dd  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000246  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000258  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+0000000000000268  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000027c  0000002200000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+0000000000000338  0000001000000002 R_X86_64_PC32          0000000000000015 .LC6 - 4
+0000000000000340  0000002a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+0000000000000350  0000002a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+00000000000003a6  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000003ed  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000040a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000433  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000438  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000043f  0000001200000002 R_X86_64_PC32          0000000000000000 .LC5 - 4
+0000000000000444  0000002e00000004 R_X86_64_PLT32         0000000000000000 _ZSt20__throw_length_errorPKc - 4
+0000000000000449  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+00000000000004ac  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004c1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004d6  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004eb  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004fa  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000506  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000511  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000520  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000548  0000003500000004 R_X86_64_PLT32         0000000000000000 add_fraction - 4
+0000000000000559  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000569  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000584  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000005ce  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000005d3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000005f4  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000637  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+000000000000064f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000667  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000672  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+00000000000006cb  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000006e8  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000070b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000072a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000073e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000745  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+000000000000074a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000007bc  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000007d1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000007e6  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000007fb  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000080a  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000816  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000821  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000830  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000858  0000003700000004 R_X86_64_PLT32         0000000000000000 subtract_fraction - 4
+0000000000000869  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000879  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000894  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000008de  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000008e3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000904  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000947  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+000000000000095f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000977  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000982  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+00000000000009db  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000009f8  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000a1b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000a3a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000a4e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000a55  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000a5a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000acc  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000ae1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000af6  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b0b  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b1a  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b26  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b31  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b40  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000b68  0000003900000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
+0000000000000b79  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000b89  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000ba4  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000bee  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000bf3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000c14  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000c57  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+0000000000000c6f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000c87  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000c92  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000ceb  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000d08  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000d2b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000d4a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000d5e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000d65  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000d6a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000ddc  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000df1  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e06  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e1b  0000003300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e2a  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e36  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e42  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e50  0000003400000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000000e78  0000003900000004 R_X86_64_PLT32         0000000000000000 multiply_fraction - 4
+0000000000000e89  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000e99  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000eb4  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000efe  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000000f03  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000f24  0000002100000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000f67  0000001e00000004 R_X86_64_PLT32         0000000000000030 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_ - 4
+0000000000000f7f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000f97  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000fa2  0000002300000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000ffb  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000001018  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000103b  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000105a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000106e  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000001075  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+000000000000107a  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000010b9  0000001300000002 R_X86_64_PC32          0000000000000017 .LC12 - 4
+00000000000010c2  0000001400000002 R_X86_64_PC32          000000000000001a .LC13 - 4
+00000000000010d6  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000010e5  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000010f8  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+000000000000112d  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001155  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001167  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001189  0000001300000002 R_X86_64_PC32          0000000000000017 .LC12 - 4
+0000000000001192  0000001400000002 R_X86_64_PC32          000000000000001a .LC13 - 4
+00000000000011a6  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000011b5  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000011c8  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+00000000000011fd  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001225  0000003d00000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001237  0000003c00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001330  0000003600000004 R_X86_64_PLT32         0000000000000780 _ZN11arithmetica8FractionmiERKS0_ - 4
+0000000000001362  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000137f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001397  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000013af  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000141d  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000143a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000145d  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000147a  0000002c00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000001490  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+0000000000001495  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000149a  0000002f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+00000000000014a1  0000001100000002 R_X86_64_PC32          0000000000000000 .LC4 - 4
+00000000000014a6  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
 000000000000008e  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely - 4
 0000000000000148  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 30
 00000000000001f8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 64
 0000000000000297  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 98
-0000000000000590  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + e4
-000000000000059c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
-00000000000005a8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + fe
-00000000000008a0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 128
-00000000000008ac  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 110
-00000000000008b8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 142
-0000000000000bb0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 16c
-0000000000000bbc  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 154
-0000000000000bc8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 186
-0000000000000ec0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1b0
-0000000000000ecc  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 198
-0000000000000ed8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1ca
-00000000000012ef  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1dc
-00000000000012fb  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1fc
+000000000000045a  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
+0000000000000466  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + cc
+0000000000000760  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 104
+000000000000076c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + ec
+0000000000000778  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 11e
+0000000000000a70  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 148
+0000000000000a7c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 130
+0000000000000a88  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 162
+0000000000000d80  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 18c
+0000000000000d8c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 174
+0000000000000d98  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1a6
+0000000000001090  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1d0
+000000000000109c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1b8
+00000000000010a8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1ea
+00000000000014bf  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1fc
+00000000000014cb  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 21c
 
-Relocation section '.rela.text.unlikely' at offset 0x3938 contains 32 entries:
+Relocation section '.rela.text.unlikely' at offset 0x3e68 contains 34 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000012  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000027  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000002f  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000046  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000005b  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000063  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000007a  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000008f  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000097  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000000ae  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000c3  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000cb  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000000e4  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000fc  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000108  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-0000000000000110  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000128  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000140  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000014c  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-0000000000000154  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000016c  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000184  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000190  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-0000000000000198  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000001b0  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001c8  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001d4  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-00000000000001dc  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000001f4  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001fc  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000204  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
-000000000000020c  0000001a00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000012  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000027  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000002f  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000046  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000005b  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000063  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000007a  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000008f  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000097  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000000ae  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000c3  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000cb  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000000e4  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000ec  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000104  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000011c  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000128  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+0000000000000130  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000148  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000160  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000016c  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+0000000000000174  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000018c  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001a4  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001b0  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+00000000000001b8  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000001d0  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001e8  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001f4  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+00000000000001fc  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000214  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000021c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000224  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZN11arithmetica8FractionD1Ev - 4
+000000000000022c  0000001d00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
 
-Relocation section '.rela.text._ZN11arithmetica8FractionD2Ev' at offset 0x3c38 contains 2 entries:
+Relocation section '.rela.text._ZN11arithmetica8FractionD2Ev' at offset 0x4198 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000001e  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000038  0000001900000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000001e  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000038  0000001c00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
 
-Relocation section '.rela.data.rel.local.DW.ref.__gxx_personality_v0' at offset 0x3c68 contains 1 entry:
+Relocation section '.rela.data.rel.local.DW.ref.__gxx_personality_v0' at offset 0x41c8 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000000  0000001800000001 R_X86_64_64            0000000000000000 __gxx_personality_v0 + 0
+0000000000000000  0000001b00000001 R_X86_64_64            0000000000000000 __gxx_personality_v0 + 0
 
-Relocation section '.rela.eh_frame' at offset 0x3c80 contains 41 entries:
+Relocation section '.rela.eh_frame' at offset 0x41e0 contains 45 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
-000000000000003f  0000001600000002 R_X86_64_PC32          0000000000000000 DW.ref.__gxx_personality_v0 + 0
+000000000000003f  0000001900000002 R_X86_64_PC32          0000000000000000 DW.ref.__gxx_personality_v0 + 0
 0000000000000054  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 30
 000000000000005d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 0
 0000000000000094  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 0
 000000000000009d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 8
 00000000000000b8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + a0
 00000000000000c1  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 10
 0000000000000108  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 34
@@ -232,30 +247,34 @@
 0000000000000135  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 21
 000000000000017c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 68
 0000000000000185  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 2a
 00000000000001a0  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 200
 00000000000001a9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 32
 00000000000001f0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 9c
 00000000000001f9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 3b
-0000000000000214  0000000900000002 R_X86_64_PC32          0000000000000000 .text._ZN11arithmetica8FractionD2Ev + 0
-0000000000000234  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 2a0
-000000000000023d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 43
-0000000000000288  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + d0
-0000000000000291  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 6e
-00000000000002ac  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 5b0
-00000000000002b5  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 76
-0000000000000300  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 114
-0000000000000309  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + a1
-0000000000000324  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 8c0
-000000000000032d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + a9
-0000000000000378  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 158
-0000000000000381  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + d4
-000000000000039c  0000000200000002 R_X86_64_PC32          0000000000000000 .text + bd0
-00000000000003a5  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + dc
-00000000000003f0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 19c
-00000000000003f9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 107
-0000000000000414  0000000200000002 R_X86_64_PC32          0000000000000000 .text + ee0
-0000000000000460  0000000200000002 R_X86_64_PC32          0000000000000000 .text + fb0
-00000000000004ac  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1080
-00000000000004b5  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 10f
-0000000000000500  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1e0
-0000000000000509  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 12f
+0000000000000214  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 2a0
+000000000000021d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 43
+000000000000025c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + d0
+0000000000000265  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 5e
+0000000000000280  0000000a00000002 R_X86_64_PC32          0000000000000000 .text._ZN11arithmetica8FractionD2Ev + 0
+00000000000002a0  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 470
+00000000000002a9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 66
+00000000000002f4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + f0
+00000000000002fd  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 91
+0000000000000318  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 780
+0000000000000321  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 99
+000000000000036c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 134
+0000000000000375  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + c4
+0000000000000390  0000000200000002 R_X86_64_PC32          0000000000000000 .text + a90
+0000000000000399  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + cc
+00000000000003e4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 178
+00000000000003ed  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + f7
+0000000000000408  0000000200000002 R_X86_64_PC32          0000000000000000 .text + da0
+0000000000000411  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + ff
+000000000000045c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1bc
+0000000000000465  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 12a
+0000000000000480  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 10b0
+00000000000004cc  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1180
+0000000000000518  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1250
+0000000000000521  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 132
+000000000000056c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 200
+0000000000000575  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 152
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -225,371 +225,414 @@
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_nop
 
-0000020c 000000000000001c 00000210 FDE cie=00000000 pc=0000000000000000..0000000000000042
+0000020c 0000000000000044 000001e4 FDE cie=0000002c pc=00000000000002a0..000000000000046a
+  Augmentation data:     26 fe ff ff
+  DW_CFA_advance_loc: 6 to 00000000000002a6
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_advance_loc: 2 to 00000000000002a8
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_advance_loc: 2 to 00000000000002aa
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_advance_loc: 4 to 00000000000002ae
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_advance_loc: 1 to 00000000000002af
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_advance_loc: 7 to 00000000000002b6
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_advance_loc2: 268 to 00000000000003c2
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 4 to 00000000000003c6
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 1 to 00000000000003c7
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 00000000000003c9
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 00000000000003cb
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 00000000000003cd
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 3 to 00000000000003d0
+  DW_CFA_restore_state
+
+00000254 0000000000000020 0000022c FDE cie=0000002c pc=00000000000000d0..00000000000000f0
+  Augmentation data:     f9 fd ff ff
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000278 000000000000001c 0000027c FDE cie=00000000 pc=0000000000000000..0000000000000042
   DW_CFA_advance_loc: 5 to 0000000000000005
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
   DW_CFA_advance_loc: 46 to 0000000000000033
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 13 to 0000000000000040
   DW_CFA_restore_state
   DW_CFA_advance_loc: 1 to 0000000000000041
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-0000022c 0000000000000050 00000204 FDE cie=0000002c pc=00000000000002a0..00000000000005ac
-  Augmentation data:     06 fe ff ff
-  DW_CFA_advance_loc: 6 to 00000000000002a6
+00000298 0000000000000050 00000270 FDE cie=0000002c pc=0000000000000470..000000000000077c
+  Augmentation data:     bd fd ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000476
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000002a8
+  DW_CFA_advance_loc: 2 to 0000000000000478
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000002aa
+  DW_CFA_advance_loc: 2 to 000000000000047a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000002ac
+  DW_CFA_advance_loc: 2 to 000000000000047c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000002ad
+  DW_CFA_advance_loc: 1 to 000000000000047d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 00000000000002b1
+  DW_CFA_advance_loc: 4 to 0000000000000481
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 00000000000002bb
+  DW_CFA_advance_loc: 10 to 000000000000048b
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 00000000000004c6
+  DW_CFA_advance_loc2: 523 to 0000000000000696
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000004c7
+  DW_CFA_advance_loc: 1 to 0000000000000697
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000004c8
+  DW_CFA_advance_loc: 1 to 0000000000000698
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000004ca
+  DW_CFA_advance_loc: 2 to 000000000000069a
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000004cc
+  DW_CFA_advance_loc: 2 to 000000000000069c
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000004ce
+  DW_CFA_advance_loc: 2 to 000000000000069e
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000004d0
+  DW_CFA_advance_loc: 2 to 00000000000006a0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 00000000000004d8
+  DW_CFA_advance_loc: 8 to 00000000000006a8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000280 0000000000000020 00000258 FDE cie=0000002c pc=00000000000000d0..0000000000000114
-  Augmentation data:     dd fd ff ff
+000002ec 0000000000000020 000002c4 FDE cie=0000002c pc=00000000000000f0..0000000000000134
+  Augmentation data:     94 fd ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-000002a4 0000000000000050 0000027c FDE cie=0000002c pc=00000000000005b0..00000000000008bc
-  Augmentation data:     c1 fd ff ff
-  DW_CFA_advance_loc: 6 to 00000000000005b6
+00000310 0000000000000050 000002e8 FDE cie=0000002c pc=0000000000000780..0000000000000a8c
+  Augmentation data:     78 fd ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000786
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000005b8
+  DW_CFA_advance_loc: 2 to 0000000000000788
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000005ba
+  DW_CFA_advance_loc: 2 to 000000000000078a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000005bc
+  DW_CFA_advance_loc: 2 to 000000000000078c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000005bd
+  DW_CFA_advance_loc: 1 to 000000000000078d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 00000000000005c1
+  DW_CFA_advance_loc: 4 to 0000000000000791
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 00000000000005cb
+  DW_CFA_advance_loc: 10 to 000000000000079b
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 00000000000007d6
+  DW_CFA_advance_loc2: 523 to 00000000000009a6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000007d7
+  DW_CFA_advance_loc: 1 to 00000000000009a7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000007d8
+  DW_CFA_advance_loc: 1 to 00000000000009a8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000007da
+  DW_CFA_advance_loc: 2 to 00000000000009aa
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000007dc
+  DW_CFA_advance_loc: 2 to 00000000000009ac
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000007de
+  DW_CFA_advance_loc: 2 to 00000000000009ae
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000007e0
+  DW_CFA_advance_loc: 2 to 00000000000009b0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 00000000000007e8
+  DW_CFA_advance_loc: 8 to 00000000000009b8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002f8 0000000000000020 000002d0 FDE cie=0000002c pc=0000000000000114..0000000000000158
-  Augmentation data:     98 fd ff ff
+00000364 0000000000000020 0000033c FDE cie=0000002c pc=0000000000000134..0000000000000178
+  Augmentation data:     4f fd ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-0000031c 0000000000000050 000002f4 FDE cie=0000002c pc=00000000000008c0..0000000000000bcc
-  Augmentation data:     7c fd ff ff
-  DW_CFA_advance_loc: 6 to 00000000000008c6
+00000388 0000000000000050 00000360 FDE cie=0000002c pc=0000000000000a90..0000000000000d9c
+  Augmentation data:     33 fd ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000a96
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000008c8
+  DW_CFA_advance_loc: 2 to 0000000000000a98
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000008ca
+  DW_CFA_advance_loc: 2 to 0000000000000a9a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000008cc
+  DW_CFA_advance_loc: 2 to 0000000000000a9c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000008cd
+  DW_CFA_advance_loc: 1 to 0000000000000a9d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 00000000000008d1
+  DW_CFA_advance_loc: 4 to 0000000000000aa1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 00000000000008db
+  DW_CFA_advance_loc: 10 to 0000000000000aab
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 0000000000000ae6
+  DW_CFA_advance_loc2: 523 to 0000000000000cb6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000ae7
+  DW_CFA_advance_loc: 1 to 0000000000000cb7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000ae8
+  DW_CFA_advance_loc: 1 to 0000000000000cb8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000000aea
+  DW_CFA_advance_loc: 2 to 0000000000000cba
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000aec
+  DW_CFA_advance_loc: 2 to 0000000000000cbc
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000aee
+  DW_CFA_advance_loc: 2 to 0000000000000cbe
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000af0
+  DW_CFA_advance_loc: 2 to 0000000000000cc0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000000af8
+  DW_CFA_advance_loc: 8 to 0000000000000cc8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000370 0000000000000020 00000348 FDE cie=0000002c pc=0000000000000158..000000000000019c
-  Augmentation data:     53 fd ff ff
+000003dc 0000000000000020 000003b4 FDE cie=0000002c pc=0000000000000178..00000000000001bc
+  Augmentation data:     0a fd ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00000394 0000000000000050 0000036c FDE cie=0000002c pc=0000000000000bd0..0000000000000edc
-  Augmentation data:     37 fd ff ff
-  DW_CFA_advance_loc: 6 to 0000000000000bd6
+00000400 0000000000000050 000003d8 FDE cie=0000002c pc=0000000000000da0..00000000000010ac
+  Augmentation data:     ee fc ff ff
+  DW_CFA_advance_loc: 6 to 0000000000000da6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000000bd8
+  DW_CFA_advance_loc: 2 to 0000000000000da8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000000bda
+  DW_CFA_advance_loc: 2 to 0000000000000daa
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000000bdc
+  DW_CFA_advance_loc: 2 to 0000000000000dac
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000bdd
+  DW_CFA_advance_loc: 1 to 0000000000000dad
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000be1
+  DW_CFA_advance_loc: 4 to 0000000000000db1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 0000000000000beb
+  DW_CFA_advance_loc: 10 to 0000000000000dbb
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 523 to 0000000000000df6
+  DW_CFA_advance_loc2: 523 to 0000000000000fc6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000df7
+  DW_CFA_advance_loc: 1 to 0000000000000fc7
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000df8
+  DW_CFA_advance_loc: 1 to 0000000000000fc8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000000dfa
+  DW_CFA_advance_loc: 2 to 0000000000000fca
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000dfc
+  DW_CFA_advance_loc: 2 to 0000000000000fcc
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000dfe
+  DW_CFA_advance_loc: 2 to 0000000000000fce
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000e00
+  DW_CFA_advance_loc: 2 to 0000000000000fd0
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000000e08
+  DW_CFA_advance_loc: 8 to 0000000000000fd8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003e8 0000000000000020 000003c0 FDE cie=0000002c pc=000000000000019c..00000000000001e0
-  Augmentation data:     0e fd ff ff
+00000454 0000000000000020 0000042c FDE cie=0000002c pc=00000000000001bc..0000000000000200
+  Augmentation data:     c5 fc ff ff
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-0000040c 0000000000000048 00000410 FDE cie=00000000 pc=0000000000000ee0..0000000000000faf
-  DW_CFA_advance_loc: 6 to 0000000000000ee6
+00000478 0000000000000048 0000047c FDE cie=00000000 pc=00000000000010b0..000000000000117f
+  DW_CFA_advance_loc: 6 to 00000000000010b6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 9 to 0000000000000eef
+  DW_CFA_advance_loc: 9 to 00000000000010bf
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 8 to 0000000000000ef7
+  DW_CFA_advance_loc: 8 to 00000000000010c7
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 7 to 0000000000000efe
+  DW_CFA_advance_loc: 7 to 00000000000010ce
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 7 to 0000000000000f05
+  DW_CFA_advance_loc: 7 to 00000000000010d5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 59 to 0000000000000f40
+  DW_CFA_advance_loc: 59 to 0000000000001110
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000000f41
+  DW_CFA_advance_loc: 1 to 0000000000001111
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000000f42
+  DW_CFA_advance_loc: 1 to 0000000000001112
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000f44
+  DW_CFA_advance_loc: 2 to 0000000000001114
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000f46
+  DW_CFA_advance_loc: 2 to 0000000000001116
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 0000000000000f50
+  DW_CFA_advance_loc: 10 to 0000000000001120
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 83 to 0000000000000fa3
+  DW_CFA_advance_loc1: 83 to 0000000000001173
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 6 to 0000000000000fa9
+  DW_CFA_advance_loc: 6 to 0000000000001179
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000000faa
+  DW_CFA_advance_loc: 1 to 000000000000117a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000fac
+  DW_CFA_advance_loc: 2 to 000000000000117c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000fae
+  DW_CFA_advance_loc: 2 to 000000000000117e
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000458 0000000000000048 0000045c FDE cie=00000000 pc=0000000000000fb0..000000000000107f
-  DW_CFA_advance_loc: 6 to 0000000000000fb6
+000004c4 0000000000000048 000004c8 FDE cie=00000000 pc=0000000000001180..000000000000124f
+  DW_CFA_advance_loc: 6 to 0000000000001186
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 9 to 0000000000000fbf
+  DW_CFA_advance_loc: 9 to 000000000000118f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 8 to 0000000000000fc7
+  DW_CFA_advance_loc: 8 to 0000000000001197
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 7 to 0000000000000fce
+  DW_CFA_advance_loc: 7 to 000000000000119e
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 7 to 0000000000000fd5
+  DW_CFA_advance_loc: 7 to 00000000000011a5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 59 to 0000000000001010
+  DW_CFA_advance_loc: 59 to 00000000000011e0
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000001011
+  DW_CFA_advance_loc: 1 to 00000000000011e1
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000001012
+  DW_CFA_advance_loc: 1 to 00000000000011e2
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001014
+  DW_CFA_advance_loc: 2 to 00000000000011e4
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001016
+  DW_CFA_advance_loc: 2 to 00000000000011e6
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 0000000000001020
+  DW_CFA_advance_loc: 10 to 00000000000011f0
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 83 to 0000000000001073
+  DW_CFA_advance_loc1: 83 to 0000000000001243
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 6 to 0000000000001079
+  DW_CFA_advance_loc: 6 to 0000000000001249
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 000000000000107a
+  DW_CFA_advance_loc: 1 to 000000000000124a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000107c
+  DW_CFA_advance_loc: 2 to 000000000000124c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000107e
+  DW_CFA_advance_loc: 2 to 000000000000124e
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-000004a4 0000000000000050 0000047c FDE cie=0000002c pc=0000000000001080..00000000000012ff
-  Augmentation data:     5a fc ff ff
-  DW_CFA_advance_loc: 6 to 0000000000001086
+00000510 0000000000000050 000004e8 FDE cie=0000002c pc=0000000000001250..00000000000014cf
+  Augmentation data:     11 fc ff ff
+  DW_CFA_advance_loc: 6 to 0000000000001256
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001088
+  DW_CFA_advance_loc: 2 to 0000000000001258
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000108a
+  DW_CFA_advance_loc: 2 to 000000000000125a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000108f
+  DW_CFA_advance_loc: 5 to 000000000000125f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001090
+  DW_CFA_advance_loc: 1 to 0000000000001260
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001091
+  DW_CFA_advance_loc: 1 to 0000000000001261
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 000000000000109b
+  DW_CFA_advance_loc: 10 to 000000000000126b
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 358 to 0000000000001201
+  DW_CFA_advance_loc2: 358 to 00000000000013d1
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000001205
+  DW_CFA_advance_loc: 4 to 00000000000013d5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001206
+  DW_CFA_advance_loc: 1 to 00000000000013d6
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001208
+  DW_CFA_advance_loc: 2 to 00000000000013d8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000120a
+  DW_CFA_advance_loc: 2 to 00000000000013da
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000120c
+  DW_CFA_advance_loc: 2 to 00000000000013dc
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000120e
+  DW_CFA_advance_loc: 2 to 00000000000013de
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 2 to 0000000000001210
+  DW_CFA_advance_loc: 2 to 00000000000013e0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004f8 0000000000000024 000004d0 FDE cie=0000002c pc=00000000000001e0..0000000000000210
-  Augmentation data:     26 fc ff ff
+00000564 0000000000000020 0000053c FDE cie=0000002c pc=0000000000000200..0000000000000230
+  Augmentation data:     dd fb ff ff
   DW_CFA_def_cfa_offset: 224
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
```

##### strings --all --bytes=8 {}

```diff
@@ -1,28 +1,31 @@
 []A\A]A^
 []A\A]A^A_
 AWAVAUATUSH
 []A\A]A^A_
 []A\A]A^A_
+[]A\A]A^
 AWAVAUATUH
 []A\A]A^A_
 AWAVAUATUH
 []A\A]A^A_
 AWAVAUATUH
 []A\A]A^A_
 AWAVAUATUH
 []A\A]A^A_
 []A\A]A^A_
 basic_string::_M_construct null not valid
+basic_string::append
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 Fraction.cpp
 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_.cold
 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 _ZN11arithmetica8FractionC2EPKc.cold
 _ZN11arithmetica8FractionC2ERK8fraction.cold
+_ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
 _ZN11arithmetica8FractionplERKS0_.cold
 _ZN11arithmetica8FractionmiERKS0_.cold
 _ZN11arithmetica8FractionmlERKS0_.cold
 _ZN11arithmetica8FractiondvERKS0_.cold
 _ZltRKN11arithmetica8FractionES2_.cold
 _ZN11arithmetica8FractionD5Ev
 _ZN11arithmetica8FractionC2Ev
@@ -37,35 +40,38 @@
 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
 delete_fraction
 _ZN11arithmetica8FractionC1ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
 _ZN11arithmetica8FractionC2EPKc
 _ZN11arithmetica8FractionC1EPKc
 _ZN11arithmetica8FractionC2ERK8fraction
 _ZN11arithmetica8FractionC1ERK8fraction
+_ZN11arithmetica8Fraction9to_stringB5cxx11Ev
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
+_ZSt19__throw_logic_errorPKc
+_ZSt20__throw_length_errorPKc
+__stack_chk_fail
 _ZN11arithmetica8FractionD2Ev
 _ZN11arithmetica8FractionD1Ev
 _ZN11arithmetica8FractionplERKS0_
 add_fraction
-_ZSt19__throw_logic_errorPKc
-_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
-__stack_chk_fail
 _ZN11arithmetica8FractionmiERKS0_
 subtract_fraction
 _ZN11arithmetica8FractionmlERKS0_
 multiply_fraction
 _ZN11arithmetica8FractiondvERKS0_
 _ZN11arithmetica8FractioneqERKS0_
 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
 _ZeqRKN11arithmetica8FractionES2_
 _ZltRKN11arithmetica8FractionES2_
 .shstrtab
 .rela.text
 .rela.text.unlikely
 .gcc_except_table
-.rela.text._ZN11arithmetica8FractionD2Ev
 .rodata.str1.8
 .rodata.str1.1
+.rela.text._ZN11arithmetica8FractionD2Ev
 .rela.data.rel.local.DW.ref.__gxx_personality_v0
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### readelf --wide --decompress --hex-dump=.group {}

```diff
@@ -1,8 +1,8 @@
 
 Hex dump of section '.group':
-  0x00000000 01000000 0a000000 0b000000          ............
+  0x00000000 01000000 0c000000 0d000000          ............
 
 
 Hex dump of section '.group':
   0x00000000 01000000 0e000000 0f000000          ............
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -235,15 +235,143 @@
 	endbr64
 	mov    %rax,%rbp
 	jmp    29b <arithmetica::Fraction::Fraction(fraction const&)+0x9b>
  R_X86_64_PC32	.text.unlikely+0x98
 	nop
 	nopl   0x0(%rax)
 
-00000000000002a0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)>:
+00000000000002a0 <arithmetica::Fraction::to_string[abi:cxx11]()>:
+arithmetica::Fraction::to_string[abi:cxx11]():
+	endbr64
+	push   %r14
+	push   %r13
+	push   %r12
+	mov    %rdi,%r12
+	push   %rbp
+	push   %rbx
+	mov    %rsi,%rbx
+	sub    $0x40,%rsp
+	mov    (%rsi),%r14
+	mov    0x8(%rsi),%r13
+	mov    %fs:0x28,%rax
+	mov    %rax,0x38(%rsp)
+	xor    %eax,%eax
+	lea    0x20(%rsp),%rbp
+	mov    %r14,%rax
+	mov    %rbp,0x10(%rsp)
+	add    %r13,%rax
+	je     2e8 <arithmetica::Fraction::to_string[abi:cxx11]()+0x48>
+	test   %r14,%r14
+	je     430 <arithmetica::Fraction::to_string[abi:cxx11]()+0x190>
+	mov    %r13,0x8(%rsp)
+	cmp    $0xf,%r13
+	ja     3e0 <arithmetica::Fraction::to_string[abi:cxx11]()+0x140>
+	cmp    $0x1,%r13
+	jne    3d0 <arithmetica::Fraction::to_string[abi:cxx11]()+0x130>
+	movzbl (%r14),%eax
+	mov    %al,0x20(%rsp)
+	mov    %rbp,%rax
+	mov    %r13,0x18(%rsp)
+	movb   $0x0,(%rax,%r13,1)
+	movabs $0x3fffffffffffffff,%rax
+	cmp    %rax,0x18(%rsp)
+	je     43c <arithmetica::Fraction::to_string[abi:cxx11]()+0x19c>
+	lea    0x10(%rsp),%r13
+	mov    $0x1,%edx
+	lea    0x0(%rip),%rsi        
+ R_X86_64_PC32	.LC6-0x4
+	mov    %r13,%rdi
+	call   344 <arithmetica::Fraction::to_string[abi:cxx11]()+0xa4>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x28(%rbx),%rdx
+	mov    0x20(%rbx),%rsi
+	mov    %r13,%rdi
+	call   354 <arithmetica::Fraction::to_string[abi:cxx11]()+0xb4>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	lea    0x10(%r12),%rdx
+	mov    %rdx,(%r12)
+	mov    (%rax),%rcx
+	lea    0x10(%rax),%rdx
+	cmp    %rdx,%rcx
+	je     420 <arithmetica::Fraction::to_string[abi:cxx11]()+0x180>
+	mov    %rcx,(%r12)
+	mov    0x10(%rax),%rcx
+	mov    %rcx,0x10(%r12)
+	mov    0x8(%rax),%rcx
+	mov    %rdx,(%rax)
+	mov    0x10(%rsp),%rdi
+	movq   $0x0,0x8(%rax)
+	mov    %rcx,0x8(%r12)
+	movb   $0x0,0x10(%rax)
+	cmp    %rbp,%rdi
+	je     3aa <arithmetica::Fraction::to_string[abi:cxx11]()+0x10a>
+	mov    0x20(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   3aa <arithmetica::Fraction::to_string[abi:cxx11]()+0x10a>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    0x38(%rsp),%rax
+	sub    %fs:0x28,%rax
+	jne    448 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a8>
+	add    $0x40,%rsp
+	mov    %r12,%rax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	ret
+	xchg   %ax,%ax
+	test   %r13,%r13
+	jne    44d <arithmetica::Fraction::to_string[abi:cxx11]()+0x1ad>
+	mov    %rbp,%rax
+	jmp    30c <arithmetica::Fraction::to_string[abi:cxx11]()+0x6c>
+	nopl   (%rax)
+	lea    0x10(%rsp),%rdi
+	lea    0x8(%rsp),%rsi
+	xor    %edx,%edx
+	call   3f1 <arithmetica::Fraction::to_string[abi:cxx11]()+0x151>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
+	mov    %rax,0x10(%rsp)
+	mov    %rax,%rdi
+	mov    0x8(%rsp),%rax
+	mov    %rax,0x20(%rsp)
+	mov    %r13,%rdx
+	mov    %r14,%rsi
+	call   40e <arithmetica::Fraction::to_string[abi:cxx11]()+0x16e>
+ R_X86_64_PLT32	memcpy-0x4
+	mov    0x8(%rsp),%r13
+	mov    0x10(%rsp),%rax
+	jmp    30c <arithmetica::Fraction::to_string[abi:cxx11]()+0x6c>
+	nopl   (%rax)
+	movdqu 0x10(%rax),%xmm0
+	movups %xmm0,0x10(%r12)
+	jmp    37a <arithmetica::Fraction::to_string[abi:cxx11]()+0xda>
+	lea    0x0(%rip),%rdi        
+ R_X86_64_PC32	.LC4-0x4
+	call   43c <arithmetica::Fraction::to_string[abi:cxx11]()+0x19c>
+ R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
+	lea    0x0(%rip),%rdi        
+ R_X86_64_PC32	.LC5-0x4
+	call   448 <arithmetica::Fraction::to_string[abi:cxx11]()+0x1a8>
+ R_X86_64_PLT32	std::__throw_length_error(char const*)-0x4
+	call   44d <arithmetica::Fraction::to_string[abi:cxx11]()+0x1ad>
+ R_X86_64_PLT32	__stack_chk_fail-0x4
+	mov    %rbp,%rdi
+	jmp    403 <arithmetica::Fraction::to_string[abi:cxx11]()+0x163>
+	endbr64
+	mov    %rax,%r12
+	jmp    45e <arithmetica::Fraction::to_string[abi:cxx11]()+0x1be>
+ R_X86_64_PC32	.text.unlikely+0xcc
+	endbr64
+	mov    %rax,%r12
+	jmp    46a <arithmetica::Fraction::to_string[abi:cxx11]()+0x1ca>
+ R_X86_64_PC32	.text.unlikely+0xcc
+	nopw   0x0(%rax,%rax,1)
+
+0000000000000470 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator+(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -253,220 +381,220 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   2e0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x40>
+	call   4b0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   2f5 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x55>
+	call   4c5 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   30a <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x6a>
+	call   4da <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   31f <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x7f>
+	call   4ef <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   32e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x8e>
+	call   4fe <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   33a <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x9a>
+	call   50a <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r15,%rdi
-	call   345 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xa5>
+	call   515 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xa5>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   354 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xb4>
+	call   524 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   37c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xdc>
+	call   54c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	add_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   38d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xed>
+	call   55d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   39d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xfd>
+	call   56d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     572 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
+	je     742 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   3b8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x118>
+	call   588 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     4f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x250>
+	ja     6c0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    410 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x170>
+	jne    5e0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    420 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x180>
+	jne    5f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   407 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x167>
+	call   5d7 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    583 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2e3>
+	jne    753 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    3db <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
+	jmp    5ab <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   428 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x188>
+	call   5f8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     530 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x290>
+	ja     700 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    4d8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x238>
+	jne    6a8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   46b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1cb>
+	call   63b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     483 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
+	je     653 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   483 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
+	call   653 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     49b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
+	je     66b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   49b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
+	call   66b <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   4a6 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x206>
+	call   676 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    56d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2cd>
+	jne    73d <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    57e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
+	jne    74e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    452 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
+	jmp    622 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   4ff <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x25f>
+	call   6cf <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   51c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x27c>
+	call   6ec <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    3db <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
+	jmp    5ab <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   53f <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x29f>
+	call   70f <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   55e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2be>
+	call   72e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    452 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
-	call   572 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
+	jmp    622 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x1b2>
+	call   742 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   57e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
+	call   74e <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    551 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2b1>
+	jmp    721 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    511 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x271>
+	jmp    6e1 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    594 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0xe4
+	jmp    764 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x104
 	endbr64
 	mov    %rax,%rbp
-	jmp    5a0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0xcc
+	jmp    770 <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0xec
 	endbr64
 	mov    %rax,%rbp
-	jmp    5ac <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0xfe
+	jmp    77c <arithmetica::Fraction::operator+(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x11e
 	nopl   0x0(%rax)
 
-00000000000005b0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)>:
+0000000000000780 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator-(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -476,220 +604,220 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   5f0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x40>
+	call   7c0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   605 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x55>
+	call   7d5 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   61a <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x6a>
+	call   7ea <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   62f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x7f>
+	call   7ff <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   63e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x8e>
+	call   80e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   64a <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x9a>
+	call   81a <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r15,%rdi
-	call   655 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xa5>
+	call   825 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xa5>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   664 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xb4>
+	call   834 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   68c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xdc>
+	call   85c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	subtract_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   69d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xed>
+	call   86d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   6ad <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xfd>
+	call   87d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     882 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
+	je     a52 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   6c8 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x118>
+	call   898 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     800 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x250>
+	ja     9d0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    720 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x170>
+	jne    8f0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    730 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x180>
+	jne    900 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   717 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x167>
+	call   8e7 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    893 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2e3>
+	jne    a63 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    6eb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
+	jmp    8bb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   738 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x188>
+	call   908 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     840 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x290>
+	ja     a10 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    7e8 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x238>
+	jne    9b8 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   77b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1cb>
+	call   94b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     793 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
+	je     963 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   793 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
+	call   963 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     7ab <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
+	je     97b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   7ab <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
+	call   97b <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   7b6 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x206>
+	call   986 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    87d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2cd>
+	jne    a4d <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    88e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
+	jne    a5e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    762 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
+	jmp    932 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   80f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x25f>
+	call   9df <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   82c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x27c>
+	call   9fc <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    6eb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
+	jmp    8bb <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   84f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x29f>
+	call   a1f <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   86e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2be>
+	call   a3e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    762 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
-	call   882 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
+	jmp    932 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x1b2>
+	call   a52 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   88e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
+	call   a5e <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    861 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2b1>
+	jmp    a31 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    821 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x271>
+	jmp    9f1 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    8a4 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x128
+	jmp    a74 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x148
 	endbr64
 	mov    %rax,%rbp
-	jmp    8b0 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0x110
+	jmp    a80 <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x130
 	endbr64
 	mov    %rax,%rbp
-	jmp    8bc <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x142
+	jmp    a8c <arithmetica::Fraction::operator-(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x162
 	nopl   0x0(%rax)
 
-00000000000008c0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)>:
+0000000000000a90 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator*(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -699,220 +827,220 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   900 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x40>
+	call   ad0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   915 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x55>
+	call   ae5 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   92a <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x6a>
+	call   afa <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   93f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x7f>
+	call   b0f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   94e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x8e>
+	call   b1e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   95a <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x9a>
+	call   b2a <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r15,%rdi
-	call   965 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xa5>
+	call   b35 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xa5>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   974 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xb4>
+	call   b44 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   99c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xdc>
+	call   b6c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	multiply_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   9ad <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xed>
+	call   b7d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   9bd <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xfd>
+	call   b8d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     b92 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
+	je     d62 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   9d8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x118>
+	call   ba8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     b10 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x250>
+	ja     ce0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    a30 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x170>
+	jne    c00 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    a40 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x180>
+	jne    c10 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   a27 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x167>
+	call   bf7 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    ba3 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2e3>
+	jne    d73 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    9fb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
+	jmp    bcb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   a48 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x188>
+	call   c18 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     b50 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x290>
+	ja     d20 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    af8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x238>
+	jne    cc8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   a8b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1cb>
+	call   c5b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     aa3 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
+	je     c73 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   aa3 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
+	call   c73 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     abb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
+	je     c8b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   abb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
+	call   c8b <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   ac6 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x206>
+	call   c96 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    b8d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2cd>
+	jne    d5d <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    b9e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
+	jne    d6e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    a72 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
+	jmp    c42 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   b1f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x25f>
+	call   cef <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   b3c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x27c>
+	call   d0c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    9fb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
+	jmp    bcb <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   b5f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x29f>
+	call   d2f <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   b7e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2be>
+	call   d4e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    a72 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
-	call   b92 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
+	jmp    c42 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x1b2>
+	call   d62 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   b9e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
+	call   d6e <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    b71 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2b1>
+	jmp    d41 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    b31 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x271>
+	jmp    d01 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    bb4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x16c
+	jmp    d84 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x18c
 	endbr64
 	mov    %rax,%rbp
-	jmp    bc0 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0x154
+	jmp    d90 <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x174
 	endbr64
 	mov    %rax,%rbp
-	jmp    bcc <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x186
+	jmp    d9c <arithmetica::Fraction::operator*(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x1a6
 	nopl   0x0(%rax)
 
-0000000000000bd0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)>:
+0000000000000da0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator/(arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -922,380 +1050,380 @@
 	sub    $0x88,%rsp
 	mov    %rdi,0x8(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x78(%rsp)
 	mov    0x8(%rsi),%rax
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdi
-	call   c10 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x40>
+	call   de0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x40>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r13
 	mov    0x28(%rbp),%rax
 	lea    0x1(%rax),%rdi
-	call   c25 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x55>
+	call   df5 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x55>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r14
 	mov    0x28(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   c3a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x6a>
+	call   e0a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x6a>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rax,%r15
 	mov    0x8(%rbx),%rax
 	lea    0x1(%rax),%rdi
-	call   c4f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x7f>
+	call   e1f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x7f>
  R_X86_64_PLT32	calloc-0x4
 	mov    0x0(%rbp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,%r12
-	call   c5e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x8e>
+	call   e2e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x8e>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbp),%rsi
 	mov    %r14,%rdi
-	call   c6a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x9a>
+	call   e3a <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x9a>
  R_X86_64_PLT32	strcpy-0x4
 	mov    0x20(%rbx),%rsi
 	mov    %r15,%rdi
-	call   c76 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xa6>
+	call   e46 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xa6>
  R_X86_64_PLT32	strcpy-0x4
 	mov    (%rbx),%rsi
 	mov    %r12,%rdi
 	mov    %r12,%rbx
-	call   c84 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xb4>
+	call   e54 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xb4>
  R_X86_64_PLT32	strcpy-0x4
 	movq   %r12,%xmm1
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	movq   %r15,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
-	call   cac <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xdc>
+	call   e7c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xdc>
  R_X86_64_PLT32	multiply_fraction-0x4
 	mov    %r13,%rdi
 	mov    %r14,%rsi
 	mov    %rax,%r12
 	mov    %rdx,%rbp
-	call   cbd <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xed>
+	call   e8d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xed>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	lea    0x60(%rsp),%rbx
-	call   ccd <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xfd>
+	call   e9d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0xfd>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbx,0x50(%rsp)
 	test   %rbp,%rbp
-	je     ea2 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
+	je     1072 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
 	mov    %rbp,%rdi
 	lea    0x50(%rsp),%r15
-	call   ce8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x118>
+	call   eb8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x118>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x28(%rsp)
 	mov    %rax,%r14
 	cmp    $0xf,%rax
-	ja     e20 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x250>
+	ja     ff0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x250>
 	cmp    $0x1,%rax
-	jne    d40 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x170>
+	jne    f10 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x170>
 	movzbl 0x0(%rbp),%edx
 	mov    %dl,0x60(%rsp)
 	mov    %rbx,%rdx
 	mov    %rax,0x58(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rdx,%rax,1)
 	lea    0x30(%rsp),%rax
 	mov    %r14,0x30(%rsp)
 	mov    %rax,%r13
 	test   %r12,%r12
-	jne    d50 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x180>
+	jne    f20 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x180>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   d37 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x167>
+	call   f07 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x167>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jne    eb3 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2e3>
+	jne    1083 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2e3>
 	mov    %rbx,%rdx
-	jmp    d0b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
+	jmp    edb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   d58 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x188>
+	call   f28 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x188>
  R_X86_64_PLT32	strlen-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,0x28(%rsp)
 	cmp    $0xf,%rax
-	ja     e60 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x290>
+	ja     1030 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x290>
 	cmp    $0x1,%rax
-	jne    e08 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x238>
+	jne    fd8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x238>
 	movzbl (%r12),%edx
 	mov    %dl,0x40(%rsp)
 	mov    %r14,%rdx
 	mov    %rax,0x38(%rsp)
 	mov    0x8(%rsp),%rdi
 	mov    %r13,%rsi
 	movb   $0x0,(%rdx,%rax,1)
 	mov    %r15,%rdx
-	call   d9b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1cb>
+	call   f6b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1cb>
  R_X86_64_PLT32	arithmetica::Fraction::Fraction(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&, std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     db3 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
+	je     f83 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   db3 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
+	call   f83 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1e3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     dcb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
+	je     f9b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   dcb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
+	call   f9b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1fb>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
 	mov    %rbp,%rsi
-	call   dd6 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x206>
+	call   fa6 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x206>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x78(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    e9d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2cd>
+	jne    106d <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2cd>
 	mov    0x8(%rsp),%rax
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x10(%rsp)
-	jne    eae <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
+	jne    107e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
 	mov    %r14,%rdx
-	jmp    d82 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
+	jmp    f52 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
-	call   e2f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x25f>
+	call   fff <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x25f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x50(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x60(%rsp)
 	mov    %r14,%rdx
 	mov    %rbp,%rsi
-	call   e4c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x27c>
+	call   101c <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x27c>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x50(%rsp),%rdx
-	jmp    d0b <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
+	jmp    edb <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x13b>
 	nopl   0x0(%rax,%rax,1)
 	lea    0x28(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r13,%rdi
-	call   e6f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x29f>
+	call   103f <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x29f>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x28(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    0x10(%rsp),%rdx
 	mov    %r12,%rsi
-	call   e8e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2be>
+	call   105e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2be>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rax
 	mov    0x30(%rsp),%rdx
-	jmp    d82 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
-	call   ea2 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
+	jmp    f52 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x1b2>
+	call   1072 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2d2>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   eae <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
+	call   107e <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2de>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    e81 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2b1>
+	jmp    1051 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2b1>
 	mov    %rbx,%rdi
-	jmp    e41 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x271>
+	jmp    1011 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x271>
 	endbr64
 	mov    %rax,%rbp
-	jmp    ec4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2f4>
- R_X86_64_PC32	.text.unlikely+0x1b0
+	jmp    1094 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x2f4>
+ R_X86_64_PC32	.text.unlikely+0x1d0
 	endbr64
 	mov    %rax,%rbp
-	jmp    ed0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x300>
- R_X86_64_PC32	.text.unlikely+0x198
+	jmp    10a0 <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x300>
+ R_X86_64_PC32	.text.unlikely+0x1b8
 	endbr64
 	mov    %rax,%rbp
-	jmp    edc <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x30c>
- R_X86_64_PC32	.text.unlikely+0x1ca
+	jmp    10ac <arithmetica::Fraction::operator/(arithmetica::Fraction const&)+0x30c>
+ R_X86_64_PC32	.text.unlikely+0x1ea
 	nopl   0x0(%rax)
 
-0000000000000ee0 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)>:
+00000000000010b0 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)>:
 arithmetica::Fraction::operator==(arithmetica::Fraction const&):
 	endbr64
 	push   %r13
 	lea    0x0(%rip),%r13        
- R_X86_64_PC32	.LC9-0x4
+ R_X86_64_PC32	.LC12-0x4
 	push   %r12
 	lea    0x0(%rip),%r12        
- R_X86_64_PC32	.LC10-0x4
+ R_X86_64_PC32	.LC13-0x4
 	push   %rbp
 	mov    %rsi,%rbp
 	mov    %r13,%rsi
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
-	call   f0a <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x2a>
+	call   10da <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x2a>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    f21 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x41>
+	jne    10f1 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x41>
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
-	call   f19 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x39>
+	call   10e9 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x39>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     f9f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
+	je     116f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
 	mov    %r12,%rsi
 	mov    %rbx,%rdi
-	call   f2c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x4c>
+	call   10fc <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x4c>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     f90 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xb0>
+	je     1160 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xb0>
 	mov    0x8(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x8(%rbp),%rdx
-	je     f50 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x70>
+	je     1120 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x70>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
 	mov    0x0(%rbp),%rsi
 	test   %rdx,%rdx
-	je     f6b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x8b>
-	call   f61 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x81>
+	je     113b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x8b>
+	call   1131 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x81>
  R_X86_64_PLT32	memcmp-0x4
 	mov    %eax,%r8d
 	xor    %eax,%eax
 	test   %r8d,%r8d
-	jne    f3c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
+	jne    110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
 	mov    0x28(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x28(%rbp),%rdx
-	jne    f3c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
+	jne    110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
 	mov    0x20(%rbx),%rdi
 	mov    0x20(%rbp),%rsi
 	test   %rdx,%rdx
-	je     f9f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
-	call   f89 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xa9>
+	je     116f <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbf>
+	call   1159 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xa9>
  R_X86_64_PLT32	memcmp-0x4
 	test   %eax,%eax
 	sete   %al
-	jmp    f3c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
+	jmp    110c <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x5c>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
-	call   f9b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbb>
+	call   116b <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0xbb>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    f30 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x50>
+	jne    1100 <arithmetica::Fraction::operator==(arithmetica::Fraction const&)+0x50>
 	add    $0x8,%rsp
 	mov    $0x1,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nop
 
-0000000000000fb0 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
+0000000000001180 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
 operator==(arithmetica::Fraction const&, arithmetica::Fraction const&):
 	endbr64
 	push   %r13
 	lea    0x0(%rip),%r13        
- R_X86_64_PC32	.LC9-0x4
+ R_X86_64_PC32	.LC12-0x4
 	push   %r12
 	lea    0x0(%rip),%r12        
- R_X86_64_PC32	.LC10-0x4
+ R_X86_64_PC32	.LC13-0x4
 	push   %rbp
 	mov    %rsi,%rbp
 	mov    %r13,%rsi
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
-	call   fda <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x2a>
+	call   11aa <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x2a>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    ff1 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x41>
+	jne    11c1 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x41>
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
-	call   fe9 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x39>
+	call   11b9 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x39>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     106f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
+	je     123f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
 	mov    %r12,%rsi
 	mov    %rbx,%rdi
-	call   ffc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x4c>
+	call   11cc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x4c>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	je     1060 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xb0>
+	je     1230 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xb0>
 	mov    0x8(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x8(%rbp),%rdx
-	je     1020 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x70>
+	je     11f0 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x70>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
 	mov    0x0(%rbp),%rsi
 	test   %rdx,%rdx
-	je     103b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x8b>
-	call   1031 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x81>
+	je     120b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x8b>
+	call   1201 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x81>
  R_X86_64_PLT32	memcmp-0x4
 	mov    %eax,%r8d
 	xor    %eax,%eax
 	test   %r8d,%r8d
-	jne    100c <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
+	jne    11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
 	mov    0x28(%rbx),%rdx
 	xor    %eax,%eax
 	cmp    0x28(%rbp),%rdx
-	jne    100c <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
+	jne    11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
 	mov    0x20(%rbx),%rdi
 	mov    0x20(%rbp),%rsi
 	test   %rdx,%rdx
-	je     106f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
-	call   1059 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa9>
+	je     123f <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbf>
+	call   1229 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa9>
  R_X86_64_PLT32	memcmp-0x4
 	test   %eax,%eax
 	sete   %al
-	jmp    100c <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
+	jmp    11dc <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x5c>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
-	call   106b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbb>
+	call   123b <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xbb>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
 	test   %eax,%eax
-	jne    1000 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
+	jne    11d0 <operator==(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
 	add    $0x8,%rsp
 	mov    $0x1,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nop
 
-0000000000001080 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
+0000000000001250 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)>:
 operator<(arithmetica::Fraction const&, arithmetica::Fraction const&):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	mov    %rsi,%r13
 	push   %r12
@@ -1308,157 +1436,157 @@
 	mov    %fs:0x28,%rax
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	lea    0x20(%rsp),%rbp
 	mov    %r14,%rax
 	mov    %rbp,0x10(%rsp)
 	add    %r12,%rax
-	je     10d0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
+	je     12a0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x50>
 	test   %r14,%r14
-	je     12bd <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x23d>
+	je     148d <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x23d>
 	mov    %r12,0x8(%rsp)
 	cmp    $0xf,%r12
-	ja     1240 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1c0>
+	ja     1410 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1c0>
 	cmp    $0x1,%r12
-	jne    1210 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x190>
+	jne    13e0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x190>
 	movzbl (%r14),%eax
 	mov    %al,0x20(%rsp)
 	mov    %rbp,%rax
 	mov    %r12,0x18(%rsp)
 	lea    0x40(%rsp),%r14
 	movb   $0x0,(%rax,%r12,1)
 	mov    0x20(%rbx),%r15
 	mov    0x28(%rbx),%r12
 	mov    %r14,0x30(%rsp)
 	mov    %r15,%rax
 	add    %r12,%rax
-	je     1121 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa1>
+	je     12f1 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xa1>
 	test   %r15,%r15
-	je     12ce <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
+	je     149e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
 	mov    %r12,0x8(%rsp)
 	cmp    $0xf,%r12
-	ja     1280 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x200>
+	ja     1450 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x200>
 	cmp    $0x1,%r12
-	jne    1228 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1a8>
+	jne    13f8 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1a8>
 	movzbl (%r15),%eax
 	mov    %al,0x40(%rsp)
 	mov    %r14,%rax
 	mov    %r12,0x38(%rsp)
 	lea    0x50(%rsp),%rdi
 	mov    %r13,%rdx
 	movb   $0x0,(%rax,%r12,1)
 	lea    0x10(%rsp),%r12
 	mov    %r12,%rsi
-	call   1164 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xe4>
+	call   1334 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xe4>
  R_X86_64_PLT32	arithmetica::Fraction::operator-(arithmetica::Fraction const&)-0x4
 	mov    0x50(%rsp),%rdi
 	mov    0x70(%rsp),%r8
 	lea    0x80(%rsp),%rax
 	cmpb   $0x2d,(%rdi)
 	sete   %r12b
 	cmp    %rax,%r8
-	je     119b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x11b>
+	je     136b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x11b>
 	mov    0x80(%rsp),%rax
 	mov    %r8,%rdi
 	lea    0x1(%rax),%rsi
-	call   1196 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x116>
+	call   1366 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x116>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	lea    0x60(%rsp),%rax
 	cmp    %rax,%rdi
-	je     11b3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
+	je     1383 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   11b3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
+	call   1383 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x133>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     11cb <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
+	je     139b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   11cb <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
+	call   139b <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x14b>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x10(%rsp),%rdi
 	cmp    %rbp,%rdi
-	je     11e3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
+	je     13b3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   11e3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
+	call   13b3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x163>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x98(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    12c9 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
+	jne    1499 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
 	add    $0xa8,%rsp
 	mov    %r12d,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nop
 	test   %r12,%r12
-	jne    12df <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25f>
+	jne    14af <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25f>
 	mov    %rbp,%rax
-	jmp    10f4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
+	jmp    12c4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
 	nopl   0x0(%rax)
 	test   %r12,%r12
-	jne    12da <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
+	jne    14aa <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
 	mov    %r14,%rax
-	jmp    1145 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
+	jmp    1315 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
 	nopl   0x0(%rax)
 	lea    0x10(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
 	xor    %edx,%edx
-	call   1251 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1d1>
+	call   1421 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1d1>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x20(%rsp)
 	mov    %r12,%rdx
 	mov    %r14,%rsi
-	call   126e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1ee>
+	call   143e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1ee>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r12
 	mov    0x10(%rsp),%rax
-	jmp    10f4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
+	jmp    12c4 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x74>
 	nopl   (%rax)
 	lea    0x8(%rsp),%rsi
 	lea    0x30(%rsp),%rdi
 	xor    %edx,%edx
-	call   1291 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x211>
+	call   1461 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x211>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    %r12,%rdx
 	mov    %r15,%rsi
-	call   12ae <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x22e>
+	call   147e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x22e>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r12
 	mov    0x30(%rsp),%rax
-	jmp    1145 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
+	jmp    1315 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0xc5>
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   12c9 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
+	call   1499 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x249>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
-	call   12ce <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
+	call   149e <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x24e>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC4-0x4
-	call   12da <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
+	call   14aa <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x25a>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	mov    %r14,%rdi
-	jmp    12a3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x223>
+	jmp    1473 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x223>
 	mov    %rbp,%rdi
-	jmp    1263 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1e3>
+	jmp    1433 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x1e3>
 	endbr64
 	mov    %rax,%r12
-	jmp    12f3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x273>
- R_X86_64_PC32	.text.unlikely+0x1dc
+	jmp    14c3 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x273>
+ R_X86_64_PC32	.text.unlikely+0x1fc
 	endbr64
 	mov    %rax,%rbp
-	jmp    12ff <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x27f>
- R_X86_64_PC32	.text.unlikely+0x1fc
+	jmp    14cf <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&)+0x27f>
+ R_X86_64_PC32	.text.unlikely+0x21c
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text.unlikely {}

```diff
@@ -83,121 +83,134 @@
 	call   c7 <arithmetica::Fraction::Fraction(fraction const&) [clone .cold]+0x2b>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %rbp,%rdi
 	call   cf <arithmetica::Fraction::Fraction(fraction const&) [clone .cold]+0x33>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 	nop
 
-00000000000000d0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]>:
+00000000000000d0 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]>:
+arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]:
+	mov    0x10(%rsp),%rdi
+	cmp    %rbp,%rdi
+	je     e8 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x18>
+	mov    0x20(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   e8 <arithmetica::Fraction::to_string[abi:cxx11]() [clone .cold]+0x18>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    %r12,%rdi
+	call   f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]>
+ R_X86_64_PLT32	_Unwind_Resume-0x4
+
+00000000000000f0 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     e8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     108 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   e8 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   108 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     10c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     12c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   100 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   120 <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    10c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    12c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   10c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   12c <arithmetica::Fraction::operator+(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   114 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>
+	call   134 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-0000000000000114 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>:
+0000000000000134 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     12c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     14c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   12c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   14c <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     150 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     170 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   144 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   164 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    150 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    170 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   150 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   170 <arithmetica::Fraction::operator-(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   158 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>
+	call   178 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-0000000000000158 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>:
+0000000000000178 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     170 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     190 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   170 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   190 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     194 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     1b4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   188 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   1a8 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    194 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    1b4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   194 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   1b4 <arithmetica::Fraction::operator*(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   19c <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>
+	call   1bc <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-000000000000019c <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>:
+00000000000001bc <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]>:
 arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]:
 	mov    0x30(%rsp),%rdi
 	cmp    %r14,%rdi
-	je     1b4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     1d4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1b4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   1d4 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x50(%rsp),%rdi
 	cmp    %rbx,%rdi
-	je     1d8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	je     1f8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x60(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1cc <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x30>
+	call   1ec <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    1d8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	jmp    1f8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
 	mov    0x8(%rsp),%rdi
-	call   1d8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
+	call   1f8 <arithmetica::Fraction::operator/(arithmetica::Fraction const&) [clone .cold]+0x3c>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   1e0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>
+	call   200 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 
-00000000000001e0 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>:
+0000000000000200 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]>:
 operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]:
 	mov    0x10(%rsp),%rdi
 	cmp    %rbp,%rdi
-	je     1f8 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
+	je     218 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1f8 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
+	call   218 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x18>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
-	call   200 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x20>
+	call   220 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x20>
  R_X86_64_PLT32	_Unwind_Resume-0x4
 	mov    %r12,%rdi
-	call   208 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x28>
+	call   228 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x28>
  R_X86_64_PLT32	arithmetica::Fraction::~Fraction()-0x4
 	mov    %rbp,%rdi
-	call   210 <arithmetica::Fraction::Fraction(fraction const&)+0x10>
+	call   230 <operator<(arithmetica::Fraction const&, arithmetica::Fraction const&) [clone .cold]+0x30>
  R_X86_64_PLT32	_Unwind_Resume-0x4
```

##### readelf --wide --decompress --hex-dump=.gcc_except_table {}

```diff
@@ -1,23 +1,25 @@
 
 Hex dump of section '.gcc_except_table':
   0x00000000 ffff0104 39145600 ffff0104 2e050000 ....9.V.........
   0x00000010 ffff0105 3f52a001 00ffff01 042e0500 ....?R..........
   0x00000020 00ffff01 053f52a0 0100ffff 01042e05 .....?R.........
   0x00000030 0000ffff 01055729 8f0100ff ff01042e ......W)........
-  0x00000040 050000ff ff0127d7 01260000 e20205e8 ......'..&......
-  0x00000050 0500c603 05f40500 81040580 0600da04 ................
-  0x00000060 0500009a 0505e805 00d90505 0000ffff ................
-  0x00000070 01043f05 0000ffff 0127d701 260000e2 ..?......'..&...
-  0x00000080 0205e805 00c60305 f4050081 04058006 ................
-  0x00000090 00da0405 00009a05 05e80500 d9050500 ................
-  0x000000a0 00ffff01 043f0500 00ffff01 27d70126 .....?......'..&
-  0x000000b0 0000e202 05e80500 c60305f4 05008104 ................
-  0x000000c0 05800600 da040500 009a0505 e80500d9 ................
-  0x000000d0 05050000 ffff0104 3f050000 ffff0127 ........?......'
-  0x000000e0 d7012600 00e20205 e80500c6 0305f405 ..&.............
-  0x000000f0 00810405 800600da 04050000 9a0505e8 ................
-  0x00000100 0500d905 050000ff ff01043f 050000ff ...........?....
-  0x00000110 ff011cdf 0105f304 00cc0305 00008c04 ................
-  0x00000120 05e70400 c4040500 00d50405 e70400ff ................
-  0x00000130 ff01041b 150000                     .......
+  0x00000040 050000ff ff01179f 0105be03 00af0105 ................
+  0x00000050 b20300cc 02500000 a30305be 0300ffff .....P..........
+  0x00000060 01041b05 0000ffff 0127d701 260000e2 .........'..&...
+  0x00000070 0205e805 00c60305 f4050081 04058006 ................
+  0x00000080 00da0405 00009a05 05e80500 d9050500 ................
+  0x00000090 00ffff01 043f0500 00ffff01 27d70126 .....?......'..&
+  0x000000a0 0000e202 05e80500 c60305f4 05008104 ................
+  0x000000b0 05800600 da040500 009a0505 e80500d9 ................
+  0x000000c0 05050000 ffff0104 3f050000 ffff0127 ........?......'
+  0x000000d0 d7012600 00e20205 e80500c6 0305f405 ..&.............
+  0x000000e0 00810405 800600da 04050000 9a0505e8 ................
+  0x000000f0 0500d905 050000ff ff01043f 050000ff ...........?....
+  0x00000100 ff0127d7 01260000 e20205e8 0500c603 ..'..&..........
+  0x00000110 05f40500 81040580 0600da04 0500009a ................
+  0x00000120 0505e805 00d90505 0000ffff 01043f05 ..............?.
+  0x00000130 0000ffff 011cdf01 05f30400 cc030500 ................
+  0x00000140 008c0405 e70400c4 04050000 d50405e7 ................
+  0x00000150 0400ffff 01041b15 0000              ..........
```

##### readelf --wide --decompress --string-dump=.rodata.str1.1 {}

```diff
@@ -1,5 +1,7 @@
 
 String dump of section '.rodata.str1.1':
-  [     0]  -0
-  [     3]  0
+  [     0]  basic_string::append
+  [    15]  /
+  [    17]  -0
+  [    1a]  0
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -29,58 +29,65 @@
   0x00000190 058d048e 038f0200 4c000000 70010000 ........L...p...
   0x000001a0 00000000 9b000000 04000000 00460e10 .............F..
   0x000001b0 8f02420e 188e0346 0e208d04 460e288c ..B....F. ..F.(.
   0x000001c0 05410e30 8606440e 38830747 0e400264 .A.0..D.8..G.@.d
   0x000001d0 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
   0x000001e0 0e10420e 08410b00 20000000 c0010000 ..B..A.. .......
   0x000001f0 00000000 33000000 04000000 000e4083 ....3.........@.
-  0x00000200 0786068c 058d048e 038f0200 1c000000 ................
-  0x00000210 10020000 00000000 42000000 00450e10 ........B....E..
-  0x00000220 83026e0a 0e084d0b 410e0800 50000000 ..n...M.A...P...
-  0x00000230 04020000 00000000 0c030000 04000000 ................
-  0x00000240 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
-  0x00000250 420e288c 05410e30 8606440e 3883074a B.(..A.0..D.8..J
-  0x00000260 0ec00103 0b020a0e 38410e30 410e2842 ........8A.0A.(B
-  0x00000270 0e20420e 18420e10 420e0848 0b000000 . B..B..B..H....
-  0x00000280 20000000 58020000 00000000 44000000  ...X.......D...
-  0x00000290 04000000 000ec001 83078606 8c058d04 ................
-  0x000002a0 8e038f02 50000000 7c020000 00000000 ....P...|.......
-  0x000002b0 0c030000 04000000 00460e10 8f02420e .........F....B.
-  0x000002c0 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
-  0x000002d0 8606440e 3883074a 0ec00103 0b020a0e ..D.8..J........
-  0x000002e0 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
-  0x000002f0 420e0848 0b000000 20000000 d0020000 B..H.... .......
-  0x00000300 00000000 44000000 04000000 000ec001 ....D...........
-  0x00000310 83078606 8c058d04 8e038f02 50000000 ............P...
-  0x00000320 f4020000 00000000 0c030000 04000000 ................
-  0x00000330 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
-  0x00000340 420e288c 05410e30 8606440e 3883074a B.(..A.0..D.8..J
-  0x00000350 0ec00103 0b020a0e 38410e30 410e2842 ........8A.0A.(B
-  0x00000360 0e20420e 18420e10 420e0848 0b000000 . B..B..B..H....
-  0x00000370 20000000 48030000 00000000 44000000  ...H.......D...
-  0x00000380 04000000 000ec001 83078606 8c058d04 ................
-  0x00000390 8e038f02 50000000 6c030000 00000000 ....P...l.......
-  0x000003a0 0c030000 04000000 00460e10 8f02420e .........F....B.
-  0x000003b0 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
-  0x000003c0 8606440e 3883074a 0ec00103 0b020a0e ..D.8..J........
-  0x000003d0 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
-  0x000003e0 420e0848 0b000000 20000000 c0030000 B..H.... .......
-  0x000003f0 00000000 44000000 04000000 000ec001 ....D...........
-  0x00000400 83078606 8c058d04 8e038f02 48000000 ............H...
-  0x00000410 10040000 00000000 cf000000 00460e10 .............F..
-  0x00000420 8d02490e 188c0348 0e208604 470e2883 ..I....H. ..G.(.
-  0x00000430 05470e30 7b0a0e28 410e2041 0e18420e .G.0{..(A. A..B.
-  0x00000440 10420e08 4a0b0253 0e28460e 20410e18 .B..J..S.(F. A..
-  0x00000450 420e1042 0e080000 48000000 5c040000 B..B....H...\...
-  0x00000460 00000000 cf000000 00460e10 8d02490e .........F....I.
-  0x00000470 188c0348 0e208604 470e2883 05470e30 ...H. ..G.(..G.0
-  0x00000480 7b0a0e28 410e2041 0e18420e 10420e08 {..(A. A..B..B..
-  0x00000490 4a0b0253 0e28460e 20410e18 420e1042 J..S.(F. A..B..B
-  0x000004a0 0e080000 50000000 7c040000 00000000 ....P...|.......
-  0x000004b0 7f020000 04000000 00460e10 8f02420e .........F....B.
-  0x000004c0 188e0342 0e208d04 450e288c 05410e30 ...B. ..E.(..A.0
-  0x000004d0 8606410e 3883074a 0ee00103 66010a0e ..A.8..J....f...
-  0x000004e0 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
-  0x000004f0 420e0842 0b000000 24000000 d0040000 B..B....$.......
-  0x00000500 00000000 30000000 04000000 000ee001 ....0...........
-  0x00000510 83078606 8c058d04 8e038f02 00000000 ................
+  0x00000200 0786068c 058d048e 038f0200 44000000 ............D...
+  0x00000210 e4010000 00000000 ca010000 04000000 ................
+  0x00000220 00460e10 8e02420e 188d0342 0e208c04 .F....B....B. ..
+  0x00000230 440e2886 05410e30 8306470e 70030c01 D.(..A.0..G.p...
+  0x00000240 0a0e3044 0e28410e 20420e18 420e1042 ..0D.(A. B..B..B
+  0x00000250 0e08430b 20000000 2c020000 00000000 ..C. ...,.......
+  0x00000260 20000000 04000000 000e7083 0686058c  .........p.....
+  0x00000270 048d038e 02000000 1c000000 7c020000 ............|...
+  0x00000280 00000000 42000000 00450e10 83026e0a ....B....E....n.
+  0x00000290 0e084d0b 410e0800 50000000 70020000 ..M.A...P...p...
+  0x000002a0 00000000 0c030000 04000000 00460e10 .............F..
+  0x000002b0 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
+  0x000002c0 05410e30 8606440e 3883074a 0ec00103 .A.0..D.8..J....
+  0x000002d0 0b020a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
+  0x000002e0 18420e10 420e0848 0b000000 20000000 .B..B..H.... ...
+  0x000002f0 c4020000 00000000 44000000 04000000 ........D.......
+  0x00000300 000ec001 83078606 8c058d04 8e038f02 ................
+  0x00000310 50000000 e8020000 00000000 0c030000 P...............
+  0x00000320 04000000 00460e10 8f02420e 188e0342 .....F....B....B
+  0x00000330 0e208d04 420e288c 05410e30 8606440e . ..B.(..A.0..D.
+  0x00000340 3883074a 0ec00103 0b020a0e 38410e30 8..J........8A.0
+  0x00000350 410e2842 0e20420e 18420e10 420e0848 A.(B. B..B..B..H
+  0x00000360 0b000000 20000000 3c030000 00000000 .... ...<.......
+  0x00000370 44000000 04000000 000ec001 83078606 D...............
+  0x00000380 8c058d04 8e038f02 50000000 60030000 ........P...`...
+  0x00000390 00000000 0c030000 04000000 00460e10 .............F..
+  0x000003a0 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
+  0x000003b0 05410e30 8606440e 3883074a 0ec00103 .A.0..D.8..J....
+  0x000003c0 0b020a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
+  0x000003d0 18420e10 420e0848 0b000000 20000000 .B..B..H.... ...
+  0x000003e0 b4030000 00000000 44000000 04000000 ........D.......
+  0x000003f0 000ec001 83078606 8c058d04 8e038f02 ................
+  0x00000400 50000000 d8030000 00000000 0c030000 P...............
+  0x00000410 04000000 00460e10 8f02420e 188e0342 .....F....B....B
+  0x00000420 0e208d04 420e288c 05410e30 8606440e . ..B.(..A.0..D.
+  0x00000430 3883074a 0ec00103 0b020a0e 38410e30 8..J........8A.0
+  0x00000440 410e2842 0e20420e 18420e10 420e0848 A.(B. B..B..B..H
+  0x00000450 0b000000 20000000 2c040000 00000000 .... ...,.......
+  0x00000460 44000000 04000000 000ec001 83078606 D...............
+  0x00000470 8c058d04 8e038f02 48000000 7c040000 ........H...|...
+  0x00000480 00000000 cf000000 00460e10 8d02490e .........F....I.
+  0x00000490 188c0348 0e208604 470e2883 05470e30 ...H. ..G.(..G.0
+  0x000004a0 7b0a0e28 410e2041 0e18420e 10420e08 {..(A. A..B..B..
+  0x000004b0 4a0b0253 0e28460e 20410e18 420e1042 J..S.(F. A..B..B
+  0x000004c0 0e080000 48000000 c8040000 00000000 ....H...........
+  0x000004d0 cf000000 00460e10 8d02490e 188c0348 .....F....I....H
+  0x000004e0 0e208604 470e2883 05470e30 7b0a0e28 . ..G.(..G.0{..(
+  0x000004f0 410e2041 0e18420e 10420e08 4a0b0253 A. A..B..B..J..S
+  0x00000500 0e28460e 20410e18 420e1042 0e080000 .(F. A..B..B....
+  0x00000510 50000000 e8040000 00000000 7f020000 P...............
+  0x00000520 04000000 00460e10 8f02420e 188e0342 .....F....B....B
+  0x00000530 0e208d04 450e288c 05410e30 8606410e . ..E.(..A.0..A.
+  0x00000540 3883074a 0ee00103 66010a0e 38440e30 8..J....f...8D.0
+  0x00000550 410e2842 0e20420e 18420e10 420e0842 A.(B. B..B..B..B
+  0x00000560 0b000000 20000000 3c050000 00000000 .... ...<.......
+  0x00000570 30000000 04000000 000ee001 83078606 0...............
+  0x00000580 8c058d04 8e038f02                   ........
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -14,106 +14,119 @@
   0x000000b0 73496345 53614963 4545452e 636f6c64 sIcESaIcEEE.cold
   0x000000c0 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
   0x000000d0 61384672 61637469 6f6e4332 45504b63 a8FractionC2EPKc
   0x000000e0 2e636f6c 64005f5a 4e313161 72697468 .cold._ZN11arith
   0x000000f0 6d657469 63613846 72616374 696f6e43 metica8FractionC
   0x00000100 3245524b 38667261 6374696f 6e2e636f 2ERK8fraction.co
   0x00000110 6c64005f 5a4e3131 61726974 686d6574 ld._ZN11arithmet
-  0x00000120 69636138 46726163 74696f6e 706c4552 ica8FractionplER
-  0x00000130 4b53305f 2e636f6c 64005f5a 4e313161 KS0_.cold._ZN11a
-  0x00000140 72697468 6d657469 63613846 72616374 rithmetica8Fract
-  0x00000150 696f6e6d 6945524b 53305f2e 636f6c64 ionmiERKS0_.cold
-  0x00000160 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
-  0x00000170 61384672 61637469 6f6e6d6c 45524b53 a8FractionmlERKS
-  0x00000180 305f2e63 6f6c6400 5f5a4e31 31617269 0_.cold._ZN11ari
-  0x00000190 74686d65 74696361 38467261 6374696f thmetica8Fractio
-  0x000001a0 6e647645 524b5330 5f2e636f 6c64005f ndvERKS0_.cold._
-  0x000001b0 5a6c7452 4b4e3131 61726974 686d6574 ZltRKN11arithmet
-  0x000001c0 69636138 46726163 74696f6e 4553325f ica8FractionES2_
-  0x000001d0 2e636f6c 64002e4c 4334002e 4c433900 .cold..LC4..LC9.
-  0x000001e0 2e4c4331 30005f5a 4e313161 72697468 .LC10._ZN11arith
-  0x000001f0 6d657469 63613846 72616374 696f6e44 metica8FractionD
-  0x00000200 35457600 5f5a4e31 31617269 74686d65 5Ev._ZN11arithme
-  0x00000210 74696361 38467261 6374696f 6e433245 tica8FractionC2E
-  0x00000220 76005f5a 4e313161 72697468 6d657469 v._ZN11arithmeti
-  0x00000230 63613846 72616374 696f6e43 31457600 ca8FractionC1Ev.
-  0x00000240 5f5a4e31 31617269 74686d65 74696361 _ZN11arithmetica
-  0x00000250 38467261 6374696f 6e433245 524b4e53 8FractionC2ERKNS
-  0x00000260 74375f5f 63787831 31313262 61736963 t7__cxx1112basic
-  0x00000270 5f737472 696e6749 63537431 31636861 _stringIcSt11cha
-  0x00000280 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
-  0x00000290 45455338 5f004457 2e726566 2e5f5f67 EES8_.DW.ref.__g
-  0x000002a0 78785f70 6572736f 6e616c69 74795f76 xx_personality_v
-  0x000002b0 30005f5a 4e537437 5f5f6378 78313131 0._ZNSt7__cxx111
-  0x000002c0 32626173 69635f73 7472696e 67496353 2basic_stringIcS
-  0x000002d0 74313163 6861725f 74726169 74734963 t11char_traitsIc
-  0x000002e0 45536149 63454539 5f4d5f61 73736967 ESaIcEE9_M_assig
-  0x000002f0 6e45524b 53345f00 5f5a646c 50766d00 nERKS4_._ZdlPvm.
-  0x00000300 5f556e77 696e645f 52657375 6d65005f _Unwind_Resume._
-  0x00000310 5a4e3131 61726974 686d6574 69636138 ZN11arithmetica8
-  0x00000320 46726163 74696f6e 43314552 4b4e5374 FractionC1ERKNSt
-  0x00000330 375f5f63 78783131 31326261 7369635f 7__cxx1112basic_
-  0x00000340 73747269 6e674963 53743131 63686172 stringIcSt11char
-  0x00000350 5f747261 69747349 63455361 49634545 _traitsIcESaIcEE
-  0x00000360 4553385f 005f5a4e 31316172 6974686d ES8_._ZN11arithm
-  0x00000370 65746963 61384672 61637469 6f6e4332 etica8FractionC2
-  0x00000380 45524b4e 5374375f 5f637878 31313132 ERKNSt7__cxx1112
-  0x00000390 62617369 635f7374 72696e67 49635374 basic_stringIcSt
-  0x000003a0 31316368 61725f74 72616974 73496345 11char_traitsIcE
-  0x000003b0 53614963 45454500 70617273 655f6672 SaIcEEE.parse_fr
-  0x000003c0 61637469 6f6e0073 74726c65 6e005f5a action.strlen._Z
-  0x000003d0 4e537437 5f5f6378 78313131 32626173 NSt7__cxx1112bas
-  0x000003e0 69635f73 7472696e 67496353 74313163 ic_stringIcSt11c
-  0x000003f0 6861725f 74726169 74734963 45536149 har_traitsIcESaI
-  0x00000400 63454531 305f4d5f 7265706c 61636545 cEE10_M_replaceE
-  0x00000410 6d6d504b 636d0064 656c6574 655f6672 mmPKcm.delete_fr
-  0x00000420 61637469 6f6e005f 5a4e3131 61726974 action._ZN11arit
-  0x00000430 686d6574 69636138 46726163 74696f6e hmetica8Fraction
-  0x00000440 43314552 4b4e5374 375f5f63 78783131 C1ERKNSt7__cxx11
-  0x00000450 31326261 7369635f 73747269 6e674963 12basic_stringIc
-  0x00000460 53743131 63686172 5f747261 69747349 St11char_traitsI
-  0x00000470 63455361 49634545 45005f5a 4e313161 cESaIcEEE._ZN11a
-  0x00000480 72697468 6d657469 63613846 72616374 rithmetica8Fract
-  0x00000490 696f6e43 3245504b 63005f5a 4e313161 ionC2EPKc._ZN11a
-  0x000004a0 72697468 6d657469 63613846 72616374 rithmetica8Fract
-  0x000004b0 696f6e43 3145504b 63005f5a 4e313161 ionC1EPKc._ZN11a
-  0x000004c0 72697468 6d657469 63613846 72616374 rithmetica8Fract
-  0x000004d0 696f6e43 3245524b 38667261 6374696f ionC2ERK8fractio
-  0x000004e0 6e005f5a 4e313161 72697468 6d657469 n._ZN11arithmeti
-  0x000004f0 63613846 72616374 696f6e43 3145524b ca8FractionC1ERK
-  0x00000500 38667261 6374696f 6e005f5a 4e313161 8fraction._ZN11a
-  0x00000510 72697468 6d657469 63613846 72616374 rithmetica8Fract
-  0x00000520 696f6e44 32457600 5f5a4e31 31617269 ionD2Ev._ZN11ari
-  0x00000530 74686d65 74696361 38467261 6374696f thmetica8Fractio
-  0x00000540 6e443145 76005f5a 4e313161 72697468 nD1Ev._ZN11arith
-  0x00000550 6d657469 63613846 72616374 696f6e70 metica8Fractionp
-  0x00000560 6c45524b 53305f00 63616c6c 6f630073 lERKS0_.calloc.s
-  0x00000570 74726370 79006164 645f6672 61637469 trcpy.add_fracti
-  0x00000580 6f6e005f 5a537431 395f5f74 68726f77 on._ZSt19__throw
-  0x00000590 5f6c6f67 69635f65 72726f72 504b6300 _logic_errorPKc.
-  0x000005a0 5f5a4e53 74375f5f 63787831 31313262 _ZNSt7__cxx1112b
-  0x000005b0 61736963 5f737472 696e6749 63537431 asic_stringIcSt1
-  0x000005c0 31636861 725f7472 61697473 49634553 1char_traitsIcES
-  0x000005d0 61496345 45395f4d 5f637265 61746545 aIcEE9_M_createE
-  0x000005e0 526d6d00 6d656d63 7079005f 5f737461 Rmm.memcpy.__sta
-  0x000005f0 636b5f63 686b5f66 61696c00 5f5a4e31 ck_chk_fail._ZN1
-  0x00000600 31617269 74686d65 74696361 38467261 1arithmetica8Fra
-  0x00000610 6374696f 6e6d6945 524b5330 5f007375 ctionmiERKS0_.su
-  0x00000620 62747261 63745f66 72616374 696f6e00 btract_fraction.
-  0x00000630 5f5a4e31 31617269 74686d65 74696361 _ZN11arithmetica
-  0x00000640 38467261 6374696f 6e6d6c45 524b5330 8FractionmlERKS0
-  0x00000650 5f006d75 6c746970 6c795f66 72616374 _.multiply_fract
-  0x00000660 696f6e00 5f5a4e31 31617269 74686d65 ion._ZN11arithme
-  0x00000670 74696361 38467261 6374696f 6e647645 tica8FractiondvE
-  0x00000680 524b5330 5f005f5a 4e313161 72697468 RKS0_._ZN11arith
-  0x00000690 6d657469 63613846 72616374 696f6e65 metica8Fractione
-  0x000006a0 7145524b 53305f00 5f5a4e4b 5374375f qERKS0_._ZNKSt7_
-  0x000006b0 5f637878 31313132 62617369 635f7374 _cxx1112basic_st
-  0x000006c0 72696e67 49635374 31316368 61725f74 ringIcSt11char_t
-  0x000006d0 72616974 73496345 53614963 45453763 raitsIcESaIcEE7c
-  0x000006e0 6f6d7061 72654550 4b63006d 656d636d ompareEPKc.memcm
-  0x000006f0 70005f5a 6571524b 4e313161 72697468 p._ZeqRKN11arith
-  0x00000700 6d657469 63613846 72616374 696f6e45 metica8FractionE
-  0x00000710 53325f00 5f5a6c74 524b4e31 31617269 S2_._ZltRKN11ari
-  0x00000720 74686d65 74696361 38467261 6374696f thmetica8Fractio
-  0x00000730 6e455332 5f00                       nES2_.
+  0x00000120 69636138 46726163 74696f6e 39746f5f ica8Fraction9to_
+  0x00000130 73747269 6e674235 63787831 3145762e stringB5cxx11Ev.
+  0x00000140 636f6c64 005f5a4e 31316172 6974686d cold._ZN11arithm
+  0x00000150 65746963 61384672 61637469 6f6e706c etica8Fractionpl
+  0x00000160 45524b53 305f2e63 6f6c6400 5f5a4e31 ERKS0_.cold._ZN1
+  0x00000170 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x00000180 6374696f 6e6d6945 524b5330 5f2e636f ctionmiERKS0_.co
+  0x00000190 6c64005f 5a4e3131 61726974 686d6574 ld._ZN11arithmet
+  0x000001a0 69636138 46726163 74696f6e 6d6c4552 ica8FractionmlER
+  0x000001b0 4b53305f 2e636f6c 64005f5a 4e313161 KS0_.cold._ZN11a
+  0x000001c0 72697468 6d657469 63613846 72616374 rithmetica8Fract
+  0x000001d0 696f6e64 7645524b 53305f2e 636f6c64 iondvERKS0_.cold
+  0x000001e0 005f5a6c 74524b4e 31316172 6974686d ._ZltRKN11arithm
+  0x000001f0 65746963 61384672 61637469 6f6e4553 etica8FractionES
+  0x00000200 325f2e63 6f6c6400 2e4c4336 002e4c43 2_.cold..LC6..LC
+  0x00000210 34002e4c 4335002e 4c433132 002e4c43 4..LC5..LC12..LC
+  0x00000220 3133005f 5a4e3131 61726974 686d6574 13._ZN11arithmet
+  0x00000230 69636138 46726163 74696f6e 44354576 ica8FractionD5Ev
+  0x00000240 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
+  0x00000250 61384672 61637469 6f6e4332 4576005f a8FractionC2Ev._
+  0x00000260 5a4e3131 61726974 686d6574 69636138 ZN11arithmetica8
+  0x00000270 46726163 74696f6e 43314576 005f5a4e FractionC1Ev._ZN
+  0x00000280 31316172 6974686d 65746963 61384672 11arithmetica8Fr
+  0x00000290 61637469 6f6e4332 45524b4e 5374375f actionC2ERKNSt7_
+  0x000002a0 5f637878 31313132 62617369 635f7374 _cxx1112basic_st
+  0x000002b0 72696e67 49635374 31316368 61725f74 ringIcSt11char_t
+  0x000002c0 72616974 73496345 53614963 45454553 raitsIcESaIcEEES
+  0x000002d0 385f0044 572e7265 662e5f5f 6778785f 8_.DW.ref.__gxx_
+  0x000002e0 70657273 6f6e616c 6974795f 7630005f personality_v0._
+  0x000002f0 5a4e5374 375f5f63 78783131 31326261 ZNSt7__cxx1112ba
+  0x00000300 7369635f 73747269 6e674963 53743131 sic_stringIcSt11
+  0x00000310 63686172 5f747261 69747349 63455361 char_traitsIcESa
+  0x00000320 49634545 395f4d5f 61737369 676e4552 IcEE9_M_assignER
+  0x00000330 4b53345f 005f5a64 6c50766d 005f556e KS4_._ZdlPvm._Un
+  0x00000340 77696e64 5f526573 756d6500 5f5a4e31 wind_Resume._ZN1
+  0x00000350 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x00000360 6374696f 6e433145 524b4e53 74375f5f ctionC1ERKNSt7__
+  0x00000370 63787831 31313262 61736963 5f737472 cxx1112basic_str
+  0x00000380 696e6749 63537431 31636861 725f7472 ingIcSt11char_tr
+  0x00000390 61697473 49634553 61496345 45455338 aitsIcESaIcEEES8
+  0x000003a0 5f005f5a 4e313161 72697468 6d657469 _._ZN11arithmeti
+  0x000003b0 63613846 72616374 696f6e43 3245524b ca8FractionC2ERK
+  0x000003c0 4e537437 5f5f6378 78313131 32626173 NSt7__cxx1112bas
+  0x000003d0 69635f73 7472696e 67496353 74313163 ic_stringIcSt11c
+  0x000003e0 6861725f 74726169 74734963 45536149 har_traitsIcESaI
+  0x000003f0 63454545 00706172 73655f66 72616374 cEEE.parse_fract
+  0x00000400 696f6e00 7374726c 656e005f 5a4e5374 ion.strlen._ZNSt
+  0x00000410 375f5f63 78783131 31326261 7369635f 7__cxx1112basic_
+  0x00000420 73747269 6e674963 53743131 63686172 stringIcSt11char
+  0x00000430 5f747261 69747349 63455361 49634545 _traitsIcESaIcEE
+  0x00000440 31305f4d 5f726570 6c616365 456d6d50 10_M_replaceEmmP
+  0x00000450 4b636d00 64656c65 74655f66 72616374 Kcm.delete_fract
+  0x00000460 696f6e00 5f5a4e31 31617269 74686d65 ion._ZN11arithme
+  0x00000470 74696361 38467261 6374696f 6e433145 tica8FractionC1E
+  0x00000480 524b4e53 74375f5f 63787831 31313262 RKNSt7__cxx1112b
+  0x00000490 61736963 5f737472 696e6749 63537431 asic_stringIcSt1
+  0x000004a0 31636861 725f7472 61697473 49634553 1char_traitsIcES
+  0x000004b0 61496345 4545005f 5a4e3131 61726974 aIcEEE._ZN11arit
+  0x000004c0 686d6574 69636138 46726163 74696f6e hmetica8Fraction
+  0x000004d0 43324550 4b63005f 5a4e3131 61726974 C2EPKc._ZN11arit
+  0x000004e0 686d6574 69636138 46726163 74696f6e hmetica8Fraction
+  0x000004f0 43314550 4b63005f 5a4e3131 61726974 C1EPKc._ZN11arit
+  0x00000500 686d6574 69636138 46726163 74696f6e hmetica8Fraction
+  0x00000510 43324552 4b386672 61637469 6f6e005f C2ERK8fraction._
+  0x00000520 5a4e3131 61726974 686d6574 69636138 ZN11arithmetica8
+  0x00000530 46726163 74696f6e 43314552 4b386672 FractionC1ERK8fr
+  0x00000540 61637469 6f6e005f 5a4e3131 61726974 action._ZN11arit
+  0x00000550 686d6574 69636138 46726163 74696f6e hmetica8Fraction
+  0x00000560 39746f5f 73747269 6e674235 63787831 9to_stringB5cxx1
+  0x00000570 31457600 5f5a4e53 74375f5f 63787831 1Ev._ZNSt7__cxx1
+  0x00000580 31313262 61736963 5f737472 696e6749 112basic_stringI
+  0x00000590 63537431 31636861 725f7472 61697473 cSt11char_traits
+  0x000005a0 49634553 61496345 45395f4d 5f617070 IcESaIcEE9_M_app
+  0x000005b0 656e6445 504b636d 005f5a4e 5374375f endEPKcm._ZNSt7_
+  0x000005c0 5f637878 31313132 62617369 635f7374 _cxx1112basic_st
+  0x000005d0 72696e67 49635374 31316368 61725f74 ringIcSt11char_t
+  0x000005e0 72616974 73496345 53614963 4545395f raitsIcESaIcEE9_
+  0x000005f0 4d5f6372 65617465 45526d6d 006d656d M_createERmm.mem
+  0x00000600 63707900 5f5a5374 31395f5f 7468726f cpy._ZSt19__thro
+  0x00000610 775f6c6f 6769635f 6572726f 72504b63 w_logic_errorPKc
+  0x00000620 005f5a53 7432305f 5f746872 6f775f6c ._ZSt20__throw_l
+  0x00000630 656e6774 685f6572 726f7250 4b63005f ength_errorPKc._
+  0x00000640 5f737461 636b5f63 686b5f66 61696c00 _stack_chk_fail.
+  0x00000650 5f5a4e31 31617269 74686d65 74696361 _ZN11arithmetica
+  0x00000660 38467261 6374696f 6e443245 76005f5a 8FractionD2Ev._Z
+  0x00000670 4e313161 72697468 6d657469 63613846 N11arithmetica8F
+  0x00000680 72616374 696f6e44 31457600 5f5a4e31 ractionD1Ev._ZN1
+  0x00000690 31617269 74686d65 74696361 38467261 1arithmetica8Fra
+  0x000006a0 6374696f 6e706c45 524b5330 5f006361 ctionplERKS0_.ca
+  0x000006b0 6c6c6f63 00737472 63707900 6164645f lloc.strcpy.add_
+  0x000006c0 66726163 74696f6e 005f5a4e 31316172 fraction._ZN11ar
+  0x000006d0 6974686d 65746963 61384672 61637469 ithmetica8Fracti
+  0x000006e0 6f6e6d69 45524b53 305f0073 75627472 onmiERKS0_.subtr
+  0x000006f0 6163745f 66726163 74696f6e 005f5a4e act_fraction._ZN
+  0x00000700 31316172 6974686d 65746963 61384672 11arithmetica8Fr
+  0x00000710 61637469 6f6e6d6c 45524b53 305f006d actionmlERKS0_.m
+  0x00000720 756c7469 706c795f 66726163 74696f6e ultiply_fraction
+  0x00000730 005f5a4e 31316172 6974686d 65746963 ._ZN11arithmetic
+  0x00000740 61384672 61637469 6f6e6476 45524b53 a8FractiondvERKS
+  0x00000750 305f005f 5a4e3131 61726974 686d6574 0_._ZN11arithmet
+  0x00000760 69636138 46726163 74696f6e 65714552 ica8FractioneqER
+  0x00000770 4b53305f 005f5a4e 4b537437 5f5f6378 KS0_._ZNKSt7__cx
+  0x00000780 78313131 32626173 69635f73 7472696e x1112basic_strin
+  0x00000790 67496353 74313163 6861725f 74726169 gIcSt11char_trai
+  0x000007a0 74734963 45536149 63454537 636f6d70 tsIcESaIcEE7comp
+  0x000007b0 61726545 504b6300 6d656d63 6d70005f areEPKc.memcmp._
+  0x000007c0 5a657152 4b4e3131 61726974 686d6574 ZeqRKN11arithmet
+  0x000007d0 69636138 46726163 74696f6e 4553325f ica8FractionES2_
+  0x000007e0 005f5a6c 74524b4e 31316172 6974686d ._ZltRKN11arithm
+  0x000007f0 65746963 61384672 61637469 6f6e4553 etica8FractionES
+  0x00000800 325f00                              2_.
```

##### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -1,19 +1,19 @@
 
 Hex dump of section '.shstrtab':
   0x00000000 002e7379 6d746162 002e7374 72746162 ..symtab..strtab
   0x00000010 002e7368 73747274 6162002e 72656c61 ..shstrtab..rela
   0x00000020 2e746578 74002e64 61746100 2e627373 .text..data..bss
   0x00000030 002e7265 6c612e74 6578742e 756e6c69 ..rela.text.unli
   0x00000040 6b656c79 002e6763 635f6578 63657074 kely..gcc_except
-  0x00000050 5f746162 6c65002e 72656c61 2e746578 _table..rela.tex
-  0x00000060 742e5f5a 4e313161 72697468 6d657469 t._ZN11arithmeti
-  0x00000070 63613846 72616374 696f6e44 32457600 ca8FractionD2Ev.
-  0x00000080 2e726f64 6174612e 73747231 2e38002e .rodata.str1.8..
-  0x00000090 726f6461 74612e73 7472312e 31002e72 rodata.str1.1..r
+  0x00000050 5f746162 6c65002e 726f6461 74612e73 _table..rodata.s
+  0x00000060 7472312e 38002e72 6f646174 612e7374 tr1.8..rodata.st
+  0x00000070 72312e31 002e7265 6c612e74 6578742e r1.1..rela.text.
+  0x00000080 5f5a4e31 31617269 74686d65 74696361 _ZN11arithmetica
+  0x00000090 38467261 6374696f 6e443245 76002e72 8FractionD2Ev..r
   0x000000a0 656c612e 64617461 2e72656c 2e6c6f63 ela.data.rel.loc
   0x000000b0 616c2e44 572e7265 662e5f5f 6778785f al.DW.ref.__gxx_
   0x000000c0 70657273 6f6e616c 6974795f 7630002e personality_v0..
   0x000000d0 636f6d6d 656e7400 2e6e6f74 652e474e comment..note.GN
   0x000000e0 552d7374 61636b00 2e6e6f74 652e676e U-stack..note.gn
   0x000000f0 752e7072 6f706572 7479002e 72656c61 u.property..rela
   0x00000100 2e65685f 6672616d 65002e67 726f7570 .eh_frame..group
```

### Comparing `arithmetica-py-1.0.202/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.203/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.202/src/python-module/module.c` & `arithmetica-py-1.0.203/src/python-module/module.c`

 * *Files identical despite different names*

