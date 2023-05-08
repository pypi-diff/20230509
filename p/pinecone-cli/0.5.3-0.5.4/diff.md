# Comparing `tmp/pinecone_cli-0.5.3-py3-none-any.whl.zip` & `tmp/pinecone_cli-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17258 bytes, number of entries: 8
--rw-r--r--  2.0 unx    37249 b- defN 23-May-08 21:15 pinecli.py
--rw-r--r--  2.0 unx     1066 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    16800 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-27 19:09 pinecone_cli-0.5.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      670 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/RECORD
-8 files, 55926 bytes uncompressed, 16076 bytes compressed:  71.3%
+Zip file size: 17165 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    36709 b- defN 23-May-08 23:35 pinecli.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-May-08 23:36 pinecone_cli-0.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16800 b- defN 23-May-08 23:36 pinecone_cli-0.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 23:36 pinecone_cli-0.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-08 23:36 pinecone_cli-0.5.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-08 23:36 pinecone_cli-0.5.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Mar-27 19:09 pinecone_cli-0.5.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      670 b- defN 23-May-08 23:36 pinecone_cli-0.5.4.dist-info/RECORD
+8 files, 55386 bytes uncompressed, 15983 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pinecli.py
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/LICENSE
+Filename: pinecone_cli-0.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/METADATA
+Filename: pinecone_cli-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/WHEEL
+Filename: pinecone_cli-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/entry_points.txt
+Filename: pinecone_cli-0.5.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/top_level.txt
+Filename: pinecone_cli-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/zip-safe
+Filename: pinecone_cli-0.5.4.dist-info/zip-safe
 Comment: 
 
-Filename: pinecone_cli-0.5.3.dist-info/RECORD
+Filename: pinecone_cli-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pinecli.py

```diff
@@ -26,84 +26,55 @@
 from numpy import random
 from sklearn.manifold import TSNE
 from sklearn.cluster import KMeans
 from retry import retry
 from rich.console import Console
 from rich.table import Table
 from tqdm.auto import tqdm
-from typing import Dict, List, Tuple, Optional, Union, TypeVar
+from typing import List, Optional, TypeVar
 
 DEFAULT_REGION = 'us-west1-gcp'
 OPENAI_EMBED_MODEL = "text-embedding-ada-002"
 REGION_HELP = 'Pinecone cluster region'
 
 # take environment variables from .env
 load_dotenv(find_dotenv(), override=True)
 
-
 U = TypeVar('U')
-
-
 def nn(inst: Optional[U]) -> U:
     """Not-none helper to stop mypy errors"""
     assert inst is not None
     return inst
 
-
 def tag_visible(element: Tag) -> bool:
     """ Strip out undesirables """
     parent: Tag = nn(element.parent)
     if parent.name in ['style', 'script', 'head', 'title', 'meta', '[document]']:
         return False
     if isinstance(element, Comment):
         return False
     return True
 
-
 def _text_from_html(body: str) -> str:
     """ Obv pull text from doc with tag_visible filters """
     soup = BeautifulSoup(body, 'html.parser')
     texts = soup.findAll(string=True)
     visible_texts = filter(tag_visible, texts)
     return " ".join(t.strip() for t in visible_texts)
 
-
-"""
-def _get_openai_embedding(apikey: str, data: str) -> openai.Embedding:
-    openai.api_key = apikey
-    try:
-        res = openai.Embedding.create(input=data, engine=OPENAI_EMBED_MODEL)
-    except:
-        done = False
-        while not done:
-            sleep(5)
-            try:
-                res = openai.Embedding.create(
-                    input=data, engine=OPENAI_EMBED_MODEL)
-                done = True
-            except Exception as e:
-                click.echo(e)
-    return res
-"""
-
-
 @retry(tries=3, delay=5)
-def _get_openai_embedding(apikey: str, data: list[str]) -> openai.Embedding:
+def _get_openai_embedding(apikey: str, data: List[str]) -> openai.Embedding:
     openai.api_key = apikey
     return openai.Embedding.create(input=data, engine=OPENAI_EMBED_MODEL)
 
-
 @click.group()
 def cli() -> None:
-    """
-    A command line interface for working with Pinecone.
-    """
+    """ A command line interface for working with Pinecone. """
     pass
 
-
 def _pinecone_init(apikey: str, environment: str, indexname: str = '') -> pinecone.GRPCIndex:
     index = None
     apikey = os.environ.get(
         'PINECONE_API_KEY', apikey) if apikey is None else apikey
     environment = os.environ.get(
         'PINECONE_ENVIRONMENT', environment) if environment is None else environment
     if apikey is None:
```

## Comparing `pinecone_cli-0.5.3.dist-info/LICENSE` & `pinecone_cli-0.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pinecone_cli-0.5.3.dist-info/METADATA` & `pinecone_cli-0.5.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-cli
-Version: 0.5.3
+Version: 0.5.4
 Summary: pinecone-cli is a command-line client for interacting with the pinecone vector embedding database.
 Home-page: https://github.com/tullytim/pinecone-cli
 Author: Tim Tully
 Author-email: tim@menlovc.com
 License: MIT
 Keywords: pinecone vector vectors embeddings database transformers models
 Platform: any
```

