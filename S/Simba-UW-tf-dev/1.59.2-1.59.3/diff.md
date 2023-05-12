# Comparing `tmp/Simba-UW-tf-dev-1.59.2.tar.gz` & `tmp/Simba-UW-tf-dev-1.59.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.2.tar", last modified: Tue May  9 21:10:46 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.3.tar", last modified: Fri May 12 17:13:05 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.59.2.tar` & `Simba-UW-tf-dev-1.59.3.tar`

### file list

```diff
@@ -1,496 +1,498 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-08 20:25:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9493 2023-05-07 18:06:51.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.59.2/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.2/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20792 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)    10045 2023-05-09 12:31:02.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7020 2023-05-09 20:47:56.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8522 2023-05-09 20:40:07.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6069 2023-05-09 14:09:16.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.2/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42325 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21264 2023-05-09 14:34:28.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13454 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23739 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16652 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.2/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41761 2023-05-09 20:29:25.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29735 2023-05-08 15:27:56.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18431 2023-05-09 17:53:31.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    25962 2023-05-09 13:55:01.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61037 2023-05-08 16:28:07.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    56361 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7630 2023-05-08 15:03:37.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12196 2023-05-08 14:58:46.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1720 2023-05-08 15:05:19.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15320 2023-05-08 15:06:46.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12645 2023-05-08 15:03:37.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.59.2/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.2/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5837 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    34300 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2335 2023-05-07 19:58:55.000000 Simba-UW-tf-dev-1.59.2/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.2/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.59.2/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8378 2023-05-09 12:23:43.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    15294 2023-05-07 18:00:44.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12769 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5217 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11290 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9514 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13262 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9046 2023-05-09 14:13:06.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9801 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16351 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6468 2023-05-07 17:57:11.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11814 2023-05-07 17:03:08.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12854 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4817 2023-05-05 01:13:02.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2945 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9616 2023-05-08 15:27:56.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7596 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19309 2023-05-08 19:28:39.000000 Simba-UW-tf-dev-1.59.2/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.59.2/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.59.2/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3256 2023-05-08 19:18:20.000000 Simba-UW-tf-dev-1.59.2/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19774 2023-05-09 14:43:23.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8029 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11066 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7374 2023-05-09 19:41:31.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    11817 2023-05-09 19:15:18.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6947 2023-05-09 20:29:25.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    42300 2023-05-08 18:44:41.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24710 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7343 2023-05-08 18:23:30.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11101 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2853 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.59.2/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.2/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18901 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.2/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.2/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.2/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-09 21:10:40.000000 Simba-UW-tf-dev-1.59.2/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-08 20:25:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9493 2023-05-07 18:06:51.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.59.3/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.59.3/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.3/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20792 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)    10045 2023-05-09 12:31:02.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7036 2023-05-11 18:18:55.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23576 2023-05-11 15:34:10.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8522 2023-05-10 01:30:19.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6069 2023-05-09 14:09:16.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11275 2023-05-10 01:31:30.000000 Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.3/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42325 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21312 2023-05-10 01:45:20.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13664 2023-05-10 14:48:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46271 2023-05-10 14:43:16.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23787 2023-05-10 01:48:07.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16700 2023-05-10 01:45:20.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.3/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42147 2023-05-10 02:11:17.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29762 2023-05-10 01:52:46.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18516 2023-05-10 02:13:29.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    25962 2023-05-09 13:55:01.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61203 2023-05-10 11:39:12.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    56361 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.3/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7675 2023-05-10 01:34:21.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12265 2023-05-10 01:34:21.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16782 2023-05-10 01:34:21.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1720 2023-05-08 15:05:19.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15347 2023-05-10 01:37:18.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12672 2023-05-10 01:37:18.000000 Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.59.3/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.3/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.3/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-10 19:45:32.000000 Simba-UW-tf-dev-1.59.3/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    34300 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2703 2023-05-12 17:13:03.000000 Simba-UW-tf-dev-1.59.3/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.3/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.59.3/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8378 2023-05-09 12:23:43.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    15294 2023-05-07 18:00:44.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12769 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5217 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7919 2023-05-11 20:33:52.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11289 2023-05-10 14:49:41.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9409 2023-05-10 14:54:58.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13262 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9046 2023-05-09 14:13:06.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9801 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16351 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6721 2023-05-10 01:37:18.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11848 2023-05-10 01:41:05.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12747 2023-05-10 01:39:08.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9692 2023-05-10 01:39:08.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4837 2023-05-10 01:43:03.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2947 2023-05-10 01:43:03.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9643 2023-05-10 01:41:05.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7596 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.3/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19309 2023-05-08 19:28:39.000000 Simba-UW-tf-dev-1.59.3/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.59.3/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.59.3/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3256 2023-05-08 19:18:20.000000 Simba-UW-tf-dev-1.59.3/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19774 2023-05-09 14:43:23.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8029 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11066 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7374 2023-05-09 19:41:31.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    11817 2023-05-09 19:15:18.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6947 2023-05-09 20:29:25.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.3/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    42300 2023-05-08 18:44:41.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24710 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7343 2023-05-08 18:23:30.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11101 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2804 2023-05-12 17:10:03.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-12 16:12:08.000000 Simba-UW-tf-dev-1.59.3/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.3/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.3/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.3/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.3/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19089 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-12 17:13:04.000000 Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.3/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.3/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.3/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-12 17:13:03.000000 Simba-UW-tf-dev-1.59.3/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-12 17:13:05.000000 Simba-UW-tf-dev-1.59.3/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.59.2/PKG-INFO` & `Simba-UW-tf-dev-1.59.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.2
+Version: 1.59.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.59.3/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.59.3/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.59.3/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.59.3/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.59.3/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,27 @@
 from simba.utils.errors import NotDirectoryError
 from simba.utils.data import detect_bouts, plug_holes_shortest_bout
 from simba.mixins.config_reader import ConfigReader
 
 class AggBoundaryStatisticsCalculator(ConfigReader):
 
     """
-    Class computing aggregate boundary statistics
+    Compute aggregate boundary statistics
 
     Parameters
     ----------
-    config_path: str
-        Path to SimBA project config file in Configparser format
+    config_path: str Path to SimBA project config file in Configparser format
     measures: list
-        Aggregate statistics measurements. OPTIONS: 'INTERACTION TIME (s)', 'INTERACTION BOUT COUNT', 'INTERACTION BOUT MEAN (s)', 'INTERACTION BOUT MEDIAN (s)'
+        Aggregate statistics measurements. OPTIONS: 'DETAILED INTERACTIONS TABLE', 'INTERACTION TIME (s)', 'INTERACTION BOUT COUNT', 'INTERACTION BOUT MEAN (s)', 'INTERACTION BOUT MEDIAN (s)'
     shortest_allowed_interaction: int
         The shortest allowed animal-anchored ROI intersection in millisecond.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md__.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
 
     Examples
     ----------
     >>> boundary_stats_calculator = AggBoundaryStatisticsCalculator('MyProjectConfig', measures=['INTERACTION TIME (s)'], shortest_allowed_interaction=200)
     >>> boundary_stats_calculator.run()
     >>> boundary_stats_calculator.save()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_menus.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,24 @@
 from simba.utils.read_write import get_fn_ext, find_all_videos_in_project
 from simba.utils.checks import check_int
 from simba.utils.enums import Formats
 from simba.utils.lookups import get_named_colors
 
 class BoundaryMenus(ConfigReader, PopUpMixin):
     """
-    Class creating GUI interface for extrapolating bounding boxes from pose-estimation data, and calculating
-    statstics on bounding boxes and pose-estmated key-point intersections.
+    Launch GUI interface for extrapolating bounding boxes from pose-estimation data, and calculating
+    statstics on bounding boxes and pose-estimated key-point intersections.
 
     Parameters
     ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    config_path: str path to SimBA project config file in Configparser format
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md__.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>`_.
 
     Examples
     ----------
     >>> _ = BoundaryMenus(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini')
     """
 
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/boundary_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     roi_keypoint_intersections: bool
         If True, calculates intersection of animal-anchored ROIs and pose-estimated animal key-points.
     save_format: str
         Output data format. OPTIONS: CSV, PARQUET, PICKLE.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md_>`.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>_`.
 
     Examples
     ----------
     >>> boundary_stats_calculator = BoundaryStatisticsCalculator(config_path='MyConfigFile',roi_intersections=True, roi_keypoint_intersections=True, save_format='CSV')
     >>> boundary_stats_calculator.save_results()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.59.3/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import pickle
 import functools
 import cv2
 import multiprocessing
 from multiprocessing import pool
 import platform
 import os
+from typing import Union
+
 
 from simba.utils.errors import NoFilesFoundError
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.read_write import (read_df,
                                     get_fn_ext,
                                     get_video_meta_data,
@@ -74,24 +76,24 @@
     greyscale: bool
         If True, converts the video (but not the shapes/keypoints) to greyscale.
     show_intersections: bool or None
         If True, then produce highlight boundaries/keypoints to signify present intersections.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md__.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md>_`.
 
     Examples
     ----------
     >>> boundary_visualizer = BoundaryVisualizer(config_path='MySimBAConfig', video_name='MyVideoName', include_key_points=True, greyscale=True)
     >>> boundary_visualizer.run_visualization()
     """
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  video_name: str,
                  include_key_points: bool,
                  greyscale: bool,
                  show_intersections: bool or None,
                  roi_attributes: dict or None):
 
         ConfigReader.__init__(self, config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
 from collections import defaultdict
 import scipy
+from typing import Union
+
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.feature_extractors.perimeter_jit import jitted_hull
 
 class ExtractFeaturesFrom7bps(ConfigReader, FeatureExtractionMixin):
@@ -34,15 +36,15 @@
     ----------
     >>> feature_extractor = ExtractFeaturesFrom7bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
 
     """
      
     def __init__(self,
-                 config_path: str):
+                 config_path: Union[str, os.PathLike]):
 
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         self.in_headers = self.get_feature_extraction_headers(pose='1 animal 7 body-parts')
         self.mouse_p_headers = [x for x in self.in_headers if x[-2:] == '_p']
         self.mouse_headers = [x for x in self.in_headers if x[-2:] != '_p']
         print('Extracting features from {} file(s)...'.format(str(len(self.files_found))))
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_subsets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 import numpy as np
+from typing import Union
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 from itertools import combinations
 from simba.feature_extractors.perimeter_jit import jitted_hull
@@ -16,29 +17,38 @@
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
 
 class FeatureSubsetsCalculator(ConfigReader, FeatureExtractionMixin):
     def __init__(self,
-                 config_path: str,
-                 save_dir: str,
+                 config_path: Union[str, os.PathLike],
+                 save_dir: Union[str, os.PathLike],
                  feature_family: Literal[Options.FEATURE_SUBSET_OPTIONS]):
 
         """
         Computes frame-wise user-defined family subset of features from pose for non-ML downstream purposes.
         E.g., returns the size of animal convex hull in each frame.
 
-        :param config_path: path to SimBA configparser.ConfigParser project_config.ini
-        :param save_dir: directory where to save the results.
-        :param feature_family: feature family: E.g., Two-point body-part distances (mm).
-
-        :example:
-        >>> calculator = FeatureSubsetsCalculator(config_path='project_folder/project_config.ini', feature_family='Frame-by-frame body-parts inside ROIs (Boolean)', save_dir='data')
-        >>> calculator.run()
+        Parameters
+        ----------
+        config_path: str
+            path to SimBA project config file in Configparser format
+        save_dir: str
+            directory where to store results.
+        feature_family: str
+            Feature subtype to calculate
+
+        Notes
+        ----------
+        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/feature_subsets.md>_`
+
+        Examples
+        ----------
+        >>> _ = FeatureSubsetsCalculator(config_path='project_folder/project_config.ini', feature_family='Frame-by-frame body-parts inside ROIs (Boolean)', save_dir='data').run()
         """
 
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         check_if_filepath_list_is_empty(
             filepaths=self.outlier_corrected_paths,
             error_msg=f"SIMBA ERROR: Zero data files found in {self.outlier_corrected_paths} directory",
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
 class ExtractFeaturesFrom16bps(ConfigReader, FeatureExtractionMixin):
     """
     Class for creating a hard-coded set of features from two animals with 8 tracked body-parts
     each using pose-estimation. Results are stored in the `project_folder/csv/features_extracted`
     directory of the SimBA project
+
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
 
     Notes
     ----------
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import os
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 import math
 from collections import defaultdict
+from typing import Union
+
 from simba.utils.enums import Formats
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
@@ -31,15 +33,15 @@
     Examples
     ----------
     >>> feature_extractor = ExtractFeaturesFrom8bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
     """
 
     def __init__(self,
-                 config_path=None):
+                 config_path: Union[str, os.PathLike]):
 
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         self.in_headers = self.get_feature_extraction_headers(pose='1 animal 8 body-parts')
         self.mouse_p_headers = [x for x in self.in_headers if x[-2:] == '_p']
         self.mouse_headers = [x for x in self.in_headers if x[-2:] != '_p']
         print('Extracting features from {} file(s)...'.format(str(len(self.files_found))))
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from collections import defaultdict
 import scipy
+from typing import Union
+
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 
 class ExtractFeaturesFrom4bps(ConfigReader, FeatureExtractionMixin):
     """
@@ -31,15 +33,15 @@
     ----------
     >>> feature_extractor = ExtractFeaturesFrom4bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
 
     """
     
     def __init__(self,
-                 config_path: str):
+                 config_path: Union[str, os.PathLike]):
 
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         self.in_headers = self.get_feature_extraction_headers(pose='1 animal 4 body-parts')
         self.mouse_p_headers = [x for x in self.in_headers if x[-2:] == '_p']
         self.mouse_headers = [x for x in self.in_headers if x[-2:] != '_p']
         print('Extracting features from {} file(s)...'.format(str(len(self.files_found))))
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.3/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/requirements.txt` & `Simba-UW-tf-dev-1.59.3/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/pop_up_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from tkinter import *
 from PIL import ImageTk
 import PIL.Image
 from tkinter import messagebox
 import os
 from simba.pose_importers import trk_importer
-from typing import Tuple, Optional, List
+from typing import Tuple, Optional, List, Dict
 
 
 from simba.utils.checks import (check_int,
                                 check_str,
                                 check_float,
                                 check_if_dir_exists)
 from simba.pose_importers.read_DANNCE_mat import import_DANNCE_file, import_DANNCE_folder
@@ -68,24 +68,30 @@
         self.menu_icons = get_icons_paths()
         for k in self.menu_icons.keys():
             self.menu_icons[k]['img'] = ImageTk.PhotoImage(image=PIL.Image.open(os.path.join(os.path.dirname(__file__), self.menu_icons[k]['icon_path'])))
         if config_path:
             print(config_path)
             ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
 
-    def create_clf_checkboxes(self, main_frm: Frame, clfs: list):
+    def create_clf_checkboxes(self,
+                              main_frm: Frame,
+                              clfs: List[str]):
         self.choose_clf_frm = LabelFrame(self.main_frm, text='SELECT CLASSIFIER ANNOTATIONS', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.clf_selections = {}
         for clf_cnt, clf in enumerate(clfs):
             self.clf_selections[clf] = BooleanVar(value=False)
             self.calculate_distance_moved_cb = Checkbutton(self.choose_clf_frm, text=clf, variable=self.clf_selections[clf])
             self.calculate_distance_moved_cb.grid(row=clf_cnt, column=0, sticky=NW)
         self.choose_clf_frm.grid(row=self.children_cnt_main(), column=0, sticky=NW)
 
-    def create_cb_frame(self, main_frm: Frame, cb_titles: list, frm_title: str) -> dict:
+    def create_cb_frame(self,
+                        main_frm: Frame,
+                        cb_titles: List[str],
+                        frm_title: str) -> Dict[str, BooleanVar]:
+
         cb_frm = LabelFrame(main_frm, text=frm_title, font=Formats.LABELFRAME_HEADER_FORMAT.value)
         cb_dict = {}
         for cnt, title in enumerate(cb_titles):
             cb_dict[title] = BooleanVar(value=False)
             cb = Checkbutton(cb_frm, text=title, variable=cb_dict[title])
             cb.grid(row=cnt, column=0, sticky=NW)
         cb_frm.grid(row=self.children_cnt_main(), column=0, sticky=NW)
@@ -140,33 +146,39 @@
         if hasattr(self, 'time_bin_frm'):
             self.time_bin_frm.destroy()
         self.time_bin_frm = LabelFrame(self.main_frm, text="TIME BIN", font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.time_bin_entrybox = Entry_Box(self.time_bin_frm, 'Time-bin size (s): ', '12', validation='numeric')
         self.time_bin_entrybox.grid(row=0, column=0, sticky=NW)
         self.time_bin_frm.grid(row=self.children_cnt_main(), column=0, sticky=NW)
 
-    def create_run_frm(self, run_function: object, title: str='RUN'):
+    def create_run_frm(self,
+                       run_function: object,
+                       title: str = 'RUN'):
         if hasattr(self, 'run_frm'):
             self.run_frm.destroy()
             self.run_btn.destroy()
         self.run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.run_btn = Button(self.run_frm, text=title, fg='blue', command=lambda: run_function())
         self.run_frm.grid(row=self.children_cnt_main()+1, column=0, sticky=NW)
         self.run_btn.grid(row=0, column=0, sticky=NW)
 
-    def create_choose_number_of_body_parts_frm(self, project_body_parts: list, run_function: object):
+    def create_choose_number_of_body_parts_frm(self,
+                                               project_body_parts: List[str],
+                                               run_function: object):
         self.bp_cnt_frm = LabelFrame(self.main_frm, text='SELECT NUMBER OF BODY-PARTS',  font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.bp_cnt_dropdown = DropDownMenu(self.bp_cnt_frm, '# of body-parts', list(range(1, len(project_body_parts))), '12')
         self.bp_cnt_dropdown.setChoices(1)
         self.bp_cnt_confirm_btn = Button(self.bp_cnt_frm, text="Confirm", command=lambda: self.create_choose_bp_frm(project_body_parts, run_function))
         self.bp_cnt_frm.grid(row=0, sticky=NW)
         self.bp_cnt_dropdown.grid(row=0, column=0, sticky=NW)
         self.bp_cnt_confirm_btn.grid(row=0, column=1, sticky=NW)
 
-    def add_to_listbox_from_entrybox(self, list_box: Listbox, entry_box: Entry_Box):
+    def add_to_listbox_from_entrybox(self,
+                                     list_box: Listbox,
+                                     entry_box: Entry_Box):
         value = entry_box.entry_get
         check_float(name='VALUE', value=value)
         list_box_content = [float(x) for x in list_box.get(0, END)]
         if float(value) not in list_box_content:
             list_box.insert(0, value)
 
     def add_value_to_listbox(self,
@@ -208,15 +220,14 @@
         self.body_part_frm.grid(row=self.frame_children(frame=parent), sticky=NW)
         for bp_cnt in range(int(self.animal_cnt_dropdown.getChoices())):
             self.body_parts_dropdowns[bp_cnt] = DropDownMenu(self.body_part_frm, f'Body-part {str(bp_cnt + 1)}:', bp_options, '20')
             self.body_parts_dropdowns[bp_cnt].grid(row=bp_cnt, column=0, sticky=NW)
             self.body_parts_dropdowns[bp_cnt].setChoices(bp_options[bp_cnt])
 
 
-
     def children_cnt_main(self) -> int:
         return int(len(list(self.main_frm.children.keys())))
 
     def frame_children(self, frame: Frame) -> int:
         return int(len(list(frame.children.keys())))
 
     def update_config(self) -> None:
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/config_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class ConfigReader(object):
     def __init__(self,
                  config_path: str,
                  read_video_info: bool = True):
 
         """
-        Methods for reading SimBA configparser.Configparser project config..
+        Methods for reading SimBA configparser.Configparser project config and associated project data.
 
         :param configparser.Configparser config_path: path to SimBA project_config.ini
         :param bool read_video_info: if true, read the project_folder/logs/video_info.csv file.
         """
 
         self.timer = SimbaTimer(start=True)
         self.config_path = config_path
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/pose_importer_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 from numba import jit, prange
 import numpy as np
 from copy import deepcopy
 from collections import defaultdict
 import itertools
 import scipy.io as sio
 import h5py
-
+from typing import List, Union, Optional
 
 import pandas as pd
-
 from simba.utils.errors import NoDataError, NoFilesFoundError, IntegerError, InvalidInputError, CountError
 from simba.utils.read_write import get_fn_ext
 from simba.utils.enums import ConfigKey
 
 class PoseImporterMixin(object):
     def __init__(self):
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
@@ -39,33 +38,33 @@
         space_scale, radius_scale, resolution_scale, font_scale = 40, 10, 1500, 1.2
         max_video_dimension = max(video_info['width'], video_info['height'])
         self.scalers['circle'] = int(radius_scale / (resolution_scale / max_video_dimension))
         self.scalers['font'] = font_scale / (resolution_scale / max_video_dimension)
         self.scalers['space'] = int(space_scale / (resolution_scale / max_video_dimension))
 
     def find_data_files(self,
-                        dir: str,
-                        extensions: list):
+                        dir: Union[str, os.PathLike],
+                        extensions: List[str]):
 
         data_paths = []
         paths = [f for f in next(os.walk(dir))[2] if not f[0] == '.']
         paths = [os.path.join(dir, f) for f in paths]
         for extension in extensions:
             for path in paths:
                 if path.endswith(extension):
                     data_paths.append(path)
         if len(data_paths) == 0:
             raise NoDataError(msg=f'No files with {extensions} extensions found in {dir}.')
 
         return data_paths
 
     def link_video_paths_to_data_paths(self,
-                                       data_paths: list,
-                                       video_paths: list,
-                                       str_splits: list or None=None):
+                                       data_paths: List[str],
+                                       video_paths: List[str],
+                                       str_splits: Optional[List[str]] = None):
         results, video_names = {}, []
         for video_path in video_paths:
             _, video_file_name, _ = get_fn_ext(video_path)
             video_names.append(video_file_name.lower())
         for data_path in data_paths:
             _, data_file_name, _ = get_fn_ext(data_path)
             data_file_names = [data_file_name.lower()]
@@ -84,15 +83,15 @@
     def get_x_y_loc_of_mouse_click(self, event, x, y, flags, param):
         if event == 7:
             self.click_loc = (x,y)
             self.id_cords[self.animal_cnt] = {}
             self.id_cords[self.animal_cnt]['cord'] = self.click_loc
             self.id_cords[self.animal_cnt]['name'] = self.animal_name
 
-    def insert_all_bodyparts_into_img(self, img: np.array, body_parts: dict):
+    def insert_all_bodyparts_into_img(self, img: np.ndarray, body_parts: dict):
         for animal, bp_data in body_parts.items():
             for bp_cnt, bp_tuple in enumerate(bp_data):
                 try:
                     cv2.circle(img, bp_tuple, self.scalers['circle'], self.animal_bp_dict[animal]['colors'][bp_cnt], -1, lineType=cv2.LINE_AA)
                 except Exception as err:
                     if type(err) == OverflowError:
                         raise IntegerError(f'SimBA encountered a pose-estimated body-part located at pixel position {str(bp_tuple)}. '
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi` & `Simba-UW-tf-dev-1.59.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/plotting_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import matplotlib
 import shutil
 import random
 from matplotlib import cm
 import imutils
 import itertools
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, Dict, Any
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 import simba
 from simba.utils.lookups import get_color_dict, get_named_colors
@@ -90,15 +90,15 @@
         open_cv_image = np.uint8(open_cv_image)
         buffer_.close()
         plt.close(fig)
 
         return open_cv_image
 
     def create_single_color_lst(self,
-                                pallete_name: str,
+                                pallete_name: Literal[Options.PALETTE_OPTIONS],
                                 increments: int,
                                 as_rgb_ratio: bool = False,
                                 as_hex: bool = False) -> List[int]:
         """
         Helper to create a color palette of bgr colors in a list.
         Parameters
         ----------
@@ -147,19 +147,19 @@
                 data_arr[df_cnt]['group'] = df_cnt
         obs_per_split = len(data_arr[0])
 
         return data_arr, obs_per_split
 
     def make_distance_plot(self,
                            data: np.array,
-                           line_attr: dict,
-                           style_attr: dict,
+                           line_attr: Dict[int, str],
+                           style_attr: Dict[str, Any],
                            fps: int,
-                           save_path: str or None = None,
-                           save_img: bool = False) -> np.ndarray:
+                           save_img: bool = False,
+                           save_path: Optional[str] = None) -> np.ndarray:
         """
         Helper to make a single line plot .png image with N lines.
 
         Parameters
         ----------
         data: np.array
             Two-dimensional array where rows represent frames and columns represent values.
@@ -297,15 +297,15 @@
 
     def make_path_plot(self,
                        data_df: pd.DataFrame,
                        video_info: pd.DataFrame,
                        style_attr: dict,
                        deque_dict: dict,
                        clf_attr: dict,
-                       save_path: str or None) -> np.ndarray:
+                       save_path: Optional[str] = None) -> np.ndarray:
 
         video_timer = SimbaTimer(start=True)
         for frm_cnt in range(len(data_df)):
             for animal_cnt, (animal_name, animal_data) in enumerate(deque_dict.items()):
                 bp_x = int(data_df.loc[frm_cnt, '{}_{}'.format(animal_data['bp'], 'x')])
                 bp_y = int(data_df.loc[frm_cnt, '{}_{}'.format(animal_data['bp'], 'y')])
                 deque_dict[animal_name]['deque'].appendleft((bp_x, bp_y))
@@ -987,18 +987,18 @@
     @staticmethod
     def validation_video_mp(data: pd.DataFrame,
                             bp_dict: dict,
                             video_save_dir: str,
                             settings: dict,
                             video_path: str,
                             video_meta_data: dict,
-                            gantt_setting: str or None,
-                            final_gantt: np.array or None,
-                            clf_data: np.array,
-                            clrs: list,
+                            gantt_setting: Optional[Literal['Gantt chart: final frame only (slightly faster)', 'Gantt chart: video']],
+                            final_gantt: Optional[np.ndarray],
+                            clf_data: np.ndarray,
+                            clrs: List[List],
                             clf_name: str,
                             bouts_df: pd.DataFrame):
 
         dpi = plt.rcParams['figure.dpi']
 
         def create_gantt(bouts_df: pd.DataFrame,
                          clf_name: str,
@@ -1087,16 +1087,16 @@
 
         return group
 
     @staticmethod
     def bbox_mp(frm_range: list,
                 polygon_data: dict,
                 animal_bp_dict: dict,
-                data_df: pd.DataFrame or None,
-                intersection_data_df: pd.DataFrame or None,
+                data_df: Optional[pd.DataFrame],
+                intersection_data_df: Optional[pd.DataFrame],
                 roi_attributes: dict,
                 video_path: str,
                 key_points: bool,
                 greyscale: bool):
 
         cap, current_frame = cv2.VideoCapture(video_path), frm_range[0]
         cap.set(1, frm_range[0])
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.59.3/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os, glob
 from typing import List
+from typing import Union
 
 
 from simba.utils.read_write import read_df, get_fn_ext, read_config_entry
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_that_column_exist
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.utils.errors import NoFilesFoundError
@@ -41,15 +42,15 @@
     >>> cue_light_clf_analyzer = CueLightClfAnalyzer(config_path='MyProjectConfig', pre_window=1000, post_window=1000, cue_light_names=['Cue_light'], clf_list=['Attack'])
     >>> cue_light_clf_analyzer.analyze_clf()
     >>> cue_light_clf_analyzer.organize_results()
     >>> cue_light_clf_analyzer.save_data()
     """
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  pre_window: int,
                  post_window: int,
                  cue_light_names: List[str],
                  clf_list: List[str]):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.pre_window, self.post_window = pre_window, post_window
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 import pandas as pd
 import cv2
 import numpy as np
 import multiprocessing
 import functools
 import time
 import platform
+from typing import List, Union
+
 from simba.utils.read_write import read_df, write_df, get_fn_ext, find_video_of_file, get_video_meta_data, find_core_cnt
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.errors import NoFilesFoundError, CountError, NoROIDataError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.warnings import NoDataFoundWarning
 
 
-def get_intensity_scores_in_rois(frm_list: list=None,
-                                 video_path: str = None,
-                                 rectangles_df: pd.DataFrame = None,
-                                 polygon_df: pd.DataFrame = None,
-                                 circles_df: pd.DataFrame = None):
+def get_intensity_scores_in_rois(frm_list: List[int],
+                                 video_path: Union[str, os.PathLike],
+                                 rectangles_df: pd.DataFrame,
+                                 polygon_df: pd.DataFrame,
+                                 circles_df: pd.DataFrame):
 
     cap = cv2.VideoCapture(video_path)
     start, end = frm_list[0], frm_list[-1]
     cap.set(1, start)
     frm_cnt = start
     results_dict = {}
     while frm_cnt <= end:
@@ -79,17 +81,17 @@
     Examples
     ----------
     >>> cue_light_analyzer = CueLightAnalyzer(config_path='MyProjectConfig', in_dir='project_folder/csv/outlier_corrected_movement_location', cue_light_names=['Cue_light'])
     >>> cue_light_analyzer.analyze_files()
     """
 
     def __init__(self,
-                 config_path: str,
-                 in_dir: str,
-                 cue_light_names: list):
+                 config_path: Union[str, os.PathLike],
+                 in_dir: Union[str, os.PathLike],
+                 cue_light_names: List[str]):
 
 
         ConfigReader.__init__(self, config_path=config_path)
 
         if len(cue_light_names) == 0:
             raise CountError(msg='SIMBA ERROR: Please select one or more cue lights')
         if platform.system() == "Darwin":
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_menues.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 from tkinter import *
 import glob, os
 import itertools
 import pandas as pd
+from typing import Union
 
 from simba.utils.checks import check_float, check_int
 from simba.utils.read_write import get_fn_ext, find_video_of_file, get_all_clf_names, read_config_entry
 from simba.cue_light_tools.cue_light_analyzer import CueLightAnalyzer
 from simba.cue_light_tools.cue_light_visualizer import CueLightVisualizer
 from simba.cue_light_tools.cue_light_clf_statistics import CueLightClfAnalyzer
 from simba.cue_light_tools.cue_light_movement_statistics import CueLightMovementAnalyzer
@@ -38,15 +39,15 @@
     >>> cue_light_gui = CueLightAnalyzerMenu(config_path='MySimBAConfigPath')
     >>> cue_light_gui.cue_light_main_frame.mainloop()
     """
 
 
 
     def __init__(self,
-                 config_path: str):
+                 config_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.data_dir = os.path.join(self.project_path, 'csv', 'outlier_corrected_movement_location')
         self.cue_light_data_folder = os.path.join(self.project_path, 'csv', 'cue_lights')
         self.read_roi_data()
         if len(self.shape_names) == 0:
             raise CountError(msg='SIMBA ERROR: Cue light analysis require ROI definitions. Please define ROIs before doing cue light analysis')
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import itertools, os
 import pandas as pd
 import cv2
-from typing import List
+from typing import List, Union
 
 
 from simba.utils.errors import NoSpecifiedOutputError, NoROIDataError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, get_fn_ext, get_video_meta_data
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_file_exist_and_readable
@@ -38,15 +38,15 @@
     Examples
     ----------
     >>> cue_light_visualizer = CueLightVisualizer(config_path='SimBAConfig', cue_light_names=['Cue_light'], video_path='VideoPath', video_setting=True, frame_setting=False)
     >>> cue_light_visualizer.visualize_cue_light_data()
     """
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  cue_light_names: List[str],
                  video_path: str,
                  frame_setting: bool,
                  video_setting: bool):
 
         ConfigReader.__init__(self, config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.59.3/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 from collections import defaultdict
 import pandas as pd
 import numpy as np
 from statistics import mean
-from typing import List
+from typing import List, Union
 
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.printing import stdout_success
 
@@ -47,15 +47,15 @@
     >>> cue_light_movement_analyzer = CueLightMovementAnalyzer(config_path='MyProjectConfig', cue_light_names=['Cue_light'], pre_window=1000, post_window=1000, threshold=0.0, roi_setting=True)
     >>> cue_light_movement_analyzer.calculate_whole_session_movement()
     >>> cue_light_movement_analyzer.organize_results()
     >>> cue_light_movement_analyzer.save_results()
     """
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  pre_window: int,
                  post_window: int,
                  cue_light_names: List[str],
                  threshold: float,
                  roi_setting: bool):
 
         ConfigReader.__init__(self, config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/enums.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/checks.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         pass
 
 
 def check_int(name: str,
               value: Any,
               max_value: Optional[int] = None,
               min_value: Optional[int] = None,
-              raise_error: bool=True) -> (bool, str):
+              raise_error: bool = True) -> (bool, str):
 
     msg = ''
     try:
         t.Int().check(value)
     except t.DataError as e:
         msg=f'{name} should be an integer number in SimBA, but is set to {str(value)}'
         if raise_error:
@@ -55,15 +55,15 @@
             else:
                 return False, msg
     return True, msg
 
 
 def check_str(name: str,
               value: Any,
-              options: Tuple[str, ...] = (),
+              options: Tuple[Any] = (),
               allow_blank: bool = False,
               raise_error: bool = True) -> (bool, str):
     msg = ''
     try:
         t.String(allow_blank=allow_blank).check(value)
     except t.DataError as e:
         msg = f'{name} should be an string in SimBA, but is set to {str(value)}'
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/cli/cli_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os, glob
 
+import pandas as pd
+
 from simba.utils.enums import ConfigKey, Dtypes, Paths
 from simba.utils.read_write import read_config_file, read_config_entry, read_project_path_and_file_type, read_video_info_csv, get_fn_ext
 from simba.utils.lookups import get_bp_config_code_class_pairs
 from simba.utils.printing import SimbaTimer, stdout_success
 
 def feature_extraction_runner(config_path: str):
     config = read_config_file(config_path=config_path)
@@ -21,22 +23,26 @@
 def set_video_parameters(config_path: str,
                          px_per_mm: float,
                          fps: float,
                          resolution: tuple):
     timer = SimbaTimer(start=True)
     config = read_config_file(config_path=config_path)
     project_path, file_type = read_project_path_and_file_type(config=config)
+    video_info_path = os.path.join(project_path, Paths.VIDEO_INFO.value)
+    if not os.path.isfile(video_info_path):
+        df = pd.DataFrame(columns=['Video', 'fps', 'Resolution_width', 'Resolution_height', 'Distance_in_mm', 'pixels/mm']).set_index('Video')
+        df.to_csv(video_info_path)
     video_info = read_video_info_csv(os.path.join(project_path, Paths.VIDEO_INFO.value))
     data_paths = glob.glob(os.path.join(project_path, Paths.OUTLIER_CORRECTED.value) + '/*.' + file_type)
     for file_path in data_paths:
         _, video_name, _ = get_fn_ext(file_path)
         if video_name not in list(video_info['Video']):
-            video_info.loc[len(video_info)] = [video_name, fps, 1, resolution[0], resolution[1], 0, px_per_mm]
-    video_info.reset_index(drop=True).to_csv(os.path.join(project_path, Paths.VIDEO_INFO.value))
+            video_info.loc[len(video_info)] = [video_name, fps, resolution[0], resolution[1], 0, px_per_mm]
+    video_info.reset_index(drop=True).set_index('Video').to_csv(os.path.join(project_path, Paths.VIDEO_INFO.value))
     timer.stop_timer()
     stdout_success(msg='Video parameters set', elapsed_time=timer.elapsed_time_str)
 
-# set_video_parameters(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini', px_per_mm=5.6)
+#set_video_parameters(config_path='/Users/simon/Desktop/envs/troubleshooting/notebook_example/project_folder/project_config.ini', px_per_mm=5.6, fps=25, resolution=(400, 400))
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/errors.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/data.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/utils/printing.py` & `Simba-UW-tf-dev-1.59.3/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,17 @@
     video_name: str
         Video to visualize directionality for (e.g., ``My_video.mp4``)
     style_attr: dict
         Video style attribitions.
     core_cnt: int
         How many cores to use to create the video.
 
-    Notes
-    -----
-    Requires the pose-estimation data for the ``left ear``, ``right ear`` and ``nose`` of
-    each individual animals. `YouTube example of expected output <https://youtu.be/4WXs3sKu41I>`__.
+    .. note::
+        Requires the pose-estimation data for the ``left ear``, ``right ear`` and ``nose`` of
+        each individual animals. `YouTube example of expected output <https://youtu.be/4WXs3sKu41I>`__.
 
     Examples
     -----
     >>> style_attr = {'Show_pose': True, 'Pose_circle_size': 3, "Direction_color": 'Random', 'Direction_thickness': 4, 'Highlight_endpoints': True}
     >>> directing_visualizer = DirectingOtherAnimalsVisualizerMultiprocess(config_path='project_folder/project_config.ini', video_name='Testing_Video_3.mp4', style_attr=style_attr)
     >>> directing_visualizer.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/clf_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     video_speed: float,
         FPS rate in relation to original video. E.g., the same as original video if 1.0.
     concat_video: bool
         If True, creates a single video including all events bouts for each video.
 
     Notes
     ----------
-    `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/classifier_validation.md#classifier-validation>`__.
+    `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/classifier_validation.md#classifier-validation>`_.
 
     Examples
     ----------
     >>> clf_validator = ClassifierValidationClips(config_path='MyProjectConfigPath', window=5, clf_name='Attack', text_clr=(255,255,0), clips=False, concat_video=True)
     >>> clf_validator.run()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/data_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,28 @@
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.lookups import get_color_dict
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext
 
 class DataPlotter(ConfigReader):
     """
-    Class for tabular data visualizations of animal movement and distances in the current frame and their aggregate
+    Tabular data visualization of animal movement and distances in the current frame and their aggregate
     statistics.
 
     Parameters
     ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    config_path: str path to SimBA project config file in Configparser format
 
     Notes
     ----------
-    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables`__.
+    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables`>_.
 
     Examples
     -----
-    >>> data_plotter = DataPlotter(config_path='MyConfigPath')
-    >>> data_plotter.process_movement()
-    >>> data_plotter.create_data_plots()
+    >>> _ = DataPlotter(config_path='MyConfigPath').run()
     """
 
     def __init__(self,
                  config_path: str,
                  style_attr: Dict,
                  body_part_attr: List[List[str]],
                  data_paths: List[str],
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.59.3/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.59.3/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.59.3/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.59.3/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/agg_clf_calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
-from typing import List
+from typing import List, Union
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
@@ -37,16 +37,16 @@
     -----
     >>> clf_log_creator = AggregateClfCalculator(config_path="MyConfigPath", data_measures=['Bout count', 'Total event duration'], classifiers=['Attack', 'Sniffing'])
     >>> clf_log_creator.run()
     >>> clf_log_creator.save()
     """
 
     def __init__(self,
-                 config_path: str,
-                 data_measures: List[str],
+                 config_path: Union[str, os.PathLike],
+                 data_measures: List[Literal['Bout count', 'Total event duration (s)', 'Mean event bout duration (s)', 'Median event bout duration (s)', 'First event occurrence (s)', 'Mean event bout interval duration (s)', 'Median event bout interval duration (s)']],
                  classifiers: List[str]):
 
         super().__init__(config_path=config_path)
         self.chosen_measures, self.classifiers = data_measures, classifiers
         self.file_save_name = os.path.join(self.project_path, 'logs', 'data_summary_' + str(self.datetime) + '.csv')
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg='SIMBA ERROR: No data files found in the project_folder/csv/machine_results directory. Run classifiers before analysing results.')
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolation_smoothing.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             print(f'Video {video_name} interpolated (elapsed time {video_timer.elapsed_time_str}) ...')
 
 class Smooth(ConfigReader):
     def __init__(self,
                  config_path: str,
                  input_path: str,
                  time_window: int,
-                 smoothing_method: str,
+                 smoothing_method: Literal['Gaussian', 'Savitzky-Golay'],
                  initial_import_multi_index: bool = False):
 
         super().__init__(config_path=config_path, read_video_info=False)
         if os.path.isdir(input_path):
             self.files_found = glob.glob(input_path + '/*' + self.file_type)
             self.input_dir = input_path
             check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f"SIMBA ERROR: {self.input_dir} does not contain any {self.file_type} files.")
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/fsttc_calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import os
 import pandas as pd
 import itertools
 import seaborn as sns
-from typing import List
+from typing import List, Union
 
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.errors import CountError
 from simba.mixins.config_reader import ConfigReader
@@ -32,37 +32,33 @@
 
     Notes
     -----
     `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/FSTTC.md>`__.
 
     Examples
     -----
-    >>> fsttc_calculator = FSTTCPerformer(config_path='MyConfigPath', time_window=2, behavior_lst=['Attack', 'Sniffing'], create_graphs=True)
-    >>> fsttc_calculator.find_sequences()
-    >>> fsttc_calculator.calculate_FSTTC()
-    >>> fsttc_calculator.save_FSTTC()
-    >>> fsttc_calculator.plot_FSTTC()
+    >>> fsttc_calculator = FSTTCCalculator(config_path='MyConfigPath', time_window=2, behavior_lst=['Attack', 'Sniffing'], create_graphs=True)
+    >>> fsttc_calculator.run()
 
     References
     ----------
     .. [1] Lee et al., Temporal microstructure of dyadic social behavior during relationship formation in mice, `PLOS One`,
            2019.
     .. [2] Cutts et al., Detecting Pairwise Correlations in Spike Trains: An Objective Comparison of Methods and
            Application to the Study of Retinal Waves, `J Neurosci`, 2014.
     """
 
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  time_window: int,
                  behavior_lst: List[str],
                  create_graphs: bool):
 
         super().__init__(config_path=config_path)
-
         self.time_delta = int(time_window)
         self.behavior_lst = behavior_lst
         if len(self.behavior_lst) < 2:
             raise CountError(msg='FSTCC requires at least two behaviors')
         self.graph_status = create_graphs
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg=f'Cannot calculate FSTTC, no data found in {self.machine_results_paths} directory')
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/directing_other_animals_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import itertools
 import numpy as np
 import os
