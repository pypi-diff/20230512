# Comparing `tmp/snews_pt-1.3.2.tar.gz` & `tmp/snews_pt-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/bj7780/Desktop/Kara/GitHub/SNEWS/SNEWS_Publishing_Tools/dist/.tmp-kc52we8s/snews_pt-1.3.2.tar", last modified: Fri Apr 21 11:57:32 2023, max compression
+gzip compressed data, was "/mnt/c/Users/bj7780/Desktop/Kara/GitHub/SNEWS/SNEWS_Publishing_Tools/dist/.tmp-0pipga2x/snews_pt-1.3.3.tar", last modified: Fri May 12 08:19:34 2023, max compression
```

## Comparing `snews_pt-1.3.2.tar` & `snews_pt-1.3.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/.github/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/.github/workflows/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac10-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac10-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1877 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac11-py310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac11-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac11-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1817 2022-07-29 18:24:09.000000 snews_pt-1.3.2/.github/workflows/mac11-py39.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2367 2023-02-06 12:44:04.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2135 2023-02-06 12:44:04.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py37-310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2090 2023-02-06 12:44:04.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py39.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      178 2022-05-20 14:39:26.000000 snews_pt-1.3.2/.readthedocs.yaml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      436 2023-04-21 11:57:26.000000 snews_pt-1.3.2/AUTHORS
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    16863 2023-04-21 11:57:25.000000 snews_pt-1.3.2/ChangeLog
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-04-21 11:57:32.000000 snews_pt-1.3.2/PKG-INFO
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9034 2022-09-27 15:09:46.000000 snews_pt-1.3.2/README.md
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/docs/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      623 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/Makefile
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      205 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/README.md
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/docs/_static/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/_static/css/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/_static/css/my_theme.css
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/_templates/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       60 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/_templates/layout.html
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/api/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      148 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/api/api.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      129 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/message_schema.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/snews_pt_utils.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      111 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/snews_pub.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      114 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/snews_sub.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6080 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/cli_docs.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      535 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/cli_help.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4472 2022-09-27 15:04:20.000000 snews_pt-1.3.2/docs/conf.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   139863 2022-04-28 07:02:44.000000 snews_pt-1.3.2/docs/custom_logo.png
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      408 2022-09-27 15:01:02.000000 snews_pt-1.3.2/docs/index.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    17706 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/snews_logo.png
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1107 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/subscribed_messages.json
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/user/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      258 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/user/architecture.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5119 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/user/command_line_interface.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4242 2022-09-29 07:36:14.000000 snews_pt-1.3.2/docs/user/firedrills.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      840 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/user/installation.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1603 2023-03-30 14:38:00.000000 snews_pt-1.3.2/docs/user/message_schema.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1259 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/user/protocol.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1258 2023-03-30 14:38:00.000000 snews_pt-1.3.2/docs/user/publishing_protocols.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     8746 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/user/quickstart.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4786 2022-12-01 10:17:24.000000 snews_pt-1.3.2/examples.ipynb
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    19290 2023-03-30 14:38:00.000000 snews_pt-1.3.2/firedrill.ipynb
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   108013 2022-05-20 12:43:49.000000 snews_pt-1.3.2/img.png
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/logs/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        2 2022-08-01 20:52:31.000000 snews_pt-1.3.2/logs/.gitignore
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      440 2023-04-21 11:47:54.000000 snews_pt-1.3.2/requirements.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      169 2023-04-21 11:57:32.000000 snews_pt-1.3.2/setup.cfg
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2419 2023-03-30 14:38:00.000000 snews_pt-1.3.2/setup.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/snews_pt/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      747 2022-09-27 12:03:30.000000 snews_pt-1.3.2/snews_pt/__init__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9762 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/__main__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       19 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/_version.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/snews_pt/auxiliary/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1523 2022-05-20 13:27:18.000000 snews_pt-1.3.2/snews_pt/auxiliary/custom_script.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1565 2022-11-18 16:58:48.000000 snews_pt-1.3.2/snews_pt/auxiliary/detector_properties.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2435 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/auxiliary/make_scenarios.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3543 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/auxiliary/scenarios.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/auxiliary/test-config.env
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2267 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/auxiliary/try_scenarios.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/snews_pt/core/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2022-09-27 12:03:31.000000 snews_pt-1.3.2/snews_pt/core/__init__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1314 2022-09-27 12:03:31.000000 snews_pt-1.3.2/snews_pt/core/logging.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4011 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/message_schema.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6196 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/remote_commands.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9366 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_format_checker.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    11921 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_pt_utils.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9081 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_pub.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5042 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_sub.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/snews_pt/test/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      272 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_coincidence_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      483 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_combined_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      182 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_heartbeat_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      318 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_significance_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      328 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_timing_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1161 2022-05-20 13:27:19.000000 snews_pt-1.3.2/snews_pt/test/random_plugin.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1689 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/test/test_coincidence_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      239 2022-05-20 13:27:19.000000 snews_pt-1.3.2/snews_pt/test/test_install.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1705 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/test_old_crashes.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      842 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/test_plugin.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1288 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/test/test_retraction.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2384 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/test/test_significance_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      643 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/test_subscribe.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1820 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/test/test_timing_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3880 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/tier_decider.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/snews_pt.egg-info/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/PKG-INFO
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2398 2023-04-21 11:57:30.000000 snews_pt-1.3.2/snews_pt.egg-info/SOURCES.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/dependency_links.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       52 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/entry_points.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2022-05-20 13:36:30.000000 snews_pt-1.3.2/snews_pt.egg-info/not-zip-safe
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       47 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/pbr.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      417 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/requires.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        9 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/top_level.txt
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:34.000000 snews_pt-1.3.3/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:31.000000 snews_pt-1.3.3/.github/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/.github/workflows/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac10-py37.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac10-py38.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1877 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac11-py310.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac11-py37.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.3/.github/workflows/mac11-py38.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1817 2022-07-29 18:24:09.000000 snews_pt-1.3.3/.github/workflows/mac11-py39.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2367 2023-02-06 12:44:04.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py310.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2135 2023-02-06 12:44:04.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py37-310.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py37.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py38.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2090 2023-02-06 12:44:04.000000 snews_pt-1.3.3/.github/workflows/ubuntu20-py39.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      178 2022-05-20 14:39:26.000000 snews_pt-1.3.3/.readthedocs.yaml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      436 2023-05-12 08:19:27.000000 snews_pt-1.3.3/AUTHORS
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    16952 2023-05-12 08:19:26.000000 snews_pt-1.3.3/ChangeLog
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-05-12 08:19:34.000000 snews_pt-1.3.3/PKG-INFO
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9034 2022-09-27 15:09:46.000000 snews_pt-1.3.3/README.md
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      623 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/Makefile
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      205 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/README.md
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:31.000000 snews_pt-1.3.3/docs/_static/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/_static/css/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/_static/css/my_theme.css
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/_templates/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       60 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/_templates/layout.html
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/api/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      148 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/api/api.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      129 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/message_schema.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/snews_pt_utils.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      111 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/snews_pub.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      114 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/api/snews_sub.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6080 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/cli_docs.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      535 2022-05-20 12:43:48.000000 snews_pt-1.3.3/docs/cli_help.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4472 2022-09-27 15:04:20.000000 snews_pt-1.3.3/docs/conf.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   139863 2022-04-28 07:02:44.000000 snews_pt-1.3.3/docs/custom_logo.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      408 2022-09-27 15:01:02.000000 snews_pt-1.3.3/docs/index.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    17706 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/snews_logo.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1107 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/subscribed_messages.json
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/docs/user/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      258 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/user/architecture.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5119 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/user/command_line_interface.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4242 2022-09-29 07:36:14.000000 snews_pt-1.3.3/docs/user/firedrills.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      840 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/user/installation.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1603 2023-03-30 14:38:00.000000 snews_pt-1.3.3/docs/user/message_schema.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1259 2022-05-20 12:43:49.000000 snews_pt-1.3.3/docs/user/protocol.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1258 2023-03-30 14:38:00.000000 snews_pt-1.3.3/docs/user/publishing_protocols.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     8746 2022-05-20 13:27:18.000000 snews_pt-1.3.3/docs/user/quickstart.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4786 2022-12-01 10:17:24.000000 snews_pt-1.3.3/examples.ipynb
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    34654 2023-05-08 14:52:18.000000 snews_pt-1.3.3/firedrill.ipynb
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   108013 2022-05-20 12:43:49.000000 snews_pt-1.3.3/img.png
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:32.000000 snews_pt-1.3.3/logs/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        2 2022-08-01 20:52:31.000000 snews_pt-1.3.3/logs/.gitignore
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      440 2023-04-21 11:47:54.000000 snews_pt-1.3.3/requirements.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      169 2023-05-12 08:19:34.000000 snews_pt-1.3.3/setup.cfg
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2419 2023-03-30 14:38:00.000000 snews_pt-1.3.3/setup.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      747 2022-09-27 12:03:30.000000 snews_pt-1.3.3/snews_pt/__init__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9898 2023-05-08 13:02:05.000000 snews_pt-1.3.3/snews_pt/__main__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       19 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/_version.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt/auxiliary/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1523 2022-05-20 13:27:18.000000 snews_pt-1.3.3/snews_pt/auxiliary/custom_script.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1565 2022-11-18 16:58:48.000000 snews_pt-1.3.3/snews_pt/auxiliary/detector_properties.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2435 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/auxiliary/make_scenarios.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3543 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/auxiliary/scenarios.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      619 2023-05-08 13:02:06.000000 snews_pt-1.3.3/snews_pt/auxiliary/test-config.env
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2267 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/auxiliary/try_scenarios.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt/core/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2022-09-27 12:03:31.000000 snews_pt-1.3.3/snews_pt/core/__init__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1314 2022-09-27 12:03:31.000000 snews_pt-1.3.3/snews_pt/core/logging.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4011 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/message_schema.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6361 2023-05-08 13:02:05.000000 snews_pt-1.3.3/snews_pt/remote_commands.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9366 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_format_checker.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    11921 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_pt_utils.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9081 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_pub.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5042 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/snews_sub.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:34.000000 snews_pt-1.3.3/snews_pt/test/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      272 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_coincidence_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      483 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_combined_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      182 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_heartbeat_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      318 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_significance_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      328 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/example_timing_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1161 2022-05-20 13:27:19.000000 snews_pt-1.3.3/snews_pt/test/random_plugin.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1689 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/test/test_coincidence_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      239 2022-05-20 13:27:19.000000 snews_pt-1.3.3/snews_pt/test/test_install.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1705 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/test_old_crashes.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      842 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/test_plugin.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1288 2023-03-30 14:38:00.000000 snews_pt-1.3.3/snews_pt/test/test_retraction.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2384 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/test/test_significance_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      643 2022-11-18 16:58:49.000000 snews_pt-1.3.3/snews_pt/test/test_subscribe.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1820 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/test/test_timing_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3880 2023-04-21 11:47:54.000000 snews_pt-1.3.3/snews_pt/tier_decider.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-05-12 08:19:33.000000 snews_pt-1.3.3/snews_pt.egg-info/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/PKG-INFO
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2398 2023-05-12 08:19:31.000000 snews_pt-1.3.3/snews_pt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       52 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/entry_points.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2022-05-20 13:36:30.000000 snews_pt-1.3.3/snews_pt.egg-info/not-zip-safe
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       47 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/pbr.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      417 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/requires.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        9 2023-05-12 08:19:27.000000 snews_pt-1.3.3/snews_pt.egg-info/top_level.txt
```

### Comparing `snews_pt-1.3.2/.github/workflows/mac10-py37.yml` & `snews_pt-1.3.3/.github/workflows/mac10-py37.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/mac10-py38.yml` & `snews_pt-1.3.3/.github/workflows/mac10-py38.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/mac11-py310.yml` & `snews_pt-1.3.3/.github/workflows/mac11-py310.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/mac11-py37.yml` & `snews_pt-1.3.3/.github/workflows/mac11-py37.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/mac11-py38.yml` & `snews_pt-1.3.3/.github/workflows/mac11-py38.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/mac11-py39.yml` & `snews_pt-1.3.3/.github/workflows/mac11-py39.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/ubuntu20-py310.yml` & `snews_pt-1.3.3/.github/workflows/ubuntu20-py310.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/ubuntu20-py37-310.yml` & `snews_pt-1.3.3/.github/workflows/ubuntu20-py37-310.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/ubuntu20-py37.yml` & `snews_pt-1.3.3/.github/workflows/ubuntu20-py37.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/ubuntu20-py38.yml` & `snews_pt-1.3.3/.github/workflows/ubuntu20-py38.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/.github/workflows/ubuntu20-py39.yml` & `snews_pt-1.3.3/.github/workflows/ubuntu20-py39.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/ChangeLog` & `snews_pt-1.3.3/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+v1.3.3
+------
+
+* fix docstring
+* add doc
+* add patience
+* update notebook
+* fix testing
+
 v1.3.2
 ------
 
 * Update snews\_sub.py
 * add correct topic
 * add correct topic
 * add write hb logs command
