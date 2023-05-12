# Comparing `tmp/bagbag-0.58.9.tar.gz` & `tmp/bagbag-0.59.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagbag-0.58.9.tar", max compression
+gzip compressed data, was "bagbag-0.59.0.tar", max compression
```

## Comparing `bagbag-0.58.9.tar` & `bagbag-0.59.0.tar`

### file list

```diff
@@ -1,231 +1,250 @@
--rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.58.9/LICENSE
--rw-r--r--   0        0        0    16310 2023-05-03 13:30:21.697775 bagbag-0.58.9/README.md
--rw-r--r--   0        0        0     2152 2023-05-05 17:15:04.292498 bagbag-0.58.9/pyproject.toml
--rw-r--r--   0        0        0      456 2022-12-18 14:46:48.344905 bagbag-0.58.9/src/bagbag/Base64.py
--rw-r--r--   0        0        0     5749 2023-04-18 10:31:59.025703 bagbag-0.58.9/src/bagbag/Cmd.py
--rw-r--r--   0        0        0     2530 2023-04-28 07:15:37.583071 bagbag-0.58.9/src/bagbag/Cryptoo.py
--rw-r--r--   0        0        0     4558 2023-04-27 09:57:17.336471 bagbag-0.58.9/src/bagbag/File.py
--rw-r--r--   0        0        0      951 2023-04-06 11:26:46.488789 bagbag-0.58.9/src/bagbag/Funcs/CutSentence.py
--rw-r--r--   0        0        0    16724 2022-10-11 13:26:11.473001 bagbag-0.58.9/src/bagbag/Funcs/CutSentenceStopWords.py
--rw-r--r--   0        0        0     6790 2023-02-21 10:25:15.382302 bagbag-0.58.9/src/bagbag/Funcs/FakeIdentity.py
--rw-r--r--   0        0        0      515 2023-03-15 05:06:17.699339 bagbag-0.58.9/src/bagbag/Funcs/FileType.py
--rw-r--r--   0        0        0      783 2022-10-16 15:29:21.224299 bagbag-0.58.9/src/bagbag/Funcs/Format.py
--rw-r--r--   0        0        0      825 2022-08-25 08:45:04.248840 bagbag-0.58.9/src/bagbag/Funcs/GetPublicIP.py
--rw-r--r--   0        0        0      253 2022-08-06 09:50:15.275766 bagbag-0.58.9/src/bagbag/Funcs/IPAddressConvert.py
--rw-r--r--   0        0        0      185 2022-12-20 12:28:30.619497 bagbag-0.58.9/src/bagbag/Funcs/Markdown.py
--rw-r--r--   0        0        0     1107 2023-04-06 11:12:42.351012 bagbag-0.58.9/src/bagbag/Funcs/Ping.py
--rw-r--r--   0        0        0     1687 2022-12-25 11:45:41.361813 bagbag-0.58.9/src/bagbag/Funcs/ResizeImage.py
--rw-r--r--   0        0        0       70 2022-10-01 18:51:28.539798 bagbag-0.58.9/src/bagbag/Funcs/UUID.py
--rw-r--r--   0        0        0     1415 2023-02-13 06:34:05.155815 bagbag-0.58.9/src/bagbag/Funcs/Wget.py
--rw-r--r--   0        0        0      389 2023-03-15 05:07:00.007727 bagbag-0.58.9/src/bagbag/Funcs/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-26 07:07:50.732472 bagbag-0.58.9/src/bagbag/Hash.py
--rw-r--r--   0        0        0    13466 2023-04-24 16:25:51.632962 bagbag-0.58.9/src/bagbag/Http.py
--rw-r--r--   0        0        0     1628 2023-01-12 10:33:44.123536 bagbag-0.58.9/src/bagbag/Json.py
--rw-r--r--   0        0        0    10860 2022-12-22 06:05:36.078005 bagbag-0.58.9/src/bagbag/Lg.py
--rw-r--r--   0        0        0     2055 2022-08-18 13:37:24.221488 bagbag-0.58.9/src/bagbag/Math.py
--rw-r--r--   0        0        0     1665 2023-04-14 07:49:40.462303 bagbag-0.58.9/src/bagbag/Os/Path/__init__.py
--rw-r--r--   0        0        0     3050 2023-03-23 13:34:08.290027 bagbag-0.58.9/src/bagbag/Os/__init__.py
--rw-r--r--   0        0        0     1022 2023-01-26 18:08:40.527831 bagbag-0.58.9/src/bagbag/Process.py
--rw-r--r--   0        0        0      962 2022-11-30 19:42:40.659521 bagbag-0.58.9/src/bagbag/Python.py
--rw-r--r--   0        0        0      611 2022-10-07 15:25:00.730045 bagbag-0.58.9/src/bagbag/Random.py
--rw-r--r--   0        0        0     4951 2023-04-25 15:43:10.177547 bagbag-0.58.9/src/bagbag/Socket/TCP.py
--rw-r--r--   0        0        0       17 2022-08-05 14:47:59.523595 bagbag-0.58.9/src/bagbag/Socket/__init__.py
--rw-r--r--   0        0        0    15867 2023-04-24 15:52:44.638080 bagbag-0.58.9/src/bagbag/String.py
--rw-r--r--   0        0        0      439 2022-08-10 11:11:23.471024 bagbag-0.58.9/src/bagbag/Thread.py
--rw-r--r--   0        0        0     4686 2023-04-06 11:26:37.528262 bagbag-0.58.9/src/bagbag/Time.py
--rw-r--r--   0        0        0     2396 2022-09-16 08:58:48.233364 bagbag-0.58.9/src/bagbag/Tools/Argparser.py
--rw-r--r--   0        0        0     2572 2023-04-10 05:27:14.813130 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice.py
--rw-r--r--   0        0        0      918 2023-02-14 12:53:32.011975 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/OfficalAccountVertify.py
--rw-r--r--   0        0        0       68 2023-04-09 15:54:13.555282 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/__init__.py
--rw-r--r--   0        0        0       36 2023-02-20 11:29:39.344076 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
--rw-r--r--   0        0        0      272 2023-02-20 11:33:21.209236 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
--rw-r--r--   0        0        0       53 2023-02-06 12:12:49.206521 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Tron/__init__.py
--rw-r--r--   0        0        0    23137 2023-04-06 11:30:14.742190 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Tron/tron.py
--rw-r--r--   0        0        0       65 2023-02-20 11:35:34.074298 bagbag-0.58.9/src/bagbag/Tools/BlockChain/__init__.py
--rw-r--r--   0        0        0     3041 2023-02-13 06:23:00.196283 bagbag-0.58.9/src/bagbag/Tools/CSV.py
--rw-r--r--   0        0        0     3833 2023-04-25 13:07:57.003030 bagbag-0.58.9/src/bagbag/Tools/Chan.py
--rw-r--r--   0        0        0    32840 2023-05-05 14:45:08.189272 bagbag-0.58.9/src/bagbag/Tools/ComputerVision.py
--rw-r--r--   0        0        0     3274 2022-09-15 08:56:37.350792 bagbag-0.58.9/src/bagbag/Tools/Crontab.py
--rw-r--r--   0        0        0    33457 2023-03-29 10:41:45.581869 bagbag-0.58.9/src/bagbag/Tools/Database.py
--rw-r--r--   0        0        0     5342 2023-02-15 08:29:18.848798 bagbag-0.58.9/src/bagbag/Tools/DistributedLock.py
--rw-r--r--   0        0        0     4700 2023-01-19 11:17:18.748095 bagbag-0.58.9/src/bagbag/Tools/Elasticsearch.py
--rw-r--r--   0        0        0     4441 2023-01-17 15:18:13.958863 bagbag-0.58.9/src/bagbag/Tools/Github.py
--rw-r--r--   0        0        0     1398 2023-03-17 07:42:12.672824 bagbag-0.58.9/src/bagbag/Tools/JavaScript.py
--rw-r--r--   0        0        0     2201 2023-03-08 07:11:22.568544 bagbag-0.58.9/src/bagbag/Tools/Kafka.py
--rw-r--r--   0        0        0     1975 2023-05-04 17:08:07.122161 bagbag-0.58.9/src/bagbag/Tools/Lock.py
--rw-r--r--   0        0        0     6734 2023-01-16 07:23:53.117189 bagbag-0.58.9/src/bagbag/Tools/MatrixBot.py
--rw-r--r--   0        0        0      413 2022-12-27 07:28:58.688307 bagbag-0.58.9/src/bagbag/Tools/Nslookup.py
--rw-r--r--   0        0        0     2430 2023-05-03 13:29:38.917729 bagbag-0.58.9/src/bagbag/Tools/OCR.py
--rw-r--r--   0        0        0     2763 2023-02-12 16:33:24.414810 bagbag-0.58.9/src/bagbag/Tools/ProgressBar.py
--rw-r--r--   0        0        0     1607 2023-02-02 12:01:54.298178 bagbag-0.58.9/src/bagbag/Tools/Prometheus/MetricServer.py
--rw-r--r--   0        0        0     3281 2023-02-13 05:16:20.084875 bagbag-0.58.9/src/bagbag/Tools/Prometheus/PushGateway.py
--rw-r--r--   0        0        0       75 2023-01-08 14:37:29.001741 bagbag-0.58.9/src/bagbag/Tools/Prometheus/__init__.py
--rw-r--r--   0        0        0     4670 2023-02-02 11:59:41.614890 bagbag-0.58.9/src/bagbag/Tools/Prometheus/metrics.py
--rw-r--r--   0        0        0     2669 2022-12-25 18:30:26.203387 bagbag-0.58.9/src/bagbag/Tools/Queue.py
--rw-r--r--   0        0        0     2364 2022-12-21 11:16:06.096822 bagbag-0.58.9/src/bagbag/Tools/RSS/Feed.py
--rw-r--r--   0        0        0      608 2022-12-20 13:54:34.868627 bagbag-0.58.9/src/bagbag/Tools/RSS/Opml.py
--rw-r--r--   0        0        0       63 2022-12-20 13:51:52.113940 bagbag-0.58.9/src/bagbag/Tools/RSS/__init__.py
--rw-r--r--   0        0        0     3734 2023-02-01 12:01:16.040605 bagbag-0.58.9/src/bagbag/Tools/Ratelimit.py
--rw-r--r--   0        0        0    18528 2023-03-08 07:40:25.704818 bagbag-0.58.9/src/bagbag/Tools/Redis.py
--rw-r--r--   0        0        0     5584 2023-03-14 17:28:24.607245 bagbag-0.58.9/src/bagbag/Tools/SSH.py
--rw-r--r--   0        0        0    32178 2023-05-05 17:14:55.298931 bagbag-0.58.9/src/bagbag/Tools/Selenium.py
--rw-r--r--   0        0        0    24493 2023-04-27 09:55:24.505212 bagbag-0.58.9/src/bagbag/Tools/Telegram.py
--rw-r--r--   0        0        0    14070 2022-10-11 17:50:44.936863 bagbag-0.58.9/src/bagbag/Tools/TelegramAsync.py
--rw-r--r--   0        0        0     3205 2023-04-26 11:42:55.114246 bagbag-0.58.9/src/bagbag/Tools/TelegramBot.py
--rw-r--r--   0        0        0     5034 2023-04-03 05:37:03.126681 bagbag-0.58.9/src/bagbag/Tools/TelegramBotOfficial.py
--rw-r--r--   0        0        0      142 2023-02-03 16:58:05.049775 bagbag-0.58.9/src/bagbag/Tools/Test.py
--rw-r--r--   0        0        0     4174 2023-01-20 21:55:20.155790 bagbag-0.58.9/src/bagbag/Tools/Translater.py
--rw-r--r--   0        0        0     9625 2023-03-14 10:07:44.832848 bagbag-0.58.9/src/bagbag/Tools/Twitter/Elevated.py
--rw-r--r--   0        0        0     2026 2023-01-19 08:07:09.796818 bagbag-0.58.9/src/bagbag/Tools/Twitter/Essential.py
--rw-r--r--   0        0        0      115 2023-02-10 11:22:25.584307 bagbag-0.58.9/src/bagbag/Tools/Twitter/__init__.py
--rw-r--r--   0        0        0     3069 2023-01-10 07:22:39.926298 bagbag-0.58.9/src/bagbag/Tools/URL.py
--rw-r--r--   0        0        0      706 2022-09-22 12:55:34.535377 bagbag-0.58.9/src/bagbag/Tools/WaitGroup.py
--rw-r--r--   0        0        0     8073 2023-04-12 13:00:33.539301 bagbag-0.58.9/src/bagbag/Tools/WebCrawler.py
--rw-r--r--   0        0        0     5519 2023-04-26 09:49:53.097526 bagbag-0.58.9/src/bagbag/Tools/WebServer.py
--rw-r--r--   0        0        0     1649 2022-09-29 08:11:47.066310 bagbag-0.58.9/src/bagbag/Tools/XPath.py
--rw-r--r--   0        0        0     3141 2023-02-17 12:39:22.967883 bagbag-0.58.9/src/bagbag/Tools/Xlsx.py
--rw-r--r--   0        0        0     1298 2023-05-03 13:23:08.445668 bagbag-0.58.9/src/bagbag/Tools/__init__.py
--rw-r--r--   0        0        0      297 2022-08-07 06:00:20.038297 bagbag-0.58.9/src/bagbag/Tools/orator/__init__.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.038583 bagbag-0.58.9/src/bagbag/Tools/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2022-08-07 06:00:20.038727 bagbag-0.58.9/src/bagbag/Tools/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2022-08-07 06:00:20.038865 bagbag-0.58.9/src/bagbag/Tools/orator/commands/command.py
--rw-r--r--   0        0        0      330 2022-08-07 06:00:20.039098 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2022-08-07 06:00:20.039235 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2022-08-07 06:00:20.039365 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2022-08-07 06:00:20.039505 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2022-08-07 06:00:20.039641 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2022-08-07 06:00:20.039774 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2022-08-07 06:00:20.039842 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2022-08-07 06:00:20.039917 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2022-08-07 06:00:20.040021 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2022-08-07 06:00:20.040169 bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2022-08-07 06:00:20.040266 bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2022-08-07 06:00:20.040350 bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2022-08-07 06:00:20.040493 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2022-08-07 06:00:20.040578 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2022-08-07 06:00:20.040660 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2022-08-07 06:00:20.040748 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2022-08-07 06:00:20.040920 bagbag-0.58.9/src/bagbag/Tools/orator/connections/__init__.py
--rw-r--r--   0        0        0    15063 2022-08-07 06:00:20.041031 bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2022-08-07 06:00:20.041124 bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2022-08-07 06:00:20.041207 bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2022-08-07 06:00:20.041284 bagbag-0.58.9/src/bagbag/Tools/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2056 2022-08-07 06:00:20.041364 bagbag-0.58.9/src/bagbag/Tools/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2022-08-07 06:00:20.041439 bagbag-0.58.9/src/bagbag/Tools/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2022-08-07 06:00:20.041571 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2022-08-07 06:00:20.041658 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2022-08-07 09:41:15.514461 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connector.py
--rw-r--r--   0        0        0     3982 2022-08-08 19:39:59.546483 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2022-08-07 06:00:20.041888 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2172 2022-08-08 19:41:02.356677 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2022-08-07 06:00:20.042031 bagbag-0.58.9/src/bagbag/Tools/orator/database_manager.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.042156 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2022-08-07 06:00:20.042224 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2022-08-07 06:00:20.042293 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2022-08-07 06:00:20.042368 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2022-08-07 06:00:20.042446 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2022-08-07 06:00:20.042563 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2022-08-07 06:00:20.042633 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2022-08-07 06:00:20.042698 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2022-08-07 06:00:20.042768 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2022-08-07 06:00:20.042837 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2022-08-07 06:00:20.042961 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.043084 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2022-08-07 06:00:20.043158 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2022-08-07 06:00:20.043230 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2022-08-07 06:00:20.043299 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2022-08-07 06:00:20.043366 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1289 2022-08-07 06:00:20.043436 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2022-08-07 06:00:20.043505 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2022-08-07 06:00:20.043582 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2022-08-07 06:00:20.043657 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2022-08-07 06:00:20.043740 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2022-08-07 06:00:20.043817 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2022-08-07 06:00:20.043891 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2022-08-07 06:00:20.043965 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2022-08-07 06:00:20.044039 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2022-08-07 06:00:20.044104 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.044199 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2022-08-07 06:00:20.044295 bagbag-0.58.9/src/bagbag/Tools/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2022-08-07 06:00:20.044403 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2022-08-07 06:00:20.044462 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2022-08-07 06:00:20.044523 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2022-08-07 06:00:20.044585 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2022-08-07 06:00:20.044641 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2022-08-07 06:00:20.044755 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2022-08-07 06:00:20.044822 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2022-08-07 06:00:20.044893 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2022-08-07 06:00:20.044962 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2022-08-07 06:00:20.045025 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2022-08-07 06:00:20.045084 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2022-08-07 06:00:20.045189 bagbag-0.58.9/src/bagbag/Tools/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2022-08-07 06:00:20.045255 bagbag-0.58.9/src/bagbag/Tools/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2022-08-07 06:00:20.045316 bagbag-0.58.9/src/bagbag/Tools/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2022-08-07 06:00:20.045377 bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2022-08-07 06:00:20.045436 bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2022-08-07 06:00:20.045540 bagbag-0.58.9/src/bagbag/Tools/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2022-08-07 06:00:20.045606 bagbag-0.58.9/src/bagbag/Tools/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2022-08-07 06:00:20.045826 bagbag-0.58.9/src/bagbag/Tools/orator/orm/model.py
--rw-r--r--   0        0        0      371 2022-08-07 06:00:20.045999 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2022-08-07 06:00:20.046068 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23248 2022-08-07 06:08:32.255340 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2022-08-07 06:00:20.046219 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2022-08-07 06:00:20.046291 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2022-08-07 06:00:20.046375 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2022-08-07 06:00:20.046441 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2022-08-07 06:00:20.046507 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2022-08-07 06:00:20.046569 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2022-08-07 06:00:20.046631 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2022-08-07 06:00:20.046687 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2022-08-07 06:00:20.046748 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2022-08-07 06:00:20.046819 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2022-08-07 06:00:20.046886 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2022-08-07 06:00:20.046948 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2022-08-07 06:00:20.047011 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2022-08-07 06:00:20.047082 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2022-08-07 06:00:20.047192 bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2022-08-07 06:00:20.047249 bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2022-08-07 06:00:20.047310 bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13642 2022-08-07 06:00:20.047371 bagbag-0.58.9/src/bagbag/Tools/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2022-08-07 06:00:20.047490 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2022-08-07 06:00:20.047576 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2022-08-07 06:00:20.047639 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2022-08-07 06:00:20.047708 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2022-08-07 06:00:20.047810 bagbag-0.58.9/src/bagbag/Tools/orator/query/__init__.py
--rw-r--r--   0        0        0    44030 2023-02-12 15:39:50.939251 bagbag-0.58.9/src/bagbag/Tools/orator/query/builder.py
--rw-r--r--   0        0        0      230 2022-08-07 06:00:20.047933 bagbag-0.58.9/src/bagbag/Tools/orator/query/expression.py
--rw-r--r--   0        0        0      202 2022-08-07 06:00:20.048024 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2022-08-07 06:00:20.048082 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2022-08-07 06:00:20.048144 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2022-08-07 06:00:20.048201 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2022-08-07 06:00:20.048271 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2022-08-07 06:00:20.048331 bagbag-0.58.9/src/bagbag/Tools/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2022-08-07 06:00:20.048431 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2022-08-07 06:00:20.048489 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2022-08-07 06:00:20.048547 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2022-08-07 06:00:20.048615 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2022-08-07 06:00:20.048676 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2022-08-07 06:00:20.048774 bagbag-0.58.9/src/bagbag/Tools/orator/schema/__init__.py
--rw-r--r--   0        0        0    19482 2022-08-07 06:00:20.048840 bagbag-0.58.9/src/bagbag/Tools/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2022-08-07 06:00:20.048903 bagbag-0.58.9/src/bagbag/Tools/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2022-08-07 06:00:20.048999 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2022-08-07 06:00:20.049052 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2022-08-07 06:00:20.049109 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7103 2022-08-07 06:00:20.049180 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2022-08-07 06:00:20.049247 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2022-08-07 06:00:20.049305 bagbag-0.58.9/src/bagbag/Tools/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2022-08-07 06:00:20.049367 bagbag-0.58.9/src/bagbag/Tools/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2022-08-07 06:00:20.049468 bagbag-0.58.9/src/bagbag/Tools/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2022-08-07 06:00:20.049522 bagbag-0.58.9/src/bagbag/Tools/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2022-08-07 06:00:20.049577 bagbag-0.58.9/src/bagbag/Tools/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2022-08-07 06:00:20.049675 bagbag-0.58.9/src/bagbag/Tools/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2022-08-07 06:00:20.049735 bagbag-0.58.9/src/bagbag/Tools/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2022-08-07 06:00:20.049798 bagbag-0.58.9/src/bagbag/Tools/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2022-08-07 06:00:20.049852 bagbag-0.58.9/src/bagbag/Tools/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2022-08-07 06:00:20.049949 bagbag-0.58.9/src/bagbag/Tools/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2022-08-07 06:00:20.050007 bagbag-0.58.9/src/bagbag/Tools/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2022-08-07 06:00:20.050061 bagbag-0.58.9/src/bagbag/Tools/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2022-08-07 06:00:20.050118 bagbag-0.58.9/src/bagbag/Tools/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2022-08-07 06:00:20.050175 bagbag-0.58.9/src/bagbag/Tools/orator/utils/url.py
--rw-r--r--   0        0        0     3335 2023-04-06 11:06:08.005936 bagbag-0.58.9/src/bagbag/__init__.py
--rw-r--r--   0        0        0    19046 1970-01-01 00:00:00.000000 bagbag-0.58.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.59.0/LICENSE
+-rw-r--r--   0        0        0    16310 2023-05-03 13:30:21.697775 bagbag-0.59.0/README.md
+-rw-r--r--   0        0        0     2152 2023-05-12 12:46:56.999391 bagbag-0.59.0/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.59.0/src/bagbag/Base64/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.59.0/src/bagbag/Base64/src.py
+-rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.59.0/src/bagbag/Cmd/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.59.0/src/bagbag/Cmd/src.py
+-rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.59.0/src/bagbag/Cryptoo/__init__.py
+-rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.59.0/src/bagbag/Cryptoo/src.py
+-rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.59.0/src/bagbag/Funcs/CutSentenceStopWords_src.py
+-rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.59.0/src/bagbag/Funcs/CutSentence_src.py
+-rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.59.0/src/bagbag/Funcs/FakeIdentity_src.py
+-rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.59.0/src/bagbag/Funcs/FileType_src.py
+-rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.59.0/src/bagbag/Funcs/Format/__init__.py
+-rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.59.0/src/bagbag/Funcs/Format/src.py
+-rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.59.0/src/bagbag/Funcs/GetPublicIP_src.py
+-rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.59.0/src/bagbag/Funcs/IPAddressConvert_src.py
+-rw-r--r--   0        0        0      227 2023-05-12 12:35:25.858029 bagbag-0.59.0/src/bagbag/Funcs/Markdown_src.py
+-rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.59.0/src/bagbag/Funcs/Ping_src.py
+-rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.59.0/src/bagbag/Funcs/ResizeImage_src.py
+-rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.59.0/src/bagbag/Funcs/UUID_src.py
+-rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.59.0/src/bagbag/Funcs/Wget_src.py
+-rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.59.0/src/bagbag/Funcs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.59.0/src/bagbag/Hash/__init__.py
+-rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.59.0/src/bagbag/Hash/src.py
+-rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.59.0/src/bagbag/Http/__init__.py
+-rw-r--r--   0        0        0    13440 2023-05-12 12:35:25.862718 bagbag-0.59.0/src/bagbag/Http/src.py
+-rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.59.0/src/bagbag/Json/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-12 12:35:25.863083 bagbag-0.59.0/src/bagbag/Json/src.py
+-rw-r--r--   0        0        0    10860 2023-05-12 12:35:25.814780 bagbag-0.59.0/src/bagbag/Lg.py
+-rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.59.0/src/bagbag/Math/__init__.py
+-rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.59.0/src/bagbag/Math/src.py
+-rw-r--r--   0        0        0     1771 2023-05-12 12:35:25.859343 bagbag-0.59.0/src/bagbag/Os/Path/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-12 12:35:25.859454 bagbag-0.59.0/src/bagbag/Os/Path/src_path.py
+-rw-r--r--   0        0        0      835 2023-05-12 12:35:25.859164 bagbag-0.59.0/src/bagbag/Os/__init__.py
+-rw-r--r--   0        0        0     2933 2023-05-12 12:35:25.859730 bagbag-0.59.0/src/bagbag/Os/src.py
+-rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.59.0/src/bagbag/Process/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-12 12:35:25.864234 bagbag-0.59.0/src/bagbag/Process/src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.59.0/src/bagbag/Python/__init__.py
+-rw-r--r--   0        0        0      987 2023-05-12 12:35:25.864640 bagbag-0.59.0/src/bagbag/Python/src.py
+-rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.59.0/src/bagbag/Random/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-12 12:35:25.865063 bagbag-0.59.0/src/bagbag/Random/src.py
+-rw-r--r--   0        0        0      379 2023-05-12 12:35:25.860322 bagbag-0.59.0/src/bagbag/Socket/TCP/__init__.py
+-rw-r--r--   0        0        0     4850 2023-05-12 12:35:25.860244 bagbag-0.59.0/src/bagbag/Socket/TCP/src.py
+-rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.59.0/src/bagbag/Socket/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.59.0/src/bagbag/String/__init__.py
+-rw-r--r--   0        0        0    16767 2023-05-12 12:35:25.865350 bagbag-0.59.0/src/bagbag/String/src.py
+-rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.59.0/src/bagbag/Thread/__init__.py
+-rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865712 bagbag-0.59.0/src/bagbag/Thread/src.py
+-rw-r--r--   0        0        0      517 2023-05-12 12:35:25.866500 bagbag-0.59.0/src/bagbag/Time/__init__.py
+-rw-r--r--   0        0        0     4660 2023-05-12 12:35:25.866441 bagbag-0.59.0/src/bagbag/Time/src.py
+-rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.59.0/src/bagbag/Tools/Argparser_src.py
+-rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
+-rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Binance/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
+-rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Tron/__init__.py
+-rw-r--r--   0        0        0    23255 2023-05-12 12:35:25.824849 bagbag-0.59.0/src/bagbag/Tools/BlockChain/Tron/src.py
+-rw-r--r--   0        0        0      393 2023-05-12 12:35:25.824665 bagbag-0.59.0/src/bagbag/Tools/BlockChain/__init__.py
+-rw-r--r--   0        0        0     3128 2023-05-12 12:35:25.817211 bagbag-0.59.0/src/bagbag/Tools/CSV.py
+-rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.59.0/src/bagbag/Tools/Chan_src.py
+-rw-r--r--   0        0        0    32941 2023-05-12 12:35:25.827719 bagbag-0.59.0/src/bagbag/Tools/ComputerVision.py
+-rw-r--r--   0        0        0     3327 2023-05-12 12:35:25.818786 bagbag-0.59.0/src/bagbag/Tools/Crontab_src.py
+-rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.59.0/src/bagbag/Tools/Database/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.59.0/src/bagbag/Tools/Database/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/application.py
+-rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.59.0/src/bagbag/Tools/Database/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.59.0/src/bagbag/Tools/Database/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/__init__.py
+-rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.59.0/src/bagbag/Tools/Database/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.59.0/src/bagbag/Tools/Database/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.59.0/src/bagbag/Tools/Database/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.59.0/src/bagbag/Tools/Database/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.59.0/src/bagbag/Tools/Database/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.59.0/src/bagbag/Tools/Database/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.59.0/src/bagbag/Tools/Database/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/url.py
+-rw-r--r--   0        0        0    33529 2023-05-12 12:35:25.830380 bagbag-0.59.0/src/bagbag/Tools/Database/src.py
+-rw-r--r--   0        0        0     5396 2023-05-12 12:35:25.823023 bagbag-0.59.0/src/bagbag/Tools/DistributedLock_src.py
+-rw-r--r--   0        0        0     4753 2023-05-12 12:35:25.818559 bagbag-0.59.0/src/bagbag/Tools/Elasticsearch_src.py
+-rw-r--r--   0        0        0     4579 2023-05-12 12:35:25.828651 bagbag-0.59.0/src/bagbag/Tools/File_src.py
+-rw-r--r--   0        0        0     4502 2023-05-12 12:35:25.820400 bagbag-0.59.0/src/bagbag/Tools/Github_src.py
+-rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.59.0/src/bagbag/Tools/JavaScript_src.py
+-rw-r--r--   0        0        0     2254 2023-05-12 12:35:25.820526 bagbag-0.59.0/src/bagbag/Tools/Kafka_src.py
+-rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.59.0/src/bagbag/Tools/Lock_src.py
+-rw-r--r--   0        0        0     6790 2023-05-12 12:35:25.821307 bagbag-0.59.0/src/bagbag/Tools/MatrixBot_src.py
+-rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.59.0/src/bagbag/Tools/Nslookup_src.py
+-rw-r--r--   0        0        0     2486 2023-05-12 12:35:25.828552 bagbag-0.59.0/src/bagbag/Tools/OCR_src.py
+-rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.59.0/src/bagbag/Tools/ProgressBar_src.py
+-rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.59.0/src/bagbag/Tools/Prometheus/MetricServer.py
+-rw-r--r--   0        0        0     3431 2023-05-12 12:35:25.821880 bagbag-0.59.0/src/bagbag/Tools/Prometheus/PushGateway.py
+-rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.59.0/src/bagbag/Tools/Prometheus/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.59.0/src/bagbag/Tools/Prometheus/metrics.py
+-rw-r--r--   0        0        0     2724 2023-05-12 12:35:25.820655 bagbag-0.59.0/src/bagbag/Tools/Queue_src.py
+-rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.59.0/src/bagbag/Tools/RSS/Feed.py
+-rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.59.0/src/bagbag/Tools/RSS/Opml.py
+-rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.59.0/src/bagbag/Tools/RSS/__init__.py
+-rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.59.0/src/bagbag/Tools/Ratelimit_src.py
+-rw-r--r--   0        0        0    18584 2023-05-12 12:35:25.815203 bagbag-0.59.0/src/bagbag/Tools/Redis_src.py
+-rw-r--r--   0        0        0     5565 2023-05-12 12:35:25.820157 bagbag-0.59.0/src/bagbag/Tools/SSH_src.py
+-rw-r--r--   0        0        0    31923 2023-05-12 12:35:25.815789 bagbag-0.59.0/src/bagbag/Tools/Selenium.py
+-rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.59.0/src/bagbag/Tools/TelegramAsync.py
+-rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.59.0/src/bagbag/Tools/TelegramBotOfficial_src.py
+-rw-r--r--   0        0        0     3269 2023-05-12 12:35:25.828367 bagbag-0.59.0/src/bagbag/Tools/TelegramBot_src.py
+-rw-r--r--   0        0        0    24585 2023-05-12 12:35:25.815503 bagbag-0.59.0/src/bagbag/Tools/Telegram_src.py
+-rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.59.0/src/bagbag/Tools/Test.py
+-rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.59.0/src/bagbag/Tools/Translater_src.py
+-rw-r--r--   0        0        0     9678 2023-05-12 12:35:25.823235 bagbag-0.59.0/src/bagbag/Tools/Twitter/Elevated.py
+-rw-r--r--   0        0        0     2079 2023-05-12 12:35:25.823650 bagbag-0.59.0/src/bagbag/Tools/Twitter/Essential.py
+-rw-r--r--   0        0        0      176 2023-05-12 12:35:25.823540 bagbag-0.59.0/src/bagbag/Tools/Twitter/__init__.py
+-rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.59.0/src/bagbag/Tools/URL_src.py
+-rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.59.0/src/bagbag/Tools/WaitGroup_src.py
+-rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.59.0/src/bagbag/Tools/WebCrawler_src.py
+-rw-r--r--   0        0        0     5572 2023-05-12 12:35:25.818682 bagbag-0.59.0/src/bagbag/Tools/WebServer_src.py
+-rw-r--r--   0        0        0     1702 2023-05-12 12:35:25.819763 bagbag-0.59.0/src/bagbag/Tools/XPath_src.py
+-rw-r--r--   0        0        0     3229 2023-05-12 12:35:25.819187 bagbag-0.59.0/src/bagbag/Tools/Xlsx.py
+-rw-r--r--   0        0        0     3231 2023-05-12 12:35:25.815650 bagbag-0.59.0/src/bagbag/Tools/__init__.py
+-rw-r--r--   0        0        0     4448 2023-05-12 12:35:25.861078 bagbag-0.59.0/src/bagbag/__init__.py
+-rw-r--r--   0        0        0    19046 1970-01-01 00:00:00.000000 bagbag-0.59.0/PKG-INFO
```

### Comparing `bagbag-0.58.9/LICENSE` & `bagbag-0.59.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/README.md` & `bagbag-0.59.0/README.md`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/pyproject.toml` & `bagbag-0.59.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bagbag"
-version = "0.58.9"
+version = "0.59.0"
 description = "An all in one python library"
 
 license = "MIT"
 
 authors = [
     "Darren"
 ]
```

