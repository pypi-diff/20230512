# Comparing `tmp/ucam-identitylib-1.5.0.tar.gz` & `tmp/ucam-identitylib-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam-identitylib-1.5.0.tar", last modified: Fri Apr 21 08:32:42 2023, max compression
+gzip compressed data, was "ucam-identitylib-1.6.0.tar", last modified: Fri May 12 10:19:27 2023, max compression
```

## Comparing `ucam-identitylib-1.5.0.tar` & `ucam-identitylib-1.6.0.tar`

### file list

```diff
@@ -1,268 +1,269 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.795516 ucam-identitylib-1.5.0/identitylib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-20 19:16:44.000000 ucam-identitylib-1.5.0/identitylib/api_client_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.799516 ucam-identitylib-1.5.0/identitylib/card_client/
--rw-r--r--   0 root         (0) root         (0)     8516 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.799516 ucam-identitylib-1.5.0/identitylib/card_client/api/
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13392 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/permissions_api.py
--rw-r--r--   0 root         (0) root         (0)   217309 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/v1beta1_api.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api/versions_api.py
--rw-r--r--   0 root         (0) root         (0)    46930 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.799516 ucam-identitylib-1.5.0/identitylib/card_client/apis/
--rw-r--r--   0 root         (0) root         (0)      643 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24525 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)    12776 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/card_client/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19212 2023-04-21 08:32:15.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/api_exception.py
--rw-r--r--   0 root         (0) root         (0)    19855 2023-04-21 08:32:15.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode.py
--rw-r--r--   0 root         (0) root         (0)    19301 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19607 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19919 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py
--rw-r--r--   0 root         (0) root         (0)    19449 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
--rw-r--r--   0 root         (0) root         (0)    19216 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    25129 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card.py
--rw-r--r--   0 root         (0) root         (0)    22257 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19875 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_response_type.py
--rw-r--r--   0 root         (0) root         (0)    21301 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier.py
--rw-r--r--   0 root         (0) root         (0)    19670 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19747 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
--rw-r--r--   0 root         (0) root         (0)    19680 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19600 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
--rw-r--r--   0 root         (0) root         (0)    19209 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_destroy_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19477 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19206 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    21069 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_logo.py
--rw-r--r--   0 root         (0) root         (0)    20492 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note.py
--rw-r--r--   0 root         (0) root         (0)    19441 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19208 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19191 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_response_type.py
--rw-r--r--   0 root         (0) root         (0)    30374 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request.py
--rw-r--r--   0 root         (0) root         (0)    19640 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    21306 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py
--rw-r--r--   0 root         (0) root         (0)    20037 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py
--rw-r--r--   0 root         (0) root         (0)    19489 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py
--rw-r--r--   0 root         (0) root         (0)    19671 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19284 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_create_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19213 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_distinct_values.py
--rw-r--r--   0 root         (0) root         (0)    27903 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_summary.py
--rw-r--r--   0 root         (0) root         (0)    21042 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19197 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19721 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19708 2023-04-21 08:32:16.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
--rw-r--r--   0 root         (0) root         (0)    23411 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_summary.py
--rw-r--r--   0 root         (0) root         (0)    19609 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_request_type.py
--rw-r--r--   0 root         (0) root         (0)    19176 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19276 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/college_institution_ids_list_response_type.py
--rw-r--r--   0 root         (0) root         (0)    20114 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_available_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)    20094 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_identifier_type.py
--rw-r--r--   0 root         (0) root         (0)    19851 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_logo_type.py
--rw-r--r--   0 root         (0) root         (0)    19851 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_note_type.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_request_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    20064 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_summary_type.py
--rw-r--r--   0 root         (0) root         (0)    19382 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/permissions_response_type.py
--rw-r--r--   0 root         (0) root         (0)    19244 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    19608 2023-04-21 08:32:17.000000 ucam-identitylib-1.5.0/identitylib/card_client/model/version_response_type.py
--rw-r--r--   0 root         (0) root         (0)    90312 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/card_client/models/
--rw-r--r--   0 root         (0) root         (0)     5469 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21989 2023-04-21 08:32:18.000000 ucam-identitylib-1.5.0/identitylib/card_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/card_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/hr_client/
--rw-r--r--   0 root         (0) root         (0)     2656 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/hr_client/api/
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15246 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/api/staff_members_api.py
--rw-r--r--   0 root         (0) root         (0)    41199 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.823517 ucam-identitylib-1.5.0/identitylib/hr_client/apis/
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18527 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6932 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/hr_client/model/
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15386 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation.py
--rw-r--r--   0 root         (0) root         (0)    14942 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13339 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/http_exception.py
--rw-r--r--   0 root         (0) root         (0)    13537 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    14333 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13097 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/location_inner.py
--rw-r--r--   0 root         (0) root         (0)    14276 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/paginated_results_staff_member.py
--rw-r--r--   0 root         (0) root         (0)    16189 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/staff_member.py
--rw-r--r--   0 root         (0) root         (0)    13901 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    84466 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/hr_client/models/
--rw-r--r--   0 root         (0) root         (0)     1113 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16143 2023-04-21 08:32:21.000000 ucam-identitylib-1.5.0/identitylib/hr_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     9961 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/
--rw-r--r--   0 root         (0) root         (0)     1757 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    40103 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/apis/
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17693 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5929 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/
--rw-r--r--   0 root         (0) root         (0)      368 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12946 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_datum.py
--rw-r--r--   0 root         (0) root         (0)    12728 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_response.py
--rw-r--r--   0 root         (0) root         (0)    83476 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/models/
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15153 2023-04-21 08:32:32.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/inst_identifier_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.827517 ucam-identitylib-1.5.0/identitylib/lookup_client/
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.831518 ucam-identitylib-1.5.0/identitylib/lookup_client/api/
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58215 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/group_api.py
--rw-r--r--   0 root         (0) root         (0)    10948 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/ibis_api.py
--rw-r--r--   0 root         (0) root         (0)    76192 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/institution_api.py
--rw-r--r--   0 root         (0) root         (0)   101034 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api/person_api.py
--rw-r--r--   0 root         (0) root         (0)    39272 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.831518 ucam-identitylib-1.5.0/identitylib/lookup_client/apis/
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16967 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5116 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/lookup_client/model/
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14574 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute.py
--rw-r--r--   0 root         (0) root         (0)    14850 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute_scheme.py
--rw-r--r--   0 root         (0) root         (0)    12076 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_phone_number.py
--rw-r--r--   0 root         (0) root         (0)    14778 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_row.py
--rw-r--r--   0 root         (0) root         (0)    11774 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_web_page.py
--rw-r--r--   0 root         (0) root         (0)    12447 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/error.py
--rw-r--r--   0 root         (0) root         (0)    21254 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response.py
--rw-r--r--   0 root         (0) root         (0)    11698 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11901 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response.py
--rw-r--r--   0 root         (0) root         (0)    11699 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11961 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py
--rw-r--r--   0 root         (0) root         (0)    11735 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11850 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response.py
--rw-r--r--   0 root         (0) root         (0)    11684 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    20692 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_members_of_inst.py
--rw-r--r--   0 root         (0) root         (0)    11880 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response.py
--rw-r--r--   0 root         (0) root         (0)    11532 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11962 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    18567 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py
--rw-r--r--   0 root         (0) root         (0)    11871 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11910 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response.py
--rw-r--r--   0 root         (0) root         (0)    11785 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11950 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response.py
--rw-r--r--   0 root         (0) root         (0)    11762 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11960 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response.py
--rw-r--r--   0 root         (0) root         (0)    11776 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11971 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py
--rw-r--r--   0 root         (0) root         (0)    11856 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    11900 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response.py
--rw-r--r--   0 root         (0) root         (0)    11771 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    18657 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person.py
--rw-r--r--   0 root         (0) root         (0)    11870 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response.py
--rw-r--r--   0 root         (0) root         (0)    11702 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    14062 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_identifier.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py
--rw-r--r--   0 root         (0) root         (0)    11550 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py
--rw-r--r--   0 root         (0) root         (0)    82654 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/lookup_client/models/
--rw-r--r--   0 root         (0) root         (0)     4751 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14331 2023-04-21 08:32:25.000000 ucam-identitylib-1.5.0/identitylib/lookup_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/lookup_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/photo_client/
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.835518 ucam-identitylib-1.5.0/identitylib/photo_client/api/
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11772 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/all_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    10203 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/api_versions_api.py
--rw-r--r--   0 root         (0) root         (0)    43722 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/approved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    10164 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/permissions_api.py
--rw-r--r--   0 root         (0) root         (0)    11335 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifier_api.py
--rw-r--r--   0 root         (0) root         (0)    27918 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_api.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    61774 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    11860 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api/unapproved_photos_api.py
--rw-r--r--   0 root         (0) root         (0)    43706 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/photo_client/apis/
--rw-r--r--   0 root         (0) root         (0)     1216 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21352 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     9560 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/photo_client/model/
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17123 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/action_enum.py
--rw-r--r--   0 root         (0) root         (0)    16212 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/api_versions.py
--rw-r--r--   0 root         (0) root         (0)    15964 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/bad_request.py
--rw-r--r--   0 root         (0) root         (0)    15961 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/forbidden.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/internal_server_error.py
--rw-r--r--   0 root         (0) root         (0)    15958 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/not_found.py
--rw-r--r--   0 root         (0) root         (0)    16791 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
--rw-r--r--   0 root         (0) root         (0)    16619 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
--rw-r--r--   0 root         (0) root         (0)    16028 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/permissions.py
--rw-r--r--   0 root         (0) root         (0)    18732 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier.py
--rw-r--r--   0 root         (0) root         (0)    16464 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py
--rw-r--r--   0 root         (0) root         (0)    16412 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
--rw-r--r--   0 root         (0) root         (0)    19295 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/scheme_enum.py
--rw-r--r--   0 root         (0) root         (0)    16889 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/status_enum.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/transient_image_url.py
--rw-r--r--   0 root         (0) root         (0)    15970 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/unauthorized.py
--rw-r--r--   0 root         (0) root         (0)    22401 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo.py
--rw-r--r--   0 root         (0) root         (0)    16599 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
--rw-r--r--   0 root         (0) root         (0)    16547 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py
--rw-r--r--   0 root         (0) root         (0)    87097 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/photo_client/models/
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18774 2023-04-21 08:32:28.000000 ucam-identitylib-1.5.0/identitylib/photo_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/photo_client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/student_client/
--rw-r--r--   0 root         (0) root         (0)     2582 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/student_client/api/
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21826 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/api/students_api.py
--rw-r--r--   0 root         (0) root         (0)    41093 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.839518 ucam-identitylib-1.5.0/identitylib/student_client/apis/
--rw-r--r--   0 root         (0) root         (0)      509 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18407 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6818 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/identitylib/student_client/model/
--rw-r--r--   0 root         (0) root         (0)      360 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15305 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation.py
--rw-r--r--   0 root         (0) root         (0)    14466 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation_scheme.py
--rw-r--r--   0 root         (0) root         (0)    13235 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/http_exception.py
--rw-r--r--   0 root         (0) root         (0)    13438 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)    13725 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/identifier.py
--rw-r--r--   0 root         (0) root         (0)    14035 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/identifier_scheme.py
--rw-r--r--   0 root         (0) root         (0)    12993 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/location_inner.py
--rw-r--r--   0 root         (0) root         (0)    14202 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/paginated_results_student.py
--rw-r--r--   0 root         (0) root         (0)    16439 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/student.py
--rw-r--r--   0 root         (0) root         (0)    13802 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model/validation_error.py
--rw-r--r--   0 root         (0) root         (0)    84357 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/identitylib/student_client/models/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16034 2023-04-21 08:32:30.000000 ucam-identitylib-1.5.0/identitylib/student_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/university_hr_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/identitylib/university_student_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-05 11:43:13.000000 ucam-identitylib-1.5.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-04-20 15:51:40.000000 ucam-identitylib-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 08:31:53.000000 ucam-identitylib-1.5.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5517 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/tests/test_api_client_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2023-03-30 12:19:13.000000 ucam-identitylib-1.5.0/tests/test_identifiers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 08:32:42.843518 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12331 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-21 08:32:42.000000 ucam-identitylib-1.5.0/ucam_identitylib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.814756 ucam-identitylib-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 10:19:27.814756 ucam-identitylib-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.686756 ucam-identitylib-1.6.0/identitylib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/api_client_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.686756 ucam-identitylib-1.6.0/identitylib/card_client/
+-rw-r--r--   0 root         (0) root         (0)     8516 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.690756 ucam-identitylib-1.6.0/identitylib/card_client/api/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13392 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/permissions_api.py
+-rw-r--r--   0 root         (0) root         (0)   217877 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/v1beta1_api.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api/versions_api.py
+-rw-r--r--   0 root         (0) root         (0)    46930 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.690756 ucam-identitylib-1.6.0/identitylib/card_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      643 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24525 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    12776 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.714756 ucam-identitylib-1.6.0/identitylib/card_client/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19212 2023-05-12 10:18:48.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)    19855 2023-05-12 10:18:48.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode.py
+-rw-r--r--   0 root         (0) root         (0)    19301 2023-05-12 10:18:48.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19607 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19919 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py
+-rw-r--r--   0 root         (0) root         (0)    19449 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19216 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    25221 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card.py
+-rw-r--r--   0 root         (0) root         (0)    22299 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19875 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    24195 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    19670 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19747 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19680 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19600 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19209 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_destroy_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    21322 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_summary.py
+-rw-r--r--   0 root         (0) root         (0)    19477 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19206 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    21069 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_logo.py
+-rw-r--r--   0 root         (0) root         (0)    20492 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note.py
+-rw-r--r--   0 root         (0) root         (0)    19441 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19208 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19191 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    30424 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request.py
+-rw-r--r--   0 root         (0) root         (0)    19640 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    21306 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    20037 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py
+-rw-r--r--   0 root         (0) root         (0)    19489 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py
+-rw-r--r--   0 root         (0) root         (0)    19671 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_create_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19213 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_distinct_values.py
+-rw-r--r--   0 root         (0) root         (0)    27953 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_summary.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19197 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19721 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19708 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
+-rw-r--r--   0 root         (0) root         (0)    23503 2023-05-12 10:18:49.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_summary.py
+-rw-r--r--   0 root         (0) root         (0)    19521 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_request_type.py
+-rw-r--r--   0 root         (0) root         (0)    19176 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19276 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/college_institution_ids_list_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    20114 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_available_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)    20165 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_identifier_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    19851 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_logo_type.py
+-rw-r--r--   0 root         (0) root         (0)    19851 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_note_type.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_request_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    20064 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_summary_type.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/permissions_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    19608 2023-05-12 10:18:50.000000 ucam-identitylib-1.6.0/identitylib/card_client/model/version_response_type.py
+-rw-r--r--   0 root         (0) root         (0)    90312 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.714756 ucam-identitylib-1.6.0/identitylib/card_client/models/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21989 2023-05-12 10:18:51.000000 ucam-identitylib-1.6.0/identitylib/card_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/card_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.718756 ucam-identitylib-1.6.0/identitylib/hr_client/
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.718756 ucam-identitylib-1.6.0/identitylib/hr_client/api/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15246 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/api/staff_members_api.py
+-rw-r--r--   0 root         (0) root         (0)    41199 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.718756 ucam-identitylib-1.6.0/identitylib/hr_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18527 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6932 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.726756 ucam-identitylib-1.6.0/identitylib/hr_client/model/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15386 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation.py
+-rw-r--r--   0 root         (0) root         (0)    14942 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13339 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/http_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13537 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    14333 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13097 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/location_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/paginated_results_staff_member.py
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/staff_member.py
+-rw-r--r--   0 root         (0) root         (0)    13901 2023-05-12 10:18:55.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    84466 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.726756 ucam-identitylib-1.6.0/identitylib/hr_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16143 2023-05-12 10:18:56.000000 ucam-identitylib-1.6.0/identitylib/hr_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9961 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.734756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.734756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6469 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    40103 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.734756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17693 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.742756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_datum.py
+-rw-r--r--   0 root         (0) root         (0)    12728 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_response.py
+-rw-r--r--   0 root         (0) root         (0)    83476 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.742756 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/models/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2023-05-12 10:19:13.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/inst_identifier_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.746756 ucam-identitylib-1.6.0/identitylib/lookup_client/
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.750756 ucam-identitylib-1.6.0/identitylib/lookup_client/api/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58215 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/group_api.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/ibis_api.py
+-rw-r--r--   0 root         (0) root         (0)    76192 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/institution_api.py
+-rw-r--r--   0 root         (0) root         (0)   101034 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api/person_api.py
+-rw-r--r--   0 root         (0) root         (0)    39272 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.750756 ucam-identitylib-1.6.0/identitylib/lookup_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16967 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.778756 ucam-identitylib-1.6.0/identitylib/lookup_client/model/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14574 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute.py
+-rw-r--r--   0 root         (0) root         (0)    14850 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    12076 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)    14778 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_row.py
+-rw-r--r--   0 root         (0) root         (0)    11774 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_web_page.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/error.py
+-rw-r--r--   0 root         (0) root         (0)    21254 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11698 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11901 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response.py
+-rw-r--r--   0 root         (0) root         (0)    11699 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11961 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11735 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11850 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11684 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    20692 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_members_of_inst.py
+-rw-r--r--   0 root         (0) root         (0)    11880 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11532 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11962 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    18567 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11785 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11950 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11960 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11776 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11971 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11856 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11771 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    18657 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person.py
+-rw-r--r--   0 root         (0) root         (0)    11870 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11702 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    14062 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-05-12 10:19:00.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py
+-rw-r--r--   0 root         (0) root         (0)    82654 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.778756 ucam-identitylib-1.6.0/identitylib/lookup_client/models/
+-rw-r--r--   0 root         (0) root         (0)     4751 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14331 2023-05-12 10:19:01.000000 ucam-identitylib-1.6.0/identitylib/lookup_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/lookup_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.778756 ucam-identitylib-1.6.0/identitylib/photo_client/
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.782756 ucam-identitylib-1.6.0/identitylib/photo_client/api/
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11772 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/all_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    10203 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/api_versions_api.py
+-rw-r--r--   0 root         (0) root         (0)    43722 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/approved_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    10164 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/permissions_api.py
+-rw-r--r--   0 root         (0) root         (0)    11335 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifier_api.py
+-rw-r--r--   0 root         (0) root         (0)    27918 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_api.py
+-rw-r--r--   0 root         (0) root         (0)    11127 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    61774 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api/unapproved_photos_api.py
+-rw-r--r--   0 root         (0) root         (0)    43706 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.782756 ucam-identitylib-1.6.0/identitylib/photo_client/apis/
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21352 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     9560 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.794757 ucam-identitylib-1.6.0/identitylib/photo_client/model/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17123 2023-05-12 10:19:04.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/action_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16212 2023-05-12 10:19:04.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/api_versions.py
+-rw-r--r--   0 root         (0) root         (0)    15964 2023-05-12 10:19:04.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/bad_request.py
+-rw-r--r--   0 root         (0) root         (0)    15961 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/forbidden.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/internal_server_error.py
+-rw-r--r--   0 root         (0) root         (0)    15958 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/not_found.py
+-rw-r--r--   0 root         (0) root         (0)    16791 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py
+-rw-r--r--   0 root         (0) root         (0)    16619 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py
+-rw-r--r--   0 root         (0) root         (0)    16028 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    18732 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier.py
+-rw-r--r--   0 root         (0) root         (0)    16464 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py
+-rw-r--r--   0 root         (0) root         (0)    16412 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py
+-rw-r--r--   0 root         (0) root         (0)    19295 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/scheme_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16889 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/transient_image_url.py
+-rw-r--r--   0 root         (0) root         (0)    15970 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/unauthorized.py
+-rw-r--r--   0 root         (0) root         (0)    22401 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo.py
+-rw-r--r--   0 root         (0) root         (0)    16599 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py
+-rw-r--r--   0 root         (0) root         (0)    16547 2023-05-12 10:19:05.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py
+-rw-r--r--   0 root         (0) root         (0)    87097 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.794757 ucam-identitylib-1.6.0/identitylib/photo_client/models/
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-05-12 10:19:06.000000 ucam-identitylib-1.6.0/identitylib/photo_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/photo_client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.798756 ucam-identitylib-1.6.0/identitylib/student_client/
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.798756 ucam-identitylib-1.6.0/identitylib/student_client/api/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21826 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/api/students_api.py
+-rw-r--r--   0 root         (0) root         (0)    41093 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.798756 ucam-identitylib-1.6.0/identitylib/student_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      509 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18407 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.806756 ucam-identitylib-1.6.0/identitylib/student_client/model/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15305 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation.py
+-rw-r--r--   0 root         (0) root         (0)    14466 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    13235 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/http_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13438 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    13725 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/identifier.py
+-rw-r--r--   0 root         (0) root         (0)    14035 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/identifier_scheme.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/location_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14202 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/paginated_results_student.py
+-rw-r--r--   0 root         (0) root         (0)    16439 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/student.py
+-rw-r--r--   0 root         (0) root         (0)    13802 2023-05-12 10:19:09.000000 ucam-identitylib-1.6.0/identitylib/student_client/model/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)    84357 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.806756 ucam-identitylib-1.6.0/identitylib/student_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16034 2023-05-12 10:19:10.000000 ucam-identitylib-1.6.0/identitylib/student_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/university_hr_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/identitylib/university_student_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 10:19:27.814756 ucam-identitylib-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-05-11 16:18:48.000000 ucam-identitylib-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.810757 ucam-identitylib-1.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 10:18:27.000000 ucam-identitylib-1.6.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5517 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/tests/test_api_client_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2023-05-11 10:55:25.000000 ucam-identitylib-1.6.0/tests/test_identifiers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:19:27.810757 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12396 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-12 10:19:27.000000 ucam-identitylib-1.6.0/ucam_identitylib.egg-info/top_level.txt
```

### Comparing `ucam-identitylib-1.5.0/PKG-INFO` & `ucam-identitylib-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-identitylib
-Version: 1.5.0
+Version: 1.6.0
 Summary: A module containing helpers and shared code related to identity systems within UIS, University of Cambridge.
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib
 Author: University of Cambridge Information Services
 Author-email: devops+ucam-identitylib@uis.cam.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ucam-identitylib-1.5.0/README.md` & `ucam-identitylib-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/api_client_mixin.py` & `ucam-identitylib-1.6.0/identitylib/api_client_mixin.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/__init__.py` & `ucam-identitylib-1.6.0/identitylib/card_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/api/permissions_api.py` & `ucam-identitylib-1.6.0/identitylib/card_client/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/api/v1beta1_api.py` & `ucam-identitylib-1.6.0/identitylib/card_client/api/v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from identitylib.card_client.model.card_request_distinct_values import CardRequestDistinctValues
 from identitylib.card_client.model.card_request_update_request_type import CardRequestUpdateRequestType
 from identitylib.card_client.model.card_request_update_response_type import CardRequestUpdateResponseType
 from identitylib.card_client.model.card_update_request_type import CardUpdateRequestType
 from identitylib.card_client.model.card_update_response_type import CardUpdateResponseType
 from identitylib.card_client.model.college_institution_ids_list_response_type import CollegeInstitutionIdsListResponseType
 from identitylib.card_client.model.paginated_available_barcode_type import PaginatedAvailableBarcodeType
