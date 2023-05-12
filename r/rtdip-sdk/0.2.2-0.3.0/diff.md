# Comparing `tmp/rtdip_sdk-0.2.2-py3-none-any.whl.zip` & `tmp/rtdip_sdk-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,86 +1,113 @@
-Zip file size: 99272 bytes, number of entries: 84
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/authentication/__init__.py
--rw-r--r--  2.0 unx     7210 b- defN 23-Apr-28 08:50 rtdip_sdk/authentication/authenticate.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/__init__.py
--rw-r--r--  2.0 unx     9846 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/_query_builder.py
--rw-r--r--  2.0 unx     2908 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/interpolate.py
--rw-r--r--  2.0 unx     2293 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/metadata.py
--rw-r--r--  2.0 unx     2626 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/raw.py
--rw-r--r--  2.0 unx     3052 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/resample.py
--rw-r--r--  2.0 unx     9434 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/time_weighted_average.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/__init__.py
--rw-r--r--  2.0 unx      934 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/connection_interface.py
--rw-r--r--  2.0 unx      952 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/cursor_interface.py
--rw-r--r--  2.0 unx     3498 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/db_sql_connector.py
--rw-r--r--  2.0 unx     4228 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/pyodbc_sql_connector.py
--rw-r--r--  2.0 unx     4432 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/turbodbc_sql_connector.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/__init__.py
--rw-r--r--  2.0 unx     1035 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/__init__.py
--rw-r--r--  2.0 unx     1745 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/constants.py
--rw-r--r--  2.0 unx     2434 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/models.py
--rw-r--r--  2.0 unx     5327 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/spark.py
--rw-r--r--  2.0 unx      603 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/converters/__init__.py
--rw-r--r--  2.0 unx      697 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/converters/interfaces.py
--rw-r--r--  2.0 unx     3442 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/converters/pipeline_job_json.py
--rw-r--r--  2.0 unx      630 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/__init__.py
--rw-r--r--  2.0 unx    13207 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/databricks.py
--rw-r--r--  2.0 unx      751 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/interfaces.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/__init__.py
--rw-r--r--  2.0 unx     1114 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/setup.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
--rw-r--r--  2.0 unx     3310 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
--rw-r--r--  2.0 unx     1695 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/models/__init__.py
--rw-r--r--  2.0 unx     7897 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/models/databricks.py
--rw-r--r--  2.0 unx      684 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/__init__.py
--rw-r--r--  2.0 unx      427 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/__init__.py
--rw-r--r--  2.0 unx     5112 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/delta.py
--rw-r--r--  2.0 unx     4781 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/eventhub.py
--rw-r--r--  2.0 unx     3903 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/kafka.py
--rw-r--r--  2.0 unx     3659 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/kinesis.py
--rw-r--r--  2.0 unx      611 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/__init__.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/container.py
--rw-r--r--  2.0 unx     8378 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/job.py
--rw-r--r--  2.0 unx     3037 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/models.py
--rw-r--r--  2.0 unx      618 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/__init__.py
--rw-r--r--  2.0 unx     2227 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/databricks.py
--rw-r--r--  2.0 unx      824 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/interfaces.py
--rw-r--r--  2.0 unx      887 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/models.py
--rw-r--r--  2.0 unx      779 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/__init__.py
--rw-r--r--  2.0 unx     3420 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/autoloader.py
--rw-r--r--  2.0 unx     4501 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/delta.py
--rw-r--r--  2.0 unx     4473 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/delta_sharing.py
--rw-r--r--  2.0 unx     5259 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/eventhub.py
--rw-r--r--  2.0 unx     5240 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/iot_hub.py
--rw-r--r--  2.0 unx     8114 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/kafka.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/kinesis.py
--rw-r--r--  2.0 unx      714 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/__init__.py
--rw-r--r--  2.0 unx      946 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/interfaces.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/__init__.py
--rw-r--r--  2.0 unx     2143 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/binary_to_string.py
--rw-r--r--  2.0 unx     2953 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py
--rw-r--r--  2.0 unx     3571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
--rw-r--r--  2.0 unx      727 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/__init__.py
--rw-r--r--  2.0 unx      773 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/aws/__init__.py
--rw-r--r--  2.0 unx     4674 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/azure/__init__.py
--rw-r--r--  2.0 unx     6556 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/__init__.py
--rw-r--r--  2.0 unx     2185 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/configuration.py
--rw-r--r--  2.0 unx     3857 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
--rw-r--r--  2.0 unx     3119 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
--rw-r--r--  2.0 unx     2602 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
--rw-r--r--  2.0 unx    10172 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2844 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8321 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/RECORD
-84 files, 233849 bytes uncompressed, 85614 bytes compressed:  63.4%
+Zip file size: 137015 bytes, number of entries: 111
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/_sdk_utils/__init__.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-12 16:01 rtdip_sdk/_sdk_utils/compare_versions.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/authentication/__init__.py
+-rw-r--r--  2.0 unx     7210 b- defN 23-May-12 16:01 rtdip_sdk/authentication/authenticate.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/__init__.py
+-rw-r--r--  2.0 unx     6131 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/ami_meters.py
+-rw-r--r--  2.0 unx     2161 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/utils/CreateMetaDataObject.py
+-rw-r--r--  2.0 unx     1137 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/utils/CreateUsageObject.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/utils/__init__.py
+-rw-r--r--  2.0 unx     4524 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/utils/transform.py
+-rw-r--r--  2.0 unx     2804 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/utils/transformers.py
+-rw-r--r--  2.0 unx     4852 b- defN 23-May-12 16:01 rtdip_sdk/data_models/meters/utils/utils.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/data_models/transformers/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-May-12 16:01 rtdip_sdk/data_models/transformers/london_smart_meter_transformer_2_usage.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/data_models/weather/__init__.py
+-rw-r--r--  2.0 unx     5677 b- defN 23-May-12 16:01 rtdip_sdk/data_models/weather/weather_models.py
+-rw-r--r--  2.0 unx     2876 b- defN 23-May-12 16:01 rtdip_sdk/data_models/weather/utils/CreateWeatherObject.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/data_models/weather/utils/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/functions/__init__.py
+-rw-r--r--  2.0 unx    14466 b- defN 23-May-12 16:01 rtdip_sdk/functions/_query_builder.py
+-rw-r--r--  2.0 unx     3048 b- defN 23-May-12 16:01 rtdip_sdk/functions/interpolate.py
+-rw-r--r--  2.0 unx     2546 b- defN 23-May-12 16:01 rtdip_sdk/functions/interpolation_at_time.py
+-rw-r--r--  2.0 unx     2292 b- defN 23-May-12 16:01 rtdip_sdk/functions/metadata.py
+-rw-r--r--  2.0 unx     2766 b- defN 23-May-12 16:01 rtdip_sdk/functions/raw.py
+-rw-r--r--  2.0 unx     3192 b- defN 23-May-12 16:01 rtdip_sdk/functions/resample.py
+-rw-r--r--  2.0 unx     9528 b- defN 23-May-12 16:01 rtdip_sdk/functions/time_weighted_average.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/odbc/__init__.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-12 16:01 rtdip_sdk/odbc/connection_interface.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-12 16:01 rtdip_sdk/odbc/cursor_interface.py
+-rw-r--r--  2.0 unx     3415 b- defN 23-May-12 16:01 rtdip_sdk/odbc/db_sql_connector.py
+-rw-r--r--  2.0 unx     4228 b- defN 23-May-12 16:01 rtdip_sdk/odbc/pyodbc_sql_connector.py
+-rw-r--r--  2.0 unx     4359 b- defN 23-May-12 16:01 rtdip_sdk/odbc/turbodbc_sql_connector.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/__init__.py
+-rw-r--r--  2.0 unx     1035 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/_pipeline_utils/__init__.py
+-rw-r--r--  2.0 unx     2332 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/_pipeline_utils/constants.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/_pipeline_utils/models.py
+-rw-r--r--  2.0 unx     5954 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/_pipeline_utils/spark.py
+-rw-r--r--  2.0 unx      603 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/converters/__init__.py
+-rw-r--r--  2.0 unx      697 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/converters/interfaces.py
+-rw-r--r--  2.0 unx     3442 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/converters/pipeline_job_json.py
+-rw-r--r--  2.0 unx      630 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/__init__.py
+-rw-r--r--  2.0 unx    13295 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/databricks.py
+-rw-r--r--  2.0 unx      751 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/interfaces.py
+-rw-r--r--  2.0 unx      416 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/.gitignore
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/__init__.py
+-rw-r--r--  2.0 unx     1114 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/setup.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/conf/deployment.json
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
+-rw-r--r--  2.0 unx     3310 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
+-rw-r--r--  2.0 unx     1695 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py
+-rw-r--r--  2.0 unx      571 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/models/__init__.py
+-rw-r--r--  2.0 unx     7897 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/deploy/models/databricks.py
+-rw-r--r--  2.0 unx      782 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/__init__.py
+-rw-r--r--  2.0 unx      427 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/__init__.py
+-rw-r--r--  2.0 unx     5226 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/delta.py
+-rw-r--r--  2.0 unx    11510 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/delta_merge.py
+-rw-r--r--  2.0 unx     4906 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/eventhub.py
+-rw-r--r--  2.0 unx     4025 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/kafka.py
+-rw-r--r--  2.0 unx     3761 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/kinesis.py
+-rw-r--r--  2.0 unx    10204 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/pcdm_to_delta.py
+-rw-r--r--  2.0 unx     7050 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/destinations/spark/rest_api.py
+-rw-r--r--  2.0 unx      611 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/execute/__init__.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/execute/container.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/execute/job.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/execute/models.py
+-rw-r--r--  2.0 unx      680 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/secrets/__init__.py
+-rw-r--r--  2.0 unx     2935 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/secrets/azure_key_vault.py
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/secrets/databricks.py
+-rw-r--r--  2.0 unx     2971 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/secrets/hashicorp_vault.py
+-rw-r--r--  2.0 unx      824 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/secrets/interfaces.py
+-rw-r--r--  2.0 unx      887 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/secrets/models.py
+-rw-r--r--  2.0 unx      779 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/__init__.py
+-rw-r--r--  2.0 unx     3420 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/autoloader.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/delta.py
+-rw-r--r--  2.0 unx     4473 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/delta_sharing.py
+-rw-r--r--  2.0 unx     5259 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/eventhub.py
+-rw-r--r--  2.0 unx     5240 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/iot_hub.py
+-rw-r--r--  2.0 unx     8114 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/kafka.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/sources/spark/kinesis.py
+-rw-r--r--  2.0 unx      795 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/__init__.py
+-rw-r--r--  2.0 unx      946 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/interfaces.py
+-rw-r--r--  2.0 unx      570 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/spark/__init__.py
+-rw-r--r--  2.0 unx     2174 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/spark/binary_to_string.py
+-rw-r--r--  2.0 unx     3436 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/spark/fledge_json_to_pcdm.py
+-rw-r--r--  2.0 unx     4837 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_pcdm.py
+-rw-r--r--  2.0 unx     3905 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/spark/ssip_pi_binary_file_to_pcdm.py
+-rw-r--r--  2.0 unx     5534 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/transformers/spark/ssip_pi_binary_json_to_pcdm.py
+-rw-r--r--  2.0 unx      762 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/__init__.py
+-rw-r--r--  2.0 unx      773 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/aws/__init__.py
+-rw-r--r--  2.0 unx     4680 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/azure/__init__.py
+-rw-r--r--  2.0 unx     6579 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py
+-rw-r--r--  2.0 unx      569 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/spark/__init__.py
+-rw-r--r--  2.0 unx     3375 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/spark/adls_gen2_spn_connect.py
+-rw-r--r--  2.0 unx     2173 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/spark/configuration.py
+-rw-r--r--  2.0 unx     5181 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
+-rw-r--r--  2.0 unx     3125 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
+-rw-r--r--  2.0 unx     2602 b- defN 23-May-12 16:01 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
+-rw-r--r--  2.0 unx    10172 b- defN 23-May-12 16:01 rtdip_sdk-0.3.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3058 b- defN 23-May-12 16:01 rtdip_sdk-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 16:01 rtdip_sdk-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-12 16:01 rtdip_sdk-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11191 b- defN 23-May-12 16:01 rtdip_sdk-0.3.0.dist-info/RECORD
+111 files, 334532 bytes uncompressed, 118635 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,25 +1,76 @@
 Filename: rtdip_sdk/__init__.py
 Comment: 
 
+Filename: rtdip_sdk/_sdk_utils/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/_sdk_utils/compare_versions.py
+Comment: 
+
 Filename: rtdip_sdk/authentication/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/authentication/authenticate.py
 Comment: 
 
+Filename: rtdip_sdk/data_models/meters/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/ami_meters.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/utils/CreateMetaDataObject.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/utils/CreateUsageObject.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/utils/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/utils/transform.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/utils/transformers.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/meters/utils/utils.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/transformers/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/transformers/london_smart_meter_transformer_2_usage.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/weather/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/weather/weather_models.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/weather/utils/CreateWeatherObject.py
+Comment: 
+
+Filename: rtdip_sdk/data_models/weather/utils/__init__.py
+Comment: 
+
 Filename: rtdip_sdk/functions/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/functions/_query_builder.py
 Comment: 
 
 Filename: rtdip_sdk/functions/interpolate.py
 Comment: 
 
+Filename: rtdip_sdk/functions/interpolation_at_time.py
+Comment: 
+
 Filename: rtdip_sdk/functions/metadata.py
 Comment: 
 
 Filename: rtdip_sdk/functions/raw.py
 Comment: 
 
 Filename: rtdip_sdk/functions/resample.py
@@ -78,23 +129,29 @@
 
 Filename: rtdip_sdk/pipelines/deploy/databricks.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/interfaces.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/deploy/dbx/.gitignore
