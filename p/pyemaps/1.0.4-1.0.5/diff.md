# Comparing `tmp/pyemaps-1.0.4.tar.gz` & `tmp/pyemaps-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-lzse0gda\pyemaps-1.0.4.tar", last modified: Sun May  7 17:11:58 2023, max compression
+gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-cf4xvpon\pyemaps-1.0.5.tar", last modified: Fri May 12 19:13:28 2023, max compression
```

## Comparing `pyemaps-1.0.4.tar` & `pyemaps-1.0.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/
--rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.4/COPYING
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/CifFile/
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/CifFile/src/
--rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.4/CifFile/src/CifFile_module.py
--rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.4/CifFile/src/StarFile.py
--rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/TypeContentsParser.py
--rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_1_0.py
--rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_1_1.py
--rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_2_0.py
--rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_STAR2.py
--rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/
--rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/__init__.py
--rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/drel_ast_yacc.py
--rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/drel_lex.py
--rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/drel_runtime.py
--rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/parsetab.py
--rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/py_from_ast.py
--rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/parsetab.py
--rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/yapps3_compiled_rt.py
--rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      885 2023-05-07 17:11:58.000000 pyemaps-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.4/README.md
--rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.4/__config__.py
--rw-rw-rw-   0        0        0     5814 2023-04-03 21:05:15.000000 pyemaps-1.0.4/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.4/__main__.py
--rw-rw-rw-   0        0        0       21 2023-05-07 17:11:53.000000 pyemaps-1.0.4/__version__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/cdata/
--rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Aluminium.xtl
--rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/AluminiumOxide.xtl
--rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Aluminium_FCC.xtl
--rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BariumTitanate_180k.xtl
--rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BariumTitanate_270k.xtl
--rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BariumTitanate_Tetra.xtl
--rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BiMnO3.xtl
--rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Boron_Tetra.xtl
--rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CadmiumSelenide_Hex.xtl
--rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CadmiumSulfide_Cubic.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CadmiumSulfide_Hex.xtl
--rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Chromium_BCC.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CoSb3_Skutterudite.xtl
--rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CopperOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Copper_FCC.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Cu2O_Cuprite.xtl
--rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Diamond.xtl
--rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/ErbiumPyrogermanate.xtl
--rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/FePd_Tetra.xtl
--rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/FeS2_Pyrite.xtl
--rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/GalliumAntimonide.xtl
--rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/GalliumArsenide.xtl
--rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/GalliumNitride.xtl
--rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Germanium.xtl
--rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Gold_FCC.xtl
--rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/IndiumArsenide.xtl
--rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/LaMnO3.xtl
--rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/LeadZirconateTitanate.xtl
--rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Li2MnO3.xtl
--rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/NaFeO2.xtl
--rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Nb3Sn.xtl
--rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Pentacene.xtl
--rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.4/cdata/SiAlONa.xtl
--rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Silicon.xtl
--rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/StrontiumTitanate.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TelluriumDioxide.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TinDioxide_RT.xtl
--rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TitaniumDioxide_Anatase.xtl
--rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TitaniumDioxide_Rutile.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TungstenDiselenide.xtl
--rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/VanadiumDioxide_RT.xtl
--rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/ZincOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Zinc_HCP.xtl
--rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/ZirconiumNitride.xtl
--rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/limno2.xtl
--rw-rw-rw-   0        0        0    41588 2023-05-05 15:21:45.000000 pyemaps-1.0.4/crystals.py
--rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.4/ddiffs.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/diffract/
--rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.4/diffract/__init__.py
--rw-rw-rw-   0        0        0    26094 2023-05-07 15:47:33.000000 pyemaps-1.0.4/diffract/bloch_dec.py
--rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/csf_dec.py
--rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/dif_dec.py
--rw-rw-rw-   0        0        0     5069 2023-04-03 21:05:15.000000 pyemaps-1.0.4/diffract/dpgen_dec.py
--rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/mxtal_dec.py
--rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/powder_dec.py
--rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.4/diffract/stereo_dec.py
--rw-rw-rw-   0        0        0    19525 2023-05-05 16:35:51.000000 pyemaps-1.0.4/display.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/ediom/
--rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.4/ediom/ediom.py
--rw-rw-rw-   0        0        0    35898 2023-04-23 21:58:00.000000 pyemaps-1.0.4/ediom/ediom_dec.py
--rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.4/emcontrols.py
--rw-rw-rw-   0        0        0     7175 2023-04-03 21:05:15.000000 pyemaps-1.0.4/errors.py
--rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.4/fileutils.py
--rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.4/kdiffs.py
--rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.4/license.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/
--rw-rw-rw-   0        0        0      885 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5768 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/samples/
--rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/al.img
--rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.4/samples/al_db.bin
--rw-rw-rw-   0        0        0     2703 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/al_ediom.py
--rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/powder.py
--rw-rw-rw-   0        0        0     3625 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/si_bloch.py
--rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.4/samples/si_constructor.py
--rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/si_csf.py
--rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.4/samples/si_dif.py
--rw-rw-rw-   0        0        0      795 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/si_dpgen.py
--rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/si_pyemaps.py
--rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/si_rawblochimgs.py
--rw-rw-rw-   0        0        0     3766 2023-05-03 20:38:32.000000 pyemaps-1.0.4/samples/si_scm.py
--rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/si_stereo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/scattering/
--rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.4/scattering/__init__.py
--rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.4/scattering/sct_dec.py
--rw-rw-rw-   0        0        0      734 2023-05-07 17:11:58.000000 pyemaps-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0    21517 2023-05-06 22:11:10.000000 pyemaps-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/spg/
--rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.4/spg/__init__.py
--rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.4/spg/spg_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/
+-rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.5/COPYING
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/CifFile/
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/CifFile/src/
+-rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.5/CifFile/src/CifFile_module.py
+-rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.5/CifFile/src/StarFile.py
+-rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/TypeContentsParser.py
+-rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_1_0.py
+-rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_1_1.py
+-rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_2_0.py
+-rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/YappsStarParser_STAR2.py
+-rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/CifFile/src/drel/
+-rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/__init__.py
+-rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/drel_ast_yacc.py
+-rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/drel_lex.py
+-rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/drel_runtime.py
+-rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/parsetab.py
+-rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/drel/py_from_ast.py
+-rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/parsetab.py
+-rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.5/CifFile/src/yapps3_compiled_rt.py
+-rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      885 2023-05-12 19:13:28.000000 pyemaps-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.5/README.md
+-rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.5/__config__.py
+-rw-rw-rw-   0        0        0     6016 2023-05-12 19:12:49.000000 pyemaps-1.0.5/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.5/__main__.py
+-rw-rw-rw-   0        0        0       21 2023-05-12 19:13:05.000000 pyemaps-1.0.5/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/cdata/
+-rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Aluminium.xtl
+-rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/AluminiumOxide.xtl
+-rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Aluminium_FCC.xtl
+-rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BariumTitanate_180k.xtl
+-rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BariumTitanate_270k.xtl
+-rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BariumTitanate_Tetra.xtl
+-rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/BiMnO3.xtl
+-rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Boron_Tetra.xtl
+-rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CadmiumSelenide_Hex.xtl
+-rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CadmiumSulfide_Cubic.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CadmiumSulfide_Hex.xtl
+-rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Chromium_BCC.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CoSb3_Skutterudite.xtl
+-rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/CopperOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Copper_FCC.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Cu2O_Cuprite.xtl
+-rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Diamond.xtl
+-rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/ErbiumPyrogermanate.xtl
+-rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/FePd_Tetra.xtl
+-rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/FeS2_Pyrite.xtl
+-rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/GalliumAntimonide.xtl
+-rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/GalliumArsenide.xtl
+-rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/GalliumNitride.xtl
+-rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Germanium.xtl
+-rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Gold_FCC.xtl
+-rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/IndiumArsenide.xtl
+-rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/LaMnO3.xtl
+-rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/LeadZirconateTitanate.xtl
+-rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Li2MnO3.xtl
+-rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/NaFeO2.xtl
+-rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Nb3Sn.xtl
+-rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Pentacene.xtl
+-rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.5/cdata/SiAlONa.xtl
+-rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Silicon.xtl
+-rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/StrontiumTitanate.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TelluriumDioxide.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TinDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TitaniumDioxide_Anatase.xtl
+-rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TitaniumDioxide_Rutile.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/TungstenDiselenide.xtl
+-rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/VanadiumDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/ZincOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/Zinc_HCP.xtl
+-rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/ZirconiumNitride.xtl
+-rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.5/cdata/limno2.xtl
+-rw-rw-rw-   0        0        0    41588 2023-05-07 18:11:19.000000 pyemaps-1.0.5/crystals.py
+-rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.5/ddiffs.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/diffract/
+-rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.5/diffract/__init__.py
+-rw-rw-rw-   0        0        0    28522 2023-05-12 19:12:49.000000 pyemaps-1.0.5/diffract/bloch_dec.py
+-rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/csf_dec.py
+-rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/dif_dec.py
+-rw-rw-rw-   0        0        0     5020 2023-05-12 19:12:49.000000 pyemaps-1.0.5/diffract/dpgen_dec.py
+-rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/mxtal_dec.py
+-rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.5/diffract/powder_dec.py
+-rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.5/diffract/stereo_dec.py
+-rw-rw-rw-   0        0        0    19525 2023-05-05 16:35:51.000000 pyemaps-1.0.5/display.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/ediom/
+-rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.5/ediom/ediom.py
+-rw-rw-rw-   0        0        0    35563 2023-05-11 01:51:41.000000 pyemaps-1.0.5/ediom/ediom_dec.py
+-rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.5/emcontrols.py
+-rw-rw-rw-   0        0        0     7175 2023-04-03 21:05:15.000000 pyemaps-1.0.5/errors.py
+-rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.5/fileutils.py
+-rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.5/kdiffs.py
+-rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.5/license.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5768 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 19:13:28.000000 pyemaps-1.0.5/pyemaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/samples/
+-rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/al.img
+-rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.5/samples/al_db.bin
+-rw-rw-rw-   0        0        0     2703 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/al_ediom.py
+-rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/powder.py
+-rw-rw-rw-   0        0        0     3625 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/si_bloch.py
+-rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.5/samples/si_constructor.py
+-rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/si_csf.py
+-rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.5/samples/si_dif.py
+-rw-rw-rw-   0        0        0      795 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/si_dpgen.py
+-rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/si_pyemaps.py
+-rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.5/samples/si_rawblochimgs.py
+-rw-rw-rw-   0        0        0     3884 2023-05-12 19:12:49.000000 pyemaps-1.0.5/samples/si_scm.py
+-rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.5/samples/si_stereo.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/scattering/
+-rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.5/scattering/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.5/scattering/sct_dec.py
+-rw-rw-rw-   0        0        0      734 2023-05-12 19:13:28.000000 pyemaps-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0    21517 2023-05-07 18:11:19.000000 pyemaps-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:13:28.000000 pyemaps-1.0.5/spg/
+-rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.5/spg/__init__.py
+-rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.5/spg/spg_dec.py
```

### Comparing `pyemaps-1.0.4/COPYING` & `pyemaps-1.0.5/COPYING`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/CifFile_module.py` & `pyemaps-1.0.5/CifFile/src/CifFile_module.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/StarFile.py` & `pyemaps-1.0.5/CifFile/src/StarFile.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/TypeContentsParser.py` & `pyemaps-1.0.5/CifFile/src/TypeContentsParser.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/YappsStarParser_1_0.py` & `pyemaps-1.0.5/CifFile/src/YappsStarParser_1_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/YappsStarParser_1_1.py` & `pyemaps-1.0.5/CifFile/src/YappsStarParser_1_1.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/YappsStarParser_2_0.py` & `pyemaps-1.0.5/CifFile/src/YappsStarParser_2_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/YappsStarParser_STAR2.py` & `pyemaps-1.0.5/CifFile/src/YappsStarParser_STAR2.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/drel/drel_ast_yacc.py` & `pyemaps-1.0.5/CifFile/src/drel/drel_ast_yacc.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/drel/drel_lex.py` & `pyemaps-1.0.5/CifFile/src/drel/drel_lex.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/drel/drel_runtime.py` & `pyemaps-1.0.5/CifFile/src/drel/drel_runtime.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/drel/parsetab.py` & `pyemaps-1.0.5/CifFile/src/drel/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/drel/py_from_ast.py` & `pyemaps-1.0.5/CifFile/src/drel/py_from_ast.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/parsetab.py` & `pyemaps-1.0.5/CifFile/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/CifFile/src/yapps3_compiled_rt.py` & `pyemaps-1.0.5/CifFile/src/yapps3_compiled_rt.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/PKG-INFO` & `pyemaps-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyemaps-1.0.4/__config__.py` & `pyemaps-1.0.5/__config__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/__init__.py` & `pyemaps-1.0.5/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,16 @@
 try:
     from .diffract import bloch
     
 except ImportError as e:
     raise Exception('No diffraction module found')
 else:
 
+    TY_NORMAL = 0 # Normal Bloch Image type
+    TY_LACBED = 1 # Large angle Bloch image type
     th_start, th_end, th_step = bloch.get_sam_defs()
     
     DEF_THICKNESS = (th_start, th_end, th_step)
   
     (DEF_SAMPLING, 
      DEF_PIXSIZE, 
      DEF_DETSIZE, 
@@ -138,14 +140,18 @@
 #------------------Crystal Constructor Module--------------------------------
 try:
     from .diffract import mxtal
     
 except ImportError as e:
     raise Exception('No mxtal module found')
 else:
+    
+    # TY_NORMAL = 0 # Normal Bloch Image type
+    # TY_LACBED = 1 # Large angle Bloch image type
+
     ID_MATRIX = [[1,0,0], [0,1,0], [0,0,1]]
     MLEN = 10 
     DEF_TRSHIFT = [0,0,0]
     DEF_CELLBOX = [[0,0,0], [3,3,3]]
     DEF_XZ = [[1,0,0], [0,0,1]]
     DEF_ORSHIFT = [0, 0, 0] #Origin shift
     DEF_LOCASPACE = [0, 0, 0] #location in A Space
```

