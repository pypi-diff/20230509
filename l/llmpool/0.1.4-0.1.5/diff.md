# Comparing `tmp/llmpool-0.1.4-py3-none-any.whl.zip` & `tmp/llmpool-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 9616 bytes, number of entries: 11
--rw-rw-rw-  2.0 unx      194 b- defN 23-May-09 03:01 llmpool/__init__.py
+Zip file size: 9478 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx      157 b- defN 23-May-09 04:30 llmpool/__init__.py
 -rw-rw-rw-  2.0 unx     3897 b- defN 23-May-09 02:55 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 07:36 llmpool/model.py
--rw-rw-rw-  2.0 unx      919 b- defN 23-May-08 09:30 llmpool/model_pool.py
--rw-rw-rw-  2.0 unx     1883 b- defN 23-May-09 02:54 llmpool/remote_model.py
--rw-rw-rw-  2.0 unx     1422 b- defN 23-May-08 14:49 llmpool/utils.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     2398 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      842 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/RECORD
-11 files, 23603 bytes uncompressed, 8206 bytes compressed:  65.2%
+-rw-rw-rw-  2.0 unx     2496 b- defN 23-May-09 04:30 llmpool/model_pool.py
+-rw-rw-rw-  2.0 unx     2112 b- defN 23-May-09 04:29 llmpool/remote_model.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-09 04:31 llmpool-0.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     2409 b- defN 23-May-09 04:31 llmpool-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-09 04:31 llmpool-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-09 04:31 llmpool-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      770 b- defN 23-May-09 04:31 llmpool-0.1.5.dist-info/RECORD
+10 files, 23889 bytes uncompressed, 8176 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,26 +9,23 @@
 
 Filename: llmpool/model_pool.py
 Comment: 
 
 Filename: llmpool/remote_model.py
 Comment: 
 
-Filename: llmpool/utils.py
+Filename: llmpool-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.1.4.dist-info/LICENSE
+Filename: llmpool-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.1.4.dist-info/METADATA
+Filename: llmpool-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.1.4.dist-info/WHEEL
+Filename: llmpool-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.1.4.dist-info/top_level.txt
-Comment: 
-
-Filename: llmpool-0.1.4.dist-info/RECORD
+Filename: llmpool-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,6 +1,5 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 from .local_model import LocalLLModel, LocalLoRALLModel
 from .model_pool import LLModelPool
 from .remote_model import TxtGenIfLLModel
-from .utils import instantiate_models
```

## llmpool/model_pool.py

```diff
@@ -1,9 +1,12 @@
+import yaml
 from typing import List
 from llmpool.model import LLModel
+from llmpool.local_model import LocalLLModel, LocalLoRALLModel
+from llmpool.remote_model import TxtGenIfLLModel
 
 class LLModelIter:
     def __init__(self, model_pool):
         self._models = model_pool.models
         self._pool_size = len(self._models)
         self._current_index = 0
 
@@ -28,9 +31,62 @@
     def add_models(self, models: List[LLModel]):
         for model in models:
             self.models[model.name] = model
 
     def get_model(self, name) -> LLModel:
         return self.models[name]
 
+
+    @classmethod
+    def instantiate_model(cls, name, model_spec):
+        model_type = model_spec['type']
+        load_config = model_spec['load']
+        metadata = model_spec['metadata']
+        gen_config = model_spec['generation_config']
+
+        model_ckpt = {}
+        load_config = {}
+
+        model_type = eval(model_type)
+        if isinstance(model_type, LocalLLModel) \
+            or isinstance(model_type, LocalLoRALLModel):
+            assert "model" in model_spec, "model ckpt config should be provided"
+            model_ckpt = model_spec['model']
+
+        if "model_cls" in load_config:
+            load_config['model_cls'] = eval(load_config['model_cls'])
+
+        if "tokenizer_cls" in load_config:
+            load_config['tokenizer_cls'] = eval(load_config['tokenizer_cls'])
+
+        model = model_type(
+            name=name,
+            **model_ckpt,
+            **load_config
+        )
+
+        return model
+
+    @classmethod
+    def from_yaml(cls, filepath):
+        model_pool = cls()
+
+        model_specs = cls.load_yaml(filepath)
+
+        for name, model_spec in model_specs:
+            model_pool.add_model(
+                cls.instantiate_model(name, model_spec)
+            )
+
+        return model_pool
+    
+    @classmethod
+    def load_yaml(cls, filepath):
+        yaml_dict = None
+
+        with open(filepath, 'r') as file:
+            yaml_dict = yaml.load(file, Loader=yaml.FullLoader)
+
+        return yaml_dict
+
     def __iter__(self):
-        return LLModelIter(self)
+        return LLModelIter(self)
```

## llmpool/remote_model.py

```diff
@@ -1,20 +1,27 @@
 from text_generation import Client
 from transformers import GenerationConfig
 
 from llmpool.model import LLModel
 
 class TxtGenIfLLModel(LLModel):
-    def __init__(self, name, url, headers=None, cookies=None, timeout=10):
+    def __init__(self, name, url, port, headers=None, cookies=None, timeout=10):
         super().__init__(name)
 
+        if port is not None:
+            port = f":{port}"
+
         self.client = Client(
-            base_url=url, headers=headers, cookies=cookies, timeout=timeout
+            base_url=f"{url}{port}", headers=headers, cookies=cookies, timeout=timeout
         )
 
+    def _stream_text(self, stream_results):
+        for stream_result in stream_results:
+            yield stream_result.token.text
+
     def stream_gen(self, prompt, gen_config: GenerationConfig, stopping_criteria=None):
         super().stream_gen(prompt, gen_config, stopping_criteria)
 
         stream = self.client.generate_stream(
             prompt,
             do_sample=gen_config.do_sample,
             max_new_tokens=gen_config.max_new_tokens,
@@ -26,15 +33,15 @@
             top_k=gen_config.top_k,
             top_p=gen_config.top_p,
             truncate=None,
             typical_p=gen_config.typical_p,
             watermark=False,
         )
 
-        return None, stream
+        return None, self._stream_text(stream)
 
     def batch_gen(self, prompts, gen_config: GenerationConfig, stopping_criteria=None, best_of=None):
         super().batch_gen(prompts, gen_config, stopping_criteria)
 
         batch = self.client.generate(
             prompts,
             do_sample=gen_config.do_sample,
```

## Comparing `llmpool-0.1.4.dist-info/LICENSE` & `llmpool-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.1.4.dist-info/METADATA` & `llmpool-0.1.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmpool
-Version: 0.1.4
+Version: 0.1.5
 Summary: Large Language Models' pool management library
 Home-page: https://github.com/deep-diver/LLM-Pool
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,instance pool,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 # LLM-Pool
 
 This simple project is to manage multiple LLM(Large Language Model)s in one place. Because there are too many fine-tuned LLMs, and it is hard to evaluate which one is bettern than others, it might be useful to test as many models as possible. Below is the two useful usecases that I had in mind when kicking off this project.
 
 - compare generated text from different models side by side
 - complete conversation in collaboration of different models
 
-![](https://i.ibb.co/my2tf27/overview.png)
+![](https://i.ibb.co/GH55nWs/2023-05-09-12-09-58.png)
 
 ## Usecase
 
 ```python
 
 from llmpool import LLModelPool
 from llmpool import LocalLoRAModel
```

