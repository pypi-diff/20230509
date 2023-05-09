# Comparing `tmp/gpt4all-0.1.7-py3-none-any.whl.zip` & `tmp/gpt4all-0.1.8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,13 @@
-Zip file size: 234269 bytes, number of entries: 24
--rw-r--r--  2.0 unx       65 b- defN 23-May-07 18:56 gpt4all/__init__.py
--rw-r--r--  2.0 unx     2418 b- defN 23-May-07 19:13 gpt4all/gpt4all.py
--rw-r--r--  2.0 unx     7823 b- defN 23-May-07 18:56 gpt4all/pyllmodel.py
--rw-r--r--  2.0 unx     3378 b- defN 23-May-01 04:28 gpt4all/llmodel_DO_NOT_MODIFY/common.h
--rw-r--r--  2.0 unx     2334 b- defN 23-May-01 04:28 gpt4all/llmodel_DO_NOT_MODIFY/ggml-cuda.h
--rw-r--r--  2.0 unx      639 b- defN 23-May-01 04:28 gpt4all/llmodel_DO_NOT_MODIFY/ggml-opencl.h
--rw-r--r--  2.0 unx    29631 b- defN 23-May-01 04:28 gpt4all/llmodel_DO_NOT_MODIFY/ggml.h
--rw-r--r--  2.0 unx      970 b- defN 23-May-07 18:56 gpt4all/llmodel_DO_NOT_MODIFY/gptj.h
--rw-r--r--  2.0 unx     7890 b- defN 23-May-01 04:28 gpt4all/llmodel_DO_NOT_MODIFY/llama.h
--rwxr-xr-x  2.0 unx    11979 b- defN 23-May-01 04:28 gpt4all/llmodel_DO_NOT_MODIFY/llama_util.h
--rw-r--r--  2.0 unx     1007 b- defN 23-May-07 18:56 gpt4all/llmodel_DO_NOT_MODIFY/llamamodel.h
--rw-r--r--  2.0 unx     1753 b- defN 23-May-07 18:56 gpt4all/llmodel_DO_NOT_MODIFY/llmodel.h
--rw-r--r--  2.0 unx     5737 b- defN 23-May-07 18:56 gpt4all/llmodel_DO_NOT_MODIFY/llmodel_c.h
--rw-r--r--  2.0 unx     2325 b- defN 23-Apr-26 16:10 gpt4all/llmodel_DO_NOT_MODIFY/utils.h
--rwxr-xr-x  2.0 unx   319611 b- defN 23-May-07 18:58 gpt4all/llmodel_DO_NOT_MODIFY/build/libllama.dylib
--rwxr-xr-x  2.0 unx   208445 b- defN 23-May-07 18:58 gpt4all/llmodel_DO_NOT_MODIFY/build/libllmodel.dylib
--rw-r--r--  2.0 unx        0 b- defN 23-May-07 18:56 tests/__init__.py
--rw-r--r--  2.0 unx      687 b- defN 23-May-07 18:56 tests/test_gpt4all.py
--rw-r--r--  2.0 unx     1129 b- defN 23-May-07 18:56 tests/test_pyllmodel.py
--rw-r--r--  2.0 unx     1054 b- defN 23-May-07 19:18 gpt4all-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      456 b- defN 23-May-07 19:18 gpt4all-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 19:18 gpt4all-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-07 19:18 gpt4all-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2122 b- defN 23-May-07 19:18 gpt4all-0.1.7.dist-info/RECORD
-24 files, 611559 bytes uncompressed, 230793 bytes compressed:  62.3%
+Zip file size: 9162 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       76 b- defN 23-May-09 16:44 gpt4all/__init__.py
+-rw-rw-rw-  2.0 fat    11187 b- defN 23-May-09 16:44 gpt4all/gpt4all.py
+-rw-rw-rw-  2.0 fat     7513 b- defN 23-May-09 16:44 gpt4all/pyllmodel.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-09 16:44 tests/__init__.py
+-rw-rw-rw-  2.0 fat     1863 b- defN 23-May-09 16:44 tests/test_gpt4all.py
+-rw-rw-rw-  2.0 fat     1172 b- defN 23-May-09 16:44 tests/test_pyllmodel.py
+-rw-rw-rw-  2.0 fat     1072 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      733 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      845 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/RECORD
+11 files, 24573 bytes uncompressed, 7742 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -3,71 +3,32 @@
 
 Filename: gpt4all/gpt4all.py
 Comment: 
 
 Filename: gpt4all/pyllmodel.py
 Comment: 
 
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/common.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/ggml-cuda.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/ggml-opencl.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/ggml.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/gptj.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/llama.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/llama_util.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/llamamodel.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/llmodel.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/llmodel_c.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/utils.h
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libllama.dylib
-Comment: 
-
-Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libllmodel.dylib
-Comment: 
-
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_gpt4all.py
 Comment: 
 
 Filename: tests/test_pyllmodel.py
 Comment: 
 
