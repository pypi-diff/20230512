# Comparing `tmp/google-dataproc-templates-0.2.0b0.tar.gz` & `tmp/google-dataproc-templates-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-dataproc-templates-0.2.0b0.tar", last modified: Tue Apr 11 11:21:58 2023, max compression
+gzip compressed data, was "google-dataproc-templates-0.3.0b0.tar", last modified: Fri May 12 16:47:25 2023, max compression
```

## Comparing `google-dataproc-templates-0.2.0b0.tar` & `google-dataproc-templates-0.3.0b0.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/base_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_jdbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/text_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/hbase_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_bq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/mongo_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/redshift_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/s3/s3_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.666283 google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/template_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/dataproc_templates/util/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/dataframe_reader_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/dataframe_writer_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/template_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/dataproc_templates/util/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 11:21:58.000000 google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.662283 google-dataproc-templates-0.2.0b0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/azure/test_azure_blob_storage_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/bigquery/test_bigquery_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/cassandra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/cassandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_bq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/gcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigtable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_jdbc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/gcs/test_text_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/hbase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hbase/test_hbase_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/hive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/hive/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/hive/util/test_hive_ddl_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/jdbc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_jdbc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/mongo/test_mongo_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.670283 google-dataproc-templates-0.2.0b0/test/pubsublite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/pubsublite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/pubsublite/test_pubsublite_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/test/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/redshift/test_redshift_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/test/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/s3/test_s3_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:58.674283 google-dataproc-templates-0.2.0b0/test/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/test/util/test_argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 11:21:46.000000 google-dataproc-templates-0.2.0b0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/base_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/text_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/hbase_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/mongo_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/redshift_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/s3/s3_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/template_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_reader_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_writer_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/template_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.691218 google-dataproc-templates-0.3.0b0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/azure/test_azure_blob_storage_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/bigquery/test_bigquery_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_text_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/hbase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hbase/test_hbase_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/hive/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/util/test_hive_ddl_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/jdbc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_jdbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/mongo/test_mongo_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/pubsublite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/pubsublite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/redshift/test_redshift_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/s3/test_s3_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/util/test_argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/version.py
```

### Comparing `google-dataproc-templates-0.2.0b0/MANIFEST.in` & `google-dataproc-templates-0.3.0b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/PKG-INFO` & `google-dataproc-templates-0.3.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: google-dataproc-templates
-Version: 0.2.0b0
+Version: 0.3.0b0
 Summary: Google Dataproc templates written in Python
 Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ![Build Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job-python&&subject=python-build)