-from identitylib.card_client.model.paginated_card_identifier_type import PaginatedCardIdentifierType
+from identitylib.card_client.model.paginated_card_identifier_summary_type import PaginatedCardIdentifierSummaryType
 from identitylib.card_client.model.paginated_card_logo_type import PaginatedCardLogoType
 from identitylib.card_client.model.paginated_card_note_type import PaginatedCardNoteType
 from identitylib.card_client.model.paginated_card_request_summary_type import PaginatedCardRequestSummaryType
 from identitylib.card_client.model.paginated_card_summary_type import PaginatedCardSummaryType
 from identitylib.card_client.model.validation_error import ValidationError
 
 
@@ -388,15 +388,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.v1beta1_card_identifiers_list_endpoint = _Endpoint(
             settings={
-                'response_type': (PaginatedCardIdentifierType,),
+                'response_type': (PaginatedCardIdentifierSummaryType,),
                 'auth': [
                     'API Service OAuth2 Client Credentials',
                     'API Service OAuth2 Access Code'
                 ],
                 'endpoint_path': '/v1beta1/card-identifiers',
                 'operation_id': 'v1beta1_card_identifiers_list',
                 'http_method': 'GET',
@@ -409,14 +409,15 @@
                     'retain_until__isnull',
                     'deleted_at__lte',
                     'deleted_at__gte',
                     'deleted_at__isnull',
                     'identifier',
                     'scheme',
                     'is_highest_primary_identifier',
+                    'is_deleted',
                     'cursor',
                     'page_size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
@@ -460,14 +461,16 @@
                         (bool,),
                     'identifier':
                         (str,),
                     'scheme':
                         (str,),
                     'is_highest_primary_identifier':
                         (bool,),
+                    'is_deleted':
+                        (bool,),
                     'cursor':
                         (str,),
                     'page_size':
                         (int,),
                 },
                 'attribute_map': {
                     'retain_until__lte': 'retain_until__lte',
@@ -475,27 +478,29 @@
                     'retain_until__isnull': 'retain_until__isnull',
                     'deleted_at__lte': 'deleted_at__lte',
                     'deleted_at__gte': 'deleted_at__gte',
                     'deleted_at__isnull': 'deleted_at__isnull',
                     'identifier': 'identifier',
                     'scheme': 'scheme',
                     'is_highest_primary_identifier': 'is_highest_primary_identifier',
+                    'is_deleted': 'is_deleted',
                     'cursor': 'cursor',
                     'page_size': 'page_size',
                 },
                 'location_map': {
                     'retain_until__lte': 'query',
                     'retain_until__gte': 'query',
                     'retain_until__isnull': 'query',
                     'deleted_at__lte': 'query',
                     'deleted_at__gte': 'query',
                     'deleted_at__isnull': 'query',
                     'identifier': 'query',
                     'scheme': 'query',
                     'is_highest_primary_identifier': 'query',
+                    'is_deleted': 'query',
                     'cursor': 'query',
                     'page_size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -1733,15 +1738,16 @@
                 },
                 'allowed_values': {
                     ('status',): {
 
                         "ISSUED": "ISSUED",
                         "REVOKED": "REVOKED",
                         "RETURNED": "RETURNED",
-                        "EXPIRED": "EXPIRED"
+                        "EXPIRED": "EXPIRED",
+                        "UNACTIVATED": "UNACTIVATED"
                     },
                 },
                 'openapi_types': {
                     'data':
                         (CardFilterRequestType,),
                     'status':
                         (str,),
@@ -1877,15 +1883,16 @@
                 },
                 'allowed_values': {
                     ('status',): {
 
                         "ISSUED": "ISSUED",
                         "REVOKED": "REVOKED",
                         "RETURNED": "RETURNED",
-                        "EXPIRED": "EXPIRED"
+                        "EXPIRED": "EXPIRED",
+                        "UNACTIVATED": "UNACTIVATED"
                     },
                     ('card_type',): {
 
                         "PERSONAL": "MIFARE_PERSONAL",
                         "TEMPORARY": "MIFARE_TEMPORARY"
                     },
                 },
@@ -2622,14 +2629,15 @@
             retain_until__isnull (bool): Filter retainUntil by IsoDateTime is Null. [optional]
             deleted_at__lte (datetime): Filter deletedAt by IsoDateTime less than. [optional]
             deleted_at__gte (datetime): Filter deletedAt by IsoDateTime greater than. [optional]
             deleted_at__isnull (bool): Filter deletedAt by IsoDateTime is Null. [optional]
             identifier (str): Filter identifiers by an identifier in the format {value}@{scheme}. [optional]
             scheme (str): Filter identifiers by an identifier scheme. [optional]
             is_highest_primary_identifier (bool): Filter is_highest_primary_identifier. [optional]
+            is_deleted (bool): Filter isDeleted. [optional]
             cursor (str): The pagination cursor value.. [optional]
             page_size (int): Number of results to return per page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -2656,15 +2664,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            PaginatedCardIdentifierType
+            PaginatedCardIdentifierSummaryType
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -4777,15 +4785,15 @@
         self,
         id,
         data,
         **kwargs
     ):
         """Update the card  # noqa: E501
 
-         ## Update the card  This method allows a client to submit an action in the request body and optional note for a given card. The allowed action is `cancel`.  For the `cancel` action, the client can optionally append a `note` describing the reason for cancelling the card.  ### Permissions  Principals with the `CARD_UPDATER` permission will be able to affect this endpoint.    # noqa: E501
+         ## Update the card  This method allows a client to submit an action in the request body and optional note for a given card. The allowed action is `cancel`.  The `cancel` action cancels the card. The client can optionally append a `note` describing the reason for cancelling the card.  The `refresh` action refreshes the card state. If the card is UNACTIVATED and the cardholder does not have an ISSUED card, the card state will be updated to ISSUED.  ### Permissions  Principals with the `CARD_UPDATER` permission will be able to affect this endpoint.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.v1beta1_cards_update(id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/api/versions_api.py` & `ucam-identitylib-1.6.0/identitylib/card_client/api/versions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/api_client.py` & `ucam-identitylib-1.6.0/identitylib/card_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/apis/__init__.py` & `ucam-identitylib-1.6.0/identitylib/card_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/configuration.py` & `ucam-identitylib-1.6.0/identitylib/card_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/exceptions.py` & `ucam-identitylib-1.6.0/identitylib/card_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/api_exception.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/api_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_batch_response_type_details_invalid_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/available_barcode_create_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/available_barcode_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.card_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.card_client.model.card_identifier import CardIdentifier
+    from identitylib.card_client.model.card_identifier_summary import CardIdentifierSummary
     from identitylib.card_client.model.card_note import CardNote
-    globals()['CardIdentifier'] = CardIdentifier
+    globals()['CardIdentifierSummary'] = CardIdentifierSummary
     globals()['CardNote'] = CardNote
 
 
 class Card(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -63,14 +63,15 @@
 
     allowed_values = {
         ('status',): {
             'ISSUED': "ISSUED",
             'REVOKED': "REVOKED",
             'RETURNED': "RETURNED",
             'EXPIRED': "EXPIRED",
+            'UNACTIVATED': "UNACTIVATED",
         },
         ('card_type',): {
             'PERSONAL': "MIFARE_PERSONAL",
             'TEMPORARY': "MIFARE_TEMPORARY",
         },
     }
 
@@ -101,15 +102,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'can_update': (bool,),  # noqa: E501
-            'identifiers': ([CardIdentifier],),  # noqa: E501
+            'identifiers': ([CardIdentifierSummary],),  # noqa: E501
             'notes': ([CardNote],),  # noqa: E501
             'status': (str,),  # noqa: E501
             'attributes': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'back_visualization_link': (str,),  # noqa: E501
             'card_type': (str,),  # noqa: E501
             'expires_at': (datetime, none_type,),  # noqa: E501
             'front_visualization_link': (str,),  # noqa: E501
@@ -159,15 +160,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, can_update, identifiers, notes, status, *args, **kwargs):  # noqa: E501
         """Card - a model defined in OpenAPI
 
         Args:
             can_update (bool):
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             notes ([CardNote]):
             status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -266,15 +267,15 @@
 
     @convert_js_args_to_python_args
     def __init__(self, can_update, identifiers, notes, status, *args, **kwargs):  # noqa: E501
         """Card - a model defined in OpenAPI
 
         Args:
             can_update (bool):
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             notes ([CardNote]):
             status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_request_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     allowed_values = {
         ('status',): {
             'ISSUED': "ISSUED",
             'REVOKED': "REVOKED",
             'RETURNED': "RETURNED",
             'EXPIRED': "EXPIRED",
+            'UNACTIVATED': "UNACTIVATED",
         },
     }
 
     validations = {
     }
 
     @cached_property
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_filter_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_filter_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.card_client.exceptions import ApiAttributeError
 
 
 
-class CardIdentifier(ModelNormal):
+class CardIdentifierSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -120,15 +120,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, scheme, value, *args, **kwargs):  # noqa: E501
-        """CardIdentifier - a model defined in OpenAPI
+        """CardIdentifierSummary - a model defined in OpenAPI
 
         Args:
             scheme (str): The identifier's scheme
             value (str): The identifier's value
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -212,15 +212,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, scheme, value, *args, **kwargs):  # noqa: E501
-        """CardIdentifier - a model defined in OpenAPI
+        """CardIdentifierSummary - a model defined in OpenAPI
 
         Args:
             scheme (str): The identifier's scheme
             value (str): The identifier's value
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_destroy_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_destroy_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_identifier_update_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_identifier_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_logo.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_logo.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_create_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_note_destroy_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_note_destroy_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.card_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.card_client.model.card_identifier import CardIdentifier
-    globals()['CardIdentifier'] = CardIdentifier
+    from identitylib.card_client.model.card_identifier_summary import CardIdentifierSummary
+    globals()['CardIdentifierSummary'] = CardIdentifierSummary
 
 
 class CardRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -155,15 +155,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'can_update': (bool,),  # noqa: E501
-            'identifiers': ([CardIdentifier],),  # noqa: E501
+            'identifiers': ([CardIdentifierSummary],),  # noqa: E501
             'workflow_state': (str,),  # noqa: E501
             'affiliations': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
             'attributes': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'back_visualization_link': (str,),  # noqa: E501
             'cancel_reason': (str, none_type,),  # noqa: E501
             'card_request_version': (int,),  # noqa: E501
             'card_type': (str,),  # noqa: E501
@@ -230,15 +230,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, can_update, identifiers, workflow_state, *args, **kwargs):  # noqa: E501
         """CardRequest - a model defined in OpenAPI
 
         Args:
             can_update (bool):
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             workflow_state (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -343,15 +343,15 @@
 
     @convert_js_args_to_python_args
     def __init__(self, can_update, identifiers, workflow_state, *args, **kwargs):  # noqa: E501
         """CardRequest - a model defined in OpenAPI
 
         Args:
             can_update (bool):
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             workflow_state (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_fields.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_request_type_updates_inner_identifiers_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_bulk_update_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_bulk_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_create_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_create_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_distinct_values.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_distinct_values.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_summary.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.card_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.card_client.model.card_identifier import CardIdentifier
-    globals()['CardIdentifier'] = CardIdentifier
+    from identitylib.card_client.model.card_identifier_summary import CardIdentifierSummary
+    globals()['CardIdentifierSummary'] = CardIdentifierSummary
 
 
 class CardRequestSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -154,15 +154,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'identifiers': ([CardIdentifier],),  # noqa: E501
+            'identifiers': ([CardIdentifierSummary],),  # noqa: E501
             'workflow_state': (str,),  # noqa: E501
             'back_visualization_link': (str,),  # noqa: E501
             'cancel_reason': (str, none_type,),  # noqa: E501
             'card_request_version': (int,),  # noqa: E501
             'card_type': (str,),  # noqa: E501
             'cardholder_status': (str,),  # noqa: E501
             'college_institution_id': (str, none_type,),  # noqa: E501
@@ -219,15 +219,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, identifiers, workflow_state, *args, **kwargs):  # noqa: E501
         """CardRequestSummary - a model defined in OpenAPI
 
         Args:
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             workflow_state (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -327,15 +327,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, identifiers, workflow_state, *args, **kwargs):  # noqa: E501
         """CardRequestSummary - a model defined in OpenAPI
 
         Args:
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             workflow_state (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_request_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_request_update_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_request_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_summary.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.card_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.card_client.model.card_identifier import CardIdentifier
-    globals()['CardIdentifier'] = CardIdentifier
+    from identitylib.card_client.model.card_identifier_summary import CardIdentifierSummary
+    globals()['CardIdentifierSummary'] = CardIdentifierSummary
 
 
 class CardSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -61,14 +61,15 @@
 
     allowed_values = {
         ('status',): {
             'ISSUED': "ISSUED",
             'REVOKED': "REVOKED",
             'RETURNED': "RETURNED",
             'EXPIRED': "EXPIRED",
+            'UNACTIVATED': "UNACTIVATED",
         },
         ('card_type',): {
             'PERSONAL': "MIFARE_PERSONAL",
             'TEMPORARY': "MIFARE_TEMPORARY",
         },
     }
 
@@ -98,15 +99,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'identifiers': ([CardIdentifier],),  # noqa: E501
+            'identifiers': ([CardIdentifierSummary],),  # noqa: E501
             'status': (str,),  # noqa: E501
             'back_visualization_link': (str,),  # noqa: E501
             'card_type': (str,),  # noqa: E501
             'expires_at': (datetime, none_type,),  # noqa: E501
             'front_visualization_link': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'issue_number': (int, none_type,),  # noqa: E501
@@ -150,15 +151,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, identifiers, status, *args, **kwargs):  # noqa: E501
         """CardSummary - a model defined in OpenAPI
 
         Args:
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -252,15 +253,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, identifiers, status, *args, **kwargs):  # noqa: E501
         """CardSummary - a model defined in OpenAPI
 
         Args:
-            identifiers ([CardIdentifier]):
+            identifiers ([CardIdentifierSummary]):
             status (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_request_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_request_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('action',): {
             'CANCEL': "cancel",
+            'REFRESH': "refresh",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -136,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            action (str): The action to apply to this card.. [optional] if omitted the server will use the default value of "cancel"  # noqa: E501
+            action (str): The action to apply to this card.. [optional]  # noqa: E501
             note (str): string. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -223,15 +224,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            action (str): The action to apply to this card.. [optional] if omitted the server will use the default value of "cancel"  # noqa: E501
+            action (str): The action to apply to this card.. [optional]  # noqa: E501
             note (str): string. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/card_update_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/card_update_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/college_institution_ids_list_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/college_institution_ids_list_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_available_barcode_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_available_barcode_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_identifier_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_identifier_summary_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from identitylib.card_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from identitylib.card_client.model.card_identifier import CardIdentifier
-    globals()['CardIdentifier'] = CardIdentifier
+    from identitylib.card_client.model.card_identifier_summary import CardIdentifierSummary
+    globals()['CardIdentifierSummary'] = CardIdentifierSummary
 
 
-class PaginatedCardIdentifierType(ModelNormal):
+class PaginatedCardIdentifierSummaryType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'results': ([CardIdentifier],),  # noqa: E501
+            'results': ([CardIdentifierSummary],),  # noqa: E501
             'count': (int,),  # noqa: E501
             'next': (str, none_type,),  # noqa: E501
             'previous': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -110,18 +110,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, results, *args, **kwargs):  # noqa: E501
-        """PaginatedCardIdentifierType - a model defined in OpenAPI
+        """PaginatedCardIdentifierSummaryType - a model defined in OpenAPI
 
         Args:
-            results ([CardIdentifier]):
+            results ([CardIdentifierSummary]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -202,18 +202,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, results, *args, **kwargs):  # noqa: E501
-        """PaginatedCardIdentifierType - a model defined in OpenAPI
+        """PaginatedCardIdentifierSummaryType - a model defined in OpenAPI
 
         Args:
-            results ([CardIdentifier]):
+            results ([CardIdentifierSummary]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_logo_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_logo_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_note_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_note_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_request_summary_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_request_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/paginated_card_summary_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/paginated_card_summary_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/permissions_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/permissions_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/validation_error.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model/version_response_type.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model/version_response_type.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/model_utils.py` & `ucam-identitylib-1.6.0/identitylib/card_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/models/__init__.py` & `ucam-identitylib-1.6.0/identitylib/card_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from identitylib.card_client.model.card_filter_response_type import CardFilterResponseType
 from identitylib.card_client.model.card_identifier import CardIdentifier
 from identitylib.card_client.model.card_identifier_bulk_update_request_type import CardIdentifierBulkUpdateRequestType
 from identitylib.card_client.model.card_identifier_bulk_update_request_type_updates_inner import CardIdentifierBulkUpdateRequestTypeUpdatesInner
 from identitylib.card_client.model.card_identifier_bulk_update_response_type import CardIdentifierBulkUpdateResponseType
 from identitylib.card_client.model.card_identifier_bulk_update_response_type_details_inner import CardIdentifierBulkUpdateResponseTypeDetailsInner
 from identitylib.card_client.model.card_identifier_destroy_response_type import CardIdentifierDestroyResponseType
+from identitylib.card_client.model.card_identifier_summary import CardIdentifierSummary
 from identitylib.card_client.model.card_identifier_update_request_type import CardIdentifierUpdateRequestType
 from identitylib.card_client.model.card_identifier_update_response_type import CardIdentifierUpdateResponseType
 from identitylib.card_client.model.card_logo import CardLogo
 from identitylib.card_client.model.card_note import CardNote
 from identitylib.card_client.model.card_note_create_request_type import CardNoteCreateRequestType
 from identitylib.card_client.model.card_note_destroy_request_type import CardNoteDestroyRequestType
 from identitylib.card_client.model.card_note_destroy_response_type import CardNoteDestroyResponseType
@@ -46,15 +47,15 @@
 from identitylib.card_client.model.card_request_update_request_type import CardRequestUpdateRequestType
 from identitylib.card_client.model.card_request_update_response_type import CardRequestUpdateResponseType
 from identitylib.card_client.model.card_summary import CardSummary
 from identitylib.card_client.model.card_update_request_type import CardUpdateRequestType
 from identitylib.card_client.model.card_update_response_type import CardUpdateResponseType
 from identitylib.card_client.model.college_institution_ids_list_response_type import CollegeInstitutionIdsListResponseType
 from identitylib.card_client.model.paginated_available_barcode_type import PaginatedAvailableBarcodeType
-from identitylib.card_client.model.paginated_card_identifier_type import PaginatedCardIdentifierType
+from identitylib.card_client.model.paginated_card_identifier_summary_type import PaginatedCardIdentifierSummaryType
 from identitylib.card_client.model.paginated_card_logo_type import PaginatedCardLogoType
 from identitylib.card_client.model.paginated_card_note_type import PaginatedCardNoteType
 from identitylib.card_client.model.paginated_card_request_summary_type import PaginatedCardRequestSummaryType
 from identitylib.card_client.model.paginated_card_summary_type import PaginatedCardSummaryType
 from identitylib.card_client.model.permissions_response_type import PermissionsResponseType
 from identitylib.card_client.model.validation_error import ValidationError
 from identitylib.card_client.model.version_response_type import VersionResponseType
```

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client/rest.py` & `ucam-identitylib-1.6.0/identitylib/card_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/card_client_configuration.py` & `ucam-identitylib-1.6.0/identitylib/card_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/__init__.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/api/staff_members_api.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/api/staff_members_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/api_client.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/apis/__init__.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/configuration.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/exceptions.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/affiliation_scheme.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/affiliation_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/http_exception.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/http_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/http_validation_error.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/identifier_scheme.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/identifier_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/location_inner.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/location_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/paginated_results_staff_member.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/paginated_results_staff_member.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/staff_member.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/staff_member.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model/validation_error.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/model_utils.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/models/__init__.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/hr_client/rest.py` & `ucam-identitylib-1.6.0/identitylib/hr_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/identifiers.py` & `ucam-identitylib-1.6.0/identitylib/identifiers.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/__init__.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api/default_api.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/api_client.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/apis/__init__.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/configuration.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/exceptions.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_datum.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_datum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model/mapping_response.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model/mapping_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/model_utils.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/models/__init__.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_client/rest.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/inst_identifier_configuration.py` & `ucam-identitylib-1.6.0/identitylib/inst_identifier_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/__init__.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/api/group_api.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/api/group_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/api/ibis_api.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/api/ibis_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/api/institution_api.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/api/institution_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/api/person_api.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/api/person_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/api_client.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/apis/__init__.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/configuration.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/exceptions.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/attribute_scheme.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/attribute_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_phone_number.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_phone_number.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_row.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_row.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/contact_web_page.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/contact_web_page.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/error.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_all_groups_default_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_cancelled_members200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_get_group200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_get_group200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_members_of_inst.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_members_of_inst.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/group_search_count200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/group_search_count200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_last_transaction_id200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/ibis_get_version200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/identifier.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_attribute_schemes200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_all_insts200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attribute200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_attributes200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_contact_rows200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/institution_get_inst200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_get_person200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_get_person200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_identifier.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model/person_is_member_of_group200_response_result.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/model_utils.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/models/__init__.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client/rest.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/lookup_client_configuration.py` & `ucam-identitylib-1.6.0/identitylib/lookup_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/__init__.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/all_photos_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/all_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/api_versions_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/api_versions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/approved_photos_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/approved_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/permissions_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifier_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifier_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/photo_identifiers_including_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/photos_including_unapproved_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api/unapproved_photos_api.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api/unapproved_photos_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/api_client.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/apis/__init__.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/configuration.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/exceptions.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/action_enum.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/action_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/api_versions.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/api_versions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/bad_request.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/bad_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/forbidden.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/forbidden.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/internal_server_error.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/internal_server_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/not_found.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/not_found.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_identifier_summary_list.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/paginated_v1_beta1_photo_list.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/permissions.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/permissions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_request_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/photo_identifier_bulk_update_update_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/scheme_enum.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/scheme_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/status_enum.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/status_enum.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/transient_image_url.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/transient_image_url.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/unauthorized.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/unauthorized.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model/v1_beta1_photo_identifier_summary_request.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/model_utils.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/models/__init__.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client/rest.py` & `ucam-identitylib-1.6.0/identitylib/photo_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/photo_client_configuration.py` & `ucam-identitylib-1.6.0/identitylib/photo_client_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/__init__.py` & `ucam-identitylib-1.6.0/identitylib/student_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/api/students_api.py` & `ucam-identitylib-1.6.0/identitylib/student_client/api/students_api.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/api_client.py` & `ucam-identitylib-1.6.0/identitylib/student_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/configuration.py` & `ucam-identitylib-1.6.0/identitylib/student_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/exceptions.py` & `ucam-identitylib-1.6.0/identitylib/student_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/affiliation_scheme.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/affiliation_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/http_exception.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/http_exception.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/http_validation_error.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/identifier.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/identifier.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/identifier_scheme.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/identifier_scheme.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/location_inner.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/location_inner.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/paginated_results_student.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/paginated_results_student.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/student.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/student.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model/validation_error.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/model_utils.py` & `ucam-identitylib-1.6.0/identitylib/student_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/models/__init__.py` & `ucam-identitylib-1.6.0/identitylib/student_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/student_client/rest.py` & `ucam-identitylib-1.6.0/identitylib/student_client/rest.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/university_hr_configuration.py` & `ucam-identitylib-1.6.0/identitylib/university_hr_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/identitylib/university_student_configuration.py` & `ucam-identitylib-1.6.0/identitylib/university_student_configuration.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/setup.py` & `ucam-identitylib-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 PACKAGE_NAME = "ucam-identitylib"
 PACKAGE_DESCRIPTION = (
     "A module containing helpers and shared code related to identity systems within UIS, "
     "University of Cambridge."
 )
-PACKAGE_VERSION = "1.5.0"
+PACKAGE_VERSION = "1.6.0"
 PACKAGE_URL = "https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib"
 
 
 def load_requirements(file: str):
     """
     Load requirements file and return non-empty, non-comment lines with leading and trailing
     whitespace stripped.