+Comment: 
+
 Filename: rtdip_sdk/pipelines/deploy/dbx/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/setup.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/deploy/dbx/conf/deployment.json
+Comment: 
+
 Filename: rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
@@ -117,23 +174,32 @@
 
 Filename: rtdip_sdk/pipelines/destinations/spark/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/destinations/spark/delta.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/destinations/spark/delta_merge.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/destinations/spark/eventhub.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/destinations/spark/kafka.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/destinations/spark/kinesis.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/destinations/spark/pcdm_to_delta.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/destinations/spark/rest_api.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/execute/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/execute/container.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/execute/job.py
@@ -141,17 +207,23 @@
 
 Filename: rtdip_sdk/pipelines/execute/models.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/secrets/__init__.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/secrets/azure_key_vault.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/secrets/databricks.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/secrets/hashicorp_vault.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/secrets/interfaces.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/secrets/models.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/sources/__init__.py
@@ -192,18 +264,24 @@
 
 Filename: rtdip_sdk/pipelines/transformers/spark/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/transformers/spark/binary_to_string.py
 Comment: 
 
-Filename: rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py
+Filename: rtdip_sdk/pipelines/transformers/spark/fledge_json_to_pcdm.py
 Comment: 
 
-Filename: rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
+Filename: rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_pcdm.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/transformers/spark/ssip_pi_binary_file_to_pcdm.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/transformers/spark/ssip_pi_binary_json_to_pcdm.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/interfaces.py
 Comment: 
@@ -219,35 +297,38 @@
 
 Filename: rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/__init__.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/utilities/spark/adls_gen2_spn_connect.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/utilities/spark/configuration.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
 Comment: 
 
-Filename: rtdip_sdk-0.2.2.dist-info/LICENSE.md
+Filename: rtdip_sdk-0.3.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: rtdip_sdk-0.2.2.dist-info/METADATA
+Filename: rtdip_sdk-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: rtdip_sdk-0.2.2.dist-info/WHEEL
+Filename: rtdip_sdk-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: rtdip_sdk-0.2.2.dist-info/top_level.txt
+Filename: rtdip_sdk-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rtdip_sdk-0.2.2.dist-info/RECORD
+Filename: rtdip_sdk-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rtdip_sdk/functions/_query_builder.py

```diff
@@ -12,39 +12,63 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from jinjasql import JinjaSql
 from six import string_types
 from copy import deepcopy
-from datetime import datetime
+import datetime
+from datetime import datetime, time
 
 def _is_date_format(dt, format):
     try:
         return datetime.strptime(dt , format)
     except:
         return False
 
-def _fix_date(dt, is_end_date = False):
-    if _is_date_format(dt, "%Y-%m-%d"):
+def _parse_date(dt, is_end_date=False, exclude_date_format=False):   
+    if isinstance(dt, datetime):
+        if dt.time() == time.min:
+            if dt.tzinfo is not None:
+                dt = datetime.strftime(dt, "%Y-%m-%d%z")
+            else:
+                dt = dt.date()
+        else:
+            dt = datetime.strftime(dt, "%Y-%m-%dT%H:%M:%S%z")
+    dt = str(dt)
+
+    if _is_date_format(dt, "%Y-%m-%d") and exclude_date_format == False:
         _time = "T23:59:59" if is_end_date == True else "T00:00:00"
-        return dt + _time + "+00:00"
+        return dt + _time + "+0000"
     elif _is_date_format(dt, "%Y-%m-%dT%H:%M:%S"):
-        return dt + "+00:00"
+        return dt + "+0000"
     elif _is_date_format(dt, "%Y-%m-%dT%H:%M:%S%z"):
         return dt
+    elif _is_date_format(dt, "%Y-%m-%d%z"):
+        _time = "T23:59:59" if is_end_date == True else "T00:00:00"
+        dt = dt[0:10] + _time + dt[10:]
+        return dt
     else: 
-        raise ValueError(f"Inputted datetime: '{dt}', is not in the correct format")
-        
-def _fix_dates(parameters_dict):
+        msg = f"Inputted timestamp: '{dt}', is not in the correct format."
+        if exclude_date_format == True:
+            msg += " List of timestamps must be in datetime format."
+        raise ValueError(msg)
         
-    parameters_dict["start_date"] = _fix_date(parameters_dict["start_date"])
-    parameters_dict["end_date"] = _fix_date(parameters_dict["end_date"], True)
+def _parse_dates(parameters_dict):
+    if "start_date" in parameters_dict:
+        parameters_dict["start_date"] = _parse_date(parameters_dict["start_date"])
+        sample_dt = parameters_dict["start_date"]
+    if "end_date" in parameters_dict:
+        parameters_dict["end_date"] = _parse_date(parameters_dict["end_date"], True)
+    if "timestamps" in parameters_dict:
+        parsed_timestamp = [_parse_date(dt, is_end_date=False, exclude_date_format=True) for dt in parameters_dict["timestamps"]]
+        parameters_dict["timestamps"] = parsed_timestamp
+        sample_dt = parsed_timestamp[0]
 
-    parameters_dict["time_zone"] = datetime.strptime(parameters_dict["start_date"], "%Y-%m-%dT%H:%M:%S%z").strftime("%z")
+    parameters_dict["time_zone"] = datetime.strptime(sample_dt, "%Y-%m-%dT%H:%M:%S%z").strftime("%z")
     
     return parameters_dict
 
 def _quote_sql_string(value):
     '''
     If `value` is a string type, escapes single quotes in the string
     and returns the string enclosed in single quotes.
@@ -130,44 +154,101 @@
     }
 
     sql_template = JinjaSql(param_style='pyformat')
     query, bind_params = sql_template.prepare_query(sample_query, sample_parameters)
     sql_query = _get_sql_from_template(query, bind_params)
     return sql_query, sample_query, sample_parameters    
 
-def _interpolation_query(parameters_dict: dict, sample_query: str, sample_parameters: dict, tag_name_string: str) -> str:
+def _interpolation_query(parameters_dict: dict, sample_query: str, sample_parameters: dict) -> str:
 
     if parameters_dict["interpolation_method"] == "forward_fill":
         interpolation_method = 'last_value/UNBOUNDED PRECEDING/CURRENT ROW'
 
     if parameters_dict["interpolation_method"] == "backward_fill":
         interpolation_method = 'first_value/CURRENT ROW/UNBOUNDED FOLLOWING'
 
     interpolation_options = interpolation_method.split('/')
 
     interpolate_query = (
         "SELECT a.EventTime, a.TagName, {{ interpolation_options_0 | sqlsafe }}(b.Value, true) OVER (PARTITION BY a.TagName ORDER BY a.EventTime ROWS BETWEEN {{ interpolation_options_1 | sqlsafe }} AND {{ interpolation_options_2 | sqlsafe }}) AS Value FROM "
         "(SELECT explode(sequence(from_utc_timestamp(to_timestamp({{ start_date }}), \"{{ time_zone | sqlsafe }}\"), from_utc_timestamp(to_timestamp({{ end_date }}), \"{{ time_zone | sqlsafe }}\"), INTERVAL {{ sample_rate + ' ' + sample_unit }})) AS EventTime, "
-        f"explode(array({tag_name_string})) AS TagName) a "
+        "explode(array{{ tag_names | inclause }}) AS TagName) a "
         f"LEFT OUTER JOIN ({sample_query}) b "
         "ON a.EventTime = b.EventTime "
         "AND a.TagName = b.TagName"        
     )
     
     interpolate_parameters = sample_parameters.copy()
     interpolate_parameters["interpolation_options_0"] = interpolation_options[0]
     interpolate_parameters["interpolation_options_1"] = interpolation_options[1]
     interpolate_parameters["interpolation_options_2"] = interpolation_options[2]
-    interpolate_parameters["tag_name_string"] = tag_name_string
 
     sql_template = JinjaSql(param_style='pyformat')
     query, bind_params = sql_template.prepare_query(interpolate_query, interpolate_parameters)
     sql_query = _get_sql_from_template(query, bind_params)
     return sql_query
 
+def _interpolation_at_time(parameters_dict: dict) -> str:
+    timestamps_deduplicated = list(dict.fromkeys(parameters_dict['timestamps'])) #remove potential duplicates in tags
+    parameters_dict["timestamps"] = timestamps_deduplicated.copy()
+    parameters_dict["min_timestamp"] = min(timestamps_deduplicated)
+    parameters_dict["max_timestamp"] = max(timestamps_deduplicated)
+
+    interpolate_at_time_query = (
+        "SELECT TagName, EventTime, Interpolated_Value as Value FROM "
+        "(SELECT *, lag(EventTime) OVER (PARTITION BY TagName ORDER BY EventTime) AS Previous_EventTime, "
+        "lag(Value) OVER (PARTITION BY TagName ORDER BY EventTime) AS Previous_Value, "
+        "lead(EventTime) OVER (PARTITION BY TagName ORDER BY EventTime) AS Next_EventTime, "
+        "lead(Value) OVER (PARTITION BY TagName ORDER BY EventTime) AS Next_Value, "
+        "CASE WHEN Requested_EventTime = Found_EventTime THEN Value WHEN Next_EventTime IS NULL THEN Previous_Value WHEN Previous_EventTime IS NULL and Next_EventTime IS NULL THEN NULL ELSE Previous_Value + ((Next_Value - Previous_Value) * ((unix_timestamp(EventTime) - unix_timestamp(Previous_EventTime)) / (unix_timestamp(Next_EventTime) - unix_timestamp(Previous_EventTime)))) END AS Interpolated_Value FROM "
+        "(SELECT coalesce(a.TagName, b.TagName) as TagName, coalesce(a.EventTime, b.EventTime) as EventTime, a.EventTime as Requested_EventTime, b.EventTime as Found_EventTime, b.Status, b.Value FROM "
+        "(SELECT explode(array( "
+        "{% for timestamp in timestamps -%} "
+        "from_utc_timestamp(to_timestamp({{timestamp}}), {{time_zone}})"
+        "{% if not loop.last %}"
+        ", "
+        "{% endif %}"
+        "{% endfor %} "
+        ")) AS EventTime, "
+        "explode(array{{ tag_names | inclause }}) AS TagName) a FULL OUTER JOIN "
+        "(SELECT * FROM (SELECT * FROM "
+        "{{ business_unit | sqlsafe }}.sensors.{{ asset | sqlsafe }}_{{ data_security_level | sqlsafe }}_events_{{ data_type | sqlsafe }} "
+        "WHERE EventDate BETWEEN "
+        "{% if timestamps is defined %}"
+        "date_sub(to_date(to_timestamp({{ min_timestamp }})), 1) AND date_add(to_date(to_timestamp({{ max_timestamp }})), 1)"
+        "{% endif %}"
+        "AND TagName in {{ tag_names | inclause }})) b ON a.EventTime = b.EventTime AND a.TagName = b.TagName))"
+        "WHERE EventTime in ( "
+        "{% for timestamp in timestamps -%} "
+        "from_utc_timestamp(to_timestamp({{timestamp}}), {{time_zone}})"
+        "{% if not loop.last %}"
+        ", "
+        "{% endif %}"
+        "{% endfor %} "
+        ")"       
+    )
+    
+    interpolation_at_time_parameters = {
+        "business_unit": parameters_dict['business_unit'].lower(),
+        "region": parameters_dict['region'].lower(),
+        "asset": parameters_dict['asset'].lower(),
+        "data_security_level": parameters_dict['data_security_level'].lower(),
+        "data_type": parameters_dict['data_type'].lower(),
+        "tag_names": list(dict.fromkeys(parameters_dict['tag_names'])),
+        "timestamps": parameters_dict['timestamps'],
+        "time_zone": parameters_dict["time_zone"],
+        "min_timestamp": parameters_dict["min_timestamp"],
+        "max_timestamp": parameters_dict["max_timestamp"]
+    }
+
+    sql_template = JinjaSql(param_style='pyformat')
+    query, bind_params = sql_template.prepare_query(interpolate_at_time_query, interpolation_at_time_parameters)
+    sql_query = _get_sql_from_template(query, bind_params)
+    return sql_query
+
 def _metadata_query(parameters_dict: dict) -> str:
     
     metadata_query  = (
         "SELECT * FROM "
         "{{ business_unit | sqlsafe }}.sensors.{{ asset | sqlsafe }}_{{ data_security_level | sqlsafe }}_metadata "
         "{% if tag_names is defined and tag_names|length > 0 %}" + 
         "WHERE TagName in {{ tag_names | inclause }}"
@@ -183,30 +264,35 @@
     }
 
     sql_template = JinjaSql(param_style='pyformat')
     query, bind_params = sql_template.prepare_query(metadata_query, metadata_parameters)
     sql_query = _get_sql_from_template(query, bind_params)
     return sql_query    
 
-def _query_builder(parameters_dict: dict, metadata=False) -> str:
+def _query_builder(parameters_dict: dict, metadata=False, interpolation_at_time=False) -> str:
     if "tag_names" not in parameters_dict:
         parameters_dict["tag_names"] = []
     tagnames_deduplicated = list(dict.fromkeys(parameters_dict['tag_names'])) #remove potential duplicates in tags
     parameters_dict["tag_names"] = tagnames_deduplicated.copy()
     tag_name_string = ', '.join('"{0}"'.format(tagname) for tagname in tagnames_deduplicated)
 
     if metadata:
         return _metadata_query(parameters_dict)
-
-    parameters_dict = _fix_dates(parameters_dict)
+    
+    parameters_dict = _parse_dates(parameters_dict)
+    
+    if interpolation_at_time:
+        return _interpolation_at_time(parameters_dict)
 
     if "agg_method" not in parameters_dict:
         return _raw_query(parameters_dict)
 
     if "sample_rate" in parameters_dict:
         sample_prepared_query, sample_query, sample_parameters = _sample_query(parameters_dict)
 
         if "interpolation_method" not in parameters_dict:
             return sample_prepared_query
 
     if "interpolation_method" in parameters_dict:
-        return _interpolation_query(parameters_dict, sample_query, sample_parameters, tag_name_string)
+        return _interpolation_query(parameters_dict, sample_query, sample_parameters)
+    
+
```

