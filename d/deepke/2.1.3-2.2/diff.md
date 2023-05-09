# Comparing `tmp/deepke-2.1.3.tar.gz` & `tmp/deepke-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepke-2.1.3.tar", last modified: Wed Mar 15 05:32:36 2023, max compression
+gzip compressed data, was "deepke-2.2.tar", last modified: Tue Apr  4 11:17:11 2023, max compression
```

## Comparing `deepke-2.1.3.tar` & `deepke-2.2.tar`

### file list

```diff
@@ -1,189 +1,255 @@
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.879947 deepke-2.1.3/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      508 2023-03-15 05:32:36.879947 deepke-2.1.3/PKG-INFO
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    26581 2023-03-13 12:33:01.000000 deepke-2.1.3/README.md
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       38 2023-03-15 05:32:36.879947 deepke-2.1.3/setup.cfg
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      925 2023-03-15 05:29:33.000000 deepke-2.1.3/setup.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.847943 deepke-2.1.3/src/
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.863945 deepke-2.1.3/src/deepke/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      134 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.863945 deepke-2.1.3/src/deepke/attribution_extraction/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       23 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.863945 deepke-2.1.3/src/deepke/attribution_extraction/standard/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       85 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.863945 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      846 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/BasicModule.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      944 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/BiLSTM.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1863 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/Capsule.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1016 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/GCN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      975 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/LM.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2257 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/PCNN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1169 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/Transformer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      192 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/models/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5498 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Attention.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4152 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/CNN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1785 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Capsule.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1595 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Embedding.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3759 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/GCN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2144 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/RNN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6206 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Transformer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      217 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/module/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      141 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2195 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/dataset.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1884 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/metrics.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6298 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/preprocess.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8713 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/serializer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4112 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/trainer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2964 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/vocab.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/attribution_extraction/standard/utils/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       45 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/utils/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4660 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/utils/ioUtils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2580 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/attribution_extraction/standard/utils/nnUtils.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/event_extraction/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       23 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/event_extraction/standard/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       21 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/standard/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/event_extraction/standard/degree/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       98 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/standard/degree/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    11321 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/standard/degree/data.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1843 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/standard/degree/model.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)   214556 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/standard/degree/template_generate_ace.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1309 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/event_extraction/standard/degree/utils.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/name_entity_re/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       74 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/name_entity_re/few_shot/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       64 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/name_entity_re/few_shot/models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       49 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/models/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    34718 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/models/model.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    66837 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/models/modeling_bart.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.867945 deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       95 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12200 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/datasets.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4886 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/mapping_type.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3806 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/metrics.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10334 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/train.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/few_shot/utils/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       19 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/utils/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6012 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/few_shot/utils/util.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/multimodal/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3282 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/IFA_model.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       72 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      258 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12646 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/configuration_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9151 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/feature_extraction_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    22998 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/feature_extraction_utils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)   108380 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/file_utils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9034 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/image_utils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    46165 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/modeling_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8510 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/processing_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    14497 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/tokenization_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    35007 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/modeling_IFA.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/multimodal/modules/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/modules/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     7633 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/modules/dataset.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    16969 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/multimodal/modules/train.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/standard/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       42 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/standard/models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1505 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/models/BiLSTM_CRF.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     7626 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/models/InferBert.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       50 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/models/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/standard/tools/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       48 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/tools/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3312 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/tools/dataset.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5625 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/tools/preprocess.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       68 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9024 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/data_loader.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9471 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/model.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3436 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/utils.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.871946 deepke-2.1.3/src/deepke/relation_extraction/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       98 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/document/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      138 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5962 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/evaluation.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1723 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/losses.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8509 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/model.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3791 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/module.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10803 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/prepro.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2635 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/document/utils.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/few_shot/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      112 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       23 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2174 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/base_data_module.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1799 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/dialogue.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    36438 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/processor.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1667 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/generate_k_shot.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1332 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/get_label_word.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       78 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4581 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/base.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9432 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/transformer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6979 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/util.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/multimodal/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3781 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/IFA_model.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       72 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      258 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12646 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/configuration_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9151 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/feature_extraction_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    22998 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/feature_extraction_utils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)   108380 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/file_utils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9034 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/image_utils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    46165 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/modeling_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8510 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/processing_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    14497 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/clip/tokenization_clip.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    35007 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/models/modeling_IFA.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       66 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8700 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/dataset.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1340 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/metrics.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12010 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/train.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.875946 deepke-2.1.3/src/deepke/relation_extraction/standard/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       85 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.879947 deepke-2.1.3/src/deepke/relation_extraction/standard/models/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      845 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/BasicModule.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      904 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/BiLSTM.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1819 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/Capsule.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      972 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/GCN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      974 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/LM.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2216 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/PCNN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1128 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/Transformer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      192 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/models/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.879947 deepke-2.1.3/src/deepke/relation_extraction/standard/module/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4722 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/Attention.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4148 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/CNN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1785 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/Capsule.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1518 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/Embedding.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1482 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/GCN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2143 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/RNN.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6206 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/Transformer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      217 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/module/__init__.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.879947 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      161 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2080 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/dataset.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3708 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/loss.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1884 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/metrics.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9080 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/preprocess.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8714 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/serializer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4112 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/trainer.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2966 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/tools/vocab.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.879947 deepke-2.1.3/src/deepke/relation_extraction/standard/utils/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       45 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/utils/__init__.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4660 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/utils/ioUtils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2580 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/relation_extraction/standard/utils/nnUtils.py
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3671 2023-03-13 12:33:02.000000 deepke-2.1.3/src/deepke/transform_data.py
-drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-03-15 05:32:36.863945 deepke-2.1.3/src/deepke.egg-info/
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      508 2023-03-15 05:32:36.000000 deepke-2.1.3/src/deepke.egg-info/PKG-INFO
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8305 2023-03-15 05:32:36.000000 deepke-2.1.3/src/deepke.egg-info/SOURCES.txt
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        1 2023-03-15 05:32:36.000000 deepke-2.1.3/src/deepke.egg-info/dependency_links.txt
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      332 2023-03-15 05:32:36.000000 deepke-2.1.3/src/deepke.egg-info/requires.txt
--rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        7 2023-03-15 05:32:36.000000 deepke-2.1.3/src/deepke.egg-info/top_level.txt
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.601854 deepke-2.2/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      506 2023-04-04 11:17:11.601854 deepke-2.2/PKG-INFO
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    28945 2023-04-04 11:15:57.000000 deepke-2.2/README.md
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       38 2023-04-04 11:17:11.601854 deepke-2.2/setup.cfg
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      923 2023-04-04 11:15:57.000000 deepke-2.2/setup.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.577854 deepke-2.2/src/
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.581854 deepke-2.2/src/deepke/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      171 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/attribution_extraction/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       23 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/attribution_extraction/standard/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       85 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/attribution_extraction/standard/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      846 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/BasicModule.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      944 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/BiLSTM.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1863 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/Capsule.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1016 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/GCN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      975 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/LM.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2257 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/PCNN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1169 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/Transformer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      192 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/attribution_extraction/standard/models/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/attribution_extraction/standard/module/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5498 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/Attention.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4152 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/CNN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1785 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/Capsule.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1595 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/Embedding.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3759 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/GCN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2144 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/RNN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6206 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/Transformer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      217 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/module/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/attribution_extraction/standard/tools/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      141 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2195 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/dataset.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1884 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/metrics.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6298 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/preprocess.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8713 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/serializer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4112 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/trainer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2964 2023-04-04 11:16:10.000000 deepke-2.2/src/deepke/attribution_extraction/standard/tools/vocab.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/attribution_extraction/standard/utils/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       45 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/utils/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4660 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/utils/ioUtils.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2580 2023-04-04 11:16:11.000000 deepke-2.2/src/deepke/attribution_extraction/standard/utils/nnUtils.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/event_extraction/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       23 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/event_extraction/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/event_extraction/standard/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/event_extraction/standard/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/event_extraction/standard/bertcrf/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       94 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/event_extraction/standard/bertcrf/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6972 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/event_extraction/standard/bertcrf/bert_crf.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    14535 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/event_extraction/standard/bertcrf/crf.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    21497 2023-04-04 11:16:27.000000 deepke-2.2/src/deepke/event_extraction/standard/bertcrf/processor_ee.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2698 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/event_extraction/standard/bertcrf/utils_ee.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/event_extraction/standard/degree/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       98 2023-04-04 11:16:27.000000 deepke-2.2/src/deepke/event_extraction/standard/degree/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    11373 2023-04-04 11:16:28.000000 deepke-2.2/src/deepke/event_extraction/standard/degree/data.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1892 2023-04-04 11:16:27.000000 deepke-2.2/src/deepke/event_extraction/standard/degree/model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)   202461 2023-04-04 11:16:27.000000 deepke-2.2/src/deepke/event_extraction/standard/degree/template_generate_ace.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1309 2023-04-04 11:16:27.000000 deepke-2.2/src/deepke/event_extraction/standard/degree/utils.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/name_entity_re/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       94 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke/name_entity_re/cross/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       75 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/cross/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/extraction/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      241 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      941 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/constants.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3829 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/dataset_processer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1946 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/extraction_metrics.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1611 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/label_tree.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/extraction/noiser/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       31 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/noiser/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3691 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/noiser/spot_asoc_noiser.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/extraction/predict_parser/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      302 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/predict_parser/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      434 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/predict_parser/predict_parser.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9819 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/predict_parser/spotasoc_predict_parser.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3151 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/predict_parser/utils.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1912 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/record_schema.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    25324 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/scorer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2567 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/cross/extraction/utils.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/sel2record/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       47 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/sel2record/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    15487 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/sel2record/record.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4805 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/sel2record/sel2record.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      236 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10957 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/constrained_seq2seq.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1059 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2720 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/constraint_decoder.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12011 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/spotasoc_constraint_decoder.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/data_collator/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      473 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/data_collator/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2430 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/data_collator/hybird_data_collator.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12194 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/data_collator/meta_data_collator.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8521 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/data_collator/t5mlm_data_collator.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3321 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/features.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    84245 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/modeling_t5.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    22273 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/models.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4186 2023-04-04 11:16:20.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/t5_bert_tokenizer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10220 2023-04-04 11:16:19.000000 deepke-2.2/src/deepke/name_entity_re/cross/seq2seq/trainer_arguments.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/few_shot/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       64 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/few_shot/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       49 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/models/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    36320 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/models/model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    70505 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/models/modeling_bart.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/few_shot/module/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       95 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/module/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12200 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/module/datasets.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4886 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/module/mapping_type.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3806 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/module/metrics.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10334 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/module/train.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/few_shot/utils/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       19 2023-04-04 11:16:18.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/utils/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6012 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/name_entity_re/few_shot/utils/util.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/multimodal/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.589854 deepke-2.2/src/deepke/name_entity_re/multimodal/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3215 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/models/IFA_model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       52 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/models/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    35007 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/models/modeling_IFA.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/name_entity_re/multimodal/modules/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/modules/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     7592 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/modules/dataset.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    16969 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/name_entity_re/multimodal/modules/train.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/name_entity_re/standard/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       42 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/standard/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/name_entity_re/standard/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1505 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/models/BiLSTM_CRF.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     7626 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/models/InferBert.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       50 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/models/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/name_entity_re/standard/tools/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       48 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/standard/tools/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3312 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/standard/tools/dataset.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5625 2023-04-04 11:16:21.000000 deepke-2.2/src/deepke/name_entity_re/standard/tools/preprocess.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/name_entity_re/standard/w2ner/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       68 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/w2ner/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9024 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/w2ner/data_loader.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9471 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/w2ner/model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3436 2023-04-04 11:16:22.000000 deepke-2.2/src/deepke/name_entity_re/standard/w2ner/utils.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       98 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/document/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      138 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/document/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5962 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/document/evaluation.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1723 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/document/losses.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8509 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/document/model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3791 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/document/module.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10803 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/document/prepro.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2635 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/document/utils.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/few_shot/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      112 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       23 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2174 2023-04-04 11:16:12.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/base_data_module.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1799 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/dialogue.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    36438 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/processor.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1667 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/generate_k_shot.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1332 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/get_label_word.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       78 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4581 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/base.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9432 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/transformer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6979 2023-04-04 11:16:13.000000 deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/util.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/multimodal/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       44 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/multimodal/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3714 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/models/IFA_model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       52 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/models/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    35007 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/models/modeling_IFA.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/multimodal/modules/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       66 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/modules/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8659 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/modules/dataset.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1340 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/modules/metrics.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12010 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/relation_extraction/multimodal/modules/train.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.593854 deepke-2.2/src/deepke/relation_extraction/standard/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       85 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/relation_extraction/standard/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      845 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/BasicModule.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      904 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/BiLSTM.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1819 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/Capsule.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      972 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/GCN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      974 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/LM.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2216 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/PCNN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1128 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/Transformer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      192 2023-04-04 11:16:16.000000 deepke-2.2/src/deepke/relation_extraction/standard/models/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/relation_extraction/standard/module/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4722 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/Attention.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4148 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/CNN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1785 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/Capsule.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1518 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/Embedding.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1482 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/GCN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2143 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/RNN.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     6206 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/Transformer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      217 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/module/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/relation_extraction/standard/tools/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      161 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2080 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/dataset.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3708 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/loss.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1884 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/metrics.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9080 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/preprocess.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8714 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/serializer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4112 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/trainer.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2966 2023-04-04 11:16:14.000000 deepke-2.2/src/deepke/relation_extraction/standard/tools/vocab.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/relation_extraction/standard/utils/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       45 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/utils/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4660 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/utils/ioUtils.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     2580 2023-04-04 11:16:15.000000 deepke-2.2/src/deepke/relation_extraction/standard/utils/nnUtils.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     3671 2023-04-04 11:16:17.000000 deepke-2.2/src/deepke/transform_data.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/triple_extraction/
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/triple_extraction/ASP/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      103 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/triple_extraction/ASP/metrics/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      122 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/metrics/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     9746 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/metrics/blanc.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4210 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/metrics/conll.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10783 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/metrics/metrics.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/triple_extraction/ASP/modeling_transformer/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       31 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/modeling_transformer/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1118 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/modeling_transformer/modeling_outputs.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.597854 deepke-2.2/src/deepke/triple_extraction/ASP/models/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      151 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12058 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/model_coref.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    13011 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/model_ere.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10341 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/model_ner.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     1118 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/modeling_outputs.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    25647 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/t5_coref.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    27032 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/t5_ere.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    22005 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/ASP/models/t5_ner.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.601854 deepke-2.2/src/deepke/triple_extraction/ASP/util/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       60 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    16182 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/func.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10396 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/multigpu_fused_adam.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    12983 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/runner.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10400 2023-04-04 11:16:23.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/tensorize_coref.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    13348 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/tensorize_ere.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     8976 2023-04-04 11:16:24.000000 deepke-2.2/src/deepke/triple_extraction/ASP/util/tensorize_ner.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.601854 deepke-2.2/src/deepke/triple_extraction/PRGC/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      193 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5673 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/dataloader.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     7656 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/dataloader_utils.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     7072 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/evaluate.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     4364 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/metrics.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10925 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/model.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    13225 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/optimization.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)     5082 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/PRGC/util.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.601854 deepke-2.2/src/deepke/triple_extraction/PURE/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:16:26.000000 deepke-2.2/src/deepke/triple_extraction/PURE/__init__.py
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)       62 2023-04-04 11:16:25.000000 deepke-2.2/src/deepke/triple_extraction/__init__.py
+drwxrwxr-x   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        0 2023-04-04 11:17:11.585854 deepke-2.2/src/deepke.egg-info/
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      506 2023-04-04 11:17:11.000000 deepke-2.2/src/deepke.egg-info/PKG-INFO
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)    10994 2023-04-04 11:17:11.000000 deepke-2.2/src/deepke.egg-info/SOURCES.txt
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        1 2023-04-04 11:17:11.000000 deepke-2.2/src/deepke.egg-info/dependency_links.txt
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)      332 2023-04-04 11:17:11.000000 deepke-2.2/src/deepke.egg-info/requires.txt
+-rw-rw-r--   0 qiaoshuofei  (1005) qiaoshuofei  (1005)        7 2023-04-04 11:17:11.000000 deepke-2.2/src/deepke.egg-info/top_level.txt
```

### Comparing `deepke-2.1.3/README.md` & `deepke-2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 <h1 align="center">
     <p>A Deep Learning Based Knowledge Extraction Toolkit<br>for Knowledge Graph Construction</p>
 </h1>
 
 
 [DeepKE](https://arxiv.org/pdf/2201.03335.pdf) is a knowledge extraction toolkit for knowledge graph construction supporting **cnSchema**，**low-resource**, **document-level** and **multimodal** scenarios for *entity*, *relation* and *attribute* extraction. We provide [documents](https://zjunlp.github.io/DeepKE/), [Google Colab tutorials](https://colab.research.google.com/drive/1vS8YJhJltzw3hpJczPt24O0Azcs3ZpRi?usp=sharing), [online demo](http://deepke.zjukg.cn/), [paper](https://arxiv.org/pdf/2201.03335.pdf), [slides](https://drive.google.com/file/d/1IIeIZAbVduemqXc4zD40FUMoPHCJinLy/view?usp=sharing) and [poster](https://drive.google.com/file/d/1vd7xVHlWzoAxivN4T5qKrcqIGDcSM1_7/view?usp=sharing) for beginners.
-- ❗New: We have released the [DeepKE-GPT](http://deepke.openkg.cn/EN/llm.html) (Based on ChatGPT).
 
 **Reading Materials**:
 
 Data-Efficient Knowledge Graph Construction, 高效知识图谱构建 ([Tutorial on CCKS 2022](http://sigkg.cn/ccks2022/?page_id=24)) \[[slides](https://drive.google.com/drive/folders/1xqeREw3dSiw-Y1rxLDx77r0hGUvHnuuE)\] 
 
 Efficient and Robust Knowledge Graph Construction ([Tutorial on AACL-IJCNLP 2022](https://www.aacl2022.org/Program/tutorials)) \[[slides](https://github.com/NLP-Tutorials/AACL-IJCNLP2022-KGC-Tutorial)\] 
 
@@ -48,14 +47,17 @@
 
 **Related Toolkit**:
 
 [Doccano](https://github.com/doccano/doccano)、[MarkTool](https://github.com/FXLP/MarkTool)、[LabelStudio](https://labelstud.io/ ): Data Annotation Toolkits
 
 [LambdaKG](https://github.com/zjunlp/PromptKG/tree/main/lambdaKG): A library and benchmark for PLM-based KG embeddings
 
+[EasyInstruct](https://github.com/zjunlp/EasyInstruct): An easy-to-use framework to instruct Large Language Models
+
+
 # Table of Contents
 
 * [What's New](#whats-new)
 * [Prediction Demo](#prediction-demo)
 * [Model Framework](#model-framework)
 * [Quick Start](#quick-start)
    * [Requirements](#requirements)
@@ -69,16 +71,18 @@
 * [Citation](#citation)
 * [Contributors](#contributors)
 * [Other Knowledge Extraction Open-Source Projects](#other-knowledge-extraction-open-source-projects)
 
 <br>
 
 # What's New
+## Apr, 2023
+* We have added new models, including [CP-NER](https://github.com/zjunlp/DeepKE/blob/main/example/ner/cross), [ASP(EMNLP'22)](https://github.com/zjunlp/DeepKE/tree/main/example/triple/ASP), [PRGC(ACL'21)](https://github.com/zjunlp/DeepKE/tree/main/example/triple/PRGC), [PURE(NAACL'21)](https://github.com/zjunlp/DeepKE/tree/main/example/triple/PURE), provided [event extraction](https://github.com/zjunlp/DeepKE/tree/main/example/ee/standard) capabilities (Chinese and English), and offered compatibility with higher versions of Python packages (e.g., Transformers).
 ## Feb, 2023
-* We have supported using [LLM](https://github.com/zjunlp/DeepKE/tree/main/example/llm) (GPT-3) with in-context learning (based on [Promptify](https://github.com/promptslab/Promptify)) & data generation, added a NER model [W2NER](https://github.com/zjunlp/DeepKE/tree/main/example/ner/standard/w2ner).
+* We have supported using [LLM](https://github.com/zjunlp/DeepKE/tree/main/example/llm) (GPT-3) with in-context learning (based on [EasyInstruct](https://github.com/zjunlp/EasyInstruct)) & data generation, added a NER model [W2NER(AAAI'22)](https://github.com/zjunlp/DeepKE/tree/main/example/ner/standard/w2ner).
 ## Nov, 2022
 * Add data [annotation instructions](https://github.com/zjunlp/DeepKE/blob/main/README_TAG.md) for entity recognition and relation extraction, automatic labelling of weakly supervised data ([entity extraction](https://github.com/zjunlp/DeepKE/tree/main/example/ner/prepare-data) and [relation extraction](https://github.com/zjunlp/DeepKE/tree/main/example/re/prepare-data)), and optimize [multi-GPU training](https://github.com/zjunlp/DeepKE/tree/main/example/re/standard).
 ## Sept, 2022
 * The paper [DeepKE: A Deep Learning Based Knowledge Extraction Toolkit for Knowledge Base Population](https://arxiv.org/abs/2201.03335) has been accepted by the EMNLP 2022 System Demonstration Track.
 ## Aug, 2022
 * We have added [data augmentation](https://github.com/zjunlp/DeepKE/tree/main/example/re/few-shot/DA) (Chinese, English) support for [low-resource relation extraction](https://github.com/zjunlp/DeepKE/tree/main/example/re/few-shot).
 ## June, 2022
@@ -455,14 +459,97 @@
     
     ```bash
     python predict.py
     ```
 
 <br>
 
+### 4. Event Extraction
+
+* Event extraction is the task to extract event type, event trigger words, event arguments from a unstructed text.
+* The data is stored in `.tsv` files, some instances are as follows:
+
+<table h style="text-align:center">
+    <tr>
+        <th colspan="2"> Sentence </th>
+        <th> Event type </th>
+        <th> Trigger </th>
+        <th> Role </th>
+        <th> Argument </th>
+    </tr>
+    <tr> 
+        <td rowspan="3" colspan="2"> 据《欧洲时报》报道，当地时间27日，法国巴黎卢浮宫博物馆员工因不满工作条件恶化而罢工，导致该博物馆也因此闭门谢客一天。 </td>
+      	<td rowspan="3"> 组织行为-罢工 </td>
+    		<td rowspan="3"> 罢工 </td>
+    		<td> 罢工人员 </td>
+    		<td> 法国巴黎卢浮宫博物馆员工 </td>
+    </tr>
+    <tr> 
+        <td> 时间 </td>
+        <td> 当地时间27日 </td>
+    </tr>
+    <tr> 
+        <td> 所属组织 </td>
+        <td> 法国巴黎卢浮宫博物馆 </td>
+    </tr>
+    <tr> 
+        <td rowspan="3" colspan="2"> 中国外运2019年上半年归母净利润增长17%：收购了少数股东股权 </td>
+      	<td rowspan="3"> 财经/交易-出售/收购 </td>
+    		<td rowspan="3"> 收购 </td>
+    		<td> 出售方 </td>
+    		<td> 少数股东 </td>
+    </tr>
+    <tr> 
+        <td> 收购方 </td>
+        <td> 中国外运 </td>
+    </tr>
+    <tr> 
+        <td> 交易物 </td>
+        <td> 股权 </td>
+    </tr>
+    <tr> 
+        <td rowspan="3" colspan="2"> 美国亚特兰大航展13日发生一起表演机坠机事故，飞行员弹射出舱并安全着陆，事故没有造成人员伤亡。 </td>
+      	<td rowspan="3"> 灾害/意外-坠机 </td>
+    		<td rowspan="3"> 坠机 </td>
+    		<td> 时间 </td>
+    		<td> 13日 </td>
+    </tr>
+    <tr> 
+        <td> 地点 </td>
+        <td> 美国亚特兰 </td>
+  	</tr>
+</table>
+
+* Read the detailed process in specific README
+
+  * [STANDARD(Fully Supervised)](./example/ee/standard/README.md)
+
+    **Step1** Enter the `DeepKE/example/ee/standard` folder. Download the dataset.
+
+    ```bash
+    wget 120.27.214.45/Data/ee/DuEE.zip
+    unzip DuEE.zip
+    ```
+
+    **Step 2** Training
+
+    The dataset and parameters can be customized in the `data` folder and `conf` folder respectively.
+
+    ```bash
+    python run.py
+    ```
+
+    **Step 3** Prediction
+
+    ```bash
+    python predict.py
+    ```
+
+<br>
+
 # Notebook Tutorial
 
 This toolkit provides many `Jupyter Notebook` and `Google Colab` tutorials. Users can study *DeepKE* with them.
 
 - Standard Setting<br>
 
   [NER Notebook](https://github.com/zjunlp/DeepKE/blob/main/tutorial-notebooks/ner/standard/standard_ner_tutorial.ipynb)
@@ -524,59 +611,66 @@
 7.Make sure the exact versions of requirements in `requirements.txt`.
 
 
 
 <br>
 
 # To do
-In next version, we plan to add **event extraction** to the toolkit. 
+In next version, we plan to release a LLM for KE. 
 
 Meanwhile, we will offer long-term maintenance to **fix bugs**, **solve issues** and meet **new requests**. So if you have any problems, please put issues to us.
 
 <br>
 
 # Citation
 
 Please cite our paper if you use DeepKE in your work
 
 ```bibtex
-@inproceedings{zhang-etal-2022-deepke,
-    title = "{D}eep{KE}: A Deep Learning Based Knowledge Extraction Toolkit for Knowledge Base Population",
-    author = "Zhang, Ningyu  and
-      Xu, Xin  and
-      Tao, Liankuan  and
-      Yu, Haiyang  and
-      Ye, Hongbin  and
-      Qiao, Shuofei  and
-      Xie, Xin  and
-      Chen, Xiang  and
-      Li, Zhoubo  and
-      Li, Lei",
-    booktitle = "Proceedings of the The 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
-    month = dec,
-    year = "2022",
-    address = "Abu Dhabi, UAE",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2022.emnlp-demos.10",
-    pages = "98--108",
-    abstract = "We present an open-source and extensible knowledge extraction toolkit DeepKE, supporting complicated low-resource, document-level and multimodal scenarios in the knowledge base population. DeepKE implements various information extraction tasks, including named entity recognition, relation extraction and attribute extraction. With a unified framework, DeepKE allows developers and researchers to customize datasets and models to extract information from unstructured data according to their requirements. Specifically, DeepKE not only provides various functional modules and model implementation for different tasks and scenarios but also organizes all components by consistent frameworks to maintain sufficient modularity and extensibility. We release the source code at GitHub in https://github.com/zjunlp/DeepKE with Google Colab tutorials and comprehensive documents for beginners. Besides, we present an online system in http://deepke.openkg.cn/EN/re{\_}doc{\_}show.html for real-time extraction of various tasks, and a demo video.",
+@inproceedings{DBLP:conf/emnlp/ZhangXTYYQXCLL22,
+  author    = {Ningyu Zhang and
+               Xin Xu and
+               Liankuan Tao and
+               Haiyang Yu and
+               Hongbin Ye and
+               Shuofei Qiao and
+               Xin Xie and
+               Xiang Chen and
+               Zhoubo Li and
+               Lei Li},
+  editor    = {Wanxiang Che and
+               Ekaterina Shutova},
+  title     = {DeepKE: {A} Deep Learning Based Knowledge Extraction Toolkit for Knowledge
+               Base Population},
+  booktitle = {Proceedings of the The 2022 Conference on Empirical Methods in Natural
+               Language Processing, {EMNLP} 2022 - System Demonstrations, Abu Dhabi,
+               UAE, December 7-11, 2022},
+  pages     = {98--108},
+  publisher = {Association for Computational Linguistics},
+  year      = {2022},
+  url       = {https://aclanthology.org/2022.emnlp-demos.10},
+  timestamp = {Thu, 23 Mar 2023 16:56:00 +0100},
+  biburl    = {https://dblp.org/rec/conf/emnlp/ZhangXTYYQXCLL22.bib},
+  bibsource = {dblp computer science bibliography, https://dblp.org}
 }
 ```
 <br>
 
 # Contributors
 
 Zhejiang University: [Ningyu Zhang](https://person.zju.edu.cn/en/ningyu), Liankuan Tao, Xin Xu, Xinrong Li, Haiyang Yu, Hongbin Ye, Shuofei Qiao, Peng Wang, Yuqi Zhu, Xin Xie, Xiang Chen, Zhoubo Li, Lei Li, Xiaozhuan Liang, Yunzhi Yao, Shumin Deng, Wen Zhang, Guozhou Zheng, Huajun Chen
 
 Community Contributors: [thredreams](https://github.com/thredreams), [eltociear](https://github.com/eltociear)
 
 Alibaba Group: Feiyu Xiong, Qiang Chen
 
 DAMO Academy: Zhenru Zhang, Chuanqi Tan, Fei Huang
 
+Intern: Ziwen Xu, Rui Huang, Xiaolong Weng
+
 # Other Knowledge Extraction Open-Source Projects
 
 - [CogIE](https://github.com/jinzhuoran/CogIE)
 - [OpenNRE](https://github.com/thunlp/OpenNRE)
 - [OmniEvent](https://github.com/THU-KEG/OmniEvent)
 - [OpenUE](https://github.com/zjunlp/OpenUE)
 - [OpenIE](https://stanfordnlp.github.io/CoreNLP/openie.html)
```

#### html2text {}

```diff
@@ -9,75 +9,81 @@
 *relation* and *attribute* extraction. We provide [documents](https://
 zjunlp.github.io/DeepKE/), [Google Colab tutorials](https://
 colab.research.google.com/drive/1vS8YJhJltzw3hpJczPt24O0Azcs3ZpRi?usp=sharing),
 [online demo](http://deepke.zjukg.cn/), [paper](https://arxiv.org/pdf/
 2201.03335.pdf), [slides](https://drive.google.com/file/d/
 1IIeIZAbVduemqXc4zD40FUMoPHCJinLy/view?usp=sharing) and [poster](https://
 drive.google.com/file/d/1vd7xVHlWzoAxivN4T5qKrcqIGDcSM1_7/view?usp=sharing) for
-beginners. - âNew: We have released the [DeepKE-GPT](http://deepke.openkg.cn/
-EN/llm.html) (Based on ChatGPT). **Reading Materials**: Data-Efficient
-Knowledge Graph Construction, é«æç¥è¯å¾è°±æå»º ([Tutorial on CCKS 2022]
-(http://sigkg.cn/ccks2022/?page_id=24)) \[[slides](https://drive.google.com/
-drive/folders/1xqeREw3dSiw-Y1rxLDx77r0hGUvHnuuE)\] Efficient and Robust
-Knowledge Graph Construction ([Tutorial on AACL-IJCNLP 2022](https://
-www.aacl2022.org/Program/tutorials)) \[[slides](https://github.com/NLP-
-Tutorials/AACL-IJCNLP2022-KGC-Tutorial)\] PromptKG Family: a Gallery of Prompt
-Learning & KG-related Research Works, Toolkits, and Paper-list [[Resources]
-(https://github.com/zjunlp/PromptKG)\] Knowledge Extraction in Low-Resource
-Scenarios: Survey and Perspective \[[Survey](https://arxiv.org/abs/
-2202.08063)\]\[[Paper-list](https://github.com/zjunlp/Low-resource-KEPapers)\]
-Reasoning with Language Model Prompting \[[Survey](https://arxiv.org/abs/
-2212.09597)\]\[[Paper-list](https://github.com/zjunlp/
-Prompt4ReasoningPapers)\]\[[ppt](https://github.com/zjunlp/
+beginners. **Reading Materials**: Data-Efficient Knowledge Graph Construction,
+é«æç¥è¯å¾è°±æå»º ([Tutorial on CCKS 2022](http://sigkg.cn/ccks2022/
+?page_id=24)) \[[slides](https://drive.google.com/drive/folders/1xqeREw3dSiw-
+Y1rxLDx77r0hGUvHnuuE)\] Efficient and Robust Knowledge Graph Construction (
+[Tutorial on AACL-IJCNLP 2022](https://www.aacl2022.org/Program/tutorials)) \[
+[slides](https://github.com/NLP-Tutorials/AACL-IJCNLP2022-KGC-Tutorial)\]
+PromptKG Family: a Gallery of Prompt Learning & KG-related Research Works,
+Toolkits, and Paper-list [[Resources](https://github.com/zjunlp/PromptKG)\]
+Knowledge Extraction in Low-Resource Scenarios: Survey and Perspective \[
+[Survey](https://arxiv.org/abs/2202.08063)\]\[[Paper-list](https://github.com/
+zjunlp/Low-resource-KEPapers)\] Reasoning with Language Model Prompting \[
+[Survey](https://arxiv.org/abs/2212.09597)\]\[[Paper-list](https://github.com/
+zjunlp/Prompt4ReasoningPapers)\]\[[ppt](https://github.com/zjunlp/
 Prompt4ReasoningPapers/blob/main/tutorial.pdf)\] **Related Toolkit**: [Doccano]
 (https://github.com/doccano/doccano)ã[MarkTool](https://github.com/FXLP/
 MarkTool)ã[LabelStudio](https://labelstud.io/ ): Data Annotation Toolkits
 [LambdaKG](https://github.com/zjunlp/PromptKG/tree/main/lambdaKG): A library
-and benchmark for PLM-based KG embeddings # Table of Contents * [What's New]
-(#whats-new) * [Prediction Demo](#prediction-demo) * [Model Framework](#model-
-framework) * [Quick Start](#quick-start) * [Requirements](#requirements) *
-[Introduction of Three Functions](#introduction-of-three-functions) * [1. Named
-Entity Recognition](#1-named-entity-recognition) * [2. Relation Extraction](#2-
-relation-extraction) * [3. Attribute Extraction](#3-attribute-extraction) *
-[Notebook Tutorial](#notebook-tutorial) * [Tips](#tips) * [To do](#to-do) *
-[Citation](#citation) * [Contributors](#contributors) * [Other Knowledge
-Extraction Open-Source Projects](#other-knowledge-extraction-open-source-
-projects)
-# What's New ## Feb, 2023 * We have supported using [LLM](https://github.com/
-zjunlp/DeepKE/tree/main/example/llm) (GPT-3) with in-context learning (based on
-[Promptify](https://github.com/promptslab/Promptify)) & data generation, added
-a NER model [W2NER](https://github.com/zjunlp/DeepKE/tree/main/example/ner/
-standard/w2ner). ## Nov, 2022 * Add data [annotation instructions](https://
-github.com/zjunlp/DeepKE/blob/main/README_TAG.md) for entity recognition and
-relation extraction, automatic labelling of weakly supervised data ([entity
-extraction](https://github.com/zjunlp/DeepKE/tree/main/example/ner/prepare-
-data) and [relation extraction](https://github.com/zjunlp/DeepKE/tree/main/
-example/re/prepare-data)), and optimize [multi-GPU training](https://
-github.com/zjunlp/DeepKE/tree/main/example/re/standard). ## Sept, 2022 * The
-paper [DeepKE: A Deep Learning Based Knowledge Extraction Toolkit for Knowledge
-Base Population](https://arxiv.org/abs/2201.03335) has been accepted by the
-EMNLP 2022 System Demonstration Track. ## Aug, 2022 * We have added [data
-augmentation](https://github.com/zjunlp/DeepKE/tree/main/example/re/few-shot/
-DA) (Chinese, English) support for [low-resource relation extraction](https://
-github.com/zjunlp/DeepKE/tree/main/example/re/few-shot). ## June, 2022 * We
-have added multimodal support for [entity](https://github.com/zjunlp/DeepKE/
-tree/main/example/ner/multimodal) and [relation extraction](https://github.com/
-zjunlp/DeepKE/tree/main/example/re/multimodal). ## May, 2022 * We have released
-[DeepKE-cnschema](https://github.com/zjunlp/DeepKE/blob/main/
-README_CNSCHEMA.md) with off-the-shelf knowledge extraction models. ## Jan,
-2022 * We have released a paper [DeepKE: A Deep Learning Based Knowledge
-Extraction Toolkit for Knowledge Base Population](https://arxiv.org/abs/
-2201.03335) ## Dec, 2021 * We have added `dockerfile` to create the enviroment
-automatically. ## Nov, 2021 * The demo of DeepKE, supporting real-time
-extration without deploying and training, has been released. * The
-documentation of DeepKE, containing the details of DeepKE such as source codes
-and datasets, has been released. ## Oct, 2021 * `pip install deepke` * The
-codes of deepke-v2.0 have been released. ## Aug, 2019 * The codes of deepke-
-v1.0 have been released. ## Aug, 2018 * The project DeepKE startup and codes of
-deepke-v0.1 have been released.
+and benchmark for PLM-based KG embeddings [EasyInstruct](https://github.com/
+zjunlp/EasyInstruct): An easy-to-use framework to instruct Large Language
+Models # Table of Contents * [What's New](#whats-new) * [Prediction Demo]
+(#prediction-demo) * [Model Framework](#model-framework) * [Quick Start]
+(#quick-start) * [Requirements](#requirements) * [Introduction of Three
+Functions](#introduction-of-three-functions) * [1. Named Entity Recognition]
+(#1-named-entity-recognition) * [2. Relation Extraction](#2-relation-
+extraction) * [3. Attribute Extraction](#3-attribute-extraction) * [Notebook
+Tutorial](#notebook-tutorial) * [Tips](#tips) * [To do](#to-do) * [Citation]
+(#citation) * [Contributors](#contributors) * [Other Knowledge Extraction Open-
+Source Projects](#other-knowledge-extraction-open-source-projects)
+# What's New ## Apr, 2023 * We have added new models, including [CP-NER](https:
+//github.com/zjunlp/DeepKE/blob/main/example/ner/cross), [ASP(EMNLP'22)](https:
+//github.com/zjunlp/DeepKE/tree/main/example/triple/ASP), [PRGC(ACL'21)](https:
+//github.com/zjunlp/DeepKE/tree/main/example/triple/PRGC), [PURE(NAACL'21)]
+(https://github.com/zjunlp/DeepKE/tree/main/example/triple/PURE), provided
+[event extraction](https://github.com/zjunlp/DeepKE/tree/main/example/ee/
+standard) capabilities (Chinese and English), and offered compatibility with
+higher versions of Python packages (e.g., Transformers). ## Feb, 2023 * We have
+supported using [LLM](https://github.com/zjunlp/DeepKE/tree/main/example/llm)
+(GPT-3) with in-context learning (based on [EasyInstruct](https://github.com/
+zjunlp/EasyInstruct)) & data generation, added a NER model [W2NER(AAAI'22)]
+(https://github.com/zjunlp/DeepKE/tree/main/example/ner/standard/w2ner). ##
+Nov, 2022 * Add data [annotation instructions](https://github.com/zjunlp/
+DeepKE/blob/main/README_TAG.md) for entity recognition and relation extraction,
+automatic labelling of weakly supervised data ([entity extraction](https://
+github.com/zjunlp/DeepKE/tree/main/example/ner/prepare-data) and [relation
+extraction](https://github.com/zjunlp/DeepKE/tree/main/example/re/prepare-
+data)), and optimize [multi-GPU training](https://github.com/zjunlp/DeepKE/
+tree/main/example/re/standard). ## Sept, 2022 * The paper [DeepKE: A Deep
+Learning Based Knowledge Extraction Toolkit for Knowledge Base Population]
+(https://arxiv.org/abs/2201.03335) has been accepted by the EMNLP 2022 System
+Demonstration Track. ## Aug, 2022 * We have added [data augmentation](https://
+github.com/zjunlp/DeepKE/tree/main/example/re/few-shot/DA) (Chinese, English)
+support for [low-resource relation extraction](https://github.com/zjunlp/
+DeepKE/tree/main/example/re/few-shot). ## June, 2022 * We have added multimodal
+support for [entity](https://github.com/zjunlp/DeepKE/tree/main/example/ner/
+multimodal) and [relation extraction](https://github.com/zjunlp/DeepKE/tree/
+main/example/re/multimodal). ## May, 2022 * We have released [DeepKE-cnschema]
+(https://github.com/zjunlp/DeepKE/blob/main/README_CNSCHEMA.md) with off-the-
+shelf knowledge extraction models. ## Jan, 2022 * We have released a paper
+[DeepKE: A Deep Learning Based Knowledge Extraction Toolkit for Knowledge Base
+Population](https://arxiv.org/abs/2201.03335) ## Dec, 2021 * We have added
+`dockerfile` to create the enviroment automatically. ## Nov, 2021 * The demo of
+DeepKE, supporting real-time extration without deploying and training, has been
+released. * The documentation of DeepKE, containing the details of DeepKE such
+as source codes and datasets, has been released. ## Oct, 2021 * `pip install
+deepke` * The codes of deepke-v2.0 have been released. ## Aug, 2019 * The codes
+of deepke-v1.0 have been released. ## Aug, 2018 * The project DeepKE startup
+and codes of deepke-v0.1 have been released.
 # Prediction Demo There is a demonstration of prediction. The GIF file is
 created by [Terminalizer](https://github.com/faressoft/terminalizer). Get the
 [code](https://drive.google.com/file/d/1r4tWfAkpvynH3CBSgd-XG79rf-pB-KR3/
 view?usp=share_link). [pics/demo.gif]
 # Model Framework
                       **** [pics/architectures.png] ****
 - DeepKE contains a unified framework for **named entity recognition**,
@@ -240,14 +246,32 @@
 specific README - **[STANDARD (Fully Supervised)](https://github.com/zjunlp/
 DeepKE/tree/main/example/ae/standard)** **Step1** Enter the `DeepKE/example/ae/
 standard` folder. Download the dataset. ```bash wget 120.27.214.45/Data/ae/
 standard/data.tar.gz tar -xzvf data.tar.gz ``` **Step2** Training
 The dataset and parameters can be customized in the `data` folder and `conf`
 folder respectively. ```bash python run.py ``` **Step3** Prediction ```bash
 python predict.py ```
+### 4. Event Extraction * Event extraction is the task to extract event type,
+event trigger words, event arguments from a unstructed text. * The data is
+stored in `.tsv` files, some instances are as follows:
+Sentence                                                                                                                                                                      Event type                  Trigger Role         Argument
+                                                                                                                                                                                                                  ç½¢å·¥�æ³å½å·´é»å¢æµ®å®«åç©é¦åå·¥
+æ®ãæ¬§æ´²æ¶æ¥ãæ¥éï¼å½å°æ¶é´27æ¥ï¼æ³å½å·´é»å¢æµ®å®«åç©é¦åå·¥åç»ç»è¡ä¸º-ç�ç½¢åæ¶é´�å½å°æ¶é´27æ¥�´è¯¥åç©é¦ä¹å æ­¤é­é¨è°¢å®¢ä¸å¤©ã
+                                                                                                                                                                                                                  æå±�æ³å½å·´é»å¢æµ®å®«åç©é¦
+                                                                                                                                                                                                                  åºå®�å°æ°è¡ä¸
+ä¸­å½å¤è¿2019å¹´ä¸åå¹´å½æ¯åå©æ¶¦å¢é¿17%ï¼æ¶è´­äºå°æ°è¡ä¸è¡æ                 è´¢ç»/äº¤æ-åæ¶èæ¶è´­�ä¸­å½å¤è¿
+                                                                                                                                                                                                                  äº¤æ�è¡æ
+ç¾å½äºç¹å°å¤§èªå±13æ¥åçä¸èµ·è¡¨æ¼æºå æºäºæï¼é£è¡åå¼¹å°åºè±å¹ç¾å®³/æå¤-åå ææ¶é´�13æ¥� æäººåä¼¤äº¡ã
+                                                                                                                                                                                                                  å°ç¹ ç¾å½äºç¹å°
+* Read the detailed process in specific README * [STANDARD(Fully Supervised)]
+(./example/ee/standard/README.md) **Step1** Enter the `DeepKE/example/ee/
+standard` folder. Download the dataset. ```bash wget 120.27.214.45/Data/ee/
+DuEE.zip unzip DuEE.zip ``` **Step 2** Training The dataset and parameters can
+be customized in the `data` folder and `conf` folder respectively. ```bash
+python run.py ``` **Step 3** Prediction ```bash python predict.py ```
 # Notebook Tutorial This toolkit provides many `Jupyter Notebook` and `Google
 Colab` tutorials. Users can study *DeepKE* with them. - Standard Setting
 [NER Notebook](https://github.com/zjunlp/DeepKE/blob/main/tutorial-notebooks/
 ner/standard/standard_ner_tutorial.ipynb) [NER Colab](https://
 colab.research.google.com/drive/1h4k6-_oNEHBRxrnzpxHPczO5SFaLS9uq?usp=sharing)
 [RE Notebook](https://github.com/zjunlp/DeepKE/blob/main/tutorial-notebooks/re/
 standard/standard_re_pcnn_tutorial.ipynb) [RE Colab](https://
@@ -289,49 +313,37 @@
 install *DeepKE* with source codes. Because user may meet some problems in
 Windows system with 'pip',and the source code modification will not work,see
 [issue](https://github.com/zjunlp/DeepKE/issues/117) 6.More related low-
 resource knowledge extraction works can be found in [Knowledge Extraction in
 Low-Resource Scenarios: Survey and Perspective](https://arxiv.org/pdf/
 2202.08063.pdf). 7.Make sure the exact versions of requirements in
 `requirements.txt`.
-# To do In next version, we plan to add **event extraction** to the toolkit.
-Meanwhile, we will offer long-term maintenance to **fix bugs**, **solve
-issues** and meet **new requests**. So if you have any problems, please put
-issues to us.
+# To do In next version, we plan to release a LLM for KE. Meanwhile, we will
+offer long-term maintenance to **fix bugs**, **solve issues** and meet **new
+requests**. So if you have any problems, please put issues to us.
 # Citation Please cite our paper if you use DeepKE in your work ```bibtex
-@inproceedings{zhang-etal-2022-deepke, title = "{D}eep{KE}: A Deep Learning
-Based Knowledge Extraction Toolkit for Knowledge Base Population", author =
-"Zhang, Ningyu and Xu, Xin and Tao, Liankuan and Yu, Haiyang and Ye, Hongbin
-and Qiao, Shuofei and Xie, Xin and Chen, Xiang and Li, Zhoubo and Li, Lei",
-booktitle = "Proceedings of the The 2022 Conference on Empirical Methods in
-Natural Language Processing: System Demonstrations", month = dec, year =
-"2022", address = "Abu Dhabi, UAE", publisher = "Association for Computational
-Linguistics", url = "https://aclanthology.org/2022.emnlp-demos.10", pages =
-"98--108", abstract = "We present an open-source and extensible knowledge
-extraction toolkit DeepKE, supporting complicated low-resource, document-level
-and multimodal scenarios in the knowledge base population. DeepKE implements
-various information extraction tasks, including named entity recognition,
-relation extraction and attribute extraction. With a unified framework, DeepKE
-allows developers and researchers to customize datasets and models to extract
-information from unstructured data according to their requirements.
-Specifically, DeepKE not only provides various functional modules and model
-implementation for different tasks and scenarios but also organizes all
-components by consistent frameworks to maintain sufficient modularity and
-extensibility. We release the source code at GitHub in https://github.com/
-zjunlp/DeepKE with Google Colab tutorials and comprehensive documents for
-beginners. Besides, we present an online system in http://deepke.openkg.cn/EN/
-re{\_}doc{\_}show.html for real-time extraction of various tasks, and a demo
-video.", } ```
+@inproceedings{DBLP:conf/emnlp/ZhangXTYYQXCLL22, author = {Ningyu Zhang and Xin
+Xu and Liankuan Tao and Haiyang Yu and Hongbin Ye and Shuofei Qiao and Xin Xie
+and Xiang Chen and Zhoubo Li and Lei Li}, editor = {Wanxiang Che and Ekaterina
+Shutova}, title = {DeepKE: {A} Deep Learning Based Knowledge Extraction Toolkit
+for Knowledge Base Population}, booktitle = {Proceedings of the The 2022
+Conference on Empirical Methods in Natural Language Processing, {EMNLP} 2022 -
+System Demonstrations, Abu Dhabi, UAE, December 7-11, 2022}, pages = {98--108},
+publisher = {Association for Computational Linguistics}, year = {2022}, url =
+{https://aclanthology.org/2022.emnlp-demos.10}, timestamp = {Thu, 23 Mar 2023
+16:56:00 +0100}, biburl = {https://dblp.org/rec/conf/emnlp/
+ZhangXTYYQXCLL22.bib}, bibsource = {dblp computer science bibliography, https:/
+/dblp.org} } ```
 # Contributors Zhejiang University: [Ningyu Zhang](https://person.zju.edu.cn/
 en/ningyu), Liankuan Tao, Xin Xu, Xinrong Li, Haiyang Yu, Hongbin Ye, Shuofei
 Qiao, Peng Wang, Yuqi Zhu, Xin Xie, Xiang Chen, Zhoubo Li, Lei Li, Xiaozhuan
 Liang, Yunzhi Yao, Shumin Deng, Wen Zhang, Guozhou Zheng, Huajun Chen Community
 Contributors: [thredreams](https://github.com/thredreams), [eltociear](https://
 github.com/eltociear) Alibaba Group: Feiyu Xiong, Qiang Chen DAMO Academy:
-Zhenru Zhang, Chuanqi Tan, Fei Huang # Other Knowledge Extraction Open-Source
-Projects - [CogIE](https://github.com/jinzhuoran/CogIE) - [OpenNRE](https://
-github.com/thunlp/OpenNRE) - [OmniEvent](https://github.com/THU-KEG/OmniEvent)
-- [OpenUE](https://github.com/zjunlp/OpenUE) - [OpenIE](https://
-stanfordnlp.github.io/CoreNLP/openie.html) - [RESIN](https://github.com/RESIN-
-KAIROS/RESIN-pipeline-public) - [ZShot](https://github.com/IBM/zshot) - [ZS4IE]
-(https://github.com/BBN-E/ZS4IE) - [OmniEvent](https://github.com/THU-KEG/
-OmniEvent)
+Zhenru Zhang, Chuanqi Tan, Fei Huang Intern: Ziwen Xu, Rui Huang, Xiaolong Weng
+# Other Knowledge Extraction Open-Source Projects - [CogIE](https://github.com/
+jinzhuoran/CogIE) - [OpenNRE](https://github.com/thunlp/OpenNRE) - [OmniEvent]
+(https://github.com/THU-KEG/OmniEvent) - [OpenUE](https://github.com/zjunlp/
+OpenUE) - [OpenIE](https://stanfordnlp.github.io/CoreNLP/openie.html) - [RESIN]
+(https://github.com/RESIN-KAIROS/RESIN-pipeline-public) - [ZShot](https://
+github.com/IBM/zshot) - [ZS4IE](https://github.com/BBN-E/ZS4IE) - [OmniEvent]
+(https://github.com/THU-KEG/OmniEvent)
```

### Comparing `deepke-2.1.3/setup.py` & `deepke-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
     
 setup(
     name='deepke',  # 打包后的包文件名
-    version='2.1.3',    #版本号
+    version='2.2',    #版本号
     keywords=["pip", "RE","NER","AE"],    # 关键字
     description='DeepKE is a knowledge extraction toolkit for knowledge graph construction supporting low-resource, document-level and multimodal scenarios for entity, relation and attribute extraction.',  # 说明
     license="MIT",  # 许可
     url='https://github.com/zjunlp/deepke',
     author='ZJUNLP',
     author_email='zhangningyu@zju.edu.cn',
     include_package_data=True,
```

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/BasicModule.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/BasicModule.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/BiLSTM.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/BiLSTM.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/Capsule.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/Capsule.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/GCN.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/GCN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/LM.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/LM.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/PCNN.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/PCNN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/models/Transformer.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/models/Transformer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Attention.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/Attention.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/CNN.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/CNN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Capsule.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/Capsule.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Embedding.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/Embedding.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/GCN.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/GCN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/RNN.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/RNN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/module/Transformer.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/module/Transformer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/dataset.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/tools/dataset.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/metrics.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/preprocess.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/tools/preprocess.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/serializer.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/tools/serializer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/trainer.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/tools/vocab.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/tools/vocab.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/utils/ioUtils.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/utils/ioUtils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/attribution_extraction/standard/utils/nnUtils.py` & `deepke-2.2/src/deepke/attribution_extraction/standard/utils/nnUtils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/event_extraction/standard/degree/data.py` & `deepke-2.2/src/deepke/event_extraction/standard/degree/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,15 @@
         inputs = self.tokenizer(input_text, return_tensors='pt', padding=True, max_length=self.max_length)
         enc_idxs = inputs['input_ids']
         enc_attn = inputs['attention_mask']
 
         # decoder inputs
         targets = self.tokenizer(target_text, return_tensors='pt', padding=True, max_length=self.max_output_length)
         dec_idxs = targets['input_ids']
+        # print(self.tokenizer.decode(dec_idxs[0]))
         batch_size = dec_idxs.size(0)
         dec_idxs[:, 0] = self.tokenizer.eos_token_id
         dec_attn = targets['attention_mask']
             
         # labels
         padding = torch.ones((batch_size, 1), dtype=torch.long)
         padding[:] = self.tokenizer.pad_token_id
```

### Comparing `deepke-2.1.3/src/deepke/event_extraction/standard/degree/model.py` & `deepke-2.2/src/deepke/event_extraction/standard/degree/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     def forward(self, batch):
         outputs = self.model(input_ids=batch.enc_idxs, 
                              attention_mask=batch.enc_attn, 
                              decoder_input_ids=batch.dec_idxs, 
                              decoder_attention_mask=batch.dec_attn, 
                              labels=batch.lbl_idxs, 
                              return_dict=True)
-        
         loss = outputs['loss']
         
         return loss
         
     def predict(self, batch, num_beams=4, max_length=50):
         self.eval()
         with torch.no_grad():
@@ -35,12 +34,13 @@
                                           attention_mask=batch.enc_attn, 
                                           num_beams=num_beams, 
                                           max_length=max_length)
             
         final_output = []
         for bid in range(len(batch.enc_idxs)):
             output_sentence = self.tokenizer.decode(outputs[bid], skip_special_tokens=True, clean_up_tokenization_spaces=True)
+            # output_sentence = "Event" + output_sentence
             final_output.append(output_sentence)
         self.train()
 
         return final_output
```

### Comparing `deepke-2.1.3/src/deepke/event_extraction/standard/degree/template_generate_ace.py` & `deepke-2.2/src/deepke/event_extraction/standard/degree/template_generate_ace.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,16 @@
     'Giver': 'someone',
     'Recipient': 'some other',
     'Org': 'some organization',
     'Place': 'somewhere',
     'Adjudicator': 'some adjudicator'
 }
 
-
 class eve_template_generator():
-    def __init__(self, passage, triggers, roles, input_style, output_style, vocab, instance_base=False, knowledge=None):
+    def __init__(self, passage, triggers, roles, input_style, output_style, vocab, instance_base=False):
         """
         generate strctured information for events
         
         args:
             passage(List): a list of tokens
             triggers(List): a list of triggers
             roles(List): a list of Roles
@@ -45,32 +44,27 @@
         self.triggers = triggers
         self.roles = roles
         self.events = self.process_events(passage, triggers, roles)
         self.input_style = input_style
         self.output_style = output_style
         self.vocab = vocab
         self.event_templates = []
-        self.knowledge = knowledge if knowledge != None else {}
         if instance_base:
             for e_type in self.vocab['event_type_itos']:
                 theclass = getattr(sys.modules[__name__], e_type.replace(':', '_').replace('-', '_'), False)
                 if theclass:
-                    self.event_templates.append(
-                        theclass(self.input_style, self.output_style, passage, e_type, self.events, self.knowledge))
+                    self.event_templates.append(theclass(self.input_style, self.output_style, passage, e_type, self.events))
                 else:
                     print(e_type)
 
         else:
             for event in self.events:
-                theclass = getattr(sys.modules[__name__], event['event type'].replace(':', '_').replace('-', '_'),
-                                   False)
+                theclass = getattr(sys.modules[__name__], event['event type'].replace(':', '_').replace('-', '_'), False)
                 assert theclass
-                self.event_templates.append(
-                    theclass(self.input_style, self.output_style, event['tokens'], event['event type'], event,
-                             self.knowledge))
+                self.event_templates.append(theclass(self.input_style, self.output_style, event['tokens'], event['event type'], event))
         self.data = [x.generate_pair(x.trigger_text) for x in self.event_templates]
         self.data = [x for x in self.data if x]
 
     def get_training_data(self):
         return self.data
 
     def process_events(self, passage, triggers, roles):
@@ -89,21 +83,21 @@
                 }],
                 ROLE_TYPE(str):...,
                 ROLE_TYPE(str):....
             }
             'passage': PASSAGE
         }
         """
-
+        
         events = {trigger: [] for trigger in triggers}
 
         for argument in roles:
             trigger = argument[0]
             events[trigger].append(argument)
-
+        
         event_structures = []
         for trigger, arguments in events.items():
             eve_type = trigger[2]
             eve_text = ' '.join(passage[trigger[0]:trigger[1]])
             eve_span = (trigger[0], trigger[1])
             argus = {}
             for argument in arguments:
@@ -120,42 +114,37 @@
                 'event type': eve_type,
                 'arguments': argus,
                 'passage': ' '.join(passage),
                 'tokens': passage
             })
         return event_structures
 
-
 class event_template():
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
         self.input_style = input_style
         self.output_style = output_style
         self.output_template = self.get_output_template()
         self.passage = ' '.join(passage)
         self.tokens = passage
         self.event_type = event_type
-        self.knowledge = knowledge
-        # if knowledge != '' and knowledge is not None:
-        #     self.passage = ' '.join(passage) + ' \n ' + knowledge
         if gold_event is not None:
             self.gold_event = gold_event
             if isinstance(gold_event, list):
                 # instance base
-                self.trigger_text = " and ".join(
-                    [x['trigger text'] for x in gold_event if x['event type'] == event_type])
-                self.trigger_span = [x['trigger span'] for x in gold_event if x['event type'] == event_type]
-                self.arguments = [x['arguments'] for x in gold_event if x['event type'] == event_type]
+                self.trigger_text = " and ".join([x['trigger text'] for x in gold_event if x['event type']==event_type])
+                self.trigger_span = [x['trigger span'] for x in gold_event if x['event type']==event_type]
+                self.arguments = [x['arguments'] for x in gold_event if x['event type']==event_type]
             else:
                 # trigger base
                 self.trigger_text = gold_event['trigger text']
                 self.trigger_span = [gold_event['trigger span']]
-                self.arguments = [gold_event['arguments']]
+                self.arguments = [gold_event['arguments']]         
         else:
             self.gold_event = None
-
+        
     @classmethod
     def get_keywords(self):
         pass
 
     def generate_pair(self, query_trigger):
         """
         Generate model input sentence and output sentence pair
@@ -207,87 +196,86 @@
             # find corresponding trigger
             pred_span = None
             if isinstance(self.gold_event, list):
                 # end2end case
                 try:
                     # we need this ``try'' because we cannot gurantee the model will be bug-free on the matching
                     cor_tri = pred_trigger[pred[2]['cor tri cnt']]
-                    cor_tri_span = self.predstr2span(pred[0])[0]
+                    cor_tri_span = self.predstr2span(cor_tri[0])[0]
                     if cor_tri_span > -1:
                         pred_span = self.predstr2span(pred[0], cor_tri_span)
                     else:
                         continue
                 except Exception as e:
                     print(e)
             else:
                 # argument only case
                 pred_span = self.predstr2span(pred[0], self.trigger_span[0][0])
             if (pred_span is not None) and (pred_span[0] > -1):
                 pred_arg.append((pred_span[0], pred_span[1], pred[1]))
         pred_arg = list(set(pred_arg))
         pred_arg_num = len(pred_arg)
-
+        
         target = converted_gold
         match_id = 0
         match_type = 0
         for pred in pred_arg:
             id_flag = False
             id_type = False
             for gold in target:
-                if gold[0] == pred[0] and gold[1] == pred[1]:
+                if gold[0]==pred[0] and gold[1]==pred[1]:
                     id_flag = True
                     if gold[2] == pred[2]:
                         id_type = True
                         break
             match_id += int(id_flag)
             match_type += int(id_type)
         return {
-            'gold_tri_num': gold_tri_num,
+            'gold_tri_num': gold_tri_num, 
             'pred_tri_num': pred_tri_num,
             'match_tri_num': match_tri,
             'gold_arg_num': gold_arg_num,
             'pred_arg_num': pred_arg_num,
             'match_arg_id': match_id,
             'match_arg_cls': match_type
         }
-
+    
     def get_converted_gold(self):
         converted_gold = []
         for argu in self.arguments:
             for arg_type, arg_list in argu.items():
                 for arg in arg_list:
                     converted_gold.append((arg['argument span'][0], arg['argument span'][1], arg_type))
         return list(set(converted_gold))
-
+    
     def predstr2span(self, pred_str, trigger_idx=None):
         sub_words = [_.strip() for _ in pred_str.strip().lower().split()]
-        candidates = []
+        candidates=[]
         for i in range(len(self.tokens)):
             j = 0
-            while j < len(sub_words) and i + j < len(self.tokens):
-                if self.tokens[i + j].lower() == sub_words[j]:
+            while j < len(sub_words) and i+j < len(self.tokens):
+                if self.tokens[i+j].lower() == sub_words[j]:
                     j += 1
                 else:
                     break
             if j == len(sub_words):
-                candidates.append((i, i + len(sub_words)))
+                candidates.append((i, i+len(sub_words)))
         if len(candidates) < 1:
             return -1, -1
         else:
             if trigger_idx is not None:
-                return sorted(candidates, key=lambda x: abs(trigger_idx - x[0]))[0]
+                return sorted(candidates, key=lambda x: abs(trigger_idx-x[0]))[0]
             else:
                 return candidates[0]
 
-
 class Life_Be_Born(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['born', 'birth', 'bore']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
@@ -308,17 +296,15 @@
                     input_str += ' \n {}'.format('The event is related to life and someone is given birth to.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Be-Born' in self.knowledge.keys():
-            knowledge = self.knowledge['Be-Born']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -329,18 +315,16 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} was born in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
 
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
@@ -355,16 +339,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -377,27 +360,26 @@
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Life_Marry(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['marry', 'marriage', 'married']
-
+    
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
@@ -414,17 +396,14 @@
                     input_str += ' \n {}'.format('The event is related to life and someone is married.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Marry' in self.knowledge.keys():
-            knowledge = self.knowledge['Marry']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -435,18 +414,16 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} got married in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -460,18 +437,17 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
-                                pass
+                                    pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     person = prediction.split(' got married in ', 1)[0]
                                     person = person.split(' and ')
@@ -484,20 +460,19 @@
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Life_Divorce(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['divorce', 'divorced', 'Divorce']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
@@ -518,17 +493,15 @@
                     input_str += ' \n {}'.format('The event is related to life and someone was divorced.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Divorce' in self.knowledge.keys():
-            knowledge = self.knowledge['Divorce']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -539,23 +512,21 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} divorced in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -565,16 +536,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -585,38 +555,36 @@
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
-                                pass
+                                    pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Life_Injure(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['injure', 'wounded', 'hurt']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody or some organization led to some victim injured by some way in somewhere.')
+                    output_template += ' \n {}'.format('somebody or some organization led to some victim injured by some way in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -625,17 +593,15 @@
                     input_str += ' \n {}'.format('The event is related to life and someone is injured.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Injure' in self.knowledge.keys():
-            knowledge = self.knowledge['Injure']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -646,28 +612,23 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent'],
-                            " and ".join([a['argument text'] for a in argu['Victim']]) if "Victim" in argu.keys() else
-                            ROLE_PH_MAP['Victim'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Instrument']]) if "Instrument" in argu.keys() else
-                            ROLE_PH_MAP['Instrument'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent'],
+                            " and ".join([ a['argument text'] for a in argu['Victim']]) if "Victim" in argu.keys() else ROLE_PH_MAP['Victim'],
+                            " and ".join([ a['argument text'] for a in argu['Instrument']]) if "Instrument" in argu.keys() else ROLE_PH_MAP['Instrument'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} led to {} injured by {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -677,72 +638,65 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     agent = prediction.split(' led to ', 1)[0]
                                     agent = agent.split(' and ')
                                     victim = (prediction.split(' led to ', 1)[1]).split(' injured by ', 1)[0]
                                     victim = victim.split(' and ')
-                                    instrument = \
-                                    ((prediction.split(' led to ', 1)[1]).split(' injured by ', 1)[1]).split(' in ', )[
-                                        0]
+                                    instrument = ((prediction.split(' led to ', 1)[1]).split(' injured by ', 1)[1]).split(' in ', )[0]
                                     instrument = instrument.split(' and ')
-                                    place = \
-                                    ((prediction.split(' led to ', 1)[1]).split(' injured by ', 1)[1]).split(' in ', 1)[
-                                        1].rsplit('.', 1)[0]
+                                    place = ((prediction.split(' led to ', 1)[1]).split(' injured by ', 1)[1]).split(' in ', 1)[1].rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                                     for arg in victim:
                                         if arg != ROLE_PH_MAP['Victim']:
                                             output.append((arg, 'Victim', {'cor tri cnt': a_cnt}))
                                     for arg in instrument:
                                         if arg != ROLE_PH_MAP['Instrument']:
-                                            output.append((arg, 'Instrument', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Instrument', {'cor tri cnt': a_cnt}))                    
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except Exception as e:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Life_Die(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['kill', 'death', 'assassination']
-
+    
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody or some organization led to some victim died by some way in somewhere.')
+                    output_template += ' \n {}'.format('somebody or some organization led to some victim died by some way in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -751,17 +705,15 @@
                     input_str += ' \n {}'.format('The event is related to life and someone died.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Die' in self.knowledge.keys():
-            knowledge = self.knowledge['Die']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -772,28 +724,23 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent'],
-                            " and ".join([a['argument text'] for a in argu['Victim']]) if "Victim" in argu.keys() else
-                            ROLE_PH_MAP['Victim'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Instrument']]) if "Instrument" in argu.keys() else
-                            ROLE_PH_MAP['Instrument'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent'],
+                            " and ".join([ a['argument text'] for a in argu['Victim']]) if "Victim" in argu.keys() else ROLE_PH_MAP['Victim'],
+                            " and ".join([ a['argument text'] for a in argu['Instrument']]) if "Instrument" in argu.keys() else ROLE_PH_MAP['Instrument'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} led to {} died by {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -803,90 +750,81 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     agent = prediction.split(' led to ', 1)[0]
                                     agent = agent.split(' and ')
                                     victim = (prediction.split(' led to ', 1)[1]).split(' died by ', 1)[0]
                                     victim = victim.split(' and ')
-                                    instrument = \
-                                    ((prediction.split(' led to ', 1)[1]).split(' died by ', 1)[1]).split(' in ', )[0]
+                                    instrument = ((prediction.split(' led to ', 1)[1]).split(' died by ', 1)[1]).split(' in ', )[0]
                                     instrument = instrument.split(' and ')
-                                    place = \
-                                    ((prediction.split(' led to ', 1)[1]).split(' died by ', 1)[1]).split(' in ', 1)[
-                                        1].rsplit('.', 1)[0]
+                                    place = ((prediction.split(' led to ', 1)[1]).split(' died by ', 1)[1]).split(' in ', 1)[1].rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                                     for arg in victim:
                                         if arg != ROLE_PH_MAP['Victim']:
                                             output.append((arg, 'Victim', {'cor tri cnt': a_cnt}))
                                     for arg in instrument:
                                         if arg != ROLE_PH_MAP['Instrument']:
-                                            output.append((arg, 'Instrument', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Instrument', {'cor tri cnt': a_cnt}))         
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except Exception as e:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Movement_Transport(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['travel', 'go', 'move']
-
+    
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'something was sent to somewhere from some place by some vehicle. somebody or some organization was responsible for the transport.')
+                    output_template += ' \n {}'.format('something was sent to somewhere from some place by some vehicle. somebody or some organization was responsible for the transport.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('movement event, transport sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to movement. The event occurs when a weapon or vehicle is moved from one place to another.')
+                    input_str += ' \n {}'.format('The event is related to movement. The event occurs when a weapon or vehicle is moved from one place to another.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Transport' in self.knowledge.keys():
-            knowledge = self.knowledge['Transport']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -897,32 +835,24 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Artifact']]) if "Artifact" in argu.keys() else
-                            ROLE_PH_MAP['Artifact'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Destination']]) if "Destination" in argu.keys() else
-                            ROLE_PH_MAP['Destination'],
-                            " and ".join([a['argument text'] for a in argu['Origin']]) if "Origin" in argu.keys() else
-                            ROLE_PH_MAP['Origin'],
-                            " and ".join([a['argument text'] for a in argu['Vehicle']]) if "Vehicle" in argu.keys() else
-                            ROLE_PH_MAP['Vehicle'],
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent']
+                            " and ".join([ a['argument text'] for a in argu['Artifact']]) if "Artifact" in argu.keys() else ROLE_PH_MAP['Artifact'],
+                            " and ".join([ a['argument text'] for a in argu['Destination']]) if "Destination" in argu.keys() else ROLE_PH_MAP['Destination'],
+                            " and ".join([ a['argument text'] for a in argu['Origin']]) if "Origin" in argu.keys() else ROLE_PH_MAP['Origin'],
+                            " and ".join([ a['argument text'] for a in argu['Vehicle']]) if "Vehicle" in argu.keys() else ROLE_PH_MAP['Vehicle'],
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent']
                         )
-                        output_texts.append(
-                            "{} was sent to {} from {} by {}. {} was responsible for the transport.".format(*filler))
+                        output_texts.append("{} was sent to {} from {} by {}. {} was responsible for the transport.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -932,70 +862,62 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     artifact = prediction.split(' was sent to ', 1)[0]
                                     artifact = artifact.split(' and ')
                                     destination = (prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[0]
                                     destination = destination.split(' and ')
-                                    origin = \
-                                    ((prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[1]).split(' by ', 1)[
-                                        0]
+                                    origin = ((prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[1]).split(' by ', 1)[0]
                                     origin = origin.split(' and ')
-                                    vehicle = (
-                                    ((prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[1]).split(' by ', 1)[
-                                        1]).split('.', 1)[0]
+                                    vehicle = (((prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[1]).split(' by ', 1)[1]).split('.', 1)[0]
                                     vehicle = vehicle.split(' and ')
-                                    remain = (
-                                    ((prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[1]).split(' by ', 1)[
-                                        1]).split('.', 1)[1]
+                                    remain = (((prediction.split(' was sent to ', 1)[1]).split(' from ', 1)[1]).split(' by ', 1)[1]).split('.', 1)[1]
                                     if 'was responsible for the transport' in remain:
                                         agent = (remain.split(' was responsible for the transport.')[0]).strip()
                                         agent = agent.split(' and ')
                                     else:
                                         agent = []
 
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                                     for arg in artifact:
                                         if arg != ROLE_PH_MAP['Artifact']:
                                             output.append((arg, 'Artifact', {'cor tri cnt': a_cnt}))
                                     for arg in destination:
                                         if arg != ROLE_PH_MAP['Destination']:
-                                            output.append((arg, 'Destination', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Destination', {'cor tri cnt': a_cnt}))          
                                     for arg in origin:
                                         if arg != ROLE_PH_MAP['Origin']:
                                             output.append((arg, 'Origin', {'cor tri cnt': a_cnt}))
                                     for arg in vehicle:
                                         if arg != ROLE_PH_MAP['Vehicle']:
                                             output.append((arg, 'Vehicle', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Transaction_Transfer_Ownership(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['sell', 'buy', 'acquire']
 
     def get_output_template(self):
         output_template = ''
@@ -1010,25 +932,22 @@
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('transaction event, transfer ownership sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to transaction. The event occurs when an item or an organization is sold or gave to some other.')
+                    input_str += ' \n {}'.format('The event is related to transaction. The event occurs when an item or an organization is sold or gave to some other.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Transfer-Ownership' in self.knowledge.keys():
-            knowledge = self.knowledge['Transfer-Ownership']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1040,31 +959,27 @@
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         buyer_list = []
                         if "Beneficiary" in argu.keys():
-                            buyer_list.extend([a['argument text'] for a in argu['Beneficiary']])
+                            buyer_list.extend([ a['argument text'] for a in argu['Beneficiary']])
                         if "Buyer" in argu.keys():
-                            buyer_list.extend([a['argument text'] for a in argu['Buyer']])
+                            buyer_list.extend([ a['argument text'] for a in argu['Buyer']])
                         filler = (
-                            " and ".join(buyer_list) if len(buyer_list) > 0 else ROLE_PH_MAP['Buyer'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Artifact']]) if "Artifact" in argu.keys() else
-                            ROLE_PH_MAP['Artifact'],
-                            " and ".join([a['argument text'] for a in argu['Seller']]) if "Seller" in argu.keys() else
-                            ROLE_PH_MAP['Seller'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join(buyer_list) if len(buyer_list)>0 else ROLE_PH_MAP['Buyer'],
+                            " and ".join([ a['argument text'] for a in argu['Artifact']]) if "Artifact" in argu.keys() else ROLE_PH_MAP['Artifact'],
+                            " and ".join([ a['argument text'] for a in argu['Seller']]) if "Seller" in argu.keys() else ROLE_PH_MAP['Seller'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} got {} from {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1074,16 +989,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -1095,40 +1009,39 @@
                                     artifact = artifact.split(' and ')
                                     remain = remain.split(' from ', 1)[1]
 
                                     seller = remain.split(' in ', 1)[0]
                                     seller = seller.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
 
                                     for arg in buyer:
                                         if arg != ROLE_PH_MAP['Buyer']:
                                             output.append((arg, 'Buyer', {'cor tri cnt': a_cnt}))
                                     for arg in artifact:
                                         if arg != ROLE_PH_MAP['Artifact']:
                                             output.append((arg, 'Artifact', {'cor tri cnt': a_cnt}))
                                     for arg in seller:
                                         if arg != ROLE_PH_MAP['Seller']:
-                                            output.append((arg, 'Seller', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Seller', {'cor tri cnt': a_cnt}))          
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Transaction_Transfer_Money(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['pay', 'donation', 'loan']
 
     def get_output_template(self):
         output_template = ''
@@ -1143,25 +1056,22 @@
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('transaction event, transfer money sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to transaction. The event occurs when someone is giving, receiving, borrowing, or lending money.')
+                    input_str += ' \n {}'.format('The event is related to transaction. The event occurs when someone is giving, receiving, borrowing, or lending money.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Transfer-Money' in self.knowledge.keys():
-            knowledge = self.knowledge['Transfer-Money']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1173,28 +1083,26 @@
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         recipient_list = []
                         if "Recipient" in argu.keys():
-                            recipient_list.extend([a['argument text'] for a in argu['Recipient']])
+                            recipient_list.extend([ a['argument text'] for a in argu['Recipient']])
                         if "Beneficiary" in argu.keys():
-                            recipient_list.extend([a['argument text'] for a in argu['Beneficiary']])
+                            recipient_list.extend([ a['argument text'] for a in argu['Beneficiary']])
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Giver']]) if "Giver" in argu.keys() else
-                            ROLE_PH_MAP['Giver'],
-                            " and ".join(recipient_list) if len(recipient_list) > 0 else ROLE_PH_MAP['Recipient'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Giver']]) if "Giver" in argu.keys() else ROLE_PH_MAP['Giver'],
+                            " and ".join(recipient_list) if len(recipient_list)>0 else ROLE_PH_MAP['Recipient'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} paid {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1204,16 +1112,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -1221,51 +1128,49 @@
                                     giver = giver.split(' and ')
                                     remain = prediction.split(' paid ', 1)[1]
 
                                     recipient = remain.split(' in ', 1)[0]
                                     recipient = recipient.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
 
                                     for arg in giver:
                                         if arg != ROLE_PH_MAP['Giver']:
                                             output.append((arg, 'Giver', {'cor tri cnt': a_cnt}))
                                     for arg in recipient:
                                         if arg != ROLE_PH_MAP['Recipient']:
-                                            output.append((arg, 'Recipient', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Recipient', {'cor tri cnt': a_cnt}))          
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Business_Start_Org(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['founded', 'create', 'launch']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody or some organization launched some organization in somewhere.')
+                    output_template += ' \n {}'.format('somebody or some organization launched some organization in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -1274,17 +1179,15 @@
                     input_str += ' \n {}'.format('The event is related to a new organization being created.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Start-Org' in self.knowledge.keys():
-            knowledge = self.knowledge['Start-Org']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1295,20 +1198,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent'],
-                            " and ".join([a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else
-                            ROLE_PH_MAP['Org'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent'],
+                            " and ".join([ a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else ROLE_PH_MAP['Org'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} launched {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -1322,16 +1222,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -1339,36 +1238,35 @@
                                     agent = agent.split(' and ')
                                     remain = prediction.split(' launched ', 1)[1]
 
                                     org = remain.split(' in ', 1)[0]
                                     org = org.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                                     for arg in org:
                                         if arg != ROLE_PH_MAP['Org']:
-                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))                  
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Business_Merge_Org(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['merge', 'merging', 'merger']
 
     def get_output_template(self):
         output_template = ''
@@ -1383,25 +1281,22 @@
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('business event, merge organization sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to two or more organization coming together to form a new organization.')
+                    input_str += ' \n {}'.format('The event is related to two or more organization coming together to form a new organization.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Merge-Org' in self.knowledge.keys():
-            knowledge = self.knowledge['Merge-Org']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1412,21 +1307,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else
-                            ROLE_PH_MAP['Org']
+                            " and ".join([ a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else ROLE_PH_MAP['Org']
                         )
                         output_texts.append("{} was merged.".format(filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1436,39 +1330,37 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     org = prediction.split(' was merged.', 1)[0]
                                     org = org.split(' and ')
                                     for arg in org:
                                         if arg != ROLE_PH_MAP['Org']:
-                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))                  
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Business_Declare_Bankruptcy(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['bankruptcy', 'bankrupt', 'Bankruptcy']
 
     def get_output_template(self):
         output_template = ''
@@ -1490,18 +1382,15 @@
                     input_str += ' \n {}'.format('The event is related to some organization declaring bankruptcy.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Declare-Bankruptcy' in self.knowledge.keys():
-            knowledge = self.knowledge['Declare-Bankruptcy']
-            input_str += ' \n {}'.format(knowledge[0])
-            # print(input_str)
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1512,21 +1401,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else
-                            ROLE_PH_MAP['Org']
+                            " and ".join([ a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else ROLE_PH_MAP['Org']
                         )
                         output_texts.append("{} declared bankruptcy.".format(filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1536,43 +1424,41 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     org = prediction.split(' declared bankruptcy.', 1)[0]
                                     org = org.split(' and ')
                                     for arg in org:
                                         if arg != ROLE_PH_MAP['Org']:
-                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))                  
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Business_End_Org(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
-        return ['dissolve', 'disbanded', 'close']
+        return ['dissolve', 'disbanded', 'close'] 
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
@@ -1590,17 +1476,15 @@
                     input_str += ' \n {}'.format('The event is related to some organization ceasing to exist.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'End-Org' in self.knowledge.keys():
-            knowledge = self.knowledge['End-Org']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1611,21 +1495,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else
-                            ROLE_PH_MAP['Org']
+                            " and ".join([ a['argument text'] for a in argu['Org']]) if "Org" in argu.keys() else ROLE_PH_MAP['Org']
                         )
                         output_texts.append("{} dissolved.".format(filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1635,53 +1518,50 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     org = prediction.split(' dissolved.', 1)[0]
                                     org = org.split(' and ')
                                     for arg in org:
                                         if arg != ROLE_PH_MAP['Org']:
-                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Org', {'cor tri cnt': a_cnt}))                  
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Conflict_Attack(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['war', 'attack', 'terrorism']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'some attacker attacked some facility, someone, or some organization by some way in somewhere.')
+                    output_template += ' \n {}'.format('some attacker attacked some facility, someone, or some organization by some way in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -1690,17 +1570,15 @@
                     input_str += ' \n {}'.format('The event is related to conflict and some violent physical act.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Attack' in self.knowledge.keys():
-            knowledge = self.knowledge['Attack']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1712,31 +1590,27 @@
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         attacker_list = []
                         if "Attacker" in argu.keys():
-                            attacker_list.extend([a['argument text'] for a in argu['Attacker']])
+                            attacker_list.extend([ a['argument text'] for a in argu['Attacker']])
                         if "Agent" in argu.keys():
-                            attacker_list.extend([a['argument text'] for a in argu['Agent']])
+                            attacker_list.extend([ a['argument text'] for a in argu['Agent']])  
                         filler = (
-                            " and ".join(attacker_list) if len(attacker_list) > 0 else ROLE_PH_MAP['Attacker'],
-                            " and ".join([a['argument text'] for a in argu['Target']]) if "Target" in argu.keys() else
-                            ROLE_PH_MAP['Target'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Instrument']]) if "Instrument" in argu.keys() else
-                            ROLE_PH_MAP['Instrument'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join(attacker_list) if len(attacker_list)>0 else ROLE_PH_MAP['Attacker'],
+                            " and ".join([ a['argument text'] for a in argu['Target']]) if "Target" in argu.keys() else ROLE_PH_MAP['Target'],
+                            " and ".join([ a['argument text'] for a in argu['Instrument']]) if "Instrument" in argu.keys() else ROLE_PH_MAP['Instrument'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} attacked {} by {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1746,18 +1620,17 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except Exception as e:
-                                # print(e)
+                                #print(e)
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     attack = prediction.split(' attacked ', 1)[0]
@@ -1768,38 +1641,37 @@
                                     target = target.split(' and ')
                                     remain = remain.split(' by ', 1)[1]
 
                                     instrument = remain.split(' in ', 1)[0]
                                     instrument = instrument.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in attack:
                                         if arg != ROLE_PH_MAP['Attacker']:
                                             output.append((arg, 'Attacker', {'cor tri cnt': a_cnt}))
                                     for arg in target:
                                         if arg != ROLE_PH_MAP['Target']:
                                             output.append((arg, 'Target', {'cor tri cnt': a_cnt}))
                                     for arg in instrument:
                                         if arg != ROLE_PH_MAP['Instrument']:
-                                            output.append((arg, 'Instrument', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Instrument', {'cor tri cnt': a_cnt}))                    
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Conflict_Demonstrate(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['rally', 'protest', 'demonstrate']
 
     def get_output_template(self):
         output_template = ''
@@ -1814,25 +1686,22 @@
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('conflict event, demonstrate sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to a large number of people coming together to protest.')
+                    input_str += ' \n {}'.format('The event is related to a large number of people coming together to protest.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Demonstrate' in self.knowledge.keys():
-            knowledge = self.knowledge['Demonstrate']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1843,18 +1712,16 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} protest at {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -1868,45 +1735,43 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     entity = prediction.split(' protest at ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = prediction.split(' protest at ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
-                                pass
+                                pass                                    
                         used_o_cnt += 1
-
+                    
         return output
 
-
 class Contact_Meet(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['meeting', 'met', 'summit']
 
     def get_output_template(self):
         output_template = ''
@@ -1921,25 +1786,22 @@
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('contact event, meet sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to a group of people meeting and interacting with one another face-to-face.')
+                    input_str += ' \n {}'.format('The event is related to a group of people meeting and interacting with one another face-to-face.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Meet' in self.knowledge.keys():
-            knowledge = self.knowledge['Meet']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -1950,23 +1812,21 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} met at {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -1976,79 +1836,73 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     entity = prediction.split(' met at ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = prediction.split(' met at ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
-                                pass
+                                pass                                    
                         used_o_cnt += 1
-
+                    
         return output
-
-
+    
 class Contact_Phone_Write(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['call', 'communicate', 'e-mail']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'some people or some organization called or texted messages at somewhere.')
+                    output_template += ' \n {}'.format('some people or some organization called or texted messages at somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('contact event, phone write sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to people phone calling or messaging one another.')
+                    input_str += ' \n {}'.format('The event is related to people phone calling or messaging one another.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Phone-Write' in self.knowledge.keys():
-            knowledge = self.knowledge['Phone-Write']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2059,23 +1913,21 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} called or texted messages at {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
-
+                
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
         for cnt, pred in enumerate(preds.split('\n')):
             used_o_cnt = 0
@@ -2085,80 +1937,74 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     entity = prediction.split(' called or texted messages at ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = prediction.split(' called or texted messages at ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
-                                pass
+                                pass                                   
                         used_o_cnt += 1
-
+                    
         return output
-
-
+            
 class Personnel_Start_Position(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['hire', 'appoint', 'join']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody got new job and was hired by some people or some organization in somewhere.')
+                    output_template += ' \n {}'.format('somebody got new job and was hired by some people or some organization in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('personnel event, start position sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to a person begins working for an organization or a hiring manager.')
+                    input_str += ' \n {}'.format('The event is related to a person begins working for an organization or a hiring manager.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Start-Position' in self.knowledge.keys():
-            knowledge = self.knowledge['Start-Position']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2169,20 +2015,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} got new job and was hired by {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -2196,16 +2039,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -2213,15 +2055,15 @@
                                     person = person.split(' and ')
                                     remain = prediction.split(' got new job and was hired by ', 1)[1]
 
                                     entity = remain.split(' in ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
@@ -2229,53 +2071,48 @@
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Personnel_End_Position(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['former', 'laid off', 'fired']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody stopped working for some people or some organization at somewhere.')
+                    output_template += ' \n {}'.format('somebody stopped working for some people or some organization at somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('personnel event, end position sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to a person stops working for an organization or a hiring manager.')
+                    input_str += ' \n {}'.format('The event is related to a person stops working for an organization or a hiring manager.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'End-Position' in self.knowledge.keys():
-            knowledge = self.knowledge['End-Position']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2286,20 +2123,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} stopped working for {} at {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -2313,16 +2147,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -2330,15 +2163,15 @@
                                     person = person.split(' and ')
                                     remain = prediction.split(' stopped working for ', 1)[1]
 
                                     entity = remain.split(' at ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = remain.split(' at ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
@@ -2346,33 +2179,31 @@
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Personnel_Nominate(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['named', 'nomination', 'nominate']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was nominated by somebody or some organization to do a job.')
+                    output_template += ' \n {}'.format('somebody was nominated by somebody or some organization to do a job.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -2381,17 +2212,15 @@
                     input_str += ' \n {}'.format('The event is related to a person being nominated for a position.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Nominate' in self.knowledge.keys():
-            knowledge = self.knowledge['Nominate']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2402,18 +2231,16 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent']
                         )
                         output_texts.append("{} was nominated by {} to do a job.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -2427,59 +2254,56 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     person = prediction.split(' was nominated by ', 1)[0]
                                     person = person.split(' and ')
                                     remain = prediction.split(' was nominated by ', 1)[1]
 
-                                    agent = remain.rsplit(' to do a job.', 1)[0]
+                                    agent = remain.rsplit(' to do a job.',1)[0]
                                     agent = agent.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Personnel_Elect(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
         return ['election', 'elect', 'elected']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was elected a position, and the election was voted by some people or some organization in somewhere.')
+                    output_template += ' \n {}'.format('somebody was elected a position, and the election was voted by some people or some organization in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -2488,17 +2312,15 @@
                     input_str += ' \n {}'.format('The event is related to a candidate wins an election.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Elect' in self.knowledge.keys():
-            knowledge = self.knowledge['Elect']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2509,23 +2331,19 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
-                        output_texts.append(
-                            "{} was elected a position, and the election was voted by {} in {}.".format(*filler))
+                        output_texts.append("{} was elected a position, and the election was voted by {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -2537,34 +2355,31 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
-                                    person = \
-                                    prediction.split(' was elected a position, and the election was voted by ', 1)[0]
+                                    person = prediction.split(' was elected a position, and the election was voted by ', 1)[0]
                                     person = person.split(' and ')
-                                    remain = \
-                                    prediction.split(' was elected a position, and the election was voted by ', 1)[1]
+                                    remain = prediction.split(' was elected a position, and the election was voted by ', 1)[1]
 
                                     entity = remain.split(' in ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
@@ -2572,53 +2387,48 @@
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Arrest_Jail(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['arrest', 'jail', 'detained']
-
+    
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was sent to jailed or arrested by somebody or some organization in somewhere.')
+                    output_template += ' \n {}'.format('somebody was sent to jailed or arrested by somebody or some organization in somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('justice event, arrest jail sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to a person getting arrested or a person being sent to jail.')
+                    input_str += ' \n {}'.format('The event is related to a person getting arrested or a person being sent to jail.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Arrest-Jail' in self.knowledge.keys():
-            knowledge = self.knowledge['Arrest-Jail']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2629,20 +2439,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} was sent to jailed or arrested by {} in {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -2656,16 +2463,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -2673,15 +2479,15 @@
                                     person = person.split(' and ')
                                     remain = prediction.split(' was sent to jailed or arrested by ', 1)[1]
 
                                     agent = remain.split(' in ', 1)[0]
                                     agent = agent.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
@@ -2689,33 +2495,31 @@
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except Exception as e:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Release_Parole(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['parole', 'release', 'free']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was released by some people or some organization from somewhere.')
+                    output_template += ' \n {}'.format('somebody was released by some people or some organization from somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -2724,17 +2528,15 @@
                     input_str += ' \n {}'.format("The event is related to an end to someone's custody in prison.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Release-Parole' in self.knowledge.keys():
-            knowledge = self.knowledge['Release-Parole']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2745,20 +2547,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} was released by {} from {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -2772,16 +2571,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -2789,15 +2587,15 @@
                                     person = person.split(' and ')
                                     remain = prediction.split(' was released by ', 1)[1]
 
                                     entity = remain.split(' from ', 1)[0]
                                     entity = entity.split(' and ')
                                     remain = remain.split(' from ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
@@ -2805,33 +2603,31 @@
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Trial_Hearing(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
-        return ['trial', 'hearing', 'proceeding']
-
+        return ['trial', 'hearing', 'proceeding']    
+    
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody, prosecuted by some other, faced a trial in somewhere. The hearing was judged by some adjudicator.')
+                    output_template += ' \n {}'.format('somebody, prosecuted by some other, faced a trial in somewhere. The hearing was judged by some adjudicator.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -2840,17 +2636,14 @@
                     input_str += ' \n {}'.format("The event is related to a trial or hearing for someone.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Trial-Hearing' in self.knowledge.keys():
-            knowledge = self.knowledge['Trial-Hearing']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2861,28 +2654,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Prosecutor']]) if "Prosecutor" in argu.keys() else
-                            ROLE_PH_MAP['Prosecutor'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Prosecutor']]) if "Prosecutor" in argu.keys() else ROLE_PH_MAP['Prosecutor'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
-                        output_texts.append(
-                            "{}, prosecuted by {}, faced a trial in {}. The hearing was judged by {}.".format(*filler))
+                        output_texts.append("{}, prosecuted by {}, faced a trial in {}. The hearing was judged by {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -2894,16 +2679,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -2915,15 +2699,15 @@
                                     prosecutor = prosecutor.split(' and ')
                                     remain = remain.split(', faced a trial in ', 1)[1]
 
                                     place = remain.split('. The hearing was judged by ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split('. The hearing was judged by ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in prosecutor:
                                         if arg != ROLE_PH_MAP['Prosecutor']:
                                             output.append((arg, 'Prosecutor', {'cor tri cnt': a_cnt}))
@@ -2934,53 +2718,47 @@
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except Exception as e:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Charge_Indict(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['indict', 'charged', 'accused']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was charged by some other in somewhere. The adjudication was judged by some adjudicator.')
+                    output_template += ' \n {}'.format('somebody was charged by some other in somewhere. The adjudication was judged by some adjudicator.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('justice event, charge indict sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        "The event is related to someone or some organziation being accused of a crime.")
+                    input_str += ' \n {}'.format("The event is related to someone or some organization being accused of a crime.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Charge-Indict' in self.knowledge.keys():
-            knowledge = self.knowledge['Charge-Indict']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -2991,28 +2769,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Prosecutor']]) if "Prosecutor" in argu.keys() else
-                            ROLE_PH_MAP['Prosecutor'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Prosecutor']]) if "Prosecutor" in argu.keys() else ROLE_PH_MAP['Prosecutor'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
-                        output_texts.append(
-                            "{} was charged by {} in {}. The adjudication was judged by {}.".format(*filler))
+                        output_texts.append("{} was charged by {} in {}. The adjudication was judged by {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -3024,16 +2794,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -3045,15 +2814,15 @@
                                     prosecutor = prosecutor.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
                                     place = remain.split('. The adjudication was judged by ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split('. The adjudication was judged by ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in prosecutor:
                                         if arg != ROLE_PH_MAP['Prosecutor']:
                                             output.append((arg, 'Prosecutor', {'cor tri cnt': a_cnt}))
@@ -3064,53 +2833,47 @@
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Sue(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['sue', 'lawsuit', 'suit']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was sued by some other in somewhere. The adjudication was judged by some adjudicator.')
+                    output_template += ' \n {}'.format('somebody was sued by some other in somewhere. The adjudication was judged by some adjudicator.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('justice event, sue sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        "The event is related to a court proceeding that has been initiated and someone sue the other.")
+                    input_str += ' \n {}'.format("The event is related to a court proceeding that has been initiated and someone sue the other.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Sue' in self.knowledge.keys():
-            knowledge = self.knowledge['Sue']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3121,28 +2884,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Plaintiff']]) if "Plaintiff" in argu.keys() else
-                            ROLE_PH_MAP['Plaintiff'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Plaintiff']]) if "Plaintiff" in argu.keys() else ROLE_PH_MAP['Plaintiff'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
-                        output_texts.append(
-                            "{} was sued by {} in {}. The adjudication was judged by {}.".format(*filler))
+                        output_texts.append("{} was sued by {} in {}. The adjudication was judged by {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -3154,16 +2909,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -3175,15 +2929,15 @@
                                     plaintiff = plaintiff.split(' and ')
                                     remain = remain.split(' in ', 1)[1]
 
                                     place = remain.split('. The adjudication was judged by ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split('. The adjudication was judged by ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in plaintiff:
                                         if arg != ROLE_PH_MAP['Plaintiff']:
                                             output.append((arg, 'Plaintiff', {'cor tri cnt': a_cnt}))
@@ -3194,33 +2948,31 @@
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Convict(event_template):
 
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['convicted', 'guilty', 'verdict']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was convicted of a crime in somewhere. The adjudication was judged by some adjudicator.')
+                    output_template += ' \n {}'.format('somebody was convicted of a crime in somewhere. The adjudication was judged by some adjudicator.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -3229,17 +2981,14 @@
                     input_str += ' \n {}'.format("The event is related to someone being found guilty of a crime.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Convict' in self.knowledge.keys():
-            knowledge = self.knowledge['Convict']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3250,25 +2999,19 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
-                        output_texts.append(
-                            "{} was convicted of a crime in {}. The adjudication was judged by {}.".format(*filler))
+                        output_texts.append("{} was convicted of a crime in {}. The adjudication was judged by {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -3280,16 +3023,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -3297,15 +3039,15 @@
                                     defendant = defendant.split(' and ')
                                     remain = prediction.split(' was convicted of a crime in ', 1)[1]
 
                                     place = remain.split('. The adjudication was judged by ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split('. The adjudication was judged by ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
@@ -3313,52 +3055,46 @@
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Sentence(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['sentenced', 'sentencing', 'sentence']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was sentenced to punishment in somewhere. The adjudication was judged by some adjudicator.')
+                    output_template += ' \n {}'.format('somebody was sentenced to punishment in somewhere. The adjudication was judged by some adjudicator.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('justice event, sentence sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        "The event is related to someone being sentenced to punishment because of a crime.")
+                    input_str += ' \n {}'.format("The event is related to someone being sentenced to punishment because of a crime.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Sentence' in self.knowledge.keys():
-            knowledge = self.knowledge['Sentence']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3369,25 +3105,19 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
-                        output_texts.append(
-                            "{} was sentenced to punishment in {}. The adjudication was judged by {}.".format(*filler))
+                        output_texts.append("{} was sentenced to punishment in {}. The adjudication was judged by {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -3399,16 +3129,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -3416,15 +3145,15 @@
                                     defendant = defendant.split(' and ')
                                     remain = prediction.split(' was sentenced to punishment in ', 1)[1]
 
                                     place = remain.split('. The adjudication was judged by ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split('. The adjudication was judged by ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
@@ -3432,32 +3161,30 @@
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Fine(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['fine', 'fined', 'payouts']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'some people or some organization in somewhere was ordered by some adjudicator to pay a fine.')
+                    output_template += ' \n {}'.format('some people or some organization in somewhere was ordered by some adjudicator to pay a fine.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -3466,17 +3193,14 @@
                     input_str += ' \n {}'.format("The event is related to someone being issued a financial punishment.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Fine' in self.knowledge.keys():
-            knowledge = self.knowledge['Fine']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3487,21 +3211,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else
-                            ROLE_PH_MAP['Entity'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Entity']]) if "Entity" in argu.keys() else ROLE_PH_MAP['Entity'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
                         output_texts.append("{} in {} was ordered by {} to pay a fine.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -3515,16 +3235,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -3532,15 +3251,15 @@
                                     entity = entity.split(' and ')
                                     remain = prediction.split(' in ', 1)[1]
 
                                     place = remain.split(' was ordered by ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split(' was ordered by ', 1)[1]
 
-                                    adjudicator = remain.rsplit(' to pay a fine.', 1)[0]
+                                    adjudicator = remain.rsplit(' to pay a fine.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in entity:
                                         if arg != ROLE_PH_MAP['Entity']:
                                             output.append((arg, 'Entity', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
@@ -3548,32 +3267,30 @@
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except Exception as e:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Execute(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['execution', 'executed', 'execute']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was executed by somebody or some organization at somewhere.')
+                    output_template += ' \n {}'.format('somebody was executed by somebody or some organization at somewhere.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -3582,17 +3299,14 @@
                     input_str += ' \n {}'.format("The event is related to someone being executed to death.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Execute' in self.knowledge.keys():
-            knowledge = self.knowledge['Execute']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3603,20 +3317,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place']
                         )
                         output_texts.append("{} was executed by {} at {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -3630,16 +3341,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -3647,68 +3357,63 @@
                                     person = person.split(' and ')
                                     remain = prediction.split(' was executed by ', 1)[1]
 
                                     agent = remain.split(' at ', 1)[0]
                                     agent = agent.split(' and ')
                                     remain = remain.split(' at ', 1)[1]
 
-                                    place = remain.rsplit('.', 1)[0]
+                                    place = remain.rsplit('.',1)[0]
                                     place = place.split(' and ')
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                                     for arg in agent:
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
-
-
+            
 class Justice_Extradite(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['extradition', 'extradited', 'extraditing']
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'somebody was extradicted to somewhere from some place. somebody or some organization was responsible for the extradition.')
+                    output_template += ' \n {}'.format('somebody was extradicted to somewhere from some place. somebody or some organization was responsible for the extradition.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
                     input_str += ' \n {}'.format('justice event, extradite sub-type')
                 if i_style == 'event_type_sent':
-                    input_str += ' \n {}'.format(
-                        'The event is related to justice. The event occurs when a person was extradited from one place to another place.')
+                    input_str += ' \n {}'.format('The event is related to justice. The event occurs when a person was extradited from one place to another place.')
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Extradite' in self.knowledge.keys():
-            knowledge = self.knowledge['Extradite']
-            input_str += ' \n {}'.format(knowledge[0])
+        
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3719,26 +3424,20 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join([a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else
-                            ROLE_PH_MAP['Person'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Destination']]) if "Destination" in argu.keys() else
-                            ROLE_PH_MAP['Destination'],
-                            " and ".join([a['argument text'] for a in argu['Origin']]) if "Origin" in argu.keys() else
-                            ROLE_PH_MAP['Origin'],
-                            " and ".join([a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else
-                            ROLE_PH_MAP['Agent']
+                            " and ".join([ a['argument text'] for a in argu['Person']]) if "Person" in argu.keys() else ROLE_PH_MAP['Person'],
+                            " and ".join([ a['argument text'] for a in argu['Destination']]) if "Destination" in argu.keys() else ROLE_PH_MAP['Destination'],
+                            " and ".join([ a['argument text'] for a in argu['Origin']]) if "Origin" in argu.keys() else ROLE_PH_MAP['Origin'],
+                            " and ".join([ a['argument text'] for a in argu['Agent']]) if "Agent" in argu.keys() else ROLE_PH_MAP['Agent']
                         )
-                        output_texts.append(
-                            "{} was extradicted to {} from {}. {} was responsible for the extradition.".format(*filler))
+                        output_texts.append("{} was extradicted to {} from {}. {} was responsible for the extradition.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
     def decode(self, preds):
         output = []
@@ -3750,35 +3449,32 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     person = prediction.split(' was extradicted to ')[0]
                                     person = person.split(' and ')
 
                                     destination = (prediction.split(' was extradicted to ')[1]).split(' from ')[0]
                                     destination = destination.split(' and ')
 
-                                    origin = \
-                                    ((prediction.split(' was extradicted to ')[1]).split(' from ')[1]).split('.', 1)[0]
+                                    origin = ((prediction.split(' was extradicted to ')[1]).split(' from ')[1]).split('.', 1)[0]
                                     origin = origin.split(' and ')
 
-                                    remain = \
-                                    ((prediction.split(' was extradicted to ')[1]).split(' from ')[1]).split('.', 1)[1]
+                                    remain = ((prediction.split(' was extradicted to ')[1]).split(' from ')[1]).split('.', 1)[1]
 
                                     if 'was responsible for' in remain:
                                         agent = (remain.split(' was responsible for the extradition.')[0]).strip()
                                         agent = agent.split(' and ')
                                     else:
                                         agent = []
 
@@ -3786,27 +3482,26 @@
                                         if arg != ROLE_PH_MAP['Agent']:
                                             output.append((arg, 'Agent', {'cor tri cnt': a_cnt}))
                                     for arg in person:
                                         if arg != ROLE_PH_MAP['Person']:
                                             output.append((arg, 'Person', {'cor tri cnt': a_cnt}))
                                     for arg in destination:
                                         if arg != ROLE_PH_MAP['Destination']:
-                                            output.append((arg, 'Destination', {'cor tri cnt': a_cnt}))
+                                            output.append((arg, 'Destination', {'cor tri cnt': a_cnt}))          
                                     for arg in origin:
                                         if arg != ROLE_PH_MAP['Origin']:
                                             output.append((arg, 'Origin', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Acquit(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['acquitted', 'acquittal', 'acquit']
 
     def get_output_template(self):
         output_template = ''
@@ -3828,17 +3523,14 @@
                     input_str += ' \n {}'.format("The event is related to someone being acquitted.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Acquit' in self.knowledge.keys():
-            knowledge = self.knowledge['Acquit']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3849,20 +3541,16 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
                         output_texts.append("{} was acquitted of the charges by {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -3876,44 +3564,42 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     defendant = prediction.split(' was acquitted of the charges by ', 1)[0]
                                     defendant = defendant.split(' and ')
                                     remain = prediction.split(' was acquitted of the charges by ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in adjudicator:
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Pardon(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
 
     @classmethod
     def get_keywords(self):
         return ['pardon', 'pardoned', 'remission']
 
     def get_output_template(self):
         output_template = ''
@@ -3935,17 +3621,14 @@
                     input_str += ' \n {}'.format("The event is related to someone being pardoned.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Pardon' in self.knowledge.keys():
-            knowledge = self.knowledge['Pardon']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -3956,20 +3639,16 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else
-                            ROLE_PH_MAP['Defendant'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Defendant']]) if "Defendant" in argu.keys() else ROLE_PH_MAP['Defendant'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
                         output_texts.append("{} received a pardon from {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -3983,58 +3662,55 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
                                     defendant = prediction.split(' received a pardon from ', 1)[0]
                                     defendant = defendant.split(' and ')
                                     remain = prediction.split(' received a pardon from ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
                                     for arg in defendant:
                                         if arg != ROLE_PH_MAP['Defendant']:
                                             output.append((arg, 'Defendant', {'cor tri cnt': a_cnt}))
                                     for arg in adjudicator:
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
         return output
 
-
 class Justice_Appeal(event_template):
-    def __init__(self, input_style, output_style, passage, event_type, gold_event=None, knowledge=None):
-        super().__init__(input_style, output_style, passage, event_type, gold_event, knowledge)
-
+    def __init__(self, input_style, output_style, passage, event_type, gold_event=None):
+        super().__init__(input_style, output_style, passage, event_type, gold_event)
+    
     @classmethod
     def get_keywords(self):
-        return ['appeal', 'appealing', 'appeals']
+        return ['appeal', 'appealing', 'appeals']  
 
     def get_output_template(self):
         output_template = ''
         for o_style in OUTPUT_STYLE_SET:
             if o_style in self.output_style:
                 if o_style == 'trigger:sentence':
                     output_template += ' \n {}'.format('Event trigger is <Trigger>')
                 if o_style == 'argument:sentence':
-                    output_template += ' \n {}'.format(
-                        'some other in somewhere appealed the adjudication from some adjudicator.')
+                    output_template += ' \n {}'.format('some other in somewhere appealed the adjudication from some adjudicator.')
         return ('\n'.join(output_template.split('\n')[1:])).strip()
 
     def generate_input_str(self, query_trigger):
         input_str = self.passage
         for i_style in INPUT_STYLE_SET:
             if i_style in self.input_style:
                 if i_style == 'event_type':
@@ -4043,17 +3719,14 @@
                     input_str += ' \n {}'.format("The event is related to someone appealing the decision of a court.")
                 if i_style == 'keywords':
                     input_str += ' \n Similar triggers such as {}'.format(', '.join(self.get_keywords()))
                 if i_style == 'triggers':
                     input_str += ' \n The event trigger word is {}'.format(query_trigger)
                 if i_style == 'template':
                     input_str += ' \n {}'.format(self.output_template)
-        if 'Appeal' in self.knowledge.keys():
-            knowledge = self.knowledge['Appeal']
-            input_str += ' \n {}'.format(knowledge[0])
         return input_str
 
     def generate_output_str(self, query_trigger):
         assert self.gold_event is not None
         output_str = ''
         gold_sample = False
         for o_style in OUTPUT_STYLE_SET:
@@ -4064,22 +3737,17 @@
                         gold_sample = True
                     else:
                         output_str += ' \n Event trigger is <Trigger>'
                 if o_style == 'argument:sentence':
                     output_texts = []
                     for argu in self.arguments:
                         filler = (
-                            " and ".join(
-                                [a['argument text'] for a in argu['Plaintiff']]) if "Plaintiff" in argu.keys() else
-                            ROLE_PH_MAP['Plaintiff'],
-                            " and ".join([a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else
-                            ROLE_PH_MAP['Place'],
-                            " and ".join(
-                                [a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else
-                            ROLE_PH_MAP['Adjudicator']
+                            " and ".join([ a['argument text'] for a in argu['Plaintiff']]) if "Plaintiff" in argu.keys() else ROLE_PH_MAP['Plaintiff'],
+                            " and ".join([ a['argument text'] for a in argu['Place']]) if "Place" in argu.keys() else ROLE_PH_MAP['Place'],
+                            " and ".join([ a['argument text'] for a in argu['Adjudicator']]) if "Adjudicator" in argu.keys() else ROLE_PH_MAP['Adjudicator']
                         )
                         output_texts.append("{} in {} appealed the adjudication from {}.".format(*filler))
                         gold_sample = True
                     output_str += ' \n {}'.format(' <sep> '.join(output_texts))
         output_str = ('\n'.join(output_str.split('\n')[1:])).strip()
         return (output_str, gold_sample)
 
@@ -4093,16 +3761,15 @@
                     if o_style == 'trigger:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 triggers = full_pred.split('Event trigger is ', 1)[1]
                                 triggers = triggers.split(' and ')
                                 for t_cnt, t in enumerate(triggers):
                                     if t != '<Trigger>':
-                                        output.append(
-                                            (t, self.event_type, {'tri counter': t_cnt}))  # (text, type, kwargs)
+                                        output.append((t, self.event_type, {'tri counter': t_cnt})) # (text, type, kwargs)
                             except:
                                 pass
                         used_o_cnt += 1
                     if o_style == 'argument:sentence':
                         if used_o_cnt == cnt:
                             try:
                                 for a_cnt, prediction in enumerate(full_pred.split(' <sep> ')):
@@ -4110,23 +3777,23 @@
                                     plaintiff = plaintiff.split(' and ')
                                     remain = prediction.split(' in ', 1)[1]
 
                                     place = remain.split(' appealed the adjudication from ', 1)[0]
                                     place = place.split(' and ')
                                     remain = remain.split(' appealed the adjudication from ', 1)[1]
 
-                                    adjudicator = remain.rsplit('.', 1)[0]
+                                    adjudicator = remain.rsplit('.',1)[0]
                                     adjudicator = adjudicator.split(' and ')
 
                                     for arg in plaintiff:
                                         if arg != ROLE_PH_MAP['Plaintiff']:
                                             output.append((arg, 'Plaintiff', {'cor tri cnt': a_cnt}))
                                     for arg in place:
                                         if arg != ROLE_PH_MAP['Place']:
                                             output.append((arg, 'Place', {'cor tri cnt': a_cnt}))
                                     for arg in adjudicator:
                                         if arg != ROLE_PH_MAP['Adjudicator']:
                                             output.append((arg, 'Adjudicator', {'cor tri cnt': a_cnt}))
                             except:
                                 pass
                         used_o_cnt += 1
-        return output
+        return output
```

### Comparing `deepke-2.1.3/src/deepke/event_extraction/standard/degree/utils.py` & `deepke-2.2/src/deepke/event_extraction/standard/degree/utils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/few_shot/models/model.py` & `deepke-2.2/src/deepke/name_entity_re/few_shot/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
-from transformers.configuration_bart import BartConfig
-from .modeling_bart import BartModel, _prepare_bart_decoder_inputs
+from transformers.models.bart.configuration_bart import BartConfig
+from .modeling_bart import BartModel
 
-from ..utils import avg_token_embeddings, seq_to_mask,get_model_device
+from .util import avg_token_embeddings, seq_to_mask, get_model_device
 from functools import partial
 from typing import Union
 
 
 class PromptBartEncoder(nn.Module):
     def __init__(self, encoder):
         super(PromptBartEncoder, self).__init__()
         self.bart_encoder = encoder
     
     def forward(self, src_tokens, attention_mask=None, past_key_values=None):
-        encoder_dicts = self.bart_encoder(input_ids=src_tokens, attention_mask=attention_mask, past_key_values=past_key_values, return_dict=True, output_hidden_states=True)
+        encoder_dicts = self.bart_encoder(input_ids=src_tokens, attention_mask=attention_mask, return_dict=True, output_hidden_states=True, past_prompt=past_key_values)
         return encoder_dicts.last_hidden_state, encoder_dicts.hidden_states
         
 class PromptBartDecoder(nn.Module):
     def __init__(self, decoder, pad_token_id, label_ids, use_prompt=False, prompt_len=10, learn_weights=False):
         super(PromptBartDecoder, self).__init__()
         self.bart_decoder = decoder
         self.pad_token_id = pad_token_id
@@ -78,54 +78,84 @@
         if first is not None:
             src_tokens = src_tokens.gather(index=first, dim=1)
         word_mapped_tokens = src_tokens.gather(index=src_tokens_index, dim=1)
 
         tokens = torch.where(mapping_token_mask, tag_mapped_tokens, word_mapped_tokens)  # bsz x max_len
         tokens = tokens.masked_fill(tgt_pad_mask, self.pad_token_id)
 
-        decoder_input_ids, _, causal_mask = _prepare_bart_decoder_inputs(
-                self.pad_token_id, 
-                tokens,
-                decoder_input_ids=None,
-                decoder_padding_mask=None,
-                causal_mask_dtype=self.bart_decoder.embed_tokens.weight.dtype
-        )
-
-        if self.use_prompt:
-            assert past_key_values is not None
-            _, _, seqlen, _ = past_key_values[0]['self']['prev_value'].shape
-            tgt_len = decoder_input_ids.size(1)
-            temp_mask = torch.zeros(tgt_len, seqlen).to(causal_mask.device) #tgtlen, preseqlen
-            causal_mask = torch.cat([temp_mask, causal_mask],dim=1) #tgtlen, preseqlen+tgtlen
+        # decoder_input_ids, _, causal_mask = _prepare_bart_decoder_inputs(
+        #         self.pad_token_id, 
+        #         tokens,
+        #         decoder_input_ids=None,
+        #         decoder_padding_mask=None,
+        #         causal_mask_dtype=self.bart_decoder.embed_tokens.weight.dtype
+        # )
+
+        # if self.use_prompt:
+        #     assert past_key_values is not None
+        #     _, _, seqlen, _ = past_key_values[0]['self']['prev_value'].shape
+        #     tgt_len = decoder_input_ids.size(1)
+        #     temp_mask = torch.zeros(tgt_len, seqlen).to(causal_mask.device) #tgtlen, preseqlen
+        #     causal_mask = torch.cat([temp_mask, causal_mask],dim=1) #tgtlen, preseqlen+tgtlen
 
         if self.training:
             tokens = tokens[:, :-1]
-            decoder_pad_mask = tokens.eq(self.pad_token_id) 
-            dict = self.bart_decoder(input_ids=tokens,
-                                encoder_hidden_states=encoder_outputs,  # last_hidden_state
-                                encoder_padding_mask=attention_mask,  # attention_mask
-                                decoder_padding_mask=decoder_pad_mask,
-                                decoder_causal_mask=causal_mask[:tokens.size(1), :self.prompt_len+tokens.size(1)],
-                                output_hidden_states=True,
-                                past_key_values=past_key_values,
-                                return_dict=True)
+            decoder_attention_mask = tokens.ne(self.pad_token_id)
+            # dict = self.bart_decoder(input_ids=tokens,
+            #                     encoder_hidden_states=encoder_outputs,  # last_hidden_state
+            #                     encoder_padding_mask=attention_mask,  # attention_mask
+            #                     decoder_padding_mask=decoder_pad_mask,
+            #                     decoder_causal_mask=causal_mask[:tokens.size(1), :self.prompt_len+tokens.size(1)],
+            #                     output_hidden_states=True,
+            #                     past_key_values=past_key_values,
+            #                     return_dict=True)
+            dict = self.bart_decoder(
+                input_ids=tokens,
+                attention_mask=decoder_attention_mask,
+                encoder_hidden_states=encoder_outputs,
+                encoder_attention_mask=attention_mask,
+                output_hidden_states=True,
+                return_dict=True,
+                past_prompt=past_key_values
+            )
         else:
             past_key_values = prompt_state.past_key_values
-            dict = self.bart_decoder(input_ids=tokens,
-                                encoder_hidden_states=encoder_outputs,
-                                encoder_padding_mask=attention_mask,
-                                decoder_padding_mask=None,
-                                decoder_causal_mask=None,
-                                past_key_values=past_key_values,
-                                use_cache=True,
-                                return_dict=True)
+            # dict = self.bart_decoder(input_ids=tokens,
+            #                     encoder_hidden_states=encoder_outputs,
+            #                     encoder_padding_mask=attention_mask,
+            #                     decoder_padding_mask=None,
+            #                     decoder_causal_mask=None,
+            #                     past_key_values=past_key_values,
+            #                     use_cache=True,
+            #                     return_dict=True)
+            dict = self.bart_decoder(
+                input_ids=tokens,
+                attention_mask=None,
+                encoder_hidden_states=encoder_outputs,
+                encoder_attention_mask=attention_mask,
+                past_key_values=None,
+                use_cache=True,
+                return_dict=True,
+                past_prompt=past_key_values
+            )
         hidden_state = dict.last_hidden_state  # bsz x max_len x hidden_size
         hidden_state = self.dropout_layer(hidden_state)
         if not self.training:
-            prompt_state.past_key_values = dict.past_key_values
+            dict_past_key_values = dict.past_key_values
+            state_past_key_values = []
+            for i in range(len(dict_past_key_values)):
+                tup = dict_past_key_values[i]
+                state_past_key_values.append({})
+                state_past_key_values[i]['decoder_prompt'] = {}
+                state_past_key_values[i]['decoder_prompt']['prev_key'] = tup[0]
+                state_past_key_values[i]['decoder_prompt']['prev_value'] = tup[1]
+                state_past_key_values[i]['cross_attention_prompt'] = {}
+                state_past_key_values[i]['cross_attention_prompt']['prev_key'] = tup[2]
+                state_past_key_values[i]['cross_attention_prompt']['prev_value'] = tup[3]
+            prompt_state.past_key_values = state_past_key_values
 
         logits = hidden_state.new_full((hidden_state.size(0), hidden_state.size(1), self.src_start_index+src_tokens.size(-1)),
                                        fill_value=-1e24)
 
         # compute eos scores
         eos_scores = F.linear(hidden_state, self.dropout_layer(self.bart_decoder.embed_tokens.weight[2:3]))  # bsz x max_len x 1
         
@@ -262,29 +292,29 @@
         past_key_values_enc = past_key_values_enc.view(bsz, seqlen, self.bart_config.decoder_layers * 2, 
                                                        self.bart_config.decoder_attention_heads, self.bart_config.d_model // self.bart_config.decoder_attention_heads)
         past_key_values_enc = self.dropout(past_key_values_enc)
         past_key_values_enc = past_key_values_enc.permute([2, 0, 3, 1, 4]).split(2)
 
         result = []
         for i, key_val in enumerate(past_key_values):
-            temp_dict = {'self': {"prev_key": key_val[0].contiguous(),
-                                    "prev_value": key_val[1].contiguous(),
-                                    "prev_key_padding_mask": torch.zeros(bsz, seqlen).to(key_val.device).bool() #bsz, preseqlen
-                                    },
+            temp_dict = {'decoder_prompt': {"prev_key": key_val[0].contiguous(),
+                                            "prev_value": key_val[1].contiguous(),
+                                            "prev_key_padding_mask": torch.zeros(bsz, seqlen).to(key_val.device).bool(),
+                                            },
                         }
-            key_val2 = past_key_values2[i]
-            temp_dict['encoder_decoder'] = {"prev_key": key_val2[0].contiguous(),
-                                            "prev_value": key_val2[1].contiguous(),
-                                            "prev_key_padding_mask": torch.zeros(bsz, seqlen).to(key_val2.device).bool()
-                                            }
+            key_val_dec = past_key_values2[i]
+            temp_dict['cross_attention_prompt'] = {"prev_key": key_val_dec[0].contiguous(),
+                                                   "prev_value": key_val_dec[1].contiguous(),
+                                                   "prev_key_padding_mask": torch.zeros(bsz, seqlen).to(key_val_dec.device).bool(),
+                                                  }
             key_val_enc = past_key_values_enc[i]
-            temp_dict['encoder'] = {"prev_key": key_val_enc[0].contiguous(),
-                                    "prev_value": key_val_enc[1].contiguous(),
-                                    "prev_key_padding_mask": torch.zeros(bsz, seqlen).to(key_val_enc.device).bool()
-                                    }
+            temp_dict['encoder_prompt'] = {"prev_key": key_val_enc[0].contiguous(),
+                                           "prev_value": key_val_enc[1].contiguous(),
+                                           "prev_key_padding_mask": torch.zeros(bsz, seqlen).to(key_val_enc.device).bool(),
+                                          }
             result.append(temp_dict)
 
         return result
 
     
 class PromptBartState(object):
     def __init__(self, encoder_output, encoder_mask, past_key_values, src_tokens, first, src_embed_outputs, preseqlen):
```

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/datasets.py` & `deepke-2.2/src/deepke/name_entity_re/few_shot/module/datasets.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/mapping_type.py` & `deepke-2.2/src/deepke/name_entity_re/few_shot/module/mapping_type.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/metrics.py` & `deepke-2.2/src/deepke/name_entity_re/few_shot/module/metrics.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/few_shot/module/train.py` & `deepke-2.2/src/deepke/name_entity_re/few_shot/module/train.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/few_shot/utils/util.py` & `deepke-2.2/src/deepke/name_entity_re/few_shot/utils/util.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/IFA_model.py` & `deepke-2.2/src/deepke/relation_extraction/multimodal/models/IFA_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 import torch
 from torch import nn
-from torchcrf import CRF
+
 import torch.nn.functional as F
 from .modeling_IFA import IFAModel
-from .clip.modeling_clip import CLIPModel
-from .clip.configuration_clip import CLIPConfig
-from transformers import BertConfig, BertModel
-
-class IFANERCRFModel(nn.Module):
-    def __init__(self, label_list, args):
-        super(IFANERCRFModel, self).__init__()
+from transformers import BertConfig, BertModel, CLIPConfig, CLIPModel
+
+class IFAREModel(nn.Module):
+    def __init__(self, num_labels, tokenizer, args):
+        super(IFAREModel, self).__init__()
+
         self.args = args
         self.vision_config = CLIPConfig.from_pretrained(self.args.vit_name).vision_config
         self.text_config = BertConfig.from_pretrained(self.args.bert_name)
 
         clip_model_dict = CLIPModel.from_pretrained(self.args.vit_name).vision_model.state_dict()
         bert_model_dict = BertModel.from_pretrained(self.args.bert_name).state_dict()
 
         print(self.vision_config)
         print(self.text_config)
 
+        # for re
         self.vision_config.device = args.device
         self.model = IFAModel(self.vision_config, self.text_config)
 
-        self.num_labels  = len(label_list) + 1  # pad
-        self.crf = CRF(self.num_labels, batch_first=True)
-        self.fc = nn.Linear(self.text_config.hidden_size, self.num_labels)
-        self.dropout = nn.Dropout(0.1)
-
         # load:
         vision_names, text_names = [], []
         model_dict = self.model.state_dict()
         for name in model_dict:
             if 'vision' in name:
                 clip_name = name.replace('vision_', '').replace('model.', '')
                 if clip_name in clip_model_dict:
@@ -42,38 +37,50 @@
                 if text_name in bert_model_dict:
                     text_names.append(text_name)
                     model_dict[name] = bert_model_dict[text_name]
         assert len(vision_names) == len(clip_model_dict) and len(text_names) == len(bert_model_dict), \
                     (len(vision_names), len(text_names), len(clip_model_dict), len(bert_model_dict))
         self.model.load_state_dict(model_dict)
 
+        self.model.resize_token_embeddings(len(tokenizer))
+
+        self.dropout = nn.Dropout(0.5)
+        self.classifier = nn.Linear(self.text_config.hidden_size*2, num_labels)
+        self.head_start = tokenizer.convert_tokens_to_ids("<s>")
+        self.tail_start = tokenizer.convert_tokens_to_ids("<o>")
+        self.tokenizer = tokenizer
+
     def forward(
             self, 
             input_ids=None, 
             attention_mask=None, 
             token_type_ids=None, 
             labels=None, 
             images=None, 
             aux_imgs=None,
             rcnn_imgs=None,
     ):
         bsz = input_ids.size(0)
-
         output = self.model(input_ids=input_ids,
                             attention_mask=attention_mask,
                             token_type_ids=token_type_ids,
 
                             pixel_values=images,
                             aux_values=aux_imgs, 
                             rcnn_values=rcnn_imgs,
                             return_dict=True,)
 
-        sequence_output = output.last_hidden_state       # bsz, len, hidden
-        sequence_output = self.dropout(sequence_output)  # bsz, len, hidden
-        emissions = self.fc(sequence_output)             # bsz, len, labels
-        
-        logits = self.crf.decode(emissions, attention_mask.byte())
-        loss = None
+        last_hidden_state, pooler_output = output.last_hidden_state, output.pooler_output
+        bsz, seq_len, hidden_size = last_hidden_state.shape
+        entity_hidden_state = torch.Tensor(bsz, 2*hidden_size) # batch, 2*hidden
+        for i in range(bsz):
+            head_idx = input_ids[i].eq(self.head_start).nonzero().item()
+            tail_idx = input_ids[i].eq(self.tail_start).nonzero().item()
+            head_hidden = last_hidden_state[i, head_idx, :].squeeze()
+            tail_hidden = last_hidden_state[i, tail_idx, :].squeeze()
+            entity_hidden_state[i] = torch.cat([head_hidden, tail_hidden], dim=-1)
+        entity_hidden_state = entity_hidden_state.to(self.args.device)
+        logits = self.classifier(entity_hidden_state)
         if labels is not None:
-            loss = -1 * self.crf(emissions, labels, mask=attention_mask.byte(), reduction='mean')  # 去掉CLS
-            return logits, loss
-        return logits, None
+            loss_fn = nn.CrossEntropyLoss()
+            return loss_fn(logits, labels.view(-1)), logits
+        return logits
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/clip/modeling_clip.py` & `deepke-2.2/src/deepke/name_entity_re/multimodal/models/modeling_IFA.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,104 @@
-# coding=utf-8
-# Copyright 2021 The OpenAI Team Authors and The HuggingFace Team. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-""" PyTorch CLIP model. """
-
-
 from typing import Any, Optional, Tuple
+import math
 
+import copy
 import torch
-import torch.utils.checkpoint
-from torch import nn
+from torch import nn, Tensor, device
 
 from transformers.activations import ACT2FN
-from transformers.file_utils import (
-    ModelOutput,
-    add_start_docstrings,
-    replace_return_docstrings,
+from transformers.modeling_utils import (
+    PreTrainedModel,
+    apply_chunking_to_forward,
 )
-from transformers.file_utils import ModelOutput
+from transformers.configuration_utils import PretrainedConfig
 from transformers.modeling_outputs import BaseModelOutput, BaseModelOutputWithPooling
-from transformers.modeling_utils import PreTrainedModel
-from transformers.utils import logging
-from .configuration_clip import CLIPConfig, CLIPTextConfig, CLIPVisionConfig
-
-logger = logging.get_logger(__name__)
-
-_CHECKPOINT_FOR_DOC = "openai/clip-vit-base-patch32"
-
-CLIP_PRETRAINED_MODEL_ARCHIVE_LIST = [
-    "openai/clip-vit-base-patch32",
-    # See all CLIP models at https://huggingface.co/models?filter=clip
-]
-
-
-# Copied from transformers.models.bart.modeling_bart._expand_mask
-def _expand_mask(mask: torch.Tensor, dtype: torch.dtype, tgt_len: Optional[int] = None):
-    """
-    Expands attention_mask from `[bsz, seq_len]` to `[bsz, 1, tgt_seq_len, src_seq_len]`.
-    """
-    bsz, src_len = mask.size()
-    tgt_len = tgt_len if tgt_len is not None else src_len
-
-    expanded_mask = mask[:, None, None, :].expand(bsz, 1, tgt_len, src_len).to(dtype)
-
-    inverted_mask = 1.0 - expanded_mask
-
-    return inverted_mask.masked_fill(inverted_mask.bool(), torch.finfo(dtype).min)
-
-
-# contrastive loss function, adapted from
-# https://sachinruk.github.io/blog/pytorch/pytorch%20lightning/loss%20function/gpu/2021/03/07/CLIP.html
-def contrastive_loss(logits: torch.Tensor) -> torch.Tensor:
-    return nn.functional.cross_entropy(logits, torch.arange(len(logits), device=logits.device))
-
-
-def clip_loss(similarity: torch.Tensor) -> torch.Tensor:
-    caption_loss = contrastive_loss(similarity)
-    image_loss = contrastive_loss(similarity.T)
-    return (caption_loss + image_loss) / 2.0
-
-
-class CLIPBaseModelOutput(ModelOutput):
-    last_hidden_state: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor]] = None
-    attentions: Optional[Tuple[torch.FloatTensor]] = None
-    qks: Optional[Tuple[torch.FloatTensor]] = None
-
-
-class CLIPBaseModelOutputWithPooling(ModelOutput):
-    last_hidden_state: torch.FloatTensor = None
-    pooler_output: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor]] = None
-    attentions: Optional[Tuple[torch.FloatTensor]] = None
-    qks: Optional[Tuple[torch.FloatTensor]] = None
-
-
-class CLIPOutput(ModelOutput):
-    """
-    Args:
-        loss (:obj:`torch.FloatTensor` of shape :obj:`(1,)`, `optional`, returned when :obj:`return_loss` is :obj:`True`):
-            Contrastive loss for image-text similarity.
-        logits_per_image:(:obj:`torch.FloatTensor` of shape :obj:`(image_batch_size, text_batch_size)`):
-            The scaled dot product scores between :obj:`image_embeds` and :obj:`text_embeds`. This represents the
-            image-text similarity scores.
-        logits_per_text:(:obj:`torch.FloatTensor` of shape :obj:`(text_batch_size, image_batch_size)`):
-            The scaled dot product scores between :obj:`text_embeds` and :obj:`image_embeds`. This represents the
-            text-image similarity scores.
-        text_embeds(:obj:`torch.FloatTensor` of shape :obj:`(batch_size, output_dim`):
-            The text embeddings obtained by applying the projection layer to the pooled output of
-            :class:`~transformers.CLIPTextModel`.
-        image_embeds(:obj:`torch.FloatTensor` of shape :obj:`(batch_size, output_dim`):
-            The image embeddings obtained by applying the projection layer to the pooled output of
-            :class:`~transformers.CLIPVisionModel`.
-        text_model_output(:obj:`BaseModelOutputWithPooling`):
-            The output of the :class:`~transformers.CLIPTextModel`.
-        vision_model_output(:obj:`BaseModelOutputWithPooling`):
-            The output of the :class:`~transformers.CLIPVisionModel`.
-    """
-
-    loss: Optional[torch.FloatTensor] = None
-    logits_per_image: torch.FloatTensor = None
-    logits_per_text: torch.FloatTensor = None
-    text_embeds: torch.FloatTensor = None
-    image_embeds: torch.FloatTensor = None
-    text_model_output: BaseModelOutputWithPooling = None
-    vision_model_output: BaseModelOutputWithPooling = None
-
-    def to_tuple(self) -> Tuple[Any]:
-        return tuple(
-            self[k] if k not in ["text_model_output", "vision_model_output"] else getattr(self, k).to_tuple()
-            for k in self.keys()
-        )
+
+# some function
+def get_extended_attention_mask(attention_mask: Tensor, input_shape: Tuple[int], device: device) -> Tensor:
+        """
+        Makes broadcastable attention and causal masks so that future and masked tokens are ignored.
+
+        Arguments:
+            attention_mask (:obj:`torch.Tensor`):
+                Mask with ones indicating tokens to attend to, zeros for tokens to ignore.
+            input_shape (:obj:`Tuple[int]`):
+                The shape of the input to the model.
+            device: (:obj:`torch.device`):
+                The device of the input to the model.
+
+        Returns:
+            :obj:`torch.Tensor` The extended attention mask, with a the same dtype as :obj:`attention_mask.dtype`.
+        """
+        # We can provide a self-attention mask of dimensions [batch_size, from_seq_length, to_seq_length]
+        # ourselves in which case we just need to make it broadcastable to all heads.
+        if attention_mask.dim() == 3:
+            extended_attention_mask = attention_mask[:, None, :, :]
+        elif attention_mask.dim() == 2:
+            # Provided a padding mask of dimensions [batch_size, seq_length]
+            # - if the model is a decoder, apply a causal mask in addition to the padding mask
+            # - if the model is an encoder, make the mask broadcastable to [batch_size, num_heads, seq_length, seq_length]
+            extended_attention_mask = attention_mask[:, None, None, :]
+        else:
+            raise ValueError(
+                f"Wrong shape for input_ids (shape {input_shape}) or attention_mask (shape {attention_mask.shape})"
+            )
+
+        # Since attention_mask is 1.0 for positions we want to attend and 0.0 for
+        # masked positions, this operation will create a tensor which is 0.0 for
+        # positions we want to attend and -10000.0 for masked positions.
+        # Since we are adding it to the raw scores before the softmax, this is
+        # effectively the same as removing these entirely.
+        extended_attention_mask = extended_attention_mask.to(dtype=torch.long)  # fp16 compatibility
+        extended_attention_mask = (1.0 - extended_attention_mask) * -10000.0
+        return extended_attention_mask
+
+
+def get_head_mask(
+        head_mask: Optional[Tensor], num_hidden_layers: int, is_attention_chunked: bool = False
+    ) -> Tensor:
+        """
+        Prepare the head mask if needed.
+
+        Args:
+            head_mask (:obj:`torch.Tensor` with shape :obj:`[num_heads]` or :obj:`[num_hidden_layers x num_heads]`, `optional`):
+                The mask indicating if we should keep the heads or not (1.0 for keep, 0.0 for discard).
+            num_hidden_layers (:obj:`int`):
+                The number of hidden layers in the model.
+            is_attention_chunked: (:obj:`bool`, `optional`, defaults to :obj:`False`):
+                Whether or not the attentions scores are computed by chunks or not.
+
+        Returns:
+            :obj:`torch.Tensor` with shape :obj:`[num_hidden_layers x batch x num_heads x seq_length x seq_length]` or
+            list with :obj:`[None]` for each layer.
+        """
+        head_mask = [None] * num_hidden_layers
+
+        return head_mask
+
+
+# models
+class IFAConfig(PretrainedConfig):
+    
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+
+class IFAPreTrainedModel(PreTrainedModel):
+    config_class = IFAConfig
+    base_model_prefix = "clip"
+    supports_gradient_checkpointing = True
+    _keys_to_ignore_on_load_missing = [r"position_ids"]
+    
+    def __init_weights(self, module):
+        pass
 
 
 class CLIPVisionEmbeddings(nn.Module):
-    def __init__(self, config: CLIPVisionConfig):
+    def __init__(self, config):
         super().__init__()
         self.config = config
         self.embed_dim = config.hidden_size
         self.image_size = config.image_size
         self.patch_size = config.patch_size
 
         self.class_embedding = nn.Parameter(torch.randn(self.embed_dim))
@@ -172,37 +142,65 @@
                 rcnn_embeds.append(rcnn_embed)
             rcnn_embeds = torch.stack(rcnn_embeds) # bsz, 12, 768
             rcnn_embeds = rcnn_embeds + self.rcnn_position_embedding(self.rcnn_position_ids)
             embeddings = torch.cat((embeddings, rcnn_embeds), dim=1)
         return embeddings
 
 
-class CLIPTextEmbeddings(nn.Module):
-    def __init__(self, config: CLIPTextConfig):
-        super().__init__()
-        embed_dim = config.hidden_size
-
-        self.token_embedding = nn.Embedding(config.vocab_size, embed_dim)
-        self.position_embedding = nn.Embedding(config.max_position_embeddings, embed_dim)
+class BertEmbeddings(nn.Module):
+    """Construct the embeddings from word, position and token_type embeddings."""
 
+    def __init__(self, config):
+        super().__init__()
+        self.word_embeddings = nn.Embedding(config.vocab_size, config.hidden_size, padding_idx=config.pad_token_id)
+        self.position_embeddings = nn.Embedding(config.max_position_embeddings, config.hidden_size)
+        self.token_type_embeddings = nn.Embedding(config.type_vocab_size, config.hidden_size)
+
+        # self.LayerNorm is not snake-cased to stick with TensorFlow model variable name and be able to load
+        # any TensorFlow checkpoint file
+        self.LayerNorm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.dropout = nn.Dropout(config.hidden_dropout_prob)
         # position_ids (1, len position emb) is contiguous in memory and exported when serialized
+        self.position_embedding_type = getattr(config, "position_embedding_type", "absolute")
         self.register_buffer("position_ids", torch.arange(config.max_position_embeddings).expand((1, -1)))
 
-    def forward(self, input_ids=None, position_ids=None, inputs_embeds=None):
-        seq_length = input_ids.shape[-1] if input_ids is not None else inputs_embeds.shape[-2]
+    def forward(
+        self, input_ids=None, token_type_ids=None, position_ids=None, inputs_embeds=None, past_key_values_length=0
+    ):
+        if input_ids is not None:
+            input_shape = input_ids.size()
+        else:
+            input_shape = inputs_embeds.size()[:-1]
+
+        seq_length = input_shape[1]
 
         if position_ids is None:
-            position_ids = self.position_ids[:, :seq_length]
+            position_ids = self.position_ids[:, past_key_values_length : seq_length + past_key_values_length]
 
-        if inputs_embeds is None:
-            inputs_embeds = self.token_embedding(input_ids)
+        # Setting the token_type_ids to the registered buffer in constructor where it is all zeros, which usually occurs
+        # when its auto-generated, registered buffer helps users when tracing the model without passing token_type_ids, solves
+        # issue #5664
+        if token_type_ids is None:
+            if hasattr(self, "token_type_ids"):
+                buffered_token_type_ids = self.token_type_ids[:, :seq_length]
+                buffered_token_type_ids_expanded = buffered_token_type_ids.expand(input_shape[0], seq_length)
+                token_type_ids = buffered_token_type_ids_expanded
+            else:
+                token_type_ids = torch.zeros(input_shape, dtype=torch.long, device=self.position_ids.device)
 
-        position_embeddings = self.position_embedding(position_ids)
-        embeddings = inputs_embeds + position_embeddings
+        if inputs_embeds is None:
+            inputs_embeds = self.word_embeddings(input_ids)
+        token_type_embeddings = self.token_type_embeddings(token_type_ids)
 
+        embeddings = inputs_embeds + token_type_embeddings
+        if self.position_embedding_type == "absolute":
+            position_embeddings = self.position_embeddings(position_ids)
+            embeddings += position_embeddings
+        embeddings = self.LayerNorm(embeddings)
+        embeddings = self.dropout(embeddings)
         return embeddings
 
 
 class CLIPAttention(nn.Module):
     """Multi-headed attention from 'Attention Is All You Need' paper"""
 
     def __init__(self, config):
@@ -224,64 +222,48 @@
 
     def _shape(self, tensor: torch.Tensor, seq_len: int, bsz: int):
         return tensor.view(bsz, seq_len, self.num_heads, self.head_dim).transpose(1, 2).contiguous()
 
     def forward(
         self,
         hidden_states: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        causal_attention_mask: Optional[torch.Tensor] = None,
         output_attentions: bool = False,
-        output_qks: bool = False,
+        past_key_values: torch.Tensor = None,
+        current_layer: int = None,
+        output_qks=None,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
         """Input shape: Batch x Time x Channel"""
 
         bsz, tgt_len, embed_dim = hidden_states.size()
 
         # get query proj
         query_states = self.q_proj(hidden_states) * self.scale
         key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
         value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+        qks = (key_states, value_states) if output_qks else None
+
+
+        if past_key_values is not None:
+            key_states = torch.cat([past_key_values[0], key_states], dim=2)
+            value_states = torch.cat([past_key_values[1], value_states], dim=2)
 
         proj_shape = (bsz * self.num_heads, -1, self.head_dim)
         query_states = self._shape(query_states, tgt_len, bsz)
 
-        qks = None
-        if output_qks:
-            qks = (query_states[:, :, 1:, :], key_states[:, :, 1:, :]) # 去掉cls
-
         query_states = query_states.view(*proj_shape)
         key_states = key_states.view(*proj_shape)
         value_states = value_states.view(*proj_shape)
         
         src_len = key_states.size(1)
         attn_weights = torch.bmm(query_states, key_states.transpose(1, 2))
 
         if attn_weights.size() != (bsz * self.num_heads, tgt_len, src_len):
             raise ValueError(
                 f"Attention weights should be of size {(bsz * self.num_heads, tgt_len, src_len)}, but is {attn_weights.size()}"
-            )
-
-        # apply the causal_attention_mask first
-        if causal_attention_mask is not None:
-            if causal_attention_mask.size() != (bsz, 1, tgt_len, src_len):
-                raise ValueError(
-                    f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {causal_attention_mask.size()}"
-                )
-            attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len) + causal_attention_mask
-            attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
-
-        if attention_mask is not None:
-            if attention_mask.size() != (bsz, 1, tgt_len, src_len):
-                raise ValueError(
-                    f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {attention_mask.size()}"
-                )
-            attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len) + attention_mask
-            attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
-
+            )       
         attn_weights = nn.functional.softmax(attn_weights, dim=-1)
 
         if output_attentions:
             # this operation is a bit akward, but it's required to
             # make sure that attn_weights keeps its gradient.
             # In order to do so, attn_weights have to reshaped
             # twice and have to be reused in the following
@@ -301,16 +283,15 @@
 
         attn_output = attn_output.view(bsz, self.num_heads, tgt_len, self.head_dim)
         attn_output = attn_output.transpose(1, 2)
         attn_output = attn_output.reshape(bsz, tgt_len, embed_dim)
 
         attn_output = self.out_proj(attn_output)
 
-        # return attn_output, attn_weights_reshaped
-        return attn_output, attn_output, qks
+        return attn_output, attn_weights_reshaped, qks
 
 def quick_gelu(x):
     return x * torch.sigmoid(1.702 * x)
 
 class CLIPMLP(nn.Module):
     def __init__(self, config):
         super().__init__()
@@ -322,30 +303,178 @@
     def forward(self, hidden_states):
         hidden_states = self.fc1(hidden_states)
         hidden_states = self.activation_fn(hidden_states)
         hidden_states = self.fc2(hidden_states)
         return hidden_states
 
 
+class BertSelfAttention(nn.Module):
+    def __init__(self, config):
+        super().__init__()
+        self.num_attention_heads = config.num_attention_heads   # 12
+        self.attention_head_size = int(config.hidden_size / config.num_attention_heads) # 64
+        self.all_head_size = self.num_attention_heads * self.attention_head_size    # 768
+
+        self.query = nn.Linear(config.hidden_size, self.all_head_size)
+        self.key = nn.Linear(config.hidden_size, self.all_head_size)
+        self.value = nn.Linear(config.hidden_size, self.all_head_size)
+
+        self.dropout = nn.Dropout(config.attention_probs_dropout_prob)
+
+    def transpose_for_scores(self, x):
+        new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
+        x = x.view(*new_x_shape)
+        return x.permute(0, 2, 1, 3)
+
+    def forward(
+        self,
+        hidden_states,
+        attention_mask=None,
+        head_mask=None,
+        output_attentions=False,
+        visual_hidden_state=None,
+        output_qks=None,
+        current_layer=None,
+        past_key_values=None,
+    ):
+        mixed_query_layer = self.query(hidden_states)
+
+        # If this is instantiated as a cross-attention module, the keys
+        # and values come from an encoder; the attention mask needs to be
+        # such that the encoder's padding tokens are not attended to.
+        key_layer = self.transpose_for_scores(self.key(hidden_states))
+        value_layer = self.transpose_for_scores(self.value(hidden_states))
+        query_layer = self.transpose_for_scores(mixed_query_layer)
+
+        qks = (key_layer, value_layer) if output_qks else None
+
+        if past_key_values is not None:
+            key_layer = torch.cat([past_key_values[0], key_layer], dim=2)
+            value_layer = torch.cat([past_key_values[0], value_layer], dim=2)
+        # Take the dot product between "query" and "key" to get the raw attention scores.
+        attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
+        attention_scores = attention_scores / math.sqrt(self.attention_head_size)
+        if attention_mask is not None:
+            # Apply the attention mask is (precomputed for all layers in BertModel forward() function)
+            bsz, nheads, length, dsize = past_key_values[0].size()
+            visual_attention_mask = torch.ones((bsz, 1, 1, length)).to(attention_mask.device)  # bsz, 12, len, 64
+            attention_mask = torch.cat((visual_attention_mask, attention_mask), dim=-1)
+            attention_scores = attention_scores + attention_mask
+        # Normalize the attention scores to probabilities.
+        attention_probs = nn.Softmax(dim=-1)(attention_scores)
+
+        # This is actually dropping out entire tokens to attend to, which might
+        # seem a bit unusual, but is taken from the original Transformer paper.
+        attention_probs = self.dropout(attention_probs)
+
+        # Mask heads if we want to
+        if head_mask is not None:
+            attention_probs = attention_probs * head_mask
+        context_layer = torch.matmul(attention_probs, value_layer)
+
+        context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
+        new_context_layer_shape = context_layer.size()[:-2] + (self.all_head_size,)
+        context_layer = context_layer.view(*new_context_layer_shape)    # bsz, 128, 768
+        
+        outputs = (context_layer, attention_probs) if output_attentions else (context_layer,)
+
+        return outputs, qks
+
+
+class BertSelfOutput(nn.Module):
+    def __init__(self, config):
+        super().__init__()
+        self.dense = nn.Linear(config.hidden_size, config.hidden_size)
+        self.LayerNorm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.dropout = nn.Dropout(config.hidden_dropout_prob)
+
+    def forward(self, hidden_states, input_tensor):
+        hidden_states = self.dense(hidden_states)
+        hidden_states = self.dropout(hidden_states)
+        hidden_states = self.LayerNorm(hidden_states + input_tensor)
+        return hidden_states
+
+class BertAttention(nn.Module):
+    def __init__(self, config):
+        super().__init__()
+        self.self = BertSelfAttention(config)
+        self.output = BertSelfOutput(config)
+        self.pruned_heads = set()
+
+    def forward(
+        self,
+        hidden_states,
+        attention_mask=None,
+        head_mask=None,
+        output_attentions=False,
+        visual_hidden_state=None,
+        output_qks=None,
+        current_layer=None,
+        past_key_values=None,
+    ):
+        self_outputs, qks = self.self(
+            hidden_states,
+            attention_mask,
+            head_mask,
+            output_attentions,
+            visual_hidden_state,
+            output_qks,
+            current_layer,
+            past_key_values,
+        )
+        attention_output = self.output(self_outputs[0], hidden_states)
+        outputs = (attention_output,) + self_outputs[1:]  # add attentions if we output them
+        return outputs, qks
+
+
+class BertIntermediate(nn.Module):
+    def __init__(self, config):
+        super().__init__()
+        self.dense = nn.Linear(config.hidden_size, config.intermediate_size)
+        if isinstance(config.hidden_act, str):
+            self.intermediate_act_fn = ACT2FN[config.hidden_act]
+        else:
+            self.intermediate_act_fn = config.hidden_act
+
+    def forward(self, hidden_states):
+        hidden_states = self.dense(hidden_states)
+        hidden_states = self.intermediate_act_fn(hidden_states)
+        return hidden_states
+
+
+class BertOutput(nn.Module):
+    def __init__(self, config):
+        super().__init__()
+        self.dense = nn.Linear(config.intermediate_size, config.hidden_size)
+        self.LayerNorm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
+        self.dropout = nn.Dropout(config.hidden_dropout_prob)
+
+    def forward(self, hidden_states, input_tensor):
+        hidden_states = self.dense(hidden_states)
+        hidden_states = self.dropout(hidden_states)
+        hidden_states = self.LayerNorm(hidden_states + input_tensor)
+        return hidden_states
+
+
 class CLIPEncoderLayer(nn.Module):
-    def __init__(self, config: CLIPConfig):
+    def __init__(self, config):
         super().__init__()
         self.embed_dim = config.hidden_size
         self.self_attn = CLIPAttention(config)
         self.layer_norm1 = nn.LayerNorm(self.embed_dim)
         self.mlp = CLIPMLP(config)
         self.layer_norm2 = nn.LayerNorm(self.embed_dim)
 
     def forward(
         self,
         hidden_states: torch.Tensor,
-        attention_mask: torch.Tensor,
-        causal_attention_mask: torch.Tensor,
         output_attentions: bool = False,
-        output_qks: bool = False,
+        past_key_values: torch.Tensor = None,
+        current_layer: int = None,
+        output_qks = None
     ):
         """
         Args:
             hidden_states (:obj:`torch.FloatTensor`): input to the layer of shape :obj:`(seq_len, batch, embed_dim)`
             attention_mask (:obj:`torch.FloatTensor`): attention mask of size
                 :obj:`(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
             layer_head_mask (:obj:`torch.FloatTensor`): mask for attention heads in a given layer of size
@@ -355,736 +484,346 @@
                 returned tensors for more detail.
         """
         residual = hidden_states
 
         hidden_states = self.layer_norm1(hidden_states)
         hidden_states, attn_weights, qks = self.self_attn(
             hidden_states=hidden_states,
-            attention_mask=attention_mask,
-            causal_attention_mask=causal_attention_mask,
             output_attentions=output_attentions,
+            past_key_values=past_key_values,
             output_qks=output_qks,
+            current_layer=current_layer,
         )
         hidden_states = residual + hidden_states
 
         residual = hidden_states
         hidden_states = self.layer_norm2(hidden_states)
         hidden_states = self.mlp(hidden_states)
         hidden_states = residual + hidden_states
 
         outputs = (hidden_states,)
 
         if output_attentions:
             outputs += (attn_weights,)
         
         if output_qks:
-            outputs += (qks,)
-
+            outputs += (qks, )
+    
         return outputs
 
 
-class CLIPPreTrainedModel(PreTrainedModel):
-    """
-    An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
-    models.
-    """
-
-    config_class = CLIPConfig
-    base_model_prefix = "clip"
-    supports_gradient_checkpointing = True
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
-    def _init_weights(self, module):
-        """Initialize the weights"""
-        factor = self.config.initializer_factor
-        if isinstance(module, CLIPTextEmbeddings):
-            module.token_embedding.weight.data.normal_(mean=0.0, std=factor * 0.02)
-            module.position_embedding.weight.data.normal_(mean=0.0, std=factor * 0.02)
-        elif isinstance(module, CLIPVisionEmbeddings):
-            factor = self.config.initializer_factor
-            nn.init.normal_(module.class_embedding, mean=0.0, std=module.embed_dim ** -0.5 * factor)
-            nn.init.normal_(module.patch_embedding.weight, std=module.config.initializer_range * factor)
-            nn.init.normal_(module.position_embedding.weight, std=module.config.initializer_range * factor)
-        elif isinstance(module, CLIPAttention):
-            factor = self.config.initializer_factor
-            in_proj_std = (module.embed_dim ** -0.5) * ((2 * module.config.num_hidden_layers) ** -0.5) * factor
-            out_proj_std = (module.embed_dim ** -0.5) * factor
-            nn.init.normal_(module.q_proj.weight, std=in_proj_std)
-            nn.init.normal_(module.k_proj.weight, std=in_proj_std)
-            nn.init.normal_(module.v_proj.weight, std=in_proj_std)
-            nn.init.normal_(module.out_proj.weight, std=out_proj_std)
-        elif isinstance(module, CLIPMLP):
-            factor = self.config.initializer_factor
-            in_proj_std = (
-                (module.config.hidden_size ** -0.5) * ((2 * module.config.num_hidden_layers) ** -0.5) * factor
-            )
-            fc_std = (2 * module.config.hidden_size) ** -0.5 * factor
-            nn.init.normal_(module.fc1.weight, std=fc_std)
-            nn.init.normal_(module.fc2.weight, std=in_proj_std)
-        elif isinstance(module, CLIPModel):
-            nn.init.normal_(
-                module.text_projection.weight,
-                std=module.text_embed_dim ** -0.5 * self.config.initializer_factor,
-            )
-            nn.init.normal_(
-                module.visual_projection.weight,
-                std=module.vision_embed_dim ** -0.5 * self.config.initializer_factor,
-            )
-
-        if isinstance(module, nn.LayerNorm):
-            module.bias.data.zero_()
-            module.weight.data.fill_(1.0)
-        if isinstance(module, nn.Linear) and module.bias is not None:
-            module.bias.data.zero_()
-
-    def _set_gradient_checkpointing(self, module, value=False):
-        if isinstance(module, CLIPEncoder):
-            module.gradient_checkpointing = value
-
-
-CLIP_START_DOCSTRING = r"""
-    This model is a PyTorch `torch.nn.Module <https://pytorch.org/docs/stable/nn.html#torch.nn.Module>`_ subclass. Use
-    it as a regular PyTorch Module and refer to the PyTorch documentation for all matter related to general usage and
-    behavior.
-
-    Parameters:
-        config (:class:`~transformers.CLIPConfig`): Model configuration class with all the parameters of the model.
-            Initializing with a config file does not load the weights associated with the model, only the
-            configuration. Check out the :meth:`~transformers.PreTrainedModel.from_pretrained` method to load the model
-            weights.
-"""
-
-CLIP_TEXT_INPUTS_DOCSTRING = r"""
-    Args:
-        input_ids (:obj:`torch.LongTensor` of shape :obj:`(batch_size, sequence_length)`):
-            Indices of input sequence tokens in the vocabulary. Padding will be ignored by default should you provide
-            it.
-
-            Indices can be obtained using :class:`~transformers.CLIPTokenizer`. See
-            :meth:`transformers.PreTrainedTokenizer.encode` and :meth:`transformers.PreTrainedTokenizer.__call__` for
-            details.
-
-            `What are input IDs? <../glossary.html#input-ids>`__
-        attention_mask (:obj:`torch.Tensor` of shape :obj:`(batch_size, sequence_length)`, `optional`):
-            Mask to avoid performing attention on padding token indices. Mask values selected in ``[0, 1]``:
-
-            - 1 for tokens that are **not masked**,
-            - 0 for tokens that are **masked**.
-
-            `What are attention masks? <../glossary.html#attention-mask>`__
-        position_ids (:obj:`torch.LongTensor` of shape :obj:`(batch_size, sequence_length)`, `optional`):
-            Indices of positions of each input sequence tokens in the position embeddings. Selected in the range ``[0,
-            config.max_position_embeddings - 1]``.
-
-            `What are position IDs? <../glossary.html#position-ids>`_
-        output_attentions (:obj:`bool`, `optional`):
-            Whether or not to return the attentions tensors of all attention layers. See ``attentions`` under returned
-            tensors for more detail.
-        output_hidden_states (:obj:`bool`, `optional`):
-            Whether or not to return the hidden states of all layers. See ``hidden_states`` under returned tensors for
-            more detail.
-        return_dict (:obj:`bool`, `optional`):
-            Whether or not to return a :class:`~transformers.file_utils.ModelOutput` instead of a plain tuple.
-"""
-
-CLIP_VISION_INPUTS_DOCSTRING = r"""
-    Args:
-        pixel_values (:obj:`torch.FloatTensor` of shape :obj:`(batch_size, num_channels, height, width)`):
-            Pixel values. Padding will be ignored by default should you provide it. Pixel values can be obtained using
-            :class:`~transformers.CLIPFeatureExtractor`. See :meth:`transformers.CLIPFeatureExtractor.__call__` for
-            details.
-        output_attentions (:obj:`bool`, `optional`):
-            Whether or not to return the attentions tensors of all attention layers. See ``attentions`` under returned
-            tensors for more detail.
-        output_hidden_states (:obj:`bool`, `optional`):
-            Whether or not to return the hidden states of all layers. See ``hidden_states`` under returned tensors for
-            more detail.
-        return_dict (:obj:`bool`, `optional`):
-            Whether or not to return a :class:`~transformers.file_utils.ModelOutput` instead of a plain tuple.
-"""
-
-CLIP_INPUTS_DOCSTRING = r"""
-    Args:
-        input_ids (:obj:`torch.LongTensor` of shape :obj:`(batch_size, sequence_length)`):
-            Indices of input sequence tokens in the vocabulary. Padding will be ignored by default should you provide
-            it.
-
-            Indices can be obtained using :class:`~transformers.CLIPTokenizer`. See
-            :meth:`transformers.PreTrainedTokenizer.encode` and :meth:`transformers.PreTrainedTokenizer.__call__` for
-            details.
-
-            `What are input IDs? <../glossary.html#input-ids>`__
-        attention_mask (:obj:`torch.Tensor` of shape :obj:`(batch_size, sequence_length)`, `optional`):
-            Mask to avoid performing attention on padding token indices. Mask values selected in ``[0, 1]``:
-
-            - 1 for tokens that are **not masked**,
-            - 0 for tokens that are **masked**.
-
-            `What are attention masks? <../glossary.html#attention-mask>`__
-        position_ids (:obj:`torch.LongTensor` of shape :obj:`(batch_size, sequence_length)`, `optional`):
-            Indices of positions of each input sequence tokens in the position embeddings. Selected in the range ``[0,
-            config.max_position_embeddings - 1]``.
-
-            `What are position IDs? <../glossary.html#position-ids>`_
-        pixel_values (:obj:`torch.FloatTensor` of shape :obj:`(batch_size, num_channels, height, width)`):
-            Pixel values. Padding will be ignored by default should you provide it. Pixel values can be obtained using
-            :class:`~transformers.CLIPFeatureExtractor`. See :meth:`transformers.CLIPFeatureExtractor.__call__` for
-            details.
-        return_loss (:obj:`bool`, `optional`):
-            Whether or not to return the contrastive loss.
-        output_attentions (:obj:`bool`, `optional`):
-            Whether or not to return the attentions tensors of all attention layers. See ``attentions`` under returned
-            tensors for more detail.
-        output_hidden_states (:obj:`bool`, `optional`):
-            Whether or not to return the hidden states of all layers. See ``hidden_states`` under returned tensors for
-            more detail.
-        return_dict (:obj:`bool`, `optional`):
-            Whether or not to return a :class:`~transformers.file_utils.ModelOutput` instead of a plain tuple.
-"""
-
-
-class CLIPEncoder(nn.Module):
-    """
-    Transformer encoder consisting of :obj:`config.num_hidden_layers` self attention layers. Each layer is a
-    :class:`~transformers.CLIPEncoderLayer`.
-
-    Args:
-        config: CLIPConfig
-        embed_tokens (nn.Embedding): output embedding
-    """
-
-    def __init__(self, config: CLIPConfig):
+class BertLayer(nn.Module):
+    def __init__(self, config):
         super().__init__()
-        self.config = config
-        self.layers = nn.ModuleList([CLIPEncoderLayer(config) for _ in range(config.num_hidden_layers)])
-        self.gradient_checkpointing = False
+        self.chunk_size_feed_forward = config.chunk_size_feed_forward
+        self.seq_len_dim = 1
+        self.attention = BertAttention(config)
+        self.add_cross_attention = config.add_cross_attention
+        self.intermediate = BertIntermediate(config)
+        self.output = BertOutput(config)
 
     def forward(
         self,
-        inputs_embeds,
+        hidden_states,
         attention_mask=None,
-        causal_attention_mask=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-        output_qks=False,
+        head_mask=None,
+        output_attentions=False,
+        visual_hidden_state=None,
+        output_qks=None,
+        current_layer=None,
+        past_key_values=None,
     ):
-        r"""
-        Args:
-            inputs_embeds (:obj:`torch.FloatTensor` of shape :obj:`(batch_size, sequence_length, hidden_size)`, `optional`):
-                Optionally, instead of passing :obj:`input_ids` you can choose to directly pass an embedded
-                representation. This is useful if you want more control over how to convert :obj:`input_ids` indices
-                into associated vectors than the model's internal embedding lookup matrix.
-            attention_mask (:obj:`torch.Tensor` of shape :obj:`(batch_size, sequence_length)`, `optional`):
-                Mask to avoid performing attention on padding token indices. Mask values selected in ``[0, 1]``:
-
-                - 1 for tokens that are **not masked**,
-                - 0 for tokens that are **masked**.
-
-                `What are attention masks? <../glossary.html#attention-mask>`__
-            causal_attention_mask (:obj:`torch.Tensor` of shape :obj:`(batch_size, sequence_length)`, `optional`):
-                Causal mask for the text model. Mask values selected in ``[0, 1]``:
-
-                - 1 for tokens that are **not masked**,
-                - 0 for tokens that are **masked**.
-
-                `What are attention masks? <../glossary.html#attention-mask>`__
-            output_attentions (:obj:`bool`, `optional`):
-                Whether or not to return the attentions tensors of all attention layers. See ``attentions`` under
-                returned tensors for more detail.
-            output_hidden_states (:obj:`bool`, `optional`):
-                Whether or not to return the hidden states of all layers. See ``hidden_states`` under returned tensors
-                for more detail.
-            return_dict (:obj:`bool`, `optional`):
-                Whether or not to return a :class:`~transformers.file_utils.ModelOutput` instead of a plain tuple.
-        """
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+        # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
+        # self_attn_past_key_value = past_key_value[:2] if past_key_value is not None else None
+        self_attention_outputs, qks = self.attention(
+            hidden_states,
+            attention_mask,
+            head_mask,
+            output_attentions=output_attentions,
+            visual_hidden_state=visual_hidden_state,
+            output_qks=output_qks,
+            current_layer=current_layer,
+            past_key_values=past_key_values,
         )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        encoder_states = () if output_hidden_states else None
-        all_attentions = () if output_attentions else None
-        all_qks = ()        if output_qks else None
-
-        hidden_states = inputs_embeds
-        for idx, encoder_layer in enumerate(self.layers):
-            if output_hidden_states:
-                encoder_states = encoder_states + (hidden_states,)
-            if self.gradient_checkpointing and self.training:
-
-                def create_custom_forward(module):
-                    def custom_forward(*inputs):
-                        return module(*inputs, output_attentions)
-
-                    return custom_forward
-
-                layer_outputs = torch.utils.checkpoint.checkpoint(
-                    create_custom_forward(encoder_layer),
-                    hidden_states,
-                    attention_mask,
-                    causal_attention_mask,
-                )
-            else:
-                layer_outputs = encoder_layer(
-                    hidden_states,
-                    attention_mask,
-                    causal_attention_mask,
-                    output_attentions=output_attentions,
-                    output_qks=output_qks
-                )
+        attention_output = self_attention_outputs[0]
 
-                hidden_states = layer_outputs[0]
+        outputs = self_attention_outputs[1:]  # add self attentions if we output attention weights
 
-            if output_attentions:
-                all_attentions = all_attentions + (layer_outputs[1],)
-            if output_qks:
-                all_qks = all_qks + (layer_outputs[2],)
+        layer_output = apply_chunking_to_forward(
+            self.feed_forward_chunk, self.chunk_size_feed_forward, self.seq_len_dim, attention_output
+        )
+        outputs = (layer_output,) + outputs
+        if output_qks: 
+            outputs += (qks,)
 
-        if output_hidden_states:
-            encoder_states = encoder_states + (hidden_states,)
+        return outputs
 
-        if not return_dict:
-            return tuple(v for v in [hidden_states, encoder_states, all_attentions] if v is not None)
-        return CLIPBaseModelOutput(
-            last_hidden_state=hidden_states, hidden_states=encoder_states, attentions=all_attentions, qks=all_qks
-        )
+    def feed_forward_chunk(self, attention_output):
+        intermediate_output = self.intermediate(attention_output)
+        layer_output = self.output(intermediate_output, attention_output)
+        return layer_output
 
 
-class CLIPTextTransformer(nn.Module):
-    def __init__(self, config: CLIPTextConfig):
+class IFAEncoder(nn.Module):
+    def __init__(self, vision_config, text_config):
         super().__init__()
-        self.config = config
-        embed_dim = config.hidden_size
-        self.embeddings = CLIPTextEmbeddings(config)
-        self.encoder = CLIPEncoder(config)
-        self.final_layer_norm = nn.LayerNorm(embed_dim)
+        self.vision_config = vision_config
+        self.text_config = text_config
 
-    @replace_return_docstrings(output_type=BaseModelOutputWithPooling, config_class=CLIPTextConfig)
+        self.vision_layers = nn.ModuleList([CLIPEncoderLayer(vision_config) for _ in range(vision_config.num_hidden_layers)])
+        self.text_layer = nn.ModuleList([BertLayer(text_config) for _ in range(text_config.num_hidden_layers)])
+    
     def forward(
         self,
-        input_ids=None,
+        vision_embeds=None,
+        text_embeds=None,
         attention_mask=None,
-        position_ids=None,
+        head_mask=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
     ):
-        r"""
-        Returns:
+        assert self.vision_config.num_hidden_layers == self.text_config.num_hidden_layers
 
-        """
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        if input_ids is None:
-            raise ValueError("You have to specify either input_ids")
-
-        input_shape = input_ids.size()
-        input_ids = input_ids.view(-1, input_shape[-1])
-
-        hidden_states = self.embeddings(input_ids=input_ids, position_ids=position_ids)
+        all_vision_hidden_states = () if output_hidden_states else None
+        all_text_hidden_states = () if output_hidden_states else None
+        all_vision_attentions = () if output_attentions else None
+        all_text_attentions = () if output_attentions else None
+        
+        vision_hidden_states = vision_embeds
+        text_hidden_states = text_embeds
+        for idx in range(self.vision_config.num_hidden_layers):
+            if output_hidden_states:
+                all_vision_hidden_states = all_vision_hidden_states + (vision_hidden_states, )
+                all_text_hidden_states = all_text_hidden_states + (text_hidden_states, )
+            
+            # vision
+            # TODO: 9-12 layers past text as pkv to vision
+            output_qks = True
+            if idx == 0:
+                bsz, length, dsize = text_embeds.size()
+                visual_past_key_values = (text_embeds.view(bsz, 12, length, dsize//12),
+                                          text_embeds.view(bsz, 12, length, dsize//12))
+            else:
+                visual_past_key_values = text_layer_output[-1]
+            vision_layer_module = self.vision_layers[idx]
+            vision_layer_output = vision_layer_module(
+                    vision_hidden_states,
+                    output_attentions=output_attentions,
+                    past_key_values=visual_past_key_values,
+                    current_layer=idx,
+                    output_qks=output_qks,
+            )
+            vision_hidden_states = vision_layer_output[0]
 
-        bsz, seq_len = input_shape
-        # CLIP's text model uses causal mask, prepare it here.
-        # https://github.com/openai/CLIP/blob/cfcffb90e69f37bf2ff1e988237a0fbe41f33c04/clip/model.py#L324
-        causal_attention_mask = self._build_causal_attention_mask(bsz, seq_len).to(hidden_states.device)
-        # expand attention_mask
-        if attention_mask is not None:
-            # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
-            attention_mask = _expand_mask(attention_mask, hidden_states.dtype)
+            # text
+            # TODO: 9-12 layers past vison qks to text
+            if idx == 0:
+                bsz, length, dsize = vision_embeds.size()
+                text_past_key_values = (vision_embeds.view(bsz, 12, length, dsize//12),
+                                          vision_embeds.view(bsz, 12, length, dsize//12))
+            else:
+                text_past_key_values = vision_layer_output[-1]
 
-        encoder_outputs = self.encoder(
-            inputs_embeds=hidden_states,
-            attention_mask=attention_mask,
-            causal_attention_mask=causal_attention_mask,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
+            layer_head_mask = head_mask[idx] if head_mask is not None else None
+            text_layer_module = self.text_layer[idx]
+            text_layer_output = text_layer_module(
+                    text_hidden_states,
+                    attention_mask=attention_mask,
+                    head_mask=layer_head_mask,
+                    visual_hidden_state=None,
+                    past_key_values=text_past_key_values,
+                    output_attentions=output_attentions,
+                    output_qks=output_qks,
+                    current_layer=idx,
+            )
+            text_hidden_states = text_layer_output[0]
+            if output_attentions:
+                all_vision_attentions = all_vision_attentions + (vision_layer_output[1], )
+                all_text_attentions = all_text_attentions + (text_layer_output[1], )
+        
+        if output_hidden_states:
+                all_vision_hidden_states = all_vision_hidden_states + (vision_hidden_states, )
+                all_text_hidden_states = all_text_hidden_states + (text_hidden_states, )
+        
+        if not return_dict:
+            return tuple(
+                v for v in [
+                    text_hidden_states,
+                    all_text_hidden_states,
+                    all_text_attentions,
+                ] if v is not None)
+        return BaseModelOutput(
+            last_hidden_state=text_hidden_states, hidden_states=all_text_hidden_states, attentions=all_text_attentions
         )
 
-        last_hidden_state = encoder_outputs[0]
-        last_hidden_state = self.final_layer_norm(last_hidden_state)
-
-        # text_embeds.shape = [batch_size, n_ctx, transformer.width]
-        # take features from the eot embedding (eot_token is the highest number in each sequence)
-        pooled_output = last_hidden_state[torch.arange(last_hidden_state.shape[0]), input_ids.argmax(dim=-1)]
-
-        if not return_dict:
-            return (last_hidden_state, pooled_output) + encoder_outputs[1:]
 
-        return BaseModelOutputWithPooling(
-            last_hidden_state=last_hidden_state,
-            pooler_output=pooled_output,
-            hidden_states=encoder_outputs.hidden_states,
-            attentions=encoder_outputs.attentions,
-        )
+class BertPooler(nn.Module):
+    def __init__(self, config):
+        super().__init__()
+        self.dense = nn.Linear(config.hidden_size, config.hidden_size)
+        self.activation = nn.Tanh()
 
-    def _build_causal_attention_mask(self, bsz, seq_len):
-        # lazily create causal attention mask, with full attention between the vision tokens
-        # pytorch uses additive attention mask; fill with -inf
-        mask = torch.empty(bsz, seq_len, seq_len)
-        mask.fill_(float("-inf"))
-        mask.triu_(1)  # zero out the lower diagonal
-        mask = mask.unsqueeze(1)  # expand mask
-        return mask
-
-
-class CLIPTextModel(CLIPPreTrainedModel):
-    config_class = CLIPTextConfig
-
-    def __init__(self, config: CLIPTextConfig):
-        super().__init__(config)
-        self.text_model = CLIPTextTransformer(config)
-        self.init_weights()
+    def forward(self, hidden_states):
+        # We "pool" the model by simply taking the hidden state corresponding
+        # to the first token.
+        first_token_tensor = hidden_states[:, 0]
+        pooled_output = self.dense(first_token_tensor)
+        pooled_output = self.activation(pooled_output)
+        return pooled_output
+
+
+class IFAModel(nn.Module):
+    def __init__(self, vision_config, text_config, add_pooling_layer=True):
+        super(IFAModel, self).__init__()
+        # vision model
+        self.vision_config = vision_config
+        self.vision_embeddings = CLIPVisionEmbeddings(vision_config)
+        self.vision_pre_layrnorm = nn.LayerNorm(vision_config.hidden_size)
+        self.vision_post_layernorm = nn.LayerNorm(vision_config.hidden_size)
+
+        # text model
+        self.text_config = text_config
+        self.text_embeddings = BertEmbeddings(text_config)
+        self.text_pooler = BertPooler(text_config) if add_pooling_layer else None
 
-    def get_input_embeddings(self) -> nn.Module:
-        return self.text_model.embeddings.token_embedding
+        # all
+        self.encoder = IFAEncoder(vision_config, text_config)
 
-    def set_input_embeddings(self, value):
-        self.text_model.embeddings.token_embedding = value
+        self.device = vision_config.device
 
-    @replace_return_docstrings(output_type=BaseModelOutputWithPooling, config_class=CLIPTextConfig)
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
+        token_type_ids=None,
         position_ids=None,
+        head_mask=None,
+        
+        pixel_values=None,
+        aux_values=None, 
+        rcnn_values=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
-        output_qks=False,
     ):
-        r"""
-        Returns:
-
-        Examples::
-
-            >>> from transformers import CLIPTokenizer, CLIPTextModel
+        # pre vision
+        vision_embedding_output = self.vision_embeddings(pixel_values, aux_values, rcnn_values)
+        vision_embedding_output = self.vision_pre_layrnorm(vision_embedding_output)
 
-            >>> model = CLIPTextModel.from_pretrained("openai/clip-vit-base-patch32")
-            >>> tokenizer = CLIPTokenizer.from_pretrained("openai/clip-vit-base-patch32")
+        # pre text
+        input_shape = input_ids.size()
+        batch_size, seq_length = input_shape
+        device = input_ids.device
+        if attention_mask is None:
+            attention_mask = torch.ones(((batch_size, seq_length)), device=device)
+        if token_type_ids is None:
+            raise ValueError("token_type_ids is None!")
 
-            >>> inputs = tokenizer(["a photo of a cat", "a photo of a dog"],  padding=True, return_tensors="pt")
+        extended_attention_mask: torch.Tensor = get_extended_attention_mask(attention_mask, input_shape, device)
+        head_mask = get_head_mask(head_mask, self.text_config.num_hidden_layers)    # [None]*12
 
-            >>> outputs = model(**inputs)
-            >>> last_hidden_state = outputs.last_hidden_state
-            >>> pooled_output = outputs.pooled_output # pooled (EOS token) states
-        """
-        return self.text_model(
+        text_embedding_output = self.text_embeddings(
             input_ids=input_ids,
-            attention_mask=attention_mask,
             position_ids=position_ids,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
-            output_qks=output_qks
-        )
-
-
-class CLIPVisionTransformer(nn.Module):
-    def __init__(self, config: CLIPVisionConfig):
-        super().__init__()
-        self.config = config
-        embed_dim = config.hidden_size
-
-        self.embeddings = CLIPVisionEmbeddings(config)
-        self.pre_layrnorm = nn.LayerNorm(embed_dim)
-        self.encoder = CLIPEncoder(config)
-        self.post_layernorm = nn.LayerNorm(embed_dim)
-
-    @replace_return_docstrings(output_type=BaseModelOutputWithPooling, config_class=CLIPVisionConfig)
-    def forward(
-        self,
-        pixel_values=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-        aux_embeddings=None,
-        rcnn_embeddings=None,
-        output_qks=False,
-    ):
-        r"""
-        Returns:
-
-        """
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+            token_type_ids=token_type_ids,
         )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        if pixel_values is None:
-            raise ValueError("You have to specify pixel_values")
-
-        hidden_states = self.embeddings(pixel_values, aux_embeddings, rcnn_embeddings)
-        hidden_states = self.pre_layrnorm(hidden_states)
 
+        # all encoder
         encoder_outputs = self.encoder(
-            inputs_embeds=hidden_states,
+            vision_embeds=vision_embedding_output,
+            text_embeds=text_embedding_output,
+            attention_mask=extended_attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
-            output_qks=output_qks
         )
-
-        last_hidden_state = encoder_outputs[0]
-        pooled_output = last_hidden_state[:, 0, :]
-        pooled_output = self.post_layernorm(pooled_output)
+        sequence_output = encoder_outputs[0]
+        pooled_output = self.text_pooler(sequence_output) if self.text_pooler is not None else None
 
         if not return_dict:
-            return (last_hidden_state, pooled_output) + encoder_outputs[1:]
-        return CLIPBaseModelOutputWithPooling(
-            last_hidden_state=last_hidden_state,
+            return (sequence_output, pooled_output) + encoder_outputs[1:]
+
+        return BaseModelOutputWithPooling(
+            last_hidden_state=sequence_output,
             pooler_output=pooled_output,
             hidden_states=encoder_outputs.hidden_states,
             attentions=encoder_outputs.attentions,
-            qks=encoder_outputs.qks
-        )
-
-
-class CLIPVisionModel(CLIPPreTrainedModel):
-    config_class = CLIPVisionConfig
-
-    def __init__(self, config: CLIPVisionConfig):
-        super().__init__(config)
-        self.vision_model = CLIPVisionTransformer(config)
-        self.init_weights()
-
-    def get_input_embeddings(self) -> nn.Module:
-        return self.vision_model.embeddings.patch_embedding
-
-    @replace_return_docstrings(output_type=BaseModelOutputWithPooling, config_class=CLIPVisionConfig)
-    def forward(
-        self,
-        pixel_values=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        r"""
-        Returns:
-
-        Examples::
-
-            >>> from PIL import Image
-            >>> import requests
-            >>> from transformers import CLIPProcessor, CLIPVisionModel
-
-            >>> model = CLIPVisionModel.from_pretrained("openai/clip-vit-base-patch32")
-            >>> processor = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
-
-            >>> url = "http://images.cocodataset.org/val2017/000000039769.jpg"
-            >>> image = Image.open(requests.get(url, stream=True).raw)
-
-            >>> inputs = processor(images=image, return_tensors="pt")
-
-            >>> outputs = model(**inputs)
-            >>> last_hidden_state = outputs.last_hidden_state
-            >>> pooled_output = outputs.pooled_output # pooled CLS states
-        """
-        return self.vision_model(
-            pixel_values=pixel_values,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
         )
 
+    def _init_text_weights(self, module):
+        """Initialize the weights"""
+        if isinstance(module, nn.Linear):
+            # Slightly different from the TF version which uses truncated_normal for initialization
+            # cf https://github.com/pytorch/pytorch/pull/5617
+            module.weight.data.normal_(mean=0.0, std=self.text_config.initializer_range)
+            if module.bias is not None:
+                module.bias.data.zero_()
+        elif isinstance(module, nn.Embedding):
+            module.weight.data.normal_(mean=0.0, std=self.text_config.initializer_range)
+            if module.padding_idx is not None:
+                module.weight.data[module.padding_idx].zero_()
+        elif isinstance(module, nn.LayerNorm):
+            module.bias.data.zero_()
+            module.weight.data.fill_(1.0)
 
-@add_start_docstrings(CLIP_START_DOCSTRING)
-class CLIPModel(CLIPPreTrainedModel):
-    config_class = CLIPConfig
-
-    def __init__(self, config: CLIPConfig):
-        super().__init__(config)
-
-        if not isinstance(config.text_config, CLIPTextConfig):
-            raise ValueError(
-                f"config.text_config is expected to be of type CLIPTextConfig but is of type {type(config.text_config)}."
-            )
-
-        if not isinstance(config.vision_config, CLIPVisionConfig):
-            raise ValueError(
-                f"config.vision_config is expected to be of type CLIPVisionConfig but is of type {type(config.vision_config)}."
-            )
-
-        text_config = config.text_config
-        vision_config = config.vision_config
-
-        self.projection_dim = config.projection_dim
-        self.text_embed_dim = text_config.hidden_size
-        self.vision_embed_dim = vision_config.hidden_size
-
-        self.text_model = CLIPTextTransformer(text_config)
-        self.vision_model = CLIPVisionTransformer(vision_config)
-
-        self.visual_projection = nn.Linear(self.vision_embed_dim, self.projection_dim, bias=False)
-        self.text_projection = nn.Linear(self.text_embed_dim, self.projection_dim, bias=False)
-        self.logit_scale = nn.Parameter(torch.ones([]) * self.config.logit_scale_init_value)
-
-        self.init_weights()
-
-    def get_text_features(
-        self,
-        input_ids=None,
-        attention_mask=None,
-        position_ids=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        r"""
-        Returns:
-            text_features (:obj:`torch.FloatTensor` of shape :obj:`(batch_size, output_dim`): The text embeddings
-            obtained by applying the projection layer to the pooled output of :class:`~transformers.CLIPTextModel`.
-
-        Examples::
-
-            >>> from transformers import CLIPTokenizer, CLIPModel
+    def get_input_embeddings(self):
+        return self.text_embeddings.word_embeddings
 
-            >>> model = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
-            >>> tokenizer = CLIPTokenizer.from_pretrained("openai/clip-vit-base-patch32")
+    def set_input_embeddings(self, value):
+        self.text_embeddings.word_embeddings = value
 
-            >>> inputs = tokenizer(["a photo of a cat", "a photo of a dog"],  padding=True, return_tensors="pt")
-            >>> text_features = model.get_text_features(**inputs)
+    def resize_token_embeddings(self, new_num_tokens):
+        old_embeddings = self.get_input_embeddings()
+        new_embeddings = self._get_resized_embeddings(old_embeddings, new_num_tokens)
+        self.set_input_embeddings(new_embeddings)
+
+    def _get_resized_embeddings(
+        self, old_embeddings: nn.Embedding, new_num_tokens: Optional[int] = None
+    ) -> nn.Embedding:
         """
-        text_outputs = self.text_model(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
-        )
-
-        pooled_output = text_outputs[1]
-        text_features = self.text_projection(pooled_output)
-
-        return text_features
-
-    def get_image_features(
-        self,
-        pixel_values=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        r"""
-        Returns:
-            image_features (:obj:`torch.FloatTensor` of shape :obj:`(batch_size, output_dim`): The image embeddings
-            obtained by applying the projection layer to the pooled output of :class:`~transformers.CLIPVisionModel`.
-
-        Examples::
-
-            >>> from PIL import Image
-            >>> import requests
-            >>> from transformers import CLIPProcessor, CLIPModel
-
-            >>> model = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
-            >>> processor = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
-
-            >>> url = "http://images.cocodataset.org/val2017/000000039769.jpg"
-            >>> image = Image.open(requests.get(url, stream=True).raw)
-
-            >>> inputs = processor(images=image, return_tensors="pt")
+        Build a resized Embedding Module from a provided token Embedding Module. Increasing the size will add newly
+        initialized vectors at the end. Reducing the size will remove vectors from the end
 
-            >>> image_features = model.get_image_features(**inputs)
+        Args:
+            old_embeddings (:obj:`torch.nn.Embedding`):
+                Old embeddings to be resized.
+            new_num_tokens (:obj:`int`, `optional`):
+                New number of tokens in the embedding matrix.
+
+                Increasing the size will add newly initialized vectors at the end. Reducing the size will remove
+                vectors from the end. If not provided or :obj:`None`, just returns a pointer to the input tokens
+                :obj:`torch.nn.Embedding`` module of the model without doing anything.
+
+        Return:
+            :obj:`torch.nn.Embedding`: Pointer to the resized Embedding Module or the old Embedding Module if
+            :obj:`new_num_tokens` is :obj:`None`
         """
-        vision_outputs = self.vision_model(
-            pixel_values=pixel_values,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
-        )
-
-        pooled_output = vision_outputs[1]  # pooled_output
-        image_features = self.visual_projection(pooled_output)
-
-        return image_features
-
-    @replace_return_docstrings(output_type=CLIPOutput, config_class=CLIPConfig)
-    def forward(
-        self,
-        input_ids=None,
-        pixel_values=None,
-        attention_mask=None,
-        position_ids=None,
-        return_loss=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        r"""
-        Returns:
-
-        Examples::
-
-            >>> from PIL import Image
-            >>> import requests
-            >>> from transformers import CLIPProcessor, CLIPModel
-
-            >>> model = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
-            >>> processor = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
-
-            >>> url = "http://images.cocodataset.org/val2017/000000039769.jpg"
-            >>> image = Image.open(requests.get(url, stream=True).raw)
-
-            >>> inputs = processor(text=["a photo of a cat", "a photo of a dog"], images=image, return_tensors="pt", padding=True)
+        if new_num_tokens is None:
+            return old_embeddings
+        else:
+            old_num_tokens, old_embedding_dim = old_embeddings.weight.size()
 
-            >>> outputs = model(**inputs)
-            >>> logits_per_image = outputs.logits_per_image # this is the image-text similarity score
-            >>> probs = logits_per_image.softmax(dim=1) # we can take the softmax to get the label probabilities
+        if old_num_tokens == new_num_tokens:
+            return old_embeddings
 
-        """
-        return_dict = return_dict if return_dict is not None else self.config.return_dict
-        vision_outputs = self.vision_model(
-            pixel_values=pixel_values,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
-        )
+        if not isinstance(old_embeddings, nn.Embedding):
+            raise TypeError(
+                f"Old embeddings are of type {type(old_embeddings)}, which is not an instance of {nn.Embedding}."
+                f"You should either use a different resize function or make sure that `old_embeddings` are an instance of {nn.Embedding}."
+            )
 
-        text_outputs = self.text_model(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
+        # Build new embeddings
+        new_embeddings = nn.Embedding(new_num_tokens, old_embedding_dim).to(
+            self.device, dtype=old_embeddings.weight.dtype
         )
 
-        image_embeds = vision_outputs[1]
-        image_embeds = self.visual_projection(image_embeds)
-
-        text_embeds = text_outputs[1]
-        text_embeds = self.text_projection(text_embeds)
+        # initialize all new embeddings (in particular added tokens)
+        self._init_text_weights(new_embeddings)
 
-        # normalized features
-        image_embeds = image_embeds / image_embeds.norm(dim=-1, keepdim=True)
-        text_embeds = text_embeds / text_embeds.norm(dim=-1, keepdim=True)
-
-        # cosine similarity as logits
-        logit_scale = self.logit_scale.exp()
-        logits_per_text = torch.matmul(text_embeds, image_embeds.t()) * logit_scale
-        logits_per_image = logits_per_text.T
-
-        loss = None
-        if return_loss:
-            loss = clip_loss(logits_per_text)
+        # Copy token embeddings from the previous weights
 
-        if not return_dict:
-            output = (logits_per_image, logits_per_text, text_embeds, image_embeds, text_outputs, vision_outputs)
-            return ((loss,) + output) if loss is not None else output
+        # numbers of tokens to copy
+        n = min(old_num_tokens, new_num_tokens)
+        new_embeddings.weight.data[:n, :] = old_embeddings.weight.data[:n, :]
 
-        return CLIPOutput(
-            loss=loss,
-            logits_per_image=logits_per_image,
-            logits_per_text=logits_per_text,
-            text_embeds=text_embeds,
-            image_embeds=image_embeds,
-            text_model_output=text_outputs,
-            vision_model_output=vision_outputs,
-        )
+        return new_embeddings
```

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/multimodal/models/modeling_IFA.py` & `deepke-2.2/src/deepke/relation_extraction/multimodal/models/modeling_IFA.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/multimodal/modules/dataset.py` & `deepke-2.2/src/deepke/name_entity_re/multimodal/modules/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import torch
 import os
 from PIL import Image
 from torch.utils.data import Dataset
-from transformers import BertTokenizer
-from ..models.clip.processing_clip import CLIPProcessor
+from transformers import BertTokenizer, CLIPProcessor
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class MMPNERProcessor(object):
     def __init__(self, data_path, args) -> None:
```

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/multimodal/modules/train.py` & `deepke-2.2/src/deepke/name_entity_re/multimodal/modules/train.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/models/BiLSTM_CRF.py` & `deepke-2.2/src/deepke/name_entity_re/standard/models/BiLSTM_CRF.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/models/InferBert.py` & `deepke-2.2/src/deepke/name_entity_re/standard/models/InferBert.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/tools/dataset.py` & `deepke-2.2/src/deepke/name_entity_re/standard/tools/dataset.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/tools/preprocess.py` & `deepke-2.2/src/deepke/name_entity_re/standard/tools/preprocess.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/data_loader.py` & `deepke-2.2/src/deepke/name_entity_re/standard/w2ner/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/model.py` & `deepke-2.2/src/deepke/name_entity_re/standard/w2ner/model.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/name_entity_re/standard/w2ner/utils.py` & `deepke-2.2/src/deepke/name_entity_re/standard/w2ner/utils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/document/evaluation.py` & `deepke-2.2/src/deepke/relation_extraction/document/evaluation.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/document/losses.py` & `deepke-2.2/src/deepke/relation_extraction/document/losses.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/document/model.py` & `deepke-2.2/src/deepke/relation_extraction/document/model.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/document/module.py` & `deepke-2.2/src/deepke/relation_extraction/document/module.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/document/prepro.py` & `deepke-2.2/src/deepke/relation_extraction/document/prepro.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/document/utils.py` & `deepke-2.2/src/deepke/relation_extraction/document/utils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/base_data_module.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/base_data_module.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/dialogue.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/dialogue.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/dataset/processor.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/dataset/processor.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/generate_k_shot.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/generate_k_shot.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/get_label_word.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/get_label_word.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/base.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/base.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/transformer.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/transformer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/few_shot/lit_models/util.py` & `deepke-2.2/src/deepke/relation_extraction/few_shot/lit_models/util.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/dataset.py` & `deepke-2.2/src/deepke/relation_extraction/multimodal/modules/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import random
 import os
 import torch
 import json
 import ast
 from PIL import Image
 from torch.utils.data import Dataset
-from transformers import BertTokenizer
-from ..models.clip.processing_clip import CLIPProcessor
+from transformers import BertTokenizer, CLIPProcessor
 import logging
 logger = logging.getLogger(__name__)
 
 
 class MMREProcessor(object):
     def __init__(self, data_path, re_path, args):
         self.args = args
```

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/metrics.py` & `deepke-2.2/src/deepke/relation_extraction/multimodal/modules/metrics.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/multimodal/modules/train.py` & `deepke-2.2/src/deepke/relation_extraction/multimodal/modules/train.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/BasicModule.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/BasicModule.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/BiLSTM.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/BiLSTM.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/Capsule.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/Capsule.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/GCN.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/GCN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/LM.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/LM.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/PCNN.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/PCNN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/models/Transformer.py` & `deepke-2.2/src/deepke/relation_extraction/standard/models/Transformer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/Attention.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/Attention.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/CNN.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/CNN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/Capsule.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/Capsule.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/Embedding.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/Embedding.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/GCN.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/GCN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/RNN.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/RNN.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/module/Transformer.py` & `deepke-2.2/src/deepke/relation_extraction/standard/module/Transformer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/dataset.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/dataset.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/loss.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/loss.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/metrics.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/preprocess.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/preprocess.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/serializer.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/serializer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/trainer.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/tools/vocab.py` & `deepke-2.2/src/deepke/relation_extraction/standard/tools/vocab.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/utils/ioUtils.py` & `deepke-2.2/src/deepke/relation_extraction/standard/utils/ioUtils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/relation_extraction/standard/utils/nnUtils.py` & `deepke-2.2/src/deepke/relation_extraction/standard/utils/nnUtils.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke/transform_data.py` & `deepke-2.2/src/deepke/transform_data.py`

 * *Files identical despite different names*

### Comparing `deepke-2.1.3/src/deepke.egg-info/SOURCES.txt` & `deepke-2.2/src/deepke.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -33,20 +33,57 @@
 src/deepke/attribution_extraction/standard/tools/trainer.py
 src/deepke/attribution_extraction/standard/tools/vocab.py
 src/deepke/attribution_extraction/standard/utils/__init__.py
 src/deepke/attribution_extraction/standard/utils/ioUtils.py
 src/deepke/attribution_extraction/standard/utils/nnUtils.py
 src/deepke/event_extraction/__init__.py
 src/deepke/event_extraction/standard/__init__.py
+src/deepke/event_extraction/standard/bertcrf/__init__.py
+src/deepke/event_extraction/standard/bertcrf/bert_crf.py
+src/deepke/event_extraction/standard/bertcrf/crf.py
+src/deepke/event_extraction/standard/bertcrf/processor_ee.py
+src/deepke/event_extraction/standard/bertcrf/utils_ee.py
 src/deepke/event_extraction/standard/degree/__init__.py
 src/deepke/event_extraction/standard/degree/data.py
 src/deepke/event_extraction/standard/degree/model.py
 src/deepke/event_extraction/standard/degree/template_generate_ace.py
 src/deepke/event_extraction/standard/degree/utils.py
 src/deepke/name_entity_re/__init__.py
+src/deepke/name_entity_re/cross/__init__.py
+src/deepke/name_entity_re/cross/extraction/__init__.py
+src/deepke/name_entity_re/cross/extraction/constants.py
+src/deepke/name_entity_re/cross/extraction/dataset_processer.py
+src/deepke/name_entity_re/cross/extraction/extraction_metrics.py
+src/deepke/name_entity_re/cross/extraction/label_tree.py
+src/deepke/name_entity_re/cross/extraction/record_schema.py
+src/deepke/name_entity_re/cross/extraction/scorer.py
+src/deepke/name_entity_re/cross/extraction/utils.py
+src/deepke/name_entity_re/cross/extraction/noiser/__init__.py
+src/deepke/name_entity_re/cross/extraction/noiser/spot_asoc_noiser.py
+src/deepke/name_entity_re/cross/extraction/predict_parser/__init__.py
+src/deepke/name_entity_re/cross/extraction/predict_parser/predict_parser.py
+src/deepke/name_entity_re/cross/extraction/predict_parser/spotasoc_predict_parser.py
+src/deepke/name_entity_re/cross/extraction/predict_parser/utils.py
+src/deepke/name_entity_re/cross/sel2record/__init__.py
+src/deepke/name_entity_re/cross/sel2record/record.py
+src/deepke/name_entity_re/cross/sel2record/sel2record.py
+src/deepke/name_entity_re/cross/seq2seq/__init__.py
+src/deepke/name_entity_re/cross/seq2seq/constrained_seq2seq.py
+src/deepke/name_entity_re/cross/seq2seq/features.py
+src/deepke/name_entity_re/cross/seq2seq/modeling_t5.py
+src/deepke/name_entity_re/cross/seq2seq/models.py
+src/deepke/name_entity_re/cross/seq2seq/t5_bert_tokenizer.py
+src/deepke/name_entity_re/cross/seq2seq/trainer_arguments.py
+src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/__init__.py
+src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/constraint_decoder.py
+src/deepke/name_entity_re/cross/seq2seq/constraint_decoder/spotasoc_constraint_decoder.py
+src/deepke/name_entity_re/cross/seq2seq/data_collator/__init__.py
+src/deepke/name_entity_re/cross/seq2seq/data_collator/hybird_data_collator.py
+src/deepke/name_entity_re/cross/seq2seq/data_collator/meta_data_collator.py
+src/deepke/name_entity_re/cross/seq2seq/data_collator/t5mlm_data_collator.py
 src/deepke/name_entity_re/few_shot/__init__.py
 src/deepke/name_entity_re/few_shot/models/__init__.py
 src/deepke/name_entity_re/few_shot/models/model.py
 src/deepke/name_entity_re/few_shot/models/modeling_bart.py
 src/deepke/name_entity_re/few_shot/module/__init__.py
 src/deepke/name_entity_re/few_shot/module/datasets.py
 src/deepke/name_entity_re/few_shot/module/mapping_type.py
@@ -54,23 +91,14 @@
 src/deepke/name_entity_re/few_shot/module/train.py
 src/deepke/name_entity_re/few_shot/utils/__init__.py
 src/deepke/name_entity_re/few_shot/utils/util.py
 src/deepke/name_entity_re/multimodal/__init__.py
 src/deepke/name_entity_re/multimodal/models/IFA_model.py
 src/deepke/name_entity_re/multimodal/models/__init__.py
 src/deepke/name_entity_re/multimodal/models/modeling_IFA.py
-src/deepke/name_entity_re/multimodal/models/clip/__init__.py
-src/deepke/name_entity_re/multimodal/models/clip/configuration_clip.py
-src/deepke/name_entity_re/multimodal/models/clip/feature_extraction_clip.py
-src/deepke/name_entity_re/multimodal/models/clip/feature_extraction_utils.py
-src/deepke/name_entity_re/multimodal/models/clip/file_utils.py
-src/deepke/name_entity_re/multimodal/models/clip/image_utils.py
-src/deepke/name_entity_re/multimodal/models/clip/modeling_clip.py
-src/deepke/name_entity_re/multimodal/models/clip/processing_clip.py
-src/deepke/name_entity_re/multimodal/models/clip/tokenization_clip.py
 src/deepke/name_entity_re/multimodal/modules/__init__.py
 src/deepke/name_entity_re/multimodal/modules/dataset.py
 src/deepke/name_entity_re/multimodal/modules/train.py
 src/deepke/name_entity_re/standard/__init__.py
 src/deepke/name_entity_re/standard/models/BiLSTM_CRF.py
 src/deepke/name_entity_re/standard/models/InferBert.py
 src/deepke/name_entity_re/standard/models/__init__.py
@@ -100,23 +128,14 @@
 src/deepke/relation_extraction/few_shot/lit_models/base.py
 src/deepke/relation_extraction/few_shot/lit_models/transformer.py
 src/deepke/relation_extraction/few_shot/lit_models/util.py
 src/deepke/relation_extraction/multimodal/__init__.py
 src/deepke/relation_extraction/multimodal/models/IFA_model.py
 src/deepke/relation_extraction/multimodal/models/__init__.py
 src/deepke/relation_extraction/multimodal/models/modeling_IFA.py
-src/deepke/relation_extraction/multimodal/models/clip/__init__.py
-src/deepke/relation_extraction/multimodal/models/clip/configuration_clip.py
-src/deepke/relation_extraction/multimodal/models/clip/feature_extraction_clip.py
-src/deepke/relation_extraction/multimodal/models/clip/feature_extraction_utils.py
-src/deepke/relation_extraction/multimodal/models/clip/file_utils.py
-src/deepke/relation_extraction/multimodal/models/clip/image_utils.py
-src/deepke/relation_extraction/multimodal/models/clip/modeling_clip.py
-src/deepke/relation_extraction/multimodal/models/clip/processing_clip.py
-src/deepke/relation_extraction/multimodal/models/clip/tokenization_clip.py
 src/deepke/relation_extraction/multimodal/modules/__init__.py
 src/deepke/relation_extraction/multimodal/modules/dataset.py
 src/deepke/relation_extraction/multimodal/modules/metrics.py
 src/deepke/relation_extraction/multimodal/modules/train.py
 src/deepke/relation_extraction/standard/__init__.py
 src/deepke/relation_extraction/standard/models/BasicModule.py
 src/deepke/relation_extraction/standard/models/BiLSTM.py
@@ -140,8 +159,40 @@
 src/deepke/relation_extraction/standard/tools/metrics.py
 src/deepke/relation_extraction/standard/tools/preprocess.py
 src/deepke/relation_extraction/standard/tools/serializer.py
 src/deepke/relation_extraction/standard/tools/trainer.py
 src/deepke/relation_extraction/standard/tools/vocab.py
 src/deepke/relation_extraction/standard/utils/__init__.py
 src/deepke/relation_extraction/standard/utils/ioUtils.py
-src/deepke/relation_extraction/standard/utils/nnUtils.py
+src/deepke/relation_extraction/standard/utils/nnUtils.py
+src/deepke/triple_extraction/__init__.py
+src/deepke/triple_extraction/ASP/__init__.py
+src/deepke/triple_extraction/ASP/metrics/__init__.py
+src/deepke/triple_extraction/ASP/metrics/blanc.py
+src/deepke/triple_extraction/ASP/metrics/conll.py
+src/deepke/triple_extraction/ASP/metrics/metrics.py
+src/deepke/triple_extraction/ASP/modeling_transformer/__init__.py
+src/deepke/triple_extraction/ASP/modeling_transformer/modeling_outputs.py
+src/deepke/triple_extraction/ASP/models/__init__.py
+src/deepke/triple_extraction/ASP/models/model_coref.py
+src/deepke/triple_extraction/ASP/models/model_ere.py
+src/deepke/triple_extraction/ASP/models/model_ner.py
+src/deepke/triple_extraction/ASP/models/modeling_outputs.py
+src/deepke/triple_extraction/ASP/models/t5_coref.py
+src/deepke/triple_extraction/ASP/models/t5_ere.py
+src/deepke/triple_extraction/ASP/models/t5_ner.py
+src/deepke/triple_extraction/ASP/util/__init__.py
+src/deepke/triple_extraction/ASP/util/func.py
+src/deepke/triple_extraction/ASP/util/multigpu_fused_adam.py
+src/deepke/triple_extraction/ASP/util/runner.py
+src/deepke/triple_extraction/ASP/util/tensorize_coref.py
+src/deepke/triple_extraction/ASP/util/tensorize_ere.py
+src/deepke/triple_extraction/ASP/util/tensorize_ner.py
+src/deepke/triple_extraction/PRGC/__init__.py
+src/deepke/triple_extraction/PRGC/dataloader.py
+src/deepke/triple_extraction/PRGC/dataloader_utils.py
+src/deepke/triple_extraction/PRGC/evaluate.py
+src/deepke/triple_extraction/PRGC/metrics.py
+src/deepke/triple_extraction/PRGC/model.py
+src/deepke/triple_extraction/PRGC/optimization.py
+src/deepke/triple_extraction/PRGC/util.py
+src/deepke/triple_extraction/PURE/__init__.py
```

