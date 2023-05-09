# Comparing `tmp/madai-0.1.5.tar.gz` & `tmp/madai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madai-0.1.5.tar", max compression
+gzip compressed data, was "madai-0.2.0.tar", max compression
```

## Comparing `madai-0.1.5.tar` & `madai-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      553 2023-05-04 14:53:17.872677 madai-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.1.5/madai/__init__.py
--rw-r--r--   0        0        0     5269 2023-05-08 07:13:13.567814 madai-0.1.5/madai/main.py
--rw-r--r--   0        0        0     1357 2023-05-08 06:34:11.409000 madai-0.1.5/madai/utils.py
--rw-r--r--   0        0        0      576 2023-05-08 07:13:20.995709 madai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 madai-0.1.5/setup.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 madai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      758 2023-05-09 10:01:02.650782 madai-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:10:33.818620 madai-0.2.0/madai/__init__.py
+-rw-r--r--   0        0        0     4803 2023-05-09 11:56:53.481861 madai-0.2.0/madai/chi2.py
+-rw-r--r--   0        0        0      143 2023-05-09 09:53:01.108847 madai-0.2.0/madai/cli.py
+-rw-r--r--   0        0        0     2754 2023-05-09 11:56:48.724540 madai-0.2.0/madai/spearman.py
+-rw-r--r--   0        0        0     1492 2023-05-09 09:18:16.958076 madai-0.2.0/madai/utils.py
+-rw-r--r--   0        0        0      574 2023-05-09 11:57:25.796079 madai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 madai-0.2.0/setup.py
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 madai-0.2.0/PKG-INFO
```

### Comparing `madai-0.1.5/madai/main.py` & `madai-0.2.0/madai/chi2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from argparse import ArgumentParser
 from collections import Counter
 from dataclasses import dataclass, field
 from functools import partial
 from random import sample
 from typing import Union
 
-import click
 import numpy as np
 import scipy.stats as stats
 import sienna
+import typer
 from spacy.tokenizer import Tokenizer
 from tqdm import tqdm
 
 from madai.utils import get_tokenizer, tokenize
 
 
 @dataclass
@@ -72,14 +71,15 @@
     a = a[:doc_n]
     b = b[:doc_n]
 
     print(f"Use {doc_n} documents for each corpus.")
 
     # Number of sample for each slice
     slice_size = slice_size if isinstance(slice_size, int) else int(doc_n * slice_size)
+    slice_size = max(1, slice_size)
 
     print(f"Slice size: {slice_size}")
 
     # Tokenization for freq word counting
     tokenizer = partial(tokenize, tok, remove_stopwords)
     a_words = [word for doc in a for word in tokenizer(doc)]
     b_words = [word for doc in b for word in tokenizer(doc)]
@@ -128,57 +128,39 @@
 
         score = sim(a_fc, b_fc)
         scores.append(score)
 
     return np.array(scores)
 
 
-@click.command()
-@click.argument("a", type=str)
-@click.argument("b", type=str)
-@click.option("--lang", type=str, default="en")
-@click.option("--slice-size", type=float, default=0.25)
-@click.option("--n-iter", type=int, default=50)
-@click.option("--top-n", type=int, default=1000)
-@click.option("--remove-stopwords", is_flag=True, show_default=True, default=False)
-def run(
-    a: str,
-    b: str,
-    lang: str,
-    slice_size: float,
-    n_iter: int,
-    top_n: int,
-    remove_stopwords: bool,
+app = typer.Typer()
+
+
+@app.command()
+def chi2(
+    a: str = typer.Argument(..., help="Path to a corpus"),
+    b: str = typer.Argument(..., help="Path to another corpus"),
+    lang: str = typer.Option("en", help="Language code for both corpus."),
+    slice_size: float = typer.Option(0.25, help="Size of each slice."),
+    iter_n: int = typer.Option(50, help="Number of iteration to take avg from."),
+    top_n_words: int = typer.Option(
+        500, help="Number of most frequent words to consider."
+    ),
+    remove_stopwords: bool = False,
 ):
     if remove_stopwords:
         assert lang == "en", "Stopword remove is only supported for English (en)"
 
     a_texts = sienna.load(a)
     b_texts = sienna.load(b)
 
     assert isinstance(a_texts, list)
     assert isinstance(b_texts, list)
 
     tok = get_tokenizer(lang)
 
-    scores = _run(a_texts, b_texts, tok, slice_size, top_n, n_iter, remove_stopwords)
+    scores = _run(
+        a_texts, b_texts, tok, slice_size, top_n_words, iter_n, remove_stopwords
+    )
     score_avg = np.average(scores)
     score_std = np.std(scores)
     print(f"Distance between corpus: {score_avg:.2f}±{score_std:.2f}")
-
-
-if __name__ == "__main__":
-    parser = ArgumentParser()
-    parser.add_argument("-a", type=str, required=True)
-    parser.add_argument("-b", type=str, required=True)
-    args = parser.parse_args()
-
-    a_texts = sienna.load(args.a)
-    b_texts = sienna.load(args.b)
-
-    assert isinstance(a_texts, list)
-    assert isinstance(b_texts, list)
-
-    scores = run(a_texts, b_texts, slice_size=0.25, n_iter=50, top_n=1000)
-    score_avg = np.average(scores)
-    score_std = np.std(scores)
-    print(f"{score_avg:.2f}±{score_std:.2f}")
```

### Comparing `madai-0.1.5/madai/utils.py` & `madai-0.2.0/madai/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import List
-
+import numpy as np
 from nltk.corpus import stopwords
 from spacy.lang.ar import Arabic
 from spacy.lang.bg import Bulgarian
 from spacy.lang.de import German
 from spacy.lang.el import Greek
 from spacy.lang.en import English
 from spacy.lang.es import Spanish
@@ -36,16 +35,24 @@
         "ur": Urdu(),
         "vi": Vietnamese(),
         "zh": Chinese(),
     }[lang]
     return nlp.tokenizer
 
 
