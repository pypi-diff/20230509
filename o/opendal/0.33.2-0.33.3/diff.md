# Comparing `tmp/opendal-0.33.2.tar.gz` & `tmp/opendal-0.33.3.tar.gz`

## Comparing `opendal-0.33.2.tar` & `opendal-0.33.3.tar`

### file list

```diff
@@ -1,258 +1,281 @@
--rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 opendal-0.33.2/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    66617 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6635 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10879 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     4478 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    23435 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    20940 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9888 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17355 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13556 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    51478 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13497 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    31779 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12877 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2205 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13882 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    24230 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    37745 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    12402 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3001 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    19037 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9830 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     1934 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     6512 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5578 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3394 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    11165 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2025 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11983 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1950 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     8881 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15397 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2001 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9182 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5198 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4081 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6387 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    29068 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    11623 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5870 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2079 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16278 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3519 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2736 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     4046 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    23347 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3092 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    16606 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     1900 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    19847 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    15836 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3512 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10592 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6187 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20642 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2375 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    15803 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2461 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    16169 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1875 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16861 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8716 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1834 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123    10057 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4337 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     3584 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7999 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13922 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     7436 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3492 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2057 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    21785 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    24192 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3407 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6946 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10637 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5664 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    39656 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28367 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     3734 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7387 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7530 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5518 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123     8024 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/backend.rs
--rw-r--r--   0     1001      123     5963 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/core.rs
--rw-r--r--   0     1001      123     2365 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/error.rs
--rw-r--r--   0     1001      123      894 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/mod.rs
--rw-r--r--   0     1001      123     2382 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/supabase/writer.rs
--rw-r--r--   0     1001      123    39009 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29663 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3711 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2666 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20511 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2066 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19374 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2076 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     3368 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6381 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12002 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    16557 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1511 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    24145 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3067 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    42718 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123    10788 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9569 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     6030 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    10696 2023-04-27 13:47:39.000000 opendal-0.33.2/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.2/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-04-27 13:47:39.000000 opendal-0.33.2/.gitignore
--rw-r--r--   0     1001      123      982 2023-04-27 13:47:39.000000 opendal-0.33.2/README.md
--rw-r--r--   0     1001      123      765 2023-04-27 13:47:39.000000 opendal-0.33.2/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-04-27 13:47:39.000000 opendal-0.33.2/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-04-27 13:47:39.000000 opendal-0.33.2/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-04-27 13:47:39.000000 opendal-0.33.2/examples/object.ipynb
--rw-r--r--   0     1001      123     1665 2023-04-27 13:47:39.000000 opendal-0.33.2/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-04-27 13:47:39.000000 opendal-0.33.2/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-04-27 13:47:39.000000 opendal-0.33.2/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-04-27 13:47:39.000000 opendal-0.33.2/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-04-27 13:47:39.000000 opendal-0.33.2/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-04-27 13:47:39.000000 opendal-0.33.2/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-04-27 13:47:39.000000 opendal-0.33.2/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-04-27 13:47:39.000000 opendal-0.33.2/tests/steps/binding.py
--rw-r--r--   0     1001      123   117461 2023-04-27 13:47:39.000000 opendal-0.33.2/Cargo.lock
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.33.2/PKG-INFO
+-rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 opendal-0.33.3/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    68810 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1114 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6804 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10879 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     2687 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
+-rw-r--r--   0     1001      123     4554 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    23435 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    20940 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9888 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17355 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13556 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    52134 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13497 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    31779 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12877 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2205 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13882 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    24230 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    37745 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    12402 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3001 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    19226 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9870 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     5971 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5424 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2159 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123    21679 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/multipart.rs
+-rw-r--r--   0     1001      123     2962 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11983 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1950 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     8881 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15397 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2001 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9182 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5198 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4081 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    28916 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123     5544 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    11328 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5870 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2079 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16366 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3519 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2736 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4046 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    23435 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3092 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    16707 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     1900 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    19770 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    15835 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3512 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6187 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123     8028 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gdrive/backend.rs
+-rw-r--r--   0     1001      123     4255 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gdrive/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gdrive/error.rs
+-rw-r--r--   0     1001      123      894 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gdrive/mod.rs
+-rw-r--r--   0     1001      123     1975 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/gdrive/writer.rs
+-rw-r--r--   0     1001      123    20682 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2375 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    15893 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2461 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16208 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1875 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16949 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8931 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1753 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     5712 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9165 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4337 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     4064 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7999 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13852 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     7436 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3492 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2057 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123     6524 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/onedrive/backend.rs
+-rw-r--r--   0     1001      123     4373 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/onedrive/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/onedrive/error.rs
+-rw-r--r--   0     1001      123      898 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/onedrive/mod.rs
+-rw-r--r--   0     1001      123     2189 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/onedrive/writer.rs
+-rw-r--r--   0     1001      123    21715 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    24192 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3407 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6946 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10637 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5664 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39942 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28367 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     4749 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7530 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123    14389 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sftp/backend.rs
+-rw-r--r--   0     1001      123     2894 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sftp/error.rs
+-rw-r--r--   0     1001      123      899 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sftp/mod.rs
+-rw-r--r--   0     1001      123     2700 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sftp/pager.rs
+-rw-r--r--   0     1001      123     3384 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sftp/utils.rs
+-rw-r--r--   0     1001      123     1677 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sftp/writer.rs
+-rw-r--r--   0     1001      123     5518 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     9690 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     8021 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2582 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2382 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123     4722 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
+-rw-r--r--   0     1001      123     3583 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
+-rw-r--r--   0     1001      123      912 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
+-rw-r--r--   0     1001      123     2055 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
+-rw-r--r--   0     1001      123    38936 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29663 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3711 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2666 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20653 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2066 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19508 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2076 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     3368 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6574 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12002 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    16557 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1511 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    24145 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3067 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    42775 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123    11354 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9569 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     6584 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    10696 2023-05-09 07:31:45.000000 opendal-0.33.3/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.33.3/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-05-09 07:31:45.000000 opendal-0.33.3/.gitignore
+-rw-r--r--   0     1001      123     2212 2023-05-09 07:31:45.000000 opendal-0.33.3/CONTRIBUTING.md
+-rw-r--r--   0     1001      123      982 2023-05-09 07:31:45.000000 opendal-0.33.3/README.md
+-rw-r--r--   0     1001      123      765 2023-05-09 07:31:45.000000 opendal-0.33.3/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-05-09 07:31:45.000000 opendal-0.33.3/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-05-09 07:31:45.000000 opendal-0.33.3/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-05-09 07:31:45.000000 opendal-0.33.3/examples/object.ipynb
+-rw-r--r--   0     1001      123     1665 2023-05-09 07:31:45.000000 opendal-0.33.3/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-05-09 07:31:45.000000 opendal-0.33.3/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-05-09 07:31:45.000000 opendal-0.33.3/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-05-09 07:31:45.000000 opendal-0.33.3/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-05-09 07:31:45.000000 opendal-0.33.3/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-05-09 07:31:45.000000 opendal-0.33.3/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-05-09 07:31:45.000000 opendal-0.33.3/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-05-09 07:31:45.000000 opendal-0.33.3/tests/steps/binding.py
+-rw-r--r--   0     1001      123   127590 2023-05-09 07:31:45.000000 opendal-0.33.3/Cargo.lock
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 opendal-0.33.3/PKG-INFO
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/Cargo.toml` & `opendal-0.33.3/local_dependencies/opendal/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.33.2"
+version= "0.33.3"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -104,41 +104,50 @@
 services-fs = ["tokio/fs"]
 services-ftp = ["dep:suppaftp", "dep:lazy-regex", "dep:bb8", "dep:async-tls"]
 services-gcs = [
   "dep:reqsign",
   "reqsign?/services-google",
   "reqsign?/reqwest_request",
 ]
+services-gdrive = []
 services-ghac = []
 services-hdfs = ["dep:hdrs"]
 services-http = []
 services-ipfs = ["dep:prost"]
 services-ipmfs = []
 services-memcached = ["dep:bb8"]
 services-memory = []
 services-moka = ["dep:moka"]
 services-obs = [
   "dep:reqsign",
   "reqsign?/services-huaweicloud",
   "reqsign?/reqwest_request",
 ]
+services-onedrive = []
 services-oss = [
   "dep:reqsign",
   "reqsign?/services-aliyun",
   "reqsign?/reqwest_request",
 ]
 services-redis = ["dep:redis"]
 services-rocksdb = ["dep:rocksdb"]
 services-s3 = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
+services-sftp = [
+  "dep:openssh",
+  "dep:openssh-sftp-client",
+  "dep:bb8",
+  "dep:owning_ref",
+]
 services-sled = ["dep:sled"]
 services-supabase = []
+services-vercel-artifacts = []
 services-wasabi = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-webdav = []
 services-webhdfs = []
@@ -170,35 +179,55 @@
 log = "0.4"
 madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
 minitrace = { version = "0.4.0", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
+openssh = { version = "0.9.9", optional = true }
+openssh-sftp-client = { version = "0.12.2", optional = true }
 opentelemetry = { version = "0.19.0", optional = true }
+owning_ref = { version = "0.4.1", optional = true }
 parking_lot = "0.12"
 percent-encoding = "2"
 pin-project = "1"
 prometheus = { version = "0.13", features = ["process"], optional = true }
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redis = { version = "0.22", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
 reqsign = { version = "0.9.1", default-features = false, optional = true }
 reqwest = { version = "0.11.13", features = [
-  "multipart",
   "stream",
 ], default-features = false }
 rocksdb = { version = "0.20.1", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
 sled = { version = "0.34.7", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
 tokio = "1.27"
 tracing = { version = "0.1", optional = true }
 uuid = { version = "1", features = ["serde", "v4"] }
+
+[dev-dependencies]
+criterion = { version = "0.4", features = ["async", "async_tokio"] }
+dotenvy = "0.15"
+env_logger = "0.10"
+opentelemetry = { version = "0.19", default-features = false, features = [
+  "trace",
+] }
+opentelemetry-jaeger = "0.18"
+paste = "1"
+pretty_assertions = "1"
+rand = "0.8"
+sha2 = "0.10"
+size = "0.4"
+tokio = { version = "1.27", features = ["fs", "macros", "rt-multi-thread"] }
+tracing-opentelemetry = "0.17"
+tracing-subscriber = { version = "0.3", features = ["env-filter"] }
+wiremock = "0.5"
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.33.3/local_dependencies/opendal/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,69 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.33.3] - 2023-05-06
+
+### Added
+
+- feat(services/onedrive): Add read and write support for OneDrive (#2129)
+- test(core): test for `read_with_override_cache_control` (#2155)
+- feat(http_util): Implement multipart/form-data support (#2157)
+- feat(http_util): Implement multipart/mixed support (#2161)
+- RFC-2133: Introduce Append API (#2133)
+- feat(services/sftp): Add read/write/stat support for sftp (#2186)
+- feat(services/gdrive): Add read & write & delete support for GoogleDrive (#2184)
+- feat(services/vercel): Add vercel remote cache support (#2193)
+- feat(tests): Enable supabase integration tests (#2190)
+- feat(core): merge scan and list (#2214)
+
+### Changed
+
+- refactor(java): refactor java code for java binding (#2145)
+- refactor(layers/logging): parsing level str (#2160)
+- refactor: Move not initiated logic to utils instead (#2196)
+- refactor(services/memcached): Rewrite memecached connection entirely (#2204)
+
+### Fixed
+
+- fix(service/s3): set retryable on batch (#2171)
+- fix(services/supabase): Supabase ci fix (#2200)
+
+### Docs
+
+- docs(website): try to add opendal logo (#2159)
+- doc: update vision to be more clear (#2164)
+- docs: Refactor `Contributing` and add `Developing` (#2169)
+- docs: Merge DEVELOPING into CONTRIBUTING (#2172)
+- docs: fix some grammar errors in the doc of Operator (#2173)
+- docs(nodejs): Add CONTRIBUTING docs (#2174)
+- docs: Add CONTRIBUTING for python (#2188)
+
+### CI
+
+- ci: Use microsoft rust devcontainer instead (#2165)
+- ci(devcontainer): Install development deps (#2167)
+- chore: set workspace default members (#2168)
+- ci: Setup vercel artifacts integration tests (#2197)
+- ci: Remove not used odev tools (#2202)
+- ci: Add tools to generate NOTICE and all deps licenses (#2205)
+- ci: use Temurin JDK 11 to build the bindings-java (#2213)
+
+### Chore
+
+- chore(deps): bump clap from 4.1.11 to 4.2.5 (#2183)
+- chore(deps): bump futures from 0.3.27 to 0.3.28 (#2181)
+- chore(deps): bump assert_cmd from 2.0.10 to 2.0.11 (#2180)
+- chore: Refactor behavior test (#2189)
+- chore: update readme for more information that is more friendly to newcomers (#2217)
+
 ## [v0.33.2] - 2023-04-27
 
 ### Added
 
 - feat(core): add test for `stat_with_if_none_match` (#2122)
 - feat(services/gcs): Add start-after support for list (#2107)
 - feat(services/azblob): Add supporting presign (#2120)
@@ -2008,14 +2063,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.33.3]: https://github.com/apache/incubator-opendal/compare/v0.33.2...v0.33.3
 [v0.33.2]: https://github.com/apache/incubator-opendal/compare/v0.33.1...v0.33.2
 [v0.33.1]: https://github.com/apache/incubator-opendal/compare/v0.33.0...v0.33.1
 [v0.33.0]: https://github.com/apache/incubator-opendal/compare/v0.32.0...v0.33.0
 [v0.32.0]: https://github.com/apache/incubator-opendal/compare/v0.31.1...v0.32.0
 [v0.31.1]: https://github.com/apache/incubator-opendal/compare/v0.31.0...v0.31.1
 [v0.31.0]: https://github.com/apache/incubator-opendal/compare/v0.30.5...v0.31.0
 [v0.30.5]: https://github.com/apache/incubator-opendal/compare/v0.30.4...v0.30.5
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.33.3/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # Contributing
 
 ## Get Started
 
-This is a Rust project, so [rustup](https://rustup.rs/) is the best place to start.
-
-This is a pure rust project, so only `cargo` is needed.
-
 - `cargo check` to analyze the current package and report errors.
 - `cargo build` to compile the current package.
 - `cargo clippy` to catch common mistakes and improve code.
 - `cargo test` to run unit tests.
 - `cargo bench` to run benchmark tests.
 
 Useful tips:
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/README.md` & `opendal-0.33.3/local_dependencies/opendal/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 - [memory](https://docs.rs/opendal/latest/opendal/services/struct.Memory.html): In memory backend.
 - [moka](https://docs.rs/opendal/latest/opendal/services/struct.Moka.html): [moka](https://github.com/moka-rs/moka) backend support.
 - [obs](https://docs.rs/opendal/latest/opendal/services/struct.Obs.html): [Huawei Cloud Object Storage](https://www.huaweicloud.com/intl/en-us/product/obs.html) Service (OBS).
 - [oss](https://docs.rs/opendal/latest/opendal/services/struct.Oss.html): [Aliyun Object Storage Service](https://www.aliyun.com/product/oss) (OSS).
 - [redis](https://docs.rs/opendal/latest/opendal/services/struct.Redis.html): [Redis](https://redis.io/) services support.
 - [rocksdb](https://docs.rs/opendal/latest/opendal/services/struct.Rocksdb.html): [RocksDB](http://rocksdb.org/) services support.
 - [s3](https://docs.rs/opendal/latest/opendal/services/struct.S3.html): [AWS S3](https://aws.amazon.com/s3/) alike services.
+- [sftp](https://docs.rs/opendal/latest/opendal/services/struct.Sftp.html): [SFTP](https://datatracker.ietf.org/doc/html/draft-ietf-secsh-filexfer-02) services support.
 - [sled](https://docs.rs/opendal/latest/opendal/services/sled/struct.Sled.html): [sled](https://crates.io/crates/sled) services support.
 - [webdav](https://docs.rs/opendal/latest/opendal/services/struct.Webdav.html): [WebDAV](https://datatracker.ietf.org/doc/html/rfc4918) Service Support.
 - [webhdfs](https://docs.rs/opendal/latest/opendal/services/struct.Webhdfs.html): [WebHDFS](https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/WebHDFS.html) Service Support.
 
 ## Features
 
 Access data **freely**
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.33.3/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.33.3/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.33.3/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.33.3/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.33.3/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/examples/object.rs` & `opendal-0.33.3/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/features.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -132,7 +132,10 @@
 pub mod rfc_1477_remove_object_concept {}
 
 #[doc = include_str!("1735_operation_extension.md")]
 pub mod rfc_1735_operation_extension {}
 
 #[doc = include_str!("2083_writer_sink_api.md")]
 pub mod rfc_2083_writer_sink_api {}
+
+#[doc = include_str!("2133_append_api.md")]
+pub mod rfc_2133_append_api {}
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.33.3/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/complete.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 2% similar despite different names*

```diff
@@ -101,27 +101,43 @@
 
 impl LoggingLayer {
     /// Setting the log level while expected error happened.
     ///
     /// For example: accessor returns NotFound.
     ///
     /// `None` means disable the log for error.
-    pub fn with_error_level(mut self, level: Option<Level>) -> Self {
-        self.error_level = level;
-        self
+    pub fn with_error_level(mut self, level: Option<&str>) -> Result<Self> {
+        if let Some(level_str) = level {
+            let level = level_str.parse().map_err(|_| {
+                Error::new(ErrorKind::ConfigInvalid, "invalid log level")
+                    .with_context("level", level_str)
+            })?;
+            self.error_level = Some(level);
+        } else {
+            self.error_level = None;
+        }
+        Ok(self)
     }
 
     /// Setting the log level while unexpected failure happened.
     ///
     /// For example: accessor returns Unexpected network error.
     ///
     /// `None` means disable the log for failure.
-    pub fn with_failure_level(mut self, level: Option<Level>) -> Self {
-        self.failure_level = level;
-        self
+    pub fn with_failure_level(mut self, level: Option<&str>) -> Result<Self> {
+        if let Some(level_str) = level {
+            let level = level_str.parse().map_err(|_| {
+                Error::new(ErrorKind::ConfigInvalid, "invalid log level")
+                    .with_context("level", level_str)
+            })?;
+            self.failure_level = Some(level);
+        } else {
+            self.failure_level = None;
+        }
+        Ok(self)
     }
 }
 
 impl<A: Accessor> Layer<A> for LoggingLayer {
     type LayeredAccessor = LoggingAccessor<A>;
 
     fn layer(&self, inner: A) -> Self::LayeredAccessor {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/retry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.33.3/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/lib.rs` & `opendal-0.33.3/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -219,20 +219,24 @@
         ))
     }
 
     /// Invoke the `scan` operation on the specified path.
     ///
     /// Require [`Capability::scan`]
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        let (_, _) = (path, args);
+        let mut op_list = OpList::new().with_delimiter("");
+        if let Some(limit) = args.limit() {
+            op_list = op_list.with_limit(limit)
+        }
+        let result = self.list(path, op_list).await;
 
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "operation is not supported",
-        ))
+        return match result {
+            Ok(r) => Ok((RpScan::default(), r.1)),
+            Err(e) => Err(e),
+        };
     }
 
     /// Invoke the `presign` operation on the specified path.
     ///
     /// Require [`Capability::presign`]
     ///
     /// # Behavior
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         let mut am: AccessorInfo = self.kv.metadata().into();
         am.set_root(&self.root);
 
         let cap = am.capability_mut();
         if cap.read {
             cap.read_can_seek = true;
             cap.read_can_next = true;
+            cap.read_with_range = true;
             cap.stat = true;
         }
 
         if cap.write {
             cap.create_dir = true;
             cap.delete = true;
         }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files 6% similar despite different names*