```

### Comparing `snews_pt-1.3.2/PKG-INFO` & `snews_pt-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snews_pt
-Version: 1.3.2
+Version: 1.3.3
 Summary: An alert application for observing supernovas.
 Home-page: https://github.com/SNEWS2/SNEWS_Publishing_Tools
 Author: Sebastian Torres-Lara, Melih Kara
 Author-email: sebastiantorreslara17@gmail.com, karamel.itu@gmail.com
 License: BSD 3-Clause
 Keywords: setup,distutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snews_pt-1.3.2/README.md` & `snews_pt-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/Makefile` & `snews_pt-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/_static/css/my_theme.css` & `snews_pt-1.3.3/docs/_static/css/my_theme.css`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/cli_docs.md` & `snews_pt-1.3.3/docs/cli_docs.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/cli_help.txt` & `snews_pt-1.3.3/docs/cli_help.txt`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/conf.py` & `snews_pt-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/custom_logo.png` & `snews_pt-1.3.3/docs/custom_logo.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/snews_logo.png` & `snews_pt-1.3.3/docs/snews_logo.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/subscribed_messages.json` & `snews_pt-1.3.3/docs/subscribed_messages.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/command_line_interface.md` & `snews_pt-1.3.3/docs/user/command_line_interface.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/firedrills.md` & `snews_pt-1.3.3/docs/user/firedrills.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/installation.rst` & `snews_pt-1.3.3/docs/user/installation.rst`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/message_schema.md` & `snews_pt-1.3.3/docs/user/message_schema.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/protocol.rst` & `snews_pt-1.3.3/docs/user/protocol.rst`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/publishing_protocols.md` & `snews_pt-1.3.3/docs/user/publishing_protocols.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/docs/user/quickstart.md` & `snews_pt-1.3.3/docs/user/quickstart.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/examples.ipynb` & `snews_pt-1.3.3/examples.ipynb`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/img.png` & `snews_pt-1.3.3/img.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/setup.py` & `snews_pt-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/__init__.py` & `snews_pt-1.3.3/snews_pt/__init__.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/__main__.py` & `snews_pt-1.3.3/snews_pt/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,27 +163,27 @@
     from .snews_pt_utils import set_name as _set_name
     _set_name(name)
     click.secho(f"Your detector name is set to be: {os.environ['DETECTOR_NAME']}", fg='green', bold=True)
 
 ###################### Remote Commands
 @main.command()
 @click.option('--firedrill/--no-firedrill', default=True, show_default='True', help='Whether to use firedrill brokers or default ones')
-@click.option('--start_at', '-s', type=int, default=-5)
-@click.option('--wait', '-w', type=int, default=10)
+@click.option('--start_at', '-s', type=str, default="LATEST", help='either LATEST or EARLIEST')
+@click.option('--patience', '-p', type=int, default=8)
 @click.pass_context
-def test_connection(ctx, firedrill, start_at, wait):
+def test_connection(ctx, firedrill, start_at, patience):
     """ test the server connection
-        It should prompt your whether the
-        coincidence script is running in the server
-        :param start_at: `negative int` the last N number of msg to check
-        :param wait: `int` seconds to wait before terminating the check
+        It should prompt your whether the coincidence script is running in the server
+        :param start_at: `str` Where to start looking for the confirmation LATEST or EARLIEST
+        :param patience: `int` seconds to wait before the check
+            Sometime, it takes time for server to respond, increase patience
     """
     from .remote_commands import test_connection
     test_connection(detector_name=ctx.obj['DETECTOR_NAME'],
-                    firedrill=firedrill, start_at=start_at, wait=wait)
+                    firedrill=firedrill, start_at=start_at, patience=patience)
 
 
 @main.command()
 @click.option('--firedrill/--no-firedrill', default=True, show_default='True', help='Whether to use firedrill brokers or default ones')
 @click.pass_context
 def write_hb_logs(ctx, firedrill):
     """ REQUIRES AUTHORIZATION
```