### Comparing `bagbag-0.58.9/src/bagbag/Cmd.py` & `bagbag-0.59.0/src/bagbag/Cmd/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import collections
 import queue
 import threading
 import json
 import subprocess
 import shutil
 
+print("load cmd")
+
 class continuousSubprocess:
     """
     Creates a process to execute a wanted command and
     yields a continuous output stream for consumption.
     """
 
     def __init__(self, command_string: str) -> None:
@@ -171,9 +173,10 @@
     _, output = GetStatusOutput(cmd)
 
     return output
 
 def Exist(cmd:str) -> bool:
     return shutil.which(cmd) is not None
 
+
 if __name__ == "__main__":
     print(Exist("ls"))
```

### Comparing `bagbag-0.58.9/src/bagbag/Cryptoo.py` & `bagbag-0.59.0/src/bagbag/Cryptoo/src.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from Crypto.Cipher import AES as AAAES
 from Crypto import Random
 import base64
-import hashlib
+
+print("load cryptoo")
 
 class AES():
     def __init__(self, key:str, mode:str="cfb"): 
         """
         The function takes a key and a mode as arguments, and sets the block size, key, and mode of the
         cipher
```

### Comparing `bagbag-0.58.9/src/bagbag/File.py` & `bagbag-0.59.0/src/bagbag/Tools/File_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import time
 import typing
 import magic
 import mimetypes
-from . import Hash
+from .. import Hash
+
+print("load file")
 
 class File():
     def __init__(self, path:str):
         self.path = path 
 
     def Md5Sum(self) -> str:
         return Hash.Md5sumFile(self.path)
```

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/CutSentenceStopWords.py` & `bagbag-0.59.0/src/bagbag/Funcs/CutSentenceStopWords_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/FakeIdentity.py` & `bagbag-0.59.0/src/bagbag/Funcs/FakeIdentity_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 from bs4 import BeautifulSoup
 
+print("load " + __file__.split('/')[-1])
+
 class fakeIdentityIdent:
     def __init__(self, name, address, street, city, state, zip, motherMaidenName, ssn, coords, phone, countryCode, birthday, birthdayMonth, birthdayDay, birthdayYear, age, zodiac, email, username, password, website, useragent, card, expiration, cvv2, company, occupation, height, heightcm, weight, weightkg, blood, ups, westernunion, moneygram, color, vehicle, guid):
         self.Name:str = name
         self.Address:str = address
         self.Street:str = street
         self.City:str = city
         self.State:str = state
```

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/Format.py` & `bagbag-0.59.0/src/bagbag/Funcs/Format/src.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import time 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 pformat = (lambda a:lambda v,t="    ",n="\n",i=0:a(a,v,t,n,i))(lambda f,v,t,n,i:"{%s%s%s}"%(",".join(["%s%s%s: %s"%(n,t*(i+1),repr(k),f(f,v[k],t,n,i+1))for k in v]),n,(t*i)) if type(v)in[dict] else (type(v)in[list]and"[%s%s%s]"or"(%s%s%s)")%(",".join(["%s%s%s"%(n,t*(i+1),f(f,k,t,n,i+1))for k in v]),n,(t*i)) if type(v)in[list,tuple] else repr(v))
 
 def Size(ByteNumber, suffix='B'):
     for unit in ['','K','M','G','T','P','E','Z']:
         if abs(ByteNumber) < 1024.0:
             return "%3.1f%s%s" % (ByteNumber, unit, suffix)
         ByteNumber /= 1024.0
```

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/GetPublicIP.py` & `bagbag-0.59.0/src/bagbag/Funcs/GetPublicIP_src.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-try:
-    from .. import Http
-    # from .. import Lg
-except:
-    import sys 
-    sys.path.append("..")
-    import Http
-    # import Lg
+from .. import Http
+
+print("load " + __file__.split('/')[-1])
 
 def GetPublicIP(HttpProxy:str=None) -> str:
     servers = [
         "http://ifconfig.me",
         "http://icanhazip.com",
         "http://ipinfo.io/ip",
         "http://api.ipify.org",
```

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/Ping.py` & `bagbag-0.59.0/src/bagbag/Funcs/Ping_src.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from pythonping import ping
 
-try:
-    from ..Tools import Chan
-    from ..Thread import Thread
-    from ..String import String
-except:
-    import sys
-    sys.path.append("..")
-    from Tools import Chan 
-    from Thread import Thread
-    from String import String
+from ..Tools import Chan
+from ..Thread import Thread
+from ..String import String
+
+print("load " + __file__.split('/')[-1])
 
 class filelike():
     def __init__(self, c):
         self.c = c 
 
     def write(self, msg):
         msg = msg.strip()
```

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/ResizeImage.py` & `bagbag-0.59.0/src/bagbag/Funcs/ResizeImage_src.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from PIL import Image
 
+print("load " + __file__.split('/')[-1])
+
 def ResizeImage(src:str, dst:str, width:int, quality:int=95):
     img = Image.open(src)
 
     w, h = img.size
     # print('Befor resize (w,h): ' + str((w,h)))
 
     if w > width:
```

### Comparing `bagbag-0.58.9/src/bagbag/Funcs/Wget.py` & `bagbag-0.59.0/src/bagbag/Funcs/Wget_src.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import urllib.parse as urlparse
 import time 
 import requests
 import tqdm
 
+print("load " + __file__.split('/')[-1])
+
 def download_file(url, dest):
     with requests.get(url, stream=True) as response:
         response.raise_for_status()
         total_size_in_bytes= int(response.headers.get('content-length', 0))
         chunk_size=8192
         progress_bar = tqdm.tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
         with open(dest, 'wb') as f:
```

### Comparing `bagbag-0.58.9/src/bagbag/Hash.py` & `bagbag-0.59.0/src/bagbag/Hash/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import hashlib
     
+print("load hash")
 
 def Md5sum(data:str|bytes) -> str:
     if type(data) == str:
         data = data.encode('utf-8')
     return hashlib.md5(data).hexdigest()
 
 def Md5sumFile(fpath:str, block_size=2**20) -> str:
```

### Comparing `bagbag-0.58.9/src/bagbag/Http.py` & `bagbag-0.59.0/src/bagbag/Http/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from urllib3.exceptions import InsecureRequestWarning
 from requests_toolbelt.utils import dump
 
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
 from io import BytesIO, SEEK_SET, SEEK_END
 
-try:
-    from .String import String
-except:
-    from String import String
+from ..String import String
 
 from random_user_agent.user_agent import UserAgent as useragent_generator
 from random_user_agent.params import SoftwareName as useragent_softwarename
 from random_user_agent.params import OperatingSystem as useragent_operatingsystem 
 
 useragents = useragent_generator(
     software_names=[
@@ -32,14 +29,16 @@
         useragent_operatingsystem.FREEBSD.value,
     ],
     limit=50
 ).get_user_agents()
 
 import random
 
+print("load http")
+
 class responseStream(object):
     def __init__(self, request_iterator):
         self._bytes = BytesIO()
         self._iterator = request_iterator
 
     def _load_all(self):
         self._bytes.seek(0, SEEK_END)
```

### Comparing `bagbag-0.58.9/src/bagbag/Json.py` & `bagbag-0.59.0/src/bagbag/Json/src.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 
+print("load json")
+
 def Dumps(obj, indent=4, ensure_ascii=False) -> str:
     """
     It takes a Python object and returns a JSON string
     
     :param obj: The object to be serialized
     :param indent: This is the number of spaces to indent for each level. If it is None, that
     will insert newlines but won't indent the new lines, defaults to 4 (optional)
