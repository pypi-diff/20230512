# Comparing `tmp/edx-event-routing-backends-5.2.2.tar.gz` & `tmp/edx-event-routing-backends-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-5.2.2.tar", last modified: Mon Mar 13 08:27:26 2023, max compression
+gzip compressed data, was "edx-event-routing-backends-5.3.0.tar", last modified: Fri May 12 07:34:04 2023, max compression
```

## Comparing `edx-event-routing-backends-5.2.2.tar` & `edx-event-routing-backends-5.3.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.110564 edx-event-routing-backends-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6973 2023-03-13 08:27:26.110564 edx-event-routing-backends-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3803 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.094563 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6973 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4467 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-13 08:27:26.000000 edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.094563 edx-event-routing-backends-5.2.2/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.094563 edx-event-routing-backends-5.2.2/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5834 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/backends/events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.094563 edx-event-routing-backends-5.2.2/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13242 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.098563 edx-event-routing-backends-5.2.2/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.098563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.098563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.102563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5812 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.102563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.102563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.102563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.102563 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4585 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     9997 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4372 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7794 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.090563 edx-event-routing-backends-5.2.2/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.090563 edx-event-routing-backends-5.2.2/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (122)     3185 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.090563 edx-event-routing-backends-5.2.2/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.106564 edx-event-routing-backends-5.2.2/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.110564 edx-event-routing-backends-5.2.2/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.110564 edx-event-routing-backends-5.2.2/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 08:27:26.110564 edx-event-routing-backends-5.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-03-13 08:27:26.110564 edx-event-routing-backends-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-03-13 08:27:19.000000 edx-event-routing-backends-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2649 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7155 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.429394 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7155 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4467 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-12 07:34:04.000000 edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.429394 edx-event-routing-backends-5.3.0/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.429394 edx-event-routing-backends-5.3.0/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.433394 edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13413 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7942 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.433394 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.433394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.437394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4585 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9997 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.441394 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5335 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.425394 edx-event-routing-backends-5.3.0/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.425394 edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3185 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.425394 edx-event-routing-backends-5.3.0/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 07:34:04.445394 edx-event-routing-backends-5.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-12 07:34:04.449395 edx-event-routing-backends-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-05-12 07:33:59.000000 edx-event-routing-backends-5.3.0/setup.py
```

### Comparing `edx-event-routing-backends-5.2.2/CHANGELOG.rst` & `edx-event-routing-backends-5.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 
+[5.3.0]
+~~~~~~~
+
+* Use proper externalId types XAPI and CALIPER instead of LTI
+* Make user identifier in xAPI events configurable
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Make id of xAPI statements idempotent
+
 [5.2.2]
 ~~~~~~~
 
 * Rename toggle_warnings to toggle_warning for consistency with setting_warning.
 * Added session id to all events
 * add support for video interaction events.
 * Replaced eventVersion with transformerVersion to include semantic version of event-routing-backend package.
```

### Comparing `edx-event-routing-backends-5.2.2/LICENSE.txt` & `edx-event-routing-backends-5.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/PKG-INFO` & `edx-event-routing-backends-5.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.2.2
+Version: 5.3.0
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -53,16 +53,15 @@
 
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`__ for details.
-Even though they were written with ``edx-platform`` in mind, the guidelines
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`__ for details.
 should be followed for all Open edX projects.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <.github/ISSUE_TEMPLATE.md>`_.
@@ -122,14 +121,23 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 
+[5.3.0]
+~~~~~~~
+
+* Use proper externalId types XAPI and CALIPER instead of LTI
+* Make user identifier in xAPI events configurable
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Make id of xAPI statements idempotent
+
 [5.2.2]
 ~~~~~~~
 
 * Rename toggle_warnings to toggle_warning for consistency with setting_warning.
 * Added session id to all events
 * add support for video interaction events.
 * Replaced eventVersion with transformerVersion to include semantic version of event-routing-backend package.
```

