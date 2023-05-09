# Comparing `tmp/bark-0.0.1a0.tar.gz` & `tmp/bark-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bark-0.0.1a0.tar", last modified: Mon May  1 15:17:41 2023, max compression
+gzip compressed data, was "bark-0.1.5.tar", last modified: Tue May  9 13:21:20 2023, max compression
```

## Comparing `bark-0.0.1a0.tar` & `bark-0.1.5.tar`

### file list

```diff
@@ -1,162 +1,293 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:17:41.738645 bark-0.0.1a0/
--rw-r--r--   0 martin     (501) staff       (20)    19333 2023-04-30 18:22:13.000000 bark-0.0.1a0/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)    31869 2023-05-01 15:17:41.738489 bark-0.0.1a0/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     9044 2023-04-30 18:21:15.000000 bark-0.0.1a0/README.md
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:17:41.709497 bark-0.0.1a0/bark/
--rw-r--r--   0 martin     (501) staff       (20)      140 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     3574 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/api.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:17:41.707992 bark-0.0.1a0/bark/assets/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:17:41.738147 bark-0.0.1a0/bark/assets/prompts/
--rw-r--r--   0 martin     (501) staff       (20)    16794 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/announcer.npz
--rw-r--r--   0 martin     (501) staff       (20)    31940 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    31940 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    23516 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    29060 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    20316 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    35084 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    31724 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    59348 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    25116 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    22180 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/de_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    22396 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    18396 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    33860 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    38124 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    21220 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    15516 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    13436 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    35084 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    18980 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    35940 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/en_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    27620 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    25436 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    27620 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    26500 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    24420 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    34820 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    21596 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    18660 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    22660 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/es_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    30604 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    29324 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    51084 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    31460 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    36364 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    44044 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    43564 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    53908 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    33060 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    31244 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/fr_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    32580 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    23036 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    26820 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    28684 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    24476 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    33004 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    30020 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    24956 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    30180 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/hi_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    46604 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    45268 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    52684 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    22396 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    42764 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    34180 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    41268 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    29964 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    35940 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/it_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    25220 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    44148 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    24796 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    37964 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    22716 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    24580 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    33380 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    50548 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    29540 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ja_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    24156 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    26396 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    31940 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    56628 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    23356 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    29004 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    30500 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    22180 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    24476 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    21916 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ko_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    39780 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    26500 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    43084 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    42284 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    42548 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    34020 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    45324 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    37380 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    33380 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    36364 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pl_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    32420 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    58492 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    21596 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    35300 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    49004 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    34444 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    56628 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    34020 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    30284 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    58652 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/pt_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    57852 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    24260 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    51668 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    29164 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    27940 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    23356 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    45748 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    25380 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    42924 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    38500 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/ru_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    19620 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    21380 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    19460 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    32740 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    19676 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    54548 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    23516 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    22556 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    20580 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    18396 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    26020 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    24156 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    32740 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    20100 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    16100 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    29220 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    21596 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    21276 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    35724 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    19460 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/tr_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    19620 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_0.npz
--rw-r--r--   0 martin     (501) staff       (20)    21380 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_1.npz
--rw-r--r--   0 martin     (501) staff       (20)    19460 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_2.npz
--rw-r--r--   0 martin     (501) staff       (20)    32740 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_3.npz
--rw-r--r--   0 martin     (501) staff       (20)    19676 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_4.npz
--rw-r--r--   0 martin     (501) staff       (20)    54548 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_5.npz
--rw-r--r--   0 martin     (501) staff       (20)    23516 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_6.npz
--rw-r--r--   0 martin     (501) staff       (20)    22556 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_7.npz
--rw-r--r--   0 martin     (501) staff       (20)    20580 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_8.npz
--rw-r--r--   0 martin     (501) staff       (20)    18396 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/assets/prompts/zh_speaker_9.npz
--rw-r--r--   0 martin     (501) staff       (20)    30945 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/generation.py
--rw-r--r--   0 martin     (501) staff       (20)     9139 2023-04-30 18:21:15.000000 bark-0.0.1a0/bark/model.py
--rw-r--r--   0 martin     (501) staff       (20)     5955 2023-04-14 17:33:15.000000 bark-0.0.1a0/bark/model_fine.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:17:41.710152 bark-0.0.1a0/bark.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)    31869 2023-05-01 15:17:41.000000 bark-0.0.1a0/bark.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     5445 2023-05-01 15:17:41.000000 bark-0.0.1a0/bark.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-01 15:17:41.000000 bark-0.0.1a0/bark.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)      222 2023-05-01 15:17:41.000000 bark-0.0.1a0/bark.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)        5 2023-05-01 15:17:41.000000 bark-0.0.1a0/bark.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)      960 2023-05-01 15:16:06.000000 bark-0.0.1a0/pyproject.toml
--rw-r--r--   0 martin     (501) staff       (20)       38 2023-05-01 15:17:41.738677 bark-0.0.1a0/setup.cfg
--rw-r--r--   0 martin     (501) staff       (20)       38 2023-04-14 17:33:15.000000 bark-0.0.1a0/setup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-09 13:21:20.640107 bark-0.1.5/
+-rw-r--r--   0 martin     (501) staff       (20)     1061 2023-05-02 15:45:34.000000 bark-0.1.5/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)    14544 2023-05-09 13:21:20.639879 bark-0.1.5/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)    13025 2023-05-02 15:45:34.000000 bark-0.1.5/README.md
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-09 13:21:20.597599 bark-0.1.5/bark/
+-rw-r--r--   0 martin     (501) staff       (20)      140 2023-04-30 18:21:15.000000 bark-0.1.5/bark/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     3626 2023-05-02 15:45:34.000000 bark-0.1.5/bark/api.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-09 13:21:20.596539 bark-0.1.5/bark/assets/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-09 13:21:20.618211 bark-0.1.5/bark/assets/prompts/
+-rw-r--r--   0 martin     (501) staff       (20)    16794 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/announcer.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31940 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31940 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23516 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29060 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20316 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    35084 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31724 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    59348 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25116 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22180 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/de_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22396 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    18396 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33860 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    38124 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21220 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    15516 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    13436 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    35084 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    18980 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    35940 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/en_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27620 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25436 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27620 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26500 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24420 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34820 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21596 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    18660 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22660 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/es_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30604 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29324 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    51084 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31460 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    36364 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    44044 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    43564 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    53908 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33060 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31244 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/fr_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32580 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23036 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26820 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28684 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24476 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33004 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30020 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24956 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30180 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/hi_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    46604 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    45268 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    52684 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22396 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    42764 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34180 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    41268 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29964 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    35940 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/it_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24900 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25220 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    44148 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24796 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    37964 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22716 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24580 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33380 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    50548 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29540 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ja_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24156 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26396 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31940 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    56628 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23356 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29004 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30500 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22180 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24476 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21916 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ko_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    39780 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26500 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    43084 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    42284 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    42548 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34020 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    45324 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    37380 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33380 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    36364 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pl_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32420 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    58492 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21596 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    35300 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    49004 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34444 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    56628 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34020 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30284 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    58652 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/pt_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    57852 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24260 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    51668 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29164 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27940 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23356 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    45748 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25380 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    42924 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    38500 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/ru_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19620 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21380 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19460 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32740 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19676 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    54548 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23516 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22556 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20580 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    18396 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26020 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24156 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32740 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20100 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    16100 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29220 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21596 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21276 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    35724 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19460 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/tr_speaker_9.npz
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-09 13:21:20.639585 bark-0.1.5/bark/assets/prompts/v2/
+-rw-r--r--   0 martin     (501) staff       (20)    39620 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27460 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24740 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31300 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30660 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31300 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23196 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    40100 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28524 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    51084 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/de_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28100 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25220 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26236 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34980 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23780 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24740 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25540 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22716 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23300 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30180 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/en_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22020 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25116 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26236 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23780 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23356 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25700 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20580 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22020 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25436 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19940 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/es_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    45804 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25700 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    52204 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    50764 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    49908 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    45108 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    55932 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32524 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    43244 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32100 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/fr_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32580 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25860 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27780 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29804 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25380 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    51404 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26396 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29380 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    39404 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23516 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/hi_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28740 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33804 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    40788 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30764 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28740 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30444 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29644 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    43724 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    42708 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    37644 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/it_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24420 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31244 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24100 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24476 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26716 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24956 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    40788 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25060 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20260 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31140 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ja_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26556 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26340 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19196 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    39564 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23140 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23196 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26396 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27884 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31140 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23676 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ko_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24900 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34660 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28580 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    41428 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30764 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    38180 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    38820 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29060 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19460 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30980 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pl_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    27724 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34500 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    36844 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26980 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26396 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28260 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30764 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28100 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28524 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    39780 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/pt_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    39884 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    56628 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29220 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19940 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28204 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    44628 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20476 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    26020 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    39084 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    34660 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/ru_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22076 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24476 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    24956 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28684 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    33164 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    17220 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    25276 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20260 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20580 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    28204 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/tr_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20636 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19836 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21060 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    31300 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    29964 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    17436 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    16900 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21060 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19300 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    16156 2023-05-02 15:45:34.000000 bark-0.1.5/bark/assets/prompts/v2/zh_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19620 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_0.npz
+-rw-r--r--   0 martin     (501) staff       (20)    21380 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_1.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19460 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_2.npz
+-rw-r--r--   0 martin     (501) staff       (20)    32740 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_3.npz
+-rw-r--r--   0 martin     (501) staff       (20)    19676 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_4.npz
+-rw-r--r--   0 martin     (501) staff       (20)    54548 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_5.npz
+-rw-r--r--   0 martin     (501) staff       (20)    23516 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_6.npz
+-rw-r--r--   0 martin     (501) staff       (20)    22556 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_7.npz
+-rw-r--r--   0 martin     (501) staff       (20)    20580 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_8.npz
+-rw-r--r--   0 martin     (501) staff       (20)    18396 2023-04-30 18:21:15.000000 bark-0.1.5/bark/assets/prompts/zh_speaker_9.npz
+-rw-r--r--   0 martin     (501) staff       (20)    30372 2023-05-09 13:15:47.000000 bark-0.1.5/bark/generation.py
+-rw-r--r--   0 martin     (501) staff       (20)     9139 2023-04-30 18:21:15.000000 bark-0.1.5/bark/model.py
+-rw-r--r--   0 martin     (501) staff       (20)     5955 2023-04-14 17:33:15.000000 bark-0.1.5/bark/model_fine.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-09 13:21:20.598191 bark-0.1.5/bark.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)    14544 2023-05-09 13:21:20.000000 bark-0.1.5/bark.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)    10645 2023-05-09 13:21:20.000000 bark-0.1.5/bark.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-09 13:21:20.000000 bark-0.1.5/bark.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)      230 2023-05-09 13:21:20.000000 bark-0.1.5/bark.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)        5 2023-05-09 13:21:20.000000 bark-0.1.5/bark.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)      983 2023-05-09 13:20:55.000000 bark-0.1.5/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)       38 2023-05-09 13:21:20.640150 bark-0.1.5/setup.cfg
+-rw-r--r--   0 martin     (501) staff       (20)       38 2023-04-14 17:33:15.000000 bark-0.1.5/setup.py
```

### Comparing `bark-0.0.1a0/README.md` & `bark-0.1.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,158 +1,197 @@
 # 🐶 Bark
 
