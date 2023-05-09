# Comparing `tmp/deeplake-3.4.0.tar.gz` & `tmp/deeplake-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.4.0.tar", last modified: Tue May  2 17:49:27 2023, max compression
+gzip compressed data, was "deeplake-3.4.1.tar", last modified: Tue May  9 10:10:40 2023, max compression
```

## Comparing `deeplake-3.4.0.tar` & `deeplake-3.4.1.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-05-02 17:42:56.000000 deeplake-3.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-02 17:42:56.000000 deeplake-3.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25285 2023-05-02 17:49:27.270891 deeplake-3.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24578 2023-05-02 17:42:56.000000 deeplake-3.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.240891 deeplake-3.4.0/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94028 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    79381 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5926 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19220 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     6039 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   109338 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   167215 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4242 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13294 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25667 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    49363 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7404 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    10116 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48095 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    28968 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5373 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6781 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4349 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25806 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22441 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     4986 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7196 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     5010 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-02 17:46:40.000000 deeplake-3.4.0/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4477 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34379 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    23730 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31017 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25285 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10849 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-02 17:49:27.270891 deeplake-3.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-02 17:42:56.000000 deeplake-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-05-09 10:06:24.000000 deeplake-3.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-09 10:06:24.000000 deeplake-3.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25285 2023-05-09 10:10:40.115128 deeplake-3.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24578 2023-05-09 10:06:24.000000 deeplake-3.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94061 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    79381 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19170 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   109338 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   169710 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14805 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25667 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49363 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7404 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    10116 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48823 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29082 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6781 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25806 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22441 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4477 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34661 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    24791 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31017 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25285 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10849 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-09 10:10:40.115128 deeplake-3.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-09 10:06:24.000000 deeplake-3.4.1/setup.py
```

### Comparing `deeplake-3.4.0/LICENSE` & `deeplake-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/PKG-INFO` & `deeplake-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.4.0
+Version: 3.4.1
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.4.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.4.1 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
```

### Comparing `deeplake-3.4.0/README.md` & `deeplake-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/__init__.py` & `deeplake-3.4.1/deeplake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.4.0"
+__version__ = "3.4.1"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.4.0/deeplake/api/dataset.py` & `deeplake-3.4.1/deeplake/api/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1052,24 +1052,26 @@
             )
 
         src = convert_pathlib_to_string_if_needed(src)
         dest = convert_pathlib_to_string_if_needed(dest)
 
         verify_dataset_name(dest)
 
-        report_params = {
-            "Overwrite": overwrite,
-            "Num_Workers": num_workers,
-            "Scheduler": scheduler,
-            "Progressbar": progressbar,
-            "Public": public,
-        }
-        if dest.startswith("hub://"):
-            report_params["Dest"] = dest
-        feature_report_path(src, "deepcopy", report_params, token=token)
+        deeplake_reporter.feature_report(
+            feature_name="deepcopy",
+            parameters={
+                "tensors": tensors,
+                "overwrite": overwrite,
+                "num_workers": num_workers,
+                "scheduler": scheduler,
+                "progressbar": progressbar,
+                "public": public,
+                "verbose": verbose,
+            },
+        )
 
         try:
             src_ds = deeplake.load(
                 src, read_only=True, creds=src_creds, token=token, verbose=False
             )
         except DatasetCorruptError as e:
             raise DatasetCorruptError(
```

### Comparing `deeplake-3.4.0/deeplake/api/info.py` & `deeplake-3.4.1/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/link.py` & `deeplake-3.4.1/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/link_tiled.py` & `deeplake-3.4.1/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/read.py` & `deeplake-3.4.1/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_access_method.py` & `deeplake-3.4.1/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_agreement.py` & `deeplake-3.4.1/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_api.py` & `deeplake-3.4.1/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.4.1/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.4.1/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.4.1/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.4.1/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_dataset.py` & `deeplake-3.4.1/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_dicom.py` & `deeplake-3.4.1/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_downsample.py` & `deeplake-3.4.1/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_events.py` & `deeplake-3.4.1/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_grayscale.py` & `deeplake-3.4.1/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_info.py` & `deeplake-3.4.1/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.4.1/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_json.py` & `deeplake-3.4.1/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_link.py` & `deeplake-3.4.1/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.4.1/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_linking.py` & `deeplake-3.4.1/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_mesh.py` & `deeplake-3.4.1/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_meta.py` & `deeplake-3.4.1/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_nifti.py` & `deeplake-3.4.1/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_none.py` & `deeplake-3.4.1/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.4.1/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_pickle.py` & `deeplake-3.4.1/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.4.1/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_polygons.py` & `deeplake-3.4.1/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_pop.py` & `deeplake-3.4.1/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_readonly.py` & `deeplake-3.4.1/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_rechunk.py` & `deeplake-3.4.1/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_reset.py` & `deeplake-3.4.1/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_sample_info.py` & `deeplake-3.4.1/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_text.py` & `deeplake-3.4.1/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_update_samples.py` & `deeplake-3.4.1/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_video.py` & `deeplake-3.4.1/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tests/test_views.py` & `deeplake-3.4.1/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/api/tiled.py` & `deeplake-3.4.1/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/structured/base.py` & `deeplake-3.4.1/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/structured/dataframe.py` & `deeplake-3.4.1/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.4.1/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.4.1/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.4.1/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.4.1/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/base.py` & `deeplake-3.4.1/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.4.1/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.4.1/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.4.1/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.4.1/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.4.1/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.4.1/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/util.py` & `deeplake-3.4.1/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.4.1/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.4.1/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/cli/auth.py` & `deeplake-3.4.1/deeplake/cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     )
                 write_token(token)
                 username = client.get_user_profile()["name"]
             click.echo("Successfully logged in to Activeloop.")
             reporting_config = get_reporting_config()
             if reporting_config.get("username") != username:
                 save_reporting_config(True, username=username)
-                set_username(deeplake_reporter, username)
+                set_username(username)
             break
         except AuthenticationException:
             chances -= 1
             if chances:
                 print("Login failed. Check username and password.")
                 username = ""
                 password = ""
@@ -134,15 +134,15 @@
         click.echo(
             f"Successfully registered and logged in to Activeloop as {username}."
         )
         consent_message = textwrap.dedent(
             """
             Privacy policy:
             We collect basic system information and crash reports so that we can keep
-            improving your experience using Hub to work with your data.
+            improving your experience using Deep Lake to work with your data.
             You can find out more by reading our privacy policy:
                 https://www.activeloop.ai/privacy/
             If you would like to opt out of reporting crashes and system information,
             run the following command:
                 $ activeloop reporting --off
             """
         )
```

### Comparing `deeplake-3.4.0/deeplake/cli/test_cli.py` & `deeplake-3.4.1/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/client/client.py` & `deeplake-3.4.1/deeplake/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 class DeepLakeBackendClient:
     """Communicates with Activeloop Backend"""
 
     def __init__(self, token: Optional[str] = None):
         from deeplake.util.bugout_reporter import (
             save_reporting_config,
             get_reporting_config,
-            deeplake_reporter,
             set_username,
         )
 
         self.version = deeplake.__version__
         self._token_from_env = False
         self.auth_header = None
         self.token = token or self.get_token()
@@ -71,15 +70,15 @@
             remove_token()
             self.token = token or self.get_token()
             self.auth_header = f"Bearer {self.token}"
         if self._token_from_env:
             username = self.get_user_profile()["name"]
             if get_reporting_config().get("username") != username:
                 save_reporting_config(True, username=username)
-                set_username(deeplake_reporter, username)
+                set_username(username)
 
     def get_token(self):
         """Returns a token"""
         self._token_from_env = False
         token = read_token(from_env=False)
         if token is None:
             token = read_token(from_env=True)
```

### Comparing `deeplake-3.4.0/deeplake/client/config.py` & `deeplake-3.4.1/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/client/log.py` & `deeplake-3.4.1/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/client/test_client.py` & `deeplake-3.4.1/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/client/utils.py` & `deeplake-3.4.1/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/compression.py` & `deeplake-3.4.1/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/constants.py` & `deeplake-3.4.1/deeplake/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,10 +180,12 @@
 
 # Rechunk after transform if average chunk size is less than
 # this fraction of min chunk size
 TRANSFORM_RECHUNK_AVG_SIZE_BOUND = 0.1
 
 TIME_INTERVAL_FOR_CUDA_MEMORY_CLEANING = 10 * 60
 
+MAX_TENSORS_IN_SHUFFLE_BUFFER = 32000
+
 # Transform cache sizes
 DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE = 16
 TRANSFORM_CHUNK_CACHE_SIZE = 64 * MB
