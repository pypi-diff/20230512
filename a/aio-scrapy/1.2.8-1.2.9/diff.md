# Comparing `tmp/aio-scrapy-1.2.8.tar.gz` & `tmp/aio-scrapy-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-scrapy-1.2.8.tar", last modified: Tue Mar 28 03:57:53 2023, max compression
+gzip compressed data, was "aio-scrapy-1.2.9.tar", last modified: Wed Mar 29 02:30:23 2023, max compression
```

## Comparing `aio-scrapy-1.2.8.tar` & `aio-scrapy-1.2.9.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.559682 aio-scrapy-1.2.8/
--rw-rw-rw-   0        0        0     1088 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      182 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5019 2023-03-28 03:57:53.559682 aio-scrapy-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3831 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.507520 aio-scrapy-1.2.8/aio_scrapy.egg-info/
--rw-rw-rw-   0        0        0     5019 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4195 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      399 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-28 03:57:53.000000 aio-scrapy-1.2.8/aio_scrapy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.513489 aio-scrapy-1.2.8/aioscrapy/
--rw-rw-rw-   0        0        0        5 2023-03-28 03:49:36.000000 aio-scrapy-1.2.8/aioscrapy/VERSION
--rw-rw-rw-   0        0        0      796 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/__init__.py
--rw-rw-rw-   0        0        0       84 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/__main__.py
--rw-rw-rw-   0        0        0     5329 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/cmdline.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.517478 aio-scrapy-1.2.8/aioscrapy/commands/
--rw-rw-rw-   0        0        0     4895 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/crawl.py
--rw-rw-rw-   0        0        0     5570 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/genspider.py
--rw-rw-rw-   0        0        0      360 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/list.py
--rw-rw-rw-   0        0        0     2139 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/runspider.py
--rw-rw-rw-   0        0        0     1845 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/settings.py
--rw-rw-rw-   0        0        0     4125 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/startproject.py
--rw-rw-rw-   0        0        0      506 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/commands/version.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.518476 aio-scrapy-1.2.8/aioscrapy/core/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.519474 aio-scrapy-1.2.8/aioscrapy/core/downloader/
--rw-rw-rw-   0        0        0     9588 2023-03-22 01:35:13.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.520471 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/
--rw-rw-rw-   0        0        0     3218 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/__init__.py
--rw-rw-rw-   0        0        0     3959 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/aiohttp.py
--rw-rw-rw-   0        0        0     2638 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/httpx.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.522466 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/
--rw-rw-rw-   0        0        0     3329 2023-03-28 03:29:21.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-03-28 01:32:33.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/driverpool.py
--rw-rw-rw-   0        0        0     3949 2023-03-28 03:20:47.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/webdriver.py
--rw-rw-rw-   0        0        0     2063 2023-03-28 03:20:47.000000 aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/pyhttpx.py
--rw-rw-rw-   0        0        0    10912 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/core/engine.py
--rw-rw-rw-   0        0        0     5860 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/core/scheduler.py
--rw-rw-rw-   0        0        0    11340 2023-03-28 01:32:33.000000 aio-scrapy-1.2.8/aioscrapy/core/scraper.py
--rw-rw-rw-   0        0        0    10426 2023-03-28 01:32:33.000000 aio-scrapy-1.2.8/aioscrapy/crawler.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.524460 aio-scrapy-1.2.8/aioscrapy/db/
--rw-rw-rw-   0        0        0     2415 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/db/__init__.py
--rw-rw-rw-   0        0        0     1209 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/db/absmanager.py
--rw-rw-rw-   0        0        0     2887 2023-03-21 06:25:56.000000 aio-scrapy-1.2.8/aioscrapy/db/aiomongo.py
--rw-rw-rw-   0        0        0     3979 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/db/aiomysql.py
--rw-rw-rw-   0        0        0     5810 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/db/aiorabbitmq.py
--rw-rw-rw-   0        0        0     3060 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/db/aioredis.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.525457 aio-scrapy-1.2.8/aioscrapy/dupefilters/
--rw-rw-rw-   0        0        0      855 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/dupefilters/__init__.py
--rw-rw-rw-   0        0        0     2302 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/dupefilters/disk.py
--rw-rw-rw-   0        0        0     5324 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/dupefilters/redis.py
--rw-rw-rw-   0        0        0     2072 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.526455 aio-scrapy-1.2.8/aioscrapy/http/
--rw-rw-rw-   0        0        0      612 2023-03-28 01:32:33.000000 aio-scrapy-1.2.8/aioscrapy/http/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/http/headers.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.527452 aio-scrapy-1.2.8/aioscrapy/http/request/
--rw-rw-rw-   0        0        0     7092 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/http/request/__init__.py
--rw-rw-rw-   0        0        0     1421 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/http/request/form.py
--rw-rw-rw-   0        0        0     2114 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/http/request/json_request.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.529447 aio-scrapy-1.2.8/aioscrapy/http/response/
--rw-rw-rw-   0        0        0     6939 2023-03-21 02:27:39.000000 aio-scrapy-1.2.8/aioscrapy/http/response/__init__.py
--rw-rw-rw-   0        0        0      315 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/http/response/html.py
--rw-rw-rw-   0        0        0     1087 2023-03-28 02:39:16.000000 aio-scrapy-1.2.8/aioscrapy/http/response/playwright.py
--rw-rw-rw-   0        0        0    10109 2023-03-28 01:32:33.000000 aio-scrapy-1.2.8/aioscrapy/http/response/text.py
--rw-rw-rw-   0        0        0      312 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/http/response/xml.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.529447 aio-scrapy-1.2.8/aioscrapy/libs/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.533441 aio-scrapy-1.2.8/aioscrapy/libs/downloader/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/__init__.py
--rw-rw-rw-   0        0        0      585 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/defaultheaders.py
--rw-rw-rw-   0        0        0      730 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/downloadtimeout.py
--rw-rw-rw-   0        0        0     1094 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/ja3fingerprint.py
--rw-rw-rw-   0        0        0     4813 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/retry.py
--rw-rw-rw-   0        0        0     1457 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/stats.py
--rw-rw-rw-   0        0        0      766 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/downloader/useragent.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.535431 aio-scrapy-1.2.8/aioscrapy/libs/extensions/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/extensions/__init__.py
--rw-rw-rw-   0        0        0     2829 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/extensions/closespider.py
--rw-rw-rw-   0        0        0     1862 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/extensions/corestats.py
--rw-rw-rw-   0        0        0     1904 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/extensions/logstats.py
--rw-rw-rw-   0        0        0     3677 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/extensions/throttle.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.535431 aio-scrapy-1.2.8/aioscrapy/libs/pipelines/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/pipelines/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.536428 aio-scrapy-1.2.8/aioscrapy/libs/pipelines/sink/
--rw-rw-rw-   0        0        0       93 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/pipelines/sink/__init__.py
--rw-rw-rw-   0        0        0     3171 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/pipelines/sink/mongo.py
--rw-rw-rw-   0        0        0     5495 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/pipelines/sink/mysql.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.539421 aio-scrapy-1.2.8/aioscrapy/libs/spider/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/spider/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/spider/depth.py
--rw-rw-rw-   0        0        0     1968 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/spider/httperror.py
--rw-rw-rw-   0        0        0     3068 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/spider/offsite.py
--rw-rw-rw-   0        0        0    14132 2023-03-28 01:39:33.000000 aio-scrapy-1.2.8/aioscrapy/libs/spider/referer.py
--rw-rw-rw-   0        0        0     1225 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/libs/spider/urllength.py
--rw-rw-rw-   0        0        0     1920 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/link.py
--rw-rw-rw-   0        0        0     3441 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/logformatter.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.541415 aio-scrapy-1.2.8/aioscrapy/middleware/
--rw-rw-rw-   0        0        0      396 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/middleware/__init__.py
--rw-rw-rw-   0        0        0     3772 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/middleware/absmanager.py
--rw-rw-rw-   0        0        0     3328 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/middleware/downloader.py
--rw-rw-rw-   0        0        0      436 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/middleware/extension.py
--rw-rw-rw-   0        0        0      736 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/middleware/itempipeline.py
--rw-rw-rw-   0        0        0     6493 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/middleware/spider.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.542412 aio-scrapy-1.2.8/aioscrapy/proxy/
--rw-rw-rw-   0        0        0     1885 2023-03-21 03:16:53.000000 aio-scrapy-1.2.8/aioscrapy/proxy/__init__.py
--rw-rw-rw-   0        0        0     2377 2023-03-21 03:37:58.000000 aio-scrapy-1.2.8/aioscrapy/proxy/redis.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.543409 aio-scrapy-1.2.8/aioscrapy/queue/
--rw-rw-rw-   0        0        0     2092 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/queue/__init__.py
--rw-rw-rw-   0        0        0     3229 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/queue/memory.py
--rw-rw-rw-   0        0        0     2576 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/queue/rabbitmq.py
--rw-rw-rw-   0        0        0     4966 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/queue/redis.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.544407 aio-scrapy-1.2.8/aioscrapy/scrapyd/
--rw-rw-rw-   0        0        0       71 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/scrapyd/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/scrapyd/runner.py
--rw-rw-rw-   0        0        0      773 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/serializer.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.545404 aio-scrapy-1.2.8/aioscrapy/settings/
--rw-rw-rw-   0        0        0    16247 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/settings/__init__.py
--rw-rw-rw-   0        0        0     4562 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/settings/default_settings.py
--rw-rw-rw-   0        0        0     2470 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/signalmanager.py
--rw-rw-rw-   0        0        0      634 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/signals.py
--rw-rw-rw-   0        0        0     3534 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/spiderloader.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.545404 aio-scrapy-1.2.8/aioscrapy/spiders/
--rw-rw-rw-   0        0        0     4732 2023-03-21 02:33:30.000000 aio-scrapy-1.2.8/aioscrapy/spiders/__init__.py
--rw-rw-rw-   0        0        0     2181 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/statscollectors.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.497532 aio-scrapy-1.2.8/aioscrapy/templates/
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.546401 aio-scrapy-1.2.8/aioscrapy/templates/project/
--rw-rw-rw-   0        0        0      118 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/project/aioscrapy.cfg
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.547399 aio-scrapy-1.2.8/aioscrapy/templates/project/module/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/project/module/__init__.py
--rw-rw-rw-   0        0        0     3560 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/project/module/middlewares.py.tmpl
--rw-rw-rw-   0        0        0       97 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/project/module/pipelines.py.tmpl
--rw-rw-rw-   0        0        0     1772 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/project/module/settings.py.tmpl
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.547399 aio-scrapy-1.2.8/aioscrapy/templates/project/module/spiders/
--rw-rw-rw-   0        0        0      168 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/project/module/spiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.550703 aio-scrapy-1.2.8/aioscrapy/templates/spiders/
--rw-rw-rw-   0        0        0      413 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/spiders/basic.tmpl
--rw-rw-rw-   0        0        0      885 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/templates/spiders/single.tmpl
-drwxrwxrwx   0        0        0        0 2023-03-28 03:57:53.558685 aio-scrapy-1.2.8/aioscrapy/utils/
--rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/__init__.py
--rw-rw-rw-   0        0        0     7403 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/conf.py
--rw-rw-rw-   0        0        0     3401 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/curl.py
--rw-rw-rw-   0        0        0      819 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/decorators.py
--rw-rw-rw-   0        0        0     6516 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/deprecate.py
--rw-rw-rw-   0        0        0      727 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/httpobj.py
--rw-rw-rw-   0        0        0     6426 2023-03-23 01:36:38.000000 aio-scrapy-1.2.8/aioscrapy/utils/log.py
--rw-rw-rw-   0        0        0     3611 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/misc.py
--rw-rw-rw-   0        0        0      896 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/ossignal.py
--rw-rw-rw-   0        0        0     2994 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/project.py
--rw-rw-rw-   0        0        0     4730 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/python.py
--rw-rw-rw-   0        0        0      490 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/reqser.py
--rw-rw-rw-   0        0        0     2379 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/request.py
--rw-rw-rw-   0        0        0     1379 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/response.py
--rw-rw-rw-   0        0        0     2371 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/signal.py
--rw-rw-rw-   0        0        0      672 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/spider.py
--rw-rw-rw-   0        0        0      869 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/template.py
--rw-rw-rw-   0        0        0     2133 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/tools.py
--rw-rw-rw-   0        0        0     2086 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/trackref.py
--rw-rw-rw-   0        0        0     5628 2023-03-20 07:05:57.000000 aio-scrapy-1.2.8/aioscrapy/utils/url.py
--rw-rw-rw-   0        0        0       42 2023-03-28 03:57:53.559682 aio-scrapy-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2301 2023-03-28 03:49:36.000000 aio-scrapy-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.472466 aio-scrapy-1.2.9/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      182 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5019 2023-03-29 02:30:23.471958 aio-scrapy-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3831 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:22.889529 aio-scrapy-1.2.9/aio_scrapy.egg-info/
+-rw-rw-rw-   0        0        0     5019 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4195 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      399 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-29 02:30:22.000000 aio-scrapy-1.2.9/aio_scrapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:22.963933 aio-scrapy-1.2.9/aioscrapy/
+-rw-rw-rw-   0        0        0        5 2023-03-29 02:29:52.000000 aio-scrapy-1.2.9/aioscrapy/VERSION
+-rw-rw-rw-   0        0        0      796 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/__init__.py
+-rw-rw-rw-   0        0        0       84 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/__main__.py
+-rw-rw-rw-   0        0        0     5329 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/cmdline.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.017255 aio-scrapy-1.2.9/aioscrapy/commands/
+-rw-rw-rw-   0        0        0     4895 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/crawl.py
+-rw-rw-rw-   0        0        0     5570 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/genspider.py
+-rw-rw-rw-   0        0        0      360 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/list.py
+-rw-rw-rw-   0        0        0     2139 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/runspider.py
+-rw-rw-rw-   0        0        0     1845 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/settings.py
+-rw-rw-rw-   0        0        0     4125 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/startproject.py
+-rw-rw-rw-   0        0        0      506 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/commands/version.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.029650 aio-scrapy-1.2.9/aioscrapy/core/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.038853 aio-scrapy-1.2.9/aioscrapy/core/downloader/
+-rw-rw-rw-   0        0        0     9588 2023-03-22 01:35:13.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.061305 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/
+-rw-rw-rw-   0        0        0     3218 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3959 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/aiohttp.py
+-rw-rw-rw-   0        0        0     2638 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/httpx.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.079818 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/
+-rw-rw-rw-   0        0        0     3329 2023-03-28 03:29:21.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-03-28 01:32:33.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/driverpool.py
+-rw-rw-rw-   0        0        0     3949 2023-03-28 03:20:47.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/webdriver.py
+-rw-rw-rw-   0        0        0     2200 2023-03-28 05:12:20.000000 aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/pyhttpx.py
+-rw-rw-rw-   0        0        0    10912 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/core/engine.py
+-rw-rw-rw-   0        0        0     5860 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/core/scheduler.py
+-rw-rw-rw-   0        0        0    11340 2023-03-28 01:32:33.000000 aio-scrapy-1.2.9/aioscrapy/core/scraper.py
+-rw-rw-rw-   0        0        0    10426 2023-03-28 01:32:33.000000 aio-scrapy-1.2.9/aioscrapy/crawler.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.106602 aio-scrapy-1.2.9/aioscrapy/db/
+-rw-rw-rw-   0        0        0     2415 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/db/__init__.py
+-rw-rw-rw-   0        0        0     1209 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/db/absmanager.py
+-rw-rw-rw-   0        0        0     2887 2023-03-21 06:25:56.000000 aio-scrapy-1.2.9/aioscrapy/db/aiomongo.py
+-rw-rw-rw-   0        0        0     3979 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/db/aiomysql.py
+-rw-rw-rw-   0        0        0     5810 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/db/aiorabbitmq.py
+-rw-rw-rw-   0        0        0     3060 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/db/aioredis.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.117514 aio-scrapy-1.2.9/aioscrapy/dupefilters/
+-rw-rw-rw-   0        0        0      855 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/dupefilters/__init__.py
+-rw-rw-rw-   0        0        0     2302 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/dupefilters/disk.py
+-rw-rw-rw-   0        0        0     5324 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/dupefilters/redis.py
+-rw-rw-rw-   0        0        0     2072 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.126936 aio-scrapy-1.2.9/aioscrapy/http/
+-rw-rw-rw-   0        0        0      612 2023-03-28 01:32:33.000000 aio-scrapy-1.2.9/aioscrapy/http/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/http/headers.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.141950 aio-scrapy-1.2.9/aioscrapy/http/request/
+-rw-rw-rw-   0        0        0     7176 2023-03-28 09:07:02.000000 aio-scrapy-1.2.9/aioscrapy/http/request/__init__.py
+-rw-rw-rw-   0        0        0     1421 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/http/request/form.py
+-rw-rw-rw-   0        0        0     2114 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/http/request/json_request.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.165595 aio-scrapy-1.2.9/aioscrapy/http/response/
+-rw-rw-rw-   0        0        0     6939 2023-03-21 02:27:39.000000 aio-scrapy-1.2.9/aioscrapy/http/response/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/http/response/html.py
+-rw-rw-rw-   0        0        0     1087 2023-03-28 02:39:16.000000 aio-scrapy-1.2.9/aioscrapy/http/response/playwright.py
+-rw-rw-rw-   0        0        0    10109 2023-03-28 01:32:33.000000 aio-scrapy-1.2.9/aioscrapy/http/response/text.py
+-rw-rw-rw-   0        0        0      312 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/http/response/xml.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.166588 aio-scrapy-1.2.9/aioscrapy/libs/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.194462 aio-scrapy-1.2.9/aioscrapy/libs/downloader/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/__init__.py
+-rw-rw-rw-   0        0        0      585 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/defaultheaders.py
+-rw-rw-rw-   0        0        0      730 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/downloadtimeout.py
+-rw-rw-rw-   0        0        0     1094 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/ja3fingerprint.py
+-rw-rw-rw-   0        0        0     4813 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/retry.py
+-rw-rw-rw-   0        0        0     1457 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/stats.py
+-rw-rw-rw-   0        0        0      766 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/downloader/useragent.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.214802 aio-scrapy-1.2.9/aioscrapy/libs/extensions/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2829 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/extensions/closespider.py
+-rw-rw-rw-   0        0        0     1862 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/extensions/corestats.py
+-rw-rw-rw-   0        0        0     1904 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/extensions/logstats.py
+-rw-rw-rw-   0        0        0     3677 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/extensions/throttle.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.215794 aio-scrapy-1.2.9/aioscrapy/libs/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/pipelines/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.230177 aio-scrapy-1.2.9/aioscrapy/libs/pipelines/sink/
+-rw-rw-rw-   0        0        0       93 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/pipelines/sink/__init__.py
+-rw-rw-rw-   0        0        0     3171 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/pipelines/sink/mongo.py
+-rw-rw-rw-   0        0        0     5495 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/pipelines/sink/mysql.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.256583 aio-scrapy-1.2.9/aioscrapy/libs/spider/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/spider/__init__.py
+-rw-rw-rw-   0        0        0     2083 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/spider/depth.py
+-rw-rw-rw-   0        0        0     1968 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/spider/httperror.py
+-rw-rw-rw-   0        0        0     3068 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/spider/offsite.py
+-rw-rw-rw-   0        0        0    14132 2023-03-28 01:39:33.000000 aio-scrapy-1.2.9/aioscrapy/libs/spider/referer.py
+-rw-rw-rw-   0        0        0     1225 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/libs/spider/urllength.py
+-rw-rw-rw-   0        0        0     1920 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/link.py
+-rw-rw-rw-   0        0        0     3441 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/logformatter.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.283840 aio-scrapy-1.2.9/aioscrapy/middleware/
+-rw-rw-rw-   0        0        0      396 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3772 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/middleware/absmanager.py
+-rw-rw-rw-   0        0        0     3328 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/middleware/downloader.py
+-rw-rw-rw-   0        0        0      436 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/middleware/extension.py
+-rw-rw-rw-   0        0        0      736 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/middleware/itempipeline.py
+-rw-rw-rw-   0        0        0     6493 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/middleware/spider.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.300615 aio-scrapy-1.2.9/aioscrapy/proxy/
+-rw-rw-rw-   0        0        0     1965 2023-03-28 09:07:02.000000 aio-scrapy-1.2.9/aioscrapy/proxy/__init__.py
+-rw-rw-rw-   0        0        0     2377 2023-03-21 03:37:58.000000 aio-scrapy-1.2.9/aioscrapy/proxy/redis.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.319965 aio-scrapy-1.2.9/aioscrapy/queue/
+-rw-rw-rw-   0        0        0     2092 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/queue/__init__.py
+-rw-rw-rw-   0        0        0     3229 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/queue/memory.py
+-rw-rw-rw-   0        0        0     2576 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/queue/rabbitmq.py
+-rw-rw-rw-   0        0        0     4966 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/queue/redis.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.328890 aio-scrapy-1.2.9/aioscrapy/scrapyd/
+-rw-rw-rw-   0        0        0       71 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/scrapyd/__init__.py
+-rw-rw-rw-   0        0        0     1841 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/scrapyd/runner.py
+-rw-rw-rw-   0        0        0      773 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/serializer.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.340793 aio-scrapy-1.2.9/aioscrapy/settings/
+-rw-rw-rw-   0        0        0    16247 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/settings/__init__.py
+-rw-rw-rw-   0        0        0     4562 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/settings/default_settings.py
+-rw-rw-rw-   0        0        0     2470 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/signalmanager.py
+-rw-rw-rw-   0        0        0      634 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/signals.py
+-rw-rw-rw-   0        0        0     3534 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/spiderloader.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.346745 aio-scrapy-1.2.9/aioscrapy/spiders/
+-rw-rw-rw-   0        0        0     4732 2023-03-21 02:33:30.000000 aio-scrapy-1.2.9/aioscrapy/spiders/__init__.py
+-rw-rw-rw-   0        0        0     2181 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/statscollectors.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:22.869686 aio-scrapy-1.2.9/aioscrapy/templates/
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.350221 aio-scrapy-1.2.9/aioscrapy/templates/project/
+-rw-rw-rw-   0        0        0      118 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/project/aioscrapy.cfg
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.363609 aio-scrapy-1.2.9/aioscrapy/templates/project/module/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/project/module/__init__.py
+-rw-rw-rw-   0        0        0     3560 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/project/module/middlewares.py.tmpl
+-rw-rw-rw-   0        0        0       97 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/project/module/pipelines.py.tmpl
+-rw-rw-rw-   0        0        0     1772 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/project/module/settings.py.tmpl
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.367085 aio-scrapy-1.2.9/aioscrapy/templates/project/module/spiders/
+-rw-rw-rw-   0        0        0      168 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/project/module/spiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.375021 aio-scrapy-1.2.9/aioscrapy/templates/spiders/
+-rw-rw-rw-   0        0        0      413 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/spiders/basic.tmpl
+-rw-rw-rw-   0        0        0      885 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/templates/spiders/single.tmpl
+drwxrwxrwx   0        0        0        0 2023-03-29 02:30:23.470492 aio-scrapy-1.2.9/aioscrapy/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/__init__.py
+-rw-rw-rw-   0        0        0     7403 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/conf.py
+-rw-rw-rw-   0        0        0     3401 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/curl.py
+-rw-rw-rw-   0        0        0      819 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/decorators.py
+-rw-rw-rw-   0        0        0     6516 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/deprecate.py
+-rw-rw-rw-   0        0        0      727 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/httpobj.py
+-rw-rw-rw-   0        0        0     6426 2023-03-23 01:36:38.000000 aio-scrapy-1.2.9/aioscrapy/utils/log.py
+-rw-rw-rw-   0        0        0     3611 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/misc.py
+-rw-rw-rw-   0        0        0      896 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/ossignal.py
+-rw-rw-rw-   0        0        0     2994 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/project.py
+-rw-rw-rw-   0        0        0     4730 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/python.py
+-rw-rw-rw-   0        0        0      490 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/reqser.py
+-rw-rw-rw-   0        0        0     2379 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/request.py
+-rw-rw-rw-   0        0        0     1379 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/response.py
+-rw-rw-rw-   0        0        0     2371 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/signal.py
+-rw-rw-rw-   0        0        0      672 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/spider.py
+-rw-rw-rw-   0        0        0      869 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/template.py
+-rw-rw-rw-   0        0        0     2133 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/tools.py
+-rw-rw-rw-   0        0        0     2086 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/trackref.py
+-rw-rw-rw-   0        0        0     5628 2023-03-20 07:05:57.000000 aio-scrapy-1.2.9/aioscrapy/utils/url.py
+-rw-rw-rw-   0        0        0       42 2023-03-29 02:30:23.472466 aio-scrapy-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2301 2023-03-28 03:49:36.000000 aio-scrapy-1.2.9/setup.py
```

### Comparing `aio-scrapy-1.2.8/LICENSE` & `aio-scrapy-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/PKG-INFO` & `aio-scrapy-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-scrapy
-Version: 1.2.8
+Version: 1.2.9
 Summary: A high-level Web Crawling and Web Scraping framework based on Asyncio
 Home-page: https://github.com/conlin-huang/aio-scrapy.git
 Author: conlin
 Author-email: 995018884@qq.com
 License: MIT
 Keywords: aio-scrapy,scrapy,aioscrapy,scrapy redis,asyncio,spider
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aio-scrapy-1.2.8/README.md` & `aio-scrapy-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aio_scrapy.egg-info/PKG-INFO` & `aio-scrapy-1.2.9/aio_scrapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-scrapy
-Version: 1.2.8
+Version: 1.2.9
 Summary: A high-level Web Crawling and Web Scraping framework based on Asyncio
 Home-page: https://github.com/conlin-huang/aio-scrapy.git
 Author: conlin
 Author-email: 995018884@qq.com
 License: MIT
 Keywords: aio-scrapy,scrapy,aioscrapy,scrapy redis,asyncio,spider
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aio-scrapy-1.2.8/aio_scrapy.egg-info/SOURCES.txt` & `aio-scrapy-1.2.9/aio_scrapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/cmdline.py` & `aio-scrapy-1.2.9/aioscrapy/cmdline.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/commands/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/commands/crawl.py` & `aio-scrapy-1.2.9/aioscrapy/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/commands/genspider.py` & `aio-scrapy-1.2.9/aioscrapy/commands/genspider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/commands/runspider.py` & `aio-scrapy-1.2.9/aioscrapy/commands/runspider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/commands/settings.py` & `aio-scrapy-1.2.9/aioscrapy/commands/settings.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/commands/startproject.py` & `aio-scrapy-1.2.9/aioscrapy/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/aiohttp.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/httpx.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/httpx.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/driverpool.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/driverpool.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/playwright/webdriver.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/playwright/webdriver.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/downloader/handlers/pyhttpx.py` & `aio-scrapy-1.2.9/aioscrapy/core/downloader/handlers/pyhttpx.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,17 +24,22 @@
     def from_settings(cls, settings: Settings):
         return cls(settings)
 
     async def download_request(self, request: Request, _) -> HtmlResponse:
         kwargs = {
             'timeout': self.settings.get('DOWNLOAD_TIMEOUT'),
             'cookies': dict(request.cookies),
-            'data': request.body or None,
             'verify': self.verify_ssl
         }
