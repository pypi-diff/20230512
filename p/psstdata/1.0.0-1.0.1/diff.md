# Comparing `tmp/psstdata-1.0.0.tar.gz` & `tmp/psstdata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psstdata-1.0.0.tar", last modified: Thu Mar  3 08:50:15 2022, max compression
+gzip compressed data, was "psstdata-1.0.1.tar", last modified: Fri May 12 21:21:39 2023, max compression
```

## Comparing `psstdata-1.0.0.tar` & `psstdata-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.458731 psstdata-1.0.0/
--rw-r--r--   0 galer    (1959091754) 1971611142      325 2022-03-03 08:50:15.458266 psstdata-1.0.0/PKG-INFO
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.438862 psstdata-1.0.0/psstdata/
--rw-r--r--   0 galer    (1959091754) 1971611142      322 2022-03-03 00:59:16.000000 psstdata-1.0.0/psstdata/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1835 2022-03-03 05:30:51.000000 psstdata-1.0.0/psstdata/_system.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.439851 psstdata-1.0.0/psstdata/artificialdata/
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.429504 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.442620 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/
--rw-r--r--   0 galer    (1959091754) 1971611142    20787 2022-02-28 10:24:16.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/asr_test.tsv
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.443788 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/audio/
--rw-r--r--   0 galer    (1959091754) 1971611142    58720 2022-02-28 06:38:29.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/audio/empty.wav
--rw-r--r--   0 galer    (1959091754) 1971611142     6926 2022-02-28 10:24:16.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/correctness_test.tsv
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.448148 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/
--rw-r--r--   0 galer    (1959091754) 1971611142    72267 2022-02-28 10:24:16.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/asr_train.tsv
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.449203 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/audio/
--rw-r--r--   0 galer    (1959091754) 1971611142    58720 2022-02-28 06:38:29.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/audio/empty.wav
--rw-r--r--   0 galer    (1959091754) 1971611142    27733 2022-02-28 10:24:16.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/correctness_train.tsv
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.452391 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/
--rw-r--r--   0 galer    (1959091754) 1971611142     8580 2022-02-28 10:24:16.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/asr_valid.tsv
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.453225 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/audio/
--rw-r--r--   0 galer    (1959091754) 1971611142    58720 2022-02-28 06:38:29.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/audio/empty.wav
--rw-r--r--   0 galer    (1959091754) 1971611142     3076 2022-02-28 10:24:16.000000 psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/correctness_valid.tsv
--rw-r--r--   0 galer    (1959091754) 1971611142      495 2022-02-28 10:21:48.000000 psstdata-1.0.0/psstdata/artificialdata/versions.json
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.456774 psstdata-1.0.0/psstdata/assets/
--rw-r--r--   0 galer    (1959091754) 1971611142       93 2022-02-25 03:04:17.000000 psstdata-1.0.0/psstdata/assets/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     9403 2022-03-03 00:57:56.000000 psstdata-1.0.0/psstdata/assets/correctness.json
--rw-r--r--   0 galer    (1959091754) 1971611142      604 2022-02-28 03:59:37.000000 psstdata-1.0.0/psstdata/assets/vocab_arpabet.json
--rw-r--r--   0 galer    (1959091754) 1971611142     1354 2022-03-01 04:46:08.000000 psstdata-1.0.0/psstdata/config.py
--rw-r--r--   0 galer    (1959091754) 1971611142       23 2022-03-02 11:33:52.000000 psstdata-1.0.0/psstdata/consts.py
--rw-r--r--   0 galer    (1959091754) 1971611142     6061 2022-03-03 08:45:18.000000 psstdata-1.0.0/psstdata/datastructures.py
--rw-r--r--   0 galer    (1959091754) 1971611142     3958 2022-03-02 23:54:26.000000 psstdata-1.0.0/psstdata/downloading.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1838 2022-03-02 13:25:22.000000 psstdata-1.0.0/psstdata/loading.py
--rw-r--r--   0 galer    (1959091754) 1971611142      241 2022-02-28 09:54:39.000000 psstdata-1.0.0/psstdata/logs.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1456 2022-03-01 05:16:38.000000 psstdata-1.0.0/psstdata/networking.py
--rw-r--r--   0 galer    (1959091754) 1971611142      851 2022-03-03 00:58:54.000000 psstdata-1.0.0/psstdata/tasks.py
--rw-r--r--   0 galer    (1959091754) 1971611142     3138 2022-03-03 03:58:28.000000 psstdata-1.0.0/psstdata/versioning.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2022-03-03 08:50:15.457701 psstdata-1.0.0/psstdata.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      983 2022-03-03 08:50:15.000000 psstdata-1.0.0/psstdata.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2022-03-03 08:50:15.458895 psstdata-1.0.0/setup.cfg
--rw-r--r--   0 galer    (1959091754) 1971611142      552 2022-03-03 00:13:01.000000 psstdata-1.0.0/setup.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.145420 psstdata-1.0.1/
+-rw-r--r--   0 galer    (1959091754) 1971611142      314 2023-05-12 21:21:39.145173 psstdata-1.0.1/PKG-INFO
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.137087 psstdata-1.0.1/psstdata/
+-rw-r--r--   0 galer    (1959091754) 1971611142      321 2023-05-12 03:10:18.000000 psstdata-1.0.1/psstdata/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142       33 2023-05-12 03:10:40.000000 psstdata-1.0.1/psstdata/__main__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     1835 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/_system.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.137628 psstdata-1.0.1/psstdata/artificialdata/
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.130040 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.139037 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/
+-rw-r--r--   0 galer    (1959091754) 1971611142    20537 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/asr_test.tsv
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.139460 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/audio/
+-rw-r--r--   0 galer    (1959091754) 1971611142    58720 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/audio/empty.wav
+-rw-r--r--   0 galer    (1959091754) 1971611142     6849 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/correctness_test.tsv
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.141237 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/
+-rw-r--r--   0 galer    (1959091754) 1971611142    71409 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/asr_train.tsv
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.141755 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/audio/
+-rw-r--r--   0 galer    (1959091754) 1971611142    58720 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/audio/empty.wav
+-rw-r--r--   0 galer    (1959091754) 1971611142    27426 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/correctness_train.tsv
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.142561 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/
+-rw-r--r--   0 galer    (1959091754) 1971611142     8478 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/asr_valid.tsv
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.143003 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/audio/
+-rw-r--r--   0 galer    (1959091754) 1971611142    58720 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/audio/empty.wav
+-rw-r--r--   0 galer    (1959091754) 1971611142     3042 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/correctness_valid.tsv
+-rw-r--r--   0 galer    (1959091754) 1971611142      495 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/artificialdata/versions.json
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.144357 psstdata-1.0.1/psstdata/assets/
+-rw-r--r--   0 galer    (1959091754) 1971611142       93 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/assets/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     9403 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/assets/correctness.json
+-rw-r--r--   0 galer    (1959091754) 1971611142      604 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/assets/vocab_arpabet.json
+-rw-r--r--   0 galer    (1959091754) 1971611142     1354 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/config.py
+-rw-r--r--   0 galer    (1959091754) 1971611142       23 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/consts.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     6061 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/datastructures.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     4968 2023-05-12 21:20:28.000000 psstdata-1.0.1/psstdata/downloading.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     1836 2023-05-12 03:08:29.000000 psstdata-1.0.1/psstdata/loading.py
+-rw-r--r--   0 galer    (1959091754) 1971611142      241 2023-05-12 02:41:37.000000 psstdata-1.0.1/psstdata/logs.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     1456 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/networking.py
+-rw-r--r--   0 galer    (1959091754) 1971611142      851 2022-05-19 00:32:37.000000 psstdata-1.0.1/psstdata/tasks.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     3213 2023-05-12 02:00:48.000000 psstdata-1.0.1/psstdata/versioning.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-12 21:21:39.144810 psstdata-1.0.1/psstdata.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142     1004 2023-05-12 21:21:39.000000 psstdata-1.0.1/psstdata.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-12 21:21:39.145486 psstdata-1.0.1/setup.cfg
+-rw-r--r--   0 galer    (1959091754) 1971611142      552 2023-05-12 21:12:02.000000 psstdata-1.0.1/setup.py
```

### Comparing `psstdata-1.0.0/psstdata/_system.py` & `psstdata-1.0.1/psstdata/_system.py`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/asr_test.tsv` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/correctness_train.tsv`

 * *Files 27% similar despite different names*

```diff
@@ -1,250 +1,307 @@
-id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
-MF01a-BNT02-comb	MF01a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF01a-BNT04-octopus	MF01a	octopus	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-MF01a-BNT07-canoe	MF01a	canoe	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-MF01a-BNT11-stethoscope	MF01a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF01a-BNT12-unicorn	MF01a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF01a-VNT01-01	MF01a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT02-02	MF01a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT03-03	MF01a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT04-04	MF01a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT05-05	MF01a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT06-06	MF01a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT07-07	MF01a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT08-08	MF01a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT09-09	MF01a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT10-10	MF01a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT11-11	MF01a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT12-12	MF01a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT15-15	MF01a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT16-16	MF01a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT18-18	MF01a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT19-19	MF01a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT20-20	MF01a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT21-21	MF01a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF01a-VNT22-22	MF01a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-BNT01-house	MF28a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF28a-BNT02-comb	MF28a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF28a-BNT03-toothbrush	MF28a	toothbrush	haʊ's	HH AW S	MO	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT05-bench	MF28a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF28a-BNT06-volcano	MF28a	volcano	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT07-canoe	MF28a	canoe	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT08-beaver	MF28a	beaver	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT10-hammock	MF28a	hammock	haʊ's	HH AW S	O	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT11-stethoscope	MF28a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT12-unicorn	MF28a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT14-sphinx	MF28a	sphinx	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-VNT01-01	MF28a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT02-02	MF28a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT03-03	MF28a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT04-04	MF28a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT05-05	MF28a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT06-06	MF28a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT07-07	MF28a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT08-08	MF28a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT09-09	MF28a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT11-11	MF28a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT12-12	MF28a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT13-13	MF28a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT14-14	MF28a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT16-16	MF28a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT18-18	MF28a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT19-19	MF28a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT20-20	MF28a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-MF28a-VNT22-22	MF28a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-BNT02-comb	SDB14a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-SDB14a-BNT05-bench	SDB14a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-SDB14a-BNT14-sphinx	SDB14a	sphinx	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-SDB14a-BNT15-palette	SDB14a	palette	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT03-03	SDB14a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT04-04	SDB14a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT05-05	SDB14a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT06-06	SDB14a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT07-07	SDB14a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT08-08	SDB14a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT09-09	SDB14a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT10-10	SDB14a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT11-11	SDB14a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT12-12	SDB14a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT13-13	SDB14a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT14-14	SDB14a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT15-15	SDB14a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT16-16	SDB14a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT18-18	SDB14a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT19-19	SDB14a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT20-20	SDB14a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-SDB14a-VNT21-21	SDB14a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-BNT01-house	GF10a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF10a-BNT05-bench	GF10a	bench	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-GF10a-BNT11-stethoscope	GF10a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-GF10a-VNT01-01	GF10a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT02-02	GF10a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT03-03	GF10a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT04-04	GF10a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT05-05	GF10a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT06-06	GF10a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT07-07	GF10a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT08-08	GF10a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT09-09	GF10a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT10-10	GF10a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT11-11	GF10a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT12-12	GF10a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT14-14	GF10a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT15-15	GF10a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT16-16	GF10a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT18-18	GF10a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT19-19	GF10a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT21-21	GF10a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF10a-VNT22-22	GF10a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-BNT01-house	GF17a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT02-comb	GF17a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT03-toothbrush	GF17a	toothbrush	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT05-bench	GF17a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT06-volcano	GF17a	volcano	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT07-canoe	GF17a	canoe	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT09-cactus	GF17a	cactus	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT10-hammock	GF17a	hammock	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT11-stethoscope	GF17a	stethoscope	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT12-unicorn	GF17a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT13-tripod	GF17a	tripod	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT15-palette	GF17a	palette	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-GF17a-VNT01-01	GF17a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT02-02	GF17a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT04-04	GF17a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT05-05	GF17a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT06-06	GF17a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT07-07	GF17a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT08-08	GF17a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT09-09	GF17a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT10-10	GF17a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT11-11	GF17a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT12-12	GF17a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT13-13	GF17a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT14-14	GF17a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT16-16	GF17a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT17-17	GF17a	17	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT18-18	GF17a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT19-19	GF17a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT20-20	GF17a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT21-21	GF17a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-GF17a-VNT22-22	GF17a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-BNT01-house	RCG02a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT02-comb	RCG02a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT03-toothbrush	RCG02a	toothbrush	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT04-octopus	RCG02a	octopus	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT05-bench	RCG02a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT06-volcano	RCG02a	volcano	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT07-canoe	RCG02a	canoe	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT08-beaver	RCG02a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT10-hammock	RCG02a	hammock	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT11-stethoscope	RCG02a	stethoscope	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT12-unicorn	RCG02a	unicorn	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT13-tripod	RCG02a	tripod	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT14-sphinx	RCG02a	sphinx	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG02a-BNT15-palette	RCG02a	palette	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-VNT01-01	RCG02a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT02-02	RCG02a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT03-03	RCG02a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT04-04	RCG02a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT05-05	RCG02a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT06-06	RCG02a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT07-07	RCG02a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT08-08	RCG02a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT09-09	RCG02a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT10-10	RCG02a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT11-11	RCG02a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT12-12	RCG02a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT13-13	RCG02a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT14-14	RCG02a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT15-15	RCG02a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT16-16	RCG02a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT17-17	RCG02a	17	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT19-19	RCG02a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT20-20	RCG02a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT21-21	RCG02a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG02a-VNT22-22	RCG02a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT01-house	RCG15a	house	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT02-comb	RCG15a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT03-toothbrush	RCG15a	toothbrush	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT04-octopus	RCG15a	octopus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT05-bench	RCG15a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT06-volcano	RCG15a	volcano	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT07-canoe	RCG15a	canoe	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT08-beaver	RCG15a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT09-cactus	RCG15a	cactus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT10-hammock	RCG15a	hammock	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT11-stethoscope	RCG15a	stethoscope	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT12-unicorn	RCG15a	unicorn	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT13-tripod	RCG15a	tripod	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT14-sphinx	RCG15a	sphinx	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT15-palette	RCG15a	palette	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT01-01	RCG15a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT02-02	RCG15a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT03-03	RCG15a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT04-04	RCG15a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT05-05	RCG15a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT06-06	RCG15a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT07-07	RCG15a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT08-08	RCG15a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT09-09	RCG15a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT10-10	RCG15a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT11-11	RCG15a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT12-12	RCG15a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT13-13	RCG15a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT14-14	RCG15a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT15-15	RCG15a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT16-16	RCG15a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT17-17	RCG15a	17	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT18-18	RCG15a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT19-19	RCG15a	19	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT20-20	RCG15a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT21-21	RCG15a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG15a-VNT22-22	RCG15a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT01-house	RCG19a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG19a-BNT02-comb	RCG19a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG19a-BNT03-toothbrush	RCG19a	toothbrush	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT04-octopus	RCG19a	octopus	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT05-bench	RCG19a	bench	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT06-volcano	RCG19a	volcano	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT08-beaver	RCG19a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG19a-BNT09-cactus	RCG19a	cactus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT12-unicorn	RCG19a	unicorn	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT01-01	RCG19a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT02-02	RCG19a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT03-03	RCG19a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT04-04	RCG19a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT05-05	RCG19a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT06-06	RCG19a	06	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT07-07	RCG19a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT08-08	RCG19a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT09-09	RCG19a	09	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT10-10	RCG19a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT11-11	RCG19a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT12-12	RCG19a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT13-13	RCG19a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT14-14	RCG19a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT15-15	RCG19a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT16-16	RCG19a	16	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT17-17	RCG19a	17	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT18-18	RCG19a	18	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT21-21	RCG19a	21	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG19a-VNT22-22	RCG19a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-BNT05-bench	RCG21a	bench	haʊ's	HH AW S	O	test/audio/empty.wav	28992	12.3	False
-RCG21a-BNT08-beaver	RCG21a	beaver	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-RCG21a-BNT09-cactus	RCG21a	cactus	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT01-01	RCG21a	01	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT02-02	RCG21a	02	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT03-03	RCG21a	03	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT04-04	RCG21a	04	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT05-05	RCG21a	05	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT07-07	RCG21a	07	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT08-08	RCG21a	08	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT10-10	RCG21a	10	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT11-11	RCG21a	11	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT12-12	RCG21a	12	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT13-13	RCG21a	13	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT14-14	RCG21a	14	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT15-15	RCG21a	15	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT17-17	RCG21a	17	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT20-20	RCG21a	20	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
-RCG21a-VNT22-22	RCG21a	22	haʊ's	HH AW S		test/audio/empty.wav	28992	12.3	False
+id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
+MF04a-BNT01-house	MF04a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF04a-BNT02-comb	MF04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF04a-BNT03-toothbrush	MF04a	toothbrush	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT04-octopus	MF04a	octopus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT05-bench	MF04a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF04a-BNT06-volcano	MF04a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT07-canoe	MF04a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT08-beaver	MF04a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT09-cactus	MF04a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT10-hammock	MF04a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT12-unicorn	MF04a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT13-tripod	MF04a	tripod	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT14-sphinx	MF04a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT01-house	MF06a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT02-comb	MF06a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT03-toothbrush	MF06a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT04-octopus	MF06a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT05-bench	MF06a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT06-volcano	MF06a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT07-canoe	MF06a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT08-beaver	MF06a	beaver	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT09-cactus	MF06a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT10-hammock	MF06a	hammock	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT11-stethoscope	MF06a	stethoscope	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT12-unicorn	MF06a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT13-tripod	MF06a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT14-sphinx	MF06a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT15-palette	MF06a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF08a-BNT01-house	MF08a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT02-comb	MF08a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT03-toothbrush	MF08a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT04-octopus	MF08a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT05-bench	MF08a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT06-volcano	MF08a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT07-canoe	MF08a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT09-cactus	MF08a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT11-stethoscope	MF08a	stethoscope	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT12-unicorn	MF08a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT13-tripod	MF08a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT14-sphinx	MF08a	sphinx	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT15-palette	MF08a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF13a-BNT01-house	MF13a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF13a-BNT02-comb	MF13a	comb	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT04-octopus	MF13a	octopus	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT07-canoe	MF13a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF13a-BNT09-cactus	MF13a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT12-unicorn	MF13a	unicorn	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT14-sphinx	MF13a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT02-comb	MF20a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT03-toothbrush	MF20a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT04-octopus	MF20a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT05-bench	MF20a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT06-volcano	MF20a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT07-canoe	MF20a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT08-beaver	MF20a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT09-cactus	MF20a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT10-hammock	MF20a	hammock	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT15-palette	MF20a	palette	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF23a-BNT02-comb	MF23a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT03-toothbrush	MF23a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT06-volcano	MF23a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF23a-BNT07-canoe	MF23a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT08-beaver	MF23a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT09-cactus	MF23a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF23a-BNT10-hammock	MF23a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT15-palette	MF23a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT03-toothbrush	MF24a	toothbrush	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT05-bench	MF24a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT06-volcano	MF24a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT07-canoe	MF24a	canoe	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT08-beaver	MF24a	beaver	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT09-cactus	MF24a	cactus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT11-stethoscope	MF24a	stethoscope	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT12-unicorn	MF24a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT13-tripod	MF24a	tripod	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT15-palette	MF24a	palette	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT01-house	MF30a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT02-comb	MF30a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT04-octopus	MF30a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT05-bench	MF30a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT06-volcano	MF30a	volcano	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT07-canoe	MF30a	canoe	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT08-beaver	MF30a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT13-tripod	MF30a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT15-palette	MF30a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT01-house	MF33a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT02-comb	MF33a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT03-toothbrush	MF33a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT04-octopus	MF33a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT05-bench	MF33a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT06-volcano	MF33a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT07-canoe	MF33a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT08-beaver	MF33a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT09-cactus	MF33a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT10-hammock	MF33a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT12-unicorn	MF33a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT13-tripod	MF33a	tripod	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT14-sphinx	MF33a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT15-palette	MF33a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF38a-BNT01-house	MF38a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF38a-BNT02-comb	MF38a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF38a-BNT03-toothbrush	MF38a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF38a-BNT13-tripod	MF38a	tripod	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT01-house	SDB04a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT02-comb	SDB04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT03-toothbrush	SDB04a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT04-octopus	SDB04a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT05-bench	SDB04a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT06-volcano	SDB04a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT07-canoe	SDB04a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT08-beaver	SDB04a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT09-cactus	SDB04a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT10-hammock	SDB04a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT11-stethoscope	SDB04a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT12-unicorn	SDB04a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT13-tripod	SDB04a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT14-sphinx	SDB04a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT15-palette	SDB04a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB06a-BNT03-toothbrush	SDB06a	toothbrush	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT01-house	SDB07a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT02-comb	SDB07a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT03-toothbrush	SDB07a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT05-bench	SDB07a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT06-volcano	SDB07a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT08-beaver	SDB07a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT09-cactus	SDB07a	cactus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT11-stethoscope	SDB07a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT14-sphinx	SDB07a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT01-house	SDB09a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB09a-BNT03-toothbrush	SDB09a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT05-bench	SDB09a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT07-canoe	SDB09a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT10-hammock	SDB09a	hammock	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT13-tripod	SDB09a	tripod	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT15-palette	SDB09a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT01-house	SDB12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT02-comb	SDB12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT04-octopus	SDB12a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT05-bench	SDB12a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT06-volcano	SDB12a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT07-canoe	SDB12a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT10-hammock	SDB12a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT11-stethoscope	SDB12a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT12-unicorn	SDB12a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT01-house	SDB13a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT02-comb	SDB13a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT03-toothbrush	SDB13a	toothbrush	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB13a-BNT05-bench	SDB13a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT09-cactus	SDB13a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB17a-BNT01-house	SDB17a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB17a-BNT03-toothbrush	SDB17a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+SDB17a-BNT06-volcano	SDB17a	volcano	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT01-house	SDB18a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT02-comb	SDB18a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT03-toothbrush	SDB18a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT04-octopus	SDB18a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT05-bench	SDB18a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT06-volcano	SDB18a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT07-canoe	SDB18a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT08-beaver	SDB18a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT10-hammock	SDB18a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT11-stethoscope	SDB18a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT12-unicorn	SDB18a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT13-tripod	SDB18a	tripod	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT14-sphinx	SDB18a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT15-palette	SDB18a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB19a-BNT01-house	SDB19a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT02-comb	SDB19a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT04-octopus	SDB19a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT07-canoe	SDB19a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT08-beaver	SDB19a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT09-cactus	SDB19a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT10-hammock	SDB19a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT11-stethoscope	SDB19a	stethoscope	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT14-sphinx	SDB19a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB19a-BNT15-palette	SDB19a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT01-house	GF01a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT02-comb	GF01a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT03-toothbrush	GF01a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT04-octopus	GF01a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT05-bench	GF01a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT06-volcano	GF01a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT07-canoe	GF01a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT08-beaver	GF01a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT09-cactus	GF01a	cactus	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT10-hammock	GF01a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT11-stethoscope	GF01a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT12-unicorn	GF01a	unicorn	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT14-sphinx	GF01a	sphinx	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT15-palette	GF01a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT01-house	GF02a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF02a-BNT02-comb	GF02a	comb	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT03-toothbrush	GF02a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT04-octopus	GF02a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT07-canoe	GF02a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF02a-BNT08-beaver	GF02a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT09-cactus	GF02a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT10-hammock	GF02a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT14-sphinx	GF02a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT01-house	GF07a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT02-comb	GF07a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT03-toothbrush	GF07a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT04-octopus	GF07a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT05-bench	GF07a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT06-volcano	GF07a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT07-canoe	GF07a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT11-stethoscope	GF07a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT12-unicorn	GF07a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT13-tripod	GF07a	tripod	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT14-sphinx	GF07a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT15-palette	GF07a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT01-house	GF09a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT02-comb	GF09a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT03-toothbrush	GF09a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT04-octopus	GF09a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT05-bench	GF09a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT06-volcano	GF09a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT07-canoe	GF09a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT08-beaver	GF09a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT09-cactus	GF09a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT10-hammock	GF09a	hammock	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT11-stethoscope	GF09a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT12-unicorn	GF09a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT13-tripod	GF09a	tripod	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT14-sphinx	GF09a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT15-palette	GF09a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT01-house	GF12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF12a-BNT02-comb	GF12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF12a-BNT03-toothbrush	GF12a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT05-bench	GF12a	bench	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT10-hammock	GF12a	hammock	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT12-unicorn	GF12a	unicorn	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT15-palette	GF12a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF14a-BNT01-house	GF14a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT02-comb	GF14a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT03-toothbrush	GF14a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT04-octopus	GF14a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT05-bench	GF14a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT06-volcano	GF14a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF14a-BNT07-canoe	GF14a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT08-beaver	GF14a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT09-cactus	GF14a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT10-hammock	GF14a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT12-unicorn	GF14a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT14-sphinx	GF14a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF14a-BNT15-palette	GF14a	palette	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT01-house	GF15a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT02-comb	GF15a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT03-toothbrush	GF15a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT04-octopus	GF15a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT05-bench	GF15a	bench	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT06-volcano	GF15a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT07-canoe	GF15a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT08-beaver	GF15a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT09-cactus	GF15a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT11-stethoscope	GF15a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT12-unicorn	GF15a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT14-sphinx	GF15a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT15-palette	GF15a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT01-house	RCG03a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT02-comb	RCG03a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT03-toothbrush	RCG03a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT04-octopus	RCG03a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT05-bench	RCG03a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT06-volcano	RCG03a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT07-canoe	RCG03a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT08-beaver	RCG03a	beaver	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT09-cactus	RCG03a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT10-hammock	RCG03a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT11-stethoscope	RCG03a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT12-unicorn	RCG03a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT14-sphinx	RCG03a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT15-palette	RCG03a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT01-house	RCG04a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT02-comb	RCG04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG04a-BNT03-toothbrush	RCG04a	toothbrush	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT04-octopus	RCG04a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT05-bench	RCG04a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT06-volcano	RCG04a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT08-beaver	RCG04a	beaver	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT10-hammock	RCG04a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT12-unicorn	RCG04a	unicorn	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT01-house	RCG12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT02-comb	RCG12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT03-toothbrush	RCG12a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT04-octopus	RCG12a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT05-bench	RCG12a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT06-volcano	RCG12a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT07-canoe	RCG12a	canoe	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT08-beaver	RCG12a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT09-cactus	RCG12a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT14-sphinx	RCG12a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT01-house	RCG14a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT02-comb	RCG14a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT03-toothbrush	RCG14a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT04-octopus	RCG14a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT05-bench	RCG14a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT06-volcano	RCG14a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT07-canoe	RCG14a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT08-beaver	RCG14a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT09-cactus	RCG14a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT10-hammock	RCG14a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT11-stethoscope	RCG14a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT12-unicorn	RCG14a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT14-sphinx	RCG14a	sphinx	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT15-palette	RCG14a	palette	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
```

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/audio/empty.wav` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/audio/empty.wav`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/test/correctness_test.tsv` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/test/correctness_test.tsv`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
-MF01a-BNT02-comb	MF01a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF01a-BNT04-octopus	MF01a	octopus	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-MF01a-BNT07-canoe	MF01a	canoe	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-MF01a-BNT11-stethoscope	MF01a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF01a-BNT12-unicorn	MF01a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT01-house	MF28a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF28a-BNT02-comb	MF28a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF28a-BNT03-toothbrush	MF28a	toothbrush	haʊ's	HH AW S	MO	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT05-bench	MF28a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-MF28a-BNT06-volcano	MF28a	volcano	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT07-canoe	MF28a	canoe	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT08-beaver	MF28a	beaver	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT10-hammock	MF28a	hammock	haʊ's	HH AW S	O	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT11-stethoscope	MF28a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT12-unicorn	MF28a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-MF28a-BNT14-sphinx	MF28a	sphinx	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-SDB14a-BNT02-comb	SDB14a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-SDB14a-BNT05-bench	SDB14a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-SDB14a-BNT14-sphinx	SDB14a	sphinx	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-SDB14a-BNT15-palette	SDB14a	palette	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-GF10a-BNT01-house	GF10a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF10a-BNT05-bench	GF10a	bench	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-GF10a-BNT11-stethoscope	GF10a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT01-house	GF17a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT02-comb	GF17a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT03-toothbrush	GF17a	toothbrush	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT05-bench	GF17a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT06-volcano	GF17a	volcano	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT07-canoe	GF17a	canoe	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT09-cactus	GF17a	cactus	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT10-hammock	GF17a	hammock	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT11-stethoscope	GF17a	stethoscope	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT12-unicorn	GF17a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-GF17a-BNT13-tripod	GF17a	tripod	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-GF17a-BNT15-palette	GF17a	palette	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
-RCG02a-BNT01-house	RCG02a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT02-comb	RCG02a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT03-toothbrush	RCG02a	toothbrush	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT04-octopus	RCG02a	octopus	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT05-bench	RCG02a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT06-volcano	RCG02a	volcano	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT07-canoe	RCG02a	canoe	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT08-beaver	RCG02a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT10-hammock	RCG02a	hammock	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT11-stethoscope	RCG02a	stethoscope	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT12-unicorn	RCG02a	unicorn	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT13-tripod	RCG02a	tripod	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG02a-BNT14-sphinx	RCG02a	sphinx	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG02a-BNT15-palette	RCG02a	palette	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT01-house	RCG15a	house	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT02-comb	RCG15a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT03-toothbrush	RCG15a	toothbrush	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT04-octopus	RCG15a	octopus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT05-bench	RCG15a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT06-volcano	RCG15a	volcano	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT07-canoe	RCG15a	canoe	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT08-beaver	RCG15a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT09-cactus	RCG15a	cactus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT10-hammock	RCG15a	hammock	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT11-stethoscope	RCG15a	stethoscope	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT12-unicorn	RCG15a	unicorn	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT13-tripod	RCG15a	tripod	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG15a-BNT14-sphinx	RCG15a	sphinx	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG15a-BNT15-palette	RCG15a	palette	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT01-house	RCG19a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG19a-BNT02-comb	RCG19a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG19a-BNT03-toothbrush	RCG19a	toothbrush	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT04-octopus	RCG19a	octopus	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT05-bench	RCG19a	bench	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT06-volcano	RCG19a	volcano	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT08-beaver	RCG19a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
-RCG19a-BNT09-cactus	RCG19a	cactus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
-RCG19a-BNT12-unicorn	RCG19a	unicorn	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
-RCG21a-BNT05-bench	RCG21a	bench	haʊ's	HH AW S	O	test/audio/empty.wav	28992	12.3	False
-RCG21a-BNT08-beaver	RCG21a	beaver	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
-RCG21a-BNT09-cactus	RCG21a	cactus	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
+id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
+MF01a-BNT02-comb	MF01a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+MF01a-BNT04-octopus	MF01a	octopus	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
+MF01a-BNT07-canoe	MF01a	canoe	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
+MF01a-BNT11-stethoscope	MF01a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+MF01a-BNT12-unicorn	MF01a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT01-house	MF28a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+MF28a-BNT02-comb	MF28a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+MF28a-BNT03-toothbrush	MF28a	toothbrush	haʊ's	HH AW S	MO	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT05-bench	MF28a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+MF28a-BNT06-volcano	MF28a	volcano	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT07-canoe	MF28a	canoe	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT08-beaver	MF28a	beaver	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT10-hammock	MF28a	hammock	haʊ's	HH AW S	O	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT11-stethoscope	MF28a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT12-unicorn	MF28a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+MF28a-BNT14-sphinx	MF28a	sphinx	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+SDB14a-BNT02-comb	SDB14a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+SDB14a-BNT05-bench	SDB14a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+SDB14a-BNT14-sphinx	SDB14a	sphinx	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
+SDB14a-BNT15-palette	SDB14a	palette	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+GF10a-BNT01-house	GF10a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF10a-BNT05-bench	GF10a	bench	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+GF10a-BNT11-stethoscope	GF10a	stethoscope	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+GF17a-BNT01-house	GF17a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT02-comb	GF17a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT03-toothbrush	GF17a	toothbrush	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT05-bench	GF17a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT06-volcano	GF17a	volcano	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT07-canoe	GF17a	canoe	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+GF17a-BNT09-cactus	GF17a	cactus	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT10-hammock	GF17a	hammock	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT11-stethoscope	GF17a	stethoscope	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+GF17a-BNT12-unicorn	GF17a	unicorn	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+GF17a-BNT13-tripod	GF17a	tripod	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+GF17a-BNT15-palette	GF17a	palette	haʊ's	HH AW S	M	test/audio/empty.wav	28992	12.3	False
+RCG02a-BNT01-house	RCG02a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT02-comb	RCG02a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT03-toothbrush	RCG02a	toothbrush	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT04-octopus	RCG02a	octopus	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT05-bench	RCG02a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT06-volcano	RCG02a	volcano	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT07-canoe	RCG02a	canoe	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT08-beaver	RCG02a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT10-hammock	RCG02a	hammock	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT11-stethoscope	RCG02a	stethoscope	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT12-unicorn	RCG02a	unicorn	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT13-tripod	RCG02a	tripod	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG02a-BNT14-sphinx	RCG02a	sphinx	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG02a-BNT15-palette	RCG02a	palette	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG15a-BNT01-house	RCG15a	house	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT02-comb	RCG15a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG15a-BNT03-toothbrush	RCG15a	toothbrush	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT04-octopus	RCG15a	octopus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT05-bench	RCG15a	bench	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG15a-BNT06-volcano	RCG15a	volcano	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT07-canoe	RCG15a	canoe	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG15a-BNT08-beaver	RCG15a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG15a-BNT09-cactus	RCG15a	cactus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT10-hammock	RCG15a	hammock	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT11-stethoscope	RCG15a	stethoscope	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT12-unicorn	RCG15a	unicorn	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT13-tripod	RCG15a	tripod	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG15a-BNT14-sphinx	RCG15a	sphinx	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG15a-BNT15-palette	RCG15a	palette	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
+RCG19a-BNT01-house	RCG19a	house	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG19a-BNT02-comb	RCG19a	comb	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG19a-BNT03-toothbrush	RCG19a	toothbrush	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG19a-BNT04-octopus	RCG19a	octopus	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+RCG19a-BNT05-bench	RCG19a	bench	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+RCG19a-BNT06-volcano	RCG19a	volcano	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG19a-BNT08-beaver	RCG19a	beaver	haʊ's	HH AW S	C	test/audio/empty.wav	28992	12.3	True
+RCG19a-BNT09-cactus	RCG19a	cactus	haʊ's	HH AW S	N	test/audio/empty.wav	28992	12.3	False
+RCG19a-BNT12-unicorn	RCG19a	unicorn	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
+RCG21a-BNT05-bench	RCG21a	bench	haʊ's	HH AW S	O	test/audio/empty.wav	28992	12.3	False
+RCG21a-BNT08-beaver	RCG21a	beaver	haʊ's	HH AW S	S	test/audio/empty.wav	28992	12.3	False
+RCG21a-BNT09-cactus	RCG21a	cactus	haʊ's	HH AW S	F	test/audio/empty.wav	28992	12.3	False
```

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/asr_train.tsv` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/asr_train.tsv`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,858 +1,858 @@
-id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
-MF04a-BNT01-house	MF04a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF04a-BNT02-comb	MF04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF04a-BNT03-toothbrush	MF04a	toothbrush	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT04-octopus	MF04a	octopus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT05-bench	MF04a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF04a-BNT06-volcano	MF04a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT07-canoe	MF04a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT08-beaver	MF04a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT09-cactus	MF04a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT10-hammock	MF04a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT12-unicorn	MF04a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT13-tripod	MF04a	tripod	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
-MF04a-BNT14-sphinx	MF04a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF04a-VNT01-01	MF04a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT02-02	MF04a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT03-03	MF04a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT04-04	MF04a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT05-05	MF04a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT06-06	MF04a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT07-07	MF04a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT08-08	MF04a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT09-09	MF04a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT10-10	MF04a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT11-11	MF04a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT12-12	MF04a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT13-13	MF04a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT14-14	MF04a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT15-15	MF04a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT16-16	MF04a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT17-17	MF04a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT18-18	MF04a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT19-19	MF04a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT20-20	MF04a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT21-21	MF04a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF04a-VNT22-22	MF04a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-BNT01-house	MF06a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT02-comb	MF06a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT03-toothbrush	MF06a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
-MF06a-BNT04-octopus	MF06a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT05-bench	MF06a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT06-volcano	MF06a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT07-canoe	MF06a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT08-beaver	MF06a	beaver	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-MF06a-BNT09-cactus	MF06a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT10-hammock	MF06a	hammock	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF06a-BNT11-stethoscope	MF06a	stethoscope	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF06a-BNT12-unicorn	MF06a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT13-tripod	MF06a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF06a-BNT14-sphinx	MF06a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF06a-BNT15-palette	MF06a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-MF06a-VNT02-02	MF06a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT03-03	MF06a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT04-04	MF06a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT05-05	MF06a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT06-06	MF06a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT07-07	MF06a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT08-08	MF06a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT09-09	MF06a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT10-10	MF06a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT11-11	MF06a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT12-12	MF06a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT13-13	MF06a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT14-14	MF06a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT15-15	MF06a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT16-16	MF06a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT17-17	MF06a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT18-18	MF06a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT19-19	MF06a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT20-20	MF06a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT21-21	MF06a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF06a-VNT22-22	MF06a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-BNT01-house	MF08a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT02-comb	MF08a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT03-toothbrush	MF08a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT04-octopus	MF08a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT05-bench	MF08a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT06-volcano	MF08a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT07-canoe	MF08a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT09-cactus	MF08a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT11-stethoscope	MF08a	stethoscope	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT12-unicorn	MF08a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT13-tripod	MF08a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT14-sphinx	MF08a	sphinx	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-BNT15-palette	MF08a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF08a-VNT02-02	MF08a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT03-03	MF08a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT04-04	MF08a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT05-05	MF08a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT06-06	MF08a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT07-07	MF08a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT08-08	MF08a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT09-09	MF08a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT10-10	MF08a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT11-11	MF08a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT12-12	MF08a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT13-13	MF08a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT14-14	MF08a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT15-15	MF08a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT16-16	MF08a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT17-17	MF08a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT18-18	MF08a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT19-19	MF08a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT21-21	MF08a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF08a-VNT22-22	MF08a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-BNT01-house	MF13a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF13a-BNT02-comb	MF13a	comb	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
-MF13a-BNT04-octopus	MF13a	octopus	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
-MF13a-BNT07-canoe	MF13a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF13a-BNT09-cactus	MF13a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF13a-BNT12-unicorn	MF13a	unicorn	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF13a-BNT14-sphinx	MF13a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF13a-VNT04-04	MF13a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT05-05	MF13a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT06-06	MF13a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT09-09	MF13a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT10-10	MF13a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT11-11	MF13a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT12-12	MF13a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT13-13	MF13a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT14-14	MF13a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT15-15	MF13a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT16-16	MF13a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT18-18	MF13a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT19-19	MF13a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT20-20	MF13a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT21-21	MF13a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF13a-VNT22-22	MF13a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-BNT02-comb	MF20a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF20a-BNT03-toothbrush	MF20a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF20a-BNT04-octopus	MF20a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF20a-BNT05-bench	MF20a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF20a-BNT06-volcano	MF20a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF20a-BNT07-canoe	MF20a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF20a-BNT08-beaver	MF20a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF20a-BNT09-cactus	MF20a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF20a-BNT10-hammock	MF20a	hammock	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF20a-BNT15-palette	MF20a	palette	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF20a-VNT01-01	MF20a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT02-02	MF20a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT03-03	MF20a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT04-04	MF20a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT05-05	MF20a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT06-06	MF20a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT07-07	MF20a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT08-08	MF20a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT09-09	MF20a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT10-10	MF20a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT11-11	MF20a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT13-13	MF20a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT14-14	MF20a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT15-15	MF20a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT16-16	MF20a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT17-17	MF20a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT18-18	MF20a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT20-20	MF20a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT21-21	MF20a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF20a-VNT22-22	MF20a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-BNT02-comb	MF23a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF23a-BNT03-toothbrush	MF23a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF23a-BNT06-volcano	MF23a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF23a-BNT07-canoe	MF23a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF23a-BNT08-beaver	MF23a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF23a-BNT09-cactus	MF23a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF23a-BNT10-hammock	MF23a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF23a-BNT15-palette	MF23a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-MF23a-VNT01-01	MF23a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT02-02	MF23a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT04-04	MF23a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT05-05	MF23a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT07-07	MF23a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT08-08	MF23a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT12-12	MF23a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT13-13	MF23a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT14-14	MF23a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT15-15	MF23a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT16-16	MF23a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT17-17	MF23a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT18-18	MF23a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT20-20	MF23a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF23a-VNT22-22	MF23a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-BNT03-toothbrush	MF24a	toothbrush	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT05-bench	MF24a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT06-volcano	MF24a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT07-canoe	MF24a	canoe	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT08-beaver	MF24a	beaver	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT09-cactus	MF24a	cactus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT11-stethoscope	MF24a	stethoscope	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT12-unicorn	MF24a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT13-tripod	MF24a	tripod	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF24a-BNT15-palette	MF24a	palette	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-MF24a-VNT01-01	MF24a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT02-02	MF24a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT03-03	MF24a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT04-04	MF24a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT05-05	MF24a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT06-06	MF24a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT07-07	MF24a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT08-08	MF24a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT09-09	MF24a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT10-10	MF24a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT11-11	MF24a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT12-12	MF24a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT14-14	MF24a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT15-15	MF24a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT16-16	MF24a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT18-18	MF24a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT19-19	MF24a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT20-20	MF24a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT21-21	MF24a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF24a-VNT22-22	MF24a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-BNT01-house	MF30a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF30a-BNT02-comb	MF30a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF30a-BNT04-octopus	MF30a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF30a-BNT05-bench	MF30a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF30a-BNT06-volcano	MF30a	volcano	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-MF30a-BNT07-canoe	MF30a	canoe	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
-MF30a-BNT08-beaver	MF30a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF30a-BNT13-tripod	MF30a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF30a-BNT15-palette	MF30a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF30a-VNT01-01	MF30a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT03-03	MF30a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT04-04	MF30a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT05-05	MF30a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT06-06	MF30a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT07-07	MF30a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT08-08	MF30a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT09-09	MF30a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT10-10	MF30a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT11-11	MF30a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT12-12	MF30a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT13-13	MF30a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT14-14	MF30a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT15-15	MF30a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT16-16	MF30a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT17-17	MF30a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT18-18	MF30a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT19-19	MF30a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT21-21	MF30a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF30a-VNT22-22	MF30a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-BNT01-house	MF33a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF33a-BNT02-comb	MF33a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF33a-BNT03-toothbrush	MF33a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT04-octopus	MF33a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT05-bench	MF33a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF33a-BNT06-volcano	MF33a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF33a-BNT07-canoe	MF33a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF33a-BNT08-beaver	MF33a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT09-cactus	MF33a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT10-hammock	MF33a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF33a-BNT12-unicorn	MF33a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT13-tripod	MF33a	tripod	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT14-sphinx	MF33a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-MF33a-BNT15-palette	MF33a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF33a-VNT01-01	MF33a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT02-02	MF33a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT03-03	MF33a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT04-04	MF33a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT05-05	MF33a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT06-06	MF33a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT07-07	MF33a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT08-08	MF33a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT09-09	MF33a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT11-11	MF33a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT12-12	MF33a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT13-13	MF33a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT14-14	MF33a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT15-15	MF33a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT17-17	MF33a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT18-18	MF33a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT19-19	MF33a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT20-20	MF33a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT21-21	MF33a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF33a-VNT22-22	MF33a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-BNT01-house	MF38a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF38a-BNT02-comb	MF38a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF38a-BNT03-toothbrush	MF38a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-MF38a-BNT13-tripod	MF38a	tripod	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-MF38a-VNT02-02	MF38a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT03-03	MF38a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT04-04	MF38a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT05-05	MF38a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT06-06	MF38a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT07-07	MF38a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT08-08	MF38a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT09-09	MF38a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT10-10	MF38a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT11-11	MF38a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT12-12	MF38a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT13-13	MF38a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT14-14	MF38a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT15-15	MF38a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT16-16	MF38a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT17-17	MF38a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT18-18	MF38a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT20-20	MF38a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT21-21	MF38a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-MF38a-VNT22-22	MF38a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-BNT01-house	SDB04a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT02-comb	SDB04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT03-toothbrush	SDB04a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT04-octopus	SDB04a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT05-bench	SDB04a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT06-volcano	SDB04a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT07-canoe	SDB04a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB04a-BNT08-beaver	SDB04a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB04a-BNT09-cactus	SDB04a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT10-hammock	SDB04a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT11-stethoscope	SDB04a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB04a-BNT12-unicorn	SDB04a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT13-tripod	SDB04a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-BNT14-sphinx	SDB04a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB04a-BNT15-palette	SDB04a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB04a-VNT01-01	SDB04a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT02-02	SDB04a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT03-03	SDB04a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT04-04	SDB04a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT05-05	SDB04a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT06-06	SDB04a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT07-07	SDB04a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT09-09	SDB04a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT10-10	SDB04a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT11-11	SDB04a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT12-12	SDB04a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT13-13	SDB04a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT14-14	SDB04a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT15-15	SDB04a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT16-16	SDB04a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT17-17	SDB04a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT18-18	SDB04a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT19-19	SDB04a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT20-20	SDB04a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT21-21	SDB04a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB04a-VNT22-22	SDB04a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-BNT03-toothbrush	SDB06a	toothbrush	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT01-01	SDB06a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT02-02	SDB06a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT03-03	SDB06a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT04-04	SDB06a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT05-05	SDB06a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT06-06	SDB06a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT08-08	SDB06a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT09-09	SDB06a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT10-10	SDB06a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT11-11	SDB06a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT12-12	SDB06a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT15-15	SDB06a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT18-18	SDB06a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT19-19	SDB06a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT20-20	SDB06a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB06a-VNT22-22	SDB06a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-BNT01-house	SDB07a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB07a-BNT02-comb	SDB07a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB07a-BNT03-toothbrush	SDB07a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB07a-BNT05-bench	SDB07a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB07a-BNT06-volcano	SDB07a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB07a-BNT08-beaver	SDB07a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB07a-BNT09-cactus	SDB07a	cactus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-SDB07a-BNT11-stethoscope	SDB07a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB07a-BNT14-sphinx	SDB07a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT01-01	SDB07a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT02-02	SDB07a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT04-04	SDB07a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT05-05	SDB07a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT06-06	SDB07a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT07-07	SDB07a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT08-08	SDB07a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT09-09	SDB07a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT10-10	SDB07a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT11-11	SDB07a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT12-12	SDB07a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT13-13	SDB07a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT14-14	SDB07a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT15-15	SDB07a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT16-16	SDB07a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT19-19	SDB07a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT21-21	SDB07a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB07a-VNT22-22	SDB07a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-BNT01-house	SDB09a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB09a-BNT03-toothbrush	SDB09a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB09a-BNT05-bench	SDB09a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB09a-BNT07-canoe	SDB09a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB09a-BNT10-hammock	SDB09a	hammock	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
-SDB09a-BNT13-tripod	SDB09a	tripod	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB09a-BNT15-palette	SDB09a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT01-01	SDB09a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT02-02	SDB09a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT03-03	SDB09a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT04-04	SDB09a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT06-06	SDB09a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT08-08	SDB09a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT11-11	SDB09a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT12-12	SDB09a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT13-13	SDB09a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT16-16	SDB09a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT17-17	SDB09a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT18-18	SDB09a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB09a-VNT19-19	SDB09a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-BNT01-house	SDB12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB12a-BNT02-comb	SDB12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB12a-BNT04-octopus	SDB12a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB12a-BNT05-bench	SDB12a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB12a-BNT06-volcano	SDB12a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB12a-BNT07-canoe	SDB12a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB12a-BNT10-hammock	SDB12a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB12a-BNT11-stethoscope	SDB12a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB12a-BNT12-unicorn	SDB12a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB12a-VNT01-01	SDB12a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT02-02	SDB12a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT03-03	SDB12a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT04-04	SDB12a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT05-05	SDB12a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT06-06	SDB12a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT07-07	SDB12a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT08-08	SDB12a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT09-09	SDB12a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT10-10	SDB12a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT11-11	SDB12a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT13-13	SDB12a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT14-14	SDB12a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT15-15	SDB12a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT17-17	SDB12a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT18-18	SDB12a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT19-19	SDB12a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB12a-VNT20-20	SDB12a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-BNT01-house	SDB13a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB13a-BNT02-comb	SDB13a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB13a-BNT03-toothbrush	SDB13a	toothbrush	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB13a-BNT05-bench	SDB13a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB13a-BNT09-cactus	SDB13a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT01-01	SDB13a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT03-03	SDB13a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT04-04	SDB13a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT05-05	SDB13a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT06-06	SDB13a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT07-07	SDB13a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT08-08	SDB13a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT10-10	SDB13a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT11-11	SDB13a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT12-12	SDB13a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT13-13	SDB13a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT14-14	SDB13a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT15-15	SDB13a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT17-17	SDB13a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT18-18	SDB13a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT19-19	SDB13a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT20-20	SDB13a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB13a-VNT21-21	SDB13a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-BNT01-house	SDB17a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB17a-BNT03-toothbrush	SDB17a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
-SDB17a-BNT06-volcano	SDB17a	volcano	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT01-01	SDB17a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT03-03	SDB17a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT04-04	SDB17a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT05-05	SDB17a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT06-06	SDB17a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT07-07	SDB17a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT09-09	SDB17a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT10-10	SDB17a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT11-11	SDB17a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT12-12	SDB17a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT14-14	SDB17a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT15-15	SDB17a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT16-16	SDB17a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT18-18	SDB17a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT19-19	SDB17a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT21-21	SDB17a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB17a-VNT22-22	SDB17a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-BNT01-house	SDB18a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT02-comb	SDB18a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT03-toothbrush	SDB18a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT04-octopus	SDB18a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT05-bench	SDB18a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT06-volcano	SDB18a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT07-canoe	SDB18a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT08-beaver	SDB18a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB18a-BNT10-hammock	SDB18a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB18a-BNT11-stethoscope	SDB18a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB18a-BNT12-unicorn	SDB18a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB18a-BNT13-tripod	SDB18a	tripod	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB18a-BNT14-sphinx	SDB18a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-SDB18a-BNT15-palette	SDB18a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT04-04	SDB18a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT05-05	SDB18a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT06-06	SDB18a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT07-07	SDB18a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT08-08	SDB18a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT09-09	SDB18a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT10-10	SDB18a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT12-12	SDB18a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT14-14	SDB18a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT15-15	SDB18a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT16-16	SDB18a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT17-17	SDB18a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT18-18	SDB18a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT19-19	SDB18a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT20-20	SDB18a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT21-21	SDB18a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB18a-VNT22-22	SDB18a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-BNT01-house	SDB19a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT02-comb	SDB19a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT04-octopus	SDB19a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT07-canoe	SDB19a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT08-beaver	SDB19a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT09-cactus	SDB19a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT10-hammock	SDB19a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT11-stethoscope	SDB19a	stethoscope	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-SDB19a-BNT14-sphinx	SDB19a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-SDB19a-BNT15-palette	SDB19a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT01-01	SDB19a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT02-02	SDB19a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT04-04	SDB19a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT05-05	SDB19a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT06-06	SDB19a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT08-08	SDB19a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT10-10	SDB19a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT11-11	SDB19a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT12-12	SDB19a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT14-14	SDB19a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT15-15	SDB19a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT16-16	SDB19a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT17-17	SDB19a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT19-19	SDB19a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT20-20	SDB19a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT21-21	SDB19a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-SDB19a-VNT22-22	SDB19a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-BNT01-house	GF01a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT02-comb	GF01a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT03-toothbrush	GF01a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
-GF01a-BNT04-octopus	GF01a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF01a-BNT05-bench	GF01a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT06-volcano	GF01a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT07-canoe	GF01a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT08-beaver	GF01a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT09-cactus	GF01a	cactus	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-GF01a-BNT10-hammock	GF01a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF01a-BNT11-stethoscope	GF01a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF01a-BNT12-unicorn	GF01a	unicorn	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF01a-BNT14-sphinx	GF01a	sphinx	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF01a-BNT15-palette	GF01a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF01a-VNT01-01	GF01a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT02-02	GF01a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT03-03	GF01a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT04-04	GF01a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT05-05	GF01a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT06-06	GF01a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT07-07	GF01a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT08-08	GF01a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT10-10	GF01a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT11-11	GF01a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT12-12	GF01a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT13-13	GF01a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT14-14	GF01a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT16-16	GF01a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT17-17	GF01a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT18-18	GF01a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT19-19	GF01a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT20-20	GF01a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT21-21	GF01a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF01a-VNT22-22	GF01a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-BNT01-house	GF02a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF02a-BNT02-comb	GF02a	comb	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF02a-BNT03-toothbrush	GF02a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF02a-BNT04-octopus	GF02a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF02a-BNT07-canoe	GF02a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF02a-BNT08-beaver	GF02a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF02a-BNT09-cactus	GF02a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF02a-BNT10-hammock	GF02a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF02a-BNT14-sphinx	GF02a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF02a-VNT01-01	GF02a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT02-02	GF02a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT03-03	GF02a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT05-05	GF02a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT06-06	GF02a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT07-07	GF02a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT08-08	GF02a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT09-09	GF02a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT10-10	GF02a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT11-11	GF02a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT12-12	GF02a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT13-13	GF02a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT14-14	GF02a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT15-15	GF02a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT16-16	GF02a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT17-17	GF02a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT18-18	GF02a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT19-19	GF02a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT20-20	GF02a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT21-21	GF02a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF02a-VNT22-22	GF02a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-BNT01-house	GF07a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-BNT02-comb	GF07a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-BNT03-toothbrush	GF07a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-BNT04-octopus	GF07a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF07a-BNT05-bench	GF07a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF07a-BNT06-volcano	GF07a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-BNT07-canoe	GF07a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-BNT11-stethoscope	GF07a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF07a-BNT12-unicorn	GF07a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-BNT13-tripod	GF07a	tripod	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF07a-BNT14-sphinx	GF07a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF07a-BNT15-palette	GF07a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF07a-VNT02-02	GF07a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT03-03	GF07a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT04-04	GF07a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT05-05	GF07a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT06-06	GF07a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT07-07	GF07a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT08-08	GF07a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT11-11	GF07a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT12-12	GF07a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT14-14	GF07a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT15-15	GF07a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT17-17	GF07a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT18-18	GF07a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT20-20	GF07a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT21-21	GF07a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF07a-VNT22-22	GF07a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-BNT01-house	GF09a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF09a-BNT02-comb	GF09a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF09a-BNT03-toothbrush	GF09a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT04-octopus	GF09a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT05-bench	GF09a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT06-volcano	GF09a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF09a-BNT07-canoe	GF09a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT08-beaver	GF09a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT09-cactus	GF09a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT10-hammock	GF09a	hammock	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT11-stethoscope	GF09a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT12-unicorn	GF09a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT13-tripod	GF09a	tripod	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT14-sphinx	GF09a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF09a-BNT15-palette	GF09a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF09a-VNT01-01	GF09a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT02-02	GF09a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT03-03	GF09a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT04-04	GF09a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT05-05	GF09a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT06-06	GF09a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT07-07	GF09a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT08-08	GF09a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT09-09	GF09a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT10-10	GF09a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT11-11	GF09a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT12-12	GF09a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT13-13	GF09a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT14-14	GF09a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT15-15	GF09a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT17-17	GF09a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT18-18	GF09a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT20-20	GF09a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT21-21	GF09a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF09a-VNT22-22	GF09a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-BNT01-house	GF12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF12a-BNT02-comb	GF12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF12a-BNT03-toothbrush	GF12a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
-GF12a-BNT05-bench	GF12a	bench	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF12a-BNT10-hammock	GF12a	hammock	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF12a-BNT12-unicorn	GF12a	unicorn	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF12a-BNT15-palette	GF12a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-GF12a-VNT01-01	GF12a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT02-02	GF12a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT03-03	GF12a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT04-04	GF12a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT05-05	GF12a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT06-06	GF12a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT07-07	GF12a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT08-08	GF12a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT09-09	GF12a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT11-11	GF12a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT12-12	GF12a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT13-13	GF12a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT15-15	GF12a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT17-17	GF12a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT18-18	GF12a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT19-19	GF12a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT20-20	GF12a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF12a-VNT21-21	GF12a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-BNT01-house	GF14a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT02-comb	GF14a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT03-toothbrush	GF14a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT04-octopus	GF14a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT05-bench	GF14a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT06-volcano	GF14a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF14a-BNT07-canoe	GF14a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT08-beaver	GF14a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT09-cactus	GF14a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT10-hammock	GF14a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT12-unicorn	GF14a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF14a-BNT14-sphinx	GF14a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF14a-BNT15-palette	GF14a	palette	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-GF14a-VNT01-01	GF14a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT03-03	GF14a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT04-04	GF14a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT07-07	GF14a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT08-08	GF14a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT09-09	GF14a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT10-10	GF14a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT11-11	GF14a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT12-12	GF14a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT13-13	GF14a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT16-16	GF14a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT17-17	GF14a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT18-18	GF14a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT19-19	GF14a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT20-20	GF14a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT21-21	GF14a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF14a-VNT22-22	GF14a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-BNT01-house	GF15a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT02-comb	GF15a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT03-toothbrush	GF15a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF15a-BNT04-octopus	GF15a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT05-bench	GF15a	bench	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
-GF15a-BNT06-volcano	GF15a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT07-canoe	GF15a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF15a-BNT08-beaver	GF15a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT09-cactus	GF15a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT11-stethoscope	GF15a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF15a-BNT12-unicorn	GF15a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-BNT14-sphinx	GF15a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-GF15a-BNT15-palette	GF15a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-GF15a-VNT01-01	GF15a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT03-03	GF15a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT04-04	GF15a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT05-05	GF15a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT06-06	GF15a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT07-07	GF15a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT09-09	GF15a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT10-10	GF15a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT13-13	GF15a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT14-14	GF15a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT15-15	GF15a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT16-16	GF15a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT17-17	GF15a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT18-18	GF15a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT19-19	GF15a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT20-20	GF15a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT21-21	GF15a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-GF15a-VNT22-22	GF15a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT01-house	RCG03a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT02-comb	RCG03a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG03a-BNT03-toothbrush	RCG03a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT04-octopus	RCG03a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT05-bench	RCG03a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT06-volcano	RCG03a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT07-canoe	RCG03a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG03a-BNT08-beaver	RCG03a	beaver	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT09-cactus	RCG03a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT10-hammock	RCG03a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG03a-BNT11-stethoscope	RCG03a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT12-unicorn	RCG03a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT14-sphinx	RCG03a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-RCG03a-BNT15-palette	RCG03a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT02-02	RCG03a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT03-03	RCG03a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT04-04	RCG03a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT05-05	RCG03a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT06-06	RCG03a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT07-07	RCG03a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT09-09	RCG03a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT10-10	RCG03a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT11-11	RCG03a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT13-13	RCG03a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT15-15	RCG03a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT16-16	RCG03a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT18-18	RCG03a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT19-19	RCG03a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT21-21	RCG03a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG03a-VNT22-22	RCG03a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT01-house	RCG04a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT02-comb	RCG04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG04a-BNT03-toothbrush	RCG04a	toothbrush	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT04-octopus	RCG04a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT05-bench	RCG04a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT06-volcano	RCG04a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT08-beaver	RCG04a	beaver	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT10-hammock	RCG04a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG04a-BNT12-unicorn	RCG04a	unicorn	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT02-02	RCG04a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT03-03	RCG04a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT04-04	RCG04a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT05-05	RCG04a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT06-06	RCG04a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT07-07	RCG04a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT09-09	RCG04a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT10-10	RCG04a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT11-11	RCG04a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT12-12	RCG04a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT13-13	RCG04a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT15-15	RCG04a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT16-16	RCG04a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT17-17	RCG04a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT18-18	RCG04a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT19-19	RCG04a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT20-20	RCG04a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT21-21	RCG04a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG04a-VNT22-22	RCG04a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-BNT01-house	RCG12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG12a-BNT02-comb	RCG12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG12a-BNT03-toothbrush	RCG12a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG12a-BNT04-octopus	RCG12a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG12a-BNT05-bench	RCG12a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG12a-BNT06-volcano	RCG12a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG12a-BNT07-canoe	RCG12a	canoe	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
-RCG12a-BNT08-beaver	RCG12a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG12a-BNT09-cactus	RCG12a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG12a-BNT14-sphinx	RCG12a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT01-01	RCG12a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT02-02	RCG12a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT04-04	RCG12a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT05-05	RCG12a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT06-06	RCG12a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT07-07	RCG12a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT08-08	RCG12a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT09-09	RCG12a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT10-10	RCG12a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT11-11	RCG12a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT12-12	RCG12a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT13-13	RCG12a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT14-14	RCG12a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT15-15	RCG12a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT16-16	RCG12a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT18-18	RCG12a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT19-19	RCG12a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT20-20	RCG12a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG12a-VNT21-21	RCG12a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-BNT01-house	RCG14a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT02-comb	RCG14a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT03-toothbrush	RCG14a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT04-octopus	RCG14a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT05-bench	RCG14a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT06-volcano	RCG14a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG14a-BNT07-canoe	RCG14a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT08-beaver	RCG14a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT09-cactus	RCG14a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT10-hammock	RCG14a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT11-stethoscope	RCG14a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
-RCG14a-BNT12-unicorn	RCG14a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
-RCG14a-BNT14-sphinx	RCG14a	sphinx	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
-RCG14a-BNT15-palette	RCG14a	palette	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT01-01	RCG14a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT02-02	RCG14a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT03-03	RCG14a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT04-04	RCG14a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT05-05	RCG14a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT06-06	RCG14a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT07-07	RCG14a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT08-08	RCG14a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT09-09	RCG14a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT10-10	RCG14a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT12-12	RCG14a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT13-13	RCG14a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT14-14	RCG14a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT15-15	RCG14a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT17-17	RCG14a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT18-18	RCG14a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT20-20	RCG14a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
-RCG14a-VNT21-21	RCG14a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
+MF04a-BNT01-house	MF04a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF04a-BNT02-comb	MF04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF04a-BNT03-toothbrush	MF04a	toothbrush	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT04-octopus	MF04a	octopus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT05-bench	MF04a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF04a-BNT06-volcano	MF04a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT07-canoe	MF04a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT08-beaver	MF04a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT09-cactus	MF04a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT10-hammock	MF04a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT12-unicorn	MF04a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT13-tripod	MF04a	tripod	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF04a-BNT14-sphinx	MF04a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF04a-VNT01-01	MF04a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT02-02	MF04a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT03-03	MF04a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT04-04	MF04a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT05-05	MF04a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT06-06	MF04a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT07-07	MF04a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT08-08	MF04a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT09-09	MF04a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT10-10	MF04a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT11-11	MF04a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT12-12	MF04a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT13-13	MF04a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT14-14	MF04a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT15-15	MF04a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT16-16	MF04a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT17-17	MF04a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT18-18	MF04a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT19-19	MF04a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT20-20	MF04a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT21-21	MF04a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF04a-VNT22-22	MF04a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-BNT01-house	MF06a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT02-comb	MF06a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT03-toothbrush	MF06a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT04-octopus	MF06a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT05-bench	MF06a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT06-volcano	MF06a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT07-canoe	MF06a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT08-beaver	MF06a	beaver	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT09-cactus	MF06a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT10-hammock	MF06a	hammock	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT11-stethoscope	MF06a	stethoscope	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT12-unicorn	MF06a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT13-tripod	MF06a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF06a-BNT14-sphinx	MF06a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF06a-BNT15-palette	MF06a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF06a-VNT02-02	MF06a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT03-03	MF06a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT04-04	MF06a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT05-05	MF06a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT06-06	MF06a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT07-07	MF06a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT08-08	MF06a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT09-09	MF06a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT10-10	MF06a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT11-11	MF06a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT12-12	MF06a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT13-13	MF06a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT14-14	MF06a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT15-15	MF06a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT16-16	MF06a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT17-17	MF06a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT18-18	MF06a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT19-19	MF06a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT20-20	MF06a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT21-21	MF06a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF06a-VNT22-22	MF06a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-BNT01-house	MF08a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT02-comb	MF08a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT03-toothbrush	MF08a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT04-octopus	MF08a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT05-bench	MF08a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT06-volcano	MF08a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT07-canoe	MF08a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT09-cactus	MF08a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT11-stethoscope	MF08a	stethoscope	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT12-unicorn	MF08a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT13-tripod	MF08a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT14-sphinx	MF08a	sphinx	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-BNT15-palette	MF08a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF08a-VNT02-02	MF08a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT03-03	MF08a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT04-04	MF08a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT05-05	MF08a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT06-06	MF08a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT07-07	MF08a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT08-08	MF08a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT09-09	MF08a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT10-10	MF08a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT11-11	MF08a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT12-12	MF08a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT13-13	MF08a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT14-14	MF08a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT15-15	MF08a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT16-16	MF08a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT17-17	MF08a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT18-18	MF08a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT19-19	MF08a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT21-21	MF08a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF08a-VNT22-22	MF08a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-BNT01-house	MF13a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF13a-BNT02-comb	MF13a	comb	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT04-octopus	MF13a	octopus	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT07-canoe	MF13a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF13a-BNT09-cactus	MF13a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT12-unicorn	MF13a	unicorn	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF13a-BNT14-sphinx	MF13a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF13a-VNT04-04	MF13a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT05-05	MF13a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT06-06	MF13a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT09-09	MF13a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT10-10	MF13a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT11-11	MF13a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT12-12	MF13a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT13-13	MF13a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT14-14	MF13a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT15-15	MF13a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT16-16	MF13a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT18-18	MF13a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT19-19	MF13a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT20-20	MF13a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT21-21	MF13a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF13a-VNT22-22	MF13a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-BNT02-comb	MF20a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT03-toothbrush	MF20a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT04-octopus	MF20a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT05-bench	MF20a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT06-volcano	MF20a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT07-canoe	MF20a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT08-beaver	MF20a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT09-cactus	MF20a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF20a-BNT10-hammock	MF20a	hammock	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF20a-BNT15-palette	MF20a	palette	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF20a-VNT01-01	MF20a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT02-02	MF20a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT03-03	MF20a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT04-04	MF20a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT05-05	MF20a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT06-06	MF20a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT07-07	MF20a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT08-08	MF20a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT09-09	MF20a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT10-10	MF20a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT11-11	MF20a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT13-13	MF20a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT14-14	MF20a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT15-15	MF20a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT16-16	MF20a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT17-17	MF20a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT18-18	MF20a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT20-20	MF20a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT21-21	MF20a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF20a-VNT22-22	MF20a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-BNT02-comb	MF23a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT03-toothbrush	MF23a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT06-volcano	MF23a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF23a-BNT07-canoe	MF23a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT08-beaver	MF23a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT09-cactus	MF23a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF23a-BNT10-hammock	MF23a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF23a-BNT15-palette	MF23a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF23a-VNT01-01	MF23a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT02-02	MF23a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT04-04	MF23a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT05-05	MF23a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT07-07	MF23a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT08-08	MF23a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT12-12	MF23a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT13-13	MF23a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT14-14	MF23a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT15-15	MF23a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT16-16	MF23a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT17-17	MF23a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT18-18	MF23a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT20-20	MF23a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF23a-VNT22-22	MF23a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-BNT03-toothbrush	MF24a	toothbrush	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT05-bench	MF24a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT06-volcano	MF24a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT07-canoe	MF24a	canoe	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT08-beaver	MF24a	beaver	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT09-cactus	MF24a	cactus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT11-stethoscope	MF24a	stethoscope	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT12-unicorn	MF24a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT13-tripod	MF24a	tripod	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF24a-BNT15-palette	MF24a	palette	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+MF24a-VNT01-01	MF24a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT02-02	MF24a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT03-03	MF24a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT04-04	MF24a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT05-05	MF24a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT06-06	MF24a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT07-07	MF24a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT08-08	MF24a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT09-09	MF24a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT10-10	MF24a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT11-11	MF24a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT12-12	MF24a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT14-14	MF24a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT15-15	MF24a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT16-16	MF24a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT18-18	MF24a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT19-19	MF24a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT20-20	MF24a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT21-21	MF24a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF24a-VNT22-22	MF24a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-BNT01-house	MF30a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT02-comb	MF30a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT04-octopus	MF30a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT05-bench	MF30a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT06-volcano	MF30a	volcano	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT07-canoe	MF30a	canoe	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT08-beaver	MF30a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF30a-BNT13-tripod	MF30a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF30a-BNT15-palette	MF30a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF30a-VNT01-01	MF30a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT03-03	MF30a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT04-04	MF30a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT05-05	MF30a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT06-06	MF30a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT07-07	MF30a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT08-08	MF30a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT09-09	MF30a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT10-10	MF30a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT11-11	MF30a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT12-12	MF30a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT13-13	MF30a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT14-14	MF30a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT15-15	MF30a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT16-16	MF30a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT17-17	MF30a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT18-18	MF30a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT19-19	MF30a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT21-21	MF30a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF30a-VNT22-22	MF30a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-BNT01-house	MF33a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT02-comb	MF33a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT03-toothbrush	MF33a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT04-octopus	MF33a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT05-bench	MF33a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT06-volcano	MF33a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT07-canoe	MF33a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT08-beaver	MF33a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT09-cactus	MF33a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT10-hammock	MF33a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF33a-BNT12-unicorn	MF33a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT13-tripod	MF33a	tripod	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT14-sphinx	MF33a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+MF33a-BNT15-palette	MF33a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF33a-VNT01-01	MF33a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT02-02	MF33a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT03-03	MF33a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT04-04	MF33a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT05-05	MF33a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT06-06	MF33a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT07-07	MF33a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT08-08	MF33a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT09-09	MF33a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT11-11	MF33a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT12-12	MF33a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT13-13	MF33a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT14-14	MF33a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT15-15	MF33a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT17-17	MF33a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT18-18	MF33a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT19-19	MF33a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT20-20	MF33a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT21-21	MF33a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF33a-VNT22-22	MF33a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-BNT01-house	MF38a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF38a-BNT02-comb	MF38a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF38a-BNT03-toothbrush	MF38a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+MF38a-BNT13-tripod	MF38a	tripod	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+MF38a-VNT02-02	MF38a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT03-03	MF38a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT04-04	MF38a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT05-05	MF38a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT06-06	MF38a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT07-07	MF38a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT08-08	MF38a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT09-09	MF38a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT10-10	MF38a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT11-11	MF38a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT12-12	MF38a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT13-13	MF38a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT14-14	MF38a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT15-15	MF38a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT16-16	MF38a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT17-17	MF38a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT18-18	MF38a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT20-20	MF38a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT21-21	MF38a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+MF38a-VNT22-22	MF38a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT01-house	SDB04a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT02-comb	SDB04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT03-toothbrush	SDB04a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT04-octopus	SDB04a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT05-bench	SDB04a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT06-volcano	SDB04a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT07-canoe	SDB04a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT08-beaver	SDB04a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT09-cactus	SDB04a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT10-hammock	SDB04a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT11-stethoscope	SDB04a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT12-unicorn	SDB04a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT13-tripod	SDB04a	tripod	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-BNT14-sphinx	SDB04a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB04a-BNT15-palette	SDB04a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB04a-VNT01-01	SDB04a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT02-02	SDB04a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT03-03	SDB04a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT04-04	SDB04a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT05-05	SDB04a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT06-06	SDB04a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT07-07	SDB04a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT09-09	SDB04a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT10-10	SDB04a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT11-11	SDB04a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT12-12	SDB04a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT13-13	SDB04a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT14-14	SDB04a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT15-15	SDB04a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT16-16	SDB04a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT17-17	SDB04a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT18-18	SDB04a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT19-19	SDB04a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT20-20	SDB04a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT21-21	SDB04a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB04a-VNT22-22	SDB04a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-BNT03-toothbrush	SDB06a	toothbrush	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT01-01	SDB06a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT02-02	SDB06a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT03-03	SDB06a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT04-04	SDB06a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT05-05	SDB06a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT06-06	SDB06a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT08-08	SDB06a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT09-09	SDB06a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT10-10	SDB06a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT11-11	SDB06a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT12-12	SDB06a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT15-15	SDB06a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT18-18	SDB06a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT19-19	SDB06a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT20-20	SDB06a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB06a-VNT22-22	SDB06a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT01-house	SDB07a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT02-comb	SDB07a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT03-toothbrush	SDB07a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT05-bench	SDB07a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT06-volcano	SDB07a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT08-beaver	SDB07a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB07a-BNT09-cactus	SDB07a	cactus	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT11-stethoscope	SDB07a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB07a-BNT14-sphinx	SDB07a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT01-01	SDB07a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT02-02	SDB07a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT04-04	SDB07a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT05-05	SDB07a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT06-06	SDB07a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT07-07	SDB07a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT08-08	SDB07a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT09-09	SDB07a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT10-10	SDB07a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT11-11	SDB07a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT12-12	SDB07a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT13-13	SDB07a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT14-14	SDB07a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT15-15	SDB07a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT16-16	SDB07a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT19-19	SDB07a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT21-21	SDB07a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB07a-VNT22-22	SDB07a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT01-house	SDB09a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB09a-BNT03-toothbrush	SDB09a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT05-bench	SDB09a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT07-canoe	SDB09a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT10-hammock	SDB09a	hammock	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT13-tripod	SDB09a	tripod	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB09a-BNT15-palette	SDB09a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT01-01	SDB09a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT02-02	SDB09a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT03-03	SDB09a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT04-04	SDB09a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT06-06	SDB09a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT08-08	SDB09a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT11-11	SDB09a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT12-12	SDB09a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT13-13	SDB09a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT16-16	SDB09a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT17-17	SDB09a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT18-18	SDB09a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB09a-VNT19-19	SDB09a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT01-house	SDB12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT02-comb	SDB12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT04-octopus	SDB12a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT05-bench	SDB12a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT06-volcano	SDB12a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT07-canoe	SDB12a	canoe	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT10-hammock	SDB12a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-BNT11-stethoscope	SDB12a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB12a-BNT12-unicorn	SDB12a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB12a-VNT01-01	SDB12a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT02-02	SDB12a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT03-03	SDB12a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT04-04	SDB12a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT05-05	SDB12a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT06-06	SDB12a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT07-07	SDB12a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT08-08	SDB12a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT09-09	SDB12a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT10-10	SDB12a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT11-11	SDB12a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT13-13	SDB12a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT14-14	SDB12a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT15-15	SDB12a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT17-17	SDB12a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT18-18	SDB12a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT19-19	SDB12a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB12a-VNT20-20	SDB12a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-BNT01-house	SDB13a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT02-comb	SDB13a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT03-toothbrush	SDB13a	toothbrush	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB13a-BNT05-bench	SDB13a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB13a-BNT09-cactus	SDB13a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT01-01	SDB13a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT03-03	SDB13a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT04-04	SDB13a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT05-05	SDB13a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT06-06	SDB13a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT07-07	SDB13a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT08-08	SDB13a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT10-10	SDB13a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT11-11	SDB13a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT12-12	SDB13a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT13-13	SDB13a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT14-14	SDB13a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT15-15	SDB13a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT17-17	SDB13a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT18-18	SDB13a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT19-19	SDB13a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT20-20	SDB13a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB13a-VNT21-21	SDB13a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-BNT01-house	SDB17a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB17a-BNT03-toothbrush	SDB17a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+SDB17a-BNT06-volcano	SDB17a	volcano	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT01-01	SDB17a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT03-03	SDB17a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT04-04	SDB17a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT05-05	SDB17a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT06-06	SDB17a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT07-07	SDB17a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT09-09	SDB17a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT10-10	SDB17a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT11-11	SDB17a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT12-12	SDB17a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT14-14	SDB17a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT15-15	SDB17a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT16-16	SDB17a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT18-18	SDB17a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT19-19	SDB17a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT21-21	SDB17a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB17a-VNT22-22	SDB17a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT01-house	SDB18a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT02-comb	SDB18a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT03-toothbrush	SDB18a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT04-octopus	SDB18a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT05-bench	SDB18a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT06-volcano	SDB18a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT07-canoe	SDB18a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT08-beaver	SDB18a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT10-hammock	SDB18a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB18a-BNT11-stethoscope	SDB18a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT12-unicorn	SDB18a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT13-tripod	SDB18a	tripod	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT14-sphinx	SDB18a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+SDB18a-BNT15-palette	SDB18a	palette	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT04-04	SDB18a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT05-05	SDB18a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT06-06	SDB18a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT07-07	SDB18a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT08-08	SDB18a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT09-09	SDB18a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT10-10	SDB18a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT12-12	SDB18a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT14-14	SDB18a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT15-15	SDB18a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT16-16	SDB18a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT17-17	SDB18a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT18-18	SDB18a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT19-19	SDB18a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT20-20	SDB18a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT21-21	SDB18a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB18a-VNT22-22	SDB18a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-BNT01-house	SDB19a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT02-comb	SDB19a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT04-octopus	SDB19a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT07-canoe	SDB19a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT08-beaver	SDB19a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT09-cactus	SDB19a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT10-hammock	SDB19a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT11-stethoscope	SDB19a	stethoscope	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+SDB19a-BNT14-sphinx	SDB19a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+SDB19a-BNT15-palette	SDB19a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT01-01	SDB19a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT02-02	SDB19a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT04-04	SDB19a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT05-05	SDB19a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT06-06	SDB19a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT08-08	SDB19a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT10-10	SDB19a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT11-11	SDB19a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT12-12	SDB19a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT14-14	SDB19a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT15-15	SDB19a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT16-16	SDB19a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT17-17	SDB19a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT19-19	SDB19a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT20-20	SDB19a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT21-21	SDB19a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+SDB19a-VNT22-22	SDB19a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-BNT01-house	GF01a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT02-comb	GF01a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT03-toothbrush	GF01a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT04-octopus	GF01a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT05-bench	GF01a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT06-volcano	GF01a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT07-canoe	GF01a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT08-beaver	GF01a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT09-cactus	GF01a	cactus	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT10-hammock	GF01a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF01a-BNT11-stethoscope	GF01a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT12-unicorn	GF01a	unicorn	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT14-sphinx	GF01a	sphinx	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-BNT15-palette	GF01a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF01a-VNT01-01	GF01a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT02-02	GF01a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT03-03	GF01a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT04-04	GF01a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT05-05	GF01a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT06-06	GF01a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT07-07	GF01a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT08-08	GF01a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT10-10	GF01a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT11-11	GF01a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT12-12	GF01a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT13-13	GF01a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT14-14	GF01a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT16-16	GF01a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT17-17	GF01a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT18-18	GF01a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT19-19	GF01a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT20-20	GF01a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT21-21	GF01a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF01a-VNT22-22	GF01a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-BNT01-house	GF02a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF02a-BNT02-comb	GF02a	comb	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT03-toothbrush	GF02a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT04-octopus	GF02a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT07-canoe	GF02a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF02a-BNT08-beaver	GF02a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT09-cactus	GF02a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT10-hammock	GF02a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-BNT14-sphinx	GF02a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF02a-VNT01-01	GF02a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT02-02	GF02a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT03-03	GF02a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT05-05	GF02a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT06-06	GF02a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT07-07	GF02a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT08-08	GF02a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT09-09	GF02a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT10-10	GF02a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT11-11	GF02a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT12-12	GF02a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT13-13	GF02a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT14-14	GF02a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT15-15	GF02a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT16-16	GF02a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT17-17	GF02a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT18-18	GF02a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT19-19	GF02a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT20-20	GF02a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT21-21	GF02a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF02a-VNT22-22	GF02a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-BNT01-house	GF07a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT02-comb	GF07a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT03-toothbrush	GF07a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT04-octopus	GF07a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT05-bench	GF07a	bench	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT06-volcano	GF07a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT07-canoe	GF07a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT11-stethoscope	GF07a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT12-unicorn	GF07a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-BNT13-tripod	GF07a	tripod	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT14-sphinx	GF07a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF07a-BNT15-palette	GF07a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF07a-VNT02-02	GF07a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT03-03	GF07a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT04-04	GF07a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT05-05	GF07a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT06-06	GF07a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT07-07	GF07a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT08-08	GF07a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT11-11	GF07a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT12-12	GF07a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT14-14	GF07a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT15-15	GF07a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT17-17	GF07a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT18-18	GF07a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT20-20	GF07a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT21-21	GF07a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF07a-VNT22-22	GF07a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-BNT01-house	GF09a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT02-comb	GF09a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT03-toothbrush	GF09a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT04-octopus	GF09a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT05-bench	GF09a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT06-volcano	GF09a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF09a-BNT07-canoe	GF09a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT08-beaver	GF09a	beaver	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT09-cactus	GF09a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT10-hammock	GF09a	hammock	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT11-stethoscope	GF09a	stethoscope	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT12-unicorn	GF09a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT13-tripod	GF09a	tripod	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT14-sphinx	GF09a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF09a-BNT15-palette	GF09a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF09a-VNT01-01	GF09a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT02-02	GF09a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT03-03	GF09a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT04-04	GF09a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT05-05	GF09a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT06-06	GF09a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT07-07	GF09a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT08-08	GF09a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT09-09	GF09a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT10-10	GF09a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT11-11	GF09a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT12-12	GF09a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT13-13	GF09a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT14-14	GF09a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT15-15	GF09a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT17-17	GF09a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT18-18	GF09a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT20-20	GF09a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT21-21	GF09a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF09a-VNT22-22	GF09a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-BNT01-house	GF12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF12a-BNT02-comb	GF12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF12a-BNT03-toothbrush	GF12a	toothbrush	haʊ's	HH AW S	MO	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT05-bench	GF12a	bench	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT10-hammock	GF12a	hammock	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT12-unicorn	GF12a	unicorn	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF12a-BNT15-palette	GF12a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+GF12a-VNT01-01	GF12a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT02-02	GF12a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT03-03	GF12a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT04-04	GF12a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT05-05	GF12a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT06-06	GF12a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT07-07	GF12a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT08-08	GF12a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT09-09	GF12a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT11-11	GF12a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT12-12	GF12a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT13-13	GF12a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT15-15	GF12a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT17-17	GF12a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT18-18	GF12a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT19-19	GF12a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT20-20	GF12a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF12a-VNT21-21	GF12a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-BNT01-house	GF14a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT02-comb	GF14a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT03-toothbrush	GF14a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT04-octopus	GF14a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT05-bench	GF14a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT06-volcano	GF14a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF14a-BNT07-canoe	GF14a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT08-beaver	GF14a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT09-cactus	GF14a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT10-hammock	GF14a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT12-unicorn	GF14a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF14a-BNT14-sphinx	GF14a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF14a-BNT15-palette	GF14a	palette	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+GF14a-VNT01-01	GF14a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT03-03	GF14a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT04-04	GF14a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT07-07	GF14a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT08-08	GF14a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT09-09	GF14a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT10-10	GF14a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT11-11	GF14a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT12-12	GF14a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT13-13	GF14a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT16-16	GF14a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT17-17	GF14a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT18-18	GF14a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT19-19	GF14a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT20-20	GF14a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT21-21	GF14a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF14a-VNT22-22	GF14a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-BNT01-house	GF15a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT02-comb	GF15a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT03-toothbrush	GF15a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT04-octopus	GF15a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT05-bench	GF15a	bench	haʊ's	HH AW S	S	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT06-volcano	GF15a	volcano	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT07-canoe	GF15a	canoe	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT08-beaver	GF15a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT09-cactus	GF15a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT11-stethoscope	GF15a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT12-unicorn	GF15a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-BNT14-sphinx	GF15a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+GF15a-BNT15-palette	GF15a	palette	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+GF15a-VNT01-01	GF15a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT03-03	GF15a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT04-04	GF15a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT05-05	GF15a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT06-06	GF15a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT07-07	GF15a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT09-09	GF15a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT10-10	GF15a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT13-13	GF15a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT14-14	GF15a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT15-15	GF15a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT16-16	GF15a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT17-17	GF15a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT18-18	GF15a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT19-19	GF15a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT20-20	GF15a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT21-21	GF15a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+GF15a-VNT22-22	GF15a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT01-house	RCG03a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT02-comb	RCG03a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT03-toothbrush	RCG03a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT04-octopus	RCG03a	octopus	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT05-bench	RCG03a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT06-volcano	RCG03a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT07-canoe	RCG03a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT08-beaver	RCG03a	beaver	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT09-cactus	RCG03a	cactus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT10-hammock	RCG03a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG03a-BNT11-stethoscope	RCG03a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT12-unicorn	RCG03a	unicorn	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT14-sphinx	RCG03a	sphinx	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG03a-BNT15-palette	RCG03a	palette	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT02-02	RCG03a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT03-03	RCG03a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT04-04	RCG03a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT05-05	RCG03a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT06-06	RCG03a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT07-07	RCG03a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT09-09	RCG03a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT10-10	RCG03a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT11-11	RCG03a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT13-13	RCG03a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT15-15	RCG03a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT16-16	RCG03a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT18-18	RCG03a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT19-19	RCG03a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT21-21	RCG03a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG03a-VNT22-22	RCG03a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT01-house	RCG04a	house	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT02-comb	RCG04a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG04a-BNT03-toothbrush	RCG04a	toothbrush	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT04-octopus	RCG04a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT05-bench	RCG04a	bench	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT06-volcano	RCG04a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT08-beaver	RCG04a	beaver	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT10-hammock	RCG04a	hammock	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG04a-BNT12-unicorn	RCG04a	unicorn	haʊ's	HH AW S	AN	train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT02-02	RCG04a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT03-03	RCG04a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT04-04	RCG04a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT05-05	RCG04a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT06-06	RCG04a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT07-07	RCG04a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT09-09	RCG04a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT10-10	RCG04a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT11-11	RCG04a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT12-12	RCG04a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT13-13	RCG04a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT15-15	RCG04a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT16-16	RCG04a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT17-17	RCG04a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT18-18	RCG04a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT19-19	RCG04a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT20-20	RCG04a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT21-21	RCG04a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG04a-VNT22-22	RCG04a	22	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT01-house	RCG12a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT02-comb	RCG12a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT03-toothbrush	RCG12a	toothbrush	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT04-octopus	RCG12a	octopus	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT05-bench	RCG12a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT06-volcano	RCG12a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT07-canoe	RCG12a	canoe	haʊ's	HH AW S	F	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT08-beaver	RCG12a	beaver	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-BNT09-cactus	RCG12a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG12a-BNT14-sphinx	RCG12a	sphinx	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT01-01	RCG12a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT02-02	RCG12a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT04-04	RCG12a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT05-05	RCG12a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT06-06	RCG12a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT07-07	RCG12a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT08-08	RCG12a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT09-09	RCG12a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT10-10	RCG12a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT11-11	RCG12a	11	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT12-12	RCG12a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT13-13	RCG12a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT14-14	RCG12a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT15-15	RCG12a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT16-16	RCG12a	16	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT18-18	RCG12a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT19-19	RCG12a	19	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT20-20	RCG12a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG12a-VNT21-21	RCG12a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT01-house	RCG14a	house	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT02-comb	RCG14a	comb	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT03-toothbrush	RCG14a	toothbrush	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT04-octopus	RCG14a	octopus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT05-bench	RCG14a	bench	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT06-volcano	RCG14a	volcano	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT07-canoe	RCG14a	canoe	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT08-beaver	RCG14a	beaver	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT09-cactus	RCG14a	cactus	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT10-hammock	RCG14a	hammock	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT11-stethoscope	RCG14a	stethoscope	haʊ's	HH AW S	N	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT12-unicorn	RCG14a	unicorn	haʊ's	HH AW S	C	train/audio/empty.wav	28992	12.3	True
+RCG14a-BNT14-sphinx	RCG14a	sphinx	haʊ's	HH AW S	M	train/audio/empty.wav	28992	12.3	False
+RCG14a-BNT15-palette	RCG14a	palette	haʊ's	HH AW S	O	train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT01-01	RCG14a	01	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT02-02	RCG14a	02	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT03-03	RCG14a	03	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT04-04	RCG14a	04	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT05-05	RCG14a	05	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT06-06	RCG14a	06	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT07-07	RCG14a	07	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT08-08	RCG14a	08	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT09-09	RCG14a	09	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT10-10	RCG14a	10	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT12-12	RCG14a	12	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT13-13	RCG14a	13	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT14-14	RCG14a	14	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT15-15	RCG14a	15	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT17-17	RCG14a	17	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT18-18	RCG14a	18	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT20-20	RCG14a	20	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
+RCG14a-VNT21-21	RCG14a	21	haʊ's	HH AW S		train/audio/empty.wav	28992	12.3	False
```

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/train/audio/empty.wav` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/train/audio/empty.wav`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/asr_valid.tsv` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/asr_valid.tsv`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
-MF31a-BNT01-house	MF31a	house	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT03-toothbrush	MF31a	toothbrush	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT05-bench	MF31a	bench	haʊ's	HH AW S	O	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT07-canoe	MF31a	canoe	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT15-palette	MF31a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT01-01	MF31a	01	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT02-02	MF31a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT05-05	MF31a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT06-06	MF31a	06	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT07-07	MF31a	07	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT08-08	MF31a	08	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT09-09	MF31a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT10-10	MF31a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT11-11	MF31a	11	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT12-12	MF31a	12	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT13-13	MF31a	13	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT14-14	MF31a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT15-15	MF31a	15	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT16-16	MF31a	16	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT18-18	MF31a	18	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT19-19	MF31a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-MF31a-VNT21-21	MF31a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT02-comb	SDB11a	comb	haʊ's	HH AW S	AN	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT05-bench	SDB11a	bench	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT06-volcano	SDB11a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT07-canoe	SDB11a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT09-cactus	SDB11a	cactus	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT01-01	SDB11a	01	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT02-02	SDB11a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT03-03	SDB11a	03	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT04-04	SDB11a	04	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT05-05	SDB11a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT06-06	SDB11a	06	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT07-07	SDB11a	07	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT09-09	SDB11a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT10-10	SDB11a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT11-11	SDB11a	11	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT12-12	SDB11a	12	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT13-13	SDB11a	13	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT14-14	SDB11a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT15-15	SDB11a	15	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT16-16	SDB11a	16	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT18-18	SDB11a	18	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT19-19	SDB11a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT21-21	SDB11a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-SDB11a-VNT22-22	SDB11a	22	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT01-house	GF06a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT02-comb	GF06a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT03-toothbrush	GF06a	toothbrush	haʊ's	HH AW S	MO	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT04-octopus	GF06a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT05-bench	GF06a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT06-volcano	GF06a	volcano	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT07-canoe	GF06a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT09-cactus	GF06a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT11-stethoscope	GF06a	stethoscope	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT12-unicorn	GF06a	unicorn	haʊ's	HH AW S	M	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT13-tripod	GF06a	tripod	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT14-sphinx	GF06a	sphinx	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT15-palette	GF06a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT01-01	GF06a	01	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT02-02	GF06a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT03-03	GF06a	03	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT04-04	GF06a	04	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT05-05	GF06a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT07-07	GF06a	07	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT08-08	GF06a	08	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT09-09	GF06a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT10-10	GF06a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT11-11	GF06a	11	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT12-12	GF06a	12	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT13-13	GF06a	13	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT14-14	GF06a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT15-15	GF06a	15	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT16-16	GF06a	16	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT19-19	GF06a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT20-20	GF06a	20	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT21-21	GF06a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-GF06a-VNT22-22	GF06a	22	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT01-house	RCG18a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT02-comb	RCG18a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT03-toothbrush	RCG18a	toothbrush	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT04-octopus	RCG18a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT05-bench	RCG18a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT06-volcano	RCG18a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT07-canoe	RCG18a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT08-beaver	RCG18a	beaver	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT09-cactus	RCG18a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT10-hammock	RCG18a	hammock	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT02-02	RCG18a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT03-03	RCG18a	03	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT04-04	RCG18a	04	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT05-05	RCG18a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT06-06	RCG18a	06	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT09-09	RCG18a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT10-10	RCG18a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT14-14	RCG18a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT17-17	RCG18a	17	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT19-19	RCG18a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT20-20	RCG18a	20	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT21-21	RCG18a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
-RCG18a-VNT22-22	RCG18a	22	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
+MF31a-BNT01-house	MF31a	house	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT03-toothbrush	MF31a	toothbrush	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT05-bench	MF31a	bench	haʊ's	HH AW S	O	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT07-canoe	MF31a	canoe	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT15-palette	MF31a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT01-01	MF31a	01	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT02-02	MF31a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT05-05	MF31a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT06-06	MF31a	06	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT07-07	MF31a	07	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT08-08	MF31a	08	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT09-09	MF31a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT10-10	MF31a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT11-11	MF31a	11	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT12-12	MF31a	12	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT13-13	MF31a	13	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT14-14	MF31a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT15-15	MF31a	15	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT16-16	MF31a	16	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT18-18	MF31a	18	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT19-19	MF31a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+MF31a-VNT21-21	MF31a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT02-comb	SDB11a	comb	haʊ's	HH AW S	AN	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT05-bench	SDB11a	bench	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT06-volcano	SDB11a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT07-canoe	SDB11a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT09-cactus	SDB11a	cactus	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT01-01	SDB11a	01	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT02-02	SDB11a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT03-03	SDB11a	03	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT04-04	SDB11a	04	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT05-05	SDB11a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT06-06	SDB11a	06	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT07-07	SDB11a	07	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT09-09	SDB11a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT10-10	SDB11a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT11-11	SDB11a	11	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT12-12	SDB11a	12	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT13-13	SDB11a	13	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT14-14	SDB11a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT15-15	SDB11a	15	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT16-16	SDB11a	16	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT18-18	SDB11a	18	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT19-19	SDB11a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT21-21	SDB11a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+SDB11a-VNT22-22	SDB11a	22	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT01-house	GF06a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT02-comb	GF06a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT03-toothbrush	GF06a	toothbrush	haʊ's	HH AW S	MO	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT04-octopus	GF06a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT05-bench	GF06a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT06-volcano	GF06a	volcano	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT07-canoe	GF06a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT09-cactus	GF06a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT11-stethoscope	GF06a	stethoscope	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT12-unicorn	GF06a	unicorn	haʊ's	HH AW S	M	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT13-tripod	GF06a	tripod	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT14-sphinx	GF06a	sphinx	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT15-palette	GF06a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT01-01	GF06a	01	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT02-02	GF06a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT03-03	GF06a	03	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT04-04	GF06a	04	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT05-05	GF06a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT07-07	GF06a	07	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT08-08	GF06a	08	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT09-09	GF06a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT10-10	GF06a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT11-11	GF06a	11	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT12-12	GF06a	12	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT13-13	GF06a	13	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT14-14	GF06a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT15-15	GF06a	15	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT16-16	GF06a	16	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT19-19	GF06a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT20-20	GF06a	20	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT21-21	GF06a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+GF06a-VNT22-22	GF06a	22	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT01-house	RCG18a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT02-comb	RCG18a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT03-toothbrush	RCG18a	toothbrush	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT04-octopus	RCG18a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT05-bench	RCG18a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT06-volcano	RCG18a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT07-canoe	RCG18a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT08-beaver	RCG18a	beaver	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT09-cactus	RCG18a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT10-hammock	RCG18a	hammock	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT02-02	RCG18a	02	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT03-03	RCG18a	03	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT04-04	RCG18a	04	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT05-05	RCG18a	05	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT06-06	RCG18a	06	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT09-09	RCG18a	09	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT10-10	RCG18a	10	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT14-14	RCG18a	14	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT17-17	RCG18a	17	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT19-19	RCG18a	19	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT20-20	RCG18a	20	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT21-21	RCG18a	21	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
+RCG18a-VNT22-22	RCG18a	22	haʊ's	HH AW S		valid/audio/empty.wav	28992	12.3	False
```

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/audio/empty.wav` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/audio/empty.wav`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/correctness_valid.tsv` & `psstdata-1.0.1/psstdata/artificialdata/psst-data-ARTIFICIAL/valid/correctness_valid.tsv`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
-MF31a-BNT01-house	MF31a	house	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT03-toothbrush	MF31a	toothbrush	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT05-bench	MF31a	bench	haʊ's	HH AW S	O	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT07-canoe	MF31a	canoe	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-MF31a-BNT15-palette	MF31a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT02-comb	SDB11a	comb	haʊ's	HH AW S	AN	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT05-bench	SDB11a	bench	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT06-volcano	SDB11a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT07-canoe	SDB11a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-SDB11a-BNT09-cactus	SDB11a	cactus	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT01-house	GF06a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT02-comb	GF06a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT03-toothbrush	GF06a	toothbrush	haʊ's	HH AW S	MO	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT04-octopus	GF06a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT05-bench	GF06a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT06-volcano	GF06a	volcano	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT07-canoe	GF06a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT09-cactus	GF06a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT11-stethoscope	GF06a	stethoscope	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT12-unicorn	GF06a	unicorn	haʊ's	HH AW S	M	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT13-tripod	GF06a	tripod	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-GF06a-BNT14-sphinx	GF06a	sphinx	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-GF06a-BNT15-palette	GF06a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT01-house	RCG18a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT02-comb	RCG18a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT03-toothbrush	RCG18a	toothbrush	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT04-octopus	RCG18a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT05-bench	RCG18a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT06-volcano	RCG18a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT07-canoe	RCG18a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT08-beaver	RCG18a	beaver	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
-RCG18a-BNT09-cactus	RCG18a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
-RCG18a-BNT10-hammock	RCG18a	hammock	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+id	session	prompt	transcript_ipa	transcript_arpabet	code	filename	duration_frames	aq_index	is_correct
+MF31a-BNT01-house	MF31a	house	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT03-toothbrush	MF31a	toothbrush	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT05-bench	MF31a	bench	haʊ's	HH AW S	O	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT07-canoe	MF31a	canoe	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+MF31a-BNT15-palette	MF31a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT02-comb	SDB11a	comb	haʊ's	HH AW S	AN	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT05-bench	SDB11a	bench	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT06-volcano	SDB11a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT07-canoe	SDB11a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+SDB11a-BNT09-cactus	SDB11a	cactus	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT01-house	GF06a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT02-comb	GF06a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT03-toothbrush	GF06a	toothbrush	haʊ's	HH AW S	MO	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT04-octopus	GF06a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT05-bench	GF06a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT06-volcano	GF06a	volcano	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT07-canoe	GF06a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT09-cactus	GF06a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT11-stethoscope	GF06a	stethoscope	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT12-unicorn	GF06a	unicorn	haʊ's	HH AW S	M	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT13-tripod	GF06a	tripod	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+GF06a-BNT14-sphinx	GF06a	sphinx	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+GF06a-BNT15-palette	GF06a	palette	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT01-house	RCG18a	house	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT02-comb	RCG18a	comb	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT03-toothbrush	RCG18a	toothbrush	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT04-octopus	RCG18a	octopus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT05-bench	RCG18a	bench	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT06-volcano	RCG18a	volcano	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT07-canoe	RCG18a	canoe	haʊ's	HH AW S	S	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT08-beaver	RCG18a	beaver	haʊ's	HH AW S	F	valid/audio/empty.wav	28992	12.3	False
+RCG18a-BNT09-cactus	RCG18a	cactus	haʊ's	HH AW S	C	valid/audio/empty.wav	28992	12.3	True
+RCG18a-BNT10-hammock	RCG18a	hammock	haʊ's	HH AW S	N	valid/audio/empty.wav	28992	12.3	False
```

