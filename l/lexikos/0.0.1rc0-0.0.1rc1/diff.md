# Comparing `tmp/lexikos-0.0.1rc0.tar.gz` & `tmp/lexikos-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc0.tar", last modified: Wed May  3 04:15:15 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc1.tar", last modified: Tue May  9 09:59:02 2023, max compression
```

## Comparing `lexikos-0.0.1rc0.tar` & `lexikos-0.0.1rc1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.481010 lexikos-0.0.1rc0/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc0/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc0/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    26127 2023-05-03 04:15:15.481446 lexikos-0.0.1rc0/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    12403 2023-05-03 04:06:40.000000 lexikos-0.0.1rc0/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.425787 lexikos-0.0.1rc0/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)       75 2023-05-03 04:09:34.000000 lexikos-0.0.1rc0/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.423361 lexikos-0.0.1rc0/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.428685 lexikos-0.0.1rc0/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc0/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.479429 lexikos-0.0.1rc0/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_in_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2172 2023-05-03 04:02:24.000000 lexikos-0.0.1rc0/lexikos/lexicon.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-03 04:15:15.428199 lexikos-0.0.1rc0/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    26127 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)      851 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-05-03 04:15:15.000000 lexikos-0.0.1rc0/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      819 2023-05-03 04:09:32.000000 lexikos-0.0.1rc0/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-05-03 04:15:15.482369 lexikos-0.0.1rc0/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc0/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.336356 lexikos-0.0.1rc1/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc1/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc1/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    27155 2023-05-09 09:59:02.336612 lexikos-0.0.1rc1/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    13431 2023-05-09 09:56:15.000000 lexikos-0.0.1rc1/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.300489 lexikos-0.0.1rc1/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)       77 2023-05-09 09:58:42.000000 lexikos-0.0.1rc1/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.297810 lexikos-0.0.1rc1/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.308823 lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.335995 lexikos-0.0.1rc1/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2911 2023-05-09 09:56:54.000000 lexikos-0.0.1rc1/lexikos/lexicon.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-09 09:59:02.302199 lexikos-0.0.1rc1/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    27155 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)      923 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-05-09 09:59:02.000000 lexikos-0.0.1rc1/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      821 2023-05-09 09:58:55.000000 lexikos-0.0.1rc1/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-05-09 09:59:02.337157 lexikos-0.0.1rc1/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc1/setup.py
```

### Comparing `lexikos-0.0.1rc0/LICENSE` & `lexikos-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/PKG-INFO` & `lexikos-0.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -238,23 +238,53 @@
 ```sh
 git clone https://github.com/bookbot-hive/lexikos.git
 pip install -e lexikos
 ```
 
 ## Usage
 
