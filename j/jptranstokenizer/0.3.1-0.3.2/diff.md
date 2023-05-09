# Comparing `tmp/jptranstokenizer-0.3.1.tar.gz` & `tmp/jptranstokenizer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jptranstokenizer-0.3.1.tar", max compression
+gzip compressed data, was "jptranstokenizer-0.3.2.tar", max compression
```

## Comparing `jptranstokenizer-0.3.1.tar` & `jptranstokenizer-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-03-04 01:34:48.648441 jptranstokenizer-0.3.1/LICENSE
--rw-r--r--   0        0        0     3115 2023-03-04 01:34:48.648441 jptranstokenizer-0.3.1/README.md
--rw-r--r--   0        0        0      911 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      114 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/__init__.py
--rw-r--r--   0        0        0      142 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/__init__.py
--rw-r--r--   0        0        0     1958 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/base.py
--rw-r--r--   0        0        0     3672 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/juman.py
--rw-r--r--   0        0        0     2726 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/spacy_luw.py
--rw-r--r--   0        0        0     4531 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/sudachi.py
--rw-r--r--   0        0        0       50 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/subword/__init__.py
--rw-r--r--   0        0        0     2989 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/subword/sentencepiece.py
--rw-r--r--   0        0        0    28940 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/tokenization_utils.py
--rw-r--r--   0        0        0       22 2023-03-04 01:34:48.652441 jptranstokenizer-0.3.1/src/jptranstokenizer/version.py
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 jptranstokenizer-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-09 08:08:09.207268 jptranstokenizer-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3443 2023-05-09 08:08:09.207268 jptranstokenizer-0.3.2/README.md
+-rw-r--r--   0        0        0      911 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/__init__.py
+-rw-r--r--   0        0        0     1805 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/base.py
+-rw-r--r--   0        0        0     3672 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/juman.py
+-rw-r--r--   0        0        0     2726 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/spacy_luw.py
+-rw-r--r--   0        0        0     4531 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/sudachi.py
+-rw-r--r--   0        0        0       50 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/subword/__init__.py
+-rw-r--r--   0        0        0     2989 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/subword/sentencepiece.py
+-rw-r--r--   0        0        0    28867 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/tokenization_utils.py
+-rw-r--r--   0        0        0       22 2023-05-09 08:08:09.211268 jptranstokenizer-0.3.2/src/jptranstokenizer/version.py
+-rw-r--r--   0        0        0     4262 1970-01-01 00:00:00.000000 jptranstokenizer-0.3.2/PKG-INFO
```

### Comparing `jptranstokenizer-0.3.1/LICENSE` & `jptranstokenizer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jptranstokenizer-0.3.1/README.md` & `jptranstokenizer-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,21 +54,23 @@
 
 **There will be another paper.
 Be sure to check here again when you cite.**
 
 ### This Implementation
 
 ```
-@misc{suzuki-2022-github,
-  author = {Masahiro Suzuki},
-  title = {jptranstokenizer: Japanese Tokenzier for transformers},
-  year = {2022},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/retarfi/jptranstokenizer}}
+@inproceedings{Suzuki-2023-nlp,
+  jtitle = {{異なる単語分割システムによる日本語事前学習言語モデルの性能評価}},
+  title = {{Performance Evaluation of Japanese Pre-trained Language Models with Different Word Segmentation Systems}},
+  jauthor = {鈴木, 雅弘 and 坂地, 泰紀 and 和泉, 潔},
+  author = {Suzuki, Masahiro and Sakaji, Hiroki and Izumi, Kiyoshi},
+  jbooktitle = {言語処理学会 第29回年次大会 (NLP2023)},
+  booktitle = {29th Annual Meeting of the Association for Natural Language Processing (NLP)},
+  year = {2023},
+  pages = {894-898}
 }
 ```
 
 
 ## Related Work
 - Pretrained Japanese BERT models (containing Japanese tokenizer)
   - Autor NLP Lab. in Tohoku University