### Comparing `pyemaps-1.0.4/__main__.py` & `pyemaps-1.0.5/__main__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/BiMnO3.xtl` & `pyemaps-1.0.5/cdata/BiMnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/Boron_Tetra.xtl` & `pyemaps-1.0.5/cdata/Boron_Tetra.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/ErbiumPyrogermanate.xtl` & `pyemaps-1.0.5/cdata/ErbiumPyrogermanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/FeS2_Pyrite.xtl` & `pyemaps-1.0.5/cdata/FeS2_Pyrite.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/LeadZirconateTitanate.xtl` & `pyemaps-1.0.5/cdata/LeadZirconateTitanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/Li2MnO3.xtl` & `pyemaps-1.0.5/cdata/Li2MnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/Pentacene.xtl` & `pyemaps-1.0.5/cdata/Pentacene.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/cdata/SiAlONa.xtl` & `pyemaps-1.0.5/cdata/SiAlONa.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/crystals.py` & `pyemaps-1.0.5/crystals.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/ddiffs.py` & `pyemaps-1.0.5/ddiffs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/diffract/__init__.py` & `pyemaps-1.0.5/diffract/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/diffract/bloch_dec.py` & `pyemaps-1.0.5/diffract/bloch_dec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-# def divWorks(sl, np):
-#     # numCPUs = mp.cpu_count()
-#     # if (numCPUs > len(nums)):
-#     #     numCPUs = len(nums)
-#     jobs = []
-#     slLength = sl
-
-#     jobRange = int(slLength / np)
-#     extra = slLength - (jobRange * np)
-
-#     prevEnd = 0
-#     for c in range(np):
-#         endIdx = (c * jobRange) + jobRange - 1
-#         if (c == (np-1)):
-#             endIdx += extra
-
-#         startIdx = prevEnd
-#         if ( (c > 0) and (startIdx+1 < slLength) ):
-#             startIdx += 1
-
-#         jobs.append( (startIdx, endIdx) )
-#         prevEnd = endIdx
-
-#     return jobs
-    
 def add_bloch(target):    
     """
     
     Dynamic Simulation Specific Controls Default Values:
     ---------------------------------------------------- 
 
     .. data:: DEF_APERTURE
@@ -68,14 +43,15 @@
                    DEF_XAXIS
     from .. import BImgList, EMC, SIMC
 
     from ..fileutils import compose_ofn
     from .. import BlochError,BlochListError
     import numpy as np
     from numpy import asfortranarray as farray
+    from .. import TY_NORMAL, TY_LACBED
 
     BIMG_EXT = '.im3'
     MAX_BIMGFN = 256
     CBED_MODE = DEF_MODE + 1
 
     def _getBlochFN(self):
         '''
@@ -87,15 +63,14 @@
         '''
         cfn = compose_ofn(None, self.name, ty='bloch')+BIMG_EXT
 
         l = len(cfn)
         if l > MAX_BIMGFN:
             raise BlochError('Bloch image file name too long, it cant excced 256')
         
-        # fortran string
         ffn = farray(np.empty((256), dtype='c'))
         for i in range(l):
             ffn[i] = cfn[i]
 
         return cfn, ffn, l
         
     def beginBloch(self, aperture = DEF_APERTURE,
@@ -223,20 +198,20 @@
         em_controls.simc(omega = omega, 
                          sampling = sampling
                         )
 
         self.session_controls=em_controls
         return nsampling, sp
 
-
     def getBlochImages(self, 
-                        sample_thickness = DEF_THICKNESS,
-                        pix_size = DEF_PIXSIZE,
-                        det_size = DEF_DETSIZE,
-                        bSave = False):
+                  sample_thickness = DEF_THICKNESS,
+                  pix_size = DEF_PIXSIZE,
+                  det_size = DEF_DETSIZE,
+                  nType = TY_NORMAL,
+                  bSave = False):
        """
         Retrieves a set of dynamic diffraction image from the simulation 
         sessiom marked by:
 
         `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_. and 
         `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.   
         