### Comparing `snews_pt-1.3.2/snews_pt/auxiliary/custom_script.py` & `snews_pt-1.3.3/snews_pt/auxiliary/custom_script.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/auxiliary/detector_properties.json` & `snews_pt-1.3.3/snews_pt/auxiliary/detector_properties.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/auxiliary/make_scenarios.py` & `snews_pt-1.3.3/snews_pt/auxiliary/make_scenarios.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/auxiliary/scenarios.json` & `snews_pt-1.3.3/snews_pt/auxiliary/scenarios.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/auxiliary/test-config.env` & `snews_pt-1.3.3/snews_pt/auxiliary/test-config.env`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-DETECTOR_NAME='TEST'
-HAS_NAME_CHANGED='0'
+DETECTOR_NAME='XENONnT'
+HAS_NAME_CHANGED='1'
 ADMIN_PASS='very1secret2password'
 
 DATABASE_SERVER=""
 LOCAL_SERVER="mongodb://localhost:27017"
 ALERT_OUTPUT="SNEWS_ALERTS/"
 
 NEW_DATABASE=0
```

### Comparing `snews_pt-1.3.2/snews_pt/auxiliary/try_scenarios.py` & `snews_pt-1.3.3/snews_pt/auxiliary/try_scenarios.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/core/logging.py` & `snews_pt-1.3.3/snews_pt/core/logging.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/message_schema.py` & `snews_pt-1.3.3/snews_pt/message_schema.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/remote_commands.py` & `snews_pt-1.3.3/snews_pt/remote_commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Easy handle remote commands
 
 
 Melih Kara, kara@kit.edu
 """
+import time
 
 from hop import Stream
+from hop.models import JSONBlob
+from hop.io import StartPosition
 from datetime import datetime, timedelta
 import os, click
 
-def test_connection(detector_name=None, firedrill=True, start_at=-5, wait=10):
+def test_connection(detector_name=None, firedrill=True, start_at="LATEST", patience=8):
     """ test the server connection
         It should prompt your whether the
         coincidence script is running in the server