@@ -76,9 +78,9 @@
 - SudachiTra
   - Author Works Applications
   - https://github.com/WorksApplications/SudachiTra
 - UD_Japanese-GSD
   - Author megagonlabs
   - https://github.com/megagonlabs/UD_Japanese-GSD
 - Juman++
-  - Author Kurohashi Lab. in Universyti of Kyoto
+  - Author Kurohashi Lab. in University of Kyoto
   - https://github.com/ku-nlp/jumanpp
```

#### html2text {}

```diff
@@ -13,17 +13,22 @@
 JapaneseTransformerTokenizer >>> tokenizer =
 JapaneseTransformerTokenizer.from_pretrained("nlp-waseda/roberta-base-
 japanese") >>> tokens = tokenizer.tokenize("å¤å½äººåæ¿æ¨©") # tokens:
 ['âå¤å½', 'âäºº', 'âåæ¿', 'âæ¨©'] ``` Note that different
 dependencies are required depending on the type of tokenizer you use. See also
 [Quickstart on Read the Docs](https://jptranstokenizer.readthedocs.io/en/
 latest/quickstart.html) ## Citation **There will be another paper. Be sure to
-check here again when you cite.** ### This Implementation ``` @misc{suzuki-
-2022-github, author = {Masahiro Suzuki}, title = {jptranstokenizer: Japanese
-Tokenzier for transformers}, year = {2022}, publisher = {GitHub}, journal =
-{GitHub repository}, howpublished = {\url{https://github.com/retarfi/
-jptranstokenizer}} } ``` ## Related Work - Pretrained Japanese BERT models
-(containing Japanese tokenizer) - Autor NLP Lab. in Tohoku University - https:/
-/github.com/cl-tohoku/bert-japanese - SudachiTra - Author Works Applications -
-https://github.com/WorksApplications/SudachiTra - UD_Japanese-GSD - Author
-megagonlabs - https://github.com/megagonlabs/UD_Japanese-GSD - Juman++ - Author
-Kurohashi Lab. in Universyti of Kyoto - https://github.com/ku-nlp/jumanpp
+check here again when you cite.** ### This Implementation ``` @inproceedings
+{Suzuki-2023-nlp, jtitle = {
+{ç°ãªãåèªåå²ã·ã¹ãã ã«ããæ¥æ¬èªäºåå­¦ç¿è¨èªã¢ãã«ã®æ§è½è©ä¾¡}},
+title = {{Performance Evaluation of Japanese Pre-trained Language Models with
+Different Word Segmentation Systems}}, jauthor = {é´æ¨, éå¼ and åå°,
+æ³°ç´ and åæ³, æ½}, author = {Suzuki, Masahiro and Sakaji, Hiroki and
+Izumi, Kiyoshi}, jbooktitle = {è¨èªå¦çå­¦ä¼ ç¬¬29åå¹´æ¬¡å¤§ä¼
+(NLP2023)}, booktitle = {29th Annual Meeting of the Association for Natural
+Language Processing (NLP)}, year = {2023}, pages = {894-898} } ``` ## Related
+Work - Pretrained Japanese BERT models (containing Japanese tokenizer) - Autor
+NLP Lab. in Tohoku University - https://github.com/cl-tohoku/bert-japanese -
+SudachiTra - Author Works Applications - https://github.com/WorksApplications/
+SudachiTra - UD_Japanese-GSD - Author megagonlabs - https://github.com/
+megagonlabs/UD_Japanese-GSD - Juman++ - Author Kurohashi Lab. in University of
+Kyoto - https://github.com/ku-nlp/jumanpp
```

### Comparing `jptranstokenizer-0.3.1/pyproject.toml` & `jptranstokenizer-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jptranstokenizer"
-version = "0.3.1"
+version = "0.3.2"
 description = "Japanese tokenizer with transformers library"
 authors = ["Masahiro Suzuki <msuzuki9609@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jptranstokenizer", from = "src"}]