## rtdip_sdk/functions/interpolate.py

```diff
@@ -31,17 +31,17 @@
     Attributes:
         business_unit (str): Business unit of the data
         region (str): Region
         asset (str):  Asset
         data_security_level (str): Level of data security 
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames ["tag_1", "tag_2"]
-        start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
-        end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
-        sample_rate (int): The resampling rate (numeric input)
+        start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
+        end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
+        sample_rate (str): The resampling rate (numeric input)
         sample_unit (str): The resampling unit (second, minute, day, hour)
         agg_method (str): Aggregation Method (first, last, avg, min, max)
         interpolation_method (str): Optional. Interpolation method (forward_fill, backward_fill)
         include_bad_data (bool): Include "Bad" data points with True or remove "Bad" data points with False
 
     Returns:
         DataFrame: A resampled and interpolated dataframe.
```

## rtdip_sdk/functions/metadata.py

```diff
@@ -31,15 +31,15 @@
         parameters_dict: A dictionary of parameters (see Attributes table below)
 
     Attributes:
         business_unit (str): Business unit
         region (str): Region
         asset (str): Asset 
         data_security_level (str): Level of data security
-        tag_names (list): (Optional) Either pass a list of tagname/tagnames ["tag_1", "tag_2"] or leave the list blank [] or leave the parameter out completely
+        tag_names (optional, list): Either pass a list of tagname/tagnames ["tag_1", "tag_2"] or leave the list blank [] or leave the parameter out completely
 
     Returns:
         DataFrame: A dataframe of metadata.
     '''
     try:
         query = _query_builder(parameters_dict, metadata=True)
```

## rtdip_sdk/functions/raw.py

```diff
@@ -34,16 +34,16 @@
     Attributes:
         business_unit (str): Business unit 
         region (str): Region
         asset (str): Asset 
         data_security_level (str): Level of data security
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames ["tag_1", "tag_2"]
-        start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
-        end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
+        start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
+        end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
         include_bad_data (bool): Include "Bad" data points with True or remove "Bad" data points with False
 
     Returns:
         DataFrame: A dataframe of raw timeseries data.
     '''
     try:
         query = _query_builder(parameters_dict)
```

## rtdip_sdk/functions/resample.py

```diff
@@ -33,17 +33,17 @@
     Attributes:
         business_unit (str): Business unit of the data
         region (str): Region
         asset (str):  Asset
         data_security_level (str): Level of data security
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames ["tag_1", "tag_2"]
-        start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
-        end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS)
-        sample_rate (int): The resampling rate (numeric input)
+        start_date (str): Start date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
+        end_date (str): End date (Either a date in the format YY-MM-DD or a datetime in the format YYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
+        sample_rate (str): The resampling rate (numeric input)
         sample_unit (str): The resampling unit (second, minute, day, hour)
         agg_method (str): Aggregation Method (first, last, avg, min, max)
         include_bad_data (bool): Include "Bad" data points with True or remove "Bad" data points with False
 
     Returns:
         DataFrame: A resampled dataframe.
     '''
```

## rtdip_sdk/functions/time_weighted_average.py

```diff
@@ -14,14 +14,15 @@
 import logging
 import pandas as pd
 from .raw import get as raw_get
 from .metadata import get as metadata_get
 from datetime import datetime, timedelta
 import pytz
 import numpy as np
+
 def get(connection: object, parameters_dict: dict) -> pd.DataFrame:
     '''
     A function that recieves a dataframe of raw tag data and performs a timeweighted average, returning the results. 
     
     This function requires the input of a pandas dataframe acquired via the rtdip.functions.raw() method and the user to input a dictionary of parameters. (See Attributes table below)
     
     Pi data points will either have step enabled (True) or step disabled (False). You can specify whether you want step to be fetched by "Pi" or you can set the step parameter to True/False in the dictionary below.
@@ -32,20 +33,20 @@
     Attributes:
         business_unit (str): Business unit 
         region (str): Region
         asset (str): Asset 
         data_security_level (str): Level of data security 
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames
-        start_date (str): Start date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zz:zz)
-        end_date (str): End date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zz:z)
+        start_date (str): Start date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
+        end_date (str): End date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zzzz)
         window_size_mins (int): Window size in minutes
         window_length (int): (Optional) add longer window time for the start or end of specified date to cater for edge cases
         include_bad_data (bool): Include "Bad" data points with True or remove "Bad" data points with False
-        step (bool, str): data points with step "enabled" or "disabled". The options for step are "metadata" (string), True or False (bool)
+        step (str): data points with step "enabled" or "disabled". The options for step are "metadata", "true" or "false". "metadata" will get the step requirements from the metadata table if applicable.
     Returns:
         DataFrame: A dataframe containing the time weighted averages.
     '''
     try:  
         dtz_format = "%Y-%m-%dT%H:%M:%S%z"
         utc = "Etc/UTC"
         
@@ -99,20 +100,20 @@
         preprocess_df.set_index(["EventTime", "TagName", "EventDate"], inplace=True)
         preprocess_df = preprocess_df.join(boundaries_df, how="outer", rsuffix="right")
         if isinstance(parameters_dict["step"], str) and parameters_dict["step"].lower() == "metadata":
             metadata_df = metadata_get(connection, parameters_dict)
             metadata_df.set_index("TagName", inplace=True)
             metadata_df = metadata_df.loc[:, "Step"]
             preprocess_df = preprocess_df.merge(metadata_df, left_index=True, right_index=True)
-        elif parameters_dict["step"] == True:
+        elif parameters_dict["step"].lower() == "true":
             preprocess_df["Step"] =  True
-        elif parameters_dict["step"] == False:
+        elif parameters_dict["step"].lower() == "false":
             preprocess_df["Step"] = False
         else:
-            raise Exception('Unexpected step value', parameters_dict["step"])
+            raise Exception('Unexpected step value', parameters_dict["step"]) # NOSONAR
         
         def process_time_weighted_averages_step(pandas_df):
             if pandas_df["Step"].any() == False:
                 pandas_df = pandas_df.reset_index(level=["TagName", "EventDate"]).sort_index().interpolate(method='time')
                 shift_raw_df = pandas_df.copy()
                 shift_raw_df["CalcValue"] = (shift_raw_df.index.to_series().diff().dt.seconds/86400) * shift_raw_df.Value.rolling(2).sum()
                 time_weighted_averages = shift_raw_df.resample("{}T".format(str(parameters_dict["window_size_mins"])), closed="right", label="right").CalcValue.sum() * 0.5 / parameters_dict["window_size_mins"] * 24 * 60
```

## rtdip_sdk/odbc/db_sql_connector.py

```diff
@@ -86,18 +86,16 @@
     """
     Gets all rows of a query.
     
     Returns:
         list: list of results
     """
     try:
-      result = self.cursor.fetchall()
-      cols = [column[0] for column in self.cursor.description]
-      df = pd.DataFrame(result)
-      df.columns = cols
+      result = self.cursor.fetchall_arrow()
+      df = result.to_pandas()
       return df
     except Exception as e:
       logging.exception('error while fetching the rows of a query')
       raise e
 
   def close(self) -> None: 
     """Closes the cursor."""
```

## rtdip_sdk/odbc/turbodbc_sql_connector.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 from turbodbc import connect, make_options, Megabytes
 import pandas as pd
 from .connection_interface import ConnectionInterface
 from .cursor_interface import CursorInterface
 import logging
+import os
 
 class TURBODBCSQLConnection(ConnectionInterface):
   """
   Turbodbc is a python module used to access relational databases through an ODBC interface. It will allow a user to connect to databricks clusters or sql warehouses.
   
   Turbodbc offers built-in NumPy support allowing it to be much faster for processing compared to other connectors.
   To find details for SQL warehouses server_hostname and http_path location to the SQL Warehouse tab in the documentation.
@@ -34,31 +35,31 @@
       More fields such as driver can be configured upon extension.
   """
   def __init__(self, server_hostname: str, http_path: str, access_token: str) -> None:
     options = make_options(
         autocommit=True, 
         read_buffer_size=Megabytes(100),
         use_async_io=True)
+    
     self.connection = connect(Driver="Simba Spark ODBC Driver",
-                              Server=server_hostname,
-                              HOST=server_hostname,
-                              PORT=443,
+                              Host=server_hostname,
+                              Port=443,
                               SparkServerType=3,
-                              Schema="default",
                               ThriftTransport=2,
                               SSL=1,
                               AuthMech=11,
                               Auth_AccessToken=access_token,
                               Auth_Flow=0,
                               HTTPPath=http_path,
                               UseNativeQuery=1,
                               FastSQLPrepare=1,
                               ApplyFastSQLPrepareToAllQueries=1,
                               DisableLimitZero=1,                      
                               EnableAsyncExec=1,
+                              RowsFetchedPerBlock=os.getenv("RTDIP_ODBC_ROW_BLOCK_SIZE", 500000),
                               turbodbc_options=options)
 
   def close(self) -> None:
     """Closes connection to database."""
     try:
       self.connection.close()
     except Exception as e:
@@ -106,18 +107,16 @@
     """
     Gets all rows of a query.
     
     Returns:
         list: list of results
     """
     try:
-      result = self.cursor.fetchall()
-      cols = [column[0] for column in self.cursor.description]
-      df = pd.DataFrame(result)
-      df.columns = cols
+      result = self.cursor.fetchallarrow()
+      df = result.to_pandas()
       return df
     except Exception as e:
       logging.exception('error while fetching the rows from the query')
       raise e
 
   def close(self) -> None: 
     """Closes the cursor."""
```

## rtdip_sdk/pipelines/_pipeline_utils/constants.py

```diff
@@ -33,18 +33,38 @@
     "spark_sql_kafka": MavenLibrary(
                 group_id="org.apache.spark", 
                 artifact_id="spark-sql-kafka-0-10_2.12",
                 version="3.4.0"
             ),
     "rtdip_sdk": PyPiLibrary(
                 name="rtdip_sdk",
-                version="0.2.1"
+                version="0.2.2"
             ),
     "azure_adls_gen_2": PyPiLibrary(
                 name="azure-storage-file-datalake",
                 version="12.10.1"
             ),
+    "azure_key_vault_secret": PyPiLibrary(
+                name="azure-keyvault-secrets",
+                version="4.7.0"
+            ),
     "aws_boto3": PyPiLibrary(
                 name="boto3",
                 version="1.26.118"
-            )            
+            ),
+    "hashicorp_vault": PyPiLibrary(
+                name="hvac",
+                version="1.1.0"
+            ),
+    "api_requests": PyPiLibrary(
+                name="requests",
+                version="2.30.0"
+            ),
+    "pyarrow": PyPiLibrary(
+                name="pyarrow",
+                version="12.0.0"
+            ),
+    "pandas": PyPiLibrary(
+                name="pandas",
+                version="2.0.1"
+            ),                      
 }
```

## rtdip_sdk/pipelines/_pipeline_utils/models.py

```diff
@@ -9,27 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
 
 class SystemType(Enum):
     """The type of the system."""
     # Executable in a python environment
     PYTHON = 1
     # Executable in a pyspark environment
     PYSPARK = 2
     # Executable in a databricks environment
     PYSPARK_DATABRICKS = 3
 
-
 class LibraryTypes(Enum):
     MAVEN = 1
     PYPI = 2
     PYTHONWHL = 3
 
 class MavenLibrary(BaseModel):
     group_id: str
@@ -48,17 +47,17 @@
     def to_string(self) -> str:
         return f"{self.name}=={self.version}"
 
 class PythonWheelLibrary(BaseModel):
     path: str
 
 class Libraries(BaseModel):
-    maven_libraries: list[MavenLibrary] = []
-    pypi_libraries: list[PyPiLibrary] = []
-    pythonwheel_libraries: list[PythonWheelLibrary] = []
+    maven_libraries: List[MavenLibrary] = []
+    pypi_libraries: List[PyPiLibrary] = []
+    pythonwheel_libraries: List[PythonWheelLibrary] = []
 
     def add_maven_library(self, maven_library: MavenLibrary):
         self.maven_libraries.append(maven_library)
 
     def add_pypi_library(self, pypi_library: PyPiLibrary):
         self.pypi_libraries.append(pypi_library)
