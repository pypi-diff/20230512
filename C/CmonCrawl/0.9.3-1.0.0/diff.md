# Comparing `tmp/CmonCrawl-0.9.3.tar.gz` & `tmp/CmonCrawl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CmonCrawl-0.9.3.tar", last modified: Thu May 11 23:40:28 2023, max compression
+gzip compressed data, was "CmonCrawl-1.0.0.tar", last modified: Fri May 12 21:43:44 2023, max compression
```

## Comparing `CmonCrawl-0.9.3.tar` & `CmonCrawl-1.0.0.tar`

### file list

```diff
@@ -1,926 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.949669 CmonCrawl-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.809658 CmonCrawl-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/.github/workflows/test_and_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/.vscode/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/CmonCrawl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-11 23:40:28.000000 CmonCrawl-0.9.3/CmonCrawl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    59630 2023-05-11 23:40:28.000000 CmonCrawl-0.9.3/CmonCrawl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:40:28.000000 CmonCrawl-0.9.3/CmonCrawl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 23:40:28.000000 CmonCrawl-0.9.3/CmonCrawl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-11 23:40:28.000000 CmonCrawl-0.9.3/CmonCrawl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 23:40:28.000000 CmonCrawl-0.9.3/CmonCrawl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-11 23:40:28.949669 CmonCrawl-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/aggregator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/aggregator/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/aggregator/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15299 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/aggregator/index_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/aggregator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/aggregator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/aggregator/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/aggregator/utils/ndjson_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/common/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/integrations/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/integrations/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/integrations/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/middleware/stompware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/middleware/synchronized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.825659 CmonCrawl-0.9.3/cmoncrawl/processor/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/extraction/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.829659 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.829659 CmonCrawl-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.829659 CmonCrawl-0.9.3/docs/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.829659 CmonCrawl-0.9.3/docs/build/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/_templates/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.829659 CmonCrawl-0.9.3/docs/build/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/api.doctree
--rw-r--r--   0 runner    (1001) docker     (123)   432023 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.853661 CmonCrawl-0.9.3/docs/build/doctrees/generated/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.DomainCrawl.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.DomainRecord.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aclose.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.aopen.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.RetrieveResponse.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.index_query.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.decode.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.aggregator.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    23297 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    63109 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    22264 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.article_utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.ArticleUtils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.Downloader.download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.downloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    21634 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Downloader.dummy_downloader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.dummy_extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Extractor.extractor_utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.dummy_streamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.outstreamer.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    26191 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    20720 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.OutStreamer.stream_to_file.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Pipeline.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Pipeline.pipeline.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Route.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    19442 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_module.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.load_modules.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.register_routes.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.Router.route.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.Router.router.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.processor_utils.DomainRecord.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    21042 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.processor_utils.PipeMetadata.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.App.processor_utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.process_article.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    29297 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_before_message.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_connected.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_connecting.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnected.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_disconnecting.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_error.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_heartbeat_timeout.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_message.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_receipt.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_receiver_loop_completed.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Listener.on_send.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.ListnerStats.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    15725 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.ListnerStats.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Message.__init__.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.Message.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/generated/Processor.processor.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/installation.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.853661 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/artemis-queue.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/download_article.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/installation.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/middleware.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/overview.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    45690 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/doctrees/quickstart/quick-start.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.853661 CmonCrawl-0.9.3/docs/build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.853661 CmonCrawl-0.9.3/docs/build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/api.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.877663 CmonCrawl-0.9.3/docs/build/html/_sources/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainCrawl.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.DomainRecord.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.aclose.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.aopen.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.IndexAggregator.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.RetrieveResponse.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.RetrieveResponse.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.index_query.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.decode.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.Decoder.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.ndjson_decoder.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.App.utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.aggregator.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Aggregator.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.article_utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.ArticleUtils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.Downloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.downloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.dummy_downloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Downloader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.dummy_extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.BaseExtractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.extractor_utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Extractor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.dummy_streamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.outstreamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.OutStreamer.stream_to_file.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Pipeline.pipeline.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Pipeline.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Route.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.load_module.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.load_modules.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.register_route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.register_routes.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.route.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.Router.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.router.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.Router.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.processor_utils.DomainRecord.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.processor_utils.PipeMetadata.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.processor_utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.App.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.process_article.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_before_message.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_connected.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_connecting.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_disconnected.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_disconnecting.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_error.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_heartbeat.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_heartbeat_timeout.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_message.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_receipt.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_receiver_loop_completed.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.on_send.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Listener.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.ListnerStats.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.ListnerStats.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Message.__init__.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.Message.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.processor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/generated/Processor.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/installation.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.877663 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/artemis-queue.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/download_article.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/installation.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/middleware.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/overview.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_sources/quickstart/quick-start.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.881664 CmonCrawl-0.9.3/docs/build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.813658 CmonCrawl-0.9.3/docs/build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.817659 CmonCrawl-0.9.3/docs/build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.885664 CmonCrawl-0.9.3/docs/build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    87299 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   162094 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.889664 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.893665 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.917667 CmonCrawl-0.9.3/docs/build/html/generated/
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.html
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.html
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.DomainRecord.html
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aclose.html
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.aopen.html
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.html
--rw-r--r--   0 runner    (1001) docker     (123)    19039 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.html
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.html
--rw-r--r--   0 runner    (1001) docker     (123)    28037 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.IndexAggregator.html
--rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    20354 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.RetrieveResponse.html
--rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.html
--rw-r--r--   0 runner    (1001) docker     (123)    20028 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.decode.html
--rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.html
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.html
--rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.ndjson_decoder.html
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.aggregator.html
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.html
--rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.html
--rw-r--r--   0 runner    (1001) docker     (123)    17957 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17499 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    35243 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17503 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.html
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    18043 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.article_utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.ArticleUtils.html
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.download.html
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.Downloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.html
--rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.html
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.download.html
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.html
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.downloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.html
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.html
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.html
--rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.html
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.dummy_downloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Downloader.html
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    20711 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.html
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.dummy_extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.html
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.html
--rw-r--r--   0 runner    (1001) docker     (123)    17215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.html
--rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.html
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.extractor_utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Extractor.html
--rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    18928 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.dummy_streamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    18768 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.outstreamer.html
--rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    16961 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.html
--rw-r--r--   0 runner    (1001) docker     (123)    24427 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.html
--rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.html
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.html
--rw-r--r--   0 runner    (1001) docker     (123)    22651 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.html
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.html
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.html
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.html
--rw-r--r--   0 runner    (1001) docker     (123)    22694 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.html
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.html
--rw-r--r--   0 runner    (1001) docker     (123)    17546 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.html
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.OutStreamer.stream_to_file.html
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Pipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)    16946 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.html
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Pipeline.pipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)    14956 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.html
--rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Route.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Route.html
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.html
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.load_module.html
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.load_modules.html
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.register_route.html
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.register_routes.html
--rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.Router.route.html
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.Router.router.html
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.html
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    24125 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.processor_utils.DomainRecord.html
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    22093 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.processor_utils.PipeMetadata.html
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.App.processor_utils.html
--rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.html
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.process_article.html
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    24450 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.html
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_before_message.html
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_connected.html
--rw-r--r--   0 runner    (1001) docker     (123)    16819 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_connecting.html
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_disconnected.html
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_disconnecting.html
--rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_error.html
--rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_heartbeat.html
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_heartbeat_timeout.html
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_message.html
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_receipt.html
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_receiver_loop_completed.html
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Listener.on_send.html
--rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.ListnerStats.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.ListnerStats.html
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Message.__init__.html
--rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.Message.html
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/generated/Processor.processor.html
--rw-r--r--   0 runner    (1001) docker     (123)    56110 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/installation.html
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/py-modindex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.921667 CmonCrawl-0.9.3/docs/build/html/quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/artemis-queue.html
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/download_article.html
--rw-r--r--   0 runner    (1001) docker     (123)    16829 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/installation.html
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/middleware.html
--rw-r--r--   0 runner    (1001) docker     (123)    25924 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/overview.html
--rw-r--r--   0 runner    (1001) docker     (123)    42595 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/quickstart/quick-start.html
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)    75786 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.921667 CmonCrawl-0.9.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.941669 CmonCrawl-0.9.3/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.DomainCrawl.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.DomainRecord.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.DomainRecord.rst
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.aclose.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.aopen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_all_CC_indexes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_captured_responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.get_number_of_pages.rst
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.IndexAggregator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.RetrieveResponse.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.RetrieveResponse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.index_query.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.decode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.raw_decode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.ndjson_decoder.Decoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.ndjson_decoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.App.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.aggregator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Aggregator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.article_extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.check_required.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.custom_filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.extract_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.ArticleExtractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.article_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.ArticleUtils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.Downloader.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.Downloader.download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.Downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.aclose.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.aopen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.DownloaderFull.unwrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.extract_year.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.mine_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.DownloaderDummy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.dummy_downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Downloader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.extract_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.Extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.dummy_extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.extract.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.extract_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_raw.rst
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.filter_soup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.BaseExtractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.extractor_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Extractor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.DummyStreamer.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.dummy_streamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.outstreamer.OutStreamer.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.outstreamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.get_file_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.metadata_to_string.rst
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileDefault.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.get_file_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.metadata_to_string.rst
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileHTMLContent.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.clean_up.rst
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.get_file_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.metadata_to_string.rst
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.OutStreamerFileJSON.stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.OutStreamer.stream_to_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.process_domain_record.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Pipeline.pipeline.ProcessorPipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Pipeline.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Route.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.load_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.load_modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.register_route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.register_routes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.Router.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.router.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.Router.rst
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.processor_utils.DomainRecord.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.processor_utils.DomainRecord.rst
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.processor_utils.PipeMetadata.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.processor_utils.PipeMetadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.processor_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.App.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.process_article.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_before_message.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_connected.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_connecting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_disconnected.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_disconnecting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_error.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_heartbeat.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_heartbeat_timeout.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_message.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_receipt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_receiver_loop_completed.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.on_send.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Listener.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.ListnerStats.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.ListnerStats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Message.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.Message.rst
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/generated/Processor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.941669 CmonCrawl-0.9.3/docs/source/quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/quickstart/artemis-queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/quickstart/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/quickstart/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/docs/source/quickstart/quick-start.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.821659 CmonCrawl-0.9.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.941669 CmonCrawl-0.9.3/examples/extractor_tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.941669 CmonCrawl-0.9.3/examples/extractor_tutorial/Extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/examples/extractor_tutorial/Extractors/bbc_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/examples/extractor_tutorial/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 23:40:28.949669 CmonCrawl-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.945669 CmonCrawl-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/aggregator_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/end_to_end_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/processor_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.945669 CmonCrawl-0.9.3/tests/test_extract/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/test_extract/cfg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.945669 CmonCrawl-0.9.3/tests/test_extract/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/test_extract/extractors/test_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.945669 CmonCrawl-0.9.3/tests/test_extract/files/
--rw-r--r--   0 runner    (1001) docker     (123)   828135 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/test_extract/files/file.html
--rw-r--r--   0 runner    (1001) docker     (123)  1743032 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/test_extract/files/file.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:40:28.949669 CmonCrawl-0.9.3/tests/test_routes/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/test_routes/a.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 23:40:10.000000 CmonCrawl-0.9.3/tests/test_routes/b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.379611 CmonCrawl-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.315610 CmonCrawl-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/.github/workflows/test_and_push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/.vscode/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/CmonCrawl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-12 21:43:44.000000 CmonCrawl-1.0.0/CmonCrawl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-05-12 21:43:44.000000 CmonCrawl-1.0.0/CmonCrawl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:43:44.000000 CmonCrawl-1.0.0/CmonCrawl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 21:43:44.000000 CmonCrawl-1.0.0/CmonCrawl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-12 21:43:44.000000 CmonCrawl-1.0.0/CmonCrawl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 21:43:44.000000 CmonCrawl-1.0.0/CmonCrawl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-12 21:43:44.379611 CmonCrawl-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/cmoncrawl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/cmoncrawl/aggregator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/cmoncrawl/aggregator/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/aggregator/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/aggregator/index_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/cmoncrawl/aggregator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/aggregator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/aggregator/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/aggregator/utils/ndjson_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.339610 CmonCrawl-1.0.0/cmoncrawl/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/common/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.343610 CmonCrawl-1.0.0/cmoncrawl/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/integrations/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/integrations/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/integrations/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.343610 CmonCrawl-1.0.0/cmoncrawl/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/middleware/stompware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/middleware/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.343610 CmonCrawl-1.0.0/cmoncrawl/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.343610 CmonCrawl-1.0.0/cmoncrawl/processor/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/extraction/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.343610 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.347611 CmonCrawl-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.319610 CmonCrawl-1.0.0/docs/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.347611 CmonCrawl-1.0.0/docs/build/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/doctrees/api.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)   457471 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.347611 CmonCrawl-1.0.0/docs/build/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.351611 CmonCrawl-1.0.0/docs/build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_sources/api.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.319610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.355611 CmonCrawl-1.0.0/docs/build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.323610 CmonCrawl-1.0.0/docs/build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.359611 CmonCrawl-1.0.0/docs/build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.327610 CmonCrawl-1.0.0/docs/build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.363611 CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.367611 CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.367611 CmonCrawl-1.0.0/docs/build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    87299 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.367611 CmonCrawl-1.0.0/docs/build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   162094 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.331610 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.367611 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.367611 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/api.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/build/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.335610 CmonCrawl-1.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/examples/extractor_tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/examples/extractor_tutorial/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/examples/extractor_tutorial/Extractors/bbc_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/examples/extractor_tutorial/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:43:44.379611 CmonCrawl-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/aggregator_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/end_to_end_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/processor_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/tests/test_extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/test_extract/cfg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.375611 CmonCrawl-1.0.0/tests/test_extract/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/test_extract/extractors/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.379611 CmonCrawl-1.0.0/tests/test_extract/files/
+-rw-r--r--   0 runner    (1001) docker     (123)   828135 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/test_extract/files/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1743032 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/test_extract/files/file.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:43:44.379611 CmonCrawl-1.0.0/tests/test_routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/test_routes/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-12 21:43:22.000000 CmonCrawl-1.0.0/tests/test_routes/b.py
```

### Comparing `CmonCrawl-0.9.3/.github/workflows/test_and_push.yml` & `CmonCrawl-1.0.0/.github/workflows/test_and_push.yml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/.gitignore` & `CmonCrawl-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/.vscode/launch.json` & `CmonCrawl-1.0.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/CmonCrawl.egg-info/PKG-INFO` & `CmonCrawl-1.0.0/CmonCrawl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 0.9.3
+Version: 1.0.0
 License: MIT License
         
         Copyright (c) [2023] [Hynek Kydlíček]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `CmonCrawl-0.9.3/LICENSE` & `CmonCrawl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/PKG-INFO` & `CmonCrawl-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CmonCrawl
-Version: 0.9.3
+Version: 1.0.0
 License: MIT License
         
         Copyright (c) [2023] [Hynek Kydlíček]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `CmonCrawl-0.9.3/README.md` & `CmonCrawl-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/cmoncrawl/aggregator/index_query.py` & `CmonCrawl-1.0.0/cmoncrawl/aggregator/index_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,22 +20,49 @@
 from cmoncrawl.common.types import (
     DomainRecord,
     RetrieveResponse,
     DomainCrawl,
     MatchType,
 )
 
-from aiohttp import ClientError, ClientSession, ContentTypeError
+from aiohttp import ClientError, ClientSession, ContentTypeError, ServerConnectionError
 import asyncio
 import random
 
 ALLOWED_ERR_FOR_RETRIES = [500, 502, 503, 504]
 
 
 class IndexAggregator(AsyncIterable[DomainRecord]):
+    """
+    This class is responsible for aggregating the index files from commoncrawl.
+    It is an async context manager which can then be used as an async iterator
+    which yields DomainRecord objects, found in the index files of commoncrawl.
+
+    It uses the commoncrawl index server to find the index files.
+
+
+    Args:
+        domains (List[str]): A list of domains to search for.
+        cc_indexes_server (str, optional): The commoncrawl index server to use. Defaults to "http://index.commoncrawl.org/collinfo.json".
+        match_type (MatchType, optional): Match type for cdx-api. Defaults to None.
+        cc_servers (List[str], optional): A list of commoncrawl servers to use. If [], then indexes will be retrieved from the cc_indexes_server. Defaults to [].
+        since (datetime, optional): The start date for the search. Defaults to datetime.min.
+        to (datetime, optional): The end date for the search. Defaults to datetime.max.
+        limit (int, optional): The maximum number of results to return. Defaults to None.
+        max_retry (int, optional): The maximum number of retries for a single request. Defaults to 5.
+        prefetch_size (int, optional): The number of indexes to fetch concurrently. Defaults to 3.
+        sleep_step (int, optional): Sleep increase time between retries. Defaults to 20.
+
+    Examples:
+        >>> async with IndexAggregator(["example.com"]) as aggregator:
+        >>>     async for domain_record in aggregator:
+        >>>         print(domain_record)
+
+    """
+
     def __init__(
         self,
         domains: List[str],
         cc_indexes_server: str = "http://index.commoncrawl.org/collinfo.json",
         match_type: MatchType | None = None,
         cc_servers: List[str] = [],
         since: datetime = datetime.min,
@@ -138,29 +165,28 @@
                 async with client.get(cdx_server, params=params) as response:
                     status = response.status
                     if not response.ok:
                         reason = response.reason if response.reason else "Unknown"
                         if not should_retry(retry, reason, status, **args):
                             break
                     else:
-                        try:
-                            content = await response.json(
-                                content_type=content_type, loads=Decoder().decode
-                            )
-                        except ContentTypeError as e:
-                            all_purpose_logger.error(str(e), exc_info=True)
-                            all_purpose_logger.error(e.message, exc_info=True)
-                            all_purpose_logger.error(response.content)
-                            break
+                        content = await response.json(
+                            content_type=content_type, loads=Decoder().decode
+                        )
                         all_purpose_logger.info(
                             f"Successfully retrieved page of {domain} from {cdx_server} add_info: {args}"
                         )
                         break
 
-            except (ClientError, TimeoutError) as e:
+            except (
+                ClientError,
+                TimeoutError,
+                ServerConnectionError,
+                ContentTypeError,
+            ) as e:
                 reason = f"{type(e)} {str(e)}"
                 if not should_retry(retry, reason, 500, **args):
                     break
 
             await asyncio.sleep(random.randint(0, (retry + 1) * sleep_step))
         return RetrieveResponse(status, content, reason)
 
@@ -247,14 +273,17 @@
                 )
                 for js in reponse.content
             ]
         return reponse
 
     @staticmethod
     async def get_all_CC_indexes(client: ClientSession, cdx_server: str) -> List[str]:
+        """
+        Get all CC index servers from a given CDX server
+        """
         for _ in range(3):
             async with client.get(cdx_server) as response:
                 r_json = await response.json(content_type="application/json")
                 CC_servers = [js["cdx-api"] for js in r_json]
                 return CC_servers
         all_purpose_logger.error(
             f"Failed to get CC servers from {cdx_server} after 3 attempts"
@@ -304,14 +333,17 @@
                         and crawl_to_year(crawl) <= self.__to.year
                     )
                     for domain in domains
                 ]
             )
 
         async def __prefetch_next_crawl(self) -> int:
