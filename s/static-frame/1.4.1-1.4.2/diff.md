# Comparing `tmp/static-frame-1.4.1.tar.gz` & `tmp/static-frame-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.4.1.tar", last modified: Fri May  5 16:02:33 2023, max compression
+gzip compressed data, was "static-frame-1.4.2.tar", last modified: Tue May  9 01:49:39 2023, max compression
```

## Comparing `static-frame-1.4.1.tar` & `static-frame-1.4.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.925144 static-frame-1.4.1/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.1/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.1/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-05 16:02:33.925144 static-frame-1.4.1/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-04 17:09:05.000000 static-frame-1.4.1/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.1/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-04 17:09:05.000000 static-frame-1.4.1/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-04 17:09:05.000000 static-frame-1.4.1/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-05 16:02:33.925144 static-frame-1.4.1/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.1/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.909144 static-frame-1.4.1/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7660 2023-05-05 03:07:47.000000 static-frame-1.4.1/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.917144 static-frame-1.4.1/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   379744 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    56830 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107720 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.4.1/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14787 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   185709 2023-05-05 03:05:19.000000 static-frame-1.4.1/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   128804 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.917144 static-frame-1.4.1/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.925144 static-frame-1.4.1/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.1/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   641142 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.1/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23164 2023-05-05 03:05:19.000000 static-frame-1.4.1/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.1/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-04-24 22:32:18.000000 static-frame-1.4.1/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14218 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-04-19 18:21:25.000000 static-frame-1.4.1/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10382 2023-03-23 21:26:53.000000 static-frame-1.4.1/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.1/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-05 16:02:33.909144 static-frame-1.4.1/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-05 16:02:33.000000 static-frame-1.4.1/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.262997 static-frame-1.4.2/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2022-09-18 23:42:20.000000 static-frame-1.4.2/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-08-07 22:56:47.000000 static-frame-1.4.2/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-09 01:49:39.262997 static-frame-1.4.2/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-09 00:42:47.000000 static-frame-1.4.2/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2022-09-18 23:42:20.000000 static-frame-1.4.2/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-09 00:42:47.000000 static-frame-1.4.2/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-09 00:42:47.000000 static-frame-1.4.2/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-09 01:49:39.262997 static-frame-1.4.2/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-01-27 15:25:04.000000 static-frame-1.4.2/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.254998 static-frame-1.4.2/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7660 2023-05-09 01:09:37.000000 static-frame-1.4.2/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.258997 static-frame-1.4.2/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-02-23 20:10:49.000000 static-frame-1.4.2/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-02-27 23:01:10.000000 static-frame-1.4.2/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-04-14 20:39:45.000000 static-frame-1.4.2/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2022-10-01 15:52:09.000000 static-frame-1.4.2/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-03-28 21:18:03.000000 static-frame-1.4.2/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-02-23 22:39:48.000000 static-frame-1.4.2/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   378205 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56830 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107720 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-02-01 00:09:42.000000 static-frame-1.4.2/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-01-28 23:33:40.000000 static-frame-1.4.2/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-01-28 23:33:40.000000 static-frame-1.4.2/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-03-28 21:18:03.000000 static-frame-1.4.2/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-05-02 20:46:35.000000 static-frame-1.4.2/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-03-28 21:18:03.000000 static-frame-1.4.2/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-02-28 22:54:13.000000 static-frame-1.4.2/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2022-11-10 00:09:54.000000 static-frame-1.4.2/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-02-27 23:39:36.000000 static-frame-1.4.2/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2022-10-13 03:47:27.000000 static-frame-1.4.2/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2022-09-29 04:16:16.000000 static-frame-1.4.2/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2022-09-29 04:16:16.000000 static-frame-1.4.2/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-02-21 22:37:54.000000 static-frame-1.4.2/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-08 23:21:40.000000 static-frame-1.4.2/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-02-03 19:24:20.000000 static-frame-1.4.2/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-02-23 22:39:48.000000 static-frame-1.4.2/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   185709 2023-05-05 18:43:53.000000 static-frame-1.4.2/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   129022 2023-05-08 23:21:40.000000 static-frame-1.4.2/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2022-12-20 03:10:29.000000 static-frame-1.4.2/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-02-28 22:54:13.000000 static-frame-1.4.2/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.258997 static-frame-1.4.2/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-01-30 03:11:00.000000 static-frame-1.4.2/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.262997 static-frame-1.4.2/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-02-23 22:39:48.000000 static-frame-1.4.2/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-02-21 22:37:54.000000 static-frame-1.4.2/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   641433 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-05-02 20:46:35.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-02-28 22:54:13.000000 static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23164 2023-05-05 18:43:53.000000 static-frame-1.4.2/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2022-09-29 04:16:16.000000 static-frame-1.4.2/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-05-02 20:46:35.000000 static-frame-1.4.2/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-02-21 22:37:54.000000 static-frame-1.4.2/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-08 23:21:40.000000 static-frame-1.4.2/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.254998 static-frame-1.4.2/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.4.1/LICENSE.txt` & `static-frame-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/PKG-INFO` & `static-frame-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.1
+Version: 1.4.2
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -45,15 +45,15 @@
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
-        - arraymap==0.1.7
+        - arraymap==0.1.8
         - arraykit==0.3.4
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
```

### Comparing `static-frame-1.4.1/README.rst` & `static-frame-1.4.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 Dependencies
 --------------
 
 Core StaticFrame requires the following:
 
 - Python>=3.7
 - NumPy>=1.18.5
-- arraymap==0.1.7
+- arraymap==0.1.8
 - arraykit==0.3.4
 
 For extended input and output, the following packages are required:
 
 - pandas>=0.24.2
 - xlsxwriter>=1.1.2
 - openpyxl>=3.0.9
```

### Comparing `static-frame-1.4.1/setup.py` & `static-frame-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/__init__.py` & `static-frame-1.4.2/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
```

### Comparing `static-frame-1.4.1/static_frame/__main__.py` & `static-frame-1.4.2/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/archive_npy.py` & `static-frame-1.4.2/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/axis_map.py` & `static-frame-1.4.2/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/batch.py` & `static-frame-1.4.2/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/bus.py` & `static-frame-1.4.2/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/container.py` & `static-frame-1.4.2/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/container_util.py` & `static-frame-1.4.2/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/display.py` & `static-frame-1.4.2/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/display_color.py` & `static-frame-1.4.2/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/display_config.py` & `static-frame-1.4.2/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/display_html_datatables.py` & `static-frame-1.4.2/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/display_visidata.py` & `static-frame-1.4.2/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/doc_str.py` & `static-frame-1.4.2/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/exception.py` & `static-frame-1.4.2/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/fill_value_auto.py` & `static-frame-1.4.2/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/frame.py` & `static-frame-1.4.2/static_frame/core/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -2085,70 +2085,14 @@
                 dtypes=dtypes,
                 name=name,
                 consolidate_blocks=consolidate_blocks,
                 index_constructor=index_constructor,
                 columns_constructor=columns_constructor,
                 )
 