```

## rtdip_sdk/pipelines/_pipeline_utils/spark.py

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from pyspark.sql import SparkSession
-from pyspark.sql.types import StructType, StructField, TimestampType, StringType, BinaryType, LongType, MapType, IntegerType
+from pyspark.sql.types import StructType, StructField, TimestampType, StringType, BinaryType, LongType, MapType, IntegerType, ArrayType
+
 from .models import Libraries
 
 class SparkClient():
     spark_configuration: dict
     spark_libraries: Libraries
     spark_session: SparkSession
     
@@ -93,28 +94,37 @@
     StructField('enqueuedTime', TimestampType(), True), 
     StructField('publisher', StringType(), True), 
     StructField('partitionKey', StringType(), True), 
     StructField('properties', MapType(StringType(), StringType(), True), True), 
     StructField('systemProperties', MapType(StringType(), StringType(), True), True)
 ])
 
-OPCUA_SCHEMA = StructType([
+OPC_PUBLISHER_SCHEMA = StructType([
     StructField('ApplicationUri',StringType(),True),
     StructField('DisplayName',StringType(),True),
     StructField('NodeId', StringType(),True),
     StructField('Value', StructType([
         StructField('SourceTimestamp',StringType(),True),
         StructField('StatusCode', StructType([
             StructField('Code', LongType(),True),
             StructField('Symbol', StringType(),True)
         ]), True),
         StructField('Value',StringType(),True)
     ]),True)
 ])
 
+PROCESS_DATA_MODEL_SCHEMA = StructType([
+    StructField('TagName', StringType(), True), 
+    StructField('EventTime', TimestampType(), True), 
+    StructField('Status', StringType(), True), 
+    StructField('Value', StringType(), True), 
+    StructField('ValueType', StringType(), True),
+    StructField('ChangeType', StringType(), True)
+])
+
 KAFKA_SCHEMA = StructType(
            [StructField('key', BinaryType(), True),
             StructField('value', BinaryType(), True),
             StructField('topic', StringType(), True),
             StructField('partition', IntegerType(), True),
             StructField('offset', LongType(), True),
             StructField('timestamp', TimestampType(), True),
@@ -124,8 +134,15 @@
 KINESIS_SCHEMA = StructType(
            [StructField('partitionKey', StringType(), True),
             StructField('data', BinaryType(), True),
             StructField('stream', StringType(), True),
             StructField('shardId', StringType(), True),
             StructField('sequenceNumber', StringType(), True),
             StructField('approximateArrivalTimestamp', TimestampType(), True)]
+       )
+
+FLEDGE_SCHEMA = ArrayType(
+            StructType([
+            StructField("asset", StringType(), True),
+            StructField("readings", MapType(StringType(), StringType(), True), True),
+            StructField("timestamp", TimestampType(), True)])
        )
```

## rtdip_sdk/pipelines/deploy/databricks.py

```diff
@@ -152,15 +152,16 @@
 
             # get libraries
             for step in task.step_list:
                 libraries = step.component.libraries()
                 for pypi_library in libraries.pypi_libraries:
                     databricks_job_task.libraries.append(DatabricksLibraries(pypi=DatbricksLibrariesPypi(package=pypi_library.to_string(), repo=pypi_library.repo)))
                 for maven_library in libraries.maven_libraries:
-                    databricks_job_task.libraries.append(DatabricksLibraries(maven=DatabricksLibrariesMaven(coordinates=maven_library.to_string(), repo=maven_library.repo)))
+                    if not maven_library.group_id in ["io.delta", "org.apache.spark"]:
+                        databricks_job_task.libraries.append(DatabricksLibraries(maven=DatabricksLibrariesMaven(coordinates=maven_library.to_string(), repo=maven_library.repo)))
                 for wheel_library in libraries.pythonwheel_libraries:
                     databricks_job_task.libraries.append(DatabricksLibraries(whl=wheel_library))
 
             try:
                 rtdip_version = version("rtdip-sdk")
                 databricks_job_task.libraries.append(DatabricksLibraries(pypi=DatbricksLibrariesPypi(package="rtdip-sdk[pipelines]=={}".format(rtdip_version))))
             except PackageNotFoundError as e:
@@ -217,15 +218,15 @@
         os.environ["RTDIP_PACKAGE_VERSION"] = self.pipeline_job.version
 
         # Create Databricks DBX Job
         dbx_deploy(
             workflow_name=self.pipeline_job.name,
             workflow_names=None,
             job_names=None,
-            deployment_file=Path("conf/deployment.json.j2"),
+            deployment_file=Path("conf/deployment.json"),
             environment_name="rtdip",
             requirements_file=None,
             jinja_variables_file=None,
             branch_name=None,
             tags=[],
             headers=[],
             no_rebuild=False,
```

## rtdip_sdk/pipelines/destinations/__init__.py

```diff
@@ -9,10 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .spark.delta import *
+from .spark.delta_merge import *
 from .spark.eventhub import *
 from .spark.kafka import *
 from .spark.kinesis import *
+from .spark.rest_api import *
+from .spark.pcdm_to_delta import *
```

## rtdip_sdk/pipelines/destinations/spark/delta.py

```diff
@@ -19,17 +19,18 @@
 
 from ..interfaces import DestinationInterface
 from ..._pipeline_utils.models import Libraries, MavenLibrary, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class SparkDeltaDestination(DestinationInterface):
     '''
-    The Spark Delta Source is used to write data to a Delta table. 
+    The Spark Delta Destination is used to write data to a Delta table. 
 
     Args:
+        data (DataFrame): Dataframe to be written to Delta
         table_name (str): Name of the Hive Metastore or Unity Catalog Delta Table
         options (dict): Options that can be specified for a Delta Table read operation (See Attributes table below). Further information on the options is available for [batch](https://docs.delta.io/latest/delta-batch.html#write-to-a-table){ target="_blank" } and [streaming](https://docs.delta.io/latest/delta-streaming.html#delta-table-as-a-sink){ target="_blank" }.
         mode (str): Method of writing to Delta Table - append/overwrite (batch), append/complete (stream)
         trigger (str): Frequency of the write operation
         query_name (str): Unique name for the query in associated SparkSession
 
     Attributes:
@@ -37,21 +38,23 @@
         txnAppId (str): A unique string that you can pass on each DataFrame write. (Batch & Streaming)
         txnVersion (str): A monotonically increasing number that acts as transaction version. (Batch & Streaming)
         maxRecordsPerFile (int str): Specify the maximum number of records to write to a single file for a Delta Lake table. (Batch)
         replaceWhere (str): Condition(s) for overwriting. (Batch)
         partitionOverwriteMode (str): When set to dynamic, overwrites all existing data in each logical partition for which the write will commit new data. Default is static. (Batch)
         overwriteSchema (bool str): If True, overwrites the schema as well as the table data. (Batch)
     '''
+    data: DataFrame
     table_name: str
     options: dict
     mode: str
     trigger: str
     query_name: str
 
-    def __init__(self, table_name:str, options: dict, mode: str = "append", trigger="10 seconds", query_name="DeltaDestination") -> None:
+    def __init__(self, data: DataFrame, table_name:str, options: dict, mode: str = "append", trigger="10 seconds", query_name="DeltaDestination") -> None:
+        self.data = data
         self.table_name = table_name
         self.options = options
         self.mode = mode
         self.trigger = trigger
         self.query_name = query_name
 
     @staticmethod
@@ -77,41 +80,42 @@
     
     def pre_write_validation(self):
         return True
     
     def post_write_validation(self):
         return True
 
-    def write_batch(self, df: DataFrame):
+    def write_batch(self):
         '''
         Writes batch data to Delta. Most of the options provided by the Apache Spark DataFrame write API are supported for performing batch writes on tables.
         '''
         try:
             return (
-                df
+                self.data
                 .write
                 .format("delta")
                 .mode(self.mode)
                 .options(**self.options)
                 .saveAsTable(self.table_name)
             )
 
         except Py4JJavaError as e:
             logging.exception(e.errmsg)
             raise e
         except Exception as e:
             logging.exception(str(e))
             raise e
         
-    def write_stream(self, df: DataFrame) -> DataFrame:
+    def write_stream(self):
         '''
         Writes streaming data to Delta. Exactly-once processing is guaranteed
         '''
         try:
-            query = (df
+            query = (
+                self.data
                 .writeStream
                 .trigger(processingTime=self.trigger)
                 .format("delta")
                 .queryName(self.query_name)
                 .outputMode(self.mode)
                 .options(**self.options)
                 .toTable(self.table_name)
```

## rtdip_sdk/pipelines/destinations/spark/eventhub.py

```diff
@@ -24,27 +24,30 @@
 class SparkEventhubDestination(DestinationInterface):
     '''
     This Spark destination class is used to write batch or streaming data to Eventhubs. Eventhub configurations need to be specified as options in a dictionary.
     Additionally, there are more optional configurations which can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
     If using startingPosition or endingPosition make sure to check out **Event Position** section for more details and examples.
 
     Args:
+        data (DataFrame): Dataframe to be written to Eventhub
         options (dict): A dictionary of Eventhub configurations (See Attributes table below). All Configuration options for Eventhubs can be found [here.](https://github.com/Azure/azure-event-hubs-spark/blob/master/docs/PySpark/structured-streaming-pyspark.md#event-hubs-configuration){ target="_blank" }
 
     Attributes:
         checkpointLocation (str): Path to checkpoint files. (Streaming)
         eventhubs.connectionString (str):  Eventhubs connection string is required to connect to the Eventhubs service. (Streaming and Batch)
         eventhubs.consumerGroup (str): A consumer group is a view of an entire eventhub. Consumer groups enable multiple consuming applications to each have a separate view of the event stream, and to read the stream independently at their own pace and with their own offsets. (Streaming and Batch)
         eventhubs.startingPosition (JSON str): The starting position for your Structured Streaming job. If a specific EventPosition is not set for a partition using startingPositions, then we use the EventPosition set in startingPosition. If nothing is set in either option, we will begin consuming from the end of the partition. (Streaming and Batch)
         eventhubs.endingPosition: (JSON str): The ending position of a batch query. This works the same as startingPosition. (Batch)
         maxEventsPerTrigger (long): Rate limit on maximum number of events processed per trigger interval. The specified total number of events will be proportionally split across partitions of different volume. (Stream)
     '''
+    data: DataFrame
     options: dict
 
-    def __init__(self, options: dict) -> None:
+    def __init__(self, data: DataFrame, options: dict) -> None:
+        self.data = data
         self.options = options
 
     @staticmethod
     def system_type():
         '''
         Attributes:
             SystemType (Environment): Requires PYSPARK
@@ -63,40 +66,41 @@
     
     def pre_write_validation(self):
         return True
     
     def post_write_validation(self):
         return True
 
-    def write_batch(self, df: DataFrame):
+    def write_batch(self):
         '''
         Writes batch data to Eventhubs.
         '''
         try:
             return (
-                df
+                self.data
                 .write
                 .format("eventhubs")
                 .options(**self.options)
                 .save()
             )
 
         except Py4JJavaError as e:
             logging.exception(e.errmsg)
             raise e
         except Exception as e:
             logging.exception(str(e))
             raise e
         
-    def write_stream(self, df: DataFrame):
+    def write_stream(self):
         '''
         Writes steaming data to Eventhubs.
         '''
         try:
-            query = (df
+            query = (
+                self.data
                 .writeStream
                 .format("eventhubs")
                 .options(**self.options)
                 .start()
             )
             while query.isActive:
                 if query.lastProgress:
```

## rtdip_sdk/pipelines/destinations/spark/kafka.py

```diff
@@ -24,31 +24,34 @@
 class SparkKafkaDestination(DestinationInterface):
     '''
     This Spark destination class is used to write batch or streaming data from Kafka. Required and optional configurations can be found in the Attributes tables below. 
 
     Additionally, there are more optional configurations which can be found [here.](https://spark.apache.org/docs/latest/structured-streaming-kafka-integration.html){ target="_blank" }
     
     Args:
+        data (DataFrame): Dataframe to be written to Kafka
         options (dict): A dictionary of Kafka configurations (See Attributes tables below). For more information on configuration options see [here](https://spark.apache.org/docs/latest/structured-streaming-kafka-integration.html){ target="_blank" }
 
     The following options must be set for the Kafka destination for both batch and streaming queries.
 
     Attributes:
         kafka.bootstrap.servers (A comma-separated list of host︰port): The Kafka "bootstrap.servers" configuration. (Streaming and Batch)
        
     The following configurations are optional:
 
     Attributes:
         topic (str):Sets the topic that all rows will be written to in Kafka. This option overrides any topic column that may exist in the data. (Streaming and Batch)
         includeHeaders (bool): Whether to include the Kafka headers in the row. (Streaming and Batch)
 
     '''
+    data: DataFrame
     options: dict
 
-    def __init__(self, options: dict) -> None:
+    def __init__(self, data: DataFrame, options: dict) -> None:
+        self.data = data
         self.options = options
 
     @staticmethod
     def system_type():
         '''
         Attributes:
             SystemType (Environment): Requires PYSPARK
@@ -67,40 +70,41 @@
     
     def pre_write_validation(self):
         return True
     
     def post_write_validation(self):
         return True
 
-    def write_batch(self, df: DataFrame):
+    def write_batch(self):
         '''
         Writes batch data to Kafka.
         '''
         try:
             return (
-                df
+                self.data
                 .write
                 .format("kafka")
                 .options(**self.options)
                 .save()
             )
 
         except Py4JJavaError as e:
             logging.exception(e.errmsg)
             raise e
         except Exception as e:
             logging.exception(str(e))
             raise e
         
-    def write_stream(self, df: DataFrame):
+    def write_stream(self):
         '''
         Writes steaming data to Kafka.
         '''
         try:
-            query = (df
+            query = (
+                self.data
                 .writeStream
                 .format("kafka")
                 .options(**self.options)
                 .start()
             )
             while query.isActive:
                 if query.lastProgress:
```

## rtdip_sdk/pipelines/destinations/spark/kinesis.py