@@ -35,14 +37,15 @@
             for item in obj:
                 extract(item, arr, key)
         return arr
 
     values = extract(obj, arr, key)
     return values
 
+
 if __name__ == "__main__":
     j = Dumps({1: 3, 4: 5})
     print(j)
 
     d = Loads(j)
     print(d)
```

### Comparing `bagbag-0.58.9/src/bagbag/Lg.py` & `bagbag-0.59.0/src/bagbag/Lg.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Math.py` & `bagbag-0.59.0/src/bagbag/Math/src.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import string
 
+print("load math")
+
 class base62(object):
     """
     基于abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789共计62个ascii字符
     构建62进制编码, 实现正整型十进制数据字符编码和解码
     """
     def __init__(self):
         self.BASE_STR = string.digits + string.ascii_letters
```

### Comparing `bagbag-0.58.9/src/bagbag/Os/Path/__init__.py` & `bagbag-0.59.0/src/bagbag/Os/Path/src_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,9 +46,16 @@
     :return: The function `Suffix` takes a string argument `path` and returns the file extension of the
     file specified in the path. It does this by using the `os.path.splitext()` function to split the
     path into the file name and extension, and then returning the extension. Therefore, the function
     returns a string that represents the file extension of the file specified in the path.
     """
     return os.path.splitext(path)[1]
 
-if __name__ == "__main__":
-    print(Join("a", "b"))
+class Path:
+    Basedir
+    Join
+    Exists
+    NotExists
+    Uniquify
+    IsDir
+    Basename
+    Suffix
```

### Comparing `bagbag-0.58.9/src/bagbag/Os/__init__.py` & `bagbag-0.59.0/src/bagbag/Os/src.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-try:
-    from . import Path
-except:
-    import Path
-
-# 以上是作为包给其它程序调用的时候要的, 例如Os.Path.Exists()
-
 import os
 import sys 
 import shutil
 import glob
 import subprocess
 
+print("load os")
+
 def Exit(num:int=0):
     sys.exit(num)
 
 def System(cmd:str) -> int:
     return subprocess.call(cmd, stderr=sys.stderr, stdout=sys.stdout, shell=True)
 
 def Mkdir(*path:str):
```

### Comparing `bagbag-0.58.9/src/bagbag/Process.py` & `bagbag-0.59.0/src/bagbag/Process/src.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import multiprocessing 
 from typing import Any
 
+## print("load process")
+
 def Process(func, *args:Any, daemon:bool=True) -> multiprocessing.Process:
     """
     注意调用这个函数的时候要放到if __name__ == "__main__"里面, 否则可能会报错
     
     `Process` is a function that takes a function and its arguments, and returns a
     `multiprocessing.Process` object that runs the function in a separate process. 
     
