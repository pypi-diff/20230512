# Comparing `tmp/macrometa-source-mongo-0.0.36.tar.gz` & `tmp/macrometa-source-mongo-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.36.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.37.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.36.tar` & `macrometa-source-mongo-0.0.37.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/LICENSE
--rw-r--r--   0        0        0    21341 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0     1151 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     8097 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     6267 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-05-10 04:22:49.851829 macrometa-source-mongo-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.36/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/LICENSE
+-rw-r--r--   0        0        0    20533 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7248 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-05-12 10:08:53.183191 macrometa-source-mongo-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.37/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.37/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.36/LICENSE` & `macrometa-source-mongo-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import copy
 import json
 import sys
-from typing import List, Dict, Optional
+from typing import List, Dict
 
 import pkg_resources
 import singer
 from pymongo import MongoClient
 from singer import metadata, metrics, utils
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
@@ -16,15 +16,15 @@
 from macrometa_source_mongo.sync_strategies import common
 from macrometa_source_mongo.sync_strategies import full_table
 from macrometa_source_mongo.sync_strategies.sample_data import fetch_samples
 from macrometa_source_mongo.connection import create_certficate_files, delete_certficate_files, \
     get_connection_string, get_user_databases
 from macrometa_source_mongo.exceptions import InvalidReplicationMethodException, NoReadPrivilegeException
 from macrometa_source_mongo.helper import filter_streams_by_replication_method, get_attribute_type, \
-    get_streams_to_sync, produce_collection_schema, streams_list_to_dict, validate_config, \
+    get_streams_to_sync, produce_collection_schema, streams_list_to_dict, \
     write_schema_message
 
 LOGGER = singer.get_logger('macrometa_source_mongo')
 
 REQUIRED_CONFIG_KEYS = [
     'host',
     'user',
@@ -167,18 +167,14 @@
                            placeholder_value='replica'),
             ConfigProperty('ssl', 'Use SSL', ConfigAttributeType.BOOLEAN, False, False,
                            description='Can be set to true to connect using SSL.',
                            default_value="false"),
             ConfigProperty('verify_mode', 'Verify Mode', ConfigAttributeType.BOOLEAN, False, False,
                            description='Default SSL verify mode.',
                            default_value="true"),
-            ConfigProperty('await_time_ms', 'Await Time (Milliseconds)', ConfigAttributeType.INT, False, False,
-                           description='[LOG_BASED] The maximum amount of time in milliseconds the log_based method '
-                                       'waits for new data changes before exiting.',
-                           default_value='900000'),
             ConfigProperty('direct_connection', 'Direct Connection', ConfigAttributeType.BOOLEAN, False, False,
                            description='Specifies whether to connect directly to the specified MongoDB host as a '
                                        'standalone or connect to the entire replica set of which the given MongoDB host is a part.',
                            default_value="false"),
             ConfigProperty('tls_ca_file', 'SSL/TLS CA Certificate', ConfigAttributeType.FILE, False, False,
                            description='Specific CA certificate in PEM string format. This is most often the case '
                                        'when using `self-signed` server certificate.',
@@ -213,15 +209,14 @@
                 # Optional config keys
                 'srv': integration.get('srv', False),
                 'port': integration.get('port'),
                 'replica_set': integration.get('replica_set'),
                 'ssl': integration.get('ssl', False),
                 'verify_mode': integration.get('verify_mode', True),
                 'direct_connection': integration.get('direct_connection', False),
-                'await_time_ms': integration.get('await_time_ms', 900000),
                 'tls_ca_file': integration.get('tls_ca_file'),
                 'tls_certificate_key_file': integration.get('tls_certificate_key_file'),
                 'tls_certificate_key_file_password': integration.get('tls_certificate_key_file_password'),
             }
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.') from e
 
@@ -353,25 +348,23 @@
         sync_traditional_stream(client, stream, state, replication_method)
 
 
 def sync_log_based_streams(client: MongoClient,
                            log_based_streams: List[Dict],
                            database_name: str,
                            state: Dict,
-                           await_time_ms: Optional[int],
                            replication_method: str
                            ):
     """
     Sync log_based streams all at once by listening on the database-level change streams events.
     Args:
         client: MongoDB client instance
         log_based_streams:  list of streams to sync
         database_name: name of the database to sync from
         state: state dictionary
-        await_time_ms:  the maximum time in milliseconds for the log based to wait for changes before exiting
         replication_method: replication method
     """
     if not log_based_streams:
         return
 
     streams = streams_list_to_dict(log_based_streams)
 