+![Python Integration Test Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fintegration-tests-python&&subject=python-integration-tests)
+
 
 # Dataproc Templates (Python - PySpark)
 * [AzureBlobStorageToBigQuery](/python/dataproc_templates/azure#azure-blob-storage-to-bigquery)
 * [BigQueryToGCS](/python/dataproc_templates/bigquery#bigquery-to-gcs) (blogpost [link](https://medium.com/google-cloud/moving-data-from-bigquery-to-gcs-using-gcp-dataproc-serverless-and-pyspark-f6481b86bcd1))
 * [CassandraToBigquery](/python/dataproc_templates/cassandra#cassandra-to-bigquery)
-* [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs)
+* [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs) (blogpost [link](https://medium.com/google-cloud/export-data-from-cassandra-to-google-cloud-storage-using-dataproc-serverless-2569a00e17fe))
 * [GCSToBigQuery](/python/dataproc_templates/gcs#gcs-to-bigquery) (blogpost [link](https://medium.com/@ppaglilla/getting-started-with-dataproc-serverless-pyspark-templates-e32278a6a06e))
 * [GCSToBigTable](/python/dataproc_templates/gcs#gcs-to-bigtable) (blogpost [link](https://medium.com/google-cloud/pyspark-load-data-from-gcs-to-bigtable-using-gcp-dataproc-serverless-c373430fe157))
 * [GCSToGCS](/python/dataproc_templates/gcs#gcs-to-gcs---sql-transformation)(blogpost [link](https://medium.com/@ankuljain/migrate-gcs-to-gcs-using-dataproc-serverless-3b7b0f6ad6b9))
 * [GCSToJDBC](/python/dataproc_templates/gcs#gcs-to-jdbc) (blogpost [link](https://medium.com/google-cloud/import-data-from-gcs-to-jdbc-databases-using-dataproc-serverless-c7154b242430))
 * [GCSToMongo](/python/dataproc_templates/gcs#gcs-to-mongodb) (blogpost [link](https://medium.com/google-cloud/importing-data-from-gcs-to-mongodb-using-dataproc-serverless-fed58904633a))
 * [HbaseToGCS](/python/dataproc_templates/hbase#hbase-to-gcs)
 * [HiveToBigQuery](/python/dataproc_templates/hive#hive-to-bigquery) (blogpost [link](https://medium.com/google-cloud/processing-data-from-hive-to-bigquery-using-pyspark-and-dataproc-serverless-217c7cb9e4f8))
 * [HiveToGCS](/python/dataproc_templates/hive#hive-to-gcs)(blogpost [link](https://medium.com/@surjitsh/processing-large-data-tables-from-hive-to-gcs-using-pyspark-and-dataproc-serverless-35d3d16daaf))
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
+* [PubSubLiteToBigtable](/python/dataproc_templates/pubsublite#pubsublite-to-bigtable)
 * [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
```

### Comparing `google-dataproc-templates-0.2.0b0/README.md` & `google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,41 @@
+Metadata-Version: 2.1
+Name: google-dataproc-templates
+Version: 0.3.0b0
+Summary: Google Dataproc templates written in Python
+Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
+License: Apache 2.0
+Platform: Posix; MacOS X; Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 ![Build Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job-python&&subject=python-build)
+![Python Integration Test Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fintegration-tests-python&&subject=python-integration-tests)
+
 
 # Dataproc Templates (Python - PySpark)
 * [AzureBlobStorageToBigQuery](/python/dataproc_templates/azure#azure-blob-storage-to-bigquery)
 * [BigQueryToGCS](/python/dataproc_templates/bigquery#bigquery-to-gcs) (blogpost [link](https://medium.com/google-cloud/moving-data-from-bigquery-to-gcs-using-gcp-dataproc-serverless-and-pyspark-f6481b86bcd1))
 * [CassandraToBigquery](/python/dataproc_templates/cassandra#cassandra-to-bigquery)
-* [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs)
+* [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs) (blogpost [link](https://medium.com/google-cloud/export-data-from-cassandra-to-google-cloud-storage-using-dataproc-serverless-2569a00e17fe))
 * [GCSToBigQuery](/python/dataproc_templates/gcs#gcs-to-bigquery) (blogpost [link](https://medium.com/@ppaglilla/getting-started-with-dataproc-serverless-pyspark-templates-e32278a6a06e))
 * [GCSToBigTable](/python/dataproc_templates/gcs#gcs-to-bigtable) (blogpost [link](https://medium.com/google-cloud/pyspark-load-data-from-gcs-to-bigtable-using-gcp-dataproc-serverless-c373430fe157))
 * [GCSToGCS](/python/dataproc_templates/gcs#gcs-to-gcs---sql-transformation)(blogpost [link](https://medium.com/@ankuljain/migrate-gcs-to-gcs-using-dataproc-serverless-3b7b0f6ad6b9))
 * [GCSToJDBC](/python/dataproc_templates/gcs#gcs-to-jdbc) (blogpost [link](https://medium.com/google-cloud/import-data-from-gcs-to-jdbc-databases-using-dataproc-serverless-c7154b242430))
 * [GCSToMongo](/python/dataproc_templates/gcs#gcs-to-mongodb) (blogpost [link](https://medium.com/google-cloud/importing-data-from-gcs-to-mongodb-using-dataproc-serverless-fed58904633a))
 * [HbaseToGCS](/python/dataproc_templates/hbase#hbase-to-gcs)
 * [HiveToBigQuery](/python/dataproc_templates/hive#hive-to-bigquery) (blogpost [link](https://medium.com/google-cloud/processing-data-from-hive-to-bigquery-using-pyspark-and-dataproc-serverless-217c7cb9e4f8))
 * [HiveToGCS](/python/dataproc_templates/hive#hive-to-gcs)(blogpost [link](https://medium.com/@surjitsh/processing-large-data-tables-from-hive-to-gcs-using-pyspark-and-dataproc-serverless-35d3d16daaf))
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
+* [PubSubLiteToBigtable](/python/dataproc_templates/pubsublite#pubsublite-to-bigtable)
 * [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/azure/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,17 @@
         output_mode: str = args[constants.AZ_BLOB_BQ_OUTPUT_MODE]
         storage_account: str = args[constants.AZ_BLOB_STORAGE_ACCOUNT]
         container_name: str = args[constants.AZ_BLOB_CONTAINER_NAME]
         sas_token: str = args[constants.AZ_BLOB_SAS_TOKEN]
 
         spark.conf.set(f"fs.azure.sas.{container_name}.{storage_account}.blob.core.windows.net", sas_token)
 
-        logger.info(f"Starting Azure to BigQuery spark job with parameters:\n {pprint.pformat(args)}")
+        ignore_keys = {constants.AZ_BLOB_SAS_TOKEN}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
+        logger.info(f"Starting Azure to BigQuery spark job with parameters:\n {pprint.pformat(filtered_args)}")
 
         # Read
         input_data: DataFrame
 
         if input_file_format == constants.FORMAT_PRQT:
             input_data = spark.read \
                 .parquet(input_file_location)
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/base_template.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/base_template.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_bigtable.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigtable.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_jdbc.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_jdbc.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,17 +120,19 @@
         jdbc_url: str = args[constants.GCS_JDBC_OUTPUT_URL]
         jdbc_table: str = args[constants.GCS_JDBC_OUTPUT_TABLE]
         output_mode: str = args[constants.GCS_JDBC_OUTPUT_MODE]
         output_driver: str = args[constants.GCS_JDBC_OUTPUT_DRIVER]
         batch_size: int = args[constants.GCS_JDBC_BATCH_SIZE]
         jdbc_numpartitions: int = args[constants.GCS_JDBC_NUMPARTITIONS]
 
+        ignore_keys = {constants.GCS_JDBC_OUTPUT_URL}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting Cloud Storage to JDBC Spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data = ingest_dataframe_from_cloud_storage(spark, args, input_location, input_format, "gcs.jdbc.input.")
 
         # Write
         if not jdbc_numpartitions:
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/gcs_to_mongo.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_mongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,17 +113,19 @@
         input_format: str = args[constants.GCS_MONGO_INPUT_FORMAT]
         output_uri:str = args[constants.GCS_MONGO_OUTPUT_URI]
         output_database:str = args[constants.GCS_MONGO_OUTPUT_DATABASE]
         output_collection:str = args[constants.GCS_MONGO_OUTPUT_COLLECTION]
         output_mode:str = args[constants.GCS_MONGO_OUTPUT_MODE]
         batch_size:int = args[constants.GCS_MONGO_BATCH_SIZE]
 
+        ignore_keys = {constants.GCS_MONGO_OUTPUT_URI}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting GCS to MONGO spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data = ingest_dataframe_from_cloud_storage(spark, args, input_location, input_format, "gcs.mongo.input.")
 
         # Write
         input_data.write.format(constants.FORMAT_MONGO)\
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/gcs/text_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/text_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/hbase/hbase_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/hbase_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/hive_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,17 +151,19 @@
         input_jdbc_lowerbound: str = args[constants.JDBC_BQ_INPUT_LOWERBOUND]
         input_jdbc_upperbound: str = args[constants.JDBC_BQ_INPUT_UPPERBOUND]
         jdbc_numpartitions: str = args[constants.JDBC_BQ_NUMPARTITIONS]
         input_jdbc_fetchsize: int = args[constants.JDBC_BQ_INPUT_FETCHSIZE]
         input_jdbc_sessioninitstatement: str = args[constants.JDBC_BQ_SESSIONINITSTATEMENT]
         output_mode: str = args[constants.JDBC_BQ_OUTPUT_MODE]
 
+        ignore_keys = {constants.JDBC_BQ_INPUT_URL}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting JDBC to BigQuery Spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data: DataFrame
 
         partition_parameters = str(input_jdbc_partitioncolumn) + str(input_jdbc_lowerbound) + str(input_jdbc_upperbound)
         if ((partition_parameters != "") & ((input_jdbc_partitioncolumn == "") | (input_jdbc_lowerbound == "") | (input_jdbc_upperbound == ""))):
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,17 +191,19 @@
         output_location: str = args[constants.JDBCTOGCS_OUTPUT_LOCATION]
         output_format: str = args[constants.JDBCTOGCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.JDBCTOGCS_OUTPUT_MODE]
         output_partitioncolumn: str = args[constants.JDBCTOGCS_OUTPUT_PARTITIONCOLUMN]
         temp_view: str = args[constants.JDBCTOGCS_TEMP_VIEW_NAME]
         temp_sql_query:str = args[constants.JDBCTOGCS_TEMP_SQL_QUERY]
 
+        ignore_keys = {constants.JDBCTOGCS_INPUT_URL}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting JDBC to Cloud Storage Spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data: DataFrame
 
         read_properties = {constants.JDBC_URL: input_jdbc_url,
                            constants.JDBC_DRIVER: input_jdbc_driver}
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,19 @@
         output_jdbc_table: str = args[constants.JDBCTOJDBC_OUTPUT_TABLE]
         output_jdbc_create_table_option: str = args[constants.JDBCTOJDBC_OUTPUT_CREATE_TABLE_OPTION]
         output_jdbc_mode: str = args[constants.JDBCTOJDBC_OUTPUT_MODE]
         output_jdbc_batch_size: int = args[constants.JDBCTOJDBC_OUTPUT_BATCH_SIZE]
         temp_view: str = args[constants.JDBCTOGCS_TEMP_VIEW_NAME]
         sql_query: str = args[constants.JDBCTOJDBC_SQL_QUERY]
 
+        ignore_keys = {constants.JDBCTOJDBC_INPUT_URL, constants.JDBCTOJDBC_OUTPUT_URL}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting JDBC to JDBC spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data: DataFrame
 
         partition_parameters = str(input_jdbc_partitioncolumn) + str(input_jdbc_lowerbound) + str(input_jdbc_upperbound)
         if ((partition_parameters != "") & ((input_jdbc_partitioncolumn == "") | (input_jdbc_lowerbound == "") | (input_jdbc_upperbound == ""))):
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_bq.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_bq.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,19 @@
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
 
+        ignore_keys = {constants.KAFKA_BOOTSTRAP_SERVERS}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting Kafka to Bigquery Pyspark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         #arguments
         bootstrap_server_list: str = args[constants.KAFKA_BOOTSTRAP_SERVERS]
         checkpoint_location: str = args[constants.KAFKA_BQ_CHECKPOINT_LOCATION]
         kafka_topics: str= args[constants.KAFKA_BQ_TOPIC]
         big_query_dataset: str = args[constants.KAFKA_BQ_DATASET]
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/kafka/kafka_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_gcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from logging import Logger
 import argparse
 import pprint
 
 
 
 
-from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql import SparkSession
 
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
+from dataproc_templates.util.dataframe_writer_wrappers import persist_streaming_dataframe_to_cloud_storage
 import dataproc_templates.util.template_constants as constants
 
 __all__ = ['KafkaToGCSTemplate']
 
 class KafkaToGCSTemplate(BaseTemplate):
     """
     Dataproc template implementing loads from Kafka into GCS
@@ -58,22 +60,32 @@
             required=True,
             help='Ouput format of the data (json , csv, avro, parquet)'
         )
         parser.add_argument(
             f'--{constants.KAFKA_GCS_OUPUT_MODE}',
             dest=constants.KAFKA_GCS_OUPUT_MODE,
             required=True,
-            help="Ouput type of GCS append|overwrite"
+            help="Ouput write mode (append, update, complete)",
+            choices=[
+                constants.OUTPUT_MODE_APPEND,
+                constants.OUTPUT_MODE_UPDATE,
+                constants.OUTPUT_MODE_COMPLETE
+            ]
         )
         parser.add_argument(
             f'--{constants.KAFKA_GCS_TERMINATION_TIMEOUT}',
             dest=constants.KAFKA_GCS_TERMINATION_TIMEOUT,
             required=True,
             help="Timeout for termination of kafka subscription"
         )
+        add_spark_options(
+            parser,
+            constants.get_csv_output_spark_options("kafka.gcs.output."),
+            read_options=False
+            )
 
 
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
@@ -88,30 +100,34 @@
         kafka_topics: str= args[constants.KAFKA_TOPIC]
         output_format: str= args[constants.KAFKA_GCS_OUTPUT_FORMAT]
         output_mode:str = args[constants.KAFKA_GCS_OUPUT_MODE]
         timeout: int = int(args[constants.KAFKA_GCS_TERMINATION_TIMEOUT])
         offset:str = args[constants.KAFKA_STARTING_OFFSET]
         checkpoint_loc: str = args[constants.KAFKA_GCS_CHECKPOINT_LOCATION]
 
+        ignore_keys = {constants.KAFKA_GCS_BOOTSTRAP_SERVERS}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting Kafka to GCS Pyspark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
 
         df = spark.readStream.format(constants.KAFKA_INPUT_FORMAT) \
                   .option('kafka.bootstrap.servers', bootstrap_server_list) \
                   .option('subscribe', kafka_topics) \
                   .option('startingOffsets',offset) \
                   .load()
-        
+
         df = df.selectExpr("CAST(key AS STRING)", "CAST(value AS STRING)")
+
         # Write
-        
-        df \
-        .writeStream \
-        .format(output_format) \
-        .outputMode(output_mode) \
-        .option('checkpointLocation',checkpoint_loc) \
-        .option('path',gcs_output_location) \
-        .start() \
-        .awaitTermination(timeout)
+        writer = df.writeStream
+
+        writer = persist_streaming_dataframe_to_cloud_storage(
+            writer, args, checkpoint_loc, gcs_output_location,
+            output_format, output_mode, "kafka.gcs.output.")
+
+        query = writer.start()
+
+        query.awaitTermination(timeout)
+        query.stop()
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/mongo/mongo_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/mongo_to_gcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,17 +105,19 @@
         input_uri: str = args[constants.MONGO_GCS_INPUT_URI]
         input_database: str = args[constants.MONGO_GCS_INPUT_DATABASE]
         input_collection: str = args[constants.MONGO_GCS_INPUT_COLLECTION]
         output_format: str = args[constants.MONGO_GCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.MONGO_GCS_OUTPUT_MODE]
         output_location: str = args[constants.MONGO_GCS_OUTPUT_LOCATION]
 
+        ignore_keys = {constants.MONGO_GCS_INPUT_URI}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting Mongo to Cloud Storage Spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data = spark.read \
             .format(constants.FORMAT_MONGO) \
             .option(constants.MONGO_INPUT_URI, input_uri) \
             .option(constants.MONGO_DATABASE, input_database) \
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 from typing import Dict, Sequence, Optional, Any
 from logging import Logger
 import argparse
 import pprint
 
 from pyspark.sql import SparkSession
+from pyspark.sql.types import StringType
+from pyspark.sql.functions import to_json
 
 from dataproc_templates import BaseTemplate
+from dataproc_templates.util.argument_parsing import add_spark_options
 import dataproc_templates.util.template_constants as constants
+from dataproc_templates.util.dataframe_writer_wrappers import persist_streaming_dataframe_to_cloud_storage
 
 __all__ = ['PubSubLiteToGCSTemplate']
 
 class PubSubLiteToGCSTemplate(BaseTemplate):
     """
-    Dataproc template implementing exports from PubSubLite to GCS
+    Dataproc template implementing exports from Pub/Sub Lite to Cloud Storage
     """
 
     @staticmethod
     def parse_args(args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
         parser.add_argument(
             f'--{constants.PUBSUBLITE_TO_GCS_INPUT_SUBSCRIPTION_URL}',
             dest=constants.PUBSUBLITE_TO_GCS_INPUT_SUBSCRIPTION_URL,
             required=True,
-            help='PubSubLite to GCS Input subscription url'
+            help='Pub/Sub Lite Input subscription url'
         )
         parser.add_argument(
             f'--{constants.PUBSUBLITE_TO_GCS_WRITE_MODE}',
             dest=constants.PUBSUBLITE_TO_GCS_WRITE_MODE,
             required=False,
             default=constants.OUTPUT_MODE_APPEND,
             help=(
                 'Output write mode '
-                '(one of: append,overwrite,ignore,errorifexists) '
+                '(one of: append, update, complete) '
                 '(Defaults to append)'
             ),
             choices=[
-                constants.OUTPUT_MODE_OVERWRITE,
                 constants.OUTPUT_MODE_APPEND,
-                constants.OUTPUT_MODE_IGNORE,
-                constants.OUTPUT_MODE_ERRORIFEXISTS
+                constants.OUTPUT_MODE_UPDATE,
+                constants.OUTPUT_MODE_COMPLETE
             ]
         )
         parser.add_argument(
             f'--{constants.PUBSUBLITE_TO_GCS_OUTPUT_LOCATION}',
             dest=constants.PUBSUBLITE_TO_GCS_OUTPUT_LOCATION,
             required=True,
-            help='GCS output Bucket URL'
+            help='Cloud Storage output Bucket URL'
         )
         parser.add_argument(
-            f'--{constants.PUBSUBLITE_CHECKPOINT_LOCATION}',
-            dest=constants.PUBSUBLITE_CHECKPOINT_LOCATION,
+            f'--{constants.PUBSUBLITE_TO_GCS_CHECKPOINT_LOCATION}',
+            dest=constants.PUBSUBLITE_TO_GCS_CHECKPOINT_LOCATION,
             required=True,
             help='Temporary folder for checkpoint location'
         )
         parser.add_argument(
             f'--{constants.PUBSUBLITE_TO_GCS_OUTPUT_FORMAT}',
             dest=constants.PUBSUBLITE_TO_GCS_OUTPUT_FORMAT,
             required=False,
-            default=constants.FORMAT_CSV,
+            default=constants.FORMAT_JSON,
             help=(
-                'Output Format to GCS '
+                'Output Format to Cloud Storage '
                 '(one of: json, csv, avro, parquet) '
-                '(Defaults to csv)'
+                '(Defaults to json)'
             ),
             choices=[
                 constants.FORMAT_AVRO,
                 constants.FORMAT_CSV,
                 constants.FORMAT_JSON,
                 constants.FORMAT_PRQT
             ]
@@ -80,49 +83,60 @@
         )
         parser.add_argument(
             f'--{constants.PUBSUBLITE_TO_GCS_PROCESSING_TIME}',
             dest=constants.PUBSUBLITE_TO_GCS_PROCESSING_TIME,
             required=True,
             help=('Time interval at which the query will be triggered to process input data')
         )
+        add_spark_options(
+            parser,
+            constants.get_csv_output_spark_options("pubsublite.to.gcs.output."),
+            read_options=False
+            )
 
         known_args: argparse.Namespace
         known_args, _ = parser.parse_known_args(args)
 
         return vars(known_args)
 
     def run(self, spark: SparkSession, args: Dict[str, Any]) -> None:
 
         logger: Logger = self.get_logger(spark=spark)
 
         # Arguments
         input_subscription_url: str = args[constants.PUBSUBLITE_TO_GCS_INPUT_SUBSCRIPTION_URL]
         output_location: str = args[constants.PUBSUBLITE_TO_GCS_OUTPUT_LOCATION]
         output_mode: str = args[constants.PUBSUBLITE_TO_GCS_WRITE_MODE]
-        pubsublite_checkpoint_location: str = args[constants.PUBSUBLITE_CHECKPOINT_LOCATION]
+        pubsublite_checkpoint_location: str = args[constants.PUBSUBLITE_TO_GCS_CHECKPOINT_LOCATION]
         output_format: str = args[constants.PUBSUBLITE_TO_GCS_OUTPUT_FORMAT]
         timeout: int = args[constants.PUBSUBLITE_TO_GCS_TIMEOUT]
         processing_time: str = args[constants.PUBSUBLITE_TO_GCS_PROCESSING_TIME]
 
+        ignore_keys = {constants.PUBSUBLITE_TO_GCS_INPUT_SUBSCRIPTION_URL}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
-            "Starting PubSubLite to GCS spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            "Starting Pub/Sub Lite to Cloud Storage spark job with parameters:\n"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data=(spark.readStream \
             .format(constants.FORMAT_PUBSUBLITE) \
             .option(f"{constants.FORMAT_PUBSUBLITE}.subscription", input_subscription_url) \
             .load())
+        
+        input_data = input_data.withColumn("data", input_data.data.cast(StringType()))
+        input_data = input_data.withColumn("attributes", to_json(input_data.attributes))
 
         # Write
-        query = (input_data.writeStream \
-            .format(output_format) \
-            .option("checkpointLocation", pubsublite_checkpoint_location) \
-            .option("path", output_location) \
-            .outputMode(output_mode) \
-            .trigger(processingTime=processing_time) \
-            .start())
+        writer = input_data.writeStream \
+            .trigger(processingTime=processing_time)
+
+        writer = persist_streaming_dataframe_to_cloud_storage(
+            writer, args, pubsublite_checkpoint_location, output_location,
+            output_format, output_mode, "pubsublite.to.gcs.output.")
+
+        query = writer.start()
 
         # Wait for some time (must be >= 60 seconds) to start receiving messages.
         query.awaitTermination(timeout)
-        query.stop()
+        query.stop()
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/redshift/redshift_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/redshift_to_gcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,19 @@
         input_redshift_secretkey: str = args[constants.REDSHIFTTOGCS_S3_SECRETKEY]
 
         output_location: str = args[constants.REDSHIFTTOGCS_OUTPUT_LOCATION]
         output_format: str = args[constants.REDSHIFTTOGCS_OUTPUT_FORMAT]
         output_mode: str = args[constants.REDSHIFTTOGCS_OUTPUT_MODE]
         output_partitioncolumn: str = args[constants.REDSHIFTTOGCS_OUTPUT_PARTITIONCOLUMN]
 
+        ignore_keys = {constants.REDSHIFTTOGCS_S3_ACCESSKEY, constants.REDSHIFTTOGCS_S3_SECRETKEY}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting REDSHIFT to Cloud Storage Spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         # Read
         input_data: DataFrame
 
         spark._jsc.hadoopConfiguration().set(constants.AWS_S3ACCESSKEY, input_redshift_accesskey)
         spark._jsc.hadoopConfiguration().set(constants.AWS_S3SECRETKEY, input_redshift_secretkey)
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/s3/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/s3/s3_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/s3/s3_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,19 @@
         sf_database: str = args[constants.SNOWFLAKE_TO_GCS_SF_DATABASE]
         sf_schema: str = args[constants.SNOWFLAKE_TO_GCS_SF_SCHEMA]
         sf_warehouse: str = args[constants.SNOWFLAKE_TO_GCS_SF_WAREHOUSE]
         sf_autopushdown: str = args[constants.SNOWFLAKE_TO_GCS_SF_AUTOPUSHDOWN]
         sf_table: str = args[constants.SNOWFLAKE_TO_GCS_SF_TABLE]
         sf_query: str = args[constants.SNOWFLAKE_TO_GCS_SF_QUERY]
 
+        ignore_keys = {constants.SNOWFLAKE_TO_GCS_SF_USER, constants.SNOWFLAKE_TO_GCS_SF_PASSWORD}
+        filtered_args = {key:val for key,val in args.items() if key not in ignore_keys}
         logger.info(
             "Starting Snowflake to Cloud Storage Spark job with parameters:\n"
-            f"{pprint.pformat(args)}"
+            f"{pprint.pformat(filtered_args)}"
         )
 
         sf_options = {
                      "sfURL" : sf_url,
                      "sfUser" : sf_user,
                      "sfPassword" : sf_pwd,
                      "sfDatabase" : sf_database,
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/template_name.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/template_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     AZUREBLOBSTORAGETOBQ = "AZUREBLOBSTORAGETOBQ"
     CASSANDRATOGCS = "CASSANDRATOGCS"
     HIVEDDLEXTRACTOR = "HIVEDDLEXTRACTOR"
     KAFKATOGCS="KAFKATOGCS"
     KAFKATOBQ="KAFKATOBQ"
     S3TOBIGQUERY = "S3TOBIGQUERY"
     PUBSUBLITETOGCS = "PUBSUBLITETOGCS"
-
+    PUBSUBLITETOBIGTABLE = "PUBSUBLITETOBIGTABLE"
 
 
     @classmethod
     def from_string(cls, template_name: str) -> TemplateName:
         """
         Get the TemplateName value from a string.
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/util/__init__.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/util/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/util/argument_parsing.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/util/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/util/dataframe_reader_wrappers.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_reader_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/util/dataframe_writer_wrappers.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_writer_wrappers.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional
-
-from pyspark.sql import DataFrame, SparkSession
+from pyspark.sql import DataFrame
+from pyspark.sql.streaming import DataStreamWriter
 
 import dataproc_templates.util.template_constants as constants
 
 
 def persist_dataframe_to_cloud_storage(
     input_dataframe: DataFrame,
     args: dict,
     output_location: str,
     output_format: str,
-    prefix: str
+    prefix: str,
 ) -> DataFrame:
     """Persist input_dataframe object with methods and options applied for writing to Cloud Storage."""
 
     csv_output_constant_options: dict = constants.get_csv_output_spark_options(prefix)
     spark_options = {csv_output_constant_options[k]: v for k, v in args.items() if k in csv_output_constant_options and v}
 
     if output_format == constants.FORMAT_PRQT:
@@ -41,7 +40,44 @@
     elif output_format == constants.FORMAT_CSV:
         input_dataframe \
             .options(**spark_options) \
             .csv(output_location)
     elif output_format == constants.FORMAT_JSON:
         input_dataframe \
             .json(output_location)
+
+    return input_dataframe
+
+
+def persist_streaming_dataframe_to_cloud_storage(
+    datastream_writer: DataStreamWriter,
+    args: dict,
+    checkpoint_location: str,
+    output_location: str,
+    output_format: str,
+    output_mode: str,
+    prefix: str,
+) -> DataStreamWriter:
+    """Persist streaming input_dataframe object with methods and options applied for writing to Cloud Storage."""
+
+    csv_output_constant_options: dict = constants.get_csv_output_spark_options(prefix)
+    spark_options = {
+        csv_output_constant_options[k]: v
+        for k, v in args.items()
+        if k in csv_output_constant_options and v
+    }
+
+    if output_format == constants.FORMAT_CSV:
+        datastream_writer \
+            .format(output_format) \
+            .outputMode(output_mode) \
+            .options(**spark_options) \
+            .option(constants.STREAM_CHECKPOINT_LOCATION, checkpoint_location) \
+            .option(constants.STREAM_PATH, output_location)
+    elif output_format in (constants.FORMAT_JSON, constants.FORMAT_AVRO, constants.FORMAT_PRQT):
+        datastream_writer \
+            .format(output_format) \
+            .outputMode(output_mode) \
+            .option(constants.STREAM_CHECKPOINT_LOCATION, checkpoint_location) \
+            .option(constants.STREAM_PATH, output_location)
+
+    return datastream_writer
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/util/template_constants.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/util/template_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 FORMAT_DELTA = "delta"
 FORMAT_TXT = "txt"
 FORMAT_AVRO = "avro"
 FORMAT_PRQT = "parquet"
 FORMAT_AVRO_EXTD = "com.databricks.spark.avro"
 FORMAT_BIGQUERY = "com.google.cloud.spark.bigquery"
 FORMAT_JDBC = "jdbc"
+FORMAT_PUBSUBLITE="pubsublite"
 FORMAT_REDSHIFT = "io.github.spark_redshift_community.spark.redshift"
 JDBC_URL = "url"
 JDBC_TABLE = "dbtable"
 JDBC_QUERY = "query"
 JDBC_DRIVER = "driver"
 JDBC_FETCHSIZE = "fetchsize"
 JDBC_BATCH_SIZE = "batchsize"
@@ -92,14 +93,18 @@
 AWS_S3ACCESSKEY = "fs.s3a.access.key"
 AWS_S3SECRETKEY = "fs.s3a.secret.key"
 AWS_S3ENDPOINT = "fs.s3a.endpoint"
 SQL_EXTENSION= "spark.sql.extensions"
 CASSANDRA_EXTENSION= "com.datastax.spark.connector.CassandraSparkExtensions"
 CASSANDRA_CATALOG= "com.datastax.spark.connector.datasource.CassandraCatalog"
 FORMAT_PUBSUBLITE = "pubsublite"
+PUBSUBLITE_SUBSCRIPTION = "pubsublite.subscription"
+PUBSUBLITE_CHECKPOINT_LOCATION = "checkpointLocation"
+STREAM_PATH = "path"
+STREAM_CHECKPOINT_LOCATION = "checkpointLocation"
 
 OPTION_DEFAULT = "default"
 OPTION_HELP = "help"
 OPTION_READ_HELP = "read_help"
 OPTION_WRITE_HELP = "write_help"
 
 # At the moment this is just a map of CSV related options but it will be expanded as required for other uses.
@@ -254,14 +259,16 @@
     return spark_options
 
 # Output mode
 OUTPUT_MODE_OVERWRITE = "overwrite"
 OUTPUT_MODE_APPEND = "append"
 OUTPUT_MODE_IGNORE = "ignore"
 OUTPUT_MODE_ERRORIFEXISTS = "errorifexists"
+OUTPUT_MODE_COMPLETE = "complete"
+OUTPUT_MODE_UPDATE = "update"
 
 # GCS to BigQuery
 GCS_BQ_INPUT_LOCATION = "gcs.bigquery.input.location"
 GCS_BQ_INPUT_FORMAT = "gcs.bigquery.input.format"
 GCS_BQ_OUTPUT_DATASET = "gcs.bigquery.output.dataset"
 GCS_BQ_OUTPUT_TABLE = "gcs.bigquery.output.table"
 GCS_BQ_OUTPUT_MODE = "gcs.bigquery.output.mode"
@@ -494,19 +501,30 @@
 KAFKA_STARTING_OFFSET='kafka.gcs.starting.offset'
 KAFKA_GCS_CHECKPOINT_LOCATION='kafka.gcs.checkpoint.location'
 
 #Pubsublite To GCS
 PUBSUBLITE_TO_GCS_INPUT_SUBSCRIPTION_URL = "pubsublite.to.gcs.input.subscription.url"
 PUBSUBLITE_TO_GCS_WRITE_MODE = "pubsublite.to.gcs.write.mode"
 PUBSUBLITE_TO_GCS_OUTPUT_LOCATION = "pubsublite.to.gcs.output.location"
-PUBSUBLITE_CHECKPOINT_LOCATION = "pubsublite.to.gcs.checkpoint.location"
+PUBSUBLITE_TO_GCS_CHECKPOINT_LOCATION = "pubsublite.to.gcs.checkpoint.location"
 PUBSUBLITE_TO_GCS_OUTPUT_FORMAT = "pubsublite.to.gcs.output.format"
 PUBSUBLITE_TO_GCS_TIMEOUT = "pubsublite.to.gcs.timeout"
 PUBSUBLITE_TO_GCS_PROCESSING_TIME = "pubsublite.to.gcs.processing.time"
 
+# Pub/Sub Lite to Bigtable
+PUBSUBLITE_BIGTABLE_SUBSCRIPTION_PATH = "pubsublite.bigtable.subscription.path"
+PUBSUBLITE_BIGTABLE_STREAMING_TIMEOUT = "pubsublite.bigtable.streaming.timeout"
+PUBSUBLITE_BIGTABLE_STREAMING_TRIGGER = "pubsublite.bigtable.streaming.trigger"
+PUBSUBLITE_BIGTABLE_STREAMING_CHECKPOINT_PATH = "pubsublite.bigtable.streaming.checkpoint.path"
+PUBSUBLITE_BIGTABLE_OUTPUT_PROJECT = "pubsublite.bigtable.output.project"
+PUBSUBLITE_BIGTABLE_OUTPUT_INSTANCE = "pubsublite.bigtable.output.instance"
+PUBSUBLITE_BIGTABLE_OUTPUT_TABLE = "pubsublite.bigtable.output.table"
+PUBSUBLITE_BIGTABLE_OUTPUT_COLUMN_FAMILIES = "pubsublite.bigtable.output.column.families"
+PUBSUBLITE_BIGTABLE_OUTPUT_MAX_VERSIONS = "pubsublite.bigtable.output.max.versions"
+
 # Azure Storage to BigQuery
 AZ_BLOB_BQ_INPUT_LOCATION = "azure.blob.bigquery.input.location"
 AZ_BLOB_BQ_INPUT_FORMAT = "azure.blob.bigquery.input.format"
 AZ_BLOB_BQ_OUTPUT_DATASET = "azure.blob.bigquery.output.dataset"
 AZ_BLOB_BQ_OUTPUT_TABLE = "azure.blob.bigquery.output.table"
 AZ_BLOB_BQ_OUTPUT_MODE = "azure.blob.bigquery.output.mode"
 AZ_BLOB_BQ_TEMP_BUCKET = "temporaryGcsBucket"
```

### Comparing `google-dataproc-templates-0.2.0b0/dataproc_templates/util/tracking.py` & `google-dataproc-templates-0.3.0b0/dataproc_templates/util/tracking.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/PKG-INFO` & `google-dataproc-templates-0.3.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-Metadata-Version: 2.1
-Name: google-dataproc-templates
-Version: 0.2.0b0
-Summary: Google Dataproc templates written in Python
-Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
-License: Apache 2.0
-Platform: Posix; MacOS X; Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 ![Build Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job-python&&subject=python-build)
+![Python Integration Test Status](https://dataproctemplatesci.com/buildStatus/icon?job=dataproc-templates-build%2Fintegration-tests-python&&subject=python-integration-tests)
+
 
 # Dataproc Templates (Python - PySpark)
 * [AzureBlobStorageToBigQuery](/python/dataproc_templates/azure#azure-blob-storage-to-bigquery)
 * [BigQueryToGCS](/python/dataproc_templates/bigquery#bigquery-to-gcs) (blogpost [link](https://medium.com/google-cloud/moving-data-from-bigquery-to-gcs-using-gcp-dataproc-serverless-and-pyspark-f6481b86bcd1))
 * [CassandraToBigquery](/python/dataproc_templates/cassandra#cassandra-to-bigquery)
-* [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs)
+* [CassandraToGCS](/python/dataproc_templates/cassandra#cassandra-to-gcs) (blogpost [link](https://medium.com/google-cloud/export-data-from-cassandra-to-google-cloud-storage-using-dataproc-serverless-2569a00e17fe))
 * [GCSToBigQuery](/python/dataproc_templates/gcs#gcs-to-bigquery) (blogpost [link](https://medium.com/@ppaglilla/getting-started-with-dataproc-serverless-pyspark-templates-e32278a6a06e))
 * [GCSToBigTable](/python/dataproc_templates/gcs#gcs-to-bigtable) (blogpost [link](https://medium.com/google-cloud/pyspark-load-data-from-gcs-to-bigtable-using-gcp-dataproc-serverless-c373430fe157))
 * [GCSToGCS](/python/dataproc_templates/gcs#gcs-to-gcs---sql-transformation)(blogpost [link](https://medium.com/@ankuljain/migrate-gcs-to-gcs-using-dataproc-serverless-3b7b0f6ad6b9))
 * [GCSToJDBC](/python/dataproc_templates/gcs#gcs-to-jdbc) (blogpost [link](https://medium.com/google-cloud/import-data-from-gcs-to-jdbc-databases-using-dataproc-serverless-c7154b242430))
 * [GCSToMongo](/python/dataproc_templates/gcs#gcs-to-mongodb) (blogpost [link](https://medium.com/google-cloud/importing-data-from-gcs-to-mongodb-using-dataproc-serverless-fed58904633a))
 * [HbaseToGCS](/python/dataproc_templates/hbase#hbase-to-gcs)
 * [HiveToBigQuery](/python/dataproc_templates/hive#hive-to-bigquery) (blogpost [link](https://medium.com/google-cloud/processing-data-from-hive-to-bigquery-using-pyspark-and-dataproc-serverless-217c7cb9e4f8))
 * [HiveToGCS](/python/dataproc_templates/hive#hive-to-gcs)(blogpost [link](https://medium.com/@surjitsh/processing-large-data-tables-from-hive-to-gcs-using-pyspark-and-dataproc-serverless-35d3d16daaf))
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
+* [PubSubLiteToBigtable](/python/dataproc_templates/pubsublite#pubsublite-to-bigtable)
 * [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
```

### Comparing `google-dataproc-templates-0.2.0b0/google_dataproc_templates.egg-info/SOURCES.txt` & `google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 dataproc_templates/jdbc/jdbc_to_jdbc.py
 dataproc_templates/kafka/__init__.py
 dataproc_templates/kafka/kafka_to_bq.py
 dataproc_templates/kafka/kafka_to_gcs.py
 dataproc_templates/mongo/__init__.py
 dataproc_templates/mongo/mongo_to_gcs.py
 dataproc_templates/pubsublite/__init__.py
+dataproc_templates/pubsublite/pubsublite_to_bigtable.py
 dataproc_templates/pubsublite/pubsublite_to_gcs.py
 dataproc_templates/redshift/__init__.py
 dataproc_templates/redshift/redshift_to_gcs.py
 dataproc_templates/s3/__init__.py
 dataproc_templates/s3/s3_to_bigquery.py
 dataproc_templates/snowflake/__init__.py
 dataproc_templates/snowflake/snowflake_to_gcs.py
@@ -79,14 +80,15 @@
 test/jdbc/__init__.py
 test/jdbc/test_jdbc_to_bigquery.py
 test/jdbc/test_jdbc_to_gcs.py
 test/jdbc/test_jdbc_to_jdbc.py
 test/mongo/__init__.py
 test/mongo/test_mongo_to_gcs.py
 test/pubsublite/__init__.py
+test/pubsublite/test_pubsublite_to_bigtable.py
 test/pubsublite/test_pubsublite_to_gcs.py
 test/redshift/__init__.py
 test/redshift/test_redshift_to_gcs.py
 test/s3/__init__.py
 test/s3/test_s3_to_bigquery.py
 test/util/__init__.py
 test/util/test_argument_parsing.py
```

### Comparing `google-dataproc-templates-0.2.0b0/setup.py` & `google-dataproc-templates-0.3.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/azure/test_azure_blob_storage_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/test/azure/test_azure_blob_storage_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/bigquery/test_bigquery_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/bigquery/test_bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_bq.py` & `google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_bq.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/cassandra/test_cassandra_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_bigtable.py` & `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigtable.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_jdbc.py` & `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/gcs/test_gcs_to_mongo.py` & `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_mongo.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/gcs/test_text_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/test/gcs/test_text_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/hbase/test_hbase_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/hbase/test_hbase_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/hive/test_hive_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/hive/util/test_hive_ddl_extractor.py` & `google-dataproc-templates-0.3.0b0/test/hive/util/test_hive_ddl_extractor.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/jdbc/test_jdbc_to_jdbc.py` & `google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/mongo/test_mongo_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/mongo/test_mongo_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/pubsublite/test_pubsublite_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
         pubsublite_to_gcs_template = PubSubLiteToGCSTemplate()
         parsed_args = pubsublite_to_gcs_template.parse_args(
             ["--pubsublite.to.gcs.input.subscription.url=test-sub",
              "--pubsublite.to.gcs.write.mode=append",
              "--pubsublite.to.gcs.output.location=gs://test",
              "--pubsublite.to.gcs.checkpoint.location=gs://test-checkpoint",
-             "--pubsublite.to.gcs.output.format=csv",
+             "--pubsublite.to.gcs.output.format=json",
              "--pubsublite.to.gcs.timeout=120",
              "--pubsublite.to.gcs.processing.time=1"
              ])
 
         assert parsed_args["pubsublite.to.gcs.input.subscription.url"] == "test-sub"
         assert parsed_args["pubsublite.to.gcs.write.mode"] == "append"
         assert parsed_args["pubsublite.to.gcs.output.location"] == "gs://test"
         assert parsed_args["pubsublite.to.gcs.checkpoint.location"] == "gs://test-checkpoint"
-        assert parsed_args["pubsublite.to.gcs.output.format"] == "csv"
+        assert parsed_args["pubsublite.to.gcs.output.format"] == "json"
         assert parsed_args["pubsublite.to.gcs.timeout"] == 120
         assert parsed_args["pubsublite.to.gcs.processing.time"] == "1"
 
     def test_parse_args2(self):
         """Tests PubSubLiteToGCSTemplate.parse_args() when output format not passed"""
 
         pubsublite_to_gcs_template = PubSubLiteToGCSTemplate()
@@ -60,31 +60,31 @@
              "--pubsublite.to.gcs.processing.time=1"
              ])
 
         assert parsed_args["pubsublite.to.gcs.input.subscription.url"] == "test-sub"
         assert parsed_args["pubsublite.to.gcs.write.mode"] == "append"
         assert parsed_args["pubsublite.to.gcs.output.location"] == "gs://test"
         assert parsed_args["pubsublite.to.gcs.checkpoint.location"] == "gs://test-checkpoint"
-        assert parsed_args["pubsublite.to.gcs.output.format"] == "csv"
+        assert parsed_args["pubsublite.to.gcs.output.format"] == "json"
         assert parsed_args["pubsublite.to.gcs.timeout"] == 120
         assert parsed_args["pubsublite.to.gcs.processing.time"] == "1"
 
     def test_parse_args3(self):
         """Tests PubSubLiteToGCSTemplate.parse_args() when output mode not passed"""
 
         pubsublite_to_gcs_template = PubSubLiteToGCSTemplate()
         parsed_args = pubsublite_to_gcs_template.parse_args(
             ["--pubsublite.to.gcs.input.subscription.url=test-sub",
              "--pubsublite.to.gcs.output.location=gs://test",
              "--pubsublite.to.gcs.checkpoint.location=gs://test-checkpoint",
-             "--pubsublite.to.gcs.output.format=csv",
+             "--pubsublite.to.gcs.output.format=json",
              "--pubsublite.to.gcs.timeout=120",
              "--pubsublite.to.gcs.processing.time=1"
              ])
 
         assert parsed_args["pubsublite.to.gcs.input.subscription.url"] == "test-sub"
         assert parsed_args["pubsublite.to.gcs.write.mode"] == "append"
         assert parsed_args["pubsublite.to.gcs.output.location"] == "gs://test"
         assert parsed_args["pubsublite.to.gcs.checkpoint.location"] == "gs://test-checkpoint"
-        assert parsed_args["pubsublite.to.gcs.output.format"] == "csv"
+        assert parsed_args["pubsublite.to.gcs.output.format"] == "json"
         assert parsed_args["pubsublite.to.gcs.timeout"] == 120
         assert parsed_args["pubsublite.to.gcs.processing.time"] == "1"
```

### Comparing `google-dataproc-templates-0.2.0b0/test/redshift/test_redshift_to_gcs.py` & `google-dataproc-templates-0.3.0b0/test/redshift/test_redshift_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/s3/test_s3_to_bigquery.py` & `google-dataproc-templates-0.3.0b0/test/s3/test_s3_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.2.0b0/test/util/test_argument_parsing.py` & `google-dataproc-templates-0.3.0b0/test/util/test_argument_parsing.py`

 * *Files identical despite different names*

