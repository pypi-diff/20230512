# Comparing `tmp/edc-0.4.90.tar.gz` & `tmp/edc-0.4.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.90.tar", last modified: Thu May 11 01:59:39 2023, max compression
+gzip compressed data, was "edc-0.4.91.tar", last modified: Fri May 12 04:49:28 2023, max compression
```

## Comparing `edc-0.4.90.tar` & `edc-0.4.91.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.131280 edc-0.4.90/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.90/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-02-28 00:26:10.000000 edc-0.4.90/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.90/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.90/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    39080 2023-05-11 01:59:31.000000 edc-0.4.90/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.90/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.90/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-11 01:59:39.131382 edc-0.4.90/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.90/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.117739 edc-0.4.90/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.120858 edc-0.4.90/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.90/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.90/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.90/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.121556 edc-0.4.90/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.90/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.90/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.90/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.90/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.122699 edc-0.4.90/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.90/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.126863 edc-0.4.90/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.90/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.90/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.90/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.90/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.90/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.90/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.90/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.90/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.90/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.90/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.90/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.90/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.90/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.90/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.90/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.90/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.90/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.90/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.90/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.127796 edc-0.4.90/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-11 01:59:39.000000 edc-0.4.90/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-11 01:59:39.000000 edc-0.4.90/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-11 01:59:39.000000 edc-0.4.90/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.90/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1922 2023-05-11 01:59:39.000000 edc-0.4.90/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-11 01:59:39.000000 edc-0.4.90/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.127915 edc-0.4.90/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.90/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.90/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.130662 edc-0.4.90/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.90/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.90/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.90/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.90/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.90/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.90/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.90/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.90/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.90/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.90/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.90/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2994 2023-05-11 01:59:39.131797 edc-0.4.90/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-11 01:59:39.131062 edc-0.4.90/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.90/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.90/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.344781 edc-0.4.91/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.91/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.91/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.91/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.91/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    39159 2023-05-12 04:49:20.000000 edc-0.4.91/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.91/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.91/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 04:49:28.344950 edc-0.4.91/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.91/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.326130 edc-0.4.91/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.329265 edc-0.4.91/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.91/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.91/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.91/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.330071 edc-0.4.91/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.91/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.91/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.91/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.91/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.331223 edc-0.4.91/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.338685 edc-0.4.91/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.91/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.91/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.91/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.91/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.91/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.91/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.91/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.91/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.91/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.91/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.91/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.91/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.91/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.91/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.91/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.91/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.91/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.91/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.91/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.339651 edc-0.4.91/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.91/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1922 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.339791 edc-0.4.91/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.91/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.91/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.344022 edc-0.4.91/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.91/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.91/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.91/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.91/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.91/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.91/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.91/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.91/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.91/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.91/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.91/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2994 2023-05-12 04:49:28.345480 edc-0.4.91/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.344472 edc-0.4.91/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.91/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.91/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.90/.gitignore` & `edc-0.4.91/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/.pre-commit-config.yaml` & `edc-0.4.91/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 23.1.0
@@ -38,12 +38,12 @@
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.29.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-0.4.90/CHANGES` & `edc-0.4.91/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 -------
 
+0.4.91
+------
+- add attr for custom identity fields in search (edc-listboard)
+
 0.4.90
 ------
 - add block to add buttons to top_bar (edc-subject-dashboard)
 
 0.4.89
 ------
 - add button to refresh appointments (edc-subject-dashboard)
