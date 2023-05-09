# Comparing `tmp/fastcoref-2.1.4.tar.gz` & `tmp/fastcoref-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcoref-2.1.4.tar", last modified: Tue Apr 18 15:57:58 2023, max compression
+gzip compressed data, was "fastcoref-2.1.5.tar", last modified: Tue May  9 16:58:08 2023, max compression
```

## Comparing `fastcoref-2.1.4.tar` & `fastcoref-2.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-18 15:57:58.884337 fastcoref-2.1.4/
--rw-r--r--   0 shono    (847860209) 305066103     1070 2023-04-16 21:51:10.000000 fastcoref-2.1.4/LICENSE
--rw-r--r--   0 shono    (847860209) 305066103     6754 2023-04-18 15:57:58.884189 fastcoref-2.1.4/PKG-INFO
--rw-r--r--   0 shono    (847860209) 305066103     6467 2023-04-16 21:51:10.000000 fastcoref-2.1.4/README.md
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-18 15:57:58.880865 fastcoref-2.1.4/fastcoref/
--rw-r--r--   0 shono    (847860209) 305066103      104 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/__init__.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-18 15:57:58.882518 fastcoref-2.1.4/fastcoref/coref_models/
--rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/coref_models/__init__.py
--rwxr-xr-x   0 shono    (847860209) 305066103    14767 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/coref_models/modeling_fcoref.py
--rwxr-xr-x   0 shono    (847860209) 305066103    19662 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/coref_models/modeling_lingmess.py
--rw-r--r--   0 shono    (847860209) 305066103    11773 2023-04-18 15:51:54.000000 fastcoref-2.1.4/fastcoref/modeling.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-18 15:57:58.882948 fastcoref-2.1.4/fastcoref/spacy_component/
--rw-r--r--   0 shono    (847860209) 305066103       46 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/spacy_component/__init__.py
--rw-r--r--   0 shono    (847860209) 305066103     7554 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/spacy_component/spacy_component.py
--rw-r--r--   0 shono    (847860209) 305066103    12762 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/trainer.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-18 15:57:58.883938 fastcoref-2.1.4/fastcoref/utilities/
--rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/utilities/__init__.py
--rwxr-xr-x   0 shono    (847860209) 305066103     4548 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/utilities/collate.py
--rw-r--r--   0 shono    (847860209) 305066103      984 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/utilities/consts.py
--rw-r--r--   0 shono    (847860209) 305066103     6185 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/utilities/coref_dataset.py
--rwxr-xr-x   0 shono    (847860209) 305066103     5003 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/utilities/metrics.py
--rw-r--r--   0 shono    (847860209) 305066103     9393 2023-04-16 21:51:10.000000 fastcoref-2.1.4/fastcoref/utilities/util.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-18 15:57:58.881940 fastcoref-2.1.4/fastcoref.egg-info/
--rw-r--r--   0 shono    (847860209) 305066103     6754 2023-04-18 15:57:58.000000 fastcoref-2.1.4/fastcoref.egg-info/PKG-INFO
--rw-r--r--   0 shono    (847860209) 305066103      648 2023-04-18 15:57:58.000000 fastcoref-2.1.4/fastcoref.egg-info/SOURCES.txt
--rw-r--r--   0 shono    (847860209) 305066103        1 2023-04-18 15:57:58.000000 fastcoref-2.1.4/fastcoref.egg-info/dependency_links.txt
--rw-r--r--   0 shono    (847860209) 305066103      127 2023-04-18 15:57:58.000000 fastcoref-2.1.4/fastcoref.egg-info/requires.txt
--rw-r--r--   0 shono    (847860209) 305066103       10 2023-04-18 15:57:58.000000 fastcoref-2.1.4/fastcoref.egg-info/top_level.txt
--rw-r--r--   0 shono    (847860209) 305066103       38 2023-04-18 15:57:58.884381 fastcoref-2.1.4/setup.cfg
--rw-r--r--   0 shono    (847860209) 305066103      991 2023-04-18 15:52:29.000000 fastcoref-2.1.4/setup.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.441208 fastcoref-2.1.5/
+-rw-r--r--   0 shono    (847860209) 305066103     1070 2023-04-16 21:51:10.000000 fastcoref-2.1.5/LICENSE
+-rw-r--r--   0 shono    (847860209) 305066103     6754 2023-05-09 16:58:08.441059 fastcoref-2.1.5/PKG-INFO
+-rw-r--r--   0 shono    (847860209) 305066103     6467 2023-04-16 21:51:10.000000 fastcoref-2.1.5/README.md
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.438076 fastcoref-2.1.5/fastcoref/
+-rw-r--r--   0 shono    (847860209) 305066103      104 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/__init__.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.439500 fastcoref-2.1.5/fastcoref/coref_models/
+-rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/coref_models/__init__.py
+-rwxr-xr-x   0 shono    (847860209) 305066103    14767 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/coref_models/modeling_fcoref.py
+-rwxr-xr-x   0 shono    (847860209) 305066103    19662 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/coref_models/modeling_lingmess.py
+-rw-r--r--   0 shono    (847860209) 305066103    11812 2023-05-09 16:56:18.000000 fastcoref-2.1.5/fastcoref/modeling.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.439866 fastcoref-2.1.5/fastcoref/spacy_component/
+-rw-r--r--   0 shono    (847860209) 305066103       46 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/spacy_component/__init__.py
+-rw-r--r--   0 shono    (847860209) 305066103     7554 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/spacy_component/spacy_component.py
+-rw-r--r--   0 shono    (847860209) 305066103    12762 2023-05-09 11:22:56.000000 fastcoref-2.1.5/fastcoref/trainer.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.440813 fastcoref-2.1.5/fastcoref/utilities/
+-rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/__init__.py
+-rwxr-xr-x   0 shono    (847860209) 305066103     4548 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/collate.py
+-rw-r--r--   0 shono    (847860209) 305066103      984 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/consts.py
+-rw-r--r--   0 shono    (847860209) 305066103     6185 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/coref_dataset.py
+-rwxr-xr-x   0 shono    (847860209) 305066103     5003 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/metrics.py
+-rw-r--r--   0 shono    (847860209) 305066103     9445 2023-05-09 16:56:18.000000 fastcoref-2.1.5/fastcoref/utilities/util.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.438865 fastcoref-2.1.5/fastcoref.egg-info/
+-rw-r--r--   0 shono    (847860209) 305066103     6754 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/PKG-INFO
+-rw-r--r--   0 shono    (847860209) 305066103      648 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/SOURCES.txt
+-rw-r--r--   0 shono    (847860209) 305066103        1 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/dependency_links.txt
+-rw-r--r--   0 shono    (847860209) 305066103      127 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/requires.txt
+-rw-r--r--   0 shono    (847860209) 305066103       10 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/top_level.txt
+-rw-r--r--   0 shono    (847860209) 305066103       38 2023-05-09 16:58:08.441255 fastcoref-2.1.5/setup.cfg
+-rw-r--r--   0 shono    (847860209) 305066103      991 2023-05-09 16:57:35.000000 fastcoref-2.1.5/setup.py
```

### Comparing `fastcoref-2.1.4/LICENSE` & `fastcoref-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/PKG-INFO` & `fastcoref-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcoref
-Version: 2.1.4
+Version: 2.1.5
 Home-page: https://github.com/shon-otmazgin/fastcoref
 Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
 Author-email: shon711@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
