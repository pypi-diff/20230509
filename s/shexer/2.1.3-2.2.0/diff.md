# Comparing `tmp/shexer-2.1.3.tar.gz` & `tmp/shexer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.1.3.tar", last modified: Wed May  3 18:38:14 2023, max compression
+gzip compressed data, was "shexer-2.2.0.tar", last modified: Tue May  9 18:26:37 2023, max compression
```

## Comparing `shexer-2.1.3.tar` & `shexer-2.2.0.tar`

### file list

```diff
@@ -1,239 +1,242 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.887637 shexer-2.1.3/
--rw-rw-rw-   0        0        0    11558 2019-11-23 19:24:24.000000 shexer-2.1.3/LICENSE
--rw-rw-rw-   0        0        0    26626 2023-05-03 18:38:14.887958 shexer-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    25710 2023-05-03 18:36:37.000000 shexer-2.1.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-03 18:38:14.890637 shexer-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1392 2023-05-03 18:37:15.000000 shexer-2.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.640580 shexer-2.1.3/shexer/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/__init__.py
--rw-rw-rw-   0        0        0      644 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/consts.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.683448 shexer-2.1.3/shexer/core/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.757293 shexer-2.1.3/shexer/core/instances/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/__init__.py
--rw-rw-rw-   0        0        0      713 2021-10-25 09:34:37.000000 shexer-2.1.3/shexer/core/instances/abstract_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.833421 shexer-2.1.3/shexer/core/instances/annotators/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/annotators/__init__.py
--rw-rw-rw-   0        0        0      383 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/annotator_func.py
--rw-rw-rw-   0        0        0     1817 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-rw-rw-   0        0        0     3198 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/annotators/base_annotator.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.926403 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/
--rw-rw-rw-   0        0        0        0 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-rw-rw-   0        0        0      688 2021-10-25 09:34:37.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-rw-rw-   0        0        0      592 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-rw-rw-   0        0        0      807 2021-01-14 17:50:11.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-rw-rw-   0        0        0     1793 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0      830 2021-10-25 09:34:37.000000 shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-rw-rw-   0        0        0     4260 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.938404 shexer-2.1.3/shexer/core/instances/mappings/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/mappings/__init__.py
--rw-rw-rw-   0        0        0     1081 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.958403 shexer-2.1.3/shexer/core/instances/mix/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/mix/__init__.py
--rw-rw-rw-   0        0        0     2652 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-rw-rw-   0        0        0       22 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/core/instances/pconsts.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.020357 shexer-2.1.3/shexer/core/profiling/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/profiling/__init__.py
--rw-rw-rw-   0        0        0     8614 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/class_profiler.py
--rw-rw-rw-   0        0        0      182 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/profiling/consts.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.102592 shexer-2.1.3/shexer/core/profiling/strategy/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/profiling/strategy/__init__.py
--rw-rw-rw-   0        0        0     6976 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-rw-rw-   0        0        0     1349 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-rw-rw-   0        0        0     7395 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.107272 shexer-2.1.3/shexer/core/shexing/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/shexing/__init__.py
--rw-rw-rw-   0        0        0     6191 2023-05-03 17:48:10.000000 shexer-2.1.3/shexer/core/shexing/class_shexer.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.185346 shexer-2.1.3/shexer/core/shexing/strategy/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/core/shexing/strategy/__init__.py
--rw-rw-rw-   0        0        0    17141 2023-05-03 17:48:10.000000 shexer-2.1.3/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-rw-rw-   0        0        0     5685 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-rw-rw-   0        0        0     2804 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.227464 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-rw-rw-   0        0        0        0 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-rw-rw-   0        0        0      118 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-rw-rw-   0        0        0     1088 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-rw-rw-   0        0        0      412 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.250502 shexer-2.1.3/shexer/io/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/__init__.py
--rw-rw-rw-   0        0        0      103 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.252471 shexer-2.1.3/shexer/io/graph/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.529347 shexer-2.1.3/shexer/io/graph/yielder/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/__init__.py
--rw-rw-rw-   0        0        0     1431 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/base_triples_yielder.py
--rw-rw-rw-   0        0        0    16303 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.555857 shexer-2.1.3/shexer/io/graph/yielder/filter/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/filter/__init__.py
--rw-rw-rw-   0        0        0      862 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-rw-rw-   0        0        0     1131 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-rw-rw-   0        0        0     1132 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1757 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-rw-rw-   0        0        0     1166 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     2674 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-rw-rw-   0        0        0     5686 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-rw-rw-   0        0        0     6817 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.592572 shexer-2.1.3/shexer/io/graph/yielder/remote/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/graph/yielder/remote/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-04-03 18:35:42.000000 shexer-2.1.3/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-rw-rw-   0        0        0     4724 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.607178 shexer-2.1.3/shexer/io/json/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/json/__init__.py
--rw-rw-rw-   0        0        0      207 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/json/json_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.649582 shexer-2.1.3/shexer/io/line_reader/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/line_reader/__init__.py
--rw-rw-rw-   0        0        0      285 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/io/line_reader/file_line_reader.py
--rw-rw-rw-   0        0        0      332 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/line_reader/gz_line_reader.py
--rw-rw-rw-   0        0        0      260 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/line_reader/raw_string_line_reader.py
--rw-rw-rw-   0        0        0      353 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/io/line_reader/zip_file_line_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.652583 shexer-2.1.3/shexer/io/profile/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.664212 shexer-2.1.3/shexer/io/profile/formater/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/profile/formater/__init__.py
--rw-rw-rw-   0        0        0      409 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.666675 shexer-2.1.3/shexer/io/shacl/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/shacl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.689185 shexer-2.1.3/shexer/io/shacl/formater/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/shacl/formater/__init__.py
--rw-rw-rw-   0        0        0    15833 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/io/shacl/formater/shacl_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.714186 shexer-2.1.3/shexer/io/shape_map/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.740196 shexer-2.1.3/shexer/io/shape_map/label/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/label/__init__.py
--rw-rw-rw-   0        0        0     1410 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.775381 shexer-2.1.3/shexer/io/shape_map/node_selector/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/node_selector/__init__.py
--rw-rw-rw-   0        0        0     6755 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-rw-rw-   0        0        0     4966 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shape_map/shape_map_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.777197 shexer-2.1.3/shexer/io/shex/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.809260 shexer-2.1.3/shexer/io/shex/formater/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shex/formater/__init__.py
--rw-rw-rw-   0        0        0      244 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/io/shex/formater/consts.py
--rw-rw-rw-   0        0        0     7006 2023-04-07 09:41:11.000000 shexer-2.1.3/shexer/io/shex/formater/shex_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:13.947403 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-04-13 17:29:20.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-rw-rw-   0        0        0     2287 2023-02-03 19:09:46.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.023201 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-rw-rw-   0        0        0        0 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-rw-rw-   0        0        0      383 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-rw-rw-   0        0        0      171 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-rw-rw-   0        0        0      887 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-rw-rw-   0        0        0     1278 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-rw-rw-   0        0        0     1500 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-rw-rw-   0        0        0     3211 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.051487 shexer-2.1.3/shexer/io/sparql/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/io/sparql/__init__.py
--rw-rw-rw-   0        0        0     4538 2022-07-15 19:02:46.000000 shexer-2.1.3/shexer/io/sparql/query.py
--rw-rw-rw-   0        0        0      469 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/io/wikidata.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.238240 shexer-2.1.3/shexer/model/
--rw-rw-rw-   0        0        0      552 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/IRI.py
--rw-rw-rw-   0        0        0      280 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/Literal.py
--rw-rw-rw-   0        0        0      810 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/model/Macro.py
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/__init__.py
--rw-rw-rw-   0        0        0      502 2021-10-04 17:33:25.000000 shexer-2.1.3/shexer/model/bnode.py
--rw-rw-rw-   0        0        0      100 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/const_elem_types.py
--rw-rw-rw-   0        0        0     1119 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/model/fixed_prop_choice_statement.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.310935 shexer-2.1.3/shexer/model/graph/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/graph/__init__.py
--rw-rw-rw-   0        0        0     6186 2022-07-15 19:02:46.000000 shexer-2.1.3/shexer/model/graph/abstract_sgraph.py
--rw-rw-rw-   0        0        0     7633 2023-04-04 10:53:17.000000 shexer-2.1.3/shexer/model/graph/endpoint_sgraph.py
--rw-rw-rw-   0        0        0     6201 2023-04-04 17:24:52.000000 shexer-2.1.3/shexer/model/graph/rdflib_sgraph.py
--rw-rw-rw-   0        0        0     4173 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/hierarchy_tree.py
--rw-rw-rw-   0        0        0     2527 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/node_selector.py
--rw-rw-rw-   0        0        0      427 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/property.py
--rw-rw-rw-   0        0        0     3361 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/model/shape.py
--rw-rw-rw-   0        0        0      858 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/model/shape_map.py
--rw-rw-rw-   0        0        0     2716 2023-02-02 16:28:05.000000 shexer-2.1.3/shexer/model/statement.py
--rw-rw-rw-   0        0        0    24509 2023-05-03 18:36:37.000000 shexer-2.1.3/shexer/shaper.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.492195 shexer-2.1.3/shexer/utils/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/__init__.py
--rw-rw-rw-   0        0        0      621 2022-08-11 11:37:45.000000 shexer-2.1.3/shexer/utils/compression.py
--rw-rw-rw-   0        0        0       94 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/dict.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.677481 shexer-2.1.3/shexer/utils/factories/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/factories/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/utils/factories/class_profiler_factory.py
--rw-rw-rw-   0        0        0     2322 2023-05-03 18:36:37.000000 shexer-2.1.3/shexer/utils/factories/class_shexer_factory.py
--rw-rw-rw-   0        0        0      728 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/factories/h_tree.py
--rw-rw-rw-   0        0        0    12215 2023-04-04 10:53:17.000000 shexer-2.1.3/shexer/utils/factories/instance_tracker_factory.py
--rw-rw-rw-   0        0        0      437 2021-10-03 10:32:18.000000 shexer-2.1.3/shexer/utils/factories/iri_factory.py
--rw-rw-rw-   0        0        0      286 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/utils/factories/remote_graph_factory.py
--rw-rw-rw-   0        0        0     1985 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/utils/factories/shape_map_factory.py
--rw-rw-rw-   0        0        0      616 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/factories/shape_map_parser_factory.py
--rw-rw-rw-   0        0        0     1723 2023-04-06 19:32:13.000000 shexer-2.1.3/shexer/utils/factories/shape_serializer_factory.py
--rw-rw-rw-   0        0        0    18627 2023-04-04 10:53:17.000000 shexer-2.1.3/shexer/utils/factories/triple_yielders_factory.py
--rw-rw-rw-   0        0        0      123 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/file.py
--rw-rw-rw-   0        0        0      397 2021-10-04 17:33:25.000000 shexer-2.1.3/shexer/utils/log.py
--rw-rw-rw-   0        0        0      803 2021-01-14 17:50:12.000000 shexer-2.1.3/shexer/utils/namespaces.py
--rw-rw-rw-   0        0        0      967 2019-11-23 19:24:28.000000 shexer-2.1.3/shexer/utils/obj_references.py
--rw-rw-rw-   0        0        0     2008 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/utils/shapes.py
--rw-rw-rw-   0        0        0     1397 2022-03-28 20:28:03.000000 shexer-2.1.3/shexer/utils/target_elements.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.708407 shexer-2.1.3/shexer/utils/translators/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.3/shexer/utils/translators/__init__.py
--rw-rw-rw-   0        0        0     2881 2021-04-26 09:52:52.000000 shexer-2.1.3/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-rw-rw-   0        0        0     3026 2023-04-03 15:39:42.000000 shexer-2.1.3/shexer/utils/triple_yielders.py
--rw-rw-rw-   0        0        0     5708 2023-04-13 17:29:20.000000 shexer-2.1.3/shexer/utils/uri.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:12.681762 shexer-2.1.3/shexer.egg-info/
--rw-rw-rw-   0        0        0    26626 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7817 2023-05-03 18:38:11.000000 shexer-2.1.3/shexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 18:38:10.000000 shexer-2.1.3/shexer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.829539 shexer-2.1.3/test/
--rw-rw-rw-   0        0        0        0 2021-01-14 17:50:12.000000 shexer-2.1.3/test/__init__.py
--rw-rw-rw-   0        0        0     1903 2021-11-20 10:36:36.000000 shexer-2.1.3/test/const.py
--rw-rw-rw-   0        0        0     8963 2023-04-03 18:35:42.000000 shexer-2.1.3/test/t_utils.py
--rw-rw-rw-   0        0        0     1488 2022-08-10 11:13:26.000000 shexer-2.1.3/test/test_all_classes_mode.py
--rw-rw-rw-   0        0        0     1525 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_allow_opt_cardinality.py
--rw-rw-rw-   0        0        0     3541 2023-05-03 18:36:37.000000 shexer-2.1.3/test/test_allow_redundant_or.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.836265 shexer-2.1.3/test/test_bugs/
--rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_bugs/__init__.py
--rw-rw-rw-   0        0        0      796 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-rw-rw-   0        0        0     1192 2023-04-13 17:29:20.000000 shexer-2.1.3/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
--rw-rw-rw-   0        0        0     9920 2022-08-11 11:37:45.000000 shexer-2.1.3/test/test_compression_mode.py
--rw-rw-rw-   0        0        0     2171 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_decimals.py
--rw-rw-rw-   0        0        0     5564 2023-04-03 18:13:21.000000 shexer-2.1.3/test/test_depth_for_building_subgraph.py
--rw-rw-rw-   0        0        0     3526 2023-05-03 18:36:37.000000 shexer-2.1.3/test/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0     1388 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_disable_comments.py
--rw-rw-rw-   0        0        0     2922 2023-04-04 10:53:17.000000 shexer-2.1.3/test/test_disable_endpoint_cache.py
--rw-rw-rw-   0        0        0     1491 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_disable_exact_cardinality.py
--rw-rw-rw-   0        0        0     2557 2023-05-03 18:36:37.000000 shexer-2.1.3/test/test_disable_or_statements.py
--rw-rw-rw-   0        0        0     3786 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_discard_and_compliant.py
--rw-rw-rw-   0        0        0     2090 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_file_target_classes.py
--rw-rw-rw-   0        0        0     1677 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_graph_file_input.py
--rw-rw-rw-   0        0        0     3456 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_graph_list_of_file_inputs.py
--rw-rw-rw-   0        0        0     1951 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_infer_numeric_types_for_untyped_literals.py
--rw-rw-rw-   0        0        0     7818 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_input_format.py
--rw-rw-rw-   0        0        0     3367 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_instances_file_input.py
--rw-rw-rw-   0        0        0     3852 2023-02-02 16:28:05.000000 shexer-2.1.3/test/test_instances_report.py
--rw-rw-rw-   0        0        0     3548 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_instantiation_property.py
--rw-rw-rw-   0        0        0     1964 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_inverse_paths.py
--rw-rw-rw-   0        0        0     3594 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_keep_less_specific.py
--rw-rw-rw-   0        0        0     4051 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_list_of_url_input.py
--rw-rw-rw-   0        0        0     4106 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_namespaces_dict.py
--rw-rw-rw-   0        0        0     2082 2023-04-13 17:23:12.000000 shexer-2.1.3/test/test_namespaces_to_ignore.py
--rw-rw-rw-   0        0        0     5000 2021-01-14 17:50:12.000000 shexer-2.1.3/test/test_raw_graph.py
--rw-rw-rw-   0        0        0     4300 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_raw_shape_map.py
--rw-rw-rw-   0        0        0     1711 2022-07-15 19:02:46.000000 shexer-2.1.3/test/test_rdflib_graph.py
--rw-rw-rw-   0        0        0     2930 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_remove_empty_sahpes.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.848264 shexer-2.1.3/test/test_shacl/
--rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.1.3/test/test_shacl/__init__.py
--rw-rw-rw-   0        0        0     2225 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shacl/test_annotation.py
--rw-rw-rw-   0        0        0     2242 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shacl/test_class_selection.py
--rw-rw-rw-   0        0        0     3291 2023-04-06 19:32:13.000000 shexer-2.1.3/test/test_shacl/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0      910 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_shacl/test_literal_types.py
--rw-rw-rw-   0        0        0     4313 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shape_map_file.py
--rw-rw-rw-   0        0        0     6086 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shape_map_format.py
--rw-rw-rw-   0        0        0     2307 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0     2889 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_shapes_namespaces.py
--rw-rw-rw-   0        0        0     2452 2022-03-28 20:28:03.000000 shexer-2.1.3/test/test_sort.py
--rw-rw-rw-   0        0        0     2058 2021-10-24 17:07:37.000000 shexer-2.1.3/test/test_target_classes.py
--rw-rw-rw-   0        0        0     3120 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_threshold.py
--rw-rw-rw-   0        0        0     2578 2023-04-03 18:13:27.000000 shexer-2.1.3/test/test_url_endpoint.py
--rw-rw-rw-   0        0        0     1867 2022-07-15 19:02:46.000000 shexer-2.1.3/test/test_url_graph.py
--rw-rw-rw-   0        0        0     1900 2021-10-03 10:32:18.000000 shexer-2.1.3/test/test_wikidata_annotation.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:38:14.885639 shexer-2.1.3/ws/
--rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.1.3/ws/__init__.py
--rw-rw-rw-   0        0        0    19884 2022-03-28 20:28:03.000000 shexer-2.1.3/ws/shexer_rest.py
--rw-rw-rw-   0        0        0       28 2019-11-23 19:24:29.000000 shexer-2.1.3/ws/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.411786 shexer-2.2.0/
+-rw-rw-rw-   0        0        0    11558 2019-11-23 19:24:24.000000 shexer-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0    27276 2023-05-09 18:26:37.412785 shexer-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26360 2023-05-09 18:25:27.000000 shexer-2.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-09 18:26:37.415783 shexer-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-05-09 18:25:27.000000 shexer-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.040785 shexer-2.2.0/shexer/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/consts.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.082785 shexer-2.2.0/shexer/core/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.116782 shexer-2.2.0/shexer/core/instances/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/core/instances/__init__.py
+-rw-rw-rw-   0        0        0      713 2021-10-25 09:34:37.000000 shexer-2.2.0/shexer/core/instances/abstract_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.177786 shexer-2.2.0/shexer/core/instances/annotators/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/core/instances/annotators/__init__.py
+-rw-rw-rw-   0        0        0      383 2021-01-14 17:50:11.000000 shexer-2.2.0/shexer/core/instances/annotators/annotator_func.py
+-rw-rw-rw-   0        0        0     1817 2021-01-14 17:50:11.000000 shexer-2.2.0/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-rw-rw-   0        0        0     3895 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/annotators/base_annotator.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.251824 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/
+-rw-rw-rw-   0        0        0        0 2021-01-14 17:50:11.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-rw-rw-   0        0        0      665 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-rw-rw-   0        0        0      760 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-rw-rw-   0        0        0      807 2021-01-14 17:50:11.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-rw-rw-   0        0        0     2675 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
+-rw-rw-rw-   0        0        0       86 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
+-rw-rw-rw-   0        0        0     1793 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0      815 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-rw-rw-   0        0        0     4553 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/core/instances/instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.263784 shexer-2.2.0/shexer/core/instances/mappings/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/core/instances/mappings/__init__.py
+-rw-rw-rw-   0        0        0     1081 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.285787 shexer-2.2.0/shexer/core/instances/mix/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/core/instances/mix/__init__.py
+-rw-rw-rw-   0        0        0     2652 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-rw-rw-   0        0        0       22 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/core/instances/pconsts.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.317784 shexer-2.2.0/shexer/core/profiling/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/profiling/__init__.py
+-rw-rw-rw-   0        0        0     8614 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/profiling/class_profiler.py
+-rw-rw-rw-   0        0        0      182 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/profiling/consts.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.377797 shexer-2.2.0/shexer/core/profiling/strategy/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/profiling/strategy/__init__.py
+-rw-rw-rw-   0        0        0     6976 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-rw-rw-   0        0        0     1349 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-rw-rw-   0        0        0     7395 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.381783 shexer-2.2.0/shexer/core/shexing/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/shexing/__init__.py
+-rw-rw-rw-   0        0        0     6191 2023-05-03 18:39:33.000000 shexer-2.2.0/shexer/core/shexing/class_shexer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.436787 shexer-2.2.0/shexer/core/shexing/strategy/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/core/shexing/strategy/__init__.py
+-rw-rw-rw-   0        0        0    17141 2023-05-03 18:39:33.000000 shexer-2.2.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-rw-rw-   0        0        0     5685 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-rw-rw-   0        0        0     2804 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.495787 shexer-2.2.0/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-rw-rw-   0        0        0        0 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-rw-rw-   0        0        0     1088 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-rw-rw-   0        0        0      412 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.512812 shexer-2.2.0/shexer/io/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/__init__.py
+-rw-rw-rw-   0        0        0      103 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/io/file.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.514784 shexer-2.2.0/shexer/io/graph/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.746787 shexer-2.2.0/shexer/io/graph/yielder/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/graph/yielder/__init__.py
+-rw-rw-rw-   0        0        0     1431 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-rw-rw-   0        0        0    16303 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.772784 shexer-2.2.0/shexer/io/graph/yielder/filter/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/graph/yielder/filter/__init__.py
+-rw-rw-rw-   0        0        0      862 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-rw-rw-   0        0        0     1131 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-rw-rw-   0        0        0     1132 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1757 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-rw-rw-   0        0        0     1166 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     2674 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-rw-rw-   0        0        0     5686 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     6817 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.800845 shexer-2.2.0/shexer/io/graph/yielder/remote/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/graph/yielder/remote/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-04-03 18:35:42.000000 shexer-2.2.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-rw-rw-   0        0        0     4724 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.812823 shexer-2.2.0/shexer/io/json/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/json/__init__.py
+-rw-rw-rw-   0        0        0      207 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/json/json_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.849824 shexer-2.2.0/shexer/io/line_reader/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/line_reader/__init__.py
+-rw-rw-rw-   0        0        0      285 2021-01-14 17:50:12.000000 shexer-2.2.0/shexer/io/line_reader/file_line_reader.py
+-rw-rw-rw-   0        0        0      332 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/line_reader/gz_line_reader.py
+-rw-rw-rw-   0        0        0      260 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/line_reader/raw_string_line_reader.py
+-rw-rw-rw-   0        0        0      353 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/io/line_reader/zip_file_line_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.851784 shexer-2.2.0/shexer/io/profile/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.862786 shexer-2.2.0/shexer/io/profile/formater/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/profile/formater/__init__.py
+-rw-rw-rw-   0        0        0      409 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.864783 shexer-2.2.0/shexer/io/shacl/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/io/shacl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.902786 shexer-2.2.0/shexer/io/shacl/formater/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/io/shacl/formater/__init__.py
+-rw-rw-rw-   0        0        0    15833 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/io/shacl/formater/shacl_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.924784 shexer-2.2.0/shexer/io/shape_map/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shape_map/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.974824 shexer-2.2.0/shexer/io/shape_map/label/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shape_map/label/__init__.py
+-rw-rw-rw-   0        0        0     1410 2021-01-14 17:50:12.000000 shexer-2.2.0/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.992784 shexer-2.2.0/shexer/io/shape_map/node_selector/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shape_map/node_selector/__init__.py
+-rw-rw-rw-   0        0        0     6755 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-rw-rw-   0        0        0     4966 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shape_map/shape_map_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.994799 shexer-2.2.0/shexer/io/shex/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.005786 shexer-2.2.0/shexer/io/shex/formater/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shex/formater/__init__.py
+-rw-rw-rw-   0        0        0      244 2021-01-14 17:50:12.000000 shexer-2.2.0/shexer/io/shex/formater/consts.py
+-rw-rw-rw-   0        0        0     7006 2023-04-07 09:41:11.000000 shexer-2.2.0/shexer/io/shex/formater/shex_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.098826 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-rw-rw-   0        0        0     6083 2023-04-13 17:29:20.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-rw-rw-   0        0        0     2287 2023-02-03 19:09:46.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.183790 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-rw-rw-   0        0        0        0 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-rw-rw-   0        0        0      171 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-rw-rw-   0        0        0      887 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-rw-rw-   0        0        0     1278 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-rw-rw-   0        0        0     1500 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-rw-rw-   0        0        0     3211 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.203792 shexer-2.2.0/shexer/io/sparql/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/io/sparql/__init__.py
+-rw-rw-rw-   0        0        0     4538 2022-07-15 19:02:46.000000 shexer-2.2.0/shexer/io/sparql/query.py
+-rw-rw-rw-   0        0        0      469 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/io/wikidata.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.406791 shexer-2.2.0/shexer/model/
+-rw-rw-rw-   0        0        0      552 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/IRI.py
+-rw-rw-rw-   0        0        0      280 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/Literal.py
+-rw-rw-rw-   0        0        0      810 2021-01-14 17:50:12.000000 shexer-2.2.0/shexer/model/Macro.py
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/__init__.py
+-rw-rw-rw-   0        0        0      502 2021-10-04 17:33:25.000000 shexer-2.2.0/shexer/model/bnode.py
+-rw-rw-rw-   0        0        0      100 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/const_elem_types.py
+-rw-rw-rw-   0        0        0     1119 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/model/fixed_prop_choice_statement.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.481784 shexer-2.2.0/shexer/model/graph/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/graph/__init__.py
+-rw-rw-rw-   0        0        0     6186 2022-07-15 19:02:46.000000 shexer-2.2.0/shexer/model/graph/abstract_sgraph.py
+-rw-rw-rw-   0        0        0     7633 2023-04-04 10:53:17.000000 shexer-2.2.0/shexer/model/graph/endpoint_sgraph.py
+-rw-rw-rw-   0        0        0     6201 2023-04-04 17:24:52.000000 shexer-2.2.0/shexer/model/graph/rdflib_sgraph.py
+-rw-rw-rw-   0        0        0     4173 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/hierarchy_tree.py
+-rw-rw-rw-   0        0        0     2527 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/node_selector.py
+-rw-rw-rw-   0        0        0      427 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/property.py
+-rw-rw-rw-   0        0        0     3361 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/model/shape.py
+-rw-rw-rw-   0        0        0      858 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/model/shape_map.py
+-rw-rw-rw-   0        0        0     2716 2023-02-02 16:28:05.000000 shexer-2.2.0/shexer/model/statement.py
+-rw-rw-rw-   0        0        0    24783 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/shaper.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:36.726783 shexer-2.2.0/shexer/utils/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/__init__.py
+-rw-rw-rw-   0        0        0      621 2022-08-11 11:37:45.000000 shexer-2.2.0/shexer/utils/compression.py
+-rw-rw-rw-   0        0        0       94 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/dict.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.079784 shexer-2.2.0/shexer/utils/factories/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/factories/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/utils/factories/class_profiler_factory.py
+-rw-rw-rw-   0        0        0     2322 2023-05-03 18:39:33.000000 shexer-2.2.0/shexer/utils/factories/class_shexer_factory.py
+-rw-rw-rw-   0        0        0      728 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/factories/h_tree.py
+-rw-rw-rw-   0        0        0    12338 2023-05-09 18:25:27.000000 shexer-2.2.0/shexer/utils/factories/instance_tracker_factory.py
+-rw-rw-rw-   0        0        0      437 2021-10-03 10:32:18.000000 shexer-2.2.0/shexer/utils/factories/iri_factory.py
+-rw-rw-rw-   0        0        0      286 2021-01-14 17:50:12.000000 shexer-2.2.0/shexer/utils/factories/remote_graph_factory.py
+-rw-rw-rw-   0        0        0     1985 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/utils/factories/shape_map_factory.py
+-rw-rw-rw-   0        0        0      616 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/factories/shape_map_parser_factory.py
+-rw-rw-rw-   0        0        0     1723 2023-04-06 19:32:13.000000 shexer-2.2.0/shexer/utils/factories/shape_serializer_factory.py
+-rw-rw-rw-   0        0        0    18627 2023-04-04 10:53:17.000000 shexer-2.2.0/shexer/utils/factories/triple_yielders_factory.py
+-rw-rw-rw-   0        0        0      123 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/file.py
+-rw-rw-rw-   0        0        0      397 2021-10-04 17:33:25.000000 shexer-2.2.0/shexer/utils/log.py
+-rw-rw-rw-   0        0        0      803 2021-01-14 17:50:12.000000 shexer-2.2.0/shexer/utils/namespaces.py
+-rw-rw-rw-   0        0        0      967 2019-11-23 19:24:28.000000 shexer-2.2.0/shexer/utils/obj_references.py
+-rw-rw-rw-   0        0        0     2008 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/utils/shapes.py
+-rw-rw-rw-   0        0        0     1397 2022-03-28 20:28:03.000000 shexer-2.2.0/shexer/utils/target_elements.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.189824 shexer-2.2.0/shexer/utils/translators/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.2.0/shexer/utils/translators/__init__.py
+-rw-rw-rw-   0        0        0     2881 2021-04-26 09:52:52.000000 shexer-2.2.0/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-rw-rw-   0        0        0     3026 2023-04-03 15:39:42.000000 shexer-2.2.0/shexer/utils/triple_yielders.py
+-rw-rw-rw-   0        0        0     5708 2023-04-13 17:29:20.000000 shexer-2.2.0/shexer/utils/uri.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:35.080797 shexer-2.2.0/shexer.egg-info/
+-rw-rw-rw-   0        0        0    27276 2023-05-09 18:26:33.000000 shexer-2.2.0/shexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7986 2023-05-09 18:26:33.000000 shexer-2.2.0/shexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 18:26:33.000000 shexer-2.2.0/shexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-09 18:26:33.000000 shexer-2.2.0/shexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 18:26:33.000000 shexer-2.2.0/shexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.342815 shexer-2.2.0/test/
+-rw-rw-rw-   0        0        0        0 2021-01-14 17:50:12.000000 shexer-2.2.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1903 2021-11-20 10:36:36.000000 shexer-2.2.0/test/const.py
+-rw-rw-rw-   0        0        0     8963 2023-04-03 18:35:42.000000 shexer-2.2.0/test/t_utils.py
+-rw-rw-rw-   0        0        0     1488 2022-08-10 11:13:26.000000 shexer-2.2.0/test/test_all_classes_mode.py
+-rw-rw-rw-   0        0        0     1525 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_allow_opt_cardinality.py
+-rw-rw-rw-   0        0        0     3541 2023-05-03 18:39:33.000000 shexer-2.2.0/test/test_allow_redundant_or.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.354819 shexer-2.2.0/test/test_bugs/
+-rw-rw-rw-   0        0        0        0 2022-03-28 20:28:03.000000 shexer-2.2.0/test/test_bugs/__init__.py
+-rw-rw-rw-   0        0        0      796 2022-03-28 20:28:03.000000 shexer-2.2.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-rw-rw-   0        0        0     1192 2023-04-13 17:29:20.000000 shexer-2.2.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-rw-rw-   0        0        0     9920 2022-08-11 11:37:45.000000 shexer-2.2.0/test/test_compression_mode.py
+-rw-rw-rw-   0        0        0     2171 2023-02-02 16:28:05.000000 shexer-2.2.0/test/test_decimals.py
+-rw-rw-rw-   0        0        0     5564 2023-04-03 18:13:21.000000 shexer-2.2.0/test/test_depth_for_building_subgraph.py
+-rw-rw-rw-   0        0        0     3526 2023-05-03 18:36:37.000000 shexer-2.2.0/test/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0     1388 2023-02-02 16:28:05.000000 shexer-2.2.0/test/test_disable_comments.py
+-rw-rw-rw-   0        0        0     2922 2023-04-04 10:53:17.000000 shexer-2.2.0/test/test_disable_endpoint_cache.py
+-rw-rw-rw-   0        0        0     1491 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_disable_exact_cardinality.py
+-rw-rw-rw-   0        0        0     2557 2023-05-03 18:39:33.000000 shexer-2.2.0/test/test_disable_or_statements.py
+-rw-rw-rw-   0        0        0     3786 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_discard_and_compliant.py
+-rw-rw-rw-   0        0        0     2090 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_file_target_classes.py
+-rw-rw-rw-   0        0        0     1677 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_graph_file_input.py
+-rw-rw-rw-   0        0        0     3456 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_graph_list_of_file_inputs.py
+-rw-rw-rw-   0        0        0     1951 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-rw-rw-   0        0        0     7818 2023-02-02 16:28:05.000000 shexer-2.2.0/test/test_input_format.py
+-rw-rw-rw-   0        0        0     4648 2023-05-09 18:25:27.000000 shexer-2.2.0/test/test_instances_cap.py
+-rw-rw-rw-   0        0        0     3367 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_instances_file_input.py
+-rw-rw-rw-   0        0        0     3852 2023-02-02 16:28:05.000000 shexer-2.2.0/test/test_instances_report.py
+-rw-rw-rw-   0        0        0     3548 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_instantiation_property.py
+-rw-rw-rw-   0        0        0     1964 2022-03-28 20:28:03.000000 shexer-2.2.0/test/test_inverse_paths.py
+-rw-rw-rw-   0        0        0     3594 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_keep_less_specific.py
+-rw-rw-rw-   0        0        0     4051 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_list_of_url_input.py
+-rw-rw-rw-   0        0        0     4106 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_namespaces_dict.py
+-rw-rw-rw-   0        0        0     2082 2023-04-13 17:23:12.000000 shexer-2.2.0/test/test_namespaces_to_ignore.py
+-rw-rw-rw-   0        0        0     5000 2021-01-14 17:50:12.000000 shexer-2.2.0/test/test_raw_graph.py
+-rw-rw-rw-   0        0        0     4300 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_raw_shape_map.py
+-rw-rw-rw-   0        0        0     1711 2022-07-15 19:02:46.000000 shexer-2.2.0/test/test_rdflib_graph.py
+-rw-rw-rw-   0        0        0     2930 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_remove_empty_sahpes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.366786 shexer-2.2.0/test/test_shacl/
+-rw-rw-rw-   0        0        0        0 2021-04-26 09:52:52.000000 shexer-2.2.0/test/test_shacl/__init__.py
+-rw-rw-rw-   0        0        0     2225 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_shacl/test_annotation.py
+-rw-rw-rw-   0        0        0     2242 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_shacl/test_class_selection.py
+-rw-rw-rw-   0        0        0     3291 2023-04-06 19:32:13.000000 shexer-2.2.0/test/test_shacl/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0      910 2022-03-28 20:28:03.000000 shexer-2.2.0/test/test_shacl/test_literal_types.py
+-rw-rw-rw-   0        0        0     4313 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_shape_map_file.py
+-rw-rw-rw-   0        0        0     6086 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_shape_map_format.py
+-rw-rw-rw-   0        0        0     2307 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0     2889 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_shapes_namespaces.py
+-rw-rw-rw-   0        0        0     2452 2022-03-28 20:28:03.000000 shexer-2.2.0/test/test_sort.py
+-rw-rw-rw-   0        0        0     2058 2021-10-24 17:07:37.000000 shexer-2.2.0/test/test_target_classes.py
+-rw-rw-rw-   0        0        0     3120 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_threshold.py
+-rw-rw-rw-   0        0        0     2578 2023-04-03 18:13:27.000000 shexer-2.2.0/test/test_url_endpoint.py
+-rw-rw-rw-   0        0        0     1867 2022-07-15 19:02:46.000000 shexer-2.2.0/test/test_url_graph.py
+-rw-rw-rw-   0        0        0     1900 2021-10-03 10:32:18.000000 shexer-2.2.0/test/test_wikidata_annotation.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:26:37.409783 shexer-2.2.0/ws/
+-rw-rw-rw-   0        0        0        0 2019-11-23 19:24:29.000000 shexer-2.2.0/ws/__init__.py
+-rw-rw-rw-   0        0        0    19884 2022-03-28 20:28:03.000000 shexer-2.2.0/ws/shexer_rest.py
+-rw-rw-rw-   0        0        0       28 2019-11-23 19:24:29.000000 shexer-2.2.0/ws/wsgi.py
```

### Comparing `shexer-2.1.3/LICENSE` & `shexer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/PKG-INFO` & `shexer-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.1.3
+Version: 2.2.0
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.3.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.2.0.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -196,17 +196,18 @@
 * instances_file_input (default None): in case you have a separate file in which instantiation relations can be found, provide its path here. If you dont provide any value, the shaper will look for instances in the graph used as input.
 * graph_file_input (default None): a path to the file in which the target graph can be found.
 * graph_list_of_files_input (default None): in case your graph is separated in several files (all of them with the same format), provide a list of string paths to those files here.
 * raw_graph (default None): a simple raw string containing the target graph.
 * url_graph_input (default None): use it to provide a URL of some downloadable RDF content available online to be used as target graph.
 * list_of_url_input (default None): use it to provide several URLs of downloadable RDF content available online to be used as target graph.
 * url_endpoint (default None): it expects the URL of an SPARQL endpoint. Use it if you want to get some relevant triples form that endpoint instead of providing a whole RDF graph. In this case, the triples will be those ones whose subject is one of the nodes used to build the shapes (instances of a target class, result of a node selector in a shape map).