```diff
@@ -37,31 +37,14 @@
 #[derive(Default)]
 pub enum AsyncBody {
     /// An empty body.
     #[default]
     Empty,
     /// Body with bytes.
     Bytes(Bytes),
-    /// Body with a multipart field.
-    ///
-    /// If input with this field, we will goto the internal multipart
-    /// handle logic.
-    Multipart(String, Bytes),
-}
-
-impl From<AsyncBody> for reqwest::Body {
-    fn from(v: AsyncBody) -> Self {
-        match v {
-            AsyncBody::Empty => reqwest::Body::from(""),
-            AsyncBody::Bytes(bs) => reqwest::Body::from(bs),
-            AsyncBody::Multipart(_, _) => {
-                unreachable!("reqwest multipart should not be constructed by body")
-            }
-        }
-    }
 }
 
 type BytesStream = Box<dyn Stream<Item = Result<Bytes>> + Send + Sync + Unpin>;
 
 /// IncomingAsyncBody carries the content returned by remote servers.
 ///
 /// # Notes
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files 9% similar despite different names*

```diff
@@ -90,22 +90,17 @@
             .request(
                 parts.method,
                 Url::from_str(&url).expect("input request url must be valid"),
             )
             .version(parts.version)
             .headers(parts.headers);
 
-        req_builder = if let AsyncBody::Multipart(field, r) = body {
-            let mut form = reqwest::multipart::Form::new();
-            let part = reqwest::multipart::Part::stream(AsyncBody::Bytes(r));
-            form = form.part(field, part);
-
-            req_builder.multipart(form)
-        } else {
-            req_builder.body(body)
+        req_builder = match body {
+            AsyncBody::Empty => req_builder.body(reqwest::Body::from("")),
+            AsyncBody::Bytes(bs) => req_builder.body(reqwest::Body::from(bs)),
         };
 
         let mut resp = req_builder.send().await.map_err(|err| {
             let is_temporary = !(
                 // Builder related error should not be retried.
                 err.is_builder() ||
                 // Error returned by RedirectPolicy.
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -55,7 +55,13 @@
 pub use error::ErrorResponse;
 
 mod bytes_range;
 pub use bytes_range::BytesRange;
 
 mod bytes_content_range;
 pub use bytes_content_range::BytesContentRange;
+
+mod multipart;
+pub use multipart::FormDataPart;
+pub use multipart::MixedPart;
+pub use multipart::Multipart;
+pub use multipart::Part;
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.33.3/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -456,14 +456,15 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
@@ -471,15 +472,18 @@
                 delete: true,
                 create_dir: true,
                 list: true,
                 scan: true,
                 copy: true,
                 presign: self.has_sas_token,
                 batch: true,
+                batch_delete: true,
                 batch_max_operations: Some(AZBLOB_BATCH_LIMIT),
+
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -587,32 +591,21 @@
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         let op = AzblobPager::new(
             self.core.clone(),
             path.to_string(),
-            "/".to_string(),
+            args.delimiter().to_string(),
             args.limit(),
         );
 
         Ok((RpList::default(), op))
     }
 
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        let op = AzblobPager::new(
-            self.core.clone(),
-            path.to_string(),
-            "".to_string(),
-            args.limit(),
-        );
-
-        Ok((RpScan::default(), op))
-    }
-
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
                 self.core
                     .azblob_head_blob_request(path, v.if_none_match(), v.if_match())?
             }
             PresignOperation::Read(v) => self.core.azblob_get_blob_request(
@@ -644,14 +637,15 @@
         let paths = ops.into_iter().map(|(p, _)| p).collect::<Vec<_>>();
         if paths.len() > AZBLOB_BATCH_LIMIT {
             return Err(Error::new(
                 ErrorKind::Unsupported,
                 "batch delete limit exceeded",
             ));
         }
+
         // construct and complete batch request
         let resp = self.core.azblob_batch_delete(&paths).await?;
 
         // check response status
         if resp.status() != StatusCode::ACCEPTED {
             return Err(parse_error(resp).await?);
         }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 12% similar despite different names*

```diff
@@ -15,29 +15,26 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
-use std::str::FromStr;
 
 use http::header::HeaderName;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
-use http::Uri;
 use reqsign::AzureStorageCredential;
 use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
-use super::batch::BatchDeleteRequestBuilder;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
     pub const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
     pub const X_MS_COPY_SOURCE: &str = "x-ms-copy-source";
     pub const X_MS_BLOB_CACHE_CONTROL: &str = "x-ms-blob-cache-control";
@@ -270,29 +267,33 @@
     ) -> Result<Response<IncomingAsyncBody>> {
         let mut req = self.azblob_head_blob_request(path, if_none_match, if_match)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn azblob_delete_blob(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub fn azblob_delete_blob_request(&self, path: &str) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/{}/{}",
             self.endpoint,
             self.container,
             percent_encode_path(&p)
         );
 
         let req = Request::delete(&url);
 
-        let mut req = req
+        req.header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+            .map_err(new_request_build_error)
+    }
+
+    pub async fn azblob_delete_blob(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.azblob_delete_blob_request(path)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn azblob_copy_blob(
         &self,
@@ -360,41 +361,30 @@
         self.send(req).await
     }
 
     pub async fn azblob_batch_delete(
         &self,
         paths: &[String],
     ) -> Result<Response<IncomingAsyncBody>> {
-        // init batch request
         let url = format!(
             "{}/{}?restype=container&comp=batch",
             self.endpoint, self.container
         );
-        let mut batch_delete_req_builder = BatchDeleteRequestBuilder::new(&url);
-
-        for path in paths.iter() {
-            // build sub requests
-            let p = build_abs_path(&self.root, path);
-            let encoded_path = percent_encode_path(&p);
-
-            let url = Uri::from_str(&format!(
-                "{}/{}/{}",
-                self.endpoint, self.container, encoded_path
-            ))
-            .unwrap();
 
-            let mut sub_req = Request::delete(&url.to_string())
-                .header(CONTENT_LENGTH, 0)
-                .body(AsyncBody::Empty)
-                .map_err(new_request_build_error)?;
+        let mut multipart = Multipart::new();
 
-            self.batch_sign(&mut sub_req).await?;
+        for (idx, path) in paths.iter().enumerate() {
+            let mut req = self.azblob_delete_blob_request(path)?;
 
-            batch_delete_req_builder.append(sub_req);
+            self.batch_sign(&mut req).await?;
+            multipart = multipart.part(
+                MixedPart::from_request(req).part_header("content-id".parse().unwrap(), idx.into()),
+            );
         }
 
-        let mut req = batch_delete_req_builder.try_into_req()?;
+        let req = Request::post(url);
+        let mut req = multipart.apply(req)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -307,17 +307,19 @@
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azdfs)
             .set_root(&self.core.root)
             .set_name(&self.core.filesystem)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 write: true,
                 rename: true,
                 list: true,
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -299,21 +299,23 @@
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Fs)
             .set_root(&self.root.to_string_lossy())
             .set_capability(Capability {
                 read: true,
                 read_can_seek: true,
+                read_with_range: true,
                 write: true,
                 write_without_content_length: true,
                 create_dir: true,
                 list: true,
                 copy: true,
                 rename: true,
                 blocking: true,
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 /// - [x] list
 /// - [ ] ~~scan~~
 /// - [ ] ~~presign~~
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
-/// - `endpoint`: set the endpoint for connection
+/// - `endpoint`: Set the endpoint for connection
 /// - `root`: Set the work directory for backend
-/// - `credential`:  login credentials
-/// - `tls`: tls mode
+/// - `user`: Set the login user
+/// - `password`: Set the login password
 ///
 /// You can refer to [`FtpBuilder`]'s docs for more information
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
@@ -314,16 +314,18 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ftp)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
+                read_with_range: true,
                 write: true,
                 list: true,
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -377,28 +377,31 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
 
                 list: true,
                 list_with_limit: true,
                 list_with_start_after: true,
                 scan: true,
                 copy: true,
                 presign: true,
 
+                list_with_delimiter_slash: true,
+                list_without_delimiter: true,
                 ..Default::default()
             });
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req = self
@@ -509,28 +512,21 @@
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
             GcsPager::new(
                 self.core.clone(),
                 path,
-                "/",
+                args.delimiter(),
                 args.limit(),
                 args.start_after(),
             ),
         ))
     }
 
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        Ok((
-            RpScan::default(),
-            GcsPager::new(self.core.clone(), path, "", args.limit(), None),
-        ))
-    }
-
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
                 self.core
                     .gcs_head_object_xml_request(path, v.if_match(), v.if_none_match())?
             }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 use std::fmt::Write;
 use std::time::Duration;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
 use bytes::BytesMut;
-
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -299,14 +299,16 @@
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ghac)
             .set_root(&self.root)
             .set_name(&self.version)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
+
                 write: true,
 
                 ..Default::default()
             });
         am
     }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -236,17 +236,21 @@
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Hdfs)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
                 read_can_seek: true,
+                read_with_range: true,
+
                 write: true,
                 list: true,
                 blocking: true,
+
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,15 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 ..Default::default()
             });
 
         ma
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -218,16 +218,18 @@
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Ipfs)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 list: true,
 
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         ma
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 use std::fmt;
 use std::fmt::Write;
 use std::str;
 use std::sync::Arc;
 
 use async_trait::async_trait;
+use bytes::Bytes;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 use serde::Deserialize;
 
 use super::error::parse_error;
 use super::pager::IpmfsPager;
@@ -72,16 +73,19 @@
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ipmfs)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 write: true,
 
+                list: true,
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -277,27 +281,28 @@
         self.client.send(req).await
     }
 
     /// Support write from reader.
     pub async fn ipmfs_write(
         &self,
         path: &str,
-        body: AsyncBody,
+        body: Bytes,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!(
             "{}/api/v0/files/write?arg={}&parents=true&create=true&truncate=true",
             self.endpoint,
             percent_encode_path(&p)
         );
 
-        let req = Request::post(url);
+        let multipart = Multipart::new().part(FormDataPart::new("data").content(body));
 
-        let req = req.body(body).map_err(new_request_build_error)?;
+        let req: http::request::Builder = Request::post(url);
+        let req = multipart.apply(req)?;
 
         self.client.send(req).await
     }
 }
 
 #[derive(Deserialize, Default, Debug)]
 #[serde(default)]
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -35,18 +35,15 @@
         IpmfsWriter { backend, path }
     }
 }
 
 #[async_trait]
 impl oio::Write for IpmfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
-            .backend
-            .ipmfs_write(&self.path, AsyncBody::Multipart("data".to_string(), bs))
-            .await?;
+        let resp = self.backend.ipmfs_write(&self.path, bs).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,172 @@
-// Copyright 2017 vavrusa <marek@vavrusa.com>
+// Licensed to the Apache Software Foundation (ASF) under one
+// or more contributor license agreements.  See the NOTICE file
+// distributed with this work for additional information
+// regarding copyright ownership.  The ASF licenses this file
+// to you under the Apache License, Version 2.0 (the
+// "License"); you may not use this file except in compliance
+// with the License.  You may obtain a copy of the License at
 //
-// Licensed under the MIT License (see MIT-ascii.txt);
+//   http://www.apache.org/licenses/LICENSE-2.0
+//
+// Unless required by applicable law or agreed to in writing,
+// software distributed under the License is distributed on an
+// "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+// KIND, either express or implied.  See the License for the
+// specific language governing permissions and limitations
+// under the License.
+
+use crate::*;
+
+use super::backend::parse_io_error;
+use tokio::io::AsyncBufReadExt;
+use tokio::io::AsyncReadExt;
+use tokio::io::AsyncWriteExt;
+use tokio::io::BufReader;
+use tokio::net::TcpStream;
 
-use core::fmt::Display;
-use std::io::Error;
-use std::io::ErrorKind;
-use std::marker::Unpin;
-
-use futures::io::AsyncBufReadExt;
-use futures::io::AsyncRead;
-use futures::io::AsyncReadExt;
-use futures::io::AsyncWrite;
-use futures::io::AsyncWriteExt;
-use futures::io::BufReader;
-
-/// Memcache ASCII protocol implementation.
-pub struct Protocol<S> {
-    io: BufReader<S>,
+pub struct Connection {
+    io: BufReader<TcpStream>,
     buf: Vec<u8>,
 }
 
-impl<S> Protocol<S>
-where
-    S: AsyncRead + AsyncWrite + Unpin,
-{
-    /// Creates the ASCII protocol on a stream.
-    pub fn new(io: S) -> Self {
+impl Connection {
+    pub fn new(io: TcpStream) -> Self {
         Self {
             io: BufReader::new(io),
             buf: Vec::new(),
         }
     }
 
-    /// Returns the value for given key as bytes. If the value doesn't exist, [`ErrorKind::NotFound`] is returned.
-    pub async fn get<K: AsRef<[u8]>>(&mut self, key: K) -> Result<Vec<u8>, Error> {
+    pub async fn get(&mut self, key: &str) -> Result<Option<Vec<u8>>> {
         // Send command
         let writer = self.io.get_mut();
         writer
-            .write_all(&[b"get ", key.as_ref(), b"\r\n"].concat())
-            .await?;
-        writer.flush().await?;
+            .write_all(&[b"get ", key.as_bytes(), b"\r\n"].concat())
+            .await
+            .map_err(parse_io_error)?;
+        writer.flush().await.map_err(parse_io_error)?;
 
         // Read response header
-        let header = self.read_line().await?;
-        let header = std::str::from_utf8(header).map_err(|_| ErrorKind::InvalidData)?;
+        let header = self.read_header().await?;
 
         // Check response header and parse value length
         if header.contains("ERROR") {
-            return Err(Error::new(ErrorKind::Other, header));
+            return Err(
+                Error::new(ErrorKind::Unexpected, "unexpected data received")
+                    .with_context("message", header),
+            );
         } else if header.starts_with("END") {
-            return Err(ErrorKind::NotFound.into());
+            return Ok(None);
         }
 
         // VALUE <key> <flags> <bytes> [<cas unique>]\r\n
         let length: usize = header
             .split(' ')
             .nth(3)
             .and_then(|len| len.trim_end().parse().ok())
-            .ok_or(ErrorKind::InvalidData)?;
+            .ok_or_else(|| Error::new(ErrorKind::Unexpected, "invalid data received"))?;
 
         // Read value
         let mut buffer: Vec<u8> = vec![0; length];
-        self.io.read_exact(&mut buffer).await?;
+        self.io
+            .read_exact(&mut buffer)
+            .await
+            .map_err(parse_io_error)?;
 
         // Read the trailing header
         self.read_line().await?; // \r\n
         self.read_line().await?; // END\r\n
 
-        Ok(buffer)
+        Ok(Some(buffer))
     }
 
-    /// Set key to given value and don't wait for response.
-    pub async fn set<K: Display>(
-        &mut self,
-        key: K,
-        val: &[u8],
-        expiration: u32,
-    ) -> Result<(), Error> {
+    pub async fn set(&mut self, key: &str, val: &[u8], expiration: u32) -> Result<()> {
         let header = format!("set {} 0 {} {}\r\n", key, expiration, val.len());
-        self.io.write_all(header.as_bytes()).await?;
-        self.io.write_all(val).await?;
-        self.io.write_all(b"\r\n").await?;
-        self.io.flush().await?;
+        self.io
+            .write_all(header.as_bytes())
+            .await
+            .map_err(parse_io_error)?;
+        self.io.write_all(val).await.map_err(parse_io_error)?;
+        self.io.write_all(b"\r\n").await.map_err(parse_io_error)?;
+        self.io.flush().await.map_err(parse_io_error)?;
 
         // Read response header
-        let header = self.read_line().await?;
-        let header = std::str::from_utf8(header).map_err(|_| ErrorKind::InvalidData)?;
+        let header = self.read_header().await?;
+
         // Check response header and make sure we got a `STORED`
         if header.contains("STORED") {
             return Ok(());
         } else if header.contains("ERROR") {
-            return Err(Error::new(ErrorKind::Other, header));
+            return Err(
+                Error::new(ErrorKind::Unexpected, "unexpected data received")
+                    .with_context("message", header),
+            );
         }
         Ok(())
     }
 
-    /// Delete a key and don't wait for response.
-    pub async fn delete<K: Display>(&mut self, key: K) -> Result<(), Error> {
+    pub async fn delete(&mut self, key: &str) -> Result<()> {
         let header = format!("delete {}\r\n", key);
-        self.io.write_all(header.as_bytes()).await?;
-        self.io.flush().await?;
+        self.io
+            .write_all(header.as_bytes())
+            .await
+            .map_err(parse_io_error)?;
+        self.io.flush().await.map_err(parse_io_error)?;
 
         // Read response header
-        let header = self.read_line().await?;
-        let header = std::str::from_utf8(header).map_err(|_| ErrorKind::InvalidData)?;
+        let header = self.read_header().await?;
+
         // Check response header and parse value length
-        if header.contains("NOT_FOUND") {
+        if header.contains("NOT_FOUND") || header.starts_with("END") {
             return Ok(());
-        } else if header.starts_with("END") {
-            return Err(ErrorKind::NotFound.into());
         } else if header.contains("ERROR") || !header.contains("DELETED") {
-            return Err(Error::new(ErrorKind::Other, header));
+            return Err(
+                Error::new(ErrorKind::Unexpected, "unexpected data received")
+                    .with_context("message", header),
+            );
         }
         Ok(())
     }
 
-    /// Return the version of the remote server.
-    pub async fn version(&mut self) -> Result<String, Error> {
-        self.io.write_all(b"version\r\n").await?;
-        self.io.flush().await?;
+    pub async fn version(&mut self) -> Result<String> {
+        self.io
+            .write_all(b"version\r\n")
+            .await
+            .map_err(parse_io_error)?;
+        self.io.flush().await.map_err(parse_io_error)?;
 
         // Read response header
-        let header = {
-            let buf = self.read_line().await?;
-            std::str::from_utf8(buf).map_err(|_| Error::from(ErrorKind::InvalidData))?
-        };
+        let header = self.read_header().await?;
 
         if !header.starts_with("VERSION") {
-            return Err(Error::new(ErrorKind::Other, header));
+            return Err(
+                Error::new(ErrorKind::Unexpected, "unexpected data received")
+                    .with_context("message", header),
+            );
         }
         let version = header.trim_start_matches("VERSION ").trim_end();
         Ok(version.to_string())
     }
 
-    async fn read_line(&mut self) -> Result<&[u8], Error> {
+    async fn read_line(&mut self) -> Result<&[u8]> {
         let Self { io, buf } = self;
         buf.clear();
-        io.read_until(b'\n', buf).await?;
+        io.read_until(b'\n', buf).await.map_err(parse_io_error)?;
         if buf.last().copied() != Some(b'\n') {
-            return Err(ErrorKind::UnexpectedEof.into());
+            return Err(Error::new(
+                ErrorKind::ContentIncomplete,
+                "unexpected eof, the response must be incomplete",
+            ));
         }
         Ok(&buf[..])
     }
+
+    async fn read_header(&mut self) -> Result<&str> {
+        let header = self.read_line().await?;
+        let header = std::str::from_utf8(header).map_err(|err| {
+            Error::new(ErrorKind::Unexpected, "invalid data received").set_source(err)
+        })?;
+
+        Ok(header)
+    }
 }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
 use std::time::Duration;
 
-use async_compat::Compat;
 use async_trait::async_trait;
 use bb8::RunError;
 use tokio::net::TcpStream;
 use tokio::sync::OnceCell;
 
 use super::ascii;
 use crate::raw::adapters::kv;
@@ -216,15 +215,15 @@
             })
             .await?;
 
         pool.get().await.map_err(|err| match err {
             RunError::TimedOut => {
                 Error::new(ErrorKind::Unexpected, "get connection from pool failed").set_temporary()
             }
-            RunError::User(err) => parse_io_error(err),
+            RunError::User(err) => err,
         })
     }
 }
 
 #[async_trait]
 impl kv::Adapter for Adapter {
     fn metadata(&self) -> kv::Metadata {
@@ -239,68 +238,37 @@
                 ..Default::default()
             },
         )
     }
 
     async fn get(&self, key: &str) -> Result<Option<Vec<u8>>> {
         let mut conn = self.conn().await?;
-        // TODO: memcache-async have `Sized` limit on key, can we remove it?
-        match conn.get(&percent_encode_path(key)).await {
-            Ok(bs) => Ok(Some(bs)),
-            Err(err) if err.kind() == std::io::ErrorKind::NotFound => Ok(None),
-            Err(err) => Err(parse_io_error(err)),
-        }
+
+        conn.get(&percent_encode_path(key)).await
     }
 
     async fn set(&self, key: &str, value: &[u8]) -> Result<()> {
         let mut conn = self.conn().await?;
 
         conn.set(
             &percent_encode_path(key),
             value,
             // Set expiration to 0 if ttl not set.
             self.default_ttl
                 .map(|v| v.as_secs() as u32)
                 .unwrap_or_default(),
         )
         .await
-        .map_err(parse_io_error)?;
-
-        Ok(())
     }
 
     async fn delete(&self, key: &str) -> Result<()> {
         let mut conn = self.conn().await?;
 
-        let _: () = conn
-            .delete(&percent_encode_path(key))
-            .await
-            .map_err(parse_io_error)?;
-        Ok(())
-    }
-}
-
-fn parse_io_error(err: std::io::Error) -> Error {
-    use std::io::ErrorKind::*;
-
-    let (kind, retryable) = match err.kind() {
-        NotFound => (ErrorKind::NotFound, false),
-        AlreadyExists => (ErrorKind::NotFound, false),
-        PermissionDenied => (ErrorKind::PermissionDenied, false),
-        Interrupted | UnexpectedEof | TimedOut | WouldBlock => (ErrorKind::Unexpected, true),
-        _ => (ErrorKind::Unexpected, true),
-    };
-
-    let mut err = Error::new(kind, &err.kind().to_string()).set_source(err);
-
-    if retryable {
-        err = err.set_temporary();
+        conn.delete(&percent_encode_path(key)).await
     }
-
-    err
 }
 
 /// A `bb8::ManageConnection` for `memcache_async::ascii::Protocol`.
 ///
 /// Most code is borrowed from [bb8-memcached](https://github.com/dqminh/bb8-memcached/blob/master/src/client.rs).
 #[derive(Clone, Debug)]
 struct MemcacheConnectionManager {
@@ -313,24 +281,30 @@
             address: address.to_string(),
         }
     }
 }
 
 #[async_trait]
 impl bb8::ManageConnection for MemcacheConnectionManager {
-    type Connection = ascii::Protocol<Compat<TcpStream>>;
-    type Error = std::io::Error;
+    type Connection = ascii::Connection;
+    type Error = Error;
 
     /// TODO: Implement unix stream support.
     async fn connect(&self) -> std::result::Result<Self::Connection, Self::Error> {
-        let sock = TcpStream::connect(&self.address).await?;
-        Ok(ascii::Protocol::new(Compat::new(sock)))
+        let conn = TcpStream::connect(&self.address)
+            .await
+            .map_err(parse_io_error)?;
+        Ok(ascii::Connection::new(conn))
     }
 
     async fn is_valid(&self, conn: &mut Self::Connection) -> std::result::Result<(), Self::Error> {
         conn.version().await.map(|_| ())
     }
 
     fn has_broken(&self, _: &mut Self::Connection) -> bool {
         false
     }
 }
+
+pub fn parse_io_error(err: std::io::Error) -> Error {
+    Error::new(ErrorKind::Unexpected, &err.kind().to_string()).set_source(err)
+}
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -110,31 +110,52 @@
 pub use self::rocksdb::Rocksdb;
 
 #[cfg(feature = "services-s3")]
 mod s3;
 #[cfg(feature = "services-s3")]
 pub use s3::S3;
 
+#[cfg(feature = "services-sftp")]
+mod sftp;
+#[cfg(feature = "services-sftp")]
+pub use sftp::Sftp;
+
 #[cfg(feature = "services-sled")]
 mod sled;
 #[cfg(feature = "services-sled")]
 pub use self::sled::Sled;
 
-// #[cfg(feature = "services-supabase")]
+#[cfg(feature = "services-supabase")]
 mod supabase;
-// #[cfg(feature = "services-supabase")]
+#[cfg(feature = "services-supabase")]
 pub use supabase::Supabase;
 
 #[cfg(feature = "services-wasabi")]
 mod wasabi;
 #[cfg(feature = "services-wasabi")]
 pub use wasabi::Wasabi;
 
 #[cfg(feature = "services-webdav")]
 mod webdav;
 #[cfg(feature = "services-webdav")]
 pub use webdav::Webdav;
 
 #[cfg(feature = "services-webhdfs")]
 mod webhdfs;
+
+#[cfg(feature = "services-onedrive")]
+mod onedrive;
+#[cfg(feature = "services-onedrive")]
+pub use onedrive::Onedrive;
+
+#[cfg(feature = "services-gdrive")]
+mod gdrive;
+#[cfg(feature = "services-gdrive")]
+pub use gdrive::Gdrive;
+
 #[cfg(feature = "services-webhdfs")]
 pub use webhdfs::Webhdfs;
+
+#[cfg(feature = "services-vercel-artifacts")]
+mod vercel_artifacts;
+#[cfg(feature = "services-vercel-artifacts")]
+pub use vercel_artifacts::VercelArtifacts;
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -308,25 +308,29 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_with_content_type: true,
                 write_with_cache_control: true,
 
                 list: true,
                 scan: true,
                 copy: true,
 
+                list_with_delimiter_slash: true,
+                list_without_delimiter: true,
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -429,18 +433,11 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            ObsPager::new(self.core.clone(), path, "/", args.limit()),
-        ))
-    }
-
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        Ok((
-            RpScan::default(),
-            ObsPager::new(self.core.clone(), path, "", args.limit()),
+            ObsPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
         ))
     }
 }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -426,14 +426,15 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
@@ -441,14 +442,17 @@
                 list: true,
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 batch_max_operations: Some(1000),
 
+                list_with_delimiter_slash: true,
+                list_without_delimiter: true,
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -545,22 +549,15 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            OssPager::new(self.core.clone(), path, "/", args.limit()),
-        ))
-    }
-
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        Ok((
-            RpScan::default(),
-            OssPager::new(self.core.clone(), path, "", args.limit()),
+            OssPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
 
 use super::core::*;
 use super::error::parse_error;
+use super::error::parse_s3_error_code;
 use super::pager::S3Pager;
 use super::writer::S3Writer;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
 /// Allow constructing correct region endpoint if user gives a global endpoint.
@@ -915,16 +916,18 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
+                read_with_override_cache_control: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
 
@@ -934,14 +937,17 @@
 
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 batch_max_operations: Some(1000),
 
+                list_without_delimiter: true,
+                list_with_delimiter_slash: true,
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -1046,28 +1052,21 @@
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
             S3Pager::new(
                 self.core.clone(),
                 path,
-                "/",
+                args.delimiter(),
                 args.limit(),
                 args.start_after(),
             ),
         ))
     }
 
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        Ok((
-            RpScan::default(),
-            S3Pager::new(self.core.clone(), path, "", args.limit(), None),
-        ))
-    }
-
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => {
                 self.core
                     .s3_head_object_request(path, v.if_none_match(), v.if_match())?
             }
@@ -1124,18 +1123,23 @@
                 let path = build_rel_path(&self.core.root, &i.key);
                 batched_result.push((path, Ok(RpDelete::default().into())));
             }
             // TODO: we should handle those errors with code.
             for i in result.error {
                 let path = build_rel_path(&self.core.root, &i.key);
 
-                batched_result.push((
-                    path,
-                    Err(Error::new(ErrorKind::Unexpected, &format!("{i:?}"))),
-                ));
+                // set the error kind and mark temporary if retryable
+                let (kind, retryable) =
+                    parse_s3_error_code(i.code.as_str()).unwrap_or((ErrorKind::Unexpected, false));
+                let mut err = Error::new(kind, &format!("{i:?}"));
+                if retryable {
+                    err = err.set_temporary();
+                }
+
+                batched_result.push((path, Err(err)));
             }
 
             Ok(RpBatch::new(batched_result))
         } else {
             Err(parse_error(resp).await?)
         }
     }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files 10% similar despite different names*

```diff
@@ -22,49 +22,47 @@
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
-/// S3Error is the error returned by s3 service.
+/// WasabiError is the error returned by wasabi service.
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
-struct S3Error {
+struct WasabiError {
     code: String,
     message: String,
     resource: String,
     request_id: String,
 }
 
 /// Parse error response into Error.
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
-            (ErrorKind::ConditionNotMatch, false)
-        }
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let (message, s3_err) = de::from_reader::<_, S3Error>(bs.clone().reader())
-        .map(|s3_err| (format!("{s3_err:?}"), Some(s3_err)))
+    let (message, wasabi_err) = de::from_reader::<_, WasabiError>(bs.clone().reader())
+        .map(|err| (format!("{err:?}"), Some(err)))
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
     // All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
-    if let Some(s3_err) = s3_err {
-        (kind, retryable) = match s3_err.code.as_str() {
+    if let Some(wasabi_err) = wasabi_err {
+        (kind, retryable) = match wasabi_err.code.as_str() {
             // > Your socket connection to the server was not read from
             // > or written to within the timeout period."
             //
             // It's Ok for us to retry it again.
             "RequestTimeout" => (ErrorKind::Unexpected, true),
             _ => (kind, retryable),
         }
@@ -94,15 +92,15 @@
   <Message>The resource you requested does not exist</Message>
   <Resource>/mybucket/myfoto.jpg</Resource>
   <RequestId>4442587FB7D0A2F9</RequestId>
 </Error>
 "#,
         );
 
-        let out: S3Error = de::from_reader(bs.reader()).expect("must success");
+        let out: WasabiError = de::from_reader(bs.reader()).expect("must success");
         println!("{out:?}");
 
         assert_eq!(out.code, "NoSuchKey");
         assert_eq!(out.message, "The resource you requested does not exist");
         assert_eq!(out.resource, "/mybucket/myfoto.jpg");
         assert_eq!(out.request_id, "4442587FB7D0A2F9");
     }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/supabase/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/supabase/backend.rs`

 * *Files 14% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ///     builder.root("/");
 ///     builder.bucket("test_bucket");
 ///     builder.endpoint("http://127.0.0.1:54321");
 ///     // this sets up the anon_key, which means this operator can only write public resource
 ///     builder.key("some_anon_key");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
-///    
+///
 ///     Ok(())
 /// }
 /// ```
 #[derive(Default)]
 pub struct SupabaseBuilder {
     root: Option<String>,
 
@@ -214,23 +214,50 @@
         am.set_scheme(Scheme::Supabase)
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capability(Capability {
                 stat: true,
                 read: true,
                 write: true,
+                create_dir: true,
+                delete: true,
 
                 ..Default::default()
             });
 
         am
     }
 
-    async fn read(&self, path: &str, _args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.core.supabase_get_object(path).await?;
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+        let mut req =
+            self.core
+                .supabase_upload_object_request(path, Some(0), None, AsyncBody::Empty)?;
+
+        self.core.sign(&mut req)?;
+
+        let resp = self.core.send(req).await?;
+
+        let status = resp.status();
+
+        if status.is_success() {
+            resp.into_body().consume().await?;
+            Ok(RpCreate::default())
+        } else {
+            // create duplicate dir is ok
+            let e = parse_error(resp).await?;
+            if e.kind() == ErrorKind::AlreadyExists {
+                Ok(RpCreate::default())
+            } else {
+                Err(e)
+            }
+        }
+    }
+
+    async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
+        let resp = self.core.supabase_get_object(path, args.range()).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
@@ -255,20 +282,42 @@
 
     async fn stat(&self, path: &str, _args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.supabase_get_object_info(path).await?;
+        // The get_object_info does not contain the file size. Therefore
+        // we first try the get the metadata through head, if we fail,
+        // we then use get_object_info to get the actual error info
+        let mut resp = self.core.supabase_head_object(path).await?;
 
-        let status = resp.status();
-
-        match status {
+        match resp.status() {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
-            StatusCode::NOT_FOUND if path.ends_with('/') => {
-                Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
+            _ => {
+                resp = self.core.supabase_get_object_info(path).await?;
+                match resp.status() {
+                    StatusCode::NOT_FOUND if path.ends_with('/') => {
+                        Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
+                    }
+                    _ => Err(parse_error(resp).await?),
+                }
+            }
+        }
+    }
+
+    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
+        let resp = self.core.supabase_delete_object(path).await?;
+
+        if resp.status().is_success() {
+            Ok(RpDelete::default())
+        } else {
+            // deleting not existing objects is ok
+            let e = parse_error(resp).await?;
+            if e.kind() == ErrorKind::NotFound {
+                Ok(RpDelete::default())
+            } else {
+                Err(e)
             }
-            _ => Err(parse_error(resp).await?),
         }
     }
 }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/supabase/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/onedrive/backend.rs`

 * *Files 27% similar despite different names*

```diff
@@ -13,188 +13,200 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 
-use http::header::CONTENT_LENGTH;
-use http::header::CONTENT_TYPE;
-use http::HeaderValue;
+use async_trait::async_trait;
+use http::header;
 use http::Request;
 use http::Response;
+use http::StatusCode;
 
-use crate::raw::*;
-use crate::*;
-
-pub struct SupabaseCore {
-    pub root: String,
-    pub bucket: String,
-    pub endpoint: String,
-
-    /// The key used for authorization
-    /// If loaded, the read operation will always access the nonpublic resources.
-    /// If you want to read the public resources, please do not set the key.
-    pub key: Option<String>,
-
-    pub http_client: HttpClient,
+use super::error::parse_error;
+use super::writer::OneDriveWriter;
+use crate::ops::OpRead;
+use crate::ops::OpWrite;
+use crate::raw::build_rooted_abs_path;
+use crate::raw::new_request_build_error;
+use crate::raw::parse_into_metadata;
+use crate::raw::parse_location;
+use crate::raw::percent_encode_path;
+use crate::raw::Accessor;
+use crate::raw::AccessorInfo;
+use crate::raw::AsyncBody;
+use crate::raw::HttpClient;
+use crate::raw::IncomingAsyncBody;
+use crate::raw::RpRead;
+use crate::raw::RpWrite;
+use crate::types::Result;
+use crate::Capability;
+use crate::Error;
+use crate::ErrorKind;
+
+#[derive(Clone)]
+pub struct OnedriveBackend {
+    root: String,
+    access_token: String,
+    client: HttpClient,
 }
 
-impl Debug for SupabaseCore {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("SupabaseCore")
-            .field("root", &self.root)
-            .field("bucket", &self.bucket)
-            .field("endpoint", &self.endpoint)
-            .finish_non_exhaustive()
-    }
-}
-
-impl SupabaseCore {
-    pub fn new(
-        root: &str,
-        bucket: &str,
-        endpoint: &str,
-        key: Option<String>,
-        client: HttpClient,
-    ) -> Self {
+impl OnedriveBackend {
+    pub(crate) fn new(root: String, access_token: String, http_client: HttpClient) -> Self {
         Self {
-            root: root.to_string(),
-            bucket: bucket.to_string(),
-            endpoint: endpoint.to_string(),
-            key,
-            http_client: client,
+            root,
+            access_token,
+            client: http_client,
         }
     }
+}
 
-    /// Add authorization header to the request if the key is set. Otherwise leave
-    /// the request as-is.
-    pub fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
-        if let Some(k) = &self.key {
-            let v = HeaderValue::from_str(&format!("Bearer {}", k)).unwrap();
-            req.headers_mut().insert(http::header::AUTHORIZATION, v);
-        }
-        Ok(())
+impl Debug for OnedriveBackend {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        let mut de = f.debug_struct("OneDriveBackend");
+        de.field("root", &self.root);
+        de.field("access_token", &self.access_token);
+        de.finish()
     }
 }
 
-// requests
-impl SupabaseCore {
-    pub fn supabase_upload_object_request(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-        let url = format!(
-            "{}/storage/v1/object/{}/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::post(&url);
+#[async_trait]
+impl Accessor for OnedriveBackend {
+    type Reader = IncomingAsyncBody;
+    type BlockingReader = ();
+    type Writer = OneDriveWriter;
+    type BlockingWriter = ();
+    type Pager = ();
+    type BlockingPager = ();
+
+    fn info(&self) -> AccessorInfo {
+        let mut ma = AccessorInfo::default();
+        ma.set_scheme(crate::Scheme::Onedrive)
+            .set_root(&self.root)
+            .set_capability(Capability {
+                read: true,
+                read_can_next: true,
+                write: true,
+                list: true,
+                copy: true,
+                rename: true,
+                ..Default::default()
+            });
+
+        ma
+    }
+
+    async fn read(&self, path: &str, _args: OpRead) -> Result<(RpRead, Self::Reader)> {
+        let resp = self.onedrive_get(path).await?;
+
+        let status = resp.status();
+
+        if status.is_redirection() {
+            let headers = resp.headers();
+            let location = parse_location(headers)?;
+
+            match location {
+                None => {
+                    return Err(Error::new(
+                        ErrorKind::ContentIncomplete,
+                        "redirect location not found in response",
+                    ));
+                }
+                Some(location) => {
+                    let resp = self.onedrive_get_redirection(location).await?;
+                    let meta = parse_into_metadata(path, resp.headers())?;
+                    Ok((RpRead::with_metadata(meta), resp.into_body()))
+                }
+            }
+        } else {
+            match status {
+                StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
+                    let meta = parse_into_metadata(path, resp.headers())?;
+                    Ok((RpRead::with_metadata(meta), resp.into_body()))
+                }
 
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
+                _ => Err(parse_error(resp).await?),
+            }
         }
+    }
 
-        if let Some(mime) = content_type {
-            req = req.header(CONTENT_TYPE, mime)
+    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
+        if args.content_length().is_none() {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "write without content length is not supported",
+            ));
         }
 
-        let req = req.body(body).map_err(new_request_build_error)?;
+        let path = build_rooted_abs_path(&self.root, path);
 
-        Ok(req)
+        Ok((
+            RpWrite::default(),
+            OneDriveWriter::new(self.clone(), args, path),
+        ))
     }
+}
 
-    pub fn supabase_get_object_public_request(&self, path: &str) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-        let url = format!(
-            "{}/storage/v1/object/public/{}/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
+impl OnedriveBackend {
+    async fn onedrive_get(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let path = build_rooted_abs_path(&self.root, path);
+        let url: String = format!(
+            "https://graph.microsoft.com/v1.0/me/drive/root:{}:/content",
+            percent_encode_path(&path),
         );
 
-        Request::get(&url)
+        let mut req = Request::get(&url);
+
+        let auth_header_content = format!("Bearer {}", self.access_token);
+        req = req.header(header::AUTHORIZATION, auth_header_content);
+
+        let req = req
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)
+            .map_err(new_request_build_error)?;
+
+        self.client.send(req).await
     }
 
-    pub fn supabase_get_object_auth_request(&self, path: &str) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-        let url = format!(
-            "{}/storage/v1/object/authenticated/{}/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
+    async fn onedrive_get_redirection(&self, url: &str) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = Request::get(url);
 
-        Request::get(&url)
+        let auth_header_content = format!("Bearer {}", self.access_token);
+        req = req.header(header::AUTHORIZATION, auth_header_content);
+
+        let req = req
             .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)
+            .map_err(new_request_build_error)?;
+
+        self.client.send(req).await
     }
 
-    pub fn supabase_get_object_info_public_request(
+    pub async fn onedrive_put(
         &self,
         path: &str,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
+        size: Option<usize>,
+        content_type: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let url = format!(
-            "{}/storage/v1/object/info/public/{}/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
+            "https://graph.microsoft.com/v1.0/me/drive/root:{}:/content",
+            percent_encode_path(path)
         );
 
-        Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)
-    }
+        let mut req = Request::put(&url);
 
-    pub fn supabase_get_object_info_auth_request(&self, path: &str) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-        let url = format!(
-            "{}/storage/v1/object/info/authenticated/{}/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
+        let auth_header_content = format!("Bearer {}", self.access_token);
+        req = req.header(header::AUTHORIZATION, auth_header_content);
 
-        Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)
-    }
-}
+        if let Some(size) = size {
+            req = req.header(header::CONTENT_LENGTH, size)
+        }
 
-// core utils
-impl SupabaseCore {
-    pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
-        self.http_client.send(req).await
-    }
+        if let Some(mime) = content_type {
+            req = req.header(header::CONTENT_TYPE, mime)
+        }
 
-    pub async fn supabase_get_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = if self.key.is_some() {
-            self.supabase_get_object_auth_request(path)?
-        } else {
-            self.supabase_get_object_public_request(path)?
-        };
-        self.sign(&mut req)?;
-        self.send(req).await
-    }
+        let req = req.body(body).map_err(new_request_build_error)?;
 
-    pub async fn supabase_get_object_info(
-        &self,
-        path: &str,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = if self.key.is_some() {
-            self.supabase_get_object_info_auth_request(path)?
-        } else {
-            self.supabase_get_object_info_public_request(path)?
-        };
-        self.sign(&mut req)?;
-        self.send(req).await
+        self.client.send(req).await
     }
 }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/supabase/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/supabase/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/supabase/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/supabase/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -904,23 +904,27 @@
             .set_capability(Capability {
                 stat: true,
                 stat_with_if_match: true,
                 stat_with_if_none_match: true,
 
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
 
                 write: true,
                 list: true,
                 scan: true,
                 copy: true,
                 presign: true,
                 batch: true,
                 rename: true,
 
+                list_without_delimiter: true,
+                list_with_delimiter_slash: true,
+
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -1013,22 +1017,15 @@
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            WasabiPager::new(self.core.clone(), path, "/", args.limit()),
-        ))
-    }
-
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        Ok((
-            RpScan::default(),
-            WasabiPager::new(self.core.clone(), path, "", args.limit()),
+            WasabiPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
             PresignOperation::Stat(v) => self.core.head_object_request(path, v.if_none_match())?,
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files 24% similar despite different names*

```diff
@@ -22,65 +22,87 @@
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
-/// WasabiError is the error returned by wasabi service.
+/// S3Error is the error returned by s3 service.
 #[derive(Default, Debug, Deserialize)]
 #[serde(default, rename_all = "PascalCase")]
-struct WasabiError {
+struct S3Error {
     code: String,
     message: String,
     resource: String,
     request_id: String,
 }
 
 /// Parse error response into Error.
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
 
-    let (message, wasabi_err) = de::from_reader::<_, WasabiError>(bs.clone().reader())
-        .map(|err| (format!("{err:?}"), Some(err)))
+    let (message, s3_err) = de::from_reader::<_, S3Error>(bs.clone().reader())
+        .map(|s3_err| (format!("{s3_err:?}"), Some(s3_err)))
         .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
 
-    // All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
-    if let Some(wasabi_err) = wasabi_err {
-        (kind, retryable) = match wasabi_err.code.as_str() {
-            // > Your socket connection to the server was not read from
-            // > or written to within the timeout period."
-            //
-            // It's Ok for us to retry it again.
-            "RequestTimeout" => (ErrorKind::Unexpected, true),
-            _ => (kind, retryable),
-        }
+    if let Some(s3_err) = s3_err {
+        (kind, retryable) = parse_s3_error_code(s3_err.code.as_str()).unwrap_or((kind, retryable));
     }
 
     let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
 
     if retryable {
         err = err.set_temporary();
     }
 
     Ok(err)
 }
 
+/// Returns the Errorkind of this code and whether the error is retryable.
+/// All possible error code: <https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#ErrorCodeList>
+pub fn parse_s3_error_code(code: &str) -> Option<(ErrorKind, bool)> {
+    match code {
+        // > Your socket connection to the server was not read from
+        // > or written to within the timeout period."
+        //
+        // It's Ok for us to retry it again.
+        "RequestTimeout" => Some((ErrorKind::Unexpected, true)),
+        // > An internal error occurred. Try again.
+        "InternalError" => Some((ErrorKind::Unexpected, true)),
+        // > A conflicting conditional operation is currently in progress
+        // > against this resource. Try again.
+        "OperationAborted" => Some((ErrorKind::Unexpected, true)),
+        // > Please reduce your request rate.
+        //
+        // It's Ok to retry since later on the request rate may get reduced.
+        "SlowDown" => Some((ErrorKind::RateLimited, true)),
+        // > Service is unable to handle request.
+        //
+        // ServiceUnavailable is considered a retryable error because it typically
+        // indicates a temporary issue with the service or server, such as high load,
+        // maintenance, or an internal problem.
+        "ServiceUnavailable" => Some((ErrorKind::Unexpected, true)),
+        _ => None,
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     /// Error response example is from https://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html
     #[test]
     fn test_parse_error() {
@@ -92,15 +114,15 @@
   <Message>The resource you requested does not exist</Message>
   <Resource>/mybucket/myfoto.jpg</Resource>
   <RequestId>4442587FB7D0A2F9</RequestId>
 </Error>
 "#,
         );
 
-        let out: WasabiError = de::from_reader(bs.reader()).expect("must success");
+        let out: S3Error = de::from_reader(bs.reader()).expect("must success");
         println!("{out:?}");
 
         assert_eq!(out.code, "NoSuchKey");
         assert_eq!(out.message, "The resource you requested does not exist");
         assert_eq!(out.resource, "/mybucket/myfoto.jpg");
         assert_eq!(out.request_id, "4442587FB7D0A2F9");
     }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -265,18 +265,21 @@
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Webdav)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 write: true,
                 list: true,
                 copy: true,
                 rename: true,
+                list_without_delimiter: true,
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
 
         ma
     }
 
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
@@ -429,15 +432,15 @@
     async fn webdav_get(
         &self,
         path: &str,
         range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
-        let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
+        let url: String = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/gdrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -464,16 +464,19 @@
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Webhdfs)
             .set_root(&self.root)
             .set_capability(Capability {
                 read: true,
                 read_can_next: true,
+                read_with_range: true,
                 write: true,
                 list: true,
+                list_without_delimiter: true,
+                list_with_delimiter_slash: true,
                 ..Default::default()
             });
         am
     }
 
     /// Create a file or directory
     async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/capability.rs`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,18 @@
 
     /// If operator supports list natively, it will be true.
     pub list: bool,
     /// If backend supports list with limit, it will be true.
     pub list_with_limit: bool,
     /// If backend supports list with start after, it will be true.
     pub list_with_start_after: bool,
-
+    /// If backend support list with using slash as delimiter.
+    pub list_with_delimiter_slash: bool,
+    /// If backend supports list without delimiter.
+    pub list_without_delimiter: bool,
     /// If operator supports scan natively, it will be true.
     pub scan: bool,
     /// If backend supports scan with limit, it will be true.
     pub scan_with_limit: bool,
 
     /// If operator supports copy natively, it will be true.
     pub copy: bool,
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/error.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/list.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 use crate::*;
 
 /// Operator is the entry for all public async APIs.
 /// Developer should manipulate the data from storage service through Operator only by right.
 ///
 /// We will usually do some general checks and data transformations in this layer,
 /// like normalizing path from input, checking whether the path refers to one file or one directory, and so on.
-/// Read [`concepts`][docs::concepts] for know more about [`Operator`].
+/// Read [`concepts`][docs::concepts] for more about [`Operator`].
 ///
 /// # Examples
 ///
 /// Read more backend init examples in [`services`]
 ///
 /// ```
 /// # use anyhow::Result;
@@ -160,15 +160,15 @@
 
     /// Get current path's metadata **without cache** directly.
     ///
     /// # Notes
     ///
     /// Use `stat` if you:
     ///
-    /// - Want detect the outside changes of path.
+    /// - Want to detect the outside changes of path.
     /// - Don't want to read from cached metadata.
     ///
     /// You may want to use `metadata` if you are working with entries
     /// returned by [`Lister`]. It's highly possible that metadata
     /// you want has already been cached.
     ///
     /// # Examples
@@ -195,15 +195,15 @@
 
     /// Get current path's metadata **without cache** directly with extra options.
     ///
     /// # Notes
     ///
     /// Use `stat` if you:
     ///
-    /// - Want detect the outside changes of path.
+    /// - Want to detect the outside changes of path.
     /// - Don't want to read from cached metadata.
     ///
     /// You may want to use `metadata` if you are working with entries
     /// returned by [`Lister`]. It's highly possible that metadata
     /// you want has already been cached.
     ///
     /// # Examples
@@ -243,28 +243,28 @@
     ///
     /// Use `metadata` if you are working with entries returned by
     /// [`Lister`]. It's highly possible that metadata you want
     /// has already been cached.
     ///
     /// You may want to use `stat`, if you:
     ///
-    /// - Want detect the outside changes of path.
+    /// - Want to detect the outside changes of path.
     /// - Don't want to read from cached metadata.
     ///
     /// # Behavior
     ///
     /// Visiting not fetched metadata will lead to panic in debug build.
     /// It must be a bug, please fix it instead.
     ///
     /// # Examples
     ///
     /// ## Query already cached metadata
     ///
-    /// By query metadata with `None`, we can only query in-memory metadata
-    /// cache. In this way, we can make sure that no API call will send.
+    /// By querying metadata with `None`, we can only query in-memory metadata
+    /// cache. In this way, we can make sure that no API call will be sent.
     ///
     /// ```
     /// # use anyhow::Result;
     /// # use opendal::Operator;
     /// use opendal::Entry;
     /// # #[tokio::main]
     /// # async fn test(op: Operator, entry: Entry) -> Result<()> {
@@ -296,15 +296,15 @@
     /// let _ = meta.etag();
     /// # Ok(())
     /// # }
     /// ```
     ///
     /// ## Query all metadata
     ///
-    /// By query metadata with `Complete`, we can make sure that we have fetched all metadata of this entry.
+    /// By querying metadata with `Complete`, we can make sure that we have fetched all metadata of this entry.
     ///
     /// ```
     /// # use anyhow::Result;
     /// # use opendal::Operator;
     /// use opendal::Entry;
     /// use opendal::Metakey;
     ///
@@ -652,15 +652,15 @@
 
     /// Copy a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
     /// - `to` will be overwritten if it exists.
-    /// - If `from` and `to` are the same,  a `IsSameFile` error will occur.
+    /// - If `from` and `to` are the same,  an `IsSameFile` error will occur.
     /// - `copy` is idempotent. For same `from` and `to` input, the result will be the same.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
@@ -711,15 +711,15 @@
 
     /// Rename a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
     /// - `to` will be overwritten if it exists.
-    /// - If `from` and `to` are the same, a `IsSameFile` error will occur.
+    /// - If `from` and `to` are the same, an `IsSameFile` error will occur.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     ///
@@ -877,15 +877,15 @@
         Ok(())
     }
 
     /// Delete the given path.
     ///
     /// # Notes
     ///
-    /// - Delete not existing error won't return errors.
+    /// - Deleting a file that does not exist won't return errors.
     ///
     /// # Examples
     ///
     /// ```
     /// # use anyhow::Result;
     /// # use futures::io;
     /// # use opendal::Operator;
@@ -923,17 +923,17 @@
     /// # Ok(())
     /// # }
     /// ```
     pub async fn remove(&self, paths: Vec<String>) -> Result<()> {
         self.remove_via(stream::iter(paths)).await
     }
 
-    /// remove will given paths.
-
-    /// remove_via will remove files via given stream.
+    /// remove will remove files via the given paths.
+    ///
+    /// remove_via will remove files via the given stream.
     ///
     /// We will delete by chunks with given batch limit on the stream.
     ///
     /// # Notes
     ///
     /// If underlying services support delete in batch, we will use batch
     /// delete instead.
@@ -1099,18 +1099,18 @@
     ///
     /// # Examples
     ///
     /// ```no_run
     /// # use anyhow::Result;
     /// # use futures::io;
     /// use futures::TryStreamExt;
+    /// use opendal::ops::OpList;
     /// use opendal::EntryMode;
     /// use opendal::Metakey;
     /// use opendal::Operator;
-    /// use opendal::ops::OpList;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let option = OpList::new().with_limit(10).with_start_after("start");
     /// let mut ds = op.list_with("path/to/dir/", option).await?;
     /// while let Some(mut de) = ds.try_next().await? {
     ///     let meta = op.metadata(&de, Metakey::Mode).await?;
     ///     match meta.mode() {
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/ops.rs`

 * *Files 3% similar despite different names*

```diff
@@ -46,23 +46,36 @@
     /// Create a new `OpDelete`.
     pub fn new() -> Self {
         Self {}
     }
 }
 
 /// Args for `list` operation.
