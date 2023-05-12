# Comparing `tmp/moneyonchain_prices_source-0.6.3.tar.gz` & `tmp/moneyonchain_prices_source-0.6.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.3.tar", last modified: Thu May 11 18:04:40 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.4b0.tar", last modified: Fri May 12 14:05:20 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.3.tar` & `moneyonchain_prices_source-0.6.4b0.tar`

### file list

```diff
@@ -1,62 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:04:40.840636 moneyonchain_prices_source-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-11 18:04:40.840636 moneyonchain_prices_source-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:04:40.832636 moneyonchain_prices_source-0.6.3/moc_prices_source/
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/cli_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/coins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/computed_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:04:40.832636 moneyonchain_prices_source-0.6.3/moc_prices_source/data/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/data/database_default.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/data/redis_default.json
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/data/weighing.json
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:04:40.836636 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/bnb_usdt_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_bitgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_bittrex.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_cex.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_itbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_okcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usdt_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usdt_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/coins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/engine_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/eth_btc_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/eth_btc_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/eth_btc_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_coinbene.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_mxc.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/my_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/to_db.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source/weighing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source_check
--rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/moc_prices_source_to_db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:04:40.840636 moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-11 18:04:40.000000 moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-11 18:04:40.000000 moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:04:40.000000 moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 18:04:40.000000 moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 18:04:40.000000 moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:04:40.840636 moneyonchain_prices_source-0.6.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1565 2023-05-11 18:04:30.000000 moneyonchain_prices_source-0.6.3/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 14:05:20.664843 moneyonchain_prices_source-0.6.4b0/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-05-12 14:05:20.664843 moneyonchain_prices_source-0.6.4b0/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 14:05:20.644842 moneyonchain_prices_source-0.6.4b0/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4392 2022-12-28 13:52:38.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1785 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 14:05:20.644842 moneyonchain_prices_source-0.6.4b0/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2169 2023-05-11 21:01:55.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 14:05:20.664843 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      552 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      550 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      552 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4361 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13390 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      549 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1485 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2022-12-28 13:53:38.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-05-11 20:54:21.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-05-11 20:27:59.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-05-11 20:52:38.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1485 2023-05-11 20:14:25.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-05-11 19:54:12.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        6 2023-05-11 20:00:09.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 14:05:20.664843 moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-05-12 14:05:20.000000 moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4485 2023-05-12 14:05:20.000000 moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-05-12 14:05:20.000000 moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-05-12 14:05:20.000000 moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-05-12 14:05:20.000000 moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-05-12 14:05:20.664843 moneyonchain_prices_source-0.6.4b0/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.4b0/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.3/PKG-INFO` & `moneyonchain_prices_source-0.6.4b0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: moneyonchain_prices_source
-Version: 0.6.3
-Summary: Prices source for MoC projects
-Author: Juan S. Bokser
-Author-email: juan.bokser@moneyonchain.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # MoC prices source
 
 Prices source for MoC projects
 
 
 
 ## Refrences
@@ -389,8 +376,8 @@
 >>> BTC_USD.from_.symbol
 'BTC'
 >>> BTC_USD.from_.name
 'Bitcoin'
 >>> BTC_USD.from_.small_symbol
 '₿'
 >>>
-```
+```
```

