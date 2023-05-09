# Comparing `tmp/sum_pai-0.3.0.tar.gz` & `tmp/sum_pai-0.4.0.tar.gz`

## Comparing `sum_pai-0.3.0.tar` & `sum_pai-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.isort.cfg
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.3.0/clean_all.bat
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.3.0/clean_all.sh
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.3.0/clean_sumpai.py
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 sum_pai-0.3.0/publish.bat
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.3.0/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.3.0/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.3.0/qa.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.3.0/run_pylint.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sum_pai-0.3.0/search_embedding_1442409337828784761.pickle
--rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 sum_pai-0.3.0/ss.png
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.3.0/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.3.0/style.sh
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sum_pai-0.3.0/test.ipynb
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/__init__.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/__main__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/code_extractor.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/constants.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/create_search_embedding.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/file_io.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/loguru_config.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/batch.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/convert.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/create.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/length_safe.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/__init__.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/classes.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/code_element.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/compare.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/directory.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/file.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/functions.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/global_level.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/summary_embed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search/knn.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search/svm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/summary/__init__.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/summary/text.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.3.0/LICENSE
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 sum_pai-0.3.0/README.md
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 sum_pai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 sum_pai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.4.0/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.4.0/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.4.0/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.4.0/.isort.cfg
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.4.0/clean_all.bat
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.4.0/clean_all.sh
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.4.0/clean_sumpai.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 sum_pai-0.4.0/publish.bat
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.4.0/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.4.0/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.4.0/qa.sh
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.4.0/run_pylint.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sum_pai-0.4.0/search_embedding_1442409337828784761.pickle
+-rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 sum_pai-0.4.0/ss.png
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.4.0/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.4.0/style.sh
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sum_pai-0.4.0/test.ipynb
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/__init__.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/__main__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/code_extractor.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/constants.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/create_search_embedding.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/file_io.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/loguru_config.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/search_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/embedding/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/embedding/batch.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/embedding/convert.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/embedding/create.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/embedding/length_safe.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/embedding/loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/__init__.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/classes.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/code_element.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/compare.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/directory.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/file.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/functions.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/global_level.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/process/summary_embed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/search/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/search/knn.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/search/svm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/summary/__init__.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/summary/chat_completion.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/summary/code.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/summary/feature.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 sum_pai-0.4.0/src/sum_pai/summary/text.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 sum_pai-0.4.0/README.md
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 sum_pai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 sum_pai-0.4.0/PKG-INFO
```

### Comparing `sum_pai-0.3.0/.coveragerc` & `sum_pai-0.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/clean_sumpai.py` & `sum_pai-0.4.0/clean_sumpai.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/pylintrc` & `sum_pai-0.4.0/pylintrc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/search_embedding_1442409337828784761.pickle` & `sum_pai-0.4.0/search_embedding_1442409337828784761.pickle`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/ss.png` & `sum_pai-0.4.0/ss.png`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/test.ipynb` & `sum_pai-0.4.0/test.ipynb`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/__main__.py` & `sum_pai-0.4.0/src/sum_pai/__main__.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/code_extractor.py` & `sum_pai-0.4.0/src/sum_pai/code_extractor.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/create_search_embedding.py` & `sum_pai-0.4.0/src/sum_pai/create_search_embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-import click
 import os
 import pickle
+
 import cityhash
+import click
+
 from sum_pai.embedding.convert import convert_embeddings_to_np
 from sum_pai.embedding.length_safe import len_safe_get_embedding
-
 from sum_pai.summary.text import summarize_text
 
 
 @click.command()
-@click.option("--text", prompt="Enter the text to summarize and create an embedding", 
-              help="Text to summarize and create an embedding.")
+@click.option(
+    "--text",
+    prompt="Enter the text to summarize and create an embedding",
+    help="Text to summarize and create an embedding.",
+)
 def main(text: str):
     return create_search(text)
 
 
 def create_search(text: str):
     """
     Summarizes the input text and creates a search embedding.
@@ -24,30 +28,26 @@
     """
 
     city_hash = cityhash.CityHash64(text)
     file_name = f"search_embedding_{city_hash}.pickle"
     if os.path.exists(file_name):
         print(f"Search embedding already exists for {text}")
         return pickle.load(open(file_name, "rb"))
-    
+
     # Summarize the input text
     summary = summarize_text(text)
     print(f"Summary: {summary}")
 
     # Create the search embedding
     _, embedding = len_safe_get_embedding(text)
     # len_safe_get_embedding(f"Summary: {summary} Code: {text}")
 
     # Convert the embedding to a NumPy array and print it
     embedding_array = convert_embeddings_to_np(embedding)
-    search_embedding = {
-        "embedding": embedding_array,
-        "summary": summary,
-        "text": text
-    }
+    search_embedding = {"embedding": embedding_array, "summary": summary, "text": text}
     with open(file_name, "wb") as f:
         pickle.dump(search_embedding, f)
     print(f"Search embedding created for {text}")
     return search_embedding
 
 
 if __name__ == "__main__":
```

