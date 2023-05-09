# Comparing `tmp/transition_neural_parser-0.5.3.tar.gz` & `tmp/transition_neural_parser-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transition_neural_parser-0.5.3.tar", last modified: Tue May  2 14:57:40 2023, max compression
+gzip compressed data, was "transition_neural_parser-0.5.4.tar", last modified: Tue May  9 20:51:28 2023, max compression
```

## Comparing `transition_neural_parser-0.5.3.tar` & `transition_neural_parser-0.5.4.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:40.018119 transition_neural_parser-0.5.3/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10776 2023-04-24 13:10:54.000000 transition_neural_parser-0.5.3/LICENSE
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10711 2023-05-02 14:57:40.017552 transition_neural_parser-0.5.3/PKG-INFO
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9958 2023-05-02 14:04:51.000000 transition_neural_parser-0.5.3/README.md
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      980 2023-05-02 14:57:33.000000 transition_neural_parser-0.5.3/pyproject.toml
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       38 2023-05-02 14:57:40.018202 transition_neural_parser-0.5.3/setup.cfg
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1794 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/setup.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.750837 transition_neural_parser-0.5.3/src/
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.801142 transition_neural_parser-0.5.3/src/fairseq_ext/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      165 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/__init__.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.802989 transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19730 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.822813 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10043 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8788 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15698 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15835 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21406 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21411 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10755 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10336 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8638 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28857 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info_binarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6018 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/average_checkpoints.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1100 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/binarize.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.827197 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      679 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12919 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12636 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.843203 transition_neural_parser-0.5.3/src/fairseq_ext/data/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29683 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29892 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30695 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30770 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10918 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_bpe.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9147 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/data_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16218 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/indexed_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18120 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/data/language_pair_dataset.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.851013 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6506 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/binarize_encodings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9588 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/composite_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5255 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/mapavg_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8609 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/sentence_encoding.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15450 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/generate.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16901 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/generate_sliding.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.872908 transition_neural_parser-0.5.3/src/fairseq_ext/models/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      796 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8953 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5741 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/graph_attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8485 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/graphmp_attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79650 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84503 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79562 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    75031 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    73280 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    64589 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graph.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84683 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.883112 transition_neural_parser-0.5.3/src/fairseq_ext/modules/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6304 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/factored_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23865 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23312 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention_old.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    17425 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12391 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer_old.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    31215 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/options.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20449 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/options_train.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15142 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18504 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    14481 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13349 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.889815 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4761 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/binarize_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9693 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9316 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings_bert.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65291 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65757 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    57973 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graph.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62664 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.902379 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      580 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    22251 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    27439 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    55372 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28086 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24602 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24616 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       81 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/tokenizer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23242 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/train.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7661 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1052 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/utils_font.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1748 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/fairseq_ext/utils_import.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.950107 transition_neural_parser-0.5.3/src/ibm_neural_aligner/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1226 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/README.md
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6389 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_leamr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8746 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1980 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/alignment_decoder.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5840 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/amr_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7611 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.launch_many_jobs.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9753 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.summarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      687 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/dummy_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    26107 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/evaluation.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5402 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/formatter.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4784 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/gcn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      485 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/leamr_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     2991 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/lexicon.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    60552 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/main.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1158 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/make_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1752 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/metric_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4322 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/pretrained_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13907 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/resolve_manual_alignments.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3752 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_detailed_eval.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      874 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_eval.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    11929 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_model_selection.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7781 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_sampler.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    34661 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/standalone_elmo.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1145 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/tokenize_amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4869 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/transformer_lm.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19700 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_lstm.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8380 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_rnn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3709 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/view_manual_alignments.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3202 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/vocab.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      380 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/ibm_neural_aligner/vocab_definitions.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:39.981478 transition_neural_parser-0.5.3/src/transition_amr_parser/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      867 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/__init__.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:40.010840 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3749 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/amr_parser.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    37837 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_data_oracle.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13849 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_fake_parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62718 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62580 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15856 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15861 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4040 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/roberta_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1355 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/add_id_to_amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      635 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/add_sentence_amrs_to_file.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52645 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46594 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_aligner.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5278 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_constituents.py
--rwxrwxr-x   0 gxxu     (700773) gxxu     (606684)     6746 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_latex.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74725 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/amr_machine.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4756 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/clbar.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5057 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/force_overlap_actions.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    45407 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/gold_subgraph_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18047 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/io.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10706 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/make_sliding_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5548 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/merge_sliding_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    50558 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6358 2023-05-02 14:01:59.000000 transition_neural_parser-0.5.3/src/transition_amr_parser/plots.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-02 14:57:40.016978 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10711 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/PKG-INFO
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6377 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        1 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      116 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/entry_points.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      241 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/requires.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       53 2023-05-02 14:57:39.000000 transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/top_level.txt
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.747775 transition_neural_parser-0.5.4/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10776 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/LICENSE
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10822 2023-05-09 20:51:28.747399 transition_neural_parser-0.5.4/PKG-INFO
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10098 2023-05-09 20:34:18.000000 transition_neural_parser-0.5.4/README.md
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      960 2023-05-09 20:50:16.000000 transition_neural_parser-0.5.4/pyproject.toml
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       38 2023-05-09 20:51:28.747876 transition_neural_parser-0.5.4/setup.cfg
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1919 2023-05-09 20:34:18.000000 transition_neural_parser-0.5.4/setup.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.660090 transition_neural_parser-0.5.4/src/
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.678501 transition_neural_parser-0.5.4/src/fairseq_ext/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      165 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/__init__.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.679302 transition_neural_parser-0.5.4/src/fairseq_ext/amr_reform/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_reform/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19730 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.685888 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10043 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8788 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15698 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15835 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21406 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21411 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10755 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10336 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8638 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/old_action_info.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28857 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/old_action_info_binarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6018 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/average_checkpoints.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1100 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/binarize.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.687665 transition_neural_parser-0.5.4/src/fairseq_ext/criterions/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      679 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/criterions/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12919 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12636 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.694164 transition_neural_parser-0.5.4/src/fairseq_ext/data/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29683 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29892 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30695 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30770 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10918 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_bpe.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9147 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/data_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16218 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/indexed_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18120 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/data/language_pair_dataset.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.696469 transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6506 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/binarize_encodings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9588 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/composite_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5255 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/mapavg_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8609 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/sentence_encoding.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15450 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/generate.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16901 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/generate_sliding.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.702576 transition_neural_parser-0.5.4/src/fairseq_ext/models/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      796 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8953 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5741 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/graph_attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8485 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/graphmp_attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79650 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84503 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79562 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    75031 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    73280 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    64589 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_graph.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84683 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.706261 transition_neural_parser-0.5.4/src/fairseq_ext/modules/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/modules/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6304 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/modules/factored_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23865 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/modules/multihead_attention.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23312 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/modules/multihead_attention_old.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    17425 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/modules/transformer_layer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12391 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/modules/transformer_layer_old.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    31215 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/options.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20449 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/options_train.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15142 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/preprocess.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18504 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/preprocess_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    14481 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/preprocess_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13349 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/preprocess_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.707962 transition_neural_parser-0.5.4/src/fairseq_ext/roberta/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/roberta/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4761 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/roberta/binarize_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9693 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/roberta/pretrained_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9316 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/roberta/pretrained_embeddings_bert.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65291 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65757 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    57973 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator_graph.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62664 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.712226 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      580 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    22251 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    27439 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    55372 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28086 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24602 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24616 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       81 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/tokenizer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23242 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/train.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7661 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1052 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/utils_font.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1748 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/fairseq_ext/utils_import.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.729509 transition_neural_parser-0.5.4/src/ibm_neural_aligner/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1226 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/README.md
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6389 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/align_leamr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8746 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/align_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1980 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/alignment_decoder.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5840 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/amr_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7611 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/ccc.launch_many_jobs.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9753 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/ccc.summarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      687 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/dummy_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    26107 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/evaluation.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5402 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/formatter.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4784 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/gcn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      485 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/leamr_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     2991 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/lexicon.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    60552 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/main.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1158 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/make_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1752 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/metric_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4322 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/pretrained_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13907 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/resolve_manual_alignments.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3752 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_detailed_eval.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      874 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_eval.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    11929 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_model_selection.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7781 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_sampler.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    34661 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/standalone_elmo.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1145 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/tokenize_amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4869 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/transformer_lm.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19700 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/tree_lstm.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8380 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/tree_rnn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3709 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/view_manual_alignments.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3202 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/vocab.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      380 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/ibm_neural_aligner/vocab_definitions.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.738268 transition_neural_parser-0.5.4/src/transition_amr_parser/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      877 2023-05-09 20:34:18.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/__init__.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.744389 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3749 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/amr_parser.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    37837 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_data_oracle.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13849 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_fake_parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62718 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62580 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15856 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15861 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4040 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/roberta_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1355 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/add_id_to_amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      635 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/add_sentence_amrs_to_file.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52645 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46594 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/amr_aligner.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5278 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/amr_constituents.py
+-rwxrwxr-x   0 gxxu     (700773) gxxu     (606684)     6746 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/amr_latex.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74725 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/amr_machine.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4756 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/clbar.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5057 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/force_overlap_actions.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    45407 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/gold_subgraph_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18047 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/io.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10706 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/make_sliding_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5548 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/merge_sliding_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52549 2023-05-09 20:34:18.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6358 2023-05-08 18:31:47.000000 transition_neural_parser-0.5.4/src/transition_amr_parser/plots.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-05-09 20:51:28.746934 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10822 2023-05-09 20:51:28.745098 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6377 2023-05-09 20:51:28.745533 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        1 2023-05-09 20:51:28.745922 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      116 2023-05-09 20:51:28.746302 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      232 2023-05-09 20:51:28.746658 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/requires.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       53 2023-05-09 20:51:28.747016 transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/top_level.txt
```

### Comparing `transition_neural_parser-0.5.3/LICENSE` & `transition_neural_parser-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/PKG-INFO` & `transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: transition_neural_parser
-Version: 0.5.3
+Name: transition-neural-parser
+Version: 0.5.4
 Summary: The package for transition based nueral AMR parser
 Author-email: Ramon <ramon.astudillo@ibm.com>, Young-Suk <ysuklee@us.ibm.com>, Tahira <tnaseem@us.ibm.com>, Sadhana <sadhana.kumaravel1@ibm.com>, GX <GX.Xu@ibm.com>, Hans <raduf@us.ibm.com>, Salim <roukos@us.ibm.com>
