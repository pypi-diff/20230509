# Comparing `tmp/HDRezka-3.0.0.tar.gz` & `tmp/HDRezka-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HDRezka-3.0.0.tar", last modified: Mon May  8 10:51:33 2023, max compression
+gzip compressed data, was "HDRezka-3.0.1.tar", last modified: Tue May  9 07:12:05 2023, max compression
```

## Comparing `HDRezka-3.0.0.tar` & `HDRezka-3.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.575274 HDRezka-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.498828 HDRezka-3.0.0/HDRezka.egg-info/
--rw-rw-rw-   0        0        0     4844 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 10:51:33.000000 HDRezka-3.0.0/HDRezka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     4844 2023-05-08 10:51:33.574276 HDRezka-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      980 2023-05-08 10:44:42.000000 HDRezka-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.504842 HDRezka-3.0.0/hdrezka/
--rw-rw-rw-   0        0        0      910 2023-05-08 10:49:23.000000 HDRezka-3.0.0/hdrezka/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/_antiobfuscation.py
--rw-rw-rw-   0        0        0      309 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/_bs4.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.508828 HDRezka-3.0.0/hdrezka/api/
--rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/api/__init__.py
--rw-rw-rw-   0        0        0     1472 2023-05-08 09:52:32.000000 HDRezka-3.0.0/hdrezka/api/ajax.py
--rw-rw-rw-   0        0        0      370 2023-05-08 06:08:44.000000 HDRezka-3.0.0/hdrezka/api/http.py
--rw-rw-rw-   0        0        0      832 2023-05-08 10:49:50.000000 HDRezka-3.0.0/hdrezka/api/search.py
--rw-rw-rw-   0        0        0      383 2023-05-08 10:49:13.000000 HDRezka-3.0.0/hdrezka/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.522065 HDRezka-3.0.0/hdrezka/post/
--rw-rw-rw-   0        0        0       42 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/__init__.py
--rw-rw-rw-   0        0        0      113 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/_dataclass.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.525066 HDRezka-3.0.0/hdrezka/post/info/
--rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/info/__init__.py
--rw-rw-rw-   0        0        0      622 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/info/fields.py
--rw-rw-rw-   0        0        0     5459 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/info/info.py
--rw-rw-rw-   0        0        0     2905 2023-05-08 10:49:40.000000 HDRezka-3.0.0/hdrezka/post/page.py
--rw-rw-rw-   0        0        0     2609 2023-05-08 09:52:32.000000 HDRezka-3.0.0/hdrezka/post/post.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.536023 HDRezka-3.0.0/hdrezka/post/urls/
--rw-rw-rw-   0        0        0       64 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/__init__.py
--rw-rw-rw-   0        0        0      416 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/_regexes.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.570276 HDRezka-3.0.0/hdrezka/post/urls/kind/
--rw-rw-rw-   0        0        0       71 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/__init__.py
--rw-rw-rw-   0        0        0      768 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/quality.py
--rw-rw-rw-   0        0        0     1490 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/subtitle.py
--rw-rw-rw-   0        0        0     2037 2023-05-08 10:43:14.000000 HDRezka-3.0.0/hdrezka/post/urls/kind/video.py
--rw-rw-rw-   0        0        0      553 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/short.py
--rw-rw-rw-   0        0        0      469 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/post/urls/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:51:33.573325 HDRezka-3.0.0/hdrezka/stream/
--rw-rw-rw-   0        0        0       23 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/stream/__init__.py
--rw-rw-rw-   0        0        0     3458 2023-05-08 10:06:08.000000 HDRezka-3.0.0/hdrezka/stream/player.py
--rw-rw-rw-   0        0        0      398 2023-05-08 06:05:54.000000 HDRezka-3.0.0/hdrezka/translators.py
--rw-rw-rw-   0        0        0       42 2023-05-08 10:51:33.575274 HDRezka-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2007 2023-05-08 10:08:16.000000 HDRezka-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.726275 HDRezka-3.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.663775 HDRezka-3.0.1/HDRezka.egg-info/
+-rw-rw-rw-   0        0        0     4943 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4943 2023-05-09 07:12:05.726275 HDRezka-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      986 2023-05-09 07:05:54.000000 HDRezka-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.695084 HDRezka-3.0.1/hdrezka/
+-rw-rw-rw-   0        0        0     1079 2023-05-09 07:06:59.000000 HDRezka-3.0.1/hdrezka/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/_antiobfuscation.py
+-rw-rw-rw-   0        0        0      309 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/_bs4.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.695084 HDRezka-3.0.1/hdrezka/api/
+-rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/api/__init__.py
+-rw-rw-rw-   0        0        0     1472 2023-05-08 09:52:32.000000 HDRezka-3.0.1/hdrezka/api/ajax.py
+-rw-rw-rw-   0        0        0      370 2023-05-08 06:08:44.000000 HDRezka-3.0.1/hdrezka/api/http.py
+-rw-rw-rw-   0        0        0      832 2023-05-08 10:49:50.000000 HDRezka-3.0.1/hdrezka/api/search.py
+-rw-rw-rw-   0        0        0      383 2023-05-08 10:49:13.000000 HDRezka-3.0.1/hdrezka/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/
+-rw-rw-rw-   0        0        0       42 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/_dataclass.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/info/
+-rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/info/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/info/fields.py
+-rw-rw-rw-   0        0        0     5459 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/info/info.py
+-rw-rw-rw-   0        0        0     2905 2023-05-08 10:49:40.000000 HDRezka-3.0.1/hdrezka/post/page.py
+-rw-rw-rw-   0        0        0     2612 2023-05-09 07:04:56.000000 HDRezka-3.0.1/hdrezka/post/post.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/urls/
+-rw-rw-rw-   0        0        0       64 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/_regexes.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/urls/kind/
+-rw-rw-rw-   0        0        0       71 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/__init__.py
+-rw-rw-rw-   0        0        0      768 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/quality.py
+-rw-rw-rw-   0        0        0     1490 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/subtitle.py
+-rw-rw-rw-   0        0        0     2037 2023-05-08 10:43:14.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/video.py
+-rw-rw-rw-   0        0        0      553 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/short.py
+-rw-rw-rw-   0        0        0      469 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.726275 HDRezka-3.0.1/hdrezka/stream/
+-rw-rw-rw-   0        0        0       23 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/stream/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-05-09 07:05:54.000000 HDRezka-3.0.1/hdrezka/stream/player.py
+-rw-rw-rw-   0        0        0      398 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/translators.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 07:12:05.726275 HDRezka-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2007 2023-05-09 07:11:46.000000 HDRezka-3.0.1/setup.py
```

### Comparing `HDRezka-3.0.0/HDRezka.egg-info/PKG-INFO` & `HDRezka-3.0.1/HDRezka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 3.0.0
+Version: 3.0.1
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -42,15 +42,15 @@
 # Example
 
 ```python
 import asyncio
 from hdrezka import Search
 
 async def main():
-    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use Player(646)
+    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use await Player(646)
     print(player.post.info, end='\n\n')
 
     translator_id = None  # default
     for name, id_ in player.post.translators.name_id.items():
         if 'субтитры' in name.casefold(): translator_id = id_; break
 
     stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
@@ -66,14 +66,18 @@
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 3.0.1
+
+- Now `__await__` method (need `await ...` expression) instead `ainit` method
+
 ## 3.0.0
 
 - **Now a fully asynchronous package.**
 
 - ### post.page.Page
     - Implements `__aiter__` and `__anext__` methods that list all the pages found.
     - Instead of `get_pages`, now only the `get_page` method
```