### Comparing `psstdata-1.0.0/psstdata/assets/correctness.json` & `psstdata-1.0.1/psstdata/assets/correctness.json`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/assets/vocab_arpabet.json` & `psstdata-1.0.1/psstdata/assets/vocab_arpabet.json`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/config.py` & `psstdata-1.0.1/psstdata/config.py`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/datastructures.py` & `psstdata-1.0.1/psstdata/datastructures.py`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/downloading.py` & `psstdata-1.0.1/psstdata/downloading.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import shutil
 import tarfile
+from pathlib import Path
+from logging import INFO
 
 import requests
 
 import psstdata
 import psstdata.networking
 from psstdata.config import PSSTSettings
 from psstdata.versioning import PSSTVersionCollection
 
 
 def download(destination, version_id=None):
-    local_versions = PSSTVersionCollection.from_disk(destination)
+    local_versions = PSSTVersionCollection.from_disk(destination, suppress_warnings=True)
     if version_id in local_versions and local_versions[version_id].files["test"] is not None:
         return local_versions[version_id]
     else:
         try:
             result = psstdata.networking.request("GET", _url("versions.json")).json()
             remote_versions = PSSTVersionCollection.from_object(result, root_dir=destination).apply_dir(destination)
             version = remote_versions.latest() if version_id is None else remote_versions[version_id]