-Filename: gpt4all-0.1.7.dist-info/LICENSE.txt
+Filename: gpt4all-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: gpt4all-0.1.7.dist-info/METADATA
+Filename: gpt4all-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: gpt4all-0.1.7.dist-info/WHEEL
+Filename: gpt4all-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: gpt4all-0.1.7.dist-info/top_level.txt
+Filename: gpt4all-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: gpt4all-0.1.7.dist-info/RECORD
+Filename: gpt4all-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gpt4all/__init__.py

```diff
@@ -1,2 +1,2 @@
-from . import gpt4all # noqa
-from .gpt4all import GPT4All # noqa
+from .pyllmodel import LLModel # noqa
+from .gpt4all import GPT4All # noqa
```

## gpt4all/gpt4all.py

```diff
@@ -1,70 +1,280 @@
-"""
-Python only API for running all GPT4All models.
-"""
-import os
-
-from . import pyllmodel
-
-
-class GPT4All():
-
-    def __init__(self, model_path: str, model_type: str = None):
-        self.model = None
-
-        # Model type provided for when model is custom
-        if model_type:
-            self.model = GPT4All.get_model_from_type(model_type)
-        # Else get model from gpt4all model filenames
-        else:
-            model_filename = os.path.basename(model_path)
-            self.model = GPT4All.get_model_from_filename(model_filename)
-
-        self.model.load_model(model_path)
-
-    def generate(self, prompt: str, verbose: bool = True):
-        """
-        High level method for running generate on gpt4all models.
-        NOTE: Right now, this is essentially duplicate code but will be useful
-        if underlying models' prompt or generate begin to differ.
-        """
-        return self.model.generate(prompt, verbose=verbose)
-
-    @staticmethod
-    def get_model_from_type(model_type: str) -> pyllmodel.LLModel:
-        # This needs to be updated for each new model
-        # TODO: Might be worth converting model_type to enum
-
-        if model_type == "gptj":
-            return pyllmodel.GPTJModel()
-        elif model_type == "llama":
-            return pyllmodel.LlamaModel()
-        else:
-            raise ValueError(f"No corresponding model for model_type: {model_type}")
-        
-    @staticmethod
-    def get_model_from_filename(model_filename: str) -> pyllmodel.LLModel:
-        # This needs to be updated for each new model
-        GPTJ_MODELS = [
-            "ggml-gpt4all-j-v1.3-groovy.bin",
-            "ggml-gpt4all-j-v1.2-jazzy.bin",
-            "ggml-gpt4all-j-v1.1-breezy.bin",
-            "ggml-gpt4all-j.bin"
-        ]
-
-        LLAMA_MODELS = [
-            "ggml-gpt4all-l13b-snoozy.bin",
-            "ggml-vicuna-7b-1.1-q4_2.bin",
-            "ggml-vicuna-13b-1.1-q4_2.bin",
-            "ggml-wizardLM-7B.q4_2.bin",
-            "ggml-stable-vicuna-13B.q4_2.bin"
-        ]
-
-        if model_filename in GPTJ_MODELS:
-            return pyllmodel.GPTJModel()
-        elif model_filename in LLAMA_MODELS:
-            return pyllmodel.LlamaModel()
-        else:
-            err_msg = f"""No corresponding model for provided filename {model_filename}.
-            If this is a custom model, make sure to specify a valid model_type.
-            """
-            raise ValueError(err_msg)
+"""
+Python only API for running all GPT4All models.
+"""
+import json
+import os
+from pathlib import Path
+from typing import Dict, List
+
+import requests
+from tqdm import tqdm
+
+from . import pyllmodel
+
+# TODO: move to config
+DEFAULT_MODEL_DIRECTORY = os.path.join(str(Path.home()), ".cache", "gpt4all")
+
+class GPT4All():
+    """Python API for retrieving and interacting with GPT4All models
+    
+    Attribuies:
+        model: Pointer to underlying C model.
+    """
+
+    def __init__(self, model_name: str, model_path: str = None, model_type: str = None, allow_download=True):
+        """
+        Constructor
+
+        Args:
+            model_name: Name of GPT4All or custom model. Including ".bin" file extension is optional but encouraged.
+            model_path: Path to directory containing model file or, if file does not exist, where to download model.
+                Default is None, in which case models will be stored in `~/.cache/gpt4all/`.
+            model_type: Model architecture to use - currently, only options are 'llama' or 'gptj'. Only required if model
+                is custom. Note that these models still must be built from llama.cpp or GPTJ ggml architecture.
+                Default is None.
+            allow_download: Allow API to download models from gpt4all.io. Default is True. 
+        """
+        self.model = None
+
+        # Model type provided for when model is custom
+        if model_type:
+            self.model = GPT4All.get_model_from_type(model_type)
+        # Else get model from gpt4all model filenames
+        else:
+            self.model = GPT4All.get_model_from_name(model_name)
+
+        # Retrieve model and download if allowed
+        model_dest = self.retrieve_model(model_name, model_path=model_path, allow_download=allow_download)
+        self.model.load_model(model_dest)
+
+    @staticmethod
+    def list_models():
+        """
+        Fetch model list from https://gpt4all.io/models/models.json
+
+        Returns:
+            Model list in JSON format.
+        """
+        response = requests.get("https://gpt4all.io/models/models.json")
+        model_json = json.loads(response.content)
+        return model_json
+
+    @staticmethod
+    def retrieve_model(model_name: str, model_path: str = None, allow_download = True):
+        """
+        Find model file, and if it doesn't exist, download the model.
+
+        Args:
+            model_name: Name of model.
+            model_path: Path to find model. Default is None in which case path is set to
+                ~/.cache/gpt4all/.
+            allow_download: Allow API to download model from gpt4all.io. Default is True.
+
+        Returns:
+            Model file destination.
+        """
+        
+        model_filename = model_name
+        if ".bin" not in model_filename:
+            model_filename += ".bin"
+
+        # Validate download directory
+        if model_path == None:
+            model_path = DEFAULT_MODEL_DIRECTORY
+            if not os.path.exists(DEFAULT_MODEL_DIRECTORY):
+                try:
+                    os.makedirs(DEFAULT_MODEL_DIRECTORY)
+                except:
+                    raise ValueError("Failed to create model download directory at ~/.cache/gpt4all/. \
+                    Please specify download_dir.")
+
+        if os.path.exists(model_path):
+            model_dest = os.path.join(model_path, model_filename)
+            if os.path.exists(model_dest):
+                print("Found model file.")
+                return model_dest
+
+            # If model file does not exist, download
+            elif allow_download: 
+                # Make sure valid model filename before attempting download
+                model_match = False
+                for item in GPT4All.list_models():
+                    if model_filename == item["filename"]:
+                        model_match = True
+                        break
+                if not model_match:
+                    raise ValueError(f"Model filename not in model list: {model_filename}")
+                return GPT4All.download_model(model_filename, model_path)
+            else:
+                raise ValueError("Failed to retrieve model")
+        else:
+            raise ValueError("Invalid model directory")
+        
+    @staticmethod
+    def download_model(model_filename, model_path):
+        def get_download_url(model_filename):
+            return f"https://gpt4all.io/models/{model_filename}"
+    
+        # Download model
+        download_path = os.path.join(model_path, model_filename)
+        download_url = get_download_url(model_filename)
+
+        response = requests.get(download_url, stream=True)
+        total_size_in_bytes = int(response.headers.get("content-length", 0))
+        block_size = 1048576  # 1 MB
+        progress_bar = tqdm(total=total_size_in_bytes, unit="iB", unit_scale=True)
+        with open(download_path, "wb") as file:
+            for data in response.iter_content(block_size):
+                progress_bar.update(len(data))
+                file.write(data)
+        progress_bar.close()
+
+        # Validate download was successful
+        if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
+            raise RuntimeError(
+                "An error occurred during download. Downloaded file may not work."
+            )
+
+        print("Model downloaded at: " + download_path)
+        return download_path
+
+    def generate(self, prompt: str, **generate_kwargs):
+        """
+        Surfaced method of running generate without accessing model object.
+        """
+        return self.model.generate(prompt, **generate_kwargs)
+    
+    def chat_completion(self, 
+                        messages: List[Dict], 
+                        default_prompt_header: bool = True, 
+                        default_prompt_footer: bool = True, 
+                        verbose: bool = True) -> str:
+        """
+        Format list of message dictionaries into a prompt and call model
+        generate on prompt. Returns a response dictionary with metadata and
+        generated content.
+
+        Args:
+            messages: Each dictionary should have a "role" key
+                with value of "system", "assistant", or "user" and a "content" key with a
+                string value. Messages are organized such that "system" messages are at top of prompt,
+                and "user" and "assistant" messages are displayed in order. Assistant messages get formatted as
+                "Reponse: {content}". 
+            default_prompt_header: If True (default), add default prompt header after any user specified system messages and
+                before user/assistant messages.
+            default_prompt_footer: If True (default), add default footer at end of prompt.
+            verbose: If True (default), print full prompt and generated response.
+
+        Returns:
+            Response dictionary with:  
+                "model": name of model.  
+                "usage": a dictionary with number of full prompt tokens, number of 
+                    generated tokens in response, and total tokens.  
+                "choices": List of message dictionary where "content" is generated response and "role" is set
+                as "assistant". Right now, only one choice is returned by model.
+            
+        """
+       
+        full_prompt = self._build_prompt(messages, 
+                                        default_prompt_header=default_prompt_header, 
+                                        default_prompt_footer=default_prompt_footer)
+
+        if verbose:
+            print(full_prompt)
+
+        response = self.model.generate(full_prompt)
+
+        if verbose:
+            print(response)
+
+        response_dict = {
+            "model": self.model.model_name,
+            "usage": {"prompt_tokens": len(full_prompt), 
+                      "completion_tokens": len(response), 
+                      "total_tokens" : len(full_prompt) + len(response)},
+            "choices": [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": response
+                    }
+                }
+            ]
+        }
+
+        return response_dict
+    
+    @staticmethod
+    def _build_prompt(messages: List[Dict], 
+                      default_prompt_header=True, 
+                      default_prompt_footer=False) -> str:
+        full_prompt = ""
+
+        for message in messages:
+            if message["role"] == "system":
+                system_message = message["content"] + "\n"
+                full_prompt += system_message
+
+        if default_prompt_header:
+            full_prompt += """### Instruction: 
+            The prompt below is a question to answer, a task to complete, or a conversation 
+            to respond to; decide which and write an appropriate response.
+            \n### Prompt: """
+
+        for message in messages:
+            if message["role"] == "user":
+                user_message = "\n" + message["content"]
+                full_prompt += user_message
+            if message["role"] == "assistant":
+                assistant_message = "\n### Response: " + message["content"]
+                full_prompt += assistant_message
+
+        if default_prompt_footer:
+            full_prompt += "\n### Response:"
+
+        return full_prompt
+
+    @staticmethod
+    def get_model_from_type(model_type: str) -> pyllmodel.LLModel:
+        # This needs to be updated for each new model
+        # TODO: Might be worth converting model_type to enum
+
+        if model_type == "gptj":
+            return pyllmodel.GPTJModel()
+        elif model_type == "llama":
+            return pyllmodel.LlamaModel()
+        else:
+            raise ValueError(f"No corresponding model for model_type: {model_type}")
+        
+    @staticmethod
+    def get_model_from_name(model_name: str) -> pyllmodel.LLModel:
+        # This needs to be updated for each new model
+
+        # NOTE: We are doing this preprocessing a lot, maybe there's a better way to organize
+        if ".bin" not in model_name:
+            model_name += ".bin"
+
+        GPTJ_MODELS = [
+            "ggml-gpt4all-j-v1.3-groovy.bin",
+            "ggml-gpt4all-j-v1.2-jazzy.bin",
+            "ggml-gpt4all-j-v1.1-breezy.bin",
+            "ggml-gpt4all-j.bin"
+        ]
+
+        LLAMA_MODELS = [
+            "ggml-gpt4all-l13b-snoozy.bin",
+            "ggml-vicuna-7b-1.1-q4_2.bin",
+            "ggml-vicuna-13b-1.1-q4_2.bin",
+            "ggml-wizardLM-7B.q4_2.bin",
+            "ggml-stable-vicuna-13B.q4_2.bin"
+        ]
+
+        if model_name in GPTJ_MODELS:
+            return pyllmodel.GPTJModel()
+        elif model_name in LLAMA_MODELS:
+            return pyllmodel.LlamaModel()
+        else:
+            err_msg = f"""No corresponding model for provided filename {model_name}.
+            If this is a custom model, make sure to specify a valid model_type.
+            """
+            raise ValueError(err_msg)
```