@@ -25,14 +27,8 @@
 # 
 # def p(s:str, ss:str):
 #     while True:
 #         time.sleep(1)
 #         print(s, ss, time.time())
 
 if __name__ == "__main__":
-    p = Process(p, "oo", "kk")
-
-    while True:
-        time.sleep(1)
-
-
-
+    pass
```

### Comparing `bagbag-0.58.9/src/bagbag/Python.py` & `bagbag-0.59.0/src/bagbag/Python/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Iterable
 
+## print("load python")
+
 def Range(startOrEnd:int, end:int=None) -> Iterable:
     """
     If the second argument is provided, return a range from the first argument to the second argument,
     otherwise return a range from 0 to the first argument.
     If the second argument is smaller than the first argument, the range will be reverse.
     
     :param startOrEnd: The first number in the range. If end is not specified, this is the last number
```

### Comparing `bagbag-0.58.9/src/bagbag/Random.py` & `bagbag-0.59.0/src/bagbag/Random/src.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import random 
 from typing import Any
 import copy
 
+print("load random")
+
 def Int(min:int, max:int) -> int:
     return random.randint(min, max)
 
 def Choice(obj:list|str) -> Any:
     return random.choice(obj)
 
 def String(length:int=8, charset:str="abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789") -> str:
```

### Comparing `bagbag-0.58.9/src/bagbag/Socket/TCP.py` & `bagbag-0.59.0/src/bagbag/Socket/TCP/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from __future__ import annotations
 
 import socket
 
-import sys 
-sys.path.append("..")
-try:
-    from bagbag.Tools import Chan
-    from bagbag.Thread import Thread 
-except:
-    from Tools import Chan
-    from Thread import Thread
+from ...Tools import Chan
+from ...Thread import Thread 
 
 import typing 
 import msgpack
 # import pickle
 
+print("tcp load")
+
 class StreamClosedError(Exception):
     pass
 
 class TCPPeerAddress():
     def __init__(self, host:str, port:int):
         self.Host = host 
         self.Port = port
```

### Comparing `bagbag-0.58.9/src/bagbag/String.py` & `bagbag-0.59.0/src/bagbag/String/src.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-from bagbag import Tools
 
-import re
-import langid
-import opencc
-import ipaddress
-import pypinyin
-from urllib.parse import quote_plus, unquote
-from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
-from collections import OrderedDict
-
-from lxml import etree, html
-import bs4
 
-import validators
-import tld
 
-sentimentAnalyzer = SentimentIntensityAnalyzer()
 
-addrPattern = OrderedDict({
+
+
+## print("load string")
+
+sentimentAnalyzer = None
+
+addrPattern = {
     "xmr":      "4[0-9AB][1-9A-HJ-NP-Za-km-z]{93}",
     "bech32":   "bc(0([ac-hj-np-z02-9]{39}|[ac-hj-np-z02-9]{59})|1[ac-hj-np-z02-9]{8,87})",
     "eth":      "(0x)[a-zA-Z0-9]{40}",
     "btc":      "(bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39}",
     "zec":      "(t)[a-zA-Z0-9]{34}",
     "btg":      "([GA])[a-zA-HJ-NP-Z0-9]{24,34}",
     "dash":     "X[1-9A-HJ-NP-Za-km-z]{33}",
@@ -59,15 +50,15 @@
     'avalanche': '(X|P)-[A-Za-z0-9]{43}',
     'ronin': 'ronin:[0-9a-fA-F]{42}:',
     'hive': '(STM|HIVE)[A-Za-z0-9]{44}',
     'harmony': 'one1[abcdefghijklmnopqrstuvwxyz0123456789]{38}',
     'bitcoincash': '[bitcoincash:]{0,12}(?:[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{42}|(?:[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{6,7}|[ac-hj-np-z]{1}[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{25,33})|[bc]1[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{39})', 
     'cosmos': 'cosmos1[a-z0-9]{38}',
     'polkadot': '5[1-5][a-km-zA-HJ-NP-Z1-9]{24,25}', 
-})
+}
 
 emailPattern = r'[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}'
 
 class cryptoAddress():
     def __init__(self, ctype:str, address:str) -> None:
         self.Type:str = ctype 
         self.Address = address
@@ -97,14 +88,19 @@
     
         """
         > If there are any Chinese characters in the string, return `True`. Otherwise, return `False`
         :return: A boolean value.
         """
     
     def Sentiment(self) -> sentimentResult:
+        global sentimentAnalyzer
+        if sentimentAnalyzer == None:
+            from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
+            sentimentAnalyzer = SentimentIntensityAnalyzer()
+
         res = sentimentAnalyzer.polarity_scores(self.string)
         # {'neg': 0.189, 'neu': 0.811, 'pos': 0.0, 'compound': -0.8331}
 
         resr = sentimentResult()
         resr.Negative = res['neg']
         resr.Neutral = res['neu']
         resr.Positive = res['pos']
@@ -159,39 +155,44 @@
 
         for idx in range(len(resca)):
             resca[idx].Type = ','.join(resca[idx].Type)
 
         return resca
     
     def GetURL(self) -> list[str]:
+        import re
         urls = re.findall('(?:http|ftp|https|ssh|ftps|sftp)://(?:[-\w./]|(?:%[\da-fA-F]{2}/))+', self.string)
         urls = list(set(urls))
 
         return urls
     
     def IsASCII(self) -> bool:
         return self.string.isascii()
     
     def GetDomain(self) -> list[str]:
+        import validators
+        import tld
+        from ..Tools import URL
         dms = []
         for u in self.GetURL():
             try:
-                h = URL.URL(u).Parse().Host
+                h = URL(u).Parse().Host
             except:
                 continue 
             if h.strip() != "" and h.strip() not in dms and tld.get_tld(h.strip(), fix_protocol=True, fail_silently=True) != None:
                 dms.append(h.strip())
         
         for i in self.string.split():
             if validators.domain(i) == True and tld.get_tld(i, fix_protocol=True, fail_silently=True) != None and i.strip() not in dms:
                     dms.append(i.strip())
         
         return dms
     
     def GetFirstLevelDomain(self) -> str | list[str]:
+        import tld
         res = []
         for dm in self.GetDomain():
             r = tld.get_fld(dm, fix_protocol=True, fail_silently=True)
             if r != None:
                 res.append(r)
         
         if len(res) == 0:
@@ -199,30 +200,34 @@
         elif len(res) == 1:
             return res[0]
         else:
             return res
 
 
     def HasChinese(self) -> bool:
+        import re
         return len(re.findall(r'[\u4e00-\u9fff]+', self.string)) != 0
     
     def Language(self) -> str:
         """
         The function takes a string as input and returns the language of the string
         :return: The language of the string.
         """
+        import langid
         return langid.classify(self.string)[0]
 
     def Repr(self) -> str:
         return str(repr(self.string).encode("ASCII", "backslashreplace"), "ASCII")[1:-1]
     
     def SimplifiedChineseToTraditional(self) -> str:
+        import opencc
         return opencc.OpenCC('s2t.json').convert(self.string)
     
     def TraditionalChineseToSimplified(self) -> str:
+        import opencc
         return opencc.OpenCC('t2s.json').convert(self.string)
     
     def Ommit(self, length:int) -> str:
         """
         If the length of the string is greater than the length of the argument, return the string up to
         the length of the argument and add "..." to the end. Otherwise, return the string
         
