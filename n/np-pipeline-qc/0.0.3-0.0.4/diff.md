# Comparing `tmp/np-pipeline-qc-0.0.3.tar.gz` & `tmp/np-pipeline-qc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-pipeline-qc-0.0.3.tar", last modified: Thu May 11 21:20:01 2023, max compression
+gzip compressed data, was "np-pipeline-qc-0.0.4.tar", last modified: Fri May 12 15:25:48 2023, max compression
```

## Comparing `np-pipeline-qc-0.0.3.tar` & `np-pipeline-qc-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1755 2023-05-11 21:19:50.340900 np-pipeline-qc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-20 03:48:03.334962 np-pipeline-qc-0.0.3/README.md
--rw-r--r--   0        0        0      202 2023-03-28 18:46:08.810584 np-pipeline-qc-0.0.3/src/np_pipeline_qc/__init__.py
--rw-r--r--   0        0        0     1942 2023-05-11 18:29:20.081508 np-pipeline-qc-0.0.3/src/np_pipeline_qc/__main__.py
--rw-r--r--   0        0        0    12014 2023-05-11 18:29:15.325811 np-pipeline-qc-0.0.3/src/np_pipeline_qc/classes.py
--rw-r--r--   0        0        0      361 2023-03-20 23:08:53.447944 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/__init__.py
--rw-r--r--   0        0        0     1359 2023-03-21 01:12:26.050925 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/align_physiology_plots.py
--rw-r--r--   0        0        0    71949 2023-04-21 20:37:34.750764 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/analysis.py
--rw-r--r--   0        0        0    23845 2023-03-21 01:12:26.955572 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/analyze_nwb.py
--rw-r--r--   0        0        0       93 2023-03-21 01:12:25.990930 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_copy_d2_files_for_LIMS_upload.py
--rw-r--r--   0        0        0      663 2023-03-21 01:12:26.022929 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_copy_d2_lims_files.py
--rw-r--r--   0        0        0     3775 2023-03-21 01:12:26.356528 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_hab_qc.py
--rw-r--r--   0        0        0     3344 2023-03-21 01:12:26.241483 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_lims_validation.py
--rw-r--r--   0        0        0     6543 2023-03-21 01:12:26.468049 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_qc.py
--rw-r--r--   0        0        0     7665 2023-03-21 01:12:26.632048 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_rf.py
--rw-r--r--   0        0        0     4366 2023-03-21 01:12:26.395527 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_variability_qc.py
--rw-r--r--   0        0        0     4360 2023-03-21 01:12:26.663047 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/behavior_analysis.py
--rw-r--r--   0        0        0    14730 2023-03-21 01:12:27.892306 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/build_stim_tables.py
--rw-r--r--   0        0        0     3971 2023-03-21 01:12:26.113445 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/channel_visual_modulation.py
--rw-r--r--   0        0        0    10124 2023-03-21 01:12:26.597048 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/check_datacube.py
--rw-r--r--   0        0        0     9558 2023-03-21 01:12:26.495049 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/copy_d2_lims_files_for_upload.py
--rw-r--r--   0        0        0     5030 2023-03-21 01:12:26.279483 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/D1_LIMS_schema.py
--rw-r--r--   0        0        0     7239 2023-03-21 01:41:14.441337 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/D1_local_schema.py
--rw-r--r--   0        0        0      346 2023-03-21 01:12:26.118446 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/D2_LIMS_schema.py
--rw-r--r--   0        0        0    18647 2023-03-21 01:12:27.127735 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/d2_upload_tool.py
--rw-r--r--   0        0        0    14102 2023-03-21 01:12:26.792572 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/data_getters.py
--rw-r--r--   0        0        0     1784 2023-03-21 01:12:26.401527 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/ebs_analysis.py
--rw-r--r--   0        0        0   105598 2023-03-21 01:12:31.741978 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/ebs_object_analysis.py
--rw-r--r--   0        0        0     9493 2023-03-21 01:12:26.936571 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/ecephys.py
--rw-r--r--   0        0        0    15873 2023-03-21 01:12:27.354342 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/EcephysBehaviorSession.py
--rw-r--r--   0        0        0     2007 2023-03-21 01:12:26.504048 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/get_probe_info.py
--rw-r--r--   0        0        0    12436 2023-05-10 00:34:14.618894 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/get_RFs_standalone.py
--rw-r--r--   0        0        0     5213 2023-03-21 01:12:26.892572 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/get_sessions.py
--rw-r--r--   0        0        0    10055 2023-03-21 01:12:26.957571 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/lims_validation.py
--rw-r--r--   0        0        0     2924 2023-03-21 01:12:26.670048 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/local_data_validation.py
--rw-r--r--   0        0        0     4234 2023-03-21 01:12:27.080572 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/nwb_validation_optotagging.py
--rw-r--r--   0        0        0    13017 2023-03-21 01:12:27.496862 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/probe_alignment_data_io.py
--rw-r--r--   0        0        0    13117 2023-03-21 01:12:27.267124 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/probe_track_day_assignment.py
--rw-r--r--   0        0        0    38430 2023-03-21 01:12:28.522367 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/probeSync_qc.py
--rw-r--r--   0        0        0     4046 2023-03-21 01:12:26.895572 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/qc_cmd_caller.py
--rw-r--r--   0        0        0     2339 2023-03-21 01:12:27.039571 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/query_lims.py
--rw-r--r--   0        0        0    10435 2023-03-21 01:12:27.586861 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/reformat_probe_annotation_files.py
--rw-r--r--   0        0        0     8107 2023-03-21 01:12:27.359339 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/run_qc_callable.py
--rw-r--r--   0        0        0    43266 2023-05-11 20:54:00.785726 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/run_qc_class.py
--rw-r--r--   0        0        0     4493 2023-03-21 01:12:27.184600 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/run_qc_modular.py
--rw-r--r--   0        0        0     1335 2023-03-21 01:12:27.024570 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/save_ecephysbehavior_session.py
--rw-r--r--   0        0        0    22271 2023-03-22 21:36:17.781279 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/sync_dataset.py
--rw-r--r--   0        0        0    13136 2023-03-21 01:12:27.985904 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/task1_behavior_session.py
--rw-r--r--   0        0        0     6237 2023-03-21 01:12:27.466862 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/update_probe_json.py
--rw-r--r--   0        0        0     2430 2023-03-21 01:12:27.390341 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/upload_D1_to_incoming.py
--rw-r--r--   0        0        0     8217 2023-03-21 01:12:27.611911 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/upload_opt_to_lims.py
--rw-r--r--   0        0        0    33585 2023-03-21 01:14:23.990065 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/validate_local_d2_files.py
--rw-r--r--   0        0        0    11132 2023-03-21 01:12:27.881307 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/validate_local_d2_files_ccb.py
--rw-r--r--   0        0        0     9536 2023-03-21 01:14:23.582115 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/validate_metadata_tables_VBN_release.py
--rw-r--r--   0        0        0     4266 2023-03-21 01:12:27.608910 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/vbn_stim_timing_test.py
--rw-r--r--   0        0        0     4792 2023-03-28 18:33:09.567280 np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/vbn_stim_timing_test_SDK.py
--rw-r--r--   0        0        0       70 2023-03-24 22:40:01.121024 np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/__init__.py
--rw-r--r--   0        0        0      667 2023-03-21 18:27:15.617982 np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/assets/html_templates.py
--rw-r--r--   0        0        0      928 2022-12-15 21:34:04.058641 np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/assets/single_page_img_json_report.css
--rw-r--r--   0        0        0     6312 2023-03-24 22:40:01.359023 np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/qc2html.py
--rw-r--r--   0        0        0       15 2023-03-27 23:09:19.768234 np-pipeline-qc-0.0.3/src/np_pipeline_qc/sorted/__init__.py
--rw-r--r--   0        0        0    13176 2023-04-03 20:33:29.822069 np-pipeline-qc-0.0.3/src/np_pipeline_qc/sorted/spike_depths.py
--rw-r--r--   0        0        0       20 2023-03-27 23:50:38.700137 np-pipeline-qc-0.0.3/src/np_pipeline_qc/utils/__init__.py
--rw-r--r--   0        0        0     4547 2023-03-27 23:51:59.489831 np-pipeline-qc-0.0.3/src/np_pipeline_qc/utils/utils.py
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 np-pipeline-qc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1853 2023-05-12 15:25:36.850906 np-pipeline-qc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-20 03:48:03.334962 np-pipeline-qc-0.0.4/README.md
+-rw-r--r--   0        0        0      202 2023-03-28 18:46:08.810584 np-pipeline-qc-0.0.4/src/np_pipeline_qc/__init__.py
+-rw-r--r--   0        0        0     1942 2023-05-11 18:29:20.081508 np-pipeline-qc-0.0.4/src/np_pipeline_qc/__main__.py
+-rw-r--r--   0        0        0    12014 2023-05-11 18:29:15.325811 np-pipeline-qc-0.0.4/src/np_pipeline_qc/classes.py
+-rw-r--r--   0        0        0      361 2023-03-20 23:08:53.447944 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/__init__.py
+-rw-r--r--   0        0        0     1359 2023-03-21 01:12:26.050925 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/align_physiology_plots.py
+-rw-r--r--   0        0        0    71949 2023-04-21 20:37:34.750764 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/analysis.py
+-rw-r--r--   0        0        0    23845 2023-03-21 01:12:26.955572 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/analyze_nwb.py
+-rw-r--r--   0        0        0       93 2023-03-21 01:12:25.990930 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_copy_d2_files_for_LIMS_upload.py
+-rw-r--r--   0        0        0      663 2023-03-21 01:12:26.022929 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_copy_d2_lims_files.py
+-rw-r--r--   0        0        0     3775 2023-03-21 01:12:26.356528 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_hab_qc.py
+-rw-r--r--   0        0        0     3344 2023-03-21 01:12:26.241483 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_lims_validation.py
+-rw-r--r--   0        0        0     6543 2023-03-21 01:12:26.468049 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_qc.py
+-rw-r--r--   0        0        0     7665 2023-03-21 01:12:26.632048 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_rf.py
+-rw-r--r--   0        0        0     4366 2023-03-21 01:12:26.395527 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_variability_qc.py
+-rw-r--r--   0        0        0     4360 2023-03-21 01:12:26.663047 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/behavior_analysis.py
+-rw-r--r--   0        0        0    14730 2023-03-21 01:12:27.892306 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/build_stim_tables.py
+-rw-r--r--   0        0        0     3971 2023-03-21 01:12:26.113445 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/channel_visual_modulation.py
+-rw-r--r--   0        0        0    10124 2023-03-21 01:12:26.597048 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/check_datacube.py
+-rw-r--r--   0        0        0     9558 2023-03-21 01:12:26.495049 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/copy_d2_lims_files_for_upload.py
+-rw-r--r--   0        0        0     5030 2023-03-21 01:12:26.279483 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/D1_LIMS_schema.py
+-rw-r--r--   0        0        0     7239 2023-03-21 01:41:14.441337 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/D1_local_schema.py
+-rw-r--r--   0        0        0      346 2023-03-21 01:12:26.118446 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/D2_LIMS_schema.py
+-rw-r--r--   0        0        0    18647 2023-03-21 01:12:27.127735 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/d2_upload_tool.py
+-rw-r--r--   0        0        0    14102 2023-03-21 01:12:26.792572 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/data_getters.py
+-rw-r--r--   0        0        0     1784 2023-03-21 01:12:26.401527 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/ebs_analysis.py
+-rw-r--r--   0        0        0   105598 2023-03-21 01:12:31.741978 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/ebs_object_analysis.py
+-rw-r--r--   0        0        0     9493 2023-03-21 01:12:26.936571 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/ecephys.py
+-rw-r--r--   0        0        0    15873 2023-03-21 01:12:27.354342 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/EcephysBehaviorSession.py
+-rw-r--r--   0        0        0     2007 2023-03-21 01:12:26.504048 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/get_probe_info.py
+-rw-r--r--   0        0        0    12436 2023-05-10 00:34:14.618894 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/get_RFs_standalone.py
+-rw-r--r--   0        0        0     5213 2023-03-21 01:12:26.892572 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/get_sessions.py
+-rw-r--r--   0        0        0    10055 2023-03-21 01:12:26.957571 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/lims_validation.py
+-rw-r--r--   0        0        0     2924 2023-03-21 01:12:26.670048 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/local_data_validation.py
+-rw-r--r--   0        0        0     4234 2023-03-21 01:12:27.080572 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/nwb_validation_optotagging.py
+-rw-r--r--   0        0        0    13017 2023-03-21 01:12:27.496862 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/probe_alignment_data_io.py
+-rw-r--r--   0        0        0    13117 2023-03-21 01:12:27.267124 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/probe_track_day_assignment.py
+-rw-r--r--   0        0        0    38430 2023-03-21 01:12:28.522367 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/probeSync_qc.py
+-rw-r--r--   0        0        0     4046 2023-03-21 01:12:26.895572 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/qc_cmd_caller.py
+-rw-r--r--   0        0        0     2339 2023-03-21 01:12:27.039571 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/query_lims.py
+-rw-r--r--   0        0        0    10435 2023-03-21 01:12:27.586861 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/reformat_probe_annotation_files.py
+-rw-r--r--   0        0        0     8107 2023-03-21 01:12:27.359339 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/run_qc_callable.py
+-rw-r--r--   0        0        0    43266 2023-05-11 20:54:00.785726 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/run_qc_class.py
+-rw-r--r--   0        0        0     4493 2023-03-21 01:12:27.184600 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/run_qc_modular.py
+-rw-r--r--   0        0        0     1335 2023-03-21 01:12:27.024570 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/save_ecephysbehavior_session.py
+-rw-r--r--   0        0        0    22271 2023-03-22 21:36:17.781279 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/sync_dataset.py
+-rw-r--r--   0        0        0    13136 2023-03-21 01:12:27.985904 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/task1_behavior_session.py
+-rw-r--r--   0        0        0     6237 2023-03-21 01:12:27.466862 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/update_probe_json.py
+-rw-r--r--   0        0        0     2430 2023-03-21 01:12:27.390341 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/upload_D1_to_incoming.py
+-rw-r--r--   0        0        0     8217 2023-03-21 01:12:27.611911 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/upload_opt_to_lims.py
+-rw-r--r--   0        0        0    33585 2023-03-21 01:14:23.990065 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/validate_local_d2_files.py
+-rw-r--r--   0        0        0    11132 2023-03-21 01:12:27.881307 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/validate_local_d2_files_ccb.py
+-rw-r--r--   0        0        0     9536 2023-03-21 01:14:23.582115 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/validate_metadata_tables_VBN_release.py
+-rw-r--r--   0        0        0     4266 2023-03-21 01:12:27.608910 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/vbn_stim_timing_test.py
+-rw-r--r--   0        0        0     4792 2023-03-28 18:33:09.567280 np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/vbn_stim_timing_test_SDK.py
+-rw-r--r--   0        0        0       70 2023-03-24 22:40:01.121024 np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/__init__.py
+-rw-r--r--   0        0        0      667 2023-03-21 18:27:15.617982 np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/assets/html_templates.py
+-rw-r--r--   0        0        0      928 2022-12-15 21:34:04.058641 np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/assets/single_page_img_json_report.css
+-rw-r--r--   0        0        0     6312 2023-03-24 22:40:01.359023 np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/qc2html.py
+-rw-r--r--   0        0        0       15 2023-03-27 23:09:19.768234 np-pipeline-qc-0.0.4/src/np_pipeline_qc/sorted/__init__.py
+-rw-r--r--   0        0        0    13176 2023-04-03 20:33:29.822069 np-pipeline-qc-0.0.4/src/np_pipeline_qc/sorted/spike_depths.py
+-rw-r--r--   0        0        0       20 2023-03-27 23:50:38.700137 np-pipeline-qc-0.0.4/src/np_pipeline_qc/utils/__init__.py
+-rw-r--r--   0        0        0     4547 2023-03-27 23:51:59.489831 np-pipeline-qc-0.0.4/src/np_pipeline_qc/utils/utils.py
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 np-pipeline-qc-0.0.4/PKG-INFO
```

### Comparing `np-pipeline-qc-0.0.3/pyproject.toml` & `np-pipeline-qc-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [project]
 name = "np_pipeline_qc"
