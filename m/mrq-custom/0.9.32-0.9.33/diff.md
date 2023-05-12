# Comparing `tmp/mrq-custom-0.9.32.tar.gz` & `tmp/mrq-custom-0.9.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrq-custom-0.9.32.tar", last modified: Tue May  9 16:18:52 2023, max compression
+gzip compressed data, was "mrq-custom-0.9.33.tar", last modified: Fri May 12 05:42:30 2023, max compression
```

## Comparing `mrq-custom-0.9.32.tar` & `mrq-custom-0.9.33.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.310382 mrq-custom-0.9.32/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1083 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/LICENSE
--rw-r--r--   0 ghabrielv   (501) staff       (20)      145 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/MANIFEST.in
--rw-r--r--   0 ghabrielv   (501) staff       (20)     9261 2023-05-09 16:18:52.309119 mrq-custom-0.9.32/PKG-INFO
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8270 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/README.md
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.132682 mrq-custom-0.9.32/mrq/
--rw-r--r--   0 ghabrielv   (501) staff       (20)       12 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     7352 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/agent.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.137019 mrq-custom-0.9.32/mrq/basetasks/
--rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/basetasks/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/basetasks/cleaning.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2167 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/basetasks/indexes.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3901 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/basetasks/orchestrator.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     5813 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/basetasks/utils.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.142551 mrq-custom-0.9.32/mrq/bin/
--rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/bin/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      857 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/bin/mrq_agent.py
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     2229 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/bin/mrq_run.py
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1509 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/bin/mrq_worker.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    18048 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/config.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8116 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/context.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.147619 mrq-custom-0.9.32/mrq/dashboard/
--rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/__init__.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    11412 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/app.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.149897 mrq-custom-0.9.32/mrq/dashboard/static/
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.165611 mrq-custom-0.9.32/mrq/dashboard/static/bin/
--rw-r--r--   0 ghabrielv   (501) staff       (20)   469976 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/0.bundle.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2943 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/bundle.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png
--rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.173038 mrq-custom-0.9.32/mrq/dashboard/static/css/
--rw-r--r--   0 ghabrielv   (501) staff       (20)   123361 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/css/bootstrap-theme.min.css
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3694 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/css/datatables.css
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)      367 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/css/jquery.circliful.css
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1453 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/css/mrq-dashboard.css
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.184076 mrq-custom-0.9.32/mrq/dashboard/static/fonts/
--rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.197859 mrq-custom-0.9.32/mrq/dashboard/static/images/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1406 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/favicon-old.ico
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1579 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/favicon.ico
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/sort_asc.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/sort_asc_disabled.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/sort_both.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/sort_desc.png
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/images/sort_desc_disabled.png
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.212228 mrq-custom-0.9.32/mrq/dashboard/static/js/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2620 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/app.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4947 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/main.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)       84 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/models.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3977 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/router.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.248810 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/
--rw-r--r--   0 ghabrielv   (501) staff       (20)    19967 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/backbone.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     9618 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/backbone.queryparams.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    55258 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/bootstrap.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    29110 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/bootstrap.min.js
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     7045 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/datatables.bs3.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    83614 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js
--rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3096 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery.circliful.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    70857 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    43246 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    26050 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/moment.min.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    80376 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/require.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    14643 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/underscore.min.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.280618 mrq-custom-0.9.32/mrq/dashboard/static/js/views/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/agents.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.287472 mrq-custom-0.9.32/mrq/dashboard/static/js/views/generic/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     6664 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/generic/datatablepage.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4645 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/generic/page.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4697 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/index.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4107 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/io.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)    15498 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/jobs.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     5180 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/queues.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4263 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/root.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2211 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/scheduledjobs.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2360 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/status.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2873 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/taskexceptions.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2235 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/taskpaths.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)      879 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/workergroups.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)     6884 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/js/views/workers.js
--rw-r--r--   0 ghabrielv   (501) staff       (20)      562 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/package.json
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1484 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/static/webpack.config.js
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.292446 mrq-custom-0.9.32/mrq/dashboard/templates/
--rw-r--r--   0 ghabrielv   (501) staff       (20)    17348 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/templates/index.html
--rw-r--r--   0 ghabrielv   (501) staff       (20)    43302 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/templates/library.html
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1388 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/dashboard/utils.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     1638 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/exceptions.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      918 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/helpers.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    25667 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/job.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3573 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/logger.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    15471 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/monkey.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     6460 2023-05-04 14:04:25.000000 mrq-custom-0.9.32/mrq/processes.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8652 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/queue.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8586 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/queue_raw.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4991 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/queue_regular.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     2251 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/redishelpers.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     4982 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/scheduler.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3326 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/subpool.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      737 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/supervisor.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)      663 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/task.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)     8050 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/utils.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)       88 2023-05-09 16:13:52.000000 mrq-custom-0.9.32/mrq/version.py
--rw-r--r--   0 ghabrielv   (501) staff       (20)    24783 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/mrq/worker.py
-drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-09 16:18:52.306985 mrq-custom-0.9.32/mrq_custom.egg-info/
--rw-r--r--   0 ghabrielv   (501) staff       (20)     9261 2023-05-09 16:18:52.000000 mrq-custom-0.9.32/mrq_custom.egg-info/PKG-INFO
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3821 2023-05-09 16:18:52.000000 mrq-custom-0.9.32/mrq_custom.egg-info/SOURCES.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-09 16:18:52.000000 mrq-custom-0.9.32/mrq_custom.egg-info/dependency_links.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      160 2023-05-09 16:18:52.000000 mrq-custom-0.9.32/mrq_custom.egg-info/entry_points.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-09 15:38:54.000000 mrq-custom-0.9.32/mrq_custom.egg-info/not-zip-safe
--rw-r--r--   0 ghabrielv   (501) staff       (20)      169 2023-05-09 16:18:52.000000 mrq-custom-0.9.32/mrq_custom.egg-info/requires.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)        4 2023-05-09 16:18:52.000000 mrq-custom-0.9.32/mrq_custom.egg-info/top_level.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      268 2023-05-09 16:03:30.000000 mrq-custom-0.9.32/requirements-base.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/requirements-dashboard.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      337 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/requirements-dev.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/requirements-heroku.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)      205 2023-05-09 16:04:20.000000 mrq-custom-0.9.32/requirements.txt
--rw-r--r--   0 ghabrielv   (501) staff       (20)       38 2023-05-09 16:18:52.311154 mrq-custom-0.9.32/setup.cfg
--rw-r--r--   0 ghabrielv   (501) staff       (20)     3036 2023-03-10 20:48:18.000000 mrq-custom-0.9.32/setup.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.844916 mrq-custom-0.9.33/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1083 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/LICENSE
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      145 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/MANIFEST.in
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     9261 2023-05-12 05:42:30.843635 mrq-custom-0.9.33/PKG-INFO
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8270 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/README.md
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.683685 mrq-custom-0.9.33/mrq/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       12 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     7352 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/agent.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.689653 mrq-custom-0.9.33/mrq/basetasks/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/basetasks/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/basetasks/cleaning.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2167 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/basetasks/indexes.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3901 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/basetasks/orchestrator.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     5813 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/basetasks/utils.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.693868 mrq-custom-0.9.33/mrq/bin/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/bin/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      857 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/bin/mrq_agent.py
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     2229 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/bin/mrq_run.py
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1509 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/bin/mrq_worker.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    18048 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/config.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8136 2023-05-12 05:41:10.000000 mrq-custom-0.9.33/mrq/context.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.697050 mrq-custom-0.9.33/mrq/dashboard/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        0 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/__init__.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    11412 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/app.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.699033 mrq-custom-0.9.33/mrq/dashboard/static/
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.717014 mrq-custom-0.9.33/mrq/dashboard/static/bin/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)   469976 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/0.bundle.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2943 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/bundle.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.722877 mrq-custom-0.9.33/mrq/dashboard/static/css/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)   123361 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3694 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/css/datatables.css
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)      367 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/css/jquery.circliful.css
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1453 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/css/mrq-dashboard.css
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.728956 mrq-custom-0.9.33/mrq/dashboard/static/fonts/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    20335 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    62927 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    41280 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    23320 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.735674 mrq-custom-0.9.33/mrq/dashboard/static/images/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1406 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/favicon-old.ico
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1579 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/favicon.ico
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1118 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/sort_asc.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1050 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/sort_asc_disabled.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1136 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/sort_both.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1127 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/sort_desc.png
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     1045 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/images/sort_desc_disabled.png
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.741503 mrq-custom-0.9.33/mrq/dashboard/static/js/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2620 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/app.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4947 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/main.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       84 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/models.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3977 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/router.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.770338 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    19967 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/backbone.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     9618 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/backbone.queryparams.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    55258 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/bootstrap.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    29110 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/bootstrap.min.js
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     7045 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/datatables.bs3.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    83614 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js
+-rwxr-xr-x   0 ghabrielv   (501) staff       (20)     3096 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery.circliful.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    70857 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    43246 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    26050 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/moment.min.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    80376 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/require.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    14643 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/underscore.min.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.812150 mrq-custom-0.9.33/mrq/dashboard/static/js/views/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3157 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/agents.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.821887 mrq-custom-0.9.33/mrq/dashboard/static/js/views/generic/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     6664 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/generic/datatablepage.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4645 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/generic/page.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4697 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/index.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4107 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/io.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    15498 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/jobs.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     5180 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/queues.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4263 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/root.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2211 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/scheduledjobs.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2360 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/status.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2873 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/taskexceptions.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2235 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/taskpaths.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      879 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/workergroups.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     6884 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/js/views/workers.js
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      562 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/package.json
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1484 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/static/webpack.config.js
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.829142 mrq-custom-0.9.33/mrq/dashboard/templates/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    17348 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/templates/index.html
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    43302 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/templates/library.html
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1388 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/dashboard/utils.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     1638 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/exceptions.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      918 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/helpers.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    25667 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/job.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3573 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/logger.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    15471 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/monkey.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     6460 2023-05-04 14:04:25.000000 mrq-custom-0.9.33/mrq/processes.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8652 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/queue.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8586 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/queue_raw.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4991 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/queue_regular.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     2251 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/redishelpers.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     4982 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/scheduler.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3326 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/subpool.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      737 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/supervisor.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      663 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/task.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     8050 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/utils.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       88 2023-05-12 05:42:00.000000 mrq-custom-0.9.33/mrq/version.py
+-rw-r--r--   0 ghabrielv   (501) staff       (20)    24783 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/mrq/worker.py
+drwxr-xr-x   0 ghabrielv   (501) staff       (20)        0 2023-05-12 05:42:30.841575 mrq-custom-0.9.33/mrq_custom.egg-info/
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     9261 2023-05-12 05:42:30.000000 mrq-custom-0.9.33/mrq_custom.egg-info/PKG-INFO
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3821 2023-05-12 05:42:30.000000 mrq-custom-0.9.33/mrq_custom.egg-info/SOURCES.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-12 05:42:30.000000 mrq-custom-0.9.33/mrq_custom.egg-info/dependency_links.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      160 2023-05-12 05:42:30.000000 mrq-custom-0.9.33/mrq_custom.egg-info/entry_points.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        1 2023-05-09 15:38:54.000000 mrq-custom-0.9.33/mrq_custom.egg-info/not-zip-safe
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      169 2023-05-12 05:42:30.000000 mrq-custom-0.9.33/mrq_custom.egg-info/requires.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)        4 2023-05-12 05:42:30.000000 mrq-custom-0.9.33/mrq_custom.egg-info/top_level.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      268 2023-05-09 16:03:30.000000 mrq-custom-0.9.33/requirements-base.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/requirements-dashboard.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      337 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/requirements-dev.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       13 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/requirements-heroku.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)      205 2023-05-09 16:04:20.000000 mrq-custom-0.9.33/requirements.txt
+-rw-r--r--   0 ghabrielv   (501) staff       (20)       38 2023-05-12 05:42:30.845431 mrq-custom-0.9.33/setup.cfg
+-rw-r--r--   0 ghabrielv   (501) staff       (20)     3036 2023-03-10 20:48:18.000000 mrq-custom-0.9.33/setup.py
```

### Comparing `mrq-custom-0.9.32/LICENSE` & `mrq-custom-0.9.33/LICENSE`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/PKG-INFO` & `mrq-custom-0.9.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrq-custom
-Version: 0.9.32
+Version: 0.9.33
 Summary: A simple yet powerful distributed worker task queue in Python
 Home-page: http://github.com/pricingassistant/mrq
 Author: Pricing Assistant
 Author-email: contact@pricingassistant.com
 License: MIT
 Keywords: worker,task,distributed,queue,asynchronous,redis,mongodb,job,processing,gevent
 Platform: any
```