```diff
@@ -20,29 +20,31 @@
 from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 class SparkKinesisDestination(DestinationInterface):
     '''
     This Kinesis destination class is used to write batch or streaming data to Kinesis. Kinesis configurations need to be specified as options in a dictionary.
     Args:
+        data (DataFrame): Dataframe to be written to Delta
         options (dict): A dictionary of Kinesis configurations (See Attributes table below). All Configuration options for Kinesis can be found [here.](https://github.com/qubole/kinesis-sql#kinesis-sink-configuration){ target="_blank" }
         mode (str): Method of writing to Kinesis - append, complete, update
         trigger (str): Frequency of the write operation
         
     Attributes:
         endpointUrl (str): Endpoint of the kinesis stream.
         awsAccessKey (str): AWS access key.
         awsSecretKey (str): AWS secret access key corresponding to the access key.
         streamName (List[str]): Name of the streams in Kinesis to write to.
     '''
     options: dict
     mode: str
     trigger: str
 
-    def __init__(self, options: dict, mode:str = "update", trigger:str= "10 seconds") -> None:
+    def __init__(self, data: DataFrame, options: dict, mode:str = "update", trigger:str= "10 seconds") -> None:
+        self.data = data
         self.options = options
         self.mode = mode
         self.trigger = trigger
 
     @staticmethod
     def system_type():
         '''
@@ -62,39 +64,40 @@
 
     def pre_write_validation(self):
         return True
 
     def post_write_validation(self):
         return True
 
-    def write_batch(self, df: DataFrame):
+    def write_batch(self):
         '''
         Writes batch data to Kinesis.
         '''
         try:
             return (
-                df
+                self.data
                 .write
                 .format("kinesis")
                 .options(**self.options)
                 .save()
             )
         except Py4JJavaError as e:
             logging.exception(e.errmsg)
             raise e
         except Exception as e:
             logging.exception(str(e))
             raise e
         
-    def write_stream(self, df: DataFrame):
+    def write_stream(self):
         '''
         Writes steaming data to Kinesis.
         '''
         try:
-            query = (df
+            query = (
+                self.data
                 .writeStream
                 .trigger(processingTime=self.trigger)
                 .format("kinesis")
                 .outputMode(self.mode)
                 .options(**self.options)
                 .start()
             )
```

## rtdip_sdk/pipelines/execute/job.py

```diff
@@ -8,26 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import List
 from dependency_injector import containers, providers
 from .container import Clients, Configs
 from .models import PipelineJob, PipelineTask, PipelineStep
 from .._pipeline_utils.models import Libraries, SystemType
 from ..sources.interfaces import SourceInterface
 from ..transformers.interfaces import TransformerInterface
 from ..destinations.interfaces import DestinationInterface
 from ..utilities.interfaces import UtilitiesInterface
 from ..secrets.models import PipelineSecret
 
-
-
 class PipelineJobExecute():
     '''
     Executes Pipeline components in their intended order as a complete data pipeline. It ensures that components dependencies are injected as needed.
 
     Args:
         job (PipelineJob): Contains the steps and tasks of a PipelineJob to be executed
         batch_job (bool): Specifies if the job is to be executed as a batch job
@@ -40,23 +39,25 @@
     def _get_provider_attributes(self, provider: providers.Factory, component: object) -> providers.Factory:
         attributes = getattr(component, '__annotations__', {}).items()
         # add spark session, if needed
         for key, value in attributes:
             # if isinstance(value, SparkSession): # TODO: fix this as value does not seem to be an instance of SparkSession
             if key == "spark":
                 provider.add_kwargs(spark=Clients.spark_client().spark_session)
+            if key == "data":
+                provider.add_kwargs(data=None)
         return provider
 
     def _get_secret_provider_attributes(self, pipeline_secret: PipelineSecret) -> providers.Factory:
         secret_provider = providers.Factory(pipeline_secret.type)
         secret_provider = self._get_provider_attributes(secret_provider, pipeline_secret.type)
         secret_provider.add_kwargs(vault=pipeline_secret.vault, key=pipeline_secret.key)
         return secret_provider
     
-    def _tasks_order(self, task_list: list[PipelineTask]):
+    def _tasks_order(self, task_list: List[PipelineTask]):
         '''
         Orders tasks within a job
         '''
         ordered_task_list = []
         temp_task_list = task_list.copy()
         while len(temp_task_list) > 0:
             for task in temp_task_list:
@@ -67,15 +68,15 @@
                     for ordered_task in ordered_task_list:
                         if task.depends_on_task == ordered_task.name:
                             ordered_task_list.append(task)
                             temp_task_list.remove(task)
                             break
         return ordered_task_list
     
-    def _steps_order(self, step_list: list[PipelineStep]):
+    def _steps_order(self, step_list: List[PipelineStep]):
         '''
         Orders steps within a task
         '''        
         ordered_step_list = []
         temp_step_list = step_list.copy()
         while len(temp_step_list) > 0:
             for step in temp_step_list:
@@ -86,15 +87,15 @@
                     ordered_step_names = [x.name for x in ordered_step_list]
                     if all(item in ordered_step_names for item in step.depends_on_step):
                         ordered_step_list.append(step)
                         temp_step_list.remove(step)
                         break
         return ordered_step_list
 
-    def _task_setup_dependency_injection(self, step_list: list[PipelineStep]):
+    def _task_setup_dependency_injection(self, step_list: List[PipelineStep]):
         '''
         Determines the dependencies to be injected into each component 
         '''
         container = containers.DynamicContainer()
         task_libraries = Libraries()
         task_step_configuration = {}
         task_spark_configuration = {}
@@ -120,18 +121,14 @@
 
         # setup container provider factories
         for step in step_list:
             # setup factory provider for component
             provider = providers.Factory(step.component)
             provider = self._get_provider_attributes(provider, step.component)
 
-            # add parameters
-            if isinstance(step.component, DestinationInterface):
-                step.component_parameters["query_name"] = step.name
-
             # get secrets
             for param_key, param_value in step.component_parameters.items():
                 if isinstance(param_value, PipelineSecret):
                     step.component_parameters[param_key] = self._get_secret_provider_attributes(param_value)().get()
                 if isinstance(param_value, dict):
                     for key, value in param_value.items():
                         if isinstance(value, PipelineSecret):
@@ -164,22 +161,22 @@
                     if task.batch_task:
                         result = factory().read_batch()
                     else:
                         result = factory().read_stream()
                         
                 # transformer components
                 elif isinstance(factory(), TransformerInterface):
-                    result = factory().transform(task_results[step.name])
+                    result = factory(data=task_results[step.name]).transform()
 
                 # destination components
                 elif isinstance(factory(), DestinationInterface):
                     if task.batch_task:
-                        result = factory().write_batch(task_results[step.name])
+                        result = factory(data=task_results[step.name], query_name=step.name).write_batch()
                     else:
-                        result = factory().write_stream(task_results[step.name])
+                        result = factory(data=task_results[step.name], query_name=step.name).write_stream()
 
                 # utilities components
                 elif isinstance(factory(), UtilitiesInterface):
                     result = factory().execute()  
 
                 # store results for steps that need it as input
                 if step.provide_output_to_step is not None:
```

## rtdip_sdk/pipelines/execute/models.py

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Type, Union, Dict
+from typing import List, Optional, Type, Union, Dict
 import re
 from pydantic import BaseConfig, BaseModel, validator
 from abc import ABCMeta
 from ..sources.interfaces import SourceInterface
 from ..transformers.interfaces import TransformerInterface
 from ..destinations.interfaces import DestinationInterface
 from ..utilities.interfaces import UtilitiesInterface
@@ -33,18 +33,18 @@
         raise ValueError('Can only contain lower case letters, numbers and underscores')
     else:
         return name
 
 class PipelineStep(BaseModel):
     name: str
     description: str
-    depends_on_step: Optional[list[str]]
+    depends_on_step: Optional[List[str]]
     component: Union[Type[SourceInterface], Type[TransformerInterface], Type[DestinationInterface], Type[UtilitiesInterface]]
     component_parameters: Optional[dict]
-    provide_output_to_step: Optional[list[str]]
+    provide_output_to_step: Optional[List[str]]
 
     class Config:
         json_encoders = {
             ABCMeta: lambda x: x.__name__,
             PipelineSecret: lambda x: {"pipeline_secret": x.dict()}
         }
 
@@ -52,16 +52,16 @@
     _validate_name = validator("name", allow_reuse=True, always=True)(validate_name)
     _validate_depends_on_step = validator("depends_on_step", allow_reuse=True, each_item=True)(validate_name)
     _validate_provide_output_to_step = validator("provide_output_to_step", allow_reuse=True, each_item=True)(validate_name)
 
 class PipelineTask(BaseModel):
     name: str
     description: str
-    depends_on_task: Optional[list[str]]
-    step_list: list[PipelineStep]
+    depends_on_task: Optional[List[str]]
+    step_list: List[PipelineStep]
     batch_task: Optional[bool]
 
     class Config:
         json_encoders = {
             ABCMeta: lambda x: x.__name__,
             PipelineSecret: lambda x: {"pipeline_secret": x.dict()}
         }
@@ -70,15 +70,15 @@
     _validate_name = validator("name", allow_reuse=True)(validate_name)
     _validate_depends_on_step = validator("depends_on_task", allow_reuse=True, each_item=True)(validate_name)
 
 class PipelineJob(BaseModel):
     name: str
     description: str
     version: str
-    task_list: list[PipelineTask]
+    task_list: List[PipelineTask]
 
     class Config:
         json_encoders = {
             ABCMeta: lambda x: x.__name__,
             PipelineSecret: lambda x: {"pipeline_secret": x.dict()}
         }