+            """
+            Prefetch the next index server
+            """
             while len(self.__crawls_remaining) > 0:
                 next_crawl = self.__crawls_remaining.popleft()
 
                 retr = await IndexAggregator.get_number_of_pages(
                     self.__client,
                     next_crawl.cdx_server,
                     next_crawl.domain,
@@ -329,14 +361,17 @@
                     self.prefetch_queue.add(
                         asyncio.create_task(self.__fetch_next_dc(dc, 0))
                     )
                 return pages
             return 0
 
         async def __await_next_prefetch(self):
+            """
+            Gets the next index retry
+            """
             # Wait for the next prefetch to finish
             # Don't prefetch if limit is set to avoid overfetching
             while len(self.__crawls_remaining) > 0 and (
                 len(self.prefetch_queue) == 0
                 or (
                     self.__limit is None
                     and len(self.prefetch_queue) <= self.__opt_prefetch_size
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/aggregator/utils/helpers.py` & `CmonCrawl-1.0.0/cmoncrawl/aggregator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/cmoncrawl/common/loggers.py` & `CmonCrawl-1.0.0/cmoncrawl/common/loggers.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/cmoncrawl/common/types.py` & `CmonCrawl-1.0.0/cmoncrawl/common/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from dataclasses_json import dataclass_json, config
 
 
 @dataclass_json
 @dataclass
 class DomainRecord:
+    """
+    Domain record.
+    """
+
     filename: str
     url: str | None
     offset: int
     length: int
     digest: str | None = None
     encoding: str | None = None
     timestamp: datetime | None = field(
@@ -38,21 +42,29 @@
 
     def __post_init__(self):
         self.url_parsed = urlparse(self.domain_record.url)
 
 
 @dataclass
 class RetrieveResponse:
+    """
+    Response from retrieve.
+    """
+
     status: int
     content: Any
     reason: None | str
 
 
 @dataclass
 class DomainCrawl:
+    """
+    Domain crawl.
+    """
+
     domain: str = ""
     cdx_server: str = ""
     page: int = 0
 
 
 # ===============================================================================
 # Extractor config
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/integrations/commands.py` & `CmonCrawl-1.0.0/cmoncrawl/integrations/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,32 @@
 from cmoncrawl.common.loggers import (
     all_purpose_logger,
     metadata_logger,
 )
 
 
 def add_args(parser: argparse.ArgumentParser):
-    parser.add_argument("--debug", action="store_true", default=False)
+    parser.add_argument(
+        "--debug", action="store_true", default=False, help="Debug mode"
+    )
     return parser
 
 
 def add_subparsers(parser: Any):
     parsers: Dict[str, argparse.ArgumentParser] = {}
     for add_args_fc in [add_download_args, add_extract_args]:
         add_args_fc(parser)
     return parsers
 
 
 def get_args():
     parser = argparse.ArgumentParser()
-    subparser = parser.add_subparsers(dest="command", required=True)
+    subparser = parser.add_subparsers(
+        dest="command", required=True, help="Command to run"
+    )
     add_subparsers(subparser)
     return parser
 
 
 def setup_loggers(debug: bool):
     if debug:
         all_purpose_logger.setLevel(logging.DEBUG)
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/integrations/download.py` & `CmonCrawl-1.0.0/cmoncrawl/integrations/download.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, List
 from cmoncrawl.aggregator.index_query import IndexAggregator
 from cmoncrawl.common.types import MatchType
 from cmoncrawl.processor.pipeline.downloader import AsyncDownloader
 from cmoncrawl.processor.pipeline.pipeline import ProcessorPipeline
 from cmoncrawl.processor.pipeline.streamer import StreamerFileHTML
 from cmoncrawl.processor.pipeline.extractor import HTMLExtractor, DomainRecordExtractor
-from cmoncrawl.middleware.synchronized import index_and_extract
+from cmoncrawl.middleware.synchronized import query_and_extract
 import argparse
 import asyncio
 from cmoncrawl.processor.pipeline.streamer import (
     StreamerFileJSON,
 )
 
 from cmoncrawl.processor.pipeline.router import Router
@@ -20,43 +20,91 @@
 
 class DownloadOutputFormat(Enum):
     RECORD = "record"
     HTML = "html"
 
 
 def add_mode_args(subparser: Any):
-    record_parser = subparser.add_parser(DownloadOutputFormat.RECORD.value)
-    record_parser.add_argument("--max_crawls_per_file", type=int, default=500_000)
-    subparser.add_parser(DownloadOutputFormat.HTML.value)
+    record_parser = subparser.add_parser(
+        DownloadOutputFormat.RECORD.value,
+        help="Download record files from Common Crawl",
+    )
+    record_parser.add_argument(
+        "--max_crawls_per_file",
+        type=int,
+        default=500_000,
+        help="Max number of domain records per file output",
+    )
+    subparser.add_parser(
+        DownloadOutputFormat.HTML.value, help="Download HTML files from Common Crawl"
+    )
     return subparser
 
 
 def add_args(subparser: Any):
-    parser = subparser.add_parser("download")
-    parser.add_argument("url")
-    parser.add_argument("output", type=Path)
-    mode_subparser = parser.add_subparsers(dest="mode", required=True)
+    parser = subparser.add_parser("download", help="Download data from Common Crawl")
+    parser.add_argument("url", type=str, help="URL to query")
+    parser.add_argument("output", type=Path, help="Path to output directory")
+    mode_subparser = parser.add_subparsers(
+        dest="mode", required=True, help="Download mode"
+    )
     mode_subparser = add_mode_args(mode_subparser)
-    parser.add_argument("--limit", type=int, default=5)
     parser.add_argument(
-        "--since", type=datetime.fromisoformat, default=str(datetime.min)
+        "--limit", type=int, default=5, help="Max number of urls to download"
+    )
+    parser.add_argument(
+        "--since",
+        type=datetime.fromisoformat,
+        default=str(datetime.min),
+        help="Start date in ISO format e.g. 2020-01-01",
+    )
+    parser.add_argument(
+        "--to",
+        type=datetime.fromisoformat,
+        default=str(datetime.max),
+        help="End date in ISO format e.g. 2020-01-01",
+    )
+    parser.add_argument(
+        "--cc_server",
+        nargs="+",
+        type=str,
+        default=None,
+        help="Common Crawl indexes to query, must provide whole url e.g. https://index.commoncrawl.org/CC-MAIN-2023-14-index",
+    )
+    parser.add_argument(
+        "--max_retry",
+        type=int,
+        default=30,
+        help="Max number of retries for a request, when the requests are failing increase this number",
+    )
+    parser.add_argument(
+        "--sleep_step",
+        type=int,
+        default=4,
+        help="Number of increased second to add to sleep time between each failed download attempt, increase this number if the server tell you to slow down",
     )
-    parser.add_argument("--to", type=datetime.fromisoformat, default=str(datetime.max))
-    parser.add_argument("--cc_server", nargs="+", type=str, default=None)
-    parser.add_argument("--max_retry", type=int, default=30)
-    parser.add_argument("--sleep_step", type=int, default=4)
     # Add option to output to either json or html
     parser.add_argument(
         "--match_type",
         type=MatchType,
         choices=list(MatchType.__members__.values()),
-        default=MatchType.PREFIX,
+        help="Match type for the url, see cdx-api for more info",
+    )
+    parser.add_argument(
+        "--max_directory_size",
+        type=int,
+        default=1000,
+        help="Max number of files per directory",
+    )
+    parser.add_argument(
+        "--filter_non_200",
+        action="store_true",
+        default=True,
+        help="Filter out non 200 status code",
     )
-    parser.add_argument("--max_directory_size", type=int, default=1000)
-    parser.add_argument("--filter_non_200", action="store_true", default=True)
     parser.set_defaults(func=run_download)
 
 
 def url_download_prepare_router(
     output_format: DownloadOutputFormat, filter_non_200: bool
 ):
     router = Router()
@@ -119,15 +167,15 @@
         match_type=match_type,
         since=since,
         to=to,
         limit=limit,
         max_retry=max_retry,
         sleep_step=sleep_step,
     )
-    await index_and_extract(index_agg, pipeline)
+    await query_and_extract(index_agg, pipeline)
 
 
 def run_download(args: argparse.Namespace):
     mode = DownloadOutputFormat(args.mode)
     return asyncio.run(
         url_download(
             args.url,
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/integrations/extract.py` & `CmonCrawl-1.0.0/cmoncrawl/integrations/extract.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,38 +23,80 @@
 
 class ExtractMode(Enum):
     HTML = "html"
     RECORD = "record"
 
 
 def add_mode_args(subparser: Any):
-    record_parser = subparser.add_parser(ExtractMode.RECORD.value)
-    record_parser.add_argument("--max_retry", type=int, default=30)
-    record_parser.add_argument("--sleep_step", type=int, default=4)
+    record_parser = subparser.add_parser(
+        ExtractMode.RECORD.value, help="Extract data from jsonl record files"
+    )
+    record_parser.add_argument(
+        "--max_retry", type=int, default=30, help="Max number of warc download attempts"
+    )
+    record_parser.add_argument(
+        "--sleep_step",
+        type=int,
+        default=4,
+        help="Number of increased second to add to sleep time between each failed download attempt",
+    )
 
-    html_parser = subparser.add_parser(ExtractMode.HTML.value)
+    html_parser = subparser.add_parser(
+        ExtractMode.HTML.value, help="Extract data from HTML files"
+    )
     html_parser.add_argument(
-        "--date", type=datetime.fromisoformat, default=str(datetime.now())
+        "--date",
+        type=datetime.fromisoformat,
+        default=str(datetime.now()),
+        help="Date of extraction of HTML files in iso format e.g. 2021-01-01, default is today",
+    )
+    html_parser.add_argument(
+        "--url",
+        type=str,
+        default="",
+        help="URL from which the HTML files were downloaded, by default it will try to infer from file content",
     )
-    html_parser.add_argument("--url", type=str, default="")
     return subparser
 
 
 def add_args(subparser: Any):
-    parser = subparser.add_parser("extract")
+    parser = subparser.add_parser(
+        "extract", help="Extract data from records/html files"
+    )
     parser.add_argument(
         "config_path",
         type=Path,
+        help="Path to config file containing extraction rules",
+    )
+    parser.add_argument("output_path", type=Path, help="Path to output directory")
+    parser.add_argument(
+        "files", nargs="+", type=Path, help="Files to extract data from"
+    )
+    parser.add_argument(
+        "--max_crawls_per_file",
+        type=int,
+        default=500_000,
+        help="Max number of extractions per file output",
+    )
+    parser.add_argument(
+        "--max_directory_size",
+        type=int,
+        default=1000,
+        help="Max number of extraction files per directory",
+    )
+    parser.add_argument(
+        "--n_proc",
+        type=int,
+        default=1,
+        help="Number of processes to use for extraction. The paralelization is on file level, thus for single file it's useless to use more than one process.",
+    )
+
+    mode_subparser = parser.add_subparsers(
+        dest="mode", required=True, help="Extraction mode"
     )
-    parser.add_argument("output_path", type=Path)
-    parser.add_argument("files", nargs="+", type=Path)
-    parser.add_argument("--max_crawls_per_file", type=int, default=500_000)
-    parser.add_argument("--max_directory_size", type=int, default=1000)
-    parser.add_argument("--n_proc", type=int, default=1)
-    mode_subparser = parser.add_subparsers(dest="mode", required=True)
     mode_subparser = add_mode_args(mode_subparser)
     parser.set_defaults(func=run_extract)
 
 
 def get_extract_downloader(
     mode: ExtractMode,
     files_path: List[Path],
@@ -87,15 +129,15 @@
     return records
 
 
 def get_domain_records_html(
     url: str | None, date: datetime | None
 ) -> List[Tuple[DomainRecord, Dict[str, Any]]]:
     # Just return dummy as correct crawl will be loaded from dummy downloader
-    return [DomainRecord("", url=url, offset=0, length=0, timestamp=date), {}]
+    return [(DomainRecord("", url=url, offset=0, length=0, timestamp=date), {})]
 
 
 def load_config(config_path: Path) -> ExtractConfig:
     with open(config_path, "r") as f:
         config = json.load(f)
     return ExtractConfig.schema().load(config)
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/middleware/synchronized.py` & `CmonCrawl-1.0.0/cmoncrawl/middleware/synchronized.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,47 +5,58 @@
 from cmoncrawl.common.types import DomainRecord
 from cmoncrawl.common.loggers import all_purpose_logger, metadata_logger
 from cmoncrawl.aggregator.utils.helpers import unify_url_id
 from tqdm import tqdm
 import asyncio
 
 
-async def index_and_extract(
+async def query_and_extract(
     index_agg: IndexAggregator,
     pipeline: ProcessorPipeline,
     filter_non_unique_url: bool = False,
 ):
+    """
+    Query the index and extracts the results using the pipeline
+
+    Args:
+        index_agg (IndexAggregator): Index aggregator
+        pipeline (ProcessorPipeline): Pipeline to use
+        filter_non_unique_url (bool, optional): Filter non unique urls.
+            if True, only first successful extraction of a url will be processed,
+            the rest will be skipped. Defaults to False.
+
+    """
     processed_urls: Set[str] = set()
     total_extracted: int = 0
 
     if hasattr(pipeline.downloader, "__aenter__"):
         await pipeline.downloader.__aenter__()
     try:
         async with index_agg:
             async for domain_record in index_agg:
                 url = domain_record.url or ""
                 if filter_non_unique_url and unify_url_id(url) in processed_urls:
                     continue
                 try:
                     await pipeline.process_domain_record(domain_record, {})
                     total_extracted += 1
+                    processed_urls.add(unify_url_id(url))
                 except KeyboardInterrupt as e:
                     break
 
                 except Exception as e:
                     all_purpose_logger.error(
                         f"Failed to process {domain_record.url} with {e}"
                     )
-                    continue
-                processed_urls.add(unify_url_id(url))
 
     finally:
         if hasattr(pipeline.downloader, "__aexit__"):
             await pipeline.downloader.__aexit__(None, None, None)
     all_purpose_logger.info(f"Extracted {total_extracted} urls")
+    return processed_urls
 
 
 async def _extract_task(
     domain_record: DomainRecord,
     additional_info: Dict[str, Any],
     pipeline: ProcessorPipeline,
 ):
@@ -62,16 +73,26 @@
     return result
 
 
 async def extract(
     records: List[Tuple[DomainRecord, Dict[str, Any]]],
     pipeline: ProcessorPipeline,
     concurrent_length: int = 20,
-    timeout: int = 5,
 ):
+    """
+    Extracts the records using the pipeline, with at most `concurrent_length`
+    records being processed at the same time.
+
+    Args:
+        records (List[Tuple[DomainRecord, Dict[str, Any]]]): List of records to process and additional info
+        pipeline (ProcessorPipeline): Pipeline to use
+        concurrent_length (int, optional): Number of concurrent records to process.
+            Defaults to 20.
+
+    """
     domain_records_iterator = iter(tqdm(records))
     domains_exausted = False
     total_extracted: int = 0
     if hasattr(pipeline.downloader, "__aenter__"):
         await pipeline.downloader.__aenter__()
     try:
         queue: Set[asyncio.Task[List[Path]]] = set()
@@ -86,17 +107,15 @@
 
                 queue.add(
                     asyncio.create_task(
                         _extract_task(next_domain_record, additional_info, pipeline)
                     )
                 )
 
-            done, queue = await asyncio.wait(
-                queue, timeout=timeout, return_when=asyncio.FIRST_COMPLETED
-            )
+            done, queue = await asyncio.wait(queue, return_when=asyncio.FIRST_COMPLETED)
             for task in done:
                 try:
                     await task
                     total_extracted += 1
                 except KeyboardInterrupt as e:
                     break
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/processor/extraction/filters.py` & `CmonCrawl-1.0.0/cmoncrawl/processor/extraction/filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,34 @@
 
 
 def must_exist_filter(soup: BeautifulSoup, filter_list: List[str]):
     """
     This function takes in a BeautifulSoup object and a list of
     CSS selectors.
     If all selectors are found in the soup, this function returns True.
+
+    Args:
+        soup (BeautifulSoup): BeautifulSoup object
+        filter_list (List[str]): List of CSS selectors
+
     """
     must_exist = [soup.select_one(css_selector) for css_selector in filter_list]
     if any(map(lambda x: x is None, must_exist)):
         return False
 
     return True
 
 
 def must_not_exist_filter(soup: BeautifulSoup, filter_list: List[str]):
     """
     This function takes in a BeautifulSoup object and a list of
     CSS selectors.
     If any selector is found in the soup, this function returns False.
+    Args:
+        soup (BeautifulSoup): BeautifulSoup object
+        filter_list (List[str]): List of CSS selectors
     """
     must_not_exist = [soup.select_one(css_selector) for css_selector in filter_list]
     if any(map(lambda x: x is not None, must_not_exist)):
         return False
 
     return True
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/downloader.py` & `CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 from datetime import datetime
 import io
 from pathlib import Path
 import random
 import re
 from types import TracebackType
-from aiohttp import ClientError, ClientSession
+from aiohttp import ClientError, ClientSession, ContentTypeError, ServerConnectionError
 from typing import List, Tuple, Type
 from aiofiles import open as asyncOpen
 
 
 import bs4
 
 from cmoncrawl.common.types import (
@@ -20,21 +20,37 @@
 from cmoncrawl.common.loggers import metadata_logger, all_purpose_logger
 from warcio import ArchiveIterator
 
 ALLOWED_ERR_FOR_RETRIES = [500, 502, 503, 504]
 
 
 class IDownloader:
+    """
+    Base class for all downloaders
+    """
+
     async def download(
         self, domain_record: DomainRecord
     ) -> (List[Tuple[str, PipeMetadata]]):
         raise NotImplementedError()
 
 
 class AsyncDownloader(IDownloader):
+    """
+    Downloader which asynchronously downloads the the data for the domain_record
+
+    Args:
+        base_url (str, optional): Base url where to download data from. Defaults to "https://data.commoncrawl.org/".
+        digest_verification (bool, optional): Whether to verify the digest of the downloaded data. Defaults to True.
+        max_retry (int, optional): Maximum number of retries. Defaults to 5.
+        sleep_step (int, optional): Sleep increase time between retries. Defaults to 10.
+        encoding: Default encoding to be used
+
+    """
+
     def __init__(
         self,
         base_url: str = "https://data.commoncrawl.org/",
         digest_verification: bool = True,
         max_retry: int = 5,
         sleep_step: int = 10,
         encoding: str = "latin-1",
@@ -83,16 +99,18 @@
                     else:
                         # will be unziped, we cannot use the stream since warcio doesn't support async
                         response_bytes = await response.content.read()
                         return self.unwrap(response_bytes, domain_record)
             except (
                 ClientError,
                 TimeoutError,
+                ServerConnectionError,
+                ContentTypeError,
             ) as e:
-                if not should_retry(retry, f"{str(e)} {type(e)}", 0):
+                if not should_retry(retry, f"{str(e)} {type(e)}", 500):
                     raise e
             await asyncio.sleep(random.randint(0, (retry + 1) * self.__sleep_step))
         ret: List[Tuple[str, PipeMetadata]] = []
         return ret
 
     def unwrap(
         self, response: bytes, domain_record: DomainRecord
@@ -134,14 +152,19 @@
 
 
 class DownloaderDummy(IDownloader):
     """
     Dummy downloader for testing
     It doesn't download anything but return files passed in the constructor
     and extracts metadata from the file
+
+    Args:
+        files (List[Path]): List of files to return
+        url (str, optional): Url to use for metadata. Defaults to None.
+        date (datetime, optional): Date to add to metadata. Defaults to None.
     """
 
     def __init__(
         self, files: List[Path], url: str | None = None, date: datetime | None = None
     ):
         self.files = files
         self.file_index = 0
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/extractor.py` & `CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,40 @@
 from bs4 import BeautifulSoup
 
 from cmoncrawl.common.types import PipeMetadata
 from cmoncrawl.common.loggers import metadata_logger
 
 
 class IExtractor(ABC):
+    """
+    Base class for all extractors
+    """
+
     @abstractmethod
     def extract(self, response: str, metadata: PipeMetadata) -> Dict[str, Any] | None:
+        """
+        Extracts the data from the response, if the extractor fails to extract the data it should return None
+        return None
+
+        Args:
+            response (str): response from the downloader
+            metadata (PipeMetadata): Metadata of the response
+        """
         raise NotImplementedError()
 
 
 class BaseExtractor(IExtractor, ABC):
+    """
+    Base class for all soup extractors
+
+    Args:
+        encoding (str, optional): Default encoding to be used. Defaults to None.
+
+    """
+
     def __init__(self, encoding: str | None = None):
         self.encoding = encoding
 
     def filter_raw(self, response: str, metadata: PipeMetadata) -> bool:
         # If raw fails bs4 will not be used -> speed
         return True
 
@@ -81,14 +101,17 @@
 
         return decoded
 
 
 class HTMLExtractor(BaseExtractor):
     """
     Dummy Extractor which simply extracts the html
+
+    Args:
+        filter_non_ok (bool, optional): If True, only 200 status codes will be extracted. Defaults to True.
     """
 
     def __init__(self, filter_non_ok: bool = True):
         super().__init__()
         self.filter_non_ok = filter_non_ok
 
     def extract_soup(self, soup: BeautifulSoup, metadata: PipeMetadata):
@@ -112,15 +135,18 @@
             )
             return False
         return True
 
 
 class DomainRecordExtractor(BaseExtractor):
     """
-    Dummy Extractor which simply extracts the html
+    Dummy Extractor which simply extracts the domain record
+
+    Args:
+        filter_non_ok (bool, optional): If True, only 200 status codes will be extracted. Defaults to True.
     """
 
     def __init__(self, filter_non_ok: bool = True):
         super().__init__()
         self.filter_non_ok = filter_non_ok
 
     def extract_soup(self, soup: BeautifulSoup, metadata: PipeMetadata):
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/pipeline.py` & `CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/router.py` & `CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/router.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,18 +25,25 @@
     name: str
     regexes: List[re.Pattern[str]]
     since: datetime
     to: datetime
 
 
 class IRouter(ABC):
+    """
+    Base class for all routers
+    """
+
     @abstractmethod
     def route(
         self, url: str | None, time: datetime | None, metadata: PipeMetadata
     ) -> IExtractor:
+        """
+        Routes the url to the correct extractor
+        """
         raise NotImplementedError()
 
 
 class Router(IRouter):
     def __init__(self):
         self.registered_routes: List[Route] = []
         self.modules: Dict[str, IExtractor] = {}
@@ -52,14 +59,17 @@
         if spec.loader is None:
             raise Exception("Failed to load module: " + module_name)
 
         spec.loader.exec_module(module)
         return module, module_name
 
     def load_module_as_extractor(self, module_path: Path):
+        """
+        Loads a module and returns its extractor
+        """
         module, module_name = self.load_module(module_path)
         name: str = getattr(module, "NAME", module_name)
         extractor: IExtractor | None = getattr(module, "extractor", None)
         if extractor is None:
             raise ValueError("Missing extractor variable in module: " + module_name)
         self.modules[name] = extractor
         all_purpose_logger.debug(f"Loaded module: {name}")
@@ -84,14 +94,24 @@
     def register_route(
         self,
         name: str,
         regex: Union[str, List[str]],
         since: datetime | None = None,
         to: datetime | None = None,
     ):
+        """
+        Registers a route for a given extractor name and regex
+
+        Args:
+            name (str): The name of the extractor
+            regex (Union[str, List[str]]): The regex to match against
+            since (datetime | None, optional): The earliest time to route to this extractor. Defaults to None.
+            to (datetime | None, optional): The latest time to route to this extractor. Defaults to None.
+
+        """
         if isinstance(regex, str):
             regex = [regex]
         regex_compiled = [re.compile(regex) for regex in regex]
 
         extractor = self.modules.get(name)
         if extractor is None:
             raise ValueError(f'No extractor named: "{name}" found')
@@ -117,14 +137,22 @@
         if time.tzinfo is None:
             return time.replace(tzinfo=timezone.utc)
         return time
 
     def route(
         self, url: str | None, time: datetime | None, metadata: PipeMetadata
     ) -> IExtractor:
+        """
+        Routes the url to the correct extractor based on the url and time
+
+        Args:
+            url (str | None): The url to route
+            time (datetime | None): The time to route
+            metadata (PipeMetadata): The metadata for the current pipeline
+        """
         # check if offset naive datetime if so then convert to utc
         if url is None:
             raise ValueError("Url must not be None")
         time = self._as_offset_aware(time) if time is not None else None
         for route in self.registered_routes:
             for regex in route.regexes:
                 if regex.match(url) and (
```

### Comparing `CmonCrawl-0.9.3/cmoncrawl/processor/pipeline/streamer.py` & `CmonCrawl-1.0.0/cmoncrawl/processor/pipeline/streamer.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/Makefile` & `CmonCrawl-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/doctrees/api.doctree` & `CmonCrawl-1.0.0/docs/build/doctrees/api.doctree`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9571 1300 0000 0000 008c 0f73 7068  ...q.........sph
+00000000: 8005 952b 1000 0000 0000 008c 0f73 7068  ...+.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -14,299 +14,247 @@
 000000d0: 7263 6594 4e8c 046c 696e 6594 4e75 6261  rce.N..line.Nuba
 000000e0: 8c0a 6174 7472 6962 7574 6573 947d 9428  ..attributes.}.(
 000000f0: 8c03 6964 7394 5d94 8c07 636c 6173 7365  ..ids.]...classe
 00000100: 7394 5d94 8c05 6e61 6d65 7394 5d94 8c08  s.]...names.]...
 00000110: 6475 706e 616d 6573 945d 948c 0862 6163  dupnames.]...bac
 00000120: 6b72 6566 7394 5d94 758c 0774 6167 6e61  krefs.].u..tagna
 00000130: 6d65 9468 0f68 1b68 0c68 1c68 0368 1d8c  me.h.h.h.h.h.h..
-00000140: 4a2f 686f 6d65 2f6b 7964 6c69 6365 682f  J/home/kydliceh/
-00000150: 536b 6f6c 612f 342e 7365 6d65 7374 722d  Skola/4.semestr-
-00000160: 4d46 4655 4b2f 526f 636e 696b 6f76 7920  MFFUK/Rocnikovy 
-00000170: 7072 6f6a 656b 742f 646f 6373 2f73 6f75  projekt/docs/sou
-00000180: 7263 652f 6170 692e 7273 7494 681e 4b02  rce/api.rst.h.K.
-00000190: 7562 6800 8c10 7461 6275 6c61 725f 636f  ubh...tabular_co
-000001a0: 6c5f 7370 6563 9493 9429 8194 7d94 2868  l_spec...)..}.(h
-000001b0: 0568 0668 075d 9468 1f7d 9428 6821 5d94  .h.h.].h.}.(h!].
-000001c0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000001d0: 8c04 7370 6563 948c 105c 587b 317d 7b32  ..spec...\X{1}{2
-000001e0: 7d5c 587b 317d 7b32 7d94 7568 2b68 2d68  }\X{1}{2}.uh+h-h
-000001f0: 1b68 0c68 1c68 0368 1d8c 5b2f 686f 6d65  .h.h.h.h..[/home
-00000200: 2f6b 7964 6c69 6365 682f 536b 6f6c 612f  /kydliceh/Skola/
-00000210: 342e 7365 6d65 7374 722d 4d46 4655 4b2f  4.semestr-MFFUK/
-00000220: 526f 636e 696b 6f76 7920 7072 6f6a 656b  Rocnikovy projek
-00000230: 742f 646f 6373 2f73 6f75 7263 652f 6170  t/docs/source/ap
-00000240: 692e 7273 743a 3135 3a3c 6175 746f 7375  i.rst:15:<autosu
-00000250: 6d6d 6172 793e 9468 1e4e 7562 8c16 7370  mmary>.h.Nub..sp
-00000260: 6869 6e78 2e65 7874 2e61 7574 6f73 756d  hinx.ext.autosum
-00000270: 6d61 7279 948c 1161 7574 6f73 756d 6d61  mary...autosumma
-00000280: 7279 5f74 6162 6c65 9493 9429 8194 7d94  ry_table...)..}.
-00000290: 2868 058c 1d0a 0a0a 0a41 6767 7265 6761  (h.......Aggrega
-000002a0: 746f 720a 0a0a 0a50 726f 6365 7373 6f72  tor....Processor
-000002b0: 0a0a 9468 075d 9468 098c 0574 6162 6c65  ...h.].h...table
-000002c0: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-000002d0: 9468 098c 0674 6772 6f75 7094 9394 2981  .h...tgroup...).
-000002e0: 947d 9428 6805 6806 6807 5d94 2868 098c  .}.(h.h.h.].(h..
-000002f0: 0763 6f6c 7370 6563 9493 9429 8194 7d94  .colspec...)..}.
-00000300: 2868 0568 0668 075d 9468 1f7d 9428 6821  (h.h.h.].h.}.(h!
-00000310: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000320: 5d94 8c08 636f 6c77 6964 7468 944b 0a75  ]...colwidth.K.u
-00000330: 682b 684c 681b 6849 7562 684d 2981 947d  h+hLh.hIubhM)..}
-00000340: 9428 6805 6806 6807 5d94 681f 7d94 2868  .(h.h.h.].h.}.(h
-00000350: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00000360: 295d 948c 0863 6f6c 7769 6474 6894 4b5a  )]...colwidth.KZ
-00000370: 7568 2b68 4c68 1b68 4975 6268 098c 0574  uh+hLh.hIubh...t
-00000380: 626f 6479 9493 9429 8194 7d94 2868 0568  body...)..}.(h.h
-00000390: 0668 075d 9428 6809 8c03 726f 7794 9394  .h.].(h...row...
-000003a0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-000003b0: 098c 0565 6e74 7279 9493 9429 8194 7d94  ...entry...)..}.
-000003c0: 2868 0568 0668 075d 9468 098c 0970 6172  (h.h.h.].h...par
-000003d0: 6167 7261 7068 9493 9429 8194 7d94 2868  agraph...)..}.(h
-000003e0: 058c 223a 7079 3a6f 626a 3a60 4167 6772  ..":py:obj:`Aggr
-000003f0: 6567 6174 6f72 203c 4167 6772 6567 6174  egator <Aggregat
-00000400: 6f72 3e60 5c94 6807 5d94 2868 008c 0c70  or>`\.h.].(h...p
-00000410: 656e 6469 6e67 5f78 7265 6694 9394 2981  ending_xref...).
-00000420: 947d 9428 6805 8c21 3a70 793a 6f62 6a3a  .}.(h..!:py:obj:
-00000430: 6041 6767 7265 6761 746f 7220 3c41 6767  `Aggregator <Agg
-00000440: 7265 6761 746f 723e 6094 6807 5d94 6809  regator>`.h.].h.
-00000450: 8c07 6c69 7465 7261 6c94 9394 2981 947d  ..literal...)..}
-00000460: 9428 6805 687b 6807 5d94 6816 8c0a 4167  .(h.h{h.].h...Ag
-00000470: 6772 6567 6174 6f72 9485 9481 947d 9428  gregator.....}.(
-00000480: 6805 6806 681b 687f 681c 6803 681d 4e68  h.h.h.h.h.h.h.Nh
-00000490: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-000004a0: 5d94 288c 0478 7265 6694 8c02 7079 948c  ].(..xref...py..
-000004b0: 0670 792d 6f62 6a94 6568 255d 9468 275d  .py-obj.eh%].h']
-000004c0: 9468 295d 9475 682b 687d 681b 6879 7562  .h)].uh+h}h.hyub
-000004d0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000004e0: 5d94 6827 5d94 6829 5d94 8c06 7265 6664  ].h'].h)]...refd
-000004f0: 6f63 948c 0361 7069 948c 0972 6566 646f  oc...api...refdo
-00000500: 6d61 696e 9468 8a8c 0772 6566 7479 7065  main.h...reftype
-00000510: 948c 036f 626a 948c 0b72 6566 6578 706c  ...obj...refexpl
-00000520: 6963 6974 9488 8c07 7265 6677 6172 6e94  icit....refwarn.
-00000530: 898c 0970 793a 6d6f 6475 6c65 944e 8c08  ...py:module.N..
-00000540: 7079 3a63 6c61 7373 944e 8c09 7265 6674  py:class.N..reft
-00000550: 6172 6765 7494 8c0a 4167 6772 6567 6174  arget...Aggregat
-00000560: 6f72 9475 682b 6877 681d 8c5b 2f68 6f6d  or.uh+hwh..[/hom
-00000570: 652f 6b79 646c 6963 6568 2f53 6b6f 6c61  e/kydliceh/Skola
-00000580: 2f34 2e73 656d 6573 7472 2d4d 4646 554b  /4.semestr-MFFUK
-00000590: 2f52 6f63 6e69 6b6f 7679 2070 726f 6a65  /Rocnikovy proje
-000005a0: 6b74 2f64 6f63 732f 736f 7572 6365 2f61  kt/docs/source/a
-000005b0: 7069 2e72 7374 3a31 353a 3c61 7574 6f73  pi.rst:15:<autos
-000005c0: 756d 6d61 7279 3e94 681e 4b01 681b 6873  ummary>.h.K.h.hs
-000005d0: 7562 6816 6806 8594 8194 7d94 2868 058c  ubh.h.....}.(h..
-000005e0: 015c 9468 1b68 7368 1c68 0368 1d4e 681e  .\.h.hsh.h.h.Nh.
-000005f0: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
-00000600: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00000610: 6871 681d 68a0 681e 4b01 681b 686e 7562  hqh.h.h.K.h.hnub
-00000620: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00000630: 5d94 6827 5d94 6829 5d94 7568 2b68 6c68  ].h'].h)].uh+hlh
-00000640: 1b68 6975 6268 6d29 8194 7d94 2868 0568  .hiubhm)..}.(h.h
-00000650: 0668 075d 9468 7229 8194 7d94 2868 0568  .h.].hr)..}.(h.h
-00000660: 0668 075d 9468 1f7d 9428 6821 5d94 6823  .h.].h.}.(h!].h#
-00000670: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00000680: 2b68 7168 1b68 b175 6261 681f 7d94 2868  +hqh.h.ubah.}.(h
-00000690: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000006a0: 295d 9475 682b 686c 681b 6869 7562 6568  )].uh+hlh.hiubeh
-000006b0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-000006c0: 6827 5d94 6829 5d94 7568 2b68 6768 1b68  h'].h)].uh+hgh.h
-000006d0: 6475 6268 6829 8194 7d94 2868 0568 0668  dubhh)..}.(h.h.h
-000006e0: 075d 9428 686d 2981 947d 9428 6805 6806  .].(hm)..}.(h.h.
-000006f0: 6807 5d94 6872 2981 947d 9428 6805 8c20  h.].hr)..}.(h.. 
-00000700: 3a70 793a 6f62 6a3a 6050 726f 6365 7373  :py:obj:`Process
-00000710: 6f72 203c 5072 6f63 6573 736f 723e 605c  or <Processor>`\
-00000720: 9468 075d 9428 6878 2981 947d 9428 6805  .h.].(hx)..}.(h.
-00000730: 8c1f 3a70 793a 6f62 6a3a 6050 726f 6365  ..:py:obj:`Proce
-00000740: 7373 6f72 203c 5072 6f63 6573 736f 723e  ssor <Processor>
-00000750: 6094 6807 5d94 687e 2981 947d 9428 6805  `.h.].h~)..}.(h.
-00000760: 68d5 6807 5d94 6816 8c09 5072 6f63 6573  h.h.].h...Proces
-00000770: 736f 7294 8594 8194 7d94 2868 0568 0668  sor.....}.(h.h.h
-00000780: 1b68 d768 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
-00000790: 681f 7d94 2868 215d 9468 235d 9428 6889  h.}.(h!].h#].(h.
-000007a0: 8c02 7079 948c 0670 792d 6f62 6a94 6568  ..py...py-obj.eh
-000007b0: 255d 9468 275d 9468 295d 9475 682b 687d  %].h'].h)].uh+h}
-000007c0: 681b 68d3 7562 6168 1f7d 9428 6821 5d94  h.h.ubah.}.(h!].
-000007d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000007e0: 8c06 7265 6664 6f63 9468 968c 0972 6566  ..refdoc.h...ref
-000007f0: 646f 6d61 696e 9468 e18c 0772 6566 7479  domain.h...refty
-00000800: 7065 948c 036f 626a 948c 0b72 6566 6578  pe...obj...refex
-00000810: 706c 6963 6974 9488 8c07 7265 6677 6172  plicit....refwar
-00000820: 6e94 8968 9c4e 689d 4e68 9e8c 0950 726f  n..h.Nh.Nh...Pro
-00000830: 6365 7373 6f72 9475 682b 6877 681d 8c5b  cessor.uh+hwh..[
-00000840: 2f68 6f6d 652f 6b79 646c 6963 6568 2f53  /home/kydliceh/S
-00000850: 6b6f 6c61 2f34 2e73 656d 6573 7472 2d4d  kola/4.semestr-M
-00000860: 4646 554b 2f52 6f63 6e69 6b6f 7679 2070  FFUK/Rocnikovy p
-00000870: 726f 6a65 6b74 2f64 6f63 732f 736f 7572  rojekt/docs/sour
-00000880: 6365 2f61 7069 2e72 7374 3a31 353a 3c61  ce/api.rst:15:<a
-00000890: 7574 6f73 756d 6d61 7279 3e94 681e 4b01  utosummary>.h.K.
-000008a0: 681b 68cf 7562 6816 6806 8594 8194 7d94  h.h.ubh.h.....}.
-000008b0: 2868 058c 015c 9468 1b68 cf68 1c68 0368  (h...\.h.h.h.h.h
-000008c0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
-000008d0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-000008e0: 9475 682b 6871 681d 68f3 681e 4b01 681b  .uh+hqh.h.h.K.h.
-000008f0: 68cc 7562 6168 1f7d 9428 6821 5d94 6823  h.ubah.}.(h!].h#
-00000900: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00000910: 2b68 6c68 1b68 c975 6268 6d29 8194 7d94  +hlh.h.ubhm)..}.
-00000920: 2868 0568 0668 075d 9468 7229 8194 7d94  (h.h.h.].hr)..}.
-00000930: 2868 0568 0668 075d 9468 1f7d 9428 6821  (h.h.h.].h.}.(h!
-00000940: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000950: 5d94 7568 2b68 7168 1b6a 0401 0000 7562  ].uh+hqh.j....ub
-00000960: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00000970: 5d94 6827 5d94 6829 5d94 7568 2b68 6c68  ].h'].h)].uh+hlh
-00000980: 1b68 c975 6265 681f 7d94 2868 215d 9468  .h.ubeh.}.(h!].h
-00000990: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000009a0: 682b 6867 681b 6864 7562 6568 1f7d 9428  h+hgh.hdubeh.}.(
-000009b0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000009c0: 6829 5d94 7568 2b68 6268 1b68 4975 6265  h)].uh+hbh.hIube
-000009d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000009e0: 9468 275d 9468 295d 948c 0463 6f6c 7394  .h'].h)]...cols.
-000009f0: 4b02 7568 2b68 4768 1b68 4475 6261 681f  K.uh+hGh.hDubah.
-00000a00: 7d94 2868 215d 9468 235d 948c 1561 7574  }.(h!].h#]...aut
-00000a10: 6f73 756d 6d61 7279 206c 6f6e 6774 6162  osummary longtab
-00000a20: 6c65 9461 6825 5d94 6827 5d94 6829 5d94  le.ah%].h'].h)].
-00000a30: 7568 2b68 4268 1b68 3e75 6261 681f 7d94  uh+hBh.h>ubah.}.
-00000a40: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00000a50: 9468 295d 948c 0978 6d6c 3a73 7061 6365  .h)]...xml:space
-00000a60: 948c 0870 7265 7365 7276 6594 7568 2b68  ...preserve.uh+h
-00000a70: 3c68 1b68 0c68 1c68 0368 1d68 3a68 1e4e  <h.h.h.h.h.h:h.N
-00000a80: 7562 683b 8c0f 6175 746f 7375 6d6d 6172  ubh;..autosummar
-00000a90: 795f 746f 6394 9394 2981 947d 9428 6805  y_toc...)..}.(h.
-00000aa0: 6806 6807 5d94 6800 8c07 746f 6374 7265  h.h.].h...toctre
-00000ab0: 6594 9394 2981 947d 9428 6805 6806 6807  e...)..}.(h.h.h.
-00000ac0: 5d94 681f 7d94 2868 215d 9468 235d 9468  ].h.}.(h!].h#].h
-00000ad0: 255d 9468 275d 9468 295d 948c 0c69 6e63  %].h'].h)]...inc
-00000ae0: 6c75 6465 6669 6c65 7394 5d94 288c 1467  ludefiles.].(..g
-00000af0: 656e 6572 6174 6564 2f41 6767 7265 6761  enerated/Aggrega
-00000b00: 746f 7294 8c13 6765 6e65 7261 7465 642f  tor...generated/
-00000b10: 5072 6f63 6573 736f 7294 658c 0765 6e74  Processor.e..ent
-00000b20: 7269 6573 945d 9428 4e6a 4a01 0000 8694  ries.].(NjJ.....
-00000b30: 4e6a 4b01 0000 8694 658c 086d 6178 6465  NjK.....e..maxde
-00000b40: 7074 6894 4aff ffff ff8c 0467 6c6f 6294  pth.J......glob.
-00000b50: 4e8c 0763 6170 7469 6f6e 944e 8c0a 7261  N..caption.N..ra
-00000b60: 7765 6e74 7269 6573 945d 9475 682b 6a3d  wentries.].uh+j=
-00000b70: 0100 0068 1b6a 3a01 0000 7562 6168 1f7d  ...h.j:...ubah.}
-00000b80: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00000b90: 5d94 6829 5d94 6a36 0100 006a 3701 0000  ].h)].j6...j7...
-00000ba0: 7568 2b6a 3801 0000 681b 680c 681c 6803  uh+j8...h.h.h.h.
-00000bb0: 681d 683a 681e 4e75 6265 681f 7d94 2868  h.h:h.Nubeh.}.(h
-00000bc0: 215d 948c 0361 7069 9461 6823 5d94 6825  !]...api.ah#].h%
-00000bd0: 5d94 8c03 6170 6994 6168 275d 9468 295d  ]...api.ah'].h)]
-00000be0: 9475 682b 680a 681b 6803 681c 6803 681d  .uh+h.h.h.h.h.h.
-00000bf0: 682c 681e 4b02 7562 6168 1f7d 9428 6821  h,h.K.ubah.}.(h!
-00000c00: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00000c10: 5d94 8c06 736f 7572 6365 9468 2c75 682b  ]...source.h,uh+
-00000c20: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
-00000c30: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
-00000c40: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
-00000c50: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
-00000c60: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
-00000c70: 947d 9428 680f 4e8c 0967 656e 6572 6174  .}.(h.N..generat
-00000c80: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
-00000c90: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
-00000ca0: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
-00000cb0: 746f 635f 6261 636b 6c69 6e6b 7394 686c  toc_backlinks.hl
-00000cc0: 8c12 666f 6f74 6e6f 7465 5f62 6163 6b6c  ..footnote_backl
-00000cd0: 696e 6b73 944b 018c 0d73 6563 746e 756d  inks.K...sectnum
-00000ce0: 5f78 666f 726d 944b 018c 0e73 7472 6970  _xform.K...strip
-00000cf0: 5f63 6f6d 6d65 6e74 7394 4e8c 1b73 7472  _comments.N..str
-00000d00: 6970 5f65 6c65 6d65 6e74 735f 7769 7468  ip_elements_with
-00000d10: 5f63 6c61 7373 6573 944e 8c0d 7374 7269  _classes.N..stri
-00000d20: 705f 636c 6173 7365 7394 4e8c 0c72 6570  p_classes.N..rep
-00000d30: 6f72 745f 6c65 7665 6c94 4b02 8c0a 6861  ort_level.K...ha
-00000d40: 6c74 5f6c 6576 656c 944b 058c 1165 7869  lt_level.K...exi
-00000d50: 745f 7374 6174 7573 5f6c 6576 656c 944b  t_status_level.K
-00000d60: 058c 0564 6562 7567 944e 8c0e 7761 726e  ...debug.N..warn
-00000d70: 696e 675f 7374 7265 616d 944e 8c09 7472  ing_stream.N..tr
-00000d80: 6163 6562 6163 6b94 888c 0e69 6e70 7574  aceback....input
-00000d90: 5f65 6e63 6f64 696e 6794 8c09 7574 662d  _encoding...utf-
-00000da0: 382d 7369 6794 8c1c 696e 7075 745f 656e  8-sig...input_en
-00000db0: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00000dc0: 646c 6572 948c 0673 7472 6963 7494 8c0f  dler...strict...
-00000dd0: 6f75 7470 7574 5f65 6e63 6f64 696e 6794  output_encoding.
-00000de0: 8c05 7574 662d 3894 8c1d 6f75 7470 7574  ..utf-8...output
-00000df0: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
-00000e00: 6861 6e64 6c65 7294 6a85 0100 008c 0e65  handler.j......e
-00000e10: 7272 6f72 5f65 6e63 6f64 696e 6794 8c05  rror_encoding...
-00000e20: 7574 662d 3894 8c1c 6572 726f 725f 656e  utf-8...error_en
-00000e30: 636f 6469 6e67 5f65 7272 6f72 5f68 616e  coding_error_han
-00000e40: 646c 6572 948c 1062 6163 6b73 6c61 7368  dler...backslash
-00000e50: 7265 706c 6163 6594 8c0d 6c61 6e67 7561  replace...langua
-00000e60: 6765 5f63 6f64 6594 8c02 656e 948c 1372  ge_code...en...r
-00000e70: 6563 6f72 645f 6465 7065 6e64 656e 6369  ecord_dependenci
-00000e80: 6573 944e 8c06 636f 6e66 6967 944e 8c09  es.N..config.N..
-00000e90: 6964 5f70 7265 6669 7894 6806 8c0e 6175  id_prefix.h...au
-00000ea0: 746f 5f69 645f 7072 6566 6978 948c 0269  to_id_prefix...i
-00000eb0: 6494 8c0d 6475 6d70 5f73 6574 7469 6e67  d...dump_setting
-00000ec0: 7394 4e8c 0e64 756d 705f 696e 7465 726e  s.N..dump_intern
-00000ed0: 616c 7394 4e8c 0f64 756d 705f 7472 616e  als.N..dump_tran
-00000ee0: 7366 6f72 6d73 944e 8c0f 6475 6d70 5f70  sforms.N..dump_p
-00000ef0: 7365 7564 6f5f 786d 6c94 4e8c 1065 7870  seudo_xml.N..exp
-00000f00: 6f73 655f 696e 7465 726e 616c 7394 4e8c  ose_internals.N.
-00000f10: 0e73 7472 6963 745f 7669 7369 746f 7294  .strict_visitor.
-00000f20: 4e8c 0f5f 6469 7361 626c 655f 636f 6e66  N.._disable_conf
-00000f30: 6967 944e 8c07 5f73 6f75 7263 6594 682c  ig.N.._source.h,
-00000f40: 8c0c 5f64 6573 7469 6e61 7469 6f6e 944e  .._destination.N
-00000f50: 8c0d 5f63 6f6e 6669 675f 6669 6c65 7394  .._config_files.
-00000f60: 5d94 8c16 6669 6c65 5f69 6e73 6572 7469  ]...file_inserti
-00000f70: 6f6e 5f65 6e61 626c 6564 9488 8c0b 7261  on_enabled....ra
-00000f80: 775f 656e 6162 6c65 6494 4b01 8c11 6c69  w_enabled.K...li
-00000f90: 6e65 5f6c 656e 6774 685f 6c69 6d69 7494  ne_length_limit.
-00000fa0: 4a00 e1f5 058c 0e70 6570 5f72 6566 6572  J......pep_refer
-00000fb0: 656e 6365 7394 4e8c 0c70 6570 5f62 6173  ences.N..pep_bas
-00000fc0: 655f 7572 6c94 8c18 6874 7470 733a 2f2f  e_url...https://
-00000fd0: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
-00000fe0: 948c 1570 6570 5f66 696c 655f 7572 6c5f  ...pep_file_url_
-00000ff0: 7465 6d70 6c61 7465 948c 0870 6570 2d25  template...pep-%
-00001000: 3034 6494 8c0e 7266 635f 7265 6665 7265  04d...rfc_refere
-00001010: 6e63 6573 944e 8c0c 7266 635f 6261 7365  nces.N..rfc_base
-00001020: 5f75 726c 948c 2668 7474 7073 3a2f 2f64  _url..&https://d
-00001030: 6174 6174 7261 636b 6572 2e69 6574 662e  atatracker.ietf.
-00001040: 6f72 672f 646f 632f 6874 6d6c 2f94 8c09  org/doc/html/...
-00001050: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
-00001060: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
-00001070: 7265 6e63 655f 7370 6163 6594 898c 1073  rence_space....s
-00001080: 796e 7461 785f 6869 6768 6c69 6768 7494  yntax_highlight.
-00001090: 8c04 6c6f 6e67 948c 0c73 6d61 7274 5f71  ..long...smart_q
-000010a0: 756f 7465 7394 888c 1373 6d61 7274 7175  uotes....smartqu
-000010b0: 6f74 6573 5f6c 6f63 616c 6573 945d 948c  otes_locales.]..
-000010c0: 1d63 6861 7261 6374 6572 5f6c 6576 656c  .character_level
-000010d0: 5f69 6e6c 696e 655f 6d61 726b 7570 9489  _inline_markup..
-000010e0: 8c0e 646f 6374 6974 6c65 5f78 666f 726d  ..doctitle_xform
-000010f0: 9489 8c0d 646f 6369 6e66 6f5f 7866 6f72  ....docinfo_xfor
-00001100: 6d94 4b01 8c12 7365 6374 7375 6274 6974  m.K...sectsubtit
-00001110: 6c65 5f78 666f 726d 9489 8c0d 696d 6167  le_xform....imag
-00001120: 655f 6c6f 6164 696e 6794 8c04 6c69 6e6b  e_loading...link
-00001130: 948c 1065 6d62 6564 5f73 7479 6c65 7368  ...embed_stylesh
-00001140: 6565 7494 898c 1563 6c6f 616b 5f65 6d61  eet....cloak_ema
-00001150: 696c 5f61 6464 7265 7373 6573 9488 8c11  il_addresses....
-00001160: 7365 6374 696f 6e5f 7365 6c66 5f6c 696e  section_self_lin
-00001170: 6b94 898c 0c65 6d62 6564 5f69 6d61 6765  k....embed_image
-00001180: 7394 898c 0365 6e76 944e 7562 8c08 7265  s....env.Nub..re
-00001190: 706f 7274 6572 944e 8c10 696e 6469 7265  porter.N..indire
-000011a0: 6374 5f74 6172 6765 7473 945d 948c 1173  ct_targets.]...s
-000011b0: 7562 7374 6974 7574 696f 6e5f 6465 6673  ubstitution_defs
-000011c0: 947d 948c 1273 7562 7374 6974 7574 696f  .}...substitutio
-000011d0: 6e5f 6e61 6d65 7394 7d94 8c08 7265 666e  n_names.}...refn
-000011e0: 616d 6573 947d 948c 0672 6566 6964 7394  ames.}...refids.
-000011f0: 7d94 8c07 6e61 6d65 6964 7394 7d94 6a60  }...nameids.}.j`
-00001200: 0100 006a 5d01 0000 738c 096e 616d 6574  ...j]...s..namet
-00001210: 7970 6573 947d 946a 6001 0000 4e73 6821  ypes.}.j`...Nsh!
-00001220: 7d94 6a5d 0100 0068 0c73 8c0d 666f 6f74  }.j]...h.s..foot
-00001230: 6e6f 7465 5f72 6566 7394 7d94 8c0d 6369  note_refs.}...ci
-00001240: 7461 7469 6f6e 5f72 6566 7394 7d94 8c0d  tation_refs.}...
-00001250: 6175 746f 666f 6f74 6e6f 7465 7394 5d94  autofootnotes.].
-00001260: 8c11 6175 746f 666f 6f74 6e6f 7465 5f72  ..autofootnote_r
-00001270: 6566 7394 5d94 8c10 7379 6d62 6f6c 5f66  efs.]...symbol_f
-00001280: 6f6f 746e 6f74 6573 945d 948c 1473 796d  ootnotes.]...sym
-00001290: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
-000012a0: 7394 5d94 8c09 666f 6f74 6e6f 7465 7394  s.]...footnotes.
-000012b0: 5d94 8c09 6369 7461 7469 6f6e 7394 5d94  ]...citations.].
-000012c0: 8c12 6175 746f 666f 6f74 6e6f 7465 5f73  ..autofootnote_s
-000012d0: 7461 7274 944b 018c 1573 796d 626f 6c5f  tart.K...symbol_
-000012e0: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
-000012f0: 008c 0a69 645f 636f 756e 7465 7294 8c0b  ...id_counter...
-00001300: 636f 6c6c 6563 7469 6f6e 7394 8c07 436f  collections...Co
-00001310: 756e 7465 7294 9394 7d94 8594 5294 8c0e  unter...}...R...
-00001320: 7061 7273 655f 6d65 7373 6167 6573 945d  parse_messages.]
-00001330: 948c 1274 7261 6e73 666f 726d 5f6d 6573  ...transform_mes
-00001340: 7361 6765 7394 5d94 8c0b 7472 616e 7366  sages.]...transf
-00001350: 6f72 6d65 7294 4e8c 0b69 6e63 6c75 6465  ormer.N..include
-00001360: 5f6c 6f67 945d 948c 0a64 6563 6f72 6174  _log.]...decorat
-00001370: 696f 6e94 4e68 1c68 0375 622e            ion.Nh.h.ub.
+00000140: 3d2f 686f 6d65 2f6b 7964 6c69 6365 682f  =/home/kydliceh/
+00000150: 5072 6f6a 6563 7473 2f52 6f63 6e69 6b6f  Projects/Rocniko
+00000160: 7679 2d50 726f 6a65 6b74 2f64 6f63 732f  vy-Projekt/docs/
+00000170: 736f 7572 6365 2f61 7069 2e72 7374 9468  source/api.rst.h
+00000180: 1e4b 0275 6268 008c 1074 6162 756c 6172  .K.ubh...tabular
+00000190: 5f63 6f6c 5f73 7065 6394 9394 2981 947d  _col_spec...)..}
+000001a0: 9428 6805 6806 6807 5d94 681f 7d94 2868  .(h.h.h.].h.}.(h
+000001b0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000001c0: 295d 948c 0473 7065 6394 8c10 5c58 7b31  )]...spec...\X{1
+000001d0: 7d7b 327d 5c58 7b31 7d7b 327d 9475 682b  }{2}\X{1}{2}.uh+
+000001e0: 682d 681b 680c 681c 6803 681d 8c4e 2f68  h-h.h.h.h.h..N/h
+000001f0: 6f6d 652f 6b79 646c 6963 6568 2f50 726f  ome/kydliceh/Pro
+00000200: 6a65 6374 732f 526f 636e 696b 6f76 792d  jects/Rocnikovy-
+00000210: 5072 6f6a 656b 742f 646f 6373 2f73 6f75  Projekt/docs/sou
+00000220: 7263 652f 6170 692e 7273 743a 3134 3a3c  rce/api.rst:14:<
+00000230: 6175 746f 7375 6d6d 6172 793e 9468 1e4e  autosummary>.h.N
+00000240: 7562 8c16 7370 6869 6e78 2e65 7874 2e61  ub..sphinx.ext.a
+00000250: 7574 6f73 756d 6d61 7279 948c 1161 7574  utosummary...aut
+00000260: 6f73 756d 6d61 7279 5f74 6162 6c65 9493  osummary_table..
+00000270: 9429 8194 7d94 2868 058c 0f0a 0a0a 0a63  .)..}.(h.......c
+00000280: 6d6f 6e63 7261 776c 0a0a 9468 075d 9468  moncrawl...h.].h
+00000290: 098c 0574 6162 6c65 9493 9429 8194 7d94  ...table...)..}.
+000002a0: 2868 0568 0668 075d 9468 098c 0674 6772  (h.h.h.].h...tgr
+000002b0: 6f75 7094 9394 2981 947d 9428 6805 6806  oup...)..}.(h.h.
+000002c0: 6807 5d94 2868 098c 0763 6f6c 7370 6563  h.].(h...colspec
+000002d0: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+000002e0: 9468 1f7d 9428 6821 5d94 6823 5d94 6825  .h.}.(h!].h#].h%
+000002f0: 5d94 6827 5d94 6829 5d94 8c08 636f 6c77  ].h'].h)]...colw
+00000300: 6964 7468 944b 0a75 682b 684c 681b 6849  idth.K.uh+hLh.hI
+00000310: 7562 684d 2981 947d 9428 6805 6806 6807  ubhM)..}.(h.h.h.
+00000320: 5d94 681f 7d94 2868 215d 9468 235d 9468  ].h.}.(h!].h#].h
+00000330: 255d 9468 275d 9468 295d 948c 0863 6f6c  %].h'].h)]...col
+00000340: 7769 6474 6894 4b5a 7568 2b68 4c68 1b68  width.KZuh+hLh.h
+00000350: 4975 6268 098c 0574 626f 6479 9493 9429  Iubh...tbody...)
+00000360: 8194 7d94 2868 0568 0668 075d 9468 098c  ..}.(h.h.h.].h..
+00000370: 0372 6f77 9493 9429 8194 7d94 2868 0568  .row...)..}.(h.h
+00000380: 0668 075d 9428 6809 8c05 656e 7472 7994  .h.].(h...entry.
+00000390: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+000003a0: 6809 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
+000003b0: 2981 947d 9428 6805 8c20 3a70 793a 6f62  )..}.(h.. :py:ob
+000003c0: 6a3a 6063 6d6f 6e63 7261 776c 203c 636d  j:`cmoncrawl <cm
+000003d0: 6f6e 6372 6177 6c3e 605c 9468 075d 9428  oncrawl>`\.h.].(
+000003e0: 6800 8c0c 7065 6e64 696e 675f 7872 6566  h...pending_xref
+000003f0: 9493 9429 8194 7d94 2868 058c 1f3a 7079  ...)..}.(h...:py
+00000400: 3a6f 626a 3a60 636d 6f6e 6372 6177 6c20  :obj:`cmoncrawl 
+00000410: 3c63 6d6f 6e63 7261 776c 3e60 9468 075d  <cmoncrawl>`.h.]
+00000420: 9468 098c 076c 6974 6572 616c 9493 9429  .h...literal...)
+00000430: 8194 7d94 2868 0568 7b68 075d 9468 168c  ..}.(h.h{h.].h..
+00000440: 0963 6d6f 6e63 7261 776c 9485 9481 947d  .cmoncrawl.....}
+00000450: 9428 6805 6806 681b 687f 681c 6803 681d  .(h.h.h.h.h.h.h.
+00000460: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00000470: 6823 5d94 288c 0478 7265 6694 8c02 7079  h#].(..xref...py
+00000480: 948c 0670 792d 6f62 6a94 6568 255d 9468  ...py-obj.eh%].h
+00000490: 275d 9468 295d 9475 682b 687d 681b 6879  '].h)].uh+h}h.hy
+000004a0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000004b0: 6825 5d94 6827 5d94 6829 5d94 8c06 7265  h%].h'].h)]...re
+000004c0: 6664 6f63 948c 0361 7069 948c 0972 6566  fdoc...api...ref
+000004d0: 646f 6d61 696e 9468 8a8c 0772 6566 7479  domain.h...refty
+000004e0: 7065 948c 036f 626a 948c 0b72 6566 6578  pe...obj...refex
+000004f0: 706c 6963 6974 9488 8c07 7265 6677 6172  plicit....refwar
+00000500: 6e94 898c 0970 793a 6d6f 6475 6c65 944e  n....py:module.N
+00000510: 8c08 7079 3a63 6c61 7373 944e 8c09 7265  ..py:class.N..re
+00000520: 6674 6172 6765 7494 8c09 636d 6f6e 6372  ftarget...cmoncr
+00000530: 6177 6c94 7568 2b68 7768 1d8c 4e2f 686f  awl.uh+hwh..N/ho
+00000540: 6d65 2f6b 7964 6c69 6365 682f 5072 6f6a  me/kydliceh/Proj
+00000550: 6563 7473 2f52 6f63 6e69 6b6f 7679 2d50  ects/Rocnikovy-P
+00000560: 726f 6a65 6b74 2f64 6f63 732f 736f 7572  rojekt/docs/sour
+00000570: 6365 2f61 7069 2e72 7374 3a31 343a 3c61  ce/api.rst:14:<a
+00000580: 7574 6f73 756d 6d61 7279 3e94 681e 4b01  utosummary>.h.K.
+00000590: 681b 6873 7562 6816 6806 8594 8194 7d94  h.hsubh.h.....}.
+000005a0: 2868 058c 015c 9468 1b68 7368 1c68 0368  (h...\.h.hsh.h.h
+000005b0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+000005c0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000005d0: 9475 682b 6871 681d 68a0 681e 4b01 681b  .uh+hqh.h.h.K.h.
+000005e0: 686e 7562 6168 1f7d 9428 6821 5d94 6823  hnubah.}.(h!].h#
+000005f0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00000600: 2b68 6c68 1b68 6975 6268 6d29 8194 7d94  +hlh.hiubhm)..}.
+00000610: 2868 0568 0668 075d 9468 7229 8194 7d94  (h.h.h.].hr)..}.
+00000620: 2868 0568 0668 075d 9468 1f7d 9428 6821  (h.h.h.].h.}.(h!
+00000630: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000640: 5d94 7568 2b68 7168 1b68 b175 6261 681f  ].uh+hqh.h.ubah.
+00000650: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00000660: 275d 9468 295d 9475 682b 686c 681b 6869  '].h)].uh+hlh.hi
+00000670: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00000680: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00000690: 6768 1b68 6475 6261 681f 7d94 2868 215d  gh.hdubah.}.(h!]
+000006a0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000006b0: 9475 682b 6862 681b 6849 7562 6568 1f7d  .uh+hbh.hIubeh.}
+000006c0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000006d0: 5d94 6829 5d94 8c04 636f 6c73 944b 0275  ].h)]...cols.K.u
+000006e0: 682b 6847 681b 6844 7562 6168 1f7d 9428  h+hGh.hDubah.}.(
+000006f0: 6821 5d94 6823 5d94 8c15 6175 746f 7375  h!].h#]...autosu
+00000700: 6d6d 6172 7920 6c6f 6e67 7461 626c 6594  mmary longtable.
+00000710: 6168 255d 9468 275d 9468 295d 9475 682b  ah%].h'].h)].uh+
+00000720: 6842 681b 683e 7562 6168 1f7d 9428 6821  hBh.h>ubah.}.(h!
+00000730: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000740: 5d94 8c09 786d 6c3a 7370 6163 6594 8c08  ]...xml:space...
+00000750: 7072 6573 6572 7665 9475 682b 683c 681b  preserve.uh+h<h.
+00000760: 680c 681c 6803 681d 683a 681e 4e75 6268  h.h.h.h.h:h.Nubh
+00000770: 3b8c 0f61 7574 6f73 756d 6d61 7279 5f74  ;..autosummary_t
+00000780: 6f63 9493 9429 8194 7d94 2868 0568 0668  oc...)..}.(h.h.h
+00000790: 075d 9468 008c 0774 6f63 7472 6565 9493  .].h...toctree..
+000007a0: 9429 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
+000007b0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000007c0: 6827 5d94 6829 5d94 8c0c 696e 636c 7564  h'].h)]...includ
+000007d0: 6566 696c 6573 945d 948c 1367 656e 6572  efiles.]...gener
+000007e0: 6174 6564 2f63 6d6f 6e63 7261 776c 9461  ated/cmoncrawl.a
+000007f0: 8c07 656e 7472 6965 7394 5d94 4e68 f786  ..entries.].Nh..
+00000800: 9461 8c08 6d61 7864 6570 7468 944a ffff  .a..maxdepth.J..
+00000810: ffff 8c04 676c 6f62 944e 8c07 6361 7074  ....glob.N..capt
+00000820: 696f 6e94 4e8c 0a72 6177 656e 7472 6965  ion.N..rawentrie
+00000830: 7394 5d94 7568 2b68 ea68 1b68 e775 6261  s.].uh+h.h.h.uba
+00000840: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000850: 9468 275d 9468 295d 9468 e368 e475 682b  .h'].h)].h.h.uh+
+00000860: 68e5 681b 680c 681c 6803 681d 683a 681e  h.h.h.h.h.h.h:h.
+00000870: 4e75 6265 681f 7d94 2868 215d 948c 0361  Nubeh.}.(h!]...a
+00000880: 7069 9461 6823 5d94 6825 5d94 8c03 6170  pi.ah#].h%]...ap
+00000890: 6994 6168 275d 9468 295d 9475 682b 680a  i.ah'].h)].uh+h.
+000008a0: 681b 6803 681c 6803 681d 682c 681e 4b02  h.h.h.h.h.h,h.K.
+000008b0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000008c0: 6825 5d94 6827 5d94 6829 5d94 8c06 736f  h%].h'].h)]...so
+000008d0: 7572 6365 9468 2c75 682b 6801 8c0e 6375  urce.h,uh+h...cu
+000008e0: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
+000008f0: 6375 7272 656e 745f 6c69 6e65 944e 8c08  current_line.N..
+00000900: 7365 7474 696e 6773 948c 1164 6f63 7574  settings...docut
+00000910: 696c 732e 6672 6f6e 7465 6e64 948c 0656  ils.frontend...V
+00000920: 616c 7565 7394 9394 2981 947d 9428 680f  alues...)..}.(h.
+00000930: 4e8c 0967 656e 6572 6174 6f72 944e 8c09  N..generator.N..
+00000940: 6461 7465 7374 616d 7094 4e8c 0b73 6f75  datestamp.N..sou
+00000950: 7263 655f 6c69 6e6b 944e 8c0a 736f 7572  rce_link.N..sour
+00000960: 6365 5f75 726c 944e 8c0d 746f 635f 6261  ce_url.N..toc_ba
+00000970: 636b 6c69 6e6b 7394 686c 8c12 666f 6f74  cklinks.hl..foot
+00000980: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
+00000990: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
+000009a0: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
+000009b0: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
+000009c0: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
+000009d0: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
+000009e0: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
+000009f0: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
+00000a00: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
+00000a10: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
+00000a20: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
+00000a30: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
+00000a40: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
+00000a50: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
+00000a60: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
+00000a70: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00000a80: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
+00000a90: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
+00000aa0: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
+00000ab0: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+00000ac0: 7294 6a30 0100 008c 0e65 7272 6f72 5f65  r.j0.....error_e
+00000ad0: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
+00000ae0: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+00000af0: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00000b00: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
+00000b10: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
+00000b20: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
+00000b30: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
+00000b40: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
+00000b50: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
+00000b60: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
+00000b70: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
+00000b80: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
+00000b90: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
+00000ba0: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
+00000bb0: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
+00000bc0: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
+00000bd0: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
+00000be0: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
+00000bf0: 5f73 6f75 7263 6594 682c 8c0c 5f64 6573  _source.h,.._des
+00000c00: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
+00000c10: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
+00000c20: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
+00000c30: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
+00000c40: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
+00000c50: 6774 685f 6c69 6d69 7494 4a00 e1f5 058c  gth_limit.J.....
+00000c60: 0e70 6570 5f72 6566 6572 656e 6365 7394  .pep_references.
+00000c70: 4e8c 0c70 6570 5f62 6173 655f 7572 6c94  N..pep_base_url.
+00000c80: 8c18 6874 7470 733a 2f2f 7065 7073 2e70  ..https://peps.p
+00000c90: 7974 686f 6e2e 6f72 672f 948c 1570 6570  ython.org/...pep
+00000ca0: 5f66 696c 655f 7572 6c5f 7465 6d70 6c61  _file_url_templa
+00000cb0: 7465 948c 0870 6570 2d25 3034 6494 8c0e  te...pep-%04d...
+00000cc0: 7266 635f 7265 6665 7265 6e63 6573 944e  rfc_references.N
+00000cd0: 8c0c 7266 635f 6261 7365 5f75 726c 948c  ..rfc_base_url..
+00000ce0: 2668 7474 7073 3a2f 2f64 6174 6174 7261  &https://datatra
+00000cf0: 636b 6572 2e69 6574 662e 6f72 672f 646f  cker.ietf.org/do
+00000d00: 632f 6874 6d6c 2f94 8c09 7461 625f 7769  c/html/...tab_wi
+00000d10: 6474 6894 4b08 8c1d 7472 696d 5f66 6f6f  dth.K...trim_foo
+00000d20: 746e 6f74 655f 7265 6665 7265 6e63 655f  tnote_reference_
+00000d30: 7370 6163 6594 898c 1073 796e 7461 785f  space....syntax_
+00000d40: 6869 6768 6c69 6768 7494 8c04 6c6f 6e67  highlight...long
+00000d50: 948c 0c73 6d61 7274 5f71 756f 7465 7394  ...smart_quotes.
+00000d60: 888c 1373 6d61 7274 7175 6f74 6573 5f6c  ...smartquotes_l
+00000d70: 6f63 616c 6573 945d 948c 1d63 6861 7261  ocales.]...chara
+00000d80: 6374 6572 5f6c 6576 656c 5f69 6e6c 696e  cter_level_inlin
+00000d90: 655f 6d61 726b 7570 9489 8c0e 646f 6374  e_markup....doct
+00000da0: 6974 6c65 5f78 666f 726d 9489 8c0d 646f  itle_xform....do
+00000db0: 6369 6e66 6f5f 7866 6f72 6d94 4b01 8c12  cinfo_xform.K...
+00000dc0: 7365 6374 7375 6274 6974 6c65 5f78 666f  sectsubtitle_xfo
+00000dd0: 726d 9489 8c0d 696d 6167 655f 6c6f 6164  rm....image_load
+00000de0: 696e 6794 8c04 6c69 6e6b 948c 1065 6d62  ing...link...emb
+00000df0: 6564 5f73 7479 6c65 7368 6565 7494 898c  ed_stylesheet...
+00000e00: 1563 6c6f 616b 5f65 6d61 696c 5f61 6464  .cloak_email_add
+00000e10: 7265 7373 6573 9488 8c11 7365 6374 696f  resses....sectio
+00000e20: 6e5f 7365 6c66 5f6c 696e 6b94 898c 0c65  n_self_link....e
+00000e30: 6d62 6564 5f69 6d61 6765 7394 898c 0365  mbed_images....e
+00000e40: 6e76 944e 7562 8c08 7265 706f 7274 6572  nv.Nub..reporter
+00000e50: 944e 8c10 696e 6469 7265 6374 5f74 6172  .N..indirect_tar
+00000e60: 6765 7473 945d 948c 1173 7562 7374 6974  gets.]...substit
+00000e70: 7574 696f 6e5f 6465 6673 947d 948c 1273  ution_defs.}...s
+00000e80: 7562 7374 6974 7574 696f 6e5f 6e61 6d65  ubstitution_name
+00000e90: 7394 7d94 8c08 7265 666e 616d 6573 947d  s.}...refnames.}
+00000ea0: 948c 0672 6566 6964 7394 7d94 8c07 6e61  ...refids.}...na
+00000eb0: 6d65 6964 7394 7d94 6a0b 0100 006a 0801  meids.}.j....j..
+00000ec0: 0000 738c 096e 616d 6574 7970 6573 947d  ..s..nametypes.}
+00000ed0: 946a 0b01 0000 4e73 6821 7d94 6a08 0100  .j....Nsh!}.j...
+00000ee0: 0068 0c73 8c0d 666f 6f74 6e6f 7465 5f72  .h.s..footnote_r
+00000ef0: 6566 7394 7d94 8c0d 6369 7461 7469 6f6e  efs.}...citation
+00000f00: 5f72 6566 7394 7d94 8c0d 6175 746f 666f  _refs.}...autofo
+00000f10: 6f74 6e6f 7465 7394 5d94 8c11 6175 746f  otnotes.]...auto
+00000f20: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
+00000f30: 8c10 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
+00000f40: 6573 945d 948c 1473 796d 626f 6c5f 666f  es.]...symbol_fo
+00000f50: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c09  otnote_refs.]...
+00000f60: 666f 6f74 6e6f 7465 7394 5d94 8c09 6369  footnotes.]...ci
+00000f70: 7461 7469 6f6e 7394 5d94 8c12 6175 746f  tations.]...auto
+00000f80: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
+00000f90: 018c 1573 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
+00000fa0: 7465 5f73 7461 7274 944b 008c 0a69 645f  te_start.K...id_
+00000fb0: 636f 756e 7465 7294 8c0b 636f 6c6c 6563  counter...collec
+00000fc0: 7469 6f6e 7394 8c07 436f 756e 7465 7294  tions...Counter.
+00000fd0: 9394 7d94 8594 5294 8c0e 7061 7273 655f  ..}...R...parse_
+00000fe0: 6d65 7373 6167 6573 945d 948c 1274 7261  messages.]...tra
+00000ff0: 6e73 666f 726d 5f6d 6573 7361 6765 7394  nsform_messages.
+00001000: 5d94 8c0b 7472 616e 7366 6f72 6d65 7294  ]...transformer.
+00001010: 4e8c 0b69 6e63 6c75 6465 5f6c 6f67 945d  N..include_log.]
+00001020: 948c 0a64 6563 6f72 6174 696f 6e94 4e68  ...decoration.Nh
+00001030: 1c68 0375 622e                           .h.ub.
```

### Comparing `CmonCrawl-0.9.3/docs/build/doctrees/generated/Aggregator.App.ndjson_decoder.doctree` & `CmonCrawl-1.0.0/docs/build/doctrees/index.doctree`

 * *Files 26% similar despite different names*

```diff
@@ -1,333 +1,325 @@
-00000000: 8005 95b6 1400 0000 0000 008c 0f73 7068  .............sph
+00000000: 8005 9543 1400 0000 0000 008c 0f73 7068  ...C.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
-00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
-00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
-00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
-00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
-00000080: 6594 9394 2981 947d 9428 6805 8c1e 4167  e...)..}.(h...Ag
-00000090: 6772 6567 6174 6f72 2e41 7070 2e6e 646a  gregator.App.ndj
-000000a0: 736f 6e5c 5f64 6563 6f64 6572 9468 075d  son\_decoder.h.]
-000000b0: 9468 098c 0454 6578 7494 9394 8c1e 4167  .h...Text.....Ag
-000000c0: 6772 6567 6174 6f72 2e41 7070 2e6e 646a  gregator.App.ndj
-000000d0: 736f 6e00 5f64 6563 6f64 6572 9485 9481  son._decoder....
-000000e0: 947d 9428 6805 8c1e 4167 6772 6567 6174  .}.(h...Aggregat
-000000f0: 6f72 2e41 7070 2e6e 646a 736f 6e5c 5f64  or.App.ndjson\_d
-00000100: 6563 6f64 6572 948c 0670 6172 656e 7494  ecoder...parent.
-00000110: 6811 8c09 5f64 6f63 756d 656e 7494 6803  h..._document.h.
-00000120: 8c06 736f 7572 6365 944e 8c04 6c69 6e65  ..source.N..line
-00000130: 944e 7562 618c 0a61 7474 7269 6275 7465  .Nuba..attribute
-00000140: 7394 7d94 288c 0369 6473 945d 948c 0763  s.}.(..ids.]...c
-00000150: 6c61 7373 6573 945d 948c 056e 616d 6573  lasses.]...names
-00000160: 945d 948c 0864 7570 6e61 6d65 7394 5d94  .]...dupnames.].
-00000170: 8c08 6261 636b 7265 6673 945d 9475 8c07  ..backrefs.].u..
-00000180: 7461 676e 616d 6594 680f 681c 680c 681d  tagname.h.h.h.h.
-00000190: 6803 681e 8c6e 2f68 6f6d 652f 6b79 646c  h.h..n/home/kydl
-000001a0: 6963 6568 2f53 6b6f 6c61 2f34 2e73 656d  iceh/Skola/4.sem
-000001b0: 6573 7472 2d4d 4646 554b 2f52 6f63 6e69  estr-MFFUK/Rocni
-000001c0: 6b6f 7679 2070 726f 6a65 6b74 2f64 6f63  kovy projekt/doc
-000001d0: 732f 736f 7572 6365 2f67 656e 6572 6174  s/source/generat
-000001e0: 6564 2f41 6767 7265 6761 746f 722e 4170  ed/Aggregator.Ap
-000001f0: 702e 6e64 6a73 6f6e 5f64 6563 6f64 6572  p.ndjson_decoder
-00000200: 2e72 7374 9468 1f4b 0275 6268 008c 0569  .rst.h.K.ubh...i
-00000210: 6e64 6578 9493 9429 8194 7d94 2868 0568  ndex...)..}.(h.h
-00000220: 0668 075d 9468 207d 9428 6822 5d94 6824  .h.].h }.(h"].h$
-00000230: 5d94 6826 5d94 6828 5d94 682a 5d94 8c07  ].h&].h(].h*]...
-00000240: 656e 7472 6965 7394 5d94 288c 0470 6169  entries.].(..pai
-00000250: 7294 8c25 6d6f 6475 6c65 3b20 4167 6772  r..%module; Aggr
-00000260: 6567 6174 6f72 2e41 7070 2e6e 646a 736f  egator.App.ndjso
-00000270: 6e5f 6465 636f 6465 7294 8c24 6d6f 6475  n_decoder..$modu
-00000280: 6c65 2d41 6767 7265 6761 746f 722e 4170  le-Aggregator.Ap
-00000290: 702e 6e64 6a73 6f6e 5f64 6563 6f64 6572  p.ndjson_decoder
-000002a0: 9468 064e 7494 6175 682c 682e 681c 680c  .h.Nt.auh,h.h.h.
-000002b0: 681d 6803 681e 4e68 1f4e 7562 6809 8c06  h.h.h.Nh.Nubh...
-000002c0: 7275 6272 6963 9493 9429 8194 7d94 2868  rubric...)..}.(h
-000002d0: 058c 0743 6c61 7373 6573 9468 075d 9468  ...Classes.h.].h
-000002e0: 168c 0743 6c61 7373 6573 9485 9481 947d  ...Classes.....}
-000002f0: 9428 6805 6843 681c 6841 681d 6803 681e  .(h.hCh.hAh.h.h.
-00000300: 4e68 1f4e 7562 6168 207d 9428 6822 5d94  Nh.Nubah }.(h"].
-00000310: 6824 5d94 6826 5d94 6828 5d94 682a 5d94  h$].h&].h(].h*].
-00000320: 7568 2c68 3f68 1c68 0c68 1d68 0368 1e68  uh,h?h.h.h.h.h.h
-00000330: 2d68 1f4b 1175 6268 008c 1074 6162 756c  -h.K.ubh...tabul
-00000340: 6172 5f63 6f6c 5f73 7065 6394 9394 2981  ar_col_spec...).
-00000350: 947d 9428 6805 6806 6807 5d94 6820 7d94  .}.(h.h.h.].h }.
-00000360: 2868 225d 9468 245d 9468 265d 9468 285d  (h"].h$].h&].h(]
-00000370: 9468 2a5d 948c 0473 7065 6394 8c10 5c58  .h*]...spec...\X
-00000380: 7b31 7d7b 327d 5c58 7b31 7d7b 327d 9475  {1}{2}\X{1}{2}.u
-00000390: 682c 684f 681c 680c 681d 6803 681e 8c7f  h,hOh.h.h.h.h...
-000003a0: 2f68 6f6d 652f 6b79 646c 6963 6568 2f53  /home/kydliceh/S
-000003b0: 6b6f 6c61 2f34 2e73 656d 6573 7472 2d4d  kola/4.semestr-M
-000003c0: 4646 554b 2f52 6f63 6e69 6b6f 7679 2070  FFUK/Rocnikovy p
-000003d0: 726f 6a65 6b74 2f64 6f63 732f 736f 7572  rojekt/docs/sour
-000003e0: 6365 2f67 656e 6572 6174 6564 2f41 6767  ce/generated/Agg
-000003f0: 7265 6761 746f 722e 4170 702e 6e64 6a73  regator.App.ndjs
-00000400: 6f6e 5f64 6563 6f64 6572 2e72 7374 3a32  on_decoder.rst:2
-00000410: 313a 3c61 7574 6f73 756d 6d61 7279 3e94  1:<autosummary>.
-00000420: 681f 4e75 628c 1673 7068 696e 782e 6578  h.Nub..sphinx.ex
-00000430: 742e 6175 746f 7375 6d6d 6172 7994 8c11  t.autosummary...
-00000440: 6175 746f 7375 6d6d 6172 795f 7461 626c  autosummary_tabl
-00000450: 6594 9394 2981 947d 9428 6805 8c31 0a0a  e...)..}.(h..1..
-00000460: 0a0a 4465 636f 6465 7228 2a5b 2c20 6f62  ..Decoder(*[, ob
-00000470: 6a65 6374 5f68 6f6f 6b2c 2070 6172 7365  ject_hook, parse
-00000480: 5f66 6c6f 6174 2c20 2e2e 2e5d 290a 0a94  _float, ...])...
-00000490: 6807 5d94 6809 8c05 7461 626c 6594 9394  h.].h...table...
-000004a0: 2981 947d 9428 6805 6806 6807 5d94 6809  )..}.(h.h.h.].h.
-000004b0: 8c06 7467 726f 7570 9493 9429 8194 7d94  ..tgroup...)..}.
-000004c0: 2868 0568 0668 075d 9428 6809 8c07 636f  (h.h.h.].(h...co
-000004d0: 6c73 7065 6394 9394 2981 947d 9428 6805  lspec...)..}.(h.
-000004e0: 6806 6807 5d94 6820 7d94 2868 225d 9468  h.h.].h }.(h"].h
-000004f0: 245d 9468 265d 9468 285d 9468 2a5d 948c  $].h&].h(].h*]..
-00000500: 0863 6f6c 7769 6474 6894 4b0a 7568 2c68  .colwidth.K.uh,h
-00000510: 6e68 1c68 6b75 6268 6f29 8194 7d94 2868  nh.hkubho)..}.(h
-00000520: 0568 0668 075d 9468 207d 9428 6822 5d94  .h.h.].h }.(h"].
-00000530: 6824 5d94 6826 5d94 6828 5d94 682a 5d94  h$].h&].h(].h*].
-00000540: 8c08 636f 6c77 6964 7468 944b 5a75 682c  ..colwidth.KZuh,
-00000550: 686e 681c 686b 7562 6809 8c05 7462 6f64  hnh.hkubh...tbod
-00000560: 7994 9394 2981 947d 9428 6805 6806 6807  y...)..}.(h.h.h.
-00000570: 5d94 6809 8c03 726f 7794 9394 2981 947d  ].h...row...)..}
-00000580: 9428 6805 6806 6807 5d94 2868 098c 0565  .(h.h.h.].(h...e
-00000590: 6e74 7279 9493 9429 8194 7d94 2868 0568  ntry...)..}.(h.h
-000005a0: 0668 075d 9468 098c 0970 6172 6167 7261  .h.].h...paragra
-000005b0: 7068 9493 9429 8194 7d94 2868 058c 693a  ph...)..}.(h..i:
-000005c0: 7079 3a6f 626a 3a60 4465 636f 6465 7220  py:obj:`Decoder 
-000005d0: 3c41 6767 7265 6761 746f 722e 4170 702e  <Aggregator.App.
-000005e0: 6e64 6a73 6f6e 5f64 6563 6f64 6572 2e44  ndjson_decoder.D
-000005f0: 6563 6f64 6572 3e60 5c20 5c28 5c2a 5c5b  ecoder>`\ \(\*\[
-00000600: 5c2c 206f 626a 6563 745c 5f68 6f6f 6b5c  \, object\_hook\
-00000610: 2c20 7061 7273 655c 5f66 6c6f 6174 5c2c  , parse\_float\,
-00000620: 202e 2e2e 5c5d 5c29 9468 075d 9428 6800   ...\]\).h.].(h.
-00000630: 8c0c 7065 6e64 696e 675f 7872 6566 9493  ..pending_xref..
-00000640: 9429 8194 7d94 2868 058c 393a 7079 3a6f  .)..}.(h..9:py:o
-00000650: 626a 3a60 4465 636f 6465 7220 3c41 6767  bj:`Decoder <Agg
-00000660: 7265 6761 746f 722e 4170 702e 6e64 6a73  regator.App.ndjs
-00000670: 6f6e 5f64 6563 6f64 6572 2e44 6563 6f64  on_decoder.Decod
-00000680: 6572 3e60 9468 075d 9468 098c 076c 6974  er>`.h.].h...lit
-00000690: 6572 616c 9493 9429 8194 7d94 2868 0568  eral...)..}.(h.h
-000006a0: 9d68 075d 9468 168c 0744 6563 6f64 6572  .h.].h...Decoder
-000006b0: 9485 9481 947d 9428 6805 6806 681c 68a1  .....}.(h.h.h.h.
-000006c0: 681d 6803 681e 4e68 1f4e 7562 6168 207d  h.h.h.Nh.Nubah }
-000006d0: 9428 6822 5d94 6824 5d94 288c 0478 7265  .(h"].h$].(..xre
-000006e0: 6694 8c02 7079 948c 0670 792d 6f62 6a94  f...py...py-obj.
-000006f0: 6568 265d 9468 285d 9468 2a5d 9475 682c  eh&].h(].h*].uh,
-00000700: 689f 681c 689b 7562 6168 207d 9428 6822  h.h.h.ubah }.(h"
-00000710: 5d94 6824 5d94 6826 5d94 6828 5d94 682a  ].h$].h&].h(].h*
-00000720: 5d94 8c06 7265 6664 6f63 948c 2767 656e  ]...refdoc..'gen
-00000730: 6572 6174 6564 2f41 6767 7265 6761 746f  erated/Aggregato
-00000740: 722e 4170 702e 6e64 6a73 6f6e 5f64 6563  r.App.ndjson_dec
-00000750: 6f64 6572 948c 0972 6566 646f 6d61 696e  oder...refdomain
-00000760: 9468 ac8c 0772 6566 7479 7065 948c 036f  .h...reftype...o
-00000770: 626a 948c 0b72 6566 6578 706c 6963 6974  bj...refexplicit
-00000780: 9488 8c07 7265 6677 6172 6e94 898c 0970  ....refwarn....p
-00000790: 793a 6d6f 6475 6c65 948c 1d41 6767 7265  y:module...Aggre
-000007a0: 6761 746f 722e 4170 702e 6e64 6a73 6f6e  gator.App.ndjson
-000007b0: 5f64 6563 6f64 6572 948c 0870 793a 636c  _decoder...py:cl
-000007c0: 6173 7394 4e8c 0972 6566 7461 7267 6574  ass.N..reftarget
-000007d0: 948c 2541 6767 7265 6761 746f 722e 4170  ..%Aggregator.Ap
-000007e0: 702e 6e64 6a73 6f6e 5f64 6563 6f64 6572  p.ndjson_decoder
-000007f0: 2e44 6563 6f64 6572 9475 682c 6899 681e  .Decoder.uh,h.h.
-00000800: 8c7f 2f68 6f6d 652f 6b79 646c 6963 6568  ../home/kydliceh
-00000810: 2f53 6b6f 6c61 2f34 2e73 656d 6573 7472  /Skola/4.semestr
-00000820: 2d4d 4646 554b 2f52 6f63 6e69 6b6f 7679  -MFFUK/Rocnikovy
-00000830: 2070 726f 6a65 6b74 2f64 6f63 732f 736f   projekt/docs/so
-00000840: 7572 6365 2f67 656e 6572 6174 6564 2f41  urce/generated/A
-00000850: 6767 7265 6761 746f 722e 4170 702e 6e64  ggregator.App.nd
-00000860: 6a73 6f6e 5f64 6563 6f64 6572 2e72 7374  json_decoder.rst
-00000870: 3a32 313a 3c61 7574 6f73 756d 6d61 7279  :21:<autosummary
-00000880: 3e94 681f 4b01 681c 6895 7562 6816 8c24  >.h.K.h.h.ubh..$
-00000890: 282a 5b2c 206f 626a 6563 745f 686f 6f6b  (*[, object_hook
-000008a0: 2c20 7061 7273 655f 666c 6f61 742c 202e  , parse_float, .
-000008b0: 2e2e 5d29 9485 9481 947d 9428 6805 8c30  ..]).....}.(h..0
-000008c0: 5c20 5c28 5c2a 5c5b 5c2c 206f 626a 6563  \ \(\*\[\, objec
-000008d0: 745c 5f68 6f6f 6b5c 2c20 7061 7273 655c  t\_hook\, parse\
-000008e0: 5f66 6c6f 6174 5c2c 202e 2e2e 5c5d 5c29  _float\, ...\]\)
-000008f0: 9468 1c68 9568 1d68 0368 1e4e 681f 4e75  .h.h.h.h.h.Nh.Nu
-00000900: 6265 6820 7d94 2868 225d 9468 245d 9468  beh }.(h"].h$].h
-00000910: 265d 9468 285d 9468 2a5d 9475 682c 6893  &].h(].h*].uh,h.
-00000920: 681e 68c3 681f 4b01 681c 6890 7562 6168  h.h.h.K.h.h.ubah
-00000930: 207d 9428 6822 5d94 6824 5d94 6826 5d94   }.(h"].h$].h&].
-00000940: 6828 5d94 682a 5d94 7568 2c68 8e68 1c68  h(].h*].uh,h.h.h
-00000950: 8b75 6268 8f29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-00000960: 075d 9468 9429 8194 7d94 2868 0568 0668  .].h.)..}.(h.h.h
-00000970: 075d 9468 207d 9428 6822 5d94 6824 5d94  .].h }.(h"].h$].
-00000980: 6826 5d94 6828 5d94 682a 5d94 7568 2c68  h&].h(].h*].uh,h
-00000990: 9368 1c68 d575 6261 6820 7d94 2868 225d  .h.h.ubah }.(h"]
-000009a0: 9468 245d 9468 265d 9468 285d 9468 2a5d  .h$].h&].h(].h*]
-000009b0: 9475 682c 688e 681c 688b 7562 6568 207d  .uh,h.h.h.ubeh }
-000009c0: 9428 6822 5d94 6824 5d94 6826 5d94 6828  .(h"].h$].h&].h(
-000009d0: 5d94 682a 5d94 7568 2c68 8968 1c68 8675  ].h*].uh,h.h.h.u
-000009e0: 6261 6820 7d94 2868 225d 9468 245d 9468  bah }.(h"].h$].h
-000009f0: 265d 9468 285d 9468 2a5d 9475 682c 6884  &].h(].h*].uh,h.
-00000a00: 681c 686b 7562 6568 207d 9428 6822 5d94  h.hkubeh }.(h"].
-00000a10: 6824 5d94 6826 5d94 6828 5d94 682a 5d94  h$].h&].h(].h*].
-00000a20: 8c04 636f 6c73 944b 0275 682c 6869 681c  ..cols.K.uh,hih.
-00000a30: 6866 7562 6168 207d 9428 6822 5d94 6824  hfubah }.(h"].h$
-00000a40: 5d94 8c15 6175 746f 7375 6d6d 6172 7920  ]...autosummary 
-00000a50: 6c6f 6e67 7461 626c 6594 6168 265d 9468  longtable.ah&].h
-00000a60: 285d 9468 2a5d 9475 682c 6864 681c 6860  (].h*].uh,hdh.h`
-00000a70: 7562 6168 207d 9428 6822 5d94 6824 5d94  ubah }.(h"].h$].
-00000a80: 6826 5d94 6828 5d94 682a 5d94 8c09 786d  h&].h(].h*]...xm
-00000a90: 6c3a 7370 6163 6594 8c08 7072 6573 6572  l:space...preser
-00000aa0: 7665 9475 682c 685e 681c 680c 681d 6803  ve.uh,h^h.h.h.h.
-00000ab0: 681e 685c 681f 4e75 6268 5d8c 0f61 7574  h.h\h.Nubh]..aut
-00000ac0: 6f73 756d 6d61 7279 5f74 6f63 9493 9429  osummary_toc...)
-00000ad0: 8194 7d94 2868 0568 0668 075d 9468 008c  ..}.(h.h.h.].h..
-00000ae0: 0774 6f63 7472 6565 9493 9429 8194 7d94  .toctree...)..}.
-00000af0: 2868 0568 0668 075d 9468 207d 9428 6822  (h.h.h.].h }.(h"
-00000b00: 5d94 6824 5d94 6826 5d94 6828 5d94 682a  ].h$].h&].h(].h*
-00000b10: 5d94 8c0c 696e 636c 7564 6566 696c 6573  ]...includefiles
-00000b20: 945d 948c 2f67 656e 6572 6174 6564 2f41  .]../generated/A
-00000b30: 6767 7265 6761 746f 722e 4170 702e 6e64  ggregator.App.nd
-00000b40: 6a73 6f6e 5f64 6563 6f64 6572 2e44 6563  json_decoder.Dec
-00000b50: 6f64 6572 9461 8c07 656e 7472 6965 7394  oder.a..entries.
-00000b60: 5d94 4e6a 1b01 0000 8694 618c 086d 6178  ].Nj......a..max
-00000b70: 6465 7074 6894 4aff ffff ff8c 0467 6c6f  depth.J......glo
-00000b80: 6294 4e8c 0763 6170 7469 6f6e 944e 8c0a  b.N..caption.N..
-00000b90: 7261 7765 6e74 7269 6573 945d 9475 682c  rawentries.].uh,
-00000ba0: 6a0e 0100 0068 1c6a 0b01 0000 7562 6168  j....h.j....ubah
-00000bb0: 207d 9428 6822 5d94 6824 5d94 6826 5d94   }.(h"].h$].h&].
-00000bc0: 6828 5d94 682a 5d94 6a07 0100 006a 0801  h(].h*].j....j..
-00000bd0: 0000 7568 2c6a 0901 0000 681c 680c 681d  ..uh,j....h.h.h.
-00000be0: 6803 681e 685c 681f 4e75 6265 6820 7d94  h.h.h\h.Nubeh }.
-00000bf0: 2868 225d 9428 683d 8c1d 6167 6772 6567  (h"].(h=..aggreg
-00000c00: 6174 6f72 2d61 7070 2d6e 646a 736f 6e2d  ator-app-ndjson-
-00000c10: 6465 636f 6465 7294 6568 245d 9468 265d  decoder.eh$].h&]
-00000c20: 948c 1d61 6767 7265 6761 746f 722e 6170  ...aggregator.ap
-00000c30: 702e 6e64 6a73 6f6e 5f64 6563 6f64 6572  p.ndjson_decoder
-00000c40: 9461 6828 5d94 682a 5d94 7568 2c68 0a68  .ah(].h*].uh,h.h
-00000c50: 1c68 0368 1d68 0368 1e68 2d68 1f4b 0275  .h.h.h.h.h-h.K.u
-00000c60: 6261 6820 7d94 2868 225d 9468 245d 9468  bah }.(h"].h$].h
-00000c70: 265d 9468 285d 9468 2a5d 948c 0673 6f75  &].h(].h*]...sou
-00000c80: 7263 6594 682d 7568 2c68 018c 0e63 7572  rce.h-uh,h...cur
-00000c90: 7265 6e74 5f73 6f75 7263 6594 4e8c 0c63  rent_source.N..c
-00000ca0: 7572 7265 6e74 5f6c 696e 6594 4e8c 0873  urrent_line.N..s
-00000cb0: 6574 7469 6e67 7394 8c11 646f 6375 7469  ettings...docuti
-00000cc0: 6c73 2e66 726f 6e74 656e 6494 8c06 5661  ls.frontend...Va
-00000cd0: 6c75 6573 9493 9429 8194 7d94 2868 0f4e  lues...)..}.(h.N
-00000ce0: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
-00000cf0: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
-00000d00: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
-00000d10: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
-00000d20: 6b6c 696e 6b73 9468 8e8c 1266 6f6f 746e  klinks.h...footn
-00000d30: 6f74 655f 6261 636b 6c69 6e6b 7394 4b01  ote_backlinks.K.
-00000d40: 8c0d 7365 6374 6e75 6d5f 7866 6f72 6d94  ..sectnum_xform.
-00000d50: 4b01 8c0e 7374 7269 705f 636f 6d6d 656e  K...strip_commen
-00000d60: 7473 944e 8c1b 7374 7269 705f 656c 656d  ts.N..strip_elem
-00000d70: 656e 7473 5f77 6974 685f 636c 6173 7365  ents_with_classe
-00000d80: 7394 4e8c 0d73 7472 6970 5f63 6c61 7373  s.N..strip_class
-00000d90: 6573 944e 8c0c 7265 706f 7274 5f6c 6576  es.N..report_lev
-00000da0: 656c 944b 028c 0a68 616c 745f 6c65 7665  el.K...halt_leve
-00000db0: 6c94 4b05 8c11 6578 6974 5f73 7461 7475  l.K...exit_statu
-00000dc0: 735f 6c65 7665 6c94 4b05 8c05 6465 6275  s_level.K...debu
-00000dd0: 6794 4e8c 0e77 6172 6e69 6e67 5f73 7472  g.N..warning_str
-00000de0: 6561 6d94 4e8c 0974 7261 6365 6261 636b  eam.N..traceback
-00000df0: 9488 8c0e 696e 7075 745f 656e 636f 6469  ....input_encodi
-00000e00: 6e67 948c 0975 7466 2d38 2d73 6967 948c  ng...utf-8-sig..
-00000e10: 1c69 6e70 7574 5f65 6e63 6f64 696e 675f  .input_encoding_
-00000e20: 6572 726f 725f 6861 6e64 6c65 7294 8c06  error_handler...
-00000e30: 7374 7269 6374 948c 0f6f 7574 7075 745f  strict...output_
-00000e40: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
-00000e50: 948c 1d6f 7574 7075 745f 656e 636f 6469  ...output_encodi
-00000e60: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
-00000e70: 946a 5401 0000 8c0e 6572 726f 725f 656e  .jT.....error_en
-00000e80: 636f 6469 6e67 948c 0575 7466 2d38 948c  coding...utf-8..
-00000e90: 1c65 7272 6f72 5f65 6e63 6f64 696e 675f  .error_encoding_
-00000ea0: 6572 726f 725f 6861 6e64 6c65 7294 8c10  error_handler...
-00000eb0: 6261 636b 736c 6173 6872 6570 6c61 6365  backslashreplace
-00000ec0: 948c 0d6c 616e 6775 6167 655f 636f 6465  ...language_code
-00000ed0: 948c 0265 6e94 8c13 7265 636f 7264 5f64  ...en...record_d
-00000ee0: 6570 656e 6465 6e63 6965 7394 4e8c 0663  ependencies.N..c
-00000ef0: 6f6e 6669 6794 4e8c 0969 645f 7072 6566  onfig.N..id_pref
-00000f00: 6978 9468 068c 0e61 7574 6f5f 6964 5f70  ix.h...auto_id_p
-00000f10: 7265 6669 7894 8c02 6964 948c 0d64 756d  refix...id...dum
-00000f20: 705f 7365 7474 696e 6773 944e 8c0e 6475  p_settings.N..du
-00000f30: 6d70 5f69 6e74 6572 6e61 6c73 944e 8c0f  mp_internals.N..
-00000f40: 6475 6d70 5f74 7261 6e73 666f 726d 7394  dump_transforms.
-00000f50: 4e8c 0f64 756d 705f 7073 6575 646f 5f78  N..dump_pseudo_x
-00000f60: 6d6c 944e 8c10 6578 706f 7365 5f69 6e74  ml.N..expose_int
-00000f70: 6572 6e61 6c73 944e 8c0e 7374 7269 6374  ernals.N..strict
-00000f80: 5f76 6973 6974 6f72 944e 8c0f 5f64 6973  _visitor.N.._dis
-00000f90: 6162 6c65 5f63 6f6e 6669 6794 4e8c 075f  able_config.N.._
-00000fa0: 736f 7572 6365 9468 2d8c 0c5f 6465 7374  source.h-.._dest
-00000fb0: 696e 6174 696f 6e94 4e8c 0d5f 636f 6e66  ination.N.._conf
-00000fc0: 6967 5f66 696c 6573 945d 948c 1666 696c  ig_files.]...fil
-00000fd0: 655f 696e 7365 7274 696f 6e5f 656e 6162  e_insertion_enab
-00000fe0: 6c65 6494 888c 0b72 6177 5f65 6e61 626c  led....raw_enabl
-00000ff0: 6564 944b 018c 116c 696e 655f 6c65 6e67  ed.K...line_leng
-00001000: 7468 5f6c 696d 6974 944a 00e1 f505 8c0e  th_limit.J......
-00001010: 7065 705f 7265 6665 7265 6e63 6573 944e  pep_references.N
-00001020: 8c0c 7065 705f 6261 7365 5f75 726c 948c  ..pep_base_url..
-00001030: 1868 7474 7073 3a2f 2f70 6570 732e 7079  .https://peps.py
-00001040: 7468 6f6e 2e6f 7267 2f94 8c15 7065 705f  thon.org/...pep_
-00001050: 6669 6c65 5f75 726c 5f74 656d 706c 6174  file_url_templat
-00001060: 6594 8c08 7065 702d 2530 3464 948c 0e72  e...pep-%04d...r
-00001070: 6663 5f72 6566 6572 656e 6365 7394 4e8c  fc_references.N.
-00001080: 0c72 6663 5f62 6173 655f 7572 6c94 8c26  .rfc_base_url..&
-00001090: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
-000010a0: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
-000010b0: 2f68 746d 6c2f 948c 0974 6162 5f77 6964  /html/...tab_wid
-000010c0: 7468 944b 088c 1d74 7269 6d5f 666f 6f74  th.K...trim_foot
-000010d0: 6e6f 7465 5f72 6566 6572 656e 6365 5f73  note_reference_s
-000010e0: 7061 6365 9489 8c10 7379 6e74 6178 5f68  pace....syntax_h
-000010f0: 6967 686c 6967 6874 948c 046c 6f6e 6794  ighlight...long.
-00001100: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
-00001110: 8c13 736d 6172 7471 756f 7465 735f 6c6f  ..smartquotes_lo
-00001120: 6361 6c65 7394 5d94 8c1d 6368 6172 6163  cales.]...charac
-00001130: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
-00001140: 5f6d 6172 6b75 7094 898c 0e64 6f63 7469  _markup....docti
-00001150: 746c 655f 7866 6f72 6d94 898c 0d64 6f63  tle_xform....doc
-00001160: 696e 666f 5f78 666f 726d 944b 018c 1273  info_xform.K...s
-00001170: 6563 7473 7562 7469 746c 655f 7866 6f72  ectsubtitle_xfor
-00001180: 6d94 898c 0d69 6d61 6765 5f6c 6f61 6469  m....image_loadi
-00001190: 6e67 948c 046c 696e 6b94 8c10 656d 6265  ng...link...embe
-000011a0: 645f 7374 796c 6573 6865 6574 9489 8c15  d_stylesheet....
-000011b0: 636c 6f61 6b5f 656d 6169 6c5f 6164 6472  cloak_email_addr
-000011c0: 6573 7365 7394 888c 1173 6563 7469 6f6e  esses....section
-000011d0: 5f73 656c 665f 6c69 6e6b 9489 8c0c 656d  _self_link....em
-000011e0: 6265 645f 696d 6167 6573 9489 8c03 656e  bed_images....en
-000011f0: 7694 4e75 628c 0872 6570 6f72 7465 7294  v.Nub..reporter.
-00001200: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
-00001210: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
-00001220: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
-00001230: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
-00001240: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
-00001250: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
-00001260: 6569 6473 947d 946a 2f01 0000 6a2c 0100  eids.}.j/...j,..
-00001270: 0073 8c09 6e61 6d65 7479 7065 7394 7d94  .s..nametypes.}.
-00001280: 6a2f 0100 004e 7368 227d 9428 6a2c 0100  j/...Nsh"}.(j,..
-00001290: 0068 0c68 3d68 098c 0674 6172 6765 7494  .h.h=h...target.
-000012a0: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-000012b0: 6820 7d94 2868 225d 9468 3d61 6824 5d94  h }.(h"].h=ah$].
-000012c0: 6826 5d94 6828 5d94 682a 5d94 8c05 6973  h&].h(].h*]...is
-000012d0: 6d6f 6494 8875 682c 6a9b 0100 0068 1e8c  mod..uh,j....h..
-000012e0: 7e2f 686f 6d65 2f6b 7964 6c69 6365 682f  ~/home/kydliceh/
-000012f0: 2e6c 6f63 616c 2f6c 6962 2f70 7974 686f  .local/lib/pytho
-00001300: 6e33 2e31 302f 7369 7465 2d70 6163 6b61  n3.10/site-packa
-00001310: 6765 732f 4167 6772 6567 6174 6f72 2f41  ges/Aggregator/A
-00001320: 7070 2f6e 646a 736f 6e5f 6465 636f 6465  pp/ndjson_decode
-00001330: 722e 7079 3a64 6f63 7374 7269 6e67 206f  r.py:docstring o
-00001340: 6620 4167 6772 6567 6174 6f72 2e41 7070  f Aggregator.App
-00001350: 2e6e 646a 736f 6e5f 6465 636f 6465 7294  .ndjson_decoder.
-00001360: 681f 4b01 681c 680c 681d 6803 7562 758c  h.K.h.h.h.h.ubu.
-00001370: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
-00001380: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
-00001390: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
-000013a0: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
-000013b0: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
-000013c0: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
-000013d0: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-000013e0: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
-000013f0: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
-00001400: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
-00001410: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
-00001420: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
-00001430: 6172 7494 4b00 8c0a 6964 5f63 6f75 6e74  art.K...id_count
-00001440: 6572 948c 0b63 6f6c 6c65 6374 696f 6e73  er...collections
-00001450: 948c 0743 6f75 6e74 6572 9493 947d 9485  ...Counter...}..
-00001460: 9452 948c 0e70 6172 7365 5f6d 6573 7361  .R...parse_messa
-00001470: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
-00001480: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
-00001490: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
-000014a0: 636c 7564 655f 6c6f 6794 5d94 8c0a 6465  clude_log.]...de
-000014b0: 636f 7261 7469 6f6e 944e 681d 6803 7562  coration.Nh.h.ub
-000014c0: 2e                                       .
+00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
+00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
+00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
+00000070: 6805 8cda 436f 6d6d 6f6e 4372 6177 6c20  h...CommonCrawl 
+00000080: 4578 7472 6163 746f 7220 646f 6375 6d65  Extractor docume
+00000090: 6e74 6174 696f 6e20 6d61 7374 6572 2066  ntation master f
+000000a0: 696c 652c 2063 7265 6174 6564 2062 790a  ile, created by.
+000000b0: 7370 6869 6e78 2d71 7569 636b 7374 6172  sphinx-quickstar
+000000c0: 7420 6f6e 2054 7565 204e 6f76 2020 3820  t on Tue Nov  8 
+000000d0: 3137 3a34 303a 3335 2032 3032 322e 0a59  17:40:35 2022..Y
+000000e0: 6f75 2063 616e 2061 6461 7074 2074 6869  ou can adapt thi
+000000f0: 7320 6669 6c65 2063 6f6d 706c 6574 656c  s file completel
+00000100: 7920 746f 2079 6f75 7220 6c69 6b69 6e67  y to your liking
+00000110: 2c20 6275 7420 6974 2073 686f 756c 6420  , but it should 
+00000120: 6174 206c 6561 7374 0a63 6f6e 7461 696e  at least.contain
+00000130: 2074 6865 2072 6f6f 7420 6074 6f63 7472   the root `toctr
+00000140: 6565 6020 6469 7265 6374 6976 652e 9468  ee` directive..h
+00000150: 075d 9468 098c 0454 6578 7494 9394 8cda  .].h...Text.....
+00000160: 436f 6d6d 6f6e 4372 6177 6c20 4578 7472  CommonCrawl Extr
+00000170: 6163 746f 7220 646f 6375 6d65 6e74 6174  actor documentat
+00000180: 696f 6e20 6d61 7374 6572 2066 696c 652c  ion master file,
+00000190: 2063 7265 6174 6564 2062 790a 7370 6869   created by.sphi
+000001a0: 6e78 2d71 7569 636b 7374 6172 7420 6f6e  nx-quickstart on
+000001b0: 2054 7565 204e 6f76 2020 3820 3137 3a34   Tue Nov  8 17:4
+000001c0: 303a 3335 2032 3032 322e 0a59 6f75 2063  0:35 2022..You c
+000001d0: 616e 2061 6461 7074 2074 6869 7320 6669  an adapt this fi
+000001e0: 6c65 2063 6f6d 706c 6574 656c 7920 746f  le completely to
+000001f0: 2079 6f75 7220 6c69 6b69 6e67 2c20 6275   your liking, bu
+00000200: 7420 6974 2073 686f 756c 6420 6174 206c  t it should at l
+00000210: 6561 7374 0a63 6f6e 7461 696e 2074 6865  east.contain the
+00000220: 2072 6f6f 7420 6074 6f63 7472 6565 6020   root `toctree` 
+00000230: 6469 7265 6374 6976 652e 9485 9481 947d  directive......}
+00000240: 9428 6805 6806 8c06 7061 7265 6e74 9468  .(h.h...parent.h
+00000250: 0c75 6261 8c0a 6174 7472 6962 7574 6573  .uba..attributes
+00000260: 947d 9428 8c03 6964 7394 5d94 8c07 636c  .}.(..ids.]...cl
+00000270: 6173 7365 7394 5d94 8c05 6e61 6d65 7394  asses.]...names.
+00000280: 5d94 8c08 6475 706e 616d 6573 945d 948c  ]...dupnames.]..
+00000290: 0862 6163 6b72 6566 7394 5d94 8c09 786d  .backrefs.]...xm
+000002a0: 6c3a 7370 6163 6594 8c08 7072 6573 6572  l:space...preser
+000002b0: 7665 9475 8c07 7461 676e 616d 6594 680a  ve.u..tagname.h.
+000002c0: 6816 6803 8c09 5f64 6f63 756d 656e 7494  h.h..._document.
+000002d0: 6803 8c06 736f 7572 6365 948c 3f2f 686f  h...source..?/ho
+000002e0: 6d65 2f6b 7964 6c69 6365 682f 5072 6f6a  me/kydliceh/Proj
+000002f0: 6563 7473 2f52 6f63 6e69 6b6f 7679 2d50  ects/Rocnikovy-P
+00000300: 726f 6a65 6b74 2f64 6f63 732f 736f 7572  rojekt/docs/sour
+00000310: 6365 2f69 6e64 6578 2e72 7374 948c 046c  ce/index.rst...l
+00000320: 696e 6594 4b05 7562 6809 8c07 7365 6374  ine.K.ubh...sect
+00000330: 696f 6e94 9394 2981 947d 9428 6805 6806  ion...)..}.(h.h.
+00000340: 6807 5d94 2868 098c 0574 6974 6c65 9493  h.].(h...title..
+00000350: 9429 8194 7d94 2868 058c 3157 656c 636f  .)..}.(h..1Welco
+00000360: 6d65 2074 6f20 436f 6d6d 6f6e 4372 6177  me to CommonCraw
+00000370: 6c20 4578 7472 6163 746f 7227 7320 646f  l Extractor's do
+00000380: 6375 6d65 6e74 6174 696f 6e21 9468 075d  cumentation!.h.]
+00000390: 9468 118c 3357 656c 636f 6d65 2074 6f20  .h..3Welcome to 
+000003a0: 436f 6d6d 6f6e 4372 6177 6c20 4578 7472  CommonCrawl Extr
+000003b0: 6163 746f 72e2 8099 7320 646f 6375 6d65  actor...s docume
+000003c0: 6e74 6174 696f 6e21 9485 9481 947d 9428  ntation!.....}.(
+000003d0: 6805 6833 6816 6831 6826 6803 6827 4e68  h.h3h.h1h&h.h'Nh
+000003e0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+000003f0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00000400: 2568 2f68 1668 2c68 2668 0368 2768 2868  %h/h.h,h&h.h'h(h
+00000410: 294b 0775 6268 098c 0863 6f6d 706f 756e  )K.ubh...compoun
+00000420: 6494 9394 2981 947d 9428 6805 6806 6807  d...)..}.(h.h.h.
+00000430: 5d94 6800 8c07 746f 6374 7265 6594 9394  ].h...toctree...
+00000440: 2981 947d 9428 6805 6806 6807 5d94 6817  )..}.(h.h.h.].h.
+00000450: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000460: 1f5d 9468 215d 9468 168c 0569 6e64 6578  .].h!].h...index
+00000470: 948c 0765 6e74 7269 6573 945d 9428 4e8c  ...entries.].(N.
+00000480: 0575 7361 6765 9486 944e 8c09 636c 692f  .usage...N..cli/
+00000490: 696e 6465 7894 8694 4e8c 1065 7874 7261  index...N..extra
+000004a0: 6374 696f 6e2f 696e 6465 7894 8694 4e8c  ction/index...N.
+000004b0: 1070 726f 675f 6775 6964 652f 696e 6465  .prog_guide/inde
+000004c0: 7894 8694 4e8c 0a6d 6973 632f 696e 6465  x...N..misc/inde
+000004d0: 7894 8694 4e8c 0361 7069 9486 9465 8c0c  x...N..api...e..
+000004e0: 696e 636c 7564 6566 696c 6573 945d 9428  includefiles.].(
+000004f0: 6852 6854 6856 6858 685a 685c 658c 086d  hRhThVhXhZh\e..m
+00000500: 6178 6465 7074 6894 4b03 8c07 6361 7074  axdepth.K...capt
+00000510: 696f 6e94 8c09 436f 6e74 656e 7473 3a94  ion...Contents:.
+00000520: 8c04 676c 6f62 9489 8c06 6869 6464 656e  ..glob....hidden
+00000530: 9489 8c0d 696e 636c 7564 6568 6964 6465  ....includehidde
+00000540: 6e94 898c 086e 756d 6265 7265 6494 4b00  n....numbered.K.
+00000550: 8c0a 7469 746c 6573 6f6e 6c79 9489 8c0a  ..titlesonly....
+00000560: 7261 7765 6e74 7269 6573 945d 948c 0a72  rawentries.]...r
+00000570: 6177 6361 7074 696f 6e94 6862 7568 2568  awcaption.hbuh%h
+00000580: 4468 2768 2868 294b 0968 1668 4175 6261  Dh'h(h)K.h.hAuba
+00000590: 6817 7d94 2868 195d 9468 1b5d 948c 0f74  h.}.(h.].h.]...t
+000005a0: 6f63 7472 6565 2d77 7261 7070 6572 9461  octree-wrapper.a
+000005b0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+000005c0: 3f68 1668 2c68 2668 0368 2768 2868 294e  ?h.h,h&h.h'h(h)N
+000005d0: 7562 6568 177d 9428 6819 5d94 8c30 7765  ubeh.}.(h.]..0we
+000005e0: 6c63 6f6d 652d 746f 2d63 6f6d 6d6f 6e63  lcome-to-commonc
+000005f0: 7261 776c 2d65 7874 7261 6374 6f72 2d73  rawl-extractor-s
+00000600: 2d64 6f63 756d 656e 7461 7469 6f6e 9461  -documentation.a
+00000610: 681b 5d94 681d 5d94 8c31 7765 6c63 6f6d  h.].h.]..1welcom
+00000620: 6520 746f 2063 6f6d 6d6f 6e63 7261 776c  e to commoncrawl
+00000630: 2065 7874 7261 6374 6f72 2773 2064 6f63   extractor's doc
+00000640: 756d 656e 7461 7469 6f6e 2194 6168 1f5d  umentation!.ah.]
+00000650: 9468 215d 9475 6825 682a 6816 6803 6826  .h!].uh%h*h.h.h&
+00000660: 6803 6827 6828 6829 4b07 7562 682b 2981  h.h'h(h)K.ubh+).
+00000670: 947d 9428 6805 6806 6807 5d94 2868 3029  .}.(h.h.h.].(h0)
+00000680: 8194 7d94 2868 058c 1249 6e64 6963 6573  ..}.(h...Indices
+00000690: 2061 6e64 2074 6162 6c65 7394 6807 5d94   and tables.h.].
+000006a0: 6811 8c12 496e 6469 6365 7320 616e 6420  h...Indices and 
+000006b0: 7461 626c 6573 9485 9481 947d 9428 6805  tables.....}.(h.
+000006c0: 687f 6816 687d 6826 6803 6827 4e68 294e  h.h.h}h&h.h'Nh)N
+000006d0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+000006e0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+000006f0: 2f68 1668 7a68 2668 0368 2768 2868 294b  /h.hzh&h.h'h(h)K
+00000700: 1775 6268 098c 0b62 756c 6c65 745f 6c69  .ubh...bullet_li
+00000710: 7374 9493 9429 8194 7d94 2868 0568 0668  st...)..}.(h.h.h
+00000720: 075d 9428 6809 8c09 6c69 7374 5f69 7465  .].(h...list_ite
+00000730: 6d94 9394 2981 947d 9428 6805 8c0f 3a72  m...)..}.(h...:r
+00000740: 6566 3a60 6765 6e69 6e64 6578 6094 6807  ef:`genindex`.h.
+00000750: 5d94 6809 8c09 7061 7261 6772 6170 6894  ].h...paragraph.
+00000760: 9394 2981 947d 9428 6805 6894 6807 5d94  ..)..}.(h.h.h.].
+00000770: 6800 8c0c 7065 6e64 696e 675f 7872 6566  h...pending_xref
+00000780: 9493 9429 8194 7d94 2868 0568 9468 075d  ...)..}.(h.h.h.]
+00000790: 9468 098c 0669 6e6c 696e 6594 9394 2981  .h...inline...).
+000007a0: 947d 9428 6805 6894 6807 5d94 6811 8c08  .}.(h.h.h.].h...
+000007b0: 6765 6e69 6e64 6578 9485 9481 947d 9428  genindex.....}.(
+000007c0: 6805 6806 6816 68a2 6826 6803 6827 4e68  h.h.h.h.h&h.h'Nh
+000007d0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+000007e0: 5d94 288c 0478 7265 6694 8c03 7374 6494  ].(..xref...std.
+000007f0: 8c07 7374 642d 7265 6694 6568 1d5d 9468  ..std-ref.eh.].h
+00000800: 1f5d 9468 215d 9475 6825 68a0 6816 689d  .].h!].uh%h.h.h.
+00000810: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+00000820: 681d 5d94 681f 5d94 6821 5d94 8c06 7265  h.].h.].h!]...re
+00000830: 6664 6f63 9468 4f8c 0972 6566 646f 6d61  fdoc.hO..refdoma
+00000840: 696e 9468 ad8c 0772 6566 7479 7065 948c  in.h...reftype..
+00000850: 0372 6566 948c 0b72 6566 6578 706c 6963  .ref...refexplic
+00000860: 6974 9489 8c07 7265 6677 6172 6e94 888c  it....refwarn...
+00000870: 0972 6566 7461 7267 6574 948c 0867 656e  .reftarget...gen
+00000880: 696e 6465 7894 7568 2568 9b68 2768 2868  index.uh%h.h'h(h
+00000890: 294b 1968 1668 9875 6261 6817 7d94 2868  )K.h.h.ubah.}.(h
+000008a0: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+000008b0: 215d 9475 6825 6896 6827 6828 6829 4b19  !].uh%h.h'h(h)K.
+000008c0: 6816 6892 7562 6168 177d 9428 6819 5d94  h.h.ubah.}.(h.].
+000008d0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+000008e0: 7568 2568 9068 1668 8d68 2668 0368 2768  uh%h.h.h.h&h.h'h
+000008f0: 2868 294e 7562 6891 2981 947d 9428 6805  (h)Nubh.)..}.(h.
+00000900: 8c0f 3a72 6566 3a60 6d6f 6469 6e64 6578  ..:ref:`modindex
+00000910: 6094 6807 5d94 6897 2981 947d 9428 6805  `.h.].h.)..}.(h.
+00000920: 68ce 6807 5d94 689c 2981 947d 9428 6805  h.h.].h.)..}.(h.
+00000930: 68ce 6807 5d94 68a1 2981 947d 9428 6805  h.h.].h.)..}.(h.
+00000940: 68ce 6807 5d94 6811 8c08 6d6f 6469 6e64  h.h.].h...modind
+00000950: 6578 9485 9481 947d 9428 6805 6806 6816  ex.....}.(h.h.h.
+00000960: 68d6 6826 6803 6827 4e68 294e 7562 6168  h.h&h.h'Nh)Nubah
+00000970: 177d 9428 6819 5d94 681b 5d94 2868 ac8c  .}.(h.].h.].(h..
+00000980: 0373 7464 948c 0773 7464 2d72 6566 9465  .std...std-ref.e
+00000990: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+000009a0: a068 1668 d375 6261 6817 7d94 2868 195d  .h.h.ubah.}.(h.]
+000009b0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+000009c0: 948c 0672 6566 646f 6394 684f 8c09 7265  ...refdoc.hO..re
+000009d0: 6664 6f6d 6169 6e94 68e0 8c07 7265 6674  fdomain.h...reft
+000009e0: 7970 6594 8c03 7265 6694 8c0b 7265 6665  ype...ref...refe
+000009f0: 7870 6c69 6369 7494 898c 0772 6566 7761  xplicit....refwa
+00000a00: 726e 9488 68be 8c08 6d6f 6469 6e64 6578  rn..h...modindex
+00000a10: 9475 6825 689b 6827 6828 6829 4b1a 6816  .uh%h.h'h(h)K.h.
+00000a20: 68d0 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
+00000a30: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00000a40: 2568 9668 2768 2868 294b 1a68 1668 cc75  %h.h'h(h)K.h.h.u
+00000a50: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00000a60: 1d5d 9468 1f5d 9468 215d 9475 6825 6890  .].h.].h!].uh%h.
+00000a70: 6816 688d 6826 6803 6827 6828 6829 4e75  h.h.h&h.h'h(h)Nu
+00000a80: 6268 9129 8194 7d94 2868 058c 0d3a 7265  bh.)..}.(h...:re
+00000a90: 663a 6073 6561 7263 6860 9468 075d 9468  f:`search`.h.].h
+00000aa0: 9729 8194 7d94 2868 056a 0001 0000 6807  .)..}.(h.j....h.
+00000ab0: 5d94 689c 2981 947d 9428 6805 6a00 0100  ].h.)..}.(h.j...
+00000ac0: 0068 075d 9468 a129 8194 7d94 2868 056a  .h.].h.)..}.(h.j
+00000ad0: 0001 0000 6807 5d94 6811 8c06 7365 6172  ....h.].h...sear
+00000ae0: 6368 9485 9481 947d 9428 6805 6806 6816  ch.....}.(h.h.h.
+00000af0: 6a08 0100 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00000b00: 6261 6817 7d94 2868 195d 9468 1b5d 9428  bah.}.(h.].h.].(
+00000b10: 68ac 8c03 7374 6494 8c07 7374 642d 7265  h...std...std-re
+00000b20: 6694 6568 1d5d 9468 1f5d 9468 215d 9475  f.eh.].h.].h!].u
+00000b30: 6825 68a0 6816 6a05 0100 0075 6261 6817  h%h.h.j....ubah.
+00000b40: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000b50: 1f5d 9468 215d 948c 0672 6566 646f 6394  .].h!]...refdoc.
+00000b60: 684f 8c09 7265 6664 6f6d 6169 6e94 6a12  hO..refdomain.j.
+00000b70: 0100 008c 0772 6566 7479 7065 948c 0372  .....reftype...r
+00000b80: 6566 948c 0b72 6566 6578 706c 6963 6974  ef...refexplicit
+00000b90: 9489 8c07 7265 6677 6172 6e94 8868 be8c  ....refwarn..h..
+00000ba0: 0673 6561 7263 6894 7568 2568 9b68 2768  .search.uh%h.h'h
+00000bb0: 2868 294b 1b68 166a 0201 0000 7562 6168  (h)K.h.j....ubah
+00000bc0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000bd0: 681f 5d94 6821 5d94 7568 2568 9668 2768  h.].h!].uh%h.h'h
+00000be0: 2868 294b 1b68 1668 fe75 6261 6817 7d94  (h)K.h.h.ubah.}.
+00000bf0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000c00: 9468 215d 9475 6825 6890 6816 688d 6826  .h!].uh%h.h.h.h&
+00000c10: 6803 6827 6828 6829 4e75 6265 6817 7d94  h.h'h(h)Nubeh.}.
+00000c20: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000c30: 9468 215d 948c 0662 756c 6c65 7494 8c01  .h!]...bullet...
+00000c40: 2a94 7568 2568 8b68 2768 2868 294b 1968  *.uh%h.h'h(h)K.h
+00000c50: 1668 7a68 2668 0375 6265 6817 7d94 2868  .hzh&h.ubeh.}.(h
+00000c60: 195d 948c 1269 6e64 6963 6573 2d61 6e64  .]...indices-and
+00000c70: 2d74 6162 6c65 7394 6168 1b5d 9468 1d5d  -tables.ah.].h.]
+00000c80: 948c 1269 6e64 6963 6573 2061 6e64 2074  ...indices and t
+00000c90: 6162 6c65 7394 6168 1f5d 9468 215d 9475  ables.ah.].h!].u
+00000ca0: 6825 682a 6816 6803 6826 6803 6827 6828  h%h*h.h.h&h.h'h(
+00000cb0: 6829 4b17 7562 6568 177d 9428 6819 5d94  h)K.ubeh.}.(h.].
+00000cc0: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+00000cd0: 8c06 736f 7572 6365 9468 2875 6825 6801  ..source.h(uh%h.
+00000ce0: 8c0e 6375 7272 656e 745f 736f 7572 6365  ..current_source
+00000cf0: 944e 8c0c 6375 7272 656e 745f 6c69 6e65  .N..current_line
+00000d00: 944e 8c08 7365 7474 696e 6773 948c 1164  .N..settings...d
+00000d10: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
+00000d20: 948c 0656 616c 7565 7394 9394 2981 947d  ...Values...)..}
+00000d30: 9428 682f 4e8c 0967 656e 6572 6174 6f72  .(h/N..generator
+00000d40: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
+00000d50: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
+00000d60: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
+00000d70: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
+00000d80: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
+00000d90: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
+00000da0: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
+00000db0: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
+00000dc0: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
+00000dd0: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
+00000de0: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
+00000df0: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
+00000e00: 8c0a 6861 6c74 5f6c 6576 656c 944b 058c  ..halt_level.K..
+00000e10: 1165 7869 745f 7374 6174 7573 5f6c 6576  .exit_status_lev
+00000e20: 656c 944b 058c 0564 6562 7567 944e 8c0e  el.K...debug.N..
+00000e30: 7761 726e 696e 675f 7374 7265 616d 944e  warning_stream.N
+00000e40: 8c09 7472 6163 6562 6163 6b94 888c 0e69  ..traceback....i
+00000e50: 6e70 7574 5f65 6e63 6f64 696e 6794 8c09  nput_encoding...
+00000e60: 7574 662d 382d 7369 6794 8c1c 696e 7075  utf-8-sig...inpu
+00000e70: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
+00000e80: 5f68 616e 646c 6572 948c 0673 7472 6963  _handler...stric
+00000e90: 7494 8c0f 6f75 7470 7574 5f65 6e63 6f64  t...output_encod
+00000ea0: 696e 6794 8c05 7574 662d 3894 8c1d 6f75  ing...utf-8...ou
+00000eb0: 7470 7574 5f65 6e63 6f64 696e 675f 6572  tput_encoding_er
+00000ec0: 726f 725f 6861 6e64 6c65 7294 6a63 0100  ror_handler.jc..
+00000ed0: 008c 0e65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
+00000ee0: 6794 8c05 7574 662d 3894 8c1c 6572 726f  g...utf-8...erro
+00000ef0: 725f 656e 636f 6469 6e67 5f65 7272 6f72  r_encoding_error
+00000f00: 5f68 616e 646c 6572 948c 1062 6163 6b73  _handler...backs
+00000f10: 6c61 7368 7265 706c 6163 6594 8c0d 6c61  lashreplace...la
+00000f20: 6e67 7561 6765 5f63 6f64 6594 8c02 656e  nguage_code...en
+00000f30: 948c 1372 6563 6f72 645f 6465 7065 6e64  ...record_depend
+00000f40: 656e 6369 6573 944e 8c06 636f 6e66 6967  encies.N..config
+00000f50: 944e 8c09 6964 5f70 7265 6669 7894 6806  .N..id_prefix.h.
+00000f60: 8c0e 6175 746f 5f69 645f 7072 6566 6978  ..auto_id_prefix
+00000f70: 948c 0269 6494 8c0d 6475 6d70 5f73 6574  ...id...dump_set
+00000f80: 7469 6e67 7394 4e8c 0e64 756d 705f 696e  tings.N..dump_in
+00000f90: 7465 726e 616c 7394 4e8c 0f64 756d 705f  ternals.N..dump_
+00000fa0: 7472 616e 7366 6f72 6d73 944e 8c0f 6475  transforms.N..du
+00000fb0: 6d70 5f70 7365 7564 6f5f 786d 6c94 4e8c  mp_pseudo_xml.N.
+00000fc0: 1065 7870 6f73 655f 696e 7465 726e 616c  .expose_internal
+00000fd0: 7394 4e8c 0e73 7472 6963 745f 7669 7369  s.N..strict_visi
+00000fe0: 746f 7294 4e8c 0f5f 6469 7361 626c 655f  tor.N.._disable_
+00000ff0: 636f 6e66 6967 944e 8c07 5f73 6f75 7263  config.N.._sourc
+00001000: 6594 6828 8c0c 5f64 6573 7469 6e61 7469  e.h(.._destinati
+00001010: 6f6e 944e 8c0d 5f63 6f6e 6669 675f 6669  on.N.._config_fi
+00001020: 6c65 7394 5d94 8c16 6669 6c65 5f69 6e73  les.]...file_ins
+00001030: 6572 7469 6f6e 5f65 6e61 626c 6564 9488  ertion_enabled..
+00001040: 8c0b 7261 775f 656e 6162 6c65 6494 4b01  ..raw_enabled.K.
+00001050: 8c11 6c69 6e65 5f6c 656e 6774 685f 6c69  ..line_length_li
+00001060: 6d69 7494 4a00 e1f5 058c 0e70 6570 5f72  mit.J......pep_r
+00001070: 6566 6572 656e 6365 7394 4e8c 0c70 6570  eferences.N..pep
+00001080: 5f62 6173 655f 7572 6c94 8c18 6874 7470  _base_url...http
+00001090: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
+000010a0: 6f72 672f 948c 1570 6570 5f66 696c 655f  org/...pep_file_
+000010b0: 7572 6c5f 7465 6d70 6c61 7465 948c 0870  url_template...p
+000010c0: 6570 2d25 3034 6494 8c0e 7266 635f 7265  ep-%04d...rfc_re
+000010d0: 6665 7265 6e63 6573 944e 8c0c 7266 635f  ferences.N..rfc_
+000010e0: 6261 7365 5f75 726c 948c 2668 7474 7073  base_url..&https
+000010f0: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
+00001100: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
+00001110: 2f94 8c09 7461 625f 7769 6474 6894 4b08  /...tab_width.K.
+00001120: 8c1d 7472 696d 5f66 6f6f 746e 6f74 655f  ..trim_footnote_
+00001130: 7265 6665 7265 6e63 655f 7370 6163 6594  reference_space.
+00001140: 898c 1073 796e 7461 785f 6869 6768 6c69  ...syntax_highli
+00001150: 6768 7494 8c04 6c6f 6e67 948c 0c73 6d61  ght...long...sma
+00001160: 7274 5f71 756f 7465 7394 888c 1373 6d61  rt_quotes....sma
+00001170: 7274 7175 6f74 6573 5f6c 6f63 616c 6573  rtquotes_locales
+00001180: 945d 948c 1d63 6861 7261 6374 6572 5f6c  .]...character_l
+00001190: 6576 656c 5f69 6e6c 696e 655f 6d61 726b  evel_inline_mark
+000011a0: 7570 9489 8c0e 646f 6374 6974 6c65 5f78  up....doctitle_x
+000011b0: 666f 726d 9489 8c0d 646f 6369 6e66 6f5f  form....docinfo_
+000011c0: 7866 6f72 6d94 4b01 8c12 7365 6374 7375  xform.K...sectsu
+000011d0: 6274 6974 6c65 5f78 666f 726d 9489 8c0d  btitle_xform....
+000011e0: 696d 6167 655f 6c6f 6164 696e 6794 8c04  image_loading...
+000011f0: 6c69 6e6b 948c 1065 6d62 6564 5f73 7479  link...embed_sty
+00001200: 6c65 7368 6565 7494 898c 1563 6c6f 616b  lesheet....cloak
+00001210: 5f65 6d61 696c 5f61 6464 7265 7373 6573  _email_addresses
+00001220: 9488 8c11 7365 6374 696f 6e5f 7365 6c66  ....section_self
+00001230: 5f6c 696e 6b94 898c 0c65 6d62 6564 5f69  _link....embed_i
+00001240: 6d61 6765 7394 898c 0365 6e76 944e 7562  mages....env.Nub
+00001250: 8c08 7265 706f 7274 6572 944e 8c10 696e  ..reporter.N..in
+00001260: 6469 7265 6374 5f74 6172 6765 7473 945d  direct_targets.]
+00001270: 948c 1173 7562 7374 6974 7574 696f 6e5f  ...substitution_
+00001280: 6465 6673 947d 948c 1273 7562 7374 6974  defs.}...substit
+00001290: 7574 696f 6e5f 6e61 6d65 7394 7d94 8c08  ution_names.}...
+000012a0: 7265 666e 616d 6573 947d 948c 0672 6566  refnames.}...ref
+000012b0: 6964 7394 7d94 8c07 6e61 6d65 6964 7394  ids.}...nameids.
+000012c0: 7d94 2868 7768 746a 3d01 0000 6a3a 0100  }.(hwhtj=...j:..
+000012d0: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
+000012e0: 2868 774e 6a3d 0100 004e 7568 197d 9428  (hwNj=...Nuh.}.(
+000012f0: 6874 682c 6a3a 0100 0068 7a75 8c0d 666f  hth,j:...hzu..fo
+00001300: 6f74 6e6f 7465 5f72 6566 7394 7d94 8c0d  otnote_refs.}...
+00001310: 6369 7461 7469 6f6e 5f72 6566 7394 7d94  citation_refs.}.
+00001320: 8c0d 6175 746f 666f 6f74 6e6f 7465 7394  ..autofootnotes.
+00001330: 5d94 8c11 6175 746f 666f 6f74 6e6f 7465  ]...autofootnote
+00001340: 5f72 6566 7394 5d94 8c10 7379 6d62 6f6c  _refs.]...symbol
+00001350: 5f66 6f6f 746e 6f74 6573 945d 948c 1473  _footnotes.]...s
+00001360: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f72  ymbol_footnote_r
+00001370: 6566 7394 5d94 8c09 666f 6f74 6e6f 7465  efs.]...footnote
+00001380: 7394 5d94 8c09 6369 7461 7469 6f6e 7394  s.]...citations.
+00001390: 5d94 8c12 6175 746f 666f 6f74 6e6f 7465  ]...autofootnote
+000013a0: 5f73 7461 7274 944b 018c 1573 796d 626f  _start.K...symbo
+000013b0: 6c5f 666f 6f74 6e6f 7465 5f73 7461 7274  l_footnote_start
+000013c0: 944b 008c 0a69 645f 636f 756e 7465 7294  .K...id_counter.
+000013d0: 8c0b 636f 6c6c 6563 7469 6f6e 7394 8c07  ..collections...
+000013e0: 436f 756e 7465 7294 9394 7d94 8594 5294  Counter...}...R.
+000013f0: 8c0e 7061 7273 655f 6d65 7373 6167 6573  ..parse_messages
+00001400: 945d 948c 1274 7261 6e73 666f 726d 5f6d  .]...transform_m
+00001410: 6573 7361 6765 7394 5d94 8c0b 7472 616e  essages.]...tran
+00001420: 7366 6f72 6d65 7294 4e8c 0b69 6e63 6c75  sformer.N..inclu
+00001430: 6465 5f6c 6f67 945d 948c 0a64 6563 6f72  de_log.]...decor
+00001440: 6174 696f 6e94 4e68 2668 0375 622e       ation.Nh&h.ub.
```

### Comparing `CmonCrawl-0.9.3/docs/build/html/_sources/index.rst.txt` & `CmonCrawl-1.0.0/docs/build/html/_sources/index.rst.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 Welcome to CommonCrawl Extractor's documentation!
 =================================================
 
 .. toctree::
    :maxdepth: 3
    :caption: Contents:
 