```

### Comparing `deeplake-3.4.0/deeplake/core/chunk/base_chunk.py` & `deeplake-3.4.1/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.4.1/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.4.1/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.4.1/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.4.1/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.4.1/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.4.1/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/chunk_engine.py` & `deeplake-3.4.1/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/compression.py` & `deeplake-3.4.1/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/compute/process.py` & `deeplake-3.4.1/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/compute/provider.py` & `deeplake-3.4.1/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/compute/ray.py` & `deeplake-3.4.1/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/compute/serial.py` & `deeplake-3.4.1/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/compute/thread.py` & `deeplake-3.4.1/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/dataset/__init__.py` & `deeplake-3.4.1/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/dataset/dataset.py` & `deeplake-3.4.1/deeplake/core/dataset/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         self._initial_autoflush: List[
             bool
         ] = []  # This is a stack to support nested with contexts
         self._indexing_history: List[int] = []
 
         if not self.read_only:
             for temp_tensor in self._temp_tensors:
-                self.delete_tensor(temp_tensor, large_ok=True)
+                self._delete_tensor(temp_tensor, large_ok=True)
             self._temp_tensors = []
 
     def _lock_lost_handler(self):
         """This is called when lock is acquired but lost later on due to slow update."""
         self.read_only = True
         if self.verbose:
             always_warn(
@@ -571,15 +571,14 @@
         else:
             raise InvalidKeyTypeError(item)
         if hasattr(self, "_view_entry"):
             ret._view_entry = self._view_entry
         return ret
 
     @invalid_view_op
-    @deeplake_reporter.record_call
     def create_tensor(
         self,
         name: str,
         htype: str = UNSPECIFIED,
         dtype: Union[str, np.dtype] = UNSPECIFIED,
         sample_compression: str = UNSPECIFIED,
         chunk_compression: str = UNSPECIFIED,
@@ -642,14 +641,61 @@
             TensorAlreadyExistsError: If the tensor already exists and ``exist_ok`` is ``False``.
             TensorGroupAlreadyExistsError: Duplicate tensor groups are not allowed.
             InvalidTensorNameError: If ``name`` is in dataset attributes.
             NotImplementedError: If trying to override ``chunk_compression``.
             TensorMetaInvalidHtype: If invalid htype is specified.
             ValueError: If an illegal argument is specified.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="create_tensor",
+            parameters={
+                "name": name,
+                "htype": htype,
+                "dtype": dtype,
+                "sample_compression": sample_compression,
+                "chunk_compression": chunk_compression,
+            },
+        )
+
+        return self._create_tensor(
+            name,
+            htype,
+            dtype,
+            sample_compression,
+            chunk_compression,
+            hidden,
+            create_sample_info_tensor,
+            create_shape_tensor,
+            create_id_tensor,
+            verify,
+            exist_ok,
+            verbose,
+            downsampling,
+            **kwargs,
+        )
+
+    @invalid_view_op
+    def _create_tensor(
+        self,
+        name: str,
+        htype: str = UNSPECIFIED,
+        dtype: Union[str, np.dtype] = UNSPECIFIED,
+        sample_compression: str = UNSPECIFIED,
+        chunk_compression: str = UNSPECIFIED,
+        hidden: bool = False,
+        create_sample_info_tensor: bool = True,
+        create_shape_tensor: bool = True,
+        create_id_tensor: bool = True,
+        verify: bool = True,
+        exist_ok: bool = False,
+        verbose: bool = True,
+        downsampling: Optional[Tuple[int, int]] = None,
+        **kwargs,
+    ):
         # if not the head node, checkout to an auto branch that is newly created
         auto_checkout(self)
 
         name = filter_name(name, self.group_index)
         key = self.version_state["tensor_names"].get(name)
         is_sequence, is_link, htype = parse_complex_htype(htype)
         if key:
@@ -696,15 +742,15 @@
         ):
             warnings.warn(
                 "Setting `verify` to True. `verify`, `create_shape_tensor` and `create_sample_info_tensor` should all be False if you do not want to verify your link samples."
             )
         kwargs["verify"] = create_shape_tensor or create_sample_info_tensor or verify
 
         if not self._is_root():
