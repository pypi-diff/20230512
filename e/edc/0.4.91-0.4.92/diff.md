# Comparing `tmp/edc-0.4.91.tar.gz` & `tmp/edc-0.4.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.91.tar", last modified: Fri May 12 04:49:28 2023, max compression
+gzip compressed data, was "edc-0.4.92.tar", last modified: Fri May 12 17:56:07 2023, max compression
```

## Comparing `edc-0.4.91.tar` & `edc-0.4.92.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.344781 edc-0.4.91/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.91/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.91/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.91/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.91/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    39159 2023-05-12 04:49:20.000000 edc-0.4.91/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.91/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.91/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 04:49:28.344950 edc-0.4.91/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.91/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.326130 edc-0.4.91/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.329265 edc-0.4.91/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.91/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.91/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.91/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.330071 edc-0.4.91/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.91/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.91/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.91/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.91/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.331223 edc-0.4.91/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.91/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.338685 edc-0.4.91/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.91/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.91/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.91/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.91/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.91/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.91/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.91/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.91/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.91/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.91/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.91/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.91/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.91/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.91/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.91/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.91/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.91/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.91/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.91/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.339651 edc-0.4.91/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.91/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1922 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-12 04:49:28.000000 edc-0.4.91/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.339791 edc-0.4.91/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.91/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.91/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.344022 edc-0.4.91/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.91/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.91/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.91/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.91/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.91/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.91/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.91/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.91/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.91/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.91/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.91/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2994 2023-05-12 04:49:28.345480 edc-0.4.91/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:49:28.344472 edc-0.4.91/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.91/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.91/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.095125 edc-0.4.92/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.92/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.92/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.92/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.92/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    39242 2023-05-12 17:55:59.000000 edc-0.4.92/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.92/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.92/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 17:56:07.095229 edc-0.4.92/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.92/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.081873 edc-0.4.92/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.084725 edc-0.4.92/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.92/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.92/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.92/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.085376 edc-0.4.92/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.92/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.92/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.92/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.92/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.086547 edc-0.4.92/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.090528 edc-0.4.92/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.92/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.92/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.92/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.92/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.92/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.92/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.92/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.92/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.92/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.92/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.92/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.92/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.92/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.92/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.92/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.92/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.92/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.92/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.92/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.091517 edc-0.4.92/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.92/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1922 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.091645 edc-0.4.92/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.92/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.92/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.094533 edc-0.4.92/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.92/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.92/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.92/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.92/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.92/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.92/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.92/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.92/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.92/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.92/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.92/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2994 2023-05-12 17:56:07.095650 edc-0.4.92/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.094892 edc-0.4.92/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.92/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.92/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.91/.gitignore` & `edc-0.4.92/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/.pre-commit-config.yaml` & `edc-0.4.92/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/CHANGES` & `edc-0.4.92/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 -------
 
+0.4.92
+------
+- override methods for url and message in validator (edc-screening)
+
 0.4.91
 ------
 - add attr for custom identity fields in search (edc-listboard)
 
 0.4.90
 ------
 - add block to add buttons to top_bar (edc-subject-dashboard)
```

### Comparing `edc-0.4.91/LICENSE` & `edc-0.4.92/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/PKG-INFO` & `edc-0.4.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.91
+Version: 0.4.92
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.91/README.rst` & `edc-0.4.92/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/bin/nginx/edc-uat.conf` & `edc-0.4.92/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/bin/nginx/edc.conf` & `edc-0.4.92/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/bin/scripts/dev_repos.sh` & `edc-0.4.92/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/bin/scripts/update_edc.sh` & `edc-0.4.92/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/bin/systemd/celery-uat.service` & `edc-0.4.92/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/bin/systemd/celery.service` & `edc-0.4.92/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/Makefile` & `edc-0.4.92/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/README.rst` & `edc-0.4.92/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/backup.rst` & `edc-0.4.92/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/celery.rst` & `edc-0.4.92/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/conda.rst` & `edc-0.4.92/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/conf.py` & `edc-0.4.92/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/configure_web_services.rst` & `edc-0.4.92/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/deploy_new_droplet.rst` & `edc-0.4.92/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/exporting_encrypted_data.rst` & `edc-0.4.92/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/forms_reference.md` & `edc-0.4.92/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/landing_page.rst` & `edc-0.4.92/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/make.bat` & `edc-0.4.92/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/prepare_database.rst` & `edc-0.4.92/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/printing.rst` & `edc-0.4.92/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/docs/update_deployment.rst` & `edc-0.4.92/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/edc.egg-info/PKG-INFO` & `edc-0.4.92/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.91
+Version: 0.4.92
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.91/edc.egg-info/SOURCES.txt` & `edc-0.4.92/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/edc.egg-info/requires.txt` & `edc-0.4.92/edc.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 edc-randomization==0.3.45
 edc-reference==0.3.14
 edc-refusal==0.1.10
 edc-registration==0.3.26
 edc-reportable==0.3.30
 edc-review-dashboard==0.3.18
 edc-rx==0.1.5
-edc-screening==0.3.31
+edc-screening==0.3.32
 edc-search==0.3.6
 edc-sites==0.3.19
 edc-subject-dashboard==0.3.34
 edc-subject-model-wrappers==0.3.13
 edc-timepoint==0.3.10
 edc-transfer==0.3.13
 edc-unblinding==0.1.13
```

### Comparing `edc-0.4.91/image/icon-pycharm.png` & `edc-0.4.92/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/requirements.tests/edc.txt` & `edc-0.4.92/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/requirements.tests/edc_dev.txt` & `edc-0.4.92/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.91/setup.cfg` & `edc-0.4.92/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 	edc-randomization==0.3.45
 	edc-reference==0.3.14
 	edc-refusal==0.1.10
 	edc-registration==0.3.26
 	edc-reportable==0.3.30
 	edc-review-dashboard==0.3.18
 	edc-rx==0.1.5
-	edc-screening==0.3.31
+	edc-screening==0.3.32
 	edc-search==0.3.6
 	edc-sites==0.3.19
 	edc-subject-dashboard==0.3.34
 	edc-subject-model-wrappers==0.3.13
 	edc-timepoint==0.3.10
 	edc-transfer==0.3.13
 	edc-unblinding==0.1.13
```

### Comparing `edc-0.4.91/utils/get_edc_requirements.py` & `edc-0.4.92/utils/get_edc_requirements.py`

 * *Files identical despite different names*

