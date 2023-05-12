# Comparing `tmp/rns-0.5.1.tar.gz` & `tmp/rns-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rns-0.5.1.tar", last modified: Fri May  5 09:18:33 2023, max compression
+gzip compressed data, was "rns-0.5.2.tar", last modified: Fri May 12 10:36:53 2023, max compression
```

## Comparing `rns-0.5.1.tar` & `rns-0.5.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.936600 rns-0.5.1/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rns-0.5.1/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-05-05 09:18:33.936600 rns-0.5.1/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rns-0.5.1/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10082 2023-03-05 17:21:52.000000 rns-0.5.1/RNS/Buffer.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19810 2023-03-05 17:21:52.000000 rns-0.5.1/RNS/Channel.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/Cryptography/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/AES.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/Ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/Fernet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rns-0.5.1/RNS/Cryptography/HKDF.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/HMAC.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/Hashes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/PKCS7.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/Provider.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/Proxies.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/SHA256.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/SHA512.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/X25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/Cryptography/aes/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/aes/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/aes/aes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/aes/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/Cryptography/pure25519/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/pure25519/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/pure25519/_ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/pure25519/basic.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/pure25519/ed25519_oop.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Cryptography/pure25519/eddsa.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rns-0.5.1/RNS/Destination.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24033 2022-12-21 18:12:50.000000 rns-0.5.1/RNS/Identity.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/Interfaces/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Interfaces/AX25KISSInterface.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/Interfaces/Android/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rns-0.5.1/RNS/Interfaces/Android/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49037 2023-05-02 15:44:28.000000 rns-0.5.1/RNS/Interfaces/Android/RNodeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rns-0.5.1/RNS/Interfaces/Android/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rns-0.5.1/RNS/Interfaces/Android/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20050 2023-05-04 15:53:57.000000 rns-0.5.1/RNS/Interfaces/AutoInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rns-0.5.1/RNS/Interfaces/I2PInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Interfaces/Interface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Interfaces/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-03 10:21:20.000000 rns-0.5.1/RNS/Interfaces/LocalInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Interfaces/PipeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30633 2023-05-02 15:44:01.000000 rns-0.5.1/RNS/Interfaces/RNodeInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Interfaces/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rns-0.5.1/RNS/Interfaces/TCPInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rns-0.5.1/RNS/Interfaces/UDPInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rns-0.5.1/RNS/Interfaces/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    52133 2023-03-05 17:21:52.000000 rns-0.5.1/RNS/Link.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    21750 2023-05-02 15:27:36.000000 rns-0.5.1/RNS/Packet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45889 2022-12-19 00:09:16.000000 rns-0.5.1/RNS/Resource.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rns-0.5.1/RNS/Reticulum.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129918 2023-03-05 17:21:52.000000 rns-0.5.1/RNS/Transport.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.933266 rns-0.5.1/RNS/Utilities/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Utilities/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14872 2023-02-02 12:40:06.000000 rns-0.5.1/RNS/Utilities/rncp.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-02-03 19:26:09.000000 rns-0.5.1/RNS/Utilities/rnid.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)   205846 2023-05-03 13:56:01.000000 rns-0.5.1/RNS/Utilities/rnodeconf.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Utilities/rnpath.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/Utilities/rnprobe.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rns-0.5.1/RNS/Utilities/rnsd.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rns-0.5.1/RNS/Utilities/rnstatus.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rns-0.5.1/RNS/Utilities/rnx.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rns-0.5.1/RNS/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-05-03 10:25:12.000000 rns-0.5.1/RNS/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.936600 rns-0.5.1/RNS/vendor/
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/__init__.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/configobj.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.936600 rns-0.5.1/RNS/vendor/i2plib/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/__version__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/aiosam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/exceptions.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/sam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/tunnel.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/i2plib/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.936600 rns-0.5.1/RNS/vendor/ifaddr/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rns-0.5.1/RNS/vendor/ifaddr/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rns-0.5.1/RNS/vendor/ifaddr/_posix.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rns-0.5.1/RNS/vendor/ifaddr/_shared.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rns-0.5.1/RNS/vendor/ifaddr/_win32.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rns-0.5.1/RNS/vendor/ifaddr/niwrapper.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rns-0.5.1/RNS/vendor/platformutils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/six.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rns-0.5.1/RNS/vendor/umsgpack.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-05 09:18:33.936600 rns-0.5.1/rns.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-05-05 09:18:33.000000 rns-0.5.1/rns.egg-info/PKG-INFO
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2237 2023-05-05 09:18:33.000000 rns-0.5.1/rns.egg-info/SOURCES.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-05-05 09:18:33.000000 rns-0.5.1/rns.egg-info/dependency_links.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-05-05 09:18:33.000000 rns-0.5.1/rns.egg-info/entry_points.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       34 2023-05-05 09:18:33.000000 rns-0.5.1/rns.egg-info/requires.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-05-05 09:18:33.000000 rns-0.5.1/rns.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-05-05 09:18:33.936600 rns-0.5.1/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rns-0.5.1/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.864273 rns-0.5.2/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rns-0.5.2/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-05-12 10:36:53.864273 rns-0.5.2/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rns-0.5.2/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.857606 rns-0.5.2/RNS/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10508 2023-05-10 16:48:56.000000 rns-0.5.2/RNS/Buffer.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24440 2023-05-11 19:18:34.000000 rns-0.5.2/RNS/Channel.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.860940 rns-0.5.2/RNS/Cryptography/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/AES.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/Ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/Fernet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rns-0.5.2/RNS/Cryptography/HKDF.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/HMAC.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/Hashes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/PKCS7.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/Provider.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/Proxies.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/SHA256.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/SHA512.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/X25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.860940 rns-0.5.2/RNS/Cryptography/aes/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/aes/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/aes/aes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/aes/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.860940 rns-0.5.2/RNS/Cryptography/pure25519/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/pure25519/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/pure25519/_ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/pure25519/basic.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/pure25519/ed25519_oop.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Cryptography/pure25519/eddsa.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rns-0.5.2/RNS/Destination.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24033 2022-12-21 18:12:50.000000 rns-0.5.2/RNS/Identity.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.860940 rns-0.5.2/RNS/Interfaces/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Interfaces/AX25KISSInterface.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.860940 rns-0.5.2/RNS/Interfaces/Android/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rns-0.5.2/RNS/Interfaces/Android/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49037 2023-05-02 15:44:28.000000 rns-0.5.2/RNS/Interfaces/Android/RNodeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rns-0.5.2/RNS/Interfaces/Android/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rns-0.5.2/RNS/Interfaces/Android/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rns-0.5.2/RNS/Interfaces/AutoInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rns-0.5.2/RNS/Interfaces/I2PInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Interfaces/Interface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Interfaces/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rns-0.5.2/RNS/Interfaces/LocalInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Interfaces/PipeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30633 2023-05-02 15:44:01.000000 rns-0.5.2/RNS/Interfaces/RNodeInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Interfaces/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rns-0.5.2/RNS/Interfaces/TCPInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rns-0.5.2/RNS/Interfaces/UDPInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rns-0.5.2/RNS/Interfaces/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    52943 2023-05-11 14:21:07.000000 rns-0.5.2/RNS/Link.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-11 13:48:09.000000 rns-0.5.2/RNS/Packet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rns-0.5.2/RNS/Resource.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rns-0.5.2/RNS/Reticulum.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129920 2023-05-11 13:43:33.000000 rns-0.5.2/RNS/Transport.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.864273 rns-0.5.2/RNS/Utilities/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Utilities/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14872 2023-02-02 12:40:06.000000 rns-0.5.2/RNS/Utilities/rncp.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-05-09 18:30:37.000000 rns-0.5.2/RNS/Utilities/rnid.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208355 2023-05-09 13:30:30.000000 rns-0.5.2/RNS/Utilities/rnodeconf.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Utilities/rnpath.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/Utilities/rnprobe.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rns-0.5.2/RNS/Utilities/rnsd.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rns-0.5.2/RNS/Utilities/rnstatus.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rns-0.5.2/RNS/Utilities/rnx.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rns-0.5.2/RNS/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-05-09 21:07:38.000000 rns-0.5.2/RNS/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.864273 rns-0.5.2/RNS/vendor/
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/__init__.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/configobj.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.864273 rns-0.5.2/RNS/vendor/i2plib/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/__version__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/aiosam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/exceptions.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/sam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/tunnel.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/i2plib/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.864273 rns-0.5.2/RNS/vendor/ifaddr/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rns-0.5.2/RNS/vendor/ifaddr/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rns-0.5.2/RNS/vendor/ifaddr/_posix.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rns-0.5.2/RNS/vendor/ifaddr/_shared.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rns-0.5.2/RNS/vendor/ifaddr/_win32.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rns-0.5.2/RNS/vendor/ifaddr/niwrapper.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rns-0.5.2/RNS/vendor/platformutils.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/six.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rns-0.5.2/RNS/vendor/umsgpack.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:53.864273 rns-0.5.2/rns.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-05-12 10:36:53.000000 rns-0.5.2/rns.egg-info/PKG-INFO
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2237 2023-05-12 10:36:53.000000 rns-0.5.2/rns.egg-info/SOURCES.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-05-12 10:36:53.000000 rns-0.5.2/rns.egg-info/dependency_links.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-05-12 10:36:53.000000 rns-0.5.2/rns.egg-info/entry_points.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       34 2023-05-12 10:36:53.000000 rns-0.5.2/rns.egg-info/requires.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-05-12 10:36:53.000000 rns-0.5.2/rns.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-05-12 10:36:53.864273 rns-0.5.2/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rns-0.5.2/setup.py
```

### Comparing `rns-0.5.1/LICENSE` & `rns-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/PKG-INFO` & `rns-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rns
-Version: 0.5.1
+Version: 0.5.2
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rns-0.5.1/README.md` & `rns-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Buffer.py` & `rns-0.5.2/RNS/Buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
+import bz2
 import sys
 import threading
 from threading import RLock
 import struct
 from RNS.Channel import Channel, MessageBase, SystemMessageTypes
 import RNS
 from io import RawIOBase, BufferedRWPair, BufferedReader, BufferedWriter
 from typing import Callable
 from contextlib import AbstractContextManager
 