@@ -52,36 +54,56 @@
             psstdata.logger.info(f"Downloaded `{split}` to {version.local_dir()}.")
         except FileExistsError as e:
             psstdata.logger.info(f"Already `{split}` data in directory: {version.local_dir()}, skipping.")
             continue
         except Exception as e:
             raise PSSTDownloadError(split, e) from e
 
-    local_versions = PSSTVersionCollection.from_disk(destination)
+    local_versions = PSSTVersionCollection.from_disk(destination, suppress_warnings=True)
     return local_versions[version.version_id]
 
 
 def _download_split(destination_folder, split: str, url: str):
     split_destination = os.path.join(destination_folder, split)
     if os.path.exists(split_destination):
         raise FileExistsError(split_destination)
 
     incomplete = os.path.join(destination_folder, "incomplete")
 
     with psstdata.networking.request("GET", url, stream=True) as response:
+        content_length = response.raw.length_remaining
         with tarfile.open(fileobj=response.raw, mode="r:gz") as t:
             def itermembers():
                 for tarinfo in t:
+                    _log_progress(content_length, response.raw.length_remaining, split)
                     yield tarinfo
             t.extractall(incomplete, itermembers())
+            _log_progress(content_length, 0, split)
 
     shutil.move(os.path.join(incomplete, split), destination_folder)
