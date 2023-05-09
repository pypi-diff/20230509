# Comparing `tmp/nwebclient-1.0.88.tar.gz` & `tmp/nwebclient-1.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.88.tar", last modified: Sun May  7 14:06:58 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.89.tar", last modified: Tue May  9 13:51:06 2023, max compression
```

## Comparing `nwebclient-1.0.88.tar` & `nwebclient-1.0.89.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 14:06:58.583065 nwebclient-1.0.88/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.88/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 14:06:58.583065 nwebclient-1.0.88/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.88/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 14:06:58.583065 nwebclient-1.0.88/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6475 2023-05-07 14:06:28.000000 nwebclient-1.0.88/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.88/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.88/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.88/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.88/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.88/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 14:06:58.583065 nwebclient-1.0.88/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 14:06:58.000000 nwebclient-1.0.88/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 14:06:58.000000 nwebclient-1.0.88/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 14:06:58.000000 nwebclient-1.0.88/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 14:06:58.000000 nwebclient-1.0.88/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 14:06:58.000000 nwebclient-1.0.88/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 14:06:58.000000 nwebclient-1.0.88/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 14:06:58.583065 nwebclient-1.0.88/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 14:06:51.000000 nwebclient-1.0.88/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 13:51:06.125096 nwebclient-1.0.89/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.89/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-09 13:51:06.125096 nwebclient-1.0.89/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.89/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 13:51:06.125096 nwebclient-1.0.89/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6469 2023-05-07 16:18:58.000000 nwebclient-1.0.89/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.89/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.89/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13240 2023-05-09 13:20:07.000000 nwebclient-1.0.89/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.89/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.89/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-09 13:51:06.125096 nwebclient-1.0.89/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-09 13:51:06.000000 nwebclient-1.0.89/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-09 13:51:05.000000 nwebclient-1.0.89/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-09 13:51:06.125096 nwebclient-1.0.89/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-09 13:50:59.000000 nwebclient-1.0.89/setup.py
```

### Comparing `nwebclient-1.0.88/LICENSE` & `nwebclient-1.0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.88/PKG-INFO` & `nwebclient-1.0.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.88
+Version: 1.0.89
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.88/README.md` & `nwebclient-1.0.89/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.88/nwebclient/__init__.py` & `nwebclient-1.0.89/nwebclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,25 +96,28 @@
             self.__pass = self.__cfg['password']
         else:
             self.__url = url
             self.__user = username
             self.__pass = password
     def __call__(self, q):
         return "NWebClient TODO"
-    #def __getitem__(self, key):
-    #    return self.__getattribute__(key)
+    def __getitem__(self, key):
+        if key in self.__cfg:
+            return self.__cfg[key]
+        else:
+            return "Non Existing"
     def file_get_contents(self, filename):
         with open(filename) as f:
             return f.read()
     def _appendGet(self, url, name, value):
         v = name + '=' + urllib.quote(value)
         if '?' in url:
-          return url + '&' + v
+            return url + '&' + v
         else:
-          return url + '?' + v
+            return url + '?' + v
     def reqToFile(self, path, name):
         url = self.__url + path
         url = self._appendGet(url, 'username', self.__user)
         url = self._appendGet(url, 'password', self.__pass)
         r = requests.get(url, stream=True, verify=self.ssl_verify) 
         if r.status_code == 200:
             with open(name, 'wb') as f:
@@ -148,15 +151,14 @@
         return list(map(lambda x: NWebDoc(self, x), items))
     def group(self, id): 
         data = json.loads(self.req("api/group/"+id, {format:"json"}))
         return NWebGroup(self, data)
     def getOrCreateGroup(self, guid, title):
         return "TODO"
     def createDoc(self, name, content, group_id, kind='markup'):
-        # https://bsnx.net/4.0/w/group/DBCD3638B55EA1ECE7EE1BDEC7E04131/create
         res = self.req("w/group/"+str(group_id)+"/create", {
             "title": name,
             "content": content,
             "kind": kind
         })
         return res
     def createFileDoc(self, name, group_id, data):