-Project-URL: homepage, https://github.ibm.com/mnlp/transition-amr-parser/tree/master
-Project-URL: tracker, https://github.ibm.com/mnlp/transition-amr-parser/issues
+Project-URL: homepage, https://github.com/IBM/transition-amr-parser
+Project-URL: tracker, https://github.com/IBM/transition-amr-parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: ~=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Transition-based Neural Parser
 ============================
 
 State-of-the-Art Abstract Meaning Representation (AMR) parsing, see [papers
 with code](https://paperswithcode.com/task/amr-parsing). Models both
 distribution over graphs and aligments with a transition-based approach. Parser
-supports any other graph formalism as long as it is expressed in [Penman
+supports generic text-to-graph as long as it is expressed in [Penman
 notation](https://penman.readthedocs.io/en/latest/notation.html).
 
 Some of the main features
 
 - [Smatch](https://github.com/snowblink14/smatch) wrapper providing [significance testing](scripts/README.md#paired-boostrap-significance-test-for-Smatch) for Smatch and [MBSE](scripts/README.md#maximum-bayesian-smatch-ensemble-mbse) ensembling.
 - `Structured-BART` [(Zhou et al 2021b)](https://aclanthology.org/2021.emnlp-main.507/) with [trained checkpoints](#available-pretrained-model-checkpoints) for document-level AMR [(Naseem et al 2022)](https://aclanthology.org/2022.naacl-main.256), MBSE [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) and latent alignments training [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464)
 - `Structured-mBART` for multi-lingual support (EN, DE, Zh, IT) [(Lee et al 2022)](https://arxiv.org/abs/2112.07790)
@@ -39,42 +39,49 @@
 ```
 
 or alternatively use `virtualenv` and `pyenv` for python versions. Note that
 all scripts source a `set_environment.sh` script that you can use to activate
 your virtual environment as above and set environment variables. If not used,
 just create an empty version
 
-```
+```bash
 # or e.g. put inside conda activate ./cenv_x86
 touch set_environment.sh
 ```
 
-Then install the parser package using pip. You will need to install
-`torch-scatter` by separate since it is custom built for CUDA. Here we specify the
+Then install the parser package using pip. You will need to manually install
+`torch-scatter` since it is custom built for CUDA. Here we specify the
 call for `torch 1.13.1` and `cuda 11.7`. See [torch-scatter
 repository](https://pypi.org/project/torch-scatter/) to find the appropriate
-installation instructions.
+installation instructions. 
 
-```
+**For MacOS users** 
+
+(Please install the cpu version of torch-scatter; and model training is not fully supported here.)
+
+```bash
 pip install transition-neural-parser
+# for linux users
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
+# for cpu installation for MacOS
+# pip install torch-scatter
 ```
 
 If you plan to edit the code, clone and install instead
 
-```
+```bash
 # clone this repo (see link above), then
 cd transition-neural-parser
 pip install --editable .
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
 ```
 
 If you want to train a document-level AMR parser you will also need 
 
-```
+```bash
 git clone https://github.com/IBM/docAMR.git
 cd docAMR
 pip install .
 cd ..
 ```
 
 ## Parse with a pretrained model
@@ -188,28 +195,26 @@
 | AMR3-joint-ontowiki-seed44 | amr3joint_ontowiki2_g2g-structured-bart-large-seed44  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4          |
 | doc-sen-conll-amr-seed42   | both_doc+sen_trainsliding_ws400x100-seed42            |                                                                 | 82.3<sup>1</sup>/71.8 <sup>2</sup>|              |
 
 <sup>1 Smatch on AMR3.0 sentences</sup>
 
 <sup>2 Smatch on AMR3.0 Multi-Sentence dataset </sup>
 
-we also provide the trained `ibm-neural-aligner` under names
-`AMR2.0_ibm_neural_aligner.zip` and `AMR3.0_ibm_neural_aligner.zip`. For the
+contact authors to obtain the trained `ibm-neural-aligner`. For the
 ensemble we provide the three seeds. Following fairseq conventions, to run the
 ensemble just give the three checkpoint paths joined by `:` to the normal
 checkpoint argument `-c`. Note that the checkpoints were trained with the
 `v0.5.1` tokenizer, this reduces performance by `0.1` on `v0.5.2` tokenized
 data.
 
 Note that we allways report average of three seeds in papers while these are
 individual models. A fast way to test models standalone is
 
     bash tests/standalone.sh configs/<config>.sh
 
-
 ## Training a model
 
 You first need to pre-process and align the data. For AMR2.0 do
 
 ```bash
 conda activate ./cenv_x86 # activate parser environment
 python scripts/merge_files.py /path/to/LDC2017T10/data/amrs/split/ DATA/AMR2.0/corpora/
```

### Comparing `transition_neural_parser-0.5.3/README.md` & `transition_neural_parser-0.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Transition-based Neural Parser
 ============================
 
 State-of-the-Art Abstract Meaning Representation (AMR) parsing, see [papers
 with code](https://paperswithcode.com/task/amr-parsing). Models both
 distribution over graphs and aligments with a transition-based approach. Parser
-supports any other graph formalism as long as it is expressed in [Penman
+supports generic text-to-graph as long as it is expressed in [Penman
 notation](https://penman.readthedocs.io/en/latest/notation.html).
 
 Some of the main features
 
 - [Smatch](https://github.com/snowblink14/smatch) wrapper providing [significance testing](scripts/README.md#paired-boostrap-significance-test-for-Smatch) for Smatch and [MBSE](scripts/README.md#maximum-bayesian-smatch-ensemble-mbse) ensembling.
 - `Structured-BART` [(Zhou et al 2021b)](https://aclanthology.org/2021.emnlp-main.507/) with [trained checkpoints](#available-pretrained-model-checkpoints) for document-level AMR [(Naseem et al 2022)](https://aclanthology.org/2022.naacl-main.256), MBSE [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) and latent alignments training [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464)
 - `Structured-mBART` for multi-lingual support (EN, DE, Zh, IT) [(Lee et al 2022)](https://arxiv.org/abs/2112.07790)
@@ -25,42 +25,49 @@
 ```
 
 or alternatively use `virtualenv` and `pyenv` for python versions. Note that
 all scripts source a `set_environment.sh` script that you can use to activate
 your virtual environment as above and set environment variables. If not used,
 just create an empty version
 
-```
+```bash
 # or e.g. put inside conda activate ./cenv_x86
 touch set_environment.sh
 ```
 
-Then install the parser package using pip. You will need to install
-`torch-scatter` by separate since it is custom built for CUDA. Here we specify the
+Then install the parser package using pip. You will need to manually install
+`torch-scatter` since it is custom built for CUDA. Here we specify the
 call for `torch 1.13.1` and `cuda 11.7`. See [torch-scatter
 repository](https://pypi.org/project/torch-scatter/) to find the appropriate
-installation instructions.
+installation instructions. 
 
-```
+**For MacOS users** 
+
+(Please install the cpu version of torch-scatter; and model training is not fully supported here.)
+
+```bash
 pip install transition-neural-parser
+# for linux users
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
+# for cpu installation for MacOS
+# pip install torch-scatter
 ```
 
 If you plan to edit the code, clone and install instead
 
-```
+```bash
 # clone this repo (see link above), then
 cd transition-neural-parser
 pip install --editable .
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
 ```
 
 If you want to train a document-level AMR parser you will also need 
 
-```
+```bash
 git clone https://github.com/IBM/docAMR.git
 cd docAMR
 pip install .
 cd ..
 ```
 
 ## Parse with a pretrained model
@@ -174,28 +181,26 @@
 | AMR3-joint-ontowiki-seed44 | amr3joint_ontowiki2_g2g-structured-bart-large-seed44  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4          |
 | doc-sen-conll-amr-seed42   | both_doc+sen_trainsliding_ws400x100-seed42            |                                                                 | 82.3<sup>1</sup>/71.8 <sup>2</sup>|              |
 
 <sup>1 Smatch on AMR3.0 sentences</sup>
 
 <sup>2 Smatch on AMR3.0 Multi-Sentence dataset </sup>
 
-we also provide the trained `ibm-neural-aligner` under names
-`AMR2.0_ibm_neural_aligner.zip` and `AMR3.0_ibm_neural_aligner.zip`. For the
+contact authors to obtain the trained `ibm-neural-aligner`. For the
 ensemble we provide the three seeds. Following fairseq conventions, to run the
 ensemble just give the three checkpoint paths joined by `:` to the normal
 checkpoint argument `-c`. Note that the checkpoints were trained with the
 `v0.5.1` tokenizer, this reduces performance by `0.1` on `v0.5.2` tokenized
 data.
 
 Note that we allways report average of three seeds in papers while these are
 individual models. A fast way to test models standalone is
 
     bash tests/standalone.sh configs/<config>.sh
 
-
 ## Training a model
 
 You first need to pre-process and align the data. For AMR2.0 do
 
 ```bash
 conda activate ./cenv_x86 # activate parser environment
 python scripts/merge_files.py /path/to/LDC2017T10/data/amrs/split/ DATA/AMR2.0/corpora/
```

### Comparing `transition_neural_parser-0.5.3/pyproject.toml` & `transition_neural_parser-0.5.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "transition_neural_parser"
-version = '0.5.3'
+version = '0.5.4'
 authors = [
   { name="Ramon", email="ramon.astudillo@ibm.com" },
   { name="Young-Suk", email="ysuklee@us.ibm.com" },
   { name="Tahira", email="tnaseem@us.ibm.com" },
   { name="Sadhana", email="sadhana.kumaravel1@ibm.com" },
   { name="GX", email="GX.Xu@ibm.com" },
   { name="Hans", email="raduf@us.ibm.com" },
   { name="Salim", email="roukos@us.ibm.com" },
 ]
 description = "The package for transition based nueral AMR parser"
 readme = "README.md"
-requires-python = "~=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
 ]
 
 [tool.poetry.platforms]
-os = "linux"
+os = "linux, darwin"
 
 [project.urls]
-homepage = "https://github.ibm.com/mnlp/transition-amr-parser/tree/master"
-tracker = "https://github.ibm.com/mnlp/transition-amr-parser/issues"
+homepage = "https://github.com/IBM/transition-amr-parser"
+tracker = "https://github.com/IBM/transition-amr-parser"
```

### Comparing `transition_neural_parser-0.5.3/setup.py` & `transition_neural_parser-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from setuptools import setup, find_packages
+import sys
 
-VERSION = '0.5.3'
+VERSION = '0.5.4'
 
 install_requires = [
     "torch==1.13.1",
     'numpy<=1.23.5',
     'ipython<=8.12', # python 3.8 vs ipython 8.13 incompatibility
     'tqdm>=4.55.0',
-    'fairseq==0.10.2', # seems to not work on python 3.9 for some platforms
     'packaging>=20.8',
     'requests>=2.25.1',
     # for data (ELMO embeddings)
     'h5py>=3.0.0',
     'python-dateutil>=2.8.1',
     # for scoringy
     'penman>=1.1.0',
-    # needs tools to be importable > 1.0.4
-    'smatch>=1.0.3.2',
+    # needs tools to be importable > 1.0.4. As of now, no official release
+    'smatch',
     # for debugging
     'ipdb',
     'line_profiler>=4.0.2',
     'pyinstrument>=4.4.0',
     # for aws download
     'boto3>=1.26.1',
     'progressbar',
 ]
 
+# platform dependent fairseq version
+if sys.platform == 'darwin':
+    install_requires.append("fairseq==0.10.0")
+else:
+    install_requires.append("fairseq==0.10.2")
+
 if __name__ == '__main__':
     setup(
         name='transition_amr_parser',
         version=VERSION,
         description="Trasition-based neural parser",
         package_dir={"": "src"},
         # packages=['fairseq_ext', 'transition_amr_parser'],
```

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_bartsv.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/old_action_info.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/amr_spec/old_action_info_binarize.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/amr_spec/old_action_info_binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/average_checkpoints.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/average_checkpoints.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/binarize.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/criterions/__init__.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/criterions/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_dataset.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/amr_bpe.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/amr_bpe.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/data_utils.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/indexed_dataset.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/data/language_pair_dataset.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/data/language_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/binarize_encodings.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/binarize_encodings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/composite_embeddings.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/composite_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/mapavg_embeddings.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/mapavg_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/extract_bart/sentence_encoding.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/extract_bart/sentence_encoding.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/generate.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/generate.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/generate_sliding.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/generate_sliding.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/__init__.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/attention_masks.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/graph_attention_masks.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/graph_attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/graphmp_attention_masks.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/graphmp_attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graph.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_graph.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/factored_embeddings.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/modules/factored_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/modules/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/multihead_attention_old.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/modules/multihead_attention_old.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/modules/transformer_layer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/modules/transformer_layer_old.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/modules/transformer_layer_old.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/options.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/options.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/options_train.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/options_train.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/preprocess.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bart.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/preprocess_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_bartsv.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/preprocess_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/preprocess_graphmp.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/preprocess_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/roberta/binarize_embeddings.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/roberta/binarize_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/roberta/pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/roberta/pretrained_embeddings_bert.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/roberta/pretrained_embeddings_bert.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_bartsv.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graph.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator_graph.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/sequence_generator_graphmp.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/sequence_generator_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/__init__.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/train.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/train.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/utils.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/utils_font.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/utils_font.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/fairseq_ext/utils_import.py` & `transition_neural_parser-0.5.4/src/fairseq_ext/utils_import.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/README.md` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/README.md`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_leamr.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/align_leamr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/align_utils.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/align_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/alignment_decoder.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/alignment_decoder.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/amr_utils.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/amr_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.launch_many_jobs.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/ccc.launch_many_jobs.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/ccc.summarize.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/ccc.summarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/dummy_align.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/dummy_align.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/evaluation.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/evaluation.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/formatter.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/formatter.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/gcn.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/gcn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/lexicon.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/lexicon.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/main.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/main.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/make_splits.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/make_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/metric_utils.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/metric_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/pretrained_embeddings.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/resolve_manual_alignments.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/resolve_manual_alignments.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_detailed_eval.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_detailed_eval.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_eval.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_eval.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_model_selection.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_model_selection.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/run_sampler.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/run_sampler.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/standalone_elmo.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/standalone_elmo.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/tokenize_amr.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/tokenize_amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/transformer_lm.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_lstm.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/tree_lstm.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/tree_rnn.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/tree_rnn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/view_manual_alignments.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/view_manual_alignments.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/ibm_neural_aligner/vocab.py` & `transition_neural_parser-0.5.4/src/ibm_neural_aligner/vocab.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/__init__.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import subprocess
 import warnings
 # check for installation of torch-scatter
 try:
     import torch_scatter
 except:
     warnings.warn("torch-scatter is either not installed or not properly installed; please check for the appropriate version", UserWarning)
-    raise Exception("please review instruction on installing the appropriate version of torch-scatter")
+    raise Exception("please review README.d instructions on installing the appropriate version of torch-scatter")
     # cmd = ["pip", "install", "torch-scatter", "-f", "https://data.pyg.org/whl/torch-1.13.1+cu117.html"]
     # print("try downloading torch-scatter")
     # subprocess.call(cmd)
 
 # set this to true to start the debugger on any exception
 DEBUG_MODE = False
 if DEBUG_MODE:
```

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/amr_parser.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/amr_parser.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_data_oracle.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_data_oracle.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_fake_parse.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_fake_parse.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/parse.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/parse.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/action_pointer/roberta_utils.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/action_pointer/roberta_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/add_id_to_amr.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/add_id_to_amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/add_sentence_amrs_to_file.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/add_sentence_amrs_to_file.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_aligner.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/amr_aligner.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_constituents.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/amr_constituents.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_latex.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/amr_latex.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/amr_machine.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/amr_machine.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/clbar.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/clbar.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/force_overlap_actions.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/force_overlap_actions.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/gold_subgraph_align.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/gold_subgraph_align.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/io.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/io.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/make_sliding_splits.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/make_sliding_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/merge_sliding_splits.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/merge_sliding_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/parse.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Standalone AMR parser from an existing trained APT model
 
 import os
+import re
 import time
 import math
 import copy
 import signal
 import argparse
 from datetime import timedelta
 import urllib.request
@@ -43,29 +44,39 @@
     check_pointers
 )
 from transition_amr_parser.amr_machine import play_all_actions
 from transition_amr_parser.clbar import yellow_font
 from transition_amr_parser.amr_machine import make_eos_force_actions
 
 
+UNICODE_WHITESPACE = [
+    u'\t', u'\n', u'\x0b', u'\x0c', u'\r', u'\x1c', u'\x1d', u'\x1e', u'\x1f',
+    u'\x85', u'\xa0', u'\u1680', u'\u2000', u'\u2001', u'\u2002', u'\u2003',
+    u'\u2004', u'\u2005', u'\u2006', u'\u2007', u'\u2008', u'\u2009',
+    u'\u200a', u'\u2028', u'\u2029', u'\u202f', u'\u205f', u'\u3000'
+]
+UNI_WHITESPACE_RE = re.compile('|'.join(UNICODE_WHITESPACE))
+
+
 def argument_parsing():
 
     # Argument hanlding
     parser = argparse.ArgumentParser(
         description='Call parser from the command line'
     )
     parser.add_argument(
         '-i', '--in-tokenized-sentences',
         type=str,
         help='File with one __tokenized__ sentence per line'
     )
     parser.add_argument(
         '--in-doc',
         type=str,
-        help='File with one __tokenized__ sentence per line and one newline separating each doc (and the end)'
+        help='File with one __tokenized__ sentence per line and one newline '
+             'separating each doc (and the end)'
     )
     parser.add_argument(
         '--in-amr',
         type=str,
         help='AMR in Penman format to align'
     )
     parser.add_argument(
@@ -135,16 +146,18 @@
         '-c', '--in-checkpoint',
         type=str,
         help='one fairseq model checkpoint (or various, separated by :)'
     )
     parser.add_argument(
         '-m', '--model-name',
         type=str,
-        help='name of model config (instead of checkpoint) and optionally'
-             'seed separated by : e.g. amr2.0-structured-bart-large:42'
+        help="pretrained checkpoint name; will first check if it is already in \
+            cache, if not will automatically download and save to cache.; \
+            eg: AMR2-structbart-L \
+            for complete list of available checkpoint names, see README"
     )
     parser.add_argument(
         '-o', '--out-amr',
         type=str,
         help='File to store AMR in PENNMAN format'
     )
     parser.add_argument(
@@ -213,45 +226,59 @@
     )
     args = parser.parse_args()
 
     # sanity checks
     assert (
         bool(args.in_tokenized_sentences) or bool(args.in_amr)
     ) or bool(args.service) or bool(args.in_doc), \
-        "Must either specify --in-tokenized-sentences or --in-doc or set --service"
+        "Must either specify --in-tokenized-sentences or --in-doc or set " \
+        "--service"
 
     if not (bool(args.model_name) ^ bool(args.in_checkpoint)):
         raise Exception("Use either --model-name or --in-checkpoint")
 
     if bool(args.in_actions) and bool(args.tokenize):
         raise Exception(
             "Remove --tokenize option when enabling --force-actions and"
             "provide tokenized input matching the dimensions of force actions."
         )
     if bool(args.in_actions) and bool(args.in_doc):
         print(yellow_font(
-            'WARNING: Given force actions will be used superseding the force actions generated by the inhouse force action generator. Make sure it is in the correct format '))
+            'WARNING: Given force actions will be used superseding the force '
+            'actions generated by the inhouse force action generator. Make '
+            'sure it is in the correct format '
+        ))
 
     # num samples replaces beam search
     if args.num_samples:
         assert args.nbest == 1
         assert args.beam == 1
 
     if args.sampling_topp != -1:
         assert args.num_samples
 
     return args
 
-
+############### HELPER FUNCTIONS ##########################
 def ordered_exit(signum, frame):
     print("\nStopped by user\n")
     exit(0)
 
 
 def load_models_and_task(args, use_cuda, task=None):
+    """Fairseq load from task method
+
+    Args:
+        args (args): args from argparser
+        use_cuda (bool): _description_
+        task (FaiseqTask, optional): _description_. Defaults to None.
+
+    Returns:
+        _type_: _description_
+    """
     # if `task` is not provided, it will be from the saved model args
     models, model_args, task = checkpoint_utils.load_model_ensemble_and_task(
         args.path.split(':'),
         arg_overrides=args.model_overrides,
         task=task,
     )
     # Optimize ensemble for generation
@@ -270,15 +297,22 @@
             print('using CPU for models')
 
     # model = Model(models, task.target_dictionary)
     return models, model_args, task
 
 
 def load_args_from_config(config_path):
-    """Load args from bash configuration scripts"""
+    """Load args from bash configuration scripts
+
+    Args:
+        config_path (str): the path to a training configuration file
+
+    Returns:
+        dict: dictionary containing config info
+    """
     # TODO there might be better ways; e.g. source the bash script in python
     # and use $BERT_LAYERS directly
     config_dict = {}
     with open(config_path, 'r') as f:
         for line in f:
             if line.strip():
                 if not line.startswith('#') and '=' in line:
@@ -485,14 +519,15 @@
         all_tokens.append(tokens)
 
     # create final graphs
     annotations, machines = play_all_actions(
         all_tokens, all_actions, parser.machine_config)
     return annotations, machines
 
+############### END HELPER FUNCTIONS ##########################
 
 class AMRParser:
     def __init__(
         self,
         models,           # PyTorch model
         task,             # fairseq task
         src_dict,         # fairseq dict
@@ -581,22 +616,22 @@
         return cls.from_checkpoint(checkpoint, **kwargs)
 
     @classmethod
     def from_pretrained(cls, model_name, dict_dir=None,
                         roberta_cache_path=None, fp16=False,
                         inspector=None, beam=1, nbest=1, num_samples=None,
                         sampling_topp=-1, temperature=1.0):
-        """ Load model checkpoints from available model names; 
-        Will check if the model is downloaded to cache, if not, download from cloud storage; 
+        """ Load model checkpoints from available model names;
+        Will check if the model is downloaded to cache, if not, download from cloud storage;
         Below is a list of available modelnames to trun
             {
                 'AMR3.0':'https://s3.us-east.cloud-object-storage.appdomain.cloud/cloud-object-storage-xc-cos-standard-htg/amr3.0-structured-bart-large-neur-al-sampling5.zip'
             }
         Args:
-            modelname (str): a model name within our pretrained model library. 
+            modelname (str): a model name within our pretrained model library.
             dict_dir (_type_, optional): _description_. Defaults to None.
             roberta_cache_path (_type_, optional): _description_. Defaults to None.
             fp16 (bool, optional): _description_. Defaults to False.
             inspector (_type_, optional): _description_. Defaults to None.
             beam (int, optional): _description_. Defaults to 1.
             nbest (int, optional): _description_. Defaults to 1.
             num_samples (_type_, optional): _description_. Defaults to None.
@@ -643,14 +678,15 @@
             eval_metric = "wiki.smatch"
 
         model_name = zip_file.split("-seed")[0]
         seed = zip_file.split("-seed")[1][:2]
 
         # get cache storage dir, in which we save the downloaded models
         cache_dir = torch.hub._get_torch_home() + '/'
+        os.makedirs(cache_dir, exist_ok=True)
         cache_save_zip = cache_dir + zip_file
 
         # get checkpoint path
         model_dir_path = os.path.join(
             cache_dir, "DATA", model_class, "models", model_name, "seed"+str(seed))
         checkpoint_path = model_dir_path + "/checkpoint_"+eval_metric+"_top5-avg.pt"
 
@@ -680,36 +716,55 @@
                 urllib.request.urlretrieve(
                     model_url, cache_save_zip, show_progress)
             else:
                 print("a model zip file is already downloaded")
 
             if os.path.getsize(cache_save_zip) < 1000000:
                 raise Exception(
-                    "our model download limit is reached; please try downloading  again next week.")
+                    "our model download limit is reached; please try "
+                    "downloading  again next week."
+                )
 
             with zipfile.ZipFile(cache_dir + zip_file, 'r') as zip_ref:
                 zip_ref.extractall(torch.hub._get_torch_home())
-            print("downloaded model unzipped")
-            assert os.path.isfile(
-                checkpoint_path), 'checkpoint still not available after downloads;'
+            print(f"downloaded model unzipped to {checkpoint_path}")
+            assert os.path.isfile(checkpoint_path), \
+                'checkpoint still not available after downloads'
         else:
-            print('model is already in cache')
+            print(f'load from cache {checkpoint_path}')
         return cls.from_checkpoint(checkpoint_path, dict_dir,
                                    roberta_cache_path, fp16, inspector,
                                    beam, nbest, num_samples, sampling_topp,
                                    temperature)
 
     @classmethod
     def from_checkpoint(cls, checkpoint, dict_dir=None,
                         roberta_cache_path=None, fp16=False,
                         inspector=None, beam=1, nbest=1, num_samples=None,
                         sampling_topp=-1, temperature=1.0):
-        '''
-        Initialize model from checkpoint
-        '''
+        """ Load a checkpoint from model path
+
+        Args:
+            checkpoint (str): path to the model checkpoint
+            dict_dir (_type_, optional): _description_. Defaults to None.
+            roberta_cache_path (_type_, optional): _description_. Defaults to None.
+            fp16 (bool, optional): _description_. Defaults to False.
+            inspector (_type_, optional): _description_. Defaults to None.
+            beam (int, optional): _description_. Defaults to 1.
+            nbest (int, optional): _description_. Defaults to 1.
+            num_samples (_type_, optional): _description_. Defaults to None.
+            sampling_topp (int, optional): _description_. Defaults to -1.
+            temperature (float, optional): _description_. Defaults to 1.0.
+
+        Raises:
+            ValueError: _description_
+
+        Returns:
+            _type_: _description_
+        """
         # load default args: some are dummy
         parser = options.get_interactive_generation_parser()
         # model path set here
         default_args = cls.default_args(checkpoint, fp16=fp16)
         args = options.parse_args_and_arch(parser, input_args=default_args)
         import_user_module(args)
         # when `input_args` is fed in, it overrides the command line input args
@@ -937,15 +992,15 @@
 
     def parse_sentence(self, tokens, **kwargs):
         annotations, decoding_data = self.parse_sentences([tokens], **kwargs)
         return annotations[0], decoding_data[0]
 
     def parse_sentences(self, batch, batch_size=128, roberta_batch_size=128,
                         gold_amrs=None, force_actions=None, beam=1, jamr=False,
-                        no_isi=False):
+                        no_isi=False, unicode_normalize=True):
         """parse a list of sentences.
 
         Args:
             batch (List[List[str]]): list of tokenized sentences.
             batch_size (int, optional): batch size. Defaults to 128.
             roberta_batch_size (int, optional): RoBerta batch size. Defaults to
             10.
@@ -959,15 +1014,19 @@
         if len(batch) < batch_size:
             batch_size = len(batch)
         print("Running on batch size: " + str(batch_size))
 
         sentences = []
         # The model expects <ROOT> token at the end of the input sentence
         for tokens in batch:
-            sentences.append(" ".join(tokens))
+            sentence = " ".join(tokens).strip()
+            if unicode_normalize:
+                sentence = UNI_WHITESPACE_RE.sub(' ', sentence)
+                sentence = re.sub('  +', ' ', sentence)
+            sentences.append(sentence)
 
         data = self.convert_sentences_to_data(
             sentences,
             batch_size,
             roberta_batch_size,
             gold_amrs=gold_amrs,
             force_actions=force_actions
@@ -1100,37 +1159,40 @@
             with open(f'{out_path}.{j}', 'w') as fid:
                 fid.write('\n'.join([x[j] for x in string_list]))
                 fid.write('\n')
             print(f'{out_path}.{j}')
 
 
 def load_parser(args, inspector):
+    """ A meta load to check for loading from model name, or loading 
+    from checkpoint path
+
+    Args:
+        args (_type_): arguments from arg parser
+        inspector (_type_): function to call after each step
+
+    Returns:
+        AMRParser: AMRParser class object
+
+    """
 
     if args.model_name:
-        # load from name and optionally seed
-        items = args.model_name.split(':')
-        model_name = items[0]
-        if len(items) > 1:
-            seed = items[1]
-        else:
-            seed = None
-        # load from model/config name
-        return AMRParser.load(
-            model_name,
-            seed=seed,
+        return AMRParser.from_pretrained(
+            args.model_name,
             roberta_cache_path=args.roberta_cache_path,
             inspector=inspector,
             # selected fairseq decoder arguments
             beam=args.beam,
             nbest=args.nbest,
             fp16=args.fp16,
             sampling_topp=args.sampling_topp,
             # this is not, but implies --sampling
             num_samples=args.num_samples
         )
+
     else:
         # load from checkpoint and files in its folder
         return AMRParser.from_checkpoint(
             args.in_checkpoint,
             roberta_cache_path=args.roberta_cache_path,
             inspector=inspector,
             # selected fairseq decoder arguments
@@ -1219,15 +1281,14 @@
 
         else:
             print(''.join(result[0]))
 
 
 def prepare_data(args, parser):
 
-    force_actions = None
     if args.in_amr:
 
         # align mode: read input AMR to be aligned
         gold_amrs = read_amr(args.in_amr)
         if args.tokenize:
             # jamr-like tokenization
             assert all(amr.sentence is not None for amr in gold_amrs), \
@@ -1354,16 +1415,16 @@
         tok_sentences, gold_amrs = prepare_data(args, parser)
         force_actions = None
 
         # read constrained decoding forced actions if provided
         if args.in_actions:
             with open(args.in_actions) as fact:
                 force_actions = [eval(line.strip()) + [[]] for line in fact]
-            assert len(tok_sentences) == len(
-                force_actions), "Number of force actions doesn't match the number of sentences"
+            assert len(tok_sentences) == len(force_actions), \
+                "Number of force actions doesn't match the number of sentences"
 
             # sampling needs copy of force actions N times
             if args.num_samples is not None:
                 force_actions = [
                     a
                     for a in force_actions
                     for _ in range(args.num_samples)
@@ -1372,23 +1433,25 @@
         # TODO: max batch sizes could be computed from max sentence length
 
         num_sent = len(tok_sentences)
         print(f'Parsing {num_sent} sentences')
         start = time.time()
 
         if args.in_doc:
-            annotations, machines = parser.parse_docs(tok_sentences,
-                                                      gold_amrs=gold_amrs,
-                                                      window_size=args.window_size,
-                                                      window_overlap=args.window_overlap,
-                                                      batch_size=args.batch_size,
-                                                      roberta_batch_size=args.roberta_batch_size,
-                                                      beam=args.beam,
-                                                      jamr=args.jamr,
-                                                      no_isi=args.no_isi)
+            annotations, machines = parser.parse_docs(
+                tok_sentences,
+                gold_amrs=gold_amrs,
+                window_size=args.window_size,
+                window_overlap=args.window_overlap,
+                batch_size=args.batch_size,
+                roberta_batch_size=args.roberta_batch_size,
+                beam=args.beam,
+                jamr=args.jamr,
+                no_isi=args.no_isi
+            )
 
         else:
 
             # normal parsing
             annotations, machines = parser.parse_sentences(
                 tok_sentences,
                 batch_size=args.batch_size,
```

### Comparing `transition_neural_parser-0.5.3/src/transition_amr_parser/plots.py` & `transition_neural_parser-0.5.4/src/transition_amr_parser/plots.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/PKG-INFO` & `transition_neural_parser-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: transition-neural-parser
-Version: 0.5.3
+Name: transition_neural_parser
+Version: 0.5.4
 Summary: The package for transition based nueral AMR parser
 Author-email: Ramon <ramon.astudillo@ibm.com>, Young-Suk <ysuklee@us.ibm.com>, Tahira <tnaseem@us.ibm.com>, Sadhana <sadhana.kumaravel1@ibm.com>, GX <GX.Xu@ibm.com>, Hans <raduf@us.ibm.com>, Salim <roukos@us.ibm.com>
-Project-URL: homepage, https://github.ibm.com/mnlp/transition-amr-parser/tree/master
-Project-URL: tracker, https://github.ibm.com/mnlp/transition-amr-parser/issues
+Project-URL: homepage, https://github.com/IBM/transition-amr-parser
+Project-URL: tracker, https://github.com/IBM/transition-amr-parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: ~=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Transition-based Neural Parser
 ============================
 
 State-of-the-Art Abstract Meaning Representation (AMR) parsing, see [papers
 with code](https://paperswithcode.com/task/amr-parsing). Models both
 distribution over graphs and aligments with a transition-based approach. Parser
-supports any other graph formalism as long as it is expressed in [Penman
+supports generic text-to-graph as long as it is expressed in [Penman
 notation](https://penman.readthedocs.io/en/latest/notation.html).
 
 Some of the main features
 
 - [Smatch](https://github.com/snowblink14/smatch) wrapper providing [significance testing](scripts/README.md#paired-boostrap-significance-test-for-Smatch) for Smatch and [MBSE](scripts/README.md#maximum-bayesian-smatch-ensemble-mbse) ensembling.
 - `Structured-BART` [(Zhou et al 2021b)](https://aclanthology.org/2021.emnlp-main.507/) with [trained checkpoints](#available-pretrained-model-checkpoints) for document-level AMR [(Naseem et al 2022)](https://aclanthology.org/2022.naacl-main.256), MBSE [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) and latent alignments training [(Drozdov et al 2022)](https://arxiv.org/abs/2205.01464)
 - `Structured-mBART` for multi-lingual support (EN, DE, Zh, IT) [(Lee et al 2022)](https://arxiv.org/abs/2112.07790)
@@ -39,42 +39,49 @@
 ```
 
 or alternatively use `virtualenv` and `pyenv` for python versions. Note that
 all scripts source a `set_environment.sh` script that you can use to activate
 your virtual environment as above and set environment variables. If not used,
 just create an empty version
 
-```
+```bash
 # or e.g. put inside conda activate ./cenv_x86
 touch set_environment.sh
 ```
 
-Then install the parser package using pip. You will need to install
-`torch-scatter` by separate since it is custom built for CUDA. Here we specify the
+Then install the parser package using pip. You will need to manually install
+`torch-scatter` since it is custom built for CUDA. Here we specify the
 call for `torch 1.13.1` and `cuda 11.7`. See [torch-scatter
 repository](https://pypi.org/project/torch-scatter/) to find the appropriate
-installation instructions.
+installation instructions. 
 
-```
+**For MacOS users** 
+
+(Please install the cpu version of torch-scatter; and model training is not fully supported here.)
+
+```bash
 pip install transition-neural-parser
+# for linux users
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
+# for cpu installation for MacOS
+# pip install torch-scatter
 ```
 
 If you plan to edit the code, clone and install instead
 
-```
+```bash
 # clone this repo (see link above), then
 cd transition-neural-parser
 pip install --editable .
 pip install torch-scatter -f https://data.pyg.org/whl/torch-1.13.1+cu117.html
 ```
 
 If you want to train a document-level AMR parser you will also need 
 
-```
+```bash
 git clone https://github.com/IBM/docAMR.git
 cd docAMR
 pip install .
 cd ..
 ```
 
 ## Parse with a pretrained model
@@ -188,28 +195,26 @@
 | AMR3-joint-ontowiki-seed44 | amr3joint_ontowiki2_g2g-structured-bart-large-seed44  | [(Lee et al 2022)](https://arxiv.org/abs/2112.07790) (ensemble) | 84.4          |
 | doc-sen-conll-amr-seed42   | both_doc+sen_trainsliding_ws400x100-seed42            |                                                                 | 82.3<sup>1</sup>/71.8 <sup>2</sup>|              |
 
 <sup>1 Smatch on AMR3.0 sentences</sup>
 
 <sup>2 Smatch on AMR3.0 Multi-Sentence dataset </sup>
 
-we also provide the trained `ibm-neural-aligner` under names
-`AMR2.0_ibm_neural_aligner.zip` and `AMR3.0_ibm_neural_aligner.zip`. For the
+contact authors to obtain the trained `ibm-neural-aligner`. For the
 ensemble we provide the three seeds. Following fairseq conventions, to run the
 ensemble just give the three checkpoint paths joined by `:` to the normal
 checkpoint argument `-c`. Note that the checkpoints were trained with the
 `v0.5.1` tokenizer, this reduces performance by `0.1` on `v0.5.2` tokenized
 data.
 
 Note that we allways report average of three seeds in papers while these are
 individual models. A fast way to test models standalone is
 
     bash tests/standalone.sh configs/<config>.sh
 
-
 ## Training a model
 
 You first need to pre-process and align the data. For AMR2.0 do
 
 ```bash
 conda activate ./cenv_x86 # activate parser environment
 python scripts/merge_files.py /path/to/LDC2017T10/data/amrs/split/ DATA/AMR2.0/corpora/
```

### Comparing `transition_neural_parser-0.5.3/src/transition_neural_parser.egg-info/SOURCES.txt` & `transition_neural_parser-0.5.4/src/transition_neural_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