-   installation
-   quickstart/index
+   usage
+   cli/index
+   extraction/index
+   prog_guide/index
+   misc/index
    api
 
 
 
-
-
-
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `CmonCrawl-1.0.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/basic.css` & `CmonCrawl-1.0.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/clipboard.min.js` & `CmonCrawl-1.0.0/docs/build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/copybutton.css` & `CmonCrawl-1.0.0/docs/build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/copybutton.js` & `CmonCrawl-1.0.0/docs/build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/copybutton_funcs.js` & `CmonCrawl-1.0.0/docs/build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/doctools.js` & `CmonCrawl-1.0.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/images/logo_binder.svg` & `CmonCrawl-1.0.0/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/images/logo_colab.png` & `CmonCrawl-1.0.0/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/images/logo_deepnote.svg` & `CmonCrawl-1.0.0/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/images/logo_jupyterhub.svg` & `CmonCrawl-1.0.0/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/jquery-3.6.0.js` & `CmonCrawl-1.0.0/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/jquery.js` & `CmonCrawl-1.0.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/language_data.js` & `CmonCrawl-1.0.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `CmonCrawl-1.0.0/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/pygments.css` & `CmonCrawl-1.0.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `CmonCrawl-1.0.0/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/scripts/sphinx-book-theme.js` & `CmonCrawl-1.0.0/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `CmonCrawl-1.0.0/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/searchtools.js` & `CmonCrawl-1.0.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/sphinx_highlight.js` & `CmonCrawl-1.0.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `CmonCrawl-1.0.0/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/styles/sphinx-book-theme.css` & `CmonCrawl-1.0.0/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/styles/theme.css` & `CmonCrawl-1.0.0/docs/build/html/_static/styles/theme.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/underscore-1.13.1.js` & `CmonCrawl-1.0.0/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/underscore.js` & `CmonCrawl-1.0.0/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2` & `CmonCrawl-1.0.0/docs/build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/_static/webpack-macros.html` & `CmonCrawl-1.0.0/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/build/html/api.html` & `CmonCrawl-1.0.0/docs/build/html/search.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
-
-    <title>API &#8212; CommonCrawl Extractor 1.0 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+    <title>Search &#8212; CmonCrawl 0.9.3 documentation</title>
     
   <!-- Loaded before other Sphinx assets -->
   <link href="_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
 <link href="_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
 
     
   <link rel="stylesheet"
@@ -23,34 +22,38 @@
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" href="_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     
   <!-- Pre-loaded scripts that we'll load fully later -->
   <link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
 
+    
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/clipboard.min.js"></script>
     <script src="_static/copybutton.js"></script>
     <script src="_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
+    <script src="_static/searchtools.js"></script>
+    <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Aggregator" href="generated/Aggregator.html" />
-    <link rel="prev" title="Quickstart" href="quickstart/quick-start.html" />
+    <link rel="search" title="Search" href="#" />
+  <script src="searchindex.js" defer></script>
+  
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <meta name="docsearch:language" content="en">
     
 
     <!-- Google Analytics -->
     
+
   </head>
   <body data-spy="scroll" data-target="#bd-toc-nav" data-offset="60">
 <!-- Checkboxes to toggle the left sidebar -->
 <input type="checkbox" class="sidebar-toggle" name="__navigation" id="__navigation" aria-label="Toggle navigation sidebar">
 <label class="overlay overlay-navbar" for="__navigation">
     <div class="visually-hidden">Toggle navigation sidebar</div>
 </label>
@@ -75,189 +78,208 @@
 <div class="bd-sidebar noprint" id="site-navigation">
     <div class="bd-sidebar__content">
         <div class="bd-sidebar__top"><div class="navbar-brand-box">
     <a class="navbar-brand text-wrap" href="index.html">
       
       
       
-      <h1 class="site-logo" id="site-title">CommonCrawl Extractor 1.0 documentation</h1>
+      <h1 class="site-logo" id="site-title">CmonCrawl 0.9.3 documentation</h1>
       
     </a>
-</div><form class="bd-search d-flex align-items-center" action="search.html" method="get">
+</div><form class="bd-search d-flex align-items-center" action="#" method="get">
   <i class="icon fas fa-search"></i>
   <input type="search" class="form-control" name="q" id="search-input" placeholder="Search the docs ..." aria-label="Search the docs ..." autocomplete="off" >
 </form><nav class="bd-links" id="bd-docs-nav" aria-label="Main">
     <div class="bd-toc-item active">
         <p aria-level="2" class="caption" role="heading">
  <span class="caption-text">
   Contents:
  </span>
 </p>
-<ul class="current nav bd-sidenav">
+<ul class="nav bd-sidenav">
+ <li class="toctree-l1">
+  <a class="reference internal" href="usage.html">
+   Usage
+  </a>
+ </li>
  <li class="toctree-l1 has-children">
-  <a class="reference internal" href="quickstart/index.html">
-   Quick Start Guide
+  <a class="reference internal" href="cli/index.html">
+   Command Line Interface
   </a>
   <input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" type="checkbox"/>
   <label for="toctree-checkbox-1">
    <i class="fas fa-chevron-down">
    </i>
   </label>
   <ul>
    <li class="toctree-l2">
-    <a class="reference internal" href="quickstart/overview.html">
-     Quick Overview
+    <a class="reference internal" href="cli/cli.html">
+     Command Line Interface
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="cli/download.html">
+     Command Line Download
     </a>
    </li>
    <li class="toctree-l2">
-    <a class="reference internal" href="quickstart/quick-start.html">
-     Quickstart
+    <a class="reference internal" href="cli/extract.html">
+     Command line Extract
     </a>
    </li>
   </ul>
  </li>
- <li class="toctree-l1 current active has-children">
-  <a class="current reference internal" href="#">
-   API
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="extraction/index.html">
+   Extraction
   </a>
-  <input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
+  <input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
   <label for="toctree-checkbox-2">
    <i class="fas fa-chevron-down">
    </i>
   </label>
   <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/creating_extractor.html">
+     Custom Extractor
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/config_file.html">
+     Extractor config file
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/utils.html">
+     Extraction utils
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="prog_guide/index.html">
+   Programming Guide
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
+  <label for="toctree-checkbox-3">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/overview.html">
+     Programming Guide
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/pip.html">
+     Custom Pipeline
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="misc/index.html">
+   Miscellaneous
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
+  <label for="toctree-checkbox-4">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="misc/domain_record.html">
+     Domain Record
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="api.html">
+   API
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
+  <label for="toctree-checkbox-5">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
    <li class="toctree-l2 has-children">
-    <a class="reference internal" href="generated/Aggregator.html">
-     Aggregator
+    <a class="reference internal" href="generated/cmoncrawl.html">
+     cmoncrawl
     </a>
-    <input class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
-    <label for="toctree-checkbox-3">
+    <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
+    <label for="toctree-checkbox-6">
      <i class="fas fa-chevron-down">
      </i>
     </label>
     <ul>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="generated/Aggregator.App.html">
-       Aggregator.App
+      <a class="reference internal" href="generated/cmoncrawl.aggregator.html">
+       cmoncrawl.aggregator
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
-      <label for="toctree-checkbox-4">
+      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
+      <label for="toctree-checkbox-7">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="generated/Aggregator.App.index_query.html">
-         Aggregator.App.index_query
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Aggregator.App.ndjson_decoder.html">
-         Aggregator.App.ndjson_decoder
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.index_query.html">
+         cmoncrawl.aggregator.index_query
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="generated/Aggregator.App.utils.html">
-         Aggregator.App.utils
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.utils.html">
+         cmoncrawl.aggregator.utils
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="generated/Aggregator.aggregator.html">
-       Aggregator.aggregator
-      </a>
-     </li>
-    </ul>
-   </li>
-   <li class="toctree-l2 has-children">
-    <a class="reference internal" href="generated/Processor.html">
-     Processor
-    </a>
-    <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
-    <label for="toctree-checkbox-5">
-     <i class="fas fa-chevron-down">
-     </i>
-    </label>
-    <ul>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="generated/Processor.App.html">
-       Processor.App
+      <a class="reference internal" href="generated/cmoncrawl.common.html">
+       cmoncrawl.common
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
-      <label for="toctree-checkbox-6">
+      <input class="toctree-checkbox" id="toctree-checkbox-8" name="toctree-checkbox-8" type="checkbox"/>
+      <label for="toctree-checkbox-8">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.Downloader.html">
-         Processor.App.Downloader
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.Extractor.html">
-         Processor.App.Extractor
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.OutStreamer.html">
-         Processor.App.OutStreamer
+        <a class="reference internal" href="generated/cmoncrawl.common.loggers.html">
+         cmoncrawl.common.loggers
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.Pipeline.html">
-         Processor.App.Pipeline
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.Router.html">
-         Processor.App.Router
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.processor_utils.html">
-         Processor.App.processor_utils
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.App.ArticleUtils.html">
-         Processor.App.ArticleUtils
+        <a class="reference internal" href="generated/cmoncrawl.common.types.html">
+         cmoncrawl.common.types
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="generated/Processor.process_article.html">
-       Processor.process_article
-      </a>
-     </li>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="generated/Processor.processor.html">
-       Processor.processor
+      <a class="reference internal" href="generated/cmoncrawl.processor.html">
+       cmoncrawl.processor
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
-      <label for="toctree-checkbox-7">
+      <input class="toctree-checkbox" id="toctree-checkbox-9" name="toctree-checkbox-9" type="checkbox"/>
+      <label for="toctree-checkbox-9">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.processor.Listener.html">
-         Processor.processor.Listener
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.processor.ListnerStats.html">
-         Processor.processor.ListnerStats
+        <a class="reference internal" href="generated/cmoncrawl.processor.extraction.html">
+         cmoncrawl.processor.extraction
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="generated/Processor.processor.Message.html">
-         Processor.processor.Message
+        <a class="reference internal" href="generated/cmoncrawl.processor.pipeline.html">
+         cmoncrawl.processor.pipeline
         </a>
        </li>
       </ul>
      </li>
     </ul>
    </li>
   </ul>
@@ -323,123 +345,75 @@
 
 <span class="headerbtn__icon-container">
   <i class="fas fa-expand"></i>
   </span>
 
 </button>
 
-<div class="menu-dropdown menu-dropdown-download-buttons">
-  <button class="headerbtn menu-dropdown__trigger"
-      aria-label="Download this page">
-      <i class="fas fa-download"></i>
-  </button>
-  <div class="menu-dropdown__content">
-    <ul>
-      <li>
-        <a href="_sources/api.rst.txt"
-   class="headerbtn"
-   data-toggle="tooltip"
-data-placement="left"
-title="Download source file"
->
-  
-
-<span class="headerbtn__icon-container">
-  <i class="fas fa-file"></i>
-  </span>
-<span class="headerbtn__text-container">.rst</span>
-</a>
-
-      </li>
-      
-      <li>
-        
-<button onclick="printPdf(this)"
-  class="headerbtn"
-  data-toggle="tooltip"
-data-placement="left"
-title="Print to PDF"
->
-  
-
-<span class="headerbtn__icon-container">
-  <i class="fas fa-file-pdf"></i>
-  </span>
-<span class="headerbtn__text-container">.pdf</span>
-</button>
-
-      </li>
-      
-    </ul>
-  </div>
-</div>
-
     </div>
 </div>
 
 <!-- Table of contents -->
 <div class="col-md-3 bd-toc show noprint">
 </div>
     </div>
     <div class="article row">
         <div class="col pl-md-3 pl-lg-5 content-container">
             <!-- Table of contents that is only displayed when printing the page -->
             <div id="jb-print-docs-body" class="onlyprint">
-                <h1>API</h1>
+                <h1></h1>
                 <!-- Table of contents -->
                 <div id="print-main-content">
                     <div id="jb-print-toc">
                         
                     </div>
                 </div>
             </div>
             <main id="main-content" role="main">
                 
               <div>
                 
-  <section id="api">
-<h1>API<a class="headerlink" href="#api" title="Permalink to this heading">#</a></h1>
-<table class="autosummary longtable table autosummary">
-<colgroup>
-<col style="width: 10%" />
-<col style="width: 90%" />
-</colgroup>
-<tbody>
-<tr class="row-odd"><td><p><a class="reference internal" href="generated/Aggregator.html#module-Aggregator" title="Aggregator"><code class="xref py py-obj docutils literal notranslate"><span class="pre">Aggregator</span></code></a></p></td>
-<td><p></p></td>
-</tr>
-<tr class="row-even"><td><p><a class="reference internal" href="generated/Processor.html#module-Processor" title="Processor"><code class="xref py py-obj docutils literal notranslate"><span class="pre">Processor</span></code></a></p></td>
-<td><p></p></td>
-</tr>
-</tbody>
-</table>
-</section>
-
+  <h1 id="search-documentation">Search</h1>
+  
+  <noscript>
+  <div class="admonition warning">
+  <p>
+    Please activate JavaScript to enable the search
+    functionality.
+  </p>
+  </div>
+  </noscript>
+  
+  
+  <p>
+    Searching for multiple words only shows matches that contain
+    all words.
+  </p>
+  
+  
+  <form action="" method="get">
+    <input type="text" name="q" aria-labelledby="search-documentation" value="" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
+    <input type="submit" value="search" />
+    <span id="search-progress" style="padding-left: 10px"></span>
+  </form>
+  
+  
+  
+  <div id="search-results">
+  
+  </div>
+  
 
               </div>
               
             </main>
             <footer class="footer-article noprint">
                 
     <!-- Previous / next buttons -->
 <div class='prev-next-area'>
-    <a class='left-prev' id="prev-link" href="quickstart/quick-start.html" title="previous page">
-        <i class="fas fa-angle-left"></i>
-        <div class="prev-next-info">
-            <p class="prev-next-subtitle">previous</p>
-            <p class="prev-next-title">Quickstart</p>
-        </div>
-    </a>
-    <a class='right-next' id="next-link" href="generated/Aggregator.html" title="next page">
-    <div class="prev-next-info">
-        <p class="prev-next-subtitle">next</p>
-        <p class="prev-next-title">Aggregator</p>
-    </div>
-    <i class="fas fa-angle-right"></i>
-    </a>
 </div>
             </footer>
         </div>
     </div>
     <div class="footer-content row">
         <footer class="col footer"><p>
```