-
 class StreamDataMessage(MessageBase):
     MSGTYPE = SystemMessageTypes.SMT_STREAM_DATA
     """
     Message type for ``Channel``. ``StreamDataMessage``
     uses a system-reserved message type.
     """
 
-    STREAM_ID_MAX = 0x7fff  # 32767
+    STREAM_ID_MAX = 0x3fff  # 16383
     """
-    The stream id is limited to 2 bytes - 1 bit
+    The stream id is limited to 2 bytes - 2 bit
     """
 
     MAX_DATA_LEN = RNS.Link.MDU - 2 - 6  # 2 for stream data message header, 6 for channel envelope
     """
     When the Buffer package is imported, this value is
     calculcated based on the value of OVERHEAD
     """
@@ -35,30 +35,42 @@
 
         :param stream_id: id of stream relative to receiver
         :param data: binary data
         :param eof: set to True if signalling End of File
         """
         super().__init__()
         if stream_id is not None and stream_id > self.STREAM_ID_MAX:
-            raise ValueError("stream_id must be 0-32767")
+            raise ValueError("stream_id must be 0-16383")
         self.stream_id = stream_id
+        self.compressed = False
         self.data = data or bytes()
         self.eof = eof
 
     def pack(self) -> bytes:
         if self.stream_id is None:
             raise ValueError("stream_id")
-        header_val = (0x7fff & self.stream_id) | (0x8000 if self.eof else 0x0000)
+
+        compressed_data   = bz2.compress(self.data)
+        saved = len(self.data)-len(compressed_data)
+
+        if saved > 0:
+            self.data = compressed_data
+            self.compressed = True
+
+        header_val = (0x3fff & self.stream_id) | (0x8000 if self.eof else 0x0000) | (0x4000 if self.compressed > 0 else 0x0000)
         return bytes(struct.pack(">H", header_val) + (self.data if self.data else bytes()))
 
     def unpack(self, raw):
         self.stream_id = struct.unpack(">H", raw[:2])[0]
         self.eof = (0x8000 & self.stream_id) > 0
-        self.stream_id = self.stream_id & 0x7fff
+        self.compressed = (0x4000 & self.stream_id) > 0
+        self.stream_id = self.stream_id & 0x3fff
         self.data = raw[2:]
+        if self.compressed:
+            self.data = bz2.decompress(self.data)
 
 
 class RawChannelReader(RawIOBase, AbstractContextManager):
     """
     An implementation of RawIOBase that receives
     binary stream data sent over a ``Channel``.