@@ -385,17 +378,16 @@
         singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
         write_schema_message(stream)
         common.SCHEMA_COUNT[tap_stream_id] += 1
 
     with metrics.job_timer('sync_table') as timer:
         timer.tags['database'] = database_name
-        await_time_ms = await_time_ms or log_based.DEFAULT_AWAIT_TIME_MS
 
-        log_based.sync_database(client[database_name], streams, state, await_time_ms)
+        log_based.sync_database(client[database_name], streams, state)
 
     state = singer.set_currently_syncing(state, None)
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def do_sync(client: MongoClient, catalog: Dict, config: Dict, replication_method: str, state: Dict):
     """
@@ -403,15 +395,14 @@
     Args:
         client: MongoDb client instance
         catalog: dictionary with all the streams details
         config: config dictionary
         replication_method: replication method
         state: state
     """
-    validate_config(config)
 
     all_streams = catalog['streams']
     streams_to_sync = get_streams_to_sync(all_streams, state)
 
     log_based_streams, traditional_streams = filter_streams_by_replication_method(streams_to_sync,
                                                                                   replication_method)
     LOGGER.debug('Starting sync of traditional streams ...')
@@ -419,15 +410,14 @@
     LOGGER.debug('Sync of traditional streams done')
 
     LOGGER.debug('Starting sync of log based streams ...')
     sync_log_based_streams(client,
                            log_based_streams,
                            config['database'],
                            state,
-                           config.get('await_time_ms'),
                            replication_method
                            )
     LOGGER.debug('Sync of log based streams done')
 
     LOGGER.info(common.get_sync_summary(catalog, replication_method))
```

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,7 @@
 
 class NoReadPrivilegeException(Exception):
     """Raised if the user has no read privilege on the Mongo DB"""
 
     def __init__(self, user, db_name):
         msg = f"The user '{user}' has no read privilege on the database '{db_name}'!"
         super().__init__(msg)
-
-
-class InvalidAwaitTimeException(Exception):
-    """Raised if the given await time used in log_based replication is invalid"""
-
-    def __init__(self, time_ms, reason):
-        msg = f"Invalid await time {time_ms}! {reason}"
-        super().__init__(msg)
```

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,17 @@
 
 import singer
 from c8connector import SchemaAttributeType
 from pymongo.collection import Collection
 from singer import get_logger, metadata, SchemaMessage, write_message
 
 from macrometa_source_mongo.sync_strategies.common import calculate_destination_stream_name
-from macrometa_source_mongo.exceptions import InvalidAwaitTimeException
-
 
 logger = get_logger('macrometa_source_mongo')
 
-def validate_config(config: Dict) -> None:
-    """
-    Checks the configuration parameters for correctness and raises an exception for invalid values.
-    Args:
-        config (Dict): A dictionary of configuration parameters to validate.
-
-    Returns:
-        None
-
-    Raises:
-        InvalidAwaitTimeException: If the 'await_time_ms' parameter is not an integer or less than or equal to 0.
-    """
-    if 'await_time_ms' in config:
-        await_time_ms = config['await_time_ms']
-
-        if not isinstance(await_time_ms, int):
-            raise InvalidAwaitTimeException(await_time_ms, 'Await time should be an integer')
-
-        if await_time_ms <= 0:
-            raise InvalidAwaitTimeException(
-                await_time_ms, 'Await time should be greater than 0')
-
 
 def get_replication_method_from_stream(stream: Dict, replication_method: str) -> Optional[str]:
     """
     Retrieves the replication method for a given stream.
     Args:
         stream (Dict): A stream dictionary.
         replication_method (str): The replication method.
```

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import copy
 import time
 import singer
 
 from typing import Set, Dict, Optional
 from pymongo.database import Database
+from pymongo.errors import CursorNotFound
 from singer import utils
 
 from macrometa_source_mongo.sync_strategies import common
 
 LOGGER = singer.get_logger('macrometa_source_mongo')
 
 BOOKMARK_KEY = 'token' # bookmark key for logbased replication
-DEFAULT_AWAIT_TIME_MS = 900000 # default max await time in milliseconds
+DEFAULT_AWAIT_TIME_MS = 600000 # default max await time for database watcher in milliseconds
 
 
 def update_bookmarks(state: Dict, tap_stream_ids: Set[str], token: Dict) -> Dict:
     """
     Updates the stream state by re-setting the change stream token
     Args:
         state: State dictionary