@@ -245,35 +220,52 @@
 
         :param pix_size: Detector pixel size in microns
         :type pix_size: int, optional
 
         :param det_size: Detector size or output image size
         :type det_size: int, optional
 
+        :param nType: type of bloch images generated. 0 for normal or 1 for large angle CBED images
+        :type nType: int, optional. defaults to 0
+
         :param bSave: True - save the output to a raw image file with extension of 'im3'
         :type bSave: bool, optional
 
         :return: `BImgList <pyemaps.ddiffs.html#pyemaps.ddiffs.BlochImgs>`_ object
         :rtype: BImgList
 
         Default values:
 
         ::
 
             DEF_PIXSIZE = 25
             DEF_DETSIZE = 512
             DEF_THICKNESS = (200, 200, 100)
 
+        .. warning::
+
+            Dynamic diffraction pattern generation or Bloch has an extensive memory 
+            requirement for regular image generation:
+            
+                nType = TY_NORMAL
+
+            Even more so for a large angle CBED generation when nType = TY_LACBED. 
+
+            To reduce the memory needed, it is recommended to lower input parameters, particularly:
+
+            - The detector size *det_size*. 
+              A reduction of the default value of 512 to 218 for example can reduce memory usage in 
+              pyemaps without losing accuracies of the results.
+
+            - The number of sampling points in *sampling*. 
+              With less available memory on the system where pyemaps is running, decreased sampling 
+              points in *sampling* parameter can make a big difference in pyemaps performance. 
        """
        from copy import deepcopy
 
-       # check to see if control parameters passed in already in session control
-       # passed in 
-       # 
-
        if pix_size is None or not isinstance(pix_size, int):
             raise BlochListError('Pixel size input must be valid integert')
 
        if det_size is None or not isinstance(det_size, int):
             raise BlochListError('Pixel size input must be valid integert')
 
        if sample_thickness is None or \
@@ -289,51 +281,75 @@
        thlist = []
        if th_start == th_end:
             thlist.append(th_start)
        else:
             thlist = list(range(th_start, th_end, th_step))
             thlist.append(th_end)
 
-       dep = len(thlist)
+       ndep = len(thlist)
 
-       if dep > MAX_DEPTH:
+       if ndep > MAX_DEPTH:
             raise BlochListError(f'Number of sample thickness cannot exceed {MAX_DEPTH}')
 
+       # save the input as optional control attributes
        imgfn =''
        if bSave: 
             imgfn, bfn, l = self._getBlochFN()
-            if bloch.openimgfile(det_size, dep, bfn, l) != 0:
-                raise BlochError('Error opening file for write, check if you have write permission')
+            if l > MAX_BIMGFN-1:
+                raise BlochError(f'File name must not exceed {MAX_BIMGFN-1}')
             
+            if bloch.openimgfile(det_size, ndep, bfn, l) != 0:
+                raise BlochError('Error opening file for write, check if you have write permission')
+
+       isLACBED = (nType == TY_LACBED)
+    #    for th in thlist:
+       nslices = ndep
+       nout = 0
+       if isLACBED:
+           nout = bloch.getncalcbeams()
+           nslices = ndep*nout
+           
+       bimg = farray(np.zeros((det_size, det_size, nslices), dtype=np.float32))
+       thl = farray(np.array(thlist), dtype=int)
+
+       bimg, ret = bloch.getimage(thl,
+                                  bimg,
+                                  teta = 0,
+                                  pix = pix_size,
+                                  det = det_size,
+                                  blacbed = isLACBED,
+                                  bsave = bSave)
+       
+       if(ret != 0):
+            raise BlochError("bloch image generation failed!")
+       
+# build a image list
        bimgs = BImgList(self.name)
 
-       # save the input as optional control attributes   
        self.session_controls(pix_size=pix_size, det_size=det_size)
        
-       for th in thlist:
-            bimg = farray(np.zeros((det_size, det_size), dtype=np.float32))
-            
-            bimg, ret = bloch.getimage(bimg, th, 0, pix_size,
-                                        det_size, bsave = bSave)
-            
-            if(ret != 0):
-              raise BlochError("bloch image generation failed!")
-            emc = deepcopy(self.session_controls)
-            emc.simc(sth=th) # save the thickness as optional simulation control attributes
-            bimgs.add(emc, bimg)
+       for i, th in enumerate(thlist):
+          emc = deepcopy(self.session_controls)
+          emc.simc(sth=th)
+          if isLACBED:
+                for j in range(nout):
+                    bimgs.add(emc, bimg[:,:,i*nout + j])
+          else:
+              bimgs.add(emc, bimg[:,:,i])
+
 
        if bSave:
             if bloch.closeimgfile() != 0:
                 raise BlochError('Error closing file')
 
-            print(f'The raw bloch image(s) of dimensions {det_size}x{det_size}x{dep} and an offset of 8 bytes successfully saved to: \n{imgfn}')
+            print(f'The raw bloch image(s) of dimensions {det_size}x{det_size}x{nslices} and an offset of 8 bytes successfully saved to: \n{imgfn}')
             print(f'To view, import the file into ImageJ or other raw image visualization tools')
 
        return bimgs
-       
+           
     def printIBDetails(self):
         '''
         Prints a dynamic diffraction simulation details during a session
         marked by 
         `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_. and 
         `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.   
 
@@ -379,55 +395,57 @@
             sn2 = '{0: < #06d}'. format(int(net2))
             st1 = '{0: < #016.10f}'. format(float(t1))
             st2 = '{0: < #016.10f}'. format(float(t2))
             st3 = '{0: < #016.7g}'. format(float(t3))
 
             print(f"{sn1}{sn2}{st1}{st2}{st3}")   
 
-    # def getBeams(self, bPrint=False):
-    #     '''
-    #     Prints selected beams for current dynamic diffraction simulation 
-    #     session marked by 
-    #     `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_
-    #     and `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.
+    def getCalculatedBeams(self, bPrint=False):
+        '''
+        Retieves and/or prints calculated beams for current dynamic diffraction simulation 
+        session marked by 
+        `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_
+        and `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.
         
-    #     This information is available right after beginBloch call.
+        This information is available right after beginBloch call.
 
-    #     :param bPrint: whether to print selected beams info on standard output
-    #     :type bPrint: bool, optional, default `False`
+        :param bPrint: whether to print selected diffracted beams info on standard output
+        :type bPrint: bool, optional, default `False`
 
-    #     :return: The number of selected beams and the selected beams list in Miller indexes.
-    #     :rtype: a python tuple.
+        :return: The number of selected beams and the selected beams list in Miller indexes.
+        :rtype: a python tuple.
 
-    #     '''    
-    #     nmidx = bloch.get_nbeams()
-    #     if nmidx <= 0:
-    #         raise BlochError("failed to retrieve diffracted beams info")
+        '''    
+        ncalcbeams = bloch.getncalcbeams()
+        if ncalcbeams <= 0:
+            raise BlochError("failed to retrieve diffracted beams info")
 
-    #     ev = farray(np.zeros((3, nmidx), dtype=int))
-    #     ev, ret = bloch.getbeams(ev)
+        cb = farray(np.zeros((3, ncalcbeams), dtype=int))
+        # cb, ret = bloch.GETCALCBEAMS(cb)
+        cb, ret = bloch.getcalcbeams(cb)
 
-    #     if ret != 0:
-    #         raise BlochError("failed to retrieve incidental beams info")
+        if ret != 0:
+            raise BlochError("failed to retrieve incidental beams info")
 
-    #     evv = np.transpose(ev) 
+        cbms = np.transpose(cb) 
         
-    #     if bPrint:
-    #         shkl = "h   K   l"
-    #         print(f"{shkl:^12}")
+        if bPrint:
+            print('---------Calculated Beams in Miller Indexes---------')
+            shkl = "h   K   l"
+            print(f"{shkl:^12}")
+
+            for cbm in cbms:
+                h,k,l = cbm
+                sh = '{0: < #04d}'. format(int(h))
+                sk = '{0: < #04d}'. format(int(k))
+                sl = '{0: < #04d}'. format(int(l))
 
-    #         for e in evv:
-    #             h,k,l = e
-    #             sh = '{0: < #04d}'. format(int(h))
-    #             sk = '{0: < #04d}'. format(int(k))
-    #             sl = '{0: < #04d}'. format(int(l))
+                print(f"{sh}{sk}{sl}") 
 
-    #             print(f"{sh}{sk}{sl}") 
-
-    #     return nmidx, evv  
+        return ncalcbeams, cbms  
      
 # ----------------deprecated and folded into getSCMatrix call----------------
     # def getEigen(self, ib_coords=(0,0)):
     #     '''
     #     Returns eigen values for given sampling point.
     #     It must be called during a dynamic diffraction simulation session
     #     marked by
@@ -556,14 +574,15 @@
                             sampling = DEF_SAMPLING,                    
                             pix_size = DEF_PIXSIZE,                     
                             det_size = DEF_DETSIZE,                     
                             disk_size = DEF_CBED_DSIZE,                 
                             sample_thickness = DEF_THICKNESS,           
                             em_controls = EMC(cl=200, # set smaller that 1000 default value
                                               simc = SIMC(gmax=1.0, excitation=(0.3,1.0))),
+                            nType = TY_NORMAL,
                             bSave = False):
         """
         Generates dynamic diffraction (Bloch) image(s). This function is equivalent to 
         calling :
         
         1. `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_ 
         2. `getBlockImages <pyemaps.crystals.html#pyemaps.crystals.Crystal.getBlockImages>`_