-        :param start_at: `negative int` the last N number of msg to check
-        :param wait: `int` seconds to wait before terminating the check
+        :param start_at: "LATEST" or "EARLIEST"
+        :param patience: `int` seconds to wait before the check
     """
     detector_name = detector_name or os.getenv("DETECTOR_NAME")
     default_connection_topic = "kafka://kafka.scimma.org/snews.connection-testing"
     connection_broker = os.getenv("CONNECTION_TEST_TOPIC", default_connection_topic)
     stamp_time = datetime.utcnow().isoformat()
     message = {'_id': '0_test-connection',
                'detector_name': detector_name,
@@ -26,39 +29,43 @@
                'status': 'sending',
                'meta':{}}
     if firedrill:
         topic = os.getenv("FIREDRILL_OBSERVATION_TOPIC")
     else:
         topic = os.getenv("OBSERVATION_TOPIC")
 
-    # substream = Stream(until_eos=False, auth=True, start_at=start_at) # when False, while loop doesn't break
-    substream = Stream(until_eos=True, auth=True, start_at=start_at)
+    _start_at = StartPosition.LATEST if start_at=="LATEST" else StartPosition.EARLIEST
+    substream = Stream(until_eos=True, auth=True, start_at=_start_at)
     pubstream = Stream(until_eos=True, auth=True)
     click.secho(f"\n> Testing your connection.\n> Sending to {topic}\n"
-                f"> Expecting from {connection_broker}. \n> Should take ~{wait} seconds...\n")
+                f"> Expecting from {connection_broker}. \n"
+                f"> Going to wait {patience} seconds before checking for confirmation...\n")
 
-    start_time = datetime.utcnow()
+    # start_time = datetime.utcnow()
     confirmed = False
-    # with pubstream.open(topic, "w") as ps, substream.open(topic, "r") as ss:
+    message_expected = message.copy()
+    message_expected["status"] = "received"
+
     with pubstream.open(topic, "w") as ps, substream.open(connection_broker, "r") as ss:
-        ps.write(message)
-        while (datetime.utcnow() - start_time) < timedelta(seconds=wait):
-            for read in ss:
-                message_expected = message.copy()
-                message_expected["status"] = "received"
-                if read == message_expected:
-                    read_name = click.style(read['detector_name'], fg='green', bold=True)
-                    read_time = click.style(read['time'], fg='green', bold=True)
-                    click.echo(f"You ({read_name}) have a connection to the server at {read_time}")
-                    confirmed=True
-                    break
+        ps.write(JSONBlob(message))
+        # while (datetime.utcnow() - start_time) < timedelta(seconds=wait):
+        time.sleep(patience)
+        for read in ss:
+            read = read.content
+            if read == message_expected:
+                read_name = click.style(read['detector_name'], fg='green', bold=True)
+                read_time = click.style(read['time'], fg='green', bold=True)
+                click.echo(f"You ({read_name}) have a connection to the server at {read_time}")
+                confirmed=True
                 break
-            break
+            else: # if there is no else: continue statement, it does not work
+                continue
     if not confirmed:
-        click.secho(f"\tCouldn't get a confirmation in {wait} sec. "
+        click.secho(f"\tWaited for {patience} sec and checked from {start_at},"
+                    f" couldn't get a confirmation"
                     f"\n\tMaybe increase timeout and try again.", fg='red', bold=True)
 
 
 def write_hb_logs(detector_name=None, admin_pass=None, firedrill=True):
     """ REQUIRES AUTHORIZATION
         ask to print the HB logs on the server standard output
         later admins can see them remotely
