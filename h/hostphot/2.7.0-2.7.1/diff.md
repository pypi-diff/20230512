# Comparing `tmp/hostphot-2.7.0.tar.gz` & `tmp/hostphot-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostphot-2.7.0.tar", last modified: Thu May 11 09:43:07 2023, max compression
+gzip compressed data, was "hostphot-2.7.1.tar", last modified: Fri May 12 03:55:03 2023, max compression
```

## Comparing `hostphot-2.7.0.tar` & `hostphot-2.7.1.tar`

### file list

```diff
@@ -1,330 +1,331 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.779374 hostphot-2.7.0/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.7.0/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.7.0/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9455 2023-05-11 09:43:07.779374 hostphot-2.7.0/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8923 2023-05-11 09:42:22.000000 hostphot-2.7.0/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.7.0/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      190 2023-05-11 02:29:33.000000 hostphot-2.7.0/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-11 09:43:07.779374 hostphot-2.7.0/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.7.0/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.727375 hostphot-2.7.0/src/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.7.0/src/hostphot/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      386 2023-05-11 09:42:22.000000 hostphot-2.7.0/src/hostphot/_constants.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-05-11 09:42:22.000000 hostphot-2.7.0/src/hostphot/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/coadd.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    45897 2023-05-11 02:29:33.000000 hostphot-2.7.0/src/hostphot/cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/dust.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot/filters/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot/filters/2MASS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/2MASS/2MASS_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/2MASS/2MASS_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/2MASS/2MASS_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/2MASS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/AAA_README
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot/filters/DES/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.7.0/src/hostphot/filters/DES/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/DES/DES_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/DES/DES_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/DES/DES_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/DES/DES_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/DES/DES_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot/filters/GALEX/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/GALEX/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/GALEX/GALEX_FUV.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/GALEX/GALEX_NUV.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot/filters/HST/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.739375 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/filters/HST/IR_err.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.743375 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.743375 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.747375 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/filters/HST/UVIS1_err.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/filters/HST/UVIS2_err.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.751375 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.763375 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.775375 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/filters/HST/ir_aper_corrections.csv
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.7.0/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.775375 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/BASS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.775375 hostphot-2.7.0/src/hostphot/filters/PS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.7.0/src/hostphot/filters/PS1/AAA_README.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/PS1/PS1_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/PS1/PS1_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/PS1/PS1_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/PS1/PS1_y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/PS1/PS1_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.775375 hostphot-2.7.0/src/hostphot/filters/SDSS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.7.0/src/hostphot/filters/SDSS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_u.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.779374 hostphot-2.7.0/src/hostphot/filters/Spitzer/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/Spitzer/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.779374 hostphot-2.7.0/src/hostphot/filters/VISTA/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/VISTA/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_Z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.779374 hostphot-2.7.0/src/hostphot/filters/WISE/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.0/src/hostphot/filters/WISE/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.7.0/src/hostphot/filters/config.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22737 2023-05-11 09:42:22.000000 hostphot-2.7.0/src/hostphot/global_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2488 2023-05-11 02:29:33.000000 hostphot-2.7.0/src/hostphot/image_cleaning.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12645 2023-05-11 09:42:22.000000 hostphot-2.7.0/src/hostphot/image_masking.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.7.0/src/hostphot/interactive_aperture.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13859 2023-05-11 02:29:33.000000 hostphot-2.7.0/src/hostphot/local_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9169 2023-05-11 09:42:22.000000 hostphot-2.7.0/src/hostphot/objects_detect.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.7.0/src/hostphot/rgb_images.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30315 2023-05-11 09:42:22.000000 hostphot-2.7.0/src/hostphot/utils.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.731375 hostphot-2.7.0/src/hostphot.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9455 2023-05-11 09:43:07.000000 hostphot-2.7.0/src/hostphot.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14942 2023-05-11 09:43:07.000000 hostphot-2.7.0/src/hostphot.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-11 09:43:07.000000 hostphot-2.7.0/src/hostphot.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      193 2023-05-11 09:43:07.000000 hostphot-2.7.0/src/hostphot.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-05-11 09:43:07.000000 hostphot-2.7.0/src/hostphot.egg-info/top_level.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 09:43:07.779374 hostphot-2.7.0/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.7.0/tests/test_cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1074 2023-05-11 02:29:33.000000 hostphot-2.7.0/tests/test_global_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.7.0/tests/test_interactivity.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1089 2023-05-11 02:29:33.000000 hostphot-2.7.0/tests/test_local_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.7.0/tests/test_preprocessing.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      861 2023-05-11 02:29:33.000000 hostphot-2.7.0/tests/test_rgb_images.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.7.1/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.7.1/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9525 2023-05-12 03:55:03.700277 hostphot-2.7.1/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8993 2023-05-12 03:49:47.000000 hostphot-2.7.1/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.7.1/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      190 2023-05-11 02:29:33.000000 hostphot-2.7.1/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-12 03:55:03.700277 hostphot-2.7.1/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.7.1/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.680278 hostphot-2.7.1/src/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      439 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      386 2023-05-11 09:42:22.000000 hostphot-2.7.1/src/hostphot/_constants.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/coadd.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    45897 2023-05-11 02:29:33.000000 hostphot-2.7.1/src/hostphot/cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/dust.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/2MASS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/AAA_README
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/DES/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.7.1/src/hostphot/filters/DES/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/GALEX/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/GALEX/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_FUV.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_NUV.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/HST/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/IR_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/UVIS1_err.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/UVIS2_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.692277 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.696277 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/ir_aper_corrections.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/PS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.7.1/src/hostphot/filters/PS1/AAA_README.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/SDSS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/Spitzer/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/VISTA/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/WISE/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/WISE/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.7.1/src/hostphot/filters/config.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22710 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/global_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2488 2023-05-11 02:29:33.000000 hostphot-2.7.1/src/hostphot/image_cleaning.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12647 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/image_masking.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.7.1/src/hostphot/interactive_aperture.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13859 2023-05-11 02:29:33.000000 hostphot-2.7.1/src/hostphot/local_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9169 2023-05-11 09:42:22.000000 hostphot-2.7.1/src/hostphot/objects_detect.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/rgb_images.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4805 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/sed_plotting.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30315 2023-05-12 03:03:08.000000 hostphot-2.7.1/src/hostphot/utils.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9525 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14971 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      193 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.7.1/tests/test_cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1074 2023-05-11 02:29:33.000000 hostphot-2.7.1/tests/test_global_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.7.1/tests/test_interactivity.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1089 2023-05-11 02:29:33.000000 hostphot-2.7.1/tests/test_local_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.7.1/tests/test_preprocessing.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      861 2023-05-11 02:29:33.000000 hostphot-2.7.1/tests/test_rgb_images.py
```

### Comparing `hostphot-2.7.0/LICENSE` & `hostphot-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/PKG-INFO` & `hostphot-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.7.0
+Version: 2.7.1
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,17 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.7.1
+* Adding SED plotting
+* Fixed plotting angle of masked object 
 v2.7.0
 * MAJOR BUG: Convertion factor between different pixel scales fixed (it was previously inverted). This affects the common aperture photometry between different surveys!
 * Moving font family to `_constant.py` file
 v2.6.2
 * Prettier plots (now using `aplpy`), but also more informative!
 * Scale of the apertures for the masks is now a parameter (`r`) 
 * Raise exception is now `True` by default when calculating photometry