```

### Comparing `jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/base.py` & `jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,15 @@
         self, do_lower_case: bool = False, normalize_text: bool = True
     ) -> None:
         self.do_lower_case = do_lower_case
         self.normalize_text = normalize_text
 
     @abstractmethod
     def tokenize(self, text: str, **kwargs: Dict[str, Any]) -> List[str]:
-        """Devide the sequence into words.
-
-        Args:
-            text (``str``): A sequence to be encoded.
-
-        Returns:
-            ``List[str]``: A list of words.
-        """
-        pass
+        """Devide the sequence into words."""
 
 
 class Normalizer(MainTokenizerABC):
     """A main word tokenizer, which only normalize and make lower case.
 
     Args:
         do_lower_case (``bool``, *optional*, defaults to ``False``):
```

### Comparing `jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/juman.py` & `jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/juman.py`

 * *Files identical despite different names*

### Comparing `jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/spacy_luw.py` & `jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/spacy_luw.py`

 * *Files identical despite different names*

### Comparing `jptranstokenizer-0.3.1/src/jptranstokenizer/mainword/sudachi.py` & `jptranstokenizer-0.3.2/src/jptranstokenizer/mainword/sudachi.py`

 * *Files identical despite different names*

### Comparing `jptranstokenizer-0.3.1/src/jptranstokenizer/subword/sentencepiece.py` & `jptranstokenizer-0.3.2/src/jptranstokenizer/subword/sentencepiece.py`

 * *Files identical despite different names*

### Comparing `jptranstokenizer-0.3.1/src/jptranstokenizer/tokenization_utils.py` & `jptranstokenizer-0.3.2/src/jptranstokenizer/tokenization_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
 import os
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
 import transformers
 from transformers import (
+    AddedToken,
     AlbertTokenizer,
     BertJapaneseTokenizer,
     PreTrainedTokenizer,
     logging,
 )
 from transformers.models.bert.tokenization_bert import (
     BasicTokenizer,
@@ -17,35 +18,14 @@
 )
 from transformers.models.bert_japanese.tokenization_bert_japanese import (
     CharacterTokenizer,
     MecabTokenizer,
 )
 
 
-if transformers.is_tokenizers_available():
-    from tokenizers import AddedToken
-else:
-
-    @dataclass(frozen=True, eq=True)
-    class AddedToken:
-        """
-        AddedToken represents a token to be added to a Tokenizer An AddedToken can have special options defining the
-        way it should behave.
-        """
-
-        content: str = field(default_factory=str)
-        single_word: bool = False
-        lstrip: bool = False
-        rstrip: bool = False
-        normalized: bool = True
-
-        def __getstate__(self):
-            return self.__dict__
-
-
 logging.set_verbosity_info()
 logging.enable_explicit_format()
 logger = logging.get_logger()
 
 PUBLIC_AVAILABLE_SETTING_MAP: Dict[str, Dict[str, Union[str, bool]]] = {
     "cl-tohoku/bert-base-japanese": {
         "word_tokenizer_type": "mecab",
@@ -58,14 +38,26 @@
         "mecab_dic": "unidic_lite",
     },
     "cl-tohoku/bert-base-japanese-whole-word-masking": {
         "word_tokenizer_type": "mecab",
         "tokenizer_class": "BertJapaneseTokenizer",
         "mecab_dic": "ipadic",
     },
+    "cl-tohoku/bert-base-japanese-char": {
+        "do_lower_case": False,
+        "word_tokenizer_type": "mecab",
+        "tokenizer_class": "BertJapaneseTokenizer",
+        "subword_tokenizer_type": "character",
+    },
+    "cl-tohoku/bert-base-japanese-char-whole-word-masking": {
+        "do_lower_case": False,
+        "word_tokenizer_type": "mecab",
+        "tokenizer_class": "BertJapaneseTokenizer",
+        "subword_tokenizer_type": "character",
+    },
     "cl-tohoku/bert-large-japanese": {
         "word_tokenizer_type": "mecab",
         "tokenizer_class": "BertJapaneseTokenizer",
         "mecab_dic": "unidic_lite",
     },
     "ken11/albert-base-japanese-v1-with-japanese-tokenizer": {
         "word_tokenizer_type": "mecab",
@@ -516,15 +508,15 @@
                 # WordPiece or character
                 subword_tokenizer = tentative_tokenizer.subword_tokenizer
                 if isinstance(subword_tokenizer, WordpieceTokenizer):
                     subword_tokenizer_type = "wordpiece"
                 elif isinstance(subword_tokenizer, CharacterTokenizer):
                     subword_tokenizer_type = "character"
                 else:
-                    raise ValueError()
+                    raise NotImplementedError()
                 vocab = tentative_tokenizer.vocab
                 ids_to_tokens = tentative_tokenizer.ids_to_tokens
             else:
                 raise NotImplementedError()
             tokenizer = cls(
                 word_tokenizer_type=word_tokenizer_type,
                 subword_tokenizer_type=subword_tokenizer_type,
@@ -578,17 +570,17 @@
         if tokenizer_name_or_path in PUBLIC_AVAILABLE_SETTING_MAP.keys():
             dct_setting: Dict[str, str] = PUBLIC_AVAILABLE_SETTING_MAP[
                 tokenizer_name_or_path
             ]
             for k, v in dct_setting.items():
                 kwargs[k] = v
         else:
-            if kwargs["word_tokenizer_type"] is None:
+            if kwargs.get("word_tokenizer_type") is None:
                 raise ValueError("word_tokenizer must be specified")
-            if kwargs["tokenizer_class"] is None:
+            if kwargs.get("tokenizer_class") is None:
                 raise ValueError("tokenizer_class must be specified")
         return _from_pretrained(**kwargs)
 
     def _tokenize(self, text):
         if self.do_word_tokenize:
             tokens = self.word_tokenizer.tokenize(
                 text, never_split=self.all_special_tokens
@@ -608,14 +600,14 @@
         else:
             split_tokens = tokens
 
         return split_tokens
 
     def convert_tokens_to_string(self, tokens: List[str]):
         if self.subword_tokenizer_type in ["character", "wordpiece"]:
-            return super().convert_tokens_to_string(self, tokens)
+            return super().convert_tokens_to_string(tokens)
         elif self.subword_tokenizer_type == "sentencepiece":
             return self.subword_tokenizer.sp_model.decode(tokens)
         else:
             raise NotImplementedError(
                 f"{self.subword_tokenizer} is not allowed for convert_tokens_to_string"
             )
```

### Comparing `jptranstokenizer-0.3.1/PKG-INFO` & `jptranstokenizer-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jptranstokenizer
-Version: 0.3.1
+Version: 0.3.2
 Summary: Japanese tokenizer with transformers library
 License: MIT
 Author: Masahiro Suzuki
 Author-email: msuzuki9609@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -76,21 +76,23 @@
 
 **There will be another paper.
 Be sure to check here again when you cite.**
 
 ### This Implementation
 
 ```
-@misc{suzuki-2022-github,
-  author = {Masahiro Suzuki},
-  title = {jptranstokenizer: Japanese Tokenzier for transformers},
-  year = {2022},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/retarfi/jptranstokenizer}}
+@inproceedings{Suzuki-2023-nlp,
+  jtitle = {{異なる単語分割システムによる日本語事前学習言語モデルの性能評価}},
+  title = {{Performance Evaluation of Japanese Pre-trained Language Models with Different Word Segmentation Systems}},
+  jauthor = {鈴木, 雅弘 and 坂地, 泰紀 and 和泉, 潔},
+  author = {Suzuki, Masahiro and Sakaji, Hiroki and Izumi, Kiyoshi},
+  jbooktitle = {言語処理学会 第29回年次大会 (NLP2023)},
+  booktitle = {29th Annual Meeting of the Association for Natural Language Processing (NLP)},
+  year = {2023},
+  pages = {894-898}
 }
 ```
 
 
 ## Related Work
 - Pretrained Japanese BERT models (containing Japanese tokenizer)
   - Autor NLP Lab. in Tohoku University
@@ -98,10 +100,10 @@
 - SudachiTra
   - Author Works Applications
   - https://github.com/WorksApplications/SudachiTra
 - UD_Japanese-GSD
   - Author megagonlabs
   - https://github.com/megagonlabs/UD_Japanese-GSD
 - Juman++
-  - Author Kurohashi Lab. in Universyti of Kyoto
+  - Author Kurohashi Lab. in University of Kyoto
   - https://github.com/ku-nlp/jumanpp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jptranstokenizer Version: 0.3.1 Summary: Japanese
+Metadata-Version: 2.1 Name: jptranstokenizer Version: 0.3.2 Summary: Japanese
 tokenizer with transformers library License: MIT Author: Masahiro Suzuki
 Author-email: msuzuki9609@gmail.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: SudachiTra
@@ -24,17 +24,22 @@
 JapaneseTransformerTokenizer >>> tokenizer =
 JapaneseTransformerTokenizer.from_pretrained("nlp-waseda/roberta-base-
 japanese") >>> tokens = tokenizer.tokenize("å¤å½äººåæ¿æ¨©") # tokens:
 ['âå¤å½', 'âäºº', 'âåæ¿', 'âæ¨©'] ``` Note that different
 dependencies are required depending on the type of tokenizer you use. See also
 [Quickstart on Read the Docs](https://jptranstokenizer.readthedocs.io/en/
 latest/quickstart.html) ## Citation **There will be another paper. Be sure to
-check here again when you cite.** ### This Implementation ``` @misc{suzuki-
-2022-github, author = {Masahiro Suzuki}, title = {jptranstokenizer: Japanese
-Tokenzier for transformers}, year = {2022}, publisher = {GitHub}, journal =
-{GitHub repository}, howpublished = {\url{https://github.com/retarfi/
-jptranstokenizer}} } ``` ## Related Work - Pretrained Japanese BERT models
-(containing Japanese tokenizer) - Autor NLP Lab. in Tohoku University - https:/
-/github.com/cl-tohoku/bert-japanese - SudachiTra - Author Works Applications -
-https://github.com/WorksApplications/SudachiTra - UD_Japanese-GSD - Author
-megagonlabs - https://github.com/megagonlabs/UD_Japanese-GSD - Juman++ - Author
-Kurohashi Lab. in Universyti of Kyoto - https://github.com/ku-nlp/jumanpp
+check here again when you cite.** ### This Implementation ``` @inproceedings
+{Suzuki-2023-nlp, jtitle = {
+{ç°ãªãåèªåå²ã·ã¹ãã ã«ããæ¥æ¬èªäºåå­¦ç¿è¨èªã¢ãã«ã®æ§è½è©ä¾¡}},
+title = {{Performance Evaluation of Japanese Pre-trained Language Models with
+Different Word Segmentation Systems}}, jauthor = {é´æ¨, éå¼ and åå°,
+æ³°ç´ and åæ³, æ½}, author = {Suzuki, Masahiro and Sakaji, Hiroki and
+Izumi, Kiyoshi}, jbooktitle = {è¨èªå¦çå­¦ä¼ ç¬¬29åå¹´æ¬¡å¤§ä¼
+(NLP2023)}, booktitle = {29th Annual Meeting of the Association for Natural
+Language Processing (NLP)}, year = {2023}, pages = {894-898} } ``` ## Related
+Work - Pretrained Japanese BERT models (containing Japanese tokenizer) - Autor
+NLP Lab. in Tohoku University - https://github.com/cl-tohoku/bert-japanese -
+SudachiTra - Author Works Applications - https://github.com/WorksApplications/
+SudachiTra - UD_Japanese-GSD - Author megagonlabs - https://github.com/
+megagonlabs/UD_Japanese-GSD - Juman++ - Author Kurohashi Lab. in University of
+Kyoto - https://github.com/ku-nlp/jumanpp
```

