# Comparing `tmp/spotify-to-apple-py-0.2.0.tar.gz` & `tmp/spotify-to-apple-py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spotify-to-apple-py-0.2.0.tar", last modified: Wed May 10 22:13:36 2023, max compression
+gzip compressed data, was "spotify-to-apple-py-0.2.1.tar", last modified: Thu May 11 23:25:51 2023, max compression
```

## Comparing `spotify-to-apple-py-0.2.0.tar` & `spotify-to-apple-py-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,45 @@
-drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/
--rw-r--r--   0 bezaamsalu   (501) staff       (20)      265 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/PKG-INFO
-drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/
--rw-r--r--   0 bezaamsalu   (501) staff       (20)      265 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/PKG-INFO
--rw-r--r--   0 bezaamsalu   (501) staff       (20)      180 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/SOURCES.txt
--rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/top_level.txt
--rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/spotify_to_apple_py.egg-info/dependency_links.txt
--rw-r--r--   0 bezaamsalu   (501) staff       (20)      318 2023-05-10 22:13:17.000000 spotify-to-apple-py-0.2.0/setup.py
--rw-r--r--   0 bezaamsalu   (501) staff       (20)       59 2023-05-10 22:13:36.000000 spotify-to-apple-py-0.2.0/setup.cfg
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.385197 spotify-to-apple-py-0.2.1/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     6148 2023-04-05 21:09:58.000000 spotify-to-apple-py-0.2.1/.DS_Store
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.359311 spotify-to-apple-py-0.2.1/.github/
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.360175 spotify-to-apple-py-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      834 2023-02-20 03:14:06.000000 spotify-to-apple-py-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      595 2023-02-20 03:14:06.000000 spotify-to-apple-py-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      118 2023-03-11 03:05:14.000000 spotify-to-apple-py-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.360504 spotify-to-apple-py-0.2.1/.github/workflows/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     1184 2023-03-30 02:11:43.000000 spotify-to-apple-py-0.2.1/.github/workflows/workflow.yml
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     1831 2023-05-11 23:11:56.000000 spotify-to-apple-py-0.2.1/.gitignore
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      429 2023-04-05 21:44:27.000000 spotify-to-apple-py-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     2477 2023-04-05 04:00:07.000000 spotify-to-apple-py-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     1074 2023-02-20 03:14:06.000000 spotify-to-apple-py-0.2.1/LICENSE
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     2123 2023-03-29 22:27:17.000000 spotify-to-apple-py-0.2.1/Makefile
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     7820 2023-05-11 23:25:51.384836 spotify-to-apple-py-0.2.1/PKG-INFO
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     5637 2023-05-11 23:22:23.000000 spotify-to-apple-py-0.2.1/README.md
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        0 2023-03-04 01:32:58.000000 spotify-to-apple-py-0.2.1/__init__.py
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-03-09 00:01:38.000000 spotify-to-apple-py-0.2.1/codecov.yml
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.375554 spotify-to-apple-py-0.2.1/docs/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     6148 2023-04-15 02:45:46.000000 spotify-to-apple-py-0.2.1/docs/.DS_Store
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      634 2023-04-05 05:05:57.000000 spotify-to-apple-py-0.2.1/docs/Makefile
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     1307 2023-04-06 04:02:01.000000 spotify-to-apple-py-0.2.1/docs/conf.py
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     4582 2023-04-06 08:12:20.000000 spotify-to-apple-py-0.2.1/docs/index.rst
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      800 2023-04-05 05:05:57.000000 spotify-to-apple-py-0.2.1/docs/make.bat
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      137 2023-04-06 17:31:49.000000 spotify-to-apple-py-0.2.1/docs/requirements.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20) 11245160 2023-04-15 02:45:46.000000 spotify-to-apple-py-0.2.1/docs/transfer-all.gif
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)  5171798 2023-04-15 02:45:46.000000 spotify-to-apple-py-0.2.1/docs/transfer-single.gif
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     2343 2023-05-11 23:22:29.000000 spotify-to-apple-py-0.2.1/pyproject.toml
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)       95 2023-03-30 02:33:47.000000 spotify-to-apple-py-0.2.1/requirements.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)       38 2023-05-11 23:25:51.385272 spotify-to-apple-py-0.2.1/setup.cfg
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      394 2023-05-11 23:22:29.000000 spotify-to-apple-py-0.2.1/setup.py
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.381843 spotify-to-apple-py-0.2.1/src/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        0 2023-03-04 01:27:49.000000 spotify-to-apple-py-0.2.1/src/__init__.py
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      257 2023-03-30 01:57:29.000000 spotify-to-apple-py-0.2.1/src/apple_private_key.p8
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)    11471 2023-05-11 22:54:15.000000 spotify-to-apple-py-0.2.1/src/spotify_client.py
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.383524 spotify-to-apple-py-0.2.1/src/spotify_to_apple_py.egg-info/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     7820 2023-05-11 23:25:51.000000 spotify-to-apple-py-0.2.1/src/spotify_to_apple_py.egg-info/PKG-INFO
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      783 2023-05-11 23:25:51.000000 spotify-to-apple-py-0.2.1/src/spotify_to_apple_py.egg-info/SOURCES.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        1 2023-05-11 23:25:51.000000 spotify-to-apple-py-0.2.1/src/spotify_to_apple_py.egg-info/dependency_links.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      250 2023-05-11 23:25:51.000000 spotify-to-apple-py-0.2.1/src/spotify_to_apple_py.egg-info/requires.txt
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)       24 2023-05-11 23:25:51.000000 spotify-to-apple-py-0.2.1/src/spotify_to_apple_py.egg-info/top_level.txt
+drwxr-xr-x   0 bezaamsalu   (501) staff       (20)        0 2023-05-11 23:25:51.384444 spotify-to-apple-py-0.2.1/tests/
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)        0 2023-03-04 01:30:31.000000 spotify-to-apple-py-0.2.1/tests/__init__.py
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)      257 2023-04-05 04:19:32.000000 spotify-to-apple-py-0.2.1/tests/sample_apple_private_key.p8
+-rw-r--r--   0 bezaamsalu   (501) staff       (20)     6851 2023-04-05 20:17:55.000000 spotify-to-apple-py-0.2.1/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