#### html2text {}

```diff
@@ -10,59 +10,50 @@
 
 
 
 
 
 
 
-
-
  ⁰
 Toggle navigation sidebar
   ⁰
 Toggle in-page Table of Contents
 
-******_CommonCrawl_Extractor_1.0_documentation_******
+******_CmonCrawl_0.9.3_documentation_******
  [Unknown INPUT type]
  Contents:
-    * Quick_Start_Guide ⁰
-          o Quick_Overview
-          o Quickstart
-    * API *
-          o Aggregator ⁰
-                # Aggregator.App ⁰
-                      # Aggregator.App.index_query
-                      # Aggregator.App.ndjson_decoder
-                      # Aggregator.App.utils
-                # Aggregator.aggregator
-          o Processor ⁰
-                # Processor.App ⁰
-                      # Processor.App.Downloader
-                      # Processor.App.Extractor
-                      # Processor.App.OutStreamer
-                      # Processor.App.Pipeline
-                      # Processor.App.Router
-                      # Processor.App.processor_utils
-                      # Processor.App.ArticleUtils
-                # Processor.process_article
-                # Processor.processor ⁰
-                      # Processor.processor.Listener
-                      # Processor.processor.ListnerStats
-                      # Processor.processor.Message
+    * Usage
+    * Command_Line_Interface ⁰
+          o Command_Line_Interface
+          o Command_Line_Download
+          o Command_line_Extract
+    * Extraction ⁰
+          o Custom_Extractor
+          o Extractor_config_file
+          o Extraction_utils
+    * Programming_Guide ⁰
+          o Programming_Guide
+          o Custom_Pipeline
+    * Miscellaneous ⁰
+          o Domain_Record
+    * API ⁰
+          o cmoncrawl ⁰
+                # cmoncrawl.aggregator ⁰
+                      # cmoncrawl.aggregator.index_query
+                      # cmoncrawl.aggregator.utils
+                # cmoncrawl.common ⁰
+                      # cmoncrawl.common.loggers
+                      # cmoncrawl.common.types
+                # cmoncrawl.processor ⁰
+                      # cmoncrawl.processor.extraction
+                      # cmoncrawl.processor.pipeline
 Theme by the Executable_Book_Project
 
 
+****** Search ******
+Please activate JavaScript to enable the search functionality.
+Searching for multiple words only shows matches that contain all words.
+[q                   ] [search]
 
-    *    .rst
-    *     .pdf
-****** API ******
-****** API# ******
-Aggregator
-Processor
-
-previous
-Quickstart
-
-next
-Aggregator
 By Hynek KydlÃ­Äek
 © Copyright 2022, Hynek KydlÃ­Äek.
```