@@ -243,133 +248,163 @@
         
         return ''.join(res)
     
     def Len(self) -> int:
         return len(self.string)
     
     def PinYin(self) -> str:
+        import pypinyin
         res = pypinyin.lazy_pinyin(self.string, style=pypinyin.Style.TONE3)
         py = String(('-'.join(res)).replace(" ", "-")).Filter('1234567890qwertyuioplkjhgfdsazxcvbnmQWERTYUIOPLKJHGFDSAZXCVBNM -').replace('--', '-')
         return py
     
     def EnsureUTF8(self) -> str:
         return self.string.encode('utf-8', errors='ignore').decode('utf-8')
 
     def URLEncode(self) -> str:
+        from urllib.parse import quote_plus
         return quote_plus(self.string)
     
     def URLDecode(self) -> str:
+        from urllib.parse import unquote
         return unquote(self.string)
 
     def FormatHTML(self) -> str:
+        import bs4
+        from lxml import etree, html
         try:
             document_root = html.fromstring(self.string)
             return etree.tostring(document_root, encoding='unicode', pretty_print=True)
         except:
             soup = bs4.BeautifulSoup(self.string, 'html.parser')
             return soup.prettify()
     
     def IsURL(self, public:bool=False) -> bool:
+        import validators
         return validators.url(self.string, public=public) == True
 
     def IsDomain(self) -> bool:
+        import validators
+        import tld
         if validators.domain(self.string) == True:
             if tld.get_tld(self.string, fix_protocol=True, fail_silently=True) != None:
                 return True 
             
         return False
     
     def IsEmail(self) -> bool:
+        import validators
         return validators.email(self.string) == True 
     
     def IsIBAN(self) -> bool:
+        import validators
         return validators.iban(self.string) == True 
 
     def IsIPAddress(self) -> bool:
+        import ipaddress
         try:
             ipaddress.ip_address(self.string)
             return True 
         except ValueError:
             return False 
     
     def IsIPv4(self) -> bool:
+        import validators
         return validators.ipv4(self.string) == True
     
     def IsIPv4CIDR(self) -> bool:
         """
         Returns True if the string is a valid IPv4 CIDR notation, otherwise returns False
         
         >>> IsIPv4CIDR('1.1.1.1/8')
         True
         
         :return: True or False
         """
+        import validators
         return validators.ipv4_cidr(self.string) == True
 
     def IsIPv6(self) -> bool:
+        import validators
         return validators.ipv6(self.string) == True
     
     def IsIPv6CIDR(self) -> bool:
+        import validators
         """
         Returns True if the string is a valid IPv6 CIDR notation, otherwise False
         
         >>> ipv6_cidr('::1/128')
         True
         
         :return: True or False
         """
         return validators.ipv6_cidr(self.string) == True
     
     def IsMacAddress(self) -> bool:
+        import validators
         return validators.mac_address(self.string) == True
 
     def IsUUID(self) -> bool:
+        import validators
         return validators.uuid(self.string) == True 
     
     def IsMD5(self) -> bool:
+        import validators
         return validators.md5(self.string) == True 
     
     def IsSHA1(self) -> bool:
+        import validators
         return validators.sha1(self.string) == True 
     
     def IsSHA224(self) -> bool:
+        import validators
         return validators.sha224(self.string) == True 
     
     def IsSHA256(self) -> bool:
+        import validators
         return validators.sha256(self.string) == True 
     
     def IsSHA512(self) -> bool:
+        import validators
         return validators.sha512(self.string) == True 
     
     def IsJCBCardNumber(self) -> bool:
+        import validators
         """
         It checks if the card number is a JCB card number.
         :return: True or False
         """
         return validators.jcb(self.string) == True 
     
     def IsDinersClubCardNumber(self) -> bool:
+        import validators
         return validators.diners(self.string) == True 
     
     def IsMastercardCardNumber(self) -> bool:
+        import validators
         return validators.mastercard(self.string) == True 
 
     def IsUnionpayCardNumber(self) -> bool:
+        import validators
         return validators.unionpay(self.string) == True 
 
     def IsUnionpayCardNumber(self) -> bool:
+        import validators
         return validators.unionpay(self.string) == True 
     
     def IsAmericanExpressCardNumber(self) -> bool:
+        import validators
         return validators.amex(self.string) == True 
 
     def IsVisaCardNumber(self) -> bool:
+        import validators
         return validators.visa(self.string) == True
     
     def RegexFind(self, pattern:str, multiline=False) -> list[list[str]]:
+        import re
         res = []
 
         pattern1 = ""
         lasti = ""
         for idx in range(len(pattern)):
             i = pattern[idx]
             pattern1 = pattern1 + i
