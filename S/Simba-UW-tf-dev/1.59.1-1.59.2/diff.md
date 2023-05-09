# Comparing `tmp/Simba-UW-tf-dev-1.59.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.59.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.1.tar", last modified: Mon May  8 03:20:54 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.2.tar", last modified: Tue May  9 21:10:46 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.59.1.tar` & `Simba-UW-tf-dev-1.59.2.tar`

### file list

```diff
@@ -1,484 +1,496 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-03 18:36:16.000000 Simba-UW-tf-dev-1.59.1/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9493 2023-05-07 18:06:51.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.1/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.1/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.59.1/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.1/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.59.1/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.1/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.59.1/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    20790 2023-05-04 17:45:45.000000 Simba-UW-tf-dev-1.59.1/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.1/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.59.1/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.1/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9910 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6791 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    43012 2023-05-03 18:35:59.000000 Simba-UW-tf-dev-1.59.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.1/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42212 2023-05-08 03:07:31.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29499 2023-05-05 16:25:43.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    23591 2023-05-04 16:32:32.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60449 2023-05-03 18:46:32.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.59.1/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12195 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.59.1/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20258 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.1/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.59.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5837 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    34295 2023-05-04 19:36:13.000000 Simba-UW-tf-dev-1.59.1/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)     2335 2023-05-07 19:58:55.000000 Simba-UW-tf-dev-1.59.1/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.59.1/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.59.1/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8385 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.1/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    15294 2023-05-07 18:00:44.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11263 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9514 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13232 2023-05-03 18:58:48.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9036 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6468 2023-05-07 17:57:11.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11814 2023-05-07 17:03:08.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12854 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4817 2023-05-05 01:13:02.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2945 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9608 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7755 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.59.1/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.59.1/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.59.1/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19806 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/sleap_csv_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23531 2023-05-08 03:18:48.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6944 2023-05-07 17:07:14.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.1/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    41779 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.59.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2853 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.59.1/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.59.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.1/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-08 03:20:53.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18493 2023-05-08 03:20:53.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-08 03:20:53.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-08 03:20:53.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-08 03:20:53.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-08 03:20:53.000000 Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.1/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.1/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.1/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-08 03:20:48.000000 Simba-UW-tf-dev-1.59.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-08 03:20:54.000000 Simba-UW-tf-dev-1.59.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-08 20:25:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9493 2023-05-07 18:06:51.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6032 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12633 2023-05-08 03:02:50.000000 Simba-UW-tf-dev-1.59.2/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    33955 2023-05-04 19:55:21.000000 Simba-UW-tf-dev-1.59.2/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20792 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3466 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)    10045 2023-05-09 12:31:02.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7020 2023-05-09 20:47:56.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8522 2023-05-09 20:40:07.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6069 2023-05-09 14:09:16.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42325 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21264 2023-05-09 14:34:28.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13454 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23739 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16652 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.2/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41761 2023-05-09 20:29:25.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29735 2023-05-08 15:27:56.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18431 2023-05-09 17:53:31.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    25962 2023-05-09 13:55:01.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61037 2023-05-08 16:28:07.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    56361 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6858 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7630 2023-05-08 15:03:37.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12196 2023-05-08 14:58:46.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1720 2023-05-08 15:05:19.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15320 2023-05-08 15:06:46.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12645 2023-05-08 15:03:37.000000 Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11617 2023-05-04 13:26:06.000000 Simba-UW-tf-dev-1.59.2/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.2/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5837 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    34300 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2335 2023-05-07 19:58:55.000000 Simba-UW-tf-dev-1.59.2/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14225 2023-05-07 19:37:44.000000 Simba-UW-tf-dev-1.59.2/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8378 2023-05-09 12:23:43.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2641 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9140 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10199 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8571 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12404 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    15294 2023-05-07 18:00:44.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15872 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12769 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5217 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5834 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12806 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12434 2023-05-04 17:45:23.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11290 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15234 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9514 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13262 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11539 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13164 2023-05-04 15:02:11.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9046 2023-05-09 14:13:06.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9801 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16351 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6468 2023-05-07 17:57:11.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11814 2023-05-07 17:03:08.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7444 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12854 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8258 2023-05-04 17:41:51.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4817 2023-05-05 01:13:02.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16856 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2945 2023-05-04 14:18:28.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9616 2023-05-08 15:27:56.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7596 2023-05-09 14:38:58.000000 Simba-UW-tf-dev-1.59.2/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19309 2023-05-08 19:28:39.000000 Simba-UW-tf-dev-1.59.2/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.59.2/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18698 2023-05-04 19:56:21.000000 Simba-UW-tf-dev-1.59.2/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3256 2023-05-08 19:18:20.000000 Simba-UW-tf-dev-1.59.2/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5917 2023-05-04 19:36:28.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19774 2023-05-09 14:43:23.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11373 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11432 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8029 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11066 2023-05-09 19:08:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7374 2023-05-09 19:41:31.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    11817 2023-05-09 19:15:18.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6947 2023-05-09 20:29:25.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.2/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    42300 2023-05-08 18:44:41.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24710 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7343 2023-05-08 18:23:30.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11101 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2853 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-07 17:25:49.000000 Simba-UW-tf-dev-1.59.2/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-09 20:23:32.000000 Simba-UW-tf-dev-1.59.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.2/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18901 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-09 21:10:45.000000 Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.2/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-09 21:10:40.000000 Simba-UW-tf-dev-1.59.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-09 21:10:46.000000 Simba-UW-tf-dev-1.59.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.59.1/PKG-INFO` & `Simba-UW-tf-dev-1.59.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.1
+Version: 1.59.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/.DS_Store`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000a  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,84 +26,84 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00000230: 0000 0001 7b5b 0000 000b 005f 005f 0070  ....{[....._._.p
+00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00000250: 6d6f 4444 626c 6f62 0000 0008 efc0 0270  moDDblob.......p
+00000260: 4305 c541 0000 000b 005f 005f 0070 0079  C..A....._._.p.y
+00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000280: 6444 626c 6f62 0000 0008 efc0 0270 4305  dDblob.......pC.
+00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000002b0: 636f 6d70 0000 0000 0001 e000 0000 0004  comp............
+000002c0: 006d 0069 0073 0063 6473 636c 626f 6f6c  .m.i.s.cdsclbool
+000002d0: 0000 0000 0400 6d00 6900 7300 636c 6731  ......m.i.s.clg1
+000002e0: 5363 6f6d 7000 0000 0000 0037 0b00 0000  Scomp......7....
+000002f0: 0400 6d00 6900 7300 636d 6f44 4462 6c6f  ..m.i.s.cmoDDblo
+00000300: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
+00000310: 0400 6d00 6900 7300 636d 6f64 4462 6c6f  ..m.i.s.cmodDblo
+00000320: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
+00000330: 0400 6d00 6900 7300 6370 6831 5363 6f6d  ..m.i.s.cph1Scom
+00000340: 7000 0000 0000 0040 0000 0000 0000 0000  p......@........
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 000a 0000 000b  ................
-00000410: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000420: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000430: 0000 0003 7661 0000 000b 005f 005f 0070  ....va....._._.p
-00000440: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000450: 6d6f 4444 626c 6f62 0000 0008 e8b0 86b9  moDDblob........
-00000460: 5f01 c541 0000 000b 005f 005f 0070 0079  _..A....._._.p.y
-00000470: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000480: 6444 626c 6f62 0000 0008 29d7 a4d0 97fe  dDblob....).....
-00000490: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000004a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000004b0: 636f 6d70 0000 0000 0003 b000 0000 0007  comp............
-000004c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
-000004d0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
-000004e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
-000004f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00000500: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
-00000510: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00000520: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00000530: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00000540: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00000550: 6261 7208 0809 0809 5f10 187b 7b33 3532  bar....._..{{352
-00000560: 2c20 3234 377d 2c20 7b39 3839 2c20 3433  , 247}, {989, 43
-00000570: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
-00000580: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
-00000590: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 9a00 0000 0700 7000 6f00 7000 5f00  ........p.o.p._.
-000005b0: 7500 7000 736c 6731 5363 6f6d 7000 0000  u.p.slg1Scomp...
-000005c0: 0000 070b b000 0000 0700 7000 6f00 7000  ..........p.o.p.
-000005d0: 5f00 7500 7000 736d 6f44 4462 6c6f 6200  _.u.p.smoDDblob.
-000005e0: 0000 083d 87ac 5070 01c5 4100 0000 0700  ...=..Pp..A.....
-000005f0: 7000 6f00 7000 5f00 7500 7000 736d 6f64  p.o.p._.u.p.smod
-00000600: 4462 6c6f 6200 0000 083d 87ac 5070 01c5  Dblob....=..Pp..
-00000610: 4100 0000 0700 7000 6f00 7000 5f00 7500  A.....p.o.p._.u.
-00000620: 7000 7370 6831 5363 6f6d 7000 0000 0000  p.sph1Scomp.....
-00000630: 09a0 0000 0000 0700 7000 6f00 7000 5f00  ........p.o.p._.
-00000640: 7500 7000 7376 5372 6e6c 6f6e 6700 0000  u.p.svSrnlong...
-00000650: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 040a 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -319,15 +319,15 @@
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
 00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001450: 0100 0002 0000 0000 0000 0000 0200 0008  ................
+00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.59.2/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def __init__(self,
                  config_path: str,
                  file_path: str,
                  threshold_dict: Optional[Dict[str, float]] = None,
                  setting: Literal['from_scratch', 'pseudo'] = 'pseudo',
-                 continuing: bool=False):
+                 continuing: bool = False):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.padding, self.file_path = 5, file_path
         self.frm_no, self.threshold_dict = 0, threshold_dict
         self.setting = setting
         self.play_video_script_path = os.path.join(os.path.dirname(simba.__file__), 'play_annotation_video.py')
         _, self.video_name, _ = get_fn_ext(filepath=file_path)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.59.2/simba/labelling/extract_labelled_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from simba.utils.enums import Dtypes
 from simba.utils.errors import FrameRangeError
 from simba.utils.checks import check_that_column_exist
 
 
 class AnnotationFrameExtractor(ConfigReader):
     def __init__(self,
-                 clfs: List[int],
+                 clfs: List[str],
                  settings: Dict[str, int],
                  config_path: str):
         """
         Extracts all human annotated frames where behavior is annotated as present into .pngs within a SimBA project
 
         :param clfs: Names of classifiers to extract behavior-present images from.
         :param settings: User-defined settings. E.g., how much to downsample the png images.
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.59.2/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.59.2/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0005 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000120: 0065 005f 005f 6473 636c 626f 6f6c 0100  .e._._dsclbool..
+00000120: 0065 005f 005f 6473 636c 626f 6f6c 0000  .e._._dsclbool..
 00000130: 0000 0b00 5f00 5f00 7000 7900 6300 6100  ...._._.p.y.c.a.
 00000140: 6300 6800 6500 5f00 5f6c 6731 5363 6f6d  c.h.e._._lg1Scom
 00000150: 7000 0000 0000 0384 b200 0000 0b00 5f00  p............._.
 00000160: 5f00 7000 7900 6300 6100 6300 6800 6500  _.p.y.c.a.c.h.e.
 00000170: 5f00 5f6d 6f44 4462 6c6f 6200 0000 08f2  _._moDDblob.....
 00000180: 30a5 26c4 f8c4 4100 0000 0b00 5f00 5f00  0.&...A....._._.
 00000190: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,23 @@
                                                PrintEmBeddingInfoPopUp,
                                                DBCVPopUp)
 
 class UnsupervisedGUI(ConfigReader, PopUpMixin):
     def __init__(self,
                  config_path: str):
 
+        """
+        Main access to unsupervised interface
+
+        :param config_path:
+
+        :examples:
+        #>>> _ = UnsupervisedGUI(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+        """
+
         ConfigReader.__init__(self, config_path=config_path)
         PopUpMixin.__init__(self, title="UNSUPERVISED ANALYSIS", config_path=config_path, size=(1000, 800))
         self.main_frm = Toplevel()
         self.main_frm.minsize(1000, 800)
         self.main_frm.wm_title("UNSUPERVISED ANALYSIS")
         self.main_frm.columnconfigure(0, weight=1)
         self.main_frm.rowconfigure(0, weight=1)
@@ -106,15 +115,15 @@
         self.dbcv_btn.grid(row=0, column=0, sticky='NW')
         self.extract_single_metrics_btn.grid(row=1, column=0, sticky='NW')
         self.cluster_descriptives_btn.grid(row=2, column=0, sticky='NW')
         self.cluster_xai_btn.grid(row=3, column=0, sticky='NW')
         self.embedding_corr_btn.grid(row=4, column=0, sticky='NW')
         self.print_embedding_info_btn.grid(row=5, column=0, sticky='NW')
 
-        self.main_frm.mainloop()
+        #self.main_frm.mainloop()
 
     def change_status_of_file_select(self):
         if self.data_slice_dropdown.getChoices() == 'USER-DEFINED FEATURE SET':
             self.feature_file_selected.set_state(setstatus=NORMAL)
         else:
             self.feature_file_selected.set_state(setstatus=DISABLED)
 
@@ -131,8 +140,7 @@
                     'clf_slice': classifier_slice_type,
                     'bout_aggregation_type': bout_selection,
                     'min_bout_length': bout_length,
                     'feature_file_path': feature_file_path}
         _ = DatasetCreator(settings=settings, config_path=self.config_path)
 
 
-_ = UnsupervisedGUI(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.59.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 __author__ = "Simon Nilsson"
-
 import pandas as pd
 import os, glob
+from typing import List
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
+
 from simba.utils.read_write import read_df, get_fn_ext
 from simba.utils.printing import stdout_success
 from simba.utils.errors import NotDirectoryError
 from simba.utils.data import detect_bouts, plug_holes_shortest_bout
 from simba.mixins.config_reader import ConfigReader
 
 class AggBoundaryStatisticsCalculator(ConfigReader):
@@ -32,15 +37,15 @@
     >>> boundary_stats_calculator.run()
     >>> boundary_stats_calculator.save()
     """
 
 
     def __init__(self,
                  config_path: str,
-                 measures: list,
+                 measures: List[Literal['INTERACTION TIME (s)', 'INTERACTION BOUT COUNT', 'INTERACTION BOUT MEAN (s)', 'INTERACTION BOUT MEDIAN (s)']],
                  shortest_allowed_interaction: int):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.measures, self.shortest_allowed_interaction_ms = measures, shortest_allowed_interaction
         self.anchored_roi_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         self.data_path = os.path.join(self.project_path, 'csv', 'anchored_roi_data')
         if not os.path.isdir(self.data_path):
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     roi_keypoint_intersections: bool
         If True, calculates intersection of animal-anchored ROIs and pose-estimated animal key-points.
     save_format: str
         Output data format. OPTIONS: CSV, PARQUET, PICKLE.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md__.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md_>`.
 
     Examples
     ----------
     >>> boundary_stats_calculator = BoundaryStatisticsCalculator(config_path='MyConfigFile',roi_intersections=True, roi_keypoint_intersections=True, save_format='CSV')
     >>> boundary_stats_calculator.save_results()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/find_boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     body_parts: dict
         Body-parts to anchor the ROI to with keys as animal names and values as body-parts. E.g., body_parts={'Animal_1': 'Head_1', 'Animal_2': 'Head_2'}.
     parallel_offset: int
         Offset of ROI from the animal outer bounds in millimeter.
 
     Notes
     ----------
-    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md__.
+    `Bounding boxes tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/anchored_rois.md/>`_.
 
     Examples
     ----------
     >>> animal_boundary_finder= AnimalBoundaryFinder(config_path='/Users/simon/Desktop/troubleshooting/termites/project_folder/project_config.ini', roi_type='SINGLE BODY-PART CIRCLE',body_parts={'Animal_1': 'Head_1', 'Animal_2': 'Head_2'}, force_rectangle=False, parallel_offset=15)
     >>> animal_boundary_finder.find_boundaries()
     """
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.59.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: 0000 0001 4275 6431 0000 a000 0000 0800  ....Bud1........
-00000010: 0000 a000 0000 100c 0000 900c 0000 200c  .............. .
-00000020: 0000 300c 0000 0000 0000 0000 0000 0800  ..0.............
+00000000: 0000 0001 4275 6431 0000 2800 0000 0800  ....Bud1..(.....
+00000010: 0000 2800 0000 300c 0000 100c 0000 400c  ..(...0.......@.
+00000020: 0000 500c 0000 0000 0000 0000 0000 0800  ..P.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 00ac  ................
-00000050: 0000 0009 0000 1000 0075 006e 0064 0069  .........u.n.d.i
-00000060: 006e 0067 0000 0000 0000 0000 0000 0000  .n.g............
+00000040: 0000 0000 0000 000a 0000 0002 0000 00b6  ................
+00000050: 0000 000c 0000 1000 0078 0069 006e 0073  .........x.i.n.s
+00000060: 6c73 7670 0000 0000 0000 0000 0000 0000  lsvp............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,79 +58,79 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
+00000400: 0000 0000 0000 0003 0000 0001 0000 000b  ................
+00000410: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
+00000420: 6c73 7670 626c 6f62 0000 025e 6270 6c69  lsvpblob...^bpli
+00000430: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00000440: 1a46 470a 4458 6963 6f6e 5369 7a65 5f10  .FG.DXiconSize_.
+00000450: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00000460: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00000470: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00000480: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00000490: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+000004a0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+000004b0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+000004c0: 0009 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
+000004d0: 2d32 373c 4158 636f 6d6d 656e 7473 5e64  -27<AXcomments^d
+000004e0: 6174 654c 6173 744f 7065 6e65 645b 6461  ateLastOpened[da
+000004f0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+00000500: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+00000510: 6e54 6e61 6d65 5c64 6174 654d 6f64 6966  nTname\dateModif
+00000520: 6965 64d4 1617 1819 1a1b 0a1d 5776 6973  ied.........Wvis
+00000530: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00000540: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+00000550: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
+00000560: d416 1718 191a 251a 2708 10b5 0810 02d4  ......%.'.......
+00000570: 1617 1819 0a2a 1a2c 0910 6108 1003 d416  .....*.,..a.....
+00000580: 1718 191a 2f0a 3108 1064 0910 05d4 1617  ..../.1..d......
+00000590: 1819 0a34 0a36 0910 7309 1004 d416 1718  ...4.6..s.......
+000005a0: 191a 390a 3b08 104b 0910 06d4 1617 1819  ..9.;..K........
+000005b0: 0a3e 0a40 0911 01c7 0910 00d4 1617 1819  .>.@............
+000005c0: 0a25 1a44 0908 1001 0823 4028 0000 0000  .%.D.....#@(....
+000005d0: 0000 546e 616d 6509 0008 0019 0022 0034  ..Tname......".4
+000005e0: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
+000005f0: 00a9 00b2 00c1 00cd 00d2 00d8 00dd 00e5  ................
+00000600: 00ea 00f7 0100 0108 010e 0118 011e 011f  ................
+00000610: 0122 0123 0125 012e 012f 0131 0132 0134  .".#.%.../.1.2.4
+00000620: 013d 013e 0140 0141 0143 014c 014d 014f  .=.>.@.A.C.L.M.O
+00000630: 0150 0152 015b 015c 015e 015f 0161 016a  .P.R.[.\.^._.a.j
+00000640: 016b 016d 016e 0170 0179 017a 017c 017d  .k.m.n.p.y.z.|.}
+00000650: 017f 0188 0189 018c 018d 018f 0198 0199  ................
+00000660: 019a 019c 019d 01a6 01ab 0000 0000 0000  ................
+00000670: 0201 0000 0000 0000 0049 0000 0000 0000  .........I......
+00000680: 0000 0000 0000 0000 01ac 6564 0808 d40d  ..........ed....
+00000690: 0e0f 1024 1826 0954 7369 7a65 0810 6109  ...$.&.Tsize..a.
+000006a0: d40d 0e0f 1029 092b 0954 6b69 6e64 0910  .....).+.Tkind..
+000006b0: 7309 d40d 0e0f 102e 0930 1855 6c61 6265  s........0.Ulabe
+000006c0: 6c09 1064 08d4 0d0e 0f10 3309 3518 5776  l..d......3.5.Wv
+000006d0: 6572 7369 6f6e 0910 4b08 d40d 0e0f 1038  ersion..K......8
+000006e0: 093a 1858 636f 6d6d 656e 7473 0911 012c  .:.Xcomments...,
+000006f0: 08d4 0d0e 0f10 3d18 3f18 5e64 6174 654c  ......=.?.^dateL
+00000700: 6173 744f 7065 6e65 6408 10c8 08d4 0d0f  astOpened.......
+00000710: 0e10 421d 1818 5964 6174 6541 6464 6564  ..B...YdateAdded
+00000720: 0808 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00000730: 6523 4030 0000 0000 0000 1001 0008 0019  e#@0............
+00000740: 002c 003e 0046 005a 0063 006e 0077 008c  .,.>.F.Z.c.n.w..
+00000750: 008d 008e 009a 00a3 00ae 00b8 00be 00c6  ................
+00000760: 00cb 00cc 00cf 00d0 00d9 00e2 00e4 00e5  ................
+00000770: 00e6 00ef 00fc 00fd 00ff 0100 0109 0115  ................
+00000780: 0116 0117 0120 0125 0126 0128 0129 0132  ..... .%.&.(.).2
+00000790: 0137 0138 013a 013b 0144 014a 014b 014d  .7.8.:.;.D.J.K.M
+000007a0: 014e 0157 015f 0160 0162 0163 016c 0175  .N.W._.`.b.c.l.u
+000007b0: 0176 0179 017a 0183 0192 0193 0195 0196  .v.y.z..........
+000007c0: 019f 01a9 01aa 01ab 01ac 01b5 01ba 01c3  ................
+000007d0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+000007e0: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+000007f0: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
+00000800: 0072 0076 0000 0001 0000 0000 0000 080b  .r.v............
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,232 +250,232 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 000f 0000 0005  ................
-00001010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00001020: 6d70 0000 0000 0003 9e73 0000 0005 0075  mp.......s.....u
-00001030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
-00001040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
-00001050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
-00001060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00001070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00001080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00001090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-000010a0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-000010b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000010c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-000010d0: 1001 09ab 0c15 1d22 262b 3035 3a3f 44d4  ......."&+05:?D.
-000010e0: 0d0e 0f10 0a0a 1314 5776 6973 6962 6c65  ........Wvisible
-000010f0: 5961 7363 656e 6469 6e67 5577 6964 7468  YascendingUwidth
-00001100: 5a69 6465 6e74 6966 6965 7209 0911 0204  Zidentifier.....
-00001110: 546e 616d 65d4 1617 1810 191a 191c 5776  Tname.........Wv
-00001120: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00001130: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
-00001140: 6974 79d4 0d0e 0f10 0a19 2021 0908 10b5  ity....... !....
-00001150: 5c64 6174 654d 6f64 6966 6965 64d4 0d0e  \dateModified...
-00001160: 0f10 1919 2025 0808 5b64 6174 6543 7265  .... %..[dateCre
-00001170: 6174 6564 d40d 0e0f 100a 1929 2a09 0810  ated.......)*...
-00001180: 6154 7369 7a65 d40d 0e0f 100a 0a2e 2f09  aTsize......../.
-00001190: 0910 7354 6b69 6e64 d40d 0e0f 1019 0a33  ..sTkind.......3
-000011a0: 3408 0910 6455 6c61 6265 6cd4 0d0e 0f10  4...dUlabel.....
-000011b0: 190a 3839 0809 104b 5776 6572 7369 6f6e  ..89...KWversion
-000011c0: d40d 0e0f 1019 0a3d 3e08 0911 012c 5863  .......=>....,Xc
-000011d0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1919 4243  omments.......BC
-000011e0: 0808 10c8 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
-000011f0: 6e65 64d4 1617 1810 1920 1947 0808 5964  ned...... .G..Yd
-00001200: 6174 6541 6464 6564 0823 4028 0000 0000  ateAdded.#@(....
-00001210: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
-00001220: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-00001230: 7000 8300 8c00 8e00 8f00 9b00 a400 ac00  p...............
-00001240: b600 bc00 c700 c800 c900 cc00 d100 da00  ................
-00001250: e200 e800 f200 f300 f500 f600 ff01 0801  ................
-00001260: 0901 0a01 0c01 1901 2201 2301 2401 3001  ........".#.$.0.
-00001270: 3901 3a01 3b01 3d01 4201 4b01 4c01 4d01  9.:.;.=.B.K.L.M.
-00001280: 4f01 5401 5d01 5e01 5f01 6101 6701 7001  O.T.].^._.a.g.p.
-00001290: 7101 7201 7401 7c01 8501 8601 8701 8a01  q.r.t.|.........
-000012a0: 9301 9c01 9d01 9e01 a001 af01 b801 b901  ................
-000012b0: ba01 c401 c501 ce01 d301 d400 0000 0000  ................
-000012c0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-000012d0: 0000 0000 0000 0000 0001 dd00 0000 0500  ................
-000012e0: 7500 7400 6900 6c00 736c 7376 7062 6c6f  u.t.i.l.slsvpblo
-000012f0: 6200 0002 5e62 706c 6973 7430 30d8 0102  b...^bplist00...
-00001300: 0304 0506 0708 090a 0b1d 4546 0a48 5f10  ..........EF.H_.
-00001310: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00001320: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00001330: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00001340: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00001350: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00001360: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00001370: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
-00001380: 6510 0109 d90c 0d0e 0f10 1112 1314 151e  e...............
-00001390: 2328 2d32 373c 4158 636f 6d6d 656e 7473  #(-27<AXcomments
-000013a0: 5e64 6174 654c 6173 744f 7065 6e65 645b  ^dateLastOpened[
-000013b0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-000013c0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-000013d0: 696f 6e54 6e61 6d65 5c64 6174 654d 6f64  ionTname\dateMod
-000013e0: 6966 6965 64d4 1617 1819 1a0a 1c1d 5569  ified.........Ui
-000013f0: 6e64 6578 5961 7363 656e 6469 6e67 5577  ndexYascendingUw
-00001400: 6964 7468 5776 6973 6962 6c65 1007 0911  idthWvisible....
-00001410: 012c 08d4 1617 1819 1f1d 211d 1008 0810  .,........!.....
-00001420: c808 d416 1718 1924 1d26 1d10 0208 10b5  .......$.&......
-00001430: 08d4 1617 1819 291d 2b0a 1003 0810 6109  ......).+.....a.
-00001440: d416 1718 192e 0a30 1d10 0509 1064 08d4  .......0.....d..
-00001450: 1617 1819 330a 350a 1004 0910 7309 d416  ....3.5.....s...
-00001460: 1718 1938 0a3a 1d10 0609 104b 08d4 1617  ...8.:.....K....
-00001470: 1819 3d0a 3f0a 1000 0911 0204 09d4 1617  ..=.?...........
-00001480: 1819 091d 260a 0809 0823 4028 0000 0000  ....&....#@(....
-00001490: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
-000014a0: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-000014b0: 7000 8300 8c00 8e00 8f00 a200 ab00 ba00  p...............
-000014c0: c600 cb00 d100 d600 de00 e300 f000 f900  ................
-000014d0: ff01 0901 0f01 1701 1901 1a01 1d01 1e01  ................
-000014e0: 2701 2901 2a01 2c01 2d01 3601 3801 3901  '.).*.,.-.6.8.9.
-000014f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
-00001500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
-00001510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
-00001520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
-00001530: a201 a300 0000 0000 0002 0100 0000 0000  ................
-00001540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
-00001550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00001560: 736d 6f44 4462 6c6f 6200 0000 0814 4083  smoDDblob.....@.
-00001570: 1561 01c5 4100 0000 0500 7500 7400 6900  .a..A.....u.t.i.
-00001580: 6c00 736d 6f64 4462 6c6f 6200 0000 08cc  l.smodDblob.....
-00001590: dc81 8648 fec4 4100 0000 0500 7500 7400  ...H..A.....u.t.
-000015a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000015b0: 0000 0420 0000 0000 0500 7500 7400 6900  ... ......u.t.i.
-000015c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
-000015d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-000015e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000015f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
-00001600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00001610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00001620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00001630: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00001640: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00001650: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00001660: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00001670: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-00001680: 7b7b 3335 322c 2032 3437 7d2c 207b 3938  {{352, 247}, {98
-00001690: 392c 2034 3336 7d7d 0908 1725 313d 4960  9, 436}}...%1=I`
-000016a0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
-000016b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-000016c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
-000016d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
-000016e0: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-000016f0: 636f 6d70 0000 0000 0003 61f1 0000 0010  comp......a.....
-00001700: 0076 0069 0064 0065 006f 005f 0070 0072  .v.i.d.e.o._.p.r
-00001710: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
-00001720: 6c73 7643 626c 6f62 0000 0307 6270 6c69  lsvCblob....bpli
-00001730: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00001740: 1956 570a 5958 6963 6f6e 5369 7a65 5f10  .VW.YXiconSize_.
-00001750: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001760: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001770: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00001780: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00001790: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-000017a0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-000017b0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-000017c0: 0009 ae0c 151d 2226 2b30 353a 3f44 484d  ......"&+05:?DHM
-000017d0: 51d4 0d0e 0f10 1112 0a0a 5a69 6465 6e74  Q.........Zident
-000017e0: 6966 6965 7255 7769 6474 6859 6173 6365  ifierUwidthYasce
-000017f0: 6e64 696e 6757 7669 7369 626c 6554 6e61  ndingWvisibleTna
-00001800: 6d65 1103 2a09 09d4 1617 180d 191a 191c  me..*...........
-00001810: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00001820: 7363 656e 6469 6e67 0810 2308 5875 6269  scending..#.Xubi
-00001830: 7175 6974 79d4 0d0e 0f10 1e1f 190a 5c64  quity.........\d
-00001840: 6174 654d 6f64 6966 6965 6410 b508 09d4  ateModified.....
-00001850: 0d0e 0f10 231f 1919 5b64 6174 6543 7265  ....#...[dateCre
-00001860: 6174 6564 0808 d40d 0e0f 1027 2819 0a54  ated.......'(..T
-00001870: 7369 7a65 1061 0809 d40d 0e0f 102c 2d0a  size.a.......,-.
-00001880: 0a54 6b69 6e64 1073 0909 d40d 0e0f 1031  .Tkind.s.......1
-00001890: 320a 1955 6c61 6265 6c10 6409 08d4 0d0e  2..Ulabel.d.....
-000018a0: 0f10 3637 0a19 5776 6572 7369 6f6e 104b  ..67..Wversion.K
-000018b0: 0908 d40d 0e0f 103b 3c0a 1958 636f 6d6d  .......;<..Xcomm
-000018c0: 656e 7473 1101 2c09 08d4 0d0e 0f10 4041  ents..,.......@A
-000018d0: 1919 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-000018e0: 6410 c808 08d4 1617 180d 191f 1947 0808  d............G..
-000018f0: 5964 6174 6541 6464 6564 d40d 1718 1649  YdateAdded.....I
-00001900: 4a19 195a 7368 6172 654f 776e 6572 10d2  J..ZshareOwner..
-00001910: 0808 d40d 1718 164e 4a19 195f 100f 7368  .......NJ.._..sh
-00001920: 6172 654c 6173 7445 6469 746f 7208 08d4  areLastEditor...
-00001930: 0d17 1816 524a 1919 5f10 1069 6e76 6974  ....RJ.._..invit
-00001940: 6174 696f 6e53 7461 7475 7308 0808 2340  ationStatus...#@
-00001950: 2800 0000 0000 0054 6e61 6d65 0910 0100  (......Tname....
-00001960: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
-00001970: 7700 8c00 9500 9600 a500 ae00 b900 bf00  w...............
-00001980: c900 d100 d600 d900 da00 db00 e400 ec00  ................
-00001990: f200 fc00 fd00 ff01 0001 0901 1201 1f01  ................
-000019a0: 2101 2201 2301 2c01 3801 3901 3a01 4301  !.".#.,.8.9.:.C.
-000019b0: 4801 4a01 4b01 4c01 5501 5a01 5c01 5d01  H.J.K.L.U.Z.\.].
-000019c0: 5e01 6701 6d01 6f01 7001 7101 7a01 8201  ^.g.m.o.p.q.z...
-000019d0: 8401 8501 8601 8f01 9801 9b01 9c01 9d01  ................
-000019e0: a601 b501 b701 b801 b901 c201 c301 c401  ................
-000019f0: ce01 d701 e201 e401 e501 e601 ef02 0102  ................
-00001a00: 0202 0302 0c02 1f02 2002 2102 2202 2b02  ........ .!.".+.
-00001a10: 3002 3100 0000 0000 0002 0100 0000 0000  0.1.............
-00001a20: 0000 5a00 0000 0000 0000 0000 0000 0000  ..Z.............
-00001a30: 0002 3300 0000 1000 7600 6900 6400 6500  ..3.....v.i.d.e.
-00001a40: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
-00001a50: 7300 6f00 7200 736c 7376 7062 6c6f 6200  s.o.r.slsvpblob.
-00001a60: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
-00001a70: 0506 0708 090a 0b1a 4647 0a35 5869 636f  ........FG.5Xico
-00001a80: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
-00001a90: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00001aa0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00001ab0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-00001ac0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-00001ad0: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
-00001ae0: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
-00001af0: 4030 0000 0000 0000 09d9 0c0d 0e0f 1011  @0..............
-00001b00: 1213 1415 1e23 282d 3236 3b40 5863 6f6d  .....#(-26;@Xcom
-00001b10: 6d65 6e74 7355 6c61 6265 6c57 7665 7273  mentsUlabelWvers
-00001b20: 696f 6e5b 6461 7465 4372 6561 7465 6454  ion[dateCreatedT
-00001b30: 7369 7a65 5c64 6174 654d 6f64 6966 6965  size\dateModifie
-00001b40: 6454 6b69 6e64 546e 616d 655e 6461 7465  dTkindTname^date
-00001b50: 4c61 7374 4f70 656e 6564 d416 1718 191a  LastOpened......
-00001b60: 1b0a 1d57 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
-00001b70: 6859 6173 6365 6e64 696e 6755 696e 6465  hYascendingUinde
-00001b80: 7808 1101 2c09 1007 d416 1718 191a 200a  x...,......... .
-00001b90: 2208 1064 0910 05d4 1617 1819 1a25 0a27  "..d.........%.'
-00001ba0: 0810 4b09 1006 d416 1718 191a 2a1a 2c08  ..K.........*.,.
-00001bb0: 10b5 0810 02d4 1617 1819 0a2f 1a31 0910  .........../.1..
-00001bc0: 6108 1003 d416 1718 190a 2a1a 3509 0810  a.........*.5...
-00001bd0: 01d4 1617 1819 0a38 0a3a 0910 7309 1004  .......8.:..s...
-00001be0: d416 1718 190a 3d0a 3f09 1103 2a09 1000  ......=.?...*...
-00001bf0: d416 1718 191a 421a 4408 10c8 0810 0808  ......B.D.......
-00001c00: 2340 2800 0000 0000 0054 6e61 6d65 0900  #@(......Tname..
-00001c10: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
-00001c20: 7700 8c00 9500 9600 a900 b200 b800 c000  w...............
-00001c30: cc00 d100 de00 e300 e800 f701 0001 0801  ................
-00001c40: 0e01 1801 1e01 1f01 2201 2301 2501 2e01  ........".#.%...
-00001c50: 2f01 3101 3201 3401 3d01 3e01 4001 4101  /.1.2.4.=.>.@.A.
-00001c60: 4301 4c01 4d01 4f01 5001 5201 5b01 5c01  C.L.M.O.P.R.[.\.
-00001c70: 5e01 5f01 6101 6a01 6b01 6c01 6e01 7701  ^._.a.j.k.l.n.w.
-00001c80: 7801 7a01 7b01 7d01 8601 8701 8a01 8b01  x.z.{.}.........
-00001c90: 8d01 9601 9701 9901 9a01 9c01 9d01 a601  ................
-00001ca0: ab00 0000 0000 0002 0100 0000 0000 0000  ................
-00001cb0: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-00001cc0: ac00 0000 1000 7600 6900 6400 6500 6f00  ......v.i.d.e.o.
-00001cd0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-00001ce0: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00001cf0: 0858 fa45 86d0 fec4 4100 0000 1000 7600  .X.E....A.....v.
-00001d00: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
-00001d10: 6300 6500 7300 7300 6f00 7200 736d 6f64  c.e.s.s.o.r.smod
-00001d20: 4462 6c6f 6200 0000 0858 fa45 86d0 fec4  Dblob....X.E....
-00001d30: 4100 0000 1000 7600 6900 6400 6500 6f00  A.....v.i.d.e.o.
-00001d40: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-00001d50: 6f00 7200 7370 6831 5363 6f6d 7000 0000  o.r.sph1Scomp...
-00001d60: 0000 0440 0000 0000 1000 7600 6900 6400  ...@......v.i.d.
-00001d70: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
-00001d80: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
-00001d90: 6700 0000 0100 0000 0000 0000 0000 0000  g...............
+00001000: 0000 0000 0000 0002 0000 0005 0000 0007  ................
+00001010: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+00001020: 006e 0067 6c73 7643 626c 6f62 0000 02b0  .n.glsvCblob....
+00001030: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00001040: 0809 0a0b 0c0d 1848 4948 4a0c 4c5f 1012  .......HIHJ.L_..
+00001050: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001060: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00001070: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001080: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00001090: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000010a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000010b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000010c0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000010d0: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
+000010e0: 5369 7a65 1001 09ab 0e17 1c21 252a 2f34  Size.......!%*/4
+000010f0: 393e 43d4 0f10 1112 0c14 0c16 5776 6973  9>C.........Wvis
+00001100: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00001110: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
+00001120: 1101 c709 546e 616d 65d4 0f10 1112 1819  ....Tname.......
+00001130: 181b 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
+00001140: 0f10 1112 0c1e 1820 0910 b508 5c64 6174  ....... ....\dat
+00001150: 654d 6f64 6966 6965 64d4 0f10 1112 181e  eModified.......
+00001160: 1824 0808 5b64 6174 6543 7265 6174 6564  .$..[dateCreated
+00001170: d40f 1011 120c 2718 2909 1061 0854 7369  ......'.)..a.Tsi
+00001180: 7a65 d40f 1011 120c 2c0c 2e09 1073 0954  ze......,....s.T
+00001190: 6b69 6e64 d40f 1011 1218 310c 3308 1064  kind......1.3..d
+000011a0: 0955 6c61 6265 6cd4 0f10 1112 1836 0c38  .Ulabel......6.8
+000011b0: 0810 4b09 5776 6572 7369 6f6e d40f 1011  ..K.Wversion....
+000011c0: 1218 3b0c 3d08 1101 2c09 5863 6f6d 6d65  ..;.=...,.Xcomme
+000011d0: 6e74 73d4 0f10 1112 1840 1842 0810 c808  nts......@.B....
+000011e0: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
+000011f0: 0f10 1112 181e 1846 0808 5964 6174 6541  .......F..YdateA
+00001200: 6464 6564 0823 0000 0000 0000 0000 2340  dded.#........#@
+00001210: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
+00001220: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
+00001230: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
+00001240: 00b7 00c3 00cc 00d4 00da 00e4 00ef 00f0  ................
+00001250: 00f3 00f4 00f9 0102 0103 0105 0106 010f  ................
+00001260: 0118 0119 011b 011c 0129 0132 0133 0134  .........).2.3.4
+00001270: 0140 0149 014a 014c 014d 0152 015b 015c  .@.I.J.L.M.R.[.\
+00001280: 015e 015f 0164 016d 016e 0170 0171 0177  .^._.d.m.n.p.q.w
+00001290: 0180 0181 0183 0184 018c 0195 0196 0199  ................
+000012a0: 019a 01a3 01ac 01ad 01af 01b0 01bf 01c8  ................
+000012b0: 01c9 01ca 01d4 01d5 01de 01e7 01ec 01ed  ................
+000012c0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
+000012d0: 0000 0000 0000 0000 0000 0000 0000 01f6  ................
+000012e0: 0000 0008 0000 000e 0070 006f 0073 0065  .........p.o.s.e
+000012f0: 005f 0069 006d 0070 006f 0072 0074 0065  ._.i.m.p.o.r.t.e
+00001300: 0072 0073 6c73 7643 626c 6f62 0000 0281  .r.slsvCblob....
+00001310: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+00001320: 0809 0a0b 1846 4748 0a5f 1012 7669 6577  .....FGH._..view
+00001330: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00001340: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001350: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00001360: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00001370: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00001380: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
+00001390: 656c 6174 6976 6544 6174 6573 1001 09ab  elativeDates....
+000013a0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
+000013b0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+000013c0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+000013d0: 7669 7369 626c 6554 6e61 6d65 1101 c709  visibleTname....
+000013e0: 09d4 0d0e 0f10 1617 1818 5875 6269 7175  ..........Xubiqu
+000013f0: 6974 7910 2308 08d4 0d0e 0f10 1b1c 180a  ity.#...........
+00001400: 5c64 6174 654d 6f64 6966 6965 6410 b508  \dateModified...
+00001410: 09d4 0d0e 0f10 201c 1818 5b64 6174 6543  ...... ...[dateC
+00001420: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
+00001430: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
+00001440: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
+00001450: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
+00001460: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
+00001470: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
+00001480: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
+00001490: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
+000014a0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
+000014b0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
+000014c0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+000014d0: 6965 6423 4030 0000 0000 0000 0900 0800  ied#@0..........
+000014e0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
+000014f0: 8c00 8e00 8f00 9b00 a400 af00 b500 bf00  ................
+00001500: c700 cc00 cf00 d000 d100 da00 e300 e500  ................
+00001510: e600 e700 f000 fd00 ff01 0001 0101 0a01  ................
+00001520: 1601 1701 1801 2101 2601 2801 2901 2a01  ......!.&.(.).*.
+00001530: 3301 3801 3a01 3b01 3c01 4501 4b01 4d01  3.8.:.;.<.E.K.M.
+00001540: 4e01 4f01 5801 6001 6201 6301 6401 6d01  N.O.X.`.b.c.d.m.
+00001550: 7601 7901 7a01 7b01 8401 9301 9501 9601  v.y.z.{.........
+00001560: 9701 a001 aa01 ab01 ac01 ad01 b601 c301  ................
+00001570: cc00 0000 0000 0002 0100 0000 0000 0000  ................
+00001580: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
+00001590: cd00 0000 0900 0000 0900 7200 6f00 6900  ..........r.o.i.
+000015a0: 5f00 7400 6f00 6f00 6c00 736c 7376 7062  _.t.o.o.l.slsvpb
+000015b0: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
+000015c0: 0102 0304 0506 0708 090a 0b1d 4546 470a  ............EFG.
+000015d0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000015e0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+000015f0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00001600: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00001610: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00001620: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+00001630: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001640: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
+00001650: 151e 2327 2b30 353a 3f58 636f 6d6d 656e  ..#'+05:?Xcommen
+00001660: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+00001670: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
+00001680: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00001690: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+000016a0: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
+000016b0: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
+000016c0: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
+000016d0: 1101 2c09 08d4 1617 1819 1f20 1d1d 1008  ..,........ ....
+000016e0: 10c8 0808 d416 1718 1909 241d 0a10 b508  ..........$.....
+000016f0: 09d4 1617 1819 2824 1d1d 1002 0808 d416  ......($........
+00001700: 1718 192c 2d1d 0a10 0310 6108 09d4 1617  ...,-.....a.....
+00001710: 1819 3132 0a1d 1005 1064 0908 d416 1718  ..12.....d......
+00001720: 1936 370a 0a10 0410 7309 09d4 1617 1819  .67.....s.......
+00001730: 3b3c 0a1d 1006 104b 0908 d416 1718 1940  ;<.....K.......@
+00001740: 410a 0a10 0011 01c7 0909 0823 4028 0000  A..........#@(..
+00001750: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
+00001760: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+00001770: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
+00001780: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
+00001790: f900 ff01 0501 0f01 1701 1901 1c01 1d01  ................
+000017a0: 1e01 2701 2901 2b01 2c01 2d01 3601 3801  ..'.).+.,.-.6.8.
+000017b0: 3901 3a01 4301 4501 4601 4701 5001 5201  9.:.C.E.F.G.P.R.
+000017c0: 5401 5501 5601 5f01 6101 6301 6401 6501  T.U.V._.a.c.d.e.
+000017d0: 6e01 7001 7201 7301 7401 7d01 7f01 8101  n.p.r.s.t.}.....
+000017e0: 8201 8301 8c01 8e01 9101 9201 9301 9401  ................
+000017f0: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
+00001800: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
+00001810: 0000 0001 ac00 0000 0c00 0000 0200 7500  ..............u.
+00001820: 6976 5372 6e6c 6f6e 6700 0000 0100 0000  ivSrnlong.......
+00001830: 0d00 0000 0500 7500 7400 6900 6c00 7364  ......u.t.i.l.sd
+00001840: 7363 6c62 6f6f 6c00 0000 0000 0000 0000  sclbool.........
+00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -506,2184 +506,2568 @@
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0000 0000 0016 0000 000b  ................
-00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0042 034e 0000 000b 005f 005f 0070  ...B.N....._._.p
-00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 d651 eebb  moDDblob.....Q..
-00002060: 6401 c541 0000 000b 005f 005f 0070 0079  d..A....._._.p.y
-00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00002080: 6444 626c 6f62 0000 0008 be68 6b6a 58ff  dDblob.....hkjX.
-00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000020b0: 636f 6d70 0000 0000 004f e000 0000 0006  comp.....O......
-000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
-000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
-000020e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-000020f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00002100: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00002110: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00002120: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00002130: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00002140: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002150: 7208 0809 0809 5f10 177b 7b32 302c 2039  r....._..{{20, 9
-00002160: 307d 2c20 7b31 3031 352c 2037 3637 7d7d  0}, {1015, 767}}
-00002170: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
-00002180: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00002190: 0000 0000 0000 0000 0000 0000 0000 0099  ................
-000021a0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021b0: 6c67 3153 636f 6d70 0000 0000 007d db93  lg1Scomp.....}..
-000021c0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021d0: 6c73 7643 626c 6f62 0000 02b0 6270 6c69  lsvCblob....bpli
-000021e0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-000021f0: 0c0d 1848 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
-00002200: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00002210: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00002220: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00002230: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00002240: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00002250: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-00002260: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-00002270: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-00002280: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00002290: 1001 09ab 0e17 1c21 252a 2f34 393e 43d4  .......!%*/49>C.
-000022a0: 0f10 1112 0c14 0c16 5776 6973 6962 6c65  ........Wvisible
-000022b0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-000022c0: 5a69 6465 6e74 6966 6965 7209 1101 2709  Zidentifier...'.
-000022d0: 546e 616d 65d4 0f10 1112 1819 181b 0810  Tname...........
-000022e0: 2308 5875 6269 7175 6974 79d4 0f10 1112  #.Xubiquity.....
-000022f0: 0c1e 1820 0910 b508 5c64 6174 654d 6f64  ... ....\dateMod
-00002300: 6966 6965 64d4 0f10 1112 181e 1824 0808  ified........$..
-00002310: 5b64 6174 6543 7265 6174 6564 d40f 1011  [dateCreated....
-00002320: 120c 2718 2909 1061 0854 7369 7a65 d40f  ..'.)..a.Tsize..
-00002330: 1011 120c 2c0c 2e09 1073 0954 6b69 6e64  ....,....s.Tkind
-00002340: d40f 1011 1218 310c 3308 1064 0955 6c61  ......1.3..d.Ula
-00002350: 6265 6cd4 0f10 1112 1836 0c38 0810 4b09  bel......6.8..K.
-00002360: 5776 6572 7369 6f6e d40f 1011 1218 3b0c  Wversion......;.
-00002370: 3d08 1101 2c09 5863 6f6d 6d65 6e74 73d4  =...,.Xcomments.
-00002380: 0f10 1112 1840 1842 0810 c808 5e64 6174  .....@.B....^dat
-00002390: 654c 6173 744f 7065 6e65 64d4 0f10 1112  eLastOpened.....
-000023a0: 181e 1846 0808 5964 6174 6541 6464 6564  ...F..YdateAdded
-000023b0: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
-000023c0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-000023d0: 0009 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
-000023e0: 007b 008d 0098 00a1 00b4 00b6 00b7 00c3  .{..............
-000023f0: 00cc 00d4 00da 00e4 00ef 00f0 00f3 00f4  ................
-00002400: 00f9 0102 0103 0105 0106 010f 0118 0119  ................
-00002410: 011b 011c 0129 0132 0133 0134 0140 0149  .....).2.3.4.@.I
-00002420: 014a 014c 014d 0152 015b 015c 015e 015f  .J.L.M.R.[.\.^._
-00002430: 0164 016d 016e 0170 0171 0177 0180 0181  .d.m.n.p.q.w....
-00002440: 0183 0184 018c 0195 0196 0199 019a 01a3  ................
-00002450: 01ac 01ad 01af 01b0 01bf 01c8 01c9 01ca  ................
-00002460: 01d4 01d5 01de 01e7 01ec 01f5 0000 0000  ................
-00002470: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
-00002480: 0000 0000 0000 0000 0000 01f6 0000 0006  ................
-00002490: 0061 0073 0073 0065 0074 0073 6c73 7670  .a.s.s.e.t.slsvp
-000024a0: 626c 6f62 0000 0295 6270 6c69 7374 3030  blob....bplist00
-000024b0: da01 0203 0405 0607 0809 0a0b 0c0d 1f47  ...............G
-000024c0: 4847 494a 0c5f 1012 7669 6577 4f70 7469  HGIJ._..viewOpti
-000024d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-000024e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-000024f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00002500: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00002510: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-00002520: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-00002530: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00002540: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
-00002550: 656c 6174 6976 6544 6174 6573 1001 09d9  elativeDates....
-00002560: 0e0f 1011 1213 1415 1617 2025 292d 3237  .......... %)-27
-00002570: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00002580: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
-00002590: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
-000025a0: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
-000025b0: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
-000025c0: d418 191a 1b1c 1d0c 1f55 696e 6465 7855  .........UindexU
-000025d0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-000025e0: 7669 7369 626c 6510 0711 012c 0908 d418  visible....,....
-000025f0: 191a 1b21 221f 1f10 0810 c808 08d4 1819  ...!"...........
-00002600: 1a1b 0b26 1f0c 10b5 0809 d418 191a 1b2a  ...&...........*
-00002610: 261f 1f10 0208 08d4 1819 1a1b 2e2f 1f0c  &............/..
-00002620: 1003 1061 0809 d418 191a 1b33 340c 1f10  ...a.......34...
-00002630: 0510 6409 08d4 1819 1a1b 3839 0c0c 1004  ..d.......89....
-00002640: 1073 0909 d418 191a 1b3d 3e0c 1f10 0610  .s.......=>.....
-00002650: 4b09 08d4 1819 1a1b 4243 0c0c 1000 1101  K.......BC......
-00002660: 2709 0908 2300 0000 0000 0000 0023 4028  '...#........#@(
-00002670: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-00002680: 0000 0000 0900 0800 1d00 3200 4400 4c00  ..........2.D.L.
-00002690: 6000 7200 7b00 8d00 9800 a100 b400 b600  `.r.{...........
-000026a0: b700 ca00 d300 e200 ef00 fb01 0001 0601  ................
-000026b0: 0b01 1301 1801 2101 2701 2d01 3701 3f01  ......!.'.-.7.?.
-000026c0: 4101 4401 4501 4601 4f01 5101 5301 5401  A.D.E.F.O.Q.S.T.
-000026d0: 5501 5e01 6001 6101 6201 6b01 6d01 6e01  U.^.`.a.b.k.m.n.
-000026e0: 6f01 7801 7a01 7c01 7d01 7e01 8701 8901  o.x.z.|.}.~.....
-000026f0: 8b01 8c01 8d01 9601 9801 9a01 9b01 9c01  ................
-00002700: a501 a701 a901 aa01 ab01 b401 b601 b901  ................
-00002710: ba01 bb01 bc01 c501 ce01 d301 dc00 0000  ................
-00002720: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
-00002730: 0000 0000 0000 0000 0000 0001 dd00 0000  ................
-00002740: 0600 6100 7300 7300 6500 7400 736d 6f44  ..a.s.s.e.t.smoD
-00002750: 4462 6c6f 6200 0000 08cf 958c e8d0 e1c4  Dblob...........
-00002760: 4100 0000 0600 6100 7300 7300 6500 7400  A.....a.s.s.e.t.
-00002770: 736d 6f64 4462 6c6f 6200 0000 08cf 958c  smodDblob.......
-00002780: e8d0 e1c4 4100 0000 0600 6100 7300 7300  ....A.....a.s.s.
-00002790: 6500 7400 7370 6831 5363 6f6d 7000 0000  e.t.sph1Scomp...
-000027a0: 0000 81a0 0000 0000 0600 6100 7300 7300  ..........a.s.s.
-000027b0: 6500 7400 7376 5372 6e6c 6f6e 6700 0000  e.t.svSrnlong...
-000027c0: 0100 0000 0c00 6200 6c00 6f00 6200 5f00  ......b.l.o.b._.
-000027d0: 7300 7400 6f00 7200 6100 6700 6562 7773  s.t.o.r.a.g.ebws
-000027e0: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
-000027f0: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00002800: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00002810: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00002820: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00002830: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00002840: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00002850: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00002860: 6172 0808 0908 095f 1018 7b7b 3531 392c  ar....._..{{519,
-00002870: 2033 3334 7d2c 207b 3737 302c 2034 3336   334}, {770, 436
-00002880: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00002890: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-000028a0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-000028b0: 009a 0000 000c 0062 006c 006f 0062 005f  .......b.l.o.b._
-000028c0: 0073 0074 006f 0072 0061 0067 0065 6c67  .s.t.o.r.a.g.elg
-000028d0: 3153 636f 6d70 0000 0000 0000 1804 0000  1Scomp..........
-000028e0: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
-000028f0: 006f 0072 0061 0067 0065 6d6f 4444 626c  .o.r.a.g.emoDDbl
-00002900: 6f62 0000 0008 3f3c 3f74 e2dd c441 0000  ob....?<?t...A..
-00002910: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
-00002920: 006f 0072 0061 0067 0065 6d6f 6444 626c  .o.r.a.g.emodDbl
-00002930: 6f62 0000 0008 3f3c 3f74 e2dd c441 0000  ob....?<?t...A..
-00002940: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
-00002950: 006f 0072 0061 0067 0065 7068 3153 636f  .o.r.a.g.eph1Sco
-00002960: 6d70 0000 0000 0000 2000 0000 000c 0062  mp...... ......b
-00002970: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
-00002980: 0061 0067 0065 7653 726e 6c6f 6e67 0000  .a.g.evSrnlong..
-00002990: 0001 0000 0012 0062 006f 0075 006e 0064  .......b.o.u.n.d
-000029a0: 0069 006e 0067 005f 0062 006f 0078 005f  .i.n.g._.b.o.x._
-000029b0: 0074 006f 006f 006c 0073 6277 7370 626c  .t.o.o.l.sbwspbl
-000029c0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
-000029d0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-000029e0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-000029f0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00002a00: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00002a10: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00002a20: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002a30: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00002a40: 0809 0809 5f10 187b 7b33 3934 2c20 3138  ...._..{{394, 18
-00002a50: 317d 2c20 7b37 3730 2c20 3433 367d 7d09  1}, {770, 436}}.
-00002a60: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
-00002a70: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00002a80: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
-00002a90: 0000 1200 6200 6f00 7500 6e00 6400 6900  ....b.o.u.n.d.i.
-00002aa0: 6e00 6700 5f00 6200 6f00 7800 5f00 7400  n.g._.b.o.x._.t.
-00002ab0: 6f00 6f00 6c00 7364 7363 6c62 6f6f 6c00  o.o.l.sdsclbool.
-00002ac0: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
-00002ad0: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
-00002ae0: 006f 006f 006c 0073 6c67 3153 636f 6d70  .o.o.l.slg1Scomp
-00002af0: 0000 0000 0002 6bd2 0000 0012 0062 006f  ......k......b.o
-00002b00: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
-00002b10: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
-00002b20: 6c73 7643 626c 6f62 0000 0278 6270 6c69  lsvCblob...xbpli
-00002b30: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00002b40: 1846 470a 4958 6963 6f6e 5369 7a65 5f10  .FG.IXiconSize_.
-00002b50: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00002b60: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00002b70: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00002b80: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00002b90: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00002ba0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00002bb0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00002bc0: 0009 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
-00002bd0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
-00002be0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-00002bf0: 6e67 5776 6973 6962 6c65 546e 616d 6510  ngWvisibleTname.
-00002c00: f009 09d4 0d0e 0f10 1617 1818 5875 6269  ............Xubi
-00002c10: 7175 6974 7910 2308 08d4 0d0e 0f10 1b1c  quity.#.........
-00002c20: 180a 5c64 6174 654d 6f64 6966 6965 6410  ..\dateModified.
-00002c30: b508 09d4 0d0e 0f10 201c 1818 5b64 6174  ........ ...[dat
-00002c40: 6543 7265 6174 6564 0808 d40d 0e0f 1024  eCreated.......$
-00002c50: 2518 0a54 7369 7a65 1061 0809 d40d 0e0f  %..Tsize.a......
-00002c60: 1029 2a0a 0a54 6b69 6e64 1073 0909 d40d  .)*..Tkind.s....
-00002c70: 0e0f 102e 2f0a 1855 6c61 6265 6c10 6409  ..../..Ulabel.d.
-00002c80: 08d4 0d0e 0f10 3334 0a18 5776 6572 7369  ......34..Wversi
-00002c90: 6f6e 104b 0908 d40d 0e0f 1038 390a 1858  on.K.......89..X
-00002ca0: 636f 6d6d 656e 7473 1101 2c09 08d4 0d0e  comments..,.....
-00002cb0: 0f10 3d3e 1818 5e64 6174 654c 6173 744f  ..=>..^dateLastO
-00002cc0: 7065 6e65 6410 c808 08d4 0d0e 0f10 421c  pened.........B.
-00002cd0: 1818 5964 6174 6541 6464 6564 0808 0823  ..YdateAdded...#
-00002ce0: 4028 0000 0000 0000 546e 616d 6509 1001  @(......Tname...
-00002cf0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00002d00: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
-00002d10: 00c6 00ce 00d3 00d5 00d6 00d7 00e0 00e9  ................
-00002d20: 00eb 00ec 00ed 00f6 0103 0105 0106 0107  ................
-00002d30: 0110 011c 011d 011e 0127 012c 012e 012f  .........'.,.../
-00002d40: 0130 0139 013e 0140 0141 0142 014b 0151  .0.9.>.@.A.B.K.Q
-00002d50: 0153 0154 0155 015e 0166 0168 0169 016a  .S.T.U.^.f.h.i.j
-00002d60: 0173 017c 017f 0180 0181 018a 0199 019b  .s.|............
-00002d70: 019c 019d 01a6 01b0 01b1 01b2 01b3 01bc  ................
-00002d80: 01c1 01c2 0000 0000 0000 0201 0000 0000  ................
-00002d90: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-00002da0: 0000 01c4 0000 0000 0000 0000 0000 0000  ................
-00002db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003000: 0000 0000 0000 0000 0000 0023 0000 0012  ...........#....
-00003010: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
-00003020: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
-00003030: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
-00003040: d59a 2b59 34fe c441 0000 0012 0062 006f  ..+Y4..A.....b.o
-00003050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
-00003060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
-00003070: 6d6f 6444 626c 6f62 0000 0008 180d d46b  modDblob.......k
-00003080: 2dfc c441 0000 0012 0062 006f 0075 006e  -..A.....b.o.u.n
-00003090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
-000030a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-000030b0: 636f 6d70 0000 0000 0002 e000 0000 0012  comp............
-000030c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
-000030d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
-000030e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
-000030f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
-00003100: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
-00003110: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
-00003120: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00003130: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00003140: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00003150: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00003160: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00003170: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00003180: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00003190: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-000031a0: 7b33 3934 2c20 3138 317d 2c20 7b37 3730  {394, 181}, {770
-000031b0: 2c20 3433 367d 7d09 0817 2531 3d49 606d  , 436}}...%1=I`m
-000031c0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-000031d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000031e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
-000031f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
-00003200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
-00003210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
-00003220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
-00003230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00003240: 0001 d866 0000 000f 0063 0075 0065 005f  ...f.....c.u.e._
-00003250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
-00003260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
-00003270: 0008 2402 2eb2 2800 c541 0000 000f 0063  ..$...(..A.....c
-00003280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
-00003290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-000032a0: 626c 6f62 0000 0008 2402 2eb2 2800 c541  blob....$...(..A
-000032b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
-000032c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
-000032d0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
-000032e0: 6000 0000 000f 0063 0075 0065 005f 006c  `......c.u.e._.l
-000032f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
-00003300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
-00003310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
-00003320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
-00003330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-00003340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-00003350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-00003360: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00003370: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00003380: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00003390: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-000033a0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-000033b0: 187b 7b36 3537 2c20 3237 307d 2c20 7b39  .{{657, 270}, {9
-000033c0: 3839 2c20 3433 367d 7d09 0817 2531 3d49  89, 436}}...%1=I
-000033d0: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
-000033e0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-000033f0: 0000 0000 0000 0000 9a00 0000 0800 6400  ..............d.
-00003400: 6100 7300 6800 5f00 6100 7000 706c 6731  a.s.h._.a.p.plg1
-00003410: 5363 6f6d 7000 0000 0000 0135 6200 0000  Scomp......5b...
-00003420: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
-00003430: 706d 6f44 4462 6c6f 6200 0000 087e 81a5  pmoDDblob....~..
-00003440: d736 fec4 4100 0000 0800 6400 6100 7300  .6..A.....d.a.s.
-00003450: 6800 5f00 6100 7000 706d 6f64 4462 6c6f  h._.a.p.pmodDblo
-00003460: 6200 0000 087e 81a5 d736 fec4 4100 0000  b....~...6..A...
-00003470: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
-00003480: 7070 6831 5363 6f6d 7000 0000 0000 0150  pph1Scomp......P
-00003490: 0000 0000 0800 6400 6100 7300 6800 5f00  ......d.a.s.h._.
-000034a0: 6100 7000 7076 5372 6e6c 6f6e 6700 0000  a.p.pvSrnlong...
-000034b0: 0100 0000 0f00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
-000034c0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000034d0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
-000034e0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-000034f0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00003500: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00003510: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00003520: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00003530: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00003540: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00003550: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-00003560: 7b7b 3635 372c 2032 3730 7d2c 207b 3938  {{657, 270}, {98
-00003570: 392c 2034 3336 7d7d 0908 1725 313d 4960  9, 436}}...%1=I`
-00003580: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
-00003590: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-000035a0: 0000 0000 0000 009a 0000 000f 0064 0061  .............d.a
-000035b0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
-000035c0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
-000035d0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
-000035e0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-000035f0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
-00003600: 0000 02c7 4300 0000 0f00 6400 6100 7400  ....C.....d.a.t.
-00003610: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
-00003620: 7300 6f00 7200 736d 6f44 4462 6c6f 6200  s.o.r.smoDDblob.
-00003630: 0000 080d 4b59 4254 01c5 4100 0000 0f00  ....KYBT..A.....
-00003640: 6400 6100 7400 6100 5f00 7000 7200 6f00  d.a.t.a._.p.r.o.
-00003650: 6300 6500 7300 7300 6f00 7200 736d 6f64  c.e.s.s.o.r.smod
-00003660: 4462 6c6f 6200 0000 08d8 72d8 a8f8 ffc4  Dblob.....r.....
-00003670: 4100 0000 0f00 6400 6100 7400 6100 5f00  A.....d.a.t.a._.
-00003680: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00003690: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-000036a0: 0390 0000 0000 0f00 6400 6100 7400 6100  ........d.a.t.a.
-000036b0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-000036c0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
-000036d0: 0100 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
-000036e0: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
-000036f0: 6300 7400 6f00 7200 7362 7773 7062 6c6f  c.t.o.r.sbwspblo
-00003700: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
-00003710: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-00003720: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-00003730: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-00003740: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00003750: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00003760: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-00003770: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00003780: 0908 095f 1017 7b7b 3230 2c20 3930 7d2c  ..._..{{20, 90},
-00003790: 207b 3130 3135 2c20 3736 377d 7d09 0817   {1015, 767}}...
-000037a0: 2531 3d49 606d 797a 7b7c 7d7e 9800 0000  %1=I`myz{|}~....
-000037b0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000037c0: 0000 0000 0000 0000 0000 0000 9900 0000  ................
-000037d0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
-000037e0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
-000037f0: 6f00 7200 7364 7363 6c62 6f6f 6c00 0000  o.r.sdsclbool...
-00003800: 0012 0066 0065 0061 0074 0075 0072 0065  ...f.e.a.t.u.r.e
-00003810: 005f 0065 0078 0074 0072 0061 0063 0074  ._.e.x.t.r.a.c.t
-00003820: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00003830: 0000 0013 573f 0000 0012 0066 0065 0061  ....W?.....f.e.a
-00003840: 0074 0075 0072 0065 005f 0065 0078 0074  .t.u.r.e._.e.x.t
-00003850: 0072 0061 0063 0074 006f 0072 0073 6c73  .r.a.c.t.o.r.sls
-00003860: 7643 626c 6f62 0000 02b8 6270 6c69 7374  vCblob....bplist
-00003870: 3030 da01 0203 0405 0607 0809 0a0b 0c0d  00..............
-00003880: 1a48 4948 4a4b 0c5f 1012 7669 6577 4f70  .HIHJK._..viewOp
-00003890: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
-000038a0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-000038b0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000038c0: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-000038d0: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-000038e0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
-000038f0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
-00003900: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
-00003910: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
-00003920: 09ab 0e17 1c21 252a 2f34 393e 43d4 0f10  .....!%*/49>C...
-00003930: 1112 1314 0c0c 5a69 6465 6e74 6966 6965  ......Zidentifie
-00003940: 7255 7769 6474 6859 6173 6365 6e64 696e  rUwidthYascendin
-00003950: 6757 7669 7369 626c 6554 6e61 6d65 1101  gWvisibleTname..
-00003960: a609 09d4 0f10 1112 1819 1a1a 5875 6269  ............Xubi
-00003970: 7175 6974 7910 2308 08d4 0f10 1112 1d1e  quity.#.........
-00003980: 1a0c 5c64 6174 654d 6f64 6966 6965 6410  ..\dateModified.
-00003990: b508 09d4 0f10 1112 221e 1a1a 5b64 6174  ........"...[dat
-000039a0: 6543 7265 6174 6564 0808 d40f 1011 1226  eCreated.......&
-000039b0: 271a 0c54 7369 7a65 1061 0809 d40f 1011  '..Tsize.a......
-000039c0: 122b 2c0c 0c54 6b69 6e64 1073 0909 d40f  .+,..Tkind.s....
-000039d0: 1011 1230 310c 1a55 6c61 6265 6c10 6409  ...01..Ulabel.d.
-000039e0: 08d4 0f10 1112 3536 0c1a 5776 6572 7369  ......56..Wversi
-000039f0: 6f6e 104b 0908 d40f 1011 123a 3b0c 1a58  on.K.......:;..X
-00003a00: 636f 6d6d 656e 7473 1101 2c09 08d4 0f10  comments..,.....
-00003a10: 1112 3f40 1a1a 5e64 6174 654c 6173 744f  ..?@..^dateLastO
-00003a20: 7065 6e65 6410 c808 08d4 0f10 1112 441e  pened.........D.
-00003a30: 1a1a 5964 6174 6541 6464 6564 0808 0823  ..YdateAdded...#
-00003a40: 0000 0000 0000 0000 2340 2800 0000 0000  ........#@(.....
-00003a50: 005c 6461 7465 4d6f 6469 6669 6564 2340  .\dateModified#@
-00003a60: 3000 0000 0000 0009 0008 001d 0032 0044  0............2.D
-00003a70: 004c 0060 0072 007b 008d 0098 00a1 00b4  .L.`.r.{........
-00003a80: 00b6 00b7 00c3 00cc 00d7 00dd 00e7 00ef  ................
-00003a90: 00f4 00f7 00f8 00f9 0102 010b 010d 010e  ................
-00003aa0: 010f 0118 0125 0127 0128 0129 0132 013e  .....%.'.(.).2.>
-00003ab0: 013f 0140 0149 014e 0150 0151 0152 015b  .?.@.I.N.P.Q.R.[
-00003ac0: 0160 0162 0163 0164 016d 0173 0175 0176  .`.b.c.d.m.s.u.v
-00003ad0: 0177 0180 0188 018a 018b 018c 0195 019e  .w..............
-00003ae0: 01a1 01a2 01a3 01ac 01bb 01bd 01be 01bf  ................
-00003af0: 01c8 01d2 01d3 01d4 01d5 01de 01e7 01f4  ................
-00003b00: 01fd 0000 0000 0000 0201 0000 0000 0000  ................
-00003b10: 004d 0000 0000 0000 0000 0000 0000 0000  .M..............
-00003b20: 01fe 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
-00003b30: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
-00003b40: 0063 0074 006f 0072 0073 6c73 7670 626c  .c.t.o.r.slsvpbl
-00003b50: 6f62 0000 029d 6270 6c69 7374 3030 da01  ob....bplist00..
-00003b60: 0203 0405 0607 0809 0a0b 0c0d 1c47 4847  .............GHG
-00003b70: 494a 0c5f 1012 7669 6577 4f70 7469 6f6e  IJ._..viewOption
-00003b80: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00003b90: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00003ba0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00003bb0: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
-00003bc0: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
-00003bd0: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
-00003be0: 6f6e 585a 736f 7274 436f 6c75 6d6e 5869  onXZsortColumnXi
-00003bf0: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
-00003c00: 6174 6976 6544 6174 6573 1001 09d9 0e0f  ativeDates......
-00003c10: 1011 1213 1415 1617 2025 292d 3237 3c41  ........ %)-27<A
-00003c20: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
-00003c30: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
-00003c40: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
-00003c50: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
-00003c60: 6457 7665 7273 696f 6e54 6e61 6d65 d418  dWversionTname..
-00003c70: 191a 1b1c 1d0c 1f57 7669 7369 626c 6555  .......WvisibleU
-00003c80: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
-00003c90: 696e 6465 7808 1101 2c09 1007 d418 191a  index...,.......
-00003ca0: 1b1c 221c 2408 10c8 0810 08d4 1819 1a1b  ..".$...........
-00003cb0: 0c27 1c0b 0910 b508 d418 191a 1b1c 271c  .'............'.
-00003cc0: 2c08 0810 02d4 1819 1a1b 0c2f 1c31 0910  ,........../.1..
-00003cd0: 6108 1003 d418 191a 1b1c 340c 3608 1064  a.........4.6..d
-00003ce0: 0910 05d4 1819 1a1b 0c39 0c3b 0910 7309  .........9.;..s.
-00003cf0: 1004 d418 191a 1b1c 3e0c 4008 104b 0910  ........>.@..K..
-00003d00: 06d4 1819 1a1b 0c43 0c45 0911 01a6 0910  .......C.E......
-00003d10: 0008 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
-00003d20: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00003d30: 6423 4030 0000 0000 0000 0900 0800 1d00  d#@0............
-00003d40: 3200 4400 4c00 6000 7200 7b00 8d00 9800  2.D.L.`.r.{.....
-00003d50: a100 b400 b600 b700 ca00 d300 e200 ef00  ................
-00003d60: fb01 0001 0601 0b01 1301 1801 2101 2901  ............!.).
-00003d70: 2f01 3901 3f01 4001 4301 4401 4601 4f01  /.9.?.@.C.D.F.O.
-00003d80: 5001 5201 5301 5501 5e01 5f01 6101 6201  P.R.S.U.^._.a.b.
-00003d90: 6b01 6c01 6d01 6f01 7801 7901 7b01 7c01  k.l.m.o.x.y.{.|.
-00003da0: 7e01 8701 8801 8a01 8b01 8d01 9601 9701  ~...............
-00003db0: 9901 9a01 9c01 a501 a601 a801 a901 ab01  ................
-00003dc0: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
-00003dd0: db01 e400 0000 0000 0002 0100 0000 0000  ................
-00003de0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
-00003df0: 0001 e500 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
-00003e00: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
-00003e10: 6100 6300 7400 6f00 7200 736d 6f44 4462  a.c.t.o.r.smoDDb
-00003e20: 6c6f 6200 0000 0866 04c9 1d50 01c5 4100  lob....f...P..A.
-00003e30: 0000 1200 6600 6500 6100 7400 7500 7200  ....f.e.a.t.u.r.
-00003e40: 6500 5f00 6500 7800 7400 7200 6100 6300  e._.e.x.t.r.a.c.
-00003e50: 7400 6f00 7200 736d 6f64 4462 6c6f 6200  t.o.r.smodDblob.
-00003e60: 0000 082d e1ee 5c25 fec4 4100 0000 1200  ...-..\%..A.....
-00003e70: 6600 6500 6100 7400 7500 7200 6500 5f00  f.e.a.t.u.r.e._.
-00003e80: 6500 7800 7400 7200 6100 6300 7400 6f00  e.x.t.r.a.c.t.o.
-00003e90: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-00003ea0: 15d0 0000 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
-00003eb0: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
-00003ec0: 6100 6300 7400 6f00 7200 7376 5372 6e6c  a.c.t.o.r.svSrnl
-00003ed0: 6f6e 6700 0000 0100 0000 0900 6c00 6100  ong.........l.a.
-00003ee0: 6200 6500 6c00 6c00 6900 6e00 6762 7773  b.e.l.l.i.n.gbws
-00003ef0: 7062 6c6f 6200 0000 c662 706c 6973 7430  pblob....bplist0
-00003f00: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00003f10: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00003f20: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00003f30: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00003f40: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00003f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00003f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00003f70: 6172 0808 0908 095f 1015 7b7b 302c 2030  ar....._..{{0, 0
-00003f80: 7d2c 207b 3134 3430 2c20 3837 377d 7d09  }, {1440, 877}}.
-00003f90: 0817 2531 3d49 606d 797a 7b7c 7d7e 9600  ..%1=I`myz{|}~..
-00003fa0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00003fb0: 0000 0000 0000 0000 0000 0000 0000 9700  ................
-00003fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00003fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00003fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00002000: 0000 0000 0000 0006 0000 0002 0000 0004  ................
+00002010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
+00002020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
+00002030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
+00002040: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
+00002050: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
+00002060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00002070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00002080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00002090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000020a0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+000020b0: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+000020c0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000020d0: 1001 09d9 0c0d 0e0f 1011 1213 1415 1e23  ...............#
+000020e0: 272b 3035 3a3f 5863 6f6d 6d65 6e74 735e  '+05:?Xcomments^
+000020f0: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
+00002100: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
+00002110: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
+00002120: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
+00002130: 6e61 6d65 d416 1718 191a 1b0a 1d55 696e  name.........Uin
+00002140: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
+00002150: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
+00002160: 0908 d416 1718 191f 201d 1d10 0810 c808  ........ .......
+00002170: 08d4 1617 1819 0924 1d0a 10b5 0809 d416  .......$........
+00002180: 1718 1928 241d 1d10 0208 08d4 1617 1819  ...($...........
+00002190: 2c2d 1d0a 1003 1061 0809 d416 1718 1931  ,-.....a.......1
+000021a0: 320a 1d10 0510 6409 08d4 1617 1819 3637  2.....d.......67
+000021b0: 0a0a 1004 1073 0909 d416 1718 193b 3c0a  .....s.......;<.
+000021c0: 1d10 0610 4b09 08d4 1617 1819 4041 0a0a  ....K.......@A..
+000021d0: 1000 1101 c709 0908 2340 2800 0000 0000  ........#@(.....
+000021e0: 0054 6e61 6d65 2340 3000 0000 0000 0009  .Tname#@0.......
+000021f0: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+00002200: 0079 008c 008e 008f 00a2 00ab 00ba 00c7  .y..............
+00002210: 00d3 00d8 00de 00e3 00eb 00f0 00f9 00ff  ................
+00002220: 0105 010f 0117 0119 011c 011d 011e 0127  ...............'
+00002230: 0129 012b 012c 012d 0136 0138 0139 013a  .).+.,.-.6.8.9.:
+00002240: 0143 0145 0146 0147 0150 0152 0154 0155  .C.E.F.G.P.R.T.U
+00002250: 0156 015f 0161 0163 0164 0165 016e 0170  .V._.a.c.d.e.n.p
+00002260: 0172 0173 0174 017d 017f 0181 0182 0183  .r.s.t.}........
+00002270: 018c 018e 0191 0192 0193 0194 019d 01a2  ................
+00002280: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
+00002290: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+000022a0: 01ac 0000 0005 0000 0012 0066 0065 0061  ...........f.e.a
+000022b0: 0074 0075 0072 0065 005f 0065 0078 0074  .t.u.r.e._.e.x.t
+000022c0: 0072 0061 0063 0074 006f 0072 0073 6c73  .r.a.c.t.o.r.sls
+000022d0: 7643 626c 6f62 0000 02b8 6270 6c69 7374  vCblob....bplist
+000022e0: 3030 da01 0203 0405 0607 0809 0a0b 0c0d  00..............
+000022f0: 1848 4948 4a0c 4c58 6963 6f6e 5369 7a65  .HIHJ.LXiconSize
+00002300: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00002310: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00002320: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
+00002330: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
+00002340: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
+00002350: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
+00002360: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
+00002370: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
+00002380: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
+00002390: 3000 0000 0000 0009 ab0e 171c 2125 2a2f  0...........!%*/
+000023a0: 3439 3e43 d40f 1011 120c 140c 1657 7669  49>C.........Wvi
+000023b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+000023c0: 6e64 696e 675a 6964 656e 7469 6669 6572  ndingZidentifier
+000023d0: 0911 01c7 0954 6e61 6d65 d40f 1011 1218  .....Tname......
+000023e0: 1918 1b08 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
+000023f0: d40f 1011 120c 1e18 2009 10b5 085c 6461  ........ ....\da
+00002400: 7465 4d6f 6469 6669 6564 d40f 1011 1218  teModified......
+00002410: 1e18 2408 085b 6461 7465 4372 6561 7465  ..$..[dateCreate
+00002420: 64d4 0f10 1112 0c27 1829 0910 6108 5473  d......'.)..a.Ts
+00002430: 697a 65d4 0f10 1112 0c2c 0c2e 0910 7309  ize......,....s.
+00002440: 546b 696e 64d4 0f10 1112 1831 0c33 0810  Tkind......1.3..
+00002450: 6409 556c 6162 656c d40f 1011 1218 360c  d.Ulabel......6.
+00002460: 3808 104b 0957 7665 7273 696f 6ed4 0f10  8..K.Wversion...
+00002470: 1112 183b 0c3d 0811 012c 0958 636f 6d6d  ...;.=...,.Xcomm
+00002480: 656e 7473 d40f 1011 1218 4018 4208 10c8  ents......@.B...
+00002490: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
+000024a0: d40f 1011 1218 1e18 4608 0859 6461 7465  ........F..Ydate
+000024b0: 4164 6465 6408 2300 0000 0000 0000 0023  Added.#........#
+000024c0: 4028 0000 0000 0000 5c64 6174 654d 6f64  @(......\dateMod
+000024d0: 6966 6965 6409 1001 0008 001d 0026 0038  ified........&.8
+000024e0: 0040 0054 0066 006f 0081 008c 009f 00b4  .@.T.f.o........
+000024f0: 00bd 00be 00ca 00d3 00db 00e1 00eb 00f6  ................
+00002500: 00f7 00fa 00fb 0100 0109 010a 010c 010d  ................
+00002510: 0116 011f 0120 0122 0123 0130 0139 013a  ..... .".#.0.9.:
+00002520: 013b 0147 0150 0151 0153 0154 0159 0162  .;.G.P.Q.S.T.Y.b
+00002530: 0163 0165 0166 016b 0174 0175 0177 0178  .c.e.f.k.t.u.w.x
+00002540: 017e 0187 0188 018a 018b 0193 019c 019d  .~..............
+00002550: 01a0 01a1 01aa 01b3 01b4 01b6 01b7 01c6  ................
+00002560: 01cf 01d0 01d1 01db 01dc 01e5 01ee 01fb  ................
+00002570: 01fc 0000 0000 0000 0201 0000 0000 0000  ................
+00002580: 004d 0000 0000 0000 0000 0000 0000 0000  .M..............
+00002590: 01fe 0000 0900 0000 0900 7200 6f00 6900  ..........r.o.i.
+000025a0: 5f00 7400 6f00 6f00 6c00 736c 7376 7062  _.t.o.o.l.slsvpb
+000025b0: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
+000025c0: 0102 0304 0506 0708 090a 0b1d 4546 470a  ............EFG.
+000025d0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000025e0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+000025f0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00002600: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00002610: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00002620: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+00002630: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00002640: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
+00002650: 151e 2327 2b30 353a 3f58 636f 6d6d 656e  ..#'+05:?Xcommen
+00002660: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+00002670: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
+00002680: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00002690: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+000026a0: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
+000026b0: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
+000026c0: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
+000026d0: 1101 2c09 08d4 1617 1819 1f20 1d1d 1008  ..,........ ....
+000026e0: 10c8 0808 d416 1718 1909 241d 0a10 b508  ..........$.....
+000026f0: 09d4 1617 1819 2824 1d1d 1002 0808 d416  ......($........
+00002700: 1718 192c 2d1d 0a10 0310 6108 09d4 1617  ...,-.....a.....
+00002710: 1819 3132 0a1d 1005 1064 0908 d416 1718  ..12.....d......
+00002720: 1936 370a 0a10 0410 7309 09d4 1617 1819  .67.....s.......
+00002730: 3b3c 0a1d 1006 104b 0908 d416 1718 1940  ;<.....K.......@
+00002740: 410a 0a10 0011 01c7 0909 0823 4028 0000  A..........#@(..
+00002750: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
+00002760: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
+00002770: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
+00002780: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
+00002790: f900 ff01 0501 0f01 1701 1901 1c01 1d01  ................
+000027a0: 1e01 2701 2901 2b01 2c01 2d01 3601 3801  ..'.).+.,.-.6.8.
+000027b0: 3901 3a01 4301 4501 4601 4701 5001 5201  9.:.C.E.F.G.P.R.
+000027c0: 5401 5501 5601 5f01 6101 6301 6401 6501  T.U.V._.a.c.d.e.
+000027d0: 6e01 7001 7201 7301 7401 7d01 7f01 8101  n.p.r.s.t.}.....
+000027e0: 8201 8301 8c01 8e01 9101 9201 9301 9401  ................
+000027f0: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
+00002800: 0000 0000 0000 000e 0000 0000 0000 280b  ..............(.
+00002810: 0000 0045 0000 300c 0000 100c 0000 400c  ...E..0.......@.
+00002820: 0000 500c 0000 600c 0000 700c 0000 800c  ..P...`...p.....
+00002830: 0000 900c 0000 040a 0000 200b 0000 a00c  .......... .....
+00002840: 0000 b00c 0000 0000 0000 0000 0000 0000  ................
+00002850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000028c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000028d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000028e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000028f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00002c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00002c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00002c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00002c50: 0100 0002 0000 0000 0000 0000 0100 0008  ................
+00002c60: 0000 0000 0000 0000 0000 0000 0100 00c0  ................
+00002c70: 0000 0000 0000 0000 0100 0100 0000 0000  ................
+00002c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
+00002c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
+00002ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
+00002cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
+00002cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
+00002cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
+00002ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
+00002cf0: 0061 6265 6c54 6b69 6e64 5776 6572 7369  .abelTkindWversi
+00002d00: 6f6e 546e 616d 65d4 1617 1819 1a09 1c1d  onTname.........
+00002d10: 5776 6973 6962 6c65 5961 7363 656e 6469  WvisibleYascendi
+00002d20: 6e67 5577 6964 7468 5569 6e64 6578 0809  ngUwidthUindex..
+00002d30: 1101 2c10 07d4 1617 1819 1a1a 2122 0808  ..,.........!"..
+00002d40: 10c8 1008 d416 1718 1909 1a26 2709 0810  ...........&'...
+00002d50: b510 01d4 1617 1819 1a1a 262b 0808 1002  ..........&+....
+00002d60: d416 1718 1909 1a2f 3009 0810 6110 03d4  ......./0...a...
+00002d70: 1617 1819 1a09 3435 0809 1064 1005 d416  ......45...d....
+00002d80: 1718 1909 0939 3a09 0910 7310 04d4 1617  .....9:...s.....
+00002d90: 1819 1a09 3e3f 0809 104b 1006 d416 1718  ....>?...K......
+00002da0: 1909 0943 4409 0911 01c7 1000 0823 4028  ...CD........#@(
+00002db0: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+00002dc0: 0000 0000 0008 0019 002c 003e 0046 005a  .........,.>.F.Z
+00002dd0: 0063 006e 0077 008c 008d 008e 00a1 00aa  .c.n.w..........
+00002de0: 00b9 00c6 00d2 00d7 00dd 00e2 00ea 00ef  ................
+00002df0: 00f8 0100 010a 0110 0116 0117 0118 011b  ................
+00002e00: 011d 0126 0127 0128 012a 012c 0135 0136  ...&.'.(.*.,.5.6
+00002e10: 0137 0139 013b 0144 0145 0146 0148 0151  .7.9.;.D.E.F.H.Q
+00002e20: 0152 0153 0155 0157 0160 0161 0162 0164  .R.S.U.W.`.a.b.d
+00002e30: 0166 016f 0170 0171 0173 0175 017e 017f  .f.o.p.q.s.u.~..
+00002e40: 0180 0182 0184 018d 018e 018f 0192 0194  ................
+00002e50: 0195 019e 01a3 0000 0000 0000 0201 0000  ................
+00002e60: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+00002e70: 0000 0000 01ac 0000 000c 0075 006e 0073  ...........u.n.s
+00002e80: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00002e90: 0064 6d6f 4444 626c 6f62 0000 0008 6269  .dmoDDblob....bi
+00002ea0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
+00002eb0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00002ec0: 0064 6d6f 6444 626c 6f62 0000 0008 6269  .dmodDblob....bi
+00002ed0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
+00002ee0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00002ef0: 0064 7068 3153 636f 6d70 0000 0000 0007  .dph1Scomp......
+00002f00: 9000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+00002f10: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
+00002f20: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
+00002f30: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
+00002f40: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00002f50: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00002f60: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00002f70: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00002f80: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00002f90: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00002fa0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00002fb0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00002fc0: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
+00002fd0: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
+00002fe0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+00002ff0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+00003000: 0000 0000 0000 0000 0000 0010 0000 0005  ................
+00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
+00003020: 6d70 0000 0000 0003 cc2d 0000 0005 0075  mp.......-.....u
+00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
+00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
+00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
+00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000030a0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+000030b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000030c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000030d0: 1001 09ab 0c15 1d22 262b 3035 3a3f 44d4  ......."&+05:?D.
+000030e0: 0d0e 0f10 0a0a 1314 5776 6973 6962 6c65  ........Wvisible
+000030f0: 5961 7363 656e 6469 6e67 5577 6964 7468  YascendingUwidth
+00003100: 5a69 6465 6e74 6966 6965 7209 0911 0204  Zidentifier.....
+00003110: 546e 616d 65d4 1617 1810 191a 191c 5776  Tname.........Wv
+00003120: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00003130: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
+00003140: 6974 79d4 0d0e 0f10 0a19 2021 0908 10b5  ity....... !....
+00003150: 5c64 6174 654d 6f64 6966 6965 64d4 0d0e  \dateModified...
+00003160: 0f10 1919 2025 0808 5b64 6174 6543 7265  .... %..[dateCre
+00003170: 6174 6564 d40d 0e0f 100a 1929 2a09 0810  ated.......)*...
+00003180: 6154 7369 7a65 d40d 0e0f 100a 0a2e 2f09  aTsize......../.
+00003190: 0910 7354 6b69 6e64 d40d 0e0f 1019 0a33  ..sTkind.......3
+000031a0: 3408 0910 6455 6c61 6265 6cd4 0d0e 0f10  4...dUlabel.....
+000031b0: 190a 3839 0809 104b 5776 6572 7369 6f6e  ..89...KWversion
+000031c0: d40d 0e0f 1019 0a3d 3e08 0911 012c 5863  .......=>....,Xc
+000031d0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1919 4243  omments.......BC
+000031e0: 0808 10c8 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
+000031f0: 6e65 64d4 1617 1810 1920 1947 0808 5964  ned...... .G..Yd
+00003200: 6174 6541 6464 6564 0823 4028 0000 0000  ateAdded.#@(....
+00003210: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
+00003220: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+00003230: 7000 8300 8c00 8e00 8f00 9b00 a400 ac00  p...............
+00003240: b600 bc00 c700 c800 c900 cc00 d100 da00  ................
+00003250: e200 e800 f200 f300 f500 f600 ff01 0801  ................
+00003260: 0901 0a01 0c01 1901 2201 2301 2401 3001  ........".#.$.0.
+00003270: 3901 3a01 3b01 3d01 4201 4b01 4c01 4d01  9.:.;.=.B.K.L.M.
+00003280: 4f01 5401 5d01 5e01 5f01 6101 6701 7001  O.T.].^._.a.g.p.
+00003290: 7101 7201 7401 7c01 8501 8601 8701 8a01  q.r.t.|.........
+000032a0: 9301 9c01 9d01 9e01 a001 af01 b801 b901  ................
+000032b0: ba01 c401 c501 ce01 d301 d400 0000 0000  ................
+000032c0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000032d0: 0000 0000 0000 0000 0001 dd00 0000 0500  ................
+000032e0: 7500 7400 6900 6c00 736c 7376 7062 6c6f  u.t.i.l.slsvpblo
+000032f0: 6200 0002 5e62 706c 6973 7430 30d8 0102  b...^bplist00...
+00003300: 0304 0506 0708 090a 0b1d 4546 0a48 5f10  ..........EF.H_.
+00003310: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00003320: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+00003330: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00003340: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00003350: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
+00003360: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
+00003370: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
+00003380: 6510 0109 d90c 0d0e 0f10 1112 1314 151e  e...............
+00003390: 2328 2d32 373c 4158 636f 6d6d 656e 7473  #(-27<AXcomments
+000033a0: 5e64 6174 654c 6173 744f 7065 6e65 645b  ^dateLastOpened[
+000033b0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+000033c0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+000033d0: 696f 6e54 6e61 6d65 5c64 6174 654d 6f64  ionTname\dateMod
+000033e0: 6966 6965 64d4 1617 1819 1a0a 1c1d 5569  ified.........Ui
+000033f0: 6e64 6578 5961 7363 656e 6469 6e67 5577  ndexYascendingUw
+00003400: 6964 7468 5776 6973 6962 6c65 1007 0911  idthWvisible....
+00003410: 012c 08d4 1617 1819 1f1d 211d 1008 0810  .,........!.....
+00003420: c808 d416 1718 1924 1d26 1d10 0208 10b5  .......$.&......
+00003430: 08d4 1617 1819 291d 2b0a 1003 0810 6109  ......).+.....a.
+00003440: d416 1718 192e 0a30 1d10 0509 1064 08d4  .......0.....d..
+00003450: 1617 1819 330a 350a 1004 0910 7309 d416  ....3.5.....s...
+00003460: 1718 1938 0a3a 1d10 0609 104b 08d4 1617  ...8.:.....K....
+00003470: 1819 3d0a 3f0a 1000 0911 0204 09d4 1617  ..=.?...........
+00003480: 1819 091d 260a 0809 0823 4028 0000 0000  ....&....#@(....
+00003490: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
+000034a0: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+000034b0: 7000 8300 8c00 8e00 8f00 a200 ab00 ba00  p...............
+000034c0: c600 cb00 d100 d600 de00 e300 f000 f900  ................
+000034d0: ff01 0901 0f01 1701 1901 1a01 1d01 1e01  ................
+000034e0: 2701 2901 2a01 2c01 2d01 3601 3801 3901  '.).*.,.-.6.8.9.
+000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
+00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
+00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
+00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
+00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
+00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
+00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
+00003560: 736d 6f44 4462 6c6f 6200 0000 08e5 d1d7  smoDDblob.......
+00003570: 0ac9 04c5 4100 0000 0500 7500 7400 6900  ....A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08e5  l.smodDblob.....
+00003590: d1d7 0ac9 04c5 4100 0000 0500 7500 7400  ......A.....u.t.
+000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
+000035b0: 0000 0490 0000 0000 0500 7500 7400 6900  ..........u.t.i.
+000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
+000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
+000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+000035f0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
+00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00003630: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00003640: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00003650: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00003660: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00003670: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00003680: 7b7b 3233 322c 2031 3931 7d2c 207b 3133  {{232, 191}, {13
+00003690: 3032 2c20 3731 347d 7d09 0817 2531 3d49  02, 714}}...%1=I
+000036a0: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+000036b0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+000036c0: 0000 0000 0000 0000 9b00 0000 1000 7600  ..............v.
+000036d0: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
+000036e0: 6300 6500 7300 7300 6f00 7200 7364 7363  c.e.s.s.o.r.sdsc
+000036f0: 6c62 6f6f 6c00 0000 0010 0076 0069 0064  lbool......v.i.d
+00003700: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
+00003710: 0073 0073 006f 0072 0073 6c67 3153 636f  .s.s.o.r.slg1Sco
+00003720: 6d70 0000 0000 0003 85ef 0000 0010 0076  mp.............v
+00003730: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
+00003740: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
+00003750: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
+00003760: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
+00003770: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
+00003780: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00003790: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+000037a0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+000037b0: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
+000037c0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+000037d0: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
+000037e0: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
+000037f0: ab0c 151d 2226 2b30 353a 3f44 d40d 0e0f  ...."&+05:?D....
+00003800: 1011 120a 0a5a 6964 656e 7469 6669 6572  .....Zidentifier
+00003810: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00003820: 5776 6973 6962 6c65 546e 616d 6511 01c7  WvisibleTname...
+00003830: 0909 d416 1718 0d19 1a19 1c57 7669 7369  ...........Wvisi
+00003840: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+00003850: 696e 6708 1023 0858 7562 6971 7569 7479  ing..#.Xubiquity
+00003860: d40d 0e0f 101e 1f19 0a5c 6461 7465 4d6f  .........\dateMo
+00003870: 6469 6669 6564 10b5 0809 d40d 0e0f 1023  dified.........#
+00003880: 1f19 195b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
+00003890: 08d4 0d0e 0f10 2728 190a 5473 697a 6510  ......'(..Tsize.
+000038a0: 6108 09d4 0d0e 0f10 2c2d 0a0a 546b 696e  a.......,-..Tkin
+000038b0: 6410 7309 09d4 0d0e 0f10 3132 0a19 556c  d.s.......12..Ul
+000038c0: 6162 656c 1064 0908 d40d 0e0f 1036 370a  abel.d.......67.
+000038d0: 1957 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
+000038e0: 0f10 3b3c 0a19 5863 6f6d 6d65 6e74 7311  ..;<..Xcomments.
+000038f0: 012c 0908 d40d 0e0f 1040 4119 195e 6461  .,.......@A..^da
+00003900: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
+00003910: d416 1718 0d19 1f19 4708 0859 6461 7465  ........G..Ydate
+00003920: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
+00003930: 6e61 6d65 0910 0100 0800 1900 2200 3400  name........".4.
+00003940: 3c00 5000 5900 6400 7700 8c00 9500 9600  <.P.Y.d.w.......
+00003950: a200 ab00 b600 bc00 c600 ce00 d300 d600  ................
+00003960: d700 d800 e100 e900 ef00 f900 fa00 fc00  ................
+00003970: fd01 0601 0f01 1c01 1e01 1f01 2001 2901  ............ .).
+00003980: 3501 3601 3701 4001 4501 4701 4801 4901  5.6.7.@.E.G.H.I.
+00003990: 5201 5701 5901 5a01 5b01 6401 6a01 6c01  R.W.Y.Z.[.d.j.l.
+000039a0: 6d01 6e01 7701 7f01 8101 8201 8301 8c01  m.n.w...........
+000039b0: 9501 9801 9901 9a01 a301 b201 b401 b501  ................
+000039c0: b601 bf01 c001 c101 cb01 cc01 d501 da01  ................
+000039d0: db00 0000 0000 0002 0100 0000 0000 0000  ................
+000039e0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
+000039f0: dd00 0000 1000 7600 6900 6400 6500 6f00  ......v.i.d.e.o.
+00003a00: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00003a10: 6f00 7200 736c 7376 7062 6c6f 6200 0002  o.r.slsvpblob...
+00003a20: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
+00003a30: 0708 090a 0b1a 4647 0a44 5869 636f 6e53  ......FG.DXiconS
+00003a40: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
+00003a50: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00003a60: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00003a70: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
+00003a80: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
+00003a90: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
+00003aa0: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
+00003ab0: 0000 0000 0000 09d9 0c0d 0e0f 1011 1213  ................
+00003ac0: 1415 1e23 282d 3237 3c41 5863 6f6d 6d65  ...#(-27<AXcomme
+00003ad0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+00003ae0: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00003af0: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00003b00: 6572 7369 6f6e 546e 616d 655c 6461 7465  ersionTname\date
+00003b10: 4d6f 6469 6669 6564 d416 1718 191a 1b0a  Modified........
+00003b20: 1d57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00003b30: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
+00003b40: 1101 2c09 1007 d416 1718 191a 201a 2208  ..,......... .".
+00003b50: 10c8 0810 08d4 1617 1819 1a25 1a27 0810  ...........%.'..
+00003b60: b508 1002 d416 1718 190a 2a1a 2c09 1061  ..........*.,..a
+00003b70: 0810 03d4 1617 1819 1a2f 0a31 0810 6409  ........./.1..d.
+00003b80: 1005 d416 1718 190a 340a 3609 1073 0910  ........4.6..s..
+00003b90: 04d4 1617 1819 1a39 0a3b 0810 4b09 1006  .......9.;..K...
+00003ba0: d416 1718 190a 3e0a 4009 1101 c709 1000  ......>.@.......
+00003bb0: d416 1718 190a 251a 4409 0810 0108 2340  ......%.D.....#@
+00003bc0: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
+00003bd0: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
+00003be0: 8c00 9500 9600 a900 b200 c100 cd00 d200  ................
+00003bf0: d800 dd00 e500 ea00 f701 0001 0801 0e01  ................
+00003c00: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
+00003c10: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
+00003c20: 4c01 4d01 4f01 5001 5201 5b01 5c01 5e01  L.M.O.P.R.[.\.^.
+00003c30: 5f01 6101 6a01 6b01 6d01 6e01 7001 7901  _.a.j.k.m.n.p.y.
+00003c40: 7a01 7c01 7d01 7f01 8801 8901 8c01 8d01  z.|.}...........
+00003c50: 8f01 9801 9901 9a01 9c01 9d01 a601 ab00  ................
+00003c60: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
+00003c70: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
+00003c80: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
+00003c90: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+00003ca0: 7200 736d 6f44 4462 6c6f 6200 0000 0858  r.smoDDblob....X
+00003cb0: 3fde 4cbd 04c5 4100 0000 1000 7600 6900  ?.L...A.....v.i.
+00003cc0: 6400 6500 6f00 5f00 7000 7200 6f00 6300  d.e.o._.p.r.o.c.
+00003cd0: 6500 7300 7300 6f00 7200 736d 6f64 4462  e.s.s.o.r.smodDb
+00003ce0: 6c6f 6200 0000 0858 3fde 4cbd 04c5 4100  lob....X?.L...A.
+00003cf0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
+00003d00: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+00003d10: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
+00003d20: 0460 0000 0000 1000 7600 6900 6400 6500  .`......v.i.d.e.
+00003d30: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
+00003d40: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
+00003d50: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004000: 0000 0000 0000 0000 0000 0016 0000 0009  ................
-00004010: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-00004020: 0067 6c73 7670 626c 6f62 0000 025e 6270  .glsvpblob...^bp
-00004030: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
-00004040: 0a0b 1a46 470a 2758 6963 6f6e 5369 7a65  ...FG.'XiconSize
-00004050: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00004060: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00004070: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
-00004080: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
-00004090: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
-000040a0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
-000040b0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
-000040c0: 0000 0009 d90c 0d0e 0f10 1112 1314 151e  ................
-000040d0: 2328 2c31 363b 4058 636f 6d6d 656e 7473  #(,16;@Xcomments
-000040e0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
-000040f0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
-00004100: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
-00004110: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
-00004120: 546e 616d 65d4 1617 1819 1a0a 1c1d 5776  Tname.........Wv
-00004130: 6973 6962 6c65 5961 7363 656e 6469 6e67  isibleYascending
-00004140: 5577 6964 7468 5569 6e64 6578 0809 1101  UwidthUindex....
-00004150: 2c10 07d4 1617 1819 1a1a 2122 0808 10c8  ,.........!"....
-00004160: 1008 d416 1718 190a 1a26 2709 0810 b510  .........&'.....
-00004170: 01d4 1617 1819 1a1a 262b 0808 1002 d416  ........&+......
-00004180: 1718 190a 1a2f 3009 0810 6110 03d4 1617  ...../0...a.....
-00004190: 1819 1a0a 3435 0809 1064 1005 d416 1718  ....45...d......
-000041a0: 190a 0a39 3a09 0910 7310 04d4 1617 1819  ...9:...s.......
-000041b0: 1a0a 3e3f 0809 104b 1006 d416 1718 190a  ..>?...K........
-000041c0: 0a43 4409 0911 0251 1000 0823 4028 0000  .CD....Q...#@(..
-000041d0: 0000 0000 546e 616d 6509 0008 0019 0022  ....Tname......"
-000041e0: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
-000041f0: 0096 00a9 00b2 00c1 00ce 00da 00df 00e5  ................
-00004200: 00ea 00f2 00f7 0100 0108 0112 0118 011e  ................
-00004210: 011f 0120 0123 0125 012e 012f 0130 0132  ... .#.%.../.0.2
-00004220: 0134 013d 013e 013f 0141 0143 014c 014d  .4.=.>.?.A.C.L.M
-00004230: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
-00004240: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
-00004250: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
-00004260: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
-00004270: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
-00004280: 0000 0000 0000 0000 0000 01ac 0000 0009  ................
-00004290: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-000042a0: 0067 6d6f 4444 626c 6f62 0000 0008 7246  .gmoDDblob....rF
-000042b0: 2c98 4a00 c541 0000 0009 006c 0061 0062  ,.J..A.....l.a.b
-000042c0: 0065 006c 006c 0069 006e 0067 6d6f 6444  .e.l.l.i.n.gmodD
-000042d0: 626c 6f62 0000 0008 cb5b 96d0 97fe c441  blob.....[.....A
-000042e0: 0000 0009 006c 0061 0062 0065 006c 006c  .....l.a.b.e.l.l
-000042f0: 0069 006e 0067 7068 3153 636f 6d70 0000  .i.n.gph1Scomp..
-00004300: 0000 0001 c000 0000 0009 006c 0061 0062  ...........l.a.b
-00004310: 0065 006c 006c 0069 006e 0067 7653 726e  .e.l.l.i.n.gvSrn
-00004320: 6c6f 6e67 0000 0001 0000 0006 006d 0069  long.........m.i
-00004330: 0078 0069 006e 0073 6277 7370 626c 6f62  .x.i.n.sbwspblob
-00004340: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00004350: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00004360: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00004370: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00004380: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00004390: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-000043a0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-000043b0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-000043c0: 0809 5f10 187b 7b33 3934 2c20 3138 317d  .._..{{394, 181}
-000043d0: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-000043e0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-000043f0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00004400: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-00004410: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
-00004420: 5363 6f6d 7000 0000 0000 0965 c500 0000  Scomp......e....
-00004430: 0600 6d00 6900 7800 6900 6e00 736d 6f44  ..m.i.x.i.n.smoD
-00004440: 4462 6c6f 6200 0000 0892 2cee 1963 01c5  Dblob.....,..c..
-00004450: 4100 0000 0600 6d00 6900 7800 6900 6e00  A.....m.i.x.i.n.
-00004460: 736d 6f64 4462 6c6f 6200 0000 0892 2cee  smodDblob.....,.
-00004470: 1963 01c5 4100 0000 0600 6d00 6900 7800  .c..A.....m.i.x.
-00004480: 6900 6e00 7370 6831 5363 6f6d 7000 0000  i.n.sph1Scomp...
-00004490: 0000 0a40 0000 0000 0600 6d00 6900 7800  ...@......m.i.x.
-000044a0: 6900 6e00 7376 5372 6e6c 6f6e 6700 0000  i.n.svSrnlong...
-000044b0: 0100 0000 0500 6d00 6f00 6400 6500 6c62  ......m.o.d.e.lb
-000044c0: 7773 7062 6c6f 6200 0000 c662 706c 6973  wspblob....bplis
-000044d0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
-000044e0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-000044f0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
-00004500: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00004510: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00004520: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00004530: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00004540: 6562 6172 0808 0908 095f 1015 7b7b 302c  ebar....._..{{0,
-00004550: 2030 7d2c 207b 3134 3430 2c20 3837 377d   0}, {1440, 877}
-00004560: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00004570: 9600 0000 0000 0001 0100 0000 0000 0000  ................
-00004580: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00004590: 9700 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
-000045a0: 6731 5363 6f6d 7000 0000 0000 0114 7400  g1Scomp.......t.
-000045b0: 0000 0500 6d00 6f00 6400 6500 6c6c 7376  ....m.o.d.e.llsv
-000045c0: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
-000045d0: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
-000045e0: 4b0a 5f10 1276 6965 774f 7074 696f 6e73  K._..viewOptions
-000045f0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00004600: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00004610: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00004620: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00004630: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-00004640: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-00004650: 4461 7465 7310 0109 ab0c 151d 2226 2b30  Dates......."&+0
-00004660: 353a 3f44 d40d 0e0f 100a 0a13 1457 7669  5:?D.........Wvi
-00004670: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00004680: 7769 6474 685a 6964 656e 7469 6669 6572  widthZidentifier
-00004690: 0909 1102 5154 6e61 6d65 d416 1718 1019  ....QTname......
-000046a0: 1a19 1c57 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
-000046b0: 6859 6173 6365 6e64 696e 6708 1023 0858  hYascending..#.X
-000046c0: 7562 6971 7569 7479 d40d 0e0f 100a 1920  ubiquity....... 
-000046d0: 2109 0810 b55c 6461 7465 4d6f 6469 6669  !....\dateModifi
-000046e0: 6564 d40d 0e0f 1019 1920 2508 085b 6461  ed....... %..[da
-000046f0: 7465 4372 6561 7465 64d4 0d0e 0f10 0a19  teCreated.......
-00004700: 292a 0908 1061 5473 697a 65d4 0d0e 0f10  )*...aTsize.....
-00004710: 0a0a 2e2f 0909 1073 546b 696e 64d4 0d0e  .../...sTkind...
-00004720: 0f10 190a 3334 0809 1064 556c 6162 656c  ....34...dUlabel
-00004730: d40d 0e0f 1019 0a38 3908 0910 4b57 7665  .......89...KWve
-00004740: 7273 696f 6ed4 0d0e 0f10 190a 3d3e 0809  rsion.......=>..
-00004750: 1101 2c58 636f 6d6d 656e 7473 d40d 0e0f  ..,Xcomments....
-00004760: 1019 1942 4308 0810 c85e 6461 7465 4c61  ...BC....^dateLa
-00004770: 7374 4f70 656e 6564 d416 1718 1019 2019  stOpened...... .
-00004780: 4708 0859 6461 7465 4164 6465 6408 2340  G..YdateAdded.#@
-00004790: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
-000047a0: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
-000047b0: 005c 0065 0070 0079 008c 008e 008f 009b  .\.e.p.y........
-000047c0: 00a4 00ac 00b6 00bc 00c7 00c8 00c9 00cc  ................
-000047d0: 00d1 00da 00e2 00e8 00f2 00f3 00f5 00f6  ................
-000047e0: 00ff 0108 0109 010a 010c 0119 0122 0123  .............".#
-000047f0: 0124 0130 0139 013a 013b 013d 0142 014b  .$.0.9.:.;.=.B.K
-00004800: 014c 014d 014f 0154 015d 015e 015f 0161  .L.M.O.T.].^._.a
-00004810: 0167 0170 0171 0172 0174 017c 0185 0186  .g.p.q.r.t.|....
-00004820: 0187 018a 0193 019c 019d 019e 01a0 01af  ................
-00004830: 01b8 01b9 01ba 01c4 01c5 01ce 01d3 01dc  ................
-00004840: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
-00004850: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
-00004860: 0000 0005 006d 006f 0064 0065 006c 6c73  .....m.o.d.e.lls
-00004870: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
-00004880: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
-00004890: 4647 0a5f 1012 7669 6577 4f70 7469 6f6e  FG._..viewOption
-000048a0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-000048b0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-000048c0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-000048d0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-000048e0: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-000048f0: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-00004900: 6544 6174 6573 1001 09d9 0c0d 0e0f 1011  eDates..........
-00004910: 1213 1415 1e23 282d 3237 3c41 5863 6f6d  .....#(-27<AXcom
-00004920: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
-00004930: 656e 6564 5b64 6174 6543 7265 6174 6564  ened[dateCreated
-00004940: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-00004950: 5776 6572 7369 6f6e 546e 616d 655c 6461  WversionTname\da
-00004960: 7465 4d6f 6469 6669 6564 d416 1718 191a  teModified......
-00004970: 0a1c 1d55 696e 6465 7859 6173 6365 6e64  ...UindexYascend
-00004980: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00004990: 6510 0709 1101 2c08 d416 1718 191f 1d21  e.....,........!
-000049a0: 1d10 0808 10c8 08d4 1617 1819 241d 261d  ............$.&.
-000049b0: 1002 0810 b508 d416 1718 1929 1d2b 0a10  ...........).+..
-000049c0: 0308 1061 09d4 1617 1819 2e0a 301d 1005  ...a........0...
-000049d0: 0910 6408 d416 1718 1933 0a35 0a10 0409  ..d......3.5....
-000049e0: 1073 09d4 1617 1819 380a 3a1d 1006 0910  .s......8.:.....
-000049f0: 4b08 d416 1718 193d 0a3f 0a10 0009 1102  K......=.?......
-00004a00: 5109 d416 1718 1909 1d26 0a08 0908 2340  Q........&....#@
-00004a10: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
-00004a20: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
-00004a30: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
-00004a40: 00ab 00ba 00c6 00cb 00d1 00d6 00de 00e3  ................
-00004a50: 00f0 00f9 00ff 0109 010f 0117 0119 011a  ................
-00004a60: 011d 011e 0127 0129 012a 012c 012d 0136  .....'.).*.,.-.6
-00004a70: 0138 0139 013b 013c 0145 0147 0148 014a  .8.9.;.<.E.G.H.J
-00004a80: 014b 0154 0156 0157 0159 015a 0163 0165  .K.T.V.W.Y.Z.c.e
-00004a90: 0166 0168 0169 0172 0174 0175 0177 0178  .f.h.i.r.t.u.w.x
-00004aa0: 0181 0183 0184 0187 0188 0191 0192 0193  ................
-00004ab0: 0194 019d 01a2 01ab 0000 0000 0000 0201  ................
-00004ac0: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
-00004ad0: 0000 0000 0000 01ac 0000 0005 006d 006f  .............m.o
-00004ae0: 0064 0065 006c 6d6f 4444 626c 6f62 0000  .d.e.lmoDDblob..
-00004af0: 0008 e652 eadf 2c00 c541 0000 0005 006d  ...R..,..A.....m
-00004b00: 006f 0064 0065 006c 6d6f 6444 626c 6f62  .o.d.e.lmodDblob
-00004b10: 0000 0008 e8d9 3f86 d0fe c441 0000 0005  ......?....A....
-00004b20: 006d 006f 0064 0065 006c 7068 3153 636f  .m.o.d.e.lph1Sco
-00004b30: 6d70 0000 0000 0001 4000 0000 0005 006d  mp......@......m
-00004b40: 006f 0064 0065 006c 7653 726e 6c6f 6e67  .o.d.e.lvSrnlong
-00004b50: 0000 0001 0000 000d 006f 0075 0074 006c  .........o.u.t.l
-00004b60: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00004b70: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
-00004b80: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00004b90: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00004ba0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00004bb0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00004bc0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00004bd0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00004be0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00004bf0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00004c00: 7b33 3934 2c20 3138 317d 2c20 7b37 3730  {394, 181}, {770
-00004c10: 2c20 3433 367d 7d09 0817 2531 3d49 606d  , 436}}...%1=I`m
-00004c20: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-00004c30: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00004c40: 0000 0000 0000 9a00 0000 0d00 6f00 7500  ............o.u.
-00004c50: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
-00004c60: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
-00004c70: 0000 012d 2d00 0000 0d00 6f00 7500 7400  ...--.....o.u.t.
-00004c80: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
-00004c90: 6c00 736c 7376 4362 6c6f 6200 0002 af62  l.slsvCblob....b
-00004ca0: 706c 6973 7430 30da 0102 0304 0506 0708  plist00.........
-00004cb0: 090a 0b0c 0d1a 4849 484a 0c4c 5869 636f  ......HIHJ.LXico
-00004cc0: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
-00004cd0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00004ce0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00004cf0: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
-00004d00: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
-00004d10: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
-00004d20: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00004d30: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00004d40: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00004d50: 696f 6e23 4030 0000 0000 0000 09ab 0e17  ion#@0..........
-00004d60: 1c21 252a 2f34 393e 43d4 0f10 1112 0c14  .!%*/49>C.......
-00004d70: 0c16 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00004d80: 5961 7363 656e 6469 6e67 5a69 6465 6e74  YascendingZident
-00004d90: 6966 6965 7209 10f0 0954 6e61 6d65 d412  ifier....Tname..
-00004da0: 1011 0f18 191a 1a58 7562 6971 7569 7479  .......Xubiquity
-00004db0: 1023 0808 d412 1011 0f1d 1e1a 0c5c 6461  .#...........\da
-00004dc0: 7465 4d6f 6469 6669 6564 10b5 0809 d412  teModified......
-00004dd0: 1011 0f22 1e1a 1a5b 6461 7465 4372 6561  ..."...[dateCrea
-00004de0: 7465 6408 08d4 1210 110f 2627 1a0c 5473  ted.......&'..Ts
-00004df0: 697a 6510 6108 09d4 1210 110f 2b2c 0c0c  ize.a.......+,..
-00004e00: 546b 696e 6410 7309 09d4 1210 110f 3031  Tkind.s.......01
-00004e10: 0c1a 556c 6162 656c 1064 0908 d412 1011  ..Ulabel.d......
-00004e20: 0f35 360c 1a57 7665 7273 696f 6e10 4b09  .56..Wversion.K.
-00004e30: 08d4 1210 110f 3a3b 0c1a 5863 6f6d 6d65  ......:;..Xcomme
-00004e40: 6e74 7311 012c 0908 d412 1011 0f3f 401a  nts..,.......?@.
-00004e50: 1a5e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00004e60: 10c8 0808 d412 1011 0f44 1e1a 1a59 6461  .........D...Yda
-00004e70: 7465 4164 6465 6408 0808 2300 0000 0000  teAdded...#.....
-00004e80: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00004e90: 6509 1001 0008 001d 0026 0038 0040 0054  e........&.8.@.T
-00004ea0: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
-00004eb0: 00ca 00d3 00db 00e1 00eb 00f6 00f7 00f9  ................
-00004ec0: 00fa 00ff 0108 0111 0113 0114 0115 011e  ................
-00004ed0: 012b 012d 012e 012f 0138 0144 0145 0146  .+.-.../.8.D.E.F
-00004ee0: 014f 0154 0156 0157 0158 0161 0166 0168  .O.T.V.W.X.a.f.h
-00004ef0: 0169 016a 0173 0179 017b 017c 017d 0186  .i.j.s.y.{.|.}..
-00004f00: 018e 0190 0191 0192 019b 01a4 01a7 01a8  ................
-00004f10: 01a9 01b2 01c1 01c3 01c4 01c5 01ce 01d8  ................
-00004f20: 01d9 01da 01db 01e4 01ed 01f2 01f3 0000  ................
-00004f30: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-00004f40: 0000 0000 0000 0000 0000 0000 01f5 5368  ..............Sh
-00004f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00004f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00004f70: 6172 0808 0908 095f 1015 7b7b 302c 2030  ar....._..{{0, 0
-00004f80: 7d2c 207b 3134 3430 2c20 3837 377d 7d09  }, {1440, 877}}.
-00004f90: 0817 2531 3d49 606d 797a 7b7c 7d7e 9600  ..%1=I`myz{|}~..
-00004fa0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00004fb0: 0000 0000 0000 0000 0000 0000 0000 9700  ................
-00004fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00004fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00004fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00004000: 0000 0000 0000 0000 0000 0018 0000 000b  ................
+00004010: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
+00004020: 002e 0070 0079 7074 624c 7573 7472 0000  ...p.yptbLustr..
+00004030: 003d 0053 0079 0073 0074 0065 006d 002f  .=.S.y.s.t.e.m./
+00004040: 0056 006f 006c 0075 006d 0065 0073 002f  .V.o.l.u.m.e.s./
+00004050: 0044 0061 0074 0061 002f 0055 0073 0065  .D.a.t.a./.U.s.e
+00004060: 0072 0073 002f 0073 0069 006d 006f 006e  .r.s./.s.i.m.o.n
+00004070: 002f 0044 0065 0073 006b 0074 006f 0070  ./.D.e.s.k.t.o.p
+00004080: 002f 0065 006e 0076 0073 002f 0073 0069  ./.e.n.v.s./.s.i
+00004090: 006d 0062 0061 005f 0064 0065 0076 002f  .m.b.a._.d.e.v./
+000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
+000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
+000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
+000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
+000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
+000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
+00004100: 005f 6c67 3153 636f 6d70 0000 0000 0042  ._lg1Scomp.....B
+00004110: 0340 0000 000b 005f 005f 0070 0079 0063  .@....._._.p.y.c
+00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
+00004130: 626c 6f62 0000 0008 3b88 1802 0f04 c541  blob....;......A
+00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
+00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
+00004160: 6f62 0000 0008 3b88 1802 0f04 c541 0000  ob....;......A..
+00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
+00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
+00004190: 0000 0000 004f e000 0000 0006 0061 0073  .....O.......a.s
+000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
+000041b0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+000041c0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+000041d0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+000041e0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+000041f0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00004200: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00004210: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00004220: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00004230: 0809 5f10 187b 7b33 362c 2031 3331 7d2c  .._..{{36, 131},
+00004240: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
+00004250: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+00004260: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00004270: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
+00004280: 0600 6100 7300 7300 6500 7400 736c 6731  ..a.s.s.e.t.slg1
+00004290: 5363 6f6d 7000 0000 0000 7ddb 9300 0000  Scomp.....}.....
+000042a0: 0600 6100 7300 7300 6500 7400 736c 7376  ..a.s.s.e.t.slsv
+000042b0: 4362 6c6f 6200 0002 b062 706c 6973 7430  Cblob....bplist0
+000042c0: 30da 0102 0304 0506 0708 090a 0b0c 0d1a  0...............
+000042d0: 4849 484a 0c4c 5869 636f 6e53 697a 655f  HIHJ.LXiconSize_
+000042e0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+000042f0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+00004300: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
+00004310: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
+00004320: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
+00004330: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
+00004340: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
+00004350: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
+00004360: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
+00004370: 0000 0000 0000 09ab 0e17 1c21 252a 2f34  ...........!%*/4
+00004380: 393e 43d4 0f10 1112 1314 0c0c 5a69 6465  9>C.........Zide
+00004390: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
+000043a0: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
+000043b0: 6e61 6d65 1101 c709 09d4 0f10 1112 1819  name............
+000043c0: 1a1a 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
+000043d0: 0f10 1112 1d1e 1a0c 5c64 6174 654d 6f64  ........\dateMod
+000043e0: 6966 6965 6410 b508 09d4 0f10 1112 221e  ified.........".
+000043f0: 1a1a 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
+00004400: d40f 1011 1226 271a 0c54 7369 7a65 1061  .....&'..Tsize.a
+00004410: 0809 d40f 1011 122b 2c0c 0c54 6b69 6e64  .......+,..Tkind
+00004420: 1073 0909 d40f 1011 1230 310c 1a55 6c61  .s.......01..Ula
+00004430: 6265 6c10 6409 08d4 0f10 1112 3536 0c1a  bel.d.......56..
+00004440: 5776 6572 7369 6f6e 104b 0908 d40f 1011  Wversion.K......
+00004450: 123a 3b0c 1a58 636f 6d6d 656e 7473 1101  .:;..Xcomments..
+00004460: 2c09 08d4 0f10 1112 3f40 1a1a 5e64 6174  ,.......?@..^dat
+00004470: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
+00004480: 0f10 1112 441e 1a1a 5964 6174 6541 6464  ....D...YdateAdd
+00004490: 6564 0808 0823 0000 0000 0000 0000 2340  ed...#........#@
+000044a0: 2800 0000 0000 0054 6e61 6d65 0910 0100  (......Tname....
+000044b0: 0800 1d00 2600 3800 4000 5400 6600 6f00  ....&.8.@.T.f.o.
+000044c0: 8100 8c00 9f00 b400 bd00 be00 ca00 d300  ................
+000044d0: de00 e400 ee00 f600 fb00 fe00 ff01 0001  ................
+000044e0: 0901 1201 1401 1501 1601 1f01 2c01 2e01  ............,...
+000044f0: 2f01 3001 3901 4501 4601 4701 5001 5501  /.0.9.E.F.G.P.U.
+00004500: 5701 5801 5901 6201 6701 6901 6a01 6b01  W.X.Y.b.g.i.j.k.
+00004510: 7401 7a01 7c01 7d01 7e01 8701 8f01 9101  t.z.|.}.~.......
+00004520: 9201 9301 9c01 a501 a801 a901 aa01 b301  ................
+00004530: c201 c401 c501 c601 cf01 d901 da01 db01  ................
+00004540: dc01 e501 ee01 f301 f400 0000 0000 0002  ................
+00004550: 0100 0000 0000 0000 4d00 0000 0000 0000  ........M.......
+00004560: 0000 0000 0000 0001 f600 0000 0600 6100  ..............a.
+00004570: 7300 7300 6500 7400 736c 7376 7062 6c6f  s.s.e.t.slsvpblo
+00004580: 6200 0002 9562 706c 6973 7430 30da 0102  b....bplist00...
+00004590: 0304 0506 0708 090a 0b0c 0d1c 4849 484a  ............HIHJ
+000045a0: 0c29 5869 636f 6e53 697a 655f 100f 7368  .)XiconSize_..sh
+000045b0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+000045c0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+000045d0: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
+000045e0: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+000045f0: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00004600: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00004610: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
+00004620: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
+00004630: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
+00004640: 0000 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
+00004650: 2a2e 3338 3d42 5863 6f6d 6d65 6e74 735e  *.38=BXcomments^
+00004660: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
+00004670: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
+00004680: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
+00004690: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
+000046a0: 6e61 6d65 d418 191a 1b1c 1d0c 1f57 7669  name.........Wvi
+000046b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+000046c0: 6e64 696e 6755 696e 6465 7808 1101 2c09  ndingUindex...,.
+000046d0: 1007 d418 191a 1b1c 221c 2408 10c8 0810  ........".$.....
+000046e0: 08d4 1819 1a1b 0c27 1c29 0910 b508 1001  .......'.)......
+000046f0: d418 191a 1b1c 271c 2d08 0810 02d4 1819  ......'.-.......
+00004700: 1a1b 0c30 1c32 0910 6108 1003 d418 191a  ...0.2..a.......
+00004710: 1b1c 350c 3708 1064 0910 05d4 1819 1a1b  ..5.7..d........
+00004720: 0c3a 0c3c 0910 7309 1004 d418 191a 1b1c  .:.<..s.........
+00004730: 3f0c 4108 104b 0910 06d4 1819 1a1b 0c44  ?.A..K.........D
+00004740: 0c46 0911 01c7 0910 0008 2300 0000 0000  .F........#.....
+00004750: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00004760: 6509 0008 001d 0026 0038 0040 0054 0066  e......&.8.@.T.f
+00004770: 006f 0081 008c 009f 00b4 00bd 00be 00d1  .o..............
+00004780: 00da 00e9 00f6 0102 0107 010d 0112 011a  ................
+00004790: 011f 0128 0130 0136 0140 0146 0147 014a  ...(.0.6.@.F.G.J
+000047a0: 014b 014d 0156 0157 0159 015a 015c 0165  .K.M.V.W.Y.Z.\.e
+000047b0: 0166 0168 0169 016b 0174 0175 0176 0178  .f.h.i.k.t.u.v.x
+000047c0: 0181 0182 0184 0185 0187 0190 0191 0193  ................
+000047d0: 0194 0196 019f 01a0 01a2 01a3 01a5 01ae  ................
+000047e0: 01af 01b1 01b2 01b4 01bd 01be 01c1 01c2  ................
+000047f0: 01c4 01c5 01ce 01d7 01dc 0000 0000 0000  ................
+00004800: 0201 0000 0000 0000 004c 0000 0000 0000  .........L......
+00004810: 0000 0000 0000 0000 01dd 0000 0006 0061  ...............a
+00004820: 0073 0073 0065 0074 0073 6d6f 4444 626c  .s.s.e.t.smoDDbl
+00004830: 6f62 0000 0008 cf95 8ce8 d0e1 c441 0000  ob...........A..
+00004840: 0006 0061 0073 0073 0065 0074 0073 6d6f  ...a.s.s.e.t.smo
+00004850: 6444 626c 6f62 0000 0008 cf95 8ce8 d0e1  dDblob..........
+00004860: c441 0000 0006 0061 0073 0073 0065 0074  .A.....a.s.s.e.t
+00004870: 0073 7068 3153 636f 6d70 0000 0000 0081  .sph1Scomp......
+00004880: a000 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
+00004890: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
+000048a0: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
+000048b0: 006f 0072 0061 0067 0065 6277 7370 626c  .o.r.a.g.ebwspbl
+000048c0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+000048d0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+000048e0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+000048f0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00004900: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00004910: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00004920: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00004930: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00004940: 0809 0809 5f10 187b 7b35 3139 2c20 3333  ...._..{{519, 33
+00004950: 347d 2c20 7b37 3730 2c20 3433 367d 7d09  4}, {770, 436}}.
+00004960: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+00004970: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00004980: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+00004990: 0000 0c00 6200 6c00 6f00 6200 5f00 7300  ....b.l.o.b._.s.
+000049a0: 7400 6f00 7200 6100 6700 656c 6731 5363  t.o.r.a.g.elg1Sc
+000049b0: 6f6d 7000 0000 0000 0018 0400 0000 0c00  omp.............
+000049c0: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
+000049d0: 7200 6100 6700 656d 6f44 4462 6c6f 6200  r.a.g.emoDDblob.
+000049e0: 0000 083f 3c3f 74e2 ddc4 4100 0000 0c00  ...?<?t...A.....
+000049f0: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
+00004a00: 7200 6100 6700 656d 6f64 4462 6c6f 6200  r.a.g.emodDblob.
+00004a10: 0000 083f 3c3f 74e2 ddc4 4100 0000 0c00  ...?<?t...A.....
+00004a20: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
+00004a30: 7200 6100 6700 6570 6831 5363 6f6d 7000  r.a.g.eph1Scomp.
+00004a40: 0000 0000 0020 0000 0000 0c00 6200 6c00  ..... ......b.l.
+00004a50: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
+00004a60: 6700 6576 5372 6e6c 6f6e 6700 0000 0100  g.evSrnlong.....
+00004a70: 0000 1200 6200 6f00 7500 6e00 6400 6900  ....b.o.u.n.d.i.
+00004a80: 6e00 6700 5f00 6200 6f00 7800 5f00 7400  n.g._.b.o.x._.t.
+00004a90: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
+00004aa0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00004ab0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+00004ac0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+00004ad0: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+00004ae0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00004af0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00004b00: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00004b10: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+00004b20: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
+00004b30: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
+00004b40: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
+00004b50: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00004b60: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
+00004b70: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
+00004b80: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
+00004b90: 6f00 6c00 7364 7363 6c62 6f6f 6c00 0000  o.l.sdsclbool...
+00004ba0: 0012 0062 006f 0075 006e 0064 0069 006e  ...b.o.u.n.d.i.n
+00004bb0: 0067 005f 0062 006f 0078 005f 0074 006f  .g._.b.o.x._.t.o
+00004bc0: 006f 006c 0073 6c67 3153 636f 6d70 0000  .o.l.slg1Scomp..
+00004bd0: 0000 0002 6c79 0000 0012 0062 006f 0075  ....ly.....b.o.u
+00004be0: 006e 0064 0069 006e 0067 005f 0062 006f  .n.d.i.n.g._.b.o
+00004bf0: 0078 005f 0074 006f 006f 006c 0073 6c73  .x._.t.o.o.l.sls
+00004c00: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
+00004c10: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
+00004c20: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
+00004c30: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00004c40: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00004c50: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00004c60: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00004c70: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
+00004c80: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
+00004c90: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
+00004ca0: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
+00004cb0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00004cc0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
+00004cd0: 7209 1101 c709 546e 616d 65d4 0d0e 0f10  r.....Tname.....
+00004ce0: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
+00004cf0: 79d4 0d0e 0f10 0a1c 161e 0910 b508 5c64  y.............\d
+00004d00: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
+00004d10: 161c 1622 0808 5b64 6174 6543 7265 6174  ..."..[dateCreat
+00004d20: 6564 d40d 0e0f 100a 2516 2709 1061 0854  ed......%.'..a.T
+00004d30: 7369 7a65 d40d 0e0f 100a 2a0a 2c09 1073  size......*.,..s
+00004d40: 0954 6b69 6e64 d40d 0e0f 1016 2f0a 3108  .Tkind....../.1.
+00004d50: 1064 0955 6c61 6265 6cd4 0d0e 0f10 1634  .d.Ulabel......4
+00004d60: 0a36 0810 4b09 5776 6572 7369 6f6e d40d  .6..K.Wversion..
+00004d70: 0e0f 1016 390a 3b08 1101 2c09 5863 6f6d  ....9.;...,.Xcom
+00004d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
+00004d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00004da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
+00004db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
+00004dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
+00004dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
+00004de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
+00004df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
+00004e00: dd00 de00 e700 f000 f100 f300 f401 0101  ................
+00004e10: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
+00004e20: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
+00004e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
+00004e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
+00004e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
+00004e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
+00004e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00004e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
+00004e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005000: 0000 0000 0000 0000 0000 0014 0000 000d  ................
-00005010: 006f 0075 0074 006c 0069 0065 0072 005f  .o.u.t.l.i.e.r._
-00005020: 0074 006f 006f 006c 0073 6d6f 4444 626c  .t.o.o.l.smoDDbl
-00005030: 6f62 0000 0008 b7c8 5a86 d0fe c441 0000  ob......Z....A..
-00005040: 000d 006f 0075 0074 006c 0069 0065 0072  ...o.u.t.l.i.e.r
-00005050: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-00005060: 626c 6f62 0000 0008 b7c8 5a86 d0fe c441  blob......Z....A
-00005070: 0000 000d 006f 0075 0074 006c 0069 0065  .....o.u.t.l.i.e
-00005080: 0072 005f 0074 006f 006f 006c 0073 7068  .r._.t.o.o.l.sph
-00005090: 3153 636f 6d70 0000 0000 0002 1000 0000  1Scomp..........
-000050a0: 000d 006f 0075 0074 006c 0069 0065 0072  ...o.u.t.l.i.e.r
-000050b0: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
-000050c0: 6c6f 6e67 0000 0001 0000 0008 0070 006c  long.........p.l
-000050d0: 006f 0074 0074 0069 006e 0067 6277 7370  .o.t.t.i.n.gbwsp
-000050e0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
-000050f0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00005100: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00005110: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00005120: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00005130: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00005140: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00005150: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00005160: 7208 0809 0809 5f10 177b 7b32 302c 2039  r....._..{{20, 9
-00005170: 307d 2c20 7b31 3031 352c 2037 3637 7d7d  0}, {1015, 767}}
-00005180: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
-00005190: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-000051a0: 0000 0000 0000 0000 0000 0000 0000 0099  ................
-000051b0: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-000051c0: 006e 0067 6c67 3153 636f 6d70 0000 0000  .n.glg1Scomp....
-000051d0: 0009 1177 0000 0008 0070 006c 006f 0074  ...w.....p.l.o.t
-000051e0: 0074 0069 006e 0067 6c73 7643 626c 6f62  .t.i.n.glsvCblob
-000051f0: 0000 02b0 6270 6c69 7374 3030 da01 0203  ....bplist00....
-00005200: 0405 0607 0809 0a0b 0c0d 1a48 4948 4a0c  ...........HIHJ.
-00005210: 4c58 6963 6f6e 5369 7a65 5f10 0f73 686f  LXiconSize_..sho
-00005220: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00005230: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00005240: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00005250: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-00005260: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-00005270: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00005280: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00005290: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-000052a0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-000052b0: 0009 ab0e 171c 2125 2a2f 3439 3e43 d40f  ......!%*/49>C..
-000052c0: 1011 1213 140c 0c5a 6964 656e 7469 6669  .......Zidentifi
-000052d0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-000052e0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-000052f0: 0127 0909 d40f 1011 1218 191a 1a58 7562  .'...........Xub
-00005300: 6971 7569 7479 1023 0808 d40f 1011 121d  iquity.#........
-00005310: 1e1a 0c5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00005320: 10b5 0809 d40f 1011 1222 1e1a 1a5b 6461  ........."...[da
-00005330: 7465 4372 6561 7465 6408 08d4 0f10 1112  teCreated.......
-00005340: 2627 1a0c 5473 697a 6510 6108 09d4 0f10  &'..Tsize.a.....
-00005350: 1112 2b2c 0c0c 546b 696e 6410 7309 09d4  ..+,..Tkind.s...
-00005360: 0f10 1112 3031 0c1a 556c 6162 656c 1064  ....01..Ulabel.d
-00005370: 0908 d40f 1011 1235 360c 1a57 7665 7273  .......56..Wvers
-00005380: 696f 6e10 4b09 08d4 0f10 1112 3a3b 0c1a  ion.K.......:;..
-00005390: 5863 6f6d 6d65 6e74 7311 012c 0908 d40f  Xcomments..,....
-000053a0: 1011 123f 401a 1a5e 6461 7465 4c61 7374  ...?@..^dateLast
-000053b0: 4f70 656e 6564 10c8 0808 d40f 1011 1244  Opened.........D
-000053c0: 1e1a 1a59 6461 7465 4164 6465 6408 0808  ...YdateAdded...
-000053d0: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
-000053e0: 0000 546e 616d 6509 1001 0008 001d 0026  ..Tname........&
-000053f0: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
-00005400: 00b4 00bd 00be 00ca 00d3 00de 00e4 00ee  ................
-00005410: 00f6 00fb 00fe 00ff 0100 0109 0112 0114  ................
-00005420: 0115 0116 011f 012c 012e 012f 0130 0139  .......,.../.0.9
-00005430: 0145 0146 0147 0150 0155 0157 0158 0159  .E.F.G.P.U.W.X.Y
-00005440: 0162 0167 0169 016a 016b 0174 017a 017c  .b.g.i.j.k.t.z.|
-00005450: 017d 017e 0187 018f 0191 0192 0193 019c  .}.~............
-00005460: 01a5 01a8 01a9 01aa 01b3 01c2 01c4 01c5  ................
-00005470: 01c6 01cf 01d9 01da 01db 01dc 01e5 01ee  ................
-00005480: 01f3 01f4 0000 0000 0000 0201 0000 0000  ................
-00005490: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
-000054a0: 0000 01f6 0000 0008 0070 006c 006f 0074  .........p.l.o.t
-000054b0: 0074 0069 006e 0067 6c73 7670 626c 6f62  .t.i.n.glsvpblob
-000054c0: 0000 0295 6270 6c69 7374 3030 da01 0203  ....bplist00....
-000054d0: 0405 0607 0809 0a0b 0c0d 1c48 4948 4a0c  ...........HIHJ.
-000054e0: 2958 6963 6f6e 5369 7a65 5f10 0f73 686f  )XiconSize_..sho
-000054f0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00005500: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00005510: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00005520: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-00005530: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-00005540: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00005550: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00005560: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00005570: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00005580: 0009 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
-00005590: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
-000055a0: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-000055b0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-000055c0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-000055d0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-000055e0: 616d 65d4 1819 1a1b 1c1d 0c1f 5776 6973  ame.........Wvis
-000055f0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-00005600: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-00005610: 07d4 1819 1a1b 1c22 1c24 0810 c808 1008  .......".$......
-00005620: d418 191a 1b0c 271c 2909 10b5 0810 01d4  ......'.).......
-00005630: 1819 1a1b 1c27 1c2d 0808 1002 d418 191a  .....'.-........
-00005640: 1b0c 301c 3209 1061 0810 03d4 1819 1a1b  ..0.2..a........
-00005650: 1c35 0c37 0810 6409 1005 d418 191a 1b0c  .5.7..d.........
-00005660: 3a0c 3c09 1073 0910 04d4 1819 1a1b 1c3f  :.<..s.........?
-00005670: 0c41 0810 4b09 1006 d418 191a 1b0c 440c  .A..K.........D.
-00005680: 4609 1101 2709 1000 0823 0000 0000 0000  F...'....#......
-00005690: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
-000056a0: 0900 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
-000056b0: 6f00 8100 8c00 9f00 b400 bd00 be00 d100  o...............
-000056c0: da00 e900 f601 0201 0701 0d01 1201 1a01  ................
-000056d0: 1f01 2801 3001 3601 4001 4601 4701 4a01  ..(.0.6.@.F.G.J.
-000056e0: 4b01 4d01 5601 5701 5901 5a01 5c01 6501  K.M.V.W.Y.Z.\.e.
-000056f0: 6601 6801 6901 6b01 7401 7501 7601 7801  f.h.i.k.t.u.v.x.
-00005700: 8101 8201 8401 8501 8701 9001 9101 9301  ................
-00005710: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
-00005720: af01 b101 b201 b401 bd01 be01 c101 c201  ................
-00005730: c401 c501 ce01 d701 dc00 0000 0000 0002  ................
-00005740: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
-00005750: 0000 0000 0000 0001 dd00 0000 0800 7000  ..............p.
-00005760: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-00005770: 4462 6c6f 6200 0000 0858 13c8 10f2 00c5  Dblob....X......
-00005780: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
-00005790: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-000057a0: 0838 ff78 5163 ffc4 4100 0000 0800 7000  .8.xQc..A.....p.
-000057b0: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
-000057c0: 5363 6f6d 7000 0000 0000 0b20 0000 0000  Scomp...... ....
-000057d0: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
-000057e0: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
-000057f0: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-00005800: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00005810: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
-00005820: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-00005830: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-00005840: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-00005850: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-00005860: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00005870: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00005880: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00005890: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-000058a0: 095f 1019 7b7b 3135 392c 2031 3233 7d2c  ._..{{159, 123},
-000058b0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
-000058c0: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
-000058d0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000058e0: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
-000058f0: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-00005900: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00005910: 6900 6f00 6e00 7364 7363 6c62 6f6f 6c00  i.o.n.sdsclbool.
-00005920: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-00005930: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-00005940: 0074 0069 006f 006e 0073 6c67 3153 636f  .t.i.o.n.slg1Sco
-00005950: 6d70 0000 0000 0006 ae56 0000 0013 0070  mp.......V.....p
-00005960: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
-00005970: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
-00005980: 006e 0073 6c73 7643 626c 6f62 0000 02b0  .n.slsvCblob....
-00005990: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-000059a0: 0809 0a0b 0b0d 1a48 4948 4a4b 4c5f 1010  .......HIHJKL_..
-000059b0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000059c0: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-000059d0: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-000059e0: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
-000059f0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
-00005a00: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
-00005a10: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
-00005a20: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-00005a30: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00005a40: 7369 6f6e 0909 ab0e 171c 2125 2a2f 3439  sion......!%*/49
-00005a50: 3e43 d40f 1011 1213 140b 0b5a 6964 656e  >C.........Ziden
-00005a60: 7469 6669 6572 5577 6964 7468 5961 7363  tifierUwidthYasc
-00005a70: 656e 6469 6e67 5776 6973 6962 6c65 546e  endingWvisibleTn
-00005a80: 616d 6511 0127 0909 d40f 1011 1218 191a  ame..'..........
-00005a90: 1a58 7562 6971 7569 7479 1023 0808 d40f  .Xubiquity.#....
-00005aa0: 1011 121d 1e1a 0b5c 6461 7465 4d6f 6469  .......\dateModi
-00005ab0: 6669 6564 10b5 0809 d40f 1011 1222 1e1a  fied........."..
-00005ac0: 1a5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
-00005ad0: 0f10 1112 2627 1a0b 5473 697a 6510 6108  ....&'..Tsize.a.
-00005ae0: 09d4 0f10 1112 2b2c 0b0b 546b 696e 6410  ......+,..Tkind.
-00005af0: 7309 09d4 0f10 1112 3031 0b1a 556c 6162  s.......01..Ulab
-00005b00: 656c 1064 0908 d40f 1011 1235 360b 1a57  el.d.......56..W
-00005b10: 7665 7273 696f 6e10 4b09 08d4 0f10 1112  version.K.......
-00005b20: 3a3b 0b1a 5863 6f6d 6d65 6e74 7311 012c  :;..Xcomments..,
-00005b30: 0908 d40f 1011 123f 401a 1a5e 6461 7465  .......?@..^date
-00005b40: 4c61 7374 4f70 656e 6564 10c8 0808 d40f  LastOpened......
-00005b50: 1011 1244 1e1a 1a59 6461 7465 4164 6465  ...D...YdateAdde
-00005b60: 6408 0808 2300 0000 0000 0000 0023 4028  d...#........#@(
-00005b70: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-00005b80: 0000 0000 1001 0008 001d 0030 0042 004a  ...........0.B.J
-00005b90: 005e 0070 0079 008b 0096 009f 00b4 00b5  .^.p.y..........
-00005ba0: 00b6 00c2 00cb 00d6 00dc 00e6 00ee 00f3  ................
-00005bb0: 00f6 00f7 00f8 0101 010a 010c 010d 010e  ................
-00005bc0: 0117 0124 0126 0127 0128 0131 013d 013e  ...$.&.'.(.1.=.>
-00005bd0: 013f 0148 014d 014f 0150 0151 015a 015f  .?.H.M.O.P.Q.Z._
-00005be0: 0161 0162 0163 016c 0172 0174 0175 0176  .a.b.c.l.r.t.u.v
-00005bf0: 017f 0187 0189 018a 018b 0194 019d 01a0  ................
-00005c00: 01a1 01a2 01ab 01ba 01bc 01bd 01be 01c7  ................
-00005c10: 01d1 01d2 01d3 01d4 01dd 01e6 01eb 01f4  ................
-00005c20: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
-00005c30: 0000 0000 0000 0000 0000 0000 0000 01f6  ................
-00005c40: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-00005c50: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-00005c60: 0074 0069 006f 006e 0073 6c73 7670 626c  .t.i.o.n.slsvpbl
-00005c70: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
-00005c80: 0203 0405 0607 0809 0a0b 0b0d 1c48 4948  .............HIH
-00005c90: 4a4b 295f 1010 7573 6552 656c 6174 6976  JK)_..useRelativ
-00005ca0: 6544 6174 6573 5f10 0f73 686f 7749 636f  eDates_..showIco
-00005cb0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00005cc0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00005cd0: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
-00005ce0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
-00005cf0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-00005d00: 585a 736f 7274 436f 6c75 6d6e 5869 636f  XZsortColumnXico
-00005d10: 6e53 697a 655f 1012 7669 6577 4f70 7469  nSize_..viewOpti
-00005d20: 6f6e 7356 6572 7369 6f6e 0909 d90e 0f10  onsVersion......
-00005d30: 1112 1314 1516 1720 252a 2e33 383d 4258  ....... %*.38=BX
-00005d40: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
-00005d50: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
-00005d60: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
-00005d70: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-00005d80: 5776 6572 7369 6f6e 546e 616d 65d4 1819  WversionTname...
-00005d90: 1a1b 1c1d 0b1f 5776 6973 6962 6c65 5577  ......WvisibleUw
-00005da0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
-00005db0: 6e64 6578 0811 012c 0910 07d4 1819 1a1b  ndex...,........
-00005dc0: 1c22 1c24 0810 c808 1008 d418 191a 1b0b  .".$............
-00005dd0: 271c 2909 10b5 0810 01d4 1819 1a1b 1c27  '.)............'
-00005de0: 1c2d 0808 1002 d418 191a 1b0b 301c 3209  .-..........0.2.
-00005df0: 1061 0810 03d4 1819 1a1b 1c35 0b37 0810  .a.........5.7..
-00005e00: 6409 1005 d418 191a 1b0b 3a0b 3c09 1073  d.........:.<..s
-00005e10: 0910 04d4 1819 1a1b 1c3f 0b41 0810 4b09  .........?.A..K.
-00005e20: 1006 d418 191a 1b0b 440b 4609 1101 2709  ........D.F...'.
-00005e30: 1000 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
-00005e40: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
-00005e50: 0000 0000 0800 1d00 3000 4200 4a00 5e00  ........0.B.J.^.
-00005e60: 7000 7900 8b00 9600 9f00 b400 b500 b600  p.y.............
-00005e70: c900 d200 e100 ee00 fa00 ff01 0501 0a01  ................
-00005e80: 1201 1701 2001 2801 2e01 3801 3e01 3f01  .... .(...8.>.?.
-00005e90: 4201 4301 4501 4e01 4f01 5101 5201 5401  B.C.E.N.O.Q.R.T.
-00005ea0: 5d01 5e01 6001 6101 6301 6c01 6d01 6e01  ].^.`.a.c.l.m.n.
-00005eb0: 7001 7901 7a01 7c01 7d01 7f01 8801 8901  p.y.z.|.}.......
-00005ec0: 8b01 8c01 8e01 9701 9801 9a01 9b01 9d01  ................
-00005ed0: a601 a701 a901 aa01 ac01 b501 b601 b901  ................
-00005ee0: ba01 bc01 bd01 c601 cf01 d400 0000 0000  ................
-00005ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00005f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
-00005f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
-00005f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
-00005f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
-00005f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
-00005f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
-00005f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00005f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
-00005f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
-00005f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00005fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00005fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
-00005fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00005fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00005fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00005000: 0000 0000 0000 0000 0000 001d 0000 0012  ................
+00005010: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
+00005020: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
+00005030: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
+00005040: c351 4bc6 4505 c541 0000 0012 0062 006f  .QK.E..A.....b.o
+00005050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
+00005060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
+00005070: 6d6f 6444 626c 6f62 0000 0008 0270 b7c1  modDblob.....p..
+00005080: 4105 c541 0000 0012 0062 006f 0075 006e  A..A.....b.o.u.n
+00005090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
+000050a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
+000050b0: 636f 6d70 0000 0000 0002 f000 0000 0012  comp............
+000050c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
+000050d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
+000050e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
+000050f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
+00005100: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
+00005110: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+00005120: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00005130: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00005140: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00005150: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00005160: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00005170: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00005180: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00005190: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+000051a0: 7b33 3934 2c20 3138 317d 2c20 7b37 3730  {394, 181}, {770
+000051b0: 2c20 3433 367d 7d09 0817 2531 3d49 606d  , 436}}...%1=I`m
+000051c0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+000051d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+000051e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
+000051f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
+00005200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
+00005210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
+00005220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
+00005230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
+00005240: 0001 d983 0000 000f 0063 0075 0065 005f  .........c.u.e._
+00005250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
+00005260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
+00005270: 0008 a4c2 03c3 a304 c541 0000 000f 0063  .........A.....c
+00005280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
+00005290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
+000052a0: 626c 6f62 0000 0008 dc16 211a fb01 c541  blob......!....A
+000052b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
+000052c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
+000052d0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
+000052e0: 6000 0000 000f 0063 0075 0065 005f 006c  `......c.u.e._.l
+000052f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
+00005300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
+00005310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
+00005320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
+00005330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00005340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+00005350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00005360: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00005370: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00005380: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00005390: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+000053a0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+000053b0: 187b 7b36 3537 2c20 3237 307d 2c20 7b39  .{{657, 270}, {9
+000053c0: 3839 2c20 3433 367d 7d09 0817 2531 3d49  89, 436}}...%1=I
+000053d0: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
+000053e0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+000053f0: 0000 0000 0000 0000 9a00 0000 0800 6400  ..............d.
+00005400: 6100 7300 6800 5f00 6100 7000 706c 6731  a.s.h._.a.p.plg1
+00005410: 5363 6f6d 7000 0000 0000 0135 6200 0000  Scomp......5b...
+00005420: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
+00005430: 706d 6f44 4462 6c6f 6200 0000 087e 81a5  pmoDDblob....~..
+00005440: d736 fec4 4100 0000 0800 6400 6100 7300  .6..A.....d.a.s.
+00005450: 6800 5f00 6100 7000 706d 6f64 4462 6c6f  h._.a.p.pmodDblo
+00005460: 6200 0000 087e 81a5 d736 fec4 4100 0000  b....~...6..A...
+00005470: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
+00005480: 7070 6831 5363 6f6d 7000 0000 0000 0150  pph1Scomp......P
+00005490: 0000 0000 0800 6400 6100 7300 6800 5f00  ......d.a.s.h._.
+000054a0: 6100 7000 7076 5372 6e6c 6f6e 6700 0000  a.p.pvSrnlong...
+000054b0: 0100 0000 0f00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
+000054c0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+000054d0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
+000054e0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+000054f0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00005500: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00005510: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00005520: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00005530: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00005540: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00005550: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00005560: 7b7b 3233 322c 2031 3931 7d2c 207b 3133  {{232, 191}, {13
+00005570: 3032 2c20 3731 347d 7d09 0817 2531 3d49  02, 714}}...%1=I
+00005580: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
+000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
+000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
+000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
+000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
+00005600: 0000 0002 c428 0000 000f 0064 0061 0074  .....(.....d.a.t
+00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
+00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
+00005630: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
+00005640: 0405 0607 0809 0a0b 1949 4a0a 4c58 6963  .........IJ.LXic
+00005650: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00005660: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00005670: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00005680: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+00005690: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000056a0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+000056b0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000056c0: 2340 3000 0000 0000 0009 ab0c 151d 2226  #@0..........."&
+000056d0: 2b30 353a 3f44 d40d 0e0f 1011 120a 0a5a  +05:?D.........Z
+000056e0: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
+000056f0: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00005700: 6c65 546e 616d 6511 01c7 0909 d416 1718  leTname.........
+00005710: 0d19 1a19 1c57 7669 7369 626c 6555 7769  .....WvisibleUwi
+00005720: 6474 6859 6173 6365 6e64 696e 6708 1023  dthYascending..#
+00005730: 0858 7562 6971 7569 7479 d40d 0e0f 101e  .Xubiquity......
+00005740: 1f19 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00005750: 10b5 0809 d40d 0e0f 1023 1f19 195b 6461  .........#...[da
+00005760: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
+00005770: 2728 190a 5473 697a 6510 6108 09d4 0d0e  '(..Tsize.a.....
+00005780: 0f10 2c2d 0a0a 546b 696e 6410 7309 09d4  ..,-..Tkind.s...
+00005790: 0d0e 0f10 3132 0a19 556c 6162 656c 1064  ....12..Ulabel.d
+000057a0: 0908 d40d 0e0f 1036 370a 1957 7665 7273  .......67..Wvers
+000057b0: 696f 6e10 4b09 08d4 0d0e 0f10 3b3c 0a19  ion.K.......;<..
+000057c0: 5863 6f6d 6d65 6e74 7311 012c 0908 d40d  Xcomments..,....
+000057d0: 0e0f 1040 4119 195e 6461 7465 4c61 7374  ...@A..^dateLast
+000057e0: 4f70 656e 6564 10c8 0808 d416 1718 0d19  Opened..........
+000057f0: 1f19 4708 0859 6461 7465 4164 6465 6408  ..G..YdateAdded.
+00005800: 2340 2800 0000 0000 0054 6e61 6d65 0910  #@(......Tname..
+00005810: 0100 0800 1900 2200 3400 3c00 5000 5900  ......".4.<.P.Y.
+00005820: 6400 7700 8c00 9500 9600 a200 ab00 b600  d.w.............
+00005830: bc00 c600 ce00 d300 d600 d700 d800 e100  ................
+00005840: e900 ef00 f900 fa00 fc00 fd01 0601 0f01  ................
+00005850: 1c01 1e01 1f01 2001 2901 3501 3601 3701  ...... .).5.6.7.
+00005860: 4001 4501 4701 4801 4901 5201 5701 5901  @.E.G.H.I.R.W.Y.
+00005870: 5a01 5b01 6401 6a01 6c01 6d01 6e01 7701  Z.[.d.j.l.m.n.w.
+00005880: 7f01 8101 8201 8301 8c01 9501 9801 9901  ................
+00005890: 9a01 a301 b201 b401 b501 b601 bf01 c001  ................
+000058a0: c101 cb01 cc01 d501 da01 db00 0000 0000  ................
+000058b0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000058c0: 0000 0000 0000 0000 0001 dd00 0000 0f00  ................
+000058d0: 6400 6100 7400 6100 5f00 7000 7200 6f00  d.a.t.a._.p.r.o.
+000058e0: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
+000058f0: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+00005900: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
+00005910: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
+00005920: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00005930: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00005940: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00005950: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+00005960: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00005970: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00005980: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
+00005990: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
+000059a0: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
+000059b0: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
+000059c0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+000059d0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+000059e0: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
+000059f0: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
+00005a00: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+00005a10: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
+00005a20: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
+00005a30: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
+00005a40: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
+00005a50: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
+00005a60: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
+00005a70: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
+00005a80: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
+00005a90: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
+00005aa0: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
+00005ab0: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
+00005ac0: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
+00005ad0: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
+00005ae0: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
+00005af0: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
+00005b00: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
+00005b10: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
+00005b20: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
+00005b30: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
+00005b40: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+00005b50: 0000 0000 0001 ac00 0000 0f00 6400 6100  ............d.a.
+00005b60: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
+00005b70: 7300 7300 6f00 7200 736d 6f44 4462 6c6f  s.s.o.r.smoDDblo
+00005b80: 6200 0000 080b 5109 4149 05c5 4100 0000  b.....Q.AI..A...
+00005b90: 0f00 6400 6100 7400 6100 5f00 7000 7200  ..d.a.t.a._.p.r.
+00005ba0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
+00005bb0: 6f64 4462 6c6f 6200 0000 080b 5109 4149  odDblob.....Q.AI
+00005bc0: 05c5 4100 0000 0f00 6400 6100 7400 6100  ..A.....d.a.t.a.
+00005bd0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00005be0: 6f00 7200 7370 6831 5363 6f6d 7000 0000  o.r.sph1Scomp...
+00005bf0: 0000 03a0 0000 0000 0f00 6400 6100 7400  ..........d.a.t.
+00005c00: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
+00005c10: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
+00005c20: 0000 0100 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
+00005c30: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
+00005c40: 6100 6300 7400 6f00 7200 7362 7773 7062  a.c.t.o.r.sbwspb
+00005c50: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
+00005c60: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
+00005c70: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00005c80: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
+00005c90: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00005ca0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00005cb0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00005cc0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+00005cd0: 0808 0908 095f 1019 7b7b 3233 322c 2031  ....._..{{232, 1
+00005ce0: 3931 7d2c 207b 3133 3032 2c20 3731 347d  91}, {1302, 714}
+00005cf0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+00005d00: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
+00005d10: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+00005d20: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
+00005d30: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
+00005d40: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
+00005d50: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
+00005d60: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
+00005d70: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
+00005d80: 6d70 0000 0000 0013 5536 163e 1640 0810  mp......U6.>.@..
+00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
+00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
+00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
+00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
+00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
+00005df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
+00005e00: dd00 de00 e700 f000 f100 f300 f401 0101  ................
+00005e10: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
+00005e20: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
+00005e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
+00005e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
+00005e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
+00005e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
+00005e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00005e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
+00005e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006000: 0000 0000 0000 0000 0000 0015 0000 001b  ................
-00006010: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
-00006020: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
-00006030: 006f 006e 0073 005f 0061 0072 0063 0068  .o.n.s._.a.r.c.h
-00006040: 0069 0076 0065 6c67 3153 636f 6d70 0000  .i.v.elg1Scomp..
-00006050: 0000 0006 faed 0000 001b 0070 006f 0073  ...........p.o.s
-00006060: 0065 005f 0063 006f 006e 0066 0069 0067  .e._.c.o.n.f.i.g
-00006070: 0075 0072 0061 0074 0069 006f 006e 0073  .u.r.a.t.i.o.n.s
-00006080: 005f 0061 0072 0063 0068 0069 0076 0065  ._.a.r.c.h.i.v.e
-00006090: 6d6f 4444 626c 6f62 0000 0008 8983 1ea9  moDDblob........
-000060a0: cbfe c441 0000 001b 0070 006f 0073 0065  ...A.....p.o.s.e
-000060b0: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
-000060c0: 0072 0061 0074 0069 006f 006e 0073 005f  .r.a.t.i.o.n.s._
-000060d0: 0061 0072 0063 0068 0069 0076 0065 6d6f  .a.r.c.h.i.v.emo
-000060e0: 6444 626c 6f62 0000 0008 8983 1ea9 cbfe  dDblob..........
-000060f0: c441 0000 001b 0070 006f 0073 0065 005f  .A.....p.o.s.e._
-00006100: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
-00006110: 0061 0074 0069 006f 006e 0073 005f 0061  .a.t.i.o.n.s._.a
-00006120: 0072 0063 0068 0069 0076 0065 7068 3153  .r.c.h.i.v.eph1S
-00006130: 636f 6d70 0000 0000 0007 9000 0000 000e  comp............
-00006140: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
-00006150: 006f 0072 0074 0065 0072 0073 6277 7370  .o.r.t.e.r.sbwsp
-00006160: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
-00006170: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00006180: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00006190: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-000061a0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-000061b0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-000061c0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-000061d0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-000061e0: 7208 0809 0809 5f10 197b 7b36 3432 2c20  r....._..{{642, 
-000061f0: 3132 397d 2c20 7b31 3031 352c 2037 3637  129}, {1015, 767
-00006200: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00006210: 7e9a 0000 0000 0000 0101 0000 0000 0000  ~...............
-00006220: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00006230: 009b 0000 000e 0070 006f 0073 0065 005f  .......p.o.s.e._
-00006240: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
-00006250: 0073 6c67 3153 636f 6d70 0000 0000 0003  .slg1Scomp......
-00006260: fb81 0000 000e 0070 006f 0073 0065 005f  .......p.o.s.e._
-00006270: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
-00006280: 0073 6c73 7643 626c 6f62 0000 0278 6270  .slsvCblob...xbp
-00006290: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
-000062a0: 0a0b 1646 4748 0a5f 1012 7669 6577 4f70  ...FGH._..viewOp
-000062b0: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
-000062c0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-000062d0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000062e0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
-000062f0: 697a 655a 736f 7274 436f 6c75 6d6e 5869  izeZsortColumnXi
-00006300: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
-00006310: 6174 6976 6544 6174 6573 1001 09ab 0c15  ativeDates......
-00006320: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 0a12  ..#(-27<A.......
-00006330: 0a14 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00006340: 5961 7363 656e 6469 6e67 5a69 6465 6e74  YascendingZident
-00006350: 6966 6965 7209 10ea 0954 6e61 6d65 d40d  ifier....Tname..
-00006360: 0e0f 1016 1716 1908 1023 0858 7562 6971  .........#.Xubiq
-00006370: 7569 7479 d40d 0e0f 100a 1c16 1e09 10b5  uity............
-00006380: 085c 6461 7465 4d6f 6469 6669 6564 d40d  .\dateModified..
-00006390: 0e0f 1016 1c16 2208 085b 6461 7465 4372  ......"..[dateCr
-000063a0: 6561 7465 64d4 0d0e 0f10 0a25 1627 0910  eated......%.'..
-000063b0: 6108 5473 697a 65d4 0d0e 0f10 0a2a 0a2c  a.Tsize......*.,
-000063c0: 0910 7309 546b 696e 64d4 0d0e 0f10 162f  ..s.Tkind....../
-000063d0: 0a31 0810 6409 556c 6162 656c d40d 0e0f  .1..d.Ulabel....
-000063e0: 1016 340a 3608 104b 0957 7665 7273 696f  ..4.6..K.Wversio
-000063f0: 6ed4 0d0e 0f10 1639 0a3b 0811 012c 0958  n......9.;...,.X
-00006400: 636f 6d6d 656e 7473 d40d 0e0f 1016 3e16  comments......>.
-00006410: 4008 10c8 085e 6461 7465 4c61 7374 4f70  @....^dateLastOp
-00006420: 656e 6564 d40d 0e0f 1016 1c16 4408 0859  ened........D..Y
-00006430: 6461 7465 4164 6465 6408 2340 2800 0000  dateAdded.#@(...
-00006440: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-00006450: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-00006460: 0070 0079 008c 008e 008f 009b 00a4 00ac  .p.y............
-00006470: 00b2 00bc 00c7 00c8 00ca 00cb 00d0 00d9  ................
-00006480: 00da 00dc 00dd 00e6 00ef 00f0 00f2 00f3  ................
-00006490: 0100 0109 010a 010b 0117 0120 0121 0123  ........... .!.#
-000064a0: 0124 0129 0132 0133 0135 0136 013b 0144  .$.).2.3.5.6.;.D
-000064b0: 0145 0147 0148 014e 0157 0158 015a 015b  .E.G.H.N.W.X.Z.[
-000064c0: 0163 016c 016d 0170 0171 017a 0183 0184  .c.l.m.p.q.z....
-000064d0: 0186 0187 0196 019f 01a0 01a1 01ab 01ac  ................
-000064e0: 01b5 01ba 01c3 0000 0000 0000 0201 0000  ................
-000064f0: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
-00006500: 0000 0000 01c4 0000 000e 0070 006f 0073  ...........p.o.s
-00006510: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
-00006520: 0065 0072 0073 6c73 7670 626c 6f62 0000  .e.r.slsvpblob..
-00006530: 025d 6270 6c69 7374 3030 d801 0203 0405  .]bplist00......
-00006540: 0607 0809 0a0b 1d45 4647 0a5f 1012 7669  .......EFG._..vi
-00006550: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00006560: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00006570: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00006580: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
-00006590: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
-000065a0: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
-000065b0: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
-000065c0: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
-000065d0: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
-000065e0: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
-000065f0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
-00006600: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
-00006610: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
-00006620: 6d65 d416 1718 191a 1b0a 1d55 696e 6465  me.........Uinde
-00006630: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
-00006640: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
-00006650: d416 1718 191f 201d 1d10 0810 c808 08d4  ...... .........
-00006660: 1617 1819 0924 1d0a 10b5 0809 d416 1718  .....$..........
-00006670: 1928 241d 1d10 0208 08d4 1617 1819 2c2d  .($...........,-
-00006680: 1d0a 1003 1061 0809 d416 1718 1931 320a  .....a.......12.
-00006690: 1d10 0510 6409 08d4 1617 1819 3637 0a0a  ....d.......67..
-000066a0: 1004 1073 0909 d416 1718 193b 3c0a 1d10  ...s.......;<...
-000066b0: 0610 4b09 08d4 1617 1819 4041 0a0a 1000  ..K.......@A....
-000066c0: 10ea 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
-000066d0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-000066e0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
-000066f0: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
-00006700: d800 de00 e300 eb00 f000 f900 ff01 0501  ................
-00006710: 0f01 1701 1901 1c01 1d01 1e01 2701 2901  ............'.).
-00006720: 2b01 2c01 2d01 3601 3801 3901 3a01 4301  +.,.-.6.8.9.:.C.
-00006730: 4501 4601 4701 5001 5201 5401 5501 5601  E.F.G.P.R.T.U.V.
-00006740: 5f01 6101 6301 6401 6501 6e01 7001 7201  _.a.c.d.e.n.p.r.
-00006750: 7301 7401 7d01 7f01 8101 8201 8301 8c01  s.t.}...........
-00006760: 8e01 9001 9101 9201 9301 9c01 a101 aa00  ................
-00006770: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00006780: 0000 0000 0000 0000 0000 0000 0001 ab00  ................
-00006790: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
-000067a0: 6d00 7000 6f00 7200 7400 6500 7200 736d  m.p.o.r.t.e.r.sm
-000067b0: 6f44 4462 6c6f 6200 0000 0890 22c3 eb97  oDDblob....."...
-000067c0: ffc4 4100 0000 0e00 7000 6f00 7300 6500  ..A.....p.o.s.e.
-000067d0: 5f00 6900 6d00 7000 6f00 7200 7400 6500  _.i.m.p.o.r.t.e.
-000067e0: 7200 736d 6f64 4462 6c6f 6200 0000 0890  r.smodDblob.....
-000067f0: 22c3 eb97 ffc4 4100 0000 0e00 7000 6f00  ".....A.....p.o.
-00006800: 7300 6500 5f00 6900 6d00 7000 6f00 7200  s.e._.i.m.p.o.r.
-00006810: 7400 6500 7200 7370 6831 5363 6f6d 7000  t.e.r.sph1Scomp.
-00006820: 0000 0000 04a0 0000 0000 0e00 7000 6f00  ............p.o.
-00006830: 7300 6500 5f00 6900 6d00 7000 6f00 7200  s.e._.i.m.p.o.r.
-00006840: 7400 6500 7200 7376 5372 6e6c 6f6e 6700  t.e.r.svSrnlong.
-00006850: 0000 0100 0000 0f00 7000 6f00 7300 6500  ........p.o.s.e.
-00006860: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-00006870: 6f00 7200 7362 7773 7062 6c6f 6200 0000  o.r.sbwspblob...
-00006880: c962 706c 6973 7430 30d7 0102 0304 0506  .bplist00.......
-00006890: 0708 080a 080a 0d0a 5d53 686f 7753 7461  ........]ShowSta
-000068a0: 7475 7342 6172 5b53 686f 7750 6174 6862  tusBar[ShowPathb
-000068b0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
-000068c0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
-000068d0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
-000068e0: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
-000068f0: 686f 7753 6964 6562 6172 0808 0908 095f  howSidebar....._
-00006900: 1018 7b7b 3635 372c 2032 3730 7d2c 207b  ..{{657, 270}, {
-00006910: 3938 392c 2034 3336 7d7d 0908 1725 313d  989, 436}}...%1=
-00006920: 4960 6d79 7a7b 7c7d 7e99 0000 0000 0000  I`myz{|}~.......
-00006930: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00006940: 0000 0000 0000 0000 009a 0000 000f 0070  ...............p
-00006950: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
-00006960: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-00006970: 636f 6d70 0000 0000 0000 84be 0000 000f  comp............
-00006980: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
-00006990: 0063 0065 0073 0073 006f 0072 0073 6d6f  .c.e.s.s.o.r.smo
-000069a0: 4444 626c 6f62 0000 0008 9e55 85d0 97fe  DDblob.....U....
-000069b0: c441 0000 000f 0070 006f 0073 0065 005f  .A.....p.o.s.e._
-000069c0: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
-000069d0: 0072 0073 6d6f 6444 626c 6f62 0000 0008  .r.smodDblob....
-000069e0: 9e55 85d0 97fe c441 0000 000f 0070 006f  .U.....A.....p.o
-000069f0: 0073 0065 005f 0070 0072 006f 0063 0065  .s.e._.p.r.o.c.e
-00006a00: 0073 0073 006f 0072 0073 7068 3153 636f  .s.s.o.r.sph1Sco
-00006a10: 6d70 0000 0000 0000 d000 0000 000f 0070  mp.............p
-00006a20: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
-00006a30: 0065 0073 0073 006f 0072 0073 7653 726e  .e.s.s.o.r.svSrn
-00006a40: 6c6f 6e67 0000 0001 0000 0009 0072 006f  long.........r.o
-00006a50: 0069 005f 0074 006f 006f 006c 0073 6277  .i._.t.o.o.l.sbw
-00006a60: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
-00006a70: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
-00006a80: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00006a90: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
-00006aa0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00006ab0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00006ac0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00006ad0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00006ae0: 6261 7208 0809 0809 5f10 187b 7b36 3537  bar....._..{{657
-00006af0: 2c20 3237 307d 2c20 7b39 3839 2c20 3433  , 270}, {989, 43
-00006b00: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
-00006b10: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
-00006b20: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-00006b30: 0000 9a00 0000 0900 7200 6f00 6900 5f00  ........r.o.i._.
-00006b40: 7400 6f00 6f00 6c00 736c 6731 5363 6f6d  t.o.o.l.slg1Scom
-00006b50: 7000 0000 0000 0425 3e00 0000 0900 7200  p......%>.....r.
-00006b60: 6f00 6900 5f00 7400 6f00 6f00 6c00 736c  o.i._.t.o.o.l.sl
-00006b70: 7376 4362 6c6f 6200 0002 7862 706c 6973  svCblob...xbplis
-00006b80: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
-00006b90: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
-00006ba0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00006bb0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00006bc0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00006bd0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
-00006be0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00006bf0: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
-00006c00: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
-00006c10: 09ab 0c15 1a1f 2328 2d32 373c 41d4 0d0e  ......#(-27<A...
-00006c20: 0f10 1112 0a0a 5a69 6465 6e74 6966 6965  ......Zidentifie
-00006c30: 7255 7769 6474 6859 6173 6365 6e64 696e  rUwidthYascendin
-00006c40: 6757 7669 7369 626c 6554 6e61 6d65 10d0  gWvisibleTname..
-00006c50: 0909 d40d 0e0f 1016 1718 1858 7562 6971  ...........Xubiq
-00006c60: 7569 7479 1023 0808 d40d 0e0f 101b 1c18  uity.#..........
-00006c70: 0a5c 6461 7465 4d6f 6469 6669 6564 10b5  .\dateModified..
-00006c80: 0809 d40d 0e0f 1020 1c18 185b 6461 7465  ....... ...[date
-00006c90: 4372 6561 7465 6408 08d4 0d0e 0f10 2425  Created.......$%
-00006ca0: 180a 5473 697a 6510 6108 09d4 0d0e 0f10  ..Tsize.a.......
-00006cb0: 292a 0a0a 546b 696e 6410 7309 09d4 0d0e  )*..Tkind.s.....
-00006cc0: 0f10 2e2f 0a18 556c 6162 656c 1064 0908  .../..Ulabel.d..
-00006cd0: d40d 0e0f 1033 340a 1857 7665 7273 696f  .....34..Wversio
-00006ce0: 6e10 4b09 08d4 0d0e 0f10 3839 0a18 5863  n.K.......89..Xc
-00006cf0: 6f6d 6d65 6e74 7311 012c 0908 d40d 0e0f  omments..,......
-00006d00: 103d 3e18 185e 6461 7465 4c61 7374 4f70  .=>..^dateLastOp
-00006d10: 656e 6564 10c8 0808 d40d 0e0f 1042 1c18  ened.........B..
-00006d20: 1859 6461 7465 4164 6465 6408 0808 2340  .YdateAdded...#@
-00006d30: 2800 0000 0000 0054 6e61 6d65 0910 0100  (......Tname....
-00006d40: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
-00006d50: 7700 8c00 9500 9600 a200 ab00 b600 bc00  w...............
-00006d60: c600 ce00 d300 d500 d600 d700 e000 e900  ................
-00006d70: eb00 ec00 ed00 f601 0301 0501 0601 0701  ................
-00006d80: 1001 1c01 1d01 1e01 2701 2c01 2e01 2f01  ........'.,.../.
-00006d90: 3001 3901 3e01 4001 4101 4201 4b01 5101  0.9.>.@.A.B.K.Q.
-00006da0: 5301 5401 5501 5e01 6601 6801 6901 6a01  S.T.U.^.f.h.i.j.
-00006db0: 7301 7c01 7f01 8001 8101 8a01 9901 9b01  s.|.............
-00006dc0: 9c01 9d01 a601 b001 b101 b201 b301 bc01  ................
-00006dd0: c101 c200 0000 0000 0002 0100 0000 0000  ................
-00006de0: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00006df0: 0001 c410 03d4 1819 1a1b 1c35 0b37 0810  ...........5.7..
-00006e00: 6409 1005 d418 191a 1b0b 3a0b 3c09 1073  d.........:.<..s
-00006e10: 0910 04d4 1819 1a1b 1c3f 0b41 0810 4b09  .........?.A..K.
-00006e20: 1006 d418 191a 1b0b 440b 4609 1101 2709  ........D.F...'.
-00006e30: 1000 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
-00006e40: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
-00006e50: 0000 0000 0800 1d00 3000 4200 4a00 5e00  ........0.B.J.^.
-00006e60: 7000 7900 8b00 9600 9f00 b400 b500 b600  p.y.............
-00006e70: c900 d200 e100 ee00 fa00 ff01 0501 0a01  ................
-00006e80: 1201 1701 2001 2801 2e01 3801 3e01 3f01  .... .(...8.>.?.
-00006e90: 4201 4301 4501 4e01 4f01 5101 5201 5401  B.C.E.N.O.Q.R.T.
-00006ea0: 5d01 5e01 6001 6101 6301 6c01 6d01 6e01  ].^.`.a.c.l.m.n.
-00006eb0: 7001 7901 7a01 7c01 7d01 7f01 8801 8901  p.y.z.|.}.......
-00006ec0: 8b01 8c01 8e01 9701 9801 9a01 9b01 9d01  ................
-00006ed0: a601 a701 a901 aa01 ac01 b501 b601 b901  ................
-00006ee0: ba01 bc01 bd01 c601 cf01 d400 0000 0000  ................
-00006ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00006f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
-00006f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
-00006f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
-00006f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
-00006f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
-00006f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
-00006f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00006f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
-00006f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
-00006f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00006fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00006fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
-00006fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00006fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00006fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00006000: 0000 0000 0000 0000 0000 0010 0000 0012  ................
+00006010: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
+00006020: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
+00006030: 0072 0073 6c73 7670 626c 6f62 0000 029d  .r.slsvpblob....
+00006040: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00006050: 0809 0a0b 0c0d 1f48 4948 4a0c 2658 6963  .......HIHJ.&Xic
+00006060: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00006070: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00006080: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00006090: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+000060a0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+000060b0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+000060c0: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
+000060d0: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
+000060e0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+000060f0: 7369 6f6e 2340 3000 0000 0000 0009 d90e  sion#@0.........
+00006100: 0f10 1112 1314 1516 1720 252a 2e33 383d  ......... %*.38=
+00006110: 4258 636f 6d6d 656e 7473 5e64 6174 654c  BXcomments^dateL
+00006120: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
+00006130: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
+00006140: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
+00006150: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+00006160: 1819 1a1b 1c1d 0c1f 5569 6e64 6578 5577  ........UindexUw
+00006170: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+00006180: 6973 6962 6c65 1007 1101 2c09 08d4 1819  isible....,.....
+00006190: 1a1b 2122 1f1f 1008 10c8 0808 d418 191a  ..!"............
+000061a0: 1b26 271f 0c10 0110 b508 09d4 1819 1a1b  .&'.............
+000061b0: 2b27 1f1f 1002 0808 d418 191a 1b2f 301f  +'.........../0.
+000061c0: 0c10 0310 6108 09d4 1819 1a1b 3435 0c1f  ....a.......45..
+000061d0: 1005 1064 0908 d418 191a 1b39 3a0c 0c10  ...d.......9:...
+000061e0: 0410 7309 09d4 1819 1a1b 3e3f 0c1f 1006  ..s.......>?....
+000061f0: 104b 0908 d418 191a 1b43 440c 0c10 0011  .K.......CD.....
+00006200: 01c7 0909 0823 0000 0000 0000 0000 2340  .....#........#@
+00006210: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
+00006220: 6669 6564 0900 0800 1d00 2600 3800 4000  fied......&.8.@.
+00006230: 5400 6600 6f00 8100 8c00 9f00 b400 bd00  T.f.o...........
+00006240: be00 d100 da00 e900 f601 0201 0701 0d01  ................
+00006250: 1201 1a01 1f01 2801 2e01 3401 3e01 4601  ......(...4.>.F.
+00006260: 4801 4b01 4c01 4d01 5601 5801 5a01 5b01  H.K.L.M.V.X.Z.[.
+00006270: 5c01 6501 6701 6901 6a01 6b01 7401 7601  \.e.g.i.j.k.t.v.
+00006280: 7701 7801 8101 8301 8501 8601 8701 9001  w.x.............
+00006290: 9201 9401 9501 9601 9f01 a101 a301 a401  ................
+000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
+000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
+000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
+000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
+000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
+000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
+00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
+00006310: 08b3 7108 4149 05c5 4100 0000 1200 6600  ..q.AI..A.....f.
+00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
+00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
+00006340: 736d 6f64 4462 6c6f 6200 0000 0866 04c9  smodDblob....f..
+00006350: 1d50 01c5 4100 0000 1200 6600 6500 6100  .P..A.....f.e.a.
+00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
+00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
+00006380: 5363 6f6d 7000 0000 0000 15d0 0000 0000  Scomp...........
+00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
+000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
+000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
+000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
+000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
+000063e0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+00006400: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+00006410: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+00006420: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00006430: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00006440: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00006450: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+00006460: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
+00006470: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
+00006480: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
+00006490: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+000064a0: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
+000064b0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
+000064c0: 6e00 676c 6731 5363 6f6d 7000 0000 0000  n.glg1Scomp.....
+000064d0: 019c f300 0000 0900 6c00 6100 6200 6500  ........l.a.b.e.
+000064e0: 6c00 6c00 6900 6e00 676c 7376 4362 6c6f  l.l.i.n.glsvCblo
+000064f0: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
+00006500: 0304 0506 0708 090a 0b16 4647 480a 5f10  ..........FGH._.
+00006510: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00006520: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+00006530: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00006540: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00006550: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
+00006560: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
+00006570: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00006580: 7310 0109 ab0c 151a 1f23 282d 3237 3c41  s........#(-27<A
+00006590: d40d 0e0f 100a 120a 1457 7669 7369 626c  .........Wvisibl
+000065a0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+000065b0: 675a 6964 656e 7469 6669 6572 0911 01c7  gZidentifier....
+000065c0: 0954 6e61 6d65 d40d 0e0f 1016 1716 1908  .Tname..........
+000065d0: 1023 0858 7562 6971 7569 7479 d40d 0e0f  .#.Xubiquity....
+000065e0: 100a 1c16 1e09 10b5 085c 6461 7465 4d6f  .........\dateMo
+000065f0: 6469 6669 6564 d40d 0e0f 1016 1c16 2208  dified........".
+00006600: 085b 6461 7465 4372 6561 7465 64d4 0d0e  .[dateCreated...
+00006610: 0f10 0a25 1627 0910 6108 5473 697a 65d4  ...%.'..a.Tsize.
+00006620: 0d0e 0f10 0a2a 0a2c 0910 7309 546b 696e  .....*.,..s.Tkin
+00006630: 64d4 0d0e 0f10 162f 0a31 0810 6409 556c  d....../.1..d.Ul
+00006640: 6162 656c d40d 0e0f 1016 340a 3608 104b  abel......4.6..K
+00006650: 0957 7665 7273 696f 6ed4 0d0e 0f10 1639  .Wversion......9
+00006660: 0a3b 0811 012c 0958 636f 6d6d 656e 7473  .;...,.Xcomments
+00006670: d40d 0e0f 1016 3e16 4008 10c8 085e 6461  ......>.@....^da
+00006680: 7465 4c61 7374 4f70 656e 6564 d40d 0e0f  teLastOpened....
+00006690: 1016 1c16 4408 0859 6461 7465 4164 6465  ....D..YdateAdde
+000066a0: 6408 2340 2800 0000 0000 0054 6e61 6d65  d.#@(......Tname
+000066b0: 2340 3000 0000 0000 0009 0008 0019 002e  #@0.............
+000066c0: 0040 0048 005c 0065 0070 0079 008c 008e  .@.H.\.e.p.y....
+000066d0: 008f 009b 00a4 00ac 00b2 00bc 00c7 00c8  ................
+000066e0: 00cb 00cc 00d1 00da 00db 00dd 00de 00e7  ................
+000066f0: 00f0 00f1 00f3 00f4 0101 010a 010b 010c  ................
+00006700: 0118 0121 0122 0124 0125 012a 0133 0134  ...!.".$.%.*.3.4
+00006710: 0136 0137 013c 0145 0146 0148 0149 014f  .6.7.<.E.F.H.I.O
+00006720: 0158 0159 015b 015c 0164 016d 016e 0171  .X.Y.[.\.d.m.n.q
+00006730: 0172 017b 0184 0185 0187 0188 0197 01a0  .r.{............
+00006740: 01a1 01a2 01ac 01ad 01b6 01bb 01c4 0000  ................
+00006750: 0000 0000 0201 0000 0000 0000 004a 0000  .............J..
+00006760: 0000 0000 0000 0000 0000 0000 01c5 0000  ................
+00006770: 0009 006c 0061 0062 0065 006c 006c 0069  ...l.a.b.e.l.l.i
+00006780: 006e 0067 6c73 7670 626c 6f62 0000 025e  .n.glsvpblob...^
+00006790: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+000067a0: 0809 0a0b 1d45 4647 0a5f 1012 7669 6577  .....EFG._..view
+000067b0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+000067c0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000067d0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000067e0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+000067f0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00006800: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
+00006810: 656c 6174 6976 6544 6174 6573 1001 09d9  elativeDates....
+00006820: 0c0d 0e0f 1011 1213 1415 1e23 272b 3035  ...........#'+05
+00006830: 3a3f 5863 6f6d 6d65 6e74 735e 6461 7465  :?Xcomments^date
+00006840: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
+00006850: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
+00006860: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
+00006870: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
+00006880: d416 1718 191a 1b0a 1d55 696e 6465 7855  .........UindexU
+00006890: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+000068a0: 7669 7369 626c 6510 0711 012c 0908 d416  visible....,....
+000068b0: 1718 191f 201d 1d10 0810 c808 08d4 1617  .... ...........
+000068c0: 1819 0924 1d0a 10b5 0809 d416 1718 1928  ...$...........(
+000068d0: 241d 1d10 0208 08d4 1617 1819 2c2d 1d0a  $...........,-..
+000068e0: 1003 1061 0809 d416 1718 1931 320a 1d10  ...a.......12...
+000068f0: 0510 6409 08d4 1617 1819 3637 0a0a 1004  ..d.......67....
+00006900: 1073 0909 d416 1718 193b 3c0a 1d10 0610  .s.......;<.....
+00006910: 4b09 08d4 1617 1819 4041 0a0a 1000 1101  K.......@A......
+00006920: c709 0908 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
+00006930: 6d65 2340 3000 0000 0000 0009 0008 0019  me#@0...........
+00006940: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
+00006950: 008e 008f 00a2 00ab 00ba 00c7 00d3 00d8  ................
+00006960: 00de 00e3 00eb 00f0 00f9 00ff 0105 010f  ................
+00006970: 0117 0119 011c 011d 011e 0127 0129 012b  ...........'.).+
+00006980: 012c 012d 0136 0138 0139 013a 0143 0145  .,.-.6.8.9.:.C.E
+00006990: 0146 0147 0150 0152 0154 0155 0156 015f  .F.G.P.R.T.U.V._
+000069a0: 0161 0163 0164 0165 016e 0170 0172 0173  .a.c.d.e.n.p.r.s
+000069b0: 0174 017d 017f 0181 0182 0183 018c 018e  .t.}............
+000069c0: 0191 0192 0193 0194 019d 01a2 01ab 0000  ................
+000069d0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
+000069e0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
+000069f0: 0009 006c 0061 0062 0065 006c 006c 0069  ...l.a.b.e.l.l.i
+00006a00: 006e 0067 6d6f 4444 626c 6f62 0000 0008  .n.gmoDDblob....
+00006a10: c446 b51b 4305 c541 0000 0009 006c 0061  .F..C..A.....l.a
+00006a20: 0062 0065 006c 006c 0069 006e 0067 6d6f  .b.e.l.l.i.n.gmo
+00006a30: 6444 626c 6f62 0000 0008 c446 b51b 4305  dDblob.....F..C.
+00006a40: c541 0000 0009 006c 0061 0062 0065 006c  .A.....l.a.b.e.l
+00006a50: 006c 0069 006e 0067 7068 3153 636f 6d70  .l.i.n.gph1Scomp
+00006a60: 0000 0000 0001 e000 0000 0009 006c 0061  .............l.a
+00006a70: 0062 0065 006c 006c 0069 006e 0067 7653  .b.e.l.l.i.n.gvS
+00006a80: 726e 6c6f 6e67 0000 0001 0000 0006 006d  rnlong.........m
+00006a90: 0069 0078 0069 006e 0073 6277 7370 626c  .i.x.i.n.sbwspbl
+00006aa0: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
+00006ab0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00006ac0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00006ad0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00006ae0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00006af0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00006b00: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00006b10: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00006b20: 0809 0809 5f10 197b 7b32 3332 2c20 3139  ...._..{{232, 19
+00006b30: 317d 2c20 7b31 3330 322c 2037 3134 7d7d  1}, {1302, 714}}
+00006b40: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+00006b50: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+00006b60: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+00006b70: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
+00006b80: 6c67 3153 636f 6d70 0000 0000 000a 5c2e  lg1Scomp......\.
+00006b90: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
+00006ba0: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
+00006bb0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00006bc0: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
+00006bd0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00006be0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00006bf0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00006c00: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00006c10: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00006c20: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00006c30: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+00006c40: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
+00006c50: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
+00006c60: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+00006c70: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+00006c80: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
+00006c90: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+00006ca0: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
+00006cb0: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
+00006cc0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+00006cd0: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
+00006ce0: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
+00006cf0: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
+00006d00: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
+00006d10: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
+00006d20: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
+00006d30: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
+00006d40: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
+00006d50: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+00006d60: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
+00006d70: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+00006d80: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
+00006d90: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
+00006da0: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
+00006db0: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
+00006dc0: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
+00006dd0: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
+00006de0: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
+00006df0: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
+00006e00: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
+00006e10: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
+00006e20: da01 db00 0000 0000 0002 0100 0000 0000  ................
+00006e30: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
+00006e40: 0001 dd01 7101 7201 7b01 8401 8501 8701  ....q.r.{.......
+00006e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
+00006e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
+00006e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00006e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
+00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
-00007010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
-00007020: 0073 6d6f 4444 626c 6f62 0000 0008 2506  .smoDDblob....%.
-00007030: b721 6f01 c541 0000 0009 0072 006f 0069  .!o..A.....r.o.i
-00007040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-00007050: 626c 6f62 0000 0008 b5b2 2bb8 e5fc c441  blob......+....A
-00007060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
-00007070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-00007080: 0000 0005 1000 0000 0009 0072 006f 0069  ...........r.o.i
-00007090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
-000070a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
-000070b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
-000070c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
-000070d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
-000070e0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
-000070f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00007100: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00007110: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00007120: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00007130: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00007140: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00007150: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00007160: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00007170: 7b33 322c 2031 3233 7d2c 207b 3132 3033  {32, 123}, {1203
-00007180: 2c20 3735 347d 7d09 0817 2531 3d49 606d  , 754}}...%1=I`m
-00007190: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-000071a0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000071b0: 0000 0000 0000 9a00 0000 1b00 7400 6800  ............t.h.
-000071c0: 6900 7200 6400 5f00 7000 6100 7200 7400  i.r.d._.p.a.r.t.
-000071d0: 7900 5f00 6c00 6100 6200 6500 6c00 5f00  y._.l.a.b.e.l._.
-000071e0: 6100 7000 7000 6500 6e00 6400 6500 7200  a.p.p.e.n.d.e.r.
-000071f0: 736c 6731 5363 6f6d 7000 0000 0000 021a  slg1Scomp.......
-00007200: b600 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
-00007210: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
-00007220: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
-00007230: 6500 6e00 6400 6500 7200 736c 7376 4362  e.n.d.e.r.slsvCb
-00007240: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
-00007250: 0102 0304 0506 0708 090a 0b16 4647 480a  ............FGH.
-00007260: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00007270: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-00007280: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00007290: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-000072a0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-000072b0: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
-000072c0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-000072d0: 7465 7310 0109 ab0c 151a 1f23 282d 3237  tes........#(-27
-000072e0: 3c41 d40d 0e0f 100a 120a 1457 7669 7369  <A.........Wvisi
-000072f0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00007300: 696e 675a 6964 656e 7469 6669 6572 0911  ingZidentifier..
-00007310: 01a6 0954 6e61 6d65 d40d 0e0f 1016 1716  ...Tname........
-00007320: 1908 1023 0858 7562 6971 7569 7479 d40d  ...#.Xubiquity..
-00007330: 0e0f 100a 1c16 1e09 10b5 085c 6461 7465  ...........\date
-00007340: 4d6f 6469 6669 6564 d40d 0e0f 1016 1c16  Modified........
-00007350: 2208 085b 6461 7465 4372 6561 7465 64d4  "..[dateCreated.
-00007360: 0d0e 0f10 0a25 1627 0910 6108 5473 697a  .....%.'..a.Tsiz
-00007370: 65d4 0d0e 0f10 0a2a 0a2c 0910 7309 546b  e......*.,..s.Tk
-00007380: 696e 64d4 0d0e 0f10 162f 0a31 0810 6409  ind....../.1..d.
-00007390: 556c 6162 656c d40d 0e0f 1016 340a 3608  Ulabel......4.6.
-000073a0: 104b 0957 7665 7273 696f 6ed4 0d0e 0f10  .K.Wversion.....
-000073b0: 1639 0a3b 0811 012c 0958 636f 6d6d 656e  .9.;...,.Xcommen
-000073c0: 7473 d40d 0e0f 1016 3e16 4008 10c8 085e  ts......>.@....^
-000073d0: 6461 7465 4c61 7374 4f70 656e 6564 d40d  dateLastOpened..
-000073e0: 0e0f 1016 1c16 4408 0859 6461 7465 4164  ......D..YdateAd
-000073f0: 6465 6408 2340 2800 0000 0000 0054 6e61  ded.#@(......Tna
-00007400: 6d65 2340 3000 0000 0000 0009 0008 0019  me#@0...........
-00007410: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
-00007420: 008e 008f 009b 00a4 00ac 00b2 00bc 00c7  ................
-00007430: 00c8 00cb 00cc 00d1 00da 00db 00dd 00de  ................
-00007440: 00e7 00f0 00f1 00f3 00f4 0101 010a 010b  ................
-00007450: 010c 0118 0121 0122 0124 0125 012a 0133  .....!.".$.%.*.3
-00007460: 0134 0136 0137 013c 0145 0146 0148 0149  .4.6.7.<.E.F.H.I
-00007470: 014f 0158 0159 015b 015c 0164 016d 016e  .O.X.Y.[.\.d.m.n
-00007480: 0171 0172 017b 0184 0185 0187 0188 0197  .q.r.{..........
-00007490: 01a0 01a1 01a2 01ac 01ad 01b6 01bb 01c4  ................
-000074a0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-000074b0: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-000074c0: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
-000074d0: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
-000074e0: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
-000074f0: 006e 0064 0065 0072 0073 6c73 7670 626c  .n.d.e.r.slsvpbl
-00007500: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
-00007510: 0203 0405 0607 0809 0a0b 1d45 4647 0a5f  ...........EFG._
-00007520: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00007530: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-00007540: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00007550: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00007560: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-00007570: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-00007580: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00007590: 6573 1001 09d9 0c0d 0e0f 1011 1213 1415  es..............
-000075a0: 1e23 272b 3035 3a3f 5863 6f6d 6d65 6e74  .#'+05:?Xcomment
-000075b0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-000075c0: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
-000075d0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-000075e0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-000075f0: 6e54 6e61 6d65 d416 1718 191a 1b0a 1d55  nTname.........U
-00007600: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
-00007610: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
-00007620: 012c 0908 d416 1718 191f 201d 1d10 0810  .,........ .....
-00007630: c808 08d4 1617 1819 0924 1d0a 10b5 0809  .........$......
-00007640: d416 1718 1928 241d 1d10 0208 08d4 1617  .....($.........
-00007650: 1819 2c2d 1d0a 1003 1061 0809 d416 1718  ..,-.....a......
-00007660: 1931 320a 1d10 0510 6409 08d4 1617 1819  .12.....d.......
-00007670: 3637 0a0a 1004 1073 0909 d416 1718 193b  67.....s.......;
-00007680: 3c0a 1d10 0610 4b09 08d4 1617 1819 4041  <.....K.......@A
-00007690: 0a0a 1000 1101 a609 0908 2340 2800 0000  ..........#@(...
-000076a0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-000076b0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-000076c0: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
-000076d0: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
-000076e0: 00ff 0105 010f 0117 0119 011c 011d 011e  ................
-000076f0: 0127 0129 012b 012c 012d 0136 0138 0139  .'.).+.,.-.6.8.9
-00007700: 013a 0143 0145 0146 0147 0150 0152 0154  .:.C.E.F.G.P.R.T
-00007710: 0155 0156 015f 0161 0163 0164 0165 016e  .U.V._.a.c.d.e.n
-00007720: 0170 0172 0173 0174 017d 017f 0181 0182  .p.r.s.t.}......
-00007730: 0183 018c 018e 0191 0192 0193 0194 019d  ................
-00007740: 01a2 01ab 0000 0000 0000 0201 0000 0000  ................
-00007750: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-00007760: 0000 01ac 0000 001b 0074 0068 0069 0072  .........t.h.i.r
-00007770: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
-00007780: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
-00007790: 0070 0065 006e 0064 0065 0072 0073 6d6f  .p.e.n.d.e.r.smo
-000077a0: 4444 626c 6f62 0000 0008 801f e384 2efe  DDblob..........
-000077b0: c441 0000 001b 0074 0068 0069 0072 0064  .A.....t.h.i.r.d
-000077c0: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
-000077d0: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
-000077e0: 0065 006e 0064 0065 0072 0073 6d6f 6444  .e.n.d.e.r.smodD
-000077f0: 626c 6f62 0000 0008 4c89 caff 10fc c441  blob....L......A
-00007800: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
-00007810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
-00007820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
-00007830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
-00007840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
-00007850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
-00007860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
-00007870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
-00007880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
-00007890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
-000078a0: 0000 00c6 6270 6c69 7374 3030 d701 0203  ....bplist00....
-000078b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-000078c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-000078d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-000078e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-000078f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00007900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00007910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00007920: 0809 5f10 157b 7b30 2c20 307d 2c20 7b31  .._..{{0, 0}, {1
-00007930: 3434 302c 2038 3737 7d7d 0908 1725 313d  440, 877}}...%1=
-00007940: 4960 6d79 7a7b 7c7d 7e96 0000 0000 0000  I`myz{|}~.......
-00007950: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00007960: 0000 0000 0000 0000 0097 0000 0002 0075  ...............u
-00007970: 0069 6473 636c 626f 6f6c 0100 0000 0200  .idsclbool......
-00007980: 7500 696c 6731 5363 6f6d 7000 0000 0000  u.ilg1Scomp.....
-00007990: 0bf8 5c00 0000 0200 7500 696c 7376 4362  ..\.....u.ilsvCb
-000079a0: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
-000079b0: 0102 0304 0506 0708 090a 0b16 4647 0a49  ............FG.I
-000079c0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-000079d0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-000079e0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-000079f0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00007a00: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00007a10: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00007a20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00007a30: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
-00007a40: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 110a  ..#(-27<A.......
-00007a50: 130a 5a69 6465 6e74 6966 6965 7259 6173  ..ZidentifierYas
-00007a60: 6365 6e64 696e 6755 7769 6474 6857 7669  cendingUwidthWvi
-00007a70: 7369 626c 6554 6e61 6d65 0911 0251 09d4  sibleTname...Q..
-00007a80: 100f 0e0d 1617 1619 0810 2308 5875 6269  ..........#.Xubi
-00007a90: 7175 6974 79d4 100e 0f0d 0a16 1d1e 0908  quity...........
-00007aa0: 10b5 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
-00007ab0: 100e 0f0d 1616 1d22 0808 5b64 6174 6543  ......."..[dateC
-00007ac0: 7265 6174 6564 d410 0e0f 0d0a 1626 2709  reated.......&'.
-00007ad0: 0810 6154 7369 7a65 d410 0e0f 0d0a 0a2b  ..aTsize.......+
-00007ae0: 2c09 0910 7354 6b69 6e64 d410 0e0f 0d16  ,...sTkind......
-00007af0: 0a30 3108 0910 6455 6c61 6265 6cd4 100e  .01...dUlabel...
-00007b00: 0f0d 160a 3536 0809 104b 5776 6572 7369  ....56...KWversi
-00007b10: 6f6e d410 0e0f 0d16 0a3a 3b08 0911 012c  on.......:;....,
-00007b20: 5863 6f6d 6d65 6e74 73d4 100e 0f0d 1616  Xcomments.......
-00007b30: 3f40 0808 10c8 5e64 6174 654c 6173 744f  ?@....^dateLastO
-00007b40: 7065 6e65 64d4 100f 0e0d 161d 1644 0808  pened........D..
-00007b50: 5964 6174 6541 6464 6564 0823 4028 0000  YdateAdded.#@(..
-00007b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
-00007b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-00007b80: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
-00007b90: 00d3 00d4 00d7 00d8 00e1 00e2 00e4 00e5  ................
-00007ba0: 00ee 00f7 00f8 00f9 00fb 0108 0111 0112  ................
-00007bb0: 0113 011f 0128 0129 012a 012c 0131 013a  .....(.).*.,.1.:
-00007bc0: 013b 013c 013e 0143 014c 014d 014e 0150  .;.<.>.C.L.M.N.P
-00007bd0: 0156 015f 0160 0161 0163 016b 0174 0175  .V._.`.a.c.k.t.u
-00007be0: 0176 0179 0182 018b 018c 018d 018f 019e  .v.y............
-00007bf0: 01a7 01a8 01a9 01b3 01b4 01bd 01c2 01c3  ................
-00007c00: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-00007c10: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-00007c20: 0000 0002 0075 0069 6c73 7670 626c 6f62  .....u.ilsvpblob
-00007c30: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
-00007c40: 0405 0607 0809 0a0b 1d46 470a 2458 6963  .........FG.$Xic
-00007c50: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00007c60: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00007c70: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00007c80: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00007c90: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-00007ca0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-00007cb0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00007cc0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
-00007cd0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
-00007ce0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
-00007cf0: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
-00007d00: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00007d10: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00007d20: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
-00007d30: 1a0a 1c1d 5569 6e64 6578 5961 7363 656e  ....UindexYascen
-00007d40: 6469 6e67 5577 6964 7468 5776 6973 6962  dingUwidthWvisib
-00007d50: 6c65 1007 0911 012c 08d4 1617 1819 1f1d  le.....,........
-00007d60: 211d 1008 0810 c808 d416 1718 1924 1d26  !............$.&
-00007d70: 0a10 0108 10b5 09d4 1617 1819 291d 261d  ............).&.
-00007d80: 1002 0808 d416 1718 192d 1d2f 0a10 0308  .........-./....
-00007d90: 1061 09d4 1617 1819 320a 341d 1005 0910  .a......2.4.....
-00007da0: 6408 d416 1718 1937 0a39 0a10 0409 1073  d......7.9.....s
-00007db0: 09d4 1617 1819 3c0a 3e1d 1006 0910 4b08  ......<.>.....K.
-00007dc0: d419 1718 160a 0a43 4409 0911 0251 1000  .......CD....Q..
-00007dd0: 0823 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
-00007de0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00007df0: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
-00007e00: 00da 00df 00e5 00ea 00f2 00f7 0100 0106  ................
-00007e10: 0110 0116 011e 0120 0121 0124 0125 012e  ....... .!.$.%..
-00007e20: 0130 0131 0133 0134 013d 013f 0140 0142  .0.1.3.4.=.?.@.B
-00007e30: 0143 014c 014e 014f 0150 0159 015b 015c  .C.L.N.O.P.Y.[.\
-00007e40: 015e 015f 0168 016a 016b 016d 016e 0177  .^._.h.j.k.m.n.w
-00007e50: 0179 017a 017c 017d 0186 0188 0189 018b  .y.z.|.}........
-00007e60: 018c 0195 0196 0197 019a 019c 019d 01a6  ................
-00007e70: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
-00007e80: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00007e90: 01ac 0000 0002 0075 0069 6d6f 4444 626c  .......u.imoDDbl
-00007ea0: 6f62 0000 0008 6da9 747c 5e01 c541 0000  ob....m.t|^..A..
-00007eb0: 0002 0075 0069 6d6f 6444 626c 6f62 0000  ...u.imodDblob..
-00007ec0: 0008 6da9 747c 5e01 c541 0000 0002 0075  ..m.t|^..A.....u
-00007ed0: 0069 7068 3153 636f 6d70 0000 0000 000f  .iph1Scomp......
-00007ee0: 1000 bc01 bd01 c601 cf01 d400 0000 0000  ................
-00007ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00007f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
-00007f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
-00007f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
-00007f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
-00007f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
-00007f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
-00007f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00007f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
-00007f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
-00007f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00007fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00007fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
-00007fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00007fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00007fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
+00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
+00007020: 626c 6f62 0000 0008 0432 5913 6f05 c541  blob.....2Y.o..A
+00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
+00007040: 6d6f 6444 626c 6f62 0000 0008 3b9d 9b1a  modDblob....;...
+00007050: 4405 c541 0000 0006 006d 0069 0078 0069  D..A.....m.i.x.i
+00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
+00007070: 000b 6000 0000 0006 006d 0069 0078 0069  ..`......m.i.x.i
+00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
+00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
+000070a0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
+000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+000070f0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00007100: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00007120: 6261 7208 0809 0809 5f10 197b 7b32 3332  bar....._..{{232
+00007130: 2c20 3139 317d 2c20 7b31 3330 322c 2037  , 191}, {1302, 7
+00007140: 3134 7d7d 0908 1725 313d 4960 6d79 7a7b  14}}...%1=I`myz{
+00007150: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
+00007160: 0000 000f 0000 0000 0000 0000 0000 0000  ................
+00007170: 0000 009b 0000 0005 006d 006f 0064 0065  .........m.o.d.e
+00007180: 006c 6c67 3153 636f 6d70 0000 0000 0001  .llg1Scomp......
+00007190: 1648 0000 0005 006d 006f 0064 0065 006c  .H.....m.o.d.e.l
+000071a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
+000071b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+000071c0: 1846 470a 4958 6963 6f6e 5369 7a65 5f10  .FG.IXiconSize_.
+000071d0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000071e0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000071f0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00007200: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00007210: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00007220: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00007230: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+00007240: 0009 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
+00007250: 0e0f 1011 0a13 0a5a 6964 656e 7469 6669  .......Zidentifi
+00007260: 6572 5961 7363 656e 6469 6e67 5577 6964  erYascendingUwid
+00007270: 7468 5776 6973 6962 6c65 546e 616d 6509  thWvisibleTname.
+00007280: 1101 c709 d40d 0f0e 1016 1718 1858 7562  .............Xub
+00007290: 6971 7569 7479 1023 0808 d40d 0e0f 101b  iquity.#........
+000072a0: 181d 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+000072b0: 0810 b509 d40d 0e0f 1020 181d 185b 6461  ......... ...[da
+000072c0: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
+000072d0: 2418 260a 5473 697a 6508 1061 09d4 0d0e  $.&.Tsize..a....
+000072e0: 0f10 290a 2b0a 546b 696e 6409 1073 09d4  ..).+.Tkind..s..
+000072f0: 0d0e 0f10 2e0a 3018 556c 6162 656c 0910  ......0.Ulabel..
+00007300: 6408 d40d 0e0f 1033 0a35 1857 7665 7273  d......3.5.Wvers
+00007310: 696f 6e09 104b 08d4 0d0e 0f10 380a 3a18  ion..K......8.:.
+00007320: 5863 6f6d 6d65 6e74 7309 1101 2c08 d40d  Xcomments...,...
+00007330: 0e0f 103d 183f 185e 6461 7465 4c61 7374  ...=.?.^dateLast
+00007340: 4f70 656e 6564 0810 c808 d40d 0f0e 1042  Opened.........B
+00007350: 1d18 1859 6461 7465 4164 6465 6408 0808  ...YdateAdded...
+00007360: 2340 2800 0000 0000 0054 6e61 6d65 0910  #@(......Tname..
+00007370: 0100 0800 1900 2200 3400 3c00 5000 5900  ......".4.<.P.Y.
+00007380: 6400 7700 8c00 9500 9600 a200 ab00 b600  d.w.............
+00007390: c000 c600 ce00 d300 d400 d700 d800 e100  ................
+000073a0: ea00 ec00 ed00 ee00 f701 0401 0501 0701  ................
+000073b0: 0801 1101 1d01 1e01 1f01 2801 2d01 2e01  ..........(.-...
+000073c0: 3001 3101 3a01 3f01 4001 4201 4301 4c01  0.1.:.?.@.B.C.L.
+000073d0: 5201 5301 5501 5601 5f01 6701 6801 6a01  R.S.U.V._.g.h.j.
+000073e0: 6b01 7401 7d01 7e01 8101 8201 8b01 9a01  k.t.}.~.........
+000073f0: 9b01 9d01 9e01 a701 b101 b201 b301 b401  ................
+00007400: bd01 c201 c300 0000 0000 0002 0100 0000  ................
+00007410: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
+00007420: 0000 0001 c500 0000 0500 6d00 6f00 6400  ..........m.o.d.
+00007430: 6500 6c6c 7376 7062 6c6f 6200 0002 5e62  e.llsvpblob...^b
+00007440: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+00007450: 090a 0b1a 4647 0a27 5869 636f 6e53 697a  ....FG.'XiconSiz
+00007460: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
+00007470: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00007480: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00007490: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+000074a0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+000074b0: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
+000074c0: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
+000074d0: 0000 0000 09d9 0c0d 0e0f 1011 1213 1415  ................
+000074e0: 1e23 282c 3136 3b40 5863 6f6d 6d65 6e74  .#(,16;@Xcomment
+000074f0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+00007500: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
+00007510: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+00007520: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+00007530: 6e54 6e61 6d65 d416 1718 191a 0a1c 1d57  nTname.........W
+00007540: 7669 7369 626c 6559 6173 6365 6e64 696e  visibleYascendin
+00007550: 6755 7769 6474 6855 696e 6465 7808 0911  gUwidthUindex...
+00007560: 012c 1007 d416 1718 191a 1a21 2208 0810  .,.........!"...
+00007570: c810 08d4 1617 1819 0a1a 2627 0908 10b5  ..........&'....
+00007580: 1001 d416 1718 191a 1a26 2b08 0810 02d4  .........&+.....
+00007590: 1617 1819 0a1a 2f30 0908 1061 1003 d416  ....../0...a....
+000075a0: 1718 191a 0a34 3508 0910 6410 05d4 1617  .....45...d.....
+000075b0: 1819 0a0a 393a 0909 1073 1004 d416 1718  ....9:...s......
+000075c0: 191a 0a3e 3f08 0910 4b10 06d4 1617 1819  ...>?...K.......
+000075d0: 0a0a 4344 0909 1101 c710 0008 2340 2800  ..CD........#@(.
+000075e0: 0000 0000 0054 6e61 6d65 0900 0800 1900  .....Tname......
+000075f0: 2200 3400 3c00 5000 5900 6400 7700 8c00  ".4.<.P.Y.d.w...
+00007600: 9500 9600 a900 b200 c100 ce00 da00 df00  ................
+00007610: e500 ea00 f200 f701 0001 0801 1201 1801  ................
+00007620: 1e01 1f01 2001 2301 2501 2e01 2f01 3001  .... .#.%.../.0.
+00007630: 3201 3401 3d01 3e01 3f01 4101 4301 4c01  2.4.=.>.?.A.C.L.
+00007640: 4d01 4e01 5001 5901 5a01 5b01 5d01 5f01  M.N.P.Y.Z.[.]._.
+00007650: 6801 6901 6a01 6c01 6e01 7701 7801 7901  h.i.j.l.n.w.x.y.
+00007660: 7b01 7d01 8601 8701 8801 8a01 8c01 9501  {.}.............
+00007670: 9601 9701 9a01 9c01 9d01 a601 ab00 0000  ................
+00007680: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+00007690: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+000076a0: 0500 6d00 6f00 6400 6500 6c6d 6f44 4462  ..m.o.d.e.lmoDDb
+000076b0: 6c6f 6200 0000 08dc c0ca 73c2 04c5 4100  lob.......s...A.
+000076c0: 0000 0500 6d00 6f00 6400 6500 6c6d 6f64  ....m.o.d.e.lmod
+000076d0: 4462 6c6f 6200 0000 087a 22ce b222 02c5  Dblob....z".."..
+000076e0: 4100 0000 0500 6d00 6f00 6400 6500 6c70  A.....m.o.d.e.lp
+000076f0: 6831 5363 6f6d 7000 0000 0000 0140 0000  h1Scomp......@..
+00007700: 0000 0500 6d00 6f00 6400 6500 6c76 5372  ....m.o.d.e.lvSr
+00007710: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
+00007720: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
+00007730: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
+00007740: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00007750: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+00007760: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+00007770: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+00007780: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00007790: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+000077a0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+000077b0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+000077c0: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
+000077d0: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
+000077e0: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
+000077f0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00007800: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
+00007810: 0d00 6f00 7500 7400 6c00 6900 6500 7200  ..o.u.t.l.i.e.r.
+00007820: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
+00007830: 6f6d 7000 0000 0000 0124 b500 0000 0d00  omp......$......
+00007840: 6f00 7500 7400 6c00 6900 6500 7200 5f00  o.u.t.l.i.e.r._.
+00007850: 7400 6f00 6f00 6c00 736c 7376 4362 6c6f  t.o.o.l.slsvCblo
+00007860: 6200 0002 b062 706c 6973 7430 30da 0102  b....bplist00...
+00007870: 0304 0506 0708 090a 0b0c 0d18 4849 484a  ............HIHJ
+00007880: 0c4c 5f10 1276 6965 774f 7074 696f 6e73  .L_..viewOptions
+00007890: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+000078a0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+000078b0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+000078c0: 5369 7a65 735f 100f 7363 726f 6c6c 506f  Sizes_..scrollPo
+000078d0: 7369 7469 6f6e 5958 7465 7874 5369 7a65  sitionYXtextSize
+000078e0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000078f0: 6e58 5a73 6f72 7443 6f6c 756d 6e5f 1010  nXZsortColumn_..
+00007900: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00007910: 5869 636f 6e53 697a 6510 0109 ab0e 171c  XiconSize.......
+00007920: 2125 2a2f 3439 3e43 d40f 1011 1213 140c  !%*/49>C........
+00007930: 0c5a 6964 656e 7469 6669 6572 5577 6964  .ZidentifierUwid
+00007940: 7468 5961 7363 656e 6469 6e67 5776 6973  thYascendingWvis
+00007950: 6962 6c65 546e 616d 6511 01c7 0909 d412  ibleTname.......
+00007960: 1011 0f18 1918 1b08 1023 0858 7562 6971  .........#.Xubiq
+00007970: 7569 7479 d412 1011 0f0c 1e18 2009 10b5  uity........ ...
+00007980: 085c 6461 7465 4d6f 6469 6669 6564 d412  .\dateModified..
+00007990: 1011 0f18 1e18 2408 085b 6461 7465 4372  ......$..[dateCr
+000079a0: 6561 7465 64d4 1210 110f 0c27 1829 0910  eated......'.)..
+000079b0: 6108 5473 697a 65d4 1210 110f 0c2c 0c2e  a.Tsize......,..
+000079c0: 0910 7309 546b 696e 64d4 1210 110f 1831  ..s.Tkind......1
+000079d0: 0c33 0810 6409 556c 6162 656c d412 1011  .3..d.Ulabel....
+000079e0: 0f18 360c 3808 104b 0957 7665 7273 696f  ..6.8..K.Wversio
+000079f0: 6ed4 1210 110f 183b 0c3d 0811 012c 0958  n......;.=...,.X
+00007a00: 636f 6d6d 656e 7473 d412 1011 0f18 4018  comments......@.
+00007a10: 4208 10c8 085e 6461 7465 4c61 7374 4f70  B....^dateLastOp
+00007a20: 656e 6564 d412 1011 0f18 1e18 4608 0859  ened........F..Y
+00007a30: 6461 7465 4164 6465 6408 2300 0000 0000  dateAdded.#.....
+00007a40: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00007a50: 6509 2340 3000 0000 0000 0000 0800 1d00  e.#@0...........
+00007a60: 3200 4400 4c00 6000 7200 7b00 8d00 9800  2.D.L.`.r.{.....
+00007a70: ab00 b400 b600 b700 c300 cc00 d700 dd00  ................
+00007a80: e700 ef00 f400 f700 f800 f901 0201 0301  ................
+00007a90: 0501 0601 0f01 1801 1901 1b01 1c01 2901  ..............).
+00007aa0: 3201 3301 3401 4001 4901 4a01 4c01 4d01  2.3.4.@.I.J.L.M.
+00007ab0: 5201 5b01 5c01 5e01 5f01 6401 6d01 6e01  R.[.\.^._.d.m.n.
+00007ac0: 7001 7101 7701 8001 8101 8301 8401 8c01  p.q.w...........
+00007ad0: 9501 9601 9901 9a01 a301 ac01 ad01 af01  ................
+00007ae0: b001 bf01 c801 c901 ca01 d401 d501 de01  ................
+00007af0: e701 ec01 ed00 0000 0000 0002 0100 0000  ................
+00007b00: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
+00007b10: 0000 0001 f600 0000 0d00 6f00 7500 7400  ..........o.u.t.
+00007b20: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00007b30: 6c00 736c 7376 7062 6c6f 6200 0002 9562  l.slsvpblob....b
+00007b40: 706c 6973 7430 30da 0102 0304 0506 0708  plist00.........
+00007b50: 090a 0b0c 0d1f 4748 4749 0c4b 5f10 1276  ......GHGI.K_..v
+00007b60: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00007b70: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00007b80: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00007b90: 6c63 756c 6174 6541 6c6c 5369 7a65 735f  lculateAllSizes_
+00007ba0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+00007bb0: 5958 7465 7874 5369 7a65 5f10 0f73 6372  YXtextSize_..scr
+00007bc0: 6f6c 6c50 6f73 6974 696f 6e58 5a73 6f72  ollPositionXZsor
+00007bd0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+00007be0: 6174 6976 6544 6174 6573 5869 636f 6e53  ativeDatesXiconS
+00007bf0: 697a 6510 0109 d90e 0f10 1112 1314 1516  ize.............
+00007c00: 1720 2529 2d32 373c 4158 636f 6d6d 656e  . %)-27<AXcommen
+00007c10: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+00007c20: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
+00007c30: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+00007c40: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00007c50: 6f6e 546e 616d 65d4 1819 1a1b 1c1d 0c1f  onTname.........
+00007c60: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
+00007c70: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
+00007c80: 1101 2c09 08d4 1819 1a1b 2122 1f1f 1008  ..,.......!"....
+00007c90: 10c8 0808 d418 191a 1b0b 261f 0c10 b508  ..........&.....
+00007ca0: 09d4 1819 1a1b 2a26 1f1f 1002 0808 d418  ......*&........
+00007cb0: 191a 1b2e 2f1f 0c10 0310 6108 09d4 1819  ..../.....a.....
+00007cc0: 1a1b 3334 0c1f 1005 1064 0908 d418 191a  ..34.....d......
+00007cd0: 1b38 390c 0c10 0410 7309 09d4 1819 1a1b  .89.....s.......
+00007ce0: 3d3e 0c1f 1006 104b 0908 d41b 191a 180c  =>.....K........
+00007cf0: 430c 4509 1101 c709 1000 0823 0000 0000  C.E........#....
+00007d00: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
+00007d10: 6d65 0923 4030 0000 0000 0000 0008 001d  me.#@0..........
+00007d20: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
+00007d30: 00ab 00b4 00b6 00b7 00ca 00d3 00e2 00ef  ................
+00007d40: 00fb 0100 0106 010b 0113 0118 0121 0127  .............!.'
+00007d50: 012d 0137 013f 0141 0144 0145 0146 014f  .-.7.?.A.D.E.F.O
+00007d60: 0151 0153 0154 0155 015e 0160 0161 0162  .Q.S.T.U.^.`.a.b
+00007d70: 016b 016d 016e 016f 0178 017a 017c 017d  .k.m.n.o.x.z.|.}
+00007d80: 017e 0187 0189 018b 018c 018d 0196 0198  .~..............
+00007d90: 019a 019b 019c 01a5 01a7 01a9 01aa 01ab  ................
+00007da0: 01b4 01b5 01b8 01b9 01bb 01bc 01c5 01ce  ................
+00007db0: 01d3 01d4 0000 0000 0000 0201 0000 0000  ................
+00007dc0: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
+00007dd0: 0000 01dd 0000 000d 006f 0075 0074 006c  .........o.u.t.l
+00007de0: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00007df0: 0073 6d6f 4444 626c 6f62 0000 0008 0bdb  .smoDDblob......
+00007e00: a04e 0b04 c541 0000 000d 006f 0075 0074  .N...A.....o.u.t
+00007e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00007e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
+00007e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
+00007e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
+00007e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
+00007e60: 0000 0002 0000 0000 000d 006f 0075 0074  ...........o.u.t
+00007e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00007e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
+00007e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+00007ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
+00007eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00007ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+00007ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00007ee0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00007ef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00007f00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00007f10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00007f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+00007f30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
+00007f40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
+00007f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+00007f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00007f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
+00007f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
+00007f90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
-00008010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-00008020: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
-00008030: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00008040: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00008050: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00008060: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00008070: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00008080: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00008090: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-000080a0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-000080b0: 0809 5f10 197b 7b32 3630 2c20 3136 327d  .._..{{260, 162}
-000080c0: 2c20 7b31 3138 302c 2035 3538 7d7d 0908  , {1180, 558}}..
-000080d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
-000080e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
-000080f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
-00008100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
-00008110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
-00008120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
-00008130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
-00008140: 6731 5363 6f6d 7000 0000 0000 05cf 0200  g1Scomp.........
-00008150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
-00008160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
-00008170: 6c6f 6200 0002 9762 706c 6973 7430 30d8  lob....bplist00.
-00008180: 0102 0304 0506 0708 090a 0b19 494a 0a4c  ............IJ.L
-00008190: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-000081a0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-000081b0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-000081c0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-000081d0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-000081e0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-000081f0: 6174 6976 6544 6174 6573 5869 636f 6e53  ativeDatesXiconS
-00008200: 697a 6510 0109 ab0c 151d 2226 2b30 353a  ize......."&+05:
-00008210: 3f44 d40d 0e0f 100a 0a13 1457 7669 7369  ?D.........Wvisi
-00008220: 626c 6559 6173 6365 6e64 696e 6755 7769  bleYascendingUwi
-00008230: 6474 685a 6964 656e 7469 6669 6572 0909  dthZidentifier..
-00008240: 1101 8f54 6e61 6d65 d416 1718 1019 1a19  ...Tname........
-00008250: 1c57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-00008260: 6173 6365 6e64 696e 6708 1023 0858 7562  ascending..#.Xub
-00008270: 6971 7569 7479 d40d 0e0f 100a 1920 2109  iquity....... !.
-00008280: 0810 b55c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00008290: d40d 0e0f 1019 1920 2508 085b 6461 7465  ....... %..[date
-000082a0: 4372 6561 7465 64d4 0d0e 0f10 0a19 292a  Created.......)*
-000082b0: 0908 1061 5473 697a 65d4 0d0e 0f10 0a0a  ...aTsize.......
-000082c0: 2e2f 0909 1073 546b 696e 64d4 0d0e 0f10  ./...sTkind.....
-000082d0: 190a 3334 0809 1064 556c 6162 656c d40d  ..34...dUlabel..
-000082e0: 0e0f 1019 0a38 3908 0910 4b57 7665 7273  .....89...KWvers
-000082f0: 696f 6ed4 0d0e 0f10 190a 3d3e 0809 1101  ion.......=>....
-00008300: 2c58 636f 6d6d 656e 7473 d40d 0e0f 1019  ,Xcomments......
-00008310: 1942 4308 0810 c85e 6461 7465 4c61 7374  .BC....^dateLast
-00008320: 4f70 656e 6564 d416 1718 1019 2019 4708  Opened...... .G.
-00008330: 0859 6461 7465 4164 6465 6408 2340 2800  .YdateAdded.#@(.
-00008340: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
-00008350: 0000 0000 0008 0019 002e 0040 0048 005c  ...........@.H.\
-00008360: 0065 0070 0083 008c 008e 008f 009b 00a4  .e.p............
-00008370: 00ac 00b6 00bc 00c7 00c8 00c9 00cc 00d1  ................
-00008380: 00da 00e2 00e8 00f2 00f3 00f5 00f6 00ff  ................
-00008390: 0108 0109 010a 010c 0119 0122 0123 0124  ...........".#.$
-000083a0: 0130 0139 013a 013b 013d 0142 014b 014c  .0.9.:.;.=.B.K.L
-000083b0: 014d 014f 0154 015d 015e 015f 0161 0167  .M.O.T.].^._.a.g
-000083c0: 0170 0171 0172 0174 017c 0185 0186 0187  .p.q.r.t.|......
-000083d0: 018a 0193 019c 019d 019e 01a0 01af 01b8  ................
-000083e0: 01b9 01ba 01c4 01c5 01ce 01d3 01d4 0000  ................
-000083f0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-00008400: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
-00008410: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
-00008420: 0076 0069 0073 0065 0064 6c73 7670 626c  .v.i.s.e.dlsvpbl
-00008430: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
-00008440: 0203 0405 0607 0809 0a0b 1d45 460a 485f  ...........EF.H_
-00008450: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00008460: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-00008470: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00008480: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00008490: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-000084a0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
-000084b0: 7469 7665 4461 7465 7358 6963 6f6e 5369  tiveDatesXiconSi
-000084c0: 7a65 1001 09d9 0c0d 0e0f 1011 1213 1415  ze..............
-000084d0: 1e23 282d 3237 3c41 5863 6f6d 6d65 6e74  .#(-27<AXcomment
-000084e0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-000084f0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-00008500: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00008510: 7369 6f6e 546e 616d 655c 6461 7465 4d6f  sionTname\dateMo
-00008520: 6469 6669 6564 d416 1718 191a 0a1c 1d55  dified.........U
-00008530: 696e 6465 7859 6173 6365 6e64 696e 6755  indexYascendingU
-00008540: 7769 6474 6857 7669 7369 626c 6510 0709  widthWvisible...
-00008550: 1101 2c08 d416 1718 191f 1d21 1d10 0808  ..,........!....
-00008560: 10c8 08d4 1617 1819 241d 261d 1002 0810  ........$.&.....
-00008570: b508 d416 1718 1929 1d2b 0a10 0308 1061  .......).+.....a
-00008580: 09d4 1617 1819 2e0a 301d 1005 0910 6408  ........0.....d.
-00008590: d416 1718 1933 0a35 0a10 0409 1073 09d4  .....3.5.....s..
-000085a0: 1617 1819 380a 3a1d 1006 0910 4b08 d416  ....8.:.....K...
-000085b0: 1718 193d 0a3f 0a10 0009 1101 8f09 d416  ...=.?..........
-000085c0: 1718 1909 1d26 0a08 0908 2340 2800 0000  .....&....#@(...
-000085d0: 0000 0054 6e61 6d65 0923 4030 0000 0000  ...Tname.#@0....
-000085e0: 0000 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-000085f0: 0070 0083 008c 008e 008f 00a2 00ab 00ba  .p..............
-00008600: 00c6 00cb 00d1 00d6 00de 00e3 00f0 00f9  ................
-00008610: 00ff 0109 010f 0117 0119 011a 011d 011e  ................
-00008620: 0127 0129 012a 012c 012d 0136 0138 0139  .'.).*.,.-.6.8.9
-00008630: 013b 013c 0145 0147 0148 014a 014b 0154  .;.<.E.G.H.J.K.T
-00008640: 0156 0157 0159 015a 0163 0165 0166 0168  .V.W.Y.Z.c.e.f.h
-00008650: 0169 0172 0174 0175 0177 0178 0181 0183  .i.r.t.u.w.x....
-00008660: 0184 0187 0188 0191 0192 0193 0194 019d  ................
-00008670: 01a2 01a3 0000 0000 0000 0201 0000 0000  ................
-00008680: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-00008690: 0000 01ac 0000 000c 0075 006e 0073 0075  .........u.n.s.u
-000086a0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-000086b0: 6d6f 4444 626c 6f62 0000 0008 0e97 7a42  moDDblob......zB
-000086c0: c500 c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-000086d0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-000086e0: 6d6f 6444 626c 6f62 0000 0008 785b 2585  modDblob....x[%.
-000086f0: fefd c441 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
-00008700: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00008710: 7068 3153 636f 6d70 0000 0000 0007 4000  ph1Scomp......@.
-00008720: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
-00008730: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
-00008740: 6c6f 6e67 0000 0001 0000 0005 0075 0074  long.........u.t
-00008750: 0069 006c 0073 6277 7370 626c 6f62 0000  .i.l.sbwspblob..
-00008760: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00008770: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00008780: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00008790: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-000087a0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-000087b0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-000087c0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-000087d0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-000087e0: 5f10 187b 7b33 3532 2c20 3234 377d 2c20  _..{{352, 247}, 
-000087f0: 7b39 3839 2c20 3433 367d 7d09 0817 2531  {989, 436}}...%1
-00008800: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
-00008810: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
-00008820: 0000 0000 0000 0000 0000 9a70 0070 0065  ...........p.p.e
-00008830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
-00008840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
-00008850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
-00008860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
-00008870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
-00008880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
-00008890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
-000088a0: 0000 00c6 6270 6c69 7374 3030 d701 0203  ....bplist00....
-000088b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-000088c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-000088d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-000088e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-000088f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00008900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00008910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00008920: 0809 5f10 157b 7b30 2c20 307d 2c20 7b31  .._..{{0, 0}, {1
-00008930: 3434 302c 2038 3737 7d7d 0908 1725 313d  440, 877}}...%1=
-00008940: 4960 6d79 7a7b 7c7d 7e96 0000 0000 0000  I`myz{|}~.......
-00008950: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00008960: 0000 0000 0000 0000 0097 0000 0002 0075  ...............u
-00008970: 0069 6473 636c 626f 6f6c 0100 0000 0200  .idsclbool......
-00008980: 7500 696c 6731 5363 6f6d 7000 0000 0000  u.ilg1Scomp.....
-00008990: 0bf8 5c00 0000 0200 7500 696c 7376 4362  ..\.....u.ilsvCb
-000089a0: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
-000089b0: 0102 0304 0506 0708 090a 0b16 4647 0a49  ............FG.I
-000089c0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-000089d0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-000089e0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-000089f0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00008a00: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00008a10: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00008a20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00008a30: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
-00008a40: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 110a  ..#(-27<A.......
-00008a50: 130a 5a69 6465 6e74 6966 6965 7259 6173  ..ZidentifierYas
-00008a60: 6365 6e64 696e 6755 7769 6474 6857 7669  cendingUwidthWvi
-00008a70: 7369 626c 6554 6e61 6d65 0911 0251 09d4  sibleTname...Q..
-00008a80: 100f 0e0d 1617 1619 0810 2308 5875 6269  ..........#.Xubi
-00008a90: 7175 6974 79d4 100e 0f0d 0a16 1d1e 0908  quity...........
-00008aa0: 10b5 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
-00008ab0: 100e 0f0d 1616 1d22 0808 5b64 6174 6543  ......."..[dateC
-00008ac0: 7265 6174 6564 d410 0e0f 0d0a 1626 2709  reated.......&'.
-00008ad0: 0810 6154 7369 7a65 d410 0e0f 0d0a 0a2b  ..aTsize.......+
-00008ae0: 2c09 0910 7354 6b69 6e64 d410 0e0f 0d16  ,...sTkind......
-00008af0: 0a30 3108 0910 6455 6c61 6265 6cd4 100e  .01...dUlabel...
-00008b00: 0f0d 160a 3536 0809 104b 5776 6572 7369  ....56...KWversi
-00008b10: 6f6e d410 0e0f 0d16 0a3a 3b08 0911 012c  on.......:;....,
-00008b20: 5863 6f6d 6d65 6e74 73d4 100e 0f0d 1616  Xcomments.......
-00008b30: 3f40 0808 10c8 5e64 6174 654c 6173 744f  ?@....^dateLastO
-00008b40: 7065 6e65 64d4 100f 0e0d 161d 1644 0808  pened........D..
-00008b50: 5964 6174 6541 6464 6564 0823 4028 0000  YdateAdded.#@(..
-00008b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
-00008b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-00008b80: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
-00008b90: 00d3 00d4 00d7 00d8 00e1 00e2 00e4 00e5  ................
-00008ba0: 00ee 00f7 00f8 00f9 00fb 0108 0111 0112  ................
-00008bb0: 0113 011f 0128 0129 012a 012c 0131 013a  .....(.).*.,.1.:
-00008bc0: 013b 013c 013e 0143 014c 014d 014e 0150  .;.<.>.C.L.M.N.P
-00008bd0: 0156 015f 0160 0161 0163 016b 0174 0175  .V._.`.a.c.k.t.u
-00008be0: 0176 0179 0182 018b 018c 018d 018f 019e  .v.y............
-00008bf0: 01a7 01a8 01a9 01b3 01b4 01bd 01c2 01c3  ................
-00008c00: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-00008c10: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-00008c20: 0000 0002 0075 0069 6c73 7670 626c 6f62  .....u.ilsvpblob
-00008c30: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
-00008c40: 0405 0607 0809 0a0b 1d46 470a 2458 6963  .........FG.$Xic
-00008c50: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00008c60: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00008c70: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00008c80: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00008c90: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-00008ca0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-00008cb0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00008cc0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
-00008cd0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
-00008ce0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
-00008cf0: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
-00008d00: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00008d10: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00008d20: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
-00008d30: 1a0a 1c1d 5569 6e64 6578 5961 7363 656e  ....UindexYascen
-00008d40: 6469 6e67 5577 6964 7468 5776 6973 6962  dingUwidthWvisib
-00008d50: 6c65 1007 0911 012c 08d4 1617 1819 1f1d  le.....,........
-00008d60: 211d 1008 0810 c808 d416 1718 1924 1d26  !............$.&
-00008d70: 0a10 0108 10b5 09d4 1617 1819 291d 261d  ............).&.
-00008d80: 1002 0808 d416 1718 192d 1d2f 0a10 0308  .........-./....
-00008d90: 1061 09d4 1617 1819 320a 341d 1005 0910  .a......2.4.....
-00008da0: 6408 d416 1718 1937 0a39 0a10 0409 1073  d......7.9.....s
-00008db0: 09d4 1617 1819 3c0a 3e1d 1006 0910 4b08  ......<.>.....K.
-00008dc0: d419 1718 160a 0a43 4409 0911 0251 1000  .......CD....Q..
-00008dd0: 0823 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
-00008de0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00008df0: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
-00008e00: 00da 00df 00e5 00ea 00f2 00f7 0100 0106  ................
-00008e10: 0110 0116 011e 0120 0121 0124 0125 012e  ....... .!.$.%..
-00008e20: 0130 0131 0133 0134 013d 013f 0140 0142  .0.1.3.4.=.?.@.B
-00008e30: 0143 014c 014e 014f 0150 0159 015b 015c  .C.L.N.O.P.Y.[.\
-00008e40: 015e 015f 0168 016a 016b 016d 016e 0177  .^._.h.j.k.m.n.w
-00008e50: 0179 017a 017c 017d 0186 0188 0189 018b  .y.z.|.}........
-00008e60: 018c 0195 0196 0197 019a 019c 019d 01a6  ................
-00008e70: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
-00008e80: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00008e90: 01ac 0000 0002 0075 0069 6d6f 4444 626c  .......u.imoDDbl
-00008ea0: 6f62 0000 0008 6da9 747c 5e01 c541 0000  ob....m.t|^..A..
-00008eb0: 0002 0075 0069 6d6f 6444 626c 6f62 0000  ...u.imodDblob..
-00008ec0: 0008 6da9 747c 5e01 c541 0000 0002 0075  ..m.t|^..A.....u
-00008ed0: 0069 7068 3153 636f 6d70 0000 0000 000f  .iph1Scomp......
-00008ee0: 1000 bc01 bd01 c601 cf01 d400 0000 0000  ................
-00008ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00008f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
-00008f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
-00008f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
-00008f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
-00008f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
-00008f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
-00008f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00008f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
-00008f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
-00008f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00008fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00008fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
-00008fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00008fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00008fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
+00008010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
+00008020: 6c73 7670 626c 6f62 0000 0295 6270 6c69  lsvpblob....bpli
+00008030: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00008040: 0c0d 1f47 4847 490c 4b5f 1012 7669 6577  ...GHGI.K_..view
+00008050: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00008060: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00008070: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00008080: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00008090: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+000080a0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+000080b0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+000080c0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000080d0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000080e0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
+000080f0: 292d 3237 3c41 5863 6f6d 6d65 6e74 735e  )-27<AXcomments^
+00008100: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
+00008110: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
+00008120: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
+00008130: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
+00008140: 6e61 6d65 d418 191a 1b1c 1d0c 1f55 696e  name.........Uin
+00008150: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
+00008160: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
+00008170: 0908 d418 191a 1b21 221f 1f10 0810 c808  .......!".......
+00008180: 08d4 1819 1a1b 0b26 1f0c 10b5 0809 d418  .......&........
+00008190: 191a 1b2a 261f 1f10 0208 08d4 1819 1a1b  ...*&...........
+000081a0: 2e2f 1f0c 1003 1061 0809 d418 191a 1b33  ./.....a.......3
+000081b0: 340c 1f10 0510 6409 08d4 1819 1a1b 3839  4.....d.......89
+000081c0: 0c0c 1004 1073 0909 d418 191a 1b3d 3e0c  .....s.......=>.
+000081d0: 1f10 0610 4b09 08d4 1819 1a1b 4243 0c0c  ....K.......BC..
+000081e0: 1000 1101 c709 0908 2300 0000 0000 0000  ........#.......
+000081f0: 0023 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
+00008200: 2340 3000 0000 0000 0000 0800 1d00 3200  #@0...........2.
+00008210: 4400 4c00 6000 7200 7b00 8d00 9800 ab00  D.L.`.r.{.......
+00008220: b400 b600 b700 ca00 d300 e200 ef00 fb01  ................
+00008230: 0001 0601 0b01 1301 1801 2101 2701 2d01  ..........!.'.-.
+00008240: 3701 3f01 4101 4401 4501 4601 4f01 5101  7.?.A.D.E.F.O.Q.
+00008250: 5301 5401 5501 5e01 6001 6101 6201 6b01  S.T.U.^.`.a.b.k.
+00008260: 6d01 6e01 6f01 7801 7a01 7c01 7d01 7e01  m.n.o.x.z.|.}.~.
+00008270: 8701 8901 8b01 8c01 8d01 9601 9801 9a01  ................
+00008280: 9b01 9c01 a501 a701 a901 aa01 ab01 b401  ................
+00008290: b601 b901 ba01 bb01 bc01 c501 ce01 d301  ................
+000082a0: d400 0000 0000 0002 0100 0000 0000 0000  ................
+000082b0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
+000082c0: dd00 0000 0800 7000 6c00 6f00 7400 7400  ......p.l.o.t.t.
+000082d0: 6900 6e00 676d 6f44 4462 6c6f 6200 0000  i.n.gmoDDblob...
+000082e0: 089a d621 3946 05c5 4100 0000 0800 7000  ...!9F..A.....p.
+000082f0: 6c00 6f00 7400 7400 6900 6e00 676d 6f64  l.o.t.t.i.n.gmod
+00008300: 4462 6c6f 6200 0000 089a d621 3946 05c5  Dblob......!9F..
+00008310: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
+00008320: 6900 6e00 6770 6831 5363 6f6d 7000 0000  i.n.gph1Scomp...
+00008330: 0000 0b30 0000 0000 0800 7000 6c00 6f00  ...0......p.l.o.
+00008340: 7400 7400 6900 6e00 6776 5372 6e6c 6f6e  t.t.i.n.gvSrnlon
+00008350: 6700 0000 0100 0000 1300 7000 6f00 7300  g.........p.o.s.
+00008360: 6500 5f00 6300 6f00 6e00 6600 6900 6700  e._.c.o.n.f.i.g.
+00008370: 7500 7200 6100 7400 6900 6f00 6e00 7362  u.r.a.t.i.o.n.sb
+00008380: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
+00008390: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+000083a0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+000083b0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+000083c0: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+000083d0: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+000083e0: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+000083f0: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00008400: 6562 6172 0808 0908 095f 1019 7b7b 3135  ebar....._..{{15
+00008410: 392c 2031 3233 7d2c 207b 3130 3736 2c20  9, 123}, {1076, 
+00008420: 3632 317d 7d09 0817 2531 3d49 606d 797a  621}}...%1=I`myz
+00008430: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
+00008440: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
+00008450: 0000 0000 9b00 0000 1300 7000 6f00 7300  ..........p.o.s.
+00008460: 6500 5f00 6300 6f00 6e00 6600 6900 6700  e._.c.o.n.f.i.g.
+00008470: 7500 7200 6100 7400 6900 6f00 6e00 7364  u.r.a.t.i.o.n.sd
+00008480: 7363 6c62 6f6f 6c00 0000 0013 0070 006f  sclbool......p.o
+00008490: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
+000084a0: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
+000084b0: 0073 6c67 3153 636f 6d70 0000 0000 0006  .slg1Scomp......
+000084c0: ae56 0000 0013 0070 006f 0073 0065 005f  .V.....p.o.s.e._
+000084d0: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
+000084e0: 0061 0074 0069 006f 006e 0073 6c73 7643  .a.t.i.o.n.slsvC
+000084f0: 626c 6f62 0000 02b0 6270 6c69 7374 3030  blob....bplist00
+00008500: da01 0203 0405 0607 0809 0a0b 0b0d 1a48  ...............H
+00008510: 4948 4a4b 4c5f 1010 7573 6552 656c 6174  IHJKL_..useRelat
+00008520: 6976 6544 6174 6573 5f10 0f73 686f 7749  iveDates_..showI
+00008530: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00008540: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00008550: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
+00008560: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
+00008570: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
+00008580: 6f6e 585a 736f 7274 436f 6c75 6d6e 5869  onXZsortColumnXi
+00008590: 636f 6e53 697a 655f 1012 7669 6577 4f70  conSize_..viewOp
+000085a0: 7469 6f6e 7356 6572 7369 6f6e 0909 ab0e  tionsVersion....
+000085b0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
+000085c0: 140b 0b5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
+000085d0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+000085e0: 6973 6962 6c65 546e 616d 6511 0127 0909  isibleTname..'..
+000085f0: d40f 1011 1218 191a 1a58 7562 6971 7569  .........Xubiqui
+00008600: 7479 1023 0808 d40f 1011 121d 1e1a 0b5c  ty.#...........\
+00008610: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
+00008620: d40f 1011 1222 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
+00008630: 6561 7465 6408 08d4 0f10 1112 2627 1a0b  eated.......&'..
+00008640: 5473 697a 6510 6108 09d4 0f10 1112 2b2c  Tsize.a.......+,
+00008650: 0b0b 546b 696e 6410 7309 09d4 0f10 1112  ..Tkind.s.......
+00008660: 3031 0b1a 556c 6162 656c 1064 0908 d40f  01..Ulabel.d....
+00008670: 1011 1235 360b 1a57 7665 7273 696f 6e10  ...56..Wversion.
+00008680: 4b09 08d4 0f10 1112 3a3b 0b1a 5863 6f6d  K.......:;..Xcom
+00008690: 6d65 6e74 7311 012c 0908 d40f 1011 123f  ments..,.......?
+000086a0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
+000086b0: 6564 10c8 0808 d40f 1011 1244 1e1a 1a59  ed.........D...Y
+000086c0: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
+000086d0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
+000086e0: 616d 6523 4030 0000 0000 0000 1001 0008  ame#@0..........
+000086f0: 001d 0030 0042 004a 005e 0070 0079 008b  ...0.B.J.^.p.y..
+00008700: 0096 009f 00b4 00b5 00b6 00c2 00cb 00d6  ................
+00008710: 00dc 00e6 00ee 00f3 00f6 00f7 00f8 0101  ................
+00008720: 010a 010c 010d 010e 0117 0124 0126 0127  ...........$.&.'
+00008730: 0128 0131 013d 013e 013f 0148 014d 014f  .(.1.=.>.?.H.M.O
+00008740: 0150 0151 015a 015f 0161 0162 0163 016c  .P.Q.Z._.a.b.c.l
+00008750: 0172 0174 0175 0176 017f 0187 0189 018a  .r.t.u.v........
+00008760: 018b 0194 019d 01a0 01a1 01a2 01ab 01ba  ................
+00008770: 01bc 01bd 01be 01c7 01d1 01d2 01d3 01d4  ................
+00008780: 01dd 01e6 01eb 01f4 0000 0000 0000 0201  ................
+00008790: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
+000087a0: 0000 0000 0000 01f6 0000 0013 0070 006f  .............p.o
+000087b0: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
+000087c0: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
+000087d0: 0073 6c73 7670 626c 6f62 0000 0295 6270  .slsvpblob....bp
+000087e0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
+000087f0: 0a0b 0b0d 1c48 4948 4a4b 295f 1010 7573  .....HIHJK)_..us
+00008800: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+00008810: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00008820: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00008830: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00008840: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+00008850: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+00008860: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+00008870: 6c75 6d6e 5869 636f 6e53 697a 655f 1012  lumnXiconSize_..
+00008880: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00008890: 6f6e 0909 d90e 0f10 1112 1314 1516 1720  on............. 
+000088a0: 252a 2e33 383d 4258 636f 6d6d 656e 7473  %*.38=BXcomments
+000088b0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+000088c0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+000088d0: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+000088e0: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+000088f0: 546e 616d 65d4 1819 1a1b 1c1d 0b1f 5776  Tname.........Wv
+00008900: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00008910: 656e 6469 6e67 5569 6e64 6578 0811 012c  endingUindex...,
+00008920: 0910 07d4 1819 1a1b 1c22 1c24 0810 c808  .........".$....
+00008930: 1008 d418 191a 1b0b 271c 2909 10b5 0810  ........'.).....
+00008940: 01d4 1819 1a1b 1c27 1c2d 0808 1002 d418  .......'.-......
+00008950: 191a 1b0b 301c 3209 1061 0810 03d4 1819  ....0.2..a......
+00008960: 1a1b 1c35 0b37 0810 6409 1005 d418 191a  ...5.7..d.......
+00008970: 1b0b 3a0b 3c09 1073 0910 04d4 1819 1a1b  ..:.<..s........
+00008980: 1c3f 0b41 0810 4b09 1006 d418 191a 1b0b  .?.A..K.........
+00008990: 440b 4609 1101 2709 1000 0823 0000 0000  D.F...'....#....
+000089a0: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
+000089b0: 6d65 2340 3000 0000 0000 0000 0800 1d00  me#@0...........
+000089c0: 3000 4200 4a00 5e00 7000 7900 8b00 9600  0.B.J.^.p.y.....
+000089d0: 9f00 b400 b500 b600 c900 d200 e100 ee00  ................
+000089e0: fa00 ff01 0501 0a01 1201 1701 2001 2801  ............ .(.
+000089f0: 2e01 3801 3e01 3f01 4201 4301 4501 4e01  ..8.>.?.B.C.E.N.
+00008a00: 4f01 5101 5201 5401 5d01 5e01 6001 6101  O.Q.R.T.].^.`.a.
+00008a10: 6301 6c01 6d01 6e01 7001 7901 7a01 7c01  c.l.m.n.p.y.z.|.
+00008a20: 7d01 7f01 8801 8901 8b01 8c01 8e01 9701  }...............
+00008a30: 9801 9a01 9b01 9d01 a601 a701 a901 aa01  ................
+00008a40: ac01 b501 b601 b901 ba01 bc01 bd01 c601  ................
+00008a50: cf01 d400 0000 0000 0002 0100 0000 0000  ................
+00008a60: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
+00008a70: 0001 dd00 0000 1300 7000 6f00 7300 6500  ........p.o.s.e.
+00008a80: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
+00008a90: 7200 6100 7400 6900 6f00 6e00 736d 6f44  r.a.t.i.o.n.smoD
+00008aa0: 4462 6c6f 6200 0000 08d9 7e4b 74e2 ddc4  Dblob.....~Kt...
+00008ab0: 4100 0000 1300 7000 6f00 7300 6500 5f00  A.....p.o.s.e._.
+00008ac0: 6300 6f00 6e00 6600 6900 6700 7500 7200  c.o.n.f.i.g.u.r.
+00008ad0: 6100 7400 6900 6f00 6e00 736d 6f64 4462  a.t.i.o.n.smodDb
+00008ae0: 6c6f 6200 0000 08d9 7e4b 74e2 ddc4 4100  lob.....~Kt...A.
+00008af0: 0000 1300 7000 6f00 7300 6500 5f00 6300  ....p.o.s.e._.c.
+00008b00: 6f00 6e00 6600 6900 6700 7500 7200 6100  o.n.f.i.g.u.r.a.
+00008b10: 7400 6900 6f00 6e00 7370 6831 5363 6f6d  t.i.o.n.sph1Scom
+00008b20: 7000 0000 0000 0730 0000 0000 1300 7000  p......0......p.
+00008b30: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00008b40: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00008b50: 6e00 7376 5372 6e6c 6f6e 6700 0000 0100  n.svSrnlong.....
+00008b60: 0000 1b00 7000 6f00 7300 6500 5f00 6300  ....p.o.s.e._.c.
+00008b70: 6f00 6e00 6600 6900 6700 7500 7200 6100  o.n.f.i.g.u.r.a.
+00008b80: 7400 6900 6f00 6e00 7300 5f00 6100 7200  t.i.o.n.s._.a.r.
+00008b90: 6300 6800 6900 7600 656c 6731 5363 6f6d  c.h.i.v.elg1Scom
+00008ba0: 7000 0000 0000 06fa ed00 0000 1b00 7000  p.............p.
+00008bb0: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00008bc0: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00008bd0: 6e00 7300 5f00 6100 7200 6300 6800 6900  n.s._.a.r.c.h.i.
+00008be0: 7600 656d 6f44 4462 6c6f 6200 0000 0889  v.emoDDblob.....
+00008bf0: 831e a9cb fec4 4100 0000 1b00 7000 6f00  ......A.....p.o.
+00008c00: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
+00008c10: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00008c20: 7300 5f00 6100 7200 6300 6800 6900 7600  s._.a.r.c.h.i.v.
+00008c30: 656d 6f64 4462 6c6f 6200 0000 0889 831e  emodDblob.......
+00008c40: a9cb fec4 4100 0000 1b00 7000 6f00 7300  ....A.....p.o.s.
+00008c50: 6500 5f00 6300 6f00 6e00 6600 6900 6700  e._.c.o.n.f.i.g.
+00008c60: 7500 7200 6100 7400 6900 6f00 6e00 7300  u.r.a.t.i.o.n.s.
+00008c70: 5f00 6100 7200 6300 6800 6900 7600 6570  _.a.r.c.h.i.v.ep
+00008c80: 6831 5363 6f6d 7000 0000 0000 0790 0000  h1Scomp.........
+00008c90: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
+00008ca0: 6d00 7000 6f00 7200 7400 6500 7200 7362  m.p.o.r.t.e.r.sb
+00008cb0: 7773 7062 6c6f 6200 0000 c962 706c 6973  wspblob....bplis
+00008cc0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+00008cd0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00008ce0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+00008cf0: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00008d00: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+00008d10: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+00008d20: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00008d30: 6562 6172 0808 0908 095f 1018 7b7b 3336  ebar....._..{{36
+00008d40: 2c20 3133 317d 2c20 7b31 3330 322c 2037  , 131}, {1302, 7
+00008d50: 3134 7d7d 0908 1725 313d 4960 6d79 7a7b  14}}...%1=I`myz{
+00008d60: 7c7d 7e99 0000 0000 0000 0101 0000 0000  |}~.............
+00008d70: 0000 000f 0000 0000 0000 0000 0000 0000  ................
+00008d80: 0000 009a 0000 000e 0070 006f 0073 0065  .........p.o.s.e
+00008d90: 005f 0069 006d 0070 006f 0072 0074 0065  ._.i.m.p.o.r.t.e
+00008da0: 0072 0073 6473 636c 626f 6f6c 0000 0000  .r.sdsclbool....
+00008db0: 0e00 7000 6f00 7300 6500 5f00 6900 6d00  ..p.o.s.e._.i.m.
+00008dc0: 7000 6f00 7200 7400 6500 7200 736c 6731  p.o.r.t.e.r.slg1
+00008dd0: 5363 6f6d 7000 0000 0000 0327 2674 006c  Scomp......'&t.l
+00008de0: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00008df0: 0073 6d6f 4444 626c 6f62 0000 0008 0bdb  .smoDDblob......
+00008e00: a04e 0b04 c541 0000 000d 006f 0075 0074  .N...A.....o.u.t
+00008e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00008e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
+00008e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
+00008e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
+00008e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
+00008e60: 0000 0002 0000 0000 000d 006f 0075 0074  ...........o.u.t
+00008e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00008e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
+00008e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+00008ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
+00008eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00008ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+00008ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00008ee0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00008ef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00008f00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00008f10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00008f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+00008f30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
+00008f40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
+00008f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+00008f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00008f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
+00008f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
+00008f90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00009000: 0000 0000 0000 0002 0000 0007 0000 0004  ................
-00009010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
-00009020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
-00009030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
-00009040: 0000 025d 6270 6c69 7374 3030 d801 0203  ...]bplist00....
-00009050: 0405 0607 0809 0a0b 1a46 470a 2758 6963  .........FG.'Xic
-00009060: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
+00009010: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
+00009020: 006f 0072 0074 0065 0072 0073 6c73 7670  .o.r.t.e.r.slsvp
+00009030: 626c 6f62 0000 0266 6270 6c69 7374 3030  blob...fbplist00
+00009040: d801 0203 0405 0607 0809 0a0b 1a45 4647  .............EFG
+00009050: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+00009060: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00009070: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00009080: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
 00009090: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-000090a0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-000090b0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-000090c0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-000090d0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
-000090e0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
-000090f0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
-00009100: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
-00009110: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00009120: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00009130: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
-00009140: 1a1b 0a1d 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
-00009150: 7468 5961 7363 656e 6469 6e67 5569 6e64  thYascendingUind
-00009160: 6578 0811 012c 0910 07d4 1617 1819 1a20  ex...,......... 
-00009170: 1a22 0810 c808 1008 d416 1718 190a 251a  ."............%.
-00009180: 2709 10b5 0810 01d4 1617 1819 1a25 1a2b  '............%.+
-00009190: 0808 1002 d416 1718 190a 2e1a 3009 1061  ............0..a
-000091a0: 0810 03d4 1617 1819 1a33 0a35 0810 6409  .........3.5..d.
-000091b0: 1005 d416 1718 190a 380a 3a09 1073 0910  ........8.:..s..
-000091c0: 04d4 1617 1819 1a3d 0a3f 0810 4b09 1006  .......=.?..K...
-000091d0: d416 1718 190a 420a 4409 10f0 0910 0008  ......B.D.......
-000091e0: 2340 2800 0000 0000 0054 6e61 6d65 0900  #@(......Tname..
-000091f0: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
-00009200: 7700 8c00 9500 9600 a900 b200 c100 ce00  w...............
-00009210: da00 df00 e500 ea00 f200 f701 0001 0801  ................
-00009220: 0e01 1801 1e01 1f01 2201 2301 2501 2e01  ........".#.%...
-00009230: 2f01 3101 3201 3401 3d01 3e01 4001 4101  /.1.2.4.=.>.@.A.
-00009240: 4301 4c01 4d01 4e01 5001 5901 5a01 5c01  C.L.M.N.P.Y.Z.\.
-00009250: 5d01 5f01 6801 6901 6b01 6c01 6e01 7701  ]._.h.i.k.l.n.w.
-00009260: 7801 7a01 7b01 7d01 8601 8701 8901 8a01  x.z.{.}.........
-00009270: 8c01 9501 9601 9801 9901 9b01 9c01 a501  ................
-00009280: aa00 0000 0000 0002 0100 0000 0000 0000  ................
-00009290: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-000092a0: ab00 0000 0500 0000 0900 6c00 6100 6200  ..........l.a.b.
-000092b0: 6500 6c00 6c00 6900 6e00 676c 7376 4362  e.l.l.i.n.glsvCb
-000092c0: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
-000092d0: 0102 0304 0506 0708 090a 0b18 4647 0a49  ............FG.I
-000092e0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-000092f0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00009300: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00009310: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00009320: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00009330: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00009340: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00009350: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
-00009360: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 110a  ..#(-27<A.......
-00009370: 130a 5a69 6465 6e74 6966 6965 7259 6173  ..ZidentifierYas
-00009380: 6365 6e64 696e 6755 7769 6474 6857 7669  cendingUwidthWvi
-00009390: 7369 626c 6554 6e61 6d65 0911 0251 09d4  sibleTname...Q..
-000093a0: 0d0f 0e10 1617 1818 5875 6269 7175 6974  ........Xubiquit
-000093b0: 7910 2308 08d4 0d0e 0f10 1b18 1d0a 5c64  y.#...........\d
-000093c0: 6174 654d 6f64 6966 6965 6408 10b5 09d4  ateModified.....
-000093d0: 0d0e 0f10 2018 1d18 5b64 6174 6543 7265  .... ...[dateCre
-000093e0: 6174 6564 0808 d40d 0e0f 1024 1826 0a54  ated.......$.&.T
-000093f0: 7369 7a65 0810 6109 d40d 0e0f 1029 0a2b  size..a......).+
-00009400: 0a54 6b69 6e64 0910 7309 d40d 0e0f 102e  .Tkind..s.......
-00009410: 0a30 1855 6c61 6265 6c09 1064 08d4 0d0e  .0.Ulabel..d....
-00009420: 0f10 330a 3518 5776 6572 7369 6f6e 0910  ..3.5.Wversion..
-00009430: 4b08 d40d 0e0f 1038 0a3a 1858 636f 6d6d  K......8.:.Xcomm
-00009440: 656e 7473 0911 012c 08d4 0d0e 0f10 3d18  ents...,......=.
-00009450: 3f18 5e64 6174 654c 6173 744f 7065 6e65  ?.^dateLastOpene
-00009460: 6408 10c8 08d4 0d0f 0e10 421d 1818 5964  d.........B...Yd
-00009470: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
-00009480: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
-00009490: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-000094a0: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
-000094b0: 00d3 00d4 00d7 00d8 00e1 00ea 00ec 00ed  ................
-000094c0: 00ee 00f7 0104 0105 0107 0108 0111 011d  ................
-000094d0: 011e 011f 0128 012d 012e 0130 0131 013a  .....(.-...0.1.:
-000094e0: 013f 0140 0142 0143 014c 0152 0153 0155  .?.@.B.C.L.R.S.U
-000094f0: 0156 015f 0167 0168 016a 016b 0174 017d  .V._.g.h.j.k.t.}
-00009500: 017e 0181 0182 018b 019a 019b 019d 019e  .~..............
-00009510: 01a7 01b1 01b2 01b3 01b4 01bd 01c2 01c3  ................
-00009520: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-00009530: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-00009540: 0000 0006 0000 000d 006f 0075 0074 006c  .........o.u.t.l
-00009550: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00009560: 0073 6c73 7670 626c 6f62 0000 0294 6270  .slsvpblob....bp
-00009570: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-00009580: 0a0b 0c0d 1c48 4948 4a0c 2958 6963 6f6e  .....HIHJ.)Xicon
-00009590: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-000095a0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-000095b0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-000095c0: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
-000095d0: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
-000095e0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
-000095f0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-00009600: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
-00009610: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00009620: 6f6e 2340 3000 0000 0000 0009 d90e 0f10  on#@0...........
-00009630: 1112 1314 1516 1720 252a 2e33 383d 4258  ....... %*.38=BX
-00009640: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
-00009650: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
-00009660: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
-00009670: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-00009680: 5776 6572 7369 6f6e 546e 616d 65d4 1819  WversionTname...
-00009690: 1a1b 1c1d 0c1f 5776 6973 6962 6c65 5577  ......WvisibleUw
-000096a0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
-000096b0: 6e64 6578 0811 012c 0910 07d4 1819 1a1b  ndex...,........
-000096c0: 1c22 1c24 0810 c808 1008 d418 191a 1b0c  .".$............
-000096d0: 271c 2909 10b5 0810 01d4 1819 1a1b 1c27  '.)............'
-000096e0: 1c2d 0808 1002 d418 191a 1b0c 301c 3209  .-..........0.2.
-000096f0: 1061 0810 03d4 1819 1a1b 1c35 0c37 0810  .a.........5.7..
-00009700: 6409 1005 d418 191a 1b0c 3a0c 3c09 1073  d.........:.<..s
-00009710: 0910 04d4 1819 1a1b 1c3f 0c41 0810 4b09  .........?.A..K.
-00009720: 1006 d41b 191a 1843 440c 0c10 0010 f009  .......CD.......
-00009730: 0908 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
-00009740: 0000 0000 546e 616d 6509 0008 001d 0026  ....Tname......&
-00009750: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
-00009760: 00b4 00bd 00be 00d1 00da 00e9 00f6 0102  ................
-00009770: 0107 010d 0112 011a 011f 0128 0130 0136  ...........(.0.6
-00009780: 0140 0146 0147 014a 014b 014d 0156 0157  .@.F.G.J.K.M.V.W
-00009790: 0159 015a 015c 0165 0166 0168 0169 016b  .Y.Z.\.e.f.h.i.k
-000097a0: 0174 0175 0176 0178 0181 0182 0184 0185  .t.u.v.x........
-000097b0: 0187 0190 0191 0193 0194 0196 019f 01a0  ................
-000097c0: 01a2 01a3 01a5 01ae 01af 01b1 01b2 01b4  ................
-000097d0: 01bd 01bf 01c1 01c2 01c3 01c4 01cd 01d6  ................
-000097e0: 01db 0000 0000 0000 0201 0000 0000 0000  ................
-000097f0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
-00009800: 01dc 0000 0007 0000 0013 0070 006f 0073  ...........p.o.s
-00009810: 0065 005f 0063 006f 006e 0066 0069 0067  .e._.c.o.n.f.i.g
-00009820: 0075 0072 0061 0074 0069 006f 006e 0073  .u.r.a.t.i.o.n.s
-00009830: 7653 726e 6c6f 6e67 0000 0001 0000 0008  vSrnlong........
-00009840: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
-00009850: 006f 006c 0073 6c73 7670 626c 6f62 0000  .o.l.slsvpblob..
-00009860: 025d 6270 6c69 7374 3030 d801 0203 0405  .]bplist00......
-00009870: 0607 0809 0a0b 1a46 470a 2758 6963 6f6e  .......FG.'Xicon
-00009880: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-00009890: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-000098a0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-000098b0: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-000098c0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
-000098d0: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
-000098e0: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
-000098f0: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
-00009900: 1314 151e 2328 2c31 363b 4058 636f 6d6d  ....#(,16;@Xcomm
-00009910: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-00009920: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-00009930: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-00009940: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00009950: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
-00009960: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00009970: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
-00009980: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
-00009990: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
-000099a0: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
-000099b0: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
-000099c0: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
-000099d0: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
-000099e0: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
-000099f0: 1718 190a 420a 4409 10d0 0910 0008 2340  ....B.D.......#@
-00009a00: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
-00009a10: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00009a20: 8c00 9500 9600 a900 b200 c100 ce00 da00  ................
-00009a30: df00 e500 ea00 f200 f701 0001 0801 0e01  ................
-00009a40: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
-00009a50: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
-00009a60: 4c01 4d01 4e01 5001 5901 5a01 5c01 5d01  L.M.N.P.Y.Z.\.].
-00009a70: 5f01 6801 6901 6b01 6c01 6e01 7701 7801  _.h.i.k.l.n.w.x.
-00009a80: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
-00009a90: 9501 9601 9801 9901 9b01 9c01 a501 aa00  ................
-00009aa0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00009ab0: 0000 0000 0000 0000 0000 0000 0001 ab00  ................
-00009ac0: 0000 0900 0000 0200 7500 6976 5372 6e6c  ........u.ivSrnl
-00009ad0: 6f6e 6700 0000 0100 0000 0a00 0000 0500  ong.............
-00009ae0: 7500 7400 6900 6c00 7364 7363 6c62 6f6f  u.t.i.l.sdsclboo
-00009af0: 6c00 3108 0910 6455 6c61 6265 6cd4 100e  l.1...dUlabel...
-00009b00: 0f0d 160a 3536 0809 104b 5776 6572 7369  ....56...KWversi
-00009b10: 6f6e d410 0e0f 0d16 0a3a 3b08 0911 012c  on.......:;....,
-00009b20: 5863 6f6d 6d65 6e74 73d4 100e 0f0d 1616  Xcomments.......
-00009b30: 3f40 0808 10c8 5e64 6174 654c 6173 744f  ?@....^dateLastO
-00009b40: 7065 6e65 64d4 100f 0e0d 161d 1644 0808  pened........D..
-00009b50: 5964 6174 6541 6464 6564 0823 4028 0000  YdateAdded.#@(..
-00009b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
-00009b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-00009b80: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
-00009b90: 00d3 00d4 00d7 00d8 00e1 00e2 00e4 00e5  ................
-00009ba0: 00ee 00f7 00f8 00f9 00fb 0108 0111 0112  ................
-00009bb0: 0113 011f 0128 0129 012a 012c 0131 013a  .....(.).*.,.1.:
-00009bc0: 013b 013c 013e 0143 014c 014d 014e 0150  .;.<.>.C.L.M.N.P
-00009bd0: 0156 015f 0160 0161 0163 016b 0174 0175  .V._.`.a.c.k.t.u
-00009be0: 0176 0179 0182 018b 018c 018d 018f 019e  .v.y............
-00009bf0: 01a7 01a8 01a9 01b3 01b4 01bd 01c2 01c3  ................
-00009c00: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-00009c10: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-00009c20: 0000 0002 0075 0069 6c73 7670 626c 6f62  .....u.ilsvpblob
-00009c30: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
-00009c40: 0405 0607 0809 0a0b 1d46 470a 2458 6963  .........FG.$Xic
-00009c50: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00009c60: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00009c70: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00009c80: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00009c90: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-00009ca0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-00009cb0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00009cc0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
-00009cd0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
-00009ce0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
-00009cf0: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
-00009d00: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00009d10: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00009d20: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
-00009d30: 1a0a 1c1d 5569 6e64 6578 5961 7363 656e  ....UindexYascen
-00009d40: 6469 6e67 5577 6964 7468 5776 6973 6962  dingUwidthWvisib
-00009d50: 6c65 1007 0911 012c 08d4 1617 1819 1f1d  le.....,........
-00009d60: 211d 1008 0810 c808 d416 1718 1924 1d26  !............$.&
-00009d70: 0a10 0108 10b5 09d4 1617 1819 291d 261d  ............).&.
-00009d80: 1002 0808 d416 1718 192d 1d2f 0a10 0308  .........-./....
-00009d90: 1061 09d4 1617 1819 320a 341d 1005 0910  .a......2.4.....
-00009da0: 6408 d416 1718 1937 0a39 0a10 0409 1073  d......7.9.....s
-00009db0: 09d4 1617 1819 3c0a 3e1d 1006 0910 4b08  ......<.>.....K.
-00009dc0: d419 1718 160a 0a43 4409 0911 0251 1000  .......CD....Q..
-00009dd0: 0823 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
-00009de0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00009df0: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
-00009e00: 00da 00df 00e5 00ea 00f2 00f7 0100 0106  ................
-00009e10: 0110 0116 011e 0120 0121 0124 0125 012e  ....... .!.$.%..
-00009e20: 0130 0131 0133 0134 013d 013f 0140 0142  .0.1.3.4.=.?.@.B
-00009e30: 0143 014c 014e 014f 0150 0159 015b 015c  .C.L.N.O.P.Y.[.\
-00009e40: 015e 015f 0168 016a 016b 016d 016e 0177  .^._.h.j.k.m.n.w
-00009e50: 0179 017a 017c 017d 0186 0188 0189 018b  .y.z.|.}........
-00009e60: 018c 0195 0196 0197 019a 019c 019d 01a6  ................
-00009e70: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
-00009e80: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00009e90: 01ac 0000 0002 0075 0069 6d6f 4444 626c  .......u.imoDDbl
-00009ea0: 6f62 0000 0008 6da9 747c 5e01 c541 0000  ob....m.t|^..A..
-00009eb0: 0002 0075 0069 6d6f 6444 626c 6f62 0000  ...u.imodDblob..
-00009ec0: 0008 6da9 747c 5e01 c541 0000 0002 0075  ..m.t|^..A.....u
-00009ed0: 0069 7068 3153 636f 6d70 0000 0000 000f  .iph1Scomp......
-00009ee0: 1000 bc01 bd01 c601 cf01 d400 0000 0000  ................
-00009ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00009f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
-00009f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
-00009f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
-00009f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
-00009f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
-00009f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
-00009f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
-00009f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
-00009f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
-00009f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
-00009fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
-00009fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
-00009fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
-00009fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
-00009fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+000090a0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+000090b0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+000090c0: 6174 6573 1001 09d9 0c0d 0e0f 1011 1213  ates............
+000090d0: 1415 1e23 272b 3035 3a3f 5863 6f6d 6d65  ...#'+05:?Xcomme
+000090e0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+000090f0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+00009100: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+00009110: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+00009120: 696f 6e54 6e61 6d65 d416 1718 191a 1b0a  ionTname........
+00009130: 1d57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00009140: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
+00009150: 1101 2c09 1007 d416 1718 191a 201a 2208  ..,......... .".
+00009160: 10c8 0810 08d4 1617 1819 0a25 1a09 0910  ...........%....
+00009170: b508 d416 1718 191a 251a 2a08 0810 02d4  ........%.*.....
+00009180: 1617 1819 0a2d 1a2f 0910 6108 1003 d416  .....-./..a.....
+00009190: 1718 191a 320a 3408 1064 0910 05d4 1617  ....2.4..d......
+000091a0: 1819 0a37 0a39 0910 7309 1004 d416 1718  ...7.9..s.......
+000091b0: 191a 3c0a 3e08 104b 0910 06d4 1617 1819  ..<.>..K........
+000091c0: 0a41 0a43 0911 01c7 0910 0008 2340 2800  .A.C........#@(.
+000091d0: 0000 0000 005c 6461 7465 4d6f 6469 6669  .....\dateModifi
+000091e0: 6564 2340 3000 0000 0000 0009 0008 0019  ed#@0...........
+000091f0: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
+00009200: 008e 008f 00a2 00ab 00ba 00c7 00d3 00d8  ................
+00009210: 00de 00e3 00eb 00f0 00f9 0101 0107 0111  ................
+00009220: 0117 0118 011b 011c 011e 0127 0128 012a  ...........'.(.*
+00009230: 012b 012d 0136 0137 0139 013a 0143 0144  .+.-.6.7.9.:.C.D
+00009240: 0145 0147 0150 0151 0153 0154 0156 015f  .E.G.P.Q.S.T.V._
+00009250: 0160 0162 0163 0165 016e 016f 0171 0172  .`.b.c.e.n.o.q.r
+00009260: 0174 017d 017e 0180 0181 0183 018c 018d  .t.}.~..........
+00009270: 0190 0191 0193 0194 019d 01aa 01b3 0000  ................
+00009280: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
+00009290: 0000 0000 0000 0000 0000 0000 01b4 0000  ................
+000092a0: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
+000092b0: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
+000092c0: 4444 626c 6f62 0000 0008 fa4c 7240 5f05  DDblob.....Lr@_.
+000092d0: c541 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
+000092e0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
+000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 fa4c  .smodDblob.....L
+00009300: 7240 5f05 c541 0000 000e 0070 006f 0073  r@_..A.....p.o.s
+00009310: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
+00009320: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
+00009330: 0000 0003 e000 0000 000e 0070 006f 0073  ...........p.o.s
+00009340: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
+00009350: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
+00009360: 0001 0000 000f 0070 006f 0073 0065 005f  .......p.o.s.e._
+00009370: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
+00009380: 0072 0073 6277 7370 626c 6f62 0000 00ca  .r.sbwspblob....
+00009390: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+000093a0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+000093b0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+000093c0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+000093d0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+000093e0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+000093f0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00009400: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+00009410: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
+00009420: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
+00009430: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+00009440: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00009450: 0000 0000 0000 0000 009b 0000 000f 0070  ...............p
+00009460: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
+00009470: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
+00009480: 636f 6d70 0000 0000 0000 9838 0000 000f  comp.......8....
+00009490: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
+000094a0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
+000094b0: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
+000094c0: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
+000094d0: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
+000094e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+000094f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00009500: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+00009510: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
+00009520: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00009530: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
+00009540: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
+00009550: ab0c 151d 2226 2b30 353a 3f44 d40d 0e0f  ...."&+05:?D....
+00009560: 1011 120a 0a5a 6964 656e 7469 6669 6572  .....Zidentifier
+00009570: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00009580: 5776 6973 6962 6c65 546e 616d 6511 01c7  WvisibleTname...
+00009590: 0909 d416 1718 0d19 1a19 1c57 7669 7369  ...........Wvisi
+000095a0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+000095b0: 696e 6708 1023 0858 7562 6971 7569 7479  ing..#.Xubiquity
+000095c0: d40d 0e0f 101e 1f19 0a5c 6461 7465 4d6f  .........\dateMo
+000095d0: 6469 6669 6564 10b5 0809 d40d 0e0f 1023  dified.........#
+000095e0: 1f19 195b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
+000095f0: 08d4 0d0e 0f10 2728 190a 5473 697a 6510  ......'(..Tsize.
+00009600: 6108 09d4 0d0e 0f10 2c2d 0a0a 546b 696e  a.......,-..Tkin
+00009610: 6410 7309 09d4 0d0e 0f10 3132 0a19 556c  d.s.......12..Ul
+00009620: 6162 656c 1064 0908 d40d 0e0f 1036 370a  abel.d.......67.
+00009630: 1957 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
+00009640: 0f10 3b3c 0a19 5863 6f6d 6d65 6e74 7311  ..;<..Xcomments.
+00009650: 012c 0908 d40d 0e0f 1040 4119 195e 6461  .,.......@A..^da
+00009660: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
+00009670: d416 1718 0d19 1f19 4708 0859 6461 7465  ........G..Ydate
+00009680: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
+00009690: 6e61 6d65 0910 0100 0800 1900 2200 3400  name........".4.
+000096a0: 3c00 5000 5900 6400 7700 8c00 9500 9600  <.P.Y.d.w.......
+000096b0: a200 ab00 b600 bc00 c600 ce00 d300 d600  ................
+000096c0: d700 d800 e100 e900 ef00 f900 fa00 fc00  ................
+000096d0: fd01 0601 0f01 1c01 1e01 1f01 2001 2901  ............ .).
+000096e0: 3501 3601 3701 4001 4501 4701 4801 4901  5.6.7.@.E.G.H.I.
+000096f0: 5201 5701 5901 5a01 5b01 6401 6a01 6c01  R.W.Y.Z.[.d.j.l.
+00009700: 6d01 6e01 7701 7f01 8101 8201 8301 8c01  m.n.w...........
+00009710: 9501 9801 9901 9a01 a301 b201 b401 b501  ................
+00009720: b601 bf01 c001 c101 cb01 cc01 d501 da01  ................
+00009730: db00 0000 0000 0002 0100 0000 0000 0000  ................
+00009740: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
+00009750: dd00 0000 0f00 7000 6f00 7300 6500 5f00  ......p.o.s.e._.
+00009760: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+00009770: 7200 736c 7376 7062 6c6f 6200 0002 5e62  r.slsvpblob...^b
+00009780: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+00009790: 090a 0b1a 4647 0a44 5869 636f 6e53 697a  ....FG.DXiconSiz
+000097a0: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
+000097b0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+000097c0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+000097d0: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+000097e0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+000097f0: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
+00009800: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
+00009810: 0000 0000 09d9 0c0d 0e0f 1011 1213 1415  ................
+00009820: 1e23 282d 3237 3c41 5863 6f6d 6d65 6e74  .#(-27<AXcomment
+00009830: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+00009840: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+00009850: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+00009860: 7369 6f6e 546e 616d 655c 6461 7465 4d6f  sionTname\dateMo
+00009870: 6469 6669 6564 d416 1718 191a 1b0a 1d57  dified.........W
+00009880: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+00009890: 6365 6e64 696e 6755 696e 6465 7808 1101  cendingUindex...
+000098a0: 2c09 1007 d416 1718 191a 201a 2208 10c8  ,......... ."...
+000098b0: 0810 08d4 1617 1819 1a25 1a27 0810 b508  .........%.'....
+000098c0: 1002 d416 1718 190a 2a1a 2c09 1061 0810  ........*.,..a..
+000098d0: 03d4 1617 1819 1a2f 0a31 0810 6409 1005  ......./.1..d...
+000098e0: d416 1718 190a 340a 3609 1073 0910 04d4  ......4.6..s....
+000098f0: 1617 1819 1a39 0a3b 0810 4b09 1006 d416  .....9.;..K.....
+00009900: 1718 190a 3e0a 4009 1101 c709 1000 d416  ....>.@.........
+00009910: 1718 190a 251a 4409 0810 0108 2340 2800  ....%.D.....#@(.
+00009920: 0000 0000 0054 6e61 6d65 0900 0800 1900  .....Tname......
+00009930: 2200 3400 3c00 5000 5900 6400 7700 8c00  ".4.<.P.Y.d.w...
+00009940: 9500 9600 a900 b200 c100 cd00 d200 d800  ................
+00009950: dd00 e500 ea00 f701 0001 0801 0e01 1801  ................
+00009960: 1e01 1f01 2201 2301 2501 2e01 2f01 3101  ....".#.%.../.1.
+00009970: 3201 3401 3d01 3e01 4001 4101 4301 4c01  2.4.=.>.@.A.C.L.
+00009980: 4d01 4f01 5001 5201 5b01 5c01 5e01 5f01  M.O.P.R.[.\.^._.
+00009990: 6101 6a01 6b01 6d01 6e01 7001 7901 7a01  a.j.k.m.n.p.y.z.
+000099a0: 7c01 7d01 7f01 8801 8901 8c01 8d01 8f01  |.}.............
+000099b0: 9801 9901 9a01 9c01 9d01 a601 ab00 0000  ................
+000099c0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+000099d0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+000099e0: 0f00 7000 6f00 7300 6500 5f00 7000 7200  ..p.o.s.e._.p.r.
+000099f0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
+00009a00: 6f44 4462 6c6f 6200 0000 0892 deca 6739  oDDblob.......g9
+00009a10: 05c5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
+00009a20: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00009a30: 6f00 7200 736d 6f64 4462 6c6f 6200 0000  o.r.smodDblob...
+00009a40: 0892 deca 6739 05c5 4100 0000 0f00 7000  ....g9..A.....p.
+00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
+00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
+00009a70: 6f6d 7000 0000 0000 0100 0000 0000 0f00  omp.............
+00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
+00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
+00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
+00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
+00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
+00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00009af0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+00009b00: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00009b10: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+00009b20: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+00009b30: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
+00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
+00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
+00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
+00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
+00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
+00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
+00009bb0: 6f6d 7000 0000 0000 042b 6f00 0000 0900  omp......+o.....
+00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
+00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
+00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
+00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
+00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
+00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00009c30: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00009c40: 7a65 5a73 6f72 7443 6f6c 756d 6e58 6963  zeZsortColumnXic
+00009c50: 6f6e 5369 7a65 5f10 1075 7365 5265 6c61  onSize_..useRela
+00009c60: 7469 7665 4461 7465 7310 0109 ab0c 151a  tiveDates.......
+00009c70: 1f23 282d 3237 3c41 d40d 0e0f 100a 120a  .#(-27<A........
+00009c80: 1457 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00009c90: 6173 6365 6e64 696e 675a 6964 656e 7469  ascendingZidenti
+00009ca0: 6669 6572 0911 01c7 0954 6e61 6d65 d40d  fier.....Tname..
+00009cb0: 0e0f 1016 1716 1908 1023 0858 7562 6971  .........#.Xubiq
+00009cc0: 7569 7479 d40d 0e0f 100a 1c16 1e09 10b5  uity............
+00009cd0: 085c 6461 7465 4d6f 6469 6669 6564 d40d  .\dateModified..
+00009ce0: 0e0f 1016 1c16 2208 085b 6461 7465 4372  ......"..[dateCr
+00009cf0: 6561 7465 64d4 0d0e 0f10 0a25 1627 0910  eated......%.'..
+00009d00: 6108 5473 697a 65d4 0d0e 0f10 0a2a 0a2c  a.Tsize......*.,
+00009d10: 0910 7309 546b 696e 64d4 0d0e 0f10 162f  ..s.Tkind....../
+00009d20: 0a31 0810 6409 556c 6162 656c d40d 0e0f  .1..d.Ulabel....
+00009d30: 1016 340a 3608 104b 0957 7665 7273 696f  ..4.6..K.Wversio
+00009d40: 6ed4 0d0e 0f10 1639 0a3b 0811 012c 0958  n......9.;...,.X
+00009d50: 636f 6d6d 656e 7473 d40d 0e0f 1016 3e16  comments......>.
+00009d60: 4008 10c8 085e 6461 7465 4c61 7374 4f70  @....^dateLastOp
+00009d70: 656e 6564 d40d 0e0f 1016 1c16 4408 0859  ened........D..Y
+00009d80: 6461 7465 4164 6465 6408 2340 2800 0000  dateAdded.#@(...
+00009d90: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
+00009da0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+00009db0: 0070 0079 008c 008e 008f 009b 00a4 00ac  .p.y............
+00009dc0: 00b2 00bc 00c7 00c8 00cb 00cc 00d1 00da  ................
+00009dd0: 00db 00dd 00de 00e7 00f0 00f1 00f3 00f4  ................
+00009de0: 0101 010a 010b 010c 0118 0121 0122 0124  ...........!.".$
+00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
+00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
+00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
+00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
+00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
+00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
+00009e50: 0000 0000 01c5 7068 3153 636f 6d70 0000  ......ph1Scomp..
+00009e60: 0000 0002 0000 0000 000d 006f 0075 0074  ...........o.u.t
+00009e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00009e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
+00009e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+00009ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
+00009eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00009ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+00009ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00009ee0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00009ef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00009f00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00009f10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00009f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+00009f30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
+00009f40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
+00009f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+00009f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00009f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
+00009f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
+00009f90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a000: 0000 0000 0000 000b 0000 0000 0000 a00b  ................
-0000a010: 0000 0045 0000 100c 0000 900c 0000 200c  ...E.......... .
-0000a020: 0000 300c 0000 400c 0000 500c 0000 600c  ..0...@...P...`.
-0000a030: 0000 700c 0000 800c 0000 0000 0000 0000  ..p.............
-0000a040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a0a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a0b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a0c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a0d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a0e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a0f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a1a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a1b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a1c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a1d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a1e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a1f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a2a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a2b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a2c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a2d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a2e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a2f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a3a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a3b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a3c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a3d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a3e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a3f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-0000a410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
-0000a420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-0000a440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-0000a450: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-0000a460: 0200 0008 0000 00a8 0000 0000 0100 00b0  ................
-0000a470: 0000 0000 0000 0000 0100 00c0 0000 0000  ................
-0000a480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
-0000a490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
-0000a4a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
-0000a4b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
-0000a4c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
-0000a4d0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
-0000a4e0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-0000a4f0: 0000 0000 0140 0000 0000 0000 0074 017d  .....@.......t.}
-0000a500: 017e 0181 0182 018b 019a 019b 019d 019e  .~..............
-0000a510: 01a7 01b1 01b2 01b3 01b4 01bd 01c2 01c3  ................
-0000a520: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-0000a530: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
-0000a540: 0000 0006 0000 000d 006f 0075 0074 006c  .........o.u.t.l
-0000a550: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-0000a560: 0073 6c73 7670 626c 6f62 0000 0294 6270  .slsvpblob....bp
-0000a570: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-0000a580: 0a0b 0c0d 1c48 4948 4a0c 2958 6963 6f6e  .....HIHJ.)Xicon
-0000a590: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-0000a5a0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-0000a5b0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-0000a5c0: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
-0000a5d0: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
-0000a5e0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
-0000a5f0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-0000a600: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
-0000a610: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-0000a620: 6f6e 2340 3000 0000 0000 0009 d90e 0f10  on#@0...........
-0000a630: 1112 1314 1516 1720 252a 2e33 383d 4258  ....... %*.38=BX
-0000a640: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
-0000a650: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
-0000a660: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
-0000a670: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-0000a680: 5776 6572 7369 6f6e 546e 616d 65d4 1819  WversionTname...
-0000a690: 1a1b 1c1d 0c1f 5776 6973 6962 6c65 5577  ......WvisibleUw
-0000a6a0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
-0000a6b0: 6e64 6578 0811 012c 0910 07d4 1819 1a1b  ndex...,........
-0000a6c0: 1c22 1c24 0810 c808 1008 d418 191a 1b0c  .".$............
-0000a6d0: 271c 2909 10b5 0810 01d4 1819 1a1b 1c27  '.)............'
-0000a6e0: 1c2d 0808 1002 d418 191a 1b0c 301c 3209  .-..........0.2.
-0000a6f0: 1061 0810 03d4 1819 1a1b 1c35 0c37 0810  .a.........5.7..
-0000a700: 6409 1005 d418 191a 1b0c 3a0c 3c09 1073  d.........:.<..s
-0000a710: 0910 04d4 1819 1a1b 1c3f 0c41 0810 4b09  .........?.A..K.
-0000a720: 1006 d41b 191a 1843 440c 0c10 0010 f009  .......CD.......
-0000a730: 0908 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
-0000a740: 0000 0000 546e 616d 6509 0008 001d 0026  ....Tname......&
-0000a750: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
-0000a760: 00b4 00bd 00be 00d1 00da 00e9 00f6 0102  ................
-0000a770: 0107 010d 0112 011a 011f 0128 0130 0136  ...........(.0.6
-0000a780: 0140 0146 0147 014a 014b 014d 0156 0157  .@.F.G.J.K.M.V.W
-0000a790: 0159 015a 015c 0165 0166 0168 0169 016b  .Y.Z.\.e.f.h.i.k
-0000a7a0: 0174 0175 0176 0178 0181 0182 0184 0185  .t.u.v.x........
-0000a7b0: 0187 0190 0191 0193 0194 0196 019f 01a0  ................
-0000a7c0: 01a2 01a3 01a5 01ae 01af 01b1 01b2 01b4  ................
-0000a7d0: 01bd 01bf 01c1 01c2 01c3 01c4 01cd 01d6  ................
-0000a7e0: 01db 0000 0000 0000 0201 0000 0000 0000  ................
-0000a7f0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
-0000a800: 01dc 0000                                ....
+0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
+0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
+0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 6cfb  .smoDDblob....l.
+0000a030: e0c5 4905 c541 0000 0009 0072 006f 0069  ..I..A.....r.o.i
+0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
+0000a050: 626c 6f62 0000 0008 6cfb e0c5 4905 c541  blob....l...I..A
+0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
+0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
+0000a080: 0000 0005 2000 0000 0009 0072 006f 0069  .... ......r.o.i
+0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
+0000a0a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
+0000a0b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
+0000a0c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
+0000a0d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
+0000a0e0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+0000a0f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+0000a100: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+0000a110: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+0000a120: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+0000a130: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+0000a140: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+0000a150: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+0000a160: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+0000a170: 7b33 322c 2031 3233 7d2c 207b 3132 3033  {32, 123}, {1203
+0000a180: 2c20 3735 347d 7d09 0817 2531 3d49 606d  , 754}}...%1=I`m
+0000a190: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+0000a1a0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+0000a1b0: 0000 0000 0000 9a00 0000 1b00 7400 6800  ............t.h.
+0000a1c0: 6900 7200 6400 5f00 7000 6100 7200 7400  i.r.d._.p.a.r.t.
+0000a1d0: 7900 5f00 6c00 6100 6200 6500 6c00 5f00  y._.l.a.b.e.l._.
+0000a1e0: 6100 7000 7000 6500 6e00 6400 6500 7200  a.p.p.e.n.d.e.r.
+0000a1f0: 736c 6731 5363 6f6d 7000 0000 0000 021c  slg1Scomp.......
+0000a200: 9000 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
+0000a210: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
+0000a220: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
+0000a230: 6500 6e00 6400 6500 7200 736c 7376 4362  e.n.d.e.r.slsvCb
+0000a240: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
+0000a250: 0102 0304 0506 0708 090a 0b16 4647 480a  ............FGH.
+0000a260: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+0000a270: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+0000a280: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+0000a290: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+0000a2a0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+0000a2b0: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+0000a2c0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+0000a2d0: 7465 7310 0109 ab0c 151a 1f23 282d 3237  tes........#(-27
+0000a2e0: 3c41 d40d 0e0f 100a 120a 1457 7669 7369  <A.........Wvisi
+0000a2f0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+0000a300: 696e 675a 6964 656e 7469 6669 6572 0911  ingZidentifier..
+0000a310: 01a6 0954 6e61 6d65 d40d 0e0f 1016 1716  ...Tname........
+0000a320: 1908 1023 0858 7562 6971 7569 7479 d40d  ...#.Xubiquity..
+0000a330: 0e0f 100a 1c16 1e09 10b5 085c 6461 7465  ...........\date
+0000a340: 4d6f 6469 6669 6564 d40d 0e0f 1016 1c16  Modified........
+0000a350: 2208 085b 6461 7465 4372 6561 7465 64d4  "..[dateCreated.
+0000a360: 0d0e 0f10 0a25 1627 0910 6108 5473 697a  .....%.'..a.Tsiz
+0000a370: 65d4 0d0e 0f10 0a2a 0a2c 0910 7309 546b  e......*.,..s.Tk
+0000a380: 696e 64d4 0d0e 0f10 162f 0a31 0810 6409  ind....../.1..d.
+0000a390: 556c 6162 656c d40d 0e0f 1016 340a 3608  Ulabel......4.6.
+0000a3a0: 104b 0957 7665 7273 696f 6ed4 0d0e 0f10  .K.Wversion.....
+0000a3b0: 1639 0a3b 0811 012c 0958 636f 6d6d 656e  .9.;...,.Xcommen
+0000a3c0: 7473 d40d 0e0f 1016 3e16 4008 10c8 085e  ts......>.@....^
+0000a3d0: 6461 7465 4c61 7374 4f70 656e 6564 d40d  dateLastOpened..
+0000a3e0: 0e0f 1016 1c16 4408 0859 6461 7465 4164  ......D..YdateAd
+0000a3f0: 6465 6408 2340 2800 0000 0000 0054 6e61  ded.#@(......Tna
+0000a400: 6d65 2340 3000 0000 0000 0009 0008 0019  me#@0...........
+0000a410: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
+0000a420: 008e 008f 009b 00a4 00ac 00b2 00bc 00c7  ................
+0000a430: 00c8 00cb 00cc 00d1 00da 00db 00dd 00de  ................
+0000a440: 00e7 00f0 00f1 00f3 00f4 0101 010a 010b  ................
+0000a450: 010c 0118 0121 0122 0124 0125 012a 0133  .....!.".$.%.*.3
+0000a460: 0134 0136 0137 013c 0145 0146 0148 0149  .4.6.7.<.E.F.H.I
+0000a470: 014f 0158 0159 015b 015c 0164 016d 016e  .O.X.Y.[.\.d.m.n
+0000a480: 0171 0172 017b 0184 0185 0187 0188 0197  .q.r.{..........
+0000a490: 01a0 01a1 01a2 01ac 01ad 01b6 01bb 01c4  ................
+0000a4a0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+0000a4b0: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+0000a4c0: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+0000a4d0: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+0000a4e0: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+0000a4f0: 006e 0064 0065 0072 0073 6c73 7670 626c  .n.d.e.r.slsvpbl
+0000a500: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
+0000a510: 0203 0405 0607 0809 0a0b 1d45 4647 0a5f  ...........EFG._
+0000a520: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+0000a530: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+0000a540: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+0000a550: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+0000a560: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+0000a570: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+0000a580: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+0000a590: 6573 1001 09d9 0c0d 0e0f 1011 1213 1415  es..............
+0000a5a0: 1e23 272b 3035 3a3f 5863 6f6d 6d65 6e74  .#'+05:?Xcomment
+0000a5b0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+0000a5c0: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
+0000a5d0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+0000a5e0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+0000a5f0: 6e54 6e61 6d65 d416 1718 191a 1b0a 1d55  nTname.........U
+0000a600: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
+0000a610: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
+0000a620: 012c 0908 d416 1718 191f 201d 1d10 0810  .,........ .....
+0000a630: c808 08d4 1617 1819 0924 1d0a 10b5 0809  .........$......
+0000a640: d416 1718 1928 241d 1d10 0208 08d4 1617  .....($.........
+0000a650: 1819 2c2d 1d0a 1003 1061 0809 d416 1718  ..,-.....a......
+0000a660: 1931 320a 1d10 0510 6409 08d4 1617 1819  .12.....d.......
+0000a670: 3637 0a0a 1004 1073 0909 d416 1718 193b  67.....s.......;
+0000a680: 3c0a 1d10 0610 4b09 08d4 1617 1819 4041  <.....K.......@A
+0000a690: 0a0a 1000 1101 a609 0908 2340 2800 0000  ..........#@(...
+0000a6a0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
+0000a6b0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+0000a6c0: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
+0000a6d0: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
+0000a6e0: 00ff 0105 010f 0117 0119 011c 011d 011e  ................
+0000a6f0: 0127 0129 012b 012c 012d 0136 0138 0139  .'.).+.,.-.6.8.9
+0000a700: 013a 0143 0145 0146 0147 0150 0152 0154  .:.C.E.F.G.P.R.T
+0000a710: 0155 0156 015f 0161 0163 0164 0165 016e  .U.V._.a.c.d.e.n
+0000a720: 0170 0172 0173 0174 017d 017f 0181 0182  .p.r.s.t.}......
+0000a730: 0183 018c 018e 0191 0192 0193 0194 019d  ................
+0000a740: 01a2 01ab 0000 0000 0000 0201 0000 0000  ................
+0000a750: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
+0000a760: 0000 01ac 0000 001b 0074 0068 0069 0072  .........t.h.i.r
+0000a770: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
+0000a780: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
+0000a790: 0070 0065 006e 0064 0065 0072 0073 6d6f  .p.e.n.d.e.r.smo
+0000a7a0: 4444 626c 6f62 0000 0008 b989 9f32 1302  DDblob.......2..
+0000a7b0: c541 0000 001b 0074 0068 0069 0072 0064  .A.....t.h.i.r.d
+0000a7c0: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
+0000a7d0: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
+0000a7e0: 0065 006e 0064 0065 0072 0073 6d6f 6444  .e.n.d.e.r.smodD
+0000a7f0: 626c 6f62 0000 0008 b989 9f32 1302 c541  blob.......2...A
+0000a800: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+0000a810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+0000a820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+0000a830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
+0000a840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
+0000a850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
+0000a860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
+0000a870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
+0000a880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
+0000a890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
+0000a8a0: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000a8b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+0000a8c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+0000a8d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+0000a8e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+0000a8f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+0000a900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+0000a910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+0000a920: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
+0000a930: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
+0000a940: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+0000a950: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000a960: 0000 0000 0000 0000 0000 0000 009b 0000  ................
+0000a970: 0002 0075 0069 6473 636c 626f 6f6c 0000  ...u.idsclbool..
+0000a980: 0000 0200 7500 696c 6731 5363 6f6d 7000  ....u.ilg1Scomp.
+0000a990: 0000 0000 0bda 1600 0000 0200 7500 696c  ............u.il
+0000a9a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
+0000a9b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+0000a9c0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+0000a9d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+0000a9e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+0000a9f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+0000aa00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+0000aa10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+0000aa20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+0000aa30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+0000aa40: 282d 3237 3c41 d40d 0e0f 100a 120a 1457  (-27<A.........W
+0000aa50: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+0000aa60: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
+0000aa70: 6572 0911 01c7 0954 6e61 6d65 d410 0e0f  er.....Tname....
+0000aa80: 0d16 1718 1858 7562 6971 7569 7479 1023  .....Xubiquity.#
+0000aa90: 0808 d410 0f0e 0d1b 181d 0a5c 6461 7465  ...........\date
+0000aaa0: 4d6f 6469 6669 6564 0810 b509 d410 0f0e  Modified........
+0000aab0: 0d20 181d 185b 6461 7465 4372 6561 7465  . ...[dateCreate
+0000aac0: 6408 08d4 100f 0e0d 2418 260a 5473 697a  d.......$.&.Tsiz
+0000aad0: 6508 1061 09d4 100f 0e0d 290a 2b0a 546b  e..a......).+.Tk
+0000aae0: 696e 6409 1073 09d4 100f 0e0d 2e0a 3018  ind..s........0.
+0000aaf0: 556c 6162 656c 0910 6408 d410 0f0e 0d33  Ulabel..d......3
+0000ab00: 0a35 1857 7665 7273 696f 6e09 104b 08d4  .5.Wversion..K..
+0000ab10: 100f 0e0d 380a 3a18 5863 6f6d 6d65 6e74  ....8.:.Xcomment
+0000ab20: 7309 1101 2c08 d410 0f0e 0d3d 183f 185e  s...,......=.?.^
+0000ab30: 6461 7465 4c61 7374 4f70 656e 6564 0810  dateLastOpened..
+0000ab40: c808 d410 0e0f 0d42 1d18 1859 6461 7465  .......B...Ydate
+0000ab50: 4164 6465 6408 0808 2340 2800 0000 0000  Added...#@(.....
+0000ab60: 0054 6e61 6d65 2340 3000 0000 0000 0009  .Tname#@0.......
+0000ab70: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+0000ab80: 0079 008c 008e 008f 009b 00a4 00ac 00b2  .y..............
+0000ab90: 00bc 00c7 00c8 00cb 00cc 00d1 00da 00e3  ................
+0000aba0: 00e5 00e6 00e7 00f0 00fd 00fe 0100 0101  ................
+0000abb0: 010a 0116 0117 0118 0121 0126 0127 0129  .........!.&.'.)
+0000abc0: 012a 0133 0138 0139 013b 013c 0145 014b  .*.3.8.9.;.<.E.K
+0000abd0: 014c 014e 014f 0158 0160 0161 0163 0164  .L.N.O.X.`.a.c.d
+0000abe0: 016d 0176 0177 017a 017b 0184 0193 0194  .m.v.w.z.{......
+0000abf0: 0196 0197 01a0 01aa 01ab 01ac 01ad 01b6  ................
+0000ac00: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
+0000ac10: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+0000ac20: 0000 01c5 0000 0002 0075 0069 6c73 7670  .........u.ilsvp
+0000ac30: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+0000ac40: d801 0203 0405 0607 0809 0a0b 1a45 4647  .............EFG
+0000ac50: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+0000ac60: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+0000ac70: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+0000ac80: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+0000ac90: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+0000aca0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+0000acb0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+0000acc0: 6174 6573 1001 09d9 0c0d 0e0f 1011 1213  ates............
+0000acd0: 1415 1e23 272b 3035 3a3f 5863 6f6d 6d65  ...#'+05:?Xcomme
+0000ace0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+0000acf0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+0000ad00: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+0000ad10: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+0000ad20: 696f 6e54 6e61 6d65 d416 1718 191a 0a1c  ionTname........
+0000ad30: 1d57 7669 7369 626c 6559 6173 6365 6e64  .WvisibleYascend
+0000ad40: 696e 6755 7769 6474 6855 696e 6465 7808  ingUwidthUindex.
+0000ad50: 0911 012c 1007 d416 1718 191a 1a21 2208  ...,.........!".
+0000ad60: 0810 c810 08d4 1617 1819 0a1a 2609 0908  ............&...
+0000ad70: 10b5 d416 1718 191a 1a26 2a08 0810 02d4  .........&*.....
+0000ad80: 1617 1819 0a1a 2e2f 0908 1061 1003 d416  ......./...a....
+0000ad90: 1718 191a 0a33 3408 0910 6410 05d4 1617  .....34...d.....
+0000ada0: 1819 0a0a 3839 0909 1073 1004 d416 1718  ....89...s......
+0000adb0: 191a 0a3d 3e08 0910 4b10 06d4 1918 1716  ...=>...K.......
+0000adc0: 4041 0a0a 1000 1101 c709 0908 2340 2800  @A..........#@(.
+0000add0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+0000ade0: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+0000adf0: 0065 0070 0079 008c 008e 008f 00a2 00ab  .e.p.y..........
+0000ae00: 00ba 00c7 00d3 00d8 00de 00e3 00eb 00f0  ................
+0000ae10: 00f9 0101 010b 0111 0117 0118 0119 011c  ................
+0000ae20: 011e 0127 0128 0129 012b 012d 0136 0137  ...'.(.).+.-.6.7
+0000ae30: 0138 013a 0143 0144 0145 0147 0150 0151  .8.:.C.D.E.G.P.Q
+0000ae40: 0152 0154 0156 015f 0160 0161 0163 0165  .R.T.V._.`.a.c.e
+0000ae50: 016e 016f 0170 0172 0174 017d 017e 017f  .n.o.p.r.t.}.~..
+0000ae60: 0181 0183 018c 018e 0191 0192 0193 0194  ................
+0000ae70: 019d 01a2 01ab 0000 0000 0000 0201 0000  ................
+0000ae80: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+0000ae90: 0000 0000 01ac 0000 0002 0075 0069 6d6f  ...........u.imo
+0000aea0: 4444 626c 6f62 0000 0008 c9ff d919 c904  DDblob..........
+0000aeb0: c541 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
+0000aec0: 6f62 0000 0008 c9ff d919 c904 c541 0000  ob...........A..
+0000aed0: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
+0000aee0: 0000 000f 1000 546f 6f6c 6261 725b 5368  ......Toolbar[Sh
+0000aef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+0000af00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+0000af10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+0000af20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+0000af30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
+0000af40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
+0000af50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+0000af60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+0000af70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
+0000af80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
+0000af90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
+0000b010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+0000b020: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
+0000b030: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000b040: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+0000b050: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+0000b060: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+0000b070: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+0000b080: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+0000b090: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+0000b0a0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+0000b0b0: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
+0000b0c0: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
+0000b0d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+0000b0e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000b0f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
+0000b100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+0000b110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
+0000b120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
+0000b130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
+0000b140: 6731 5363 6f6d 7000 0000 0000 060e 7e00  g1Scomp.......~.
+0000b150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
+0000b160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
+0000b170: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
+0000b180: 0102 0304 0506 0708 0909 0b18 4647 4849  ............FGHI
+0000b190: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+0000b1a0: 7465 735f 100f 7368 6f77 4963 6f6e 5072  tes_..showIconPr
+0000b1b0: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+0000b1c0: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+0000b1d0: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
+0000b1e0: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
+0000b1f0: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+0000b200: 696f 6e09 09ab 0c15 1a1f 2328 2d32 373c  ion.......#(-27<
+0000b210: 41d4 0d0e 0f10 1109 1309 5a69 6465 6e74  A.........Zident
+0000b220: 6966 6965 7259 6173 6365 6e64 696e 6755  ifierYascendingU
+0000b230: 7769 6474 6857 7669 7369 626c 6554 6e61  widthWvisibleTna
+0000b240: 6d65 0911 01c7 09d4 0d0f 0e10 1617 1818  me..............
+0000b250: 5875 6269 7175 6974 7910 2308 08d4 0d0e  Xubiquity.#.....
+0000b260: 0f10 1b18 1d09 5c64 6174 654d 6f64 6966  ......\dateModif
+0000b270: 6965 6408 10b5 09d4 0d0e 0f10 2018 1d18  ied......... ...
+0000b280: 5b64 6174 6543 7265 6174 6564 0808 d40d  [dateCreated....
+0000b290: 0e0f 1024 1826 0954 7369 7a65 0810 6109  ...$.&.Tsize..a.
+0000b2a0: d40d 0e0f 1029 092b 0954 6b69 6e64 0910  .....).+.Tkind..
+0000b2b0: 7309 d40d 0e0f 102e 0930 1855 6c61 6265  s........0.Ulabe
+0000b2c0: 6c09 1064 08d4 0d0e 0f10 3309 3518 5776  l..d......3.5.Wv
+0000b2d0: 6572 7369 6f6e 0910 4b08 d40d 0e0f 1038  ersion..K......8
+0000b2e0: 093a 1858 636f 6d6d 656e 7473 0911 012c  .:.Xcomments...,
+0000b2f0: 08d4 0d0e 0f10 3d18 3f18 5e64 6174 654c  ......=.?.^dateL
+0000b300: 6173 744f 7065 6e65 6408 10c8 08d4 0d0f  astOpened.......
+0000b310: 0e10 421d 1818 5964 6174 6541 6464 6564  ..B...YdateAdded
+0000b320: 0808 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+0000b330: 6523 4030 0000 0000 0000 1001 0008 0019  e#@0............
+0000b340: 002c 003e 0046 005a 0063 006e 0077 008c  .,.>.F.Z.c.n.w..
+0000b350: 008d 008e 009a 00a3 00ae 00b8 00be 00c6  ................
+0000b360: 00cb 00cc 00cf 00d0 00d9 00e2 00e4 00e5  ................
+0000b370: 00e6 00ef 00fc 00fd 00ff 0100 0109 0115  ................
+0000b380: 0116 0117 0120 0125 0126 0128 0129 0132  ..... .%.&.(.).2
+0000b390: 0137 0138 013a 013b 0144 014a 014b 014d  .7.8.:.;.D.J.K.M
+0000b3a0: 014e 0157 015f 0160 0162 0163 016c 0175  .N.W._.`.b.c.l.u
+0000b3b0: 0176 0179 017a 0183 0192 0193 0195 0196  .v.y.z..........
+0000b3c0: 019f 01a9 01aa 01ab 01ac 01b5 01ba 01c3  ................
+0000b3d0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+0000b3e0: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+0000b3f0: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
+0000b400: 0072 0076 0069 0073 0065 0064 6c73 7670  .r.v.i.s.e.dlsvp
+0000b410: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+0000b420: d801 0203 0405 0607 0809 090b 1a46 4748  .............FGH
+0000b430: 275f 1010 7573 6552 656c 6174 6976 6544  '_..useRelativeD
+0000b440: 6174 6573 5f10 0f73 686f 7749 636f 6e50  ates_..showIconP
+0000b450: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+0000b460: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+0000b470: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+0000b480: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+0000b490: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+0000b4a0: 7369 6f6e 0909 d90c 0d0e 0f10 1112 1314  sion............
+0000b4b0: 151e 2328 2c31 363b 4058 636f 6d6d 656e  ..#(,16;@Xcommen
+0000b4c0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+0000b4d0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
+0000b4e0: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+0000b4f0: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+0000b500: 6f6e 546e 616d 65d4 1617 1819 1a09 1c1d  onTname.........
+0000b510: 5776 6973 6962 6c65 5961 7363 656e 6469  WvisibleYascendi
+0000b520: 6e67 5577 6964 7468 5569 6e64 6578 0809  ngUwidthUindex..
+0000b530: 1101 2c10 07d4 1617 1819 1a1a 2122 0808  ..,.........!"..
+0000b540: 10c8 1008 d416 1718 1909 1a26 2709 0810  ...........&'...
+0000b550: b510 01d4 1617 1819 1a1a 262b 0808 1002  ..........&+....
+0000b560: d416 1718 1909 1a2f 3009 0810 6110 03d4  ......./0...a...
+0000b570: 1617 1819 1a09 3435 0809 1064 1005 d416  ......45...d....
+0000b580: 1718 1909 0939 3a09 0910 7310 04d4 1617  .....9:...s.....
+0000b590: 1819 1a09 3e3f 0809 104b 1006 d416 1718  ....>?...K......
+0000b5a0: 1909 0943 4409 0911 01c7 1000 0823 4028  ...CD........#@(
+0000b5b0: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+0000b5c0: 0000 0000 0008 0019 002c 003e 0046 005a  .........,.>.F.Z
+0000b5d0: 0063 006e 0077 008c 008d 008e 00a1 00aa  .c.n.w..........
+0000b5e0: 00b9 00c6 00d2 00d7 00dd 00e2 00ea 00ef  ................
+0000b5f0: 00f8 0100 010a 0110 0116 0117 0118 011b  ................
+0000b600: 011d 0126 0127 0128 012a 012c 0135 0136  ...&.'.(.*.,.5.6
+0000b610: 0137 0139 013b 0144 0145 0146 0148 0151  .7.9.;.D.E.F.H.Q
+0000b620: 0152 0153 0155 0157 0160 0161 0162 0164  .R.S.U.W.`.a.b.d
+0000b630: 0166 016f 0170 0171 0173 0175 017e 017f  .f.o.p.q.s.u.~..
+0000b640: 0180 0182 0184 018d 018e 018f 0192 0194  ................
+0000b650: 0195 019e 01a3 0000 0000 0000 0201 0000  ................
+0000b660: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+0000b670: 0000 0000 01ac 0000 000c 0075 006e 0073  ...........u.n.s
+0000b680: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b690: 0064 6d6f 4444 626c 6f62 0000 0008 6269  .dmoDDblob....bi
+0000b6a0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
+0000b6b0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b6c0: 0064 6d6f 6444 626c 6f62 0000 0008 6269  .dmodDblob....bi
+0000b6d0: 0543 3a05 c541 0000 000c 0075 006e 0073  .C:..A.....u.n.s
+0000b6e0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b6f0: 0064 7068 3153 636f 6d70 0000 0000 0007  .dph1Scomp......
+0000b700: 9000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+0000b710: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
+0000b720: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
+0000b730: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
+0000b740: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000b750: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+0000b760: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+0000b770: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+0000b780: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+0000b790: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+0000b7a0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+0000b7b0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+0000b7c0: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
+0000b7d0: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
+0000b7e0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+0000b7f0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000b800: 0000 0000 0000 0000 0000 0000 009b 005f  ..............._
+0000b810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+0000b820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+0000b830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
+0000b840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
+0000b850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
+0000b860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
+0000b870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
+0000b880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
+0000b890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
+0000b8a0: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000b8b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+0000b8c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+0000b8d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+0000b8e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+0000b8f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+0000b900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+0000b910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+0000b920: 0809 5f10 197b 7b32 3332 2c20 3139 317d  .._..{{232, 191}
+0000b930: 2c20 7b31 3330 322c 2037 3134 7d7d 0908  , {1302, 714}}..
+0000b940: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+0000b950: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000b960: 0000 0000 0000 0000 0000 0000 009b 0000  ................
+0000b970: 0002 0075 0069 6473 636c 626f 6f6c 0000  ...u.idsclbool..
+0000b980: 0000 0200 7500 696c 6731 5363 6f6d 7000  ....u.ilg1Scomp.
+0000b990: 0000 0000 0bda 1600 0000 0200 7500 696c  ............u.il
+0000b9a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
+0000b9b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+0000b9c0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+0000b9d0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+0000b9e0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+0000b9f0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+0000ba00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+0000ba10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+0000ba20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+0000ba30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+0000ba40: 282d 3237 3c41 d40d 0e0f 100a 120a 1457  (-27<A.........W
+0000ba50: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+0000ba60: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
+0000ba70: 6572 0911 01c7 0954 6e61 6d65 d410 0e0f  er.....Tname....
+0000ba80: 0d16 1718 1858 7562 6971 7569 7479 1023  .....Xubiquity.#
+0000ba90: 0808 d410 0f0e 0d1b 181d 0a5c 6461 7465  ...........\date
+0000baa0: 4d6f 6469 6669 6564 0810 b509 d410 0f0e  Modified........
+0000bab0: 0d20 181d 185b 6461 7465 4372 6561 7465  . ...[dateCreate
+0000bac0: 6408 08d4 100f 0e0d 2418 260a 5473 697a  d.......$.&.Tsiz
+0000bad0: 6508 1061 09d4 100f 0e0d 290a 2b0a 546b  e..a......).+.Tk
+0000bae0: 696e 6409 1073 09d4 100f 0e0d 2e0a 3018  ind..s........0.
+0000baf0: 556c 6162 656c 0910 6408 d410 0f0e 0d33  Ulabel..d......3
+0000bb00: 0a35 1857 7665 7273 696f 6e09 104b 08d4  .5.Wversion..K..
+0000bb10: 100f 0e0d 380a 3a18 5863 6f6d 6d65 6e74  ....8.:.Xcomment
+0000bb20: 7309 1101 2c08 d410 0f0e 0d3d 183f 185e  s...,......=.?.^
+0000bb30: 6461 7465 4c61 7374 4f70 656e 6564 0810  dateLastOpened..
+0000bb40: c808 d410 0e0f 0d42 1d18 1859 6461 7465  .......B...Ydate
+0000bb50: 4164 6465 6408 0808 2340 2800 0000 0000  Added...#@(.....
+0000bb60: 0054 6e61 6d65 2340 3000 0000 0000 0009  .Tname#@0.......
+0000bb70: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+0000bb80: 0079 008c 008e 008f 009b 00a4 00ac 00b2  .y..............
+0000bb90: 00bc 00c7 00c8 00cb 00cc 00d1 00da 00e3  ................
+0000bba0: 00e5 00e6 00e7 00f0 00fd 00fe 0100 0101  ................
+0000bbb0: 010a 0116 0117 0118 0121 0126 0127 0129  .........!.&.'.)
+0000bbc0: 012a 0133 0138 0139 013b 013c 0145 014b  .*.3.8.9.;.<.E.K
+0000bbd0: 014c 014e 014f 0158 0160 0161 0163 0164  .L.N.O.X.`.a.c.d
+0000bbe0: 016d 0176 0177 017a 017b 0184 0193 0194  .m.v.w.z.{......
+0000bbf0: 0196 0197 01a0 01aa 01ab 01ac 01ad 01b6  ................
+0000bc00: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
+0000bc10: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+0000bc20: 0000 01c5 0000 0002 0075 0069 6c73 7670  .........u.ilsvp
+0000bc30: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+0000bc40: d801 0203 0405 0607 0809 0a0b 1a45 4647  .............EFG
+0000bc50: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
+0000bc60: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+0000bc70: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+0000bc80: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+0000bc90: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+0000bca0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+0000bcb0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+0000bcc0: 6174 6573 1001 09d9 0c0d 0e0f 1011 1213  ates............
+0000bcd0: 1415 1e23 272b 3035 3a3f 5863 6f6d 6d65  ...#'+05:?Xcomme
+0000bce0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+0000bcf0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+0000bd00: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+0000bd10: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+0000bd20: 696f 6e54 6e61 6d65 d416 1718 191a 0a1c  ionTname........
+0000bd30: 1d57 7669 7369 626c 6559 6173 6365 6e64  .WvisibleYascend
+0000bd40: 696e 6755 7769 6474 6855 696e 6465 7808  ingUwidthUindex.
+0000bd50: 0911 012c 1007 d416 1718 191a 1a21 2208  ...,.........!".
+0000bd60: 0810 c810 08d4 1617 1819 0a1a 2609 0908  ............&...
+0000bd70: 10b5 d416 1718 191a 1a26 2a08 0810 02d4  .........&*.....
+0000bd80: 1617 1819 0a1a 2e2f 0908 1061 1003 d416  ......./...a....
+0000bd90: 1718 191a 0a33 3408 0910 6410 05d4 1617  .....34...d.....
+0000bda0: 1819 0a0a 3839 0909 1073 1004 d416 1718  ....89...s......
+0000bdb0: 191a 0a3d 3e08 0910 4b10 06d4 1918 1716  ...=>...K.......
+0000bdc0: 4041 0a0a 1000 1101 c709 0908 2340 2800  @A..........#@(.
+0000bdd0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+0000bde0: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+0000bdf0: 0065 0070 0079 008c 008e 008f 00a2 00ab  .e.p.y..........
+0000be00: 00ba 00c7 00d3 00d8 00de 00e3 00eb 00f0  ................
+0000be10: 00f9 0101 010b 0111 0117 0118 0119 011c  ................
+0000be20: 011e 0127 0128 0129 012b 012d 0136 0137  ...'.(.).+.-.6.7
+0000be30: 0138 013a 0143 0144 0145 0147 0150 0151  .8.:.C.D.E.G.P.Q
+0000be40: 0152 0154 0156 015f 0160 0161 0163 0165  .R.T.V._.`.a.c.e
+0000be50: 016e 016f 0170 0172 0174 017d 017e 017f  .n.o.p.r.t.}.~..
+0000be60: 0181 0183 018c 018e 0191 0192 0193 0194  ................
+0000be70: 019d 01a2 01ab 0000 0000 0000 0201 0000  ................
+0000be80: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+0000be90: 0000 0000 01ac 0000 0002 0075 0069 6d6f  ...........u.imo
+0000bea0: 4444 626c 6f62 0000 0008 c9ff d919 c904  DDblob..........
+0000beb0: c541 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
+0000bec0: 6f62 0000 0008 c9ff d919 c904 c541 0000  ob...........A..
+0000bed0: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
+0000bee0: 0000 000f 1000 546f 6f6c 6261 725b 5368  ......Toolbar[Sh
+0000bef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+0000bf00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+0000bf10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+0000bf20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+0000bf30: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
+0000bf40: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
+0000bf50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+0000bf60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+0000bf70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
+0000bf80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
+0000bf90: 3153 636f 6d70 0000 0000 0009 1744 0000  1Scomp.......D..
+0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     ----------
     >>> feature_extractor = ExtractFeaturesFrom14bps(config_path='MyProjectConfig')
     >>> feature_extractor.run()
     """
     
     def __init__(self,
                  config_path: str):
+
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         self.in_headers = self.get_feature_extraction_headers(pose='2 animals 14 body-parts')
         self.mouse_1_headers, self.mouse_2_headers = self.in_headers[0:21], self.in_headers[21:]
         self.mouse_2_p_headers = [x for x in self.mouse_2_headers if x[-2:] == '_p']
         self.mouse_1_p_headers = [x for x in self.mouse_1_headers if x[-2:] == '_p']
         self.mouse_1_headers = [x for x in self.mouse_1_headers if x[-2:] != '_p']
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,15 @@
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='7 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
             mouse_array = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_poly_area'] = jitted_hull(points=mouse_array, target='perimeter') / self.px_per_mm
-            self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
-            self.in_data = pd.concat([self.out_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
+            self.in_data = self.create_shifted_df(df=self.out_data)
             self.out_data['Mouse_nose_to_tail'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Tail_base_x'].values, self.in_data['Nose_y'].values, self.in_data['Tail_base_y'].values, self.px_per_mm)
             self.out_data['Mouse_width'] = self.euclidean_distance(self.in_data['Lat_left_x'].values, self.in_data['Lat_right_x'].values, self.in_data['Lat_left_y'].values, self.in_data['Lat_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Ear_distance'] = self.euclidean_distance(self.in_data['Ear_left_x'].values, self.in_data['Ear_right_x'].values, self.in_data['Ear_left_y'].values, self.in_data['Ear_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_centroid'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Center_x'].values, self.in_data['Nose_y'].values, self.in_data['Center_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_lateral_left'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Lat_left_x'].values, self.in_data['Nose_y'].values, self.in_data['Lat_left_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_lateral_right'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Lat_right_x'].values, self.in_data['Nose_y'].values, self.in_data['Lat_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Centroid_to_lateral_left'] = self.euclidean_distance(self.in_data['Center_x'].values, self.in_data['Lat_left_x'].values, self.in_data['Center_y'].values, self.in_data['Lat_left_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_subsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 import numpy as np
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
+
 from itertools import combinations
 from simba.feature_extractors.perimeter_jit import jitted_hull
-from simba.utils.enums import Formats
+from simba.utils.enums import Formats, Options
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
 
 
 class FeatureSubsetsCalculator(ConfigReader, FeatureExtractionMixin):
     def __init__(self,
                  config_path: str,
                  save_dir: str,
-                 feature_family: str):
+                 feature_family: Literal[Options.FEATURE_SUBSET_OPTIONS]):
 
         """
         Computes frame-wise user-defined family subset of features from pose for non-ML downstream purposes.
         E.g., returns the size of animal convex hull in each frame.
 
         :param config_path: path to SimBA configparser.ConfigParser project_config.ini
         :param save_dir: directory where to save the results.
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,17 @@
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='8 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
             mouse_1_ar = np.reshape(self.out_data[self.mouse_headers].values, (len(self.out_data / 2), -1, 2)).astype(np.float32)
             self.out_data['Mouse_poly_area'] = jitted_hull(points=mouse_1_ar, target=Formats.PERIMETER.value) / self.px_per_mm
-            self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
-            self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
+            self.in_data = self.create_shifted_df(df=self.out_data)
+
+
             self.out_data['Mouse_nose_to_tail'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Tail_base_x'].values, self.in_data['Nose_y'].values, self.in_data['Tail_base_y'].values, self.px_per_mm)
             self.out_data['Mouse_width'] = self.euclidean_distance(self.in_data['Lat_left_x'].values, self.in_data['Lat_right_x'].values, self.in_data['Lat_left_y'].values, self.in_data['Lat_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Ear_distance'] = self.euclidean_distance(self.in_data['Ear_left_x'].values, self.in_data['Ear_right_x'].values, self.in_data['Ear_left_y'].values, self.in_data['Ear_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_centroid'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Center_x'].values, self.in_data['Nose_y'].values, self.in_data['Center_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_lateral_left'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Lat_left_x'].values, self.in_data['Nose_y'].values, self.in_data['Lat_left_y'].values, self.px_per_mm)
             self.out_data['Mouse_Nose_to_lateral_right'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Lat_right_x'].values, self.in_data['Nose_y'].values, self.in_data['Lat_right_y'].values, self.px_per_mm)
             self.out_data['Mouse_Centroid_to_lateral_left'] = self.euclidean_distance(self.in_data['Center_x'].values, self.in_data['Lat_left_x'].values, self.in_data['Center_y'].values, self.in_data['Lat_left_y'].values, self.px_per_mm)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
             roll_windows = []
             for window in self.roll_windows_values:
                 roll_windows.append(int(fps / window))
             self.in_data = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric).reset_index(drop=True)
             print('Processing {} ({} frames)...'.format(self.video_name, str(len(self.in_data))))
             self.in_data = self.insert_default_headers_for_feature_extraction(df=self.in_data, headers=self.in_headers, pose_config='4 body-parts', filename=file_path)
             self.out_data = deepcopy(self.in_data)
-            self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
-            self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
+            self.in_data = self.create_shifted_df(df=self.out_data)
+
             print('Calculating euclidean distances...')
             self.out_data['Mouse_nose_to_tail'] = self.euclidean_distance(self.in_data['Nose_x'].values, self.in_data['Tail_base_x'].values, self.in_data['Nose_y'].values, self.in_data['Tail_base_y'].values, self.px_per_mm)
             self.out_data['Mouse_Ear_distance'] = self.euclidean_distance(self.in_data['Ear_left_x'].values, self.in_data['Ear_right_x'].values, self.in_data['Ear_left_y'].values, self.in_data['Ear_right_y'].values, self.px_per_mm)
             self.out_data['Movement_mouse_nose'] = self.euclidean_distance(self.in_data['Nose_x_shifted'].values, self.in_data['Nose_x'].values, self.in_data['Nose_y_shifted'].values, self.in_data['Nose_y'].values, self.px_per_mm)
             self.out_data['Movement_mouse_tail_base'] = self.euclidean_distance(self.in_data['Tail_base_x_shifted'].values, self.in_data['Tail_base_x'].values, self.in_data['Tail_base_y_shifted'].values, self.in_data['Tail_base_y'].values, self.px_per_mm)
             self.out_data['Movement_mouse_left_ear'] = self.euclidean_distance(self.in_data['Ear_left_x_shifted'].values, self.in_data['Ear_left_x'].values, self.in_data['Ear_left_y_shifted'].values, self.in_data['Ear_left_y'].values, self.px_per_mm)
             self.out_data['Movement_mouse_right_ear'] = self.euclidean_distance(self.in_data['Ear_right_x_shifted'].values, self.in_data['Ear_right_x'].values, self.in_data['Ear_right_y_shifted'].values, self.in_data['Ear_right_y'].values, self.px_per_mm)
@@ -216,14 +216,14 @@
             write_df(df=self.out_data, file_type=self.file_type, save_path=save_path)
             print(f'Feature extraction complete for {self.video_name} ({file_cnt + 1}/{len(self.files_found)})...')
 
         self.timer.stop_timer()
         stdout_success(msg='All features extracted. Results are stored in the project_folder/csv/features_extracted directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = ExtractFeaturesFrom4bps(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini')
-# test.extract_features()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.59.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/pop_up_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from tkinter import *
 from PIL import ImageTk
 import PIL.Image
 from tkinter import messagebox
 import os
 from simba.pose_importers import trk_importer
-from typing import Tuple
+from typing import Tuple, Optional, List
 
 
 from simba.utils.checks import (check_int,
                                 check_str,
                                 check_float,
                                 check_if_dir_exists)
 from simba.pose_importers.read_DANNCE_mat import import_DANNCE_file, import_DANNCE_folder
 from simba.pose_importers.import_mars import MarsImporter
-from simba.pose_importers.dlc_multi_animal_importer import MADLC_Importer
-from simba.pose_importers.sleap_importer_csv import SLEAPImporterCSV
-from simba.pose_importers.sleap_importer_h5 import SLEAPImporterH5
-from simba.pose_importers.sleap_importer_slp import SLEAPImporterSLP
+from simba.pose_importers.madlc_importer import MADLCImporterH5
+from simba.pose_importers.sleap_csv_importer import SLEAPImporterCSV
+from simba.pose_importers.sleap_h5_importer import SLEAPImporterH5
+from simba.pose_importers.sleap_slp_importer import SLEAPImporterSLP
 
 
 from simba.pose_importers.dlc_importer_csv import (import_multiple_dlc_tracking_csv_file, import_single_dlc_tracking_csv_file)
 from simba.utils.enums import ConfigKey, Options, Formats
 from simba.utils.read_write import find_core_cnt, copy_single_video_to_project, copy_multiple_videos_to_project, read_config_file, read_config_entry
 from simba.ui.tkinter_functions import (hxtScrollbar,
                                         DropDownMenu,
@@ -35,16 +35,16 @@
 from simba.utils.lookups import (get_icons_paths,
                                  get_color_dict,
                                  get_named_colors)
 
 class PopUpMixin(object):
     def __init__(self,
                  title: str,
-                 config_path: str or None = None,
-                 size: Tuple[int, int] = (400,400)):
+                 config_path: Optional[str] = None,
+                 size: Tuple[int, int] = (400, 400)):
 
         """
         Methods for pop-up windows in SimBa.
 
         :param str title: Pop-up window title
         :param configparser.Configparser config_path: path to SimBA project_config.ini
         :param tuple size: HxW of the pop-up window.
@@ -77,29 +77,30 @@
         self.clf_selections = {}
         for clf_cnt, clf in enumerate(clfs):
             self.clf_selections[clf] = BooleanVar(value=False)
             self.calculate_distance_moved_cb = Checkbutton(self.choose_clf_frm, text=clf, variable=self.clf_selections[clf])
             self.calculate_distance_moved_cb.grid(row=clf_cnt, column=0, sticky=NW)
         self.choose_clf_frm.grid(row=self.children_cnt_main(), column=0, sticky=NW)
 
-    def create_cb_frame(self, main_frm: Frame, cb_titles: list, frm_title: str):
+    def create_cb_frame(self, main_frm: Frame, cb_titles: list, frm_title: str) -> dict:
         cb_frm = LabelFrame(main_frm, text=frm_title, font=Formats.LABELFRAME_HEADER_FORMAT.value)
         cb_dict = {}
         for cnt, title in enumerate(cb_titles):
             cb_dict[title] = BooleanVar(value=False)
             cb = Checkbutton(cb_frm, text=title, variable=cb_dict[title])
             cb.grid(row=cnt, column=0, sticky=NW)
         cb_frm.grid(row=self.children_cnt_main(), column=0, sticky=NW)
         return cb_dict
 
     def create_dropdown_frame(self,
                               main_frm: Frame,
-                              drop_down_titles: list,
-                              drop_down_options: list,
+                              drop_down_titles: List[str],
+                              drop_down_options: List[str],
                               frm_title: str):
+
         dropdown_frm = LabelFrame(main_frm, text=frm_title, font=Formats.LABELFRAME_HEADER_FORMAT.value)
         dropdown_dict = {}
         for cnt, title in enumerate(drop_down_titles):
             dropdown_dict[title] = DropDownMenu(dropdown_frm, title, drop_down_options, '35')
             dropdown_dict[title].setChoices(drop_down_options[0])
             dropdown_dict[title].grid(row=cnt, column=0, sticky=NW)
         dropdown_frm.grid(row=self.children_cnt_main(), column=0, sticky=NW)
@@ -170,16 +171,16 @@
 
     def add_value_to_listbox(self,
                              list_box: Listbox,
                              value: float):
         list_box.insert(0, value)
 
     def add_values_to_several_listboxes(self,
-                                        list_boxes: list,
-                                        values: list):
+                                        list_boxes: List[Listbox],
+                                        values: List[float]):
         if len(list_boxes) != len(values):
             raise CountError(msg='Value count and listboxes count are not equal')
         for i in range(len(list_boxes)):
             list_boxes[i].insert(0, values[i])
 
     def remove_from_listbox(self,
                             list_box: Listbox):
@@ -208,25 +209,25 @@
         for bp_cnt in range(int(self.animal_cnt_dropdown.getChoices())):
             self.body_parts_dropdowns[bp_cnt] = DropDownMenu(self.body_part_frm, f'Body-part {str(bp_cnt + 1)}:', bp_options, '20')
             self.body_parts_dropdowns[bp_cnt].grid(row=bp_cnt, column=0, sticky=NW)
             self.body_parts_dropdowns[bp_cnt].setChoices(bp_options[bp_cnt])
 
 
 
-    def children_cnt_main(self):
+    def children_cnt_main(self) -> int:
         return int(len(list(self.main_frm.children.keys())))
 
-    def frame_children(self, frame: Frame):
+    def frame_children(self, frame: Frame) -> int:
         return int(len(list(frame.children.keys())))
 
-    def update_config(self):
+    def update_config(self) -> None:
         with open(self.config_path, 'w') as f:
             self.config.write(f)
 
-    def show_smoothing_entry_box_from_dropdown(self, choice):
+    def show_smoothing_entry_box_from_dropdown(self, choice: str):
         if choice == 'None':
             self.smoothing_time_eb.grid_forget()
         if (choice == 'Gaussian') or (choice == 'Savitzky Golay'):
             self.smoothing_time_eb.grid(row=0, column=1, sticky=E)
 
     def choose_bp_threshold_frm(self, parent: LabelFrame):
         self.probability_frm = LabelFrame(parent, text="PROBABILITY THRESHOLD", font=Formats.LABELFRAME_HEADER_FORMAT.value)
@@ -234,15 +235,15 @@
         self.probability_entry = Entry_Box(self.probability_frm, "Probability threshold: ", labelwidth=20)
         self.probability_entry.entry_set('0.00')
         self.probability_entry.grid(row=0, column=0, sticky=NW)
 
 
     def enable_dropdown_from_checkbox(self,
                                       check_box_var: BooleanVar,
-                                      dropdown_menus: [DropDownMenu]):
+                                      dropdown_menus: List[DropDownMenu]):
         if check_box_var.get():
             for menu in dropdown_menus:
                 menu.enable()
         else:
             for menu in dropdown_menus:
                 menu.disable()
 
@@ -271,15 +272,15 @@
                 self.animal_name_entry_boxes[i+1].entry_set(self.multi_animal_id_list[i])
             self.animal_name_entry_boxes[i+1].grid(row=i, column=0, sticky=NW)
 
         self.animal_names_frm.grid(row=1, column=0, sticky=NW)
 
     def enable_entrybox_from_checkbox(self,
                                       check_box_var: BooleanVar,
-                                      entry_boxes: [Entry_Box],
+                                      entry_boxes: List[Entry_Box],
                                       reverse: bool = False):
         if reverse:
             if check_box_var.get():
                 for box in entry_boxes:
                     box.set_state('disable')
             else:
                 for box in entry_boxes:
@@ -323,35 +324,29 @@
 
 
             self.config = read_config_file(config_path=self.config_path)
             self.config.set(ConfigKey.MULTI_ANIMAL_ID_SETTING.value, ConfigKey.MULTI_ANIMAL_IDS.value, ",".join(animal_ids))
             self.update_config()
 
             if data_type == 'H5 (multi-animal DLC)':
-                dlc_multi_animal_importer = MADLC_Importer(config_path=self.config_path,
+                dlc_multi_animal_importer = MADLCImporterH5(config_path=self.config_path,
                                                            data_folder=data_path,
                                                            file_type=tracking_data_type,
                                                            id_lst=animal_ids,
                                                            interpolation_settings=interpolation,
                                                            smoothing_settings=smooth_settings)
                 dlc_multi_animal_importer.run()
 
             if data_type == 'SLP (SLEAP)':
                 sleap_importer = SLEAPImporterSLP(project_path=self.config_path,
                                                   data_folder=data_path,
-                                                  actor_IDs=animal_ids,
+                                                  id_lst=animal_ids,
                                                   interpolation_settings=interpolation,
                                                   smoothing_settings=smooth_settings)
-                sleap_importer.initate_import_slp()
-                if sleap_importer.animals_no > 1:
-                    sleap_importer.visualize_sleap()
-                sleap_importer.save_df()
-                sleap_importer.perform_interpolation()
-                sleap_importer.perform_smothing()
-                print('All SLEAP imports complete.')
+                sleap_importer.run()
 
             if data_type == 'TRK (multi-animal APT)':
                 try:
                     trk_importer(self.config_path, data_path, animal_ids, interpolation, smooth_settings)
                 except Exception as e:
                     messagebox.showerror("Error", str(e))
 
@@ -362,18 +357,18 @@
                                                       interpolation_settings=interpolation,
                                                       smoothing_settings=smooth_settings)
                 sleap_csv_importer.run()
 
             if data_type == 'H5 (SLEAP)':
                 sleap_h5_importer = SLEAPImporterH5(config_path=self.config_path,
                                                     data_folder=data_path,
-                                                    actor_IDs=animal_ids,
+                                                    id_lst=animal_ids,
                                                     interpolation_settings=interpolation,
                                                     smoothing_settings=smooth_settings)
-                sleap_h5_importer.import_sleap()
+                sleap_h5_importer.run()
 
 
         def import_menu(data_type_choice: str):
             if hasattr(self, 'choice_frm'):
                 self.choice_frm.destroy()
             self.choice_frm = Frame(self.import_tracking_frm)
             self.animal_name_entry_boxes = None
@@ -395,15 +390,15 @@
                 if data_type_choice == 'CSV (DLC/DeepPoseKit)':
                     self.import_directory_frm = LabelFrame(self.choice_frm, text='IMPORT DLC CSV DIRECTORY', pady=5, padx=5)
                     self.import_directory_select = FolderSelect(self.import_directory_frm, 'Input DIRECTORY:', lblwidth=25)
                     self.import_dir_btn = Button(self.import_directory_frm, fg='blue', text='Import DIRECTORY to SimBA project', command= lambda: import_multiple_dlc_tracking_csv_file(config_path=self.config_path,
                                                                                                                                                                                interpolation_setting=self.interpolation_dropdown.getChoices(),
                                                                                                                                                                                smoothing_setting=self.smoothing_dropdown.getChoices(),
                                                                                                                                                                                smoothing_time=self.smoothing_time_eb.entry_get,
-                                                                                                                                                                               folder_path=self.import_directory_select.folder_path))
+                                                                                                                                                                               data_dir=self.import_directory_select.folder_path))
 
                     self.import_single_frm = LabelFrame(self.choice_frm, text='IMPORT DLC CSV FILE', pady=5, padx=5)
                     self.import_file_select = FileSelect(self.import_single_frm, 'Input FILE:', lblwidth=25)
                     self.import_file_btn = Button(self.import_single_frm, fg='blue', text='Import FILE to SimBA project', command= lambda: import_single_dlc_tracking_csv_file(config_path=self.config_path,
                                                                                                                                                                                interpolation_setting=self.interpolation_dropdown.getChoices(),
                                                                                                                                                                                smoothing_setting=self.smoothing_dropdown.getChoices(),
                                                                                                                                                                                smoothing_time=self.smoothing_time_eb.entry_get,
@@ -592,18 +587,15 @@
     #     print(f'+{e.x_root}+{e.y_root}')
     #     self.main_frm.geometry(f'+{e.x_root}+{e.y_root}')
     #     #print(f'+{e.x_root}x{e.y_root}')
     #     #self.main_frm.config(width=e.x_root, height=e.y_root)
     #     #self.main_frm.update()
 
 
-# test = PopUpMixin(config_path='/Users/simon/Desktop/envs/troubleshooting/Testsasd/project_folder/project_config.ini',
-#                   title='SHIT',
-#                   hyperlink='DAMN')
 
 # test = PopUpMixin(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini',
-#                   title='SHIT')
+#                   title='ss')
 # test.create_import_pose_menu(parent_frm=test.main_frm)
 
 # test = PopUpMixin(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini',
-#                   title='SHIT')
+#                   title='ss')
 # test.create_import_videos_menu(parent_frm=test.main_frm)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/config_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import shutil
 import logging
 from configparser import ConfigParser
 import os, glob
 import pandas as pd
 import itertools
 import cv2
+from typing import List, Optional, Tuple, Union, Dict
+
+
 from simba.utils.enums import (Paths,
                                ConfigKey,
                                Dtypes,
                                Defaults,
                                Keys)
 from simba.utils.lookups import get_emojis, get_color_dict
 from simba.utils.data import create_color_palettes
@@ -35,15 +38,15 @@
                                     get_all_clf_names)
 from simba.utils.checks import check_file_exist_and_readable
 
 
 class ConfigReader(object):
     def __init__(self,
                  config_path: str,
-                 read_video_info: bool=True):
+                 read_video_info: bool = True):
 
         """
         Methods for reading SimBA configparser.Configparser project config..
 
         :param configparser.Configparser config_path: path to SimBA project_config.ini
         :param bool read_video_info: if true, read the project_folder/logs/video_info.csv file.
         """
@@ -119,14 +122,15 @@
         -------
         roi_df: dict
         rectangles_df: pd.DataFrame
         circles_df: pd.DataFrame
         polygon_df: pd.DataFrame
         shape_names: list
         roi_dict: dict
+
         """
         if not os.path.isfile(self.roi_coordinates_path):
             raise NoROIDataError(msg='SIMBA ERROR: No ROI definitions were found in your SimBA project. Please draw some ROIs before analyzing your ROI data')
         else:
             self.rectangles_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_RECTANGLES.value).dropna(how='any')
             self.circles_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_CIRCLES.value).dropna(how='any')
             self.polygon_df = pd.read_hdf(self.roi_coordinates_path, key=Keys.ROI_POLYGONS.value)
@@ -161,15 +165,15 @@
         for i in range(self.clf_cnt):
             entry_name = 'target_name_{}'.format(str(i + 1))
             model_names.append(self.read_config_entry(self.config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
         return model_names
 
     def insert_column_headers_for_outlier_correction(self,
                                                      data_df: pd.DataFrame,
-                                                     new_headers: list,
+                                                     new_headers: List[str],
                                                      filepath: str):
         """
         Helper to insert new column headers onto a dataframe.
 
         Parameters
         ----------
         data_df:  pd.DataFrame
@@ -222,15 +226,15 @@
             except ValueError:
                 pass
         raise DataHeaderError(msg='Could find the count of header columns in dataframe')
 
 
     def find_video_of_file(self,
                            video_dir: str,
-                           filename: str):
+                           filename: str) -> str:
         """
         Helper to find the video file that represents a data file.
 
         Parameters
         ----------
         video_dir: str
             Directory holding putative video file
@@ -280,45 +284,45 @@
             shape_df['Thickness'] = [5] * len(shape_df)
         if not 'Color name' in shape_df.columns:
             shape_df['Color name'] = 'White'
 
         return shape_df
 
     def remove_a_folder(self,
-                        folder_dir: str):
+                        folder_dir: str) -> None:
         """Helper to remove a directory"""
         shutil.rmtree(folder_dir, ignore_errors=True)
 
     def find_animal_name_from_body_part_name(self,
                                              bp_name: str,
                                              bp_dict: dict) -> str:
 
         """Given body-part name and animal body-part dict, return animal name"""
 
         for animal_name, animal_bps in bp_dict.items():
             if bp_name in [x[:-2] for x in animal_bps['X_bps']]:
                 return animal_name
 
     def create_logger(self,
-                      path: str):
+                      path: str) -> None:
 
         logger = logging.getLogger()
         logger.setLevel(logging.INFO)
         handler = logging.FileHandler(filename=path, encoding='utf-8')  # or whatever
         handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(message)s'))
         logger.addHandler(handler)
 
     def create_body_part_dictionary(self,
                                     multi_animal_status: bool,
                                     animal_id_lst: list,
                                     animal_cnt: int,
-                                    x_cols: list,
-                                    y_cols: list,
-                                    p_cols: list or None=None,
-                                    colors: list or None=None):
+                                    x_cols: List[str],
+                                    y_cols: List[str],
+                                    p_cols: Optional[List[str]] = None,
+                                    colors: Optional[List[List[Tuple[int, int, int]]]] = None) -> Dict[str, Union[List[str], List[Tuple]]]:
         """
         Helper to create dict of dict lookup of body-parts where the keys are animal names, and
         values are the body-part names.
 
         Parameters
         ----------
         multi_animal_status: bool
@@ -409,45 +413,45 @@
 
         missing_body_part_fields = list(set(self.bp_col_names) - set(list(df.columns)))
         if len(missing_body_part_fields) > 0:
             BodypartColumnNotFoundWarning(msg=f'SimBA could not drop body-part coordinates, some body-part names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file: {missing_body_part_fields}')
         else:
             return df.drop(self.bp_col_names, axis=1)
 
-    def get_bp_headers(self) -> list:
+
+    def get_bp_headers(self) -> None:
         """
         Helper to create ordered list of all column header fields for SimBA project dataframes.
         """
         self.bp_headers = []
         for bp in self.body_parts_lst:
             c1, c2, c3 = (f'{bp}_x', f'{bp}_y', f'{bp}_p')
             self.bp_headers.extend((c1, c2, c3))
 
     def read_config_entry(self,
                           config: ConfigParser,
                           section: str,
                           option: str,
                           data_type: str,
-                          default_value=None,
-                          options=None):
+                          default_value = None,
+                          options = None) -> Union[str, int, float]:
 
         """ Helper to read entry in a configparser.ConfigParser object"""
         try:
             if config.has_option(section, option):
                 if data_type == Dtypes.FLOAT.value:
                     value = config.getfloat(section, option)
                 elif data_type == Dtypes.INT.value:
                     value = config.getint(section, option)
                 elif data_type == Dtypes.STR.value:
                     value = config.get(section, option).strip()
                 elif data_type == Dtypes.FOLDER.value:
                     value = config.get(section, option).strip()
                     if not os.path.isdir(value):
-                        raise NotDirectoryError(
-                            msg=f'The SimBA config file includes paths to a folder ({value}) that does not exist.')
+                        raise NotDirectoryError(msg=f'The SimBA config file includes paths to a folder ({value}) that does not exist.')
                 if options != None:
                     if value not in options:
                         raise InvalidInputError(
                             msg=f'{option} is set to {str(value)} in SimBA, but this is not among the valid options: ({options})')
                     else:
                         return value
                 return value
@@ -460,15 +464,15 @@
             if default_value != None:
                 return default_value
             else:
                 raise MissingProjectConfigEntryError(
                     msg=f'SimBA could not find an entry for option {option} under section {section} in the project_config.ini. Please specify the settings in the settings menu.')
 
     def read_video_info_csv(self,
-                            file_path: str):
+                            file_path: str) -> pd.DataFrame:
         """
         Helper to read the project_folder/logs/video_info.csv of the SimBA project in as a pd.DataFrame
         Parameters
         ----------
         file_path: str
 
         Returns
@@ -489,17 +493,17 @@
             except:
                 raise ParametersFileError(msg=f'One or more values in the {c} column of the "project_folder/logs/video_info.csv" file could not be interpreted as a numeric value. Please re-create the file and make sure the entries in the {c} column are all numeric.')
         if info_df['fps'].min() <= 1:
             InvalidValueWarning(msg='Videos in your SimBA project have an FPS of 1 or less. Please use videos with more than one frame per second, or correct the inaccurate fps inside the `project_folder/logs/videos_info.csv` file')
         return info_df
 
     def read_video_info(self,
-                        video_name: str):
+                        video_name: str) -> (pd.DataFrame, float, float):
         """
-        Helper to read the meta-data (pixels per mm, resolution, fps etc) from the video_info.csv for a single input file
+        Helper to read the meta-data (pixels per mm, resolution, fps) from the video_info.csv for a single input file
 
         Parameters
         ----------
         video_name: str
             The name of the video without extension to get the meta data for.
 
         Returns
@@ -518,15 +522,15 @@
             try:
                 px_per_mm = float(video_settings['pixels/mm'])
                 fps = float(video_settings['fps'])
                 return video_settings, px_per_mm, fps
             except TypeError:
                 raise ParametersFileError(msg=f'Make sure the videos that are going to be analyzed are represented with APPROPRIATE VALUES inside the project_folder/logs/video_info.csv file in your SimBA project. Could not interpret the fps, pixels per millimeter and/or fps as numerical values for video {video_name}')
 
-    def check_multi_animal_status(self):
+    def check_multi_animal_status(self) -> None:
         """
         Helper to check if the project is a multi-animal SimBA project.
 
         Parameters
         ----------
         config: configparser.ConfigParser
             Parsed SimBA project_config.ini file.
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/pose_importer_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import h5py
 
 
 import pandas as pd
 
 from simba.utils.errors import NoDataError, NoFilesFoundError, IntegerError, InvalidInputError, CountError
 from simba.utils.read_write import get_fn_ext
+from simba.utils.enums import ConfigKey
 
 class PoseImporterMixin(object):
     def __init__(self):
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         pass
 
     def initialize_multi_animal_ui(self,
@@ -242,14 +243,36 @@
         for animal_name, animal_bps in self.animal_bp_dict.items():
             x_cols, y_cols, p_cols = animal_bps['X_bps'], animal_bps['Y_bps'], animal_bps['P_bps']
             for x_col, y_col, p_col in zip(x_cols, y_cols, p_cols):
                 df = data[[x_col, y_col, p_col]]
                 results = pd.concat([results, df], axis=1)
         return results
 
+    def __update_config_animal_cnt(self):
+        self.config.set(ConfigKey.GENERAL_SETTINGS.value, ConfigKey.ANIMAL_CNT.value, str(self.animal_cnt))
+        with open(self.project_path, "w+") as f:
+            self.config.write(f)
+        f.close()
+
+    def update_bp_headers_file(self):
+        new_headers = []
+        for animal_name in self.animal_bp_dict.keys():
+            for bp in self.animal_bp_dict[animal_name]['X_bps']:
+                if animal_name not in bp:
+                    new_headers.append('{}_{}'.format(animal_name, bp[:-2]))
+                else:
+                    new_headers.append(bp[:-2])
+        new_bp_df = pd.DataFrame(new_headers)
+        new_bp_df.to_csv(self.body_parts_path, index=False, header=False)
+
+    def update_config_animal_names(self):
+        self.config.set(ConfigKey.MULTI_ANIMAL_ID_SETTING.value, ConfigKey.MULTI_ANIMAL_IDS.value, ",".join(str(x) for x in self.id_lst))
+        with open(self.project_path, "w+") as f:
+            self.config.write(f)
+        f.close()
 
     @staticmethod
     @jit(nopython=True)
     def transpose_multi_animal_table(data: np.array, idx: np.array, animal_cnt: int) -> np.array:
         results = np.full((np.max(idx[:, 1]), data.shape[1]*animal_cnt), 0.0)
         for i in prange(np.max(idx[:, 1])):
             for j in prange(animal_cnt):
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.59.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/feature_extraction_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 from scipy.spatial.qhull import QhullError
 from scipy.signal import savgol_filter
 import math
 import os, glob
 from scipy import stats
 import pandas as pd
 from scipy.signal import find_peaks
+from typing import Optional, List
+
+
 from simba.utils.enums import Paths, Options
 from simba.utils.checks import check_if_filepath_list_is_empty, check_file_exist_and_readable, check_minimum_roll_windows
 from simba.utils.read_write import (read_project_path_and_file_type,
                                     read_video_info_csv,
                                     read_config_file,
                                     get_bp_headers)
 from simba.utils.errors import CountError
 import simba
 
 class FeatureExtractionMixin(object):
 
     def __init__(self,
-                 config_path: str or None=None):
+                 config_path: Optional[str] = None):
 
         """
         Methods for featurizing pose-estimation data
         :param configparser.Configparser config_path: path to SimBA project_config.ini
         """
 
         if config_path:
@@ -54,34 +57,48 @@
     def euclidean_distance(bp_1_x_vals, bp_2_x_vals, bp_1_y_vals, bp_2_y_vals, px_per_mm):
         series = (np.sqrt((bp_1_x_vals - bp_2_x_vals) ** 2 + (bp_1_y_vals - bp_2_y_vals) ** 2)) / px_per_mm
         return series
 
 
     @staticmethod
     @jit(nopython=True, fastmath=True)
-    def angle3pt(ax, ay, bx, by, cx, cy):
+    def angle3pt(ax: float, ay: float, bx: float, by: float, cx: float, cy: float) -> float:
+        """
+        Jitted helper for single frame 3-point angle. For multiple frame 3-point angles, use
+        ``simba.mixins.feature_extraction_mixin.FeatureExtractionMixin.angle3pt_serialized``.
+
+        """
         ang = math.degrees(math.atan2(cy - by, cx - bx) - math.atan2(ay - by, ax - bx))
         return ang + 360 if ang < 0 else ang
 
     @staticmethod
     @jit(nopython=True, fastmath=True)
-    def angle3pt_serialized(data: np.array):
+    def angle3pt_serialized(data: np.ndarray) -> np.ndarray:
+        """
+        Jitted helper for frame-wise 3-point angles.
+
+        data : ndarray
+            2D numerical array with frame number on x and [ax, ay, bx, by, cx, cy] on y.
+        """
+
         results = np.full((data.shape[0]), 0.0)
         for i in prange(data.shape[0]):
             angle = math.degrees(
-                math.atan2(data[i][5] - data[i][3], data[i][4] - data[i][2]) - math.atan2(data[i][1] - data[i][3],
-                                                                                          data[i][0] - data[i][2]))
+                math.atan2(data[i][5] - data[i][3], data[i][4] - data[i][2]) - math.atan2(data[i][1] - data[i][3], data[i][0] - data[i][2]))
             if angle < 0:
                 angle += 360
             results[i] = angle
 
         return results
 
     @staticmethod
-    def convex_hull_calculator_mp(arr: np.array, px_per_mm: float) -> float:
+    def convex_hull_calculator_mp(arr: np.ndarray, px_per_mm: float) -> float:
+        """
+        Helper calculating single frame convex hull perimeter length. Call using ``parallel.delayed``.
+        """
         arr = np.unique(arr, axis=0).astype(int)
         if arr.shape[0] < 3:
             return 0
         for i in range(1, arr.shape[0]):
             if (arr[i] != arr[0]).all():
                 try:
                     return ConvexHull(arr, qhull_options='En').area / px_per_mm
@@ -89,54 +106,80 @@
                     return 0
             else:
                 pass
         return 0
 
     @staticmethod
     @jit(nopython=True)
-    def count_values_in_range(data: np.array, ranges: np.array):
+    def count_values_in_range(data: np.ndarray, ranges: np.ndarray) -> np.ndarray:
+        """
+        Jitted helper finding count of values within data that falls within ranges. Returns np.ndarray of
+        size data.shape[0], ranges.shape[1].
+        """
         results = np.full((data.shape[0], ranges.shape[0]), 0)
         for i in prange(data.shape[0]):
             for j in prange(ranges.shape[0]):
                 lower_bound, upper_bound = ranges[j][0], ranges[j][1]
                 results[i][j] = data[i][np.logical_and(data[i] >= lower_bound, data[i] <= upper_bound)].shape[0]
         return results
 
     @staticmethod
     @jit(nopython=True)
-    def framewise_euclidean_distance_roi(location_1: np.array,
-                                         location_2: np.array,
+    def framewise_euclidean_distance_roi(location_1: np.ndarray,
+                                         location_2: np.ndarray,
                                          px_per_mm: float,
-                                         centimeter: bool = False) -> np.array:
+                                         centimeter: bool = False) -> np.ndarray:
+        """
+        Jitted helper finding frame-wise distances between moving location (location_1) and static location (location_2)
+        in millimeter or centimeter.
+        """
 
         results = np.full((location_1.shape[0]), np.nan)
         for i in prange(location_1.shape[0]):
             results[i] = np.linalg.norm(location_1[i] - location_2) / px_per_mm
         if centimeter:
             results = results / 10
         return results
 
     @staticmethod
     @jit(nopython=True)
-    def framewise_inside_rectangle_roi(bp_location: np.array,
-                                       roi_coords: np.array) -> np.array:
+    def framewise_inside_rectangle_roi(bp_location: np.ndarray,
+                                       roi_coords: np.ndarray) -> np.ndarray:
+        """
+        Jitted helper for frame-wise detection of animal is inside static rectangular ROI.
+        Returns boolean 1d ndarray.
 
+        bp_location: np.ndarray
+            2d numeric np.ndarray size len(frames) x 2
+        roi_coords:
+            2d numeric np.ndarray size 1x2 (top left, bottom right)
+
+        """
         results = np.full((bp_location.shape[0]), 0)
         within_x_idx = np.argwhere((bp_location[:, 0] <= roi_coords[1][0]) & (bp_location[:, 0] >= roi_coords[0][0])).flatten()
         within_y_idx = np.argwhere((bp_location[:, 1] <= roi_coords[1][1]) & (bp_location[:, 1] >= roi_coords[0][1])).flatten()
         for i in prange(within_x_idx.shape[0]):
             match = np.argwhere(within_y_idx == within_x_idx[i])
             if match.shape[0] > 0:
                 results[within_x_idx[i]] = 1
         return results
 
     @staticmethod
     @jit(nopython=True)
-    def framewise_inside_polygon_roi(bp_location: np.array,
-                                     roi_coords: np.array) -> np.array:
+    def framewise_inside_polygon_roi(bp_location: np.ndarray,
+                                     roi_coords: np.ndarray) -> np.ndarray:
+
+        """
+        Jitted helper for frame-wise detection of animal is inside static polygon ROI.  Returns boolean 1d ndarray.
+
+        bp_location: np.ndarray
+            2d numeric np.ndarray size len(frames) x 2
+        roi_coords:
+            2d numeric np.ndarray size len(polygon points) x 2
+        """
         results = np.full((bp_location.shape[0]), 0)
         for i in prange(0, results.shape[0]):
             x, y, n = bp_location[i][0], bp_location[i][1], len(roi_coords)
             p2x, p2y, xints, inside = 0.0, 0.0, 0.0, False
             p1x, p1y = roi_coords[0]
             for j in prange(n + 1):
                 p2x, p2y = roi_coords[j % n]
@@ -148,21 +191,20 @@
                 p1x, p1y = p2x, p2y
             if inside:
                 results[i] = 1
 
         return results
 
     def windowed_frequentist_distribution_tests(self,
-                                                data: np.array,
+                                                data: np.ndarray,
                                                 feature_name: str,
-                                                fps: int):
+                                                fps: int) -> pd.DataFrame:
         """
-        Helper to compare feature value distributions in 1-s sequential time-bins: Kolmogorov-Smirnov and T-tests
-        Compares the feature values against a normal distribution: Shapiro.
-        Find the number of peaks in *rolling* 1s long feature window.
+        Helper to compare (i) feature value distributions in 1-s sequential time-bins: Kolmogorov-Smirnov and T-tests,
+        (ii) compare feature values against a normal distribution: Shapiro, and (iii) find peak count in *rolling* 1s long feature window.
         """
 
         ks_results, = np.full((data.shape[0]), -1.0),
         t_test_results = np.full((data.shape[0]), -1.0)
         shapiro_results = np.full((data.shape[0]), -1.0)
         peak_cnt_results = np.full((data.shape[0]), -1.0)
 
@@ -186,23 +228,30 @@
 
         return pd.DataFrame(
             np.column_stack((ks_results, t_test_results, shapiro_results, peak_cnt_results)),
             columns=columns).round(4).fillna(0)
 
     @staticmethod
     @jit(nopython=True, cache=True)
-    def cdist(array_1: np.array, array_2: np.array):
+    def cdist(array_1: np.ndarray,
+              array_2: np.ndarray) -> np.ndarray:
+        """
+        Jitted analogue of scipy.cdist.
+        """
         results = np.full((array_1.shape[0], array_2.shape[0]), np.nan)
         for i in prange(array_1.shape[0]):
             for j in prange(array_2.shape[0]):
                 results[i][j] = np.linalg.norm(array_1[i] - array_2[j])
         return results
 
     @staticmethod
-    def create_shifted_df(df: pd.DataFrame):
+    def create_shifted_df(df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Helper for creating df with duplicated shifted columns with ``_shifted`` suffix.
+        """
         data_df_shifted = df.shift(periods=1)
         data_df_shifted = data_df_shifted.combine_first(df).add_suffix('_shifted')
         return pd.concat([df, data_df_shifted], axis=1, join='inner').reset_index(drop=True)
 
     def check_directionality_viable(self):
         """
         Helper to check if it is possible to calculate ``directionality`` statistics (i.e., nose, and ear coordinates from
@@ -245,28 +294,28 @@
             nose_cords = [nose_cords[i * 2:(i + 1) * 2] for i in range((len(nose_cords) + 2 - 1) // 2)]
             ear_left_cords = [ear_left_cords[i * 2:(i + 1) * 2] for i in range((len(ear_left_cords) + 2 - 1) // 2)]
             ear_right_cords = [ear_right_cords[i * 2:(i + 1) * 2] for i in range((len(ear_right_cords) + 2 - 1) // 2)]
 
         return direction_viable, nose_cords, ear_left_cords, ear_right_cords
 
     def get_feature_extraction_headers(self,
-                                       pose: str):
-        """ Helper to return the headers names that should be used during feature extraction"""
+                                       pose: str) -> List[str]:
+        """ Helper to return the headers names (body-part location columns) that should be used during feature extraction"""
         simba_dir = os.path.dirname(simba.__file__)
         feature_categories_csv_path = os.path.join(simba_dir, Paths.SIMBA_FEATURE_EXTRACTION_COL_NAMES_PATH.value)
         check_file_exist_and_readable(file_path=feature_categories_csv_path)
         bps = list(pd.read_csv(feature_categories_csv_path)[pose])
         return [x for x in bps if str(x) != 'nan']
 
     @staticmethod
     @jit(nopython=True)
-    def jitted_line_crosses_to_nonstatic_targets(left_ear_array: np.array,
-                                                 right_ear_array: np.array,
-                                                 nose_array: np.array,
-                                                 target_array: np.array) -> np.array:
+    def jitted_line_crosses_to_nonstatic_targets(left_ear_array: np.ndarray,
+                                                 right_ear_array: np.ndarray,
+                                                 nose_array: np.ndarray,
+                                                 target_array: np.ndarray) -> np.ndarray:
         """
         Jitted helper to calculate if an animal is directing towards another animals body-part coordinate.
 
         Parameters
         ----------
         left_ear_array: array
             left ear coordinates of observing animal.
@@ -300,18 +349,18 @@
             else:
                 results_array[frame_no] = [2, -1, -1, False]
 
         return results_array
 
     @staticmethod
     @jit(nopython=True)
-    def jitted_line_crosses_to_static_targets(left_ear_array: np.array,
-                                              right_ear_array: np.array,
-                                              nose_array: np.array,
-                                              target_array: np.array) -> np.array:
+    def jitted_line_crosses_to_static_targets(left_ear_array: np.ndarray,
+                                              right_ear_array: np.ndarray,
+                                              nose_array: np.ndarray,
+                                              target_array: np.ndarray) -> np.ndarray:
         """
         Jitted helper to calculate if an animal is directing towards a static coordinate
         (e.g., the center of a user-defined ROI)
 
         Parameters
         ----------
         left_ear_array: array
@@ -346,19 +395,21 @@
             else:
                 results_array[frame_no] = [2, -1, -1, False]
 
         return results_array
 
 
     def minimum_bounding_rectangle(self,
-                                   points: np.array) -> np.array:
+                                   points: np.ndarray) -> np.ndarray:
 
         """
-        Finds the minimum bounding rectangle of a convex hull
+        Finds the minimum bounding rectangle of a convex hull perimeter.
         https://stackoverflow.com/questions/13542855/algorithm-to-find-the-minimum-area-rectangle-for-given-points-in-order-to-comput
+
+        TODO: Place in numba njit.
         """
 
         pi2 = np.pi / 2.
         hull_points = points[ConvexHull(points).vertices]
         edges = hull_points[1:] - hull_points[:-1]
         angles = np.arctan2(edges[:, 1], edges[:, 0])
         angles = np.abs(np.mod(angles, pi2))
@@ -379,41 +430,49 @@
         return rval
 
 
 
 
     @staticmethod
     @jit(nopython=True)
-    def framewise_euclidean_distance(location_1: np.array,
-                                     location_2: np.array,
+    def framewise_euclidean_distance(location_1: np.ndarray,
+                                     location_2: np.ndarray,
                                      px_per_mm: float,
-                                     centimeter: bool = False) -> np.array:
-
+                                     centimeter: bool = False) -> np.ndarray:
+        """
+        Jitted helper finding frame-wise distances between two non-static locations in millimeter or centimeter.
+        """
         results = np.full((location_1.shape[0]), np.nan)
         for i in prange(location_1.shape[0]):
             results[i] = np.linalg.norm(location_1[i] - location_2[i]) / px_per_mm
         if centimeter:
             results = results / 10
         return results
 
     def dataframe_gaussian_smoother(self,
                                     df: pd.DataFrame,
                                     fps: int,
-                                    time_window: int=100):
+                                    time_window: int=100) -> pd.DataFrame:
+        """
+        Helper performing column-wise Gaussian smoothing of dataframe.
+        """
 
         frames_in_time_window = int(time_window / (1000 / fps))
         for c in df.columns:
             df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
         return df
 
 
     def dataframe_savgol_smoother(self,
                                   df: pd.DataFrame,
                                   fps: int,
                                   time_window: int = 150):
+        """
+         Helper performing column-wise Savitzky-Golay smoothing of dataframe.
+         """
         frames_in_time_window = int(time_window / (1000 / fps))
         if (frames_in_time_window % 2) == 0: frames_in_time_window = frames_in_time_window - 1
         if (frames_in_time_window % 2) <= 3: frames_in_time_window = 5
         for c in df.columns:
             df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
         return df
 
@@ -462,35 +521,35 @@
                         results[animal]['Ear_right']['X_bps'] = cord
                     elif ("right" in cord.lower()) and ("y" in cord.lower()) and ("ear".lower() in cord.lower()):
                         results[animal]['Ear_right']['Y_bps'] = cord
         return results
 
     def insert_default_headers_for_feature_extraction(self,
                                                       df: pd.DataFrame,
-                                                      headers: list,
+                                                      headers: List[str],
                                                       pose_config: str,
-                                                      filename: str):
+                                                      filename: str) -> pd.DataFrame:
         if len(headers) != len(df.columns):
             raise CountError(f'Your SimBA project is set to using the default {pose_config} pose-configuration. '
                              f'SimBA therefore expects {str(len(headers))} columns of data inside the files within the project_folder. However, '
                              f'within file {filename} file, SimBA found {str(len(df.columns))} columns.')
         else:
             df.columns = headers
             return df
 
-    def line_crosses_to_static_targets(p: list,
-                                       q: list,
-                                       n: list,
-                                       M: list,
-                                       coord: list):
+    @staticmethod
+    def line_crosses_to_static_targets(p: List[float],
+                                       q: List[float],
+                                       n: List[float],
+                                       M: List[float],
+                                       coord: List[float]):
         """
-        Non-jitted helper to calculate if an animal is directing towards a coordinate.
+        Legacy non-jitted helper to calculate if an animal is directing towards a coordinate.
         For improved runtime, use ``simba.mixins.feature_extraction_mixin.jitted_line_crosses_to_static_targets``
 
-
         Parameters
         ----------
         p: list
             left ear coordinates of observing animal.
         q: list
             right ear coordinates of observing animal.
         n: list
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/plotting_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 import matplotlib
 import shutil
 import random
 from matplotlib import cm
 import imutils
 import itertools
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
+from typing import List, Tuple, Optional
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
 
 import simba
 from simba.utils.lookups import get_color_dict, get_named_colors
 from simba.utils.read_write import get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
-from simba.utils.enums import Formats
+from simba.utils.enums import Formats, Options
 
 class PlottingMixin(object):
     def __init__(self):
 
         """
         Methods for plotting
         """
@@ -88,15 +93,15 @@
 
         return open_cv_image
 
     def create_single_color_lst(self,
                                 pallete_name: str,
                                 increments: int,
                                 as_rgb_ratio: bool = False,
-                                as_hex: bool = False) -> list:
+                                as_hex: bool = False) -> List[int]:
         """
         Helper to create a color palette of bgr colors in a list.
         Parameters
         ----------
         pallete_name: str
             Palette name (e.g., 'jet')
         increments: int
@@ -119,23 +124,26 @@
             if as_hex:
                 rgb = matplotlib.colors.to_hex(rgb)
             color_lst.append(rgb)
         return color_lst
 
     def remove_a_folder(self,
                         folder_dir: str):
-        """Helper to remove a directory"""
+        """Helper to remove a directory, use for cleaning up smaller multiprocessed videos following concat"""
         shutil.rmtree(folder_dir, ignore_errors=True)
 
     def split_and_group_df(self,
                            df: pd.DataFrame,
                            splits: int,
-                           include_split_order: bool = True):
+                           include_split_order: bool = True) -> (List[pd.DataFrame], int):
 
-        """Helper to split a dataframe for multiprocessing"""
+        """
+        Helper to split a dataframe for multiprocessing. If include_split_order, then include the group number in split data.
+        Returns split data and approximations of number of observations per split.
+        """
 
         data_arr = np.array_split(df, splits)
         if include_split_order:
             for df_cnt in range(len(data_arr)):
                 data_arr[df_cnt]['group'] = df_cnt
         obs_per_split = len(data_arr[0])
 
@@ -143,15 +151,15 @@
 
     def make_distance_plot(self,
                            data: np.array,
                            line_attr: dict,
                            style_attr: dict,
                            fps: int,
                            save_path: str or None = None,
-                           save_img: bool = False):
+                           save_img: bool = False) -> np.ndarray:
         """
         Helper to make a single line plot .png image with N lines.
 
         Parameters
         ----------
         data: np.array
             Two-dimensional array where rows represent frames and columns represent values.
@@ -215,16 +223,16 @@
         else:
             return img
 
     def make_probability_plot(self,
                               data: pd.Series,
                               style_attr: dict,
                               clf_name: str,
-                              fps,
-                              save_path: str):
+                              fps: int,
+                              save_path: str) -> np.ndarray:
         """
         Helper to make a single classifier probability plot png image.
 
         Parameters
         ----------
         data: pd.Series
             With row representing frames and field representing classification probabilities.
@@ -289,15 +297,15 @@
 
     def make_path_plot(self,
                        data_df: pd.DataFrame,
                        video_info: pd.DataFrame,
                        style_attr: dict,
                        deque_dict: dict,
                        clf_attr: dict,
-                       save_path: str or None):
+                       save_path: str or None) -> np.ndarray:
 
         video_timer = SimbaTimer(start=True)
         for frm_cnt in range(len(data_df)):
             for animal_cnt, (animal_name, animal_data) in enumerate(deque_dict.items()):
                 bp_x = int(data_df.loc[frm_cnt, '{}_{}'.format(animal_data['bp'], 'x')])
                 bp_y = int(data_df.loc[frm_cnt, '{}_{}'.format(animal_data['bp'], 'y')])
                 deque_dict[animal_name]['deque'].appendleft((bp_x, bp_y))
@@ -333,19 +341,19 @@
         img = cv2.resize(img, (style_attr['width'], style_attr['height']))
         cv2.imwrite(save_path, img)
         stdout_success(msg=f'Final path plot saved at {save_path}', elapsed_time=video_timer.elapsed_time_str)
 
     def make_gantt_plot(self,
                         data_df: pd.DataFrame,
                         bouts_df: pd.DataFrame,
-                        clf_names: list,
+                        clf_names: List[str],
                         fps: int,
                         style_attr: dict,
                         video_name: str,
-                        save_path: str):
+                        save_path: str) -> np.ndarray:
 
         video_timer = SimbaTimer(start=True)
         colours = get_named_colors()
         colour_tuple_x = list(np.arange(3.5, 203.5, 5))
         fig, ax = plt.subplots()
         for i, event in enumerate(bouts_df.groupby("Event")):
             for x in clf_names:
@@ -377,20 +385,20 @@
         video_timer.stop_timer()
         stdout_success(msg=f'Final gantt frame for video {video_name} saved at {save_path}',
                        elapsed_time=video_timer.elapsed_time_str)
 
     def make_clf_heatmap_plot(self,
                               frm_data: np.array,
                               max_scale: float,
-                              palette: str,
+                              palette: Literal[Options.PALETTE_OPTIONS],
                               aspect_ratio: float,
-                              shading: str,
+                              shading: Literal['gouraud', 'flat'],
                               clf_name: str,
-                              img_size: tuple,
-                              file_name: str or None = None,
+                              img_size: Tuple[int, int],
+                              file_name: Optional[str] = None,
                               final_img: bool = False):
 
         cum_df = pd.DataFrame(frm_data).reset_index()
         cum_df = cum_df.melt(id_vars='index', value_vars=None, var_name=None, value_name='seconds',
                              col_level=None).rename(columns={'index': 'vertical_idx', 'variable': 'horizontal_idx'})
         cum_df['color'] = (cum_df['seconds'].astype(float) / float(max_scale)).round(2).clip(upper=100)
         color_array = np.zeros((len(cum_df['vertical_idx'].unique()), len(cum_df['horizontal_idx'].unique())))
@@ -426,18 +434,18 @@
             stdout_success(msg=f'Final classifier heatmap image saved at at {file_name}')
         else:
             return image
 
     def make_location_heatmap_plot(self,
                                    frm_data: np.array,
                                    max_scale: float,
-                                   palette: str,
+                                   palette: Literal[Options.PALETTE_OPTIONS],
                                    aspect_ratio: float,
                                    shading: str,
-                                   img_size: tuple,
+                                   img_size: Tuple[int, int],
                                    file_name: str or None = None,
                                    final_img: bool = False):
 
         cum_df = pd.DataFrame(frm_data).reset_index()
         cum_df = cum_df.melt(id_vars='index', value_vars=None, var_name=None, value_name='seconds',
                              col_level=None).rename(columns={'index': 'vertical_idx', 'variable': 'horizontal_idx'})
         cum_df['color'] = (cum_df['seconds'].astype(float) / float(max_scale)).round(2).clip(upper=100)
@@ -473,15 +481,15 @@
             stdout_success(msg=f'Final location heatmap image saved at at {file_name}')
         else:
             return image
 
     def get_bouts_for_gantt(self,
                             data_df: pd.DataFrame,
                             clf_name: str,
-                            fps: int):
+                            fps: int) -> np.ndarray:
         """
         Helper to detect all behavior bouts for a specific classifier.
 
         Parameters
         ----------
         data_df: pd.DataFrame
             Pandas Dataframe with classifier prediction data.
@@ -515,17 +523,17 @@
             endFrameList.append(endFrame)
 
         return pd.DataFrame(list(zip(nameList, startTimeList, endTimeList, endFrameList, boutsList)),
                             columns=['Event', 'Start_time', 'End Time', 'End_frame', 'Bout_time'])
 
     def resize_gantt(self,
                      gantt_img: np.array,
-                     img_height: int):
+                     img_height: int) -> np.ndarray:
         """
-        Helper to resize a image in array format.
+        Helper to resize image.
         """
 
         return imutils.resize(gantt_img, height=img_height)
 
     @staticmethod
     def roi_feature_visualizer_mp(data: pd.DataFrame,
                                   text_locations: dict,
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.59.2/simba/mixins/train_model_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import configparser
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
 import multiprocessing
+from typing import List, Optional
 
 from simba.utils.enums import ConfigKey, Dtypes, MetaKeys, Defaults
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
 from simba.utils.data import detect_bouts, create_color_palette
 from simba.utils.read_write import find_core_cnt, get_memory_usage_of_df, read_config_entry, read_df, get_fn_ext
 from simba.utils.checks import (check_int,
                                 check_str,
@@ -58,17 +59,17 @@
     def __init__(self):
         pass
     """
     Methods for training and evaluating classifiers.
     """
 
     def read_all_files_in_folder(self,
-                                 file_paths: list,
+                                 file_paths: List[str],
                                  file_type: str,
-                                 classifier_names=None):
+                                 classifier_names: Optional[List[str]] = None) -> pd.DataFrame:
         """
         Helper function to read in all data files in a folder to a single pd.DataFrame for downstream ML algorithm.
         Asserts that all classifiers have annotation fields present in concatenated dataframes.
 
         Parameters
         ----------
         file_paths: list
@@ -112,15 +113,15 @@
         timer.stop_timer()
         memory_size = get_memory_usage_of_df(df=df_concat)
         print(f'Dataset size: {memory_size["megabytes"]}MB / {memory_size["gigabytes"]}GB')
         print('{} file(s) read (elapsed time: {}s) ...'.format(str(len(file_paths)), timer.elapsed_time_str))
         return df_concat.astype(np.float32)
 
     def read_in_all_model_names_to_remove(self,
-                                          config: configparser,
+                                          config: configparser.ConfigParser,
                                           model_cnt: int,
                                           clf_name: str):
         """
         Helper to find all field names that contain annotations but are not the target.
 
         Parameters
         ----------
@@ -141,15 +142,15 @@
             model_name = config.get(ConfigKey.SML_SETTINGS.value, 'target_name_' + str(model_no + 1))
             if model_name != clf_name:
                 annotation_cols_to_remove.append(model_name)
         return annotation_cols_to_remove
 
     def delete_other_annotation_columns(self,
                                         df: pd.DataFrame,
-                                        annotations_lst: list):
+                                        annotations_lst: List[str]) -> pd.DataFrame:
         """
         Helper to delete fields that contain annotations which are not the target.
 
         Parameters
         ----------
         df: pd.DataFrame
             pandas Dataframe holding features and annotations.
@@ -163,15 +164,15 @@
 
         for a_col in annotations_lst:
             df = df.drop([a_col], axis=1)
         return df
 
     def split_df_to_x_y(self,
                         df: pd.DataFrame,
-                        clf_name: str):
+                        clf_name: str) -> (pd.DataFrame, pd.DataFrame):
         """
         Helper to split dataframe into features and target.
 
         Parameters
         ----------
         df: pd.DataFrame
             pandas Dataframe holding features and annotations.
@@ -185,17 +186,17 @@
         """
 
         df = deepcopy(df)
         y = df.pop(clf_name)
         return df, y
 
     def random_undersampler(self,
-                            x_train: np.array,
-                            y_train: np.array,
-                            sample_ratio: float):
+                            x_train: np.ndarray,
+                            y_train: np.ndarray,
+                            sample_ratio: float) -> (pd.DataFrame, pd.DataFrame):
         """
         Helper to perform random undersampling of behavior-absent frames in a dataframe.
 
         Parameters
         ----------
         x_train: pd.DataFrame
             Features in train set
@@ -220,15 +221,15 @@
                 msg=f'SIMBA UNDER SAMPLING ERROR: The under-sample ratio of {str(sample_ratio)} in classifier {y_train.name} demands {str(ratio_n)} behavior-absent annotations. This is more than the number of behavior-absent annotations in the entire dataset {str(len(absent_df))}. Please annotate more images or decrease the under-sample ratio.')
         data_df = pd.concat([present_df, absent_df.sample(n=ratio_n, replace=False)], axis=0)
         return self.split_df_to_x_y(data_df, y_train.name)
 
     def smoteen_oversampler(self,
                             x_train: pd.DataFrame,
                             y_train: pd.DataFrame,
-                            sample_ratio: float):
+                            sample_ratio: float) -> (np.ndarray, np.ndarray):
 
         """
         Helper to perform smoteen oversampling of behavior-present frames in a dataframe
 
         Parameters
         ----------
         x_train: pd.DataFrame or array
@@ -248,15 +249,15 @@
         print('Performing SMOTEEN oversampling...')
         smt = SMOTEENN(sampling_strategy=sample_ratio)
         return smt.fit_sample(x_train, y_train)
 
     def smote_oversampler(self,
                           x_train: pd.DataFrame or np.array,
                           y_train: pd.DataFrame or np.array,
-                          sample_ratio: float):
+                          sample_ratio: float) -> (np.ndarray, np.ndarray):
         """
         Helper to perform smote oversampling of behavior-present frames in a dataframe
 
         Parameters
         ----------
         x_train: pd.DataFrame or array
             pandas Dataframe holding features and annotations.
@@ -272,21 +273,21 @@
 
         """
         print('Performing SMOTE oversampling...')
         smt = SMOTE(sampling_strategy=sample_ratio)
         return smt.fit_sample(x_train, y_train)
 
     def calc_permutation_importance(self,
-                                    x_test: np.array,
-                                    y_test: np.array,
+                                    x_test: np.ndarray,
+                                    y_test: np.ndarray,
                                     clf: RandomForestClassifier,
-                                    feature_names: list,
+                                    feature_names: List[str],
                                     clf_name: str,
                                     save_dir: str,
-                                    save_file_no=None):
+                                    save_file_no: Optional[int] = None):
         """
         Helper to calculate feature permutation importance scores.
 
         Parameters
         ----------
         x_test: np.array,
             Array holding feature test data
@@ -330,15 +331,15 @@
                             x_y_df: pd.DataFrame,
                             clf_name: str,
                             shuffle_splits: int,
                             dataset_splits: int,
                             tt_size: float,
                             rf_clf: RandomForestClassifier,
                             save_dir: str,
-                            save_file_no=None):
+                            save_file_no: Optional[int] = None) -> None:
         """
         Helper to compute random forest learning curves with cross-validation.
 
         Parameters
         ----------
         x_y_df: pd.DataFrame
             Pandas dataframe holding features and targets.
@@ -361,16 +362,15 @@
         Returns
         -------
         None
 
         """
 
         print('Calculating learning curves...')
-        timer = SimbaTimer()
-        timer.start_timer()
+        timer = SimbaTimer(start=True)
         x_df, y_df = self.split_df_to_x_y(x_y_df, clf_name)
         cv = ShuffleSplit(n_splits=shuffle_splits, test_size=tt_size)
         if platform.system() == "Darwin":
             with parallel_backend("threading", n_jobs=-2):
                 train_sizes, train_scores, test_scores = learning_curve(estimator=rf_clf, X=x_df, y=y_df, cv=cv,
                                                                         scoring='f1', shuffle=False, verbose=0,
                                                                         train_sizes=np.linspace(0.01, 1.0,
@@ -397,15 +397,15 @@
 
     def calc_pr_curve(self,
                       rf_clf: RandomForestClassifier,
                       x_df: pd.DataFrame,
                       y_df: pd.DataFrame,
                       clf_name: str,
                       save_dir: str,
-                      save_file_no=None):
+                      save_file_no: Optional[int] = None)  -> None:
         """
         Helper to compute random forest precision-recall curve.
 
         Parameters
         ----------
         rf_clf: RandomForestClassifier
             sklearn RandomForestClassifier object.
@@ -446,18 +446,18 @@
         pr_df.to_csv(save_file_path, index=False)
         timer.stop_timer()
         print('Precision-recall curve calculation complete (elapsed time: {}s) ...'.format(timer.elapsed_time_str))
 
     def create_example_dt(self,
                           rf_clf: RandomForestClassifier,
                           clf_name: str,
-                          feature_names: list,
-                          class_names: list,
+                          feature_names: List[str],
+                          class_names: List[str],
                           save_dir: str,
-                          save_file_no=None):
+                          save_file_no: Optional[int] = None) -> None:
         """
         Helper to produce visualization of random forest decision tree.
 
         Parameters
         ----------
         rf_clf: RandomForestClassifier
             sklearn RandomForestClassifier object.
@@ -491,17 +491,17 @@
         command = ('dot ' + str(dot_name) + ' -T pdf -o ' + str(file_name) + ' -Gdpi=600')
         call(command, shell=True)
 
     def create_clf_report(self,
                           rf_clf: RandomForestClassifier,
                           x_df: pd.DataFrame,
                           y_df: pd.DataFrame,
-                          class_names: list,
+                          class_names: List[str],
                           save_dir: str,
-                          save_file_no=None):
+                          save_file_no: Optional[int] = None) -> None:
         """
         Helper to create classifier truth table report.
 
         Parameters
         ----------
         rf_clf: RandomForestClassifier
             sklearn RandomForestClassifier object.
@@ -536,15 +536,15 @@
             NotEnoughDataWarning(msg=f'Not enough data to create classification report: {class_names[1]}')
 
     def create_x_importance_log(self,
                                 rf_clf: RandomForestClassifier,
                                 x_names: list,
                                 clf_name: str,
                                 save_dir: str,
-                                save_file_no=None):
+                                save_file_no: Optional[int] = None) -> None:
         """
         Helper to save gini or entropy based feature importance scores.
 
         Parameters
         ----------
         rf_clf: RandomForestClassifier
             sklearn RandomForestClassifier object.
@@ -577,15 +577,15 @@
 
     def create_x_importance_bar_chart(self,
                                       rf_clf: RandomForestClassifier,
                                       x_names: list,
                                       clf_name: str,
                                       save_dir: str,
                                       n_bars: int,
-                                      save_file_no=None):
+                                      save_file_no: Optional[int] = None) -> None:
         """
         Helper to create a bar chart displaying the top N gini or entropy feature importance scores.
 
         Parameters
         ----------
         rf_clf: RandomForestClassifier
             sklearn RandomForestClassifier object.
@@ -621,19 +621,19 @@
                                           clf_name + '_' + str(save_file_no) + '_feature_importance_bar_graph.png')
         else:
             save_file_path = os.path.join(save_dir, clf_name + '_feature_importance_bar_graph.png')
         plt.savefig(save_file_path, dpi=600)
         plt.close('all')
 
     def dviz_classification_visualization(self,
-                                          x_train: np.array,
-                                          y_train: np.array,
+                                          x_train: np.ndarray,
+                                          y_train: np.ndarray,
                                           clf_name: str,
-                                          class_names: list,
-                                          save_dir: str):
+                                          class_names: List[str],
+                                          save_dir: str) -> None:
         """
         Helper to create visualization of example decision tree.
 
         Parameters
         ----------
         x_train: np.array
             Array with training features
@@ -664,21 +664,21 @@
                 msg='Skipping dtreeviz example decision tree visualization. Make sure "graphviz" is installed.')
 
     def create_shap_log(self,
                         ini_file_path: str,
                         rf_clf: RandomForestClassifier,
                         x_df: pd.DataFrame,
                         y_df: pd.DataFrame,
-                        x_names: list,
+                        x_names: List[str],
                         clf_name: str,
                         cnt_present: int,
                         cnt_absent: int,
                         save_path: str,
                         save_it: int = 100,
-                        save_file_no=None):
+                        save_file_no: Optional[int] = None) -> None:
 
         """
         Helper to compute SHAP values.
 
         Parameters
         ----------
         ini_file_path: str
@@ -757,15 +757,15 @@
         _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                               classifier_name=clf_name,
                                               shap_df=out_df_shap,
                                               shap_baseline_value=int(expected_value * 100),
                                               save_path=save_path)
 
     def print_machine_model_information(self,
-                                        model_dict: dict):
+                                        model_dict: dict) -> None:
         """
         Helper to print model information in tabular form.
 
         Parameters
         ----------
         model_dict: dict
             Python dictionary holding model meta data in SimBA meta-config format.
@@ -787,15 +787,15 @@
         table = tabulate(table_view, ["Setting", "value"], tablefmt="grid")
         print(f'{table} {Defaults.STR_SPLIT_DELIMITER.value}TABLE')
 
 
     def create_meta_data_csv_training_one_model(self,
                                                 meta_data_lst: list,
                                                 clf_name: str,
-                                                save_dir: str):
+                                                save_dir: str) -> None:
         """
         Helper to save single model meta data (hyperparameters, sampling settings etc.) into SimBA
         compatible CSV config file.
 
         Parameters
         ----------
         meta_data_lst: list
@@ -815,25 +815,25 @@
         out_df.loc[len(out_df)] = meta_data_lst
         out_df.to_csv(save_path)
 
     def create_meta_data_csv_training_multiple_models(self,
                                                       meta_data,
                                                       clf_name,
                                                       save_dir,
-                                                      save_file_no=None):
+                                                      save_file_no: Optional[int] = None) -> None:
         print('Saving model meta data file...')
         save_path = os.path.join(save_dir, f'{clf_name}_{str(save_file_no)}_meta.csv')
         out_df = pd.DataFrame.from_dict(meta_data, orient='index').T
         out_df.to_csv(save_path)
 
     def save_rf_model(self,
                       rf_clf: RandomForestClassifier,
                       clf_name: str,
                       save_dir: str,
-                      save_file_no=None):
+                      save_file_no: Optional[int] = None) -> None:
         """
         Helper to save pickled classifier object to disk.
 
         Parameters
         ----------
         rf_clf: RandomForestClassifier
             sklearn random forest classifier
@@ -854,15 +854,15 @@
             save_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no) + '.sav')
         else:
             save_path = os.path.join(save_dir, clf_name + '.sav')
         pickle.dump(rf_clf, open(save_path, 'wb'))
 
     def get_model_info(self,
                        config: configparser.ConfigParser,
-                       model_cnt: int):
+                       model_cnt: int) -> dict:
         """
         Helper to read in N SimBA random forest config meta files to python dict memory.
 
         Parameters
         ----------
         config:  configparser.ConfigParser
             Parsed SimBA project_config.ini
@@ -903,15 +903,15 @@
             raise NoDataError(
                 msg=f'There are no models with accurate data specified in the RUN MODELS menu. Speficy the model information to SimBA RUN MODELS menu to use them to analyze videos')
         else:
             return model_dict
 
     def get_all_clf_names(self,
                           config: configparser.ConfigParser,
-                          target_cnt: int):
+                          target_cnt: int) -> List[str]:
         """
         Helper to get all classifier names in a SimBA project.
 
         Parameters
         ----------
         config:  configparser.ConfigParser
             Parsed SimBA project_config.ini
@@ -928,16 +928,16 @@
             entry_name = 'target_name_{}'.format(str(i + 1))
             model_names.append(
                 read_config_entry(config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
         return model_names
 
     def insert_column_headers_for_outlier_correction(self,
                                                      data_df: pd.DataFrame,
-                                                     new_headers: list,
-                                                     filepath: str):
+                                                     new_headers: List[str],
+                                                     filepath: str) -> pd.DataFrame:
         """
         Helper to insert new column headers onto a dataframe.
 
         Parameters
         ----------
         data_df:  pd.DataFrame
             Dataframe where headers to to-bo replaced.
@@ -988,15 +988,15 @@
         except pickle.UnpicklingError:
             raise CorruptedFileError(msg=f'Can not read {file_path} as a classifier file (pickle).')
         return clf
 
     def bout_train_test_splitter(self,
                                  x_df: pd.DataFrame,
                                  y_df: pd.Series,
-                                 test_size: float):
+                                 test_size: float) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray):
         """
         Helper to split train and test based on annotated `bouts`.
 
         Parameters
         ----------
         x_df:  pd.DataFrame
             Features
@@ -1034,15 +1034,17 @@
         y_train = y_df[y_df.index.isin(train_bouts_frames + train_nonbouts_frames)]
         y_test = y_df[y_df.index.isin(test_bouts_frames + test_nonbouts_frames)]
 
         return x_train, x_test, y_train, y_test
 
     def check_sampled_dataset_integrity(self,
                                         x_df: pd.DataFrame,
-                                        y_df: pd.DataFrame):
+                                        y_df: pd.DataFrame) -> None:
+
+        """ Helper to check for non-numerical entries post sampling"""
 
         x_df = x_df.replace([np.inf, -np.inf, None], np.nan)
         x_nan_cnt = x_df.isna().sum()
         x_nan_cnt = x_nan_cnt[x_nan_cnt > 0]
 
         if len(x_nan_cnt) > 0:
             if len(x_nan_cnt) < 10:
@@ -1065,16 +1067,19 @@
                     msg=f'All training annotations for classifier {str(y_df.name)} is labelled as PRESENT. A classifier has be be trained with both behavior PRESENT and ABSENT ANNOTATIONS.')
 
     def partial_dependence_calculator(self,
                                       clf: RandomForestClassifier,
                                       x_df: pd.DataFrame,
                                       clf_name: str,
                                       save_dir: str,
-                                      clf_cnt: int or None = None):
+                                      clf_cnt: int or None = None) -> None:
 
+        """
+        Helper to compute single feature partial dependencies
+        """
         print(f'Calculating partial dependencies for {len(x_df.columns)} features...')
         clf.verbose = 0
         check_if_dir_exists(save_dir)
         if clf_cnt:
             save_dir = os.path.join(save_dir, f'partial_dependencies_{clf_name}_{clf_cnt}')
         else:
             save_dir = os.path.join(save_dir, f'partial_dependencies_{clf_name}')
@@ -1086,46 +1091,48 @@
             df.to_csv(save_path)
             print(f'Partial dependencies for {feature_name} complete...')
 
     def clf_predict_proba(self,
                           clf: RandomForestClassifier,
                           x_df: pd.DataFrame,
                           model_name: str or None = None,
-                          data_path: str or None = None):
+                          data_path: str or None = None) -> np.ndarray:
+        """ Helper to run clf inference """
         if len(x_df.columns) != clf.n_features_:
             if model_name and data_path:
                 raise FeatureNumberMismatchError(f'Mismatch in the number of features in input file {data_path}, and what is expected by the model {model_name}. The model expects {str(clf.n_features_)} features. The data contains {len(x_df.columns)} features.')
             else:
                 raise FeatureNumberMismatchError(f'The model expects {str(clf.n_features_)} features. The data contains {len(x_df.columns)} features.')
         p_vals = clf.predict_proba(x_df)
         if p_vals.shape[1] != 2:
             raise ClassifierInferenceError(
                 msg='The classifier {model_name} has not been created properly. See The SimBA GitHub FAQ page or Gitter for more information and suggested fixes.')
         return p_vals[:, 1]
 
     def clf_fit(self,
                 clf: RandomForestClassifier,
                 x_df: pd.DataFrame,
-                y_df: pd.DataFrame):
+                y_df: pd.DataFrame) -> np.ndarray:
+
+        """Helper to fit clf model"""
         nan_features = x_df[~x_df.applymap(np.isreal).all(1)]
         nan_target = y_df.loc[pd.to_numeric(y_df).isna()]
         if len(nan_features) > 0:
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_features)} frame(s) in your project_folder/csv/targets_inserted directory contains FEATURES with non-numerical values')
         if len(nan_target) > 0:
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_target)} frame(s) in your project_folder/csv/targets_inserted directory contains ANNOTATIONS with non-numerical values')
         return clf.fit(x_df, y_df)
 
     def _read_data_file_helper(self,
                                file_path: str,
                                file_type: str,
-                               clf_names: list or None=None):
+                               clf_names: Optional[List[str]] = None):
         """ Private function called by ``simba.train_model_functions.read_all_files_in_folder_mp`` """
-
         timer = SimbaTimer(start=True)
         _, vid_name, _ = get_fn_ext(file_path)
         df = read_df(file_path, file_type).dropna(axis=0, how='all').fillna(0)
         df.index = [vid_name] * len(df)
         if clf_names != None:
             for clf_name in clf_names:
                 if not clf_name in df.columns:
@@ -1133,15 +1140,15 @@
         timer.stop_timer()
         print(f'Reading complete {vid_name} (elapsed time: {timer.elapsed_time_str}s)...')
         return df
 
     def read_all_files_in_folder_mp(self,
                                     file_paths: list,
                                     file_type: str,
-                                    classifier_names: list or None = None):
+                                    classifier_names: Optional[List[str]] = None):
         """
 
         Multiprocessing helper function to read in all data files in a folder to a single
         pd.DataFrame for downstream ML. Defaults to ceil(CPU COUNT / 2) cores. Asserts that all classifiers
         have annotation fields present in each dataframe.
 
         Parameters
@@ -1182,14 +1189,16 @@
                                             file_type=file_type,
                                             classifier_names=classifier_names)
 
     def check_raw_dataset_integrity(self,
                                     df: pd.DataFrame,
                                     logs_path: str) -> pd.DataFrame:
 
+        """ Helper to check column-wise NaNs in raw input data for fitting model"""
+
         nan_cols = df.reset_index(drop=True).replace([np.inf, -np.inf, None], np.nan).columns[df.isna().any()].tolist()
         if len(nan_cols) == 0:
             return df.reset_index(drop=True)
         else:
             save_log_path = os.path.join(logs_path, f'missing_columns_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
             results = {}
             for video in list(df.index.unique()):
@@ -1200,10 +1209,8 @@
                 for video in nan_videos: results[video][nan_col] = False
                 for video in non_nan_video: results[video][nan_col] = True
             results = pd.DataFrame.from_dict(data=results, orient='index')
             results.to_csv(save_log_path)
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_cols)} feature columns exist in some files, but missing in others. The feature files are found in the project_folder/csv/targets_inserted directory. ' \
                     f'SimBA expects all files within the project_folder/csv/targets_inserted directory to have the same number of features: the first 10 ' \
-                    f'column names with mismatches are: {nan_cols[0:9]}. For a log of the files that contain, and not contain, the mis-matched columns, see {save_log_path}')
-
-
+                    f'column names with mismatches are: {nan_cols[0:9]}. For a log of the files that contain, and not contain, the mis-matched columns, see {save_log_path}')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os, glob
+from typing import List
+
+
 from simba.utils.read_write import read_df, get_fn_ext, read_config_entry
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_that_column_exist
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.utils.errors import NoFilesFoundError
 from simba.mixins.config_reader import ConfigReader
 
@@ -41,16 +44,16 @@
     >>> cue_light_clf_analyzer.save_data()
     """
 
     def __init__(self,
                  config_path: str,
                  pre_window: int,
                  post_window: int,
-                 cue_light_names: list,
-                 clf_list: list):
+                 cue_light_names: List[str],
+                 clf_list: List[str]):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.pre_window, self.post_window = pre_window, post_window
         self.cue_light_names = cue_light_names
         self.clf_list = clf_list
         self.project_path = read_config_entry(self.config, 'General settings', 'project_path', data_type='folder_path')
         self.cue_light_data_dir = os.path.join(self.project_path, 'csv', 'cue_lights')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 def get_intensity_scores_in_rois(frm_list: list=None,
                                  video_path: str = None,
                                  rectangles_df: pd.DataFrame = None,
                                  polygon_df: pd.DataFrame = None,
                                  circles_df: pd.DataFrame = None):
+
     cap = cv2.VideoCapture(video_path)
     start, end = frm_list[0], frm_list[-1]
     cap.set(1, start)
     frm_cnt = start
     results_dict = {}
     while frm_cnt <= end:
         _, img = cap.read()
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
+from typing import List
+
 from simba.utils.data import detect_bouts
 
 def find_frames_when_cue_light_on(data_df: pd.DataFrame,
-                                  cue_light_names: list,
+                                  cue_light_names: List[str],
                                   fps: int,
                                   prior_window_frames_cnt: int,
                                   post_window_frames_cnt: int):
     light_on_dict = {}
     for cue_light in cue_light_names:
         light_on_dict[cue_light] = {}
         light_bouts = detect_bouts(data_df=data_df, target_lst=[cue_light], fps=fps)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import itertools, os
 import pandas as pd
 import cv2
+from typing import List
+
+
 from simba.utils.errors import NoSpecifiedOutputError, NoROIDataError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, get_fn_ext, get_video_meta_data
 from simba.utils.printing import stdout_success
 from simba.utils.checks import check_file_exist_and_readable
 
 class CueLightVisualizer(ConfigReader):
@@ -36,15 +39,15 @@
     ----------
     >>> cue_light_visualizer = CueLightVisualizer(config_path='SimBAConfig', cue_light_names=['Cue_light'], video_path='VideoPath', video_setting=True, frame_setting=False)
     >>> cue_light_visualizer.visualize_cue_light_data()
     """
 
     def __init__(self,
                  config_path: str,
-                 cue_light_names: list,
+                 cue_light_names: List[str],
                  video_path: str,
                  frame_setting: bool,
                  video_setting: bool):
 
         ConfigReader.__init__(self, config_path=config_path)
 
         if (not frame_setting) and (not video_setting):
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.59.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 from collections import defaultdict
 import pandas as pd
 import numpy as np
 from statistics import mean
+from typing import List
+
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.printing import stdout_success
 
 
@@ -48,15 +50,15 @@
     >>> cue_light_movement_analyzer.save_results()
     """
 
     def __init__(self,
                  config_path: str,
                  pre_window: int,
                  post_window: int,
-                 cue_light_names: list,
+                 cue_light_names: List[str],
                  threshold: float,
                  roi_setting: bool):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.cue_light_names = cue_light_names
         self.roi_setting = roi_setting
         self.p_threshold = threshold
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/enums.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,14 +163,23 @@
     HEATMAP_SHADING_OPTIONS = ['gouraud', 'flat']
     HEATMAP_BIN_SIZE_OPTIONS = ['10×10', '20×20', '40×40', '80×80', '160×160', '320×320', '640×640', '1280×1280']
     INTERPOLATION_OPTIONS = ['Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic']
     INTERPOLATION_OPTIONS_W_NONE = ['None', 'Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic']
     IMPORT_TYPE_OPTIONS = ['CSV (DLC/DeepPoseKit)','JSON (BENTO)','H5 (multi-animal DLC)', 'SLP (SLEAP)', 'CSV (SLEAP)', 'H5 (SLEAP)', 'TRK (multi-animal APT)', 'MAT (DANNCE 3D)']
     SMOOTHING_OPTIONS = ['Gaussian', 'Savitzky Golay']
     MULTI_DLC_TYPE_IMPORT_OPTION = ['skeleton', 'box','ellipse']
+    FEATURE_SUBSET_OPTIONS = ['Two-point body-part distances (mm)',
+                              'Within-animal three-point body-part angles (degrees)',
+                              'Within-animal three-point convex hull perimeters (mm)',
+                              'Within-animal four-point convex hull perimeters (mm)',
+                              'Entire animal convex hull perimeters (mm)',
+                              'Entire animal convex hull area (mm2)',
+                              'Frame-by-frame body-part movements (mm)',
+                              'Frame-by-frame body-part distances to ROI centers (mm)',
+                              'Frame-by-frame body-parts inside ROIs (Boolean)']
     SMOOTHING_OPTIONS_W_NONE = ['None', 'Gaussian', 'Savitzky Golay']
     VIDEO_FORMAT_OPTIONS = ['mp4', 'avi']
     ALL_VIDEO_FORMAT_OPTIONS = ('.avi', '.mp4', '.mov', '.flv', '.m4v')
     WORKFLOW_FILE_TYPE_OPTIONS = ['csv','parquet']
     TRACKING_TYPE_OPTIONS = ['Classic tracking','Multi tracking', '3D tracking']
     UNSUPERVISED_FEATURE_OPTIONS = ['INCLUDE FEATURE DATA (ORIGINAL)', 'INCLUDE FEATURES (SCALED)', 'EXCLUDE FEATURE DATA']
     TIMEBINS_MEASURMENT_OPTIONS = ['First occurance (s)', 'Event count', 'Total event duration (s)',
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/checks.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
     if return_path is None:
         NoFileFoundWarning(f'SimBA could not find a video file representing {filename} in the project video directory')
     return return_path
 
 
 def find_files_of_filetypes_in_directory(directory: str,
                                          extensions: list,
-                                         raise_warning: bool = True) -> list:
+                                         raise_warning: bool = True) -> List[str]:
     """
     Helper to find all files in a folder with specified extensions
 
     Parameters
     ----------
     directory: str
         Directory holding files
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/data.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.59.2/simba/utils/printing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 __author__ = "Simon Nilsson"
 
-from simba.utils.enums import TagNames, Defaults
 import time
+from typing import Optional
+
+from simba.utils.enums import TagNames, Defaults
+
 
-def stdout_success(msg: str, elapsed_time: str or None=None) -> None:
+def stdout_success(msg: str, elapsed_time: Optional[str] = None) -> None:
     if elapsed_time:
         print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
     else:
         print(f'SIMBA COMPLETE: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
 
-def stdout_warning(msg: str, elapsed_time: str or None=None) -> None:
+def stdout_warning(msg: str, elapsed_time: Optional[str] = None) -> None:
     if elapsed_time:
         print(f'SIMBA WARNING: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
     else:
         print(f'SIMBA WARNING: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
 
-def stdout_trash(msg: str, elapsed_time: str or None=None) -> None:
+def stdout_trash(msg: str, elapsed_time: Optional[str] = None) -> None:
     if elapsed_time:
         print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.TRASH.value}')
     else:
         print(f'SIMBA COMPLETE: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.TRASH.value}')
 
 class SimbaTimer(object):
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_processors/reorganize_keypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from datetime import datetime
 from typing import Optional
 
 from simba.utils.checks import check_if_filepath_list_is_empty, check_if_dir_exists
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Formats
 
-
 class KeypointReorganizer(object):
     """
     Class for re-organizing the order of pose-estimated keypoints in directory containing
     CSV or H5 format files.
 
     Parameters
     ----------
@@ -128,19 +127,13 @@
                 df = pd.read_csv(file_path, header=[0, 1, 2])
                 df_reorganized = pd.DataFrame(df, columns=new_df_ordered_cols)
                 df_reorganized.to_csv(df_save_path)
             print('Saved {}, Video {}/{}.'.format(os.path.basename(file_path), str(file_cnt + 1), str(len(self.files_found))))
         stdout_success(msg=f'{str(len(self.files_found))} new data files with reorganized body-parts saved in {save_directory} directory')
 
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5", pose_tool='SLEAP', file_format='csv')
-
-
-
-
-
-
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5", pose_tool='SLEAP', file_format='SLEAP H5')
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/troubleshooting/B1-MS_US/el_import", pose_tool='maDLC', file_format='h5')
 #keypoint_reorganizer.perform_reorganization(animal_list=['UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'LM', 'LM', 'UM', 'LM', 'UM', 'UM', 'UM', 'UM', 'LM', 'LM'], bp_lst=['Nose', 'Tail_base', 'Tail_base', 'Lateral_right', 'Ear_right', 'Center', 'Nose', 'Ear_left', 'Ear_right', 'Center', 'Tail_end', 'Ear_left', 'Tail_base', 'Lateral_left', 'Tail_end', 'Lateral_right'])
 
 #keypoint_reorganizer = KeypointReorganizer(data_folder="//Users/simon/Desktop/simbapypi_dev/tests/test_data/misc_test_files", pose_tool='DLC', file_format='csv')
 #keypoint_reorganizer.perform_reorganization(bp_lst=['Ear_left_1', 'Ear_right_1', 'Nose_1', 'Center_1', 'Lateral_left_1', 'Lateral_right_1', 'Tail_base_1', 'Ear_left_2', 'Ear_right_2', 'Nose_2', 'Center_2', 'Lateral_left_2', 'Lateral_right_2', 'Tail_base_2'], animal_list=None)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import os
 import cv2
 import numpy as np
 from numba import jit, prange
 import pandas as pd
+from typing import List
+
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df
 
@@ -50,15 +52,15 @@
     def __init__(self,
                  config_path: str,
                  bodypart: str,
                  style_attr: dict,
                  final_img_setting: bool,
                  video_setting: bool,
                  frame_setting: bool,
-                 files_found: list):
+                 files_found: List[str]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
 
         if (not frame_setting) and (not video_setting) and (not final_img_setting):
             raise NoSpecifiedOutputError(msg='Please choose to select either heatmap videos, frames, and/or final image.')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/interactive_probability_grapher.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     Examples
     ----------
     >>> interactive_plotter = InteractiveProbabilityGrapher(config_path=r'MyConfigPath', file_path='MyFeatureFilepath', model_path='MyPickledClassifier.sav')
     >>> interactive_plotter.create_plots()
     """
 
     def __init__(self,
-                 config_path: str=None,
-                 file_path: str=None,
-                 model_path: str=None):
+                 config_path: str,
+                 file_path: str,
+                 model_path: str):
 
         super().__init__(config_path=config_path)
         check_file_exist_and_readable(file_path=file_path)
         check_file_exist_and_readable(file_path=model_path)
         self.file_path, self.model_path = file_path, model_path
         self.click_counter = 0
         _, self.clf_name, _ = get_fn_ext(filepath=self.model_path)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/clf_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import numpy as np
 from copy import deepcopy
 import os
 import cv2
-from typing import Tuple, List
+from typing import Tuple, List, Optional
 
 
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError, NoFilesFoundError
 from simba.utils.warnings import NoDataFoundWarning
 from simba.utils.printing import stdout_success, SimbaTimer
@@ -54,15 +54,15 @@
                  window: int,
                  clf_name: str,
                  clips: bool,
                  text_clr: Tuple[int, int, int],
                  concat_video: bool,
                  video_speed: float,
                  data_paths: List[str],
-                 highlight_clr: None or tuple = None):
+                 highlight_clr: Optional[Tuple[int, int, int]] = None):
 
         super().__init__(config_path=config_path)
         if (not clips) and (not concat_video):
             raise NoSpecifiedOutputError(msg='Please select to create clips and/or a concatenated video')
 
         check_int(name='Time window', value=window)
         self.window, self.clf_name = int(window), clf_name
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/path_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import cv2
 from collections import deque
 from copy import deepcopy
 import numpy as np
 import os
+from typing import List
+
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success, SimbaTimer
@@ -47,15 +49,15 @@
 
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_frame: bool,
-                 files_found: list,
+                 files_found: List[str],
                  input_style_attr: dict,
                  animal_attr: dict,
                  input_clf_attr: dict):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
         self.video_setting, self.frame_setting, self.input_style_attr, self.files_found, self.animal_attr, self.input_clf_attr, self.last_frame = video_setting, frame_setting, input_style_attr, files_found, animal_attr, input_clf_attr, last_frame
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/distance_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     Notes
     -----
     `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     -----
-    >>> distance_plotter = DistancePlotter(config_path=r'MyProjectConfig', frame_setting=False, video_setting=True)
+    >>> distance_plotter = DistancePlotterSingleCore(config_path=r'MyProjectConfig', frame_setting=False, video_setting=True)
     >>> distance_plotter.create_distance_plot()
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 import cv2
 import numpy as np
 import random
+
 from simba.data_processors.directing_other_animals_calculator import DirectingOtherAnimalsAnalyzer
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.warnings import NoDataFoundWarning
 from simba.utils.lookups import get_color_dict
 from simba.utils.read_write import read_df, get_video_meta_data, get_fn_ext
+from simba.utils.data import create_color_palettes
 
 
 class DirectingOtherAnimalsVisualizer(ConfigReader, PlottingMixin):
     """
     Class for visualizing when animals are directing towards body-parts of other animals.
 
     > Note: Requires the pose-estimation data for the left ear, right ears and nose of individual animals.
@@ -57,17 +59,17 @@
         self.direction_analyzer = DirectingOtherAnimalsAnalyzer(config_path=config_path)
         self.direction_analyzer.process_directionality()
         self.direction_analyzer.create_directionality_dfs()
         self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
         self.style_attr, self.pose_colors = style_attr, []
         self.colors = get_color_dict()
         if self.style_attr['Show_pose']:
-            self.pose_colors = self.create_color_lst_of_lst(self.animal_cnt, int(len(self.x_cols) + 1))
+            self.pose_colors = create_color_palettes(self.animal_cnt, int(len(self.x_cols) + 1))
         if self.style_attr['Direction_color'] == 'Random':
-            self.direction_colors = self.create_color_lst_of_lst(1, int(self.animal_cnt**2))
+            self.direction_colors = create_color_palettes(1, int(self.animal_cnt**2))
         else:
             self.direction_colors = [self.colors[self.style_attr['Direction_color']]]
         self.data_dict = self.direction_analyzer.directionality_df_dict
         self.video_path = self.find_video_of_file(video_dir=self.video_dir, filename=self.video_name)
         if not os.path.exists(self.directing_animals_video_output_path): os.makedirs(self.directing_animals_video_output_path)
         print(f'Processing video {self.video_name}...')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.59.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 import platform
 import multiprocessing
 import functools
+from typing import List
+
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, remove_a_folder, concatenate_videos_in_folder, read_df
 
@@ -101,15 +103,15 @@
 
     def __init__(self,
                  config_path: str,
                  final_img_setting: bool,
                  video_setting: bool,
                  frame_setting: bool,
                  bodypart: str,
-                 files_found: list,
+                 files_found: List[str],
                  style_attr: dict,
                  core_cnt: int
                  ):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.59.2/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.59.2/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.59.2/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/kleinberg_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     .. [3] Bordes et al., Automatically annotated motion tracking identifies a distinct social behavioral profile
            following chronic social defeat stress, `bioRxiv`, 2022.
     '''
 
     def __init__(self,
                  config_path: str,
                  classifier_names: List[str],
-                 sigma: int=2,
-                 gamma: float=0.3,
-                 hierarchy: int=1,
-                 hierarchical_search: bool=False):
+                 sigma: int = 2,
+                 gamma: float = 0.3,
+                 hierarchy: int = 1,
+                 hierarchical_search: bool = False):
 
         super().__init__(config_path=config_path)
         self.hierarchical_search, sigma, gamma, hierarchy = hierarchical_search, float(sigma), float(gamma), int(hierarchy)
         check_float(value=sigma, name='sigma', min_value=1.01)
         check_float(value=gamma, name='gamma', min_value=0)
         check_int(value=hierarchy, name='hierarchy')
         self.sigma, self.gamma, self.hierarchy = float(sigma), float(gamma), float(hierarchy)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/data_processors/movement_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,15 @@
             self.movement_dfs[video_name] = pd.DataFrame()
             if self.bp_list:
                 self.data_df = self.data_df[self.bp_list]
                 for animal_cnt, animal_data in self.body_parts_dict.items():
                     animal_df = self.data_df[animal_data['BODY-PART HEADERS']]
                     if self.threshold > 0.00: animal_df = animal_df[animal_df[animal_data['BODY-PART HEADERS'][-1]] >= self.threshold]
                     animal_df = animal_df.iloc[:, 0:2].reset_index(drop=True)
-                    df_shifted = animal_df.shift(1)
-                    df_shifted = df_shifted.combine_first(animal_df).add_suffix('_shifted')
-                    animal_df = pd.concat([animal_df, df_shifted], axis=1)
+                    animal_df = self.create_shifted_df(df=animal_df)
                     bp_time_1 = animal_df[[animal_data['BODY-PART HEADERS'][0], animal_data['BODY-PART HEADERS'][1]]].values.astype(float)
                     bp_time_2 = animal_df[[animal_data['BODY-PART HEADERS'][0] + '_shifted', animal_data['BODY-PART HEADERS'][1] + '_shifted']].values.astype(float)
                     self.movement = pd.Series(self.framewise_euclidean_distance(location_1=bp_time_1, location_2=bp_time_2, px_per_mm=self.px_per_mm))
                     self.movement.loc[0] = 0
                     self.movement_dfs[video_name][f'{animal_data["ANIMAL NAME"]} {animal_data["BODY-PART"]}'] = self.movement
                     distance = round((self.movement.sum() / 10), 4)
                     velocity_lst = []
@@ -138,8 +136,8 @@
 #test.save()
 
 # test = MovementCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini',
 #                           body_parts=['Animal_1 CENTER OF GRAVITY'], #['Simon CENTER OF GRAVITY', 'JJ CENTER OF GRAVITY']
 #                           threshold=0.00)
 # test.run()
 # test.save()
-# print()
+
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.59.2/simba/model/train_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __author__ = "Simon Nilsson"
 
 import os, ast
-import numpy as np
+from typing import Union
+
 from simba.utils.checks import  check_int, check_float, check_if_filepath_list_is_empty
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 from simba.utils.read_write import read_config_entry
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.train_model_mixin import TrainModelMixin
@@ -31,15 +32,15 @@
     >>> model_trainer.train_model()
     >>> model_trainer.save_model()
 
     """
 
 
     def __init__(self,
-                 config_path: str):
+                 config_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path)
         TrainModelMixin.__init__(self)
         self.model_dir_out = os.path.join(read_config_entry(self.config, ConfigKey.SML_SETTINGS.value, ConfigKey.MODEL_DIR.value, data_type=Dtypes.STR.value), 'generated_models')
         if not os.path.exists(self.model_dir_out): os.makedirs(self.model_dir_out)
         self.eval_out_path = os.path.join(self.model_dir_out, 'model_evaluations')
         if not os.path.exists(self.eval_out_path): os.makedirs(self.eval_out_path)
@@ -153,14 +154,15 @@
             else:
                 shuffle_splits, dataset_splits = Dtypes.NAN.value, Dtypes.NAN.value
             if generate_features_importance_bar_graph in Options.PERFORM_FLAGS.value:
                 feature_importance_bars = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.IMPORTANCE_BARS_N.value, Dtypes.INT.value, Dtypes.NAN.value)
                 check_int(name=ConfigKey.IMPORTANCE_BARS_N.value, value=feature_importance_bars, min_value=1)
             else:
                 feature_importance_bars = Dtypes.NAN.value
+            shap_target_present_cnt, shap_target_absent_cnt, shap_save_n = None, None, None
             if generate_shap_scores in Options.PERFORM_FLAGS.value:
                 shap_target_present_cnt = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_PRESENT.value, data_type=Dtypes.INT.value, default_value=0)
                 shap_target_absent_cnt = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_ABSENT.value, data_type=Dtypes.INT.value, default_value=0)
                 shap_save_n = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_SAVE_ITERATION.value, data_type=Dtypes.STR.value, default_value=Dtypes.NONE.value)
                 try:
                     shap_save_n = int(shap_save_n)
                 except ValueError:
@@ -266,8 +268,8 @@
 # test.perform_sampling()
 # test.train_model()
 # test.save_model()
 
 # test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/Lucas/project_folder/project_config.ini')
 # test.perform_sampling()
 # test.train_model()
-# test.save_model()
+# test.save`_model()
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.59.2/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.59.2/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.59.2/simba/model/inference_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 from copy import deepcopy
 
 import warnings
 import os
+from typing import Union
 warnings.filterwarnings('ignore',category=FutureWarning)
 warnings.filterwarnings('ignore',category=DeprecationWarning)
 
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.utils.checks import check_file_exist_and_readable
 from simba.mixins.config_reader import ConfigReader
@@ -34,17 +35,17 @@
     -----
 
     >>> ValidateModelRunClf(config_path=r"MyProjectConfigPath", input_file_path=r"FeatureFilePath", clf_path=r"ClassifierPath")
 
     """
 
     def __init__(self,
-                 config_path: str,
-                 input_file_path: str,
-                 clf_path: str):
+                 config_path: Union[str, os.PathLike],
+                 input_file_path: Union[str, os.PathLike],
+                 clf_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path)
         TrainModelMixin.__init__(self)
         self.save_path = os.path.join(self.project_path, 'csv', 'validation')
         if not os.path.exists(self.save_path): os.makedirs(self.save_path)
 
         check_file_exist_and_readable(input_file_path)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from shapely.geometry import Point, Polygon
 import pandas as pd
 from typing import Dict, Optional
 
 from simba.utils.printing import stdout_success
 from simba.utils.enums import ConfigKey, Dtypes
 from simba.mixins.config_reader import ConfigReader
+from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.errors import NoFilesFoundError, BodypartColumnNotFoundError
 from simba.utils.warnings import NoDataFoundWarning
 from simba.utils.read_write import get_fn_ext, read_df, read_config_entry
 
-class ROIAnalyzer(ConfigReader):
+class ROIAnalyzer(ConfigReader, FeatureExtractionMixin):
     """
 
     Class for analyzing movements, entries, exits, and time-spent-in user-defined ROIs. Results are stored in the
     'project_folder/logs' directory of the SimBA project.
 
     Parameters
     ----------
@@ -47,14 +48,15 @@
     def __init__(self,
                  ini_path: str,
                  data_path: Optional[str] = None,
                  settings: Optional[dict] = None,
                  calculate_distances: bool = False):
 
         ConfigReader.__init__(self, config_path=ini_path)
+        FeatureExtractionMixin.__init__(self)
         self.calculate_distances, self.settings = calculate_distances, settings
         if not os.path.exists(self.detailed_roi_data_dir): os.makedirs(self.detailed_roi_data_dir)
         if data_path != None:
             self.input_folder = os.path.join(self.project_path, 'csv', data_path)
             self.files_found = glob.glob(self.input_folder + '/*.' + self.file_type)
             if len(self.files_found) == 0:
                 raise NoFilesFoundError(msg=f'No data files found in {self.input_folder}')
@@ -175,17 +177,15 @@
                     self.movement_dict[video_name] = {}
                     for animal, shape_dicts in self.entries_exit_dict[video_name].items():
                         self.movement_dict[video_name][animal] = {}
                         for shape_name, shape_data in shape_dicts.items():
                             d = pd.DataFrame.from_dict(shape_data, orient='index').T.values.tolist()
                             for entry in d:
                                 df = self.data_df[self.bp_dict[animal][0:2]][self.data_df.index.isin(list(range(entry[0], entry[1]+1)))]
-                                df_shifted = df.shift(1)
-                                df_shifted = df_shifted.combine_first(df).add_prefix('shifted_')
-                                df = pd.concat([df, df_shifted], axis=1)
+                                df = self.create_shifted_df(df=df)
                                 df['Movement'] = (np.sqrt((df.iloc[:, 0] - df.iloc[:, 2]) ** 2 + (df.iloc[:, 1] - df.iloc[:,3]) ** 2)) / pix_per_mm
                                 self.movement_dict[video_name][animal][shape_name] = df['Movement'].sum() / 10
             self.__transpose_dicts_to_dfs()
 
     def compute_framewise_distance_to_roi_centroids(self):
         """
         Method to compute frame-wise distances between ROI centroids and animal body-parts.
@@ -284,29 +284,29 @@
 
 # settings = {'body_parts': {'animal_1_bp': 'Ear_left_1', 'animal_2_bp': 'Ear_left_2', 'animal_3_bp': 'Ear_right_1',}, 'threshold': 0.4}
 # test = ROIAnalyzer(ini_path = r"/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini",
 #                    data_path = "outlier_corrected_movement_location",
 #                    settings=settings,
 #                    calculate_distances=True)
 # test.run()
-# test.save_data()
+# test.save()
 
 
 # settings = {'body_parts': {'Simon': 'Ear_left_1', 'JJ': 'Ear_left_2'}, 'threshold': 0.4}
 # test = ROIAnalyzer(ini_path = r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
 #                    data_path = "outlier_corrected_movement_location",
 #                    settings=settings,
 #                    calculate_distances=True)
 # test.read_roi_dfs()
 # test.analyze_ROIs()
 # test.save_data()
 
 
 # settings = {'body_parts': {'animal_1_bp': 'Ear_left_1', 'animal_2_bp': 'Ear_left_2'}, 'threshold': 0.4}
-# test = ROIAnalyzer(ini_path = r"/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini",
+# test = ROIAnalyzer(ini_path = r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
 #                    data_path = "outlier_corrected_movement_location",
 #                    calculate_distances=True)
-# test.read_roi_dfs()
+# test.run()
 # test.analyze_ROIs()
 # test.save_data()
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.59.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_csv_importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from copy import deepcopy
 
 from simba.data_processors.interpolation_smoothing import Interpolate, Smooth
 from simba.utils.read_write import find_all_videos_in_project
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
 from simba.utils.read_write import write_df, find_video_of_file, get_video_meta_data, get_fn_ext
-from simba.utils.printing import stdout_success
+from simba.utils.printing import stdout_success, SimbaTimer
+from simba.utils.enums import Methods
 
 class SLEAPImporterCSV(ConfigReader, PoseImporterMixin):
 
     """
     Class for importing SLEAP pose-estimation data into SimBA project.
 
     Parameters
@@ -57,20 +58,26 @@
         PoseImporterMixin.__init__(self)
         self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
         self.data_folder, self.id_lst = data_folder, id_lst
         self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
         self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
         self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=['.csv'])
         self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths)
+        if (self.pose_setting is Methods.USER_DEFINED.value):
+            self.__update_config_animal_cnt()
+        if self.animal_cnt > 1:
+            self.check_multi_animal_status()
+            self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.id_lst, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
+            self.update_bp_headers_file()
         print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
 
-
     def run(self):
         for file_cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
             print(f'Analysing {video_name}...')
+            video_timer = SimbaTimer(start=True)
             self.video_name = video_name
             self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
             data_df = pd.read_csv(video_data['DATA'])
             idx = data_df.iloc[:, :2]
             idx['track'] = idx['track'].str.replace(r'[^\d.]+', '').astype(int)
             data_df = data_df.iloc[:, 2:]
             if self.animal_cnt > 1:
@@ -82,27 +89,30 @@
                 idx = list(idx.drop('track', axis=1)['frame_idx'])
                 self.data_df = data_df.set_index([idx]).sort_index()
                 self.data_df.columns = np.arange(len(self.data_df.columns))
                 self.data_df = self.data_df.reindex(range(self.data_df.index[0], self.data_df.index[-1] + 1), fill_value=0)
                 p_df = pd.DataFrame(1.0, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
                 self.data_df = pd.concat([self.data_df, p_df], axis=1).sort_index(axis=1)
                 self.data_df.columns = self.bp_headers
-                self.out_df = deepcopy(self.data_df)
 
+            self.out_df = deepcopy(self.data_df)
             if self.animal_cnt > 1:
                 self.initialize_multi_animal_ui(animal_bp_dict=self.animal_bp_dict,
                                                 video_info=get_video_meta_data(video_data['VIDEO']),
                                                 data_df=self.data_df,
                                                 video_path=video_data['VIDEO'])
                 self.multianimal_identification()
             write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
             if self.interpolation_settings != 'None':
                 self.__run_interpolation()
             if self.smoothing_settings['Method'] != 'None':
                 self.__run_smoothing()
+            video_timer.stop_timer()
+            stdout_success(msg=f'Video {video_name} data imported...', elapsed_time=video_timer.elapsed_time_str)
+        self.timer.stop_timer()
         stdout_success(msg=f'{len(list(self.data_and_videos_lk.keys()))} file(s) imported to the SimBA project (project_folder/csv/input_csv directory)')
 
     def __run_interpolation(self):
         print(f'Interpolating missing values in video {self.video_name} (Method: {self.interpolation_settings})...')
         _ = Interpolate(input_path=self.save_path, config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
 
     def __run_smoothing(self):
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_h5_importer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,51 @@
-#### CODE COPIED FROM @Toshea111 - https://github.com/Toshea111/sleap/blob/develop/docs/notebooks/Convert_HDF5_to_CSV_updated.ipynb
+#### MODIFIED FROM @Toshea111 - https://github.com/Toshea111/sleap/blob/develop/docs/notebooks/Convert_HDF5_to_CSV_updated.ipynb
 import numpy as np
 import pandas as pd
 import h5py
 import os
 from copy import deepcopy
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
 from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
 from simba.utils.errors import BodypartColumnNotFoundError
 from simba.utils.read_write import get_video_meta_data, write_df, find_all_videos_in_project
-from simba.utils.printing import stdout_warning
+from simba.utils.printing import stdout_warning, stdout_success, SimbaTimer
+from simba.utils.enums import Methods
 
 class SLEAPImporterH5(ConfigReader, PoseImporterMixin):
     def __init__(self,
                  config_path: str,
                  data_folder: str,
                  id_lst: list,
                  interpolation_settings: str,
                  smoothing_settings: dict):
 
-        ConfigReader.__init__(self, config_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
         PoseImporterMixin.__init__(self)
         self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
         self.data_folder, self.id_lst = data_folder, id_lst
         self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
         self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
         self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=['.h5'])
         self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths)
+        if (self.pose_setting is Methods.USER_DEFINED.value):
+            self.__update_config_animal_cnt()
+        if self.animal_cnt > 1:
+            self.check_multi_animal_status()
+            self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.id_lst, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
+            self.update_bp_headers_file()
         print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
 
-    def import_sleap(self):
+    def run(self):
         import_log = pd.DataFrame(columns=['VIDEO', 'IMPORT_TIME', 'IMPORT_SOURCE', 'INTERPOLATION_SETTING', 'SMOOTHING_SETTING'])
         for file_cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
             print(f'Importing {video_name}...')
+            video_timer = SimbaTimer(start=True)
             self.video_name = video_name
             try:
                 with h5py.File(video_data['DATA'], "r") as sleap_dict:
                     data = {k: v[()] for k, v in sleap_dict.items()}
                     data["node_names"] = [s.decode() for s in data["node_names"].tolist()]
                     data["track_names"] = [s.decode() for s in data["track_names"].tolist()]
                     data["tracks"] = np.transpose(data["tracks"])
@@ -93,41 +101,58 @@
 
             if self.animal_cnt > 1:
                 self.initialize_multi_animal_ui(animal_bp_dict=self.animal_bp_dict,
                                                 video_info=get_video_meta_data(video_data['VIDEO']),
                                                 data_df=self.data_df,
                                                 video_path=video_data['VIDEO'])
                 self.multianimal_identification()
-                self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
-                write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
-                if self.interpolation_settings != 'None':
-                    self.__run_interpolation()
-                if self.smoothing_settings['Method'] != 'None':
-                    self.__run_smoothing()
+            self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
+            write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
+            if self.interpolation_settings != 'None':
+                self.__run_interpolation()
+            if self.smoothing_settings['Method'] != 'None':
+                self.__run_smoothing()
+            video_timer.stop_timer()
+            stdout_success(msg=f'Video {video_name} data imported...', elapsed_time=video_timer.elapsed_time_str)
+        self.timer.stop_timer()
+        stdout_success(msg='All SLEAP H5 data files imported', elapsed_time=self.timer.elapsed_time_str)
+
 
     def __run_interpolation(self):
         print(f'Interpolating missing values in video {self.video_name} (Method: {self.interpolation_settings})...')
         _ = Interpolate(input_path=self.save_path,config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
 
     def __run_smoothing(self):
         print(f'Performing {self.smoothing_settings["Method"]} smoothing on video {self.video_name}...')
         Smooth(config_path=self.config_path,
                input_path=self.save_path,
                time_window=int(self.smoothing_settings['Parameters']['Time_window']),
                smoothing_method=self.smoothing_settings['Method'],
                initial_import_multi_index=True)
 
 
-test = SLEAPImporterH5(config_path="/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini",
-                   data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5',
-                   id_lst=['Simon', 'Nastacia', 'Ben', 'John', 'JJ'],
-                   interpolation_settings="Body-parts: Nearest",
-                   smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
-test.import_sleap()
-print('All SLEAP imports complete.')
+# test = SLEAPImporterH5(config_path="/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini",
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5',
+#                    id_lst=['Simon', 'Nastacia', 'Ben', 'John', 'JJ'],
+#                    interpolation_settings="Body-parts: Nearest",
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test.run()
+# print('All SLEAP imports complete.')
+
+# test = SLEAPImporterH5(config_path="/Users/simon/Desktop/envs/troubleshooting/SLEAP_2_Animals_16_body_parts/project_folder/project_config.ini",
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/SLEAP_2_Animals_16_body_parts/data/h5',
+#                    id_lst=['Simon', 'Nastacia'],
+#                    interpolation_settings="Body-parts: Nearest",
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test.run()
+# print('All SLEAP imports complete.')
+
+
+
+
 
 
 
 # test = SLEAPImporterH5(config_path="/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini",
 #                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5',
 #                    actor_IDs=['Simon', 'Nastacia', 'Ben', 'John', 'JJ'],
 #                    interpolation_settings='None',
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/madlc_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/madlc_importer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 __author__ = "Simon Nilsson"
 
 import os
-from datetime import datetime
 import pandas as pd
 import numpy as np
+from copy import deepcopy
 
 from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
 from simba.utils.errors import BodypartColumnNotFoundError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import write_df, get_video_meta_data, find_all_videos_in_project
-
-from simba.utils.enums import Formats
+from simba.utils.enums import Formats, Methods
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
+from simba.utils.printing import stdout_success, SimbaTimer
 
 class MADLCImporterH5(ConfigReader, PoseImporterMixin):
     """
     Class for importing multi-animal deeplabcut (maDLC) pose-estimation data (in H5 format)
     into a SimBA project in parquet or CSV format.
 
     Parameters
@@ -65,53 +65,66 @@
 
         self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
         self.data_folder, self.id_lst = data_folder, id_lst
         self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
         self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
         self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=Formats.DLC_FILETYPES.value[file_type])
         self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths, str_splits=Formats.DLC_NETWORK_FILE_NAMES.value)
+        if (self.pose_setting is Methods.USER_DEFINED.value):
+            self.__update_config_animal_cnt()
+        if self.animal_cnt > 1:
+            self.check_multi_animal_status()
+            self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.id_lst, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
+            self.update_bp_headers_file()
         print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
 
     def run(self):
         import_log = pd.DataFrame(columns=['VIDEO', 'IMPORT_TIME', 'IMPORT_SOURCE', 'INTERPOLATION_SETTING', 'SMOOTHING_SETTING'])
         for cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
+            video_timer = SimbaTimer(start=True)
             self.add_spacer, self.frame_no, self.video_data, self.video_name = 2, 1, video_data, video_name
             print(f'Processing {video_name} ...')
             self.data_df = pd.read_hdf(video_data['DATA']).replace([np.inf, -np.inf], np.nan).fillna(0)
             if len(self.data_df.columns) != len(self.bp_headers):
                 raise BodypartColumnNotFoundError(msg=f'The number of body-parts in data file {video_data["DATA"]} do not match the number of body-parts in your SimBA project. '
                       f'The number of of body-parts expected by your SimBA project is {int(len(self.bp_headers) / 3)}. '
                       f'The number of of body-parts contained in data file {video_data["DATA"]} is {int(len(self.data_df.columns) / 3)}. '
                       f'Make sure you have specified the correct number of animals and body-parts in your project.')
             self.data_df.columns = self.bp_headers
-            self.initialize_multi_animal_ui(animal_bp_dict=self.animal_bp_dict,
-                                            video_info=get_video_meta_data(video_data['VIDEO']),
-                                            data_df=self.data_df,
-                                            video_path=video_data['VIDEO'])
-            self.multianimal_identification()
+            self.out_df = deepcopy(self.data_df)
+            if self.animal_cnt > 1:
+                self.initialize_multi_animal_ui(animal_bp_dict=self.animal_bp_dict,
+                                                video_info=get_video_meta_data(video_data['VIDEO']),
+                                                data_df=self.data_df,
+                                                video_path=video_data['VIDEO'])
+                self.multianimal_identification()
             self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
             write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
             if self.interpolation_settings != 'None':
                 self.__run_interpolation()
             if self.smoothing_settings['Method'] != 'None':
                 self.__run_smoothing()
+            video_timer.stop_timer()
+            stdout_success(msg=f'Video {video_name} data imported...', elapsed_time=video_timer.elapsed_time_str)
+        self.timer.stop_timer()
+        stdout_success(msg='All SLEAP H5 data files imported', elapsed_time=self.timer.elapsed_time_str)
 
     def __run_interpolation(self):
         print('Interpolating missing values in video {} (Method: {}) ...'.format(self.video_name, self.interpolation_settings))
         _ = Interpolate(input_path=self.save_path,config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
 
     def __run_smoothing(self):
         print(f'Performing {self.smoothing_settings["Method"]} smoothing on video {self.video_name}...')
         Smooth(config_path=self.config_path,
                input_path=self.save_path,
                time_window=int(self.smoothing_settings['Parameters']['Time_window']),
                smoothing_method=self.smoothing_settings['Method'],
                initial_import_multi_index=True)
 
 
-test = MADLC_Importer(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-                   data_folder=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/h5',
-                   file_type='ellipse',
-                   id_lst=['Simon', 'JJ'],
-                   interpolation_settings='Body-parts: Nearest',
-                   smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
-test.run()
+# test = MADLC_Importer(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/h5',
+#                    file_type='ellipse',
+#                    id_lst=['Simon', 'JJ'],
+#                    interpolation_settings='Body-parts: Nearest',
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/misc/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/sleap_slp_importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import json
 from collections import defaultdict
 import pandas as pd
 
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
+from simba.utils.printing import stdout_success, SimbaTimer
 from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
-
 from simba.utils.read_write import get_video_meta_data, write_df, find_all_videos_in_project
+from simba.utils.enums import Methods
 
 class SLEAPImporterSLP(ConfigReader, PoseImporterMixin):
     """
     Class for importing SLEAP pose-estimation data into a SimBA project.
 
     Parameters
     ----------
@@ -48,22 +49,28 @@
     def __init__(self,
                  project_path: str,
                  data_folder: str,
                  id_lst: list,
                  interpolation_settings: str,
                  smoothing_settings: dict):
 
-        ConfigReader.__init__(self, config_path=project_path)
+        ConfigReader.__init__(self, config_path=project_path, read_video_info=False)
         PoseImporterMixin.__init__(self)
         self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
         self.data_folder, self.id_lst = data_folder, id_lst
         self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
         self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
         self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=['.slp'])
         self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths)
+        if (self.pose_setting is Methods.USER_DEFINED.value):
+            self.__update_config_animal_cnt()
+        if self.animal_cnt > 1:
+            self.check_multi_animal_status()
+            self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.id_lst, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
+            self.update_bp_headers_file()
         print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
 
     def __h5_to_dict(self, name, obj):
         attr = list(obj.attrs.items())
         if name == 'metadata':
             jsonList = (attr[1][1])
             jsonList = jsonList.decode('utf-8')
@@ -94,14 +101,15 @@
                smoothing_method=self.smoothing_settings)
 
     def run(self):
         self.analysis_dict = defaultdict(list)
         self.save_paths_lst = []
         for file_cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
             print(f'Analysing {video_name}...')
+            video_timer = SimbaTimer(start=True)
             self.video_name = video_name
             in_h5 = h5py.File(video_data['DATA'], 'r')
             self.sleap_dict = in_h5.visititems(self.__h5_to_dict)
             self.video_info = get_video_meta_data(video_path=video_data['VIDEO'])
             self.analysis_dict['bp_names'] = []
             self.analysis_dict['ordered_ids'] = []
             self.analysis_dict['ordered_bps'] = []
@@ -139,14 +147,18 @@
                 self.multianimal_identification()
             self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
             write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
             if self.interpolation_settings != 'None':
                 self.__run_interpolation()
             if self.smoothing_settings['Method'] != 'None':
                 self.__run_smoothing()
+            video_timer.stop_timer()
+            stdout_success(msg=f'Video {video_name} data imported...', elapsed_time=video_timer.elapsed_time_str)
+        self.timer.stop_timer()
+        stdout_success(msg='All SLEAP H5 data files imported', elapsed_time=self.timer.elapsed_time_str)
 
     def __create_tracks(self):
         start_frame = 0
         for frame_cnt, frame in enumerate(range(self.analysis_dict['no_frames'])):
             frame_idx = self.analysis_dict['frames'][frame_cnt][2]
             self.frame_dict = {}
             print('Restructuring SLEAP frame: {}/{}, Video: {}'.format(str(frame_cnt), str(self.analysis_dict['no_frames']), str(self.video_name)))
@@ -179,20 +191,20 @@
                 break
 
         self.data_df.fillna(0, inplace=True)
         self.__fill_missing_indexes()
         self.data_df.sort_index(inplace=True)
         self.data_df.columns = self.bp_headers
 
-test = SLEAPImporterSLP(project_path="/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini",
-                   data_folder=r'/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/data',
-                   id_lst=['Simon', 'Nastacia', 'JJ', 'Sam', 'Liana'],
-                   interpolation_settings="Body-parts: Nearest",
-                   smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}}) #Savitzky Golay
-test.run()
+# test = SLEAPImporterSLP(project_path="/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini",
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/data',
+#                    id_lst=['Simon', 'Nastacia', 'JJ', 'Sam', 'Liana'],
+#                    interpolation_settings="Body-parts: Nearest",
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}}) #Savitzky Golay
+# test.run()
 # if test.animals_no > 1:
 #     test.visualize_sleap()
 # test.save_df()
 # test.perform_interpolation()
 # test.perform_smothing()
 # print('All SLEAP imports complete.')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,20 @@
         print(f'Pose-estimation data for video {video_name} imported to SimBA project (elapsed time: {video_timer.elapsed_time_str}s)...')
     return imported_file_paths
 
 def import_single_dlc_tracking_csv_file(config_path: str,
                                         interpolation_setting: str,
                                         smoothing_setting: str,
                                         smoothing_time: int,
-                                        data_dir: str):
+                                        file_path: str):
     timer = SimbaTimer(start=True)
     if (smoothing_setting == Methods.GAUSSIAN.value) or (smoothing_setting == Methods.SAVITZKY_GOLAY.value):
         check_int(name='SMOOTHING TIME WINDOW', value=smoothing_time, min_value=1)
-    check_file_exist_and_readable(file_path=data_dir)
-    imported_file_paths = import_dlc_csv(config_path=config_path, source=data_dir)
+    check_file_exist_and_readable(file_path=file_path)
+    imported_file_paths = import_dlc_csv(config_path=config_path, source=file_path)
     if interpolation_setting != 'None':
         _ = Interpolate(input_path=imported_file_paths[0], config_path=config_path, method=interpolation_setting, initial_import_multi_index=True)
     if (smoothing_setting == Methods.GAUSSIAN.value) or (smoothing_setting == Methods.SAVITZKY_GOLAY.value):
         _ = Smooth(config_path=config_path, input_path=imported_file_paths[0], time_window=smoothing_time, smoothing_method=smoothing_setting, initial_import_multi_index=True)
     timer.stop_timer()
     stdout_success(msg=f'Imported {str(len(imported_file_paths))} pose estimation file(s)', elapsed_time=timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.59.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.59.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/video_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         im = Image.open(file_path)
         save_name = file_path.replace('.' + str(file_type_in), '.' + str(file_type_out))
         im.save(save_name)
         os.remove(file_path)
     stdout_success(msg=f'SIMBA COMPLETE: Files in {directory} directory converted to {file_type_out}')
 
 
-def clahe_enhance_video(file_path: str) -> None:
+def clahe_enhance_video(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to convert a single video file to clahe-enhanced greyscale .avi file. The result is saved with prefix
     ``CLAHE_`` in the same directory as in the input file.
 
     Parameters
     ----------
     file_path: str
@@ -117,18 +117,14 @@
     except Exception as se:
         print(se.args)
         print('CLAHE conversion failed for video {}'.format(file_name))
         cap.release()
         writer.release()
         raise ValueError()
 
-
-
-
-
 def extract_frame_range(file_path: str,
                         start_frame: int,
                         end_frame: int) -> None:
     """
     Helper to extract a user-defined range of frames from a video file and save those in png format. Images
     are saved in a folder with the suffix `_frames` within the same directory as the video file.
 
@@ -160,15 +156,15 @@
         ret, frame = cap.read()
         frm_save_path = os.path.join(save_dir, '{}.{}'.format(str(frm_number), 'png'))
         cv2.imwrite(frm_save_path,frame)
         print('Frame {} saved (Frame {}/{})'.format(str(frm_number), str(frm_cnt), str(len(frame_range))))
     stdout_success(msg=f'{str(len(frame_range))} frames extracted for video {file_name}')
 
 
-def change_single_video_fps(file_path: str,
+def change_single_video_fps(file_path: Union[str, os.PathLike],
                             fps: int) -> None:
     """
     Helper to change the fps of a single video file. Results are stored in the same directory as in the input file with
     the suffix ``_fps_new_fps``.
 
     Parameters
     ----------
@@ -187,15 +183,15 @@
     save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
     if os.path.isfile(save_path):
         FileExistWarning(msg=f'Overwriting existing file at {save_path}')
     command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
     subprocess.call(command, shell=True)
     stdout_success(msg=f'SIMBA COMPLETE: FPS of video {file_name} changed from {str(video_meta_data["fps"])} to {str(fps)} and saved in directory {save_path}')
 
-def change_fps_of_multiple_videos(directory: str,
+def change_fps_of_multiple_videos(directory: Union[str, os.PathLike],
                                   fps: int) -> None:
     """
     Helper to change the fps of video files in a folder. Results are stored in the same directory as in the input files with
     the suffix ``_fps_new_fps``.
 
     Parameters
     ----------
@@ -221,15 +217,15 @@
         print('Converting FPS for {}...'.format(file_name))
         save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
         command = str('ffmpeg -i ') + str(file_path) + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
         subprocess.call(command, shell=True)
         print('Video {} complete...'.format(file_name))
     stdout_success(msg=f'SIMBA COMPLETE: FPS of {str(len(video_paths))} videos changed to { str(fps)}')
 
-def convert_video_powerpoint_compatible_format(file_path: str) -> None:
+def convert_video_powerpoint_compatible_format(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to make a powerpoint compatible copy of a video file. The results is stored in the same directory as the
     input file with the ``_powerpointready`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -244,15 +240,15 @@
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -c:v libx264 -preset slow  -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -codec:a aac ' + '"' + save_name + '"')
     print('Creating video in powerpoint compatible format... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
-def convert_to_mp4(file_path: str) -> None:
+def convert_to_mp4(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to convert a video file to mp4 format. The results is stored in the same directory as the
     input file with the ``_converted.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -267,15 +263,15 @@
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' ' + '"' + save_name + '"')
     print('Converting to mp4... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
-def video_to_greyscale(file_path: str) -> None:
+def video_to_greyscale(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to convert a video file to greyscale mp4 format. The results is stored in the same directory as the
     input file with the ``_grayscale.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -290,15 +286,15 @@
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf format=gray ' + '"' + save_name + '"')
     print('Converting to greyscale... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
-def superimpose_frame_count(file_path: str) -> None:
+def superimpose_frame_count(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to superimpose frame count on a video file. The results is stored in the same directory as the
     input file with the ``_frame_no.mp4`` suffix.
 
     Parameters
     ----------
     file_path: str
@@ -318,15 +314,15 @@
     except subprocess.CalledProcessError as e:
         simba_cw = os.path.dirname(simba.__file__)
         simba_font_path = Path(simba_cw, 'assets', 'UbuntuMono-Regular.ttf')
         command = 'ffmpeg -y -i ' + file_path + ' -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + "-c:a copy " + save_name
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
-def remove_beginning_of_video(file_path: str,
+def remove_beginning_of_video(file_path: Union[str, os.PathLike],
                               time: int) -> None:
     """
     Helper to remove N seconds from the beginning of a video file. The results is stored in the same directory as the
     input file with the ``_shorten.mp4`` suffix.
 
     Parameters
     ----------
@@ -342,15 +338,15 @@
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -ss ') + str(int(time)) + ' -i ' + '"' + str(file_path) + '"' + ' -c:v libx264 -c:a aac ' + '"' + save_name + '"')
     print('Shortening video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
-def clip_video_in_range(file_path: str,
+def clip_video_in_range(file_path: Union[str, os.PathLike],
                         start_time: str,
                         end_time: str) -> None:
     """
     Helper to clip video in a specific range. The results is stored in the same directory as the
     input file with the ``_clipped.mp4`` suffix.
 
     Parameters
@@ -369,15 +365,15 @@
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -ss ' + str(start_time) + ' -to ' + str(end_time) + ' -async 1 ' + '"' + save_name + '"')
     print('Clipping video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
-def downsample_video(file_path: str,
+def downsample_video(file_path: Union[str, os.PathLike],
                      video_height: int,
                      video_width: int) -> None:
     """
     Helper to down-sample a video file. The results is stored in the same directory as the
     input file with the ``_downsampled.mp4`` suffix.
 
     Parameters
@@ -434,15 +430,15 @@
         raise FileExistError('SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = 'ffmpeg -ss ' + str(start_time) + ' -t ' + str(duration) + ' -i ' + '"' + str(file_path) + '"' + ' -filter_complex "[0:v] fps=15,scale=w=' + str(width) + ':h=-1,split [a][b];[a] palettegen=stats_mode=single [p];[b][p] paletteuse=new=1" ' + '"' + str(save_name) + '"'
     print('Creating gif sample... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
-def batch_convert_video_format(directory: str,
+def batch_convert_video_format(directory: Union[str, os.PathLike],
                                input_format: str,
                                output_format: str) -> None:
     """
     Helper to batch convert all videos in a folder of specific format into a different video format. The results are
     stored in the same directory as the input files.
 
     Parameters
@@ -473,15 +469,15 @@
             raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_path))
         command = 'ffmpeg -y -i ' + '"' + file_path + '"' + ' -c:v libx264 -crf 5 -preset medium -c:a libmp3lame -b:a 320k '+'"' + save_path + '"'
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt+1), str(len(video_paths))))
 
     stdout_success(msg=f'SIMBA COMPLETE: {str(len(video_paths))} videos converted in {directory} directory!')
 
-def batch_create_frames(directory: str) -> None:
+def batch_create_frames(directory: Union[str, os.PathLike]) -> None:
     """
     Helper to extract all frames for all videos in a directory. Results are stored within sub-directories in the input
     directory named according to the video files.
 
     Parameters
     ----------
     directory: str
@@ -503,15 +499,15 @@
         print('Processing video {}...'.format(file_name))
         save_dir = os.path.join(dir_name, file_name)
         if not os.path.exists(save_dir): os.makedirs(save_dir)
         video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt + 1), str(len(video_paths))))
     stdout_success(msg=f'{str(len(video_paths))} videos converted into frames in {directory} directory!')
 
-def extract_frames_single_video(file_path: str) -> None:
+def extract_frames_single_video(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to extract all frames for a single. Results are stored within a sub-directory in the same
     directory as the input file.
 
     Parameters
     ----------
     file_path: str
@@ -523,15 +519,15 @@
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     save_dir = os.path.join(dir_name, file_name)
     if not os.path.exists(save_dir): os.makedirs(save_dir)
     print('Processing video {}...'.format(file_name))
     video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
     stdout_success(msg=f'Video {file_name} converted to images in {dir_name} directory!')
 
-def multi_split_video(file_path: str,
+def multi_split_video(file_path: Union[str, os.PathLike],
                       start_times: List[str],
                       end_times: List[str]) -> None:
     """
     Helper divide a video file into multiple video files from specified start and stop times.
 
     Parameters
     ----------
@@ -568,15 +564,15 @@
         if os.path.isfile(save_path):
             raise FileExistError(msg=f'The outfile file already exist: {save_path}.')
         command = (str('ffmpeg -i ') + '"' + file_path + '"' + ' -ss ' + start_time + ' -to ' + end_time + ' -async 1 ' + '"' + save_path + '"')
         print('Processing video clip {}...'.format(str(clip_cnt+1)))
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!')
 
-def crop_single_video(file_path: str) -> None:
+def crop_single_video(file_path: Union[str, os.PathLike]) -> None:
     """
     Helper to crop a single video,
 
     Parameters
     ----------
     file_path: str
         Path to video file.
@@ -600,16 +596,16 @@
     save_path = os.path.join(dir_name, file_name + '_cropped.mp4')
     if os.path.isfile(save_path):
         raise FileExistError(msg='SIMBA ERROR: The out file file already exist: {}.'.format(save_path))
     command = str('ffmpeg -y -i ') + '"' + str(file_path) + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
     subprocess.call(command, shell=True)
     stdout_success(f'Video {file_name} cropped and saved at {save_path}')
 
-def crop_multiple_videos(directory_path: str,
-                         output_path: str) -> None:
+def crop_multiple_videos(directory_path: Union[str, os.PathLike],
+                         output_path: Union[str, os.PathLike]) -> None:
     """
     Helper to crop multiple videos in a folder according to coordinates defines in one video.
 
     Parameters
     ----------
     directory_path: str
         Path to directory holding video files.
@@ -645,15 +641,15 @@
         _ = get_video_meta_data(file_path)
         save_path = os.path.join(output_path, file_name + '_cropped.mp4')
         command = str('ffmpeg -i ') + '"' + file_path + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
         subprocess.call(command, shell=True)
         print('Video {} cropped (Video {}/{})'.format(file_name, str(file_cnt+1), str(len(video_paths))))
     stdout_success(msg=f'{str(len(video_paths))} videos cropped and saved in {directory_path} directory')
 
-def frames_to_movie(directory: str,
+def frames_to_movie(directory: Union[str, os.PathLike],
                     fps: int,
                     bitrate: int,
                     img_format: str) -> None:
 
     """
     Helper to merge frames in a folder to a mp4 video file. Video file is stored in the same directory as the
     input directory sub-folder.
@@ -685,18 +681,18 @@
     save_path = os.path.join(os.path.dirname(directory), os.path.basename(directory) + '.mp4')
     command = str('ffmpeg -y -r ' + str(fps) + ' -f image2 -s ' + str(img_h) + 'x' + str(img_w) + ' -i ' + '"' + ffmpeg_fn + '"' + ' -vcodec libx264 -b ' + str(bitrate) + 'k ' + '"' + str(save_path) + '"')
     print('Creating {} from {} images...'.format(os.path.basename(save_path), str(len(img_paths_in_folder))))
     subprocess.call(command, shell=True)
     stdout_success(msg=f'Video created at {save_path}')
 
 
-def video_concatenator(video_one_path: str,
-                       video_two_path: str,
+def video_concatenator(video_one_path: Union[str, os.PathLike],
+                       video_two_path: Union[str, os.PathLike],
                        resolution: Union[int, str],
-                       horizontal: bool):
+                       horizontal: bool) -> None:
 
 
     for file_path in [video_one_path, video_two_path]:
         check_file_exist_and_readable(file_path=file_path)
         _ = get_video_meta_data(file_path)
     if type(resolution) is int:
         video_meta_data = {}
@@ -719,16 +715,16 @@
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'Videos concatenated and saved at {save_path}')
 
 
 
 class VideoRotator(ConfigReader):
     def __init__(self,
-                 input_path: str,
-                 output_dir: str) -> None:
+                 input_path: Union[str, os.PathLike],
+                 output_dir: Union[str, os.PathLike]) -> None:
 
         _, self.cpu_cnt  = find_core_cnt()
         self.save_dir = output_dir
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         if os.path.isfile(input_path):
             self.video_paths = [input_path]
         else:
@@ -819,16 +815,16 @@
     def run(self):
         self.results = {}
         for video_path in self.video_paths:
             self.__run_interface(video_path)
         self.main_frm.mainloop()
 
 
-def extract_frames_from_all_videos_in_directory(config_path: str,
-                                                directory: str) -> None:
+def extract_frames_from_all_videos_in_directory(config_path: Union[str, os.PathLike],
+                                                directory: Union[str, os.PathLike]) -> None:
 
     """
     Helper to extract all frames from all videos in a directory. The results are saved in the project_folder/frames/input
     directory of the SimBa project
 
     Parameters
     ----------
@@ -866,15 +862,15 @@
         if not os.path.exists(save_path): os.makedirs(save_path)
         else: print(f'Frames for video {video_name} already extracted. SimBA is overwriting prior frames...')
         video_to_frames(video_path, save_path, overwrite=True, every=1, chunk_size=1000)
     timer.stop_timer()
     stdout_success(f'Frames created for {str(len(video_paths))} videos', elapsed_time=timer.elapsed_time_str)
 
 
-def copy_img_folder(config_path: str, source: str) -> None:
+def copy_img_folder(config_path: Union[str, os.PathLike], source: Union[str, os.PathLike]) -> None:
     """
     Copy directory of png files to the SimBA project. The directory is stored in the project_folder/frames/input
     folder of the SimBA project.
     """
     timer = SimbaTimer()
     timer.start_timer()
     if not os.path.isdir(source):
@@ -890,17 +886,14 @@
         raise DirectoryExistError(msg=f'SIMBA ERROR: {destination} already exist in SimBA project.')
     print(f'Importing image files for {input_basename}...')
     shutil.copytree(source, destination)
     timer.stop_timer()
     stdout_success(msg=f'{destination} imported to SimBA project', elapsed_time=timer.elapsed_time_str)
 
 
-
-
-
 # r = VideoRotator(input_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Testing/Together_1_downsampled.mp4',
 #              output_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Blah')
 # r.run()
 
 
 # video_concatenator(video_one_path='/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT_2.mp4',
 #                    video_two_path= '/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT.mp4',
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tkinter import *
 import glob, os, re
 import datetime
 import cv2
 import json
+from typing import Union
 
 from simba.video_processors.batch_process_create_ffmpeg_commands import FFMPEGCommandCreator
 from simba.utils.enums import Options, Keys, Links
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.errors import InvalidInputError, IntegerError, NoFilesFoundError
 from simba.utils.checks import check_file_exist_and_readable
@@ -37,16 +38,16 @@
     >>> batch_preprocessor.create_video_rows()
     >>> batch_preprocessor.create_execute_btn()
     >>> batch_preprocessor.main_frm.mainloop()
 
     """
 
     def __init__(self,
-                 input_dir: str,
-                 output_dir: str):
+                 input_dir: Union[str, os.PathLike],
+                 output_dir: Union[str, os.PathLike]):
 
         PopUpMixin.__init__(self, title='BATCH PRE-PROCESS VIDEOS IN SIMBA', size=(1600, 600))
         self.input_dir, self.output_dir = input_dir, output_dir
         if not os.path.exists(self.output_dir):
             os.makedirs(self.output_dir)
         self.videos_in_dir_dict, self.crop_dict = {}, {}
         self.get_input_files()
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/multi_cropper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
-
 import os, glob
 import cv2
 import subprocess
+from typing import Union
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
+
 from copy import deepcopy
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.checks import  (check_int, check_str, check_if_filepath_list_is_empty)
 from simba.utils.read_write import get_fn_ext
 from simba.utils.enums import Formats
 from simba.utils.errors import CountError, InvalidVideoFileError
 
@@ -35,17 +40,17 @@
     Examples
     ----------
     >>> MultiCropper(file_type='mp4', input_folder='InputDirectory', output_folder='OutputDirectory', crop_cnt=2)
 
     """
 
     def __init__(self,
-                 file_type: str,
-                 input_folder: str,
-                 output_folder: str,
+                 file_type: Literal['mp4', 'avi'],
+                 input_folder: Union[str, os.PathLike],
+                 output_folder: Union[str, os.PathLike],
                  crop_cnt: int):
 
         self.file_type, self.crop_cnt = file_type, crop_cnt
         self.input_folder, self.output_folder = input_folder, output_folder
         self.crop_df = pd.DataFrame(columns=['Video', "height", "width", "topLeftX", "topLeftY"])
         check_int(name='CROP COUNT', value=self.crop_cnt, min_value=2)
         self.crop_cnt = int(crop_cnt)
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/calculate_px_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 __author__ = "Simon Nilsson"
 
 import cv2
 import os
 from copy import deepcopy
 import numpy as np
+from typing import Union
 from simba.utils.read_write import get_fn_ext, get_video_meta_data
 
-
 class CalculatePixelDistanceTool(object):
     def __init__(self,
-                 video_path: str,
-                 known_mm_distance: float):
+                 video_path: Union[str, os.PathLike],
+                 known_mm_distance: float) -> None:
 
         self.video_path = video_path
         self.known_mm_distance = known_mm_distance
         self.video_dir, self.video_name, self.video_ext = get_fn_ext(video_path)
         if not os.access(video_path, os.R_OK):
             print('{} is not readable.'.format(video_path))
             raise FileNotFoundError
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.59.2/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     >>> ffmpeg_executor.apply_grayscale()
     >>> ffmpeg_executor.apply_frame_count()
     >>> ffmpeg_executor.apply_clahe()
     >>> ffmpeg_executor.move_all_processed_files_to_output_folder()
     """
 
     def __init__(self,
-                 json_path: str=None):
+                 json_path: str):
 
         check_file_exist_and_readable(json_path)
         with open(json_path, 'r') as fp:
             self.video_dict = json.load(fp)
         self.input_dir = self.video_dict['meta_data']['in_dir']
         self.out_dir = self.video_dict['meta_data']['out_dir']
         self.temp_dir = os.path.join(self.out_dir, 'temp')
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.59.2/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.59.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/assets/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -492,29 +492,29 @@
 00001eb0: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
 00001ec0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
 00001ed0: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
 00001ee0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
 00001ef0: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
 00001f00: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
 00001f10: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00001f20: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00001f20: 6762 7773 7062 6c6f 6200 0000 c962 706c  gbwspblob....bpl
 00001f30: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
 00001f40: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00001f50: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
 00001f60: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
 00001f70: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
 00001f80: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
 00001f90: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00001fa0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
-00001fb0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
-00001fc0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
-00001fd0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
-00001fe0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00001ff0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
-00002000: 676c 6731 0000 0000 0000 0012 0000 0005  glg1............
+00001fa0: 6964 6562 6172 0808 0908 095f 1018 7b7b  idebar....._..{{
+00001fb0: 3336 2c20 3133 317d 2c20 7b31 3330 322c  36, 131}, {1302,
+00001fc0: 2037 3134 7d7d 0908 1725 313d 4960 6d79   714}}...%1=I`my
+00001fd0: 7a7b 7c7d 7e99 0000 0000 0000 0101 0000  z{|}~...........
+00001fe0: 0000 0000 000f 0000 0000 0000 0000 0000  ................
+00001ff0: 0000 0000 009a 0000 0003 0069 006d 0067  ...........i.m.g
+00002000: 6c67 3153 0000 0000 0000 0012 0000 0005  lg1S............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
 00002020: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
@@ -620,140 +620,140 @@
 000026b0: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
 000026c0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
 000026d0: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
 000026e0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
 000026f0: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
 00002700: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
 00002710: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00002720: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00002720: 6762 7773 7062 6c6f 6200 0000 c962 706c  gbwspblob....bpl
 00002730: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
 00002740: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00002750: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
 00002760: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
 00002770: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
 00002780: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
 00002790: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-000027a0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
-000027b0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
-000027c0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
-000027d0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
-000027e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000027f0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
-00002800: 676c 6731 5363 6f6d 7000 0000 0000 1110  glg1Scomp.......
-00002810: bf00 0000 0300 6900 6d00 676c 7376 4362  ......i.m.glsvCb
-00002820: 6c6f 6200 0002 b062 706c 6973 7430 30da  lob....bplist00.
-00002830: 0102 0304 0506 0708 090a 0b0c 0d1a 4849  ..............HI
-00002840: 484a 0c4c 5f10 1276 6965 774f 7074 696f  HJ.L_..viewOptio
-00002850: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00002860: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002870: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002880: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002890: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-000028a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-000028b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
-000028c0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-000028d0: 6573 5869 636f 6e53 697a 6510 0109 ab0e  esXiconSize.....
-000028e0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
-000028f0: 140c 0c5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
-00002900: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-00002910: 6973 6962 6c65 546e 616d 6511 0137 0909  isibleTname..7..
-00002920: d40f 1011 1218 191a 1a58 7562 6971 7569  .........Xubiqui
-00002930: 7479 1023 0808 d40f 1011 121d 1e1a 0c5c  ty.#...........\
-00002940: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
-00002950: d40f 1011 1222 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
-00002960: 6561 7465 6408 08d4 0f10 1112 2627 1a0c  eated.......&'..
-00002970: 5473 697a 6510 6108 09d4 0f10 1112 2b2c  Tsize.a.......+,
-00002980: 0c0c 546b 696e 6410 7309 09d4 0f10 1112  ..Tkind.s.......
-00002990: 3031 0c1a 556c 6162 656c 1064 0908 d40f  01..Ulabel.d....
-000029a0: 1011 1235 360c 1a57 7665 7273 696f 6e10  ...56..Wversion.
-000029b0: 4b09 08d4 0f10 1112 3a3b 0c1a 5863 6f6d  K.......:;..Xcom
-000029c0: 6d65 6e74 7311 012c 0908 d40f 1011 123f  ments..,.......?
-000029d0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
-000029e0: 6564 10c8 0808 d40f 1011 1244 1e1a 1a59  ed.........D...Y
-000029f0: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
-00002a00: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-00002a10: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
-00002a20: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
-00002a30: 9800 ab00 b400 b600 b700 c300 cc00 d700  ................
-00002a40: dd00 e700 ef00 f400 f700 f800 f901 0201  ................
-00002a50: 0b01 0d01 0e01 0f01 1801 2501 2701 2801  ..........%.'.(.
-00002a60: 2901 3201 3e01 3f01 4001 4901 4e01 5001  ).2.>.?.@.I.N.P.
-00002a70: 5101 5201 5b01 6001 6201 6301 6401 6d01  Q.R.[.`.b.c.d.m.
-00002a80: 7301 7501 7601 7701 8001 8801 8a01 8b01  s.u.v.w.........
-00002a90: 8c01 9501 9e01 a101 a201 a301 ac01 bb01  ................
-00002aa0: bd01 be01 bf01 c801 d201 d301 d401 d501  ................
-00002ab0: de01 e701 ec01 ed00 0000 0000 0002 0100  ................
-00002ac0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
-00002ad0: 0000 0000 0001 f600 0000 0300 6900 6d00  ............i.m.
-00002ae0: 676c 7376 7062 6c6f 6200 0002 9562 706c  glsvpblob....bpl
-00002af0: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-00002b00: 0b0c 0d1c 4748 4749 0c4b 5f10 1276 6965  ....GHGI.K_..vie
-00002b10: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
-00002b20: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-00002b30: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00002b40: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
-00002b50: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
-00002b60: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
-00002b70: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00002b80: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00002b90: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
-00002ba0: 6510 0109 d90e 0f10 1112 1314 1516 1720  e.............. 
-00002bb0: 2529 2d32 373c 4158 636f 6d6d 656e 7473  %)-27<AXcomments
-00002bc0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
-00002bd0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
-00002be0: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
-00002bf0: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
-00002c00: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5776  Tname.........Wv
-00002c10: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00002c20: 656e 6469 6e67 5569 6e64 6578 0811 012c  endingUindex...,
-00002c30: 0910 07d4 1819 1a1b 1c22 1c24 0810 c808  .........".$....
-00002c40: 1008 d418 191a 1b0c 271c 0b09 10b5 08d4  ........'.......
-00002c50: 1819 1a1b 1c27 1c2c 0808 1002 d418 191a  .....'.,........
-00002c60: 1b0c 2f1c 3109 1061 0810 03d4 1819 1a1b  ../.1..a........
-00002c70: 1c34 0c36 0810 6409 1005 d418 191a 1b0c  .4.6..d.........
-00002c80: 390c 3b09 1073 0910 04d4 1819 1a1b 1c3e  9.;..s.........>
-00002c90: 0c40 0810 4b09 1006 d418 191a 1b0c 430c  .@..K.........C.
-00002ca0: 4509 1101 3709 1000 0823 0000 0000 0000  E...7....#......
+000027a0: 6964 6562 6172 0808 0908 095f 1018 7b7b  idebar....._..{{
+000027b0: 3336 2c20 3133 317d 2c20 7b31 3330 322c  36, 131}, {1302,
+000027c0: 2037 3134 7d7d 0908 1725 313d 4960 6d79   714}}...%1=I`my
+000027d0: 7a7b 7c7d 7e99 0000 0000 0000 0101 0000  z{|}~...........
+000027e0: 0000 0000 000f 0000 0000 0000 0000 0000  ................
+000027f0: 0000 0000 009a 0000 0003 0069 006d 0067  ...........i.m.g
+00002800: 6c67 3153 636f 6d70 0000 0000 0011 10bf  lg1Scomp........
+00002810: 0000 0003 0069 006d 0067 6c73 7643 626c  .....i.m.glsvCbl
+00002820: 6f62 0000 02b0 6270 6c69 7374 3030 da01  ob....bplist00..
+00002830: 0203 0405 0607 0809 0a0b 0b0d 1848 4948  .............HIH
+00002840: 4a4b 4c5f 1010 7573 6552 656c 6174 6976  JKL_..useRelativ
+00002850: 6544 6174 6573 5f10 0f73 686f 7749 636f  eDates_..showIco
+00002860: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00002870: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00002880: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+00002890: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+000028a0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+000028b0: 585a 736f 7274 436f 6c75 6d6e 5869 636f  XZsortColumnXico
+000028c0: 6e53 697a 655f 1012 7669 6577 4f70 7469  nSize_..viewOpti
+000028d0: 6f6e 7356 6572 7369 6f6e 0909 ab0e 171c  onsVersion......
+000028e0: 2125 2a2f 3439 3e43 d40f 1011 120b 140b  !%*/49>C........
+000028f0: 1657 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00002900: 6173 6365 6e64 696e 675a 6964 656e 7469  ascendingZidenti
+00002910: 6669 6572 0911 01c7 0954 6e61 6d65 d40f  fier.....Tname..
+00002920: 1011 1218 1918 1b08 1023 0858 7562 6971  .........#.Xubiq
+00002930: 7569 7479 d40f 1011 120b 1e18 2009 10b5  uity........ ...
+00002940: 085c 6461 7465 4d6f 6469 6669 6564 d40f  .\dateModified..
+00002950: 1011 1218 1e18 2408 085b 6461 7465 4372  ......$..[dateCr
+00002960: 6561 7465 64d4 0f10 1112 0b27 1829 0910  eated......'.)..
+00002970: 6108 5473 697a 65d4 0f10 1112 0b2c 0b2e  a.Tsize......,..
+00002980: 0910 7309 546b 696e 64d4 0f10 1112 1831  ..s.Tkind......1
+00002990: 0b33 0810 6409 556c 6162 656c d40f 1011  .3..d.Ulabel....
+000029a0: 1218 360b 3808 104b 0957 7665 7273 696f  ..6.8..K.Wversio
+000029b0: 6ed4 0f10 1112 183b 0b3d 0811 012c 0958  n......;.=...,.X
+000029c0: 636f 6d6d 656e 7473 d40f 1011 1218 4018  comments......@.
+000029d0: 4208 10c8 085e 6461 7465 4c61 7374 4f70  B....^dateLastOp
+000029e0: 656e 6564 d40f 1011 1218 1e18 4608 0859  ened........F..Y
+000029f0: 6461 7465 4164 6465 6408 2300 0000 0000  dateAdded.#.....
+00002a00: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00002a10: 6523 4030 0000 0000 0000 1001 0008 001d  e#@0............
+00002a20: 0030 0042 004a 005e 0070 0079 008b 0096  .0.B.J.^.p.y....
+00002a30: 009f 00b4 00b5 00b6 00c2 00cb 00d3 00d9  ................
+00002a40: 00e3 00ee 00ef 00f2 00f3 00f8 0101 0102  ................
+00002a50: 0104 0105 010e 0117 0118 011a 011b 0128  ...............(
+00002a60: 0131 0132 0133 013f 0148 0149 014b 014c  .1.2.3.?.H.I.K.L
+00002a70: 0151 015a 015b 015d 015e 0163 016c 016d  .Q.Z.[.].^.c.l.m
+00002a80: 016f 0170 0176 017f 0180 0182 0183 018b  .o.p.v..........
+00002a90: 0194 0195 0198 0199 01a2 01ab 01ac 01ae  ................
+00002aa0: 01af 01be 01c7 01c8 01c9 01d3 01d4 01dd  ................
+00002ab0: 01e6 01eb 01f4 0000 0000 0000 0201 0000  ................
+00002ac0: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
+00002ad0: 0000 0000 01f6 0000 0003 0069 006d 0067  ...........i.m.g
+00002ae0: 6c73 7670 626c 6f62 0000 0295 6270 6c69  lsvpblob....bpli
+00002af0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00002b00: 0b0d 1f48 4948 4a4b 265f 1010 7573 6552  ...HIHJK&_..useR
+00002b10: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
+00002b20: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00002b30: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00002b40: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00002b50: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00002b60: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+00002b70: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+00002b80: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
+00002b90: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00002ba0: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+00002bb0: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
+00002bc0: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+00002bd0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+00002be0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+00002bf0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+00002c00: 616d 65d4 1819 1a1b 1c1d 0b1f 5569 6e64  ame.........Uind
+00002c10: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
+00002c20: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
+00002c30: 08d4 1819 1a1b 2122 1f1f 1008 10c8 0808  ......!"........
+00002c40: d418 191a 1b26 271f 0b10 0110 b508 09d4  .....&'.........
+00002c50: 1819 1a1b 2b27 1f1f 1002 0808 d418 191a  ....+'..........
+00002c60: 1b2f 301f 0b10 0310 6108 09d4 1819 1a1b  ./0.....a.......
+00002c70: 3435 0b1f 1005 1064 0908 d418 191a 1b39  45.....d.......9
+00002c80: 3a0b 0b10 0410 7309 09d4 1819 1a1b 3e3f  :.....s.......>?
+00002c90: 0b1f 1006 104b 0908 d418 191a 1b43 440b  .....K.......CD.
+00002ca0: 0b10 0011 01c7 0909 0823 0000 0000 0000  .........#......
 00002cb0: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
-00002cc0: 0923 4030 0000 0000 0000 0008 001d 0032  .#@0...........2
-00002cd0: 0044 004c 0060 0072 007b 008d 0098 00ab  .D.L.`.r.{......
-00002ce0: 00b4 00b6 00b7 00ca 00d3 00e2 00ef 00fb  ................
-00002cf0: 0100 0106 010b 0113 0118 0121 0129 012f  ...........!.)./
-00002d00: 0139 013f 0140 0143 0144 0146 014f 0150  .9.?.@.C.D.F.O.P
-00002d10: 0152 0153 0155 015e 015f 0161 0162 016b  .R.S.U.^._.a.b.k
-00002d20: 016c 016d 016f 0178 0179 017b 017c 017e  .l.m.o.x.y.{.|.~
-00002d30: 0187 0188 018a 018b 018d 0196 0197 0199  ................
-00002d40: 019a 019c 01a5 01a6 01a8 01a9 01ab 01b4  ................
-00002d50: 01b5 01b8 01b9 01bb 01bc 01c5 01ce 01d3  ................
-00002d60: 01d4 0000 0000 0000 0201 0000 0000 0000  ................
-00002d70: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
-00002d80: 01dd 0000 0003 0069 006d 0067 6d6f 4444  .......i.m.gmoDD
-00002d90: 626c 6f62 0000 0008 69d3 090c 67f2 c441  blob....i...g..A
-00002da0: 0000 0003 0069 006d 0067 6d6f 6444 626c  .....i.m.gmodDbl
-00002db0: 6f62 0000 0008 69d3 090c 67f2 c441 0000  ob....i...g..A..
-00002dc0: 0003 0069 006d 0067 7068 3153 636f 6d70  ...i.m.gph1Scomp
-00002dd0: 0000 0000 0011 3000 0000 0003 0069 006d  ......0......i.m
-00002de0: 0067 7653 726e 6c6f 6e67 0000 0001 0000  .gvSrnlong......
-00002df0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
-00002e00: 6277 7370 626c 6f62 0000 00c8 6270 6c69  bwspblob....bpli
-00002e10: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
-00002e20: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00002e30: 725b 5368 6f77 5061 7468 6261 725b 5368  r[ShowPathbar[Sh
-00002e40: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00002e50: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-00002e60: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-00002e70: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00002e80: 6465 6261 7208 0809 0809 5f10 177b 7b32  debar....._..{{2
-00002e90: 302c 2039 307d 2c20 7b31 3031 352c 2037  0, 90}, {1015, 7
-00002ea0: 3637 7d7d 0908 1725 313d 4960 6d79 7a7b  67}}...%1=I`myz{
-00002eb0: 7c7d 7e98 0000 0000 0000 0101 0000 0000  |}~.............
-00002ec0: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-00002ed0: 0000 0099 0000 0007 006c 006f 006f 006b  .........l.o.o.k
-00002ee0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-00002ef0: 0000 0004 b1fb 0000 0000 0000 0000 0000  ................
+00002cc0: 2340 3000 0000 0000 0000 0800 1d00 3000  #@0...........0.
+00002cd0: 4200 4a00 5e00 7000 7900 8b00 9600 9f00  B.J.^.p.y.......
+00002ce0: b400 b500 b600 c900 d200 e100 ee00 fa00  ................
+00002cf0: ff01 0501 0a01 1201 1701 2001 2601 2c01  .......... .&.,.
+00002d00: 3601 3e01 4001 4301 4401 4501 4e01 5001  6.>.@.C.D.E.N.P.
+00002d10: 5201 5301 5401 5d01 5f01 6101 6201 6301  R.S.T.]._.a.b.c.
+00002d20: 6c01 6e01 6f01 7001 7901 7b01 7d01 7e01  l.n.o.p.y.{.}.~.
+00002d30: 7f01 8801 8a01 8c01 8d01 8e01 9701 9901  ................
+00002d40: 9b01 9c01 9d01 a601 a801 aa01 ab01 ac01  ................
+00002d50: b501 b701 ba01 bb01 bc01 bd01 c601 cf01  ................
+00002d60: d400 0000 0000 0002 0100 0000 0000 0000  ................
+00002d70: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
+00002d80: dd00 0000 0300 6900 6d00 676d 6f44 4462  ......i.m.gmoDDb
+00002d90: 6c6f 6200 0000 0869 d309 0c67 f2c4 4100  lob....i...g..A.
+00002da0: 0000 0300 6900 6d00 676d 6f64 4462 6c6f  ....i.m.gmodDblo
+00002db0: 6200 0000 0869 d309 0c67 f2c4 4100 0000  b....i...g..A...
+00002dc0: 0300 6900 6d00 6770 6831 5363 6f6d 7000  ..i.m.gph1Scomp.
+00002dd0: 0000 0000 1130 0000 0000 0300 6900 6d00  .....0......i.m.
+00002de0: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
+00002df0: 0700 6c00 6f00 6f00 6b00 7500 7000 7362  ..l.o.o.k.u.p.sb
+00002e00: 7773 7062 6c6f 6200 0000 c862 706c 6973  wspblob....bplis
+00002e10: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+00002e20: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00002e30: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+00002e40: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00002e50: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+00002e60: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+00002e70: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00002e80: 6562 6172 0808 0908 095f 1017 7b7b 3230  ebar....._..{{20
+00002e90: 2c20 3930 7d2c 207b 3130 3135 2c20 3736  , 90}, {1015, 76
+00002ea0: 377d 7d09 0817 2531 3d49 606d 797a 7b7c  7}}...%1=I`myz{|
+00002eb0: 7d7e 9800 0000 0000 0001 0100 0000 0000  }~..............
+00002ec0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+00002ed0: 0000 9900 0000 0700 6c00 6f00 6f00 6b00  ........l.o.o.k.
+00002ee0: 7500 7000 736c 6731 5363 6f6d 7000 0000  u.p.slg1Scomp...
+00002ef0: 0000 04b4 2c00 0000 0000 0000 0000 0000  ....,...........
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -876,29 +876,29 @@
 000036b0: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
 000036c0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
 000036d0: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
 000036e0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
 000036f0: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
 00003700: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
 00003710: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00003720: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00003720: 6762 7773 7062 6c6f 6200 0000 c962 706c  gbwspblob....bpl
 00003730: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
 00003740: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00003750: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
 00003760: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
 00003770: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
 00003780: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
 00003790: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-000037a0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
-000037b0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
-000037c0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
-000037d0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
-000037e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000037f0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
-00003800: 676c 6731 0000 0006 0000 0000 0000 380b  glg1..........8.
+000037a0: 6964 6562 6172 0808 0908 095f 1018 7b7b  idebar....._..{{
+000037b0: 3336 2c20 3133 317d 2c20 7b31 3330 322c  36, 131}, {1302,
+000037c0: 2037 3134 7d7d 0908 1725 313d 4960 6d79   714}}...%1=I`my
+000037d0: 7a7b 7c7d 7e99 0000 0000 0000 0101 0000  z{|}~...........
+000037e0: 0000 0000 000f 0000 0000 0000 0000 0000  ................
+000037f0: 0000 0000 009a 0000 0003 0069 006d 0067  ...........i.m.g
+00003800: 6c67 3153 0000 0006 0000 0000 0000 380b  lg1S..........8.
 00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
 00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
 00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1004,22 +1004,22 @@
 00003eb0: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
 00003ec0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
 00003ed0: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
 00003ee0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
 00003ef0: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
 00003f00: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
 00003f10: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00003f20: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00003f20: 6762 7773 7062 6c6f 6200 0000 c962 706c  gbwspblob....bpl
 00003f30: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
 00003f40: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00003f50: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
 00003f60: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
 00003f70: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
 00003f80: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
 00003f90: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00003fa0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
-00003fb0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
-00003fc0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
-00003fd0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
-00003fe0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00003ff0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
-00004000: 676c 6731                                glg1
+00003fa0: 6964 6562 6172 0808 0908 095f 1018 7b7b  idebar....._..{{
+00003fb0: 3336 2c20 3133 317d 2c20 7b31 3330 322c  36, 131}, {1302,
+00003fc0: 2037 3134 7d7d 0908 1725 313d 4960 6d79   714}}...%1=I`my
+00003fd0: 7a7b 7c7d 7e99 0000 0000 0000 0101 0000  z{|}~...........
+00003fe0: 0000 0000 000f 0000 0000 0000 0000 0000  ................
+00003ff0: 0000 0000 009a 0000 0003 0069 006d 0067  ...........i.m.g
+00004000: 6c67 3153                                lg1S
```

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.59.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.59.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.59.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.59.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.59.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.59.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.59.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.1
+Version: 1.59.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 simba/assets/icons/concat_icons/vertical.png
 simba/assets/img/.DS_Store
 simba/assets/img/about_me.png
 simba/assets/img/bg.png
 simba/assets/img/bg_2.png
 simba/assets/img/splash.mp4
 simba/assets/img/splash.pptx
+simba/assets/img/~$splash.pptx
 simba/assets/lookups/.DS_Store
 simba/assets/lookups/feature_extraction_headers.csv
 simba/assets/lookups/features.csv
 simba/assets/lookups/model_names.parquet
 simba/assets/lookups/unsupervised_example_x.csv
 simba/assets/shap/.DS_Store
 simba/assets/shap/UbuntuMono-Regular.ttf
@@ -105,14 +106,15 @@
 simba/assets/stl/operant_tray.stl
 simba/assets/stl/operant_walls.stl
 simba/assets/unsupervised/.DS_Store
 simba/assets/unsupervised/features.csv
 simba/assets/unsupervised/model_names.parquet
 simba/blob_storage/.DS_Store
 simba/bounding_box_tools/.DS_Store
+simba/bounding_box_tools/__init__.py
 simba/bounding_box_tools/agg_boundary_stats.py
 simba/bounding_box_tools/boundary_menus.py
 simba/bounding_box_tools/boundary_statistics.py
 simba/bounding_box_tools/find_boundaries.py
 simba/bounding_box_tools/visualize_boundaries.py
 simba/cue_light_tools/.DS_Store
 simba/cue_light_tools/__init__.py
@@ -121,14 +123,15 @@
 simba/cue_light_tools/cue_light_menues.py
 simba/cue_light_tools/cue_light_movement_statistics.py
 simba/cue_light_tools/cue_light_tools.py
 simba/cue_light_tools/cue_light_visualizer.py
 simba/dash_app/SimBA_dash_app.py
 simba/dash_app/dash_app.py
 simba/dash_app/run_dash_tkinter.py
+simba/data_processors/__init__.py
 simba/data_processors/agg_clf_calculator.py
 simba/data_processors/directing_other_animals_calculator.py
 simba/data_processors/fsttc_calculator.py
 simba/data_processors/interpolate_pose.py
 simba/data_processors/interpolation_smoothing.py
 simba/data_processors/kleinberg_calculator.py
 simba/data_processors/movement_calculator.py
@@ -185,19 +188,21 @@
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/feature_extractors/misc/time_stamp_calculator.py
 simba/feature_extractors/misc/video_color.py
 simba/feature_extractors/misc/video_rotator.py
 simba/feature_extractors/misc/video_rotator_mp.py
 simba/labelling/.DS_Store
+simba/labelling/__init__.py
 simba/labelling/extract_labelled_frames.py
 simba/labelling/labelling_advanced_interface.py
 simba/labelling/labelling_interface.py
 simba/labelling/play_annotation_video.py
 simba/mixins/.DS_Store
+simba/mixins/__init__.py
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/plotting_mixin.py
 simba/mixins/pop_up_mixin.py
 simba/mixins/pose_importer_mixin.py
 simba/mixins/train_model_mixin.py
 simba/mixins/unsupervised_mixin.py
@@ -205,14 +210,16 @@
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
 simba/model/grid_search_rf.py
 simba/model/inference_batch.py
 simba/model/inference_validation.py
 simba/model/train_rf.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
@@ -228,14 +235,15 @@
 simba/plotting/.DS_Store
 simba/plotting/Directing_animals_visualizer.py
 simba/plotting/Directing_animals_visualizer_mp.py
 simba/plotting/ROI_feature_visualizer.py
 simba/plotting/ROI_feature_visualizer_mp.py
 simba/plotting/ROI_plotter.py
 simba/plotting/ROI_plotter_mp.py
+simba/plotting/__init__.py
 simba/plotting/clf_validator.py
 simba/plotting/data_plotter.py
 simba/plotting/distance_plotter.py
 simba/plotting/distance_plotter_mp.py
 simba/plotting/ez_lineplot.py
 simba/plotting/frame_mergerer_ffmpeg.py
 simba/plotting/gantt_creator.py
@@ -293,27 +301,26 @@
 simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
 simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
 simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
 simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
 simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
 simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
 simba/pose_importers/.DS_Store
+simba/pose_importers/__init__.py
 simba/pose_importers/dlc_importer_csv.py
-simba/pose_importers/dlc_multi_animal_importer.py
 simba/pose_importers/import_mars.py
+simba/pose_importers/madlc_importer.py
 simba/pose_importers/read_DANNCE_mat.py
-simba/pose_importers/sleap_importer_csv.py
-simba/pose_importers/sleap_importer_h5.py
-simba/pose_importers/sleap_importer_slp.py
+simba/pose_importers/sleap_csv_importer.py
+simba/pose_importers/sleap_h5_importer.py
+simba/pose_importers/sleap_slp_importer.py
 simba/pose_importers/trk_importer.py
+simba/pose_importers/misc/.DS_Store
 simba/pose_importers/misc/apt_trk_importer.py
-simba/pose_importers/misc/madlc_importer.py
-simba/pose_importers/misc/sleap_csv_importer.py
-simba/pose_importers/misc/sleap_h5_importer.py
-simba/pose_importers/misc/sleap_slp_importer.py
+simba/pose_processors/__init__.py
 simba/pose_processors/pose_reset.py
 simba/pose_processors/remove_keypoints.py
 simba/pose_processors/reorganize_keypoint.py
 simba/pose_processors/reverse_pose.py
 simba/roi_tools/.DS_Store
 simba/roi_tools/ROI_analyzer.py
 simba/roi_tools/ROI_clf_calculator.py
@@ -336,20 +343,22 @@
 simba/third_party_label_appenders/deepethogram_importer.py
 simba/third_party_label_appenders/ethovision_import.py
 simba/third_party_label_appenders/observer_importer.py
 simba/third_party_label_appenders/solomon_importer.py
 simba/third_party_label_appenders/third_party_appender.py
 simba/third_party_label_appenders/tools.py
 simba/ui/.DS_Store
+simba/ui/__init__.py
 simba/ui/create_project_ui.py
 simba/ui/machine_model_settings_ui.py
 simba/ui/tkinter_functions.py
 simba/ui/user_defined_pose_creator.py
 simba/ui/video_info_ui.py
 simba/ui/pop_ups/.DS_Store
+simba/ui/pop_ups/__init__.py
 simba/ui/pop_ups/about_simba_pop_up.py
 simba/ui/pop_ups/append_roi_features_animals_pop_up.py
 simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
 simba/ui/pop_ups/archive_files_pop_up.py
 simba/ui/pop_ups/batch_preprocess_pop_up.py
 simba/ui/pop_ups/clf_add_remove_print_pop_up.py
 simba/ui/pop_ups/clf_by_roi_pop_up.py
@@ -386,14 +395,15 @@
 simba/ui/pop_ups/smoothing_interpolation_pop_up.py
 simba/ui/pop_ups/subset_feature_extractor_pop_up.py
 simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
 simba/ui/pop_ups/validation_plot_pop_up.py
 simba/ui/pop_ups/video_processing_pop_up.py
 simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
 simba/unsupervised/.DS_Store
+simba/unsupervised/__init__.py
 simba/unsupervised/bout_aggregator.py
 simba/unsupervised/cluster_statistics.py
 simba/unsupervised/cluster_visualizer.py
 simba/unsupervised/data_extractor.py
 simba/unsupervised/data_map.yaml
 simba/unsupervised/dataset_creator.py
 simba/unsupervised/dbcv_calculator.py
@@ -401,23 +411,25 @@
 simba/unsupervised/grid_search_visualizers.py
 simba/unsupervised/hdbscan_clusterer.py
 simba/unsupervised/pop_up_classes.py
 simba/unsupervised/tsne.py
 simba/unsupervised/ui.py
 simba/unsupervised/umap_embedder.py
 simba/utils/.DS_Store
+simba/utils/__init__.py
 simba/utils/checks.py
 simba/utils/config_creator.py
 simba/utils/data.py
 simba/utils/enums.py
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
 simba/utils/read_write.py
 simba/utils/warnings.py
+simba/utils/cli/__init__.py
 simba/utils/cli/cli_tools.py
 simba/video_processors/.DS_Store
 simba/video_processors/__init__.py
 simba/video_processors/batch_process_create_ffmpeg_commands.py
 simba/video_processors/batch_process_menus.py
 simba/video_processors/calculate_px_dist.py
 simba/video_processors/extract_frames.py
```

### Comparing `Simba-UW-tf-dev-1.59.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.59.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/LICENSE.md` & `Simba-UW-tf-dev-1.59.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/README.md` & `Simba-UW-tf-dev-1.59.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.1/setup.py` & `Simba-UW-tf-dev-1.59.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.59.1",
+    version="1.59.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