```

### Comparing `hostphot-2.7.0/README.md` & `hostphot-2.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,17 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.7.1
+* Adding SED plotting
+* Fixed plotting angle of masked object 
 v2.7.0
 * MAJOR BUG: Convertion factor between different pixel scales fixed (it was previously inverted). This affects the common aperture photometry between different surveys!
 * Moving font family to `_constant.py` file
 v2.6.2
 * Prettier plots (now using `aplpy`), but also more informative!
 * Scale of the apertures for the masks is now a parameter (`r`) 
 * Raise exception is now `True` by default when calculating photometry
```

### Comparing `hostphot-2.7.0/setup.py` & `hostphot-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/coadd.py` & `hostphot-2.7.1/src/hostphot/coadd.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/cutouts.py` & `hostphot-2.7.1/src/hostphot/cutouts.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/dust.py` & `hostphot-2.7.1/src/hostphot/dust.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/2MASS/2MASS_H.dat` & `hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/2MASS/2MASS_J.dat` & `hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/2MASS/2MASS_Ks.dat` & `hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/AAA_README` & `hostphot-2.7.1/src/hostphot/filters/AAA_README`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/DES/DES_Y.dat` & `hostphot-2.7.1/src/hostphot/filters/DES/DES_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/DES/DES_g.dat` & `hostphot-2.7.1/src/hostphot/filters/DES/DES_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/DES/DES_i.dat` & `hostphot-2.7.1/src/hostphot/filters/DES/DES_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/DES/DES_r.dat` & `hostphot-2.7.1/src/hostphot/filters/DES/DES_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/DES/DES_z.dat` & `hostphot-2.7.1/src/hostphot/filters/DES/DES_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/GALEX/GALEX_FUV.dat` & `hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_FUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/GALEX/GALEX_NUV.dat` & `hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_NUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/IR_err.txt` & `hostphot-2.7.1/src/hostphot/filters/HST/IR_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/UVIS1_err.txt` & `hostphot-2.7.1/src/hostphot/filters/HST/UVIS1_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/UVIS2_err.txt` & `hostphot-2.7.1/src/hostphot/filters/HST/UVIS2_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat` & `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/ir_aper_corrections.csv` & `hostphot-2.7.1/src/hostphot/filters/HST/ir_aper_corrections.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv` & `hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv` & `hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/BASS_g.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/BASS_r.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat` & `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/PS1/PS1_g.dat` & `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/PS1/PS1_i.dat` & `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/PS1/PS1_r.dat` & `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/PS1/PS1_y.dat` & `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/PS1/PS1_z.dat` & `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_g.dat` & `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_i.dat` & `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_r.dat` & `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_u.dat` & `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_u.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/SDSS/SDSS_z.dat` & `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat` & `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat` & `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat` & `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat` & `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat` & `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_H.dat` & `hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_J.dat` & `hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_Ks.dat` & `hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_Y.dat` & `hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/VISTA/VISTA_Z.dat` & `hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W1.dat` & `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W2.dat` & `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W3.dat` & `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/WISE/WISE_W4.dat` & `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/filters/config.txt` & `hostphot-2.7.1/src/hostphot/filters/config.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/global_photometry.py` & `hostphot-2.7.1/src/hostphot/global_photometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,14 @@
         if flip == flip2:
             flip_ = False
         else:
             flip_ = True
 
         gal_obj, conv_factor = adapt_aperture(gal_obj, master_img_wcs, img_wcs, flip_)
         # factor used for scaling the Kron radius between different pixel scales
-        print(conv_factor)
 
         flux, flux_err = kron_flux(
             data_sub, bkg_rms, gain, gal_obj, kronrad * conv_factor, scale
         )
         flux, flux_err = flux[0], flux_err[0]
     else:
         # extract galaxy
```