```

### Comparing `rns-0.5.1/RNS/Channel.py` & `rns-0.5.2/RNS/Channel.py`

 * *Files 13% similar despite different names*

```diff
@@ -219,27 +219,79 @@
     provides reliable delivery (automatic retries) as well
     as a structure for exchanging several types of
     messages over the ``Link``.
 
     ``Channel`` is not instantiated directly, but rather
     obtained from a ``Link`` with ``get_channel()``.
     """
+
+    # The initial window size at channel setup
+    WINDOW     = 2
+
+    # Absolute minimum window size
+    WINDOW_MIN = 1
+
+    # The maximum window size for transfers on slow links
+    WINDOW_MAX_SLOW      = 5
+
+    # The maximum window size for transfers on mid-speed links
+    WINDOW_MAX_MEDIUM    = 16
+
+    # The maximum window size for transfers on fast links
+    WINDOW_MAX_FAST      = 48
+    
+    # For calculating maps and guard segments, this
+    # must be set to the global maximum window.
+    WINDOW_MAX           = WINDOW_MAX_FAST
+    
+    # If the fast rate is sustained for this many request
+    # rounds, the fast link window size will be allowed.
+    FAST_RATE_THRESHOLD  = 10
+
+    # If the RTT rate is higher than this value,
+    # the max window size for fast links will be used.
+    RTT_FAST            = 0.25
+    RTT_MEDIUM          = 0.75
+    RTT_SLOW            = 1.45
+
+    # The minimum allowed flexibility of the window size.
+    # The difference between window_max and window_min
+    # will never be smaller than this value.
+    WINDOW_FLEXIBILITY   = 4
+
+    SEQ_MAX     = 0xFFFF
+    SEQ_MODULUS = SEQ_MAX+1
+
     def __init__(self, outlet: ChannelOutletBase):
         """
 
         @param outlet:
         """
         self._outlet = outlet
         self._lock = threading.RLock()
         self._tx_ring: collections.deque[Envelope] = collections.deque()
         self._rx_ring: collections.deque[Envelope] = collections.deque()
         self._message_callbacks: [MessageCallbackType] = []
         self._next_sequence = 0
+        self._next_rx_sequence = 0
         self._message_factories: dict[int, Type[MessageBase]] = {}
         self._max_tries = 5
+        self.fast_rate_rounds    = 0
+        self.medium_rate_rounds  = 0
+
+        if self._outlet.rtt > Channel.RTT_SLOW:
+            self.window              = 1
+            self.window_max          = 1
+            self.window_min          = 1
+            self.window_flexibility  = 1
+        else:
+            self.window              = Channel.WINDOW
+            self.window_max          = Channel.WINDOW_MAX_SLOW
+            self.window_min          = Channel.WINDOW_MIN
+            self.window_flexibility  = Channel.WINDOW_FLEXIBILITY
 
     def __enter__(self) -> Channel:
         return self
 
     def __exit__(self, __exc_type: Type[BaseException] | None, __exc_value: BaseException | None,
                  __traceback: TracebackType | None) -> bool | None:
         self._shutdown()
@@ -321,109 +373,164 @@
             i = 0
             for existing in ring:
                 if existing.sequence > envelope.sequence \
                    and not existing.sequence // 2 > envelope.sequence:  # account for overflow
                     ring.insert(i, envelope)
                     return True
                 if existing.sequence == envelope.sequence:
-                    RNS.log(f"Envelope: Emplacement of duplicate envelope sequence.", RNS.LOG_EXTREME)
+                    RNS.log(f"Envelope: Emplacement of duplicate envelope with sequence "+str(envelope.sequence), RNS.LOG_EXTREME)
                     return False
                 i += 1
             envelope.tracked = True
             ring.append(envelope)
             return True
 
-    def _prune_rx_ring(self):
-        with self._lock:
-            # Implementation for fixed window = 1
-            stale = list(sorted(self._rx_ring, key=lambda env: env.sequence, reverse=True))[1:]
-            for env in stale:
-                env.tracked = False
-                self._rx_ring.remove(env)
-
     def _run_callbacks(self, message: MessageBase):
         with self._lock:
             cbs = self._message_callbacks.copy()
 
         for cb in cbs:
             try:
                 if cb(message):
                     return
-            except Exception as ex:
-                RNS.log(f"Channel: Error running message callback: {ex}", RNS.LOG_ERROR)
+            except Exception as e:
+                RNS.log("Channel "+str(self)+" experienced an error while running a message callback. The contained exception was: "+str(e), RNS.LOG_ERROR)
 
     def _receive(self, raw: bytes):
         try:
             envelope = Envelope(outlet=self._outlet, raw=raw)
             with self._lock:
                 message = envelope.unpack(self._message_factories)
-                prev_env = self._rx_ring[0] if len(self._rx_ring) > 0 else None
-                if prev_env and envelope.sequence != (prev_env.sequence + 1) % 0x10000:
-                    RNS.log("Channel: Out of order packet received", RNS.LOG_DEBUG)
-                    return
+
+                if envelope.sequence < self._next_rx_sequence:
+                    window_overflow = (self._next_rx_sequence+Channel.WINDOW_MAX) % Channel.SEQ_MODULUS
+                    if window_overflow < self._next_rx_sequence:
+                        if envelope.sequence > window_overflow:
+                            RNS.log("Invalid packet sequence ("+str(envelope.sequence)+") received on channel "+str(self), RNS.LOG_DEBUG)
+                            return
+                    else:
+                        if envelope.sequence < self._next_rx_sequence:
+                            RNS.log("Invalid packet sequence ("+str(envelope.sequence)+") received on channel "+str(self), RNS.LOG_DEBUG)
+                            return
+
                 is_new = self._emplace_envelope(envelope, self._rx_ring)
-                self._prune_rx_ring()
+
             if not is_new:
-                RNS.log("Channel: Duplicate message received", RNS.LOG_DEBUG)
+                RNS.log("Duplicate message received on channel "+str(self), RNS.LOG_EXTREME)
                 return
-            RNS.log(f"Message received: {message}", RNS.LOG_DEBUG)
-            threading.Thread(target=self._run_callbacks, name="Message Callback", args=[message], daemon=True).start()
-        except Exception as ex:
-            RNS.log(f"Channel: Error receiving data: {ex}")
+            else:            
+                with self._lock:
+                    contigous = []
+                    for e in self._rx_ring:
+                        if e.sequence == self._next_rx_sequence:
+                            contigous.append(e)
+                            self._next_rx_sequence = (self._next_rx_sequence + 1) % Channel.SEQ_MODULUS
+
+                    for e in contigous:
+                        m = e.unpack(self._message_factories)
+                        self._rx_ring.remove(e)
+                        threading.Thread(target=self._run_callbacks, name="Message Callback", args=[m], daemon=True).start()
+
+        except Exception as e:
+            RNS.log("An error ocurred while receiving data on "+str(self)+". The contained exception was: "+str(e), RNS.LOG_ERROR)
 
     def is_ready_to_send(self) -> bool:
         """
         Check if ``Channel`` is ready to send.
 
         :return: True if ready
         """
         if not self._outlet.is_usable:
-            RNS.log("Channel: Link is not usable.", RNS.LOG_EXTREME)
             return False
 
         with self._lock:
+            outstanding = 0
             for envelope in self._tx_ring:
-                if envelope.outlet == self._outlet and (not envelope.packet
-                                                        or self._outlet.get_packet_state(envelope.packet) == MessageState.MSGSTATE_SENT):
-                    # TODO: Check if this should be enabled with some kind of
-                    # rate limiting, since it currently floods log output when
-                    # messages are waiting.
-                    # RNS.log("Channel: Link has a pending message.", RNS.LOG_EXTREME)
-                    return False
+                if envelope.outlet == self._outlet: 
+                    if not envelope.packet or not self._outlet.get_packet_state(envelope.packet) == MessageState.MSGSTATE_DELIVERED:
+                        outstanding += 1
+
+            if outstanding >= self.window:
+                return False
+
         return True
 
     def _packet_tx_op(self, packet: TPacket, op: Callable[[TPacket], bool]):
         with self._lock:
             envelope = next(filter(lambda e: self._outlet.get_packet_id(e.packet) == self._outlet.get_packet_id(packet),
                                    self._tx_ring), None)
             if envelope and op(envelope):
                 envelope.tracked = False
                 if envelope in self._tx_ring:
                     self._tx_ring.remove(envelope)
+
+                    if self.window < self.window_max:
+                        self.window += 1
+                        if (self.window - self.window_min) > (self.window_flexibility-1):
+                            self.window_min += 1
+
+                        # TODO: Remove at some point
+                        RNS.log("Increased "+str(self)+" window to "+str(self.window), RNS.LOG_DEBUG)
+
+                    if self._outlet.rtt != 0:
+                        if self._outlet.rtt > Channel.RTT_FAST:
+                            self.fast_rate_rounds = 0
+
+                            if self._outlet.rtt > Channel.RTT_MEDIUM:
+                                self.medium_rate_rounds = 0
+
+                            else:
+                                self.medium_rate_rounds += 1
+                                if self.window_max < Channel.WINDOW_MAX_MEDIUM and self.medium_rate_rounds == Channel.FAST_RATE_THRESHOLD:
+                                    self.window_max = Channel.WINDOW_MAX_MEDIUM
+                                    # TODO: Remove at some point
+                                    RNS.log("Increased "+str(self)+" max window to "+str(self.window_max), RNS.LOG_EXTREME)
+                            
+                        else:
+                            self.fast_rate_rounds += 1
+                            if self.window_max < Channel.WINDOW_MAX_FAST and self.fast_rate_rounds == Channel.FAST_RATE_THRESHOLD:
+                                self.window_max = Channel.WINDOW_MAX_FAST                                
+                                # TODO: Remove at some point
+                                RNS.log("Increased "+str(self)+" max window to "+str(self.window_max), RNS.LOG_EXTREME)
+
+
+
                 else:
-                    RNS.log("Channel: Envelope not found in TX ring", RNS.LOG_DEBUG)
+                    RNS.log("Envelope not found in TX ring for "+str(self), RNS.LOG_DEBUG)
         if not envelope:
-            RNS.log("Channel: Spurious message received.", RNS.LOG_EXTREME)
+            RNS.log("Spurious message received on "+str(self), RNS.LOG_EXTREME)
 
     def _packet_delivered(self, packet: TPacket):
         self._packet_tx_op(packet, lambda env: True)
 
     def _get_packet_timeout_time(self, tries: int) -> float:
         return pow(2, tries - 1) * max(self._outlet.rtt, 0.01) * 5
 
     def _packet_timeout(self, packet: TPacket):
         def retry_envelope(envelope: Envelope) -> bool:
             if envelope.tries >= self._max_tries:
-                RNS.log("Channel: Retry count exceeded, tearing down Link.", RNS.LOG_ERROR)
+                RNS.log("Retry count exceeded on "+str(self)+", tearing down Link.", RNS.LOG_ERROR)
                 self._shutdown()  # start on separate thread?
                 self._outlet.timed_out()
                 return True
             envelope.tries += 1
             self._outlet.resend(envelope.packet)
+            self._outlet.set_packet_delivered_callback(envelope.packet, self._packet_delivered)
             self._outlet.set_packet_timeout_callback(envelope.packet, self._packet_timeout, self._get_packet_timeout_time(envelope.tries))
+
+            if self.window > self.window_min:
+                self.window -= 1
+                if self.window_max > self.window_min:
+                    self.window_max -= 1
+                    if (self.window_max - self.window) > (self.window_flexibility-1):
+                        self.window_max -= 1
+
+                # TODO: Remove at some point
+                RNS.log("Decreased "+str(self)+" window to "+str(self.window), RNS.LOG_EXTREME)
+
             return False
 
         if self._outlet.get_packet_state(packet) != MessageState.MSGSTATE_DELIVERED:
             self._packet_tx_op(packet, retry_envelope)
 
     def send(self, message: MessageBase) -> Envelope:
         """