-#[derive(Debug, Clone, Default)]
+#[derive(Debug, Clone)]
 pub struct OpList {
     /// The limit passed to underlying service to specify the max results
     /// that could return.
     limit: Option<usize>,
 
     /// The start_after passes to underlying service to specify the specified key
     /// to start listing from.
     start_after: Option<String>,
+
+    /// The delimiter used to for the list operation. Default to be `/`
+    delimiter: String,
+}
+
+impl Default for OpList {
+    fn default() -> Self {
+        OpList {
+            limit: None,
+            start_after: None,
+            delimiter: "/".to_string(),
+        }
+    }
 }
 
 impl OpList {
     /// Create a new `OpList`.
     pub fn new() -> Self {
         Self::default()
     }
@@ -84,14 +97,25 @@
         self
     }
 
     /// Get the start_after of list operation.
     pub fn start_after(&self) -> Option<&str> {
         self.start_after.as_deref()
     }
+
+    /// Change the delimiter. The default delimiter is "/"
+    pub fn with_delimiter(mut self, delimiter: &str) -> Self {
+        self.delimiter = delimiter.to_string();
+        self
+    }
+
+    /// Get the current delimiter.
+    pub fn delimiter(&self) -> &str {
+        &self.delimiter
+    }
 }
 
 /// Args for `scan` operation.
 #[derive(Debug, Default, Clone)]
 pub struct OpScan {
     /// The limit passed to underlying service to specify the max results
     /// that could return.
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/scheme.rs`

 * *Files 6% similar despite different names*

```diff
@@ -57,26 +57,34 @@
     Memcached,
     /// [memory][crate::services::Memory]: In memory backend support.
     Memory,
     /// [moka][crate::services::Moka]: moka backend support.
     Moka,
     /// [obs][crate::services::Obs]: Huawei Cloud OBS services.
     Obs,
+    /// [onedrive][crate::services::Onedrive]: Microsoft OneDrive services.
+    Onedrive,
+    /// [gdrive][crate::services::Gdrive]: GoogleDrive services.
+    Gdrive,
     /// [oss][crate::services::Oss]: Aliyun Object Storage Services
     Oss,
     /// [redis][crate::services::Redis]: Redis services
     Redis,
     /// [rocksdb][crate::services::Rocksdb]: RocksDB services
     Rocksdb,
     /// [s3][crate::services::S3]: AWS S3 alike services.
     S3,
+    /// [sftp][crate::services::Sftp]: SFTP services
+    Sftp,
     /// [sled][crate::services::Sled]: Sled services
     Sled,
     /// [Supabase][crate::services::Supabase]: Supabase storage service
     Supabase,
+    /// [Vercel Artifacts][crate::services::vercel_artifacts]: Vercel Artifacts service, as known as Vercel Remote Caching.
+    VercelArtifacts,
     /// [wasabi][crate::services::Wasabi]: Wasabi service
     Wasabi,
     /// [webdav][crate::services::Webdav]: WebDAV support.
     Webdav,
     /// [webhdfs][crate::services::Webhdfs]: WebHDFS RESTful API Services
     Webhdfs,
     /// Custom that allow users to implement services outside of OpenDAL.
@@ -156,19 +164,23 @@
             Scheme::Ftp => "ftp",
             Scheme::Ipfs => "ipfs",
             Scheme::Ipmfs => "ipmfs",
             Scheme::Memcached => "memcached",
             Scheme::Memory => "memory",
             Scheme::Moka => "moka",
             Scheme::Obs => "obs",
+            Scheme::Onedrive => "onedrive",
+            Scheme::Gdrive => "gdrive",
             Scheme::Redis => "redis",
             Scheme::Rocksdb => "rocksdb",
             Scheme::S3 => "s3",
+            Scheme::Sftp => "sftp",
             Scheme::Sled => "sled",
             Scheme::Supabase => "supabase",
+            Scheme::VercelArtifacts => "vercel_artifacts",
             Scheme::Oss => "oss",
             Scheme::Wasabi => "wasabi",
             Scheme::Webdav => "webdav",
             Scheme::Webhdfs => "webhdfs",
             Scheme::Custom(v) => v,
         }
     }
