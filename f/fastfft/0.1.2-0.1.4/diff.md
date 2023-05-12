# Comparing `tmp/fastfft-0.1.2.tar.gz` & `tmp/fastfft-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.1.2.tar", last modified: Thu May 11 20:08:18 2023, max compression
+gzip compressed data, was "fastfft-0.1.4.tar", last modified: Fri May 12 11:25:02 2023, max compression
```

## Comparing `fastfft-0.1.2.tar` & `fastfft-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 20:08:18.293334 fastfft-0.1.2/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      337 2023-05-11 20:08:18.293217 fastfft-0.1.2/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.2/README.md
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 20:08:18.292909 fastfft-0.1.2/fastfft.egg-info/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      337 2023-05-11 20:08:18.000000 fastfft-0.1.2/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      202 2023-05-11 20:08:18.000000 fastfft-0.1.2/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-11 20:08:18.000000 fastfft-0.1.2/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      111 2023-05-11 20:08:18.000000 fastfft-0.1.2/fastfft.egg-info/requires.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        4 2023-05-11 20:08:18.000000 fastfft-0.1.2/fastfft.egg-info/top_level.txt
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      125 2023-05-11 20:07:27.000000 fastfft-0.1.2/pyproject.toml
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       38 2023-05-11 20:08:18.293365 fastfft-0.1.2/setup.cfg
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     2035 2023-05-11 20:07:06.000000 fastfft-0.1.2/setup.py
-drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-11 20:08:18.293005 fastfft-0.1.2/src/
--rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   114095 2023-05-11 20:08:18.000000 fastfft-0.1.2/src/__init__.c
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629638 fastfft-0.1.4/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1069 2023-05-12 10:51:03.000000 fastfft-0.1.4/LICENSE.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:25:02.629704 fastfft-0.1.4/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       80 2023-05-11 18:18:49.000000 fastfft-0.1.4/README.md
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      125 2023-05-11 20:07:27.000000 fastfft-0.1.4/pyproject.toml
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1477 2023-05-12 11:25:02.629976 fastfft-0.1.4/setup.cfg
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     3689 2023-05-12 11:09:35.000000 fastfft-0.1.4/setup.py
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.627877 fastfft-0.1.4/src/
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629137 fastfft-0.1.4/src/fastfft.egg-info/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)     1525 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      321 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        1 2023-05-12 11:21:18.000000 fastfft-0.1.4/src/fastfft.egg-info/not-zip-safe
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)       43 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/requires.txt
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        5 2023-05-12 11:25:02.000000 fastfft-0.1.4/src/fastfft.egg-info/top_level.txt
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629318 fastfft-0.1.4/src/fft2/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 10:56:37.000000 fastfft-0.1.4/src/fft2/__init__.py
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)   222791 2023-05-12 11:21:18.000000 fastfft-0.1.4/src/fft2/main.cpp
+drwxr-xr-x   0 maxim-movshin (1120574582) LD\Domain Users (593637566)        0 2023-05-12 11:25:02.629550 fastfft-0.1.4/tests/
+-rw-r--r--   0 maxim-movshin (1120574582) LD\Domain Users (593637566)      131 2023-05-12 11:18:47.000000 fastfft-0.1.4/tests/test_fft2.py
```