+    Path(os.path.join(incomplete, ".DS_Store")).unlink(missing_ok=True)
     os.rmdir(incomplete)
 
 
+def _log_progress(content_length, length_remaining, split):
+    try:
+        percent_complete = 100 * (content_length - length_remaining) / content_length
+        if psstdata.logger.level <= INFO:
+            for logger_handler in psstdata.logger.handlers:
+                logger_handler.stream.flush()
+                logger_handler.stream.write(
+                    f"\rDownloading & extracting `{split}` "
+                    f"({percent_complete:.0f}% complete of {content_length * 1024**-2:.0f}MB)"
+                )
+                if length_remaining == 0:
+                    logger_handler.stream.write("\n")
+    except:
+        pass
+
+
 def _url(path):
     settings = PSSTSettings.load()
     return f"{settings.base_url.rstrip('/')}/{path}"
 
 
 class PSSTDownloadError(Exception):
     def __init__(self, message, inner_error):
```

### Comparing `psstdata-1.0.0/psstdata/loading.py` & `psstdata-1.0.1/psstdata/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,11 +45,11 @@
         tsv_files["test"] = tsv_files["valid"]
         valid_as_test = True
 
     data = {}
     for split, tsv_file in tsv_files.items():
         data[split] = PSSTUtteranceCollection.from_tsv(tsv_file)
 