```

### Comparing `opendal-0.33.2/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.33.3/local_dependencies/opendal/src/types/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/Cargo.toml` & `opendal-0.33.3/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.33.2"
+version= "0.33.3"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
-futures = "0.3.27"
+futures = "0.3.28"
 opendal.path = "local_dependencies/opendal"
 pyo3 = { version = "0.18", features = ["chrono"] }
 pyo3-asyncio = { version = "0.18", features = ["tokio-runtime"] }
 tokio = "1"
```

### Comparing `opendal-0.33.2/.gitignore` & `opendal-0.33.3/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/README.md` & `opendal-0.33.3/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/benchmark/README.md` & `opendal-0.33.3/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/benchmark/async_opendal_benchmark.py` & `opendal-0.33.3/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.33.3/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/examples/object.ipynb` & `opendal-0.33.3/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/pyproject.toml` & `opendal-0.33.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/python/opendal/__init__.py` & `opendal-0.33.3/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/python/opendal/__init__.pyi` & `opendal-0.33.3/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/src/asyncio.rs` & `opendal-0.33.3/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/src/layers.rs` & `opendal-0.33.3/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/src/lib.rs` & `opendal-0.33.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/tests/binding.feature` & `opendal-0.33.3/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/tests/steps/binding.py` & `opendal-0.33.3/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.33.2/Cargo.lock` & `opendal-0.33.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -34,48 +34,103 @@
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
+name = "anstream"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+dependencies = [
+ "anstyle 1.0.0",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
 name = "anstyle"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23ea9e81bd02e310c216d080f6223c179012256e5151c41db88d12c88a1684d2"
 
 [[package]]
+name = "anstyle"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle 1.0.0",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "anyhow"
 version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
+name = "array-init"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
+
+[[package]]
 name = "assert-json-diff"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "47e4f2b81832e72834d7518d8487a0396a28cc408186a2e8854c0f98011faf12"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "assert_cmd"
-version = "2.0.10"
+version = "2.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec0b2340f55d9661d76793b2bfc2eb0e62689bd79d067a95707ea762afd5e9dd"
+checksum = "86d6b683edf8d1119fe420a94f8a7e389239666aa72e65495d91c00462510151"
 dependencies = [
- "anstyle",
+ "anstyle 1.0.0",
  "bstr",
  "doc-comment",
  "predicates 3.0.1",
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
@@ -260,14 +315,30 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "awaitable"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "70af449c9a763cb655c6a1e5338b42d99c67190824ff90658c1e30be844c0775"
+dependencies = [
+ "awaitable-error",
+ "cfg-if",
+]
+
+[[package]]
+name = "awaitable-error"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5b3469636cdf8543cceab175efca534471f36eee12fb8374aba00eb5e7e7f8a"
+
+[[package]]
 name = "backon"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f34fac4d7cdaefa2deded0eda2d5d59dbfd43370ff3f856209e72340ae84c294"
 dependencies = [
  "futures",
  "pin-project",
@@ -588,55 +659,67 @@
  "strsim",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap"
-version = "4.1.11"
+version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42dfd32784433290c51d92c438bb72ea5063797fc3cc9a21a8c4346bebbb2098"
+checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
 dependencies = [
- "bitflags 2.0.2",
- "clap_lex 0.3.3",
- "is-terminal",
+ "clap_builder",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
+dependencies = [
+ "anstream",
+ "anstyle 1.0.0",
+ "bitflags 1.3.2",
+ "clap_lex 0.4.1",
  "once_cell",
  "strsim",
- "termcolor",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.3.3"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "033f6b7a4acb1f358c742aaca805c939ee73b4c6209ae4318ec7aca81c42e646"
-dependencies = [
- "os_str_bytes",
-]
+checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
 
 [[package]]
 name = "codespan-reporting"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "combine"
 version = "4.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
 dependencies = [
  "bytes",
  "futures-core",
@@ -652,20 +735,39 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "concurrent_arena"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24bfeb060a299f86521bb3940344800fc861cc506356e44a273a42cb552afde5"
+dependencies = [
+ "arc-swap",
+ "array-init",
+ "const_fn_assert",
+ "parking_lot 0.12.1",
+ "triomphe",
+]
+
+[[package]]
 name = "const-oid"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
 
 [[package]]
+name = "const_fn_assert"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "27d614f23f34f7b5165a77dc1591f497e2518f9cec4b4f4b92bfc4dc6cf7a190"
+
+[[package]]
 name = "convert_case"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
 dependencies = [
  "unicode-segmentation",
 ]
@@ -930,14 +1032,25 @@
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
+name = "derive_destructure2"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "35cb7e5875e1028a73e551747d6d0118f25c3d6dbba2dadf97cc0f4d0c53f2f5"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
 [[package]]
 name = "difflib"
@@ -955,19 +1068,39 @@
  "const-oid",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dirs"
+version = "4.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+dependencies = [
+ "dirs-sys 0.3.7",
+]
+
+[[package]]
+name = "dirs"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
 dependencies = [
- "dirs-sys",
+ "dirs-sys 0.4.0",
+]
+
+[[package]]
+name = "dirs-sys"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
 ]
 
 [[package]]
 name = "dirs-sys"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04414300db88f70d74c5ff54e50f9e1d1737d9a5b90f53fcf2e95ca2a9ab554b"
@@ -1139,59 +1272,59 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "531ac96c6ff5fd7c62263c5e3c67a603af4fcaee2e1a0ae5565ba3a11e69e549"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1997dd9df74cdac935c76252744c1ed5794fac083242ea4fe77ef3ed60ba0f83"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-lite"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
 dependencies = [
@@ -1202,46 +1335,46 @@
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-timer"
 version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64b03909df88034c26dc1547e8970b91f98bdb65165d6a4e9110d94263dbb2c"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -2021,24 +2154,14 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
-name = "mime_guess"
-version = "2.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
-dependencies = [
- "mime",
- "unicase",
-]
-
-[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "minitrace"
@@ -2247,14 +2370,25 @@
  "num-traits",
  "rand 0.8.5",
  "smallvec",
  "zeroize",
 ]
 
 [[package]]
+name = "num-derive"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
@@ -2289,19 +2423,19 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.33.2"
+version = "0.33.3"
 dependencies = [
  "anyhow",
- "clap 4.1.11",
- "dirs",
+ "clap 4.2.5",
+ "dirs 5.0.0",
  "env_logger",
  "futures",
  "log",
  "opendal",
  "serde",
  "tokio",
  "toml 0.7.3",
@@ -2326,32 +2460,32 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.33.2"
+version = "0.33.3"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.33.2"
+version = "0.33.3"
 dependencies = [
  "anyhow",
  "assert_cmd",
- "clap 4.1.11",
- "dirs",
+ "clap 4.2.5",
+ "dirs 5.0.0",
  "env_logger",
  "futures",
  "log",
  "opendal",
  "predicates 2.1.5",
  "serde",
  "tokio",
@@ -2369,25 +2503,24 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.33.2"
+version = "0.33.3"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
  "bb8",
  "bytes",
- "cfg-if",
  "chrono",
  "criterion",
  "dashmap",
  "dotenvy",
  "env_logger",
  "flagset",
  "futures",
@@ -2398,16 +2531,19 @@
  "log",
  "madsim",
  "md-5",
  "metrics",
  "minitrace",
  "moka",
  "once_cell",
+ "openssh",
+ "openssh-sftp-client",
  "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
+ "owning_ref",
  "parking_lot 0.12.1",
  "paste",
  "percent-encoding",
  "pin-project",
  "pretty_assertions",
  "prometheus",
  "prost",
@@ -2449,26 +2585,26 @@
  "once_cell",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.33.2"
+version = "0.33.3"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.33.2"
+version = "0.33.3"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
@@ -2481,14 +2617,103 @@
  "magnus",
  "opendal",
  "rb-sys",
  "rb-sys-env",
 ]
 
 [[package]]
+name = "openssh"
+version = "0.9.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ca6c277973fb549b36dd8980941b5ea3ecebea026f5b1f0060acde74d893c22"
+dependencies = [
+ "dirs 4.0.0",
+ "libc",
+ "once_cell",
+ "shell-escape",
+ "tempfile",
+ "thiserror",
+ "tokio",
+ "tokio-pipe",
+]
+
+[[package]]
+name = "openssh-sftp-client"
+version = "0.12.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa8e5f26e549bd266d9bcd9e5b4fd344729985ef1a7f5ac3e51f3f96a4a620"
+dependencies = [
+ "bytes",
+ "derive_destructure2",
+ "once_cell",
+ "openssh-sftp-client-lowlevel",
+ "openssh-sftp-error",
+ "scopeguard",
+ "tokio",
+ "tokio-io-utility",
+ "tokio-util",
+]
+
+[[package]]
+name = "openssh-sftp-client-lowlevel"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "406bf41d8372365497d5645e802a8dfe22008b8183edbe6c79e4b75614431daa"
+dependencies = [
+ "awaitable",
+ "bytes",
+ "concurrent_arena",
+ "derive_destructure2",
+ "openssh-sftp-error",
+ "openssh-sftp-protocol",
+ "pin-project",
+ "tokio",
+ "tokio-io-utility",
+]
+
+[[package]]
+name = "openssh-sftp-error"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d836b428ead150165d1178ed0aa672791c13b3ae9616ea1e34d13730a2cb486"
+dependencies = [
+ "awaitable-error",
+ "openssh-sftp-protocol-error",
+ "ssh_format_error",
+ "thiserror",
+ "tokio",
+]
+
+[[package]]
+name = "openssh-sftp-protocol"
+version = "0.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf38532d784978966f95d241226223823f351d5bb2a4bebcf6b20b9cb1e393e0"
+dependencies = [
+ "bitflags 2.0.2",
+ "num-derive",
+ "num-traits",
+ "openssh-sftp-protocol-error",
+ "serde",
+ "ssh_format",
+ "vec-strings",
+]
+
+[[package]]
+name = "openssh-sftp-protocol-error"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0719269eb3f037866ae07ec89cb44ed2c1d63b72b2390cef8e1aa3016a956ff8"
+dependencies = [
+ "serde",
+ "thiserror",
+ "vec-strings",
+]
+
+[[package]]
 name = "openssl"
 version = "0.10.47"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8b277f87dacc05a6b709965d1cbafac4649d6ce9f3ce9ceb88508b5666dfec9"
 dependencies = [
  "bitflags 1.3.2",
  "cfg-if",
@@ -2663,14 +2888,23 @@
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
+name = "owning_ref"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ff55baddef9e4ad00f88b6c743a2a8062d4c6ade126c2a528644b8e444d52ce"
+dependencies = [
+ "stable_deref_trait",
+]
+
+[[package]]
 name = "parking"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
 
 [[package]]
 name = "parking_lot"
@@ -2888,15 +3122,15 @@
 
 [[package]]
 name = "predicates"
 version = "3.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ba7d6ead3e3966038f68caa9fc1f860185d95a793180bbcfe0d0da47b3961ed"
 dependencies = [
- "anstyle",
+ "anstyle 0.3.5",
  "difflib",
  "itertools",
  "predicates-core",
 ]
 
 [[package]]
 name = "predicates-core"
@@ -3370,15 +3604,15 @@
 checksum = "3875de6d7d0468315194cb8332913aae0d6803cfd5c7f089dc174ff5350f7b29"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.0",
  "bytes",
  "chrono",
- "dirs",
+ "dirs 5.0.0",
  "form_urlencoded",
  "hex",
  "hmac",
  "http",
  "jsonwebtoken",
  "log",
  "once_cell",
@@ -3412,15 +3646,14 @@
  "hyper",
  "hyper-rustls",
  "hyper-tls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
- "mime_guess",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
  "rustls 0.20.8",
  "rustls-native-certs",
  "rustls-pemfile",
@@ -3788,14 +4021,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
+name = "shell-escape"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "45bb67a18fa91266cc7807181f62f9178a6873bfad7dc788c42e6430db40184f"
+
+[[package]]
 name = "shell-words"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24188a676b6ae68c3b2cb3a01be17fbf7240ce009799bb56d5b1409051e78fde"
 
 [[package]]
 name = "shlex"
@@ -3940,14 +4179,40 @@
 checksum = "67cf02bbac7a337dc36e4f5a693db6c21e7863f45070f7064577eb4367a3212b"
 dependencies = [
  "base64ct",
  "der",
 ]
 
 [[package]]
+name = "ssh_format"
+version = "0.14.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24ab31081d1c9097c327ec23550858cb5ffb4af6b866c1ef4d728455f01f3304"
+dependencies = [
+ "bytes",
+ "serde",
+ "ssh_format_error",
+]
+
+[[package]]
+name = "ssh_format_error"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "be3c6519de7ca611f71ef7e8a56eb57aa1c818fecb5242d0a0f39c83776c210c"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "stable_deref_trait"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
+
+[[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "subtle"
@@ -4035,14 +4300,20 @@
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
+name = "thin-vec"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aac81b6fd6beb5884b0cf3321b8117e6e5d47ecb6fc89f414cfdcca8b2fe2dd8"
+
+[[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
@@ -4169,14 +4440,24 @@
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "tokio-io-utility"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d672654d175710e52c7c41f6aec77c62b3c0954e2a7ebce9049d1e94ed7c263"
+dependencies = [
+ "bytes",
+ "tokio",
+]
+
+[[package]]
 name = "tokio-macros"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -4190,29 +4471,39 @@
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
+name = "tokio-pipe"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f213a84bffbd61b8fa0ba8a044b4bbe35d471d0b518867181e82bd5c15542784"
+dependencies = [
+ "libc",
+ "tokio",
+]
+
+[[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
 dependencies = [
  "rustls 0.20.8",
  "tokio",
  "webpki 0.22.0",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -4344,14 +4635,19 @@
 ]
 
 [[package]]
 name = "triomphe"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1ee9bd9239c339d714d657fac840c6d2a4f9c45f4f9ec7b0975113458be78db"
+dependencies = [
+ "arc-swap",
+ "serde",
+ "stable_deref_trait",
+]
 
 [[package]]
 name = "trust-dns-proto"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f7f83d1e4a0e4358ac54c5c3681e5d7da5efc5a7a632c90bb6d6669ddd9bc26"
 dependencies = [
@@ -4475,14 +4771,20 @@
 [[package]]
 name = "urlencoding"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "uuid"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
 dependencies = [
  "getrandom 0.2.8",
  "serde",
@@ -4507,14 +4809,24 @@
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
+name = "vec-strings"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c8509489e2a7ee219522238ad45fd370bec6808811ac15ac6b07453804e77659"
+dependencies = [
+ "serde",
+ "thin-vec",
+]
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wait-timeout"
@@ -4732,99 +5044,165 @@
 
 [[package]]
 name = "windows"
 version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winnow"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
 dependencies = [
  "memchr",
 ]
```

### Comparing `opendal-0.33.2/PKG-INFO` & `opendal-0.33.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.33.2
+Version: 0.33.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: pdoc; extra == 'docs'
-Requires-Dist: behave; extra == 'test'
-Requires-Dist: gevent; extra == 'benchmark'
-Requires-Dist: greenify; extra == 'benchmark'
-Requires-Dist: greenlet; extra == 'benchmark'
-Requires-Dist: boto3; extra == 'benchmark'
-Requires-Dist: pydantic; extra == 'benchmark'
-Requires-Dist: boto3-stubs[essential]; extra == 'benchmark'
+Requires-Dist: gevent ; extra == 'benchmark'
+Requires-Dist: greenify ; extra == 'benchmark'
+Requires-Dist: greenlet ; extra == 'benchmark'
+Requires-Dist: boto3 ; extra == 'benchmark'
+Requires-Dist: pydantic ; extra == 'benchmark'
+Requires-Dist: boto3-stubs[essential] ; extra == 'benchmark'
+Requires-Dist: pdoc ; extra == 'docs'
+Requires-Dist: behave ; extra == 'test'
+Provides-Extra: benchmark
 Provides-Extra: docs
 Provides-Extra: test
-Provides-Extra: benchmark
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 Project-URL: Homepage, https://opendal.apache.org/
 Project-URL: Repository, https://github.com/apache/incubator-opendal
-Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 
 # OpenDAL Python Binding
 
 Documentation: [main](https://opendal.apache.org/docs/python/)
 
 This crate intends to build a native python binding.
```