@@ -417,14 +452,15 @@
                     t = list()
                     t.append(i)
                     res.append(t)
 
         return res 
     
     def RegexReplace(self, pattern:str, string:str) -> str:
+        import re
         return re.sub(pattern, string, self.string)
 
 if __name__ == "__main__":
     print(1, String("ABC").HasChinese())
     print(2, String("ddddd中kkkkkkk").HasChinese())
     print(3, String("\"wef\t测\b试....\n\tffef'").Repr())
     print(4, String("这是一段用鼠标写的简体中文").SimplifiedChineseToTraditional())
```

### Comparing `bagbag-0.58.9/src/bagbag/Time.py` & `bagbag-0.59.0/src/bagbag/Time/src.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import time
 import datetime
 import tqdm
 from dateutil.parser import parse as dateparser
 from dateutil.parser import ParserError
 
-try:
-    from .String import String
-except:
-    from String import String
+from ..String import String
+
+print("load time")
 
 def FormatDuration(seconds:int) -> str:
     return time.strftime("%H:%M:%S", time.gmtime(seconds))
 
 Now = time.time 
 
 def Sleep(num:int=0, title:str=None, bar:bool=None):
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Argparser.py` & `bagbag-0.59.0/src/bagbag/Tools/Argparser_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 import argparse
 
 class Argparser():
     def __init__(self, description:str=None) -> None:
         self.parser = argparse.ArgumentParser(description=description)
 
     def Add(self, arg:str, help:str=None) -> Argparser:
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice.py` & `bagbag-0.59.0/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from bagbag import Http, Json, Time, Tools, String
-import typing 
+from .... import Http, Json, Time, Tools, String
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 # https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md
 
 class CoinsPairPrice():
     def __init__(self, pair:str, price:float, time:float) -> None:
         self.Pair:str = pair 
         self.Price:float = price  
@@ -22,15 +23,15 @@
     global servertime 
     if servertime == None:
         servertime = Json.Loads(Http.Get("https://api.binance.com/api/v3/time").Content)['serverTime'] / 1000
     timegap = Time.Now() - servertime
 
     return Time.Now() - timegap
 
-def GetPrice(pair:str|list=None) -> CoinsPairPrice | list[CoinsPairPrice]:
+def GetPrice(pair:str|list="BTCUSDT") -> CoinsPairPrice | list[CoinsPairPrice]:
     """
     The function `GetPrice` retrieves the current price of a specified cryptocurrency pair or a list of
     pairs from the Binance API.
     
     :param pair: For example: BTCUSDT. The trading pair(s) for which you want to retrieve the current price(s). 
     It can be a string for a single pair or a list of strings for multiple pairs. If no pair is specified, the
     function will return the prices for all available trading pairs
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/OfficalAccountVertify.py` & `bagbag-0.59.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from bagbag import Http
+from ..... import Http
+
 import json
 import uuid
 import time
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 url = 'https://www.binance.com/bapi/composite/v1/public/official-channel/verify'
 
 def Twitter(account:str, waiteOnRateLimit:bool=True) -> bool:
     tu = f"https://twitter.com/{account}"
     data = {"content": tu}
 
     while True:
@@ -31,8 +34,8 @@
     if len(c["data"]['data']) == 0:
         return False 
     
     for d in c['data']['data']:
         if d['content'] == tu:
             return True 
     
-    return False 
+    return False
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/BlockChain/Tron/tron.py` & `bagbag-0.59.0/src/bagbag/Tools/BlockChain/Tron/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import tronpy
 from tronpy import Tron as TronAPI
 from tronpy.providers import HTTPProvider
 
 import traceback
 
-from bagbag import Http, Json, String, Lg, Time, Random
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
+from .... import Http, Json, String, Lg, Time, Random
 
 tronOfficialNodes = [
     '3.225.171.164',
     '52.53.189.99',
     '18.196.99.16',
     '34.253.187.192',
     '35.180.51.163',
@@ -583,14 +585,19 @@
         if blockNumber == None:
             block = self.tron.get_latest_block()
         else:
             block = self.tron.get_block(blockNumber)
         # Lg.Trace(block)
         return tronBlock(block, self)
 
+# class Tron:
+#     TronClient
+#     TronContract
+#     TronAsset
+
 if __name__ == "__main__":
     # tttt = TronClient("http://13.124.62.58:8090")
     # bdf = tttt.Block(48311298)
     # Lg.Trace(bdf)
     # txs = bdf.Transcations()
     # for tx in txs:
     #     if tx.TxID == '8e055811c777cd0cf5ec2b74f79a2cb4f1aaf143011e9afe468760d654f86465':
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/CSV.py` & `bagbag-0.59.0/src/bagbag/Tools/CSV.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import csv 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class Reader():
     def __init__(self, fpath:str, withHeader:bool=True):
         self.fpath = fpath 
         self.fd = open(self.fpath)
         self.csvrd = csv.reader(self.fd, delimiter=',', quotechar='"', escapechar='\\')
         self.withHeader = withHeader
         if self.withHeader:
@@ -75,14 +77,18 @@
 
     def Close(self):
         self.fd.close()
     
     def Flush(self):
         self.fd.flush()
 
+class CSV:
+    Reader
+    Writer
+
 if __name__ == "__main__":
     w = Writer("test.csv")
 
     w.SetHeaders("h1", "h2")
 
     w.Write({"h1": "v1", "h2": '"v2,kkk|'})
     w.Write({"h1": "v,1", "h2": '"v222'})
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Chan.py` & `bagbag-0.59.0/src/bagbag/Tools/Chan_src.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class ChannelClosed(ChannelException):
     pass 
 
 class NoNewItem(ChannelException):
     pass 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 # > A `Chan` is a thread-safe queue with a `Size` method
 class Chan(Generic[_T]):
     def __init__(self, size=1) -> None:
         self.q = queue.Queue(maxsize=size)
         self.closed = False 
     
     def Size(self) -> int:
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/ComputerVision.py` & `bagbag-0.59.0/src/bagbag/Tools/ComputerVision.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,26 @@
 import types
 import typing
 import time
 import os
 import copy
 import flask
 
-try:
-    from ..Thread import Thread
-    from .. import Time
-    from .Ratelimit import RateLimit
-    from .. import Socket
-    from ..String import String
-    from .. import Lg
-    from .. import Base64
-    from .. import Http
-    from .. import Json
-    from .. import Random
-except:
-    import sys 
-    sys.path.append("..")
-    from Thread import Thread
-    import Time
-    from Ratelimit import RateLimit
-    import Socket
-    from String import String
-    import Lg
-    import Base64
-    import Http
-    import Json
-    import Random
+from ..Thread import Thread
+from .. import Time
+from .Ratelimit_src import RateLimit
+from .. import Socket
+from ..String import String
+from .. import Lg
+from ..Base64 import src
+from .. import Http
+from .. import Json
+from .. import Random
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 netssd = None 
 classesssd = ["background", "aeroplane", "bicycle", "bird", "boat",
     "bottle", "bus", "car", "cat", "chair", "cow", "diningtable",
     "dog", "horse", "motorbike", "person", "pottedplant", "sheep",
@@ -272,28 +260,34 @@
         detections = netyolo.forward(output_layers)
 
         return cvStreamFrameObjectDetectionResult(detections, self.objectDetectModel, self.frame)
 
     def objectsByAPIServer(self) -> cvStreamFrameObjectDetectionResult:
         (flag, encodedImage) = cv2.imencode(".jpg", self.frame)
         encodedImage = bytearray(encodedImage)
-        encodedImage = Base64.Encode(encodedImage)
+        encodedImage = src.Encode(encodedImage)
 
         a = self.objectDetectModel.split("|")
         server = a[1]
         model = a[2]
 
         if not server.startswith("http://") and not server.startswith("https://"):
             server = "https://" + server 
 
         while True:
-            resp = Http.PostJson(server + "/object-detect", {
-                "model": model,
-                "data": encodedImage,
-            }, timeout=60)
+            try:
+                resp = Http.PostJson(server + "/object-detect", {
+                    "model": model,
+                    "data": encodedImage,
+                }, timeout=60)
+                break
+            except Exception as e:
+                Lg.Warn("调用API服务器识别失败:", e)
+                Time.Sleep(5)
+                pass 
 
             if resp.StatusCode > 500:
                 Lg.Warn("调用API服务器识别失败: " + str(resp.StatusCode))
                 Time.Sleep(1)
                 Lg.Trace("重试")
             elif resp.StatusCode == 500:
                 raise Exception("调用API服务器识别失败: " + str(resp.StatusCode))
@@ -782,15 +776,18 @@
                 if self.FPSRead != None:
                     Time.Sleep(1/self.FPSRead)
                 else:
                     Time.Sleep(1/30)
                 continue
 
             encodedImage = encodedImage.tobytes()
-            tc.Send(encodedImage)
+            try:
+                tc.Send(encodedImage)
+            except:
+                break
 
             lastgettime = self.lastFrameUpdateTime
 
         tc.Close()
 
     def socketServer(self, ipaddr:str, port:int):
         for tc in Socket.TCP.Listen(ipaddr, port):
@@ -910,14 +907,20 @@
             self.writer.write(frame.frame) 
 
     def Close(self):
         if self.closed == False:
             self.closed = True 
             self.writer.release() 
 
+class ComputerVision:
+    VideoWriter
+    LoadImage
+    StreamAsync
+    StreamSync
+
 if __name__ == "__main__":
     import os
     import datetime 
     
     # web camera
     # stream = Stream("http://10.129.129.207:8080/video")
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Crontab.py` & `bagbag-0.59.0/src/bagbag/Tools/Crontab_src.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 try:
     from ..Thread import Thread
 except:
     import sys 
     sys.path.append("..")
     from Thread import Thread
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class Crontab():
     def __init__(self):
         Thread(self.run)
 
     def run(self):
         while True:
             schedule.run_pending()
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Database.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from . import orator
-    from .Lock import Lock
-    from .. import Lg
-    from .. import Base64
-    from .. import Time 
-    from .Redis import redisKey
+    from ..Lock_src import Lock
+    from ... import Lg
+    from ... import Base64
+    from ... import Time 
+    from ..Redis_src import redisKey
 except:
     import orator
-    from Lock import Lock
+    from Lock_src import Lock
     import sys
-    sys.path.append("..")
+    sys.path.append("...")
     import Lg
     import Base64
     import Time 
 
 import pickle
 import typing
 import bagbag
@@ -867,14 +869,15 @@
             }
         }
         self.db = orator.DatabaseManager(config)
         self.schema = orator.Schema(self.db)
         self.driver = "sqlite"
         self.lock = Lock()
 
+
 if __name__ == "__main__":
     # db = SQLite("data.db")
     # tbl = db.Table("test_tbl").AddColumn("string", "string").AddColumn("int", "string").AddIndex("int")
     # tbl.Data({"string":"string2", "int": 2}).Insert()
     # c = tbl.Where("string", "=", "string2").Count()
     # print(c)
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/DistributedLock.py` & `bagbag-0.59.0/src/bagbag/Tools/DistributedLock_src.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 #     restart: always
 #     #ports:
 #     #   - "8888:8888" 
 #     environment:
 #       PASSWORD: password
 #       DEBUG: "False"
 
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from .. import Time
     from .. import Http
     from ..Thread import Thread
     from .. import Lg
 except:
     import sys
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Elasticsearch.py` & `bagbag-0.59.0/src/bagbag/Tools/Elasticsearch_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 except:
     import sys 
     sys.path.append("..")
     import Http, Lg
 
 # requests.exceptions.ReadTimeout
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 def retryOnNetworkError(func): # func是被包装的函数
     def ware(self, *args, **kwargs): # self是类的实例
         while True:
             try:
                 res = func(self, *args, **kwargs)
                 break
             except requests.exceptions.ReadTimeout as e:
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Github.py` & `bagbag-0.59.0/src/bagbag/Tools/Github_src.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from github import Github as githubclient
 from github.GithubException import RateLimitExceededException
 from github.GithubException import GithubException
 
 try:
     from .. import Http
-    from .Ratelimit import RateLimit
+    from .Ratelimit_src import RateLimit
     from ..String import String
     from .. import Time
     from .. import Lg
 except:
-    from Ratelimit import RateLimit
+    from Ratelimit_src import RateLimit
     import sys
     sys.path.append("..")
     import Http
     from String import String
     import Time
     import Lg
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 import typing
 
 # class GithuException(Exception):
 #     pass 
 
 # class NoNewItem(GithuException):
 #     pass
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/JavaScript.py` & `bagbag-0.59.0/src/bagbag/Tools/JavaScript_src.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import js2py
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class JavaScript():
     def __init__(self) -> None:
         pass
 
     def Eval(self, code:str):
         """
         Just like javascript eval. Translates javascript to python, executes and returns python object. js is javascript source code
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Kafka.py` & `bagbag-0.59.0/src/bagbag/Tools/Kafka_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from kafka import KafkaProducer as kkp
 from kafka import KafkaConsumer as kkc
 import json
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class kafkaProducer():
     def __init__(self, topic:str, servers:str|list, value_serializer):
         self.kp = kkp(bootstrap_servers=servers, value_serializer=value_serializer)
         self.topic = topic
     
     def Send(self, data:dict):
         self.kp.send(self.topic, data)
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Lock.py` & `bagbag-0.59.0/src/bagbag/Tools/Lock_src.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import multiprocessing
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 # > The `Lock` class is a wrapper around the `multiprocessing.Lock` class
 class Lock():
     def __init__(self):
         self.lock = multiprocessing.Lock()
         self.islocked = False
     
     def Acquire(self, block:bool=True) -> bool:
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/MatrixBot.py` & `bagbag-0.59.0/src/bagbag/Tools/MatrixBot_src.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 #       - /data/cr-volumes/matrix-bot/data:/data
 # 备注:
 # 版本0.0.1
 #     arm64的可以调用http api发送消息, 也可以收消息(发送id给bot返回房间号)
 #     amd64的可以调用http api发送消息, 但是不能收消息, 一脸蒙逼
 #     
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from .. import Http
-    from .. import Base64
+    from ..Base64 import src
     from .. import Json
     from .. import Lg
 except:
     import sys
     sys.path.append("..")
     import Http 
     import Base64
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/OCR.py` & `bagbag-0.59.0/src/bagbag/Tools/OCR_src.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 #         ipv4_address: 192.168.168.63
 #     container_name: ocr-server-192.168.168.63
 #     restart: always
 #     ports:
 #       - 8990:8990
 # 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from .. import Http