@@ -433,26 +540,28 @@
         :param message: an instance of a ``MessageBase`` subclass
         """
         envelope: Envelope | None = None
         with self._lock:
             if not self.is_ready_to_send():
                 raise ChannelException(CEType.ME_LINK_NOT_READY, f"Link is not ready")
             envelope = Envelope(self._outlet, message=message, sequence=self._next_sequence)
-            self._next_sequence = (self._next_sequence + 1) % 0x10000
+            self._next_sequence = (self._next_sequence + 1) % Channel.SEQ_MODULUS
+
             self._emplace_envelope(envelope, self._tx_ring)
         if envelope is None:
             raise BlockingIOError()
 
         envelope.pack()
         if len(envelope.raw) > self._outlet.mdu:
             raise ChannelException(CEType.ME_TOO_BIG, f"Packed message too big for packet: {len(envelope.raw)} > {self._outlet.mdu}")
         envelope.packet = self._outlet.send(envelope.raw)
         envelope.tries += 1
         self._outlet.set_packet_delivered_callback(envelope.packet, self._packet_delivered)
         self._outlet.set_packet_timeout_callback(envelope.packet, self._packet_timeout, self._get_packet_timeout_time(envelope.tries))
+
         return envelope
 
     @property
     def MDU(self):
         """
         Maximum Data Unit: the number of bytes available
         for a message to consume in a single send. This