### Comparing `edx-event-routing-backends-5.2.2/README.rst` & `edx-event-routing-backends-5.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`__ for details.
-Even though they were written with ``edx-platform`` in mind, the guidelines
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`__ for details.
 should be followed for all Open edX projects.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <.github/ISSUE_TEMPLATE.md>`_.
```

### Comparing `edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.2.2
+Version: 5.3.0
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -53,16 +53,15 @@
 
 Please see `LICENSE.txt <LICENSE.txt>`_ for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`__ for details.
-Even though they were written with ``edx-platform`` in mind, the guidelines
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`__ for details.
 should be followed for all Open edX projects.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <.github/ISSUE_TEMPLATE.md>`_.
@@ -122,14 +121,23 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 
+[5.3.0]
+~~~~~~~
+
+* Use proper externalId types XAPI and CALIPER instead of LTI
+* Make user identifier in xAPI events configurable
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Make id of xAPI statements idempotent
+
 [5.2.2]
 ~~~~~~~
 
 * Rename toggle_warnings to toggle_warning for consistency with setting_warning.
 * Added session id to all events
 * add support for video interaction events.
 * Replaced eventVersion with transformerVersion to include semantic version of event-routing-backend package.
```

### Comparing `edx-event-routing-backends-5.2.2/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-5.3.0/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/admin.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/apps.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/backends/events_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,20 @@
         Event is processed through the configured processors. A router config
         object matching the backend_name and other match params is used to get
         the list of hosts to which the event is required to be delivered to.
 
         Arguments:
             event (dict):      original event dictionary
         """
+        routers = RouterConfiguration.get_enabled_routers(self.backend_name)
+
+        if not routers:
+            logger.info('Could not find any enabled router configuration for backend %s', self.backend_name)
+            return
+
         try:
             event_name = event['name']
         except TypeError as exc:
             raise ValueError('Expected event as dict but {type} was given.'.format(type=type(event))) from exc
         try:
             logger.debug('Processing edx event "{}" for router with backend {}'.format(event_name, self.backend_name))
 
@@ -60,20 +66,14 @@
         logger.debug(
             'Successfully processed edx event "%s" for router with backend %s. Processed event: %s',
             event_name,
             self.backend_name,
             processed_event
         )
 
-        routers = RouterConfiguration.get_enabled_routers(self.backend_name)
-
-        if not routers:
-            logger.error('Could not find any enabled router configuration for backend %s', self.backend_name)
-            return
-
         for router in routers:
             host = router.get_allowed_host(event)
 
             router_url = router.route_url
             if not host:
                 logger.info(
                     'Event %s is not allowed to be sent to any host for router %s with backend "%s"',
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/backends/tests/test_events_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,22 +80,25 @@
             },
         }
 
         self.router = EventsRouter(processors=[], backend_name='test')
 
     @patch('event_routing_backends.utils.http_client.requests.post')
     @patch('event_routing_backends.backends.events_router.logger')
-    def test_with_processor_exception(self, mocked_logger, mocked_post):
+    @patch('event_routing_backends.models.RouterConfiguration.get_enabled_routers')
+    def test_with_processor_exception(self, mocked_get_enabled_routers, mocked_logger, mocked_post):
         processors = [
             MagicMock(return_value=self.transformed_event),
             MagicMock(side_effect=EventEmissionExit, return_value=self.transformed_event),
             MagicMock(return_value=self.transformed_event),
         ]
         processors[1].side_effect = EventEmissionExit
 
+        mocked_get_enabled_routers.return_value = ['test']
+
         router = EventsRouter(processors=processors, backend_name='test')
         router.send(self.transformed_event)
 
         processors[0].assert_called_once_with(self.transformed_event)
         processors[1].assert_called_once_with(self.transformed_event)
         processors[2].assert_not_called()
 
@@ -139,15 +142,15 @@
         router = EventsRouter(processors=[], backend_name='test')
         router.send(self.transformed_event)
 
         mocked_post.assert_not_called()
 
         self.assertIn(
             call('Could not find any enabled router configuration for backend %s', 'test'),
-            mocked_logger.error.mock_calls
+            mocked_logger.info.mock_calls
         )
 
     @patch('event_routing_backends.utils.http_client.requests.post')
     @patch('event_routing_backends.tasks.logger')
     def test_with_unsupported_routing_strategy(self, mocked_logger, mocked_post):
         RouterConfigurationFactory.create(
             backend_name='test_backend',
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/helpers.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,132 @@
 """
 Helper utilities for event transformers.
 """
+import datetime
 import logging
-from datetime import timedelta
+import uuid
 from urllib.parse import parse_qs, urlparse
-from uuid import uuid4
 
+# Imported from edx-platform
+# pylint: disable=import-error
+from common.djangoapps.student.models import get_potentially_retired_user_by_username
 from dateutil.parser import parse
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from isodate import duration_isoformat
-# Imported from edx-platform
-# pylint: disable=import-error
 from opaque_keys.edx.keys import CourseKey
 from openedx.core.djangoapps.content.course_overviews.api import get_course_overviews
 from openedx.core.djangoapps.external_user_ids.models import ExternalId, ExternalIdType
 
 logger = logging.getLogger(__name__)
 User = get_user_model()
 
 UTC_DATETIME_FORMAT = '%Y-%m-%dT%H:%M:%S.%f'
 
 
-def get_anonymous_user_id(username_or_id):
+def get_uuid5(namespace_key, name):
+    """
+    Create a UUID5 string based on custom namesapce and name.
+
+    Arguments:
+    namespace_key (str):    key to be used to create a custom namespace
+    name  (str):            string for which we need to creat a UUID
+
+    Returns:
+        str
+
+    """
+    # We are not pulling base uuid from settings to avoid
+    # data discrepancies incase setting is changed inadvertently
+    base_uuid = uuid.UUID('6ba7b810-9dad-11d1-80b4-00c04fd430c8')
+    base_namespace = uuid.uuid5(base_uuid, namespace_key)
+    return uuid.uuid5(base_namespace, name)
+
+
+def get_anonymous_user_id(username_or_id, external_type):
     """
     Generate anonymous user id.
 
     Generate anonymous id for student.
     In case of anonymous user, return random uuid.
 
     Arguments:
         username_or_id (str):     username for the learner