```

### Comparing `snews_pt-1.3.2/snews_pt/snews_format_checker.py` & `snews_pt-1.3.3/snews_pt/snews_format_checker.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/snews_pt_utils.py` & `snews_pt-1.3.3/snews_pt/snews_pt_utils.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/snews_pub.py` & `snews_pt-1.3.3/snews_pt/snews_pub.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/snews_sub.py` & `snews_pt-1.3.3/snews_pt/snews_sub.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/random_plugin.py` & `snews_pt-1.3.3/snews_pt/test/random_plugin.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_coincidence_tier.py` & `snews_pt-1.3.3/snews_pt/test/test_coincidence_tier.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_old_crashes.py` & `snews_pt-1.3.3/snews_pt/test/test_old_crashes.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_plugin.py` & `snews_pt-1.3.3/snews_pt/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_retraction.py` & `snews_pt-1.3.3/snews_pt/test/test_retraction.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_significance_tier.py` & `snews_pt-1.3.3/snews_pt/test/test_significance_tier.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_subscribe.py` & `snews_pt-1.3.3/snews_pt/test/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/test/test_timing_tier.py` & `snews_pt-1.3.3/snews_pt/test/test_timing_tier.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt/tier_decider.py` & `snews_pt-1.3.3/snews_pt/tier_decider.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.2/snews_pt.egg-info/PKG-INFO` & `snews_pt-1.3.3/snews_pt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snews-pt
-Version: 1.3.2
+Version: 1.3.3
 Summary: An alert application for observing supernovas.
 Home-page: https://github.com/SNEWS2/SNEWS_Publishing_Tools
 Author: Sebastian Torres-Lara, Melih Kara
 Author-email: sebastiantorreslara17@gmail.com, karamel.itu@gmail.com
 License: BSD 3-Clause
 Keywords: setup,distutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snews_pt-1.3.2/snews_pt.egg-info/SOURCES.txt` & `snews_pt-1.3.3/snews_pt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