### Comparing `sum_pai-0.3.0/src/sum_pai/search_project.py` & `sum_pai-0.4.0/src/sum_pai/search_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-import click
 import os
 import pickle
+
+import click
 import numpy as np
 from loguru import logger
+
 from sum_pai.create_search_embedding import create_search
 from sum_pai.embedding.convert import convert_embeddings_to_np
 
 
 @click.command()
-@click.option("--text", prompt="Enter the text to search for", 
-              help="Text to search for.")
-@click.option("--target", prompt="Enter the target directory", 
-              help="The project to scan.")
-@click.option("--search-type", default="svm",
-              help="The type of search to perform.")
+@click.option(
+    "--text", prompt="Enter the text to search for", help="Text to search for."
+)
+@click.option(
+    "--target", prompt="Enter the target directory", help="The project to scan."
+)
+@click.option("--search-type", default="svm", help="The type of search to perform.")
 def main(text: str, target: str, search_type: str):
     """
     Summarizes the input text and creates a search embedding.
 
     Args:
         text (str): The text to be summarized and used to create an embedding.
         target (str): The project to scan.
@@ -42,15 +45,15 @@
         for file in files:
             if file.endswith(".sumpai"):
                 file_path = os.path.join(root, file)
                 with open(file_path, "rb") as f:
                     summaries.append(pickle.load(f))
     embeddings = [summary["embedding"] for summary in summaries]
     logger.debug(f"Embeddings: {len(embeddings)}")
-    
+
     vector = None
     for embed in embeddings:
         logger.debug(f"Chunked Embeddings: {len(embed[1])}")
         embed = convert_embeddings_to_np(embed[0][0])
         logger.debug(f"Chunked Embedding: {len(embed)}")
         embed = embed[np.newaxis, :]
         if vector is None:
@@ -63,17 +66,19 @@
                 ],
                 axis=0,
             )
     logger.debug(f"Vector: {vector.shape}")
 
     if search_type == "knn":
         from sum_pai.search.knn import knn_search
+
         result = knn_search(vector, search_embedding["embedding"])
     elif search_type == "svm":
         from sum_pai.search.svm import svm_search
+
         result = svm_search(vector, search_embedding["embedding"])
     else:
         raise ValueError(f"Invalid search type: {search_type}")
     logger.debug(f"result: {result}")
     logger.info(f"Search complete for {text} in {target}")
     logger.info("Results:")
     summary_found = summaries[result[0]]
```

### Comparing `sum_pai-0.3.0/src/sum_pai/embedding/batch.py` & `sum_pai-0.4.0/src/sum_pai/embedding/batch.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/embedding/create.py` & `sum_pai-0.4.0/src/sum_pai/embedding/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 
 from sum_pai.constants import EMBEDDING_MODEL
 
 
 @retry(
     wait=wait_random_exponential(min=1, max=20),
-    stop=stop_after_attempt(2),
+    stop=stop_after_attempt(4),
     retry=retry_if_not_exception_type(openai.InvalidRequestError),
 )
 def get_embedding(
     text_or_tokens: Union[str, List[str]],
     model: str = EMBEDDING_MODEL,
     hashed_key: Optional[str] = None,
 ) -> List[float]:
```

### Comparing `sum_pai-0.3.0/src/sum_pai/embedding/length_safe.py` & `sum_pai-0.4.0/src/sum_pai/embedding/length_safe.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/embedding/loading.py` & `sum_pai-0.4.0/src/sum_pai/embedding/loading.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/process/classes.py` & `sum_pai-0.4.0/src/sum_pai/process/classes.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/process/code_element.py` & `sum_pai-0.4.0/src/sum_pai/process/code_element.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/process/compare.py` & `sum_pai-0.4.0/src/sum_pai/process/compare.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/process/directory.py` & `sum_pai-0.4.0/src/sum_pai/process/directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import cityhash
 from loguru import logger
 
 from sum_pai.file_io import save_sum
 from sum_pai.process.compare import same_hash
 from sum_pai.process.file import process_file
 from sum_pai.process.summary_embed import summarize_and_embed
-from sum_pai.summary.text import summarize_text
+from sum_pai.summary.feature import summarize_features
 
 
 def process_directory(directory_path: str) -> None:
     """Processes all Python files within a directory and its subdirectories.
 
     Args:
         directory_path (str): The path to the directory containing Python files
@@ -26,24 +26,25 @@
                 file_path = os.path.join(root, file)
                 file_summary = process_file(file_path)
                 if file_summary:
                     file_summaries[file_path] = file_summary
     logger.info(f"Processed {len(file_summaries)} files")
     collated_summary = "\n".join(
         [
-            f"{file_path}: {file_summary}\n"
+            f"File: {file_path}: {file_summary}\n"
             for file_path, file_summary in file_summaries.items()
+            if not file_summary.strip().startswith("As an AI")
         ]
     )
     logger.debug(f"Collated summary:\n{collated_summary}")
     city_hash = cityhash.CityHash64(collated_summary)
     existing_output_name = f"{directory_path}__dir_overview.sumpai"
     if same_hash(city_hash, "dir_overview", existing_output_name, path_is_full=True):
         return