@@ -586,21 +605,24 @@
 
         :param disk_size: Diffracted beams size in range
         :type disk_size: float, optional
 
         :param sample_thickness: Sample thickness in (start, end, step) tuple
         :type sample_thickness: tuple of int, optional
         
+        :param nType: type of bloch images generated. 0 for normal or 1 for large angle CBED images
+        :type nType: int, optional. defaults to 0
+
         :param em_controls: Microscope controls object
         :type em_controls: `Microscope control <pyemaps.emcontrols.html#module-pyemaps.emcontrols>`_, optional
 
         :param bSave: `True` - save the output to a raw image file (ext: im3)
         :type bSave: bool, optional
 
-        :return: BImgList object
+        :return: `BImgList <pyemaps.ddiffs.html#pyemaps.ddiffs.BlochImgs>`_ object
         :rtype: BImgList
         
         Default values:
 
         ::
 
             DEF_APERTURE = 1.0
@@ -615,14 +637,33 @@
         .. note::
 
             There will be one slice of image generated for each sample
             thickness specified by sample_thickness = (start, end, step) arguement:
 
             start, start+step ... start+N*step, end
 
+        .. warning::
+
+            Dynamic diffraction pattern generation or Bloch has an extensive memory 
+            requirement for regular image generation:
+            
+                nType = TY_NORMAL
+
+            Even more so for a large angle CBED generation when nType = TY_LACBED. 
+
+            To reduce the memory needed, it is recommended to lower input parameters, particularly:
+
+            - The detector size *det_size*. 
+              A reduction of the default value of 512 to 218 for example can reduce memory usage in 
+              pyemaps without losing accuracies of the results.
+
+            - The number of sampling points in *sampling*. 
+              With less available memory on the system where pyemaps is running, decreased sampling 
+              points in *sampling* parameter can make a big difference in pyemaps performance. 
+
         """
         try:
            
             _, _ = self.beginBloch(aperture=aperture, 
                             omega=omega, 
                             sampling=sampling, 
                             dbsize = disk_size,
@@ -638,21 +679,22 @@
         
         else:
             try:
                 bimgs = self.getBlochImages(
                     sample_thickness = sample_thickness,
                     pix_size = pix_size,
                     det_size = det_size,
+                    nType = nType,
                     bSave = bSave)
 
             except (BlochError, BlochListError) as e:
                 raise
 
             except Exception as e:
-                raise BlochError(f'Something went wrong when retrieving bloch image') from e
+                raise BlochError(f'Something went wrong when retrieving bloch image {e}') from e
 
             else:
                 return bimgs
 
             finally:
                 self.endBloch()
 
@@ -665,14 +707,16 @@
     target._getBlochFN = _getBlochFN
 
     # ---These calls must be between beginBloch and endBloch calls
     target.printIBDetails = printIBDetails
     # target.getBeams = getBeams     <-------deprecate
     target.getSCMatrix = getSCMatrix
     target.getBlochImages = getBlochImages
+    target.getCalculatedBeams = getCalculatedBeams
+    # target.getLACBEDImage = getLACBEDImage
     # ---These calls must be between beginBloch and endBloch calls
 
     target.endBloch = endBloch
 
     target.generateBloch = generateBloch
 
     return target
```

### Comparing `pyemaps-1.0.4/diffract/csf_dec.py` & `pyemaps-1.0.5/diffract/csf_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/diffract/dif_dec.py` & `pyemaps-1.0.5/diffract/dif_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/diffract/dpgen_dec.py` & `pyemaps-1.0.5/diffract/dpgen_dec.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,18 +78,19 @@
         :rtype: tuple of an integer and a string
         
 
         Input zone axis indexes define the vertices of the stereo projection map. The default
         for a cubic crystal is *DEF_VERTMAT* = [[0,0,1],[1,1,1],[0,1,1]].
 
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojectionmap.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojectionmap.png
+           :width: 75%
+           :align: center
 
         The diffraction patterns database file produced will be consumed by pyemaps ediom module
-        for experimental diffraction pattern serach adn indexing.
+        for experimental diffraction pattern serach and indexing.
 
         """
         import os
         
         if (res > HIGH_RES) or (res < LOW_RES):
             print(f'Resolution input {res} is out of range: ({LOW_RES}, {HIGH_RES})')
             return -1, None