@@ -479,15 +588,16 @@
         packet = RNS.Packet(self.link, raw, context=RNS.Packet.CHANNEL)
         if self.link.status == RNS.Link.ACTIVE:
             packet.send()
         return packet
 
     def resend(self, packet: RNS.Packet) -> RNS.Packet:
         RNS.log("Resending packet " + RNS.prettyhexrep(packet.packet_hash), RNS.LOG_DEBUG)
-        if not packet.resend():
+        receipt = packet.resend()
+        if not receipt:
             RNS.log("Failed to resend packet", RNS.LOG_ERROR)
         return packet
 
     @property
     def mdu(self):
         return self.link.MDU
 
@@ -534,8 +644,11 @@
         def inner(receipt: RNS.PacketReceipt):
             callback(packet)
 
         if packet and packet.receipt:
             packet.receipt.set_delivery_callback(inner if callback else None)
 
     def get_packet_id(self, packet: RNS.Packet) -> any:
-        return packet.get_hash()
+        if packet and hasattr(packet, "get_hash") and callable(packet.get_hash):
+            return packet.get_hash()
+        else:
+            return None
```

### Comparing `rns-0.5.1/RNS/Cryptography/AES.py` & `rns-0.5.2/RNS/Cryptography/AES.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/Ed25519.py` & `rns-0.5.2/RNS/Cryptography/Ed25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/Fernet.py` & `rns-0.5.2/RNS/Cryptography/Fernet.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/HKDF.py` & `rns-0.5.2/RNS/Cryptography/HKDF.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/HMAC.py` & `rns-0.5.2/RNS/Cryptography/HMAC.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/Hashes.py` & `rns-0.5.2/RNS/Cryptography/Hashes.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/PKCS7.py` & `rns-0.5.2/RNS/Cryptography/PKCS7.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/Provider.py` & `rns-0.5.2/RNS/Cryptography/Provider.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/Proxies.py` & `rns-0.5.2/RNS/Cryptography/Proxies.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/SHA256.py` & `rns-0.5.2/RNS/Cryptography/SHA256.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/SHA512.py` & `rns-0.5.2/RNS/Cryptography/SHA512.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/X25519.py` & `rns-0.5.2/RNS/Cryptography/X25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/__init__.py` & `rns-0.5.2/RNS/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/aes/aes.py` & `rns-0.5.2/RNS/Cryptography/aes/aes.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/aes/utils.py` & `rns-0.5.2/RNS/Cryptography/aes/utils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/pure25519/_ed25519.py` & `rns-0.5.2/RNS/Cryptography/pure25519/_ed25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/pure25519/basic.py` & `rns-0.5.2/RNS/Cryptography/pure25519/basic.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/pure25519/ed25519_oop.py` & `rns-0.5.2/RNS/Cryptography/pure25519/ed25519_oop.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Cryptography/pure25519/eddsa.py` & `rns-0.5.2/RNS/Cryptography/pure25519/eddsa.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Destination.py` & `rns-0.5.2/RNS/Destination.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Identity.py` & `rns-0.5.2/RNS/Identity.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/AX25KISSInterface.py` & `rns-0.5.2/RNS/Interfaces/AX25KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/Android/KISSInterface.py` & `rns-0.5.2/RNS/Interfaces/Android/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/Android/RNodeInterface.py` & `rns-0.5.2/RNS/Interfaces/Android/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/Android/SerialInterface.py` & `rns-0.5.2/RNS/Interfaces/Android/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/Android/__init__.py` & `rns-0.5.2/RNS/Interfaces/Android/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/AutoInterface.py` & `rns-0.5.2/RNS/Interfaces/AutoInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .Interface import Interface
+from collections import deque
 import socketserver
 import threading
 import re
 import socket
 import struct
 import time
 import sys
@@ -46,14 +47,16 @@
 
     ALL_IGNORE_IFS     = ["lo0"]
     DARWIN_IGNORE_IFS  = ["awdl0", "llw0", "lo0", "en5"]
     ANDROID_IGNORE_IFS = ["dummy0", "lo", "tun0"]
 
     BITRATE_GUESS      = 10*1000*1000
 
+    MULTI_IF_DEQUE_LEN = 64
+
     def handler_factory(self, callback):
         def create_handler(*args, **keys):
             return AutoInterfaceHandler(callback, *args, **keys)
         return create_handler
 
     def descope_linklocal(self, link_local_addr):
         # Drop scope specifier expressd as %ifname (macOS)
@@ -85,14 +88,15 @@
         self.online = False
         self.peers = {}
         self.link_local_addresses = []
         self.adopted_interfaces = {}
         self.interface_servers = {}
         self.multicast_echoes = {}
         self.timed_out_interfaces = {}
+        self.mif_deque = deque(maxlen=AutoInterface.MULTI_IF_DEQUE_LEN)
         self.carrier_changed = False
 
         self.outbound_udp_socket = None
 
         self.announce_rate_target = None
         self.announce_interval = AutoInterface.PEERING_TIMEOUT/6.0
         self.peer_job_interval = AutoInterface.PEERING_TIMEOUT*1.1
@@ -387,16 +391,19 @@
             else:
                 self.refresh_peer(addr)
 
     def refresh_peer(self, addr):
         self.peers[addr][1] = time.time()
 
     def processIncoming(self, data):
-        self.rxb += len(data)
-        self.owner.inbound(data, self)
+        data_hash = RNS.Identity.full_hash(data)
+        if not data_hash in self.mif_deque:
+            self.mif_deque.append(data_hash)
+            self.rxb += len(data)
+            self.owner.inbound(data, self)
 
     def processOutgoing(self,data):
             for peer in self.peers:
                 try:
                     if self.outbound_udp_socket == None:
                         self.outbound_udp_socket = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM)