## gpt4all/pyllmodel.py

```diff
@@ -1,254 +1,235 @@
-from io import StringIO
-import pkg_resources
-import ctypes
-import os
-import platform
-import re
-import sys
-
-# TODO: provide a config file to make this more robust
-LLMODEL_PATH = "llmodel_DO_NOT_MODIFY/build/"
-
-def load_llmodel_library():
-    system = platform.system()
-
-    def get_c_shared_lib_extension():
-        if system == "Darwin":
-            return "dylib"
-        elif system == "Linux":
-            return "so"
-        elif system == "Windows":
-            return "dll"
-        else:
-            raise Exception("Operating System not supported")
-        
-    c_lib_ext = get_c_shared_lib_extension()
-    
-    llmodel_file = "libllmodel" + '.' + c_lib_ext
-    llama_file = "libllama" + '.' + c_lib_ext
-    llama_dir = str(pkg_resources.resource_filename('gpt4all', LLMODEL_PATH + llama_file))
-    llmodel_dir = str(pkg_resources.resource_filename('gpt4all', LLMODEL_PATH + llmodel_file))
-
-    llama_lib = ctypes.CDLL(llama_dir, mode=ctypes.RTLD_GLOBAL)
-
-    llmodel_lib = ctypes.CDLL(llmodel_dir)
-
-    return llmodel_lib, llama_lib
-
-
-llmodel, llama = load_llmodel_library()
-
-# Define C function signatures using ctypes
-llmodel.llmodel_gptj_create.restype = ctypes.c_void_p
-llmodel.llmodel_gptj_destroy.argtypes = [ctypes.c_void_p]
-llmodel.llmodel_llama_create.restype = ctypes.c_void_p
-llmodel.llmodel_llama_destroy.argtypes = [ctypes.c_void_p]
-
-llmodel.llmodel_loadModel.argtypes = [ctypes.c_void_p, ctypes.c_char_p]
-llmodel.llmodel_loadModel.restype = ctypes.c_bool
-llmodel.llmodel_isModelLoaded.argtypes = [ctypes.c_void_p]
-llmodel.llmodel_isModelLoaded.restype = ctypes.c_bool
-
-class LLModelPromptContext(ctypes.Structure):
-    _fields_ = [("logits", ctypes.POINTER(ctypes.c_float)),
-                ("logits_size", ctypes.c_size_t),
-                ("tokens", ctypes.POINTER(ctypes.c_int32)),
-                ("tokens_size", ctypes.c_size_t),
-                ("n_past", ctypes.c_int32),
-                ("n_ctx", ctypes.c_int32),
-                ("n_predict", ctypes.c_int32),
-                ("top_k", ctypes.c_int32),
-                ("top_p", ctypes.c_float),
-                ("temp", ctypes.c_float),
-                ("n_batch", ctypes.c_int32),
-                ("repeat_penalty", ctypes.c_float),
-                ("repeat_last_n", ctypes.c_int32),
-                ("context_erase", ctypes.c_float)]
-    
-ResponseCallback = ctypes.CFUNCTYPE(ctypes.c_bool, ctypes.c_int32, ctypes.c_char_p)
-RecalculateCallback = ctypes.CFUNCTYPE(ctypes.c_bool, ctypes.c_bool)
-
-llmodel.llmodel_prompt.argtypes = [ctypes.c_void_p, 
-                                   ctypes.c_char_p, 
-                                   ResponseCallback, 
-                                   ResponseCallback, 
-                                   RecalculateCallback, 
-                                   ctypes.POINTER(LLModelPromptContext)]
-
-
-class LLModel:
-    """
-    Base class and universal wrapper for GPT4All language models
-    built around llmodel C-API.
-
-    Attributes
-    ----------
-    model: llmodel_model
-        Ctype pointer to underlying model
-    model_type : str
-        Model architecture identifier
-    """
-
-    model_type: str = None
-
-    def __init__(self):
-        self.model = None
-
-    def __del__(self):
-        pass
-
-    def load_model(self, model_path: str) -> bool:
-        """
-        Load model from a file.
-
-        Parameters
-        ----------
-        model_path : str
-            Model filepath
-
-        Returns
-        -------
-        True if model loaded successfully, False otherwise
-        """
-        llmodel.llmodel_loadModel(self.model, model_path.encode('utf-8'))
-    
-        if llmodel.llmodel_isModelLoaded(self.model):
-            return True
-        else:
-            return False
-
-    def generate(self, 
-                 prompt: str,
-                 add_default_header: bool = True, 
-                 add_default_footer: bool = True,
-                 logits_size: int = 0, 
-                 tokens_size: int = 0, 
-                 n_past: int = 0, 
-                 n_ctx: int = 1024, 
-                 n_predict: int = 128, 
-                 top_k: int = 40, 
-                 top_p: float = .9, 
-                 temp: float = .1, 
-                 n_batch: int = 8, 
-                 repeat_penalty: float = 1.2, 
-                 repeat_last_n: int = 10, 
-                 context_erase: float = .5,
-                 verbose: bool = True) -> str:
-        """
-        Generate response from model from a prompt.
-
-        Parameters
-        ----------
-        prompt: str
-            Question, task, or conversation for model to respond to
-        add_default_header: bool, optional
-            Whether to add a prompt header (default is True)
-        add_default_footer: bool, optional
-            Whether to add a prompt footer (default is True)
-        verbose: bool, optional
-            Whether to print prompt and response
-
-        Returns
-        -------
-        Model response str
-        """
-
-        full_prompt = ""
-        if add_default_header:
-            full_prompt += """### Instruction:\n 
-            The prompt below is a question to answer, a task to complete, or a conversation 
-            to respond to; decide which and write an appropriate response.
-            \n### Prompt: """
-        
-        full_prompt += prompt
-
-        if add_default_footer:
-            full_prompt += "\n### Response:"
-
-        if verbose:
-            print(full_prompt)
-        
-        full_prompt = full_prompt.encode('utf-8')
-        full_prompt = ctypes.c_char_p(full_prompt)
-
-        # Change stdout to StringIO so we can collect response
-        old_stdout = sys.stdout 
-        collect_response = StringIO()
-        sys.stdout = collect_response
-
-        context = LLModelPromptContext(
-            logits_size=logits_size, 
-            tokens_size=tokens_size, 
-            n_past=n_past, 
-            n_ctx=n_ctx, 
-            n_predict=n_predict, 
-            top_k=top_k, 
-            top_p=top_p, 
-            temp=temp, 
-            n_batch=n_batch, 
-            repeat_penalty=repeat_penalty, 
-            repeat_last_n=repeat_last_n, 
-            context_erase=context_erase
-        )
-
-        llmodel.llmodel_prompt(self.model, 
-                               full_prompt, 
-                               ResponseCallback(self._prompt_callback), 
-                               ResponseCallback(self._response_callback), 
-                               RecalculateCallback(self._recalculate_callback), 
-                               context)
-        
-        response = collect_response.getvalue()
-        sys.stdout = old_stdout
-
-        response = re.sub(r"\n(?!\n)", "", response)
-
-        if verbose:
-            print(response)
-        
-        # Remove the unnecessary new lines from response
-        return response
-
-    # Empty prompt callback
-    @staticmethod
-    def _prompt_callback(token_id, response):
-        return True
-
-    # Empty response callback method that just prints response to be collected
-    @staticmethod
-    def _response_callback(token_id, response):
-        print(response.decode('utf-8'))
-        return True
-
-    # Empty recalculate callback
-    @staticmethod
-    def _recalculate_callback(is_recalculating):
-        return is_recalculating
-
-
-class GPTJModel(LLModel):
-
-    model_type = "gptj"
-
-    def __init__(self):
-        super().__init__()
-        self.model = llmodel.llmodel_gptj_create()
-
-    def __del__(self):
-        if self.model is not None:
-            llmodel.llmodel_gptj_destroy(self.model)
-        super().__del__()
-
-
-class LlamaModel(LLModel):
-
-    model_type = "llama"
-
-    def __init__(self):
-        super().__init__()
-        self.model = llmodel.llmodel_llama_create()
-
-    def __del__(self):
-        if self.model is not None:
-            llmodel.llmodel_llama_destroy(self.model)
-        super().__del__()
+from io import StringIO
+import pkg_resources
+import ctypes
+import os
+import platform
+import re
+import sys
+
+# TODO: provide a config file to make this more robust
+LLMODEL_PATH = "llmodel_DO_NOT_MODIFY/build/"
+
+def load_llmodel_library():
+    system = platform.system()
+
+    def get_c_shared_lib_extension():
+        if system == "Darwin":
+            return "dylib"
+        elif system == "Linux":
+            return "so"
+        elif system == "Windows":
+            return "dll"
+        else:
+            raise Exception("Operating System not supported")
+        
+    c_lib_ext = get_c_shared_lib_extension()
+    
+    llmodel_file = "libllmodel" + '.' + c_lib_ext
+    llama_file = "libllama" + '.' + c_lib_ext
+    llama_dir = str(pkg_resources.resource_filename('gpt4all', LLMODEL_PATH + llama_file))
+    llmodel_dir = str(pkg_resources.resource_filename('gpt4all', LLMODEL_PATH + llmodel_file))
+
+    llama_lib = ctypes.CDLL(llama_dir, mode=ctypes.RTLD_GLOBAL)
+    llmodel_lib = ctypes.CDLL(llmodel_dir)
+
+    return llmodel_lib, llama_lib
+
+
+llmodel, llama = load_llmodel_library()
+
+# Define C function signatures using ctypes
+llmodel.llmodel_gptj_create.restype = ctypes.c_void_p
+llmodel.llmodel_gptj_destroy.argtypes = [ctypes.c_void_p]
+llmodel.llmodel_llama_create.restype = ctypes.c_void_p
+llmodel.llmodel_llama_destroy.argtypes = [ctypes.c_void_p]
+
+llmodel.llmodel_loadModel.argtypes = [ctypes.c_void_p, ctypes.c_char_p]
+llmodel.llmodel_loadModel.restype = ctypes.c_bool
+llmodel.llmodel_isModelLoaded.argtypes = [ctypes.c_void_p]
+llmodel.llmodel_isModelLoaded.restype = ctypes.c_bool
+
+class LLModelPromptContext(ctypes.Structure):
+    _fields_ = [("logits", ctypes.POINTER(ctypes.c_float)),
+                ("logits_size", ctypes.c_size_t),
+                ("tokens", ctypes.POINTER(ctypes.c_int32)),
+                ("tokens_size", ctypes.c_size_t),
+                ("n_past", ctypes.c_int32),
+                ("n_ctx", ctypes.c_int32),
+                ("n_predict", ctypes.c_int32),
+                ("top_k", ctypes.c_int32),
+                ("top_p", ctypes.c_float),
+                ("temp", ctypes.c_float),
+                ("n_batch", ctypes.c_int32),
+                ("repeat_penalty", ctypes.c_float),
+                ("repeat_last_n", ctypes.c_int32),
+                ("context_erase", ctypes.c_float)]
+    
+ResponseCallback = ctypes.CFUNCTYPE(ctypes.c_bool, ctypes.c_int32, ctypes.c_char_p)
+RecalculateCallback = ctypes.CFUNCTYPE(ctypes.c_bool, ctypes.c_bool)
+
+llmodel.llmodel_prompt.argtypes = [ctypes.c_void_p, 
+                                   ctypes.c_char_p, 
+                                   ResponseCallback, 
+                                   ResponseCallback, 
+                                   RecalculateCallback, 
+                                   ctypes.POINTER(LLModelPromptContext)]
+
+
+class LLModel:
+    """
+    Base class and universal wrapper for GPT4All language models
+    built around llmodel C-API.
+
+    Attributes
+    ----------
+    model: llmodel_model
+        Ctype pointer to underlying model
+    model_type : str
+        Model architecture identifier
+    """
+
+    model_type: str = None
+
+    def __init__(self):
+        self.model = None
+        self.model_name = None
+
+    def __del__(self):
+        pass
+
+    def load_model(self, model_path: str) -> bool:
+        """
+        Load model from a file.
+
+        Parameters
+        ----------
+        model_path : str
+            Model filepath
+
+        Returns
+        -------
+        True if model loaded successfully, False otherwise
+        """
+        llmodel.llmodel_loadModel(self.model, model_path.encode('utf-8'))
+        filename = os.path.basename(model_path)
+        self.model_name = os.path.splitext(filename)[0]
+    
+        if llmodel.llmodel_isModelLoaded(self.model):
+            return True
+        else:
+            return False
+
+    def generate(self, 
+                 prompt: str,
+                 logits_size: int = 0, 
+                 tokens_size: int = 0, 
+                 n_past: int = 0, 
+                 n_ctx: int = 1024, 
+                 n_predict: int = 128, 
+                 top_k: int = 40, 
+                 top_p: float = .9, 
+                 temp: float = .1, 
+                 n_batch: int = 8, 
+                 repeat_penalty: float = 1.2, 
+                 repeat_last_n: int = 10, 
+                 context_erase: float = .5) -> str:
+        """
+        Generate response from model from a prompt.
+
+        Parameters
+        ----------
+        prompt: str
+            Question, task, or conversation for model to respond to
+        add_default_header: bool, optional
+            Whether to add a prompt header (default is True)
+        add_default_footer: bool, optional
+            Whether to add a prompt footer (default is True)
+        verbose: bool, optional
+            Whether to print prompt and response
+
+        Returns
+        -------
+        Model response str
+        """
+        
+        prompt = prompt.encode('utf-8')
+        prompt = ctypes.c_char_p(prompt)
+
+        # Change stdout to StringIO so we can collect response
+        old_stdout = sys.stdout 
+        collect_response = StringIO()
+        sys.stdout = collect_response
+
+        context = LLModelPromptContext(
+            logits_size=logits_size, 
+            tokens_size=tokens_size, 
+            n_past=n_past, 
+            n_ctx=n_ctx, 
+            n_predict=n_predict, 
+            top_k=top_k, 
+            top_p=top_p, 
+            temp=temp, 
+            n_batch=n_batch, 
+            repeat_penalty=repeat_penalty, 
+            repeat_last_n=repeat_last_n, 
+            context_erase=context_erase
+        )
+
+        llmodel.llmodel_prompt(self.model, 
+                               prompt, 
+                               ResponseCallback(self._prompt_callback), 
+                               ResponseCallback(self._response_callback), 
+                               RecalculateCallback(self._recalculate_callback), 
+                               context)
+        
+        response = collect_response.getvalue()
+        sys.stdout = old_stdout
+
+        # Remove the unnecessary new lines from response
+        response = re.sub(r"\n(?!\n)", "", response).strip()
+        
+        return response
+
+    # Empty prompt callback
+    @staticmethod
+    def _prompt_callback(token_id, response):
+        return True
+
+    # Empty response callback method that just prints response to be collected
+    @staticmethod
+    def _response_callback(token_id, response):
+        print(response.decode('utf-8'))
+        return True
+
+    # Empty recalculate callback
+    @staticmethod
+    def _recalculate_callback(is_recalculating):
+        return is_recalculating
+
+
+class GPTJModel(LLModel):
+
+    model_type = "gptj"
+
+    def __init__(self):
+        super().__init__()
+        self.model = llmodel.llmodel_gptj_create()
+
+    def __del__(self):
+        if self.model is not None:
+            llmodel.llmodel_gptj_destroy(self.model)
+        super().__del__()
+
+
+class LlamaModel(LLModel):
+
+    model_type = "llama"
+
+    def __init__(self):
+        super().__init__()
+        self.model = llmodel.llmodel_llama_create()
+
+    def __del__(self):
+        if self.model is not None:
+            llmodel.llmodel_llama_destroy(self.model)
+        super().__del__()
```