### Comparing `mrq-custom-0.9.32/README.md` & `mrq-custom-0.9.33/README.md`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/agent.py` & `mrq-custom-0.9.33/mrq/agent.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/basetasks/cleaning.py` & `mrq-custom-0.9.33/mrq/basetasks/cleaning.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/basetasks/indexes.py` & `mrq-custom-0.9.33/mrq/basetasks/indexes.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/basetasks/orchestrator.py` & `mrq-custom-0.9.33/mrq/basetasks/orchestrator.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/basetasks/utils.py` & `mrq-custom-0.9.33/mrq/basetasks/utils.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/bin/mrq_agent.py` & `mrq-custom-0.9.33/mrq/bin/mrq_agent.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/bin/mrq_run.py` & `mrq-custom-0.9.33/mrq/bin/mrq_run.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/bin/mrq_worker.py` & `mrq-custom-0.9.33/mrq/bin/mrq_worker.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/config.py` & `mrq-custom-0.9.33/mrq/config.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/context.py` & `mrq-custom-0.9.33/mrq/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 db=int((redis_url.path or "").replace("/", "") or "0"),
                 password=redis_url.password if redis_url.password is not None else redis_url.username,
                 max_connections=int(config.get("redis_max_connections")),
                 timeout=int(config.get("redis_timeout")),
                 decode_responses=False,
                 connection_class=connection_class
             )
