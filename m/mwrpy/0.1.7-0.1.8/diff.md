# Comparing `tmp/mwrpy-0.1.7.tar.gz` & `tmp/mwrpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.1.7.tar", last modified: Thu May 11 08:07:08 2023, max compression
+gzip compressed data, was "mwrpy-0.1.8.tar", last modified: Fri May 12 11:13:06 2023, max compression
```

## Comparing `mwrpy-0.1.7.tar` & `mwrpy-0.1.8.tar`

### file list

```diff
@@ -1,72 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 08:06:53.000000 mwrpy-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 08:06:53.000000 mwrpy-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-11 08:07:08.595337 mwrpy-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-11 08:06:53.000000 mwrpy-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.587336 mwrpy-0.1.7/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.591336 mwrpy-0.1.7/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    48094 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    24730 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.591336 mwrpy-0.1.7/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.583336 mwrpy-0.1.7/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.595337 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 08:06:53.000000 mwrpy-0.1.7/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:07:08.591336 mwrpy-0.1.7/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 08:07:08.000000 mwrpy-0.1.7/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 08:07:08.595337 mwrpy-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-11 08:06:53.000000 mwrpy-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.137483 mwrpy-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-12 11:12:51.000000 mwrpy-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 11:12:51.000000 mwrpy-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-12 11:13:06.137483 mwrpy-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-12 11:12:51.000000 mwrpy-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.125483 mwrpy-0.1.8/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20186 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.133484 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1208422 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.125483 mwrpy-0.1.8/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.133484 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.133484 mwrpy-0.1.8/mwrpy/site_config/lindenberg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.137483 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/HZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/TEL_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/TZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.125483 mwrpy-0.1.8/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-12 11:13:06.000000 mwrpy-0.1.8/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:13:06.137483 mwrpy-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-12 11:12:51.000000 mwrpy-0.1.8/setup.py
```

### Comparing `mwrpy-0.1.7/LICENSE` & `mwrpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/PKG-INFO` & `mwrpy-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
         