### Comparing `CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.html` & `CmonCrawl-1.0.0/docs/build/html/api.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Aggregator.App &#8212; CommonCrawl Extractor 1.0 documentation</title>
+    <title>API &#8212; CmonCrawl 0.9.3 documentation</title>
     
   <!-- Loaded before other Sphinx assets -->
-  <link href="../_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
-<link href="../_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
+  <link href="_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
+<link href="_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
 
     
   <link rel="stylesheet"
-    href="../_static/vendor/fontawesome/5.13.0/css/all.min.css">
+    href="_static/vendor/fontawesome/5.13.0/css/all.min.css">
   <link rel="preload" as="font" type="font/woff2" crossorigin
-    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
+    href="_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
   <link rel="preload" as="font" type="font/woff2" crossorigin
-    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">
+    href="_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">
 
-    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" href="../_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
-    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" href="_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
+    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     
   <!-- Pre-loaded scripts that we'll load fully later -->
-  <link rel="preload" as="script" href="../_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
+  <link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
 
-    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
-    <script src="../_static/jquery.js"></script>
-    <script src="../_static/underscore.js"></script>
-    <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="../_static/doctools.js"></script>
-    <script src="../_static/sphinx_highlight.js"></script>
-    <script src="../_static/clipboard.min.js"></script>
-    <script src="../_static/copybutton.js"></script>
-    <script src="../_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/jquery.js"></script>
+    <script src="_static/underscore.js"></script>
+    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/clipboard.min.js"></script>
+    <script src="_static/copybutton.js"></script>
+    <script src="_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
-    <link rel="index" title="Index" href="../genindex.html" />
-    <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="Aggregator.App.index_query" href="Aggregator.App.index_query.html" />
-    <link rel="prev" title="Aggregator" href="Aggregator.html" />
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="cmoncrawl" href="generated/cmoncrawl.html" />
+    <link rel="prev" title="Domain Record" href="misc/domain_record.html" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <meta name="docsearch:language" content="en">
     
 
     <!-- Google Analytics -->
     
   </head>
