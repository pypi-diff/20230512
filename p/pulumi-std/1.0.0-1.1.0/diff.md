# Comparing `tmp/pulumi_std-1.0.0.tar.gz` & `tmp/pulumi_std-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_std-1.0.0.tar", last modified: Tue Jan 17 17:55:39 2023, max compression
+gzip compressed data, was "pulumi_std-1.1.0.tar", last modified: Fri May 12 13:24:25 2023, max compression
```

## Comparing `pulumi_std-1.0.0.tar` & `pulumi_std-1.1.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:55:39.071383 pulumi_std-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-17 17:55:39.071383 pulumi_std-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:55:39.067383 pulumi_std-1.0.0/pulumi_std/
--rw-------   0 runner    (1001) docker     (123)     2583 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     1896 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/abs.py
--rw-------   0 runner    (1001) docker     (123)     2018 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/abspath.py
--rw-------   0 runner    (1001) docker     (123)     1943 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/alltrue.py
--rw-------   0 runner    (1001) docker     (123)     1959 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/anytrue.py
--rw-------   0 runner    (1001) docker     (123)     1904 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/base64decode.py
--rw-------   0 runner    (1001) docker     (123)     1876 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/base64encode.py
--rw-------   0 runner    (1001) docker     (123)     1872 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/base64gzip.py
--rw-------   0 runner    (1001) docker     (123)     2134 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/base64sha256.py
--rw-------   0 runner    (1001) docker     (123)     2134 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/base64sha512.py
--rw-------   0 runner    (1001) docker     (123)     1770 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/basename.py
--rw-------   0 runner    (1001) docker     (123)     2031 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/bcrypt.py
--rw-------   0 runner    (1001) docker     (123)     1762 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/ceil.py
--rw-------   0 runner    (1001) docker     (123)     1774 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/chomp.py
--rw-------   0 runner    (1001) docker     (123)     2053 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/chunklist.py
--rw-------   0 runner    (1001) docker     (123)     2427 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/cidrhost.py
--rw-------   0 runner    (1001) docker     (123)     2338 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/cidrnetmask.py
--rw-------   0 runner    (1001) docker     (123)     2568 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/cidrsubnet.py
--rw-------   0 runner    (1001) docker     (123)     1822 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/coalesce.py
--rw-------   0 runner    (1001) docker     (123)     1932 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/coalescelist.py
--rw-------   0 runner    (1001) docker     (123)     1782 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/compact.py
--rw-------   0 runner    (1001) docker     (123)     1792 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/concat.py
--rw-------   0 runner    (1001) docker     (123)     1992 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/contains.py
--rw-------   0 runner    (1001) docker     (123)     2800 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/csvdecode.py
--rw-------   0 runner    (1001) docker     (123)     1812 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/dirname.py
--rw-------   0 runner    (1001) docker     (123)     1788 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/distinct.py
--rw-------   0 runner    (1001) docker     (123)     1907 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/element.py
--rw-------   0 runner    (1001) docker     (123)     1930 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/endswith.py
--rw-------   0 runner    (1001) docker     (123)     1702 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/file.py
--rw-------   0 runner    (1001) docker     (123)     1866 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filebase64.py
--rw-------   0 runner    (1001) docker     (123)     2012 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filebase64sha256.py
--rw-------   0 runner    (1001) docker     (123)     2012 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filebase64sha512.py
--rw-------   0 runner    (1001) docker     (123)     1821 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/fileexists.py
--rw-------   0 runner    (1001) docker     (123)     1814 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filemd5.py
--rw-------   0 runner    (1001) docker     (123)     1834 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filesha1.py
--rw-------   0 runner    (1001) docker     (123)     1874 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filesha256.py
--rw-------   0 runner    (1001) docker     (123)     1874 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/filesha512.py
--rw-------   0 runner    (1001) docker     (123)     1918 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/flatten.py
--rw-------   0 runner    (1001) docker     (123)     1780 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/floor.py
--rw-------   0 runner    (1001) docker     (123)     1997 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/format.py
--rw-------   0 runner    (1001) docker     (123)     1941 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/indent.py
--rw-------   0 runner    (1001) docker     (123)     1863 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/index.py
--rw-------   0 runner    (1001) docker     (123)     1889 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/join.py
--rw-------   0 runner    (1001) docker     (123)     2078 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/jsondecode.py
--rw-------   0 runner    (1001) docker     (123)     2094 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/jsonencode.py
--rw-------   0 runner    (1001) docker     (123)     1748 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/keys.py
--rw-------   0 runner    (1001) docker     (123)     1742 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/length.py
--rw-------   0 runner    (1001) docker     (123)     1869 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/log.py
--rw-------   0 runner    (1001) docker     (123)     2034 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/lookup.py
--rw-------   0 runner    (1001) docker     (123)     1792 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/lower.py
--rw-------   0 runner    (1001) docker     (123)     1768 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/map.py
--rw-------   0 runner    (1001) docker     (123)     2228 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/matchkeys.py
--rw-------   0 runner    (1001) docker     (123)     1692 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/max.py
--rw-------   0 runner    (1001) docker     (123)     1770 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/md5.py
--rw-------   0 runner    (1001) docker     (123)     1958 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/merge.py
--rw-------   0 runner    (1001) docker     (123)     1694 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/min.py
--rw-------   0 runner    (1001) docker     (123)     2163 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/parseint.py
--rw-------   0 runner    (1001) docker     (123)     1848 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/pathexpand.py
--rw-------   0 runner    (1001) docker     (123)     1859 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/pow.py
--rw-------   0 runner    (1001) docker     (123)     2707 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/provider.py
--rw-------   0 runner    (1001) docker     (123)       40 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/py.typed
--rw-------   0 runner    (1001) docker     (123)     2466 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/range.py
--rw-------   0 runner    (1001) docker     (123)     2840 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/replace.py
--rw-------   0 runner    (1001) docker     (123)     1824 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/reverse.py
--rw-------   0 runner    (1001) docker     (123)     2104 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/rsadecrypt.py
--rw-------   0 runner    (1001) docker     (123)     1762 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/sha1.py
--rw-------   0 runner    (1001) docker     (123)     1802 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/sha256.py
--rw-------   0 runner    (1001) docker     (123)     1802 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/sha512.py
--rw-------   0 runner    (1001) docker     (123)     1798 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/signum.py
--rw-------   0 runner    (1001) docker     (123)     2067 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/slice.py
--rw-------   0 runner    (1001) docker     (123)     1746 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/sort.py
--rw-------   0 runner    (1001) docker     (123)     1947 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/split.py
--rw-------   0 runner    (1001) docker     (123)     1974 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/startswith.py
--rw-------   0 runner    (1001) docker     (123)     1802 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/strrev.py
--rw-------   0 runner    (1001) docker     (123)     2004 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/substr.py
--rw-------   0 runner    (1001) docker     (123)     1736 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/sum.py
--rw-------   0 runner    (1001) docker     (123)     2889 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/timeadd.py
--rw-------   0 runner    (1001) docker     (123)     2813 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/timecmp.py
--rw-------   0 runner    (1001) docker     (123)     1438 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/timestamp.py
--rw-------   0 runner    (1001) docker     (123)     1774 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/title.py
--rw-------   0 runner    (1001) docker     (123)     2017 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/tobool.py
--rw-------   0 runner    (1001) docker     (123)     1756 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/tolist.py
--rw-------   0 runner    (1001) docker     (123)     2082 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/tonumber.py
--rw-------   0 runner    (1001) docker     (123)     1736 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/toset.py
--rw-------   0 runner    (1001) docker     (123)     2016 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/tostring.py
--rw-------   0 runner    (1001) docker     (123)     1980 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/transpose.py
--rw-------   0 runner    (1001) docker     (123)     1909 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/trim.py
--rw-------   0 runner    (1001) docker     (123)     2015 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/trimprefix.py
--rw-------   0 runner    (1001) docker     (123)     2024 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/trimspace.py
--rw-------   0 runner    (1001) docker     (123)     2011 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/trimsuffix.py
--rw-------   0 runner    (1001) docker     (123)     1750 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/upper.py
--rw-------   0 runner    (1001) docker     (123)     1780 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/urlencode.py
--rw-------   0 runner    (1001) docker     (123)     1393 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/uuid.py
--rw-------   0 runner    (1001) docker     (123)     1768 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/values.py
--rw-------   0 runner    (1001) docker     (123)     1979 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/pulumi_std/zipmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:55:39.071383 pulumi_std-1.0.0/pulumi_std.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-17 17:55:39.000000 pulumi_std-1.0.0/pulumi_std.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-17 17:55:39.000000 pulumi_std-1.0.0/pulumi_std.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 17:55:39.000000 pulumi_std-1.0.0/pulumi_std.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 17:55:39.000000 pulumi_std-1.0.0/pulumi_std.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-17 17:55:39.000000 pulumi_std-1.0.0/pulumi_std.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-17 17:55:39.000000 pulumi_std-1.0.0/pulumi_std.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 17:55:39.071383 pulumi_std-1.0.0/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     1937 2023-01-17 17:55:38.000000 pulumi_std-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:25.446937 pulumi_std-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-12 13:24:25.446937 pulumi_std-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:25.446937 pulumi_std-1.1.0/pulumi_std/
+-rw-------   0 runner    (1001) docker     (123)     2583 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8047 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     1896 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/abs.py
+-rw-------   0 runner    (1001) docker     (123)     2018 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/abspath.py
+-rw-------   0 runner    (1001) docker     (123)     1943 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/alltrue.py
+-rw-------   0 runner    (1001) docker     (123)     1959 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/anytrue.py
+-rw-------   0 runner    (1001) docker     (123)     1904 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/base64decode.py
+-rw-------   0 runner    (1001) docker     (123)     1876 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/base64encode.py
+-rw-------   0 runner    (1001) docker     (123)     1872 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/base64gzip.py
+-rw-------   0 runner    (1001) docker     (123)     2134 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/base64sha256.py
+-rw-------   0 runner    (1001) docker     (123)     2134 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/base64sha512.py
+-rw-------   0 runner    (1001) docker     (123)     1770 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/basename.py
+-rw-------   0 runner    (1001) docker     (123)     2031 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/bcrypt.py
+-rw-------   0 runner    (1001) docker     (123)     1762 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/ceil.py
+-rw-------   0 runner    (1001) docker     (123)     1774 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/chomp.py
+-rw-------   0 runner    (1001) docker     (123)     2053 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/chunklist.py
+-rw-------   0 runner    (1001) docker     (123)     2427 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/cidrhost.py
+-rw-------   0 runner    (1001) docker     (123)     2338 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/cidrnetmask.py
+-rw-------   0 runner    (1001) docker     (123)     2568 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/cidrsubnet.py
+-rw-------   0 runner    (1001) docker     (123)     1822 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/coalesce.py
+-rw-------   0 runner    (1001) docker     (123)     1932 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/coalescelist.py
+-rw-------   0 runner    (1001) docker     (123)     1782 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/compact.py
+-rw-------   0 runner    (1001) docker     (123)     1792 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/concat.py
+-rw-------   0 runner    (1001) docker     (123)     1992 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/contains.py
+-rw-------   0 runner    (1001) docker     (123)     2800 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/csvdecode.py
+-rw-------   0 runner    (1001) docker     (123)     1812 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/dirname.py
+-rw-------   0 runner    (1001) docker     (123)     1788 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/distinct.py
+-rw-------   0 runner    (1001) docker     (123)     1907 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/element.py
+-rw-------   0 runner    (1001) docker     (123)     1930 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/endswith.py
+-rw-------   0 runner    (1001) docker     (123)     1702 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/file.py
+-rw-------   0 runner    (1001) docker     (123)     1866 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filebase64.py
+-rw-------   0 runner    (1001) docker     (123)     2012 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filebase64sha256.py
+-rw-------   0 runner    (1001) docker     (123)     2012 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filebase64sha512.py
+-rw-------   0 runner    (1001) docker     (123)     1821 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/fileexists.py
+-rw-------   0 runner    (1001) docker     (123)     1814 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filemd5.py
+-rw-------   0 runner    (1001) docker     (123)     1834 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filesha1.py
+-rw-------   0 runner    (1001) docker     (123)     1874 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filesha256.py
+-rw-------   0 runner    (1001) docker     (123)     1874 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/filesha512.py
+-rw-------   0 runner    (1001) docker     (123)     1918 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/flatten.py
+-rw-------   0 runner    (1001) docker     (123)     1780 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/floor.py
+-rw-------   0 runner    (1001) docker     (123)     1997 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/format.py
+-rw-------   0 runner    (1001) docker     (123)     1941 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/indent.py
+-rw-------   0 runner    (1001) docker     (123)     1863 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/index.py
+-rw-------   0 runner    (1001) docker     (123)     1889 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/join.py
+-rw-------   0 runner    (1001) docker     (123)     2078 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/jsondecode.py
+-rw-------   0 runner    (1001) docker     (123)     2094 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/jsonencode.py
+-rw-------   0 runner    (1001) docker     (123)     1748 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/keys.py
+-rw-------   0 runner    (1001) docker     (123)     1742 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/length.py
+-rw-------   0 runner    (1001) docker     (123)     1869 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/log.py
+-rw-------   0 runner    (1001) docker     (123)     2034 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/lookup.py
+-rw-------   0 runner    (1001) docker     (123)     1792 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/lower.py
+-rw-------   0 runner    (1001) docker     (123)     1768 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/map.py
+-rw-------   0 runner    (1001) docker     (123)     2228 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/matchkeys.py
+-rw-------   0 runner    (1001) docker     (123)     1692 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/max.py
+-rw-------   0 runner    (1001) docker     (123)     1770 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/md5.py
+-rw-------   0 runner    (1001) docker     (123)     1958 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/merge.py
+-rw-------   0 runner    (1001) docker     (123)     1694 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/min.py
+-rw-------   0 runner    (1001) docker     (123)     2163 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/parseint.py
+-rw-------   0 runner    (1001) docker     (123)     1848 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/pathexpand.py
+-rw-------   0 runner    (1001) docker     (123)     1859 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/pow.py
+-rw-------   0 runner    (1001) docker     (123)     2707 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/provider.py
+-rw-------   0 runner    (1001) docker     (123)       40 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/py.typed
+-rw-------   0 runner    (1001) docker     (123)     2466 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/range.py
+-rw-------   0 runner    (1001) docker     (123)     2840 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/replace.py
+-rw-------   0 runner    (1001) docker     (123)     1824 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/reverse.py
+-rw-------   0 runner    (1001) docker     (123)     2104 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/rsadecrypt.py
+-rw-------   0 runner    (1001) docker     (123)     1762 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/sha1.py
+-rw-------   0 runner    (1001) docker     (123)     1802 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/sha256.py
+-rw-------   0 runner    (1001) docker     (123)     1802 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/sha512.py
+-rw-------   0 runner    (1001) docker     (123)     1798 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/signum.py
+-rw-------   0 runner    (1001) docker     (123)     2067 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/slice.py
+-rw-------   0 runner    (1001) docker     (123)     1746 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/sort.py
+-rw-------   0 runner    (1001) docker     (123)     1947 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/split.py
+-rw-------   0 runner    (1001) docker     (123)     1974 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/startswith.py
+-rw-------   0 runner    (1001) docker     (123)     1802 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/strrev.py
+-rw-------   0 runner    (1001) docker     (123)     2004 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/substr.py
+-rw-------   0 runner    (1001) docker     (123)     1736 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/sum.py
+-rw-------   0 runner    (1001) docker     (123)     2889 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/timeadd.py
+-rw-------   0 runner    (1001) docker     (123)     2813 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/timecmp.py
+-rw-------   0 runner    (1001) docker     (123)     1438 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/timestamp.py
+-rw-------   0 runner    (1001) docker     (123)     1774 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/title.py
+-rw-------   0 runner    (1001) docker     (123)     2017 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/tobool.py
+-rw-------   0 runner    (1001) docker     (123)     1756 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/tolist.py
+-rw-------   0 runner    (1001) docker     (123)     2082 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/tonumber.py
+-rw-------   0 runner    (1001) docker     (123)     1736 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/toset.py
+-rw-------   0 runner    (1001) docker     (123)     2016 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/tostring.py
+-rw-------   0 runner    (1001) docker     (123)     1980 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/transpose.py
+-rw-------   0 runner    (1001) docker     (123)     1909 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/trim.py
+-rw-------   0 runner    (1001) docker     (123)     2015 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/trimprefix.py
+-rw-------   0 runner    (1001) docker     (123)     2024 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/trimspace.py
+-rw-------   0 runner    (1001) docker     (123)     2011 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/trimsuffix.py
+-rw-------   0 runner    (1001) docker     (123)     1750 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/upper.py
+-rw-------   0 runner    (1001) docker     (123)     1780 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/urlencode.py
+-rw-------   0 runner    (1001) docker     (123)     1393 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/uuid.py
+-rw-------   0 runner    (1001) docker     (123)     1768 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/values.py
+-rw-------   0 runner    (1001) docker     (123)     1979 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std/zipmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:25.446937 pulumi_std-1.1.0/pulumi_std.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/pulumi_std.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:24:25.446937 pulumi_std-1.1.0/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     1968 2023-05-12 13:24:25.000000 pulumi_std-1.1.0/setup.py
```

### Comparing `pulumi_std-1.0.0/pulumi_std/__init__.py` & `pulumi_std-1.1.0/pulumi_std/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/_utilities.py` & `pulumi_std-1.1.0/pulumi_std/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/abs.py` & `pulumi_std-1.1.0/pulumi_std/abs.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/abspath.py` & `pulumi_std-1.1.0/pulumi_std/abspath.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/alltrue.py` & `pulumi_std-1.1.0/pulumi_std/alltrue.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/anytrue.py` & `pulumi_std-1.1.0/pulumi_std/anytrue.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/base64decode.py` & `pulumi_std-1.1.0/pulumi_std/base64decode.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/base64encode.py` & `pulumi_std-1.1.0/pulumi_std/base64encode.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/base64gzip.py` & `pulumi_std-1.1.0/pulumi_std/base64gzip.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/base64sha256.py` & `pulumi_std-1.1.0/pulumi_std/base64sha256.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/base64sha512.py` & `pulumi_std-1.1.0/pulumi_std/base64sha512.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/basename.py` & `pulumi_std-1.1.0/pulumi_std/basename.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/bcrypt.py` & `pulumi_std-1.1.0/pulumi_std/bcrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/ceil.py` & `pulumi_std-1.1.0/pulumi_std/ceil.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/chomp.py` & `pulumi_std-1.1.0/pulumi_std/chomp.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/chunklist.py` & `pulumi_std-1.1.0/pulumi_std/chunklist.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/cidrhost.py` & `pulumi_std-1.1.0/pulumi_std/cidrhost.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/cidrnetmask.py` & `pulumi_std-1.1.0/pulumi_std/cidrnetmask.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/cidrsubnet.py` & `pulumi_std-1.1.0/pulumi_std/cidrsubnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/coalesce.py` & `pulumi_std-1.1.0/pulumi_std/coalesce.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/coalescelist.py` & `pulumi_std-1.1.0/pulumi_std/coalescelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/compact.py` & `pulumi_std-1.1.0/pulumi_std/compact.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/concat.py` & `pulumi_std-1.1.0/pulumi_std/concat.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/contains.py` & `pulumi_std-1.1.0/pulumi_std/contains.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/csvdecode.py` & `pulumi_std-1.1.0/pulumi_std/csvdecode.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/dirname.py` & `pulumi_std-1.1.0/pulumi_std/dirname.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/distinct.py` & `pulumi_std-1.1.0/pulumi_std/distinct.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/element.py` & `pulumi_std-1.1.0/pulumi_std/element.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/endswith.py` & `pulumi_std-1.1.0/pulumi_std/endswith.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/file.py` & `pulumi_std-1.1.0/pulumi_std/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filebase64.py` & `pulumi_std-1.1.0/pulumi_std/filebase64.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filebase64sha256.py` & `pulumi_std-1.1.0/pulumi_std/filebase64sha256.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filebase64sha512.py` & `pulumi_std-1.1.0/pulumi_std/filebase64sha512.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/fileexists.py` & `pulumi_std-1.1.0/pulumi_std/fileexists.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filemd5.py` & `pulumi_std-1.1.0/pulumi_std/filemd5.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filesha1.py` & `pulumi_std-1.1.0/pulumi_std/filesha1.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filesha256.py` & `pulumi_std-1.1.0/pulumi_std/filesha256.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/filesha512.py` & `pulumi_std-1.1.0/pulumi_std/filesha512.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/flatten.py` & `pulumi_std-1.1.0/pulumi_std/flatten.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/floor.py` & `pulumi_std-1.1.0/pulumi_std/floor.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/format.py` & `pulumi_std-1.1.0/pulumi_std/format.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/indent.py` & `pulumi_std-1.1.0/pulumi_std/indent.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/index.py` & `pulumi_std-1.1.0/pulumi_std/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/join.py` & `pulumi_std-1.1.0/pulumi_std/join.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/jsondecode.py` & `pulumi_std-1.1.0/pulumi_std/jsondecode.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/jsonencode.py` & `pulumi_std-1.1.0/pulumi_std/jsonencode.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/keys.py` & `pulumi_std-1.1.0/pulumi_std/keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/length.py` & `pulumi_std-1.1.0/pulumi_std/length.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/log.py` & `pulumi_std-1.1.0/pulumi_std/log.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/lookup.py` & `pulumi_std-1.1.0/pulumi_std/lookup.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/lower.py` & `pulumi_std-1.1.0/pulumi_std/lower.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/map.py` & `pulumi_std-1.1.0/pulumi_std/map.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/matchkeys.py` & `pulumi_std-1.1.0/pulumi_std/matchkeys.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/max.py` & `pulumi_std-1.1.0/pulumi_std/max.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/md5.py` & `pulumi_std-1.1.0/pulumi_std/md5.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/merge.py` & `pulumi_std-1.1.0/pulumi_std/merge.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/min.py` & `pulumi_std-1.1.0/pulumi_std/min.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/parseint.py` & `pulumi_std-1.1.0/pulumi_std/parseint.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/pathexpand.py` & `pulumi_std-1.1.0/pulumi_std/pathexpand.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/pow.py` & `pulumi_std-1.1.0/pulumi_std/pow.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/provider.py` & `pulumi_std-1.1.0/pulumi_std/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/range.py` & `pulumi_std-1.1.0/pulumi_std/range.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/replace.py` & `pulumi_std-1.1.0/pulumi_std/replace.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/reverse.py` & `pulumi_std-1.1.0/pulumi_std/reverse.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/rsadecrypt.py` & `pulumi_std-1.1.0/pulumi_std/rsadecrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/sha1.py` & `pulumi_std-1.1.0/pulumi_std/sha1.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/sha256.py` & `pulumi_std-1.1.0/pulumi_std/sha256.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/sha512.py` & `pulumi_std-1.1.0/pulumi_std/sha512.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/signum.py` & `pulumi_std-1.1.0/pulumi_std/signum.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/slice.py` & `pulumi_std-1.1.0/pulumi_std/slice.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/sort.py` & `pulumi_std-1.1.0/pulumi_std/sort.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/split.py` & `pulumi_std-1.1.0/pulumi_std/split.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/startswith.py` & `pulumi_std-1.1.0/pulumi_std/startswith.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/strrev.py` & `pulumi_std-1.1.0/pulumi_std/strrev.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/substr.py` & `pulumi_std-1.1.0/pulumi_std/substr.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/sum.py` & `pulumi_std-1.1.0/pulumi_std/sum.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/timeadd.py` & `pulumi_std-1.1.0/pulumi_std/timeadd.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/timecmp.py` & `pulumi_std-1.1.0/pulumi_std/timecmp.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/timestamp.py` & `pulumi_std-1.1.0/pulumi_std/timestamp.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/title.py` & `pulumi_std-1.1.0/pulumi_std/title.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/tobool.py` & `pulumi_std-1.1.0/pulumi_std/tobool.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/tolist.py` & `pulumi_std-1.1.0/pulumi_std/tolist.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/tonumber.py` & `pulumi_std-1.1.0/pulumi_std/tonumber.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/toset.py` & `pulumi_std-1.1.0/pulumi_std/toset.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/tostring.py` & `pulumi_std-1.1.0/pulumi_std/tostring.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/transpose.py` & `pulumi_std-1.1.0/pulumi_std/transpose.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/trim.py` & `pulumi_std-1.1.0/pulumi_std/trim.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/trimprefix.py` & `pulumi_std-1.1.0/pulumi_std/trimprefix.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/trimspace.py` & `pulumi_std-1.1.0/pulumi_std/trimspace.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/trimsuffix.py` & `pulumi_std-1.1.0/pulumi_std/trimsuffix.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/upper.py` & `pulumi_std-1.1.0/pulumi_std/upper.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/urlencode.py` & `pulumi_std-1.1.0/pulumi_std/urlencode.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/uuid.py` & `pulumi_std-1.1.0/pulumi_std/uuid.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/values.py` & `pulumi_std-1.1.0/pulumi_std/values.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std/zipmap.py` & `pulumi_std-1.1.0/pulumi_std/zipmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/pulumi_std.egg-info/SOURCES.txt` & `pulumi_std-1.1.0/pulumi_std.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_std-1.0.0/setup.py` & `pulumi_std-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.0"
-PLUGIN_VERSION = "1.0.0"
+VERSION = "1.1.0"
+PLUGIN_VERSION = "1.1.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'std', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "std Pulumi Package - Development Version"
 
 
 setup(name='pulumi_std',
+      python_requires='>=3.7',
       version=VERSION,
       description="Standard library functions",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