```

### Comparing `pyemaps-1.0.4/diffract/mxtal_dec.py` & `pyemaps-1.0.5/diffract/mxtal_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/diffract/powder_dec.py` & `pyemaps-1.0.5/diffract/powder_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/diffract/stereo_dec.py` & `pyemaps-1.0.5/diffract/stereo_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/display.py` & `pyemaps-1.0.5/display.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/ediom/ediom.py` & `pyemaps-1.0.5/ediom/ediom.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/ediom/ediom_dec.py` & `pyemaps-1.0.5/ediom/ediom_dec.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,15 +579,16 @@
     def _showDPDBMMask(mr, mc):
 
         """
         Internal function to display loaded DP database stereo projection map
         as explained in the following
         
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojectionmap.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojectionmap.png
+           :width: 75%
+           :align: center
 
         """
         len = mr*mc
         
         mask = np.ascontiguousarray(np.zeros(len), dtype=np.short)
         
         ret= ediom.DPGetMask(mask)
@@ -622,15 +623,16 @@
 
         :return: status code, stereo projection map dimension - two integers tuple 
         :rtype: tuple
 
         See the following for stereo projection map representing the DP database:
         
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojectionmap.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojectionmap.png
+           :width: 75%
+           :align: center
 
         """
         # load DP database into ediom and return database fitmap dimensions
         ret, mrow, mcol = ediom.readDPDB(dbfn)
         if ret != 0:            #need to replace this with ediom return value
             print(f'Error loading image file')
             return ret, 0, 0
@@ -756,37 +758,41 @@
 
         The following is a typical sequence of displays during the execution:
 
         1. Once the DP database is loaded successfully, the steoreo projection map associated
         with the DP database will be shown.
         
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojmap.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/stereoprojmap.png
+            :width: 75%
+            :align: center
 
         2. Successful experimental DP image importing will also show the image. This gives users
         the opportunity to verify the image:
 
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/expimagoriginal.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/expimagoriginal.png
+            :width: 75%
+            :align: center
 
         3. Following the display of the experimental DP image and if *bDebug* is not set (by default), 
         the indexing result will be displayed on top of the experimental image:
 
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/expimgindexed.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/expimgindexed.png
+            :width: 75%
+            :align: center
 
         4. Once the indexing results are generated, users have the option to call more display
         *EDIOM* functions to show other results generated by this call. For examples, 
         the matching database DP image and DP database matching index map as shown below:
 
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/matchingDPDB.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/matchingDPDB.png
+            :width: 75%
+            :align: center
 
         .. image:: https://github.com/emlab-solutions/imagepypy/raw/main/matchingindexmap.png
-            :target: https://github.com/emlab-solutions/imagepypy/raw/main/matchingindexmap.png
+            :width: 75%
             :align: center
 
         The latter map presents the likely matching location  (in red) between the DP in database, 
         also considered the theoretical diffraction patterns, and the experimental DP image. 
 
         5. Finally, in addition to the above visual representation of the run and results, 
         more verbose results are also shown in standard output:
```

### Comparing `pyemaps-1.0.4/emcontrols.py` & `pyemaps-1.0.5/emcontrols.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/errors.py` & `pyemaps-1.0.5/errors.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/fileutils.py` & `pyemaps-1.0.5/fileutils.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/kdiffs.py` & `pyemaps-1.0.5/kdiffs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/license.txt` & `pyemaps-1.0.5/license.txt`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/pyemaps.egg-info/PKG-INFO` & `pyemaps-1.0.5/pyemaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyemaps-1.0.4/pyemaps.egg-info/SOURCES.txt` & `pyemaps-1.0.5/pyemaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/al.img` & `pyemaps-1.0.5/samples/al.img`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/al_db.bin` & `pyemaps-1.0.5/samples/al_db.bin`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/al_ediom.py` & `pyemaps-1.0.5/samples/al_ediom.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/powder.py` & `pyemaps-1.0.5/samples/powder.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_bloch.py` & `pyemaps-1.0.5/samples/si_bloch.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_constructor.py` & `pyemaps-1.0.5/samples/si_constructor.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_csf.py` & `pyemaps-1.0.5/samples/si_csf.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_dif.py` & `pyemaps-1.0.5/samples/si_dif.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_dpgen.py` & `pyemaps-1.0.5/samples/si_dpgen.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_pyemaps.py` & `pyemaps-1.0.5/samples/si_pyemaps.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_rawblochimgs.py` & `pyemaps-1.0.5/samples/si_rawblochimgs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/samples/si_scm.py` & `pyemaps-1.0.5/samples/si_scm.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,13 +96,14 @@
                 print(f'Size of the scattering matrix: {nd}x{nd}')
                 print(f'{si_scm}')
                 print(f'\n----Eigen values at: {ib_coords}----')
                 print(si_ev)
                 print(f'\n----Diffracted beams at: {ib_coords}----')
                 print(si_beams)
 
-    
+        # show a list of calculated beams for current bloch session
+        ncb, cbs = si.getCalculatedBeams(bPrint=True)
     # cleanup 
     si.endBloch()
 
 if __name__ == "__main__":
     runSCMTests()
```

### Comparing `pyemaps-1.0.4/samples/si_stereo.py` & `pyemaps-1.0.5/samples/si_stereo.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/scattering/__init__.py` & `pyemaps-1.0.5/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/setup.cfg` & `pyemaps-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/setup.py` & `pyemaps-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/spg/__init__.py` & `pyemaps-1.0.5/spg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.4/spg/spg_dec.py` & `pyemaps-1.0.5/spg/spg_dec.py`

 * *Files identical despite different names*