### Comparing `moneyonchain_prices_source-0.6.3/README.md` & `moneyonchain_prices_source-0.6.4b0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,383 +1,398 @@
-# MoC prices source
-
-Prices source for MoC projects
-
-
-
-## Refrences
-
-* [Source code in Github](https://github.com/money-on-chain/moc_prices_source)
-* [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
-
-
-
-## Requirements
-
-* Python 3.6+ support
-
-
-
-## Installation
-
-### From the Python package index (PyPI) 
-
-Run:
-
-```
-$ pip3 install moneyonchain-prices-source 
-```
-
-And then run:
-
-```
-$ moc_prices_source_check --version
-```
-
-To verify that it has been installed correctly
-
-### From source
-
-Download from [Github](https://github.com/money-on-chain/moc_prices_source)
-
-Standing inside the folder, run:
-
-```
-$ pip3 install -r requirements.txt 
-```
-
-For install the dependencies and then run:
-
-```
-$ pip3 install .
-```
-
-Finally run:
-
-```
-$ moc_prices_source_check --version
-```
-
-To verify that it has been installed correctly
-
-
-
-## Check that all is working ok
-
-```
-user@host:~$ moc_prices_source_check 
-
-From       To       Exchnage        Response  U.      Weigh     %  Time
----------  -------  ----------  ------------  ----  -------  ----  ------
-Bitcoin    Dollar   Bitfinex    15245         $        0.15  15.4  0.88s
-Bitcoin    Dollar   Bitstamp    15241.9       $        0.23  22.6  0.34s
-Bitcoin    Dollar   Coinbase    15236.5       $        0.4   40.3  0.27s
-Bitcoin    Dollar   Gemini      15246.8       $        0.06   6.4  0.87s
-Bitcoin    Dollar   Kraken      15239.4       $        0.15  15.2  0.4s
-RIF Token  Bitcoin  BitHumb         6.64e-06  ₿        0.33  33.3  3.09s
-RIF Token  Bitcoin  Coinbene        5.78e-06  ₿        0.33  33.3  1.27s
-RIF Token  Bitcoin  Kucoin          6.37e-06  ₿        0.33  33.3  1.16s
-
-Coin pair          Mediam             Mean    Weighted median  Sources
------------  ------------  ---------------  -----------------  ---------
-BTC/USD      15241.9       15241.9               15239.4       5
-RIF/BTC          6.37e-06      6.26333e-06           6.37e-06  3
-RIF/USD          0.097091      0.0954653             0.097075  N/A
-
-Response time 3.1s
-
-user@host:~$
-```
-
-More options
-
-```
-user@host:~$ moc_prices_source_check --help
-Usage: moc_prices_source_check [OPTIONS]
-
-Options:
-  -v, --version   Show version and exit.
-  -j, --json      Show data in JSON format and exit.
-  -w, --weighing  Show the default weighing and exit.
-  -h, --help      Show this message and exit.
-user@host:~$ 
-```
-
-
-## Usage
-
-Do some imports first
-
-```
-user@host:~$ python3
-Python 3.8.5 (default, Jul 28 2020, 12:59:40) 
-[GCC 9.3.0] on linux
-Type "help", "copyright", "credits" or "license" for more information.
->>> from moc_prices_source import get_price, BTC_USD, RIF_BTC, ALL
->>>
-```
-
-Get de BTC USD coin pair
-
-```
->>> get_price(BTC_USD)
-Decimal('13089.82')
->>> 
-```
-
-Get de RIF BTC coin pair
-
-```
->>> get_price(RIF_BTC)
-Decimal('0.00000713')
->>> 
-```
-
-Get errors detail (forced errors for example)
-
-```
->>> d = {}
->>> values = get_price(detail = d)
->>> for e in d['prices']:
-...     if not e["ok"]:
-...         print('{}: {}'.format(e["name"], e["error"]))
-...
-btc_usd_kraken: HTTPSConnectionPool(host='api.bad_uri.com', port=443): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.VerifiedHTTPSConnection object at 0x7f2c48700b50>: Failed to establish a new connection: [Errno -2] Name or service not known'))
->>>
-```
-
-Show the default weighing
-
-```
->>> from moc_prices_source.weighing import weighing
->>> print(weighing)
-Engine                  Weigh
-------------------  ---------
-btc_usd_bitstamp    0.22619
-btc_usd_bitfinex    0.153778
-btc_usd_kraken      0.152346
-btc_usd_coinbase    0.403366
-btc_usd_gemini      0.0643202
-rif_btc_bithumbpro  0.333333
-rif_btc_kucoin      0.333333
-rif_btc_coinbene    0.333333
->>> weighing.as_dict
-{'btc_usd_bitstamp': Decimal('0.226189632'), 'btc_usd_bitfinex': Decimal('0.1537782868'), 'btc_usd_kraken': Decimal('0.1523461274'), 'btc_usd_coinbase': Decimal('0.4033657328'), 'btc_usd_gemini': Decimal('0.06432022093'), 'rif_btc_bithumbpro': Decimal('0.333333333'), 'rif_btc_kucoin': Decimal('0.333333333'), 'rif_btc_coinbene': Decimal('0.333333333')}
->>> 
-```
-
-Override the default weighing
-
-```
->>> w = {"btc_usd_bitstamp": 0.2, "btc_usd_bitfinex": 0.8}
->>> get_price(weighing = w)
-Decimal('13070')
->>> 
-```
-
-Show all details of the coin pair obtained
-
-```
->>> import json
->>> d = {}
->>> values = get_price(ALL, detail = d, serializable = True)
->>>
->>> values
-{<BTC/USD Coin Pair object>: Decimal('15250.00000'), <RIF/BTC Coin Pair object>: Decimal('0.00000637'), <RIF/USD Coin Pair object>: Decimal('0.0971425000000')}
->>>
->>> print(json.dumps(d, indent=4, sort_keys=True))
-{
-    "prices": [
+Metadata-Version: 2.1
+Name: moneyonchain_prices_source
+Version: 0.6.4b0
+Summary: Prices source for MoC projects
+Home-page: UNKNOWN
+Author: Juan S. Bokser
+Author-email: juan.bokser@moneyonchain.com
+License: UNKNOWN
+Description: # MoC prices source
+        
+        Prices source for MoC projects
+        
+        
+        
+        ## Refrences
+        
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source)
+        * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
+        
+        
+        
+        ## Requirements
+        
+        * Python 3.6+ support
+        
+        
+        
+        ## Installation
+        
+        ### From the Python package index (PyPI) 
+        
+        Run:
+        
+        ```
+        $ pip3 install moneyonchain-prices-source 
+        ```
+        
+        And then run:
+        
+        ```
+        $ moc_prices_source_check --version
+        ```
+        
+        To verify that it has been installed correctly
+        
+        ### From source
+        
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source)
+        
+        Standing inside the folder, run:
+        
+        ```
+        $ pip3 install -r requirements.txt 
+        ```
+        
+        For install the dependencies and then run:
+        
+        ```
+        $ pip3 install .
+        ```
+        
+        Finally run:
+        
+        ```
+        $ moc_prices_source_check --version
+        ```
+        
+        To verify that it has been installed correctly
+        
+        
+        
+        ## Check that all is working ok
+        
+        ```
+        user@host:~$ moc_prices_source_check 
+        
+        From       To       Exchnage        Response  U.      Weigh     %  Time
+        ---------  -------  ----------  ------------  ----  -------  ----  ------
+        Bitcoin    Dollar   Bitfinex    15245         $        0.15  15.4  0.88s
+        Bitcoin    Dollar   Bitstamp    15241.9       $        0.23  22.6  0.34s
+        Bitcoin    Dollar   Coinbase    15236.5       $        0.4   40.3  0.27s
+        Bitcoin    Dollar   Gemini      15246.8       $        0.06   6.4  0.87s
+        Bitcoin    Dollar   Kraken      15239.4       $        0.15  15.2  0.4s
+        RIF Token  Bitcoin  BitHumb         6.64e-06  ₿        0.33  33.3  3.09s
+        RIF Token  Bitcoin  Coinbene        5.78e-06  ₿        0.33  33.3  1.27s
+        RIF Token  Bitcoin  Kucoin          6.37e-06  ₿        0.33  33.3  1.16s
+        
+        Coin pair          Mediam             Mean    Weighted median  Sources
+        -----------  ------------  ---------------  -----------------  ---------
+        BTC/USD      15241.9       15241.9               15239.4       5
+        RIF/BTC          6.37e-06      6.26333e-06           6.37e-06  3
+        RIF/USD          0.097091      0.0954653             0.097075  N/A
+        
+        Response time 3.1s
+        
+        user@host:~$
+        ```
+        
+        More options
+        
+        ```
+        user@host:~$ moc_prices_source_check --help
+        Usage: moc_prices_source_check [OPTIONS]
+        
+        Options:
+          -v, --version   Show version and exit.
+          -j, --json      Show data in JSON format and exit.
+          -w, --weighing  Show the default weighing and exit.
+          -h, --help      Show this message and exit.
+        user@host:~$ 
+        ```
+        
+        
+        ## Usage
+        
+        Do some imports first
+        
+        ```
+        user@host:~$ python3
+        Python 3.8.5 (default, Jul 28 2020, 12:59:40) 
+        [GCC 9.3.0] on linux
+        Type "help", "copyright", "credits" or "license" for more information.
+        >>> from moc_prices_source import get_price, BTC_USD, RIF_BTC, ALL
+        >>>
+        ```
+        
+        Get de BTC USD coin pair
+        
+        ```
+        >>> get_price(BTC_USD)
+        Decimal('13089.82')
+        >>> 
+        ```
+        
+        Get de RIF BTC coin pair
+        
+        ```
+        >>> get_price(RIF_BTC)
+        Decimal('0.00000713')
+        >>> 
+        ```
+        
+        Get errors detail (forced errors for example)
+        
+        ```
+        >>> d = {}
+        >>> values = get_price(detail = d)
+        >>> for e in d['prices']:
+        ...     if not e["ok"]:
+        ...         print('{}: {}'.format(e["name"], e["error"]))
+        ...
+        btc_usd_kraken: HTTPSConnectionPool(host='api.bad_uri.com', port=443): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.VerifiedHTTPSConnection object at 0x7f2c48700b50>: Failed to establish a new connection: [Errno -2] Name or service not known'))
+        >>>
+        ```
+        
+        Show the default weighing
+        
+        ```
+        >>> from moc_prices_source.weighing import weighing
+        >>> print(weighing)
+        Engine                  Weigh
+        ------------------  ---------
+        btc_usd_bitstamp    0.22619
+        btc_usd_bitfinex    0.153778
+        btc_usd_kraken      0.152346
+        btc_usd_coinbase    0.403366
+        btc_usd_gemini      0.0643202
+        rif_btc_bithumbpro  0.333333
+        rif_btc_kucoin      0.333333
+        rif_btc_coinbene    0.333333
+        >>> weighing.as_dict
+        {'btc_usd_bitstamp': Decimal('0.226189632'), 'btc_usd_bitfinex': Decimal('0.1537782868'), 'btc_usd_kraken': Decimal('0.1523461274'), 'btc_usd_coinbase': Decimal('0.4033657328'), 'btc_usd_gemini': Decimal('0.06432022093'), 'rif_btc_bithumbpro': Decimal('0.333333333'), 'rif_btc_kucoin': Decimal('0.333333333'), 'rif_btc_coinbene': Decimal('0.333333333')}
+        >>> 
+        ```
+        
+        Override the default weighing
+        
+        ```
+        >>> w = {"btc_usd_bitstamp": 0.2, "btc_usd_bitfinex": 0.8}
+        >>> get_price(weighing = w)
+        Decimal('13070')
+        >>> 
+        ```
+        
+        Show all details of the coin pair obtained
+        
+        ```
+        >>> import json
+        >>> d = {}
+        >>> values = get_price(ALL, detail = d, serializable = True)
+        >>>
+        >>> values
+        {<BTC/USD Coin Pair object>: Decimal('15250.00000'), <RIF/BTC Coin Pair object>: Decimal('0.00000637'), <RIF/USD Coin Pair object>: Decimal('0.0971425000000')}
+        >>>
+        >>> print(json.dumps(d, indent=4, sort_keys=True))
         {
-            "coinpair": "BTC/USD",
-            "description": "Bitstamp",
-            "error": null,
-            "name": "btc_usd_bitstamp",
-            "ok": true,
-            "percentual_weighing": 0.22618963201583328,
-            "price": 15248.38,
-            "time": 0.279066,
-            "timeout": 10,
-            "timestamp": "2020-11-08 14:23:02",
-            "uri": "https://www.bitstamp.net/api/v2/ticker/btcusd/",
-            "volume": 10835.66006591,
-            "weighing": 0.226189632
-        },
-        {
-            "coinpair": "RIF/BTC",
-            "description": "Coinbene",
-            "error": null,
-            "name": "rif_btc_coinbene",
-            "ok": true,
-            "percentual_weighing": 0.3333333333333333,
-            "price": 5.8e-06,
-            "time": 1.571258,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:04",
-            "uri": "http://api.coinbene.com/v1/market/ticker?symbol=RIFBTC",
-            "volume": 806810.93,
-            "weighing": 0.333333333
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Bitfinex",
-            "error": null,
-            "name": "btc_usd_bitfinex",
-            "ok": true,
-            "percentual_weighing": 0.15377828681076447,
-            "price": 15248.22269385,
-            "time": 0.267649,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:02",
-            "uri": "https://api-pub.bitfinex.com/v2/ticker/tBTCUSD",
-            "volume": 14362.55862314,
-            "weighing": 0.1537782868
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Gemini",
-            "error": null,
-            "name": "btc_usd_gemini",
-            "ok": true,
-            "percentual_weighing": 0.06432022093450242,
-            "price": 15254.3,
-            "time": 0.952623,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:03",
-            "uri": "https://api.gemini.com/v1/pubticker/BTCUSD",
-            "volume": 0.0,
-            "weighing": 0.06432022093
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Coinbase",
-            "error": null,
-            "name": "btc_usd_coinbase",
-            "ok": true,
-            "percentual_weighing": 0.4033657328282356,
-            "price": 15251.88,
-            "time": 0.246729,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:02",
-            "uri": "https://api.coinbase.com/v2/prices/spot?currency=USD",
-            "volume": 0.0,
-            "weighing": 0.4033657328
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Kraken",
-            "error": null,
-            "name": "btc_usd_kraken",
-            "ok": true,
-            "percentual_weighing": 0.15234612741066422,
-            "price": 15250.0,
-            "time": 0.265883,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:02",
-            "uri": "https://api.kraken.com/0/public/Ticker?pair=XXBTZUSD",
-            "volume": 8018.38037875,
-            "weighing": 0.1523461274
-        },
-        {
-            "coinpair": "RIF/BTC",
-            "description": "Kucoin",
-            "error": null,
-            "name": "rif_btc_kucoin",
-            "ok": true,
-            "percentual_weighing": 0.3333333333333333,
-            "price": 6.37e-06,
-            "time": 0.932421,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:03",
-            "uri": "https://openapi-v2.kucoin.com/api/v1/market/orderbook/level1?symbol=RIF-BTC",
-            "volume": 963.5025,
-            "weighing": 0.333333333
-        },
-        {
-            "coinpair": "RIF/BTC",
-            "description": "BitHumb",
-            "error": null,
-            "name": "rif_btc_bithumbpro",
-            "ok": true,
-            "percentual_weighing": 0.3333333333333333,
-            "price": 6.67e-06,
-            "time": 1.836675,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:04",
-            "uri": "https://global-openapi.bithumb.pro/openapi/v1/spot/ticker?symbol=RIF-BTC",
-            "volume": 27932.67,
-            "weighing": 0.333333333
-        }
-    ],
-    "time": 1.882155,
-    "values": {
-        "BTC/USD": {
-            "mean_price": 15250.55653877,
-            "median_price": 15250.0,
-            "prices": [
-                15248.38,
-                15248.22269385,
-                15254.3,
-                15251.88,
-                15250.0
-            ],
-            "weighings": [
-                0.22618963201583328,
-                0.15377828681076447,
-                0.06432022093450242,
-                0.4033657328282356,
-                0.15234612741066422
-            ],
-            "weighted_median_price": 15250.0
-        },
-        "RIF/BTC": {
-            "mean_price": 6.28e-06,
-            "median_price": 6.37e-06,
             "prices": [
-                5.8e-06,
-                6.37e-06,
-                6.67e-06
-            ],
-            "weighings": [
-                0.3333333333333333,
-                0.3333333333333333,
-                0.3333333333333333
-            ],
-            "weighted_median_price": 6.37e-06
-        },
-        "RIF/USD": {
-            "mean_price": 0.0957734950634756,
-            "median_price": 0.0971425,
-            "requirements": [
-                "RIF/BTC",
-                "BTC/USD"
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Bitstamp",
+                    "error": null,
+                    "name": "btc_usd_bitstamp",
+                    "ok": true,
+                    "percentual_weighing": 0.22618963201583328,
+                    "price": 15248.38,
+                    "time": 0.279066,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 14:23:02",
+                    "uri": "https://www.bitstamp.net/api/v2/ticker/btcusd/",
+                    "volume": 10835.66006591,
+                    "weighing": 0.226189632
+                },
+                {
+                    "coinpair": "RIF/BTC",
+                    "description": "Coinbene",
+                    "error": null,
+                    "name": "rif_btc_coinbene",
+                    "ok": true,
+                    "percentual_weighing": 0.3333333333333333,
+                    "price": 5.8e-06,
+                    "time": 1.571258,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:04",
+                    "uri": "http://api.coinbene.com/v1/market/ticker?symbol=RIFBTC",
+                    "volume": 806810.93,
+                    "weighing": 0.333333333
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Bitfinex",
+                    "error": null,
+                    "name": "btc_usd_bitfinex",
+                    "ok": true,
+                    "percentual_weighing": 0.15377828681076447,
+                    "price": 15248.22269385,
+                    "time": 0.267649,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:02",
+                    "uri": "https://api-pub.bitfinex.com/v2/ticker/tBTCUSD",
+                    "volume": 14362.55862314,
+                    "weighing": 0.1537782868
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Gemini",
+                    "error": null,
+                    "name": "btc_usd_gemini",
+                    "ok": true,
+                    "percentual_weighing": 0.06432022093450242,
+                    "price": 15254.3,
+                    "time": 0.952623,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:03",
+                    "uri": "https://api.gemini.com/v1/pubticker/BTCUSD",
+                    "volume": 0.0,
+                    "weighing": 0.06432022093
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Coinbase",
+                    "error": null,
+                    "name": "btc_usd_coinbase",
+                    "ok": true,
+                    "percentual_weighing": 0.4033657328282356,
+                    "price": 15251.88,
+                    "time": 0.246729,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:02",
+                    "uri": "https://api.coinbase.com/v2/prices/spot?currency=USD",
+                    "volume": 0.0,
+                    "weighing": 0.4033657328
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Kraken",
+                    "error": null,
+                    "name": "btc_usd_kraken",
+                    "ok": true,
+                    "percentual_weighing": 0.15234612741066422,
+                    "price": 15250.0,
+                    "time": 0.265883,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:02",
+                    "uri": "https://api.kraken.com/0/public/Ticker?pair=XXBTZUSD",
+                    "volume": 8018.38037875,
+                    "weighing": 0.1523461274
+                },
+                {
+                    "coinpair": "RIF/BTC",
+                    "description": "Kucoin",
+                    "error": null,
+                    "name": "rif_btc_kucoin",
+                    "ok": true,
+                    "percentual_weighing": 0.3333333333333333,
+                    "price": 6.37e-06,
+                    "time": 0.932421,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:03",
+                    "uri": "https://openapi-v2.kucoin.com/api/v1/market/orderbook/level1?symbol=RIF-BTC",
+                    "volume": 963.5025,
+                    "weighing": 0.333333333
+                },
+                {
+                    "coinpair": "RIF/BTC",
+                    "description": "BitHumb",
+                    "error": null,
+                    "name": "rif_btc_bithumbpro",
+                    "ok": true,
+                    "percentual_weighing": 0.3333333333333333,
+                    "price": 6.67e-06,
+                    "time": 1.836675,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:04",
+                    "uri": "https://global-openapi.bithumb.pro/openapi/v1/spot/ticker?symbol=RIF-BTC",
+                    "volume": 27932.67,
+                    "weighing": 0.333333333
+                }
             ],
-            "weighted_median_price": 0.0971425
+            "time": 1.882155,
+            "values": {
+                "BTC/USD": {
+                    "mean_price": 15250.55653877,
+                    "median_price": 15250.0,
+                    "prices": [
+                        15248.38,
+                        15248.22269385,
+                        15254.3,
+                        15251.88,
+                        15250.0
+                    ],
+                    "weighings": [
+                        0.22618963201583328,
+                        0.15377828681076447,
+                        0.06432022093450242,
+                        0.4033657328282356,
+                        0.15234612741066422
+                    ],
+                    "weighted_median_price": 15250.0
+                },
+                "RIF/BTC": {
+                    "mean_price": 6.28e-06,
+                    "median_price": 6.37e-06,
+                    "prices": [
+                        5.8e-06,
+                        6.37e-06,
+                        6.67e-06
+                    ],
+                    "weighings": [
+                        0.3333333333333333,
+                        0.3333333333333333,
+                        0.3333333333333333
+                    ],
+                    "weighted_median_price": 6.37e-06
+                },
+                "RIF/USD": {
+                    "mean_price": 0.0957734950634756,
+                    "median_price": 0.0971425,
+                    "requirements": [
+                        "RIF/BTC",
+                        "BTC/USD"
+                    ],
+                    "weighted_median_price": 0.0971425
+                }
+            }
         }
-    }
-}
->>> 
-```
-
-`Coin object` and `Coin Pair object` usage:
-
-```
->>> BTC_USD
-<BTC/USD Coin Pair object>
->>> str(BTC_USD)
-'BTC/USD'
->>> BTC_USD.from_
-<Bitcoin Coin object>
->>> str(BTC_USD.from_)
-'BTC'
->>> BTC_USD.to_
-<Dollar Coin object>
->>> str(BTC_USD.to_)
-'USD'
->>> BTC_USD.from_.symbol
-'BTC'
->>> BTC_USD.from_.name
-'Bitcoin'
->>> BTC_USD.from_.small_symbol
-'₿'
->>>
-```
+        >>> 
+        ```
+        
+        `Coin object` and `Coin Pair object` usage:
+        
+        ```
+        >>> BTC_USD
+        <BTC/USD Coin Pair object>
+        >>> str(BTC_USD)
+        'BTC/USD'
+        >>> BTC_USD.from_
+        <Bitcoin Coin object>
+        >>> str(BTC_USD.from_)
+        'BTC'
+        >>> BTC_USD.to_
+        <Dollar Coin object>
+        >>> str(BTC_USD.to_)
+        'USD'
+        >>> BTC_USD.from_.symbol
+        'BTC'
+        >>> BTC_USD.from_.name
+        'Bitcoin'
+        >>> BTC_USD.from_.small_symbol
+        '₿'
+        >>>
+        ```
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/cli_check.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/computed_pairs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 from types   import LambdaType
 
 base_dir = dirname(abspath(__file__))
 
 bkpath   = sys.path[:]
 sys.path.append(dirname(base_dir))
 