+        post_data = request.body or None
+        if isinstance(post_data, dict):
+            kwargs['json'] = post_data
+        else:
+            kwargs['data'] = post_data
+
         headers = request.headers or self.settings.get('DEFAULT_REQUEST_HEADERS')
         kwargs['headers'] = headers
 
         proxy = request.meta.get("proxy")
         if proxy:
             parsed_url = urlparse(proxy)
             kwargs["proxies"] = {'https': parsed_url.netloc.split('@')[-1]}
```

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/engine.py` & `aio-scrapy-1.2.9/aioscrapy/core/engine.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/scheduler.py` & `aio-scrapy-1.2.9/aioscrapy/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/core/scraper.py` & `aio-scrapy-1.2.9/aioscrapy/core/scraper.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/crawler.py` & `aio-scrapy-1.2.9/aioscrapy/crawler.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/db/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/db/absmanager.py` & `aio-scrapy-1.2.9/aioscrapy/db/absmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/db/aiomongo.py` & `aio-scrapy-1.2.9/aioscrapy/db/aiomongo.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/db/aiomysql.py` & `aio-scrapy-1.2.9/aioscrapy/db/aiomysql.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/db/aiorabbitmq.py` & `aio-scrapy-1.2.9/aioscrapy/db/aiorabbitmq.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/db/aioredis.py` & `aio-scrapy-1.2.9/aioscrapy/db/aioredis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/dupefilters/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/dupefilters/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/dupefilters/disk.py` & `aio-scrapy-1.2.9/aioscrapy/dupefilters/disk.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/dupefilters/redis.py` & `aio-scrapy-1.2.9/aioscrapy/dupefilters/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/exceptions.py` & `aio-scrapy-1.2.9/aioscrapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/headers.py` & `aio-scrapy-1.2.9/aioscrapy/http/headers.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/request/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/http/request/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class Request(object):
     attributes: Tuple[str, ...] = (
         "url", "callback", "method", "headers", "body",
         "cookies", "meta", "encoding", "priority",
         "dont_filter", "errback", "flags", "cb_kwargs",
-        "fingerprint"
+        "fingerprint", "use_proxy"
     )
 
     def __init__(
             self,
             url: str,
             callback: Optional[Callable] = None,
             method: str = 'GET',
@@ -41,14 +41,15 @@
             encoding: str = 'utf-8',
             priority: int = 0,
             dont_filter: bool = False,
             errback: Optional[Callable] = None,
             flags: Optional[List[str]] = None,
             cb_kwargs: Optional[Callable] = None,
             fingerprint: Optional[str] = None,
+            use_proxy: bool = True,
     ):
 
         self._encoding = encoding
         self.method = str(method).upper()
         self._set_url(url)
         self._set_body(body)
         assert isinstance(priority, int), f"Request priority not an integer: {priority!r}"
@@ -57,14 +58,15 @@
         self.callback = callback
         self.errback = errback
 
         self.cookies = cookies or {}
         self.headers = Headers(headers or {})
         self.dont_filter = dont_filter
         self._fingerprint = fingerprint
+        self.use_proxy=use_proxy
 
         self._meta = dict(meta) if meta else None
         self._cb_kwargs = dict(cb_kwargs) if cb_kwargs else None
         self.flags = [] if flags is None else list(flags)
 
     @property
     def cb_kwargs(self) -> dict:
```

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/request/form.py` & `aio-scrapy-1.2.9/aioscrapy/http/request/form.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/request/json_request.py` & `aio-scrapy-1.2.9/aioscrapy/http/request/json_request.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/response/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/http/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/response/playwright.py` & `aio-scrapy-1.2.9/aioscrapy/http/response/playwright.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/http/response/text.py` & `aio-scrapy-1.2.9/aioscrapy/http/response/text.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/downloader/defaultheaders.py` & `aio-scrapy-1.2.9/aioscrapy/libs/downloader/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/downloader/downloadtimeout.py` & `aio-scrapy-1.2.9/aioscrapy/libs/downloader/downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/downloader/ja3fingerprint.py` & `aio-scrapy-1.2.9/aioscrapy/libs/downloader/ja3fingerprint.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/downloader/retry.py` & `aio-scrapy-1.2.9/aioscrapy/libs/downloader/retry.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/downloader/stats.py` & `aio-scrapy-1.2.9/aioscrapy/libs/downloader/stats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/downloader/useragent.py` & `aio-scrapy-1.2.9/aioscrapy/libs/downloader/useragent.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/extensions/closespider.py` & `aio-scrapy-1.2.9/aioscrapy/libs/extensions/closespider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/extensions/corestats.py` & `aio-scrapy-1.2.9/aioscrapy/libs/extensions/corestats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/extensions/logstats.py` & `aio-scrapy-1.2.9/aioscrapy/libs/extensions/logstats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/extensions/throttle.py` & `aio-scrapy-1.2.9/aioscrapy/libs/extensions/throttle.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/pipelines/sink/mongo.py` & `aio-scrapy-1.2.9/aioscrapy/libs/pipelines/sink/mongo.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/pipelines/sink/mysql.py` & `aio-scrapy-1.2.9/aioscrapy/libs/pipelines/sink/mysql.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/spider/depth.py` & `aio-scrapy-1.2.9/aioscrapy/libs/spider/depth.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/spider/httperror.py` & `aio-scrapy-1.2.9/aioscrapy/libs/spider/httperror.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/spider/offsite.py` & `aio-scrapy-1.2.9/aioscrapy/libs/spider/offsite.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/spider/referer.py` & `aio-scrapy-1.2.9/aioscrapy/libs/spider/referer.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/libs/spider/urllength.py` & `aio-scrapy-1.2.9/aioscrapy/libs/spider/urllength.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/link.py` & `aio-scrapy-1.2.9/aioscrapy/link.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/logformatter.py` & `aio-scrapy-1.2.9/aioscrapy/logformatter.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/middleware/absmanager.py` & `aio-scrapy-1.2.9/aioscrapy/middleware/absmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/middleware/downloader.py` & `aio-scrapy-1.2.9/aioscrapy/middleware/downloader.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/middleware/itempipeline.py` & `aio-scrapy-1.2.9/aioscrapy/middleware/itempipeline.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/middleware/spider.py` & `aio-scrapy-1.2.9/aioscrapy/middleware/spider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/proxy/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/proxy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 
 class AbsProxy(metaclass=ABCMeta):
     def __init__(self, settings):
         self.use_proxy = settings.getbool('USE_PROXY', False)
         self.max_count = settings.getint('PROXY_MAX_COUNT', 16)
         self.min_count = settings.getint('PROXY_MIN_COUNT', 1)