-    psstdata.logger.info(f"Loaded data version {version.version_id} from {local_dir}")
+    psstdata.logger.info(f"Loaded data version {version.version_id} at {local_dir}")
 
     return cast_dict({**data, "version": version, "test_is_placeholder": valid_as_test}, PSSTData)
```

### Comparing `psstdata-1.0.0/psstdata/networking.py` & `psstdata-1.0.1/psstdata/networking.py`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/tasks.py` & `psstdata-1.0.1/psstdata/tasks.py`

 * *Files identical despite different names*

### Comparing `psstdata-1.0.0/psstdata/versioning.py` & `psstdata-1.0.1/psstdata/versioning.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,21 +68,22 @@
         versions = (cast_dict({**v, "root_dir": root_dir}, PSSTVersion) for v in obj["versions"])
         return cls(
             comment=obj["comment"],
             versions=tuple([v for v in versions if version_filter(v)])
         )
 
     @classmethod
-    def from_disk(cls, dir):
+    def from_disk(cls, dir, suppress_warnings=False):
         def check_version(version: PSSTVersion):
             for split, tsv in version.tsv_files().items():
                 if tsv is None:
                     continue
                 if not os.path.exists(tsv):
-                    psstdata.logger.warning(f"Missing file {tsv}")
+                    if not suppress_warnings:
+                        psstdata.logger.warning(f"Missing file {tsv}")
                     return False
             return True
 
         version_file = os.path.join(dir, "versions.json")
         try:
             with open(version_file) as f:
                 return PSSTVersionCollection.from_object(
```

### Comparing `psstdata-1.0.0/psstdata.egg-info/SOURCES.txt` & `psstdata-1.0.1/psstdata.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 setup.py
 psstdata/__init__.py
+psstdata/__main__.py
 psstdata/_system.py
 psstdata/config.py
 psstdata/consts.py
 psstdata/datastructures.py
 psstdata/downloading.py
 psstdata/loading.py
 psstdata/logs.py
```

### Comparing `psstdata-1.0.0/setup.py` & `psstdata-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name='psstdata',
-    version='1.0.0',
+    version='1.0.1',
     author='Portland Allied Labs for Aphasia Technology (PALAT)',
     author_email='galer@ohsu.edu',
     packages=[
         'psstdata'
     ],
     url='https://github.com/PSST-Challenge/psstdata',
     description='Tool for downloading and loading the data for the PSST Challenge',
```