-<a href="http://www.repostatus.org/#active"><img src="http://www.repostatus.org/badges/latest/active.svg" /></a>
+[![](https://dcbadge.vercel.app/api/server/J2B2vsjKuE?style=flat&compact=True)](https://discord.gg/J2B2vsjKuE)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/OnusFM.svg?style=social&label=@OnusFM)](https://twitter.com/OnusFM)
-[![](https://dcbadge.vercel.app/api/server/J2B2vsjKuE?compact=true&style=flat&)](https://discord.gg/J2B2vsjKuE)
-
-
-[Examples](https://suno-ai.notion.site/Bark-Examples-5edae8b02a604b54a42244ba45ebc2e2) | [Model Card](./model-card.md) | [Playground Waitlist](https://3os84zs17th.typeform.com/suno-studio)
+<a href="http://www.repostatus.org/#active"><img src="http://www.repostatus.org/badges/latest/active.svg" /></a>
 
-Bark is a transformer-based text-to-audio model created by [Suno](https://suno.ai). Bark can generate highly realistic, multilingual speech as well as other audio - including music, background noise and simple sound effects. The model can also produce nonverbal communications like laughing, sighing and crying. To support the research community, we are providing access to pretrained model checkpoints ready for inference.
+[Examples](https://suno-ai.notion.site/Bark-Examples-5edae8b02a604b54a42244ba45ebc2e2) • [Suno Studio Waitlist](https://3os84zs17th.typeform.com/suno-studio) • [Updates](#-updates) • [How to Use](#-usage-in-python) • [Installation](#-installation) • [FAQ](#-faq)
 
+[//]: <br> (vertical spaces around image)
+<br>
 <p align="center">
-<img src="https://user-images.githubusercontent.com/5068315/230698495-cbb1ced9-c911-4c9a-941d-a1a4a1286ac6.png" width="500"></img>
+<img src="https://user-images.githubusercontent.com/5068315/235310676-a4b3b511-90ec-4edf-8153-7ccf14905d73.png" width="500"></img>
 </p>
+<br>
+
+Bark is a transformer-based text-to-audio model created by [Suno](https://suno.ai). Bark can generate highly realistic, multilingual speech as well as other audio - including music, background noise and simple sound effects. The model can also produce nonverbal communications like laughing, sighing and crying. To support the research community, we are providing access to pretrained model checkpoints, which are ready for inference and available for commercial use.
+
+## ⚠ Disclaimer
+Bark was developed for research purposes. It is not a conventional text-to-speech model but instead a fully generative text-to-audio model, which can deviate in unexpected ways from provided prompts. Suno does not take responsibility for any output generated. Use at your own risk, and please act responsibly.
 
-## 🔊 Demos
+## 🎧 Demos  
 
-[![Open in Spaces](https://img.shields.io/badge/🤗-Open%20In%20Spaces-blue.svg)](https://huggingface.co/spaces/suno/bark)
+[![Open in Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue.svg)](https://huggingface.co/spaces/suno/bark)
+[![Open on Replicate](https://img.shields.io/badge/®️-Open%20on%20Replicate-blue.svg)](https://replicate.com/suno-ai/bark)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eJfA2XUa-mXwdMy7DoYKVYHI1iTd9Vkt?usp=sharing)
 
-## 🤖 Usage
+## 🚀 Updates
+
+**2023.05.01**
+- ©️ Bark is now licensed under the MIT License, meaning it's now available for commercial use!  
+- ⚡ 2x speed-up on GPU. 10x speed-up on CPU. We also added an option for a smaller version of Bark, which offers additional speed-up with the trade-off of slightly lower quality. 
+- 📕 [Long-form generation](notebooks/long_form_generation.ipynb), voice consistency enhancements and other examples are now documented in a new [notebooks](./notebooks) section.
+- 👥 We created a [voice prompt library](https://suno-ai.notion.site/8b8e8749ed514b0cbf3f699013548683?v=bc67cff786b04b50b3ceb756fd05f68c). We hope this resource helps you find useful prompts for your use cases! You can also join us on [Discord](https://discord.gg/J2B2vsjKuE), where the community actively shares useful prompts in the **#audio-prompts** channel.  
+- 💬 Growing community support and access to new features here: 
+
+     [![](https://dcbadge.vercel.app/api/server/J2B2vsjKuE)](https://discord.gg/J2B2vsjKuE)
+
+- 💾 You can now use Bark with GPUs that have low VRAM (<4GB).
+
+**2023.04.20**
+- 🐶 Bark release!
+
+## 🐍 Usage in Python
+
+<details open>
+  <summary><h3>🪑 Basics</h3></summary>
 
 ```python
 from bark import SAMPLE_RATE, generate_audio, preload_models
+from scipy.io.wavfile import write as write_wav
 from IPython.display import Audio
 
 # download and load all models
 preload_models()
 
 # generate audio from text
 text_prompt = """
      Hello, my name is Suno. And, uh — and I like pizza. [laughs] 
      But I also have other interests such as playing tic tac toe.
 """
 audio_array = generate_audio(text_prompt)
 
+# save audio to disk
+write_wav("bark_generation.wav", SAMPLE_RATE, audio_array)
+  
 # play text in notebook
 Audio(audio_array, rate=SAMPLE_RATE)
 ```
 
 [pizza.webm](https://user-images.githubusercontent.com/5068315/230490503-417e688d-5115-4eee-9550-b46a2b465ee3.webm)
 
+</details>
 
-To save `audio_array` as a WAV file:
-
-```python
-from scipy.io.wavfile import write as write_wav
-
-write_wav("/path/to/audio.wav", SAMPLE_RATE, audio_array)
-```
-
-### 🌎 Foreign Language
-
+<details open>
+  <summary><h3>🌎 Foreign Language</h3></summary>
+<br>
 Bark supports various languages out-of-the-box and automatically determines language from input text. When prompted with code-switched text, Bark will attempt to employ the native accent for the respective languages. English quality is best for the time being, and we expect other languages to further improve with scaling. 
+<br>
+<br>
 
 ```python
+
 text_prompt = """
-    Buenos días Miguel. Tu colega piensa que tu alemán es extremadamente malo. 
-    But I suppose your english isn't terrible.
+    추석은 내가 가장 좋아하는 명절이다. 나는 며칠 동안 휴식을 취하고 친구 및 가족과 시간을 보낼 수 있습니다.
 """
 audio_array = generate_audio(text_prompt)
 ```
+[suno_korean.webm](https://user-images.githubusercontent.com/32879321/235313033-dc4477b9-2da0-4b94-9c8b-a8c2d8f5bb5e.webm)
+  
+*Note: since Bark recognizes languages automatically from input text, it is possible to use for example a german history prompt with english text. This usually leads to english audio with a german accent.*
 
-[miguel.webm](https://user-images.githubusercontent.com/5068315/230684752-10baadfe-1e7c-46a2-8323-43282aef2c8c.webm)
-
-### 🎶 Music
+</details>
 
+<details open>
+  <summary><h3>🎶 Music</h3></summary>
 Bark can generate all types of audio, and, in principle, doesn't see a difference between speech and music. Sometimes Bark chooses to generate text as music, but you can help it out by adding music notes around your lyrics.
+<br>
+<br>
 
 ```python
 text_prompt = """
     ♪ In the jungle, the mighty jungle, the lion barks tonight ♪
 """
 audio_array = generate_audio(text_prompt)
 ```
-
 [lion.webm](https://user-images.githubusercontent.com/5068315/230684766-97f5ea23-ad99-473c-924b-66b6fab24289.webm)
+</details>
 
-### 🎤 Voice Presets and Voice/Audio Cloning
-
-Bark has the capability to fully clone voices - including tone, pitch, emotion and prosody. The model also attempts to preserve music, ambient noise, etc. from input audio. However, to mitigate misuse of this technology, we limit the audio history prompts to a limited set of Suno-provided, fully synthetic options to choose from for each language. Specify following the pattern: `{lang_code}_speaker_{0-9}`.
+<details open>
+<summary><h3>🎤 Voice Presets</h3></summary>
+  
+Bark supports 100+ speaker presets across [supported languages](#supported-languages). You can browse the library of speaker presets [here](https://suno-ai.notion.site/8b8e8749ed514b0cbf3f699013548683?v=bc67cff786b04b50b3ceb756fd05f68c), or in the [code](bark/assets/prompts). The community also often shares presets in [Discord](https://discord.gg/J2B2vsjKuE).
+
+Bark tries to match the tone, pitch, emotion and prosody of a given preset, but does not currently support custom voice cloning. The model also attempts to preserve music, ambient noise, etc.
+<br>
+<br>
 
 ```python
 text_prompt = """
     I have a silky smooth voice, and today I will tell you about 
     the exercise regimen of the common sloth.
 """
-audio_array = generate_audio(text_prompt, history_prompt="en_speaker_1")
+audio_array = generate_audio(text_prompt, history_prompt="v2/en_speaker_1")
 ```
 
-
 [sloth.webm](https://user-images.githubusercontent.com/5068315/230684883-a344c619-a560-4ff5-8b99-b4463a34487b.webm)
+</details>
 
-*Note: since Bark recognizes languages automatically from input text, it is possible to use for example a german history prompt with english text. This usually leads to english audio with a german accent.*
+### Generating Longer Audio
+  
+By default, `generate_audio` works well with around 13 seconds of spoken text. For an example of how to do long-form generation, see this [example notebook](notebooks/long_form_generation.ipynb).
 
-### 👥 Speaker Prompts
+<details>
+<summary>Click to toggle example long-form generations (from the example notebook)</summary>
 
-You can provide certain speaker prompts such as NARRATOR, MAN, WOMAN, etc. Please note that these are not always respected, especially if a conflicting audio history prompt is given.
+[dialog.webm](https://user-images.githubusercontent.com/2565833/235463539-f57608da-e4cb-4062-8771-148e29512b01.webm)
+
+[longform_advanced.webm](https://user-images.githubusercontent.com/2565833/235463547-1c0d8744-269b-43fe-9630-897ea5731652.webm)
+
+[longform_basic.webm](https://user-images.githubusercontent.com/2565833/235463559-87efe9f8-a2db-4d59-b764-57db83f95270.webm)
+
+</details>
 
-```python
-text_prompt = """
-    WOMAN: I would like an oatmilk latte please.
-    MAN: Wow, that's expensive!
-"""
-audio_array = generate_audio(text_prompt)
-```
 
-[latte.webm](https://user-images.githubusercontent.com/5068315/230684864-12d101a1-a726-471d-9d56-d18b108efcb8.webm)
 
 
 ## 💻 Installation
 
 ```
 pip install git+https://github.com/suno-ai/bark.git
 ```
 
 or
 
 ```
 git clone https://github.com/suno-ai/bark
 cd bark && pip install . 
 ```
+*Note: Do NOT use 'pip install bark'. It installs a different package, which is not managed by Suno.*
+
 
 ## 🛠️ Hardware and Inference Speed
 
 Bark has been tested and works on both CPU and GPU (`pytorch 2.0+`, CUDA 11.7 and CUDA 12.0).
-Running Bark requires running >100M parameter transformer models.
-On modern GPUs and PyTorch nightly, Bark can generate audio in roughly realtime. On older GPUs, default colab, or CPU, inference time might be 10-100x slower. 
 
-If you don't have new hardware available or if you want to play with bigger versions of our models, you can also sign up for early access to our model playground [here](https://3os84zs17th.typeform.com/suno-studio).
+On enterprise GPUs and PyTorch nightly, Bark can generate audio in roughly real-time. On older GPUs, default colab, or CPU, inference time might be significantly slower. For older GPUs or CPU you might want to consider using smaller models. Details can be found in out tutorial sections here.
+
+The full version of Bark requires around 12GB of VRAM to hold everything on GPU at the same time. 
+To use a smaller version of the models, which should fit into 8GB VRAM, set the environment flag `SUNO_USE_SMALL_MODELS=True`.
+
+If you don't have hardware available or if you want to play with bigger versions of our models, you can also sign up for early access to our model playground [here](https://3os84zs17th.typeform.com/suno-studio).
 
 ## ⚙️ Details
 
-Similar to [Vall-E](https://arxiv.org/abs/2301.02111) and some other amazing work in the field, Bark uses GPT-style 
-models to generate audio from scratch. Different from Vall-E, the initial text prompt is embedded into high-level semantic tokens without the use of phonemes. It can therefore generalize to arbitrary instructions beyond speech that occur in the training data, such as music lyrics, sound effects or other non-speech sounds. A subsequent second model is used to convert the generated semantic tokens into audio codec tokens to generate the full waveform. To enable the community to use Bark via public code we used the fantastic 
-[EnCodec codec](https://github.com/facebookresearch/encodec) from Facebook to act as an audio representation.
+Bark is fully generative tex-to-audio model devolved for research and demo purposes. It follows a GPT style architecture similar to [AudioLM](https://arxiv.org/abs/2209.03143) and [Vall-E](https://arxiv.org/abs/2301.02111) and a quantized Audio representation from [EnCodec](https://github.com/facebookresearch/encodec). It is not a conventional TTS model, but instead a fully generative text-to-audio model capable of deviating in unexpected ways from any given script. Different to previous approaches, the input text prompt is converted directly to audio without the intermediate use of phonemes. It can therefore generalize to arbitrary instructions beyond speech such as music lyrics, sound effects or other non-speech sounds.
 
 Below is a list of some known non-speech sounds, but we are finding more every day. Please let us know if you find patterns that work particularly well on [Discord](https://discord.gg/J2B2vsjKuE)!
 
 - `[laughter]`
 - `[laughs]`
 - `[sighs]`
 - `[music]`
 - `[gasps]`
 - `[clears throat]`
 - `—` or `...` for hesitations
 - `♪` for song lyrics
-- capitalization for emphasis of a word
-- `MAN/WOMAN:` for bias towards speaker
+- CAPITALIZATION for emphasis of a word
+- `[MAN]` and `[WOMAN]` to bias Bark toward male and female speakers, respectively
 
-**Supported Languages**
+### Supported Languages
 
 | Language | Status |
 | --- | --- |
 | English (en) | ✅ |
 | German (de) | ✅ |
 | Spanish (es) | ✅ |
 | French (fr) | ✅ |
@@ -161,44 +200,60 @@
 | Japanese (ja) | ✅ |
 | Korean (ko) | ✅ |
 | Polish (pl) | ✅ |
 | Portuguese (pt) | ✅ |
 | Russian (ru) | ✅ |
 | Turkish (tr) | ✅ |
 | Chinese, simplified (zh) | ✅ |
-| Arabic  | Coming soon! |
-| Bengali | Coming soon! |
-| Telugu | Coming soon! |
+
+Requests for future language support [here](https://github.com/suno-ai/bark/discussions/111) or in the **#forums** channel on [Discord](https://discord.com/invite/J2B2vsjKuE). 
 
 ## 🙏 Appreciation
 
 - [nanoGPT](https://github.com/karpathy/nanoGPT) for a dead-simple and blazing fast implementation of GPT-style models
 - [EnCodec](https://github.com/facebookresearch/encodec) for a state-of-the-art implementation of a fantastic audio codec
-- [AudioLM](https://github.com/lucidrains/audiolm-pytorch) for very related training and inference code
+- [AudioLM](https://github.com/lucidrains/audiolm-pytorch) for related training and inference code
 - [Vall-E](https://arxiv.org/abs/2301.02111), [AudioLM](https://arxiv.org/abs/2209.03143) and many other ground-breaking papers that enabled the development of Bark
 
 ## © License
 
-Bark is licensed under a non-commercial license: CC-BY 4.0 NC. The Suno models themselves may be used commercially. However, this version of Bark uses `EnCodec` as a neural codec backend, which is licensed under a [non-commercial license](https://github.com/facebookresearch/encodec/blob/main/LICENSE).
+Bark is licensed under the MIT License. 
 
-Please contact us at `bark@suno.ai` if you need access to a larger version of the model and/or a version of the model you can use commercially.  
+Please contact us at `bark@suno.ai` to request access to a larger version of the model.  
 
 ## 📱 Community
 
 - [Twitter](https://twitter.com/OnusFM)
 - [Discord](https://discord.gg/J2B2vsjKuE)
 
 ## 🎧 Suno Studio (Early Access)
 
 We’re developing a playground for our models, including Bark. 
 
 If you are interested, you can sign up for early access [here](https://3os84zs17th.typeform.com/suno-studio).
 
-## FAQ
+## ❓ FAQ
 
 #### How do I specify where models are downloaded and cached?
+* Bark uses Hugging Face to download and store models. You can see find more info [here](https://huggingface.co/docs/huggingface_hub/package_reference/environment_variables#hfhome). 
 
-Use the `XDG_CACHE_HOME` env variable to override where models are downloaded and cached (otherwise defaults to a subdirectory of `~/.cache`).
 
 #### Bark's generations sometimes differ from my prompts. What's happening?
+* Bark is a GPT-style model. As such, it may take some creative liberties in its generations, resulting in higher-variance model outputs than traditional text-to-speech approaches.
+
+#### What voices are supported by Bark?  
+* Bark supports 100+ speaker presets across [supported languages](#supported-languages). You can browse the library of speaker presets [here](https://suno-ai.notion.site/8b8e8749ed514b0cbf3f699013548683?v=bc67cff786b04b50b3ceb756fd05f68c). The community also shares presets in [Discord](https://discord.gg/J2B2vsjKuE). Bark also supports generating unique random voices that fit the input text. Bark does not currently support custom voice cloning.
+
+#### Why is the output limited to ~13-14 seconds?
+* Bark is a GPT-style model, and its architecture/context window is optimized to output generations with roughly this length.
+
+#### How much VRAM do I need?
+* The full version of Bark requires around 12Gb of memory to hold everything on GPU at the same time. However, even smaller cards down to ~2Gb work with some additional settings. Simply add the following code snippet before your generation: 
+
+```python
+import os
+os.environ["SUNO_OFFLOAD_CPU"] = True
+os.environ["SUNO_USE_SMALL_MODELS"] = True
+```
 
-Bark is a GPT-style model. As such, it may take some creative liberties in its generations, resulting in higher-variance model outputs than traditional text-to-speech approaches.
+#### My generated audio sounds like a 1980s phone call. What's happening?
+* Bark generates audio from scratch. It is not meant to create only high-fidelity, studio-quality speech. Rather, outputs could be anything from perfect speech to multiple people arguing at a baseball game recorded with bad microphones.
```

#### html2text {}

```diff
@@ -1,118 +1,181 @@
-# ð¶ Bark [http://www.repostatus.org/badges/latest/active.svg] [![Twitter]
+# ð¶ Bark [![](https://dcbadge.vercel.app/api/server/
+J2B2vsjKuE?style=flat&compact=True)](https://discord.gg/J2B2vsjKuE) [![Twitter]
 (https://img.shields.io/twitter/url/https/twitter.com/
-OnusFM.svg?style=social&label=@OnusFM)](https://twitter.com/OnusFM) [![](https:
-//dcbadge.vercel.app/api/server/J2B2vsjKuE?compact=true&style=flat&)](https://
-discord.gg/J2B2vsjKuE) [Examples](https://suno-ai.notion.site/Bark-Examples-
-5edae8b02a604b54a42244ba45ebc2e2) | [Model Card](./model-card.md) | [Playground
-Waitlist](https://3os84zs17th.typeform.com/suno-studio) Bark is a transformer-
-based text-to-audio model created by [Suno](https://suno.ai). Bark can generate
-highly realistic, multilingual speech as well as other audio - including music,
-background noise and simple sound effects. The model can also produce nonverbal
-communications like laughing, sighing and crying. To support the research
-community, we are providing access to pretrained model checkpoints ready for
-inference.
-  [https://user-images.githubusercontent.com/5068315/230698495-cbb1ced9-c911-
-                          4c9a-941d-a1a4a1286ac6.png]
-## ð Demos [![Open in Spaces](https://img.shields.io/badge/ð¤-
-Open%20In%20Spaces-blue.svg)](https://huggingface.co/spaces/suno/bark) [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+OnusFM.svg?style=social&label=@OnusFM)](https://twitter.com/OnusFM) [http://
+www.repostatus.org/badges/latest/active.svg] [Examples](https://suno-
+ai.notion.site/Bark-Examples-5edae8b02a604b54a42244ba45ebc2e2) â¢ [Suno Studio
+Waitlist](https://3os84zs17th.typeform.com/suno-studio) â¢ [Updates](#-
+updates) â¢ [How to Use](#-usage-in-python) â¢ [Installation](#-installation)
+â¢ [FAQ](#-faq) [//]:
+(vertical spaces around image)
+  [https://user-images.githubusercontent.com/5068315/235310676-a4b3b511-90ec-
+                          4edf-8153-7ccf14905d73.png]
+
+Bark is a transformer-based text-to-audio model created by [Suno](https://
+suno.ai). Bark can generate highly realistic, multilingual speech as well as
+other audio - including music, background noise and simple sound effects. The
+model can also produce nonverbal communications like laughing, sighing and
+crying. To support the research community, we are providing access to
+pretrained model checkpoints, which are ready for inference and available for
+commercial use. ## â  Disclaimer Bark was developed for research purposes. It
+is not a conventional text-to-speech model but instead a fully generative text-
+to-audio model, which can deviate in unexpected ways from provided prompts.
+Suno does not take responsibility for any output generated. Use at your own
+risk, and please act responsibly. ## ð§ Demos [![Open in Spaces](https://
+img.shields.io/badge/ð¤-Open%20in%20Spaces-blue.svg)](https://huggingface.co/
+spaces/suno/bark) [![Open on Replicate](https://img.shields.io/badge/Â®ï¸-
+Open%20on%20Replicate-blue.svg)](https://replicate.com/suno-ai/bark) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1eJfA2XUa-mXwdMy7DoYKVYHI1iTd9Vkt?usp=sharing)
-## ð¤ Usage ```python from bark import SAMPLE_RATE, generate_audio,
-preload_models from IPython.display import Audio # download and load all models
-preload_models() # generate audio from text text_prompt = """ Hello, my name is
-Suno. And, uh â and I like pizza. [laughs] But I also have other interests
-such as playing tic tac toe. """ audio_array = generate_audio(text_prompt) #
-play text in notebook Audio(audio_array, rate=SAMPLE_RATE) ``` [pizza.webm]
-(https://user-images.githubusercontent.com/5068315/230490503-417e688d-5115-
-4eee-9550-b46a2b465ee3.webm) To save `audio_array` as a WAV file: ```python
-from scipy.io.wavfile import write as write_wav write_wav("/path/to/audio.wav",
-SAMPLE_RATE, audio_array) ``` ### ð Foreign Language Bark supports various
-languages out-of-the-box and automatically determines language from input text.
-When prompted with code-switched text, Bark will attempt to employ the native
-accent for the respective languages. English quality is best for the time
-being, and we expect other languages to further improve with scaling. ```python
-text_prompt = """ Buenos dÃ­as Miguel. Tu colega piensa que tu alemÃ¡n es
-extremadamente malo. But I suppose your english isn't terrible. """ audio_array
-= generate_audio(text_prompt) ``` [miguel.webm](https://user-
-images.githubusercontent.com/5068315/230684752-10baadfe-1e7c-46a2-8323-
-43282aef2c8c.webm) ### ð¶ Music Bark can generate all types of audio, and, in
-principle, doesn't see a difference between speech and music. Sometimes Bark
-chooses to generate text as music, but you can help it out by adding music
-notes around your lyrics. ```python text_prompt = """ âª In the jungle, the
-mighty jungle, the lion barks tonight âª """ audio_array = generate_audio
-(text_prompt) ``` [lion.webm](https://user-images.githubusercontent.com/
-5068315/230684766-97f5ea23-ad99-473c-924b-66b6fab24289.webm) ### ð¤ Voice
-Presets and Voice/Audio Cloning Bark has the capability to fully clone voices -
-including tone, pitch, emotion and prosody. The model also attempts to preserve
-music, ambient noise, etc. from input audio. However, to mitigate misuse of
-this technology, we limit the audio history prompts to a limited set of Suno-
-provided, fully synthetic options to choose from for each language. Specify
-following the pattern: `{lang_code}_speaker_{0-9}`. ```python text_prompt = """
-I have a silky smooth voice, and today I will tell you about the exercise
-regimen of the common sloth. """ audio_array = generate_audio(text_prompt,
-history_prompt="en_speaker_1") ``` [sloth.webm](https://user-
-images.githubusercontent.com/5068315/230684883-a344c619-a560-4ff5-8b99-
-b4463a34487b.webm) *Note: since Bark recognizes languages automatically from
-input text, it is possible to use for example a german history prompt with
-english text. This usually leads to english audio with a german accent.* ###
-ð¥ Speaker Prompts You can provide certain speaker prompts such as NARRATOR,
-MAN, WOMAN, etc. Please note that these are not always respected, especially if
-a conflicting audio history prompt is given. ```python text_prompt = """ WOMAN:
-I would like an oatmilk latte please. MAN: Wow, that's expensive! """
-audio_array = generate_audio(text_prompt) ``` [latte.webm](https://user-
-images.githubusercontent.com/5068315/230684864-12d101a1-a726-471d-9d56-
-d18b108efcb8.webm) ## ð» Installation ``` pip install git+https://github.com/
-suno-ai/bark.git ``` or ``` git clone https://github.com/suno-ai/bark cd bark
-&& pip install . ``` ## ð ï¸ Hardware and Inference Speed Bark has been
-tested and works on both CPU and GPU (`pytorch 2.0+`, CUDA 11.7 and CUDA 12.0).
-Running Bark requires running >100M parameter transformer models. On modern
-GPUs and PyTorch nightly, Bark can generate audio in roughly realtime. On older
-GPUs, default colab, or CPU, inference time might be 10-100x slower. If you
-don't have new hardware available or if you want to play with bigger versions
-of our models, you can also sign up for early access to our model playground
-[here](https://3os84zs17th.typeform.com/suno-studio). ## âï¸ Details Similar
-to [Vall-E](https://arxiv.org/abs/2301.02111) and some other amazing work in
-the field, Bark uses GPT-style models to generate audio from scratch. Different
-from Vall-E, the initial text prompt is embedded into high-level semantic
-tokens without the use of phonemes. It can therefore generalize to arbitrary
-instructions beyond speech that occur in the training data, such as music
-lyrics, sound effects or other non-speech sounds. A subsequent second model is
-used to convert the generated semantic tokens into audio codec tokens to
-generate the full waveform. To enable the community to use Bark via public code
-we used the fantastic [EnCodec codec](https://github.com/facebookresearch/
-encodec) from Facebook to act as an audio representation. Below is a list of
-some known non-speech sounds, but we are finding more every day. Please let us
-know if you find patterns that work particularly well on [Discord](https://
-discord.gg/J2B2vsjKuE)! - `[laughter]` - `[laughs]` - `[sighs]` - `[music]` - `
-[gasps]` - `[clears throat]` - `â` or `...` for hesitations - `âª` for song
-lyrics - capitalization for emphasis of a word - `MAN/WOMAN:` for bias towards
-speaker **Supported Languages** | Language | Status | | --- | --- | | English
-(en) | â | | German (de) | â | | Spanish (es) | â | | French (fr) | â |
-| Hindi (hi) | â | | Italian (it) | â | | Japanese (ja) | â | | Korean
-(ko) | â | | Polish (pl) | â | | Portuguese (pt) | â | | Russian (ru) |
-â | | Turkish (tr) | â | | Chinese, simplified (zh) | â | | Arabic |
-Coming soon! | | Bengali | Coming soon! | | Telugu | Coming soon! | ## ð
-Appreciation - [nanoGPT](https://github.com/karpathy/nanoGPT) for a dead-simple
-and blazing fast implementation of GPT-style models - [EnCodec](https://
+## ð Updates **2023.05.01** - Â©ï¸ Bark is now licensed under the MIT
+License, meaning it's now available for commercial use! - â¡ 2x speed-up on
+GPU. 10x speed-up on CPU. We also added an option for a smaller version of
+Bark, which offers additional speed-up with the trade-off of slightly lower
+quality. - ð [Long-form generation](notebooks/long_form_generation.ipynb),
+voice consistency enhancements and other examples are now documented in a new
+[notebooks](./notebooks) section. - ð¥ We created a [voice prompt library]
+(https://suno-ai.notion.site/
+8b8e8749ed514b0cbf3f699013548683?v=bc67cff786b04b50b3ceb756fd05f68c). We hope
+this resource helps you find useful prompts for your use cases! You can also
+join us on [Discord](https://discord.gg/J2B2vsjKuE), where the community
+actively shares useful prompts in the **#audio-prompts** channel. - ð¬
+Growing community support and access to new features here: [![](https://
+dcbadge.vercel.app/api/server/J2B2vsjKuE)](https://discord.gg/J2B2vsjKuE) -
+ð¾ You can now use Bark with GPUs that have low VRAM (<4GB). **2023.04.20** -
+ð¶ Bark release! ## ð Usage in Python
+**** ðª Basics ****
+```python from bark import SAMPLE_RATE, generate_audio, preload_models from
+scipy.io.wavfile import write as write_wav from IPython.display import Audio #
+download and load all models preload_models() # generate audio from text
+text_prompt = """ Hello, my name is Suno. And, uh â and I like pizza.
+[laughs] But I also have other interests such as playing tic tac toe. """
+audio_array = generate_audio(text_prompt) # save audio to disk write_wav
+("bark_generation.wav", SAMPLE_RATE, audio_array) # play text in notebook Audio
+(audio_array, rate=SAMPLE_RATE) ``` [pizza.webm](https://user-
+images.githubusercontent.com/5068315/230490503-417e688d-5115-4eee-9550-
+b46a2b465ee3.webm)
+**** ð Foreign Language ****
+
+Bark supports various languages out-of-the-box and automatically determines
+language from input text. When prompted with code-switched text, Bark will
+attempt to employ the native accent for the respective languages. English
+quality is best for the time being, and we expect other languages to further
+improve with scaling.
+
+```python text_prompt = """ ì¶ìì ë´ê° ê°ì¥ ì¢ìíë ëªì ì´ë¤.
+ëë ë©°ì¹  ëì í´ìì ì·¨íê³  ì¹êµ¬ ë° ê°ì¡±ê³¼ ìê°ì ë³´ë¼
+ì ììµëë¤. """ audio_array = generate_audio(text_prompt) ```
+[suno_korean.webm](https://user-images.githubusercontent.com/32879321/
+235313033-dc4477b9-2da0-4b94-9c8b-a8c2d8f5bb5e.webm) *Note: since Bark
+recognizes languages automatically from input text, it is possible to use for
+example a german history prompt with english text. This usually leads to
+english audio with a german accent.*
+**** ð¶ Music ****
+Bark can generate all types of audio, and, in principle, doesn't see a
+difference between speech and music. Sometimes Bark chooses to generate text as
+music, but you can help it out by adding music notes around your lyrics.
+
+```python text_prompt = """ âª In the jungle, the mighty jungle, the lion
+barks tonight âª """ audio_array = generate_audio(text_prompt) ``` [lion.webm]
+(https://user-images.githubusercontent.com/5068315/230684766-97f5ea23-ad99-
+473c-924b-66b6fab24289.webm)
+**** ð¤ Voice Presets ****
+Bark supports 100+ speaker presets across [supported languages](#supported-
+languages). You can browse the library of speaker presets [here](https://suno-
+ai.notion.site/
+8b8e8749ed514b0cbf3f699013548683?v=bc67cff786b04b50b3ceb756fd05f68c), or in the
+[code](bark/assets/prompts). The community also often shares presets in
+[Discord](https://discord.gg/J2B2vsjKuE). Bark tries to match the tone, pitch,
+emotion and prosody of a given preset, but does not currently support custom
+voice cloning. The model also attempts to preserve music, ambient noise, etc.
+
+```python text_prompt = """ I have a silky smooth voice, and today I will tell
+you about the exercise regimen of the common sloth. """ audio_array =
+generate_audio(text_prompt, history_prompt="v2/en_speaker_1") ``` [sloth.webm]
+(https://user-images.githubusercontent.com/5068315/230684883-a344c619-a560-
+4ff5-8b99-b4463a34487b.webm)  ### Generating Longer Audio By default,
+`generate_audio` works well with around 13 seconds of spoken text. For an
+example of how to do long-form generation, see this [example notebook]
+(notebooks/long_form_generation.ipynb).  Click to toggle example long-form
+generations (from the example notebook) [dialog.webm](https://user-
+images.githubusercontent.com/2565833/235463539-f57608da-e4cb-4062-8771-
+148e29512b01.webm) [longform_advanced.webm](https://user-
+images.githubusercontent.com/2565833/235463547-1c0d8744-269b-43fe-9630-
+897ea5731652.webm) [longform_basic.webm](https://user-
+images.githubusercontent.com/2565833/235463559-87efe9f8-a2db-4d59-b764-
+57db83f95270.webm)  ## ð» Installation ``` pip install git+https://
+github.com/suno-ai/bark.git ``` or ``` git clone https://github.com/suno-ai/
+bark cd bark && pip install . ``` *Note: Do NOT use 'pip install bark'. It
+installs a different package, which is not managed by Suno.* ## ð ï¸
+Hardware and Inference Speed Bark has been tested and works on both CPU and GPU
+(`pytorch 2.0+`, CUDA 11.7 and CUDA 12.0). On enterprise GPUs and PyTorch
+nightly, Bark can generate audio in roughly real-time. On older GPUs, default
+colab, or CPU, inference time might be significantly slower. For older GPUs or
+CPU you might want to consider using smaller models. Details can be found in
+out tutorial sections here. The full version of Bark requires around 12GB of
+VRAM to hold everything on GPU at the same time. To use a smaller version of
+the models, which should fit into 8GB VRAM, set the environment flag
+`SUNO_USE_SMALL_MODELS=True`. If you don't have hardware available or if you
+want to play with bigger versions of our models, you can also sign up for early
+access to our model playground [here](https://3os84zs17th.typeform.com/suno-
+studio). ## âï¸ Details Bark is fully generative tex-to-audio model devolved
+for research and demo purposes. It follows a GPT style architecture similar to
+[AudioLM](https://arxiv.org/abs/2209.03143) and [Vall-E](https://arxiv.org/abs/
+2301.02111) and a quantized Audio representation from [EnCodec](https://
+github.com/facebookresearch/encodec). It is not a conventional TTS model, but
+instead a fully generative text-to-audio model capable of deviating in
+unexpected ways from any given script. Different to previous approaches, the
+input text prompt is converted directly to audio without the intermediate use
+of phonemes. It can therefore generalize to arbitrary instructions beyond
+speech such as music lyrics, sound effects or other non-speech sounds. Below is
+a list of some known non-speech sounds, but we are finding more every day.
+Please let us know if you find patterns that work particularly well on
+[Discord](https://discord.gg/J2B2vsjKuE)! - `[laughter]` - `[laughs]` - `
+[sighs]` - `[music]` - `[gasps]` - `[clears throat]` - `â` or `...` for
+hesitations - `âª` for song lyrics - CAPITALIZATION for emphasis of a word - `
+[MAN]` and `[WOMAN]` to bias Bark toward male and female speakers, respectively
+### Supported Languages | Language | Status | | --- | --- | | English (en) |
+â | | German (de) | â | | Spanish (es) | â | | French (fr) | â | |
+Hindi (hi) | â | | Italian (it) | â | | Japanese (ja) | â | | Korean (ko)
+| â | | Polish (pl) | â | | Portuguese (pt) | â | | Russian (ru) | â |
+| Turkish (tr) | â | | Chinese, simplified (zh) | â | Requests for future
+language support [here](https://github.com/suno-ai/bark/discussions/111) or in
+the **#forums** channel on [Discord](https://discord.com/invite/J2B2vsjKuE). ##
+ð Appreciation - [nanoGPT](https://github.com/karpathy/nanoGPT) for a dead-
+simple and blazing fast implementation of GPT-style models - [EnCodec](https://
 github.com/facebookresearch/encodec) for a state-of-the-art implementation of a
 fantastic audio codec - [AudioLM](https://github.com/lucidrains/audiolm-
-pytorch) for very related training and inference code - [Vall-E](https://
-arxiv.org/abs/2301.02111), [AudioLM](https://arxiv.org/abs/2209.03143) and many
-other ground-breaking papers that enabled the development of Bark ## Â© License
-Bark is licensed under a non-commercial license: CC-BY 4.0 NC. The Suno models
-themselves may be used commercially. However, this version of Bark uses
-`EnCodec` as a neural codec backend, which is licensed under a [non-commercial
-license](https://github.com/facebookresearch/encodec/blob/main/LICENSE). Please
-contact us at `bark@suno.ai` if you need access to a larger version of the
-model and/or a version of the model you can use commercially. ##
-ð±Â Community - [Twitter](https://twitter.com/OnusFM) - [Discord](https://
-discord.gg/J2B2vsjKuE) ## ð§Â Suno Studio (Early Access) Weâre developing a
-playground for our models, including Bark. If you are interested, you can sign
-up for early access [here](https://3os84zs17th.typeform.com/suno-studio). ##
-FAQ #### How do I specify where models are downloaded and cached? Use the
-`XDG_CACHE_HOME` env variable to override where models are downloaded and
-cached (otherwise defaults to a subdirectory of `~/.cache`). #### Bark's
-generations sometimes differ from my prompts. What's happening? Bark is a GPT-
-style model. As such, it may take some creative liberties in its generations,
-resulting in higher-variance model outputs than traditional text-to-speech
-approaches.
+pytorch) for related training and inference code - [Vall-E](https://arxiv.org/
+abs/2301.02111), [AudioLM](https://arxiv.org/abs/2209.03143) and many other
+ground-breaking papers that enabled the development of Bark ## Â© License Bark
+is licensed under the MIT License. Please contact us at `bark@suno.ai` to
+request access to a larger version of the model. ## ð±Â Community - [Twitter]
+(https://twitter.com/OnusFM) - [Discord](https://discord.gg/J2B2vsjKuE) ##
+ð§Â Suno Studio (Early Access) Weâre developing a playground for our
+models, including Bark. If you are interested, you can sign up for early access
+[here](https://3os84zs17th.typeform.com/suno-studio). ## â FAQ #### How do I
+specify where models are downloaded and cached? * Bark uses Hugging Face to
+download and store models. You can see find more info [here](https://
+huggingface.co/docs/huggingface_hub/package_reference/
+environment_variables#hfhome). #### Bark's generations sometimes differ from my
+prompts. What's happening? * Bark is a GPT-style model. As such, it may take
+some creative liberties in its generations, resulting in higher-variance model
+outputs than traditional text-to-speech approaches. #### What voices are
+supported by Bark? * Bark supports 100+ speaker presets across [supported
+languages](#supported-languages). You can browse the library of speaker presets
+[here](https://suno-ai.notion.site/
+8b8e8749ed514b0cbf3f699013548683?v=bc67cff786b04b50b3ceb756fd05f68c). The
+community also shares presets in [Discord](https://discord.gg/J2B2vsjKuE). Bark
+also supports generating unique random voices that fit the input text. Bark
+does not currently support custom voice cloning. #### Why is the output limited
+to ~13-14 seconds? * Bark is a GPT-style model, and its architecture/context
+window is optimized to output generations with roughly this length. #### How
+much VRAM do I need? * The full version of Bark requires around 12Gb of memory
+to hold everything on GPU at the same time. However, even smaller cards down to
+~2Gb work with some additional settings. Simply add the following code snippet
+before your generation: ```python import os os.environ["SUNO_OFFLOAD_CPU"] =
+True os.environ["SUNO_USE_SMALL_MODELS"] = True ``` #### My generated audio
+sounds like a 1980s phone call. What's happening? * Bark generates audio from
+scratch. It is not meant to create only high-fidelity, studio-quality speech.
+Rather, outputs could be anything from perfect speech to multiple people
+arguing at a baseball game recorded with bad microphones.
```

### Comparing `bark-0.0.1a0/bark/api.py` & `bark-0.1.5/bark/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional
+from typing import Dict, Optional, Union
 
 import numpy as np
 
 from .generation import codec_decode, generate_coarse, generate_fine, generate_text_semantic
 
 
 def text_to_semantic(
     text: str,
-    history_prompt: Optional[str] = None,
+    history_prompt: Optional[Union[Dict, str]] = None,
     temp: float = 0.7,
     silent: bool = False,
 ):
     """Generate semantic array from text.
 
     Args:
         text: text to be turned into audio
@@ -30,15 +30,15 @@
         use_kv_caching=True
     )
     return x_semantic
 
 
 def semantic_to_waveform(
     semantic_tokens: np.ndarray,
-    history_prompt: Optional[str] = None,
+    history_prompt: Optional[Union[Dict, str]] = None,
     temp: float = 0.7,
     silent: bool = False,
     output_full: bool = False,
 ):
     """Generate audio array from semantic input.
 
     Args:
@@ -81,15 +81,15 @@
     assert("coarse_prompt" in full_generation)
     assert("fine_prompt" in full_generation)
     np.savez(filepath, **full_generation)
 
 
 def generate_audio(
     text: str,
-    history_prompt: Optional[str] = None,
+    history_prompt: Optional[Union[Dict, str]] = None,
     text_temp: float = 0.7,
     waveform_temp: float = 0.7,
     silent: bool = False,
     output_full: bool = False,
 ):
     """Generate audio array from input text.
```

### Comparing `bark-0.0.1a0/bark/assets/prompts/announcer.npz` & `bark-0.1.5/bark/assets/prompts/announcer.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/de_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/en_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/es_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/fr_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/hi_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/it_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ja_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ko_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pl_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/pt_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/ru_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/tr_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_0.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_1.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_2.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_3.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_4.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_5.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_6.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_7.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_8.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/assets/prompts/zh_speaker_9.npz` & `bark-0.1.5/bark/assets/prompts/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/generation.py` & `bark-0.1.5/bark/generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import contextlib
 import gc
-import hashlib
 import os
 import re
-import requests
 
 from encodec import EncodecModel
 import funcy
 import logging
 import numpy as np
 from scipy.special import softmax
 import torch
@@ -68,109 +66,94 @@
     ("Russian", "ru"),
     ("Turkish", "tr"),
     ("Chinese", "zh"),
 ]
 
 ALLOWED_PROMPTS = {"announcer"}
 for _, lang in SUPPORTED_LANGS:
-    for n in range(10):
-        ALLOWED_PROMPTS.add(f"{lang}_speaker_{n}")
+    for prefix in ("", f"v2{os.path.sep}"):
+        for n in range(10):
+            ALLOWED_PROMPTS.add(f"{prefix}{lang}_speaker_{n}")
 
 
 logger = logging.getLogger(__name__)
 
 
 CUR_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 default_cache_dir = os.path.join(os.path.expanduser("~"), ".cache")
 CACHE_DIR = os.path.join(os.getenv("XDG_CACHE_HOME", default_cache_dir), "suno", "bark_v0")
 
 
-USE_SMALL_MODELS = os.environ.get("SUNO_USE_SMALL_MODELS", False)
-GLOBAL_ENABLE_MPS = os.environ.get("SUNO_ENABLE_MPS", False)
-OFFLOAD_CPU = os.environ.get("SUNO_OFFLOAD_CPU", False)
+def _cast_bool_env_var(s):
+    return s.lower() in ('true', '1', 't')
+
+
+USE_SMALL_MODELS = _cast_bool_env_var(os.environ.get("SUNO_USE_SMALL_MODELS", "False"))
+GLOBAL_ENABLE_MPS = _cast_bool_env_var(os.environ.get("SUNO_ENABLE_MPS", "False"))
+OFFLOAD_CPU = _cast_bool_env_var(os.environ.get("SUNO_OFFLOAD_CPU", "False"))
 
 
 REMOTE_MODEL_PATHS = {
     "text_small": {
         "repo_id": "suno/bark",
         "file_name": "text.pt",
-        "checksum": "b3e42bcbab23b688355cd44128c4cdd3",
     },
     "coarse_small": {
         "repo_id": "suno/bark",
         "file_name": "coarse.pt",
-        "checksum": "5fe964825e3b0321f9d5f3857b89194d",
     },
     "fine_small": {
         "repo_id": "suno/bark",
         "file_name": "fine.pt",
-        "checksum": "5428d1befe05be2ba32195496e58dc90",
     },
     "text": {
         "repo_id": "suno/bark",
         "file_name": "text_2.pt",
-        "checksum": "54afa89d65e318d4f5f80e8e8799026a",
     },
     "coarse": {
         "repo_id": "suno/bark",
         "file_name": "coarse_2.pt",
-        "checksum": "8a98094e5e3a255a5c9c0ab7efe8fd28",
     },
     "fine": {
         "repo_id": "suno/bark",
         "file_name": "fine_2.pt",
-        "checksum": "59d184ed44e3650774a2f0503a48a97b",
     },
 }
 
 
 if not hasattr(torch.nn.functional, 'scaled_dot_product_attention') and torch.cuda.is_available():
     logger.warning(
         "torch version does not support flash attention. You will get faster" +
         " inference speed by upgrade torch to newest nightly version."
     )
 
 
-def _string_md5(s):
-    m = hashlib.md5()
-    m.update(s.encode("utf-8"))
-    return m.hexdigest()
-
-
-def _md5(fname):
-    hash_md5 = hashlib.md5()
-    with open(fname, "rb") as f:
-        for chunk in iter(lambda: f.read(4096), b""):
-            hash_md5.update(chunk)
-    return hash_md5.hexdigest()
-
-
-def _get_ckpt_path(model_type, use_small=False):
-    model_key = f"{model_type}_small" if use_small or USE_SMALL_MODELS else model_type
-    model_name = _string_md5(REMOTE_MODEL_PATHS[model_key]["file_name"])
-    return os.path.join(CACHE_DIR, f"{model_name}.pt")
-
-
 def _grab_best_device(use_gpu=True):
     if torch.cuda.device_count() > 0 and use_gpu:
         device = "cuda"
     elif torch.backends.mps.is_available() and use_gpu and GLOBAL_ENABLE_MPS:
         device = "mps"
     else:
         device = "cpu"
     return device
 
 
-def _download(from_hf_path, file_name, to_local_path):
+def _get_ckpt_path(model_type, use_small=False):
+    key = model_type
+    if use_small or USE_SMALL_MODELS:
+        key += "_small"
+    return os.path.join(CACHE_DIR, REMOTE_MODEL_PATHS[key]["file_name"])
+
+
+def _download(from_hf_path, file_name):
     os.makedirs(CACHE_DIR, exist_ok=True)
-    destination_file_name = to_local_path.split("/")[-1]
     hf_hub_download(repo_id=from_hf_path, filename=file_name, local_dir=CACHE_DIR)
-    os.replace(os.path.join(CACHE_DIR, file_name), to_local_path)
+
 
 class InferenceContext:
     def __init__(self, benchmark=False):
         # we can't expect inputs to be the same length, so disable benchmarking by default
         self._chosen_cudnn_benchmark = benchmark
         self._cudnn_benchmark = None
 
@@ -219,23 +202,17 @@
     elif model_type == "fine":
         ConfigClass = FineGPTConfig
         ModelClass = FineGPT
     else:
         raise NotImplementedError()
     model_key = f"{model_type}_small" if use_small or USE_SMALL_MODELS else model_type
     model_info = REMOTE_MODEL_PATHS[model_key]
-    if (
-        os.path.exists(ckpt_path) and
-        _md5(ckpt_path) != model_info["checksum"]
-    ):
-        logger.warning(f"found outdated {model_type} model, removing.")
-        os.remove(ckpt_path)
     if not os.path.exists(ckpt_path):
         logger.info(f"{model_type} model not found, downloading into `{CACHE_DIR}`.")
-        _download(model_info["repo_id"], model_info["file_name"], ckpt_path)
+        _download(model_info["repo_id"], model_info["file_name"])
     checkpoint = torch.load(ckpt_path, map_location=device)
     # this is a hack
     model_args = checkpoint["model_args"]
     if "input_vocab_size" not in model_args:
         model_args["input_vocab_size"] = model_args["vocab_size"]
         model_args["output_vocab_size"] = model_args["vocab_size"]
         del model_args["vocab_size"]
@@ -372,14 +349,35 @@
 
 TEXT_ENCODING_OFFSET = 10_048
 SEMANTIC_PAD_TOKEN = 10_000
 TEXT_PAD_TOKEN = 129_595
 SEMANTIC_INFER_TOKEN = 129_599
 
 
+def _load_history_prompt(history_prompt_input):
+    if isinstance(history_prompt_input, str) and history_prompt_input.endswith(".npz"):
+        history_prompt = np.load(history_prompt_input)
+    elif isinstance(history_prompt_input, str):
+        # make sure this works on non-ubuntu
+        history_prompt_input = os.path.join(*history_prompt_input.split("/"))
+        if history_prompt_input not in ALLOWED_PROMPTS:
+            raise ValueError("history prompt not found")
+        history_prompt = np.load(
+            os.path.join(CUR_PATH, "assets", "prompts", f"{history_prompt_input}.npz")
+        )
+    elif isinstance(history_prompt_input, dict):
+        assert("semantic_prompt" in history_prompt_input)
+        assert("coarse_prompt" in history_prompt_input)
+        assert("fine_prompt" in history_prompt_input)
+        history_prompt = history_prompt_input
+    else:
+        raise ValueError("history prompt format unrecognized")
+    return history_prompt
+
+
 def generate_text_semantic(
     text,
     history_prompt=None,
     temp=0.7,
     top_k=None,
     top_p=None,
     silent=False,
@@ -389,21 +387,16 @@
     use_kv_caching=False,
 ):
     """Generate semantic tokens from text."""
     assert isinstance(text, str)
     text = _normalize_whitespace(text)
     assert len(text.strip()) > 0
     if history_prompt is not None:
-        if history_prompt.endswith(".npz"):
-            semantic_history = np.load(history_prompt)["semantic_prompt"]
-        else:
-            assert (history_prompt in ALLOWED_PROMPTS)
-            semantic_history = np.load(
-                os.path.join(CUR_PATH, "assets", "prompts", f"{history_prompt}.npz")
-            )["semantic_prompt"]
+        history_prompt = _load_history_prompt(history_prompt)
+        semantic_history = history_prompt["semantic_prompt"]
         assert (
             isinstance(semantic_history, np.ndarray)
             and len(semantic_history.shape) == 1
             and len(semantic_history) > 0
             and semantic_history.min() >= 0
             and semantic_history.max() <= SEMANTIC_VOCAB_SIZE - 1
         )
@@ -558,23 +551,17 @@
         and x_semantic.max() <= SEMANTIC_VOCAB_SIZE - 1
     )
     assert 60 <= max_coarse_history <= 630
     assert max_coarse_history + sliding_window_len <= 1024 - 256
     semantic_to_coarse_ratio = COARSE_RATE_HZ / SEMANTIC_RATE_HZ * N_COARSE_CODEBOOKS
     max_semantic_history = int(np.floor(max_coarse_history / semantic_to_coarse_ratio))
     if history_prompt is not None:
-        if history_prompt.endswith(".npz"):
-            x_history = np.load(history_prompt)
-        else:
-            assert (history_prompt in ALLOWED_PROMPTS)
-            x_history = np.load(
-                os.path.join(CUR_PATH, "assets", "prompts", f"{history_prompt}.npz")
-            )
-        x_semantic_history = x_history["semantic_prompt"]
-        x_coarse_history = x_history["coarse_prompt"]
+        history_prompt = _load_history_prompt(history_prompt)
+        x_semantic_history = history_prompt["semantic_prompt"]
+        x_coarse_history = history_prompt["coarse_prompt"]
         assert (
             isinstance(x_semantic_history, np.ndarray)
             and len(x_semantic_history.shape) == 1
             and len(x_semantic_history) > 0
             and x_semantic_history.min() >= 0
             and x_semantic_history.max() <= SEMANTIC_VOCAB_SIZE - 1
             and isinstance(x_coarse_history, np.ndarray)
@@ -723,21 +710,16 @@
         and len(x_coarse_gen.shape) == 2
         and 1 <= x_coarse_gen.shape[0] <= N_FINE_CODEBOOKS - 1
         and x_coarse_gen.shape[1] > 0
         and x_coarse_gen.min() >= 0
         and x_coarse_gen.max() <= CODEBOOK_SIZE - 1
     )
     if history_prompt is not None:
-        if history_prompt.endswith(".npz"):
-            x_fine_history = np.load(history_prompt)["fine_prompt"]
-        else:
-            assert (history_prompt in ALLOWED_PROMPTS)
-            x_fine_history = np.load(
-                os.path.join(CUR_PATH, "assets", "prompts", f"{history_prompt}.npz")
-            )["fine_prompt"]
+        history_prompt = _load_history_prompt(history_prompt)
+        x_fine_history = history_prompt["fine_prompt"]
         assert (
             isinstance(x_fine_history, np.ndarray)
             and len(x_fine_history.shape) == 2
             and x_fine_history.shape[0] == N_FINE_CODEBOOKS
             and x_fine_history.shape[1] >= 0
             and x_fine_history.min() >= 0
             and x_fine_history.max() <= CODEBOOK_SIZE - 1
```

### Comparing `bark-0.0.1a0/bark/model.py` & `bark-0.1.5/bark/model.py`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/bark/model_fine.py` & `bark-0.1.5/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `bark-0.0.1a0/pyproject.toml` & `bark-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bark"
-version = "0.0.1a"
+version = "0.1.5"
 description = "Bark text to audio model"
 readme = "README.md"
 requires-python = ">=3.8"
 authors =  [
     {name = "Suno Inc", email = "hello@suno.ai"},
 ]
-# Apache 2.0
+
 license = {file = "LICENSE"}
 
 dependencies = [
     "boto3",
     "encodec",
     "funcy",
+    "huggingface-hub>=0.14.1",
     "numpy",
     "scipy",
     "tokenizers",
     "torch",
     "tqdm",
     "transformers",
 ]
@@ -31,15 +32,14 @@
 
 [project.optional-dependencies]
 dev = [
     "bandit",
     "black",
     "codecov",
     "flake8",
-    "huggingface-hub",
     "hypothesis>=6.14,<7",
     "isort>=5.0.0,<6",
     "jupyter",
     "mypy",
     "nbconvert",
     "nbformat",
     "pydocstyle",
@@ -48,11 +48,12 @@
     "pytest-cov",
 ]
 
 [tool.setuptools]
 packages = ["bark"]
 
 [tool.setuptools.package-data]
-bark = ["assets/prompts/*.npz"]
+bark = ["assets/prompts/*.npz", "assets/prompts/v2/*.npz"]
+
 
 [tool.black]
 line-length = 100
```