-        self.allow_status_code = settings.get('PROXY_ALLOW_STATUS_CODE', [200, 404, 302, 307])
+        self.allow_status_code = settings.get('PROXY_ALLOW_STATUS_CODE', [404])
         self.cache = []
 
     async def add_proxy(self, request):
         """add proxy for request"""
-        if self.use_proxy:
+        if self.use_proxy and request.use_proxy:
             request.meta['proxy'] = await self.get()
         else:
             request.meta.pop('proxy', None)
         return request
 
     def remove(self, proxy, reason=None):
         if callable(reason):
@@ -35,15 +35,16 @@
         if proxy in self.cache:
             logger.info(f"remove proxy: {proxy}, reason: {reason}")
             self.cache.remove(proxy)
 
     def check(self, request, response=None, exception=None):
         if not self.use_proxy:
             return
-
+        if response and 200 <= response.status < 400:
+            return
         if response and response.status not in self.allow_status_code:
             self.remove(request.meta['proxy'], f"Don't allow response status code:{response.status}")
 
         if exception and isinstance(exception, BaseException):
             self.remove(request.meta['proxy'], exception)
 
     @classmethod
```

### Comparing `aio-scrapy-1.2.8/aioscrapy/proxy/redis.py` & `aio-scrapy-1.2.9/aioscrapy/proxy/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/queue/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/queue/memory.py` & `aio-scrapy-1.2.9/aioscrapy/queue/memory.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/queue/rabbitmq.py` & `aio-scrapy-1.2.9/aioscrapy/queue/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/queue/redis.py` & `aio-scrapy-1.2.9/aioscrapy/queue/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/scrapyd/runner.py` & `aio-scrapy-1.2.9/aioscrapy/scrapyd/runner.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/serializer.py` & `aio-scrapy-1.2.9/aioscrapy/serializer.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/settings/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/settings/default_settings.py` & `aio-scrapy-1.2.9/aioscrapy/settings/default_settings.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/signalmanager.py` & `aio-scrapy-1.2.9/aioscrapy/signalmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/signals.py` & `aio-scrapy-1.2.9/aioscrapy/signals.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/spiderloader.py` & `aio-scrapy-1.2.9/aioscrapy/spiderloader.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/spiders/__init__.py` & `aio-scrapy-1.2.9/aioscrapy/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/statscollectors.py` & `aio-scrapy-1.2.9/aioscrapy/statscollectors.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/templates/project/module/middlewares.py.tmpl` & `aio-scrapy-1.2.9/aioscrapy/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/templates/project/module/settings.py.tmpl` & `aio-scrapy-1.2.9/aioscrapy/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/templates/spiders/single.tmpl` & `aio-scrapy-1.2.9/aioscrapy/templates/spiders/single.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/conf.py` & `aio-scrapy-1.2.9/aioscrapy/utils/conf.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/curl.py` & `aio-scrapy-1.2.9/aioscrapy/utils/curl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/decorators.py` & `aio-scrapy-1.2.9/aioscrapy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/deprecate.py` & `aio-scrapy-1.2.9/aioscrapy/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/httpobj.py` & `aio-scrapy-1.2.9/aioscrapy/utils/httpobj.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/log.py` & `aio-scrapy-1.2.9/aioscrapy/utils/log.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/misc.py` & `aio-scrapy-1.2.9/aioscrapy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/ossignal.py` & `aio-scrapy-1.2.9/aioscrapy/utils/ossignal.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/project.py` & `aio-scrapy-1.2.9/aioscrapy/utils/project.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/python.py` & `aio-scrapy-1.2.9/aioscrapy/utils/python.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/request.py` & `aio-scrapy-1.2.9/aioscrapy/utils/request.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/response.py` & `aio-scrapy-1.2.9/aioscrapy/utils/response.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/signal.py` & `aio-scrapy-1.2.9/aioscrapy/utils/signal.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/spider.py` & `aio-scrapy-1.2.9/aioscrapy/utils/spider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/template.py` & `aio-scrapy-1.2.9/aioscrapy/utils/template.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/tools.py` & `aio-scrapy-1.2.9/aioscrapy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/trackref.py` & `aio-scrapy-1.2.9/aioscrapy/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/aioscrapy/utils/url.py` & `aio-scrapy-1.2.9/aioscrapy/utils/url.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-1.2.8/setup.py` & `aio-scrapy-1.2.9/setup.py`

 * *Files identical despite different names*