-from moc_prices_source.engines.coins import BTC_USD, RIF_BTC, ETH_BTC, RIF_USD, ETH_USD, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS
+from moc_prices_source.engines.coins import BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, ETH_USD, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS
 
 sys.path = bkpath
 
 
 
 computed_pairs = {
+    MOC_USD: {
+        'requirements': [MOC_BTC, BTC_USD],
+        'formula': lambda moc_btc, btc_usd: moc_btc * btc_usd
+    },
     RIF_USD: {
         'requirements': [RIF_BTC, BTC_USD],
         'formula': lambda rif_btc, btc_usd: rif_btc * btc_usd
     },
     ETH_USD: {
         'requirements': [ETH_BTC, BTC_USD],
         'formula': lambda eth_btc, btc_usd: eth_btc * btc_usd
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from engine_base import Base, BTC_USD
+from engine_base import Base, ETH_BTC
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
     _description = "Kraken"
-    _uri         = "https://api.kraken.com/0/public/Ticker?pair=XXBTZUSD"
-    _coinpair    = BTC_USD
+    _uri         = "https://api.kraken.com/0/public/Ticker?pair=ETHBTC"
+    _coinpair    = ETH_BTC
 
     def _map(self, data):
         return {
-            'price':  data['result']['XXBTZUSD']['c'][0],
-            'volume': data['result']['XXBTZUSD']['v'][1] }
+            'price':  data['result']['XETHXXBT']['c'][0],
+            'volume': data['result']['XETHXXBT']['v'][1] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/coins.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     def __hash__(self):
         return hash(str(self))
 
 
 BTC  = Coin('Bitcoin',        'btc',  '₿')
 USD  = Coin('Dollar',         'usd',  '$')
 RIF  = Coin('RIF Token',      'rif')
+MOC  = Coin('MOC Token',      'moc')
 ETH  = Coin('Ether',          'eth',  '⟠')
 USDT = Coin('Tether',         'usdt', '₮')
 BNB  = Coin('Binance Coin',   'bnb',  'Ƀ')
 ARS  = Coin('Peso Argentino', 'ars',  '$')
 MXN  = Coin('Peso Mexicano',  'mxn',  '$')
 
 
@@ -116,14 +117,16 @@
         return hash(str(self))
 
 
 BTC_USD         = CoinPair(BTC,  USD)
 BTC_ARS         = CoinPair(BTC,  ARS)
 RIF_BTC         = CoinPair(RIF,  BTC)
 RIF_USD         = CoinPair(RIF,  USD)
+MOC_BTC         = CoinPair(MOC,  BTC)
+MOC_USD         = CoinPair(MOC,  USD)
 ETH_BTC         = CoinPair(ETH,  BTC)
 ETH_USD         = CoinPair(ETH,  USD)
 BTC_USDT        = CoinPair(BTC,  USDT)
 USDT_USD        = CoinPair(USDT, USD)
 BNB_USDT        = CoinPair(BNB,  USDT)
 BNB_USD         = CoinPair(BNB,  USD)
 USD_ARS         = CoinPair(USD,  ARS)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/engine_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sys          import stderr
 from os.path      import basename, dirname, abspath, expanduser
 from decimal      import Decimal
 from json.decoder import JSONDecodeError
 from redis        import Redis, ConnectionError
 from coins        import *
 from bs4          import BeautifulSoup
+from web3         import Web3, HTTPProvider
 
 
 
 class Base(object):
 
     _name                          = "base"
     _description                   = "Base Engine"
@@ -412,9 +413,76 @@
         if self._uri_failover and not ok:
             uri_failover, uri = self._uri_failover, self._uri
             self._uri_failover, self._uri =  uri, uri_failover
             ok = Base.__call__(self, start_time)
         return ok
 
 
+class BaseOnChain(Base):
+
+    erc20_simplified_abi = """
+[
+    {
+        "constant": true,
+        "inputs": [
+            {
+                "name": "_owner",
+                "type": "address"
+            }
+        ],
+        "name": "balanceOf",
+        "outputs": [
+            {
+                "name": "balance",
+                "type": "uint256"
+            }
+        ],
+        "payable": false,
+        "stateMutability": "view",
+        "type": "function"
+    }
+]
+"""
+    Web3 = Web3
+    HTTPProvider = HTTPProvider
+
+    def _get_price(self):
+
+        try:
+
+            return 0
+
+        except Exception as e:
+            self._error = str(e)
+            return None
+
+
+    def __call__(self, start_time=None):
+
+        if start_time is None:
+            start_time = datetime.datetime.now()
+        
+        price = self._get_price()
+ 
+        if not price:
+            if not self._error:
+                self._error = "Engine error trying to get 'price'"
+            return False
+
+        try:
+            self._price = Decimal(str(price))
+        except Exception:
+            self._error = "Engine error trying to get 'price'"
+            return False
+
+        self._timestamp = self._now()
+        self._last_change_timestamp = self._timestamp
+
+        self._volume = 0.0
+        self._time = datetime.datetime.now() - start_time
+
+        return True
+
+
+
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from engine_base import Base, ETH_BTC
+from engine_base import Base, BTC_USDT
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Kraken"
-    _uri         = "https://api.kraken.com/0/public/Ticker?pair=ETHBTC"
-    _coinpair    = ETH_BTC
+    _description = "Bitfinex"
+    _uri         = "https://api-pub.bitfinex.com/v2/ticker/tBTCUST"
+    _coinpair    = BTC_USDT
 
     def _map(self, data):
         return {
-            'price':  data['result']['XETHXXBT']['c'][0],
-            'volume': data['result']['XETHXXBT']['v'][1] }
+            'price':  data[6],
+            'volume': data[7]}
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from engine_base import Base, RIF_BTC
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "BitHumb"
-    _uri         = "https://global-openapi.bithumb.pro/openapi/v1/spot/ticker?symbol=RIF-BTC"
+    _description = "MXC"
+    _uri         = "https://www.mxc.com/open/api/v2/market/ticker?symbol=RIF_BTC"
     _coinpair    = RIF_BTC
     _max_time_without_price_change = 0 # zero means infinity
 
     def _map(self, data):
         return {
-            'price':  data['data'][0]['c'],
-            'volume': data['data'][0]['v'] }
+            'price':  data['data'][0]['last'],
+            'volume': data['data'][0]['volume']}
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from engine_base import Base, RIF_BTC
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Coinbene"
-    _uri         = "https://openapi-exchange.coinbene.com/api/exchange/v2/market/ticker/one?symbol=RIF%2FBTC"
+    _description = "BitHumb"
+    _uri         = "https://global-openapi.bithumb.pro/openapi/v1/spot/ticker?symbol=RIF-BTC"
     _coinpair    = RIF_BTC
     _max_time_without_price_change = 0 # zero means infinity
 
     def _map(self, data):
         return {
-            'price':  data['data']['latestPrice'],
-            'volume': data['data']['volume24h'] }
-
+            'price':  data['data'][0]['c'],
+            'volume': data['data'][0]['v'] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-from engine_base import Base, RIF_BTC
+from engine_base import Base, BTC_ARS
+from decimal import Decimal
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "MXC"
-    _uri         = "https://www.mxc.com/open/api/v2/market/ticker?symbol=RIF_BTC"
-    _coinpair    = RIF_BTC
-    _max_time_without_price_change = 0 # zero means infinity
+    _description = "Decrypto"
+    _uri         = "https://api.decrypto.la/1.0/frontend/trading/data/prices"
+    _coinpair    = BTC_ARS
+    
+    _max_age                       = 3600 # 1hs.
+    _max_time_without_price_change = 0    # zero means infinity
 
     def _map(self, data):