### Comparing `HDRezka-3.0.0/HDRezka.egg-info/SOURCES.txt` & `HDRezka-3.0.1/HDRezka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/LICENSE` & `HDRezka-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/PKG-INFO` & `HDRezka-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 3.0.0
+Version: 3.0.1
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -42,15 +42,15 @@
 # Example
 
 ```python
 import asyncio
 from hdrezka import Search
 
 async def main():
-    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use Player(646)
+    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use await Player(646)
     print(player.post.info, end='\n\n')
 
     translator_id = None  # default
     for name, id_ in player.post.translators.name_id.items():
         if 'субтитры' in name.casefold(): translator_id = id_; break
 
     stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
@@ -66,14 +66,18 @@
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 3.0.1
+
+- Now `__await__` method (need `await ...` expression) instead `ainit` method
+
 ## 3.0.0
 
 - **Now a fully asynchronous package.**
 
 - ### post.page.Page
     - Implements `__aiter__` and `__anext__` methods that list all the pages found.
     - Instead of `get_pages`, now only the `get_page` method
```

### Comparing `HDRezka-3.0.0/README.md` & `HDRezka-3.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Example
 
 ```python
 import asyncio
 from hdrezka import Search
 
 async def main():
-    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use Player(646)
+    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use await Player(646)
     print(player.post.info, end='\n\n')
 
     translator_id = None  # default
     for name, id_ in player.post.translators.name_id.items():
         if 'субтитры' in name.casefold(): translator_id = id_; break
 
     stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
```