+        external_type  (str):     external type id e.g caliper or xapi
 
     Returns:
         str
     """
+    user = get_user(username_or_id)
+    if not user:
+        logger.info('User with username "%s" does not exist. '
+                    'Cannot generate anonymous ID', username_or_id)
+
+        anonymous_id = str(uuid.uuid4())
+    else:
+        type_name = getattr(ExternalIdType, external_type)
+        external_id, _ = ExternalId.add_new_user_id(user, type_name)
+        if not external_id:
+            raise ValueError("External ID type: %s does not exist" % type_name)
+
+        anonymous_id = str(external_id.external_user_id)
+
+    return anonymous_id
+
+
+def get_user(username_or_id):
+    """
+    Get user by username or user id.
+
+    Arguments:
+        username_or_id (str):     username or user id of the learner
+
+    Returns:
+        user object
+    """
     user = user_id = username = None
     if username_or_id:
         try:
             user_id = int(username_or_id)
         except ValueError:
             username = username_or_id
 
     if username:
         user = User.objects.filter(username=username).first()
     elif user_id:
         user = User.objects.filter(id=user_id).first()
 
-    if not user:
-        logger.info('User with username "%s" does not exist. '
-                    'Cannot generate anonymous ID', username_or_id)
+    if username and not user:
+        try:
+            user = get_potentially_retired_user_by_username(username)
+        except Exception as ex:  # pylint: disable=broad-except
+            logger.info('User with username "%s" does not exist.%s', username, ex)
 
-        anonymous_id = str(uuid4())
-    else:
-        type_name = ExternalIdType.LTI
-        external_id, _ = ExternalId.add_new_user_id(user, type_name)
-        if not external_id:
-            raise ValueError("External ID type: %s does not exist" % type_name)
+    return user
 
-        anonymous_id = str(external_id.external_user_id)
 
-    return anonymous_id
+def get_user_email(username_or_id):
+    """
+    Get user's email from username or user id.
+
+    Arguments:
+        username_or_id (str):     username for the learner
+
+    Returns:
+        str
+    """
+    user = get_user(username_or_id)
+
+    if not user:
+        logger.info('User with username "%s" does not exist.', username_or_id)
+        user_email = 'unknown@example.com'
+    else:
+        user_email = user.email
+
+    return user_email
 
 
 def get_course_from_id(course_id):
     """
     Get Course object using the `course_id`.
 
     Arguments:
@@ -85,15 +147,15 @@
         seconds (int): number of seconds
 
     Returns:
         str
     """
     if seconds is None:
         return None
-    return duration_isoformat(timedelta(
+    return duration_isoformat(datetime.timedelta(
         seconds=seconds
     ))
 
 
 def convert_seconds_to_float(seconds):
     """
     Convert seconds from integer to Float format.
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/models.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             object_id = get_problem_block_id(
                 self.get_data('context.referer', True),
                 self.get_data('data'),
                 self.get_data('context.course_id')
             )
         key = self.get_event_name_key()
 
-        anonymous_user_id = get_anonymous_user_id(self.extract_username_or_userid())
+        anonymous_user_id = get_anonymous_user_id(self.extract_username_or_userid(), 'CALIPER')
         if key == 'showanswer':
             iri_url = '{}/solution'.format(object_id)
         elif key == 'edx.problem.hint.demandhint_displayed':
             iri_url = '{}/hint/{}'.format(object_id, event_data.get('hint_index', ''))
         elif key == 'problem_check_server':
             iri_url = '{}/user/{}/attempt/{}'.format(
                 object_id,
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def _add_actor_info(self):
         """
         Add all generic information related to `actor`.
         """
         self.transformed_event['actor'] = {
             'id': self.get_object_iri(
                 'user',
-                get_anonymous_user_id(self.extract_username_or_userid()),
+                get_anonymous_user_id(self.extract_username_or_userid(), 'CALIPER'),
             ),
             'type': 'Person'
         }
 
     def _add_session_info(self):
         """
         Add session info related to the event
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # no limit to diff in the output of tests
     maxDiff = None
 
     registry = None
     EXCEPTED_EVENTS_FIXTURES_PATH = None
 
     def setUp(self):
-        UserFactory.create(username='edx')
+        UserFactory.create(username='edx', email='edx@example.com')
 
     def get_raw_event(self, event_filename):
         """
         Return raw event json parsed from current fixtures
         """
 
         input_event_file_path = '{test_dir}/fixtures/current/{event_filename}'.format(
@@ -85,18 +85,19 @@
 
     @abstractmethod
     def compare_events(self, transformed_event, expected_event):
         """
         Every transformer's test case will implement its own logic to test
         events transformation
         """
-    @patch('event_routing_backends.helpers.uuid4')
+    @patch('event_routing_backends.helpers.uuid')
     @ddt.data(*EVENT_FIXTURE_FILENAMES)
-    def test_event_transformer(self, event_filename, mocked_uuid4):
-        mocked_uuid4.return_value = '32e08e30-f8ae-4ce2-94a8-c2bfe38a70cb'
+    def test_event_transformer(self, event_filename, mocked_uuid):
+        mocked_uuid.uuid4.return_value = '32e08e30-f8ae-4ce2-94a8-c2bfe38a70cb'
+        mocked_uuid.uuid5.return_value = '32e08e30-f8ae-4ce2-94a8-c2bfe38a70cb'
 
         # if an event's expected fixture doesn't exist, the test shouldn't fail.
         # evaluate transformation of only supported event fixtures.
         expected_event_file_path = '{expected_events_fixtures_path}/{event_filename}'.format(
             expected_events_fixtures_path=self.EXCEPTED_EVENTS_FIXTURES_PATH, event_filename=event_filename
         )
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 """
-Test the transformers for all of the currently supported events into xAPI format.
+xAPI processor for transforming and routing events.
 """
 import json
-import os
+from logging import getLogger
 
-from django.test import TestCase
+from eventtracking.processors.exceptions import NoBackendEnabled
 
-from event_routing_backends.processors.tests.transformers_test_mixin import TransformersTestMixin
-from event_routing_backends.processors.xapi import constants
+from event_routing_backends.processors.mixins.base_transformer_processor import BaseTransformerProcessorMixin
+from event_routing_backends.processors.xapi import XAPI_EVENTS_ENABLED
 from event_routing_backends.processors.xapi.registry import XApiTransformersRegistry
 
+xapi_logger = getLogger('xapi_tracking')
 
-class TestXApiTransformers(TransformersTestMixin, TestCase):
+
+class XApiProcessor(BaseTransformerProcessorMixin):
     """
-    Test that supported events are transformed into xAPI format correctly.
+    xAPI Processor for transforming and routing events.
+
+    This processor first transform the event using the registered transformer
+    and then route the events through the configured routers.
+
+    Every router configured to be used MUST support the transformed event type.
     """
-    EXCEPTED_EVENTS_FIXTURES_PATH = '{}/fixtures/expected'.format(os.path.dirname(os.path.abspath(__file__)))
-    registry = XApiTransformersRegistry
 
-    def assert_correct_transformer_version(self, transformed_event, transformer_version):
-        self.assertEqual(
-            transformed_event.context.extensions[constants.XAPI_TRANSFORMER_VERSION_KEY],
-            transformer_version
-        )
+    registry = XApiTransformersRegistry
 
-    def compare_events(self, transformed_event, expected_event):
+    def transform_event(self, event):
         """
-        Test that transformed_event and expected_event are identical.
+        Transform the event into IMS xAPI format.
 
         Arguments:
-            transformed_event (dict)
-            expected_event (dict)
+            event (dict):   Event to be transformed.
+
+        Returns:
+            dict:           transformed event
 
         Raises:
-            AssertionError:     Raised if the two events are not same.
+            Any Exception
         """
-        # id is a randomly generated UUID therefore not comparing that
-        transformed_event_json = json.loads(transformed_event.to_json())
-        self.assertIn('id', transformed_event_json)
-        expected_event.pop('id')
-        transformed_event_json.pop('id')
-        self.assertDictEqual(expected_event, transformed_event_json)
+        if not XAPI_EVENTS_ENABLED.is_enabled():
+            raise NoBackendEnabled
+
+        transformed_event = super().transform_event(event)
+
+        if transformed_event:
+            event_json = transformed_event.to_json()
+            xapi_logger.info(event_json)
+            xapi_logger.info('xAPI statement of edx event "{}" is: {}'.format(event["name"], event_json))
+            return json.loads(event_json)
+
+        return transformed_event
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/settings/production.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/settings/production.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,7 +27,11 @@
         'EVENT_TRACKING_BACKENDS',
         settings.EVENT_TRACKING_BACKENDS
     )
     settings.EVENT_TRACKING_BACKENDS_BUSINESS_CRITICAL_EVENTS = settings.ENV_TOKENS.get(
         'EVENT_TRACKING_BACKENDS_BUSINESS_CRITICAL_EVENTS',
         settings.EVENT_TRACKING_BACKENDS_BUSINESS_CRITICAL_EVENTS
     )
+    settings.XAPI_AGENT_IFI_TYPE = settings.ENV_TOKENS.get(
+        'XAPI_AGENT_IFI_TYPE',
+        settings.XAPI_AGENT_IFI_TYPE
+    )
```

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-5.3.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/tasks.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-5.3.0/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/requirements/constraints.txt` & `edx-event-routing-backends-5.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.2.2/setup.py` & `edx-event-routing-backends-5.3.0/setup.py`

 * *Files identical despite different names*