-version = "0.0.3"
+version = "0.0.4"
 description = "Analysis and visualization code for quality-control of Neuropixels pipeline data."
 authors = [
     { name = "corbennett", email = "corbettb@alleninstitute.org" },
 ]
 maintainers = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
+    "setuptools",
+    "cmake>=3.26.3",
     "np-session>=0.4.26",
     "np-vba>=0.13.1",
 ]
 requires-python = ">=3.8, <3.11"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -20,32 +22,34 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
 ]
 
 [project.optional-dependencies]
+html = [
+    "beautifulsoup4",
+    "pywin32",
+]
 dev = [
+    "np_pipeline_qc[html]",
     "isort",
     "mypy",
     "pytest",
     "pytest-cov",
     "blue>=0.9.1",
     "coverage[toml]>=7.2.2",
     "pdm>=2.4.9",
     "bump>=1.3.2",
     "types-backports>=0.1.3",
     "ruff>=0.0.260",
 ]
-html = [
-    "beautifulsoup4",
-    "pywin32",
-]
 
 [tool.pdm.resolution.overrides]
+matplotlib = "<3.4.3, >=1.4.3"
 async-timeout = ">=4.0.0"
 
 [tool.pdm.scripts]
 ruff = "ruff --fix src"
 blue = "blue src"
 pytest = "pytest --cov"
 bump = "bump -p pyproject.toml"
