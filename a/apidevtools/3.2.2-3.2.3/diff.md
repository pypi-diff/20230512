# Comparing `tmp/apidevtools-3.2.2.tar.gz` & `tmp/apidevtools-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.2.2.tar", last modified: Mon May  8 01:32:51 2023, max compression
+gzip compressed data, was "apidevtools-3.2.3.tar", last modified: Fri May 12 02:04:18 2023, max compression
```

## Comparing `apidevtools-3.2.2.tar` & `apidevtools-3.2.3.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.476144 apidevtools-3.2.2/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-05-08 01:32:51.475144 apidevtools-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.2/README.md
--rw-rw-rw-   0        0        0     1774 2023-05-08 01:32:36.000000 apidevtools-3.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 01:32:51.476144 apidevtools-3.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.408144 apidevtools-3.2.2/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.411144 apidevtools-3.2.2/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.2/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.2/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.433169 apidevtools-3.2.2/src/apidevtools/media/
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.2/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.2.2/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.2/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.436143 apidevtools-3.2.2/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.2/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.2/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.440143 apidevtools-3.2.2/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.445144 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4793 2023-05-01 17:19:11.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3392 2023-05-08 01:29:46.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6745 2023-05-08 01:31:17.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2087 2023-05-03 02:07:38.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.448143 apidevtools-3.2.2/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/types/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.456143 apidevtools-3.2.2/src/apidevtools/template/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/__init__.py
--rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/create.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.403144 apidevtools-3.2.2/src/apidevtools/template/template/
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.457143 apidevtools-3.2.2/src/apidevtools/template/template/api/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.459152 apidevtools-3.2.2/src/apidevtools/template/template/api/build/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/build/__init__.py
--rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/build/compose.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.462149 apidevtools-3.2.2/src/apidevtools/template/template/api/src/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/app.py
--rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/const.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.466143 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/
--rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/auth.py
--rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/item.py
--rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/user.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.470158 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/
--rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/auth.py
--rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/item.py
--rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/user.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.474144 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/
--rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/__init__.py
--rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/item.py
--rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/user.py
--rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template.zip
--rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.2/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.430143 apidevtools-3.2.2/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.706202 apidevtools-3.2.3/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-05-12 02:04:18.705201 apidevtools-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.3/README.md
+-rw-rw-rw-   0        0        0     1795 2023-05-12 01:54:56.000000 apidevtools-3.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 02:04:18.706202 apidevtools-3.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.645202 apidevtools-3.2.3/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.649221 apidevtools-3.2.3/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.3/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.3/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.668237 apidevtools-3.2.3/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.2.3/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.3/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     4114 2023-05-12 01:53:42.000000 apidevtools-3.2.3/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.3/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.672203 apidevtools-3.2.3/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.3/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.3/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.675202 apidevtools-3.2.3/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.681202 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4793 2023-05-01 17:19:11.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3392 2023-05-08 01:29:46.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6745 2023-05-08 01:31:17.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2087 2023-05-03 02:07:38.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.684203 apidevtools-3.2.3/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/types/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.687210 apidevtools-3.2.3/src/apidevtools/template/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/create.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.640202 apidevtools-3.2.3/src/apidevtools/template/template/
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.689206 apidevtools-3.2.3/src/apidevtools/template/template/api/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.690203 apidevtools-3.2.3/src/apidevtools/template/template/api/build/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/build/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/build/compose.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.693201 apidevtools-3.2.3/src/apidevtools/template/template/api/src/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/app.py
+-rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/const.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.698212 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/
+-rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/__init__.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/auth.py
+-rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/item.py
+-rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/user.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.702215 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/
+-rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/auth.py
+-rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/item.py
+-rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/user.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.704213 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/
+-rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/__init__.py
+-rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/item.py
+-rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/user.py
+-rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template.zip
+-rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.3/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.664202 apidevtools-3.2.3/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.2.2/LICENSE.txt` & `apidevtools-3.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/PKG-INFO` & `apidevtools-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.2
+Version: 3.2.3
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.2/README.md` & `apidevtools-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/pyproject.toml` & `apidevtools-3.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.2.2"
+version = "3.2.3"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
@@ -57,14 +57,14 @@
 #    "ujson~=5.7.0",
 #    "aiodns~=3.0.0",
 #    "cchardet~=2.1.7",
 #    "uvloop~=0.17.0"
 ]
 
 [tool.setuptools.package-data]
-apidevtools = ["template/template.zip"]
+apidevtools = ["template/template.zip", "media/ARIALNB.TTF"]
 
 [project.urls]
 "Homepage" = "https://github.com/cxllmerichie/apidevtools"
 "Bug Tracker" = "https://github.com/cxllmerichie/apidevtools/issues"
 "Repository" = "https://github.com/cxllmerichie/apidevtools"
 "Documentation" = "https://github.com/cxllmerichie/apidevtools/README.md"