-            return pyredis.StrictRedis(connection_pool=redis_pool)
+            return pyredis.StrictRedis(connection_pool=redis_pool, ssl_cert_reqs=None)
 
         # Let's just assume we got a StrictRedis-like object!
         else:
             return config_obj
 
     elif attr.startswith("mongodb"):
```

### Comparing `mrq-custom-0.9.32/mrq/dashboard/app.py` & `mrq-custom-0.9.33/mrq/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/0.bundle.js` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/0.bundle.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/32941d6330044744c02493835b799e90.svg`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/64f2d23d70cb2b2810031880f554b13c.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/68ed1dac06bf0409c18ae7bc62889170.woff`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/6c56b94fd0540844a7118cdff565b0ae.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/7ad17c6085dee9a33787bac28fb23d46.eot`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/8f88d990024975797f96ce7648dacd2f.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/94b34ff5224ba38210d67623bb1a1504.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/bundle.js` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/bundle.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/d48475e6c742940f44e62622e16865b9.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf` & `mrq-custom-0.9.33/mrq/dashboard/static/bin/e49d52e74b7689a0727def99da31f3eb.ttf`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/css/bootstrap-theme.min.css` & `mrq-custom-0.9.33/mrq/dashboard/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/css/datatables.css` & `mrq-custom-0.9.33/mrq/dashboard/static/css/datatables.css`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/css/mrq-dashboard.css` & `mrq-custom-0.9.33/mrq/dashboard/static/css/mrq-dashboard.css`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot` & `mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg` & `mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf` & `mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff` & `mrq-custom-0.9.33/mrq/dashboard/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/favicon-old.ico` & `mrq-custom-0.9.33/mrq/dashboard/static/images/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/favicon.ico` & `mrq-custom-0.9.33/mrq/dashboard/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/sort_asc.png` & `mrq-custom-0.9.33/mrq/dashboard/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/sort_asc_disabled.png` & `mrq-custom-0.9.33/mrq/dashboard/static/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/sort_both.png` & `mrq-custom-0.9.33/mrq/dashboard/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/sort_desc.png` & `mrq-custom-0.9.33/mrq/dashboard/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/images/sort_desc_disabled.png` & `mrq-custom-0.9.33/mrq/dashboard/static/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/app.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/app.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/main.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/main.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/router.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/router.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/backbone.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/backbone.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/backbone.queryparams.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/backbone.queryparams.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/bootstrap.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/bootstrap.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/datatables.bs3.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/datatables.bs3.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery-2.1.0.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery.circliful.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery.circliful.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/moment.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/moment.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/require.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/require.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/vendor/underscore.min.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/vendor/underscore.min.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/agents.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/agents.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/generic/datatablepage.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/generic/datatablepage.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/generic/page.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/generic/page.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/index.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/index.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/io.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/io.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/jobs.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/jobs.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/queues.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/queues.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/root.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/root.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/scheduledjobs.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/scheduledjobs.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/status.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/status.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/taskexceptions.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/taskexceptions.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/taskpaths.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/taskpaths.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/workergroups.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/workergroups.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/js/views/workers.js` & `mrq-custom-0.9.33/mrq/dashboard/static/js/views/workers.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/package.json` & `mrq-custom-0.9.33/mrq/dashboard/static/package.json`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/static/webpack.config.js` & `mrq-custom-0.9.33/mrq/dashboard/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/templates/index.html` & `mrq-custom-0.9.33/mrq/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/templates/library.html` & `mrq-custom-0.9.33/mrq/dashboard/templates/library.html`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/dashboard/utils.py` & `mrq-custom-0.9.33/mrq/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/exceptions.py` & `mrq-custom-0.9.33/mrq/exceptions.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/helpers.py` & `mrq-custom-0.9.33/mrq/helpers.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/job.py` & `mrq-custom-0.9.33/mrq/job.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/logger.py` & `mrq-custom-0.9.33/mrq/logger.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/monkey.py` & `mrq-custom-0.9.33/mrq/monkey.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/processes.py` & `mrq-custom-0.9.33/mrq/processes.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/queue.py` & `mrq-custom-0.9.33/mrq/queue.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/queue_raw.py` & `mrq-custom-0.9.33/mrq/queue_raw.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/queue_regular.py` & `mrq-custom-0.9.33/mrq/queue_regular.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/redishelpers.py` & `mrq-custom-0.9.33/mrq/redishelpers.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/scheduler.py` & `mrq-custom-0.9.33/mrq/scheduler.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/subpool.py` & `mrq-custom-0.9.33/mrq/subpool.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/supervisor.py` & `mrq-custom-0.9.33/mrq/supervisor.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/task.py` & `mrq-custom-0.9.33/mrq/task.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/utils.py` & `mrq-custom-0.9.33/mrq/utils.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq/worker.py` & `mrq-custom-0.9.33/mrq/worker.py`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/mrq_custom.egg-info/PKG-INFO` & `mrq-custom-0.9.33/mrq_custom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrq-custom
-Version: 0.9.32
+Version: 0.9.33
 Summary: A simple yet powerful distributed worker task queue in Python
 Home-page: http://github.com/pricingassistant/mrq
 Author: Pricing Assistant
 Author-email: contact@pricingassistant.com
 License: MIT
 Keywords: worker,task,distributed,queue,asynchronous,redis,mongodb,job,processing,gevent
 Platform: any
```

### Comparing `mrq-custom-0.9.32/mrq_custom.egg-info/SOURCES.txt` & `mrq-custom-0.9.33/mrq_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mrq-custom-0.9.32/setup.py` & `mrq-custom-0.9.33/setup.py`

 * *Files identical despite different names*