-        [![Tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
+        [![MWRpy tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
+        [![PyPI version](https://badge.fury.io/py/mwrpy.svg)](https://badge.fury.io/py/mwrpy)
         
         ### Usage
         
         ```python
         import mwrpy
         hatpro = mwrpy.lev1_to_nc("hyytiala", "1C01", "/path/to/files/")
         ```
```

### Comparing `mwrpy-0.1.7/README.md` & `mwrpy-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # MWRpy
 
-[![Tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
+[![MWRpy tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/mwrpy.svg)](https://badge.fury.io/py/mwrpy)
 
 ### Usage
 
 ```python
 import mwrpy
 hatpro = mwrpy.lev1_to_nc("hyytiala", "1C01", "/path/to/files/")
 ```
```

### Comparing `mwrpy-0.1.7/mwrpy/cli.py` & `mwrpy-0.1.8/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.1.8/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/level1/met_quality_control.py` & `mwrpy-0.1.8/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.1.8/mwrpy/level1/write_lev1_nc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Module for writing Level 1 netCDF files"""
 import datetime
 from collections.abc import Callable
 from itertools import groupby
 from typing import TypeAlias
 
 import numpy as np
-import pandas as pd
 from numpy import ma
 
-from mwrpy import rpg_mwr, utils
+from mwrpy import atmos, rpg_mwr
 from mwrpy.level1.lev1_meta_nc import get_data_attributes
 from mwrpy.level1.met_quality_control import apply_met_qc
 from mwrpy.level1.quality_control import apply_qc
 from mwrpy.level1.rpg_bin import RpgBin
 from mwrpy.utils import (
     add_interpol1d,
     add_time_bounds,
-    epoch2unix,
     get_file_list,
     isbit,
     read_yaml_config,
     update_lev1_attributes,
 )
 
 Fill_Value_Float = -999.0
 Fill_Value_Int = -99
+FuncType: TypeAlias = Callable[[str], np.ndarray]
 
 
 def lev1_to_nc(
     site: str,
     data_type: str,
     path_to_files: str,
     output_file: str | None = None,
@@ -90,15 +89,15 @@
         )
         rpg_bin.data["pointing_flag"] = np.zeros(len(rpg_bin.data["time"]), np.int32)
 
         if data_type == "1B01":
             (
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
-            ) = find_lwcl_free(rpg_bin.data, np.arange(len(rpg_bin.data["time"])))
+            ) = atmos.find_lwcl_free(rpg_bin.data, np.arange(len(rpg_bin.data["time"])))
         else:
             (
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
             ) = np.ones(len(rpg_bin.data["time"]), np.int32) * 2, np.ones(
                 len(rpg_bin.data["time"]), np.int32
             )
@@ -170,15 +169,15 @@
                         rpg_irt.data["time"],
                         "ir_azimuth_angle",
                     )
 
             (
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
-            ) = find_lwcl_free(rpg_bin.data, np.arange(len(rpg_bin.data["time"])))
+            ) = atmos.find_lwcl_free(rpg_bin.data, np.arange(len(rpg_bin.data["time"])))
 
             try:
                 file_list_met = get_file_list(path_to_files, "MET")
             except RuntimeError as err:
                 print(err)
             rpg_met = RpgBin(file_list_met)
             add_interpol1d(
@@ -255,30 +254,30 @@
 def _append_hkd(
     file_list_hkd: list, rpg_bin: RpgBin, data_type: str, params: dict
 ) -> None:
     """Append hkd data on same time grid and perform TB sanity check"""
 
     hkd = RpgBin(file_list_hkd)
 
-    if all(hkd.data["latitude"] == Fill_Value_Float):
+    if "latitude" not in hkd.data:
         add_interpol1d(
             rpg_bin.data,
             np.ones(len(hkd.data["time"])) * params["latitude"],
             hkd.data["time"],
             "latitude",
         )
     else:
         idx = np.where(hkd.data["latitude"] != Fill_Value_Float)[0]
         add_interpol1d(
             rpg_bin.data,
             hkd.data["latitude"][idx],
             hkd.data["time"][idx],
             "latitude",
         )
-    if all(hkd.data["longitude"] == Fill_Value_Float):
+    if "longitude" not in hkd.data:
         add_interpol1d(
             rpg_bin.data,
             np.ones(len(hkd.data["time"])) * params["longitude"],
             hkd.data["time"],
             "longitude",
         )
     else:
@@ -324,61 +323,14 @@
                 | (~isbit(status, 26) & ~isbit(status, 27)),
                 irec,
             ] = 1
 
     return status_flag
 
 
-def find_lwcl_free(lev1: dict, ix: np.ndarray) -> tuple:
-    """Identification of liquid water cloud free periods
-    using TB variability at 31.4 GHz and IRT.
-    Uses pre-defined time index and additionally returns status of IRT availability
-    """
-
-    if "elevation_angle" in lev1:
-        elevation_angle = lev1["elevation_angle"][:]
-    else:
-        elevation_angle = 90 - lev1["zenith_angle"][:]
-
-    index = np.ones(len(ix)) * np.nan
-    status = np.ones(len(ix), dtype=np.int32)
-    freq_31 = np.where(np.round(lev1["frequency"][:], 1) == 31.4)[0]
-    if len(freq_31) == 1:
-        tb = np.squeeze(lev1["tb"][ix, freq_31])
-        tb[(lev1["pointing_flag"][ix] == 1) | (elevation_angle[ix] < 89.0)] = np.nan
-        ind = utils.time_to_datetime_index(lev1["time"][ix])
-        tb_df = pd.DataFrame({"Tb": tb}, index=ind)
-        tb_std = tb_df.rolling("2min", center=True, min_periods=10).std()
-        tb_mx = tb_std.rolling("20min", center=True, min_periods=100).max()
-
-        if "irt" in lev1:
-            tb_thres = 0.1
-            irt = lev1["irt"][ix, :]
-            irt[irt == Fill_Value_Float] = np.nan
-            irt = np.nanmean(irt, axis=1)
-            irt[
-                (lev1["pointing_flag"][ix] == 1) | (elevation_angle[ix] < 89.0)
-            ] = np.nan
-            irt_df = pd.DataFrame({"Irt": irt[:]}, index=ind)
-            irt_mx = irt_df.rolling("20min", center=True, min_periods=100).max()
-            index[(irt_mx["Irt"] > 263.15) & (tb_mx["Tb"] > tb_thres)] = 1
-            status[:] = 0
-
-        tb_thres = 0.2
-        index[(tb_mx["Tb"] > tb_thres)] = 1
-        df = pd.DataFrame({"index": index}, index=ind)
-        df = df.fillna(method="bfill", limit=120)
-        df = df.fillna(method="ffill", limit=120)
-        index = np.array(df["index"])
-        index[(tb_mx["Tb"] < tb_thres) & (index != 1.0)] = 0.0
-        index[(elevation_angle[ix] < 89.0) & (index != 1.0)] = 2.0
-
-    return np.nan_to_num(index, nan=2).astype(int), status
-
-
 def _add_bls(brt: RpgBin, bls: RpgBin, hkd: RpgBin, params: dict) -> None:
     """Add BLS boundary-layer scans using a linear time axis"""
 
     bls.data["time_bnds"] = add_time_bounds(bls.data["time"] + 1, params["int_time"])
     bls.data["status"] = np.zeros(
         (len(bls.data["time"]), len(params["receiver"])), np.int32
     )
@@ -435,22 +387,22 @@
         [],
         [],
         [],
         [],
         [],
         [],
     )
-    seqs = [
+    seqs_all = [
         (key, len(list(val)))
         for key, val in groupby(hkd.data["status"][:] & 2**18 > 0)
     ]
     seqs = np.array(
         [
-            (key, sum(s[1] for s in seqs[:i]), len)
-            for i, (key, len) in enumerate(seqs)
+            (key, sum(s[1] for s in seqs_all[:i]), length)
+            for i, (key, length) in enumerate(seqs_all)
             if bool(key) is True
         ]
     )
 
     for time_ind, time_blb in enumerate(blb.data["time"]):
         if (
             (site in ["juelich", "cologne"])
@@ -468,16 +420,16 @@
             continue
 
         if (
             np.abs(time_blb - hkd.data["time"][seqs[seqi, 1]][0])
             >= blb.header["_n_ang"]
         ):
             scan_quadrant = 0.0  # scan quadrant, 0 deg: 1st, 180 deg: 2nd
-            if (isbit(blb.data["rf_mod"][time_ind], 1)) & (
-                not isbit(blb.data["rf_mod"][time_ind], 2)
+            if (isbit(blb.data["rain"][time_ind], 1)) & (
+                not isbit(blb.data["rain"][time_ind], 2)
             ):
                 scan_quadrant = 180.0
 
             time_add = np.concatenate(
                 (
                     time_add,
                     np.squeeze(
@@ -516,15 +468,15 @@
                 )
             )
 
             rain_add = np.concatenate(
                 (
                     rain_add,
                     np.ones(blb.header["_n_ang"], np.int32)
-                    * int(isbit(blb.data["rf_mod"][time_ind], 0)),
+                    * int(isbit(blb.data["rain"][time_ind], 0)),
                 )
             )
             elevation_angle_add = np.concatenate(
                 (elevation_angle_add, blb.header["_ang"])
             )
 
             for ang in range(blb.header["_n_ang"]):
@@ -569,15 +521,14 @@
         pointing_flag_add = np.ones(len(time_add), np.int32)
         liquid_cloud_flag_add = np.ones(len(time_add), np.int32) * 2
         liquid_cloud_flag_status_add = np.ones(len(time_add), np.int32) * Fill_Value_Int
         brt.data["time"] = np.concatenate((brt.data["time"], time_add))
         ind = np.argsort(brt.data["time"])
         brt.data["time"] = brt.data["time"][ind]
 
-        FuncType: TypeAlias = Callable[[str], np.array]
         names_add: dict[str, FuncType] = {
             "time_bnds": time_bnds_add,
             "elevation_angle": elevation_angle_add,
             "azimuth_angle": azimuth_angle_add,
             "rain": rain_add,
             "tb": tb_add,
             "pointing_flag": pointing_flag_add,
@@ -602,73 +553,7 @@
         (brt["azimuth_angle"][:] > 180) & (brt["azimuth_angle"][:] <= 360)
     )
     brt["azimuth_angle"][ind180] = params["azi_cor"] - brt["azimuth_angle"][ind180]
     brt["azimuth_angle"][ind360] = (
         360.0 + params["azi_cor"] - brt["azimuth_angle"][ind360]
     )
     brt["azimuth_angle"][brt["azimuth_angle"][:] < 0] += 360.0
-
-
-def cal_his(params: dict, glob_att: dict, time0: int) -> RpgBin:
-    """Load and add information from ABSCAL.HIS file"""
-    file_list_cal, rpg_cal = [], []
-    cal_type = [
-        "instrument performs no absolute calibration",
-        "liquid nitrogen calibration",
-        "sky tipping calibration",
-    ]
-    try:
-        file_list_cal = get_file_list(params["path_to_cal"], " ")
-    except RuntimeError:
-        print(
-            [
-                "No binary files with extension his found in directory "
-                + params["path_to_cal"]
-            ]
-        )
-
-    if len(file_list_cal) > 0:
-        rpg_cal = RpgBin(file_list_cal)
-        cal_times1 = epoch2unix(rpg_cal.data["t1"], rpg_cal.header["_time_ref"])
-        cal_times2 = epoch2unix(rpg_cal.data["t2"], rpg_cal.header["_time_ref"])
-        cal_ind1 = np.where(cal_times1 < time0)[0]
-        cal_ind2 = np.where(cal_times2 < time0)[0]
-
-        if (len(cal_ind1) > 0) & (len(cal_ind2) > 0):
-            if (
-                (rpg_cal.data["cal1_t"][cal_ind1[-1]] > 0)
-                & (rpg_cal.data["cal2_t"][cal_ind2[-1]] > 0)
-                & ((time0 - cal_times1[cal_ind1[-1]]) / 86400.0 < 183.0)
-                & ((time0 - cal_times2[cal_ind2[-1]]) / 86400.0 < 183.0)
-            ):
-                glob_att["instrument_calibration_status"] = "calibrated"
-            else:
-                glob_att["instrument_calibration_status"] = "needs calibration"
-
-            glob_att[
-                "receiver1_date_of_last_absolute_calibration"
-            ] = datetime.datetime.utcfromtimestamp(
-                epoch2unix(
-                    rpg_cal.data["t1"][cal_ind1[-1]], rpg_cal.header["_time_ref"]
-                )
-            ).strftime(
-                "%Y%m%d"
-            )
-            glob_att["receiver1_type_of_last_absolute_calibration"] = cal_type[
-                int(rpg_cal.data["cal1_t"][cal_ind1[-1]])
-            ]
-            glob_att[
-                "receiver2_date_of_last_absolute_calibration"
-            ] = datetime.datetime.utcfromtimestamp(
-                epoch2unix(
-                    rpg_cal.data["t2"][cal_ind2[-1]], rpg_cal.header["_time_ref"]
-                )
-            ).strftime(
-                "%Y%m%d"
-            )
-            glob_att["receiver2_type_of_last_absolute_calibration"] = cal_type[
-                int(rpg_cal.data["cal2_t"][cal_ind2[-1]])
-            ]
-        else:
-            glob_att["instrument_calibration_status"] = "needs calibration"
-
-    return rpg_cal
```

### Comparing `mwrpy-0.1.7/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.1.8/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.1.8/mwrpy/level2/write_lev2_nc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Module for writing Level 2 netCDF files"""
 from datetime import datetime
 
 import netCDF4 as nc
 import numpy as np
 import pytz
-from numpy import ma
 from timezonefinder import TimezoneFinder
 
 from mwrpy import rpg_mwr
 from mwrpy.atmos import eq_pot_tem, pot_tem, rel_hum
 from mwrpy.level2.get_ret_coeff import get_mvr_coeff
 from mwrpy.level2.lev2_meta_nc import get_data_attributes
 from mwrpy.level2.lwp_offset import correct_lwp_offset
 from mwrpy.utils import (
     add_time_bounds,
+    get_coeff_list,
     get_ret_ang,
     get_ret_freq,
     interpol_2d,
     read_yaml_config,
 )
 
 Fill_Value_Float = -999.0
@@ -36,15 +36,17 @@
     applies retrieval coefficients for Level 2 products
     and writes it into a netCDF file.
 
     Args:
         site: Name of site.
         data_type: Data type of the netCDF file.
         lev1_path: Path of Level 1 file.
-        lev2_path: Path of Level 2 output directory.
+        output_file: Name of output file.
+        temp_file: Name of temperature product file.
+        hum_file: Name of humidity product file.
 
     """
 
     if data_type not in (
         "2P01",
         "2P02",
         "2P03",
@@ -55,22 +57,24 @@
         "2I02",
     ):
         raise RuntimeError(
             ["Data type " + data_type + " not supported for file writing."]
         )
 
     with nc.Dataset(lev1_path) as lev1:
-        BL_scan = _test_BL_scan(site, lev1)
-        if (data_type == "2P02") & (not BL_scan):
-            data_type = "2P01"
+        if data_type == "2P02":
+            bl_scan = _test_bl_scan(site, lev1)
+            if not bl_scan:
+                data_type = "2P01"
         if data_type in ("2P04", "2P07", "2P08"):
-            T_product = "2P02"
-            if not BL_scan:
-                T_product = "2P01"
-            for d_type in [T_product, "2P03"]:
+            bl_scan = _test_bl_scan(site, lev1)
+            t_product = "2P02"
+            if not bl_scan:
+                t_product = "2P01"
+            for d_type in [t_product, "2P03"]:
                 global_attributes, params = read_yaml_config(site)
                 rpg_dat, coeff, index = get_products(
                     site, lev1, d_type, params, temp_file=temp_file, hum_file=hum_file
                 )
                 _combine_lev1(lev1, rpg_dat, index, d_type, params)
                 hatpro = rpg_mwr.Rpg(rpg_dat)
                 hatpro.data = get_data_attributes(hatpro.data, d_type)
@@ -90,34 +94,33 @@
 def get_products(
     site: str,
     lev1: nc.Dataset,
     data_type: str,
     params: dict,
     temp_file: str | None = None,
     hum_file: str | None = None,
-) -> tuple:
+) -> tuple[dict, dict, np.ndarray]:
     """Derive specified Level 2 products."""
 
     if "elevation_angle" in lev1.variables:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
-    rpg_dat = {}
+    rpg_dat, coeff, index = {}, {}, np.empty(0)
 
     if data_type in ("2I01", "2I02"):
         if data_type == "2I01":
             product = "lwp"
         else:
             product = "iwv"
 
         coeff = get_mvr_coeff(site, product, lev1["frequency"][:])
-
-        if coeff[0]["ret_type"] < 2:
-            coeff, offset, lin, quad, _, _ = get_mvr_coeff(
+        if coeff[0]["RT"] < 2:
+            coeff, offset, lin, quad = get_mvr_coeff(
                 site, product, lev1["frequency"][:]
             )
         else:
             (
                 coeff,
                 input_scale,
                 input_offset,
@@ -129,67 +132,69 @@
             ) = get_mvr_coeff(site, product, lev1["frequency"][:])
         ret_in = retrieval_input(lev1, coeff)
 
         index = np.where(
             (lev1["pointing_flag"][:] == 0)
             & np.any(
                 np.abs(
-                    (np.ones((len(elevation_angle), len(coeff["ele"]))) * coeff["ele"])
+                    (np.ones((len(elevation_angle[:]), len(coeff["AG"]))) * coeff["AG"])
                     - np.transpose(
-                        np.ones((len(coeff["ele"]), len(elevation_angle)))
-                        * elevation_angle
+                        np.ones((len(coeff["AG"]), len(elevation_angle[:])))
+                        * elevation_angle[:]
                     )
                 )
                 < 0.5,
                 axis=1,
             )
         )[0]
         if len(index) == 0:
             raise RuntimeError(
                 ["No suitable data found for processing for data type: " + data_type]
             )
         coeff["retrieval_elevation_angles"] = str(
             np.sort(np.unique(ele_retrieval(elevation_angle[index], coeff)))
         )
-        coeff["retrieval_frequencies"] = str(np.sort(np.unique(coeff["freq"])))
+        coeff["retrieval_frequencies"] = str(np.sort(np.unique(coeff["FR"])))
 
-        if coeff["ret_type"] < 2:
+        if coeff["RT"] < 2:
             coeff_offset = offset(elevation_angle[index])
             coeff_lin = lin(elevation_angle[index])
             coeff_quad = quad(elevation_angle[index])
             tmp_product = (
-                coeff_offset
-                + np.sum(coeff_lin * ret_in[index, :], axis=1)
-                + np.sum(coeff_quad * ret_in[index, :] ** 2, axis=1)
+                coeff_offset[:]
+                + np.einsum("ij,ij->i", ret_in[index, :], coeff_lin)
+                + np.einsum("ij,ij->i", ret_in[index, :] ** 2, coeff_quad)
             )
 
         else:
-            tmp_product = np.ones(len(index), np.float32) * Fill_Value_Float
-
             c_w1, c_w2, fac = (
                 weights1(elevation_angle[index]),
                 weights2(elevation_angle[index]),
                 factor(elevation_angle[index]),
             )
-
             in_sc, in_os = input_scale(elevation_angle[index]), input_offset(
                 elevation_angle[index]
             )
             op_sc, op_os = output_scale(elevation_angle[index]), output_offset(
                 elevation_angle[index]
             )
 
-            for ix, iv in enumerate(index):
-                ret_in[iv, 1:] = (ret_in[iv, 1:] - in_os[ix, :]) * in_sc[ix, :]
-                hidden_layer = np.ones(c_w1.shape[2] + 1, np.float32)
-                hidden_layer[1:] = np.tanh(fac[ix] * ret_in[iv, :].dot(c_w1[ix, :, :]))
-                tmp_product[ix] = (
-                    np.tanh(fac[ix] * hidden_layer.dot(c_w2[ix, :])) * op_sc[ix, :]
-                    + op_os[ix, :]
+            ret_in[index, 1:] = (ret_in[index, 1:] - in_os[:, :]) * in_sc[:, :]
+            hidden_layer = np.ones((len(index), c_w1.shape[2] + 1), np.float32)
+            hidden_layer[:, 1:] = np.tanh(
+                fac[:] * np.einsum("ijk,ij->ik", c_w1, ret_in[index, :])
+            )
+            tmp_product = np.squeeze(
+                np.tanh(
+                    fac[:]
+                    * np.einsum("ij,ij->i", hidden_layer, c_w2).reshape((len(index), 1))
                 )
+                * op_sc
+                + op_os
+            )
 
         if product == "lwp":
             freq_31 = np.where(np.round(lev1["frequency"][:], 1) == 31.4)[0]
             if len(freq_31) != 1:
                 rpg_dat["lwp"], rpg_dat["lwp_offset"] = (
                     tmp_product,
                     np.ones(len(index)) * Fill_Value_Float,
@@ -204,231 +209,215 @@
     elif data_type in ("2P01", "2P03"):
         if data_type == "2P01":
             product, ret = "temperature", "tpt"
         else:
             product, ret = "absolute_humidity", "hpt"
 
         coeff = get_mvr_coeff(site, ret, lev1["frequency"][:])
-        if coeff[0]["ret_type"] < 2:
-            coeff, offset, lin, quad, _, _ = get_mvr_coeff(
-                site, ret, lev1["frequency"][:]
-            )
+        if coeff[0]["RT"] < 2:
+            coeff, offset, lin, quad = get_mvr_coeff(site, ret, lev1["frequency"][:])
         else:
             (
                 coeff,
                 input_scale,
                 input_offset,
                 output_scale,
                 output_offset,
                 weights1,
                 weights2,
                 factor,
             ) = get_mvr_coeff(site, ret, lev1["frequency"][:])
+
         ret_in = retrieval_input(lev1, coeff)
 
         index = np.where(
             (lev1["pointing_flag"][:] == 0)
             & np.any(
                 np.abs(
-                    (np.ones((len(elevation_angle), len(coeff["ele"]))) * coeff["ele"])
+                    (np.ones((len(elevation_angle[:]), len(coeff["AG"]))) * coeff["AG"])
                     - np.transpose(
-                        np.ones((len(coeff["ele"]), len(elevation_angle)))
-                        * elevation_angle
+                        np.ones((len(coeff["AG"]), len(elevation_angle[:])))
+                        * elevation_angle[:]
                     )
                 )
                 < 0.5,
                 axis=1,
             )
         )[0]
         if len(index) == 0:
             raise RuntimeError(
                 ["No suitable data found for processing for data type: " + data_type]
             )
         coeff["retrieval_elevation_angles"] = str(
             np.sort(np.unique(ele_retrieval(elevation_angle[index], coeff)))
         )
-        coeff["retrieval_frequencies"] = str(np.sort(np.unique(coeff["freq"])))
+        coeff["retrieval_frequencies"] = str(np.sort(np.unique(coeff["FR"])))
 
-        rpg_dat["height"] = coeff["height_grid"][:] + params["altitude"]
-        rpg_dat[product] = ma.masked_all((len(index), coeff["n_height_grid"]))
+        rpg_dat["height"] = coeff["AL"][:] + params["altitude"]
 
-        if coeff["ret_type"] < 2:
+        if coeff["RT"] < 2:
             coeff_offset = offset(elevation_angle[index])
             coeff_lin = lin(elevation_angle[index])
             coeff_quad = quad(elevation_angle[index])
-
-            for ialt, _ in enumerate(rpg_dat["height"]):
-                rpg_dat[product][:, ialt] = (
-                    coeff_offset[:, ialt]
-                    + np.sum(coeff_lin[:, ialt, :] * ret_in[index, :], axis=1)
-                    + np.sum(coeff_quad[:, ialt, :] * ret_in[index, :] ** 2, axis=1)
-                )
+            rpg_dat[product] = (
+                coeff_offset
+                + np.einsum("ijk,ik->ij", coeff_lin, ret_in[index, :])
+                + np.einsum("ijk,ik->ij", coeff_quad, ret_in[index, :] ** 2)
+            )
+            if (coeff["RT"] == 1) & (data_type == "2P03"):
+                rpg_dat[product][:, :] = rpg_dat[product][:, :] / 1000.0
 
         else:
             c_w1, c_w2, fac = (
                 weights1(elevation_angle[index]),
                 weights2(elevation_angle[index]),
                 factor(elevation_angle[index]),
             )
             in_sc, in_os = input_scale(elevation_angle[index]), input_offset(
                 elevation_angle[index]
             )
             op_sc, op_os = output_scale(elevation_angle[index]), output_offset(
                 elevation_angle[index]
             )
 
-            for ix, iv in enumerate(index):
-                hidden_in = np.concatenate(
-                    ([1.0], (ret_in[iv, 1:] - in_os[ix, :]) * in_sc[ix, :])
-                )
-                hidden_layer = np.concatenate(
-                    ([1.0], np.tanh(fac[ix] * hidden_in.dot(c_w1[ix, :, :])))
-                )
-                rpg_dat[product][ix, :] = (
-                    np.tanh(fac[ix] * hidden_layer.dot(c_w2[ix, :, :])) * op_sc[ix, :]
-                    + op_os[ix, :]
+            ret_in[index, 1:] = (ret_in[index, 1:] - in_os) * in_sc
+            hidden_layer = np.ones((len(index), c_w1.shape[2] + 1), np.float32)
+            hidden_layer[:, 1:] = np.tanh(
+                fac[:].reshape((len(index), 1))
+                * np.einsum("ijk,ij->ik", c_w1, ret_in[index, :])
+            )
+            rpg_dat[product] = (
+                np.tanh(
+                    fac[:].reshape((len(index), 1))
+                    * np.einsum("ijk,ik->ij", c_w2, hidden_layer)
                 )
-                if product == "absolute_humidity":
-                    rpg_dat[product][ix, :] = rpg_dat[product][ix, :] / 1000.0
+                * op_sc
+                + op_os
+            )
+            if product == "absolute_humidity":
+                rpg_dat[product] = rpg_dat[product] / 1000.0
 
     elif data_type == "2P02":
         coeff = get_mvr_coeff(site, "tpb", lev1["frequency"][:])
-        if coeff[0]["ret_type"] < 2:
-            coeff, offset, lin, quad, _, _ = get_mvr_coeff(
-                site, "tpb", lev1["frequency"][:]
-            )
+        if coeff[0]["RT"] < 2:
+            coeff, offset, lin, quad = get_mvr_coeff(site, "tpb", lev1["frequency"][:])
         else:
             coeff, _, _, _, _, _, _, _ = get_mvr_coeff(
                 site, "tpb", lev1["frequency"][:]
             )
-            coeff["ele"] = np.sort(coeff["ele"])
-        ret_in = retrieval_input(lev1, coeff)
 
+        coeff["AG"] = np.sort(coeff["AG"])
         _, freq_ind, _ = np.intersect1d(
             lev1["frequency"][:],
-            coeff["freq"],
+            coeff["FR"],
             assume_unique=False,
             return_indices=True,
         )
         _, freq_bl, _ = np.intersect1d(
-            coeff["freq"], coeff["freq_bl"], assume_unique=False, return_indices=True
+            coeff["FR"], coeff["FR_BL"], assume_unique=False, return_indices=True
         )
+        coeff["retrieval_frequencies"] = str(np.sort(np.unique(coeff["FR"])))
 
-        coeff["retrieval_frequencies"] = str(np.sort(np.unique(coeff["freq"])))
-
-        # starting indices (elevation ~4.2)
         ix0 = np.where(
-            (elevation_angle > coeff["ele"][0] - 0.5)
-            & (elevation_angle < coeff["ele"][0] + 0.5)
+            (elevation_angle[:] > coeff["AG"][0] - 0.5)
+            & (elevation_angle[:] < coeff["AG"][0] + 0.5)
             & (lev1["pointing_flag"][:] == 1)
-            & (np.arange(len(lev1["time"])) + len(coeff["ele"]) < len(lev1["time"]))
+            & (np.arange(len(lev1["time"])) + len(coeff["AG"]) < len(lev1["time"]))
         )[0]
-
         ibl, tb = (
-            np.empty([0, len(coeff["ele"])], np.int32),
-            np.ones((len(freq_ind), len(coeff["ele"]), 0), np.float32)
+            np.empty([0, len(coeff["AG"])], np.int32),
+            np.ones((len(freq_ind), len(coeff["AG"]), 0), np.float32)
             * Fill_Value_Float,
         )
 
         for ix0v in ix0:
-            if (ix0v + len(coeff["ele"]) < len(lev1["time"])) & (
+            if (ix0v + len(coeff["AG"]) < len(lev1["time"])) & (
                 np.allclose(
-                    elevation_angle[ix0v : ix0v + len(coeff["ele"])],
-                    coeff["ele"],
+                    elevation_angle[ix0v : ix0v + len(coeff["AG"])],
+                    coeff["AG"],
                     atol=0.5,
                 )
             ):
                 ibl = np.append(
-                    ibl, [np.array(range(ix0v, ix0v + len(coeff["ele"])))], axis=0
+                    ibl, [np.array(range(ix0v, ix0v + len(coeff["AG"])))], axis=0
                 )
                 tb = np.concatenate(
                     (
                         tb,
                         np.expand_dims(
-                            lev1["tb"][ix0v : ix0v + len(coeff["ele"]), freq_ind].T, 2
+                            lev1["tb"][ix0v : ix0v + len(coeff["AG"]), freq_ind].T, 2
                         ),
                     ),
                     axis=2,
                 )
 
         if len(ibl) == 0:
             raise RuntimeError(
                 ["No suitable data found for processing for data type: " + data_type]
             )
 
         index = ibl[:, -1]
-        rpg_dat["height"] = coeff["height_grid"][:] + params["altitude"]
-        rpg_dat["temperature"] = ma.masked_all((len(index), coeff["n_height_grid"]))
+        rpg_dat["height"] = coeff["AL"][:] + params["altitude"]
 
-        if coeff["ret_type"] < 2:
+        if coeff["RT"] < 2:
             tb_alg = []
             if len(freq_ind) - len(freq_bl) > 0:
                 tb_alg = np.squeeze(tb[0 : len(freq_ind) - len(freq_bl), 0, :])
-            for ifq, _ in enumerate(coeff["freq_bl"]):
-                tb_alg = np.append(tb_alg, np.squeeze(tb[freq_bl[ifq], :, :]), axis=0)
+            for ifq, _ in enumerate(coeff["FR_BL"]):
+                if len(tb_alg) == 0:
+                    tb_alg = np.squeeze(tb[freq_bl[ifq], :, :])
+                else:
+                    tb_alg = np.append(
+                        tb_alg, np.squeeze(tb[freq_bl[ifq], :, :]), axis=0
+                    )
 
-            for ialt, _ in enumerate(rpg_dat["height"]):
-                rpg_dat["temperature"][:, ialt] = offset[ialt] + np.sum(
-                    lin[:, ialt] * tb_alg[:, :].T, axis=1
-                )
+            rpg_dat["temperature"] = offset() + np.einsum(
+                "jk,ij->ik", lin(), np.transpose(tb_alg)
+            )
 
         else:
-            for ix in range(ibl.shape[0]):
-                ret_array = np.reshape(
-                    ret_in[
-                        np.ix_(
-                            ibl[ix, :],
-                            np.linspace(1, len(freq_ind), len(freq_ind)).astype(int),
-                        )
-                    ],
-                    len(coeff["ele"]) * len(freq_ind),
-                )
-                for i_add in range(ret_in.shape[1] - len(freq_ind) - 1, 0, -1):
-                    ret_array = np.concatenate(
-                        (ret_array, [ma.median(ret_in[ibl[ix, :], -i_add])])
-                    )
-                hidden_in = np.concatenate(
-                    (
-                        [1.0],
-                        (ret_array - coeff["input_offset"][0, :])
-                        * coeff["input_scale"][0, :],
-                    )
-                )
-                hidden_layer = np.concatenate(
-                    (
-                        [1.0],
-                        np.tanh(
-                            coeff["factor"][0]
-                            * hidden_in.dot(coeff["weights1"][0, :, :])
-                        ),
-                    )
-                )
-                rpg_dat["temperature"][ix, :] = (
-                    np.tanh(
-                        coeff["factor"][0]
-                        * hidden_layer.dot(coeff["weights2"][0, :, :])
-                    )
-                    * coeff["output_scale"][0, :]
-                    + coeff["output_offset"][0, :]
+            ret_in = retrieval_input(lev1, coeff)
+            ret_array = np.reshape(
+                tb, (len(coeff["AG"]) * len(freq_ind), len(ibl)), "F"
+            )
+            ret_array = np.concatenate((np.ones((1, len(ibl)), np.float32), ret_array))
+            for i_add in range(ret_in.shape[1] - len(coeff["FR"]) - 1, 0, -1):
+                ret_array = np.concatenate((ret_array, [ret_in[ibl[:, 0], -i_add]]))
+            ret_array[1:, :] = (
+                ret_array[1:, :] - coeff["input_offset"][:, np.newaxis]
+            ) * coeff["input_scale"][:, np.newaxis]
+            hidden_layer = np.tanh(
+                coeff["NP"][:] * np.einsum("ij,ik->kj", coeff["W1"], ret_array)
+            )
+            hidden_layer = np.concatenate(
+                (np.ones((len(ibl), 1), np.float32), hidden_layer), axis=1
+            )
+            rpg_dat["temperature"] = np.transpose(
+                np.tanh(
+                    coeff["NP"][:] * np.einsum("ij,kj->ik", coeff["W2"], hidden_layer)
                 )
+                * coeff["output_scale"][:, np.newaxis]
+                + coeff["output_offset"][:, np.newaxis]
+            )
 
     elif data_type in ("2P04", "2P07", "2P08"):
-        product = data_type
         tem_dat, tem_freq, tem_ang = load_product(temp_file)
         hum_dat, hum_freq, hum_ang = load_product(hum_file)
 
-        coeff, index = {}, []
+        coeff, index = {}, np.empty(0, np.int32)
         coeff["retrieval_frequencies"] = str(
             np.unique(np.sort(np.concatenate([tem_freq, hum_freq])))
         )
         coeff["retrieval_elevation_angles"] = str(
             np.unique(np.sort(np.concatenate([tem_ang, hum_ang])))
         )
-        coeff["retrieval_description"] = "derived product from: " + product + ", 2P03"
-        coeff["dependencies"] = product + ", 2P03"
+        coeff["retrieval_description"] = (
+            "derived product from: " + temp_file + ", " + hum_file
+        )
+        coeff["dependencies"] = temp_file + ", " + hum_file
 
         hum_int = interpol_2d(
             hum_dat.variables["time"][:],
             hum_dat.variables["absolute_humidity"][:, :],
             tem_dat.variables["time"][:],
         )
 
@@ -438,31 +427,34 @@
         )
         if data_type == "2P04":
             rpg_dat["relative_humidity"] = rel_hum(
                 tem_dat.variables["temperature"][:, :], hum_int
             )
         if data_type == "2P07":
             rpg_dat["potential_temperature"] = pot_tem(
-                tem_dat.variables["temperature"][:, :], hum_int, pres, rpg_dat["height"]
+                tem_dat.variables["temperature"][:, :],
+                hum_int,
+                pres,
+                rpg_dat["height"],
             )
         if data_type == "2P08":
             rpg_dat["equivalent_potential_temperature"] = eq_pot_tem(
-                tem_dat.variables["temperature"][:, :], hum_int, pres, rpg_dat["height"]
+                tem_dat.variables["temperature"][:, :],
+                hum_int,
+                pres,
+                rpg_dat["height"],
             )
 
         _combine_lev1(
             tem_dat,
             rpg_dat,
             np.arange(len(tem_dat.variables["time"][:])),
             data_type,
             params,
         )
-        tem_dat.close()
-        hum_dat.close()
-
     return rpg_dat, coeff, index
 
 
 def _combine_lev1(
     lev1: nc.Dataset,
     rpg_dat: dict,
     index: np.ndarray,
@@ -476,15 +468,15 @@
         "azimuth_angle",
         "elevation_angle",
         "zenith_angle",
         "altitude",
         "latitude",
         "longitude",
     ]
-    if index != []:
+    if index.any():
         for ivars in lev1_vars:
             if ivars not in lev1.variables:
                 continue
             if (ivars == "time_bnds") & (data_type == "2P02"):
                 rpg_dat[ivars] = add_time_bounds(
                     lev1["time"][index], params["scan_time"]
                 )
@@ -524,141 +516,155 @@
     """load existing lev2 file for deriving other products"""
     file = nc.Dataset(filename)
     ret_freq = get_ret_freq(filename)
     ret_ang = get_ret_ang(filename)
     return file, ret_freq, ret_ang
 
 
-def _test_BL_scan(site: str, lev1: nc.Dataset) -> bool:
-    """Check for exiEsting BL scans in lev1 data"""
+def _test_bl_scan(site: str, lev1: nc.Dataset) -> bool:
+    """Check for existing BL scans in lev1 data"""
 
     if "elevation_angle" in lev1.variables:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
-    BL_scan = True
-    coeff = get_mvr_coeff(site, "tpb", lev1["frequency"][:])
-    BL_ind = np.where(
-        (elevation_angle > coeff[0]["ele"][0] - 0.5)
-        & (elevation_angle < coeff[0]["ele"][0] + 0.5)
-        & (lev1["pointing_flag"][:] == 1)
-    )[0]
-    if len(BL_ind) == 0:
-        BL_scan = False
-    return BL_scan
+    bl_scan = True
+    coeff_file = get_coeff_list(site, "tpb")
+    if len(coeff_file) > 0:
+        coeff = get_mvr_coeff(site, "tpb", lev1["frequency"][:])
+        bl_ind = np.where(
+            (elevation_angle[:] > coeff[0]["AG"][0] - 0.5)
+            & (elevation_angle[:] < coeff[0]["AG"][0] + 0.5)
+            & (lev1["pointing_flag"][:] == 1)
+        )[0]
+        if len(bl_ind) == 0:
+            bl_scan = False
+    else:
+        bl_scan = False
+    return bl_scan
 
 
 def ele_retrieval(ele_obs: np.ndarray, coeff: dict) -> np.ndarray:
     """Extracts elevation angles used in retrieval"""
-    ele_ret = coeff["ele"]
+    ele_ret = coeff["AG"]
     if ele_ret.shape == ():
         ele_ret = np.array([ele_ret])
     return np.array([ele_ret[(np.abs(ele_ret - v)).argmin()] for v in ele_obs])
 
 
-def retrieval_input(lev1: nc.Dataset, coeff: dict) -> np.ndarray:
+def retrieval_input(lev1: dict | nc.Dataset, coeff: dict) -> np.ndarray:
     """Get retrieval input"""
-    bias = np.ones((len(lev1["time"][:]), 1), np.float32)
-    doy = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
-    sun = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
-    # irt = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
-    tf = TimezoneFinder()
-
-    for ind, time in enumerate(lev1["time"][:].data):
-        if time < 24:
-            date = [lev1.year, lev1.month, lev1.day]
-            time = decimal_hour2unix(date, time)
 
-        # Make me faster
-        timezone_str = tf.timezone_at(
-            lng=lev1["longitude"][ind], lat=lev1["latitude"][ind]
-        )
-        timezone = pytz.timezone(timezone_str)
-        dtime = datetime.fromtimestamp(time, timezone)
+    time_median = np.nanmedian(lev1["time"][:])
+    if time_median < 24:
+        date = [lev1.year, lev1.month, lev1.day]
+        time_median = decimal_hour2unix(date, time_median)
+
+    _, freq_ind, _ = np.intersect1d(
+        lev1["frequency"][:],
+        coeff["FR"][:],
+        assume_unique=False,
+        return_indices=True,
+    )
+    bias = np.ones((len(lev1["time"][:]), 1), np.float32)
 
-        dyear = datetime(dtime.year, 12, 31, 0, 0).timetuple().tm_yday
-        doy[ind, 0] = np.cos(
-            datetime.fromtimestamp(time).timetuple().tm_yday / dyear * 2 * np.pi
-        )
-        doy[ind, 1] = np.sin(
-            datetime.fromtimestamp(time).timetuple().tm_yday / dyear * 2 * np.pi
-        )
-        sun[ind, 0] = np.cos(
-            (dtime.hour + dtime.minute / 60 + dtime.second / 3600) / 24 * 2 * np.pi
-        )
-        sun[ind, 1] = np.sin(
-            (dtime.hour + dtime.minute / 60 + dtime.second / 3600) / 24 * 2 * np.pi
-        )
+    latitude = float(np.median(lev1["latitude"][:]))
+    longitude = float(np.median(lev1["longitude"][:]))
 
-    if coeff["ret_type"] < 2:
+    if coeff["RT"] == Fill_Value_Int:
         ret_in = lev1["tb"][:, :]
+    elif coeff["RT"] in (0, 1):
+        ret_in = lev1["tb"][:, freq_ind]
     else:
-        _, freq_ind, _ = np.intersect1d(
-            lev1["frequency"][:],
-            coeff["freq"][:, 0],
-            assume_unique=False,
-            return_indices=True,
-        )
         ret_in = np.concatenate((bias, lev1["tb"][:, freq_ind]), axis=1)
-        for i, field in enumerate(coeff["aux"]):
-            if (field == "TS") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate(
-                    (
-                        ret_in,
-                        np.reshape(
-                            lev1["air_temperature"][:].data, (len(lev1["time"][:]), 1)
-                        ),
-                    ),
-                    axis=1,
-                )
-            if (field == "HS") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate(
-                    (
-                        ret_in,
-                        np.reshape(
-                            lev1["relative_humidity"][:].data, (len(lev1["time"][:]), 1)
-                        ),
-                    ),
-                    axis=1,
-                )
-            if (field == "PS") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate(
-                    (
-                        ret_in,
-                        np.reshape(
-                            lev1["air_pressure"][:].data, (len(lev1["time"][:]), 1)
-                        ),
-                    ),
-                    axis=1,
-                )
-            if (field == "ZS") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate((ret_in, lev1["irt"][:, :]), axis=1)
-            if (field == "IR") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate((ret_in, lev1["irt"][:, :]), axis=1)
-            if (field == "I1") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate(
-                    (
-                        ret_in,
-                        np.reshape(lev1["irt"][:, 0].data, (len(lev1["time"][:]), 1)),
-                    ),
-                    axis=1,
-                )
-            if (field == "I2") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate(
-                    (
-                        ret_in,
-                        np.reshape(lev1["irt"][:, 1].data, (len(lev1["time"][:]), 1)),
-                    ),
-                    axis=1,
-                )
-            if (field == "DY") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate((ret_in, doy), axis=1)
-            if (field == "SU") & (coeff["aux_flag"][i] == 1):
-                ret_in = np.concatenate((ret_in, sun), axis=1)
+
+        if coeff.get("TS")[0] == 1:
+            ret_in = np.concatenate(
+                (
+                    ret_in,
+                    np.reshape(lev1["air_temperature"][:], (len(lev1["time"][:]), 1)),
+                ),
+                axis=1,
+            )
+        if coeff.get("HS")[0] == 1:
+            ret_in = np.concatenate(
+                (
+                    ret_in,
+                    np.reshape(lev1["relative_humidity"][:], (len(lev1["time"][:]), 1)),
+                ),
+                axis=1,
+            )
+        if coeff.get("PS")[0] == 1:
+            ret_in = np.concatenate(
+                (
+                    ret_in,
+                    np.reshape(lev1["air_pressure"][:], (len(lev1["time"][:]), 1)),
+                ),
+                axis=1,
+            )
+        if coeff.get("ZS") == 1:
+            ret_in = np.concatenate((ret_in, lev1["irt"][:, :]), axis=1)
+        if coeff.get("IR") == 1:
+            ret_in = np.concatenate((ret_in, lev1["irt"][:, :]), axis=1)
+        if coeff.get("I1") == 1:
+            ret_in = np.concatenate(
+                (
+                    ret_in,
+                    np.reshape(lev1["irt"][:, 0], (len(lev1["time"][:]), 1)),
+                ),
+                axis=1,
+            )
+        if coeff.get("I2") == 1:
+            ret_in = np.concatenate(
+                (
+                    ret_in,
+                    np.reshape(lev1["irt"][:, 1], (len(lev1["time"][:]), 1)),
+                ),
+                axis=1,
+            )
+        if coeff.get("DY") == 1:
+            doy = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
+            tf = TimezoneFinder()
+            timezone_str = tf.timezone_at(
+                lng=longitude,
+                lat=latitude,
+            )
+            timezone = pytz.timezone(timezone_str)
+            dtime = datetime.fromtimestamp(time_median, timezone)
+            dyear = datetime(dtime.year, 12, 31, 0, 0).timetuple().tm_yday
+            doy[:, 0] = np.cos(
+                datetime.fromtimestamp(time_median).timetuple().tm_yday
+                / dyear
+                * 2
+                * np.pi
+            )
+            doy[:, 1] = np.sin(
+                datetime.fromtimestamp(time_median).timetuple().tm_yday
+                / dyear
+                * 2
+                * np.pi
+            )
+            ret_in = np.concatenate((ret_in, doy), axis=1)
+        if coeff.get("SU") == 1:
+            sun = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
+            tf = TimezoneFinder()
+            timezone_str = tf.timezone_at(
+                lng=longitude,
+                lat=latitude,
+            )
+            timezone = pytz.timezone(timezone_str)
+            dtime = datetime.fromtimestamp(time_median, timezone)
+            sun[:, 0] = np.cos(
+                (dtime.hour + dtime.minute / 60 + dtime.second / 3600) / 24 * 2 * np.pi
+            )
+            sun[:, 1] = np.sin(
+                (dtime.hour + dtime.minute / 60 + dtime.second / 3600) / 24 * 2 * np.pi
+            )
+            ret_in = np.concatenate((ret_in, sun), axis=1)
 
     return ret_in
 
 
 def decimal_hour2unix(date: list, time: np.ndarray) -> np.ndarray:
     unix_timestamp = np.datetime64("-".join(date)).astype("datetime64[s]").astype("int")
     return (time * 60 * 60 + unix_timestamp).astype(int)
```

### Comparing `mwrpy-0.1.7/mwrpy/plots/generate_plots.py` & `mwrpy-0.1.8/mwrpy/plots/generate_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     max_y: int = 5,
     ele_range: list = [0.0, 91.0],
     pointing: int = 0,
     dpi: int = 120,
     image_name: str | None = None,
     sub_title: bool = True,
     title: bool = True,
-) -> Dimensions:
+) -> tuple[Dimensions, str]:
     """Generates a mwrpy figure.
     Args:
         nc_file (str): Input file.
         field_names (list): Variable names to be plotted.
         show (bool, optional): If True, shows the figure. Default is True.
         save_path (str, optional): Setting this path will save the figure (in the
             given path). Default is None, when the figure is not saved.
@@ -98,15 +98,15 @@
             Overrides the *save_path* option. Default is None.
         sub_title (bool, optional): Add subtitle to image. Default is True.
         title (bool, optional): Add title to image. Default is True.
     Returns:
         Dimensions of the generated figure in pixels.
         File name of the generated figure.
     Examples:
-        >>> from plots import generate_figure
+        >>> from mwrpy.plots import generate_figure
         >>> generate_figure('lev2_file.nc', ['lwp'])
     """
 
     valid_fields, valid_names = _find_valid_fields(nc_file, field_names)
     file_name = []
     if len(valid_fields) > 0:
         is_height = _is_height_dimension(nc_file)
@@ -137,15 +137,15 @@
                 if plot_type == "mesh":
                     _plot_colormesh_data(ax, field, name, ax_value, nc_file)
 
         case_date = _set_labels(fig, axes[-1], nc_file, sub_title)
         file_name = handle_saving(
             nc_file, image_name, save_path, show, case_date, valid_names
         )
-    return Dimensions(fig, axes)
+    return Dimensions(fig, axes), file_name
 
 
 def _mark_gaps(
     time: ndarray,
     data: ma.MaskedArray,
     max_allowed_gap: float = 1,
     mask_edge: int = 0,
@@ -463,30 +463,29 @@
         nlev1 = 41
         hum_file = nc_file.replace("2P08", "2P03")
 
     if name == "absolute_humidity":
         nbin = 6
 
     if name == "relative_humidity":
-        data[data_in.mask == True] = np.nan
+        data[data_in.mask] = np.nan
         data[data > 1.0] = 1.0
         data[data < 0.0] = 0.0
         data *= 100.0
         nbin = 6
         hum_file = nc_file.replace("2P04", "2P03")
 
     if name in (
         "relative_humidity",
         "potential_temperature",
         "equivalent_potential_temperature",
     ):
         hum_time = seconds2hours(read_nc_fields(hum_file, "time"))
         hum_flag = _get_ret_flag(hum_file, hum_time)
         hum_tmp, width = _calculate_rolling_mean(hum_time, hum_flag, win=15 / 60)
-        # hum_flag = np.interp(hum_time, hum_time[int(width / 2 - 1) : int(-width / 2)], hum_tmp)
         hum_flag = np.interp(
             axes[0], hum_time[int(width / 2 - 1) : int(-width / 2)], hum_tmp
         )
     else:
         hum_flag = np.zeros(len(axes[0]), np.int32)
 
     if variables.plot_type == "bit":
```

### Comparing `mwrpy-0.1.7/mwrpy/plots/plot_meta.py` & `mwrpy-0.1.8/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/plots/plot_utils.py` & `mwrpy-0.1.8/mwrpy/plots/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module containing additional helper functions for plotting"""
 import locale
 from datetime import datetime, timezone
 
-import matplotlib.ticker as ticker
+from matplotlib import ticker
 import netCDF4
 import numpy as np
 from numpy import ma, ndarray
 
 from mwrpy.utils import (
     convolve2DFFT,
     get_ret_freq,
@@ -191,15 +191,15 @@
 
 def annotate_heatmap(
     im,
     data=None,
     valfmt="{x:.2f}",
     textcolors=("black", "white"),
     threshold=None,
-    **textkw
+    **textkw,
 ):
     """
     A function to annotate a heatmap.
 
     Parameters
     ----------
     im
```

### Comparing `mwrpy-0.1.7/mwrpy/process_mwrpy.py` & `mwrpy-0.1.8/mwrpy/process_mwrpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 product = [
     ("1C01", ""),
     ("2I01", "lwp"),
     ("2I02", "iwv"),
     ("2P01", "temperature"),
     ("2P02", "temperature"),
-    ("2P03", "water_vapor_vmr"),
+    ("2P03", "absolute_humidity"),
     ("2P04", "relative_humidity"),
     ("2P07", "potential_temperature"),
     ("2P08", "equivalent_potential_temperature"),
     ("2S02", "tb_spectrum"),
     ("stats", ""),
 ]
```

### Comparing `mwrpy-0.1.7/mwrpy/rpg_mwr.py` & `mwrpy-0.1.8/mwrpy/rpg_mwr.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,14 @@
 ) -> netCDF4.Dataset:
     """Initializes an RPG MWR file for writing.
     Args:
         file_name: File name to be generated.
         dimensions: Dictionary containing dimension for this file.
         rpg_arrays: Dictionary containing :class:`RpgArray` instances.
         att_global: Dictionary containing site specific global attributes
-        date: Date string of file
     """
 
     nc_file = netCDF4.Dataset(file_name, "w", format="NETCDF4_CLASSIC")
     for key, dimension in dimensions.items():
         nc_file.createDimension(key, dimension)
     _write_vars2nc(nc_file, rpg_arrays)
     _add_standard_global_attributes(nc_file, att_global)
```

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.1.8/mwrpy/site_config/hatpro.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # thresholds for met quality flags
     # air_temperature [K]
     # relative_humidity [1]
     # air_pressure [hPa]
     # rainfall_rate [mm/h]
     # wind_direction [°]
     # wind_speed [m/s]
-    met_thresholds: [[213.15, 333.15], [0., 1.], [900., 1100.], [0., 300.], [0., 360.], [0., 100.]]
+    met_thresholds: [[213.15, 333.15], [0., 1.], [90000., 110000.], [0., 300.], [0., 360.], [0., 100.]]
 
 
 # Missing entries are filled with site specific config file
 global_specs:
     # Name of the conventions followed by the dataset
     conventions: CF-1.8
```

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.1.8/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.7/mwrpy/utils.py` & `mwrpy-0.1.8/mwrpy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for general helper functions."""
 
 import glob
 import os
 import re
 import time
 from datetime import date, datetime, timedelta, timezone
-from typing import Iterator, NamedTuple
+from typing import Any, Iterator, NamedTuple
 
 import netCDF4
 import numpy as np
 import pandas as pd
 import yaml
 from numpy import ma
 from scipy import signal
@@ -64,15 +64,15 @@
         for index, _ in enumerate(unix_time):
             unix_time[index] = time.mktime(
                 datetime.fromtimestamp(unix_time[index], timezone.utc).timetuple()
             )
     return unix_time
 
 
-def isscalar(array: any) -> bool:
+def isscalar(array: Any) -> bool:
     """Tests if input is scalar.
     By "scalar" we mean that array has a single value.
     Examples:
         >>> isscalar(1)
             True
         >>> isscalar([1])
             True
@@ -84,15 +84,15 @@
 
     arr = ma.array(array)
     if not hasattr(arr, "__len__") or arr.shape == () or len(arr) == 1:
         return True
     return False
 
 
-def isbit(array: np.ndarray, nth_bit: int) -> np.ndarray:
+def isbit(array: int | np.ndarray, nth_bit: int) -> np.ndarray:
     """Tests if nth bit (0,1,2..) is set.
     Args:
         array: Integer array.
         nth_bit: Investigated bit.
     Returns:
         Boolean array denoting values where nth_bit is set.
     Raises:
@@ -107,15 +107,15 @@
     """
     if nth_bit < 0:
         raise ValueError("Negative bit number")
     mask = 1 << nth_bit
     return array & mask > 0
 
 
-def setbit(array: np.ndarray, nth_bit: int) -> np.ndarray:
+def setbit(array: int | np.ndarray, nth_bit: int) -> np.ndarray:
     """Sets nth bit (0, 1, 2..) on number.
     Args:
         array: Integer array.
         nth_bit: Bit to be set.
     Returns:
         Integer where nth bit is set.
     Raises:
@@ -250,19 +250,21 @@
 
 def get_file_list(path_to_files: str, extension: str):
     """Returns file list for specified path."""
     f_list = sorted(glob.glob(path_to_files + "/*." + extension))
     if len(f_list) == 0:
         f_list = sorted(glob.glob(path_to_files + "/*." + extension.lower()))
     if len(f_list) == 0:
-        raise RuntimeError(
-            "Error: no binary files with extension "
-            + extension
-            + " found in directory "
-            + path_to_files
+        print(
+            [
+                "Error: no binary files with extension "
+                + extension
+                + " found in directory "
+                + path_to_files
+            ]
         )
     return f_list
 
 
 def read_yaml_config(site: str) -> tuple[dict, dict]:
     """Reads config yaml files."""
```

### Comparing `mwrpy-0.1.7/mwrpy.egg-info/PKG-INFO` & `mwrpy-0.1.8/mwrpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
         
-        [![Tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
+        [![MWRpy tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
+        [![PyPI version](https://badge.fury.io/py/mwrpy.svg)](https://badge.fury.io/py/mwrpy)
         
         ### Usage
         
         ```python
         import mwrpy
         hatpro = mwrpy.lev1_to_nc("hyytiala", "1C01", "/path/to/files/")
         ```
```

### Comparing `mwrpy-0.1.7/setup.py` & `mwrpy-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,20 +16,22 @@
     author="University of Cologne",
     author_email="actris-ccres-mwr@uni-koeln.de",
     url="https://github.com/actris-cloudnet/mwrpy",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.10",
     install_requires=[
+        "numpy",
         "scipy",
         "netCDF4",
         "matplotlib",
         "metpy",
         "ephem",
         "pandas",
         "pyyaml",
         "timezonefinder",
+        "pytz",
     ],
     extras_require={
         "test": ["pylint", "mypy", "pytest", "pytest-flakefinder"],
     },
 )
```