```

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/__main__.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/classes.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/classes.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/align_physiology_plots.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/align_physiology_plots.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/analysis.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/analysis.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/analyze_nwb.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/analyze_nwb.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_copy_d2_lims_files.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_copy_d2_lims_files.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_hab_qc.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_hab_qc.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_lims_validation.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_lims_validation.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_qc.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_qc.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_rf.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_rf.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/batch_variability_qc.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/batch_variability_qc.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/behavior_analysis.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/behavior_analysis.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/build_stim_tables.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/build_stim_tables.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/channel_visual_modulation.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/channel_visual_modulation.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/check_datacube.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/check_datacube.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/copy_d2_lims_files_for_upload.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/copy_d2_lims_files_for_upload.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/D1_LIMS_schema.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/D1_LIMS_schema.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/D1_local_schema.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/D1_local_schema.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/d2_upload_tool.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/d2_upload_tool.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/data_getters.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/ebs_analysis.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/ebs_analysis.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/ebs_object_analysis.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/ebs_object_analysis.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/ecephys.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/ecephys.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/EcephysBehaviorSession.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/EcephysBehaviorSession.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/get_probe_info.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/get_probe_info.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/get_RFs_standalone.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/get_RFs_standalone.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/get_sessions.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/get_sessions.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/lims_validation.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/lims_validation.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/local_data_validation.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/local_data_validation.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/nwb_validation_optotagging.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/nwb_validation_optotagging.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/probe_alignment_data_io.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/probe_alignment_data_io.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/probe_track_day_assignment.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/probe_track_day_assignment.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/probeSync_qc.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/probeSync_qc.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/qc_cmd_caller.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/qc_cmd_caller.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/query_lims.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/query_lims.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/reformat_probe_annotation_files.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/reformat_probe_annotation_files.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/run_qc_callable.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/run_qc_callable.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/run_qc_class.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/run_qc_class.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/run_qc_modular.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/run_qc_modular.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/save_ecephysbehavior_session.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/save_ecephysbehavior_session.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/sync_dataset.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/sync_dataset.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/task1_behavior_session.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/task1_behavior_session.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/update_probe_json.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/update_probe_json.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/upload_D1_to_incoming.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/upload_D1_to_incoming.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/upload_opt_to_lims.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/upload_opt_to_lims.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/validate_local_d2_files.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/validate_local_d2_files.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/validate_local_d2_files_ccb.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/validate_local_d2_files_ccb.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/validate_metadata_tables_VBN_release.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/validate_metadata_tables_VBN_release.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/vbn_stim_timing_test.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/vbn_stim_timing_test.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/legacy/vbn_stim_timing_test_SDK.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/legacy/vbn_stim_timing_test_SDK.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/assets/html_templates.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/assets/html_templates.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/assets/single_page_img_json_report.css` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/assets/single_page_img_json_report.css`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/reports/qc2html.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/reports/qc2html.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/sorted/spike_depths.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/sorted/spike_depths.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/src/np_pipeline_qc/utils/utils.py` & `np-pipeline-qc-0.0.4/src/np_pipeline_qc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `np-pipeline-qc-0.0.3/PKG-INFO` & `np-pipeline-qc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np_pipeline_qc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Analysis and visualization code for quality-control of Neuropixels pipeline data.
 Author-email: corbennett <corbettb@alleninstitute.org>
 Maintainer-email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.8, <3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
```