-            return self.root.create_tensor(
+            return self.root._create_tensor(
                 name=key,
                 htype=htype,
                 dtype=dtype,
                 sample_compression=sample_compression,
                 chunk_compression=chunk_compression,
                 hidden=hidden,
                 create_sample_info_tensor=create_sample_info_tensor,
@@ -798,15 +844,15 @@
                     downsampling_factor,
                     number_of_layers,
                 )
         return tensor
 
     def _create_sample_shape_tensor(self, tensor: str, htype: str):
         shape_tensor = get_sample_shape_tensor_key(tensor)
-        self.create_tensor(
+        self._create_tensor(
             shape_tensor,
             dtype="int64",
             hidden=True,
             create_id_tensor=False,
             create_sample_info_tensor=False,
             create_shape_tensor=False,
             max_chunk_size=SAMPLE_INFO_TENSOR_MAX_CHUNK_SIZE,
@@ -823,15 +869,15 @@
             extend_f=extend_f,
             update_f=update_f,
             flatten_sequence=True,
         )
 
     def _create_sample_id_tensor(self, tensor: str):
         id_tensor = get_sample_id_tensor_key(tensor)
-        self.create_tensor(
+        self._create_tensor(
             id_tensor,
             hidden=True,
             create_id_tensor=False,
             create_sample_info_tensor=False,
             create_shape_tensor=False,
         )
         self._link_tensors(
@@ -839,15 +885,15 @@
             id_tensor,
             extend_f="extend_id",
             flatten_sequence=False,
         )
 
     def _create_sample_info_tensor(self, tensor: str):
         sample_info_tensor = get_sample_info_tensor_key(tensor)
-        self.create_tensor(
+        self._create_tensor(
             sample_info_tensor,
             htype="json",
             max_chunk_size=SAMPLE_INFO_TENSOR_MAX_CHUNK_SIZE,
             hidden=True,
             create_id_tensor=False,
             create_sample_info_tensor=False,
             create_shape_tensor=False,
@@ -874,15 +920,15 @@
         downsampled_tensor = get_downsampled_tensor_key(tensor, downsampling_factor)
         if number_of_layers == 1:
             downsampling = None
         else:
             downsampling = (downsampling_factor, number_of_layers - 1)
         meta_kwargs = meta_kwargs.copy()
         meta_kwargs.pop("is_link", None)
-        new_tensor = self.create_tensor(
+        new_tensor = self._create_tensor(
             downsampled_tensor,
             htype=htype,
             dtype=dtype,
             sample_compression=sample_compression,
             chunk_compression=chunk_compression,
             hidden=True,
             create_id_tensor=False,
@@ -902,15 +948,14 @@
 
     def _hide_tensor(self, tensor: str):
         self._tensors()[tensor].meta.set_hidden(True)
         self.meta._hide_tensor(tensor)
         self.storage.maybe_flush()
 
     @invalid_view_op
-    @deeplake_reporter.record_call
     def delete_tensor(self, name: str, large_ok: bool = False):
         """Delete a tensor from the dataset.
 
         Examples:
 
             >>> ds.delete_tensor("images/cats")
 
@@ -921,27 +966,37 @@
         Returns:
             None
 
         Raises:
             TensorDoesNotExistError: If tensor of name ``name`` does not exist in the dataset.
             TensorTooLargeToDelete: If the tensor is larger than 1 GB and ``large_ok`` is ``False``.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="delete_tensor",
+            parameters={"name": name, "large_ok": large_ok},
+        )
+
+        return self._delete_tensor(name, large_ok)
+
+    @invalid_view_op
+    def _delete_tensor(self, name: str, large_ok: bool = False):
         auto_checkout(self)
 
         name = filter_name(name, self.group_index)
         key = self.version_state["tensor_names"].get(name)
 
         if not key:
             raise TensorDoesNotExistError(name)
 
         if not tensor_exists(key, self.storage, self.version_state["commit_id"]):
             raise TensorDoesNotExistError(name)
 
         if not self._is_root():
-            return self.root.delete_tensor(name, large_ok)
+            return self.root._delete_tensor(name, large_ok)
 
         if not large_ok:
             chunk_engine = self.version_state["full_tensors"][key].chunk_engine
             size_approx = chunk_engine.num_samples * chunk_engine.min_chunk_size
             if size_approx > deeplake.constants.DELETE_SAFETY_SIZE:
                 raise TensorTooLargeToDelete(name)
 
@@ -966,20 +1021,19 @@
                 get_sample_shape_tensor_key,
             )
         ]:
             t_key = self.meta.tensor_names.get(t_name)
             if t_key and tensor_exists(
                 t_key, self.storage, self.version_state["commit_id"]
             ):
-                self.delete_tensor(t_name, large_ok=True)
+                self._delete_tensor(t_name, large_ok=True)
 
         self.storage.flush()
 
     @invalid_view_op
-    @deeplake_reporter.record_call
     def delete_group(self, name: str, large_ok: bool = False):
         """Delete a tensor group from the dataset.
 
         Examples:
             >>> ds.delete_group("images/dogs")
 
         Args:
@@ -988,23 +1042,33 @@
 
         Returns:
             None
 
         Raises:
             TensorGroupDoesNotExistError: If tensor group of name ``name`` does not exist in the dataset.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="delete_group",
+            parameters={"name": name, "large_ok": large_ok},
+        )
+
+        return self._delete_group(name, large_ok)
+
+    @invalid_view_op
+    def _delete_group(self, name: str, large_ok: bool = False):
         auto_checkout(self)
 
         full_path = filter_name(name, self.group_index)
 
         if full_path not in self._groups:
             raise TensorGroupDoesNotExistError(name)
 
         if not self._is_root():
-            return self.root.delete_group(full_path, large_ok)
+            return self.root._delete_group(full_path, large_ok)
 
         if not large_ok:
             size_approx = self[name].size_approx()
             if size_approx > deeplake.constants.DELETE_SAFETY_SIZE:
                 logger.info(
                     f"Group {name} was too large to delete. Try again with large_ok=True."
                 )
@@ -1027,15 +1091,14 @@
                         self._dataset_diff.tensor_deleted(name)
                 delete_tensor(key, self)
                 self.version_state["full_tensors"].pop(key)
 
         self.storage.maybe_flush()
 
     @invalid_view_op
-    @deeplake_reporter.record_call
     def create_tensor_like(
         self, name: str, source: "Tensor", unlink: bool = False
     ) -> "Tensor":
         """Copies the ``source`` tensor's meta information and creates a new tensor with it. No samples are copied, only the meta/info for the tensor is.
 
         Examples:
             >>> ds.create_tensor_like("cats", ds["images"])
@@ -1045,26 +1108,31 @@
             source (Tensor): Tensor who's meta/info will be copied. May or may not be contained in the same dataset.
             unlink (bool): Whether to unlink linked tensors.
 
         Returns:
             Tensor: New Tensor object.
         """
 
+        deeplake_reporter.feature_report(
+            feature_name="create_tensor_like",
+            parameters={"name": name, "unlink": unlink},
+        )
+
         info = source.info.__getstate__().copy()
         meta = source.meta.__getstate__().copy()
         if unlink:
             meta["is_link"] = False
         del meta["min_shape"]
         del meta["max_shape"]
         del meta["length"]
         del meta["version"]
         del meta["name"]
         del meta["links"]
 
-        destination_tensor = self.create_tensor(
+        destination_tensor = self._create_tensor(
             name,
             verbose=False,
             create_id_tensor=bool(source._sample_id_tensor),
             create_shape_tensor=bool(source._sample_shape_tensor),
             create_sample_info_tensor=bool(source._sample_info_tensor),
             **meta,
         )
@@ -1095,15 +1163,14 @@
             if t_key and tensor_exists(
                 t_key, self.storage, self.version_state["commit_id"]
             ):
                 self._rename_tensor(t_old, t_new)
 
         return tensor
 
-    @deeplake_reporter.record_call
     def rename_tensor(self, name: str, new_name: str) -> "Tensor":
         """Renames tensor with name ``name`` to ``new_name``
 
         Args:
             name (str): Name of tensor to be renamed.
             new_name (str): New name of tensor.
 
@@ -1113,14 +1180,19 @@
         Raises:
             TensorDoesNotExistError: If tensor of name ``name`` does not exist in the dataset.
             TensorAlreadyExistsError: Duplicate tensors are not allowed.
             TensorGroupAlreadyExistsError: Duplicate tensor groups are not allowed.
             InvalidTensorNameError: If ``new_name`` is in dataset attributes.
             RenameError: If ``new_name`` points to a group different from ``name``.
         """
+        deeplake_reporter.feature_report(
+            feature_name="rename_tensor",
+            parameters={"name": name, "new_name": new_name},
+        )
+
         auto_checkout(self)
 
         if name not in self._tensors():
             raise TensorDoesNotExistError(name)
 
         name = filter_name(name, self.group_index)
         new_name = filter_name(new_name, self.group_index)
@@ -1139,29 +1211,33 @@
             raise InvalidTensorNameError(new_name)
 
         tensor = self.root._rename_tensor(name, new_name)
 
         self.storage.maybe_flush()
         return tensor
 
-    @deeplake_reporter.record_call
     def rename_group(self, name: str, new_name: str) -> None:
         """Renames group with name ``name`` to ``new_name``
 
         Args:
             name (str): Name of group to be renamed.
             new_name (str): New name of group.
 
         Raises:
             TensorGroupDoesNotExistError: If tensor group of name ``name`` does not exist in the dataset.
             TensorAlreadyExistsError: Duplicate tensors are not allowed.
             TensorGroupAlreadyExistsError: Duplicate tensor groups are not allowed.
             InvalidTensorGroupNameError: If ``name`` is in dataset attributes.
             RenameError: If ``new_name`` points to a group different from ``name``.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="rename_group",
+            parameters={"name": name, "new_name": new_name},
+        )
         auto_checkout(self)
 
         name = filter_name(name, self.group_index)
         new_name = filter_name(new_name, self.group_index)
 
         if name not in self._groups:
             raise TensorGroupDoesNotExistError(name)
@@ -1364,22 +1440,27 @@
             Exception: If dataset is a filtered view.
             EmptyCommitError: if there are no changes and user does not forced to commit unchanged data.
 
         Note:
             - Commiting from a non-head node in any branch, will lead to an automatic checkout to a new branch.
             - This same behaviour will happen if new samples are added or existing samples are updated from a non-head node.
         """
+
+        # do not store commit message
+        deeplake_reporter.feature_report(
+            feature_name="commit", parameters={"allow_empty": allow_empty}
+        )
+
         if not allow_empty and not self.has_head_changes:
             raise EmptyCommitError(
                 "There are no changes, commit is not done. Try again with allow_empty=True."
             )
 
         return self._commit(message, None, False)
 
-    @deeplake_reporter.record_call
     @spinner
     @invalid_view_op
     @suppress_iteration_warning
     def merge(
         self,
         target_id: str,
         conflict_resolution: Optional[str] = None,
@@ -1405,14 +1486,25 @@
                     - If tensor is renamed on both target and current branch, tensor on target will be registered as a new tensor on current branch.
                     - If tensor is renamed on target and a new tensor of the new name was created on the current branch, they will be merged.
 
         Raises:
             Exception: if dataset is a filtered view.
             ValueError: if the conflict resolution strategy is not one of the None, "ours", or "theirs".
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="merge",
+            parameters={
+                "target_id": target_id,
+                "conflict_resolution": conflict_resolution,
+                "delete_removed_tensors": delete_removed_tensors,
+                "force": force,
+            },
+        )
+
         if self._is_filtered_view:
             raise Exception(
                 "Cannot perform version control operations on a filtered dataset view."
             )
 
         if conflict_resolution not in [None, "ours", "theirs"]:
             raise ValueError(
@@ -1449,16 +1541,14 @@
                 self.__dict__["_vc_info_updated"] = True
             self._lock()
         finally:
             self.storage.autoflush = self._initial_autoflush.pop()
         self._info = None
         self._ds_diff = None
         [f() for f in list(self._commit_hooks.values())]
-        # do not store commit message
-        deeplake_reporter.feature_report(feature_name="commit", parameters={})
         self.maybe_flush()
         return self.commit_id  # type: ignore
 
     @invalid_view_op
     def checkout(
         self, address: str, create: bool = False, reset: bool = False
     ) -> Optional[str]:
@@ -1496,14 +1586,21 @@
             'firstdbf9474d461a19e9333c2fd19b46115348f'
             >>> ds.abc.numpy()
             array([[1, 2, 3]])
 
         Note:
             Checkout from a head node in any branch that contains uncommitted data will lead to an automatic commit before the checkout.
         """
+
+        # do not store address
+        deeplake_reporter.feature_report(
+            feature_name="checkout",
+            parameters={"create": create, "reset": reset},
+        )
+
         try:
             ret = self._checkout(address, create, None, False)
             integrity_check(self)
             return ret
         except (ReadOnlyModeError, CheckoutError) as e:
             raise e from None
         except Exception as e:
@@ -1552,40 +1649,37 @@
             self._set_read_only(read_only, err=True)
             self.storage.autoflush = self._initial_autoflush.pop()
         self._info = None
         self._ds_diff = None
 
         [f() for f in list(self._checkout_hooks.values())]
 
-        # do not store address
-        deeplake_reporter.feature_report(
-            feature_name="checkout", parameters={"Create": str(create)}
-        )
         commit_node = self.version_state["commit_node"]
         if self.verbose:
             warn_node_checkout(commit_node, create)
         if create:
             self.maybe_flush()
         return self.commit_id
 
-    @deeplake_reporter.record_call
     def log(self):
         """Displays the details of all the past commits."""
+
+        deeplake_reporter.feature_report(feature_name="log", parameters={})
+
         commit_node = self.version_state["commit_node"]
         print("---------------\nDeep Lake Version Log\n---------------\n")
         print(f"Current Branch: {self.version_state['branch']}")
         if self.has_head_changes:
             print("** There are uncommitted changes on this branch.")
         print()
         while commit_node:
             if not commit_node.is_head_node:
                 print(f"{commit_node}\n")
             commit_node = commit_node.parent
 
-    @deeplake_reporter.record_call
     def diff(
         self, id_1: Optional[str] = None, id_2: Optional[str] = None, as_dict=False
     ) -> Optional[Dict]:
         """Returns/displays the differences between commits/branches.
 
         For each tensor this contains information about the sample indexes that were added/modified as well as whether the tensor was created.
 
@@ -1613,14 +1707,19 @@
                 - If ``id_1`` and ``id_2`` are None, both the keys will have a single list as their value. This list will contain a dictionary describing changes compared to the previous commit.
                 - If only ``id_1`` is provided, both keys will have a tuple of 2 lists as their value. The lists will contain dictionaries describing commitwise differences between commits. The 2 lists will range from current state and ``id_1`` to most recent common ancestor the commits respectively.
                 - If only ``id_2`` is provided, a ValueError will be raised.
                 - If both ``id_1`` and ``id_2`` are provided, both keys will have a tuple of 2 lists as their value. The lists will contain dictionaries describing commitwise differences between commits. The 2 lists will range from ``id_1`` and ``id_2`` to most recent common ancestor the commits respectively.
 
             ``None`` is returned if ``as_dict`` is ``False``.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="diff", parameters={"as_dict": str(as_dict)}
+        )
+
         version_state, storage = self.version_state, self.storage
         res = get_changes_and_messages(version_state, storage, id_1, id_2)
         if as_dict:
             dataset_changes_1 = res[0]
             dataset_changes_2 = res[1]
             tensor_changes_1 = res[2]
             tensor_changes_2 = res[3]
@@ -1741,15 +1840,14 @@
                     raise e
 
     @read_only.setter
     @invalid_view_op
     def read_only(self, value: bool):
         self._set_read_only(value, True)
 
-    @deeplake_reporter.record_call
     def pytorch(
         self,
         transform: Optional[Callable] = None,
         tensors: Optional[Sequence[str]] = None,
         num_workers: int = 1,
         batch_size: int = 1,
         drop_last: bool = False,
@@ -1806,14 +1904,32 @@
 
         Note:
             Pytorch does not support uint16, uint32, uint64 dtypes. These are implicitly type casted to int32, int64 and int64 respectively.
             This spins up it's own workers to fetch data.
         """
         from deeplake.integrations import dataset_to_pytorch as to_pytorch
 
+        deeplake_reporter.feature_report(
+            feature_name="pytorch",
+            parameters={
+                "tensors": tensors,
+                "num_workers": num_workers,
+                "batch_size": batch_size,
+                "drop_last": drop_last,
+                "pin_memory": pin_memory,
+                "shuffle": shuffle,
+                "buffer_size": buffer_size,
+                "use_local_cache": use_local_cache,
+                "progressbar": progressbar,
+                "return_index": return_index,
+                "pad_tensors": pad_tensors,
+                "decode_method": decode_method,
+            },
+        )
+
         if transform and transform_kwargs:
             transform = partial(transform, **transform_kwargs)
 
         dataloader = to_pytorch(
             self,
             *args,
             transform=transform,
@@ -1833,15 +1949,14 @@
         )
 
         if progressbar:
             dataloader = tqdm(dataloader, desc=self.path, total=len(self) // batch_size)
         dataset_read(self)
         return dataloader
 
-    @deeplake_reporter.record_call
     def dataloader(self):
         """Returns a :class:`~deeplake.enterprise.DeepLakeDataLoader` object. To use this, install deeplake with ``pip install deeplake[enterprise]``.
 
         Returns:
             ~deeplake.enterprise.DeepLakeDataLoader: A :class:`deeplake.enterprise.DeepLakeDataLoader` object.
         
         Examples:
@@ -1891,26 +2006,21 @@
             ...     .pytorch()
             ...
             >>> # loop over the elements
             >>> for i, data in enumerate(train_loader):
             ...     # custom logic on data
             ...     pass
 
-        **Restrictions**
-
-        The new high performance C++ dataloader is part of our Growth and Enterprise Plan .
-
-        - Users of our Community plan can create dataloaders on Activeloop datasets ("hub://activeloop/..." datasets).
-        - To run queries on your own datasets, `upgrade your organization's plan <https://www.activeloop.ai/pricing/>`_.
         """
         from deeplake.enterprise import dataloader
 
+        deeplake_reporter.feature_report(feature_name="dataloader", parameters={})
+
         return dataloader(self)
 
-    @deeplake_reporter.record_call
     def filter(
         self,
         function: Union[Callable, str],
         num_workers: int = 0,
         scheduler: str = "threaded",
         progressbar: bool = True,
         save_result: bool = False,
@@ -1940,14 +2050,24 @@
             Following filters are identical and return dataset view where all the samples have label equals to 2.
 
             >>> dataset.filter(lambda sample: sample.labels.numpy() == 2)
             >>> dataset.filter('labels == 2')
         """
         from deeplake.core.query import filter_dataset, query_dataset
 
+        deeplake_reporter.feature_report(
+            feature_name="filter",
+            parameters={
+                "num_workers": num_workers,
+                "scheduler": scheduler,
+                "progressbar": progressbar,
+                "save_result": save_result,
+            },
+        )
+
         fn = query_dataset if isinstance(function, str) else filter_dataset
         ret = fn(
             self,
             function,
             num_workers=num_workers,
             scheduler=scheduler,
             progressbar=progressbar,
@@ -1981,29 +2101,30 @@
             >>> query_ds = ds.query("select * where labels != 5")
 
             Query from dataset first appeard ``1000`` samples where the ``categories`` is ``car`` and ``1000`` samples where the ``categories`` is ``motorcycle``
 
             >>> ds_train = deeplake.load('hub://activeloop/coco-train')
             >>> query_ds_train = ds_train.query("(select * where contains(categories, 'car') limit 1000) union (select * where contains(categories, 'motorcycle') limit 1000)")
 
-        **Restrictions**
-
-        Querying datasets is part of our Growth and Enterprise Plan .
-
-        - Users of our Community plan can only perform queries on Activeloop datasets ("hub://activeloop/..." datasets).
-        - To run queries on your own datasets, `upgrade your organization's plan <https://www.activeloop.ai/pricing/>`_.
         """
         if runtime is not None and runtime.get("db_engine", False):
             client = DeepLakeBackendClient(token=self._token)
             org_id, ds_name = self.path[6:].split("/")
             indicies = client.remote_query(org_id, ds_name, query_string)
             return self[indicies]
 
         from deeplake.enterprise import query
 
+        deeplake_reporter.feature_report(
+            feature_name="query",
+            parameters={
+                "query_string": query_string,
+            },
+        )
+
         return query(self, query_string)
 
     def sample_by(
         self,
         weights: Union[str, list, tuple],
         replace: Optional[bool] = True,
         size: Optional[int] = None,
@@ -2039,23 +2160,25 @@
             >>> ds = deeplake.load('hub://activeloop/coco-train')
             >>> weights = list()
             >>> for i in range(len(ds)):
             ...     weights.append(i % 5)
             ...
             >>> sampled_ds = ds.sample_by(weights, replace=False)
 
-        **Restrictions**
-
-        Querying datasets is part of our Growth and Enterprise Plan .
-
-        - Users of our Community plan can only use ``sample_by`` on Activeloop datasets ("hub://activeloop/..." datasets).
-        - To use sampling functionality on your own datasets, `upgrade your organization's plan <https://www.activeloop.ai/pricing/>`_.
         """
         from deeplake.enterprise import sample_by
 
+        deeplake_reporter.feature_report(
+            feature_name="sample_by",
+            parameters={
+                "replace": replace,
+                "size": size,
+            },
+        )
+
         return sample_by(self, weights, replace, size)
 
     def _get_total_meta(self):
         """Returns tensor metas all together"""
         return {
             tensor_key: tensor_value.meta
             for tensor_key, tensor_value in self.version_state["full_tensors"].items()
@@ -2113,15 +2236,14 @@
 
     @property
     def _dataset_diff(self):
         if self._ds_diff is None:
             self.__dict__["_ds_diff"] = load_dataset_diff(self)
         return self._ds_diff
 
-    @deeplake_reporter.record_call
     def tensorflow(
         self,
         tensors: Optional[Sequence[str]] = None,
         tobytes: Union[bool, Sequence[str]] = False,
         fetch_chunks: bool = True,
     ):
         """Converts the dataset into a tensorflow compatible format.
@@ -2132,14 +2254,23 @@
             tensors (List, Optional): Optionally provide a list of tensor names in the ordering that your training script expects. For example, if you have a dataset that has "image" and "label" tensors, if ``tensors=["image", "label"]``, your training script should expect each batch will be provided as a tuple of (image, label).
             tobytes (bool): If ``True``, samples will not be decompressed and their raw bytes will be returned instead of numpy arrays. Can also be a list of tensors, in which case those tensors alone will not be decompressed.
             fetch_chunks: See fetch_chunks argument in deeplake.core.tensor.Tensor.numpy()
 
         Returns:
             tf.data.Dataset object that can be used for tensorflow training.
         """
+        deeplake_reporter.feature_report(
+            feature_name="tensorflow",
+            parameters={
+                "tensors": tensors,
+                "tobytes": tobytes,
+                "fetch_chunks": fetch_chunks,
+            },
+        )
+
         dataset_read(self)
         return dataset_to_tensorflow(
             self, tensors=tensors, tobytes=tobytes, fetch_chunks=fetch_chunks
         )
 
     @spinner
     def flush(self):
@@ -2177,49 +2308,54 @@
         chunk_engines = [tensor.chunk_engine for tensor in tensors]
         size = sum(c.num_chunks * c.min_chunk_size for c in chunk_engines)
         for group in self._groups_filtered:
             size += self[group].size_approx()
         return size
 
     @invalid_view_op
-    @deeplake_reporter.record_call
     def rename(self, path: Union[str, pathlib.Path]):
         """Renames the dataset to `path`.
 
         Example:
 
             >>> ds = deeplake.load("hub://username/dataset")
             >>> ds.rename("hub://username/renamed_dataset")
 
         Args:
             path (str, pathlib.Path): New path to the dataset.
 
         Raises:
             RenameError: If ``path`` points to a different directory.
         """
+
+        deeplake_reporter.feature_report(feature_name="rename", parameters={})
+
         path = convert_pathlib_to_string_if_needed(path)
         path = path.rstrip("/")
         if posixpath.split(path)[0] != posixpath.split(self.path)[0]:
             raise RenameError
         self.base_storage.rename(path)
         self.path = path
 
     @invalid_view_op
-    @deeplake_reporter.record_call
     def delete(self, large_ok=False):
         """Deletes the entire dataset from the cache layers (if any) and the underlying storage.
         This is an **IRREVERSIBLE** operation. Data once deleted can not be recovered.
 
         Args:
             large_ok (bool): Delete datasets larger than 1 GB. Defaults to ``False``.
 
         Raises:
             DatasetTooLargeToDelete: If the dataset is larger than 1 GB and ``large_ok`` is ``False``.
         """
 
+        deeplake_reporter.feature_report(
+            feature_name="delete", parameters={"large_ok": large_ok}
+        )
+
         if hasattr(self, "_view_entry"):
             self._view_entry.delete()
             return
         if hasattr(self, "_vds"):
             self._vds.delete(large_ok=large_ok)
             return
         if not large_ok:
@@ -2229,14 +2365,16 @@
 
         self._unlock()
         self.storage.clear()
 
     def summary(self):
         """Prints a summary of the dataset."""
 
+        deeplake_reporter.feature_report(feature_name="summary", parameters={})
+
         pretty_print = summary_dataset(self)
 
         print(self)
         print(pretty_print)
 
     def __str__(self):
         path_str = ""
@@ -2499,15 +2637,14 @@
         while name:
             if name in self.version_state["full_tensors"]:
                 raise TensorAlreadyExistsError(name)
             meta.add_group(name)
             name, _ = posixpath.split(name)
         return self[fullname]
 
-    @deeplake_reporter.record_call
     def create_group(self, name: str, exist_ok=False) -> "Dataset":
         """Creates a tensor group. Intermediate groups in the path are also created.
 
         Args:
             name: The name of the group to create.
             exist_ok: If ``True``, the group is created if it does not exist. If ``False``, an error is raised if the group already exists.
                 Defaults to ``False``.
@@ -2523,24 +2660,30 @@
             >>> ds.create_group("images")
             >>> ds['images'].create_tensor("cats")
 
             >>> ds.create_groups("images/jpg/cats")
             >>> ds["images"].create_tensor("png")
             >>> ds["images/jpg"].create_group("dogs")
         """
-        if not self._is_root():
-            return self.root.create_group(
-                posixpath.join(self.group_index, name), exist_ok=exist_ok
-            )
-        name = filter_name(name)
-        if name in self._groups:
+
+        deeplake_reporter.feature_report(
+            feature_name="create_group",
+            parameters={
+                "name": name,
+                "exist_ok": exist_ok,
+            },
+        )
+
+        full_name = filter_name(name, self.group_index)
+        if full_name in self._groups:
             if not exist_ok:
                 raise TensorGroupAlreadyExistsError(name)
             return self[name]
-        return self._create_group(name)
+
+        return self.root._create_group(full_name)
 
     def rechunk(
         self,
         tensors: Optional[Union[str, List[str]]] = None,
         num_workers: int = 0,
         scheduler: str = "threaded",
         progressbar: bool = True,
@@ -2626,16 +2769,17 @@
         for v in samples.values():
             if len(v) != n:
                 sizes = {k: len(v) for (k, v) in samples.items()}
                 raise ValueError(
                     f"Incoming samples are not of equal lengths. Incoming sample sizes: {sizes}"
                 )
         [f() for f in list(self._update_hooks.values())]
-        for i in range(n):
-            self.append({k: v[i] for k, v in samples.items()}, skip_ok=skip_ok)
+        with self:
+            for i in range(n):
+                self.append({k: v[i] for k, v in samples.items()}, skip_ok=skip_ok)
 
     @invalid_view_op
     def append(
         self, sample: Dict[str, Any], skip_ok: bool = False, append_empty: bool = False
     ):
         """Append samples to mutliple tensors at once. This method expects all tensors being updated to be of the same length.
 
@@ -2950,14 +3094,27 @@
             DatasetViewSavingError: If HEAD node has uncommitted changes.
             TypeError: If ``id`` is not of type ``str``.
 
         Note:
             Specifying ``path`` makes the view external. External views cannot be accessed using the parent dataset's :func:`Dataset.get_view`,
             :func:`Dataset.load_view`, :func:`Dataset.delete_view` methods. They have to be loaded using :func:`deeplake.load`.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="save_view",
+            parameters={
+                "id": id,
+                "optimize": optimize,
+                "tensors": tensors,
+                "num_workers": num_workers,
+                "scheduler": scheduler,
+                "verbose": verbose,
+            },
+        )
+
         if id is not None and not isinstance(id, str):
             raise TypeError(f"id {id} is of type {type(id)}, expected `str`.")
         return self._save_view(
             path,
             id,
             message,
             optimize,
@@ -3205,14 +3362,25 @@
 
         Returns:
             Dataset: The loaded view.
 
         Raises:
             KeyError: if view with given id does not exist.
         """
+        deeplake_reporter.feature_report(
+            feature_name="load_view",
+            parameters={
+                "id": id,
+                "optimize": optimize,
+                "tensors": tensors,
+                "num_workers": num_workers,
+                "scheduler": scheduler,
+            },
+        )
+
         view = self.get_view(id)
         if optimize:
             return view.optimize(
                 tensors=tensors,
                 num_workers=num_workers,
                 scheduler=scheduler,
                 progressbar=progressbar,
@@ -3225,14 +3393,19 @@
         Args:
             id (str): Id of the view to delete.
 
         Raises:
             KeyError: if view with given id does not exist.
         """
 
+        deeplake_reporter.feature_report(
+            feature_name="delete_view",
+            parameters={"id": id},
+        )
+
         try:
             with self._lock_queries_json():
                 qjson = self._read_queries_json()
                 for i, q in enumerate(qjson):
                     if q["id"] == id:
                         qjson.pop(i)
                         self.base_storage.subdir(
@@ -3373,55 +3546,19 @@
         num_workers: int = 0,
         scheduler="threaded",
         progressbar=True,
         public: bool = False,
         unlink: bool = False,
         create_vds_index_tensor: bool = False,
     ):
-        """Copies this dataset or dataset view to `dest`. Version control history is not included.
-
-        Args:
-            dest (str, pathlib.Path): Destination dataset or path to copy to. If a Dataset instance is provided, it is expected to be empty.
-            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
-            tensors (List[str], optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
-            overwrite (bool): If ``True`` and a dataset exists at `destination`, it will be overwritten. Defaults to False.
-            creds (dict, Optional): creds required to create / overwrite datasets at `dest`.
-            token (str, Optional): token used to for fetching credentials to `dest`.
-            num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
-            scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
-                Defaults to 'threaded'.
-            progressbar (bool): Displays a progress bar If ``True`` (default).
-            public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to False.
-            unlink (bool): Whether to copy the data from source for linked tensors. Does not apply for linked video tensors.
-            create_vds_index_tensor (bool): If ``True``, a hidden tensor called "VDS_INDEX" is created which contains the sample indices in the source view.
-
-        Returns:
-            Dataset: New dataset object.
-
-        Raises:
-            DatasetHandlerError: If a dataset already exists at destination path and overwrite is False.
-        """
         if isinstance(dest, str):
             path = dest
         else:
             path = dest.path
 
-        report_params = {
-            "Tensors": tensors,
-            "Overwrite": overwrite,
-            "Num_Workers": num_workers,
-            "Scheduler": scheduler,
-            "Progressbar": progressbar,
-            "Public": public,
-        }
-
-        if path.startswith("hub://"):
-            report_params["Dest"] = path
-        feature_report_path(self.path, "copy", report_params, token=token)
-
         dest_ds = deeplake.api.dataset.dataset._like(
             dest,
             self,
             runtime=runtime,
             tensors=tensors,
             creds=creds,
             token=token,
@@ -3542,14 +3679,27 @@
 
         Returns:
             Dataset: New dataset object.
 
         Raises:
             DatasetHandlerError: If a dataset already exists at destination path and overwrite is False.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="copy",
+            parameters={
+                "tensors": tensors,
+                "overwrite": overwrite,
+                "num_workers": num_workers,
+                "scheduler": scheduler,
+                "progressbar": progressbar,
+                "public": public,
+            },
+        )
+
         return self._copy(
             dest,
             runtime,
             tensors,
             overwrite,
             creds,
             token,
@@ -3563,14 +3713,20 @@
     @spinner
     def reset(self, force: bool = False):
         """Resets the uncommitted changes present in the branch.
 
         Note:
             The uncommitted data is deleted from underlying storage, this is not a reversible operation.
         """
+
+        deeplake_reporter.feature_report(
+            feature_name="reset",
+            parameters={"force": force},
+        )
+
         storage, version_state = self.storage, self.version_state
         if version_state["commit_node"].children:
             print("You are not at the head node of the branch, cannot reset.")
             return
         if not self.has_head_changes and not force:
             print("There are no uncommitted changes on this branch.")
             return
@@ -3765,15 +3921,18 @@
             height: Union[int, str, None] Optional height of the visualizer canvas.
 
         Raises:
             Exception: If the dataset is not a Deep Lake cloud dataset and the visualization is attempted in colab.
         """
         from deeplake.visualizer import visualize
 
-        deeplake_reporter.feature_report(feature_name="visualize", parameters={})
+        deeplake_reporter.feature_report(
+            feature_name="visualize", parameters={"width": width, "height": height}
+        )
+
         if is_colab():
             provider = self.storage.next_storage
             if isinstance(provider, S3Provider):
                 creds = {
                     "aws_access_key_id": provider.aws_access_key_id,
                     "aws_secret_access_key": provider.aws_secret_access_key,
                     "aws_session_token": provider.aws_session_token,
```

### Comparing `deeplake-3.4.0/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.4.1/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.4.1/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.4.1/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/dataset/invalid_view.py` & `deeplake-3.4.1/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/dataset/view_entry.py` & `deeplake-3.4.1/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/fast_forwarding.py` & `deeplake-3.4.1/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/index/index.py` & `deeplake-3.4.1/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/io.py` & `deeplake-3.4.1/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/ipc.py` & `deeplake-3.4.1/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/link_creds.py` & `deeplake-3.4.1/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/linked_chunk_engine.py` & `deeplake-3.4.1/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/linked_sample.py` & `deeplake-3.4.1/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/linked_tiled_sample.py` & `deeplake-3.4.1/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/lock.py` & `deeplake-3.4.1/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/dataset_meta.py` & `deeplake-3.4.1/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.4.1/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.4.1/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.4.1/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/creds.py` & `deeplake-3.4.1/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/pad.py` & `deeplake-3.4.1/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/sequence.py` & `deeplake-3.4.1/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/shape.py` & `deeplake-3.4.1/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/encode/tile.py` & `deeplake-3.4.1/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/meta/tensor_meta.py` & `deeplake-3.4.1/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/partial_reader.py` & `deeplake-3.4.1/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/partial_sample.py` & `deeplake-3.4.1/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/polygon.py` & `deeplake-3.4.1/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/query/autocomplete.py` & `deeplake-3.4.1/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/query/filter.py` & `deeplake-3.4.1/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/query/query.py` & `deeplake-3.4.1/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/sample.py` & `deeplake-3.4.1/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/serialize.py` & `deeplake-3.4.1/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.4.1/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/gcs.py` & `deeplake-3.4.1/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/google_drive.py` & `deeplake-3.4.1/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/local.py` & `deeplake-3.4.1/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/lru_cache.py` & `deeplake-3.4.1/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/memory.py` & `deeplake-3.4.1/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/provider.py` & `deeplake-3.4.1/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/storage/s3.py` & `deeplake-3.4.1/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tensor.py` & `deeplake-3.4.1/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tensor_link.py` & `deeplake-3.4.1/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/test_serialize.py` & `deeplake-3.4.1/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_compression.py` & `deeplake-3.4.1/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_compute.py` & `deeplake-3.4.1/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.4.1/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_io.py` & `deeplake-3.4.1/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_locking.py` & `deeplake-3.4.1/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_readonly.py` & `deeplake-3.4.1/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tests/test_serialize.py` & `deeplake-3.4.1/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tiling/deserialize.py` & `deeplake-3.4.1/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tiling/optimizer.py` & `deeplake-3.4.1/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.4.1/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tiling/serialize.py` & `deeplake-3.4.1/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.4.1/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/tiling/test_serialize.py` & `deeplake-3.4.1/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/transform/test_transform.py` & `deeplake-3.4.1/deeplake/core/transform/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,19 @@
     compare_dataset_diff,
     compare_tensor_diff,
     get_default_tensor_diff,
     get_default_dataset_diff,
 )
 from deeplake.util.remove_cache import remove_memory_cache
 from deeplake.util.check_installation import ray_installed
-from deeplake.util.exceptions import InvalidOutputDatasetError, TransformError
+from deeplake.util.exceptions import (
+    AllSamplesSkippedError,
+    InvalidOutputDatasetError,
+    TransformError,
+)
 from deeplake.tests.common import parametrize_num_workers
 from deeplake.util.transform import get_pbar_description
 import deeplake
 import gc
 import re
 from deeplake.tests.common import get_dummy_data_path
 
@@ -1436,14 +1440,38 @@
         assert len(ds["boxes"]) == 40
         assert ds["boxes"].meta.min_shape == [1, 4]
         assert ds["boxes"].meta.max_shape == [20, 4]
 
         assert ds["labels"].numpy().shape == (40, 10)
 
 
+def test_all_samples_skipped(local_ds):
+    @deeplake.compute
+    def upload(stuff, ds):
+        if isinstance(stuff["images"], str):
+            sample = deeplake.read(stuff["images"])
+        else:
+            sample = stuff["images"]
+        ds.images.append(sample)
+
+    with local_ds as ds:
+        ds.create_tensor("images", htype="image", sample_compression="png")
+
+    samples = (
+        [{"images": "bad_path"}] * 10
+        + [{"images": BadSample()}] * 20
+        + [{"images": "bad_path"}] * 10
+    )
+
+    with pytest.raises(AllSamplesSkippedError) as e:
+        upload().eval(
+            samples, ds, num_workers=TRANSFORM_TEST_NUM_WORKERS, ignore_errors=True
+        )
+
+
 def test_transform_numpy_only(local_ds):
     @deeplake.compute
     def upload(i, ds):
         ds.abc.extend(i * np.ones((10, 5, 5)))
 
     with local_ds as ds:
         ds.create_tensor("abc")
```

### Comparing `deeplake-3.4.0/deeplake/core/transform/transform.py` & `deeplake-3.4.1/deeplake/core/transform/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     sanitize_workers_scheduler,
     store_data_slice,
     store_data_slice_with_pbar,
     check_checkpoint_interval,
 )
 from deeplake.util.encoder import merge_all_meta_info
 from deeplake.util.exceptions import (
+    AllSamplesSkippedError,
     HubComposeEmptyListError,
     HubComposeIncompatibleFunction,
     TransformError,
 )
 from deeplake.hooks import dataset_written, dataset_read
 from deeplake.util.version_control import auto_checkout
 from deeplake.util.class_label import sync_labels
@@ -292,14 +293,16 @@
                     target_ds.reset(force=True)
                 target_ds._send_compute_progress(**progress_args, status="failed")
                 close_states(compute_provider, pbar, pqueue)
                 index, sample = None, None
                 if isinstance(e, TransformError):
                     index, sample = e.index, e.sample
                     e = e.__cause__  # type: ignore
+                if isinstance(e, AllSamplesSkippedError):
+                    raise e
                 raise TransformError(
                     index=index,
                     sample=sample,
                     samples_processed=samples_processed,
                 ) from e
             finally:
                 reload_and_rechunk(
```

### Comparing `deeplake-3.4.0/deeplake/core/transform/transform_dataset.py` & `deeplake-3.4.1/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/transform/transform_tensor.py` & `deeplake-3.4.1/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.4.1/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/version_control/commit_diff.py` & `deeplake-3.4.1/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/version_control/commit_node.py` & `deeplake-3.4.1/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.4.1/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/version_control/test_merge.py` & `deeplake-3.4.1/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/core/version_control/test_version_control.py` & `deeplake-3.4.1/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.4.1/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/dataloader.py` & `deeplake-3.4.1/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.4.1/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.4.1/deeplake/enterprise/libdeeplake_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
-from deeplake.util.bugout_reporter import deeplake_reporter
 from deeplake.core.dataset.deeplake_query_dataset import DeepLakeQueryDataset
 from typing import Optional, Union
 
 import numpy as np
 
 
-@deeplake_reporter.record_call
 def query(dataset, query_string: str):
     """Returns a sliced :class:`~deeplake.core.dataset.Dataset` with given query results.
 
     It allows to run SQL like queries on dataset and extract results. See supported keywords and the Tensor Query Language documentation
     :ref:`here <tql>`.
 
 
@@ -48,15 +46,14 @@
         view = DeepLakeQueryDataset(deeplake_ds=dataset, indra_ds=dsv)
         view._tql_query = query_string
         if hasattr(dataset, "is_actually_cloud"):
             view.is_actually_cloud = dataset.is_actually_cloud
         return view
 
 
-@deeplake_reporter.record_call
 def sample_by(
     dataset,
     weights: Union[str, list, tuple, np.ndarray],
     replace: Optional[bool] = True,
     size: Optional[int] = None,
 ):
     """Returns a sliced :class:`~deeplake.core.dataset.Dataset` with given sampler applied.
```

### Comparing `deeplake-3.4.0/deeplake/enterprise/test_pytorch.py` & `deeplake-3.4.1/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/test_query.py` & `deeplake-3.4.1/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.4.1/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/enterprise/util.py` & `deeplake-3.4.1/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/hooks.py` & `deeplake-3.4.1/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/htype.py` & `deeplake-3.4.1/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.4.1/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/pytorch/common.py` & `deeplake-3.4.1/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.4.1/deeplake/integrations/pytorch/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Sequence, List, Dict
 from deeplake.constants import MB
 from deeplake.integrations.pytorch.common import PytorchTransformFunction
 from deeplake.util.exceptions import TransformFailedError
 
 from deeplake.util.iterable_ordered_dict import IterableOrderedDict
+from deeplake.util.warnings import always_warn
 from deeplake.core.io import (
     DistributedScheduler,
     SampleStreaming,
     Schedule,
     SequentialMultithreadScheduler,
     ShufflingSchedulerWrapper,
     SingleThreadScheduler,
@@ -183,15 +184,15 @@
     ) -> None:
         super().__init__()
 
         self.torch_datset = TorchDataset(
             dataset,
             tensors=tensors,
             use_local_cache=use_local_cache,
-            transform=None if buffer_size else transform,
+            transform=transform,
             num_workers=num_workers,
             shuffle=True,
             return_index=return_index,
             pad_tensors=pad_tensors,
             decode_method=decode_method,
         )
         if buffer_size:
@@ -215,21 +216,21 @@
             buffer = ShuffleBuffer(buffer_size)
             it = iter(sub_loader)
             try:
                 while True:
                     next_batch = next(it)
                     for val in next_batch:
                         result = buffer.exchange(val)
-                        if result:
-                            yield _process(result, self.transform, self.return_index)
+                        if result is not None:
+                            yield result
                     del next_batch
             except StopIteration:
                 pass
             while not buffer.emtpy():
-                yield _process(buffer.exchange(None), self.transform, self.return_index)
+                yield buffer.exchange(None)
             del it
         else:
             for batch in sub_loader:
                 yield from batch
         del sub_loader
 
     def __len__(self):
```

### Comparing `deeplake-3.4.0/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.4.1/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/tf/common.py` & `deeplake-3.4.1/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.4.1/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.4.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/integrations/wandb/wandb.py` & `deeplake-3.4.1/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/tests/cache_fixtures.py` & `deeplake-3.4.1/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/tests/client_fixtures.py` & `deeplake-3.4.1/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/tests/common.py` & `deeplake-3.4.1/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/tests/dataset_fixtures.py` & `deeplake-3.4.1/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/tests/path_fixtures.py` & `deeplake-3.4.1/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/tests/storage_fixtures.py` & `deeplake-3.4.1/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/access_method.py` & `deeplake-3.4.1/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/agreement.py` & `deeplake-3.4.1/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/array_list.py` & `deeplake-3.4.1/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/assert_byte_indexes.py` & `deeplake-3.4.1/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/auto.py` & `deeplake-3.4.1/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/bugout_reporter.py` & `deeplake-3.4.1/deeplake/util/bugout_reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,22 +116,22 @@
     session_id=session_id,
     bugout_token=BUGOUT_TOKEN,
     blacklist_fn=blacklist_token_parameters_fn,
     tags=[],
 )
 
 
-def set_username(reporter: HumbugReporter, username: str) -> None:
-    index, current_username = find_current_username(reporter)
+def set_username(username: str) -> None:
+    index, current_username = find_current_username()
 
     if current_username is None:
-        reporter.tags.append(f"username:{username}")
+        deeplake_reporter.tags.append(f"username:{username}")
     else:
         if f"username:{username}" != current_username:
-            reporter.tags[index] = f"username:{username}"
+            deeplake_reporter.tags[index] = f"username:{username}"
 
 
 hub_user = bugout_reporting_config.get("username")
 if hub_user is not None:
     deeplake_reporter.tags.append(f"username:{hub_user}")
 
 machine_id = bugout_reporting_config.get("machine_id")
@@ -152,20 +152,20 @@
     if path.startswith(starts_with):
         parameters["Path"] = path
 
     if token is not None:
         client = DeepLakeBackendClient(token=token)
         username = client.get_user_profile()["name"]
 
-        set_username(deeplake_reporter, username)
+        set_username(username)
 
     deeplake_reporter.feature_report(
         feature_name=feature_name,
         parameters=parameters,
     )
 
 
-def find_current_username(reporter: HumbugReporter):
-    for index, tag in enumerate(reporter.tags):
+def find_current_username():
+    for index, tag in enumerate(deeplake_reporter.tags):
         if "username" in tag:
             return index, tag
     return None, None
```

### Comparing `deeplake-3.4.0/deeplake/util/cache_chain.py` & `deeplake-3.4.1/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/casting.py` & `deeplake-3.4.1/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/check_latest_version.py` & `deeplake-3.4.1/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/chunk_engine.py` & `deeplake-3.4.1/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/class_label.py` & `deeplake-3.4.1/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/compute.py` & `deeplake-3.4.1/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/connect_dataset.py` & `deeplake-3.4.1/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/dataset.py` & `deeplake-3.4.1/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/diff.py` & `deeplake-3.4.1/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/downsample.py` & `deeplake-3.4.1/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/encoder.py` & `deeplake-3.4.1/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/exceptions.py` & `deeplake-3.4.1/deeplake/util/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,15 +552,15 @@
         self.index = index
         self.sample = sample
         # multiprocessing re raises error with str
         if isinstance(index, str):
             super().__init__(index)
         else:
             print_item = print_path = False
-            if sample:
+            if sample is not None:
                 print_item = is_primitive(sample)
                 print_path = has_path(sample)
 
             msg = f"Transform failed"
             if index is not None:
                 msg += f" at index {index} of the input data"
 
@@ -576,15 +576,15 @@
             msg += " See traceback for more details."
             super().__init__(msg)
 
 
 class SampleAppendError(Exception):
     def __init__(self, tensor, sample=None):
         print_item = print_path = False
-        if sample:
+        if sample is not None:
             print_item = is_primitive(sample)
             print_path = has_path(sample)
         if print_item or print_path:
             msg = "Failed to append the sample "
 
             if print_item:
                 msg += str(sample) + " "
@@ -1045,7 +1045,15 @@
 class MissingManagedCredsError(Exception):
     pass
 
 
 class SampleUpdateError(Exception):
     def __init__(self, key: str):
         super().__init__(f"Unable to update sample in tensor {key}.")
+
+
+class AllSamplesSkippedError(Exception):
+    def __init__(self):
+        super().__init__(
+            "All samples were skipped during the transform. "
+            "Ensure your transform pipeline is correct before you set `ignore_errors=True`."
+        )
```

### Comparing `deeplake-3.4.0/deeplake/util/exif.py` & `deeplake-3.4.1/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/from_tfds.py` & `deeplake-3.4.1/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/htype.py` & `deeplake-3.4.1/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/image.py` & `deeplake-3.4.1/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/invalid_view_op.py` & `deeplake-3.4.1/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/iteration_warning.py` & `deeplake-3.4.1/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/json.py` & `deeplake-3.4.1/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/keys.py` & `deeplake-3.4.1/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/link.py` & `deeplake-3.4.1/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/logging.py` & `deeplake-3.4.1/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/merge.py` & `deeplake-3.4.1/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/modified.py` & `deeplake-3.4.1/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/notebook.py` & `deeplake-3.4.1/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/mesh.py` & `deeplake-3.4.1/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.4.1/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.4.1/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.4.1/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.4.1/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.4.1/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.4.1/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.4.1/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.4.1/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.4.1/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/path.py` & `deeplake-3.4.1/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/pretty_print.py` & `deeplake-3.4.1/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/remove_cache.py` & `deeplake-3.4.1/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/scheduling.py` & `deeplake-3.4.1/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/shape_interval.py` & `deeplake-3.4.1/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/spinner.py` & `deeplake-3.4.1/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/split.py` & `deeplake-3.4.1/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/storage.py` & `deeplake-3.4.1/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tag.py` & `deeplake-3.4.1/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/testing.py` & `deeplake-3.4.1/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_auto.py` & `deeplake-3.4.1/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.4.1/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.4.1/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_read.py` & `deeplake-3.4.1/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.4.1/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_split.py` & `deeplake-3.4.1/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/tests/test_version_control.py` & `deeplake-3.4.1/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/transform.py` & `deeplake-3.4.1/deeplake/util/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from deeplake.util.remove_cache import (
     get_base_storage,
     get_dataset_with_zero_size_cache,
 )
 from deeplake.util.keys import get_tensor_meta_key
 from deeplake.util.version_control import auto_checkout, load_meta
 from deeplake.util.exceptions import (
+    AllSamplesSkippedError,
     InvalidInputDataError,
     InvalidOutputDatasetError,
     InvalidTransformDataset,
     TensorMismatchError,
     TensorDoesNotExistError,
     TransformError,
     SampleAppendError,
@@ -160,88 +161,111 @@
     transform_dataset,
     pipeline,
     tensors,
     end_input_idx,
     ignore_errors,
 ):
     start_input_idx = transform_dataset.start_input_idx
+    skipped_samples = 0
     for i in range(start_input_idx, end_input_idx + 1):
         sample = (
             data_slice[i : i + 1]
             if pd and isinstance(data_slice, pd.DataFrame)
             else data_slice[i]
         )
         try:
             out = transform_sample(sample, pipeline, tensors)
 
             write_sample_to_transform_dataset(out, transform_dataset)
 
             transform_dataset.flush()
         except Exception as e:
             if isinstance(e, SampleAppendError) and ignore_errors:
+                skipped_samples += 1
                 continue
             raise TransformError(offset + i, sample) from e
+    return skipped_samples
 
 
 def _transform_and_append_data_slice(
     data_slice,
     offset,
     transform_dataset,
     pipeline,
     tensors,
     skip_ok,
     pg_callback,
     ignore_errors,
 ):
+    """Appends a data slice. Returns ``True`` if any samples were appended and ``False`` otherwise."""
     n = len(data_slice)
+    skipped_samples = 0
+    skipped_samples_in_current_batch = 0
 
     pipeline_checked = False
 
     for i, sample in enumerate(
         (data_slice[i : i + 1] for i in range(n))
         if pd and isinstance(data_slice, pd.DataFrame)
         else data_slice
     ):
         try:
             transform_dataset.set_start_input_idx(i)
 
             try:
                 out = transform_sample(sample, pipeline, tensors)
+
+                if not pipeline_checked:
+                    _check_pipeline(out, tensors, skip_ok)
+                    pipeline_checked = True
+
+                write_sample_to_transform_dataset(out, transform_dataset)
+
             except SampleAppendError as e:
                 if ignore_errors:
-                    continue
-                raise TransformError(offset + i, sample) from e
+                    skipped_samples += 1
+                    skipped_samples_in_current_batch += 1
+                else:
+                    raise TransformError(offset + i, sample) from e
 
-            if not pipeline_checked:
-                _check_pipeline(out, tensors, skip_ok)
-                pipeline_checked = True
+            finally:
+                if i == n - 1:
+                    transform_dataset.flush()
+                else:
+                    transform_dataset.check_flush()
 
-            write_sample_to_transform_dataset(out, transform_dataset)
+                # dataset flushed, reset skipped sample count
+                if transform_dataset.start_input_idx is None:
+                    skipped_samples_in_current_batch = 0
 
-            if i == n - 1:
-                transform_dataset.flush()
-            else:
-                transform_dataset.check_flush()
+                if pg_callback is not None:
+                    pg_callback(1)
 
-            if pg_callback is not None:
-                pg_callback(1)
+        # failure at chunk_engine
+        # retry one sample at a time
         except SampleAppendError:
-            # failure at chunk_engine
-            # retry one sample at a time
-            _handle_transform_error(
+            # reset skipped sample count to avoid double counting
+            skipped_samples -= skipped_samples_in_current_batch
+            skipped_samples_in_current_batch = 0
+
+            skipped_samples += _handle_transform_error(
                 data_slice,
                 offset,
                 transform_dataset,
                 pipeline,
                 tensors,
                 i,
                 ignore_errors,
             )
             continue
 
+    if skipped_samples == n:
+        return False
+    return True
+
 
 def _retrieve_memory_objects(all_chunk_engines):
     all_tensor_metas = {}
     all_chunk_id_encoders = {}
     all_tile_encoders = {}
     all_sequence_encoders = {}
     all_pad_encoders = {}
@@ -304,32 +328,35 @@
         rel_tensors,
         all_chunk_engines,
         group_index,
         label_temp_tensors,
         cache_size=cache_size,
     )
 
+    ret = True
     if extend_only:
         _extend_data_slice(
             data_slice, offset, transform_dataset, pipeline.functions[0], pg_callback
         )
     else:
-        _transform_and_append_data_slice(
+        ret = _transform_and_append_data_slice(
             data_slice,
             offset,
             transform_dataset,
             pipeline,
             rel_tensors,
             skip_ok,
             pg_callback,
             ignore_errors,
         )
 
     # retrieve relevant objects from memory
-    return _retrieve_memory_objects(all_chunk_engines)
+    meta = _retrieve_memory_objects(all_chunk_engines)
+    meta["all_samples_skipped"] = not ret
+    return meta
 
 
 def create_worker_chunk_engines(
     tensors: List[str],
     label_temp_tensors: Dict[str, str],
     output_storage: StorageProvider,
     version_state,
@@ -561,14 +588,16 @@
     if num_workers <= 0:
         scheduler = "serial"
     num_workers = max(num_workers, 1)
     return num_workers, scheduler
 
 
 def process_transform_result(result: List[Dict]):
+    if all(res.get("all_samples_skipped") for res in result):
+        raise AllSamplesSkippedError
     if not result:
         return result
     final = defaultdict(list)
     keys = list(result[0].keys())
     for item in result:
         for key in keys:
             final[key].append(item[key])
```

### Comparing `deeplake-3.4.0/deeplake/util/version_control.py` & `deeplake-3.4.1/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/util/video.py` & `deeplake-3.4.1/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/visualizer/video_streaming.py` & `deeplake-3.4.1/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake/visualizer/visualizer.py` & `deeplake-3.4.1/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake.egg-info/PKG-INFO` & `deeplake-3.4.1/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.4.0
+Version: 3.4.1
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.4.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.4.1 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
```

### Comparing `deeplake-3.4.0/deeplake.egg-info/SOURCES.txt` & `deeplake-3.4.1/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/deeplake.egg-info/requires.txt` & `deeplake-3.4.1/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.0/setup.py` & `deeplake-3.4.1/setup.py`

 * *Files identical despite different names*