```

## rtdip_sdk/pipelines/secrets/__init__.py

```diff
@@ -9,8 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .models import *
-from .databricks import *
+from .databricks import *
+from .hashicorp_vault import *
+from .azure_key_vault import *
```

## rtdip_sdk/pipelines/transformers/__init__.py

```diff
@@ -9,9 +9,11 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .spark.binary_to_string import *
-from .spark.opc_publisher_json_to_opcua import *
-from .spark.opcua_to_process_control_data_model import *
+from .spark.opc_publisher_json_to_pcdm import *
+from .spark.fledge_json_to_pcdm import *
+from .spark.ssip_pi_binary_file_to_pcdm import *
+from .spark.ssip_pi_binary_json_to_pcdm import *
```

## rtdip_sdk/pipelines/transformers/spark/__init__.py

```diff
@@ -0,0 +1,36 @@
+00000000: 2320 436f 7079 7269 6768 7420 3230 3232  # Copyright 2022
+00000010: 2052 5444 4950 0a23 0a23 204c 6963 656e   RTDIP.#.# Licen
+00000020: 7365 6420 756e 6465 7220 7468 6520 4170  sed under the Ap
+00000030: 6163 6865 204c 6963 656e 7365 2c20 5665  ache License, Ve
+00000040: 7273 696f 6e20 322e 3020 2874 6865 2022  rsion 2.0 (the "
+00000050: 4c69 6365 6e73 6522 293b 0a23 2079 6f75  License");.# you
+00000060: 206d 6179 206e 6f74 2075 7365 2074 6869   may not use thi
+00000070: 7320 6669 6c65 2065 7863 6570 7420 696e  s file except in
+00000080: 2063 6f6d 706c 6961 6e63 6520 7769 7468   compliance with
+00000090: 2074 6865 204c 6963 656e 7365 2e0a 2320   the License..# 
+000000a0: 596f 7520 6d61 7920 6f62 7461 696e 2061  You may obtain a
+000000b0: 2063 6f70 7920 6f66 2074 6865 204c 6963   copy of the Lic
+000000c0: 656e 7365 2061 740a 230a 2320 2020 2020  ense at.#.#     
+000000d0: 2068 7474 703a 2f2f 7777 772e 6170 6163   http://www.apac
+000000e0: 6865 2e6f 7267 2f6c 6963 656e 7365 732f  he.org/licenses/
+000000f0: 4c49 4345 4e53 452d 322e 300a 230a 2320  LICENSE-2.0.#.# 
+00000100: 556e 6c65 7373 2072 6571 7569 7265 6420  Unless required 
+00000110: 6279 2061 7070 6c69 6361 626c 6520 6c61  by applicable la
+00000120: 7720 6f72 2061 6772 6565 6420 746f 2069  w or agreed to i
+00000130: 6e20 7772 6974 696e 672c 2073 6f66 7477  n writing, softw
+00000140: 6172 650a 2320 6469 7374 7269 6275 7465  are.# distribute
+00000150: 6420 756e 6465 7220 7468 6520 4c69 6365  d under the Lice
+00000160: 6e73 6520 6973 2064 6973 7472 6962 7574  nse is distribut
+00000170: 6564 206f 6e20 616e 2022 4153 2049 5322  ed on an "AS IS"
+00000180: 2042 4153 4953 2c0a 2320 5749 5448 4f55   BASIS,.# WITHOU
+00000190: 5420 5741 5252 414e 5449 4553 204f 5220  T WARRANTIES OR 
+000001a0: 434f 4e44 4954 494f 4e53 204f 4620 414e  CONDITIONS OF AN
+000001b0: 5920 4b49 4e44 2c20 6569 7468 6572 2065  Y KIND, either e
+000001c0: 7870 7265 7373 206f 7220 696d 706c 6965  xpress or implie
+000001d0: 642e 0a23 2053 6565 2074 6865 204c 6963  d..# See the Lic
+000001e0: 656e 7365 2066 6f72 2074 6865 2073 7065  ense for the spe
+000001f0: 6369 6669 6320 6c61 6e67 7561 6765 2067  cific language g
+00000200: 6f76 6572 6e69 6e67 2070 6572 6d69 7373  overning permiss
+00000210: 696f 6e73 2061 6e64 0a23 206c 696d 6974  ions and.# limit
+00000220: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
+00000230: 204c 6963 656e 7365 2e0a                  License..
```

## rtdip_sdk/pipelines/transformers/spark/binary_to_string.py

```diff
@@ -18,22 +18,24 @@
 from ..._pipeline_utils.models import Libraries, SystemType
 
 class BinaryToStringTransformer(TransformerInterface):
     '''
     Converts a dataframe body column from a binary to a string.
 
     Args:
+        data (DataFrame): Dataframe to be transformed
         source_column_name (str): Spark Dataframe column containing the Binary data
         target_column_name (str): Spark Dataframe column name to be used for the String data
     '''
-
+    data: DataFrame
     source_column_name: str
     target_column_name: str
 
-    def __init__(self, source_column_name: str, target_column_name: str) -> None:
+    def __init__(self, data: DataFrame, source_column_name: str, target_column_name: str) -> None:
+        self.data = data
         self.source_column_name = source_column_name
         self.target_column_name = target_column_name
 
     @staticmethod
     def system_type():
         '''
         Attributes:
@@ -52,19 +54,16 @@
     
     def pre_transform_validation(self):
         return True
     
     def post_transform_validation(self):
         return True
 
-    def transform(self, df: DataFrame) -> DataFrame:
+    def transform(self) -> DataFrame:
         '''
-        Args:
-            df (DataFrame): A dataframe containing a binary column.
-
         Returns:
             DataFrame: A dataframe with the body column converted to string.
         '''
         return (
-            df
-            .withColumn(self.target_column_name, df[self.source_column_name].cast("string"))
+            self.data
+            .withColumn(self.target_column_name, self.data[self.source_column_name].cast("string"))
         )
```

## rtdip_sdk/pipelines/utilities/__init__.py

```diff
@@ -11,8 +11,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .spark.delta_table_create import *
 from .spark.delta_table_optimize import *
 from .spark.delta_table_vacuum import *
+from .spark.configuration import *
 from .azure.adls_gen2_acl import *
```

## rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from typing import Dict
+from typing import Dict, List
 
 from pydantic import BaseModel
 
 from ..interfaces import UtilitiesInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
@@ -41,18 +41,18 @@
     bucket_name: str
     aws_access_key_id: str
     aws_secret_access_key: str
     aws_session_token: str
     sid: str
     effect: str
     principal: str
-    action: list[str]
-    resource: list[str]
+    action: List[str]
+    resource: List[str]
 
-    def __init__(self, bucket_name: str, aws_access_key_id: str, aws_secret_access_key: str, aws_session_token: str, sid: str, principal: str, effect: str, action: list[str], resource: list[str]) -> None:
+    def __init__(self, bucket_name: str, aws_access_key_id: str, aws_secret_access_key: str, aws_session_token: str, sid: str, principal: str, effect: str, action: List[str], resource: List[str]) -> None:
         self.bucket_name = bucket_name
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_session_token = aws_session_token
         self.sid = sid
         self.effect = effect
         self.principal = principal
```

## rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from typing import Dict
+from typing import Dict, Union
 
 from ..interfaces import UtilitiesInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
 from azure.storage.filedatalake import DataLakeServiceClient, FileSystemClient
 from azure.core.credentials import TokenCredential, AzureNamedKeyCredential, AzureSasCredential
@@ -36,24 +36,24 @@
         parent_folder_permissions (optional, str): Folder Permissions to Assign to parent directories. Parent Folder ACLs not set if None
         root_folder_permissions (optional, str): Folder Permissions to Assign to root directory. Root Folder ACL not set if None
         set_as_default_acl (bool, optional): Sets the ACL as the default ACL on the folder
         create_directory_if_not_exists (bool, optional): Creates the directory(and Parent Directories) if it does not exist
     ''' 
     storage_account: str
     container: str
-    credential: str | Dict[str, str] | AzureNamedKeyCredential | AzureSasCredential | TokenCredential | None
+    credential: Union[str, Dict[str, str], AzureNamedKeyCredential, AzureSasCredential, TokenCredential, None]
     directory: str
     group_object_id: str
     folder_permissions: str
     parent_folder_permissions: str
     root_folder_permissions: str
     set_as_default_acl: bool
     create_directory_if_not_exists: bool
 
-    def __init__(self, storage_account: str, container: str, credential: str | Dict[str, str] | AzureNamedKeyCredential | AzureSasCredential | TokenCredential | None, directory: str, group_object_id: str, folder_permissions: str = "r-x", parent_folder_permissions: str | None = "r-x", root_folder_permissions: str | None = "r-x", set_as_default_acl: bool = True, create_directory_if_not_exists: bool = True) -> None:
+    def __init__(self, storage_account: str, container: str, credential: Union[str, Dict[str, str], AzureNamedKeyCredential, AzureSasCredential, TokenCredential, None], directory: str, group_object_id: str, folder_permissions: str = "r-x", parent_folder_permissions: Union[str, None] = "r-x", root_folder_permissions: Union[str, None] = "r-x", set_as_default_acl: bool = True, create_directory_if_not_exists: bool = True) -> None:
         self.storage_account = storage_account
         self.container = container
         self.credential = credential
         self.directory = directory
         self.group_object_id = group_object_id
         self.folder_permissions = folder_permissions
         self.parent_folder_permissions = parent_folder_permissions
```

## rtdip_sdk/pipelines/utilities/spark/configuration.py

```diff
@@ -9,34 +9,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+from typing import List
 from pyspark.sql import SparkSession
 from pyspark.sql.types import StructField
 from py4j.protocol import Py4JJavaError
-from delta.tables import DeltaTable
 
 from ..interfaces import UtilitiesInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 
 class SparkConfigurationUtility(UtilitiesInterface):
     '''
     Sets configuration key value pairs to a Spark Session
 
     Args:
         spark (SparkSession): Spark Session required to read data from cloud storage
         config (dict): Dictionary of spark configuration to be applied to the spark session
     ''' 
     spark: SparkSession
     config: dict
-    columns: list[StructField]
-    partitioned_by: list[str]
+    columns: List[StructField]
+    partitioned_by: List[str]
     location: str
     properties: dict
     comment: str
 
     def __init__(self, spark: SparkSession, config: dict) -> None:
         self.spark = spark
         self.config = config
```

## rtdip_sdk/pipelines/utilities/spark/delta_table_create.py

```diff
@@ -9,45 +9,75 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+from typing import List, Optional
+from pydantic import BaseModel
 from pyspark.sql import SparkSession
 from pyspark.sql.types import StructField
 from py4j.protocol import Py4JJavaError
 from delta.tables import DeltaTable
 
 from ..interfaces import UtilitiesInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
 
+class DeltaTableColumn(BaseModel):
+    name: str
+    type: str
+    nullable: bool
+    metadata: Optional[dict]
+
 class DeltaTableCreateUtility(UtilitiesInterface):
     '''
     Creates a Delta Table in a Hive Metastore or in Databricks Unity Catalog.
 
     Args:
         spark (SparkSession): Spark Session required to read data from cloud storage
         table_name (str): Name of the table, including catalog and schema if table is to be created in Unity Catalog
-        columns (list[StructField]): List of columns and their related column properties
+        columns (list[DeltaTableColumn]): List of columns and their related column properties
         partitioned_by (list[str], optional): List of column names to partition the table by
         location (str, optional): Path to storage location
         properties (dict, optional): Propoerties that can be specified for a Delta Table. Further information on the options available are [here](https://docs.databricks.com/delta/table-properties.html#delta-table-properties)
         comment (str, optional): Provides a comment on the table metadata
+
+    Example:
+        ```python
+        from rtdip_sdk.pipelines.utilities.spark.delta_table_create import DeltaTableCreateUtility, DeltaTableColumn
+
+        table_create_utility = DeltaTableCreateUtility(
+            spark=spark_session,
+            table_name="delta_table",
+            columns=[
+                DeltaTableColumn(name="EventDate", type="date", nullable=False, metadata={"delta.generationExpression": "CAST(EventTime AS DATE)"}),
+                DeltaTableColumn(name="TagName", type="string", nullable=False),
+                DeltaTableColumn(name="EventTime", type="timestamp", nullable=False),
+                DeltaTableColumn(name="Status", type="string", nullable=True),
+                DeltaTableColumn(name="Value", type="float", nullable=True)
+            ],
+            partitioned_by=["EventDate"],
+            properties={"delta.logRetentionDuration": "7 days", "delta.enableChangeDataFeed": "true"},
+            comment="Creation of Delta Table"
+        )
+
+        result = table_create_utility.execute()       
+        ```
     ''' 
     spark: SparkSession
     table_name: str
-    columns: list[StructField]
-    partitioned_by: list[str]
+    columns: List[DeltaTableColumn]
+    partitioned_by: List[str]
     location: str
     properties: dict
     comment: str
 
-    def __init__(self, spark: SparkSession, table_name: str, columns: list[StructField], partitioned_by: list[str] = None, location: str = None, properties: dict = None, comment: str = None) -> None:
+    def __init__(self, spark: SparkSession, table_name: str, columns: List[StructField], partitioned_by: List[str] = None, location: str = None, properties: dict = None, comment: str = None) -> None:
         self.spark = spark
         self.table_name = table_name
         self.columns = columns
         self.partitioned_by = partitioned_by
         self.location = location
         self.properties = properties
         self.comment = comment
@@ -68,19 +98,21 @@
     
     @staticmethod
     def settings() -> dict:
         return {}
 
     def execute(self) -> bool:
         try:
+            columns = [StructField.fromJson(column.dict()) for column in self.columns]
+
             delta_table = (
                 DeltaTable
                 .createIfNotExists(self.spark)
                 .tableName(self.table_name)
-                .addColumns(self.columns)
+                .addColumns(columns)
             )
 
             if self.partitioned_by is not None:
                 delta_table = delta_table.partitionedBy(self.partitioned_by)
 
             if self.location is not None:
                 delta_table = delta_table.location(self.location)
```

## rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from typing import Optional
+from typing import List, Optional
 from pyspark.sql import SparkSession
 from py4j.protocol import Py4JJavaError
 from delta.tables import DeltaTable
 
 from ..interfaces import UtilitiesInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.constants import DEFAULT_PACKAGES
@@ -31,17 +31,17 @@
         table_name (str): Name of the table, including catalog and schema if table is to be created in Unity Catalog
         where (str, optional): Apply a partition filter to limit optimize to specific partitions. Example, "date='2021-11-18'" or "EventDate<=current_date()"
         zorder_by (list[str], optional): List of column names to zorder the table by. For more information, see [here.](https://docs.delta.io/latest/optimizations-oss.html#optimize-performance-with-file-management&language-python)
     ''' 
     spark: SparkSession
     table_name: str
     where: Optional[str]
-    zorder_by: Optional[list[str]]
+    zorder_by: Optional[List[str]]
 
-    def __init__(self, spark: SparkSession, table_name: str, where: str = None, zorder_by: list[str] = None) -> None:
+    def __init__(self, spark: SparkSession, table_name: str, where: str = None, zorder_by: List[str] = None) -> None:
         self.spark = spark
         self.table_name = table_name
         self.where = where
         self.zorder_by = zorder_by
 
     @staticmethod
     def system_type():
```

## Comparing `rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py` & `rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_pcdm.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,36 +9,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pyspark.sql import DataFrame
-from pyspark.sql.functions import to_timestamp, col, regexp_replace, when, lit, coalesce
+from pyspark.sql.functions import from_json, col, explode, to_timestamp, when, lit, coalesce
+from pyspark.sql.types import ArrayType, StringType
 
 from ..interfaces import TransformerInterface
 from ..._pipeline_utils.models import Libraries, SystemType
+from ..._pipeline_utils.spark import OPC_PUBLISHER_SCHEMA
 
-class OPCUAToProcessControlDataModelTransformer(TransformerInterface):
+class OPCPublisherJsonToPCDMTransformer(TransformerInterface):
     '''
-    Converts a Spark Dataframe column from a structured OPC UA schema to the RTDIP Process Control Data Model.
+    Converts a Spark Dataframe column containing a json string created by OPC Publisher to the Process Control Data Model
 
     Args:
-        source_column_name (str): Spark Dataframe column containing the OPC UA data.
+        data (DataFrame): Dataframe containing the column with Json OPC UA data
+        source_column_name (str): Spark Dataframe column containing the OPC Publisher Json OPC UA data
+        multiple_rows_per_message (bool): Each Dataframe Row contains an array of/multiple OPC UA messages. The list of Json will be exploded into rows in the Dataframe.
         status_null_value (str): If populated, will replace null values in the Status column with the specified value.
         timestamp_formats (list[str]): Specifies the timestamp formats to be used for converting the timestamp string to a Timestamp Type. For more information on formats, refer to this [documentation.](https://spark.apache.org/docs/latest/sql-ref-datetime-pattern.html)
-    '''
 
+    '''
+    data: DataFrame
     source_column_name: str
+    multiple_rows_per_message: bool
     status_null_value: str
+    change_type_value: str
     timestamp_formats: list
 
-    def __init__(self, source_column_name: str = "OPCUA", status_null_value: str = None, timestamp_formats: list = ["yyyy-MM-dd'T'HH:mm:ss.SSSX", "yyyy-MM-dd'T'HH:mm:ssX"]) -> None: # NOSONAR
+    def __init__(self, data: DataFrame, source_column_name: str, multiple_rows_per_message: bool = True, status_null_value: str = None, change_type_value: str = "insert", timestamp_formats: list = ["yyyy-MM-dd'T'HH:mm:ss.SSSX", "yyyy-MM-dd'T'HH:mm:ssX"]) -> None: # NOSONAR
+        self.data = data
         self.source_column_name = source_column_name
+        self.multiple_rows_per_message = multiple_rows_per_message
         self.status_null_value = status_null_value
+        self.change_type_value = change_type_value
         self.timestamp_formats = timestamp_formats
 
     @staticmethod
     def system_type():
         '''
         Attributes:
             SystemType (Environment): Requires PYSPARK
@@ -56,30 +66,40 @@
     
     def pre_transform_validation(self):
         return True
     
     def post_transform_validation(self):
         return True
 
-    def transform(self, df: DataFrame) -> DataFrame:
+    def transform(self) -> DataFrame:
         '''
-        Args:
-            df (DataFrame): A dataframe containing the column with Json OPC UA data
-
         Returns:
-            DataFrame: A dataframe with the specified column converted to OPC UA
+            DataFrame: A dataframe with the specified column converted to PCDM
         '''
+        if self.multiple_rows_per_message:
+            df = (self.data
+                .withColumn(self.source_column_name, from_json(col(self.source_column_name), ArrayType(StringType())))
+                .withColumn(self.source_column_name, explode(self.source_column_name))
+            )
+        else:
+            df = (self.data
+                .withColumn(self.source_column_name, from_json(col(self.source_column_name), StringType()))
+            )
 
         df = (df
-            .withColumn("TagName", (col("{}.DisplayName".format(self.source_column_name)))) # Will be in payload directly
-            .withColumn("EventTime", coalesce(*[to_timestamp(col("{}.Value.SourceTimestamp".format(self.source_column_name)), f) for f in self.timestamp_formats]))
-            .withColumn("EventDate", col("EventTime").cast("date"))     
-            .withColumn("Value", col("{}.Value.Value".format(self.source_column_name)))
+            .withColumn("OPCUA", from_json(col(self.source_column_name), OPC_PUBLISHER_SCHEMA))
+            .withColumn("TagName", (col("OPCUA.DisplayName")))
+            .withColumn("EventTime", coalesce(*[to_timestamp(col("OPCUA.Value.SourceTimestamp"), f) for f in self.timestamp_formats]))   
+            .withColumn("Value", col("OPCUA.Value.Value"))
+            .withColumn("ValueType", when(col("Value").cast("float").isNotNull(), "float")
+                                    .when(col("Value").cast("float").isNull(), "string")
+                                    .otherwise("unknown"))
+            .withColumn("ChangeType", lit(self.change_type_value))                              
         )
 
-        status_col_name = "{}.Value.StatusCode.Symbol".format(self.source_column_name)
+        status_col_name = "OPCUA.Value.StatusCode.Symbol"
         if self.status_null_value != None:
             df = df.withColumn("Status", when(col(status_col_name).isNotNull(), col(status_col_name)).otherwise(lit(self.status_null_value)))
         else:
             df = df.withColumn("Status", col(status_col_name))
 
-        return df.select("EventDate", "TagName", "EventTime", "Status", "Value")
+        return df.select("TagName", "EventTime", "Status", "Value", "ValueType", "ChangeType")
```

## Comparing `rtdip_sdk-0.2.2.dist-info/LICENSE.md` & `rtdip_sdk-0.3.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `rtdip_sdk-0.2.2.dist-info/METADATA` & `rtdip_sdk-0.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: rtdip-sdk
-Version: 0.2.2
+Version: 0.3.0
 Home-page: https://github.com/rtdip/core
 Project-URL: Issue Tracker, https://github.com/rtdip/core/issues
 Project-URL: Source, https://github.com/rtdip/core/
 Project-URL: Documentation, https://www.rtdip.io/
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: databricks-sql-connector (==2.4.0)
-Requires-Dist: azure-identity (==1.11.0)
-Requires-Dist: pyodbc (==4.0.34)
+Requires-Dist: databricks-sql-connector (==2.5.1)
+Requires-Dist: azure-identity (==1.12.0)
+Requires-Dist: pyodbc (==4.0.39)
 Requires-Dist: pandas (==1.5.2)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jinjasql (==0.1.8)
+Requires-Dist: importlib-metadata (>=1.0.0)
+Requires-Dist: semver (==3.0.0)
 Provides-Extra: pipelines
 Requires-Dist: dependency-injector (==4.41.0) ; extra == 'pipelines'
-Requires-Dist: dbx (==0.8.10) ; extra == 'pipelines'
-Requires-Dist: pydantic (==1.10.6) ; extra == 'pipelines'
+Requires-Dist: dbx (==0.8.11) ; extra == 'pipelines'
+Requires-Dist: pydantic (==1.10.7) ; extra == 'pipelines'
 Requires-Dist: azure-storage-file-datalake (==12.10.1) ; extra == 'pipelines'
-Requires-Dist: boto3 (==1.26.118) ; extra == 'pipelines'
+Requires-Dist: boto3 (==1.26.123) ; extra == 'pipelines'
+Requires-Dist: hvac (==1.1.0) ; extra == 'pipelines'
+Requires-Dist: azure-keyvault-secrets (==4.7.0) ; extra == 'pipelines'
 Provides-Extra: pyspark
-Requires-Dist: pyspark (==3.3.2) ; extra == 'pyspark'
-Requires-Dist: delta-spark (==2.3.0) ; extra == 'pyspark'
+Requires-Dist: pyspark (<3.4.0,>=3.3.0) ; extra == 'pyspark'
+Requires-Dist: delta-spark (<2.4.0,>=2.2.0) ; extra == 'pyspark'
 
 <p align="center"><img src=https://raw.githubusercontent.com/rtdip/core/develop/docs/getting-started/images/rtdip-horizontal-color.png alt="rtdip" width=50% height=50%/></p>
 
 # What is the RTDIP SDK?
 
 ​​**Real Time Data Ingestion Platform (RTDIP) SDK** is a python software development kit built to provide users, data scientists and developers with the ability to interact with components of the Real Time Data Ingestion Platform, including:
```

## Comparing `rtdip_sdk-0.2.2.dist-info/RECORD` & `rtdip_sdk-0.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,111 @@
 rtdip_sdk/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
+rtdip_sdk/_sdk_utils/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
+rtdip_sdk/_sdk_utils/compare_versions.py,sha256=pr2PUYxd1Qx4gPcrRRdQk7WthLeiN2exOC7NarJ7EDs,1068
 rtdip_sdk/authentication/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/authentication/authenticate.py,sha256=GPd7ftHVZjrGq3n9Gj7dwEjrSxpCwlSODzvQggIpfts,7210
+rtdip_sdk/data_models/meters/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/data_models/meters/ami_meters.py,sha256=UHeWNb40jFQSU3hMQgE0yQO0hn3WS0Mv6njchM1Fplg,6131
+rtdip_sdk/data_models/meters/utils/CreateMetaDataObject.py,sha256=awaSBsbwTEfKq2w8R92JlhVtM-QPmAm2LiaPqYGE860,2161
+rtdip_sdk/data_models/meters/utils/CreateUsageObject.py,sha256=BNWQ5XatXNUCiY9iNG6fqKJQQcMTNidL7np3Q3MIC0E,1137
+rtdip_sdk/data_models/meters/utils/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/data_models/meters/utils/transform.py,sha256=-NdBlngglKwi5wfqhSHDyNq1QOEq7M2Kf38cMGIns_k,4524
+rtdip_sdk/data_models/meters/utils/transformers.py,sha256=jYHnY_27f-4jQ00IANO_r5uiIrfYWZnVBfzUe88UYKE,2804
+rtdip_sdk/data_models/meters/utils/utils.py,sha256=2-W-86KUMWmmTjwHtOqDLvY9MI3EC-1GUdictDJ4vPs,4852
+rtdip_sdk/data_models/transformers/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/data_models/transformers/london_smart_meter_transformer_2_usage.py,sha256=Pabgeq2eX-GLhxSIkUqY1qYJEYCclcCTxlMQP7vIMJ8,1743
+rtdip_sdk/data_models/weather/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/data_models/weather/weather_models.py,sha256=olpTpO1fTEiY6LrH_4WSP55O0HTPjXe7Cylx2VKjr2Q,5677
+rtdip_sdk/data_models/weather/utils/CreateWeatherObject.py,sha256=Mu9mRGCoS8nUxg5Jl56X2gVluDCCAHquLbMSWbWd4xI,2876
+rtdip_sdk/data_models/weather/utils/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/functions/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
-rtdip_sdk/functions/_query_builder.py,sha256=6lhKs3NK0sKAWAXph2jmGhzl5mCa8qneB5kT30Q3s6g,9846
-rtdip_sdk/functions/interpolate.py,sha256=R5mAUWMU24oyC_DfbL3GoJE0nx4ddyBuYeTNCh2tdR8,2908
-rtdip_sdk/functions/metadata.py,sha256=DNy2X--PGw5ERj5sA2KuCJxChJ3uLN8TTgeIdLLWRcg,2293
-rtdip_sdk/functions/raw.py,sha256=zFIsYyGdgE4GfLyidjNUH5CkgXfnNHVrLGsXV5iVeUA,2626
-rtdip_sdk/functions/resample.py,sha256=NT3bA1Ia8u834C1HC9dUQ1AaLy4PN2Yc51KN1Qee0wc,3052
-rtdip_sdk/functions/time_weighted_average.py,sha256=KvrGxZUyb1XkXg9xbzQVSzgad-F4T4LePhnsJZ-6OXY,9434
+rtdip_sdk/functions/_query_builder.py,sha256=ONt7tCNuUWdSXMFkj7X7f82RwEtfFmyveYFkm3i8hTE,14466
+rtdip_sdk/functions/interpolate.py,sha256=B0GRchHArXiZfH2htHRiXV4PCyvgYyEiMmzt96s4EkA,3048
+rtdip_sdk/functions/interpolation_at_time.py,sha256=4fr3P4KX__Frwdj575E5Vd6XnsJBF_mJyD4tfMe4PPg,2546
+rtdip_sdk/functions/metadata.py,sha256=7eIQZJ-cf4V-YbUZljiQokxQkdtRuc0DSTeh8xsV3sA,2292
+rtdip_sdk/functions/raw.py,sha256=CbPzO9-vOBTEF6err3tY7QRRu3n3o8Pyvg2UKKwPTr4,2766
+rtdip_sdk/functions/resample.py,sha256=Pzi1lqqx3IDqgHaXZYA4M8FPigQxbChvT6q5bOZJQOo,3192
+rtdip_sdk/functions/time_weighted_average.py,sha256=pUL1EkfW_X9UO5ElkRFT1V31rWg2rT_C0exPnVSt4BU,9528
 rtdip_sdk/odbc/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/odbc/connection_interface.py,sha256=7FnrbBSvsCGNjutxutGvFYZfktY2hcDhyfLnCcCh-hQ,934
 rtdip_sdk/odbc/cursor_interface.py,sha256=JEWb1W72PXibztG8koTj-tOuejvoDsJh8k7mFvH-C6k,952
-rtdip_sdk/odbc/db_sql_connector.py,sha256=I6d8K3mm_ykIPh8-EjkNQDmdRGvCdFyROHsl8ErBY-g,3498
+rtdip_sdk/odbc/db_sql_connector.py,sha256=NSZlQ2NyDiepCvyOBtePC7ibBH1xGjIz_tynhpVWWtI,3415
 rtdip_sdk/odbc/pyodbc_sql_connector.py,sha256=9Ap6Qh73enYXS6GnmrybN2mVH2CUCWCwUjxq7mrmtaQ,4228
-rtdip_sdk/odbc/turbodbc_sql_connector.py,sha256=Uv4DRn1y1QOiggN5nAVPB3RrS1hUuI56OsAAHspZqq0,4432
+rtdip_sdk/odbc/turbodbc_sql_connector.py,sha256=8qWNvbg9B43e4yKN82jFY5Zee1dlweYXk2WgL68Yn0A,4359
 rtdip_sdk/pipelines/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/pipelines/interfaces.py,sha256=RdiawOPSQ5Vxch6htM03MMKhyMBtU4RVtnTdl0jVBBU,1035
 rtdip_sdk/pipelines/_pipeline_utils/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/_pipeline_utils/constants.py,sha256=xFVUWjA89a-IwWy0SeeD2ZyNYpB9i5MOyglUhMMVxn4,1745
-rtdip_sdk/pipelines/_pipeline_utils/models.py,sha256=tvviN-pD1TBZQ_9t2icYGTP0LRnslore8NHlYaALlCw,2434
-rtdip_sdk/pipelines/_pipeline_utils/spark.py,sha256=SJYHa2HzZgj0VkDzYxqOC30zaYPaDC7IQ6yj25XyPDU,5327
+rtdip_sdk/pipelines/_pipeline_utils/constants.py,sha256=gk1u81XT_DO8LNMddXq1da7TwpMzUjQy7iKaRBVQWv0,2332
+rtdip_sdk/pipelines/_pipeline_utils/models.py,sha256=8vcc3PItz_gDEchZVcTXQyJEpjInE_x0QekrwR1lvqk,2439
+rtdip_sdk/pipelines/_pipeline_utils/spark.py,sha256=v_xnsJIANhuvFnSllcXcUyZO8axzhMUhskMqWG7kimg,5954
 rtdip_sdk/pipelines/converters/__init__.py,sha256=hwO8Ac698lsn720_wfiyk7ss4cPWCFHMuNgJ7-YdMWQ,603
 rtdip_sdk/pipelines/converters/interfaces.py,sha256=wvm5Doxre6XJjc1nE9-l047MR4JjvyPCeGDIO3kUCt4,697
 rtdip_sdk/pipelines/converters/pipeline_job_json.py,sha256=8gZWk6FzsFZ3J2FjYz2Q3htpHxlXdSVHLJdqlJU6KRc,3442
 rtdip_sdk/pipelines/deploy/__init__.py,sha256=8wwgnaMDh2h_Y6kMrHKXFsXBdPASIeoLssPDgHyVSgA,630
-rtdip_sdk/pipelines/deploy/databricks.py,sha256=vNc40X7ag6uj68ULgDGF-rdNx0cGo6mYNYldLkvyk7c,13207
+rtdip_sdk/pipelines/deploy/databricks.py,sha256=aPxzjvSiN65pOUQuRA1l2cOjb-3nf1cwGrdILSahC_o,13295
 rtdip_sdk/pipelines/deploy/interfaces.py,sha256=s6FM0UjSFkF1LhPvBF52zOExuIIItXJql-1j9qiXvnQ,751
+rtdip_sdk/pipelines/deploy/dbx/.gitignore,sha256=RF2fvC1GIAYAXY9YwOfFdTFNxlRqI40x6e2WTSdo6ZA,416
 rtdip_sdk/pipelines/deploy/dbx/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/setup.py,sha256=7VEAGmbQ_qAd73g9T85DitK1EvObixrzoatjiufbeDU,1114
 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
+rtdip_sdk/pipelines/deploy/dbx/conf/deployment.json,sha256=qjq2Rsy0_fgCQ4tlhCwROJKHlwFmwaydNXG2qbO2n_0,43
 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py,sha256=f7q1C5OvcHNrRNp1iAU461DKF4XnVi-dOFVs19Oj7bQ,3310
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py,sha256=SfSnn2-D-sYWYobaRUQwFGvDg961r13oIjnEno3xWQM,1695
 rtdip_sdk/pipelines/deploy/models/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/models/databricks.py,sha256=BaVaRGHGoGiUiG_1ouBuAUOHc4t0nLCaLIIIj56Annc,7897
-rtdip_sdk/pipelines/destinations/__init__.py,sha256=oPnFMRb6Y1__25uf5yfR_ETeKDGfvn-hUAQupySWuV8,684
+rtdip_sdk/pipelines/destinations/__init__.py,sha256=mVlSEqtT8T_JaLF4GFOVmCKyQbDSINMU3uUt_ewmsrw,782
 rtdip_sdk/pipelines/destinations/interfaces.py,sha256=IjIYhBInHDAvtf52Z7zcvux9q0_ni8KkHj5kD1I6LP4,427
 rtdip_sdk/pipelines/destinations/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/destinations/spark/delta.py,sha256=WjMzdnEyZUVOS0DG-YoqVZ1FvKf1qVbOikl2VDXMi9g,5112
-rtdip_sdk/pipelines/destinations/spark/eventhub.py,sha256=12C5NvjzSctJytKv7iBoR5Qc1zxK0CM41JZQqQ5Ycqc,4781
-rtdip_sdk/pipelines/destinations/spark/kafka.py,sha256=DEZApzSLTamM7sqiPKxVLpWNpOBZY2O1ysrTYSI24AQ,3903
-rtdip_sdk/pipelines/destinations/spark/kinesis.py,sha256=gx6BhFe_M797mp-j_OMDmTooI8HoBLq2ZqBTi0Mzk8I,3659
+rtdip_sdk/pipelines/destinations/spark/delta.py,sha256=PndLlNwal7Zz6kPRejFoDKHC3bYt9LN-zo1ICI8c90g,5226
+rtdip_sdk/pipelines/destinations/spark/delta_merge.py,sha256=noNppk4zHngKDSYt-Us9YkVaMKIgO0kZKV1Ev3Iniak,11510
+rtdip_sdk/pipelines/destinations/spark/eventhub.py,sha256=W2sXuk_sNXeIgo-W7yIQMFr5gimiF7EPK-WMV28qbXo,4906
+rtdip_sdk/pipelines/destinations/spark/kafka.py,sha256=iQTMM0Q3pZweMe0yRUf-nkMs5mO7UVuRfEm0_f46NN4,4025
+rtdip_sdk/pipelines/destinations/spark/kinesis.py,sha256=CS-KWaaAiU28f9pZ33s0GgPxligHv2CJV_eQtvNrzk0,3761
+rtdip_sdk/pipelines/destinations/spark/pcdm_to_delta.py,sha256=708nmdyq3Ul9ZFrv9Qh3FNnLllYNRLuquj0Hml__Wvc,10204
+rtdip_sdk/pipelines/destinations/spark/rest_api.py,sha256=_Zwuf_AR-yesg2W7FhULoxV5ZACysc8NNgEzCjn12Bk,7050
 rtdip_sdk/pipelines/execute/__init__.py,sha256=NrQH7iM8LSCgnkbVmIWx_Gd67SxbdnJYGacS1iKshM0,611
 rtdip_sdk/pipelines/execute/container.py,sha256=0u-YsNbgMD2iyZob2W_OuxrVuGlpqGUm4Atz1jg6cA4,1448
-rtdip_sdk/pipelines/execute/job.py,sha256=UZV3mA0pVvauPcc6q4Pgyws34pxEKjaBZUOt3IKoIkE,8378
-rtdip_sdk/pipelines/execute/models.py,sha256=TQxpDl0G3EuciPREYzOo_C0gv_HvE-1uzwze9-WYdlA,3037
-rtdip_sdk/pipelines/secrets/__init__.py,sha256=wz5k9b3FvKaXT_Yxy374H_ZNqUgV5ekhffRPpSrHUC0,618
+rtdip_sdk/pipelines/execute/job.py,sha256=IEh8dpZLTXpJO0GLIJh-JI9RwDNSpsjw_DGYPmc4f3A,8373
+rtdip_sdk/pipelines/execute/models.py,sha256=HQ5eX-qyDWctTmHPxD7E9P6WumovkShWmwby5mQ6nKE,3043
+rtdip_sdk/pipelines/secrets/__init__.py,sha256=_OO-leJETl5BfO8VE9N9qePNiTS1ZID9bFiogXHN24M,680
+rtdip_sdk/pipelines/secrets/azure_key_vault.py,sha256=7voj8ObGlkbsCt5lRl2jE3Kwbwvi8pSqb1yZ8PqPYK4,2935
 rtdip_sdk/pipelines/secrets/databricks.py,sha256=pXVC_wtPVBbLUqwd04hISiAk273DLCDtmOXz4CtNgmQ,2227
+rtdip_sdk/pipelines/secrets/hashicorp_vault.py,sha256=vNjxFNyNnUqtKWnS6Z48s1W5rVRzdBSHGQ0NkAhuECo,2971
 rtdip_sdk/pipelines/secrets/interfaces.py,sha256=VoSDAhP63SrLs8DgHihZEFMi3hHgivhCDtha9xQxjO0,824
 rtdip_sdk/pipelines/secrets/models.py,sha256=wf7mqWTcgdIznuD6hBI1zpwsKOewMZUUu2rUwV2uehU,887
 rtdip_sdk/pipelines/sources/__init__.py,sha256=hPl8ifI25qmvN9IOghCOIoXjvCR0dLVke0atab6bvGg,779
 rtdip_sdk/pipelines/sources/interfaces.py,sha256=FnhgvVMd2IpizhuITFavf7oKvo9HeJwazSIQ2jihO8c,993
 rtdip_sdk/pipelines/sources/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/pipelines/sources/spark/autoloader.py,sha256=rL0t5jd-RSowkpklhdSd__6adfrVD0c8LKmKvmqYBY0,3420
 rtdip_sdk/pipelines/sources/spark/delta.py,sha256=BuWtKZPDxRfe7XA6x7pJTTL8TxjJoMXEaPAomdrEdt8,4501
 rtdip_sdk/pipelines/sources/spark/delta_sharing.py,sha256=Mbb4Be4yN1X6biLDB-S6CDDos0SdKDTA97_sMY4W-1o,4473
 rtdip_sdk/pipelines/sources/spark/eventhub.py,sha256=jgUecN1ZkBKoAyVCM52SgbAPbdRl1Nknfbp-SozCRz0,5259
 rtdip_sdk/pipelines/sources/spark/iot_hub.py,sha256=LdVZkc-xOSTyq6y4sD1nmpef5zlSySJNwwtP4tXaMao,5240
 rtdip_sdk/pipelines/sources/spark/kafka.py,sha256=7OGqTZtkvNI8TaBB7hptYywclJOAzmHxOync_1jUayE,8114
 rtdip_sdk/pipelines/sources/spark/kinesis.py,sha256=uarSt6bVe-2amI8qaLd2lwabLnVcasMnrFu86KXyIDo,3793
-rtdip_sdk/pipelines/transformers/__init__.py,sha256=kRfVwAJZ2_x58nEgV3hZj8qmwT1wS5NonF4tSJZY5bY,714
+rtdip_sdk/pipelines/transformers/__init__.py,sha256=gx9jcKnCS0FWaV5gEUv9aL-NC9PMKmQUakgKc02o4aQ,795
 rtdip_sdk/pipelines/transformers/interfaces.py,sha256=KZUm93QHDARxMobPg989HijfiBjSpOI8oVILSJlK30g,946
-rtdip_sdk/pipelines/transformers/spark/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rtdip_sdk/pipelines/transformers/spark/binary_to_string.py,sha256=sHIrhT4ncqIinZNSxmk5xcBsvpqH7lIpe3W_Pep8Vsw,2143
-rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py,sha256=Yj1ov6rxL083Pd0dHO3lTUKSs-KNVF1mGqQ3ZpcG_q4,2953
-rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py,sha256=9EiuDH6E6reseFC-W33dnS0Yb0w7eyUKTrN6xHwPP5M,3571
-rtdip_sdk/pipelines/utilities/__init__.py,sha256=TI4telg5YtXtgyD0iLEPp_2fWDMkTHGbTwBJwWFtd_I,727
+rtdip_sdk/pipelines/transformers/spark/__init__.py,sha256=EcLqp88LLcvjuHFzAdQBHxfRYh7-2yBS5SZB7waST1o,570
+rtdip_sdk/pipelines/transformers/spark/binary_to_string.py,sha256=aEU_xtjEo7t5JAw40NAj7jMxAj0nE89m8MBlmUiILe8,2174
+rtdip_sdk/pipelines/transformers/spark/fledge_json_to_pcdm.py,sha256=3pYVhz-v5bSfAbTEZ_sy0OMaPEg3wSPDg7UWB9iYxb4,3436
+rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_pcdm.py,sha256=Wvb_kizQnu2JWB0KOocR1Rj52jXG__X-sohpVMvQDTc,4837
+rtdip_sdk/pipelines/transformers/spark/ssip_pi_binary_file_to_pcdm.py,sha256=TuGWLQz4rDmP4fwVWl5vG7FdMtviGtGwsG0X98nrnBc,3905
+rtdip_sdk/pipelines/transformers/spark/ssip_pi_binary_json_to_pcdm.py,sha256=m-Ew0dZdRNTE-n8wTE6mSV0Q3R3wy2kE5HWhWoO85Uk,5534
+rtdip_sdk/pipelines/utilities/__init__.py,sha256=FjIq3KMPG2Z965auq1aKrgVH1JSEanXsAhkf-UNfHu0,762
 rtdip_sdk/pipelines/utilities/interfaces.py,sha256=jHlDdFAgbUL9alAmU3Ncye_2iqywJLglFbZ04zaqNTQ,773
 rtdip_sdk/pipelines/utilities/aws/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py,sha256=lScqjJU9fFRkgnBI1RrqG-Sswh0Ek7_waebBQrARIEY,4674
+rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py,sha256=zkX0mIX6LWabQmm5QUfMTS0dTGBcoyhfvjBqlrauAwc,4680
 rtdip_sdk/pipelines/utilities/azure/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py,sha256=SXGZsO00_ZoEY9EdKs06vxAlmKLuAPcF8xX1SVbz1J4,6556
+rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py,sha256=eeUJup9m9mjSxPWCAGY76c29jUn6fy6ObRpbgM0B5Fo,6579
 rtdip_sdk/pipelines/utilities/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/utilities/spark/configuration.py,sha256=hNlDyTCFr_ykTfigONZWtpAHLUHSH03Zet1LaM79pGs,2185
-rtdip_sdk/pipelines/utilities/spark/delta_table_create.py,sha256=NvPxUZapqt2_CZ3arKHkCUKcRnhdyruIBHmz3Jtok0k,3857
-rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py,sha256=8mBCct4mmhkypW41eFDbLYhWZEnlii1ANz5kwtWyNkM,3119
+rtdip_sdk/pipelines/utilities/spark/adls_gen2_spn_connect.py,sha256=PxYrzdvuIRYg-dcGwwMeXaoewhnL7lEUwhOF6x1h0mc,3375
+rtdip_sdk/pipelines/utilities/spark/configuration.py,sha256=_BziNCvmz4dC4U2sMs0keNPl6GxIfOV7t1cj3SRuOQ0,2173
+rtdip_sdk/pipelines/utilities/spark/delta_table_create.py,sha256=LEBiaq2NtP625B3HjDyHiZ45Eu78l9Fw1Rw2-th-v0s,5181
+rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py,sha256=_jiC1IGw4Zm_UQEwCvfn2eiUI_L8SoZS7R2m_i8_gQY,3125
 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py,sha256=BvMUPC1NCFPXz4oN9XxsCnAsZ0vdiZTNp7bFsx7dFfg,2602
-rtdip_sdk-0.2.2.dist-info/LICENSE.md,sha256=WYmcYJG1QFgu1hfo7qrEkZ3Jhcz8NUWe6XUraZvlIFs,10172
-rtdip_sdk-0.2.2.dist-info/METADATA,sha256=nD971CId17LH3wi-GcfXWYeoXTeokQ_SSXv4ezD4CWg,2844
-rtdip_sdk-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rtdip_sdk-0.2.2.dist-info/top_level.txt,sha256=DFRWw2FYwSXWlH6UsWDVt1G8Bq6QjRWN0GJ8BS4o2dg,10
-rtdip_sdk-0.2.2.dist-info/RECORD,,
+rtdip_sdk-0.3.0.dist-info/LICENSE.md,sha256=WYmcYJG1QFgu1hfo7qrEkZ3Jhcz8NUWe6XUraZvlIFs,10172
+rtdip_sdk-0.3.0.dist-info/METADATA,sha256=3SKCLj3obOF6Kfs0lGIke2DBuKrEdj6rzJVWzM1_MFQ,3058
+rtdip_sdk-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rtdip_sdk-0.3.0.dist-info/top_level.txt,sha256=DFRWw2FYwSXWlH6UsWDVt1G8Bq6QjRWN0GJ8BS4o2dg,10
+rtdip_sdk-0.3.0.dist-info/RECORD,,
```