```

### Comparing `fastcoref-2.1.4/README.md` & `fastcoref-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/coref_models/modeling_fcoref.py` & `fastcoref-2.1.5/fastcoref/coref_models/modeling_fcoref.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/coref_models/modeling_lingmess.py` & `fastcoref-2.1.5/fastcoref/coref_models/modeling_lingmess.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/modeling.py` & `fastcoref-2.1.5/fastcoref/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         self.coref_logit = coref_logit
         self.text_idx = text_idx
 
     def get_clusters(self, as_strings=True):
         if not as_strings:
             return [[self.char_map[mention][1] for mention in cluster] for cluster in self.clusters]
 
-        return [[self.text[self.char_map[mention][1][0]:self.char_map[mention][1][1]] for mention in cluster]
-                for cluster in self.clusters]
+        return [[self.text[self.char_map[mention][1][0]:self.char_map[mention][1][1]]
+                 for mention in cluster if None not in self.char_map[mention]] for cluster in self.clusters]
 
     def get_logit(self, span_i, span_j):
         if span_i not in self.reverse_char_map:
             raise ValueError(f'span_i="{self.text[span_i[0]:span_i[1]]}" is not an entity in this model!')
         if span_j not in self.reverse_char_map:
             raise ValueError(f'span_i="{self.text[span_j[0]:span_j[1]]}" is not an entity in this model!')