-    from .. import Base64
+    from ..Base64 import src
     from .. import Json
 except:
     import sys 
     sys.path.append("..")
     import Http 
     import Base64
     import Json
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/ProgressBar.py` & `bagbag-0.59.0/src/bagbag/Tools/ProgressBar_src.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import tqdm
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class ProgressBarClass():
     def __init__(self, t:tqdm.tqdm):
         self.t = t 
     
     def Add(self, num:int=1):
         self.t.update(num)
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Prometheus/MetricServer.py` & `bagbag-0.59.0/src/bagbag/Tools/Prometheus/MetricServer.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import prometheus_client as pc
 
 try:
     from .metrics import * 
 except:
     from metrics import * 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 # It creates a Prometheus server that listens on the specified port and IP address.
 class MetricServer():
     def __init__(self, listen:str="0.0.0.0", port:int=9105):
         pc.start_http_server(port, listen)
     
     def NewCounter(self, name:str, help:str) -> PrometheusCounter:
         return PrometheusCounter(name, help)
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Prometheus/PushGateway.py` & `bagbag-0.59.0/src/bagbag/Tools/Prometheus/PushGateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import annotations
 
 import prometheus_client as pc
 import time
 import socket
 
-import threading 
+import threading
+
+from ...Base64 import src 
 
 try:
     from .metrics import * 
+    from ... import Http, Tools, Lg
 except:
     from metrics import * 
+    import sys 
+    sys.path.append("...")
+    import Http, Tools, Lg, Base64
 
-from bagbag import Http, Tools, Lg, Base64
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class PushGateway():
     def __init__(self, job:str, address:str, basicAuthUser:str=None, basicAuthPass:str=None, pushinterval:int=15, instance:str=None):
         self.job = job 
         self.instance = instance if instance != None else socket.gethostname()
         self.address = address 
         self.registry = pc.CollectorRegistry()
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Prometheus/metrics.py` & `bagbag-0.59.0/src/bagbag/Tools/Prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Queue.py` & `bagbag-0.59.0/src/bagbag/Tools/Queue_src.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 #       MYSQL_DATABASE: "queue"
 
 #       # SQLITE_PATH: /data/queue.db
 
 #     # volumes:
 #     #   - /data/cr-volumes/queue-server/data:/data
     
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 try:
     from .. import Http
-    from .. import Base64
+    from ..Base64 import src
     from .. import Lg
 except:
     import sys
     sys.path.append("..")
     import Http
     import Base64
     import Lg
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/RSS/Feed.py` & `bagbag-0.59.0/src/bagbag/Tools/RSS/Feed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import feedparser
 import markdownify
 import requests
 
-from bagbag import Time
+try:
+    from ... import Time
+except:
+    import sys 
+    sys.path.append("...")
+    import Time
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class rssPage():
     def __init__(self):
         self.Title:str = ""
         self.URL:str = "" 
         self.Description:str = "" 
         self.Content:str = ""
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/RSS/Opml.py` & `bagbag-0.59.0/src/bagbag/Tools/RSS/Opml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import listparser
 import requests
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class rssFeed():
     def __init__(self, title:str, url:str):
         self.Title = title 
         self.URL = url
     
     def __str__(self) -> str:
         return f"RSSFeed(Title={self.Title} URl={self.URL})"
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Ratelimit.py` & `bagbag-0.59.0/src/bagbag/Tools/Ratelimit_src.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-try:
-    from .Lock import Lock
-    from .. import Time
-except:
-    from Lock import Lock
-    import sys
-    sys.path.append("..")
-    import Time 
+
+from .Lock_src import Lock
+from .. import Time
+
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class RateLimit:
     def __init__(self, rate:str, sleep:bool=True):
         """
         sleep=True的时候会添加一个sleep, 可以把请求平均在时间段内. 在低速率的时候能限制准确. 高速率例如每秒50次以上, 实际速率会降低, 速率越高降低越多. 
         sleep=False的时候没有sleep, 会全在一开始扔出去, 然后block住, 等下一个周期, 在需要速率很高的时候可以这样, 例如发包的时候, 一秒限制2000个包这样.
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Redis.py` & `bagbag-0.59.0/src/bagbag/Tools/Redis_src.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 import redis 
 import pickle
 import typing
 import time
 import shortuuid
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from .. import Lg
-    from .. import Base64
+    from ..Base64 import src
     from ..Process import Process
 except:
     import sys
     sys.path.append("..")
     import Lg
     import Base64
     from Process import Process
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/SSH.py` & `bagbag-0.59.0/src/bagbag/Tools/SSH_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import stat
 import paramiko
+from .. import Os
 
-try:
-    from .. import Os
-except:
-    import sys
-    sys.path.append("..")
-    import Os
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class SSH():
     def __init__(self, host:str, port:int=None, user:str=None, password:str=None, pkey:str=None) -> None:
         """
         If you have a password, use it; if you have a private key, use it; 
         if you have neither, 尝试从~/.ssh/config读取, 如果没有读取默认的~/.ssh/id_rsa
         如果都没有, 扔异常
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Selenium.py` & `bagbag-0.59.0/src/bagbag/Tools/Selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,23 @@
 from seleniumwire import webdriver as seleniumwirewebdriver
 from seleniumwire.utils import decode as decodeResponseBody
 
 import time
 import random
 import typing
 