```

### Comparing `nwebclient-1.0.88/nwebclient/__main__.py` & `nwebclient-1.0.89/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.88/nwebclient/crypt.py` & `nwebclient-1.0.89/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.88/nwebclient/sd.py` & `nwebclient-1.0.89/nwebclient/sd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from nwebclient import sdb
 from nwebclient import ticker
 import json
 import os
+import os.path
 import requests
 import time
 
 # Stable Diffusion Imports in ImageGen::__init__
 
 def gen(pipe, prompt='photo', negative_prompt = None, prefix='sd',  guidance_scale = 7.5, num_inference_steps=30, height=800, width=640, num_images=1, dbfile='data.db'):
     # https://huggingface.co/docs/diffusers/v0.14.0/en/api/pipelines/stable_diffusion/text2img#diffusers.StableDiffusionPipeline.__call__
@@ -229,7 +230,72 @@
     ext = ".sdjob"
     def __init__(self, generator=None):
         if generator is None:
             generator = ImageGen()
         self.generator = generator
     def processFile(self, filename):
         self.generator.executeJsonFile(filename)
+    def configure(self, arg):
+        self.generator.generator = arg
+class JobFetch(ticker.Ticker):
+    """ 
+      JobFetch(NWebClient(...), 42)  
+      
+      npy-ticker nwebclient.sd.JobFetch:42
+    """
+    key = None
+    def __init__(self, nwebclient=None, group=None):
+        super().__init__("jobfetch",60*60*23) 
+        from cryptography.fernet import Fernet
+        from nwebclient import NWebClient
+        self.nweb = nwebclient
+        self.group = group
+    def configure(self, arg):
+        self.nweb = NWebClient()
+        self.group = arg
+    def execute(self):
+        docs = self.nweb.docs('group_id='+str(self.group))
+        for doc in docs:
+            self.download(doc)
+    def decrypt(self, file):
+        with open(file, 'rb') as f:
+            original = f.read()
+        encrypted = fernet.decrypt(original)
+        with open(file, 'wb') as encrypted_file:
+            encrypted_file.write(encrypted)
+    def download(self, doc):
+        file = str(doc.id()) + '.sdjob'
+        doc.save(file)
+        if not self.key is None:
+            self.decrypt(file)
+        self.nweb.deleteDoc(doc.id())
+class SdbUpload(ticker.Ticker):
+    key = None
+    def __init__(self, nwebclient=None, group=None, minSize = None):
+        super().__init__("jobfetch",60*60*23) 
+        from nwebclient import crypt
+        from cryptography.fernet import Fernet
+        self.nweb = nwebclient
+        self.group = group
+        self.minSize = minSize
+    def execute(self):
+        filename = 'data.db'
+        if os.path.isfile(filename) and self.isBigEnough(filename):
+            self.upload(filename)
+    def isBigEnough(self, file):
+        if self.minSize == None:
+            return True
+        else:
+            file_stats = os.stat(file)
+            return file_stats.st_size > self.minSize
+    def upload(self, file, remove = True):
+        if not self.key is None:
+            fernet = Fernet(key)
+            with open(file, 'rb') as f:
+                original = f.read()
+            encrypted = fernet.encrypt(original)
+            with open(file, 'wb') as encrypted_file:
+                encrypted_file.write(encrypted)
+        self.nweb.createFileDoc('result', self.group, open(file, 'rb'))
+        if remove:
+            os.remove(file)
+
```

### Comparing `nwebclient-1.0.88/nwebclient/sdb.py` & `nwebclient-1.0.89/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.88/nwebclient/ticker.py` & `nwebclient-1.0.89/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.88/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.89/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.88
+Version: 1.0.89
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.88/setup.py` & `nwebclient-1.0.89/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.88",
+    version="1.0.89",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