```

### Comparing `fastcoref-2.1.4/fastcoref/spacy_component/spacy_component.py` & `fastcoref-2.1.5/fastcoref/spacy_component/spacy_component.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/trainer.py` & `fastcoref-2.1.5/fastcoref/trainer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,20 +82,20 @@
 
     return model, tokenizer
 
 
 class CorefTrainer:
     def __init__(self, args: TrainingArgs, train_file, dev_file=None, test_file=None):
         import wandb
-        self.wandb_logger = wandb.log
-        self.wandb_runner = wandb.run
 
         transformers.logging.set_verbosity_error()
         self.args = args
         wandb.init(project=self.args.output_dir, config=self.args)
+        self.wandb_logger = wandb.log
+        self.wandb_runner = wandb.run
 
         self._set_device()
 
         self.nlp = spacy.load("en_core_web_sm", exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
         self.model, self.tokenizer = _load_f_coref_model(self.args)
         self.model.to(self.device)
```

### Comparing `fastcoref-2.1.4/fastcoref/utilities/collate.py` & `fastcoref-2.1.5/fastcoref/utilities/collate.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/utilities/consts.py` & `fastcoref-2.1.5/fastcoref/utilities/consts.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/utilities/coref_dataset.py` & `fastcoref-2.1.5/fastcoref/utilities/coref_dataset.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/utilities/metrics.py` & `fastcoref-2.1.5/fastcoref/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/fastcoref/utilities/util.py` & `fastcoref-2.1.5/fastcoref/utilities/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     for idx, (start, end) in enumerate(zip(span_starts, span_ends)):
         new_start, new_end = start.copy(), end.copy()
 
         try:
             if subtoken_map is not None:
                 new_start, new_end = subtoken_map[new_start], subtoken_map[new_end]
                 if new_start is None or new_end is None:
+                    # this is a special token index
                     char_map[(start, end)] = None, None
                     continue
             if new_token_map is not None:
                 new_start, new_end = new_token_map[new_start], new_token_map[new_end]
             new_start, new_end = token_to_char[new_start][0], token_to_char[new_end][1]
             char_map[(start, end)] = idx, (new_start, new_end)
             reverse_char_map[(new_start, new_end)] = idx, (start, end)
```

### Comparing `fastcoref-2.1.4/fastcoref.egg-info/PKG-INFO` & `fastcoref-2.1.5/fastcoref.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcoref
-Version: 2.1.4
+Version: 2.1.5
 Home-page: https://github.com/shon-otmazgin/fastcoref
 Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
 Author-email: shon711@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
```

### Comparing `fastcoref-2.1.4/fastcoref.egg-info/SOURCES.txt` & `fastcoref-2.1.5/fastcoref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.4/setup.py` & `fastcoref-2.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='fastcoref',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.1.4',
+    version='2.1.5',
     license='MIT',
     author="Shon Otmazgin, Arie Cattan, Yoav Goldberg",
     author_email='shon711@gmail.com',
     packages=['fastcoref', 'fastcoref.coref_models', 'fastcoref.utilities', 'fastcoref.spacy_component'],
     url='https://github.com/shon-otmazgin/fastcoref',
     install_requires=[
         'tqdm>=4.64.0',
```