## tests/test_gpt4all.py

```diff
@@ -1,22 +1,62 @@
-import pytest
-
-from gpt4all.gpt4all import GPT4All
-
-def test_invalid_model_type():
-    model_type = "bad_type"
-    with pytest.raises(ValueError):
-        GPT4All.get_model_from_type(model_type)
-
-def test_valid_model_type():
-    model_type = "gptj"
-    assert GPT4All.get_model_from_type(model_type).model_type == model_type
-
-def test_invalid_model_filename():
-    model_filename = "bad_filename.bin"
-    with pytest.raises(ValueError):
-        GPT4All.get_model_from_filename(model_filename)
-
-def test_valid_model_filename():
-    model_filename = "ggml-gpt4all-l13b-snoozy.bin"
-    model_type = "gptj"
-    assert GPT4All.get_model_from_filename(model_filename).model_type == model_type
+import pytest
+
+from gpt4all.gpt4all import GPT4All
+
+def test_invalid_model_type():
+    model_type = "bad_type"
+    with pytest.raises(ValueError):
+        GPT4All.get_model_from_type(model_type)
+
+def test_valid_model_type():
+    model_type = "gptj"
+    assert GPT4All.get_model_from_type(model_type).model_type == model_type
+
+def test_invalid_model_name():
+    model_name = "bad_filename.bin"
+    with pytest.raises(ValueError):
+        GPT4All.get_model_from_name(model_name)
+
+def test_valid_model_name():
+    model_name = "ggml-gpt4all-l13b-snoozy"
+    model_type = "llama"
+    assert GPT4All.get_model_from_name(model_name).model_type == model_type
+    model_name += ".bin"
+    assert GPT4All.get_model_from_name(model_name).model_type == model_type
+
+def test_build_prompt():
+    messages = [
+        {
+            "role": "system",
+            "content": "You are a helpful assistant."
+        },
+        {
+            "role": "user",
+            "content": "Hello there."
+        },
+        {
+            "role": "assistant",
+            "content": "Hi, how can I help you?"
+        },
+        {
+            "role": "user",
+            "content": "Reverse a list in Python."
+        }
+    ]
+
+    expected_prompt = """You are a helpful assistant.\
+    \n### Instruction:
+            The prompt below is a question to answer, a task to complete, or a conversation 
+            to respond to; decide which and write an appropriate response.\
+    ### Prompt:\
+    Hello there.\
+    Response: Hi, how can I help you?\
+    Reverse a list in Python.\
+    ### Response:"""
+
+    print(expected_prompt)
+
+    full_prompt = GPT4All._build_prompt(messages, default_prompt_footer=True, default_prompt_header=True)
+
+    print("\n\n\n")
+    print(full_prompt)
+    assert len(full_prompt) == len(expected_prompt)
```