+* instances_cap (default -1): when this param is set to a positive value, sheXer will only use a maximun of instance_cap instances to get extract each shape. This may cause some lost of information, but if the sample of instances used is representative enough, your results won't be that different but you'll save main memory and execution time. 
 * depth_for_building_subgraph (default 1): use this param just in case you are working against a SPARQL endpoint. This integer indicates the max distance from any seed node to consider in order to track a subgraph from the endpoint. Please, remind that a high depth can cause a massive number of queries and have a high performance cost. 
 * track_classes_for_entities_at_last_depth_level (default True): use this param just in case you are working against a SPARQL endpoint. If it set to True, it makes a step further to the distance to the seed nodes indicated in the param depth. However, it will just look for triples related to typing, not the whole neighborhood of the nodes in the last level of depth.
-* limit_remote_instances (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. 
+* limit_remote_instances *DEPRECATED* (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. NOTE: This parameter only affects computation consuming SPARQL endpoints. On the other hand, the parameter instances_cap works for any case, including SPARQL endpoints. Due to retrocompatibility reasons, limit_remote_instances still works, but it will be removed in future sheXer releases.
 * disable_endpoint_cache (default False). By default, if sheXer is told to consume triples from an endpoint, it will make some SPARQL queries and store the results in a local graph. If this parameter is set to True, sheXer won't save that content locally. This will help to reduce main memory usage, but will decrease the performance, as sheXer will need to make more SPARQL queries to the endpoint.
 * namespaces_dict (default None): dictionary in which the keys are namespaces and the values are their expected prefixes in the outputs. 
 * input_format (default "NT"): the format of the graph which is going to be computed. The default value is const.NT. IMPORTANT: currently, sheXer does not guess input format, so ensure you specify the format here in case you are not providing n-triples content. In case you provide a combined input (several files, several URLs...) they all should have the same format. If you work against an endpoit, then this param do not have any effect.
 * compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP and GZ. Set compression_format to "zip" or "gz" to work with such files. Each gz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
 
 #### Params to tune the shexing process
```

### Comparing `shexer-2.1.3/README.md` & `shexer-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,18 @@
 * instances_file_input (default None): in case you have a separate file in which instantiation relations can be found, provide its path here. If you dont provide any value, the shaper will look for instances in the graph used as input.
 * graph_file_input (default None): a path to the file in which the target graph can be found.
 * graph_list_of_files_input (default None): in case your graph is separated in several files (all of them with the same format), provide a list of string paths to those files here.
 * raw_graph (default None): a simple raw string containing the target graph.
 * url_graph_input (default None): use it to provide a URL of some downloadable RDF content available online to be used as target graph.
 * list_of_url_input (default None): use it to provide several URLs of downloadable RDF content available online to be used as target graph.
 * url_endpoint (default None): it expects the URL of an SPARQL endpoint. Use it if you want to get some relevant triples form that endpoint instead of providing a whole RDF graph. In this case, the triples will be those ones whose subject is one of the nodes used to build the shapes (instances of a target class, result of a node selector in a shape map).
+* instances_cap (default -1): when this param is set to a positive value, sheXer will only use a maximun of instance_cap instances to get extract each shape. This may cause some lost of information, but if the sample of instances used is representative enough, your results won't be that different but you'll save main memory and execution time. 
 * depth_for_building_subgraph (default 1): use this param just in case you are working against a SPARQL endpoint. This integer indicates the max distance from any seed node to consider in order to track a subgraph from the endpoint. Please, remind that a high depth can cause a massive number of queries and have a high performance cost. 
 * track_classes_for_entities_at_last_depth_level (default True): use this param just in case you are working against a SPARQL endpoint. If it set to True, it makes a step further to the distance to the seed nodes indicated in the param depth. However, it will just look for triples related to typing, not the whole neighborhood of the nodes in the last level of depth.
-* limit_remote_instances (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. 
+* limit_remote_instances *DEPRECATED* (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. NOTE: This parameter only affects computation consuming SPARQL endpoints. On the other hand, the parameter instances_cap works for any case, including SPARQL endpoints. Due to retrocompatibility reasons, limit_remote_instances still works, but it will be removed in future sheXer releases.
 * disable_endpoint_cache (default False). By default, if sheXer is told to consume triples from an endpoint, it will make some SPARQL queries and store the results in a local graph. If this parameter is set to True, sheXer won't save that content locally. This will help to reduce main memory usage, but will decrease the performance, as sheXer will need to make more SPARQL queries to the endpoint.
 * namespaces_dict (default None): dictionary in which the keys are namespaces and the values are their expected prefixes in the outputs. 
 * input_format (default "NT"): the format of the graph which is going to be computed. The default value is const.NT. IMPORTANT: currently, sheXer does not guess input format, so ensure you specify the format here in case you are not providing n-triples content. In case you provide a combined input (several files, several URLs...) they all should have the same format. If you work against an endpoit, then this param do not have any effect.
 * compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP and GZ. Set compression_format to "zip" or "gz" to work with such files. Each gz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
 
 #### Params to tune the shexing process
```

### Comparing `shexer-2.1.3/setup.py` & `shexer-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.1.3',
+  version = '2.2.0',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.1.3.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.2.0.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `shexer-2.1.3/shexer/consts.py` & `shexer-2.2.0/shexer/consts.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.2.0/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.2.0/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.2.0/shexer/core/instances/annotators/base_annotator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from shexer.core.instances.pconsts import _S, _P, _O
 from shexer.core.instances.annotators.strategy_mode.target_classes_mode import TargetClassesMode
 from shexer.core.instances.annotators.strategy_mode.all_classes_mode import AllClasesMode
 from shexer.core.instances.annotators.strategy_mode.shape_qualifiers_mode import ShapeQualifiersMode
 from shexer.core.instances.annotators.strategy_mode.compound_strategy_mode import CompoundStrategyMode
+from shexer.core.instances.annotators.strategy_mode.instance_cap_mode import InstanceCapMode
 
 
 class BaseAnnotator(object):
 
     def __init__(self, instance_tracker):
         self._instance_tracker = instance_tracker
 
@@ -17,46 +18,57 @@
         self._instances_dict = self._instance_tracker._instances_dict
         self._classes_considered_in_htree = self._instance_tracker._classes_considered_in_htree
         self._htree = self._instance_tracker._htree
         self._shape_qualifiers_mode = self._instance_tracker._shape_qualifiers_mode
         self._namespaces_for_qualifiers_props = self._instance_tracker._namespaces_for_qualifiers_props
         self._target_classes = self._instance_tracker._target_classes
         self._shapes_namespace = self._instance_tracker._shapes_namespace
+        self._instances_cap = self._instance_tracker._instances_cap
 
         self._strategy_mode = self._get_proper_strategy()
 
     def is_relevant_triple(self, a_triple):
         return self._strategy_mode.is_relevant_triple(a_triple)
 
     def annotate_triple(self, a_triple):
         self._strategy_mode.annotate_triple(a_triple)
 
     def add_instance_to_instances_dict(self, a_triple):
         if a_triple[_S].iri not in self._instances_dict:
             self._instances_dict[a_triple[_S].iri] = []
 
-    def annotate_class(self, a_triple):
-        self._instances_dict[a_triple[_S].iri].append(a_triple[_O].iri)
+    # def annotate_class(self, a_triple):
+    #     self._strategy_mode.annotate_class(a_triple)
 
     def annotation_post_parsing(self):
         self._strategy_mode.annotation_post_parsing()
 
 
     def _get_proper_strategy(self):
+        result = None
         strategies_list = []
+        target_classes_flag = False
         if self._all_classes_mode:
             strategies_list.append(AllClasesMode(annotator_ref=self))
         if self._target_classes is not None and len(self._target_classes) > 0:
             strategies_list.append(TargetClassesMode(annotator_ref=self))
+            target_classes_flag = True
         if self._shape_qualifiers_mode:
             strategies_list.append(
                 ShapeQualifiersMode(annotator_ref=self,
                                     namespaces_for_qualifiers_props=self._namespaces_for_qualifiers_props,
                                     shapes_namespace=self._shapes_namespace))
 
         if len(strategies_list) == 0:
             raise ValueError("Wrong combination of params when building the instance tracker. There are not target classes")
         if len(strategies_list) == 1:
-            return strategies_list[0]
+            result = strategies_list[0]
         else:
-            return CompoundStrategyMode(annotator_ref=self,
+            result = CompoundStrategyMode(annotator_ref=self,
                                         list_of_strategies=strategies_list)
+        return result if self._instances_cap <= 0 else \
+            InstanceCapMode(annotator_ref=self,
+                            internal_strategy=result,
+                            instance_limit=self._instances_cap,
+                            n_target_classes=-1 if not target_classes_flag or len(strategies_list) > 1
+                                                   else len(self._target_classes)
+                            )
```

### Comparing `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from shexer.core.instances.annotators.strategy_mode.base_strategy_mode import BaseStrategyMode
-from shexer.core.instances.pconsts import _S, _P, _O
+from shexer.core.instances.pconsts import _P
 
 class AllClasesMode(BaseStrategyMode):
 
     def __init__(self, annotator_ref):
         super().__init__(annotator_ref)
 
 
@@ -13,10 +13,10 @@
             return False
         return True
 
 
     def annotate_triple(self, a_triple):
         if self._instance_tracker.is_an_instantiation_prop(a_triple[_P]):
             self._annotator_ref.add_instance_to_instances_dict(a_triple)
-            self._annotator_ref.annotate_class(a_triple)
+            self.annotate_class(a_triple)
```

### Comparing `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.2.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.2.0/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from shexer.core.instances.abstract_instance_tracker import AbstractInstanceTracker
+from shexer.utils.log import log_msg
 
-from shexer.core.instances.annotators.strategy_mode.base_strategy_mode import BaseStrategyMode
-from shexer.core.instances.pconsts import _P, _O
 
-class TargetClassesMode(BaseStrategyMode):
+class ShapeMapInstanceTracker(AbstractInstanceTracker):
 
-    def __init__(self, annotator_ref):
-        super().__init__(annotator_ref)
-        self._target_classes = self._annotator_ref._target_classes
-
-    def is_relevant_triple(self, a_triple):
-        if a_triple[_P] != self._instantiation_property:
-            return False
-        if a_triple[_O] not in self._target_classes:
-            return False
-        return True
-
-    def annotate_triple(self, a_triple):
-        if self._instance_tracker.is_an_instantiation_prop(a_triple[_P]):
-            self._annotator_ref.add_instance_to_instances_dict(a_triple)
-            self._annotator_ref.annotate_class(a_triple)
+    def __init__(self, shape_map):
+        self._shape_map = shape_map
+        self._instances_dict = {}
+
+    def track_instances(self, verbose=False):
+        log_msg(verbose=verbose,
+                msg="Starting instance tracker...")
+        for an_item in self._shape_map.yield_items():
+            self._solve_targets_of_an_item(an_item)
+        log_msg(verbose=verbose,
+                msg="Instance tracker finished. {} instances located".format(len(self._instances_dict)))
+        return self._instances_dict
+
+    def _solve_targets_of_an_item(self, an_item):
+        for a_node in an_item.node_selector.get_target_nodes():
+            if a_node not in self._instances_dict:
+                self._instances_dict[a_node] = []
+            self._instances_dict[a_node].append(an_item.shape_label)
 
+    def _specific_disambiguator_prefix(self):
+        return "custom_"
```

### Comparing `shexer-2.1.3/shexer/core/instances/instance_tracker.py` & `shexer-2.2.0/shexer/core/instances/instance_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from shexer.model.property import Property
 from shexer.utils.uri import remove_corners
 from shexer.utils.factories.h_tree import get_basic_h_tree
 from shexer.core.instances.annotators.annotator_func import get_proper_annotator
 from shexer.core.instances.abstract_instance_tracker import AbstractInstanceTracker
 from shexer.consts import SHAPES_DEFAULT_NAMESPACE
 from shexer.utils.log import log_msg
-
+from shexer.core.instances.annotators.strategy_mode.instances_cap_exception import InstancesCapException
 
 
 _RDF_TYPE = Property(content="http://www.w3.org/1999/02/22-rdf-syntax-ns#type")
 _RDFS_SUBCLASS_OF = Property(content="http://www.w3.org/2000/01/rdf-schema#subClassOf")
 
 
 class InstanceTracker(AbstractInstanceTracker):
 
     def __init__(self, target_classes, triples_yielder, instantiation_property=_RDF_TYPE,
                  all_classes_mode=False, subclass_property=_RDFS_SUBCLASS_OF, track_hierarchies=True,
                  shape_qualifiers_mode=False, namespaces_for_qualifier_props=None,
-                 shapes_namespace=SHAPES_DEFAULT_NAMESPACE):
+                 shapes_namespace=SHAPES_DEFAULT_NAMESPACE, instances_cap=-1):
         self._target_classes = target_classes
         self._all_classes_mode = all_classes_mode
         self._instances_dict = self._build_instances_dict()
         self._triples_yielder = triples_yielder
         self._instantiation_property = self._decide_instantiation_property(instantiation_property)
         self._relevant_triples = 0
         self._not_relevant_triples = 0
         self._subclass_property = subclass_property
         self._track_hierarchies = track_hierarchies
         self._shape_qualifiers_mode = shape_qualifiers_mode
         self._namespaces_for_qualifiers_props = [] if namespaces_for_qualifier_props is None else namespaces_for_qualifier_props
         self._shapes_namespace = shapes_namespace
+        self._instances_cap = instances_cap
 
         self._htree = get_basic_h_tree() if track_hierarchies else None
         self._classes_considered_in_htree = set() if track_hierarchies else None
 
         self._annotator = get_proper_annotator(track_hierarchies=track_hierarchies,
                                                instance_tracker_ref=self)
 
@@ -52,16 +53,19 @@
     def htree(self):
         return self._htree
 
     def track_instances(self, verbose=False):
         log_msg(verbose=verbose,
                 msg="Starting instance tracker...")
         self._reset_count()
-        for a_revelant_triple in self._yield_relevant_triples():
-            self._annotator.annotate_triple(a_revelant_triple)
+        try:
+            for a_revelant_triple in self._yield_relevant_triples():
+                self._annotator.annotate_triple(a_revelant_triple)
+        except InstancesCapException:
+            pass  # It's OK, we just don't need to explore more
         self._annotator.annotation_post_parsing()
         log_msg(verbose=verbose,
                 msg="Instance tracker finished. {} instances located".format(len(self._instances_dict)))
         return self._instances_dict
 
     def _yield_relevant_triples(self):
         for a_triple in self._triples_yielder.yield_triples():
```

### Comparing `shexer-2.1.3/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.2.0/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/profiling/class_profiler.py` & `shexer-2.2.0/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.2.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.2.0/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.2.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/shexing/class_shexer.py` & `shexer-2.2.0/shexer/core/shexing/class_shexer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.2.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.2.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.2.0/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.2.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.2.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.2.0/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.2.0/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.2.0/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.2.0/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.2.0/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.2.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.2.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.2.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.2.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.2.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/io/sparql/query.py` & `shexer-2.2.0/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/IRI.py` & `shexer-2.2.0/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/Macro.py` & `shexer-2.2.0/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.2.0/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/graph/abstract_sgraph.py` & `shexer-2.2.0/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.2.0/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.2.0/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/hierarchy_tree.py` & `shexer-2.2.0/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/node_selector.py` & `shexer-2.2.0/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/shape.py` & `shexer-2.2.0/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/shape_map.py` & `shexer-2.2.0/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/model/statement.py` & `shexer-2.2.0/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/shaper.py` & `shexer-2.2.0/shexer/shaper.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,16 @@
                  wikidata_annotation=False,
                  inverse_paths=False,
                  compression_mode=None,
                  decimals=-1,
                  instances_report_mode=RATIO_INSTANCES,
                  disable_endpoint_cache=False,
                  detect_minimal_iri=False,
-                 allow_redundant_or=False
+                 allow_redundant_or=False,
+                 instances_cap=-1
                  ):
         """
 
         :param target_classes:
         :param file_target_classes:
         :param input_format:
         :param instances_file_input:
@@ -153,21 +154,23 @@
         self._all_classes_mode = all_classes_mode
         self._shape_map_file = shape_map_file
         self._shape_map_raw = shape_map_raw
         self._decimals = decimals
         self._instances_report_mode = instances_report_mode
         self._disable_endpoint_cache=disable_endpoint_cache
         self._allow_redundant_or = allow_redundant_or
+        self._instances_cap = instances_cap
 
         self._remove_empty_shapes=remove_empty_shapes
         self._disable_comments = disable_comments
         self._disable_or_statements = disable_or_statements
         self._allow_opt_cardinality = allow_opt_cardinality
         self._disable_exact_cardinality = disable_exact_cardinality
-        self._limit_remote_instances = limit_remote_instances
+        # TODO: REMOVE THE _limit_remote_instances PARAMETER IN FUTURE RELEASES
+        self._limit_remote_instances = limit_remote_instances if instances_cap==-1 else instances_cap
         self._wikidata_annotation = wikidata_annotation
         self._inverse_paths = inverse_paths
         self._detect_minimal_iri = detect_minimal_iri
 
         self._compression_mode = compression_mode
 
         self._depth_for_building_subgraph = depth_for_building_subgraph
@@ -369,15 +372,16 @@
                                     shape_qualifiers_mode=self._shape_qualifiers_mode,
                                     built_remote_graph=self._built_remote_graph,
                                     built_shape_map=self._built_shape_map,
                                     shapes_namespace=self._shapes_namespace,
                                     limit_remote_instances=self._limit_remote_instances,
                                     inverse_paths=self._inverse_paths,
                                     compression_mode=self._compression_mode,
-                                    disable_endpoint_cache=self._disable_endpoint_cache)
+                                    disable_endpoint_cache=self._disable_endpoint_cache,
+                                    instances_cap=self._instances_cap)
 
 
     @staticmethod
     def _check_correct_output_params(string_output, target_file):
         if not string_output and target_file is None:
             raise ValueError("You must provide a target path or set string output to True")
```

### Comparing `shexer-2.1.3/shexer/utils/compression.py` & `shexer-2.2.0/shexer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.2.0/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.2.0/shexer/utils/factories/class_shexer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/h_tree.py` & `shexer-2.2.0/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.2.0/shexer/utils/factories/instance_tracker_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
                          shape_qualifiers_mode=False,
                          built_remote_graph=None,
                          built_shape_map=None,
                          shapes_namespace=SHAPES_DEFAULT_NAMESPACE,
                          limit_remote_instances=-1,
                          inverse_paths=False,
                          compression_mode=None,
-                         disable_endpoint_cache=False
+                         disable_endpoint_cache=False,
+                         instances_cap=-1
                          ):
     """
 
     :param instances_file_input:
     :param graph_file_input:
     :param graph_list_of_files_input:
     :param target_classes:
@@ -160,15 +161,16 @@
         pure_instances_tracker = InstanceTracker(target_classes=model_classes,
                                                  triples_yielder=instance_yielder,
                                                  instantiation_property=instantiation_property,
                                                  all_classes_mode=all_classes_mode,
                                                  track_hierarchies=False,
                                                  namespaces_for_qualifier_props=namespaces_for_qualifier_props,
                                                  shape_qualifiers_mode=shape_qualifiers_mode,
-                                                 shapes_namespace=shapes_namespace)
+                                                 shapes_namespace=shapes_namespace,
+                                                 instances_cap=instances_cap)
 
     return _decide_tracker_to_return(selectors_tracker, pure_instances_tracker)
 
 
 def _get_adequate_sgraph(endpoint_url, graph_file_input, url_input, graph_format,
                          raw_graph, built_remote_graph, disable_endpoint_cache):
     if endpoint_url is not None:
```

### Comparing `shexer-2.1.3/shexer/utils/factories/shape_map_factory.py` & `shexer-2.2.0/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.2.0/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.2.0/shexer/utils/factories/shape_serializer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.2.0/shexer/utils/factories/triple_yielders_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/namespaces.py` & `shexer-2.2.0/shexer/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/obj_references.py` & `shexer-2.2.0/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/shapes.py` & `shexer-2.2.0/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/target_elements.py` & `shexer-2.2.0/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.2.0/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/triple_yielders.py` & `shexer-2.2.0/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer/utils/uri.py` & `shexer-2.2.0/shexer/utils/uri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/shexer.egg-info/PKG-INFO` & `shexer-2.2.0/shexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.1.3
+Version: 2.2.0
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.1.3.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.2.0.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -196,17 +196,18 @@
 * instances_file_input (default None): in case you have a separate file in which instantiation relations can be found, provide its path here. If you dont provide any value, the shaper will look for instances in the graph used as input.
 * graph_file_input (default None): a path to the file in which the target graph can be found.
 * graph_list_of_files_input (default None): in case your graph is separated in several files (all of them with the same format), provide a list of string paths to those files here.
 * raw_graph (default None): a simple raw string containing the target graph.
 * url_graph_input (default None): use it to provide a URL of some downloadable RDF content available online to be used as target graph.
 * list_of_url_input (default None): use it to provide several URLs of downloadable RDF content available online to be used as target graph.
 * url_endpoint (default None): it expects the URL of an SPARQL endpoint. Use it if you want to get some relevant triples form that endpoint instead of providing a whole RDF graph. In this case, the triples will be those ones whose subject is one of the nodes used to build the shapes (instances of a target class, result of a node selector in a shape map).
+* instances_cap (default -1): when this param is set to a positive value, sheXer will only use a maximun of instance_cap instances to get extract each shape. This may cause some lost of information, but if the sample of instances used is representative enough, your results won't be that different but you'll save main memory and execution time. 
 * depth_for_building_subgraph (default 1): use this param just in case you are working against a SPARQL endpoint. This integer indicates the max distance from any seed node to consider in order to track a subgraph from the endpoint. Please, remind that a high depth can cause a massive number of queries and have a high performance cost. 
 * track_classes_for_entities_at_last_depth_level (default True): use this param just in case you are working against a SPARQL endpoint. If it set to True, it makes a step further to the distance to the seed nodes indicated in the param depth. However, it will just look for triples related to typing, not the whole neighborhood of the nodes in the last level of depth.
-* limit_remote_instances (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. 
+* limit_remote_instances *DEPRECATED* (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. NOTE: This parameter only affects computation consuming SPARQL endpoints. On the other hand, the parameter instances_cap works for any case, including SPARQL endpoints. Due to retrocompatibility reasons, limit_remote_instances still works, but it will be removed in future sheXer releases.
 * disable_endpoint_cache (default False). By default, if sheXer is told to consume triples from an endpoint, it will make some SPARQL queries and store the results in a local graph. If this parameter is set to True, sheXer won't save that content locally. This will help to reduce main memory usage, but will decrease the performance, as sheXer will need to make more SPARQL queries to the endpoint.
 * namespaces_dict (default None): dictionary in which the keys are namespaces and the values are their expected prefixes in the outputs. 
 * input_format (default "NT"): the format of the graph which is going to be computed. The default value is const.NT. IMPORTANT: currently, sheXer does not guess input format, so ensure you specify the format here in case you are not providing n-triples content. In case you provide a combined input (several files, several URLs...) they all should have the same format. If you work against an endpoit, then this param do not have any effect.
 * compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP and GZ. Set compression_format to "zip" or "gz" to work with such files. Each gz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
 
 #### Params to tune the shexing process
```

### Comparing `shexer-2.1.3/shexer.egg-info/SOURCES.txt` & `shexer-2.2.0/shexer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 shexer/core/instances/annotators/annotator_func.py
 shexer/core/instances/annotators/annotator_tracking_instances.py
 shexer/core/instances/annotators/base_annotator.py
 shexer/core/instances/annotators/strategy_mode/__init__.py
 shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
 shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
 shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
+shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
 shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
 shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
 shexer/core/instances/mappings/__init__.py
 shexer/core/instances/mappings/shape_map_instance_tracker.py
 shexer/core/instances/mix/__init__.py
 shexer/core/instances/mix/mixed_instance_tracker.py
 shexer/core/profiling/__init__.py
@@ -157,14 +159,15 @@
 test/test_disable_or_statements.py
 test/test_discard_and_compliant.py
 test/test_file_target_classes.py
 test/test_graph_file_input.py
 test/test_graph_list_of_file_inputs.py
 test/test_infer_numeric_types_for_untyped_literals.py
 test/test_input_format.py
+test/test_instances_cap.py
 test/test_instances_file_input.py
 test/test_instances_report.py
 test/test_instantiation_property.py
 test/test_inverse_paths.py
 test/test_keep_less_specific.py
 test/test_list_of_url_input.py
 test/test_namespaces_dict.py
```

### Comparing `shexer-2.1.3/test/const.py` & `shexer-2.2.0/test/const.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/t_utils.py` & `shexer-2.2.0/test/t_utils.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_all_classes_mode.py` & `shexer-2.2.0/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_allow_opt_cardinality.py` & `shexer-2.2.0/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_allow_redundant_or.py` & `shexer-2.2.0/test/test_allow_redundant_or.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.2.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py` & `shexer-2.2.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_compression_mode.py` & `shexer-2.2.0/test/test_compression_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_decimals.py` & `shexer-2.2.0/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_depth_for_building_subgraph.py` & `shexer-2.2.0/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_detect_minimal_iri.py` & `shexer-2.2.0/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_disable_comments.py` & `shexer-2.2.0/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_disable_endpoint_cache.py` & `shexer-2.2.0/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_disable_exact_cardinality.py` & `shexer-2.2.0/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_disable_or_statements.py` & `shexer-2.2.0/test/test_disable_or_statements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_discard_and_compliant.py` & `shexer-2.2.0/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_file_target_classes.py` & `shexer-2.2.0/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_graph_file_input.py` & `shexer-2.2.0/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_graph_list_of_file_inputs.py` & `shexer-2.2.0/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.2.0/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_input_format.py` & `shexer-2.2.0/test/test_input_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_instances_file_input.py` & `shexer-2.2.0/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_instances_report.py` & `shexer-2.2.0/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_instantiation_property.py` & `shexer-2.2.0/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_inverse_paths.py` & `shexer-2.2.0/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_keep_less_specific.py` & `shexer-2.2.0/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_list_of_url_input.py` & `shexer-2.2.0/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_namespaces_dict.py` & `shexer-2.2.0/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_namespaces_to_ignore.py` & `shexer-2.2.0/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_raw_graph.py` & `shexer-2.2.0/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_raw_shape_map.py` & `shexer-2.2.0/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_rdflib_graph.py` & `shexer-2.2.0/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_remove_empty_sahpes.py` & `shexer-2.2.0/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shacl/test_annotation.py` & `shexer-2.2.0/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shacl/test_class_selection.py` & `shexer-2.2.0/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.2.0/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shacl/test_literal_types.py` & `shexer-2.2.0/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shape_map_file.py` & `shexer-2.2.0/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shape_map_format.py` & `shexer-2.2.0/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shape_qualifiers_mode.py` & `shexer-2.2.0/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_shapes_namespaces.py` & `shexer-2.2.0/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_sort.py` & `shexer-2.2.0/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_target_classes.py` & `shexer-2.2.0/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_threshold.py` & `shexer-2.2.0/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_url_endpoint.py` & `shexer-2.2.0/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_url_graph.py` & `shexer-2.2.0/test/test_url_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/test/test_wikidata_annotation.py` & `shexer-2.2.0/test/test_wikidata_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.1.3/ws/shexer_rest.py` & `shexer-2.2.0/ws/shexer_rest.py`

 * *Files identical despite different names*