### Comparing `hostphot-2.7.0/src/hostphot/image_cleaning.py` & `hostphot-2.7.1/src/hostphot/image_cleaning.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/image_masking.py` & `hostphot-2.7.1/src/hostphot/image_masking.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,21 +364,21 @@
         2 * r * gal_obj["b"][0],
         gal_obj["theta"][0] * 180.0 / np.pi,
         coords_frame="pixel",
         linewidth=3,
         edgecolor="r",
     )
 
-    # other sources markers
+    # other sources apertures
     fig2.show_ellipses(
         objects["x"],
         objects["y"],
         2 * r * objects["a"],
         2 * r * objects["b"],
-        gal_obj["theta"] * 180.0 / np.pi,
+        objects["theta"] * 180.0 / np.pi,
         coords_frame="pixel",
         linewidth=2,
         edgecolor="orangered",
         linestyle="dotted",
     )
 
     # SN marker
```

### Comparing `hostphot-2.7.0/src/hostphot/interactive_aperture.py` & `hostphot-2.7.1/src/hostphot/interactive_aperture.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/local_photometry.py` & `hostphot-2.7.1/src/hostphot/local_photometry.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/objects_detect.py` & `hostphot-2.7.1/src/hostphot/objects_detect.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/rgb_images.py` & `hostphot-2.7.1/src/hostphot/rgb_images.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot/utils.py` & `hostphot-2.7.1/src/hostphot/utils.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/src/hostphot.egg-info/PKG-INFO` & `hostphot-2.7.1/src/hostphot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.7.0
+Version: 2.7.1
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,17 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.7.1
+* Adding SED plotting
+* Fixed plotting angle of masked object 
 v2.7.0
 * MAJOR BUG: Convertion factor between different pixel scales fixed (it was previously inverted). This affects the common aperture photometry between different surveys!
 * Moving font family to `_constant.py` file
 v2.6.2
 * Prettier plots (now using `aplpy`), but also more informative!
 * Scale of the apertures for the masks is now a parameter (`r`) 
 * Raise exception is now `True` by default when calculating photometry
```

### Comparing `hostphot-2.7.0/src/hostphot.egg-info/SOURCES.txt` & `hostphot-2.7.1/src/hostphot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

```diff
@@ -13,14 +13,15 @@
 src/hostphot/global_photometry.py
 src/hostphot/image_cleaning.py
 src/hostphot/image_masking.py
 src/hostphot/interactive_aperture.py
 src/hostphot/local_photometry.py
 src/hostphot/objects_detect.py
 src/hostphot/rgb_images.py
+src/hostphot/sed_plotting.py
 src/hostphot/utils.py
 src/hostphot.egg-info/PKG-INFO
 src/hostphot.egg-info/SOURCES.txt
 src/hostphot.egg-info/dependency_links.txt
 src/hostphot.egg-info/requires.txt
 src/hostphot.egg-info/top_level.txt
 src/hostphot/filters/AAA_README
```

### Comparing `hostphot-2.7.0/tests/test_cutouts.py` & `hostphot-2.7.1/tests/test_cutouts.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/tests/test_global_phot.py` & `hostphot-2.7.1/tests/test_global_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/tests/test_local_phot.py` & `hostphot-2.7.1/tests/test_local_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/tests/test_preprocessing.py` & `hostphot-2.7.1/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.0/tests/test_rgb_images.py` & `hostphot-2.7.1/tests/test_rgb_images.py`

 * *Files identical despite different names*