@@ -71,193 +71,212 @@
     <div class="container-xl">
       <div class="row">
           
 <!-- Sidebar -->
 <div class="bd-sidebar noprint" id="site-navigation">
     <div class="bd-sidebar__content">
         <div class="bd-sidebar__top"><div class="navbar-brand-box">
-    <a class="navbar-brand text-wrap" href="../index.html">
+    <a class="navbar-brand text-wrap" href="index.html">
       
       
       
-      <h1 class="site-logo" id="site-title">CommonCrawl Extractor 1.0 documentation</h1>
+      <h1 class="site-logo" id="site-title">CmonCrawl 0.9.3 documentation</h1>
       
     </a>
-</div><form class="bd-search d-flex align-items-center" action="../search.html" method="get">
+</div><form class="bd-search d-flex align-items-center" action="search.html" method="get">
   <i class="icon fas fa-search"></i>
   <input type="search" class="form-control" name="q" id="search-input" placeholder="Search the docs ..." aria-label="Search the docs ..." autocomplete="off" >
 </form><nav class="bd-links" id="bd-docs-nav" aria-label="Main">
     <div class="bd-toc-item active">
         <p aria-level="2" class="caption" role="heading">
  <span class="caption-text">
   Contents:
  </span>
 </p>
 <ul class="current nav bd-sidenav">
+ <li class="toctree-l1">
+  <a class="reference internal" href="usage.html">
+   Usage
+  </a>
+ </li>
  <li class="toctree-l1 has-children">
-  <a class="reference internal" href="../quickstart/index.html">
-   Quick Start Guide
+  <a class="reference internal" href="extraction/index.html">
+   Extraction
   </a>
   <input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" type="checkbox"/>
   <label for="toctree-checkbox-1">
    <i class="fas fa-chevron-down">
    </i>
   </label>
   <ul>
    <li class="toctree-l2">
-    <a class="reference internal" href="../quickstart/overview.html">
-     Quick Overview
+    <a class="reference internal" href="extraction/creating_extractor.html">
+     Extractors structure
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/config_file.html">
+     Extractor config file
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/utils.html">
+     Extraction utils
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="cli/index.html">
+   Command Line Interface
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
+  <label for="toctree-checkbox-2">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="cli/cli.html">
+     Command Line Interface
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="cli/download.html">
+     Command Line Download
     </a>
    </li>
    <li class="toctree-l2">
-    <a class="reference internal" href="../quickstart/quick-start.html">
-     Quickstart
+    <a class="reference internal" href="cli/extract.html">
+     Command line Extract
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="prog_guide/index.html">
+   Programming Guide
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
+  <label for="toctree-checkbox-3">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/overview.html">
+     Programming Guide
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/pip.html">
+     Custom Pipeline
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="misc/index.html">
+   Miscellaneous
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
+  <label for="toctree-checkbox-4">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="misc/domain_record.html">
+     Domain Record
     </a>
    </li>
   </ul>
  </li>
  <li class="toctree-l1 current active has-children">
-  <a class="reference internal" href="../api.html">
+  <a class="current reference internal" href="#">
    API
   </a>
-  <input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
-  <label for="toctree-checkbox-2">
+  <input checked="" class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
+  <label for="toctree-checkbox-5">
    <i class="fas fa-chevron-down">
    </i>
   </label>
-  <ul class="current">
-   <li class="toctree-l2 current active has-children">
-    <a class="reference internal" href="Aggregator.html">
-     Aggregator
+  <ul>
+   <li class="toctree-l2 has-children">
+    <a class="reference internal" href="generated/cmoncrawl.html">
+     cmoncrawl
     </a>
-    <input checked="" class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
-    <label for="toctree-checkbox-3">
+    <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
+    <label for="toctree-checkbox-6">
      <i class="fas fa-chevron-down">
      </i>
     </label>
-    <ul class="current">
-     <li class="toctree-l3 current active has-children">
-      <a class="current reference internal" href="#">
-       Aggregator.App
+    <ul>
+     <li class="toctree-l3 has-children">
+      <a class="reference internal" href="generated/cmoncrawl.aggregator.html">
+       cmoncrawl.aggregator
       </a>
-      <input checked="" class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
-      <label for="toctree-checkbox-4">
+      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
+      <label for="toctree-checkbox-7">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.index_query.html">
-         Aggregator.App.index_query
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.ndjson_decoder.html">
-         Aggregator.App.ndjson_decoder
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.index_query.html">
+         cmoncrawl.aggregator.index_query
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.utils.html">
-         Aggregator.App.utils
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.utils.html">
+         cmoncrawl.aggregator.utils
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="Aggregator.aggregator.html">
-       Aggregator.aggregator
-      </a>
-     </li>
-    </ul>
-   </li>
-   <li class="toctree-l2 has-children">
-    <a class="reference internal" href="Processor.html">
-     Processor
-    </a>
-    <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
-    <label for="toctree-checkbox-5">
-     <i class="fas fa-chevron-down">
-     </i>
-    </label>
-    <ul>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="Processor.App.html">
-       Processor.App
+      <a class="reference internal" href="generated/cmoncrawl.common.html">
+       cmoncrawl.common
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
-      <label for="toctree-checkbox-6">
+      <input class="toctree-checkbox" id="toctree-checkbox-8" name="toctree-checkbox-8" type="checkbox"/>
+      <label for="toctree-checkbox-8">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Downloader.html">
-         Processor.App.Downloader
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Extractor.html">
-         Processor.App.Extractor
+        <a class="reference internal" href="generated/cmoncrawl.common.loggers.html">
+         cmoncrawl.common.loggers
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.OutStreamer.html">
-         Processor.App.OutStreamer
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Pipeline.html">
-         Processor.App.Pipeline
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Router.html">
-         Processor.App.Router
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.processor_utils.html">
-         Processor.App.processor_utils
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.ArticleUtils.html">
-         Processor.App.ArticleUtils
+        <a class="reference internal" href="generated/cmoncrawl.common.types.html">
+         cmoncrawl.common.types
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="Processor.process_article.html">
-       Processor.process_article
-      </a>
-     </li>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="Processor.processor.html">
-       Processor.processor
+      <a class="reference internal" href="generated/cmoncrawl.processor.html">
+       cmoncrawl.processor
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
-      <label for="toctree-checkbox-7">
+      <input class="toctree-checkbox" id="toctree-checkbox-9" name="toctree-checkbox-9" type="checkbox"/>
+      <label for="toctree-checkbox-9">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.Listener.html">
-         Processor.processor.Listener
+        <a class="reference internal" href="generated/cmoncrawl.processor.extraction.html">
+         cmoncrawl.processor.extraction
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.ListnerStats.html">
-         Processor.processor.ListnerStats
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.Message.html">
-         Processor.processor.Message
+        <a class="reference internal" href="generated/cmoncrawl.processor.pipeline.html">
+         cmoncrawl.processor.pipeline
         </a>
        </li>
       </ul>
      </li>
     </ul>
    </li>
   </ul>
@@ -331,15 +350,15 @@
   <button class="headerbtn menu-dropdown__trigger"
       aria-label="Download this page">
       <i class="fas fa-download"></i>
   </button>
   <div class="menu-dropdown__content">
     <ul>
       <li>
-        <a href="../_sources/generated/Aggregator.App.rst.txt"
+        <a href="_sources/api.rst.txt"
    class="headerbtn"
    data-toggle="tooltip"
 data-placement="left"
 title="Download source file"
 >
   
 