### Comparing `HDRezka-3.0.0/hdrezka/_antiobfuscation.py` & `HDRezka-3.0.1/hdrezka/_antiobfuscation.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/api/ajax.py` & `HDRezka-3.0.1/hdrezka/api/ajax.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/api/search.py` & `HDRezka-3.0.1/hdrezka/api/search.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/info/fields.py` & `HDRezka-3.0.1/hdrezka/post/info/fields.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/info/info.py` & `HDRezka-3.0.1/hdrezka/post/info/info.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/page.py` & `HDRezka-3.0.1/hdrezka/post/page.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/post.py` & `HDRezka-3.0.1/hdrezka/post/post.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 class Post:
     """Stores information about the post"""
     __slots__ = ('url', 'translator_id', 'id', 'name', 'type', 'info', 'translators', 'other_parts_urls',
                  '_soup_inst')
 
     def __init__(self, url: str):
-        """Also you should call the `ainit` method"""
+        """Need await"""
         url = long_url(url)
         self.url = url
 
-    async def ainit(self):
-        _response = await get_response('GET', self.url)
+    def __await__(self):
+        _response = yield from get_response('GET', self.url).__await__()
         if _response.status_code in {301, 302}:  # redirect
-            _response = await get_response('GET', _response.url.join(_response.headers['location']))
+            _response = yield from get_response('GET', _response.url.join(_response.headers['location'])).__await__()
         _response = _response.text
         self._soup_inst = BeautifulSoup(_response)
         self.type = self._get_type()
 
         self.translator_id = int(i) if (i := _response.split(
             'sof.tv.' + {'tv_series': 'initCDNSeriesEvents', 'movie': 'initCDNMoviesEvents'}[self.type],
             1)[-1].split(',')[1].strip()).isnumeric() else None
```

### Comparing `HDRezka-3.0.0/hdrezka/post/urls/kind/quality.py` & `HDRezka-3.0.1/hdrezka/post/urls/kind/quality.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/urls/kind/subtitle.py` & `HDRezka-3.0.1/hdrezka/post/urls/kind/subtitle.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/urls/kind/video.py` & `HDRezka-3.0.1/hdrezka/post/urls/kind/video.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/post/urls/short.py` & `HDRezka-3.0.1/hdrezka/post/urls/short.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.0/hdrezka/stream/player.py` & `HDRezka-3.0.1/hdrezka/stream/player.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 __CACHE = _CacheStorage()
 
 
 class PlayerBase:
     __slots__ = ('post',)
 
     def __init__(self, url_or_cast: Any):
-        """Also you should call the `ainit` method"""
+        """Need await"""
         if isinstance(url_or_cast, PlayerBase):
             self.post = url_or_cast.post
             return
         elif not isinstance(url_or_cast, str):
             url_or_cast = str(url_or_cast)
         self.post = Post(url_or_cast)
 
-    async def ainit(self):
-        await self.post.ainit()
+    def __await__(self):
+        yield from self.post.__await__()
 
     def _translator(self, translator_id: SupportsInt = None) -> int:
         if translator_id is None:
             return self.post.translator_id
         translator_id = int(translator_id)
         return self.post.translators.ids[abs(translator_id)] if translator_id <= 0 else translator_id
 
@@ -85,15 +85,15 @@
     """
     Returns either Player Series if series, or PlayerMovie if movie, otherwise raises UnknownContentType
     """
     cast = PlayerBase(url_or_path)
     cached = __CACHE.get(cast.post.url)
     if cached is not None:
         return cached
-    await cast.ainit()
+    await cast
     type = cast.post.type
     match type:
         case 'tv_series':
             value = PlayerSeries(cast)
         case 'movie':
             value = PlayerMovie(cast)
         case _:
```

### Comparing `HDRezka-3.0.0/setup.py` & `HDRezka-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('README.md', encoding='UTF-8') as f:
     long_description = f.read().strip()
 with open('CHANGELOG.md', encoding='UTF-8') as f:
     long_description += f'\n\n---\n\n{f.read().strip()}\n'
 
 setuptools.setup(
     name='HDRezka',
-    version='3.0.0',
+    version='3.0.1',
 
     author='Nikita (NIKDISSV)',
     author_email='nikdissv@proton.me',
 
     description='HDRezka (rezka.ag) Python API',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