+### Lexicon
+
 ```py
 >>> from lexikos import Lexicon
 >>> lexicon = Lexicon()
 >>> print(lexicon["added"])
-{'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ d ɪ d', 'a d ɪ d', 'a d ə d', 'ˈæ ɾ ə d', 'ˈæ d ə d', 'æ d ɪ d', 'æ ɾ ə d', 'æ d ə d', 'ˈa d ɪ d', 'ˈa d ə d'}
+{'ˈæ d ɪ d', 'ˈæ ɾ ə d', 'æ ɾ ɪ d', 'a d ɪ d', 'ˈa d ɪ d', 'æ ɾ ə d', 'ˈa d ə d', 'a d ə d', 'ˈæ d ə d', 'æ d ə d', 'æ d ɪ d', 'ˈæ ɾ ɪ d'}
 >>> print(lexicon["runner"])
-{'ɹ ʌ n ə', 'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ'}
+{'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'ɹ ʌ n ɝ', 'ˈr ʌ n ɝ'}
 >>> print(lexicon["water"])
-{'ˈw oː t ə', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɑ ɾ ɚ', 'ˈw ɔ t ɝ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'ˈʋ aː ʈ ə r ɯ', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ ʈ ə r', 'ˈw oː ɾ ə', 'w ɔː t ə'}
+{'ˈʋ aː ʈ ə r ɯ', 'ˈw oː t ə', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ t ɝ', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɔ t ɝ', 'w ɑ ɾ ɚ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɔː t ə', 'ˈw oː ɾ ə', 'ˈw ɔ ʈ ə r'}
+```
+
+To get a lexicon where phonemes are normalized (diacritics removed, digraphs split):
+
+```py
+>>> from lexikos import Lexicon
+>>> lexicon = Lexicon(normalize_phonemes=True)
+>>> print(lexicon["added"])
+{'æ ɾ ɪ d', 'a d ɪ d', 'a d ə d', 'æ ɾ ə d', 'æ d ə d', 'æ d ɪ d'}
+>>> print(lexicon["runner"])
+{'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'r ʌ n ɝ', 'ɹ ʌ n ɝ'}
+>>> print(lexicon["water"])
+{'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
+```
+
+### Phonemization
+
+```py
+>>> from transformers import pipeline
+>>> import torch
+>>> g2p = pipeline(
+...     model="bookbot/byt5-small-wikipron-eng-latn-us-broad",
+...     device=0 if torch.cuda.is_available() else -1,
+... )
+>>> g2p("phonemizing", max_length=200)[0]['generated_text']
+'f o ʊ n ə m a ɪ z ɪ ŋ'
+>>> g2p("imposimpable", max_length=200)[0]['generated_text']
+'ɪ m p ə z ɪ m p ə b ə l'
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
```

### Comparing `lexikos-0.0.1rc0/README.md` & `lexikos-0.0.1rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,23 +19,53 @@
 ```sh
 git clone https://github.com/bookbot-hive/lexikos.git
 pip install -e lexikos
 ```
 
 ## Usage
 
+### Lexicon
+
 ```py
 >>> from lexikos import Lexicon
 >>> lexicon = Lexicon()
 >>> print(lexicon["added"])
-{'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ d ɪ d', 'a d ɪ d', 'a d ə d', 'ˈæ ɾ ə d', 'ˈæ d ə d', 'æ d ɪ d', 'æ ɾ ə d', 'æ d ə d', 'ˈa d ɪ d', 'ˈa d ə d'}
+{'ˈæ d ɪ d', 'ˈæ ɾ ə d', 'æ ɾ ɪ d', 'a d ɪ d', 'ˈa d ɪ d', 'æ ɾ ə d', 'ˈa d ə d', 'a d ə d', 'ˈæ d ə d', 'æ d ə d', 'æ d ɪ d', 'ˈæ ɾ ɪ d'}
 >>> print(lexicon["runner"])
-{'ɹ ʌ n ə', 'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ'}
+{'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'ɹ ʌ n ɝ', 'ˈr ʌ n ɝ'}
 >>> print(lexicon["water"])
-{'ˈw oː t ə', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɑ ɾ ɚ', 'ˈw ɔ t ɝ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'ˈʋ aː ʈ ə r ɯ', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ ʈ ə r', 'ˈw oː ɾ ə', 'w ɔː t ə'}
+{'ˈʋ aː ʈ ə r ɯ', 'ˈw oː t ə', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ t ɝ', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɔ t ɝ', 'w ɑ ɾ ɚ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɔː t ə', 'ˈw oː ɾ ə', 'ˈw ɔ ʈ ə r'}
+```
+
+To get a lexicon where phonemes are normalized (diacritics removed, digraphs split):
+
+```py
+>>> from lexikos import Lexicon
+>>> lexicon = Lexicon(normalize_phonemes=True)
+>>> print(lexicon["added"])
+{'æ ɾ ɪ d', 'a d ɪ d', 'a d ə d', 'æ ɾ ə d', 'æ d ə d', 'æ d ɪ d'}
+>>> print(lexicon["runner"])
+{'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'r ʌ n ɝ', 'ɹ ʌ n ɝ'}
+>>> print(lexicon["water"])
+{'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
+```
+
+### Phonemization
+
+```py
+>>> from transformers import pipeline
+>>> import torch
+>>> g2p = pipeline(
+...     model="bookbot/byt5-small-wikipron-eng-latn-us-broad",
+...     device=0 if torch.cuda.is_available() else -1,
+... )
+>>> g2p("phonemizing", max_length=200)[0]['generated_text']
+'f o ʊ n ə m a ɪ z ɪ ŋ'
+>>> g2p("imposimpable", max_length=200)[0]['generated_text']
+'ɪ m p ə z ɪ m p ə b ə l'
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
```