@@ -380,67 +399,60 @@
 <div class="col-md-3 bd-toc show noprint">
 </div>
     </div>
     <div class="article row">
         <div class="col pl-md-3 pl-lg-5 content-container">
             <!-- Table of contents that is only displayed when printing the page -->
             <div id="jb-print-docs-body" class="onlyprint">
-                <h1>Aggregator.App</h1>
+                <h1>API</h1>
                 <!-- Table of contents -->
                 <div id="print-main-content">
                     <div id="jb-print-toc">
                         
                     </div>
                 </div>
             </div>
             <main id="main-content" role="main">
                 
               <div>
                 
-  <section id="module-Aggregator.App">
-<span id="aggregator-app"></span><h1>Aggregator.App<a class="headerlink" href="#module-Aggregator.App" title="Permalink to this heading">#</a></h1>
-<p class="rubric">Modules</p>
+  <section id="api">
+<h1>API<a class="headerlink" href="#api" title="Permalink to this heading">#</a></h1>
 <table class="autosummary longtable table autosummary">
 <colgroup>
 <col style="width: 10%" />
 <col style="width: 90%" />
 </colgroup>
 <tbody>
-<tr class="row-odd"><td><p><a class="reference internal" href="Aggregator.App.index_query.html#module-Aggregator.App.index_query" title="Aggregator.App.index_query"><code class="xref py py-obj docutils literal notranslate"><span class="pre">Aggregator.App.index_query</span></code></a></p></td>
-<td><p></p></td>
-</tr>
-<tr class="row-even"><td><p><a class="reference internal" href="Aggregator.App.ndjson_decoder.html#module-Aggregator.App.ndjson_decoder" title="Aggregator.App.ndjson_decoder"><code class="xref py py-obj docutils literal notranslate"><span class="pre">Aggregator.App.ndjson_decoder</span></code></a></p></td>
-<td><p></p></td>
-</tr>
-<tr class="row-odd"><td><p><a class="reference internal" href="Aggregator.App.utils.html#module-Aggregator.App.utils" title="Aggregator.App.utils"><code class="xref py py-obj docutils literal notranslate"><span class="pre">Aggregator.App.utils</span></code></a></p></td>
+<tr class="row-odd"><td><p><a class="reference internal" href="generated/cmoncrawl.html#module-cmoncrawl" title="cmoncrawl"><code class="xref py py-obj docutils literal notranslate"><span class="pre">cmoncrawl</span></code></a></p></td>
 <td><p></p></td>
 </tr>
 </tbody>
 </table>
 </section>
 
 
               </div>
               
             </main>
             <footer class="footer-article noprint">
                 
     <!-- Previous / next buttons -->
 <div class='prev-next-area'>
-    <a class='left-prev' id="prev-link" href="Aggregator.html" title="previous page">
+    <a class='left-prev' id="prev-link" href="misc/domain_record.html" title="previous page">
         <i class="fas fa-angle-left"></i>
         <div class="prev-next-info">
             <p class="prev-next-subtitle">previous</p>
-            <p class="prev-next-title">Aggregator</p>
+            <p class="prev-next-title">Domain Record</p>
         </div>
     </a>
-    <a class='right-next' id="next-link" href="Aggregator.App.index_query.html" title="next page">
+    <a class='right-next' id="next-link" href="generated/cmoncrawl.html" title="next page">
     <div class="prev-next-info">
         <p class="prev-next-subtitle">next</p>
-        <p class="prev-next-title">Aggregator.App.index_query</p>
+        <p class="prev-next-title">cmoncrawl</p>
     </div>
     <i class="fas fa-angle-right"></i>
     </a>
 </div>
             </footer>
         </div>
     </div>
@@ -457,12 +469,12 @@
 </div>
 
 
       </div>
     </div>
   
   <!-- Scripts loaded after <body> so the DOM is not blocked -->
-  <script src="../_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf"></script>
+  <script src="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf"></script>
 
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -17,54 +17,52 @@
 
 
  ⁰
 Toggle navigation sidebar
   ⁰
 Toggle in-page Table of Contents
 
-******_CommonCrawl_Extractor_1.0_documentation_******
+******_CmonCrawl_0.9.3_documentation_******
  [Unknown INPUT type]
  Contents:
-    * Quick_Start_Guide ⁰
-          o Quick_Overview
-          o Quickstart
+    * Usage
+    * Extraction ⁰
+          o Extractors_structure
+          o Extractor_config_file
+          o Extraction_utils
+    * Command_Line_Interface ⁰
+          o Command_Line_Interface
+          o Command_Line_Download
+          o Command_line_Extract
+    * Programming_Guide ⁰
+          o Programming_Guide
+          o Custom_Pipeline
+    * Miscellaneous ⁰
+          o Domain_Record
     * API *
-          o Aggregator *
-                # Aggregator.App *
-                      # Aggregator.App.index_query
-                      # Aggregator.App.ndjson_decoder
-                      # Aggregator.App.utils
-                # Aggregator.aggregator
-          o Processor ⁰
-                # Processor.App ⁰
-                      # Processor.App.Downloader
-                      # Processor.App.Extractor
-                      # Processor.App.OutStreamer
-                      # Processor.App.Pipeline
-                      # Processor.App.Router
-                      # Processor.App.processor_utils
-                      # Processor.App.ArticleUtils
-                # Processor.process_article
-                # Processor.processor ⁰
-                      # Processor.processor.Listener
-                      # Processor.processor.ListnerStats
-                      # Processor.processor.Message
+          o cmoncrawl ⁰
+                # cmoncrawl.aggregator ⁰
+                      # cmoncrawl.aggregator.index_query
+                      # cmoncrawl.aggregator.utils
+                # cmoncrawl.common ⁰
+                      # cmoncrawl.common.loggers
+                      # cmoncrawl.common.types
+                # cmoncrawl.processor ⁰
+                      # cmoncrawl.processor.extraction
+                      # cmoncrawl.processor.pipeline
 Theme by the Executable_Book_Project
 
 
 
     *    .rst
     *     .pdf
-****** Aggregator.App ******
-****** Aggregator.App# ******
-Modules
-Aggregator.App.index_query
-Aggregator.App.ndjson_decoder
-Aggregator.App.utils
+****** API ******
+****** API# ******
+cmoncrawl
 
 previous
-Aggregator
+Domain_Record
 
 next
-Aggregator.App.index_query
+cmoncrawl
 By Hynek KydlÃ­Äek
 © Copyright 2022, Hynek KydlÃ­Äek.
```

### Comparing `CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.index_query.DomainCrawl.__init__.html` & `CmonCrawl-1.0.0/docs/build/html/py-modindex.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
-
-    <title>Aggregator.App.index_query.DomainCrawl.__init__ &#8212; CommonCrawl Extractor 1.0 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+    <title>Python Module Index &#8212; CmonCrawl 0.9.3 documentation</title>
     
   <!-- Loaded before other Sphinx assets -->
-  <link href="../_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
-<link href="../_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
+  <link href="_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
+<link href="_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
 
     
   <link rel="stylesheet"
-    href="../_static/vendor/fontawesome/5.13.0/css/all.min.css">
+    href="_static/vendor/fontawesome/5.13.0/css/all.min.css">
   <link rel="preload" as="font" type="font/woff2" crossorigin
-    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
+    href="_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
   <link rel="preload" as="font" type="font/woff2" crossorigin
-    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">
+    href="_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">
 
-    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" href="../_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
-    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" href="_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
+    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     
   <!-- Pre-loaded scripts that we'll load fully later -->
-  <link rel="preload" as="script" href="../_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
+  <link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
 
-    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
-    <script src="../_static/jquery.js"></script>
-    <script src="../_static/underscore.js"></script>
-    <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="../_static/doctools.js"></script>
-    <script src="../_static/sphinx_highlight.js"></script>
-    <script src="../_static/clipboard.min.js"></script>
-    <script src="../_static/copybutton.js"></script>
-    <script src="../_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/jquery.js"></script>
+    <script src="_static/underscore.js"></script>
+    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/clipboard.min.js"></script>
+    <script src="_static/copybutton.js"></script>
+    <script src="_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
-    <link rel="index" title="Index" href="../genindex.html" />
-    <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="Aggregator.App.index_query.DomainRecord" href="Aggregator.App.index_query.DomainRecord.html" />
-    <link rel="prev" title="Aggregator.App.index_query.DomainCrawl" href="Aggregator.App.index_query.DomainCrawl.html" />
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <meta name="docsearch:language" content="en">
     
 
     <!-- Google Analytics -->
     
+
+
   </head>
   <body data-spy="scroll" data-target="#bd-toc-nav" data-offset="60">
 <!-- Checkboxes to toggle the left sidebar -->
 <input type="checkbox" class="sidebar-toggle" name="__navigation" id="__navigation" aria-label="Toggle navigation sidebar">
 <label class="overlay overlay-navbar" for="__navigation">
     <div class="visually-hidden">Toggle navigation sidebar</div>
 </label>
@@ -71,188 +71,212 @@
     <div class="container-xl">
       <div class="row">
           
 <!-- Sidebar -->
 <div class="bd-sidebar noprint" id="site-navigation">
     <div class="bd-sidebar__content">
         <div class="bd-sidebar__top"><div class="navbar-brand-box">
-    <a class="navbar-brand text-wrap" href="../index.html">
+    <a class="navbar-brand text-wrap" href="index.html">
       
       
       
-      <h1 class="site-logo" id="site-title">CommonCrawl Extractor 1.0 documentation</h1>
+      <h1 class="site-logo" id="site-title">CmonCrawl 0.9.3 documentation</h1>
       
     </a>
-</div><form class="bd-search d-flex align-items-center" action="../search.html" method="get">
+</div><form class="bd-search d-flex align-items-center" action="search.html" method="get">
   <i class="icon fas fa-search"></i>
   <input type="search" class="form-control" name="q" id="search-input" placeholder="Search the docs ..." aria-label="Search the docs ..." autocomplete="off" >
 </form><nav class="bd-links" id="bd-docs-nav" aria-label="Main">
     <div class="bd-toc-item active">
         <p aria-level="2" class="caption" role="heading">
  <span class="caption-text">
   Contents:
  </span>
 </p>
-<ul class="current nav bd-sidenav">
+<ul class="nav bd-sidenav">
+ <li class="toctree-l1">
+  <a class="reference internal" href="usage.html">
+   Usage
+  </a>
+ </li>
  <li class="toctree-l1 has-children">
-  <a class="reference internal" href="../quickstart/index.html">
-   Quick Start Guide
+  <a class="reference internal" href="cli/index.html">
+   Command Line Interface
   </a>
   <input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" type="checkbox"/>
   <label for="toctree-checkbox-1">
    <i class="fas fa-chevron-down">
    </i>
   </label>
   <ul>
    <li class="toctree-l2">
-    <a class="reference internal" href="../quickstart/overview.html">
-     Quick Overview
+    <a class="reference internal" href="cli/cli.html">
+     Command Line Interface
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="cli/download.html">
+     Command Line Download
     </a>
    </li>
    <li class="toctree-l2">
-    <a class="reference internal" href="../quickstart/quick-start.html">
-     Quickstart
+    <a class="reference internal" href="cli/extract.html">
+     Command line Extract
     </a>
    </li>
   </ul>
  </li>
- <li class="toctree-l1 current active has-children">
-  <a class="reference internal" href="../api.html">
-   API
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="extraction/index.html">
+   Extraction
   </a>
-  <input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
+  <input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
   <label for="toctree-checkbox-2">
    <i class="fas fa-chevron-down">
    </i>
   </label>
-  <ul class="current">
-   <li class="toctree-l2 current active has-children">
-    <a class="reference internal" href="Aggregator.html">
-     Aggregator
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/creating_extractor.html">
+     Custom Extractor
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/config_file.html">
+     Extractor config file
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/utils.html">
+     Extraction utils
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="prog_guide/index.html">
+   Programming Guide
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
+  <label for="toctree-checkbox-3">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/overview.html">
+     Programming Guide
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/pip.html">
+     Custom Pipeline
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="misc/index.html">
+   Miscellaneous
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
+  <label for="toctree-checkbox-4">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="misc/domain_record.html">
+     Domain Record
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="api.html">
+   API
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
+  <label for="toctree-checkbox-5">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2 has-children">
+    <a class="reference internal" href="generated/cmoncrawl.html">
+     cmoncrawl
     </a>
-    <input checked="" class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
-    <label for="toctree-checkbox-3">
+    <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
+    <label for="toctree-checkbox-6">
      <i class="fas fa-chevron-down">
      </i>
     </label>
-    <ul class="current">
-     <li class="toctree-l3 current active has-children">
-      <a class="reference internal" href="Aggregator.App.html">
-       Aggregator.App
+    <ul>
+     <li class="toctree-l3 has-children">
+      <a class="reference internal" href="generated/cmoncrawl.aggregator.html">
+       cmoncrawl.aggregator
       </a>
-      <input checked="" class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
-      <label for="toctree-checkbox-4">
+      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
+      <label for="toctree-checkbox-7">
        <i class="fas fa-chevron-down">
        </i>
       </label>
-      <ul class="current">
-       <li class="toctree-l4 current active">
-        <a class="reference internal" href="Aggregator.App.index_query.html">
-         Aggregator.App.index_query
-        </a>
-       </li>
+      <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.ndjson_decoder.html">
-         Aggregator.App.ndjson_decoder
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.index_query.html">
+         cmoncrawl.aggregator.index_query
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.utils.html">
-         Aggregator.App.utils
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.utils.html">
+         cmoncrawl.aggregator.utils
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="Aggregator.aggregator.html">
-       Aggregator.aggregator
-      </a>
-     </li>
-    </ul>
-   </li>
-   <li class="toctree-l2 has-children">
-    <a class="reference internal" href="Processor.html">
-     Processor
-    </a>
-    <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
-    <label for="toctree-checkbox-5">
-     <i class="fas fa-chevron-down">
-     </i>
-    </label>
-    <ul>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="Processor.App.html">
-       Processor.App
+      <a class="reference internal" href="generated/cmoncrawl.common.html">
+       cmoncrawl.common
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
-      <label for="toctree-checkbox-6">
+      <input class="toctree-checkbox" id="toctree-checkbox-8" name="toctree-checkbox-8" type="checkbox"/>
+      <label for="toctree-checkbox-8">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Downloader.html">
-         Processor.App.Downloader
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Extractor.html">
-         Processor.App.Extractor
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.OutStreamer.html">
-         Processor.App.OutStreamer
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Pipeline.html">
-         Processor.App.Pipeline
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Router.html">
-         Processor.App.Router
+        <a class="reference internal" href="generated/cmoncrawl.common.loggers.html">
+         cmoncrawl.common.loggers
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.processor_utils.html">
-         Processor.App.processor_utils
+        <a class="reference internal" href="generated/cmoncrawl.common.types.html">
+         cmoncrawl.common.types
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="Processor.process_article.html">
-       Processor.process_article
-      </a>
-     </li>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="Processor.processor.html">
-       Processor.processor
+      <a class="reference internal" href="generated/cmoncrawl.processor.html">
+       cmoncrawl.processor
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
-      <label for="toctree-checkbox-7">
+      <input class="toctree-checkbox" id="toctree-checkbox-9" name="toctree-checkbox-9" type="checkbox"/>
+      <label for="toctree-checkbox-9">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.Listener.html">
-         Processor.processor.Listener
+        <a class="reference internal" href="generated/cmoncrawl.processor.extraction.html">
+         cmoncrawl.processor.extraction
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.ListnerStats.html">
-         Processor.processor.ListnerStats
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.Message.html">
-         Processor.processor.Message
+        <a class="reference internal" href="generated/cmoncrawl.processor.pipeline.html">
+         cmoncrawl.processor.pipeline
         </a>
        </li>
       </ul>
      </li>
     </ul>
    </li>
   </ul>
@@ -318,159 +342,154 @@
 
 <span class="headerbtn__icon-container">
   <i class="fas fa-expand"></i>
   </span>
 
 </button>
 
-<div class="menu-dropdown menu-dropdown-download-buttons">
-  <button class="headerbtn menu-dropdown__trigger"
-      aria-label="Download this page">
-      <i class="fas fa-download"></i>
-  </button>
-  <div class="menu-dropdown__content">
-    <ul>
-      <li>
-        <a href="../_sources/generated/Aggregator.App.index_query.DomainCrawl.__init__.rst.txt"
-   class="headerbtn"
-   data-toggle="tooltip"
-data-placement="left"
-title="Download source file"
->
-  
-
-<span class="headerbtn__icon-container">
-  <i class="fas fa-file"></i>
-  </span>
-<span class="headerbtn__text-container">.rst</span>
-</a>
-
-      </li>
-      
-      <li>
-        
-<button onclick="printPdf(this)"
-  class="headerbtn"
-  data-toggle="tooltip"
-data-placement="left"
-title="Print to PDF"
->
-  
-
-<span class="headerbtn__icon-container">
-  <i class="fas fa-file-pdf"></i>
-  </span>
-<span class="headerbtn__text-container">.pdf</span>
-</button>
-
-      </li>
-      
-    </ul>
-  </div>
-</div>
-<label for="__page-toc"
-  class="headerbtn headerbtn-page-toc"
-  
->
-  
-
-<span class="headerbtn__icon-container">
-  <i class="fas fa-list"></i>
-  </span>
-
-</label>
-
     </div>
 </div>
 
 <!-- Table of contents -->
 <div class="col-md-3 bd-toc show noprint">
-    <div class="tocsection onthispage pt-5 pb-3">
-        <i class="fas fa-list"></i> Contents
-    </div>
-    <nav id="bd-toc-nav" aria-label="Page">
-        <ul class="visible nav section-nav flex-column">
- <li class="toc-h2 nav-item toc-entry">
-  <a class="reference internal nav-link" href="#Aggregator.App.index_query.DomainCrawl.__init__">
-   <code class="docutils literal notranslate">
-    <span class="pre">
-     DomainCrawl.__init__()
-    </span>
-   </code>
-  </a>
- </li>
-</ul>
-
-    </nav>
 </div>
     </div>
     <div class="article row">
         <div class="col pl-md-3 pl-lg-5 content-container">
             <!-- Table of contents that is only displayed when printing the page -->
             <div id="jb-print-docs-body" class="onlyprint">
-                <h1>Aggregator.App.index_query.DomainCrawl.__init__</h1>
+                <h1></h1>
                 <!-- Table of contents -->
                 <div id="print-main-content">
                     <div id="jb-print-toc">
                         
-                        <div>
-                            <h2> Contents </h2>
-                        </div>
-                        <nav aria-label="Page">
-                            <ul class="visible nav section-nav flex-column">
- <li class="toc-h2 nav-item toc-entry">
-  <a class="reference internal nav-link" href="#Aggregator.App.index_query.DomainCrawl.__init__">
-   <code class="docutils literal notranslate">
-    <span class="pre">
-     DomainCrawl.__init__()
-    </span>
-   </code>
-  </a>
- </li>
-</ul>
-
-                        </nav>
                     </div>
                 </div>
             </div>
             <main id="main-content" role="main">
                 
               <div>
                 
-  <section id="aggregator-app-index-query-domaincrawl-init">
-<h1>Aggregator.App.index_query.DomainCrawl.__init__<a class="headerlink" href="#aggregator-app-index-query-domaincrawl-init" title="Permalink to this heading">#</a></h1>
-<dl class="py method">
-<dt class="sig sig-object py" id="Aggregator.App.index_query.DomainCrawl.__init__">
-<span class="sig-prename descclassname"><span class="pre">DomainCrawl.</span></span><span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">domain</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">''</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cdx_server</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">''</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">page</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#Aggregator.App.index_query.DomainCrawl.__init__" title="Permalink to this definition">#</a></dt>
-<dd></dd></dl>
 
-</section>
+   <h1>Python Module Index</h1>
+
+   <div class="modindex-jumpbox">
+   <a href="#cap-c"><strong>c</strong></a>
+   </div>
+
+   <table class="indextable modindextable">
+     <tr class="pcap"><td></td><td>&#160;</td><td></td></tr>
+     <tr class="cap" id="cap-c"><td></td><td>
+       <strong>c</strong></td><td></td></tr>
+     <tr>
+       <td><img src="_static/minus.png" class="toggler"
+              id="toggle-1" style="display: none" alt="-" /></td>
+       <td>
+       <a href="generated/cmoncrawl.html#module-cmoncrawl"><code class="xref">cmoncrawl</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.aggregator.html#module-cmoncrawl.aggregator"><code class="xref">cmoncrawl.aggregator</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.aggregator.index_query.html#module-cmoncrawl.aggregator.index_query"><code class="xref">cmoncrawl.aggregator.index_query</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.aggregator.utils.html#module-cmoncrawl.aggregator.utils"><code class="xref">cmoncrawl.aggregator.utils</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.aggregator.utils.helpers.html#module-cmoncrawl.aggregator.utils.helpers"><code class="xref">cmoncrawl.aggregator.utils.helpers</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.aggregator.utils.ndjson_decoder.html#module-cmoncrawl.aggregator.utils.ndjson_decoder"><code class="xref">cmoncrawl.aggregator.utils.ndjson_decoder</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.common.html#module-cmoncrawl.common"><code class="xref">cmoncrawl.common</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.common.loggers.html#module-cmoncrawl.common.loggers"><code class="xref">cmoncrawl.common.loggers</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.common.types.html#module-cmoncrawl.common.types"><code class="xref">cmoncrawl.common.types</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.html#module-cmoncrawl.processor"><code class="xref">cmoncrawl.processor</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.extraction.html#module-cmoncrawl.processor.extraction"><code class="xref">cmoncrawl.processor.extraction</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.extraction.filters.html#module-cmoncrawl.processor.extraction.filters"><code class="xref">cmoncrawl.processor.extraction.filters</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.extraction.utils.html#module-cmoncrawl.processor.extraction.utils"><code class="xref">cmoncrawl.processor.extraction.utils</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.pipeline.html#module-cmoncrawl.processor.pipeline"><code class="xref">cmoncrawl.processor.pipeline</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.pipeline.downloader.html#module-cmoncrawl.processor.pipeline.downloader"><code class="xref">cmoncrawl.processor.pipeline.downloader</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.pipeline.extractor.html#module-cmoncrawl.processor.pipeline.extractor"><code class="xref">cmoncrawl.processor.pipeline.extractor</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.pipeline.pipeline.html#module-cmoncrawl.processor.pipeline.pipeline"><code class="xref">cmoncrawl.processor.pipeline.pipeline</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.pipeline.router.html#module-cmoncrawl.processor.pipeline.router"><code class="xref">cmoncrawl.processor.pipeline.router</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="generated/cmoncrawl.processor.pipeline.streamer.html#module-cmoncrawl.processor.pipeline.streamer"><code class="xref">cmoncrawl.processor.pipeline.streamer</code></a></td><td>
+       <em></em></td></tr>
+   </table>
 
 
               </div>
               
             </main>
             <footer class="footer-article noprint">
                 
     <!-- Previous / next buttons -->
 <div class='prev-next-area'>
-    <a class='left-prev' id="prev-link" href="Aggregator.App.index_query.DomainCrawl.html" title="previous page">
-        <i class="fas fa-angle-left"></i>
-        <div class="prev-next-info">
-            <p class="prev-next-subtitle">previous</p>
-            <p class="prev-next-title">Aggregator.App.index_query.DomainCrawl</p>
-        </div>
-    </a>
-    <a class='right-next' id="next-link" href="Aggregator.App.index_query.DomainRecord.html" title="next page">
-    <div class="prev-next-info">
-        <p class="prev-next-subtitle">next</p>
-        <p class="prev-next-title">Aggregator.App.index_query.DomainRecord</p>
-    </div>
-    <i class="fas fa-angle-right"></i>
-    </a>
 </div>
             </footer>
         </div>
     </div>
     <div class="footer-content row">
         <footer class="col footer"><p>
   
@@ -484,12 +503,12 @@
 </div>
 
 
       </div>
     </div>
   
   <!-- Scripts loaded after <body> so the DOM is not blocked -->
-  <script src="../_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf"></script>
+  <script src="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf"></script>
 
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -10,63 +10,69 @@
 
 
 
 
 
 
 
-
-
  ⁰
 Toggle navigation sidebar
   ⁰
 Toggle in-page Table of Contents
 
-******_CommonCrawl_Extractor_1.0_documentation_******
+******_CmonCrawl_0.9.3_documentation_******
  [Unknown INPUT type]
  Contents:
-    * Quick_Start_Guide ⁰
-          o Quick_Overview
-          o Quickstart
-    * API *
-          o Aggregator *
-                # Aggregator.App *
-                      # Aggregator.App.index_query
-                      # Aggregator.App.ndjson_decoder
-                      # Aggregator.App.utils
-                # Aggregator.aggregator
-          o Processor ⁰
-                # Processor.App ⁰
-                      # Processor.App.Downloader
-                      # Processor.App.Extractor
-                      # Processor.App.OutStreamer
-                      # Processor.App.Pipeline
-                      # Processor.App.Router
-                      # Processor.App.processor_utils
-                # Processor.process_article
-                # Processor.processor ⁰
-                      # Processor.processor.Listener
-                      # Processor.processor.ListnerStats
-                      # Processor.processor.Message
+    * Usage
+    * Command_Line_Interface ⁰
+          o Command_Line_Interface
+          o Command_Line_Download
+          o Command_line_Extract
+    * Extraction ⁰
+          o Custom_Extractor
+          o Extractor_config_file
+          o Extraction_utils
+    * Programming_Guide ⁰
+          o Programming_Guide
+          o Custom_Pipeline
+    * Miscellaneous ⁰
+          o Domain_Record
+    * API ⁰
+          o cmoncrawl ⁰
+                # cmoncrawl.aggregator ⁰
+                      # cmoncrawl.aggregator.index_query
+                      # cmoncrawl.aggregator.utils
+                # cmoncrawl.common ⁰
+                      # cmoncrawl.common.loggers
+                      # cmoncrawl.common.types
+                # cmoncrawl.processor ⁰
+                      # cmoncrawl.processor.extraction
+                      # cmoncrawl.processor.pipeline
 Theme by the Executable_Book_Project
 
 
+****** Python Module Index ******
+c
+     
+    c
+[-] cmoncrawl
+        cmoncrawl.aggregator
+        cmoncrawl.aggregator.index_query
+        cmoncrawl.aggregator.utils
+        cmoncrawl.aggregator.utils.helpers
+        cmoncrawl.aggregator.utils.ndjson_decoder
+        cmoncrawl.common
+        cmoncrawl.common.loggers
+        cmoncrawl.common.types
+        cmoncrawl.processor
+        cmoncrawl.processor.extraction
+        cmoncrawl.processor.extraction.filters
+        cmoncrawl.processor.extraction.utils
+        cmoncrawl.processor.pipeline
+        cmoncrawl.processor.pipeline.downloader
+        cmoncrawl.processor.pipeline.extractor
+        cmoncrawl.processor.pipeline.pipeline
+        cmoncrawl.processor.pipeline.router
+        cmoncrawl.processor.pipeline.streamer
 
-    *    .rst
-    *     .pdf
-
- Contents
-    * _DomainCrawl.__init__()_
-****** Aggregator.App.index_query.DomainCrawl.__init__ ******
-***** Contents *****
-    * _DomainCrawl.__init__()_
-****** Aggregator.App.index_query.DomainCrawl.__init__# ******
-  DomainCrawl.__init__(domain: str = '', cdx_server: str = '', page: int = 0)
-  &#x2192; None#
-
-previous
-Aggregator.App.index_query.DomainCrawl
-
-next
-Aggregator.App.index_query.DomainRecord
 By Hynek KydlÃ­Äek
 © Copyright 2022, Hynek KydlÃ­Äek.
```

### Comparing `CmonCrawl-0.9.3/docs/build/html/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.html` & `CmonCrawl-1.0.0/docs/build/html/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -2,49 +2,48 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Aggregator.App.ndjson_decoder.Decoder.__init__ &#8212; CommonCrawl Extractor 1.0 documentation</title>
+    <title>Welcome to CommonCrawl Extractor’s documentation! &#8212; CmonCrawl 0.9.3 documentation</title>
     
   <!-- Loaded before other Sphinx assets -->
-  <link href="../_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
-<link href="../_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
+  <link href="_static/styles/theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
+<link href="_static/styles/pydata-sphinx-theme.css?digest=1999514e3f237ded88cf" rel="stylesheet">
 
     
   <link rel="stylesheet"
-    href="../_static/vendor/fontawesome/5.13.0/css/all.min.css">
+    href="_static/vendor/fontawesome/5.13.0/css/all.min.css">
   <link rel="preload" as="font" type="font/woff2" crossorigin
-    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
+    href="_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
   <link rel="preload" as="font" type="font/woff2" crossorigin
-    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">
+    href="_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">
 
-    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" href="../_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
-    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" href="_static/styles/sphinx-book-theme.css?digest=5115cc725059bd94278eecd172e13a965bf8f5a9" type="text/css" />
+    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     
   <!-- Pre-loaded scripts that we'll load fully later -->
-  <link rel="preload" as="script" href="../_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
+  <link rel="preload" as="script" href="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf">
 
-    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
-    <script src="../_static/jquery.js"></script>
-    <script src="../_static/underscore.js"></script>
-    <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="../_static/doctools.js"></script>
-    <script src="../_static/sphinx_highlight.js"></script>
-    <script src="../_static/clipboard.min.js"></script>
-    <script src="../_static/copybutton.js"></script>
-    <script src="../_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
+    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/jquery.js"></script>
+    <script src="_static/underscore.js"></script>
+    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/clipboard.min.js"></script>
+    <script src="_static/copybutton.js"></script>
+    <script src="_static/scripts/sphinx-book-theme.js?digest=9c920249402e914e316237a7dbc6769907cce411"></script>
     <script crossorigin="anonymous" integrity="sha256-Ae2Vz/4ePdIu6ZyI/5ZGsYnb+m0JlOmKPjt6XZ9JJkA=" src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.3.4/require.min.js"></script>
-    <link rel="index" title="Index" href="../genindex.html" />
-    <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="Aggregator.App.ndjson_decoder.Decoder.decode" href="Aggregator.App.ndjson_decoder.Decoder.decode.html" />
-    <link rel="prev" title="Aggregator.App.ndjson_decoder.Decoder" href="Aggregator.App.ndjson_decoder.Decoder.html" />
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Usage" href="usage.html" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <meta name="docsearch:language" content="en">
     
 
     <!-- Google Analytics -->
     
   </head>