-    summary = summarize_text(collated_summary)
+    summary = summarize_features(collated_summary)
     logger.debug(f"Summary:\n{summary}")
     save_sum(
         existing_output_name,
         summarize_and_embed(
             collated_summary, "directory", "dir_overview", directory_path, summary
         ),
     )
```

### Comparing `sum_pai-0.3.0/src/sum_pai/process/file.py` & `sum_pai-0.4.0/src/sum_pai/process/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import cityhash
 
 from sum_pai.file_io import load_sum, save_sum
 from sum_pai.process.code_element import process_code_elements
 from sum_pai.process.compare import same_hash
 from sum_pai.process.summary_embed import summarize_and_embed
-from sum_pai.summary.text import summarize_text
+from sum_pai.summary.feature import summarize_features
 
 
 def process_file(file_path: str) -> Optional[str]:
     """
     Processes a Python file, generating summaries and embeddings for its elements.
 
     Args:
@@ -31,15 +31,15 @@
     existing_output_name = f"{path_no_ext}.sumpai"
     if loaded_sum := same_hash(
         city_hash, "file", existing_output_name, path_is_full=True
     ):
         return loaded_sum["summary"]
     code_elements = process_code_elements(code, str(path))
     summaries = [element["summary"] for element in code_elements]
-    file_summary = summarize_text("\n".join(summaries))
+    file_summary = summarize_features("\n".join(summaries))
 
     save_sum(
         existing_output_name,
         summarize_and_embed(code, "file", path.name, path_no_ext, file_summary),
     )
     for element in code_elements:
         output_name = f"{path_no_ext}__{element['name']}.sumpai"
```

### Comparing `sum_pai-0.3.0/src/sum_pai/process/functions.py` & `sum_pai-0.4.0/src/sum_pai/process/functions.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/process/global_level.py` & `sum_pai-0.4.0/src/sum_pai/process/global_level.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/src/sum_pai/process/summary_embed.py` & `sum_pai-0.4.0/src/sum_pai/process/summary_embed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Any, Dict, Optional
 
 import cityhash
+from loguru import logger
 
 from sum_pai.embedding.length_safe import len_safe_get_embedding
-from sum_pai.summary.text import summarize_code
+from sum_pai.summary.code import summarize_code
+from sum_pai.summary.text import summarize_text
 
 
 def summarize_and_embed(
     source: str,
     source_type: str,
     name: str,
     path: str,
@@ -23,16 +25,24 @@
         name (str): The name of the code element.
         path (str): The file path of the code element.
 
     Returns:
         Dict[str, Any]: A dictionary containing the type, name, path,
           summary, and embedding of the code element.
     """
+    logger.info(
+        f"Summarizing and embedding code for: {name} path:"
+        f" {path} type: {source_type}"
+    )
+    system = None
     if summary is None:
-        summary = summarize_code(source)
+        if source_type == "directory":
+            summary = summarize_text(source)
+        else:
+            summary = summarize_code(source, system=system)
     if city_hash is None:
         city_hash = cityhash.CityHash64(source)
     embedding = len_safe_get_embedding(f"Summary: {summary} Code: {source}")
     return {
         "type": source_type,
         "name": name,
         "path": path,
```

### Comparing `sum_pai-0.3.0/src/sum_pai/search/svm.py` & `sum_pai-0.4.0/src/sum_pai/search/svm.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/.gitignore` & `sum_pai-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/LICENSE` & `sum_pai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_pai-0.3.0/README.md` & `sum_pai-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 It will also skip classes and functions and globals if they were not changed.
 
 It is intended for the files to be commited to the git repo and not for use by humans, it might make sense to hide these files in the future.
 
 If you're not sure why you might need to run this you probably don't.
 
+If you have a large project be aware that this code will scale models based on token count, for very large projects this might mean you will use gpt-4-32k.
+
 ## Installation
 
 ```
 pip install sum-pai
 ```
 
 ## Usage
```

### Comparing `sum_pai-0.3.0/pyproject.toml` & `sum_pai-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sum-pai"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "A Python library for cataloging and searching python files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sum_pai-0.3.0/PKG-INFO` & `sum_pai-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum-pai
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for cataloging and searching python files.
 Project-URL: Homepage, https://github.com/BillSchumacher/SumPAI
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/SumPAI
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,14 +57,16 @@
 
 It will also skip classes and functions and globals if they were not changed.
 
 It is intended for the files to be commited to the git repo and not for use by humans, it might make sense to hide these files in the future.
 
 If you're not sure why you might need to run this you probably don't.
 
+If you have a large project be aware that this code will scale models based on token count, for very large projects this might mean you will use gpt-4-32k.
+
 ## Installation
 
 ```
 pip install sum-pai
 ```
 
 ## Usage
```