```

### Comparing `ucam-identitylib-1.5.0/tests/test_api_client_mixin.py` & `ucam-identitylib-1.6.0/tests/test_api_client_mixin.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/tests/test_identifiers.py` & `ucam-identitylib-1.6.0/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `ucam-identitylib-1.5.0/ucam_identitylib.egg-info/PKG-INFO` & `ucam-identitylib-1.6.0/ucam_identitylib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-identitylib
-Version: 1.5.0
+Version: 1.6.0
 Summary: A module containing helpers and shared code related to identity systems within UIS, University of Cambridge.
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/iam/identity-lib
 Author: University of Cambridge Information Services
 Author-email: devops+ucam-identitylib@uis.cam.ac.uk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ucam-identitylib-1.5.0/ucam_identitylib.egg-info/SOURCES.txt` & `ucam-identitylib-1.6.0/ucam_identitylib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 identitylib/card_client/model/card_filter_response_type.py
 identitylib/card_client/model/card_identifier.py
 identitylib/card_client/model/card_identifier_bulk_update_request_type.py
 identitylib/card_client/model/card_identifier_bulk_update_request_type_updates_inner.py
 identitylib/card_client/model/card_identifier_bulk_update_response_type.py
 identitylib/card_client/model/card_identifier_bulk_update_response_type_details_inner.py
 identitylib/card_client/model/card_identifier_destroy_response_type.py
+identitylib/card_client/model/card_identifier_summary.py
 identitylib/card_client/model/card_identifier_update_request_type.py
 identitylib/card_client/model/card_identifier_update_response_type.py
 identitylib/card_client/model/card_logo.py
 identitylib/card_client/model/card_note.py
 identitylib/card_client/model/card_note_create_request_type.py
 identitylib/card_client/model/card_note_destroy_request_type.py
 identitylib/card_client/model/card_note_destroy_response_type.py
@@ -60,15 +61,15 @@
 identitylib/card_client/model/card_rfid_data_config_list_response_type.py
 identitylib/card_client/model/card_rfid_data_config_list_response_type_results_inner.py
 identitylib/card_client/model/card_summary.py
 identitylib/card_client/model/card_update_request_type.py
 identitylib/card_client/model/card_update_response_type.py
 identitylib/card_client/model/college_institution_ids_list_response_type.py
 identitylib/card_client/model/paginated_available_barcode_type.py
-identitylib/card_client/model/paginated_card_identifier_type.py
+identitylib/card_client/model/paginated_card_identifier_summary_type.py
 identitylib/card_client/model/paginated_card_logo_type.py
 identitylib/card_client/model/paginated_card_note_type.py
 identitylib/card_client/model/paginated_card_request_summary_type.py
 identitylib/card_client/model/paginated_card_summary_type.py
 identitylib/card_client/model/permissions_response_type.py
 identitylib/card_client/model/validation_error.py
 identitylib/card_client/model/version_response_type.py
```