```

### Comparing `edc-0.4.90/LICENSE` & `edc-0.4.91/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/PKG-INFO` & `edc-0.4.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.90
+Version: 0.4.91
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.90/README.rst` & `edc-0.4.91/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/bin/nginx/edc-uat.conf` & `edc-0.4.91/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/bin/nginx/edc.conf` & `edc-0.4.91/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/bin/scripts/dev_repos.sh` & `edc-0.4.91/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/bin/scripts/update_edc.sh` & `edc-0.4.91/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/bin/systemd/celery-uat.service` & `edc-0.4.91/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/bin/systemd/celery.service` & `edc-0.4.91/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/Makefile` & `edc-0.4.91/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/README.rst` & `edc-0.4.91/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/backup.rst` & `edc-0.4.91/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/celery.rst` & `edc-0.4.91/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/conda.rst` & `edc-0.4.91/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/conf.py` & `edc-0.4.91/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/configure_web_services.rst` & `edc-0.4.91/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/deploy_new_droplet.rst` & `edc-0.4.91/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/exporting_encrypted_data.rst` & `edc-0.4.91/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/forms_reference.md` & `edc-0.4.91/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/landing_page.rst` & `edc-0.4.91/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/make.bat` & `edc-0.4.91/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/prepare_database.rst` & `edc-0.4.91/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/printing.rst` & `edc-0.4.91/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/docs/update_deployment.rst` & `edc-0.4.91/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/edc.egg-info/PKG-INFO` & `edc-0.4.91/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.90
+Version: 0.4.91
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.90/edc.egg-info/SOURCES.txt` & `edc-0.4.91/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/edc.egg-info/requires.txt` & `edc-0.4.91/edc.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 edc-adherence==0.1.20
 edc-adverse-event==0.3.47
 edc-appointment==0.3.70
 edc-auth==0.3.59
 edc-consent==0.3.44
 edc-constants==0.3.46
 edc-crf==0.3.41
-edc-dashboard==0.3.43
+edc-dashboard==0.3.44
 edc-data-manager==0.3.52
 edc-device==0.3.10
 edc-document-status==0.1.3
 edc-dx==0.1.16
 edc-dx-review==0.1.37
 edc-egfr==0.1.10
 edc-export==0.3.25
@@ -49,15 +49,15 @@
 edc-identifier==0.3.22
 edc-lab==0.3.42
 edc-lab-dashboard==0.3.10
 edc-lab-panel==0.1.14
 edc-lab-results==0.1.37
 edc-label==0.3.11
 edc-list-data==0.3.17
-edc-listboard==0.1.7
+edc-listboard==0.1.8
 edc-locator==0.3.22
 edc-ltfu==0.3.22
 edc-metadata==0.3.50
 edc-mnsi==0.1.15
 edc-model==0.3.29
 edc-model-admin==0.3.43
 edc-model-fields==0.3.6
```

### Comparing `edc-0.4.90/image/icon-pycharm.png` & `edc-0.4.91/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/requirements.tests/edc.txt` & `edc-0.4.91/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/requirements.tests/edc_dev.txt` & `edc-0.4.91/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.90/setup.cfg` & `edc-0.4.91/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 	edc-adherence==0.1.20
 	edc-adverse-event==0.3.47
 	edc-appointment==0.3.70
 	edc-auth==0.3.59
 	edc-consent==0.3.44
 	edc-constants==0.3.46
 	edc-crf==0.3.41
-	edc-dashboard==0.3.43
+	edc-dashboard==0.3.44
 	edc-data-manager==0.3.52
 	edc-device==0.3.10
 	edc-document-status==0.1.3
 	edc-dx==0.1.16
 	edc-dx-review==0.1.37
 	edc-egfr==0.1.10
 	edc-export==0.3.25
@@ -78,15 +78,15 @@
 	edc-identifier==0.3.22
 	edc-lab==0.3.42
 	edc-lab-dashboard==0.3.10
 	edc-lab-panel==0.1.14
 	edc-lab-results==0.1.37
 	edc-label==0.3.11
 	edc-list-data==0.3.17
-	edc-listboard==0.1.7
+	edc-listboard==0.1.8
 	edc-locator==0.3.22
 	edc-ltfu==0.3.22
 	edc-metadata==0.3.50
 	edc-mnsi==0.1.15
 	edc-model==0.3.29
 	edc-model-admin==0.3.43
 	edc-model-fields==0.3.6
```

### Comparing `edc-0.4.90/utils/get_edc_requirements.py` & `edc-0.4.91/utils/get_edc_requirements.py`

 * *Files identical despite different names*