-        return {
-            'price':  data['data'][0]['last'],
-            'volume': data['data'][0]['volume']}
+        value = {}
+        for i in data['data']:
+            if i['currencyToken']['codigo']=='BTCARS':
+                value['price'] = (Decimal(i['dca']) + Decimal(i['dcb'])) / Decimal('2')
+                break
+        return value
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
+    if engine.error:
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.4b0/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.3/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.6.4b0/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,396 +1,398 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.6.3
+Version: 0.6.4b0
 Summary: Prices source for MoC projects
+Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
+License: UNKNOWN
+Description: # MoC prices source
+        
+        Prices source for MoC projects
+        
+        
+        
+        ## Refrences
+        
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source)
+        * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
+        
+        
+        
+        ## Requirements
+        
+        * Python 3.6+ support
+        
+        
+        
+        ## Installation
+        
+        ### From the Python package index (PyPI) 
+        
+        Run:
+        
+        ```
+        $ pip3 install moneyonchain-prices-source 
+        ```
+        
+        And then run:
+        
+        ```
+        $ moc_prices_source_check --version
+        ```
+        
+        To verify that it has been installed correctly
+        
+        ### From source
+        
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source)
+        
+        Standing inside the folder, run:
+        
+        ```
+        $ pip3 install -r requirements.txt 
+        ```
+        
+        For install the dependencies and then run:
+        
+        ```
+        $ pip3 install .
+        ```
+        
+        Finally run:
+        
+        ```
+        $ moc_prices_source_check --version
+        ```
+        
+        To verify that it has been installed correctly
+        
+        
+        
+        ## Check that all is working ok
+        
+        ```
+        user@host:~$ moc_prices_source_check 
+        
+        From       To       Exchnage        Response  U.      Weigh     %  Time
+        ---------  -------  ----------  ------------  ----  -------  ----  ------
+        Bitcoin    Dollar   Bitfinex    15245         $        0.15  15.4  0.88s
+        Bitcoin    Dollar   Bitstamp    15241.9       $        0.23  22.6  0.34s
+        Bitcoin    Dollar   Coinbase    15236.5       $        0.4   40.3  0.27s
+        Bitcoin    Dollar   Gemini      15246.8       $        0.06   6.4  0.87s
+        Bitcoin    Dollar   Kraken      15239.4       $        0.15  15.2  0.4s
+        RIF Token  Bitcoin  BitHumb         6.64e-06  ₿        0.33  33.3  3.09s
+        RIF Token  Bitcoin  Coinbene        5.78e-06  ₿        0.33  33.3  1.27s
+        RIF Token  Bitcoin  Kucoin          6.37e-06  ₿        0.33  33.3  1.16s
+        
+        Coin pair          Mediam             Mean    Weighted median  Sources
+        -----------  ------------  ---------------  -----------------  ---------
+        BTC/USD      15241.9       15241.9               15239.4       5
+        RIF/BTC          6.37e-06      6.26333e-06           6.37e-06  3
+        RIF/USD          0.097091      0.0954653             0.097075  N/A
+        
+        Response time 3.1s
+        
+        user@host:~$
+        ```
+        
+        More options
+        
+        ```
+        user@host:~$ moc_prices_source_check --help
+        Usage: moc_prices_source_check [OPTIONS]
+        
+        Options:
+          -v, --version   Show version and exit.
+          -j, --json      Show data in JSON format and exit.
+          -w, --weighing  Show the default weighing and exit.
+          -h, --help      Show this message and exit.
+        user@host:~$ 
+        ```
+        
+        
+        ## Usage
+        
+        Do some imports first
+        
+        ```
+        user@host:~$ python3
+        Python 3.8.5 (default, Jul 28 2020, 12:59:40) 
+        [GCC 9.3.0] on linux
+        Type "help", "copyright", "credits" or "license" for more information.
+        >>> from moc_prices_source import get_price, BTC_USD, RIF_BTC, ALL
+        >>>
+        ```
+        
+        Get de BTC USD coin pair
+        
+        ```
+        >>> get_price(BTC_USD)
+        Decimal('13089.82')
+        >>> 
+        ```
+        
+        Get de RIF BTC coin pair
+        
+        ```
+        >>> get_price(RIF_BTC)
+        Decimal('0.00000713')
+        >>> 
+        ```
+        
+        Get errors detail (forced errors for example)
+        
+        ```
+        >>> d = {}
+        >>> values = get_price(detail = d)
+        >>> for e in d['prices']:
+        ...     if not e["ok"]:
+        ...         print('{}: {}'.format(e["name"], e["error"]))
+        ...
+        btc_usd_kraken: HTTPSConnectionPool(host='api.bad_uri.com', port=443): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.VerifiedHTTPSConnection object at 0x7f2c48700b50>: Failed to establish a new connection: [Errno -2] Name or service not known'))
+        >>>
+        ```
+        
+        Show the default weighing
+        
+        ```
+        >>> from moc_prices_source.weighing import weighing
+        >>> print(weighing)
+        Engine                  Weigh
+        ------------------  ---------
+        btc_usd_bitstamp    0.22619
+        btc_usd_bitfinex    0.153778
+        btc_usd_kraken      0.152346
+        btc_usd_coinbase    0.403366
+        btc_usd_gemini      0.0643202
+        rif_btc_bithumbpro  0.333333
+        rif_btc_kucoin      0.333333
+        rif_btc_coinbene    0.333333
+        >>> weighing.as_dict
+        {'btc_usd_bitstamp': Decimal('0.226189632'), 'btc_usd_bitfinex': Decimal('0.1537782868'), 'btc_usd_kraken': Decimal('0.1523461274'), 'btc_usd_coinbase': Decimal('0.4033657328'), 'btc_usd_gemini': Decimal('0.06432022093'), 'rif_btc_bithumbpro': Decimal('0.333333333'), 'rif_btc_kucoin': Decimal('0.333333333'), 'rif_btc_coinbene': Decimal('0.333333333')}
+        >>> 
+        ```
+        
+        Override the default weighing
+        
+        ```
+        >>> w = {"btc_usd_bitstamp": 0.2, "btc_usd_bitfinex": 0.8}
+        >>> get_price(weighing = w)
+        Decimal('13070')
+        >>> 
+        ```
+        
+        Show all details of the coin pair obtained
+        
+        ```
+        >>> import json
+        >>> d = {}
+        >>> values = get_price(ALL, detail = d, serializable = True)
+        >>>
+        >>> values
+        {<BTC/USD Coin Pair object>: Decimal('15250.00000'), <RIF/BTC Coin Pair object>: Decimal('0.00000637'), <RIF/USD Coin Pair object>: Decimal('0.0971425000000')}
+        >>>
+        >>> print(json.dumps(d, indent=4, sort_keys=True))
+        {
+            "prices": [
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Bitstamp",
+                    "error": null,
+                    "name": "btc_usd_bitstamp",
+                    "ok": true,
+                    "percentual_weighing": 0.22618963201583328,
+                    "price": 15248.38,
+                    "time": 0.279066,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 14:23:02",
+                    "uri": "https://www.bitstamp.net/api/v2/ticker/btcusd/",
+                    "volume": 10835.66006591,
+                    "weighing": 0.226189632
+                },
+                {
+                    "coinpair": "RIF/BTC",
+                    "description": "Coinbene",
+                    "error": null,
+                    "name": "rif_btc_coinbene",
+                    "ok": true,
+                    "percentual_weighing": 0.3333333333333333,
+                    "price": 5.8e-06,
+                    "time": 1.571258,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:04",
+                    "uri": "http://api.coinbene.com/v1/market/ticker?symbol=RIFBTC",
+                    "volume": 806810.93,
+                    "weighing": 0.333333333
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Bitfinex",
+                    "error": null,
+                    "name": "btc_usd_bitfinex",
+                    "ok": true,
+                    "percentual_weighing": 0.15377828681076447,
+                    "price": 15248.22269385,
+                    "time": 0.267649,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:02",
+                    "uri": "https://api-pub.bitfinex.com/v2/ticker/tBTCUSD",
+                    "volume": 14362.55862314,
+                    "weighing": 0.1537782868
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Gemini",
+                    "error": null,
+                    "name": "btc_usd_gemini",
+                    "ok": true,
+                    "percentual_weighing": 0.06432022093450242,
+                    "price": 15254.3,
+                    "time": 0.952623,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:03",
+                    "uri": "https://api.gemini.com/v1/pubticker/BTCUSD",
+                    "volume": 0.0,
+                    "weighing": 0.06432022093
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Coinbase",
+                    "error": null,
+                    "name": "btc_usd_coinbase",
+                    "ok": true,
+                    "percentual_weighing": 0.4033657328282356,
+                    "price": 15251.88,
+                    "time": 0.246729,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:02",
+                    "uri": "https://api.coinbase.com/v2/prices/spot?currency=USD",
+                    "volume": 0.0,
+                    "weighing": 0.4033657328
+                },
+                {
+                    "coinpair": "BTC/USD",
+                    "description": "Kraken",
+                    "error": null,
+                    "name": "btc_usd_kraken",
+                    "ok": true,
+                    "percentual_weighing": 0.15234612741066422,
+                    "price": 15250.0,
+                    "time": 0.265883,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:02",
+                    "uri": "https://api.kraken.com/0/public/Ticker?pair=XXBTZUSD",
+                    "volume": 8018.38037875,
+                    "weighing": 0.1523461274
+                },
+                {
+                    "coinpair": "RIF/BTC",
+                    "description": "Kucoin",
+                    "error": null,
+                    "name": "rif_btc_kucoin",
+                    "ok": true,
+                    "percentual_weighing": 0.3333333333333333,
+                    "price": 6.37e-06,
+                    "time": 0.932421,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:03",
+                    "uri": "https://openapi-v2.kucoin.com/api/v1/market/orderbook/level1?symbol=RIF-BTC",
+                    "volume": 963.5025,
+                    "weighing": 0.333333333
+                },
+                {
+                    "coinpair": "RIF/BTC",
+                    "description": "BitHumb",
+                    "error": null,
+                    "name": "rif_btc_bithumbpro",
+                    "ok": true,
+                    "percentual_weighing": 0.3333333333333333,
+                    "price": 6.67e-06,
+                    "time": 1.836675,
+                    "timeout": 10,
+                    "timestamp": "2020-11-08 11:23:04",
+                    "uri": "https://global-openapi.bithumb.pro/openapi/v1/spot/ticker?symbol=RIF-BTC",
+                    "volume": 27932.67,
+                    "weighing": 0.333333333
+                }
+            ],
+            "time": 1.882155,
+            "values": {
+                "BTC/USD": {
+                    "mean_price": 15250.55653877,
+                    "median_price": 15250.0,
+                    "prices": [
+                        15248.38,
+                        15248.22269385,
+                        15254.3,
+                        15251.88,
+                        15250.0
+                    ],
+                    "weighings": [
+                        0.22618963201583328,
+                        0.15377828681076447,
+                        0.06432022093450242,
+                        0.4033657328282356,
+                        0.15234612741066422
+                    ],
+                    "weighted_median_price": 15250.0
+                },
+                "RIF/BTC": {
+                    "mean_price": 6.28e-06,
+                    "median_price": 6.37e-06,
+                    "prices": [
+                        5.8e-06,
+                        6.37e-06,
+                        6.67e-06
+                    ],
+                    "weighings": [
+                        0.3333333333333333,
+                        0.3333333333333333,
+                        0.3333333333333333
+                    ],
+                    "weighted_median_price": 6.37e-06
+                },
+                "RIF/USD": {
+                    "mean_price": 0.0957734950634756,
+                    "median_price": 0.0971425,
+                    "requirements": [
+                        "RIF/BTC",
+                        "BTC/USD"
+                    ],
+                    "weighted_median_price": 0.0971425
+                }
+            }
+        }
+        >>> 
+        ```
+        
+        `Coin object` and `Coin Pair object` usage:
+        
+        ```
+        >>> BTC_USD
+        <BTC/USD Coin Pair object>
+        >>> str(BTC_USD)
+        'BTC/USD'
+        >>> BTC_USD.from_
+        <Bitcoin Coin object>
+        >>> str(BTC_USD.from_)
+        'BTC'
+        >>> BTC_USD.to_
+        <Dollar Coin object>
+        >>> str(BTC_USD.to_)
+        'USD'
+        >>> BTC_USD.from_.symbol
+        'BTC'
+        >>> BTC_USD.from_.name
+        'Bitcoin'
+        >>> BTC_USD.from_.small_symbol
+        '₿'
+        >>>
+        ```
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-# MoC prices source
-
-Prices source for MoC projects
-
-
-
-## Refrences
-
-* [Source code in Github](https://github.com/money-on-chain/moc_prices_source)
-* [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
-
-
-
-## Requirements
-
-* Python 3.6+ support
-
-
-
-## Installation
-
-### From the Python package index (PyPI) 
-
-Run:
-
-```
-$ pip3 install moneyonchain-prices-source 
-```
-
-And then run:
-
-```
-$ moc_prices_source_check --version
-```
-
-To verify that it has been installed correctly
-
-### From source
-
-Download from [Github](https://github.com/money-on-chain/moc_prices_source)
-
-Standing inside the folder, run:
-
-```
-$ pip3 install -r requirements.txt 
-```
-
-For install the dependencies and then run:
-
-```
-$ pip3 install .
-```
-
-Finally run:
-
-```
-$ moc_prices_source_check --version
-```
-
-To verify that it has been installed correctly
-
-
-
-## Check that all is working ok
-
-```
-user@host:~$ moc_prices_source_check 
-
-From       To       Exchnage        Response  U.      Weigh     %  Time
----------  -------  ----------  ------------  ----  -------  ----  ------
-Bitcoin    Dollar   Bitfinex    15245         $        0.15  15.4  0.88s
-Bitcoin    Dollar   Bitstamp    15241.9       $        0.23  22.6  0.34s
-Bitcoin    Dollar   Coinbase    15236.5       $        0.4   40.3  0.27s
-Bitcoin    Dollar   Gemini      15246.8       $        0.06   6.4  0.87s
-Bitcoin    Dollar   Kraken      15239.4       $        0.15  15.2  0.4s
-RIF Token  Bitcoin  BitHumb         6.64e-06  ₿        0.33  33.3  3.09s
-RIF Token  Bitcoin  Coinbene        5.78e-06  ₿        0.33  33.3  1.27s
-RIF Token  Bitcoin  Kucoin          6.37e-06  ₿        0.33  33.3  1.16s
-
-Coin pair          Mediam             Mean    Weighted median  Sources
------------  ------------  ---------------  -----------------  ---------
-BTC/USD      15241.9       15241.9               15239.4       5
-RIF/BTC          6.37e-06      6.26333e-06           6.37e-06  3
-RIF/USD          0.097091      0.0954653             0.097075  N/A
-
-Response time 3.1s
-
-user@host:~$
-```
-
-More options
-
-```
-user@host:~$ moc_prices_source_check --help
-Usage: moc_prices_source_check [OPTIONS]
-
-Options:
-  -v, --version   Show version and exit.
-  -j, --json      Show data in JSON format and exit.
-  -w, --weighing  Show the default weighing and exit.
-  -h, --help      Show this message and exit.
-user@host:~$ 
-```
-
-
-## Usage
-
-Do some imports first
-
-```
-user@host:~$ python3
-Python 3.8.5 (default, Jul 28 2020, 12:59:40) 
-[GCC 9.3.0] on linux
-Type "help", "copyright", "credits" or "license" for more information.
->>> from moc_prices_source import get_price, BTC_USD, RIF_BTC, ALL
->>>
-```
-
-Get de BTC USD coin pair
-
-```
->>> get_price(BTC_USD)
-Decimal('13089.82')
->>> 
-```
-
-Get de RIF BTC coin pair
-
-```
->>> get_price(RIF_BTC)
-Decimal('0.00000713')
->>> 
-```
-
-Get errors detail (forced errors for example)
-
-```
->>> d = {}
->>> values = get_price(detail = d)
->>> for e in d['prices']:
-...     if not e["ok"]:
-...         print('{}: {}'.format(e["name"], e["error"]))
-...
-btc_usd_kraken: HTTPSConnectionPool(host='api.bad_uri.com', port=443): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.VerifiedHTTPSConnection object at 0x7f2c48700b50>: Failed to establish a new connection: [Errno -2] Name or service not known'))
->>>
-```
-
-Show the default weighing
-
-```
->>> from moc_prices_source.weighing import weighing
->>> print(weighing)
-Engine                  Weigh
-------------------  ---------
-btc_usd_bitstamp    0.22619
-btc_usd_bitfinex    0.153778
-btc_usd_kraken      0.152346
-btc_usd_coinbase    0.403366
-btc_usd_gemini      0.0643202
-rif_btc_bithumbpro  0.333333
-rif_btc_kucoin      0.333333
-rif_btc_coinbene    0.333333
->>> weighing.as_dict
-{'btc_usd_bitstamp': Decimal('0.226189632'), 'btc_usd_bitfinex': Decimal('0.1537782868'), 'btc_usd_kraken': Decimal('0.1523461274'), 'btc_usd_coinbase': Decimal('0.4033657328'), 'btc_usd_gemini': Decimal('0.06432022093'), 'rif_btc_bithumbpro': Decimal('0.333333333'), 'rif_btc_kucoin': Decimal('0.333333333'), 'rif_btc_coinbene': Decimal('0.333333333')}
->>> 
-```
-
-Override the default weighing
-
-```
->>> w = {"btc_usd_bitstamp": 0.2, "btc_usd_bitfinex": 0.8}
->>> get_price(weighing = w)
-Decimal('13070')
->>> 
-```
-
-Show all details of the coin pair obtained
-
-```
->>> import json
->>> d = {}
->>> values = get_price(ALL, detail = d, serializable = True)
->>>
->>> values
-{<BTC/USD Coin Pair object>: Decimal('15250.00000'), <RIF/BTC Coin Pair object>: Decimal('0.00000637'), <RIF/USD Coin Pair object>: Decimal('0.0971425000000')}
->>>
->>> print(json.dumps(d, indent=4, sort_keys=True))
-{
-    "prices": [
-        {
-            "coinpair": "BTC/USD",
-            "description": "Bitstamp",
-            "error": null,
-            "name": "btc_usd_bitstamp",
-            "ok": true,
-            "percentual_weighing": 0.22618963201583328,
-            "price": 15248.38,
-            "time": 0.279066,
-            "timeout": 10,
-            "timestamp": "2020-11-08 14:23:02",
-            "uri": "https://www.bitstamp.net/api/v2/ticker/btcusd/",
-            "volume": 10835.66006591,
-            "weighing": 0.226189632
-        },
-        {
-            "coinpair": "RIF/BTC",
-            "description": "Coinbene",
-            "error": null,
-            "name": "rif_btc_coinbene",
-            "ok": true,
-            "percentual_weighing": 0.3333333333333333,
-            "price": 5.8e-06,
-            "time": 1.571258,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:04",
-            "uri": "http://api.coinbene.com/v1/market/ticker?symbol=RIFBTC",
-            "volume": 806810.93,
-            "weighing": 0.333333333
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Bitfinex",
-            "error": null,
-            "name": "btc_usd_bitfinex",
-            "ok": true,
-            "percentual_weighing": 0.15377828681076447,
-            "price": 15248.22269385,
-            "time": 0.267649,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:02",
-            "uri": "https://api-pub.bitfinex.com/v2/ticker/tBTCUSD",
-            "volume": 14362.55862314,
-            "weighing": 0.1537782868
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Gemini",
-            "error": null,
-            "name": "btc_usd_gemini",
-            "ok": true,
-            "percentual_weighing": 0.06432022093450242,
-            "price": 15254.3,
-            "time": 0.952623,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:03",
-            "uri": "https://api.gemini.com/v1/pubticker/BTCUSD",
-            "volume": 0.0,
-            "weighing": 0.06432022093
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Coinbase",
-            "error": null,
-            "name": "btc_usd_coinbase",
-            "ok": true,
-            "percentual_weighing": 0.4033657328282356,
-            "price": 15251.88,
-            "time": 0.246729,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:02",
-            "uri": "https://api.coinbase.com/v2/prices/spot?currency=USD",
-            "volume": 0.0,
-            "weighing": 0.4033657328
-        },
-        {
-            "coinpair": "BTC/USD",
-            "description": "Kraken",
-            "error": null,
-            "name": "btc_usd_kraken",
-            "ok": true,
-            "percentual_weighing": 0.15234612741066422,
-            "price": 15250.0,
-            "time": 0.265883,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:02",
-            "uri": "https://api.kraken.com/0/public/Ticker?pair=XXBTZUSD",
-            "volume": 8018.38037875,
-            "weighing": 0.1523461274
-        },
-        {
-            "coinpair": "RIF/BTC",
-            "description": "Kucoin",
-            "error": null,
-            "name": "rif_btc_kucoin",
-            "ok": true,
-            "percentual_weighing": 0.3333333333333333,
-            "price": 6.37e-06,
-            "time": 0.932421,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:03",
-            "uri": "https://openapi-v2.kucoin.com/api/v1/market/orderbook/level1?symbol=RIF-BTC",
-            "volume": 963.5025,
-            "weighing": 0.333333333
-        },
-        {
-            "coinpair": "RIF/BTC",
-            "description": "BitHumb",
-            "error": null,
-            "name": "rif_btc_bithumbpro",
-            "ok": true,
-            "percentual_weighing": 0.3333333333333333,
-            "price": 6.67e-06,
-            "time": 1.836675,
-            "timeout": 10,
-            "timestamp": "2020-11-08 11:23:04",
-            "uri": "https://global-openapi.bithumb.pro/openapi/v1/spot/ticker?symbol=RIF-BTC",
-            "volume": 27932.67,
-            "weighing": 0.333333333
-        }
-    ],
-    "time": 1.882155,
-    "values": {
-        "BTC/USD": {
-            "mean_price": 15250.55653877,
-            "median_price": 15250.0,
-            "prices": [
-                15248.38,
-                15248.22269385,
-                15254.3,
-                15251.88,
-                15250.0
-            ],
-            "weighings": [
-                0.22618963201583328,
-                0.15377828681076447,
-                0.06432022093450242,
-                0.4033657328282356,
-                0.15234612741066422
-            ],
-            "weighted_median_price": 15250.0
-        },
-        "RIF/BTC": {
-            "mean_price": 6.28e-06,
-            "median_price": 6.37e-06,
-            "prices": [
-                5.8e-06,
-                6.37e-06,
-                6.67e-06
-            ],
-            "weighings": [
-                0.3333333333333333,
-                0.3333333333333333,
-                0.3333333333333333
-            ],
-            "weighted_median_price": 6.37e-06
-        },
-        "RIF/USD": {
-            "mean_price": 0.0957734950634756,
-            "median_price": 0.0971425,
-            "requirements": [
-                "RIF/BTC",
-                "BTC/USD"
-            ],
-            "weighted_median_price": 0.0971425
-        }
-    }
-}
->>> 
-```
-
-`Coin object` and `Coin Pair object` usage:
-
-```
->>> BTC_USD
-<BTC/USD Coin Pair object>
->>> str(BTC_USD)
-'BTC/USD'
->>> BTC_USD.from_
-<Bitcoin Coin object>
->>> str(BTC_USD.from_)
-'BTC'
->>> BTC_USD.to_
-<Dollar Coin object>
->>> str(BTC_USD.to_)
-'USD'
->>> BTC_USD.from_.symbol
-'BTC'
->>> BTC_USD.from_.name
-'Bitcoin'
->>> BTC_USD.from_.small_symbol
-'₿'
->>>
-```
```

### Comparing `moneyonchain_prices_source-0.6.3/setup.py` & `moneyonchain_prices_source-0.6.4b0/setup.py`

 * *Files identical despite different names*