### Comparing `lexikos-0.0.1rc0/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc1/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_ca_broad.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_in_broad.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_in_narrow.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_in_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_nz_broad.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc1/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc0/lexikos/lexicon.py` & `lexikos-0.0.1rc1/lexikos/lexicon.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,29 +17,38 @@
 from typing import Any, Dict, List, Set, Union
 import os
 
 DICTIONARIES = os.path.join(os.path.dirname(__file__), "dict")
 
 
 class Lexicon(UserDict):
-    def __init__(self, dictionaries_dir: Union[Path, str] = DICTIONARIES):
+    def __init__(
+        self,
+        normalize_phonemes: bool = False,
+        dictionaries_dir: Union[Path, str] = DICTIONARIES,
+    ):
         if isinstance(dictionaries_dir, str):
             dictionaries_dir = Path(dictionaries_dir)
 
         files = list(dictionaries_dir.rglob("*/*.tsv"))
-        dicts = [self._parse_tsv(file) for file in files]
+        dicts = [self._parse_tsv(file, normalize_phonemes) for file in files]
         mapping: Dict[str, Set[str]] = self._merge_dicts(dicts)
         super().__init__(mapping)
 
-    def _parse_tsv(self, file: Union[Path, str]) -> Dict[str, Set[str]]:
+    def _parse_tsv(
+        self, file: Union[Path, str], normalize_phonemes: bool
+    ) -> Dict[str, Set[str]]:
         lex = {}
         with open(file, "r") as f:
             for line in f.readlines():
                 word, phonemes = line.strip().split("\t")
-                phonemes = [phonemes.replace(" . ", " ")]
+                phonemes = phonemes.replace(" . ", " ")
+                if normalize_phonemes:
+                    phonemes = self._normalize_phonemes(phonemes)
+                phonemes = [phonemes]
                 word = word.lower()
                 if word in lex:
                     lex[word] = lex[word].union(phonemes)
                 else:
                     lex[word] = set(phonemes)
         return lex
 
@@ -49,13 +58,23 @@
             for k, v in d.items():
                 if k in output_dict:
                     output_dict[k] = output_dict[k].union(v)
                 else:
                     output_dict[k] = v
         return output_dict
 
+    def _normalize_phonemes(self, phonemes: str) -> str:
+        """
+        Modified from: [Michael McAuliffe](https://memcauliffe.com/speaker-dictionaries-and-multilingual-ipa.html#multilingual-ipa-mode)
+        """
+        diacritics = ["ː", "ˑ", "̆", "̯", "͡", "‿", "͜", "̩", "ˈ", "ˌ"]
+        for d in diacritics:
+            phonemes = phonemes.replace(d, "")
+        phonemes = " ".join([p for p in phonemes if p != " "]).strip()
+        return phonemes
+
 
 if __name__ == "__main__":
     lexicon = Lexicon()
     print(lexicon["added"])
     print(lexicon["runner"])
     print(lexicon["water"])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lexikos-0.0.1rc0/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc1/lexikos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -238,23 +238,53 @@
 ```sh
 git clone https://github.com/bookbot-hive/lexikos.git
 pip install -e lexikos
 ```
 
 ## Usage
 