## tests/test_pyllmodel.py

 * *Ordering differences only*

```diff
@@ -1,44 +1,44 @@
-from io import StringIO
-import sys
-
-from gpt4all import pyllmodel
-
-# TODO: Integration test for loadmodel and prompt. 
-# # Right now, too slow b/c it requries file download.
-
-def test_create_gptj():
-    gptj = pyllmodel.GPTJModel()
-    assert gptj.model_type == "gptj"
-
-def test_create_llama():
-    llama = pyllmodel.LlamaModel()
-    assert llama.model_type == "llama"
-
-def prompt_unloaded_gptj():
-    gptj = pyllmodel.GPTJModel()
-    old_stdout = sys.stdout 
-    collect_response = StringIO()
-    sys.stdout = collect_response
-
-    gptj.prompt("hello there")
-
-    response = collect_response.getvalue()
-    sys.stdout = old_stdout
-
-    response = response.strip()
-    assert response == "GPT-J ERROR: prompt won't work with an unloaded model!"
-
-def prompt_unloaded_llama():
-    llama = pyllmodel.LlamaModel()
-    old_stdout = sys.stdout 
-    collect_response = StringIO()
-    sys.stdout = collect_response
-
-    llama.prompt("hello there")
-
-    response = collect_response.getvalue()
-    sys.stdout = old_stdout
-
-    response = response.strip()
-    assert response == "LLAMA ERROR: prompt won't work with an unloaded model!"
+from io import StringIO
+import sys
+
+from gpt4all import pyllmodel
+
+# TODO: Integration test for loadmodel and prompt. 
+# # Right now, too slow b/c it requries file download.
+
+def test_create_gptj():
+    gptj = pyllmodel.GPTJModel()
+    assert gptj.model_type == "gptj"
+
+def test_create_llama():
+    llama = pyllmodel.LlamaModel()
+    assert llama.model_type == "llama"
+
+def prompt_unloaded_gptj():
+    gptj = pyllmodel.GPTJModel()
+    old_stdout = sys.stdout 
+    collect_response = StringIO()
+    sys.stdout = collect_response
+
+    gptj.prompt("hello there")
+
+    response = collect_response.getvalue()
+    sys.stdout = old_stdout
+
+    response = response.strip()
+    assert response == "GPT-J ERROR: prompt won't work with an unloaded model!"
+
+def prompt_unloaded_llama():
+    llama = pyllmodel.LlamaModel()
+    old_stdout = sys.stdout 
+    collect_response = StringIO()
+    sys.stdout = collect_response
+
+    llama.prompt("hello there")
+
+    response = collect_response.getvalue()
+    sys.stdout = old_stdout
+
+    response = response.strip()
+    assert response == "LLAMA ERROR: prompt won't work with an unloaded model!"
```

## Comparing `gpt4all-0.1.7.dist-info/LICENSE.txt` & `gpt4all-0.1.8.dist-info/LICENSE.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 Nomic, Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2023 Nomic, Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