-try:
-    from ..Http import useragents 
-    from .. import Lg
-    from ..Thread import Thread
-    from .URL import URL
-    from ..String import String 
-    from .. import Os
-    from ..File import File
-except:
-    import sys 
-    sys.path.append("..")
-    from Http import useragents 
-    import Lg 
-    from Thread import Thread
-    from URL import URL
-    from String import String 
-    import Os
-    from File import File
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
+from ..Http import useragents 
+from .. import Lg
+from ..Thread import Thread
+from .URL_src import URL
+from ..String import String 
+from .. import Os
+from .File_src import File
 
 seleniumChromeWireSkipFilesSuffix = (
     # 图片
     '.png', 
     '.jpg', 
     '.gif', 
     '.jpeg', 
@@ -319,16 +310,16 @@
                     time.sleep(1)
                 else:
                     raise e 
 
         # import ipdb
         # ipdb.set_trace()
     
-    def Exists(self, xpath:str) -> bool:
-        return self.Find(xpath, timeout=0) != None
+    def Exists(self, xpath:str, timeout:int=0) -> bool:
+        return self.Find(xpath, timeout=timeout) != None
     
     def StatusCode(self) -> int:
         self.driver.stat
     
     def ResizeWindow(self, width:int, height:int):
         """
         :param width: The width of the window in pixels
@@ -674,16 +665,15 @@
 
 class ChromeWire(seleniumBase):
     def __init__(self, 
             blockSuffix:tuple[str]=seleniumChromeWireSkipFilesSuffix,
             maxRequests:int=None, 
             requestStorage:str="disk", # memory
             urlFilterRegex:list[str]=[], 
-            excludeHosts:list[str]=[], 
-            PACFileURL:str=None, 
+            excludeHosts:list[str]=[],
             httpProxy:str=None, 
             sessionID=None, 
             randomUA:bool=True,
             userAgent:str=None):
         
         """
         :param blockSuffix: A tuple of file suffixes to block. list是中括号, tuple是小括号
@@ -692,16 +682,14 @@
         :type maxRequests: int
         :param requestStorage: The storage type for requests and responses. Can be either memory or disk, defaults to disk
         :type requestStorage: str (optional)
         :param urlFilterRegex: A list of regular expressions that will be used to filter requests
         :type urlFilterRegex: list[str]
         :param excludeHosts: A list of hosts to exclude from interception
         :type excludeHosts: list[str]
-        :param PACFileURL: The URL of the PAC file to use
-        :type PACFileURL: str
         :param httpProxy: The HTTP proxy to use
         :type httpProxy: str
         :param sessionID: If you want to use an existing session, you can pass the session ID here
         :param randomUA: Whether to use a random user agent, defaults to True
         :type randomUA: bool (optional)
         """
 
@@ -722,33 +710,36 @@
         elif randomUA:
             options.add_argument('--user-agent=' + random.choice(useragents)['user_agent'] + '')
         self.randomUA = randomUA
         self.userAgent = userAgent
 
         options.add_experimental_option("excludeSwitches", ["enable-automation"])
 
-        if PACFileURL:
-            options.add_argument("--proxy-pac-url=" + PACFileURL)
-        elif httpProxy:
-            options.add_argument('--proxy-server=' + httpProxy)
-
         seleniumwire_options = {
             # 'request_storage': 'memory',  # Store requests and responses in memory only
             # 'request_storage_max_size': maxRequests  # Store no more than 100 requests in memory
         }
 
         if maxRequests != None:
             seleniumwire_options['request_storage_max_size'] = maxRequests
 
         if requestStorage == "memory":
             seleniumwire_options['request_storage'] = requestStorage
 
         if excludeHosts != []:
             seleniumwire_options['exclude_hosts'] = excludeHosts
         
+        if httpProxy != None:
+            seleniumwire_options['proxy'] = {
+                'http': httpProxy,
+                # 'https': httpProxy
+            }
+        
+        # Lg.Trace(seleniumwire_options)
+        
         self.driver = seleniumwirewebdriver.Chrome(
             options=options,
             seleniumwire_options=seleniumwire_options
         )
 
         if self.driver.scopes != []:
             self.driver.scopes = urlFilterRegex
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Telegram.py` & `bagbag-0.59.0/src/bagbag/Tools/Telegram_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,36 @@
 from telethon.tl.types import  InputMessagesFilterVoice
 import tqdm
 
 from hachoir.metadata import extractMetadata
 from hachoir.parser import createParser
 from telethon.tl.types import DocumentAttributeVideo
 
-from bagbag import Funcs
-
 try:
     from .. import Os
-    from .Database import SQLite
+    from .Database_src import SQLite
     from .. import Time
     from .. import Lg
     from ..String import String
-    from ..File import File
-    from .Ratelimit import RateLimit
+    from .File_src import File
+    from .Ratelimit_src import RateLimit
+    from .. import Funcs
 except:
     import sys 
     sys.path.append("..")
     import Os
-    from Database import SQLite
+    from Database_src import SQLite
     import Time
     import Lg
     from String import String
-    from File import File
-    from Ratelimit import RateLimit
+    from File_src import File
+    from Ratelimit_src import RateLimit
+    import Funcs
+
+print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class TelegramGeo():
     def __init__(self):
         self.Long = None
         self.Lat = None 
         self.AccessHash = None
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/TelegramAsync.py` & `bagbag-0.59.0/src/bagbag/Tools/TelegramAsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 import telethon
 from telethon import utils
 from telethon import types
 import time
 # import ipdb
 from typing import List
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from .. import Os
-    from .Database import SQLite
+    from .Database_src import SQLite
 except:
     import sys 
     sys.path.append("..")
     import Os
-    from Database import SQLite
+    from Database_src import SQLite
 
 class TelegramGeoAsync():
     def __init__(self):
         self.Long = None
         self.Lat = None 
         self.AccessHash = None
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/TelegramBot.py` & `bagbag-0.59.0/src/bagbag/Tools/TelegramBot_src.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 try:
     from .. import Http
     from .. import Time
     from .. import Lg
-    from .. import Base64
-    from ..File import File
+    from ..Base64 import src
+    from ..File_src import File
     from .. import Funcs
 except:
     import sys
     sys.path.append("..")
 
     import Http
     import Time
     import Lg
     import Base64
-    from File import File
+    from File_src import File
     import Funcs
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 import msgpack
 import os
 
 # 配合这个镜像使用
 # 
 # version: '3'
 # services:
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/TelegramBotOfficial.py` & `bagbag-0.59.0/src/bagbag/Tools/TelegramBotOfficial_src.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import telebot # https://github.com/eternnoir/pyTelegramBotAPI
 
 try:
-    from .Ratelimit import RateLimit
-    from .Lock import Lock 
-    from .DistributedLock import DistributedLock
+    from .Ratelimit_src import RateLimit
+    from .Lock_src import Lock 
+    from .DistributedLock_src import DistributedLock
     from .. import Lg
 except:
-    from Ratelimit import RateLimit
-    from Lock import Lock
-    from DistributedLock import DistributedLock
+    from Ratelimit_src import RateLimit
+    from Lock_src import Lock
+    from DistributedLock_src import DistributedLock
     import sys
     sys.path.append("..")
     import Lg
 
 import time
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class TelegramBotOfficial():
     def __init__(self, token:str, ratelimit:str="20/m", lock:Lock|DistributedLock=None):
         """
         :param token: The token of your bot
         :type token: str
         :param ratelimit: The ratelimit for the bot. This is a string in the format of "x/y" where x is
         the number of messages and y is the time period. For example, "20/m" means 20 messages per
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Translater.py` & `bagbag-0.59.0/src/bagbag/Tools/Translater_src.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     import Http
     import Lg
     import Random
     import Hash
     import Json
     from Http import useragents 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 import pygtrans
 
 class Baidu():
     def __init__(self, appid:str, secretkey:str) -> None:
         self.appid = appid 
         self.secretkey = secretkey 
         self.apiurl = "http://api.fanyi.baidu.com/api/trans/vip/translate"
@@ -120,14 +122,19 @@
         except Exception as e:
             Lg.Trace(res.Content)
             Lg.Error("载入返回内容错误")
             raise e
         
         return res["translation"][0]
 
+class Translater:
+    NLLB
+    Google
+    Baidu
+
 if __name__ == "__main__":
     # appid, secretkey = open("baidu.ident").read().strip().split(',')
     # b = Baidu(appid, secretkey).SetLang("zh", "auto")
     # text = b.Translate("This is a test")
     # Lg.Trace(text)
 
     # g = Google("http://192.168.1.186:8899").SetLang("zh-CN")
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Twitter/Elevated.py` & `bagbag-0.59.0/src/bagbag/Tools/Twitter/Elevated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import tweepy
 import typing 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class twitterUser():
     def __init__(self) -> None:
         self.ID:int = None 
         self.Name:str = None 
         self.ScreenName:str = None 
         self.Location:str = None 
         self.RegisterTime:int = None
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Twitter/Essential.py` & `bagbag-0.59.0/src/bagbag/Tools/Twitter/Essential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tweepy
 import typing 
 
 tweetFields = ['author_id', 'created_at', 'geo', 'id', 'lang', 'text']
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class twitterTweet():
     def __init__(self) -> None:
         self.ID:int = None
         self.Time:int = None 
         self.Text:str = None 
         self.Language:str = None
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/URL.py` & `bagbag-0.59.0/src/bagbag/Tools/URL_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from urllib.parse import urlparse, quote_plus, unquote
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class URLParseResult():
     def __init__(self, Schema:str, Host:str, Port:int, User:str, Pass:str, Path:str, Query:str, Fragment:str):
         self.Schema = Schema
         self.Host = Host    
         self.Port = Port    
         self.User = User    
         self.Pass = Pass
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/WebCrawler.py` & `bagbag-0.59.0/src/bagbag/Tools/WebCrawler_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 # from bagbag import Tools, String, Range, Funcs, Hash, Os, Lg
 import typing 
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 try:
     from .. import Tools
     from .. import String
     from ..Python import Range 
     from .. import Funcs 
     from .. import Hash 
     from .. import Os
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/WebServer.py` & `bagbag-0.59.0/src/bagbag/Tools/WebServer_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 except:
     import sys 
     sys.path.append("..")
     import Random
     from Thread import Thread
     import Lg
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 import logging 
     
 class LoggingMiddleware(object):
     def __init__(self, app):
         self._app = app
 
     def __call__(self, env, resp):
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/XPath.py` & `bagbag-0.59.0/src/bagbag/Tools/XPath_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 import lxml.html 
 
 class XPath():
     def __init__(self, html:str|lxml.html.HtmlElement):
         if type(html) == str:
             self.root = lxml.html.fromstring(html)
         elif type(html) == lxml.html.HtmlElement:
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/Xlsx.py` & `bagbag-0.59.0/src/bagbag/Tools/Xlsx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import openpyxl
 import os
 
+print("load " + '/'.join(__file__.split('/')[-2:]))
+
 class Reader():
     def __init__(self, fpath:str):
         self.fpath = fpath 
         self.wb = openpyxl.load_workbook(filename=fpath)
         self.ws = self.wb.active
         self.iws = self.ws.iter_rows()
         self.headers = [j for j in filter(lambda x: x != None, [i.value for i in next(self.iws)])]
@@ -82,14 +84,18 @@
     
     def __exit__(self, exc_type, exc_value, traceback):
         try:
             self.Close()
         except:
             pass
 
+class Xlsx:
+    Reader
+    Writer
+
 if __name__ == "__main__":
     w = Writer("test.xlsx")
 
     w.SetHeaders("h1", "h2")
 
     w.Write({"h1": "v1", "h2": '"v2,kkk|'})
     w.Write({"h1": "v,1", "h2": '"v222'})
```

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/application.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/install_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/make_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/migrate_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/refresh_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/reset_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/rollback_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/status_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/make_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/make_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/seed_command.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection_interface.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connections/mysql_connection.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connections/postgres_connection.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connections/sqlite_connection.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connection_factory.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connector.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/mysql_connector.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/postgres_connector.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/sqlite_connector.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/database_manager.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/abstract_asset.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column_diff.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/comparator.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/exceptions/__init__.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/foreign_key_constraint.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/index.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/mysql_schema_manager.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/mysql_keywords.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/postgresql_keywords.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/sqlite_keywords.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql57_platform.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql_platform.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/platform.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/postgres_platform.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/sqlite_platform.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/postgres_schema_manager.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/schema_manager.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/sqlite_schema_manager.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table_diff.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/events/__init__.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/connectors.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/orm.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/database_migration_repository.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migration_creator.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migrator.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/stubs.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/builder.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/collection.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory_builder.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/mixins/soft_deletes.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/model.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to_many.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many_through.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one_or_many.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_many.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one_or_many.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_pivot.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to_many.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/pivot.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/relation.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/result.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/wrapper.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/soft_deleting.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/orm/utils.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/pagination/base.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/pagination/length_aware_paginator.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/pagination/paginator.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/builder.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/mysql_grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/postgres_grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/sqlite_grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/join_clause.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/mysql_processor.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/postgres_processor.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/processor.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/blueprint.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/builder.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/mysql_grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/postgres_grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/sqlite_grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/mysql_builder.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/schema/schema.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/seeds/seeder.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/support/fluent.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/support/grammar.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/utils/__init__.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/utils/command_formatter.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/utils/helpers.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/utils/qmarker.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/src/bagbag/Tools/orator/utils/url.py` & `bagbag-0.59.0/src/bagbag/Tools/Database/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.9/PKG-INFO` & `bagbag-0.59.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagbag
-Version: 0.58.9
+Version: 0.59.0
 Summary: An all in one python library
 Home-page: https://github.com/darren2046/bagbag
 License: MIT
 Keywords: base,library
 Author: Darren
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