-    @classmethod
-    @doc_inject(selector='constructor_frame')
-    def from_json(cls,
-            json_data: tp.Union[str, StringIO],
-            *,
-            dtypes: DtypesSpecifier = None,
-            name: tp.Hashable = None,
-            consolidate_blocks: bool = False
-            ) -> 'Frame':
-        '''Frame constructor from an in-memory JSON document.
-
-        Args:
-            json_data: a string of JSON, encoding a table as an array of JSON objects.
-            {dtypes}
-            {name}
-            {consolidate_blocks}
-
-        Returns:
-            :obj:`static_frame.Frame`
-        '''
-        # DEPRECATE for 1.0
-        return cls.from_json_records(json_data, # type: ignore
-                name=name,
-                dtypes=dtypes,
-                consolidate_blocks=consolidate_blocks
-                )
-
-    @classmethod
-    @doc_inject(selector='constructor_frame')
-    def from_json_url(cls,
-            url: str,
-            *,
-            dtypes: DtypesSpecifier = None,
-            name: tp.Hashable = None,
-            consolidate_blocks: bool = False
-            ) -> 'Frame':
-        '''Frame constructor from a JSON documenst provided via a URL.
-
-        Args:
-            url: URL to the JSON resource.
-            {dtypes}
-            {name}
-            {consolidate_blocks}
-
-        Returns:
-            :obj:`static_frame.Frame`
-        '''
-        # DEPRECATE for 1.0
-        from static_frame.core.www import WWW
-        sio = WWW.from_file(url, in_memory=True)
-        return cls.from_json(sio, # type: ignore #pragma: no cover
-                name=name,
-                dtypes=dtypes,
-                consolidate_blocks=consolidate_blocks
-                )
-
     #---------------------------------------------------------------------------
     @classmethod
     @doc_inject(selector='constructor_frame')
     def from_delimited(cls,
             fp: PathSpecifierOrFileLikeOrIterator,
             *,
             delimiter: str,
@@ -9149,25 +9093,29 @@
             raise RuntimeError(f'The provided key ({key}) is already defined in columns; if you want to change or replace this column, use .assign to get new Frame')
 
         row_count = len(self._index)
 
         if isinstance(value, Series):
             # select only the values matching our index
             block = value.reindex(self.index, fill_value=fill_value).values
+        elif isinstance(value, Index):
+            if len(value) != row_count:
+                raise RuntimeError(f'incorrectly sized unindexed value: {len(value)} != {row_count}')
+            block = value.values
         elif isinstance(value, Frame):
             raise RuntimeError(
                     f'cannot use setitem with a Frame; use {self.__class__.__name__}.extend()')
         elif value.__class__ is np.ndarray:
             # this permits unaligned assignment as no index is used, possibly remove
             if value.ndim != 1:
                 raise RuntimeError('can only use setitem with 1D containers')
             if len(value) != row_count:
                 # block may have zero shape if created without columns
                 raise RuntimeError(f'incorrectly sized unindexed value: {len(value)} != {row_count}')
-            block = value # NOTE: could own_data here with additional argument
+            block = value
 
         else:
             if not hasattr(value, '__iter__') or isinstance(value, str):
                 block = np.full(row_count, value)
                 block.flags.writeable = False
             else:
                 block, _ = iterable_to_array_1d(value) # returns immutable
```

### Comparing `static-frame-1.4.1/static_frame/core/hloc.py` & `static-frame-1.4.2/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index.py` & `static-frame-1.4.2/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index_auto.py` & `static-frame-1.4.2/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index_base.py` & `static-frame-1.4.2/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index_correspondence.py` & `static-frame-1.4.2/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index_datetime.py` & `static-frame-1.4.2/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index_hierarchy.py` & `static-frame-1.4.2/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.4.2/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/interface.py` & `static-frame-1.4.2/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/interface_meta.py` & `static-frame-1.4.2/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/join.py` & `static-frame-1.4.2/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/loc_map.py` & `static-frame-1.4.2/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/memory_measure.py` & `static-frame-1.4.2/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_dt.py` & `static-frame-1.4.2/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_fill_value.py` & `static-frame-1.4.2/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_hashlib.py` & `static-frame-1.4.2/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_iter.py` & `static-frame-1.4.2/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_re.py` & `static-frame-1.4.2/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_selector.py` & `static-frame-1.4.2/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_str.py` & `static-frame-1.4.2/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_transpose.py` & `static-frame-1.4.2/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/node_values.py` & `static-frame-1.4.2/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/pivot.py` & `static-frame-1.4.2/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/platform.py` & `static-frame-1.4.2/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/protocol_dfi.py` & `static-frame-1.4.2/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.4.2/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/quilt.py` & `static-frame-1.4.2/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/rank.py` & `static-frame-1.4.2/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/series.py` & `static-frame-1.4.2/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store.py` & `static-frame-1.4.2/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store_client_mixin.py` & `static-frame-1.4.2/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store_config.py` & `static-frame-1.4.2/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store_filter.py` & `static-frame-1.4.2/static_frame/core/store_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.interface_meta import InterfaceMeta
 from static_frame.core.util import COMPLEX_TYPES
 from static_frame.core.util import DT64_MONTH
@@ -16,16 +15,16 @@
 from static_frame.core.util import DTYPE_OBJECT
 from static_frame.core.util import DTYPE_OBJECT_KIND
 from static_frame.core.util import DTYPE_STR_KINDS
 from static_frame.core.util import EMPTY_SET
 from static_frame.core.util import FLOAT_TYPES
 from static_frame.core.util import NAT
 from static_frame.core.util import NAT_STR
+from static_frame.core.util import frozenset_filter
 
-# from static_frame.core.util import InexactTypes
 
 class StoreFilter(metaclass=InterfaceMeta):
     '''
     Utility for defining and applying translation of values going to and from a data store, as needed for XLSX and other writers.
     '''
 
     __slots__ = (
@@ -83,37 +82,37 @@
             # from type to str
             from_nan: tp.Optional[str] = '',
             from_nat: tp.Optional[str] = '',
             from_none: tp.Optional[str] = 'None',
             from_posinf: tp.Optional[str] = 'inf',
             from_neginf: tp.Optional[str] = '-inf',
             # str to type
-            to_nan: tp.FrozenSet[str] = frozenset(('', 'nan', 'NaN', 'NAN', 'NULL', '#N/A')),
-            to_nat: tp.FrozenSet[str] = frozenset(()), # do not assume there are NaTs.
-            to_none: tp.FrozenSet[str] = frozenset(('None',)),
-            to_posinf: tp.FrozenSet[str] = frozenset(('inf',)),
-            to_neginf: tp.FrozenSet[str] = frozenset(('-inf',)),
+            to_nan: tp.Collection[str] = frozenset(('', 'nan', 'NaN', 'NAN', 'NULL', '#N/A')),
+            to_nat: tp.Collection[str] = frozenset(()), # do not assume there are NaTs.
+            to_none: tp.Collection[str] = frozenset(('None',)),
+            to_posinf: tp.Collection[str] = frozenset(('inf',)),
+            to_neginf: tp.Collection[str] = frozenset(('-inf',)),
             # from float to str
             value_format_float_positional: tp.Optional[str] = None,
             value_format_float_scientific: tp.Optional[str] = None,
             value_format_complex_positional: tp.Optional[str] = None,
             value_format_complex_scientific: tp.Optional[str] = None,
             ) -> None:
 
         self.from_nan = from_nan
         self.from_nat = from_nat
         self.from_none = from_none
         self.from_posinf = from_posinf
         self.from_neginf = from_neginf
 
-        self.to_nan = to_nan
-        self.to_nat = to_nat
-        self.to_none = to_none
-        self.to_posinf = to_posinf
-        self.to_neginf = to_neginf
+        self.to_nan = frozenset_filter(to_nan)
+        self.to_nat = frozenset_filter(to_nat)
+        self.to_none = frozenset_filter(to_none)
+        self.to_posinf = frozenset_filter(to_posinf)
+        self.to_neginf = frozenset_filter(to_neginf)
 
         self.value_format_float_positional = value_format_float_positional
         self.value_format_float_scientific = value_format_float_scientific
         self.value_format_complex_positional = value_format_complex_positional
         self.value_format_complex_scientific = value_format_complex_scientific
 
         self._value_format_active = (
@@ -156,16 +155,15 @@
                 (NAT, tuple(self.to_nat)),
                 (None, tuple(self.to_none)),
                 (np.inf, tuple(self.to_posinf)),
                 (-np.inf, tuple(self.to_neginf)),
                 )
 
     # --------------------------------------------------------------------------
-    # converting from types (in memory) to datastore
-
+    # converting from types (in memory) to data store
 
     def _format_inexact_element(self,
             value: tp.Any,
             kind: str,
             ) -> tp.Any:
         '''
         Must let unexact types pass, as object arrays will have mixed types.
@@ -196,15 +194,14 @@
         # is_complex
         if self.value_format_complex_scientific is not None and is_scientific:
             return self.value_format_complex_scientific.format(value)
         elif self.value_format_complex_positional is not None:
             return self.value_format_complex_positional.format(value)
         return value
 
-
     def _format_inexact_array(self,
             array: np.ndarray,
             array_object: tp.Optional[np.ndarray],
             ) -> np.ndarray:
         '''
         Args:
             array_object: if we have already created an object array, use it as destination, mutating values in-place. ``array`` and ``array_object`` can be the same array.
@@ -344,15 +341,14 @@
                         if post is None:
                             post = array.astype(object) # get a copy to mutate
                         post[found] = value_replace
             return post if post is not None else array
 
         return array
 
-
     def to_type_filter_element(self,
             value: tp.Any
             ) -> tp.Any:
         '''
         Given a value wich may be an encoded string, decode into a type.
         '''
         if isinstance(value, str):
@@ -362,15 +358,14 @@
         return value
 
     # def to_type_filter_iterable(self, iterable: tp.Iterable[tp.Any]) -> tp.Iterator[tp.Any]:
     #     for value in iterable:
     #         yield self.to_type_filter_element(value)
 
 
-
 STORE_FILTER_DEFAULT = StoreFilter()
 
 STORE_FILTER_DISABLE = StoreFilter(
             from_nan=None,
             from_none=None,
             from_posinf=None,
             from_neginf=None,
```

### Comparing `static-frame-1.4.1/static_frame/core/store_hdf5.py` & `static-frame-1.4.2/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store_sqlite.py` & `static-frame-1.4.2/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store_xlsx.py` & `static-frame-1.4.2/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/store_zip.py` & `static-frame-1.4.2/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/style_config.py` & `static-frame-1.4.2/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/type_blocks.py` & `static-frame-1.4.2/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/util.py` & `static-frame-1.4.2/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,21 +294,18 @@
 
 CallableOrCallableMap = tp.Union[AnyCallable, tp.Mapping[tp.Hashable, AnyCallable]]
 
 # for explivitl selection hashables, or things that will be converted to lists of hashables (explicitly lists)
 KeyOrKeys = tp.Union[tp.Hashable, tp.Iterable[tp.Hashable]]
 BoolOrBools = tp.Union[bool, tp.Iterable[bool]]
 
-
-
 PathSpecifier = tp.Union[str, PathLike]
 PathSpecifierOrFileLike = tp.Union[str, PathLike, tp.TextIO]
 PathSpecifierOrFileLikeOrIterator = tp.Union[str, PathLike, tp.TextIO, tp.Iterator[str]]
 
-
 DtypeSpecifier = tp.Optional[tp.Union[str, np.dtype, type]]
 
 def validate_dtype_specifier(value: tp.Any) -> DtypeSpecifier:
     if value is None or isinstance(value, np.dtype):
         return value
 
     dt = np.dtype(value)
@@ -522,14 +519,15 @@
 class UFuncCategory(Enum):
     BOOL = 0
     SELECTION = 1
     STATISTICAL = 2 # go to default float type if int, float/complex keep size
     CUMMULATIVE = 3 # go to max size if int, float/complex keep size
     SUMMING = 4 # same except bool goes to max int
 
+
 UFUNC_MAP: tp.Dict[UFunc, UFuncCategory] = {
     all: UFuncCategory.BOOL,
     any: UFuncCategory.BOOL,
     np.all: UFuncCategory.BOOL,
     np.any: UFuncCategory.BOOL,
 
     sum: UFuncCategory.SUMMING,
@@ -620,15 +618,14 @@
             return dtype # keep same size
 
     return None
 
 #-------------------------------------------------------------------------------
 FGItemT = tp.TypeVar('FGItemT')
 
-
 class FrozenGenerator:
     '''
     A wrapper of an iterator (or iterable) that stores values iterated for later recall; this never iterates the iterator unbound, but always iterates up to a target.
     '''
     __slots__ = (
         '_gen',
         '_src',
@@ -649,30 +646,32 @@
             for k in range(start, key + 1):
                 try:
                     self._src.append(next(self._gen))
                 except StopIteration:
                     raise IndexError(k) from None
         return self._src[key]
 
-
 #-------------------------------------------------------------------------------
 # join utils
 
 class Join(Enum):
     INNER = 0
     LEFT = 1
     RIGHT = 2
     OUTER = 3
 
+
 class Pair(tuple): #type: ignore
     pass
 
+
 class PairLeft(Pair):
     pass
 
+
 class PairRight(Pair):
     pass
 
 #-------------------------------------------------------------------------------
 
 def bytes_to_size_label(size_bytes: int) -> str:
     if size_bytes == 0:
@@ -685,14 +684,24 @@
         s = size_bytes
     else:
         s = round(size_bytes / p, 2)
     return f'{s} {size_name[i]}'
 
 #-------------------------------------------------------------------------------
 
+_T = tp.TypeVar('_T', bound=tp.Hashable)
+
+def frozenset_filter(src: tp.Iterable[_T]) -> tp.FrozenSet[_T]:
+    '''
+    Return a frozenset of `src` if not already a frozenset.
+    '''
+    if isinstance(src, frozenset):
+        return src
+    return frozenset(src)
+
 # def mloc(array: np.ndarray) -> int:
 #     '''Return the memory location of an array.
 #     '''
 #     return tp.cast(int, array.__array_interface__['data'][0])
 
 
 # def immutable_filter(src_array: np.ndarray) -> np.ndarray:
@@ -793,15 +802,14 @@
     values = []
     for idx, col in enumerate(reverse_iter(), start=1):
         values.append(col)
         if idx == reverse_count:
             break
     yield from reversed(values)
 
-
 def dtype_from_element(
         value: tp.Any,
         ) -> np.dtype:
     '''Given an arbitrary hashable to be treated as an element, return the appropriate dtype. This was created to avoid using np.array(value).dtype, which for a Tuple does not return object.
     '''
     if value is np.nan:
         # NOTE: this will not catch all NaN instances, but will catch any default NaNs in function signatures that reference the same NaN object found on the NP root namespace
@@ -814,15 +822,14 @@
     # all arrays, or SF containers, should be treated as objects when elements
     # NOTE: might check for __iter__?
     if hasattr(value, '__len__') and not isinstance(value, str):
         return DTYPE_OBJECT
     # NOTE: calling array and getting dtype on np.nan is faster than combining isinstance, isnan calls
     return np.array(value).dtype
 
-
 # def resolve_dtype(dt1: np.dtype, dt2: np.dtype) -> np.dtype:
 #     '''
 #     Given two dtypes, return a compatible dtype that can hold both contents without truncation.
 #     '''
 #     # NOTE: this is not taking into account endianness; it is not clear if this is important
 #     # NOTE: np.dtype(object) == np.object_, so we can return np.object_
 
@@ -882,16 +889,14 @@
 
 #     for dt in dtypes:
 #         dt_resolve = resolve_dtype(dt_resolve, dt)
 #         if dt_resolve == DTYPE_OBJECT:
 #             return dt_resolve
 #     return dt_resolve
 
-
-
 def concat_resolved(
         arrays: tp.Iterable[np.ndarray],
         axis: int = 0,
         ) -> np.ndarray:
     '''
     Concatenation of 1D or 2D arrays that uses resolved dtypes to avoid truncation. Both axis are supported.
 
@@ -923,15 +928,14 @@
             shape[axis] += array.shape[axis]
 
     out = np.empty(shape=shape, dtype=dt_resolve)
     np.concatenate(arrays, out=out, axis=axis)
     out.flags.writeable = False
     return out
 
-
 def blocks_to_array_2d(
         blocks: tp.Iterator[np.ndarray],
         shape: tp.Optional[tp.Tuple[int, int]] = None,
         dtype: tp.Optional[np.dtype] = None,
         ) -> np.ndarray:
     '''
     Given an iterable of blocks, return a consolidatd array. This is assumed to be an axis 1 style concatenation.
@@ -993,16 +997,14 @@
             end = pos + b.shape[1]
             array[NULL_SLICE, pos: end] = b
             pos = end
 
     array.flags.writeable = False
     return array
 
-
-
 def full_for_fill(
         dtype: tp.Optional[np.dtype],
         shape: tp.Union[int, tp.Tuple[int, ...]],
         fill_value: object,
         resolve_fill_value_dtype: bool = True,
         ) -> np.ndarray:
     '''
@@ -1032,15 +1034,14 @@
         array[NULL_SLICE] = fill_value
     else:
         for iloc in np.ndindex(shape):
             array[iloc] = fill_value
 
     return array
 
-
 def dtype_to_fill_value(dtype: DtypeSpecifier) -> tp.Any:
     '''Given a dtype, return an appropriate and compatible null value. This is used to provide temporary, "dummy" fill values that reduce type coercions.
     '''
     if not isinstance(dtype, np.dtype):
         # we permit things like object, float, etc.
         dtype = np.dtype(dtype)
 
@@ -1139,15 +1140,14 @@
             array_sortable[i] = indices.setdefault(v, len(indices))
         del indices
 
         return np.argsort(array_sortable, kind=kind)
 
     return array.argsort(kind=kind)
 
-
 def ufunc_unique1d(array: np.ndarray) -> np.ndarray:
     '''
     Find the unique elements of an array, ignoring shape. Optimized from NumPy implementation based on assumption of 1D array.
     '''
     if array.dtype.kind == 'O':
         try: # some 1D object arrays are sortable
             array = np.sort(array)
@@ -1191,15 +1191,14 @@
 
     indexer = np.empty(mask.shape, dtype=DTYPE_INT_DEFAULT)
     indexer[positions] = np.cumsum(mask) - 1
     indexer.flags.writeable = False
 
     return values, indexer
 
-
 def ufunc_unique1d_positions(array: np.ndarray,
         ) -> tp.Tuple[np.ndarray, np.ndarray]:
     '''
     Find the unique elements of an array. Optimized from NumPy implementation based on assumption of 1D array. Does not return the unqiue values, but the positions in the original index of those values, as well as the locations of the unique values.
     '''
     positions = argsort_array(array)
 
@@ -1211,15 +1210,14 @@
 
     indexer = np.empty(mask.shape, dtype=np.intp)
     indexer[positions] = np.cumsum(mask) - 1
     indexer.flags.writeable = False
 
     return positions[mask], indexer
 
-
 def ufunc_unique1d_counts(array: np.ndarray,
         ) -> tp.Tuple[np.ndarray, np.ndarray]:
     '''
     Find the unique elements of an array. Optimized from NumPy implementation based on assumption of 1D array. Returns unique values as well as the counts of those unique values from the original array.
     '''
     if array.dtype.kind == 'O':
         try: # some 1D object arrays are sortable
@@ -1308,15 +1306,14 @@
     assert array.ndim == 2
     if not array.flags.c_contiguous:
         array = np.ascontiguousarray(array)
     # NOTE: this could be cached
     dtype = [(f'f{i}', array.dtype) for i in range(array.shape[1])]
     return array.view(dtype)[NULL_SLICE, 0] # get 1D representation
 
-
 def ufunc_unique2d(array: np.ndarray,
         axis: int = 0,
     ) -> np.ndarray:
     '''
     Optimized from NumPy implementation.
     '''
     if array.dtype.kind == 'O':
@@ -1338,15 +1335,14 @@
     consolidated = view_2d_as_1d(array)
     values = ufunc_unique1d(consolidated)
     values = values.view(array.dtype).reshape(-1, array.shape[1]) # restore dtype, shape
     if axis == 1:
         return values.T
     return values
 
-
 def ufunc_unique2d_indexer(array: np.ndarray,
         axis: int = 0,
         ) -> tp.Tuple[np.ndarray, np.ndarray]:
     '''
     Find the unique elements of an array and provide an indexer that shows their locations in the original.
     '''
     if axis == 1:
@@ -1363,15 +1359,14 @@
         values, indexer = ufunc_unique1d_indexer(consolidated)
         values = values.view(array.dtype).reshape(-1, array.shape[1])
 
     if axis == 1:
         return values.T, indexer
     return values, indexer
 
-
 def ufunc_unique(
         array: np.ndarray,
         *,
         axis: tp.Optional[int] = None,
         ) -> np.ndarray:
     '''
     Extended functionality of the np.unique ufunc, to handle cases of mixed typed objects, where NP will fail in finding unique values for a heterogenous object type.
@@ -1381,16 +1376,14 @@
     '''
     if axis is None and array.ndim == 2:
         return ufunc_unique1d(array.reshape(-1)) # reshape over flatten return a view if possible
     elif array.ndim == 1:
         return ufunc_unique1d(array)
     return ufunc_unique2d(array, axis=axis)
 
-
-
 def roll_1d(array: np.ndarray,
             shift: int
             ) -> np.ndarray:
     '''
     Specialized form of np.roll that, by focusing on the 1D solution, is at least four times faster.
     '''
     size = len(array)
@@ -1404,15 +1397,14 @@
 
     post = np.empty(size, dtype=array.dtype)
 
     post[0:shift] = array[-shift:]
     post[shift:] = array[0:-shift]
     return post
 
-
 def roll_2d(array: np.ndarray,
             shift: int,
             axis: int
             ) -> np.ndarray:
     '''
     Specialized form of np.roll that, by focusing on the 2D solution
     '''
@@ -1469,19 +1461,17 @@
         if not skipna:
             return np.nan
         # always use skipna ufunc if any NaNs are present, as otherwise the wrong indices are returned when a nan is encountered (rather than a nan)
         return ufunc_skipna(array)
 
     return ufunc(array)
 
-
 argmin_1d = partial(_argminmax_1d, ufunc=np.argmin, ufunc_skipna=np.nanargmin)
 argmax_1d = partial(_argminmax_1d, ufunc=np.argmax, ufunc_skipna=np.nanargmax)
 
-
 def _argminmax_2d(
         array: np.ndarray,
         ufunc: UFunc,
         ufunc_skipna: UFunc,
         skipna: bool = True,
         axis: int = 0
         ) -> np.ndarray: # int or float array
@@ -1508,15 +1498,14 @@
 
 argmin_2d = partial(_argminmax_2d, ufunc=np.argmin, ufunc_skipna=np.nanargmin)
 argmax_2d = partial(_argminmax_2d, ufunc=np.argmax, ufunc_skipna=np.nanargmax)
 
 #-------------------------------------------------------------------------------
 # array constructors
 
-
 def is_gen_copy_values(values: tp.Iterable[tp.Any]) -> tp.Tuple[bool, bool]:
     '''
     Returns:
         copy_values: True if values cannot be used in an np.array constructor.
     '''
     is_gen = not hasattr(values, '__len__')
     copy_values = is_gen
@@ -1524,15 +1513,14 @@
         is_dictlike = isinstance(values, DICTLIKE_TYPES)
         copy_values |= is_dictlike
         if not is_dictlike:
             is_iifa = isinstance(values, INVALID_ITERABLE_FOR_ARRAY)
             copy_values |= is_iifa
     return is_gen, copy_values
 
-
 def prepare_iter_for_array(
         values: tp.Iterable[tp.Any],
         restrict_copy: bool = False
         ) -> tp.Tuple[DtypeSpecifier, bool, tp.Sequence[tp.Any]]:
     '''
     Determine an appropriate DtypeSpecifier for values in an iterable. This does not try to determine the actual dtype, but instead, if the DtypeSpecifier needs to be object rather than None (which lets NumPy auto detect). This is expected to only operate on 1D data.
 
@@ -1599,15 +1587,14 @@
 
     if copy_values:
         # v_iter is an iter, we need to finish it
         values_post.extend(v_iter)
         return resolved, has_tuple, values_post
     return resolved, has_tuple, values #type: ignore
 
-
 def iterable_to_array_1d(
         values: tp.Iterable[tp.Any],
         dtype: DtypeSpecifier = None,
         count: tp.Optional[int] = None,
         ) -> tp.Tuple[np.ndarray, bool]:
     '''
     Convert an arbitrary Python iterable to a 1D NumPy array without any undesirable type coercion.
@@ -1703,15 +1690,14 @@
     else:
         # if dtype was None, we might have discovered this was object but has no tuples; faster to do this constructor instead of null slice assignment
         v = np.array(values_for_construct, dtype=dtype)
 
     v.flags.writeable = False
     return v, is_unique
 
-
 def iterable_to_array_2d(
         values: tp.Iterable[tp.Iterable[tp.Any]],
         ) -> np.ndarray:
     '''
     Convert an arbitrary Python iterable of iterables to a 2D NumPy array without any undesirable type coercion. Useful IndexHierarchy construction.
 
     Returns:
@@ -1826,15 +1812,14 @@
                 raise LocInvalid(f'Invalid loc: {key}')
         except TypeError as e: # if stop is not an int
             raise LocInvalid(f'Invalid loc: {key}') from e
 
         stop = key.stop + 1
     return slice(start, stop, key.step)
 
-
 def key_to_str(key: GetItemKeyType) -> str:
     if key.__class__ is not slice:
         return str(key)
     if key == NULL_SLICE:
         return ':'
 
     result = ':' if key.start is None else f'{key.start}:' # type: ignore [union-attr]
@@ -1919,25 +1904,23 @@
 def to_timedelta64(value: datetime.timedelta) -> np.timedelta64:
     '''
     Convert a datetime.timedelta into a NumPy timedelta64. This approach is better than using np.timedelta64(value), as that reduces all values to microseconds.
     '''
     return reduce(operator.add,
         (np.timedelta64(getattr(value, attr), code) for attr, code in TIME_DELTA_ATTR_MAP if getattr(value, attr) > 0))
 
-
 def datetime64_not_aligned(array: np.ndarray, other: np.ndarray) -> bool:
     '''Return True if both arrays are dt64 and they are not aligned by unit. Used in property tests that must skip this condition.
     '''
     array_is_dt64 = array.dtype.kind == DTYPE_DATETIME_KIND
     other_is_dt64 = other.dtype.kind == DTYPE_DATETIME_KIND
     if array_is_dt64 and other_is_dt64:
         return np.datetime_data(array.dtype)[0] != np.datetime_data(other.dtype)[0] #type: ignore
     return False
 
-
 def _slice_to_datetime_slice_args(key: slice,
         dtype: tp.Optional[np.dtype] = None
         ) -> tp.Iterator[tp.Optional[np.datetime64]]:
     '''
     Given a slice representing a datetime region, convert to arguments for a new slice, possibly using the appropriate dtype for conversion.
     '''
     for attr in SLICE_ATTRS:
@@ -2003,15 +1986,14 @@
     Args:
         unique_axis: only used if ndim > 1
     '''
     if array.ndim == 1:
         return ufunc_unique1d_indexer(array)
     return ufunc_unique2d_indexer(array, axis=unique_axis)
 
-
 # def isna_element(value: tp.Any) -> bool:
 #     '''Return Boolean if value is an NA. This does not yet handle pd.NA
 #     '''
 #     try:
 #         return np.isnan(value) #type: ignore
 #     except TypeError:
 #         pass
@@ -2050,15 +2032,14 @@
     # no other option than to do elementwise evaluation
     return np.fromiter(
             (isna_element(e, include_none) for e in array),
             dtype=DTYPE_BOOL,
             count=len(array),
             )
 
-
 def isfalsy_array(array: np.ndarray) -> np.ndarray:
     '''
     Return a Boolean array indicating the presence of Falsy or NA values.
 
     Args:
         array: 1D or 2D array.
     '''
@@ -2268,15 +2249,14 @@
         is_dupe[list(dupe_to_last.values())] = False
 
     if not exclude_first: # add in first values
         is_dupe[list(dupe_to_first.values())] = True
 
     return is_dupe
 
-
 def _array_to_duplicated_sortable(
         array: np.ndarray,
         axis: int = 0,
         exclude_first: bool = False,
         exclude_last: bool = False) -> np.ndarray:
     '''
     Algorithm for finding duplicates in sortable arrays. This may or may not be an object array, as some object arrays (those of compatible types) are sortable.
@@ -2336,16 +2316,14 @@
             # all non-first, non-last duplicates is the intersection.
             dupes = f_flags & l_flags
 
     # undo the sort: get the indices to extract Booleans from dupes; in some cases r_idx is the same as o_idx, but not all
     r_idx = np.argsort(o_idx, axis=None, kind=DEFAULT_STABLE_SORT_KIND)
     return dupes[r_idx]
 
-
-
 def array_to_duplicated(
         array: np.ndarray,
         axis: int = 0,
         exclude_first: bool = False,
         exclude_last: bool = False,
         ) -> np.ndarray:
     '''Given a numpy array (1D or 2D), return a Boolean array along the specified axis that shows which values are duplicated. By default, all duplicates are indicated. For 2d arrays, axis 0 compares rows and returns a row-length Boolean array; axis 1 compares columns and returns a column-length Boolean array.
@@ -2365,16 +2343,16 @@
         return _array_to_duplicated_hashable(
                 array=array,
                 axis=axis,
                 exclude_first=exclude_first,
                 exclude_last=exclude_last
                 )
 
-
 #-------------------------------------------------------------------------------
+
 def array_shift(*,
         array: np.ndarray,
         shift: int,
         axis: int, # 0 is rows, 1 is columns
         wrap: bool,
         fill_value: tp.Any = np.nan) -> np.ndarray:
     '''
@@ -2799,15 +2777,14 @@
     Difference on 2D array, handling diverse types and short-circuiting to preserve order where appropriate.
     '''
     return _ufunc_set_2d(np.setdiff1d,
         array,
         other,
         assume_unique=assume_unique)
 
-
 MANY_TO_ONE_MAP = {
         (1, ManyToOneType.UNION): union1d,
         (1, ManyToOneType.INTERSECT): intersect1d,
         (1, ManyToOneType.DIFFERENCE): setdiff1d,
         (2, ManyToOneType.UNION): union2d,
         (2, ManyToOneType.INTERSECT): intersect2d,
         (2, ManyToOneType.DIFFERENCE): setdiff2d,
@@ -2853,15 +2830,14 @@
                     or many_to_one_type is ManyToOneType.DIFFERENCE):
                 # short circuit for ops with no common values
                 break
 
     result.flags.writeable = False
     return result
 
-
 def _isin_1d(
         array: np.ndarray,
         other: tp.FrozenSet[tp.Any]
         ) -> np.ndarray:
     '''
     Iterate over an 1D array to build a 1D Boolean ndarray representing whether or not the original element is in the set
 
@@ -2873,15 +2849,14 @@
 
     for i, element in enumerate(array):
         result[i] = element in other
 
     result.flags.writeable = False
     return result
 
-
 def _isin_2d(
         array: np.ndarray,
         other: tp.FrozenSet[tp.Any]
         ) -> np.ndarray:
     '''
     Iterate over an 2D array to build a 2D, immutable, Boolean ndarray representing whether or not the original element is in the set
 
@@ -2893,15 +2868,14 @@
 
     for (i, j), v in np.ndenumerate(array):
         result[i, j] = v in other
 
     result.flags.writeable = False
     return result
 
-
 def isin_array(*,
         array: np.ndarray,
         array_is_unique: bool,
         other: np.ndarray,
         other_is_unique: bool,
         ) -> np.ndarray:
     '''Core isin processing after other has been converted to an array.
@@ -2921,15 +2895,14 @@
         # FutureWarning: elementwise comparison failed;
         result = func(array, other, assume_unique=assume_unique) #type: ignore
 
     result.flags.writeable = False
 
     return result
 
-
 def isin(
         array: np.ndarray,
         other: tp.Iterable[tp.Any],
         array_is_unique: bool = False,
         ) -> np.ndarray:
     '''
     Builds a same-size, immutable, Boolean ndarray representing whether or not the original element is in another ndarray
@@ -2954,14 +2927,15 @@
     return isin_array(array=array,
             array_is_unique=array_is_unique,
             other=other,
             other_is_unique=other_is_unique,
             )
 
 #-------------------------------------------------------------------------------
+
 def _ufunc_logical_skipna(
         array: np.ndarray,
         ufunc: AnyCallable,
         skipna: bool,
         axis: int = 0,
         out: tp.Optional[np.ndarray] = None
         ) -> np.ndarray:
@@ -3018,15 +2992,14 @@
     # all other types assume truthy
     # if kind in DTYPE_NAT_KINDS: # all dates are truthy, NAT is truthy
 
     if array.ndim == 1:
         return True
     return np.full(array.shape[0 if axis else 1], fill_value=True, dtype=bool)
 
-
 def ufunc_all(array: np.ndarray,
         axis: int = 0,
         out: tp.Optional[np.ndarray] = None
         ) -> np.ndarray:
     return _ufunc_logical_skipna(array,
             ufunc=np.all,
             skipna=False,
@@ -3112,15 +3085,14 @@
             post[iloc] = func(e)
     else: # a string kind that is unsized
         post = np.array([func(e) for e in np.ravel(array)], dtype=dtype).reshape(array.shape)
 
     post.flags.writeable = False
     return post
 
-
 def array_from_element_method(*,
         array: np.ndarray,
         method_name: str,
         args: tp.Tuple[tp.Any, ...],
         dtype: np.dtype,
         pre_insert: tp.Optional[AnyCallable] = None,
         ) -> np.array:
@@ -3272,15 +3244,14 @@
 
     if seed is not None:
         np.random.set_state(state)
 
     post.flags.writeable = False
     return post
 
-
 def run_length_1d(array: np.ndarray) -> tp.Tuple[np.ndarray, np.ndarray]:
     '''Given an array of values, discover contiguous values and their length.
 
     Return:
         np.ndarray: a value per contiguous width
         np.ndarray: a width per contiguous value
     '''
@@ -3303,17 +3274,14 @@
     # use the difference in positions to get widths; we need the width from the last transition to the full length in the last position
     widths = np.empty(len(idx), dtype=DTYPE_INT_DEFAULT)
     widths[-1] = size - idx[-1]
     widths[:-1] = (idx - np.roll(idx, 1))[1:]
 
     return array[transitions], widths
 
-
-
-
 #-------------------------------------------------------------------------------
 # json utils
 
 class JSONFilter:
     '''Note: this is filter for encoding NumPy arrays and Python objects in generally readible format by naive consumers. Thus all dates are represented as date strings. This differs from using `__repr__` and attempting to reanimate Python types.
     '''
 
@@ -3371,24 +3339,26 @@
 class Reanimate:
     RE: tp.Pattern[str]
 
     @classmethod
     def filter(cls, value: str) -> tp.Any:
         raise NotImplementedError() #pragma: no cover
 
+
 class ReanimateDT64(Reanimate):
     RE = re.compile(r"numpy.datetime64\('([-.T:0-9]+)'\)")
 
     @classmethod
     def filter(cls, value: str) -> tp.Any:
         post = cls.RE.fullmatch(value)
         if post is None:
             return value
         return np.datetime64(post.group(1))
 
+
 class ReanimateDTD(Reanimate):
     RE = re.compile(r"datetime.date\(([ ,0-9]+)\)")
 
     @classmethod
     def filter(cls, value: str) -> tp.Any:
         post = cls.RE.fullmatch(value)
         if post is None:
@@ -3513,16 +3483,14 @@
                     else:
                         target_slice = slice(
                                 (target_slice.start or 0) + shift,
                                 target_slice.stop)
 
             yield target_slice, value
 
-
-
 #-------------------------------------------------------------------------------
 # URL handling, file downloading, file writing
 
 def path_filter(fp: PathSpecifierOrFileLikeOrIterator) -> tp.Union[str, tp.TextIO]:
     '''Realize Path objects as strings, let TextIO pass through, if given.
     '''
     if fp is None:
@@ -3556,15 +3524,14 @@
             if fd is not None:
                 os.close(fd)
     else: # string IO
         f.write(content)
         f.seek(0)
     return fp #type: ignore
 
-
 @contextlib.contextmanager
 def file_like_manager(
         file_like: PathSpecifierOrFileLikeOrIterator,
         encoding: tp.Optional[str] = None,
         mode: str = 'r',
         ) -> tp.Iterator[tp.Iterator[str]]:
     '''
@@ -3597,24 +3564,22 @@
     # this will raise if attrs are invalid
     try:
         return namedtuple('Axis', fields)._make #type: ignore
     except ValueError:
         pass
     raise ValueError('invalid fields for namedtuple; pass `tuple` as constructor')
 
-
 def key_normalize(key: KeyOrKeys) -> tp.List[tp.Hashable]:
     '''
     Normalizing a key that might be a single element or an iterable of keys; expected return is always a list, as it will be used for getitem selection.
     '''
     if isinstance(key, str) or not hasattr(key, '__len__'):
         return [key] # type: ignore
     return key if isinstance(key, list) else list(key) # type: ignore
 
-
 def iloc_to_insertion_iloc(key: int, size: int) -> int:
     '''
     Given an iloc (possibly bipolar), return the appropriate insertion iloc (always positive)
     '''
     if key < -size or key >= size:
         raise IndexError(f'index {key} out of range for length {size} container.')
     return key % size
```

### Comparing `static-frame-1.4.1/static_frame/core/www.py` & `static-frame-1.4.2/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/core/yarn.py` & `static-frame-1.4.2/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/test_case.py` & `static-frame-1.4.2/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.4.2/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_axis_map.py` & `static-frame-1.4.2/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_batch.py` & `static-frame-1.4.2/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_bus.py` & `static-frame-1.4.2/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_container.py` & `static-frame-1.4.2/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_container_util.py` & `static-frame-1.4.2/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_display.py` & `static-frame-1.4.2/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_display_color.py` & `static-frame-1.4.2/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_doc.py` & `static-frame-1.4.2/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.4.2/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_frame.py` & `static-frame-1.4.2/static_frame/test/unit/test_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1919,14 +1919,24 @@
             f1['a'] = gen1()
         except ValueError:
             pass
 
         self.assertEqual(f1.shape, (3, 3))
         self.assertEqual(len(f1.columns), 3)
 
+
+    def test_frame_setitem_l1(self) -> None:
+        f = sf.FrameGO(index=range(3))
+        f['a'] = f.index
+        self.assertEqual(f.to_pairs(), (('a', ((0, 0), (1, 1), (2, 2))),))
+
+        with self.assertRaises(RuntimeError):
+            f['b'] = sf.Series(['a', 'b']).index
+
+
     def test_frame_setitem_m(self) -> None:
         f1 = sf.FrameGO.from_records(np.arange(9).reshape(3,3))
 
         def gen1(v: bool) -> tp.Iterator[int]:
             if v:
                 raise ValueError('gen1')
             yield 1
@@ -10037,15 +10047,15 @@
         {
         "userId": 1,
         "id": 4,
         "title": "et porro tempora",
         "completed": true
         }]'''
 
-        f1 = Frame.from_json(msg, name=msg)
+        f1 = Frame.from_json_records(msg, name=msg)
         self.assertEqual(sorted(f1.columns.values.tolist()),
                 sorted(['completed', 'id', 'title', 'userId']))
         self.assertEqual(f1['id'].sum(), 10)
 
         self.assertEqual(f1.name, msg)
 
     #---------------------------------------------------------------------------
```

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_frame_he.py` & `static-frame-1.4.2/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.4.2/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_frame_join.py` & `static-frame-1.4.2/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.4.2/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.4.2/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_hloc.py` & `static-frame-1.4.2/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index.py` & `static-frame-1.4.2/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index_auto.py` & `static-frame-1.4.2/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index_base.py` & `static-frame-1.4.2/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.4.2/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.4.2/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_interface.py` & `static-frame-1.4.2/static_frame/test/unit/test_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def test_interface_summary_b(self) -> None:
 
         post = FrameGO.interface
         counts = post.iter_group('group').apply(len)
 
         self.assertEqual(
             counts.to_pairs(),
-            (('Accessor Datetime', 22), ('Accessor Fill Value', 26), ('Accessor Hashlib', 10), ('Accessor Regular Expression', 7), ('Accessor String', 39), ('Accessor Transpose', 24), ('Accessor Values', 3), ('Assignment', 16), ('Attribute', 12), ('Constructor', 40), ('Dictionary-Like', 7), ('Display', 6), ('Exporter', 31), ('Iterator', 156), ('Method', 102), ('Operator Binary', 24), ('Operator Unary', 4), ('Selector', 13))
+            (('Accessor Datetime', 22), ('Accessor Fill Value', 26), ('Accessor Hashlib', 10), ('Accessor Regular Expression', 7), ('Accessor String', 39), ('Accessor Transpose', 24), ('Accessor Values', 3), ('Assignment', 16), ('Attribute', 12), ('Constructor', 38), ('Dictionary-Like', 7), ('Display', 6), ('Exporter', 31), ('Iterator', 156), ('Method', 102), ('Operator Binary', 24), ('Operator Unary', 4), ('Selector', 13))
             )
 
     def test_interface_summary_c(self) -> None:
         s = Series(['a', 'b', 'c'])
         post = s.interface
 
         counts = post.iter_group('group').apply(len)
```

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_loc_map.py` & `static-frame-1.4.2/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.4.2/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.4.2/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_pivot.py` & `static-frame-1.4.2/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.4.2/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_quilt.py` & `static-frame-1.4.2/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_rank.py` & `static-frame-1.4.2/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_series.py` & `static-frame-1.4.2/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_series_he.py` & `static-frame-1.4.2/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_store.py` & `static-frame-1.4.2/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_store_filter.py` & `static-frame-1.4.2/static_frame/test/unit/test_store_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,22 @@
                 sf1._format_inexact_element('foo', DTYPE_OBJECT_KIND),
                 'foo'
                 )
 
     def test_store_filter_format_inexact_element_c(self) -> None:
         sf1 = StoreFilter(
                 value_format_float_positional='{:.8f}',
-                value_format_float_scientific='{:.8f}')
+                value_format_float_scientific='{:.8f}',
+                # Use non-frozensets to test that they are converted
+                to_nan=('', 'nan', 'NaN', 'NAN', 'NULL', '#N/A'),
+                to_nat=(),
+                to_none=('None',),
+                to_posinf=('inf',),
+                to_neginf=('-inf',),
+                )
 
         self.assertEqual(
                 sf1._format_inexact_element(0.83255500, DTYPE_FLOAT_KIND),
                 '0.83255500'
                 )
         self.assertEqual(
                 sf1._format_inexact_element(0.0000011193, DTYPE_OBJECT_KIND),
```

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.4.2/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.4.2/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.4.2/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_store_zip.py` & `static-frame-1.4.2/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_style_config.py` & `static-frame-1.4.2/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.4.2/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_util.py` & `static-frame-1.4.2/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_www.py` & `static-frame-1.4.2/static_frame/test/unit/test_www.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,13 +286,13 @@
         "userId": 1,
         "id": 2,
         "title": "quis ut nam facilis et officia qui",
         "completed": false
         }]'''
         with patch('urllib.request.urlopen') as mock:
             prepare_mock(mock, content)
-            post = Frame.from_json_url(url=URL)
+            post = Frame.from_json_records(WWW.from_file(url=URL))
             self.assertEqual(post.shape, (2, 4))
             self.assertEqual([dt.kind for dt in post.dtypes.values], ['i', 'i', 'U', 'b'])
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `static-frame-1.4.1/static_frame/test/unit/test_yarn.py` & `static-frame-1.4.2/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.1/static_frame.egg-info/PKG-INFO` & `static-frame-1.4.2/static_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.1
+Version: 1.4.2
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -45,15 +45,15 @@
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
-        - arraymap==0.1.7
+        - arraymap==0.1.8
         - arraykit==0.3.4
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
```

### Comparing `static-frame-1.4.1/static_frame.egg-info/SOURCES.txt` & `static-frame-1.4.2/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