```

### Comparing `apidevtools-3.2.2/src/apidevtools/logman.py` & `apidevtools-3.2.3/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/media/imgproc.py` & `apidevtools-3.2.3/src/apidevtools/media/imgproc.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,53 +46,59 @@
         return output
 
     async def url(self) -> str | None:
         from . import telegraph
 
         return await telegraph.upload(self.bytesio)
 
-
-class Font:
-    @staticmethod
-    def system() -> list[str]:
-        """
-        Get a list of system fonts
-        :return:
-        """
-        if _os.name != 'nt':
-            raise OSError('System fonts are available only for Windows. Please wait for an update.')
-        paths = _pathlib.PurePath(_pathlib.Path.home().drive, _os.sep, 'windows', 'fonts')
-        return [str(path.absolute()) for path in list(_pathlib.Path(paths).glob('*.ttf'))]
-
-    @staticmethod
-    def font(ttf_name: str) -> str:
-        """
-        Find a system font by its name, if not found returns ARIALNB by default
-        :param ttf_name:
-        :return:
-        """
-        # try the similarity approach https://www.geeksforgeeks.org/python-word-similarity-using-spacy/
-        ttf = list(filter(lambda filepath: _os.path.basename(filepath).split('.')[0] == ttf_name, Font.system()))
-        return ttf[0] if len(ttf) else Font.font('ARIALNB')
+#
+# class Font:
+#     @staticmethod
+#     def system() -> list[str]:
+#         """
+#         Get a list of system fonts
+#         :return:
+#         """
+#         if _os.name != 'nt':
+#             raise OSError('System fonts are available only for Windows. Please wait for an update.')
+#         paths = _pathlib.PurePath(_pathlib.Path.home().drive, _os.sep, 'windows', 'fonts')
+#         return [str(path.absolute()) for path in list(_pathlib.Path(paths).glob('*.ttf'))]
+#
+#     @staticmethod
+#     def font(ttf_name: str) -> str:
+#         """
+#         Find a system font by its name, if not found returns ARIALNB by default
+#         :param ttf_name:
+#         :return:
+#         """
+#         # try the similarity approach https://www.geeksforgeeks.org/python-word-similarity-using-spacy/
+#         ttf = list(filter(lambda filepath: _os.path.basename(filepath).split('.')[0] == ttf_name, Font.system()))
+#         return ttf[0] if len(ttf) else Font.font('ARIALNB')
 
 
 def generate(
-        text: str = Image.text, size: int = 512, fonttf=Font.font('ARIALNB'),
+        # text: str = Image.text, size: int = 512, fonttf=Font.font('ARIALNB'),
+        text: str = Image.text, size: int = 512, fonttf=None,
         bg_color: tuple[int, int, int] = (0, 0, 0), font_color: tuple[int, int, int] = (255, 255, 255)
 ) -> Image:
     """
     Generate image from apidevtools.image.Image. Supposed to be used as for instance: user
     By default has "N/A" white text on the black background.
     :param text:
     :param size:
     :param fonttf:
     :param bg_color:
     :param font_color:
     :return:
     """
+    if not fonttf:
+        from site import getsitepackages
+
+        fonttf = _os.path.join(getsitepackages()[1], 'apidevtools', 'media', 'ARIALNB.TTF')
+
     font = _ImageFont.truetype(font=fonttf, size=int(size * 0.6))
     img = PIL.Image.new(mode='RGB', size=(size, size), color=bg_color)
     draw = _ImageDraw.Draw(img)
     _, _, width, height = draw.textbbox((0, 0), text, font=font)
     draw.text(xy=((size - width) / 2, (size - height) / 3), text=text, font=font, fill=font_color)
     return Image(img, text)
```

### Comparing `apidevtools-3.2.2/src/apidevtools/media/telegraph.py` & `apidevtools-3.2.3/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/security/encryptor.py` & `apidevtools-3.2.3/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/security/hasher.py` & `apidevtools-3.2.3/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.2.3/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/create.py` & `apidevtools-3.2.3/src/apidevtools/template/create.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/app.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/app.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/const.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/const.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/auth.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/item.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/user.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/auth.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/item.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/user.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/user.py` & `apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/template/template.zip` & `apidevtools-3.2.3/src/apidevtools/template/template.zip`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools/utils.py` & `apidevtools-3.2.3/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.2/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.2.3/src/apidevtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.2
+Version: 3.2.3
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.2/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.2.3/src/apidevtools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/apidevtools/logman.py
 src/apidevtools/utils.py
 src/apidevtools.egg-info/PKG-INFO
 src/apidevtools.egg-info/SOURCES.txt
 src/apidevtools.egg-info/dependency_links.txt
 src/apidevtools.egg-info/requires.txt
 src/apidevtools.egg-info/top_level.txt
+src/apidevtools/media/ARIALNB.TTF
 src/apidevtools/media/__init__.py
 src/apidevtools/media/imgproc.py
 src/apidevtools/media/telegraph.py
 src/apidevtools/security/__init__.py
 src/apidevtools/security/encryptor.py
 src/apidevtools/security/hasher.py
 src/apidevtools/simpleorm/__init__.py
```