-def tokenize(tok: Tokenizer, remove_stopwords: bool, text: str) -> List[str]:
+def tokenize(tok: Tokenizer, remove_stopwords: bool, text: str) -> list[str]:
     if remove_stopwords:
         return [
             word.text.lower()
             for word in tok(text)
             if word.text.lower() not in stopwords
         ]
     else:
         return [word.text.lower() for word in tok(text)]
+
+
+def avg(values: list) -> float:
+    return np.mean(np.array(values))
+
+
+def std(values: list) -> float:
+    return np.std(np.array(values))
```

### Comparing `madai-0.1.5/pyproject.toml` & `madai-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "madai"
-version = "0.1.5"
+version = "0.2.0"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.10.1"
-spacy = "^3.5.2"
-click = "^8.1.3"
 sienna = "^0.2.2"
 nltk = "^3.8.1"
 pyvi = "^0.1.1"
+spacy = "^3.5.2"
+typer = "0.7.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 isort = "^5.12.0"
 neovim = "^0.3.1"
 pytest = "^7.3.1"
@@ -24,8 +24,8 @@
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-madai = "madai.main:run"
+madai = "madai.cli:app"
```

### Comparing `madai-0.1.5/setup.py` & `madai-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 packages = \
 ['madai']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.1.3,<9.0.0',
- 'nltk>=3.8.1,<4.0.0',
+['nltk>=3.8.1,<4.0.0',
  'pyvi>=0.1.1,<0.2.0',
  'scipy>=1.10.1,<2.0.0',
  'sienna>=0.2.2,<0.3.0',
- 'spacy>=3.5.2,<4.0.0']
+ 'spacy>=3.5.2,<4.0.0',
+ 'typer==0.7.0']
 
 entry_points = \
-{'console_scripts': ['madai = madai.main:run']}
+{'console_scripts': ['madai = madai.cli:app']}
 
 setup_kwargs = {
     'name': 'madai',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': '',
-    'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
+    'long_description': '# madai\n\nCompute difference between two corpus by using chi2.\nImplementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).\n\nI am not fully sure if this implementation is perfectly follow this paper.\nFeel free to make issues to point out some problems if you find.\n\n## Installation\n\n```\npip install madai\n```\n\n## Usage\n\nmadai implements two ways of computing similarity between two corpus, chi2 and spearman.\nUse spearman when two corpus are different in size.\n\nTwo target corpus need to be text files, each line containing one document/sentence.\n\n```\nmadai chi2 /path/to/corpus/a /path/to/corpus/b\n\n# or\n\nmadai spearman /path/to/corpus/a /path/to/corpus/b\n```\n\nTo view parameters, run,\n```\nmadai --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `madai-0.1.5/PKG-INFO` & `madai-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: madai
-Version: 0.1.5
+Version: 0.2.0
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pyvi (>=0.1.1,<0.2.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sienna (>=0.2.2,<0.3.0)
 Requires-Dist: spacy (>=3.5.2,<4.0.0)
+Requires-Dist: typer (==0.7.0)
 Description-Content-Type: text/markdown
 
 # madai
 
 Compute difference between two corpus by using chi2.
 Implementation is based on [Measures for Corpus Similarity and Homogeneity](https://aclanthology.org/W98-1506).
 
@@ -29,18 +29,25 @@
 
 ```
 pip install madai
 ```
 
 ## Usage
 
+madai implements two ways of computing similarity between two corpus, chi2 and spearman.
+Use spearman when two corpus are different in size.
+
 Two target corpus need to be text files, each line containing one document/sentence.
 
 ```
-madai /path/to/corpus/a /path/to/corpus/b
+madai chi2 /path/to/corpus/a /path/to/corpus/b
+
+# or
+
+madai spearman /path/to/corpus/a /path/to/corpus/b
 ```
 
 To view parameters, run,
 ```
 madai --help
 ```
```