@@ -48,102 +49,109 @@
 
     return token_sorted[0] if token_sorted else None
 
 
 def sync_database(database: Database,
                   streams_to_sync: Dict[str, Dict],
                   state: Dict,
-                  await_time_ms: int
                   ) -> None:
     """
     Syncs the records from the given collection using Change Stream
     Args:
         database: MongoDB Database instance to sync
         streams_to_sync: Dict of stream dictionary with all the stream details
         state: state dictionary
-        await_time_ms:  the maximum time in milliseconds for the log based to wait for changes before exiting
     """
     LOGGER.info('LogBased sync started for stream "%s" in database "%s"', list(streams_to_sync.keys())[0], database.name)
 
-    start_time = time.time()
-
     rows_saved = {stream_id: 0 for stream_id in streams_to_sync}
     stream_ids = set(streams_to_sync.keys())
 
-    # Init a cursor to listen for changes from the last saved resume token
-    # if there are no changes after MAX_AWAIT_TIME_MS, then we'll exit
-    with database.watch(
-                    [{'$match': {
-                        '$or': [
-                            {'operationType': 'insert'}, {'operationType': 'update'}, {'operationType': 'delete'}
-                        ],
-                        '$and': [
-                            # watch collections of selected streams
-                            {'ns.coll': {'$in': [val['table_name'] for val in streams_to_sync.values()]}}
-                        ]
-                    }}],
-                    max_await_time_ms=await_time_ms,
-                    start_after=get_bookmark_key_from_state(stream_ids, state)
-            ) as cursor:
-        while cursor.alive:
-
-            change = cursor.try_next()
-            # Get resume token from '_data' to resume LOG_BASED
-            resume_token = {
-                '_data': cursor.resume_token['_data']
-            }
-
-            # After MAX_AWAIT_TIME_MS has elapsed, the cursor will return None.
-            # write state and exit
-            if change is None:
-                LOGGER.info('No changes found after max await time %s, updating bookmark and exiting...', await_time_ms)
-
-                state = update_bookmarks(state, stream_ids, resume_token)
-                singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
-                break
-
-            tap_stream_id = f'{change["ns"]["db"]}-{change["ns"]["coll"]}'
-
-            operation = change['operationType']
-
-            if operation == 'delete':
-                # Delete ops only contain the _id of the row deleted
-                singer.write_message(common.row_to_singer_record(
-                    stream=streams_to_sync[tap_stream_id],
-                    row={'_id': change['documentKey']['_id']},
-                    time_extracted=utils.now(),
-                    time_deleted=change[
-                        'clusterTime'].as_datetime()))  # returns python's datetime.datetime instance in UTC
-
-                rows_saved[tap_stream_id] += 1
-
-            elif operation == 'insert':
-                singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
-                                                                 row=change['fullDocument'],
-                                                                 time_extracted=utils.now(),
-                                                                 time_deleted=None))
-
-                rows_saved[tap_stream_id] += 1
-
-            elif operation == 'update':
-                # update operation only return _id and updated fields in the row,
-                query = {'_id': change['documentKey']['_id']}
-                row = database[streams_to_sync[tap_stream_id]['table_name']].find_one(query)
-                singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
-                                                                 row=row,
-                                                                 time_extracted=utils.now(),
-                                                                 time_deleted=None))
-
-                rows_saved[tap_stream_id] += 1
-
-            # update the states of all streams
-            state = update_bookmarks(state, stream_ids, resume_token)
-
-            # Write state after every 1000 records
-            if sum(rows_saved.values()) % 1000 == 0:
-                # write state
-                singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
-
-    for stream_id in stream_ids:
-        common.COUNTS[stream_id] += rows_saved[stream_id]
-        common.TIMES[stream_id] += time.time() - start_time
-        LOGGER.info('The number of records synchronized for %s is %s.', stream_id, rows_saved[stream_id])
+    while True:
+        start_time = time.time()
+        rows_saved_iter_start = rows_saved.copy()
+        try:
+            # Init a cursor to listen for changes from the last saved resume token
+            # if there are no changes after MAX_AWAIT_TIME_MS, the cursor returns an empty batch.
+            with database.watch(
+                            [{'$match': {
+                                '$or': [
+                                    {'operationType': 'insert'}, {'operationType': 'update'}, {'operationType': 'delete'}
+                                ],
+                                '$and': [
+                                    # watch collections of selected streams
+                                    {'ns.coll': {'$in': [val['table_name'] for val in streams_to_sync.values()]}}
+                                ]
+                            }}],
+                            max_await_time_ms=DEFAULT_AWAIT_TIME_MS,
+                            start_after=get_bookmark_key_from_state(stream_ids, state)
+                    ) as cursor:
+                while cursor.alive:
+                
+                    change = cursor.try_next()
+                    # Get resume token from '_data' to resume LOG_BASED
+                    resume_token = {
+                        '_data': cursor.resume_token['_data']
+                    }
+        
+                    # After MAX_AWAIT_TIME_MS has elapsed, the cursor will return None.
+                    if change is None:
+                        continue
+                    
+                    tap_stream_id = f'{change["ns"]["db"]}-{change["ns"]["coll"]}'
+        
+                    operation = change['operationType']
+        
+                    if operation == 'delete':
+                        # Delete ops only contain the _id of the row deleted
+                        singer.write_message(common.row_to_singer_record(
+                            stream=streams_to_sync[tap_stream_id],
+                            row={'_id': change['documentKey']['_id']},
+                            time_extracted=utils.now(),
+                            time_deleted=change[
+                                'clusterTime'].as_datetime()))  # returns python's datetime.datetime instance in UTC
+        
+                        rows_saved[tap_stream_id] += 1
+        
+                    elif operation == 'insert':
+                        singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
+                                                                         row=change['fullDocument'],
+                                                                         time_extracted=utils.now(),
+                                                                         time_deleted=None))
+        
+                        rows_saved[tap_stream_id] += 1
+        
+                    elif operation == 'update':
+                        # update operation only return _id and updated fields in the row,
+                        query = {'_id': change['documentKey']['_id']}
+                        row = database[streams_to_sync[tap_stream_id]['table_name']].find_one(query)
+                        singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
+                                                                         row=row,
+                                                                         time_extracted=utils.now(),
+                                                                         time_deleted=None))
+        
+                        rows_saved[tap_stream_id] += 1
+        
+                    # update the states of all streams
+                    state = update_bookmarks(state, stream_ids, resume_token)
+        
+                    # Write state after every 1000 records
+                    if sum(rows_saved.values()) % 1000 == 0:
+                        # write state
+                        singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
+        except Exception as e:
+            # Log the error
+            LOGGER.error('Error received while syncing database: %s', str(e))
+            # Retry or exit based on the type of error
+            if isinstance(e, CursorNotFound):
+                # If the cursor is not found, retry
+                LOGGER.info('Cursor not found, retrying...')
+                continue
+            else:
+                # For other types of errors, we may want to exit the program
+                LOGGER.error('Unhandled error type, exiting...')
+                raise e
+        for stream_id in stream_ids:
+            common.TIMES[stream_id] += time.time() - start_time
+            if rows_saved[stream_id] - rows_saved_iter_start[stream_id] > 0:
+                common.COUNTS[stream_id] += (rows_saved[stream_id] - rows_saved_iter_start[stream_id])
+                LOGGER.info('The number of records synchronized till now for %s is %s.', stream_id, rows_saved[stream_id])
```

### Comparing `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.36/pyproject.toml` & `macrometa-source-mongo-0.0.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.36'
+version='0.0.37'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.36/setup.py` & `macrometa-source-mongo-0.0.37/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.36',
+    'version': '0.0.37',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.36/PKG-INFO` & `macrometa-source-mongo-0.0.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.36
+Version: 0.0.37
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