+### Lexicon
+
 ```py
 >>> from lexikos import Lexicon
 >>> lexicon = Lexicon()
 >>> print(lexicon["added"])
-{'ˈæ ɾ ɪ d', 'æ ɾ ɪ d', 'ˈæ d ɪ d', 'a d ɪ d', 'a d ə d', 'ˈæ ɾ ə d', 'ˈæ d ə d', 'æ d ɪ d', 'æ ɾ ə d', 'æ d ə d', 'ˈa d ɪ d', 'ˈa d ə d'}
+{'ˈæ d ɪ d', 'ˈæ ɾ ə d', 'æ ɾ ɪ d', 'a d ɪ d', 'ˈa d ɪ d', 'æ ɾ ə d', 'ˈa d ə d', 'a d ə d', 'ˈæ d ə d', 'æ d ə d', 'æ d ɪ d', 'ˈæ ɾ ɪ d'}
 >>> print(lexicon["runner"])
-{'ɹ ʌ n ə', 'ɹ ʌ n ɚ', 'ˈr ʌ n ɝ'}
+{'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'ɹ ʌ n ɝ', 'ˈr ʌ n ɝ'}
 >>> print(lexicon["water"])
-{'ˈw oː t ə', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɑ ɾ ɚ', 'ˈw ɔ t ɝ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'ˈʋ aː ʈ ə r ɯ', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ ʈ ə r', 'ˈw oː ɾ ə', 'w ɔː t ə'}
+{'ˈʋ aː ʈ ə r ɯ', 'ˈw oː t ə', 'w ɑ t ə ɹ', 'ˈw aː ʈ ə r ɯ', 'ˈw ɔ t ɝ', 'w ɔ t ə ɹ', 'ˈw ɑ t ə ɹ', 'w ɔ t ɝ', 'w ɑ ɾ ɚ', 'ˈw ɑ ɾ ɚ', 'ˈʋ ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɔː t ə', 'ˈw oː ɾ ə', 'ˈw ɔ ʈ ə r'}
+```
+
+To get a lexicon where phonemes are normalized (diacritics removed, digraphs split):
+
+```py
+>>> from lexikos import Lexicon
+>>> lexicon = Lexicon(normalize_phonemes=True)
+>>> print(lexicon["added"])
+{'æ ɾ ɪ d', 'a d ɪ d', 'a d ə d', 'æ ɾ ə d', 'æ d ə d', 'æ d ɪ d'}
+>>> print(lexicon["runner"])
+{'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'r ʌ n ɝ', 'ɹ ʌ n ɝ'}
+>>> print(lexicon["water"])
+{'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
+```
+
+### Phonemization
+
+```py
+>>> from transformers import pipeline
+>>> import torch
+>>> g2p = pipeline(
+...     model="bookbot/byt5-small-wikipron-eng-latn-us-broad",
+...     device=0 if torch.cuda.is_available() else -1,
+... )
+>>> g2p("phonemizing", max_length=200)[0]['generated_text']
+'f o ʊ n ə m a ɪ z ɪ ŋ'
+>>> g2p("imposimpable", max_length=200)[0]['generated_text']
+'ɪ m p ə z ɪ m p ə b ə l'
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
```

### Comparing `lexikos-0.0.1rc0/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc1/lexikos.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 lexikos/__init__.py
 lexikos/lexicon.py
 lexikos.egg-info/PKG-INFO
 lexikos.egg-info/SOURCES.txt
 lexikos.egg-info/dependency_links.txt
 lexikos.egg-info/top_level.txt
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
 lexikos/dict/wikipron/eng_latn.tsv
 lexikos/dict/wikipron/eng_latn_au_broad.tsv
 lexikos/dict/wikipron/eng_latn_au_narrow.tsv
 lexikos/dict/wikipron/eng_latn_ca_broad.tsv
 lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
 lexikos/dict/wikipron/eng_latn_in_broad.tsv
 lexikos/dict/wikipron/eng_latn_in_narrow.tsv
```

### Comparing `lexikos-0.0.1rc0/pyproject.toml` & `lexikos-0.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1c"
+version = "0.0.1rc1"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1rc0/setup.py` & `lexikos-0.0.1rc1/setup.py`

 * *Files identical despite different names*