```

### Comparing `rns-0.5.1/RNS/Interfaces/I2PInterface.py` & `rns-0.5.2/RNS/Interfaces/I2PInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/Interface.py` & `rns-0.5.2/RNS/Interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/KISSInterface.py` & `rns-0.5.2/RNS/Interfaces/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/LocalInterface.py` & `rns-0.5.2/RNS/Interfaces/LocalInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/PipeInterface.py` & `rns-0.5.2/RNS/Interfaces/PipeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/RNodeInterface.py` & `rns-0.5.2/RNS/Interfaces/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/SerialInterface.py` & `rns-0.5.2/RNS/Interfaces/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/TCPInterface.py` & `rns-0.5.2/RNS/Interfaces/TCPInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/UDPInterface.py` & `rns-0.5.2/RNS/Interfaces/UDPInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Interfaces/__init__.py` & `rns-0.5.2/RNS/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Link.py` & `rns-0.5.2/RNS/Link.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         self.callbacks = LinkCallbacks()
         self.resource_strategy = Link.ACCEPT_NONE
         self.outgoing_resources = []
         self.incoming_resources = []
         self.pending_requests   = []
         self.last_inbound = 0
         self.last_outbound = 0
+        self.last_proof = 0
         self.tx = 0
         self.rx = 0
         self.txbytes = 0
         self.rxbytes = 0
         self.traffic_timeout_factor = Link.TRAFFIC_TIMEOUT_FACTOR
         self.keepalive_timeout_factor = Link.KEEPALIVE_TIMEOUT_FACTOR
         self.keepalive = Link.KEEPALIVE
@@ -273,14 +274,15 @@
                 
                 if self.destination.identity.validate(signature, signed_data):
                     self.rtt = time.time() - self.request_time
                     self.attached_interface = packet.receiving_interface
                     self.__remote_identity = self.destination.identity
                     self.status = Link.ACTIVE
                     self.activated_at = time.time()
+                    self.last_proof = self.activated_at
                     RNS.Transport.activate_link(self)
                     RNS.log("Link "+str(self)+" established with "+str(self.destination)+", RTT is "+str(round(self.rtt, 3))+"s", RNS.LOG_VERBOSE)
                     
                     if self.rtt != None and self.establishment_cost != None and self.rtt > 0 and self.establishment_cost > 0:
                         self.establishment_rate = self.establishment_cost/self.rtt
 
                     rtt_data = umsgpack.packb(self.rtt)
@@ -523,15 +525,15 @@
                         self.status = Link.CLOSED
                         self.teardown_reason = Link.TIMEOUT
                         self.link_closed()
                         sleep_time = 0.001
 
                 elif self.status == Link.ACTIVE:
                     activated_at = self.activated_at if self.activated_at != None else 0
-                    last_inbound = max(self.last_inbound, activated_at)
+                    last_inbound = max(max(self.last_inbound, self.last_proof), activated_at)
 
                     if time.time() >= last_inbound + self.keepalive:
                         if self.initiator:
                             self.send_keepalive()
 
                         if time.time() >= last_inbound + self.stale_time:
                             sleep_time = self.rtt * self.keepalive_timeout_factor + Link.STALE_GRACE
@@ -805,14 +807,27 @@
                         for resource in self.incoming_resources:
                             resource.receive_part(packet)
 
                     elif packet.context == RNS.Packet.CHANNEL:
                         if not self._channel:
                             RNS.log(f"Channel data received without open channel", RNS.LOG_DEBUG)
                         else:
+                            # TODO: Remove packet loss simulator ######
+                            # if not hasattr(self, "drop_counter"):
+                            #     self.drop_counter = 0
+                            # self.drop_counter += 1
+
+                            # if self.drop_counter%6 == 0:
+                            #     RNS.log("Dropping channel packet for testing", RNS.LOG_DEBUG)
+                            # else:
+                            #     packet.prove()
+                            #     plaintext = self.decrypt(packet.data)
+                            #     self._channel._receive(plaintext)
+                            ############################################
+
                             packet.prove()
                             plaintext = self.decrypt(packet.data)
                             self._channel._receive(plaintext)
 
                 elif packet.packet_type == RNS.Packet.PROOF:
                     if packet.context == RNS.Packet.RESOURCE_PRF:
                         resource_hash = packet.data[0:RNS.Identity.HASHLENGTH//8]
```

### Comparing `rns-0.5.1/RNS/Packet.py` & `rns-0.5.2/RNS/Packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,16 @@
                 elif self.packet_type == Packet.PROOF and self.context == Packet.RESOURCE_PRF:
                     # Resource proofs are not encrypted
                     self.ciphertext = self.data
                 elif self.packet_type == Packet.PROOF and self.destination.type == RNS.Destination.LINK:
                     # Packet proofs over links are not encrypted
                     self.ciphertext = self.data
                 elif self.context == Packet.RESOURCE:
-                    # A resource takes care of symmetric
-                    # encryption by itself
+                    # A resource takes care of encryption
+                    # by itself
                     self.ciphertext = self.data
                 elif self.context == Packet.KEEPALIVE:
                     # Keepalive packets contain no actual
                     # data
                     self.ciphertext = self.data
                 elif self.context == Packet.CACHE_REQUEST:
                     # Cache-requests are not encrypted
@@ -272,14 +272,18 @@
     def resend(self):
         """
         Re-sends the packet.
         
         :returns: A :ref:`RNS.PacketReceipt<api-packetreceipt>` instance if *create_receipt* was set to *True* when the packet was instantiated, if not returns *None*. If the packet could not be sent *False* is returned.
         """
         if self.sent:
+            # Re-pack the packet to obtain new ciphertext for
+            # encrypted destinations
+            self.pack()
+            
             if RNS.Transport.outbound(self):
                 return self.receipt
             else:
                 RNS.log("No interfaces could process the outbound packet", RNS.LOG_ERROR)
                 self.sent = False
                 self.receipt = None
                 return False
@@ -392,17 +396,23 @@
             if proof_hash == self.hash:
                 proof_valid = link.validate(signature, self.hash)
                 if proof_valid:
                     self.status = PacketReceipt.DELIVERED
                     self.proved = True
                     self.concluded_at = time.time()
                     self.proof_packet = proof_packet
+                    link.last_proof = self.concluded_at
 
                     if self.callbacks.delivery != None:
-                        self.callbacks.delivery(self)
+                        try:
+                            self.callbacks.delivery(self)
+                        except Exception as e:
+                            RNS.log("An error occurred while evaluating external delivery callback for "+str(link), RNS.LOG_ERROR)
+                            RNS.log("The contained exception was: "+str(e), RNS.LOG_ERROR)
+                            
                     return True
                 else:
                     return False
             else:
                 return False
         elif len(proof) == PacketReceipt.IMPL_LENGTH:
             pass
```

### Comparing `rns-0.5.1/RNS/Resource.py` & `rns-0.5.2/RNS/Resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             resource.compressed          = True if resource.flags >> 1 & 0x01 else False
             resource.initiator           = False
             resource.callback             = callback
             resource.__progress_callback = progress_callback
             resource.total_parts         = int(math.ceil(resource.size/float(Resource.SDU)))
             resource.received_count      = 0
             resource.outstanding_parts   = 0
-            resource.parts                 = [None] * resource.total_parts
+            resource.parts               = [None] * resource.total_parts
             resource.window              = Resource.WINDOW
             resource.window_max          = Resource.WINDOW_MAX_SLOW
             resource.window_min          = Resource.WINDOW_MIN
             resource.window_flexibility  = Resource.WINDOW_FLEXIBILITY
             resource.last_activity       = time.time()
 
             resource.storagepath         = RNS.Reticulum.resourcepath+"/"+resource.original_hash.hex()
```

### Comparing `rns-0.5.1/RNS/Reticulum.py` & `rns-0.5.2/RNS/Reticulum.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Transport.py` & `rns-0.5.2/RNS/Transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1580,15 +1580,15 @@
                     else:
                         proof_hash = None
 
                     # Check if this proof neds to be transported
                     if (RNS.Reticulum.transport_enabled() or from_local_client or proof_for_local_client) and packet.destination_hash in Transport.reverse_table:
                         reverse_entry = Transport.reverse_table.pop(packet.destination_hash)
                         if packet.receiving_interface == reverse_entry[1]:
-                            RNS.log("Proof received on correct interface, transporting it via "+str(reverse_entry[0]), RNS.LOG_DEBUG)
+                            RNS.log("Proof received on correct interface, transporting it via "+str(reverse_entry[0]), RNS.LOG_EXTREME)
                             new_raw = packet.raw[0:1]
                             new_raw += struct.pack("!B", packet.hops)
                             new_raw += packet.raw[2:]
                             Transport.transmit(reverse_entry[0], new_raw)
                         else:
                             RNS.log("Proof received on wrong interface, not transporting it.", RNS.LOG_DEBUG)
```

### Comparing `rns-0.5.1/RNS/Utilities/__init__.py` & `rns-0.5.2/RNS/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Utilities/rncp.py` & `rns-0.5.2/RNS/Utilities/rncp.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Utilities/rnid.py` & `rns-0.5.2/RNS/Utilities/rnid.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         parser.add_argument("-R", "--request", action="store_true", default=False, help="request unknown Identities from the network")
         parser.add_argument("-t", action="store", metavar="seconds", type=float, help="identity request timeout before giving up", default=RNS.Transport.PATH_REQUEST_TIMEOUT)
         parser.add_argument("-p", "--print-identity", action="store_true", default=False, help="print identity info and exit")
         parser.add_argument("-P", "--print-private", action="store_true", default=False, help="allow displaying private keys")
 
         parser.add_argument("-b", "--base64", action="store_true", default=False, help=argparse.SUPPRESS) # help="Use base64-encoded input and output")
 
-        parser.add_argument("--version", action="version", version="rncp {version}".format(version=__version__))
+        parser.add_argument("--version", action="version", version="rnid {version}".format(version=__version__))
         
         args = parser.parse_args()
 
         ops = 0;
         for t in [args.encrypt, args.decrypt, args.validate, args.sign]:
             if t:
                 ops += 1
```

### Comparing `rns-0.5.1/RNS/Utilities/rnodeconf.py` & `rns-0.5.2/RNS/Utilities/rnodeconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,23 +232,26 @@
 
 try:
     CNF_DIR = os.path.expanduser("~/.config/rnodeconf")
     UPD_DIR = CNF_DIR+"/update"
     FWD_DIR = CNF_DIR+"/firmware"
     EXT_DIR = CNF_DIR+"/extracted"
     RT_PATH = CNF_DIR+"/recovery_esptool.py"
+    TK_DIR  = CNF_DIR+"/trusted_keys"
 
     if not os.path.isdir(CNF_DIR):
         os.makedirs(CNF_DIR)
     if not os.path.isdir(UPD_DIR):
         os.makedirs(UPD_DIR)
     if not os.path.isdir(FWD_DIR):
         os.makedirs(FWD_DIR)
     if not os.path.isdir(EXT_DIR):
         os.makedirs(EXT_DIR)
+    if not os.path.isdir(TK_DIR):
+        os.makedirs(TK_DIR)
 
 except Exception as e:
     print("No access to directory "+str(CNF_DIR)+". This utility needs file system access to store firmware and data files. Cannot continue.")
     print("The contained exception was:")
     print(str(e))
     exit(99)
 
@@ -813,14 +816,43 @@
                                 local_key_entry = ["LOCAL", public_bytes_hex]
                                 known_keys.append(local_key_entry)
 
                         except Exception as e:
                             RNS.log("Could not deserialize local signing key")
                             RNS.log(str(e))
 
+                    # Try loading trusted signing key for 
+                    # validation of devices
+                    if os.path.isdir(TK_DIR):
+                        for f in os.listdir(TK_DIR):
+                            if os.path.isfile(TK_DIR+"/"+f) and f.endswith(".pubkey"):
+                                try:
+                                    file = open(TK_DIR+"/"+f, "rb")
+                                    public_bytes = file.read()
+                                    file.close()
+
+                                    try:
+                                        public_bytes_hex = RNS.hexrep(public_bytes, delimit=False)
+
+                                        vendor_keys = []
+                                        for known in known_keys:
+                                            vendor_keys.append(known[1])
+
+                                        if not public_bytes_hex in vendor_keys:
+                                            local_key_entry = ["LOCAL", public_bytes_hex]
+                                            known_keys.append(local_key_entry)
+
+                                    except Exception as e:
+                                        RNS.log("Could not deserialize trusted signing key "+str(f))
+                                        RNS.log(str(e))
+
+                                except Exception as e:
+                                    RNS.log("Could not load trusted signing key"+str(f))
+
+
                     for known in known_keys:
                         vendor = known[0]
                         public_hexrep = known[1]
                         public_bytes = bytes.fromhex(public_hexrep)
                         public_key = load_der_public_key(public_bytes, backend=default_backend())
                         try:
                             public_key.verify(
@@ -1115,20 +1147,22 @@
         parser.add_argument("--sf", action="store", metavar="factor", type=int, default=None, help="Spreading factor for TNC mode (7 - 12)")
         parser.add_argument("--cr", action="store", metavar="rate", type=int, default=None, help="Coding rate for TNC mode (5 - 8)")
 
         parser.add_argument("--eeprom-backup", action="store_true", help="Backup EEPROM to file")
         parser.add_argument("--eeprom-dump", action="store_true", help="Dump EEPROM to console")
         parser.add_argument("--eeprom-wipe", action="store_true", help="Unlock and wipe EEPROM")
 
+        parser.add_argument("-P", "--public", action="store_true", help="Display public part of signing key")
+        parser.add_argument("--trust-key", action="store", metavar="hexbytes", type=str, default=None, help="Public key to trust for device verification")
+
         parser.add_argument("--version", action="store_true", help="Print program version and exit")
 
         parser.add_argument("-f", "--flash", action="store_true", help=argparse.SUPPRESS) # Flash firmware and bootstrap EEPROM
         parser.add_argument("-r", "--rom", action="store_true", help=argparse.SUPPRESS) # Bootstrap EEPROM without flashing firmware
         parser.add_argument("-k", "--key", action="store_true", help=argparse.SUPPRESS) # Generate a new signing key and exit
-        parser.add_argument("-P", "--public", action="store_true", help=argparse.SUPPRESS) # Display public part of signing key
         parser.add_argument("-S", "--sign", action="store_true", help=argparse.SUPPRESS) # Display public part of signing key
         parser.add_argument("-H", "--firmware-hash", action="store", help=argparse.SUPPRESS) # Display public part of signing key
         parser.add_argument("--platform", action="store", metavar="platform", type=str, default=None, help=argparse.SUPPRESS) # Platform specification for device bootstrap
         parser.add_argument("--product", action="store", metavar="product", type=str, default=None, help=argparse.SUPPRESS) # Product specification for device bootstrap
         parser.add_argument("--model", action="store", metavar="model", type=str, default=None, help=argparse.SUPPRESS) # Model code for device bootstrap
         parser.add_argument("--hwrev", action="store", metavar="revision", type=int, default=None, help=argparse.SUPPRESS) # Hardware revision for device bootstrap
 
@@ -1165,25 +1199,44 @@
 
         if args.force_update:
             force_update = True
 
         if args.nocheck:
             upd_nocheck = True
             
-        if args.public or args.key or args.flash or args.rom or args.autoinstall:
+        if args.public or args.key or args.flash or args.rom or args.autoinstall or args.trust_key:
             from cryptography.hazmat.primitives import hashes
             from cryptography.hazmat.backends import default_backend
             from cryptography.hazmat.primitives import serialization
             from cryptography.hazmat.primitives.serialization import load_der_public_key
             from cryptography.hazmat.primitives.serialization import load_der_private_key
             from cryptography.hazmat.primitives.asymmetric import rsa
             from cryptography.hazmat.primitives.asymmetric import padding
 
         clear = lambda: os.system('clear')
 
+        if args.trust_key:
+            try:
+                public_bytes = bytes.fromhex(args.trust_key)
+                try:
+                    public_key = load_der_public_key(public_bytes, backend=default_backend())
+                    key_hash = hashlib.sha256(public_bytes).hexdigest()
+                    RNS.log("Trusting key: "+str(key_hash))
+                    f = open(TK_DIR+"/"+str(key_hash)+".pubkey", "wb")
+                    f.write(public_bytes)
+                    f.close()
+
+                except Exception as e:
+                    RNS.log("Could not create public key from supplied data. Check that the key format is valid.")
+                    RNS.log(str(e))
+
+            except Exception as e:
+                RNS.log("Invalid key data supplied")
+            exit(0)
+
         if args.use_extracted and ((args.update and args.port != None) or args.autoinstall):
             print("")
             print("You have specified that rnodeconf should use a firmware extracted")
             print("from another device. Please note that this *only* works if you are")
             print("targeting a device of the same type that the firmware came from!")
             print("")
             print("Flashing this firmware to a device it was not created for will most")
```

### Comparing `rns-0.5.1/RNS/Utilities/rnpath.py` & `rns-0.5.2/RNS/Utilities/rnpath.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Utilities/rnprobe.py` & `rns-0.5.2/RNS/Utilities/rnprobe.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Utilities/rnsd.py` & `rns-0.5.2/RNS/Utilities/rnsd.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Utilities/rnstatus.py` & `rns-0.5.2/RNS/Utilities/rnstatus.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/Utilities/rnx.py` & `rns-0.5.2/RNS/Utilities/rnx.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/__init__.py` & `rns-0.5.2/RNS/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/configobj.py` & `rns-0.5.2/RNS/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/i2plib/__init__.py` & `rns-0.5.2/RNS/vendor/i2plib/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/i2plib/aiosam.py` & `rns-0.5.2/RNS/vendor/i2plib/aiosam.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/i2plib/exceptions.py` & `rns-0.5.2/RNS/vendor/i2plib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/i2plib/sam.py` & `rns-0.5.2/RNS/vendor/i2plib/sam.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/i2plib/tunnel.py` & `rns-0.5.2/RNS/vendor/i2plib/tunnel.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/i2plib/utils.py` & `rns-0.5.2/RNS/vendor/i2plib/utils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/ifaddr/__init__.py` & `rns-0.5.2/RNS/vendor/ifaddr/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/ifaddr/_posix.py` & `rns-0.5.2/RNS/vendor/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/ifaddr/_shared.py` & `rns-0.5.2/RNS/vendor/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/ifaddr/_win32.py` & `rns-0.5.2/RNS/vendor/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/ifaddr/niwrapper.py` & `rns-0.5.2/RNS/vendor/ifaddr/niwrapper.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/platformutils.py` & `rns-0.5.2/RNS/vendor/platformutils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/six.py` & `rns-0.5.2/RNS/vendor/six.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/RNS/vendor/umsgpack.py` & `rns-0.5.2/RNS/vendor/umsgpack.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/rns.egg-info/PKG-INFO` & `rns-0.5.2/rns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rns
-Version: 0.5.1
+Version: 0.5.2
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rns-0.5.1/rns.egg-info/SOURCES.txt` & `rns-0.5.2/rns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rns-0.5.1/setup.py` & `rns-0.5.2/setup.py`

 * *Files identical despite different names*