@@ -71,188 +70,212 @@
     <div class="container-xl">
       <div class="row">
           
 <!-- Sidebar -->
 <div class="bd-sidebar noprint" id="site-navigation">
     <div class="bd-sidebar__content">
         <div class="bd-sidebar__top"><div class="navbar-brand-box">
-    <a class="navbar-brand text-wrap" href="../index.html">
+    <a class="navbar-brand text-wrap" href="#">
       
       
       
-      <h1 class="site-logo" id="site-title">CommonCrawl Extractor 1.0 documentation</h1>
+      <h1 class="site-logo" id="site-title">CmonCrawl 0.9.3 documentation</h1>
       
     </a>
-</div><form class="bd-search d-flex align-items-center" action="../search.html" method="get">
+</div><form class="bd-search d-flex align-items-center" action="search.html" method="get">
   <i class="icon fas fa-search"></i>
   <input type="search" class="form-control" name="q" id="search-input" placeholder="Search the docs ..." aria-label="Search the docs ..." autocomplete="off" >
 </form><nav class="bd-links" id="bd-docs-nav" aria-label="Main">
     <div class="bd-toc-item active">
         <p aria-level="2" class="caption" role="heading">
  <span class="caption-text">
   Contents:
  </span>
 </p>
-<ul class="current nav bd-sidenav">
+<ul class="nav bd-sidenav">
+ <li class="toctree-l1">
+  <a class="reference internal" href="usage.html">
+   Usage
+  </a>
+ </li>
  <li class="toctree-l1 has-children">
-  <a class="reference internal" href="../quickstart/index.html">
-   Quick Start Guide
+  <a class="reference internal" href="cli/index.html">
+   Command Line Interface
   </a>
   <input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" type="checkbox"/>
   <label for="toctree-checkbox-1">
    <i class="fas fa-chevron-down">
    </i>
   </label>
   <ul>
    <li class="toctree-l2">
-    <a class="reference internal" href="../quickstart/overview.html">
-     Quick Overview
+    <a class="reference internal" href="cli/cli.html">
+     Command Line Interface
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="cli/download.html">
+     Command Line Download
     </a>
    </li>
    <li class="toctree-l2">
-    <a class="reference internal" href="../quickstart/quick-start.html">
-     Quickstart
+    <a class="reference internal" href="cli/extract.html">
+     Command line Extract
     </a>
    </li>
   </ul>
  </li>
- <li class="toctree-l1 current active has-children">
-  <a class="reference internal" href="../api.html">
-   API
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="extraction/index.html">
+   Extraction
   </a>
-  <input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
+  <input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/>
   <label for="toctree-checkbox-2">
    <i class="fas fa-chevron-down">
    </i>
   </label>
-  <ul class="current">
-   <li class="toctree-l2 current active has-children">
-    <a class="reference internal" href="Aggregator.html">
-     Aggregator
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/creating_extractor.html">
+     Custom Extractor
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/config_file.html">
+     Extractor config file
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="extraction/utils.html">
+     Extraction utils
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="prog_guide/index.html">
+   Programming Guide
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
+  <label for="toctree-checkbox-3">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/overview.html">
+     Programming Guide
+    </a>
+   </li>
+   <li class="toctree-l2">
+    <a class="reference internal" href="prog_guide/pip.html">
+     Custom Pipeline
     </a>
-    <input checked="" class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/>
-    <label for="toctree-checkbox-3">
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="misc/index.html">
+   Miscellaneous
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
+  <label for="toctree-checkbox-4">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2">
+    <a class="reference internal" href="misc/domain_record.html">
+     Domain Record
+    </a>
+   </li>
+  </ul>
+ </li>
+ <li class="toctree-l1 has-children">
+  <a class="reference internal" href="api.html">
+   API
+  </a>
+  <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
+  <label for="toctree-checkbox-5">
+   <i class="fas fa-chevron-down">
+   </i>
+  </label>
+  <ul>
+   <li class="toctree-l2 has-children">
+    <a class="reference internal" href="generated/cmoncrawl.html">
+     cmoncrawl
+    </a>
+    <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
+    <label for="toctree-checkbox-6">
      <i class="fas fa-chevron-down">
      </i>
     </label>
-    <ul class="current">
-     <li class="toctree-l3 current active has-children">
-      <a class="reference internal" href="Aggregator.App.html">
-       Aggregator.App
+    <ul>
+     <li class="toctree-l3 has-children">
+      <a class="reference internal" href="generated/cmoncrawl.aggregator.html">
+       cmoncrawl.aggregator
       </a>
-      <input checked="" class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/>
-      <label for="toctree-checkbox-4">
+      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
+      <label for="toctree-checkbox-7">
        <i class="fas fa-chevron-down">
        </i>
       </label>
-      <ul class="current">
+      <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.index_query.html">
-         Aggregator.App.index_query
-        </a>
-       </li>
-       <li class="toctree-l4 current active">
-        <a class="reference internal" href="Aggregator.App.ndjson_decoder.html">
-         Aggregator.App.ndjson_decoder
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.index_query.html">
+         cmoncrawl.aggregator.index_query
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Aggregator.App.utils.html">
-         Aggregator.App.utils
+        <a class="reference internal" href="generated/cmoncrawl.aggregator.utils.html">
+         cmoncrawl.aggregator.utils
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="Aggregator.aggregator.html">
-       Aggregator.aggregator
-      </a>
-     </li>
-    </ul>
-   </li>
-   <li class="toctree-l2 has-children">
-    <a class="reference internal" href="Processor.html">
-     Processor
-    </a>
-    <input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/>
-    <label for="toctree-checkbox-5">
-     <i class="fas fa-chevron-down">
-     </i>
-    </label>
-    <ul>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="Processor.App.html">
-       Processor.App
+      <a class="reference internal" href="generated/cmoncrawl.common.html">
+       cmoncrawl.common
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/>
-      <label for="toctree-checkbox-6">
+      <input class="toctree-checkbox" id="toctree-checkbox-8" name="toctree-checkbox-8" type="checkbox"/>
+      <label for="toctree-checkbox-8">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Downloader.html">
-         Processor.App.Downloader
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Extractor.html">
-         Processor.App.Extractor
+        <a class="reference internal" href="generated/cmoncrawl.common.loggers.html">
+         cmoncrawl.common.loggers
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.OutStreamer.html">
-         Processor.App.OutStreamer
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Pipeline.html">
-         Processor.App.Pipeline
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.Router.html">
-         Processor.App.Router
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.App.processor_utils.html">
-         Processor.App.processor_utils
+        <a class="reference internal" href="generated/cmoncrawl.common.types.html">
+         cmoncrawl.common.types
         </a>
        </li>
       </ul>
      </li>
-     <li class="toctree-l3">
-      <a class="reference internal" href="Processor.process_article.html">
-       Processor.process_article
-      </a>
-     </li>
      <li class="toctree-l3 has-children">
-      <a class="reference internal" href="Processor.processor.html">
-       Processor.processor
+      <a class="reference internal" href="generated/cmoncrawl.processor.html">
+       cmoncrawl.processor
       </a>
-      <input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/>
-      <label for="toctree-checkbox-7">
+      <input class="toctree-checkbox" id="toctree-checkbox-9" name="toctree-checkbox-9" type="checkbox"/>
+      <label for="toctree-checkbox-9">
        <i class="fas fa-chevron-down">
        </i>
       </label>
       <ul>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.Listener.html">
-         Processor.processor.Listener
+        <a class="reference internal" href="generated/cmoncrawl.processor.extraction.html">
+         cmoncrawl.processor.extraction
         </a>
        </li>
        <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.ListnerStats.html">
-         Processor.processor.ListnerStats
-        </a>
-       </li>
-       <li class="toctree-l4">
-        <a class="reference internal" href="Processor.processor.Message.html">
-         Processor.processor.Message
+        <a class="reference internal" href="generated/cmoncrawl.processor.pipeline.html">
+         cmoncrawl.processor.pipeline
         </a>
        </li>
       </ul>
      </li>
     </ul>
    </li>
   </ul>
@@ -326,15 +349,15 @@
   <button class="headerbtn menu-dropdown__trigger"
       aria-label="Download this page">
       <i class="fas fa-download"></i>
   </button>
   <div class="menu-dropdown__content">
     <ul>
       <li>
-        <a href="../_sources/generated/Aggregator.App.ndjson_decoder.Decoder.__init__.rst.txt"
+        <a href="_sources/index.rst.txt"
    class="headerbtn"
    data-toggle="tooltip"
 data-placement="left"
 title="Download source file"
 >
   
 
@@ -385,115 +408,172 @@
 <!-- Table of contents -->
 <div class="col-md-3 bd-toc show noprint">
     <div class="tocsection onthispage pt-5 pb-3">
         <i class="fas fa-list"></i> Contents
     </div>
     <nav id="bd-toc-nav" aria-label="Page">
         <ul class="visible nav section-nav flex-column">
- <li class="toc-h2 nav-item toc-entry">
-  <a class="reference internal nav-link" href="#Aggregator.App.ndjson_decoder.Decoder.__init__">
-   <code class="docutils literal notranslate">
-    <span class="pre">
-     Decoder.__init__()
-    </span>
-   </code>
+ <li class="toc-h1 nav-item toc-entry">
+  <a class="reference internal nav-link" href="#">
+   Welcome to CommonCrawl Extractor’s documentation!
+  </a>
+ </li>
+ <li class="toc-h1 nav-item toc-entry">
+  <a class="reference internal nav-link" href="#indices-and-tables">
+   Indices and tables
   </a>
  </li>
 </ul>
 
     </nav>
 </div>
     </div>
     <div class="article row">
         <div class="col pl-md-3 pl-lg-5 content-container">
             <!-- Table of contents that is only displayed when printing the page -->
             <div id="jb-print-docs-body" class="onlyprint">
-                <h1>Aggregator.App.ndjson_decoder.Decoder.__init__</h1>
+                <h1>Welcome to CommonCrawl Extractor’s documentation!</h1>
                 <!-- Table of contents -->
                 <div id="print-main-content">
                     <div id="jb-print-toc">
                         
                         <div>
                             <h2> Contents </h2>
                         </div>
                         <nav aria-label="Page">
                             <ul class="visible nav section-nav flex-column">
- <li class="toc-h2 nav-item toc-entry">
-  <a class="reference internal nav-link" href="#Aggregator.App.ndjson_decoder.Decoder.__init__">
-   <code class="docutils literal notranslate">
-    <span class="pre">
-     Decoder.__init__()
-    </span>
-   </code>
+ <li class="toc-h1 nav-item toc-entry">
+  <a class="reference internal nav-link" href="#">
+   Welcome to CommonCrawl Extractor’s documentation!
+  </a>
+ </li>
+ <li class="toc-h1 nav-item toc-entry">
+  <a class="reference internal nav-link" href="#indices-and-tables">
+   Indices and tables
   </a>
  </li>
 </ul>
 
                         </nav>
                     </div>
                 </div>
             </div>
             <main id="main-content" role="main">
                 
               <div>
                 
-  <section id="aggregator-app-ndjson-decoder-decoder-init">
-<h1>Aggregator.App.ndjson_decoder.Decoder.__init__<a class="headerlink" href="#aggregator-app-ndjson-decoder-decoder-init" title="Permalink to this heading">#</a></h1>
-<dl class="py method">
-<dt class="sig sig-object py" id="Aggregator.App.ndjson_decoder.Decoder.__init__">
-<span class="sig-prename descclassname"><span class="pre">Decoder.</span></span><span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">object_hook</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parse_float</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parse_int</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parse_constant</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">strict</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">object_pairs_hook</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#Aggregator.App.ndjson_decoder.Decoder.__init__" title="Permalink to this definition">#</a></dt>
-<dd><p><code class="docutils literal notranslate"><span class="pre">object_hook</span></code>, if specified, will be called with the result
-of every JSON object decoded and its return value will be used in
-place of the given <code class="docutils literal notranslate"><span class="pre">dict</span></code>.  This can be used to provide custom
-deserializations (e.g. to support JSON-RPC class hinting).</p>
-<p><code class="docutils literal notranslate"><span class="pre">object_pairs_hook</span></code>, if specified will be called with the result of
-every JSON object decoded with an ordered list of pairs.  The return
-value of <code class="docutils literal notranslate"><span class="pre">object_pairs_hook</span></code> will be used instead of the <code class="docutils literal notranslate"><span class="pre">dict</span></code>.
-This feature can be used to implement custom decoders.
-If <code class="docutils literal notranslate"><span class="pre">object_hook</span></code> is also defined, the <code class="docutils literal notranslate"><span class="pre">object_pairs_hook</span></code> takes
-priority.</p>
-<p><code class="docutils literal notranslate"><span class="pre">parse_float</span></code>, if specified, will be called with the string
-of every JSON float to be decoded. By default this is equivalent to
-float(num_str). This can be used to use another datatype or parser
-for JSON floats (e.g. decimal.Decimal).</p>
-<p><code class="docutils literal notranslate"><span class="pre">parse_int</span></code>, if specified, will be called with the string
-of every JSON int to be decoded. By default this is equivalent to
-int(num_str). This can be used to use another datatype or parser
-for JSON integers (e.g. float).</p>
-<p><code class="docutils literal notranslate"><span class="pre">parse_constant</span></code>, if specified, will be called with one of the
-following strings: -Infinity, Infinity, NaN.
-This can be used to raise an exception if invalid JSON numbers
-are encountered.</p>
-<p>If <code class="docutils literal notranslate"><span class="pre">strict</span></code> is false (true is the default), then control
-characters will be allowed inside strings.  Control characters in
-this context are those with character codes in the 0-31 range,
-including <code class="docutils literal notranslate"><span class="pre">'\t'</span></code> (tab), <code class="docutils literal notranslate"><span class="pre">'\n'</span></code>, <code class="docutils literal notranslate"><span class="pre">'\r'</span></code> and <code class="docutils literal notranslate"><span class="pre">'\0'</span></code>.</p>
-</dd></dl>
-
+  <section id="welcome-to-commoncrawl-extractor-s-documentation">
+<h1>Welcome to CommonCrawl Extractor’s documentation!<a class="headerlink" href="#welcome-to-commoncrawl-extractor-s-documentation" title="Permalink to this heading">#</a></h1>
+<div class="toctree-wrapper compound">
+<p aria-level="2" class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="usage.html#workflow">Workflow</a></li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="cli/index.html">Command Line Interface</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="cli/cli.html">Command Line Interface</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="cli/cli.html#examples">Examples</a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="cli/download.html">Command Line Download</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="cli/download.html#positional-arguments">Positional arguments</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/download.html#options">Options</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/download.html#record-mode-options">Record mode options</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/download.html#examples">Examples</a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="cli/extract.html">Command line Extract</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="cli/extract.html#positional-arguments">Positional arguments</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/extract.html#optional-arguments">Optional arguments</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/extract.html#record-arguments">Record arguments</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/extract.html#html-arguments">Html arguments</a></li>
+<li class="toctree-l3"><a class="reference internal" href="cli/extract.html#examples">Examples</a></li>
+</ul>
+</li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="extraction/index.html">Extraction</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="extraction/creating_extractor.html">Custom Extractor</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="extraction/creating_extractor.html#baseextractor">BaseExtractor</a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/creating_extractor.html#extraction">Extraction</a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/creating_extractor.html#filtering">Filtering</a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/creating_extractor.html#example">Example</a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="extraction/config_file.html">Extractor config file</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="extraction/config_file.html#structure">Structure</a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/config_file.html#example">Example</a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/config_file.html#init-py"><cite>__init__.py</cite></a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/config_file.html#arbitrary-code-execution">Arbitrary Code Execution</a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="extraction/utils.html">Extraction utils</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="extraction/utils.html#filtering">Filtering</a></li>
+<li class="toctree-l3"><a class="reference internal" href="extraction/utils.html#extraction">Extraction</a></li>
+</ul>
+</li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="prog_guide/index.html">Programming Guide</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="prog_guide/overview.html">Programming Guide</a></li>
+<li class="toctree-l2"><a class="reference internal" href="prog_guide/overview.html#how-to-extract-from-common-crawl-theory">How to extract from Common Crawl (theory)</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/overview.html#querying-commoncrawl">1. Querying CommonCrawl</a></li>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/overview.html#downloading-a-file">2. Downloading a file</a></li>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/overview.html#choose-extractor">3. Choose extractor</a></li>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/overview.html#filtering-out-the-web-page">4. Filtering out the web page</a></li>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/overview.html#extract-fields-from-the-page">5. Extract fields from the page</a></li>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/overview.html#file-saving">6. File saving</a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="prog_guide/pip.html">Custom Pipeline</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/pip.html#pipeline">Pipeline</a></li>
+<li class="toctree-l3"><a class="reference internal" href="prog_guide/pip.html#putting-it-all-together">Putting it all together</a></li>
+</ul>
+</li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="misc/index.html">Miscellaneous</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="misc/domain_record.html">Domain Record</a></li>
+<li class="toctree-l2"><a class="reference internal" href="misc/domain_record.html#domain-record-jsonl-format">Domain Record JSONL format</a></li>
+</ul>
+</li>
+<li class="toctree-l1"><a class="reference internal" href="api.html">API</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="generated/cmoncrawl.html">cmoncrawl</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="generated/cmoncrawl.aggregator.html">cmoncrawl.aggregator</a></li>
+<li class="toctree-l3"><a class="reference internal" href="generated/cmoncrawl.common.html">cmoncrawl.common</a></li>
+<li class="toctree-l3"><a class="reference internal" href="generated/cmoncrawl.processor.html">cmoncrawl.processor</a></li>
+</ul>
+</li>
+</ul>
+</li>
+</ul>
+</div>
+</section>
+<section id="indices-and-tables">
+<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading">#</a></h1>
+<ul class="simple">
+<li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
+<li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
+<li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
+</ul>
 </section>
 
 
               </div>
               
             </main>
             <footer class="footer-article noprint">
                 
     <!-- Previous / next buttons -->
 <div class='prev-next-area'>
-    <a class='left-prev' id="prev-link" href="Aggregator.App.ndjson_decoder.Decoder.html" title="previous page">
-        <i class="fas fa-angle-left"></i>
-        <div class="prev-next-info">
-            <p class="prev-next-subtitle">previous</p>
-            <p class="prev-next-title">Aggregator.App.ndjson_decoder.Decoder</p>
-        </div>
-    </a>
-    <a class='right-next' id="next-link" href="Aggregator.App.ndjson_decoder.Decoder.decode.html" title="next page">
+    <a class='right-next' id="next-link" href="usage.html" title="next page">
     <div class="prev-next-info">
         <p class="prev-next-subtitle">next</p>
-        <p class="prev-next-title">Aggregator.App.ndjson_decoder.Decoder.decode</p>
+        <p class="prev-next-title">Usage</p>
     </div>
     <i class="fas fa-angle-right"></i>
     </a>
 </div>
             </footer>
         </div>
     </div>
@@ -510,12 +590,12 @@
 </div>
 
 
       </div>
     </div>
   
   <!-- Scripts loaded after <body> so the DOM is not blocked -->
-  <script src="../_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf"></script>
+  <script src="_static/scripts/pydata-sphinx-theme.js?digest=1999514e3f237ded88cf"></script>
 
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -11,85 +11,116 @@
 
 
 
 
 
 
 
-
  ⁰
 Toggle navigation sidebar
   ⁰
 Toggle in-page Table of Contents
 
-******_CommonCrawl_Extractor_1.0_documentation_******
+******_CmonCrawl_0.9.3_documentation_******
  [Unknown INPUT type]
  Contents:
-    * Quick_Start_Guide ⁰
-          o Quick_Overview
-          o Quickstart
-    * API *
-          o Aggregator *
-                # Aggregator.App *
-                      # Aggregator.App.index_query
-                      # Aggregator.App.ndjson_decoder
-                      # Aggregator.App.utils
-                # Aggregator.aggregator
-          o Processor ⁰
-                # Processor.App ⁰
-                      # Processor.App.Downloader
-                      # Processor.App.Extractor
-                      # Processor.App.OutStreamer
-                      # Processor.App.Pipeline
-                      # Processor.App.Router
-                      # Processor.App.processor_utils
-                # Processor.process_article
-                # Processor.processor ⁰
-                      # Processor.processor.Listener
-                      # Processor.processor.ListnerStats
-                      # Processor.processor.Message
+    * Usage
+    * Command_Line_Interface ⁰
+          o Command_Line_Interface
+          o Command_Line_Download
+          o Command_line_Extract
+    * Extraction ⁰
+          o Custom_Extractor
+          o Extractor_config_file
+          o Extraction_utils
+    * Programming_Guide ⁰
+          o Programming_Guide
+          o Custom_Pipeline
+    * Miscellaneous ⁰
+          o Domain_Record
+    * API ⁰
+          o cmoncrawl ⁰
+                # cmoncrawl.aggregator ⁰
+                      # cmoncrawl.aggregator.index_query
+                      # cmoncrawl.aggregator.utils
+                # cmoncrawl.common ⁰
+                      # cmoncrawl.common.loggers
+                      # cmoncrawl.common.types
+                # cmoncrawl.processor ⁰
+                      # cmoncrawl.processor.extraction
+                      # cmoncrawl.processor.pipeline
 Theme by the Executable_Book_Project
 
 
 
     *    .rst
     *     .pdf
 
  Contents
-    * _Decoder.__init__()_
-****** Aggregator.App.ndjson_decoder.Decoder.__init__ ******
+    * Welcome_to_CommonCrawl_Extractorâs_documentation!
+    * Indices_and_tables
+****** Welcome to CommonCrawl Extractorâs documentation! ******
 ***** Contents *****
-    * _Decoder.__init__()_
-****** Aggregator.App.ndjson_decoder.Decoder.__init__# ******
-  Decoder.__init__(*, object_hook=None, parse_float=None, parse_int=None,
-  parse_constant=None, strict=True, object_pairs_hook=None)#
-      object_hook, if specified, will be called with the result of every JSON
-      object decoded and its return value will be used in place of the given
-      dict. This can be used to provide custom deserializations (e.g. to
-      support JSON-RPC class hinting).
-      object_pairs_hook, if specified will be called with the result of every
-      JSON object decoded with an ordered list of pairs. The return value of
-      object_pairs_hook will be used instead of the dict. This feature can be
-      used to implement custom decoders. If object_hook is also defined, the
-      object_pairs_hook takes priority.
-      parse_float, if specified, will be called with the string of every JSON
-      float to be decoded. By default this is equivalent to float(num_str).
-      This can be used to use another datatype or parser for JSON floats (e.g.
-      decimal.Decimal).
-      parse_int, if specified, will be called with the string of every JSON int
-      to be decoded. By default this is equivalent to int(num_str). This can be
-      used to use another datatype or parser for JSON integers (e.g. float).
-      parse_constant, if specified, will be called with one of the following
-      strings: -Infinity, Infinity, NaN. This can be used to raise an exception
-      if invalid JSON numbers are encountered.
-      If strict is false (true is the default), then control characters will be
-      allowed inside strings. Control characters in this context are those with
-      character codes in the 0-31 range, including '\t' (tab), '\n', '\r' and
-      '\0'.
-
-previous
-Aggregator.App.ndjson_decoder.Decoder
+    * Welcome_to_CommonCrawl_Extractorâs_documentation!
+    * Indices_and_tables
+****** Welcome to CommonCrawl Extractorâs documentation!# ******
+Contents:
+    * Usage
+          o Workflow
+    * Command_Line_Interface
+          o Command_Line_Interface
+                # Examples
+          o Command_Line_Download
+                # Positional_arguments
+                # Options
+                # Record_mode_options
+                # Examples
+          o Command_line_Extract
+                # Positional_arguments
+                # Optional_arguments
+                # Record_arguments
+                # Html_arguments
+                # Examples
+    * Extraction
+          o Custom_Extractor
+                # BaseExtractor
+                # Extraction
+                # Filtering
+                # Example
+          o Extractor_config_file
+                # Structure
+                # Example
+                # __init__.py
+                # Arbitrary_Code_Execution
+          o Extraction_utils
+                # Filtering
+                # Extraction
+    * Programming_Guide
+          o Programming_Guide
+          o How_to_extract_from_Common_Crawl_(theory)
+                # 1._Querying_CommonCrawl
+                # 2._Downloading_a_file
+                # 3._Choose_extractor
+                # 4._Filtering_out_the_web_page
+                # 5._Extract_fields_from_the_page
+                # 6._File_saving
+          o Custom_Pipeline
+                # Pipeline
+                # Putting_it_all_together
+    * Miscellaneous
+          o Domain_Record
+          o Domain_Record_JSONL_format
+    * API
+          o cmoncrawl
+                # cmoncrawl.aggregator
+                # cmoncrawl.common
+                # cmoncrawl.processor
+
+****** Indices and tables# ******
+    * Index
+    * Module_Index
+    * Search_Page
 
 next
-Aggregator.App.ndjson_decoder.Decoder.decode
+Usage
 By Hynek KydlÃ­Äek
 © Copyright 2022, Hynek KydlÃ­Äek.
```

### Comparing `CmonCrawl-0.9.3/docs/make.bat` & `CmonCrawl-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/docs/source/conf.py` & `CmonCrawl-1.0.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
-project = "CommonCrawl Extractor"
+project = "CmonCrawl"
 copyright = "2022, Hynek Kydlíček"
 author = "Hynek Kydlíček"
 
 # The full version, including alpha/beta/rc tags
-release = "1.0"
+release = "0.9.3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `CmonCrawl-0.9.3/docs/source/index.rst` & `CmonCrawl-1.0.0/docs/source/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 Welcome to CommonCrawl Extractor's documentation!
 =================================================
 
 .. toctree::
    :maxdepth: 3
    :caption: Contents:
 
-   installation
-   quickstart/index
+   usage
+   cli/index
+   extraction/index
+   prog_guide/index
+   misc/index
    api
 
 
 
-
-
-
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `CmonCrawl-0.9.3/examples/extractor_tutorial/Extractors/bbc_extractor.py` & `CmonCrawl-1.0.0/examples/extractor_tutorial/Extractors/bbc_extractor.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/pyproject.toml` & `CmonCrawl-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/tests/aggregator_tests.py` & `CmonCrawl-1.0.0/tests/aggregator_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 sys.path.append(Path("App").absolute().as_posix())
 
 from datetime import datetime
 from typing import List
 from cmoncrawl.aggregator.utils.helpers import unify_url_id
-from cmoncrawl.common.types import DomainRecord
+from cmoncrawl.common.types import DomainRecord, MatchType
 from cmoncrawl.aggregator.index_query import IndexAggregator
 import unittest
 
 
 from cmoncrawl.common.loggers import all_purpose_logger
 
 all_purpose_logger.setLevel(logging.DEBUG)
@@ -22,23 +22,29 @@
         self.CC_SERVERS = ["https://index.commoncrawl.org/CC-MAIN-2022-05-index"]
         self.di = await IndexAggregator(
             ["idnes.cz"],
             cc_servers=self.CC_SERVERS,
             max_retry=50,
             sleep_step=10,
             prefetch_size=1,
+            match_type=MatchType.DOMAIN,
         ).aopen()
         self.client = self.di.client
 
     async def asyncTearDown(self) -> None:
         await self.di.aclose(None, None, None)
 
     async def test_indexer_num_pages(self):
         response = await self.di.get_number_of_pages(
-            self.client, self.CC_SERVERS[0], "idnes.cz", max_retry=20, sleep_step=4
+            self.client,
+            self.CC_SERVERS[0],
+            "idnes.cz",
+            max_retry=20,
+            sleep_step=4,
+            match_type=MatchType.DOMAIN,
         )
         self.assertIsNotNone(response)
         num, size = response.content
         self.assertEqual(num, 14)
         self.assertEqual(size, 5)
 
     async def test_indexer_all_CC(self):
```

### Comparing `CmonCrawl-0.9.3/tests/end_to_end_tests.py` & `CmonCrawl-1.0.0/tests/end_to_end_tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import shutil
 from datetime import datetime
 import json
 from pathlib import Path
 import unittest
+from cmoncrawl.common.loggers import metadata_logger, all_purpose_logger
 from cmoncrawl.integrations.extract import extract_from_files, ExtractMode
 from cmoncrawl.common.types import ExtractConfig
 
 
 class Extract_from_files(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self) -> None:
+        all_purpose_logger.setLevel("DEBUG")
+        metadata_logger.setLevel("DEBUG")
         self.base_folder = Path(__file__).parent / "test_extract"
         self.output_folder = self.base_folder / "output"
 
     async def asyncTearDown(self) -> None:
         # remoev output folder
         if self.output_folder.exists():
             shutil.rmtree(self.output_folder)
@@ -29,15 +32,15 @@
         cfg_path = self.base_folder / "cfg.json"
         with open(cfg_path, "r") as f:
             js = json.load(f)
             cfg: ExtractConfig = ExtractConfig.schema(many=False).load(js)
         results = await extract_from_files(
             config=cfg,
             files=[self.base_folder / "files" / "file.jsonl"],
-            output_path=self.base_folder / "output",
+            output_path=self.output_folder,
             mode=ExtractMode.RECORD,
             date=datetime(2021, 1, 1),
             max_crawls_per_file=10,
             max_directory_size=1,
             url="",
             max_retry=1,
             sleep_step=1,
@@ -54,15 +57,15 @@
         cfg_path = self.base_folder / "cfg.json"
         with open(cfg_path, "r") as f:
             js = json.load(f)
             cfg: ExtractConfig = ExtractConfig.schema(many=False).load(js)
         results = await extract_from_files(
             config=cfg,
             files=[self.base_folder / "files" / "file.html"],
-            output_path=self.base_folder / "output",
+            output_path=self.output_folder,
             mode=ExtractMode.HTML,
             date=datetime(2021, 1, 1),
             max_crawls_per_file=1,
             max_directory_size=10,
             url="",
             max_retry=1,
             sleep_step=1,
```

### Comparing `CmonCrawl-0.9.3/tests/processor_tests.py` & `CmonCrawl-1.0.0/tests/processor_tests.py`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/tests/test_extract/files/file.html` & `CmonCrawl-1.0.0/tests/test_extract/files/file.html`

 * *Files identical despite different names*

### Comparing `CmonCrawl-0.9.3/tests/test_extract/files/file.jsonl` & `CmonCrawl-1.0.0/tests/test_extract/files/file.jsonl`

 * *Files identical despite different names*