+from typing import Union
 
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import AnimalNumberError
@@ -35,15 +36,15 @@
     >>> directing_analyzer.process_directionality()
     >>> directing_analyzer.create_directionality_dfs()
     >>> directing_analyzer.save_directionality_dfs()
     >>> directing_analyzer.summary_statistics()
     """
 
     def __init__(self,
-                 config_path: str):
+                 config_path: Union[str, os.PathLike]):
 
         super().__init__(config_path=config_path)
         if self.animal_cnt < 2:
             raise AnimalNumberError('Cannot analyze directionality between animals in a 1 animal project.')
         if not os.path.exists(self.directionality_df_dir): os.makedirs(self.directionality_df_dir)
         check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
                                         error_msg=f'SIMBA ERROR: No data found in the {self.outlier_corrected_dir} directory')
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/severity_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}
     >>> processor = SeverityProcessor(config_path='project_folder/project_config.ini', settings=settings)
     >>> processor.run()
     >>> processor.save()
     """
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  settings: Dict):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.settings = settings
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg=f'SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty')
         save_name = os.path.join(f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/pybursts_calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### CODE MODIFID FROM PYBURST PACKAGE  https://pypi.org/project/pybursts/
 import numpy as np
 import math
 
-def kleinberg_burst_detection(offsets: np.array,
+def kleinberg_burst_detection(offsets: np.ndarray,
                               s: float,
                               gamma: float):
 
     offsets = np.array(offsets, dtype=object)
 
     if offsets.size == 1:
         bursts = np.array([0, offsets[0], offsets[0]], ndmin=2, dtype=object)
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/kleinberg_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import numpy as np
 import shutil, os
 from copy import deepcopy
-from typing import List
+from typing import List, Union
 
 
 from simba.utils.checks import (check_that_column_exist,
                                 check_int,
                                 check_float,
                                 check_if_filepath_list_is_empty)
 from simba.utils.read_write import write_df, read_df, get_fn_ext
@@ -55,15 +55,15 @@
     .. [2] Lee et al., Temporal microstructure of dyadic social behavior during relationship formation in mice, `PLOS One`,
            2019.
     .. [3] Bordes et al., Automatically annotated motion tracking identifies a distinct social behavioral profile
            following chronic social defeat stress, `bioRxiv`, 2022.
     '''
 
     def __init__(self,
-                 config_path: str,
+                 config_path: Union[str, os.PathLike],
                  classifier_names: List[str],
                  sigma: int = 2,
                  gamma: float = 0.3,
                  hierarchy: int = 1,
                  hierarchical_search: bool = False):
 
         super().__init__(config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.59.3/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.59.3/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.59.3/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.59.3/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.59.3/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.59.3/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.59.3/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.59.3/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,36 +24,30 @@
     >>> outlier_correction_skipper = OutlierCorrectionSkipper(config_path='MyProjectConfig')
     >>> outlier_correction_skipper.run()
 
     """
 
     def __init__(self, config_path: str):
 
-        super().__init__(config_path=config_path)
-        if not os.path.exists(self.outlier_corrected_dir):
-            os.makedirs(self.outlier_corrected_dir)
-        check_if_filepath_list_is_empty(
-            filepaths=self.input_csv_paths,
-            error_msg=f"No files found in {self.input_csv_dir}.",
-        )
+        ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
+        if not os.path.exists(self.outlier_corrected_dir): os.makedirs(self.outlier_corrected_dir)
+        check_if_filepath_list_is_empty(filepaths=self.input_csv_paths, error_msg=f"No files found in {self.input_csv_dir}.", )
         print(f"Processing {len(self.input_csv_paths)} file(s)...")
 
     def run(self):
         """
         Standardizes pose-estimation data (i.e., headers) from different pose-estimation packages.
         Results are stored in the project_folder/csv/outlier_corrected_movement_location` directory of
         the SimBA project
         """
 
         for file_cnt, file_path in enumerate(self.input_csv_paths):
             video_timer = SimbaTimer(start=True)
             _, video_name, ext = get_fn_ext(file_path)
-            data_df = read_df(
-                file_path=file_path, file_type=self.file_type, check_multiindex=True
-            )
+            data_df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=True)
             if "scorer" in data_df.columns:
                 data_df = data_df.set_index("scorer")
             data_df = self.insert_column_headers_for_outlier_correction(
                 data_df=data_df, new_headers=self.bp_col_names, filepath=file_path
             )
             data_df.index.name = None
             save_path = os.path.join(
@@ -66,10 +60,9 @@
             )
         self.timer.stop_timer()
         stdout_success(
             msg=f"Skipped outlier correction for {len(self.input_csv_paths)} files",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
-
 # test = OutlierCorrectionSkipper(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.3/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/SimBA.py` & `Simba-UW-tf-dev-1.59.3/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.59.3/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.3/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.59.3/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.59.3/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.59.3/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.59.3/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.3/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.59.3/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.59.3/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.59.3/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.2
+Version: 1.59.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,16 @@
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
 simba/model/grid_search_rf.py
 simba/model/inference_batch.py
 simba/model/inference_validation.py
 simba/model/train_rf.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
```

### Comparing `Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.59.3/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/LICENSE.md` & `Simba-UW-tf-dev-1.59.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/README.md` & `Simba-UW-tf-dev-1.59.3/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.2/setup.py` & `Simba-UW-tf-dev-1.59.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.59.2",
+    version="1.59.3",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

