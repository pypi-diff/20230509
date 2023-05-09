# Comparing `tmp/photoprism_client-0.1.3.tar.gz` & `tmp/photoprism_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/photoprism_client-0.1.3.tar", last modified: Tue Nov 22 21:37:55 2022, max compression
+gzip compressed data, was "photoprism_client-0.2.1.tar", last modified: Tue May  9 06:40:55 2023, max compression
```

## Comparing `photoprism_client-0.1.3.tar` & `photoprism_client-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/
-drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5741 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/PKG-INFO
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)        9 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/requires.txt
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)       11 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/top_level.txt
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      297 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/SOURCES.txt
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)        1 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/dependency_links.txt
-drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism/
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      689 2022-11-06 12:24:57.000000 photoprism_client-0.1.3/photoprism/Session.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)        0 2022-03-25 19:21:56.000000 photoprism_client-0.1.3/photoprism/__init__.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5851 2022-11-22 21:16:32.000000 photoprism_client-0.1.3/photoprism/Photo.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5741 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/PKG-INFO
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      544 2022-11-22 21:35:02.000000 photoprism_client-0.1.3/setup.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     4829 2022-11-22 21:29:35.000000 photoprism_client-0.1.3/README.md
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      103 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/setup.cfg
+drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2023-05-09 06:40:55.861996 photoprism_client-0.2.1/
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     1066 2023-04-14 10:22:46.000000 photoprism_client-0.2.1/LICENSE
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     7745 2023-05-09 06:40:55.862053 photoprism_client-0.2.1/PKG-INFO
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     6969 2023-05-07 14:55:47.000000 photoprism_client-0.2.1/README.md
+drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2023-05-09 06:40:55.861080 photoprism_client-0.2.1/photoprism/
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     6272 2023-05-06 11:24:59.000000 photoprism_client-0.2.1/photoprism/Photo.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     3508 2023-05-06 10:56:04.000000 photoprism_client-0.2.1/photoprism/Session.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)        0 2023-04-14 10:22:46.000000 photoprism_client-0.2.1/photoprism/__init__.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      548 2023-05-06 11:47:28.000000 photoprism_client-0.2.1/photoprism/mimetypes.py
+drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2023-05-09 06:40:55.861897 photoprism_client-0.2.1/photoprism_client.egg-info/
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     7745 2023-05-09 06:40:55.000000 photoprism_client-0.2.1/photoprism_client.egg-info/PKG-INFO
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      335 2023-05-09 06:40:55.000000 photoprism_client-0.2.1/photoprism_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)        1 2023-05-09 06:40:55.000000 photoprism_client-0.2.1/photoprism_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)        9 2023-05-09 06:40:55.000000 photoprism_client-0.2.1/photoprism_client.egg-info/requires.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)       11 2023-05-09 06:40:55.000000 photoprism_client-0.2.1/photoprism_client.egg-info/top_level.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      877 2023-05-09 06:38:36.000000 photoprism_client-0.2.1/pyproject.toml
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      103 2023-05-09 06:40:55.862261 photoprism_client-0.2.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `photoprism_client-0.1.3/photoprism_client.egg-info/PKG-INFO` & `photoprism_client-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,100 @@
-Metadata-Version: 2.1
-Name: photoprism-client
-Version: 0.1.3
-Summary: A Python client to interact with photoprism. 
-Home-page: https://github.com/mvlnetdev/photoprism_client
-Author: mvlnetdev
-Author-email: maartenvanleeuwen1996@gmail.com
-License: MIT license
-Description: # Python client for PhotoPrism 
-        A Python client to interact with photoprism.
-        
-        ## IMPORTANT
-        This Python client is build on the undocumented API of PhotoPrism. There may be bugs in there. Please let me know if you find some. 
-        
-        Currently tested on the [version of the 17th of June 2022](https://github.com/photoprism/photoprism/releases/tag/220617-0402b8d3). It will probably work with later versions. Just try it and let me know, I will update the readme accordingly.  
-        
-        ## Requirements
-        - requests (latest)
-        
-        ## Setup
-        To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
-        ``` python
-        from photoprism.Session import Session
-        pp_session = Session("admin", "changethis", "demo.photoprism.app")
-        pp_session.create()
-        ```
-        
-        ## Searching
-        To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
-        
-        ```python
-        from photoprism.Photo import Photo
-        
-        p = Photo(pp_session)
-        p.search(query="original:*")
-        ```
-        
-        ## Other functions
-        This is a list of all other functions within the client. If you want other functions either request them or send a pull request.
-        | function | description | variables | returns |
-        | ---- | ----- | ------ | ----- |
-        | Photo.add_photos_to_album() | Add photos to an album, you will need to provide a list of UIDs of the photos you want to add. Returns True if successfull | photos: list, album_uid: string | True if successfull  |
-        | Photo.add_to_album_from_query() | Provide a search query and add all photos that are returned into an album. Provide the albumname, not the UID of the album. | query: string, albumname: string | True if successfull |
-        | Photo.check_if_album_exists() | Small function to check if an album exists | name: string, create_if_not: bool (default is False) | True if it exists, False if not (will continue to be False if the album is created) |
-        | Photo.create_album() | Create an album, returns a boolean if it worked | title: string | True if successfull |
-        | Photo.get_album() | Get all information of an album based upon the UID of the album | uid: string | Dict object with the information of the album, False if it does not exist |
-        | Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
-        | Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100) | list of uids |
-        | Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
-        | Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
-        | Photo.search() | Create the session | query: string, count: int (default=100) | Dict object of the results of the search |
-        | Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
-        | Photo.stop_import() | Stop an import job | None | True if successfully stopped |
-        | Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
-        | Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
-        
-        ## License 
-        MIT License
-        
-        Copyright (c) 2022 maartenvl
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Keywords: photoprism
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Python client for PhotoPrism 
+A Python client to interact with photoprism.
+
+Changelog can be found in [here](./changelog.md).
+
+## IMPORTANT
+This Python client is build on the undocumented API of PhotoPrism. There may be bugs in there. Please let me know if you find some. 
+
+Currently tested on the [version of the 17th of June 2022](https://github.com/photoprism/photoprism/releases/tag/220617-0402b8d3). It will probably work with later versions. Just try it and let me know, I will update the readme accordingly.  
+
+## Requirements
+- requests (latest)
+
+## Setup
+To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
+``` python
+from photoprism.Session import Session
+pp_session = Session("admin", "changethis", "demo.photoprism.app")
+pp_session.create()
+```
+
+### HTTPS
+It is possible to connect to Photoprism using HTTPS. Two variables exist for this:
+- use_https: Boolean
+- verify_cert: Boolean
+
+By default, a connection will be made using HTTP. A session can be set up using HTTPS by setting the use_https variable to _True_. By default the certificate will be verified. This check can be disabled by setting the verify_cert variable to _False_. Only change this if you understand what this means. It is better to leave this variable unchanged. 
+
+An example is:
+```python
+from photoprism.Session import Session
+pp_session = Session("admin", "changethis", "demo.photoprism.app", use_https=True, verify_cert=False)
+pp_session.create()
+```
+
+### User agent
+The user agent is _Photoprism Python Client_ by default. You can change this using the variable _user_agent_. 
+For example:
+```python
+from photoprism.Session import Session
+pp_session = Session("admin", "changethis", "demo.photoprism.app", user_agent="Hello World! This is an example.")
+pp_session.create()
+```
+
+## Searching
+To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
+
+```python
+from photoprism.Photo import Photo
+
+p = Photo(pp_session)
+p.search(query="original:*")
+```
+
+## Other functions
+This is a list of all other functions within the client. If you want other functions either request them or send a pull request.
+| function | description | variables | returns |
+| ---- | ----- | ------ | ----- |
+| Photo.add_photos_to_album() | Add photos to an album, you will need to provide a list of UIDs of the photos you want to add. Returns True if successfull | photos: list, album_uid: string | True if successfull  |
+| Photo.add_to_album_from_query() | Provide a search query and add all photos that are returned into an album. Provide the albumname, not the UID of the album. | query: string, albumname: string, count: int (default=1000000), offset: int (default=0), order: string (default="newest") | True if successfull |
+| Photo.check_if_album_exists() | Small function to check if an album exists | name: string, create_if_not: bool (default is False) | True if it exists, False if not (will continue to be False if the album is created) |
+| Photo.create_album() | Create an album, returns a boolean if it worked | title: string | Dict object with the album information |
+| Photo.download_album() | Download an entire album as ZIP. The file will get the same name as the title of the album, by setting the filename variable the name can be changed. | uid: string, path: string (default="."), filename: string (default=None) | True if successfull |
+| Photo.download_file() | Download a single file. The file will get the same name as in photoprism, by setting the filename variable the name can be changed. | hash: string, path: string (default="."), filename: string (default=None) | True if succesfull |
+| Photo.download_files_from_query() | Download files from a query | query: string, count: int (default=100), offset: int (default=0), order: string (default="newest") | True if succesfull | 
+| Photo.get_album() | Get all information of an album based upon the UID of the album | uid: string | Dict object with the information of the album, False if it does not exist |
+| Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
+| Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100), offset: int (default=0), order: string (default="newest") | list of uids |
+| Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
+| Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
+| Photo.search() | Create the session | query: string, count: int (default=100), offset: int (default=0), order: string (default="newest") | Dict object of the results of the search |
+| Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
+| Photo.stop_import() | Stop an import job | None | True if successfully stopped |
+| Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
+| Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
+| Photo.remove_album_uid() | Remove album based on album uid | uid: string | Dict of the removed album, False if action failed. |
+
+
+## License 
+MIT License
+
+Copyright (c) 2022 maartenvl
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
+SOFTWARE.
```

### Comparing `photoprism_client-0.1.3/photoprism/Photo.py` & `photoprism_client-0.2.1/photoprism/Photo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 """Interaction with the API of PhotoPrism"""
+import uuid
 
 from photoprism import Session
 import requests, json
 
 class Photo():
     def __init__(self, session):
         """Initialize based upon a session"""
         if type(session) != Session.Session:
             raise TypeError(f"session variable is not of type photoprism.Session.Session, but {type(session)}")
 
         self.session = session
-        self.header = {
-            "X-Session-ID": self.session.session_id}
 
-
-    def search(self, query, count=100):
+    def search(self, query, count=100, offset=0, order="newest"):
         """Basic search function. Returns a Dict object based upon the returned JSON"""
+        _, data = self.session.req(f"/photos?count={count}&q={query}&offset={offset}&order={order}", "GET")
+        return data
 
-        url = f"{self.session.url}/photos?count={count}&q={query}"
-        r = requests.get(url, headers=self.header)
-        return json.loads(r.text)
-
-    def get_uid_list_of_search(self, query, count=100):
+    def get_uid_list_of_search(self, query, count=100, offset=0, order="newest"):
         """Return a list of UIDs based upon the search"""
 
-        photos = self.search(query, count)
+        photos = self.search(query, count, offset=offset, order=order)
         photolist = []
         for ps in photos:
             photolist.append(ps["UID"])
 
         return photolist
 
-    def list_albums(self):
+    def list_albums(self, count=100000):
         """Provide a list of all albums within the photoprism instance, with a max of 100000"""
-
-        url = f"{self.session.url}/albums?count=100000"
-        r = requests.get(url, headers=self.header)
-        return json.loads(r.text)
+        _, data = self.session.req(f"/albums?count={count}", "GET")
+        return data
 
     def check_if_album_exists(self, name, create_if_not=False):
         """Small function to check if an album exists"""
 
         data = self.list_albums()
         for d in data:
             if name == d["Title"]:
@@ -60,115 +54,123 @@
             if name == d["Title"]:
                 return d["UID"]
         
         return False
 
     def create_album(self, title):
         """Create an album, returns a boolean if it worked"""
-
-        url = f"{self.session.url}/albums"
         data = {"Title":title,"Favorite":False}
-        r = requests.post(url=url, data=json.dumps(data), headers=self.header)
-        
-        if r.status_code == 200:
-            return True
+        status_code, output = self.session.req("/albums", "POST", data=data)
+
+        if status_code == 200:
+            return output
         
         return False
 
     def add_photos_to_album(self, photos, album_uid):
         """Add photos to an album, you will need to provide a list of UIDs of the photos you want to add. Returns True if successfull"""
-
-        url = f"{self.session.url}/albums/{album_uid}/photos"
         data = {
             "photos":photos
         }
-        r = requests.post(url, data=json.dumps(data), headers=self.header)
-        
-        if r.status_code == 200:
+        status_code, _ = self.session.req(f"/albums/{album_uid}/photos", "POST", data=data)
+        if status_code == 200:
             return True
 
         return False
 
-    def add_to_album_from_query(self, query, albumname):
+    def add_to_album_from_query(self, query, albumname, count=1000000, offset=0, order="newest"):
         """Provide a search query and add all photos that are returned into an album. Provide the albumname, not the UID of the album."""
 
         self.check_if_album_exists(albumname, create_if_not=True)
         album_uid = self.get_album_uid_by_name(albumname)
-        photolist = self.get_uid_list_of_search(query, count=1000000)
+        photolist = self.get_uid_list_of_search(query, count=count, offset=offset, order=order)
         result = self.add_photos_to_album(photolist, album_uid)
         return result
 
     def get_album(self, uid):
         """Get all information of an album based upon the UID of the album"""
+        status_code, data = self.session.req(f"/albums/{uid}", "GET")
+        if status_code == 200:
+            return data
 
-        url = f"{self.session.url}/albums/{uid}"
-        r = requests.get(url, headers=self.header)
-        
-        if r.status_code == 200:
-            return json.loads(r.text)
-        
         return False
 
-    def remove_photos_from_album(self,albumname, photos=False, count=1000000):
+    def remove_photos_from_album(self, albumname, photos=False, count=1000000):
         """Remove photos from an album, Returns True if successfull"""
         album_uid = self.get_album_uid_by_name(albumname)
         if photos == False:
             query = f"album:\"{albumname}\""
             photos = self.get_uid_list_of_search(query,count=count)
 
-        url = f"{self.session.url}/albums/{album_uid}/photos"
         data = {
             "photos":photos
         }
-        r = requests.delete(url, data=json.dumps(data), headers=self.header)
-        result = False
-        if r.status_code == 200:
-            result = True
-        return result
+        status_code, _ = self.session.req(f"/albums/{album_uid}/photos", "DELETE", data=data)
+        if status_code == 200:
+            return True
+
+        return False
 
     def remove_album(self, albumname):
         """Remove album based on album name"""
         album_uid = self.get_album_uid_by_name(albumname)
-        url = f"{self.session.url}/albums/{album_uid}"
-        r = requests.delete(url, headers=self.header)
-        result = False
-        if r.status_code == 200:
-            result = json.loads(r.text)
-        return result
+        return self.remove_album_uid(album_uid)
+
+    def remove_album_uid(self, uid):
+        """Remove album based on album uid"""
+        status_code, data = self.session.req(f"/albums/{uid}", "DELETE")
+        if status_code == 200:
+            return data
+
+        return False
 
     def start_import(self, path="upload", move=False):
         """Start an import job, default path is upload. It returns True when the import started, not when finished"""
-
-        url = f"{self.session.url}/import"
         data = {
             "path": path,
             "move": move
         }
-        r = requests.post(url, data=json.dumps(data), headers=self.header)
-        
-        if r.status_code == 200:
+        status_code, _ = self.session.req(f"/import", "POST", data=data)
+        if status_code == 200:
             return True
         
         return False
 
     def stop_import(self):
         """Stop an import job"""
-        url = f"{self.session.url}/import"
-        r = requests.delete(url, headers=self.header)
-
-        if r.status_code == 200:
+        status_code, _ = self.session.req("/import", "DELETE")
+        if status_code == 200:
             return True
         
         return False
 
-    def raw_call(self, endpoint, type="GET", data=None):
-        """Function to perform a request to the photoprism server"""
+    def download_file(self, hash, path=".", filename=None):
+        """Download a single file"""
+        status_code, data = self.session.req(f"/dl/{hash}", "GET", path=path, filename=filename)
 
-        url = f"{self.session.url}/{endpoint}"
-        if type == "GET":
-            return requests.get(url, headers=self.header)
-        elif type == "POST":
-            return requests.post(url, data=json.dumps(data) if data else None, headers=self.header)
-        elif type == "DELETE":
-            return requests.delete(url, headers=self.header)
-        
+        if status_code == 200:
+            return True
+        return False
+
+    def download_album(self, uid, path=".", filename=None):
+        """Download an entire album as ZIP"""
+        status_code, data = self.session.req(f"/albums/{uid}/dl", "GET", stream=True, path=path, filename=filename)
+
+        if status_code == 200:
+            return True
         return False
+
+    def download_files_from_query(self, query, count=100, offset=0, order="newest"):
+        """Download files from a query"""
+        # In order to make it easy, files are first put into a temporary album
+        # After which they are downloaded
+        # After the download is complete, the folder is removed.
+
+        temp_album = self.create_album(str(uuid.uuid4()))
+        status = self.add_to_album_from_query(query, temp_album["Title"], count=count, offset=offset, order=order)
+        status = self.download_album(temp_album["UID"])
+        status = self.remove_album_uid(temp_album["UID"])
+        return status
+
+
+
+
```

### Comparing `photoprism_client-0.1.3/PKG-INFO` & `photoprism_client-0.2.1/photoprism_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,117 @@
 Metadata-Version: 2.1
-Name: photoprism_client
-Version: 0.1.3
-Summary: A Python client to interact with photoprism. 
-Home-page: https://github.com/mvlnetdev/photoprism_client
-Author: mvlnetdev
-Author-email: maartenvanleeuwen1996@gmail.com
-License: MIT license
-Description: # Python client for PhotoPrism 
-        A Python client to interact with photoprism.
-        
-        ## IMPORTANT
-        This Python client is build on the undocumented API of PhotoPrism. There may be bugs in there. Please let me know if you find some. 
-        
-        Currently tested on the [version of the 17th of June 2022](https://github.com/photoprism/photoprism/releases/tag/220617-0402b8d3). It will probably work with later versions. Just try it and let me know, I will update the readme accordingly.  
-        
-        ## Requirements
-        - requests (latest)
-        
-        ## Setup
-        To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
-        ``` python
-        from photoprism.Session import Session
-        pp_session = Session("admin", "changethis", "demo.photoprism.app")
-        pp_session.create()
-        ```
-        
-        ## Searching
-        To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
-        
-        ```python
-        from photoprism.Photo import Photo
-        
-        p = Photo(pp_session)
-        p.search(query="original:*")
-        ```
-        
-        ## Other functions
-        This is a list of all other functions within the client. If you want other functions either request them or send a pull request.
-        | function | description | variables | returns |
-        | ---- | ----- | ------ | ----- |
-        | Photo.add_photos_to_album() | Add photos to an album, you will need to provide a list of UIDs of the photos you want to add. Returns True if successfull | photos: list, album_uid: string | True if successfull  |
-        | Photo.add_to_album_from_query() | Provide a search query and add all photos that are returned into an album. Provide the albumname, not the UID of the album. | query: string, albumname: string | True if successfull |
-        | Photo.check_if_album_exists() | Small function to check if an album exists | name: string, create_if_not: bool (default is False) | True if it exists, False if not (will continue to be False if the album is created) |
-        | Photo.create_album() | Create an album, returns a boolean if it worked | title: string | True if successfull |
-        | Photo.get_album() | Get all information of an album based upon the UID of the album | uid: string | Dict object with the information of the album, False if it does not exist |
-        | Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
-        | Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100) | list of uids |
-        | Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
-        | Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
-        | Photo.search() | Create the session | query: string, count: int (default=100) | Dict object of the results of the search |
-        | Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
-        | Photo.stop_import() | Stop an import job | None | True if successfully stopped |
-        | Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
-        | Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
-        
-        ## License 
-        MIT License
-        
-        Copyright (c) 2022 maartenvl
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Keywords: photoprism
-Platform: UNKNOWN
+Name: photoprism-client
+Version: 0.2.1
+Summary: A Python client to interact with photoprism.
+Author-email: mvlnetdev <maartenvanleeuwen1996@gmail.com>
+Project-URL: Homepage, https://github.com/mvlnetdev/photoprism_client
+Project-URL: Bug Tracker, https://github.com/mvlnetdev/photoprism_client/issues
+Project-URL: documentation, https://github.com/mvlnetdev/photoprism_client/blob/main/README.md
+Project-URL: changelog, https://github.com/mvlnetdev/photoprism_client/blob/main/changelog.md
+Keywords: photoprism,client,api
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python client for PhotoPrism 
+A Python client to interact with photoprism.
+
+Changelog can be found in [here](./changelog.md).
+
+## IMPORTANT
+This Python client is build on the undocumented API of PhotoPrism. There may be bugs in there. Please let me know if you find some. 
+
+Currently tested on the [version of the 17th of June 2022](https://github.com/photoprism/photoprism/releases/tag/220617-0402b8d3). It will probably work with later versions. Just try it and let me know, I will update the readme accordingly.  
+
+## Requirements
+- requests (latest)
+
+## Setup
+To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
+``` python
+from photoprism.Session import Session
+pp_session = Session("admin", "changethis", "demo.photoprism.app")
+pp_session.create()
+```
+
+### HTTPS
+It is possible to connect to Photoprism using HTTPS. Two variables exist for this:
+- use_https: Boolean
+- verify_cert: Boolean
+
+By default, a connection will be made using HTTP. A session can be set up using HTTPS by setting the use_https variable to _True_. By default the certificate will be verified. This check can be disabled by setting the verify_cert variable to _False_. Only change this if you understand what this means. It is better to leave this variable unchanged. 
+
+An example is:
+```python
+from photoprism.Session import Session
+pp_session = Session("admin", "changethis", "demo.photoprism.app", use_https=True, verify_cert=False)
+pp_session.create()
+```
+
+### User agent
+The user agent is _Photoprism Python Client_ by default. You can change this using the variable _user_agent_. 
+For example:
+```python
+from photoprism.Session import Session
+pp_session = Session("admin", "changethis", "demo.photoprism.app", user_agent="Hello World! This is an example.")
+pp_session.create()
+```
+
+## Searching
+To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
+
+```python
+from photoprism.Photo import Photo
+
+p = Photo(pp_session)
+p.search(query="original:*")
+```
+
+## Other functions
+This is a list of all other functions within the client. If you want other functions either request them or send a pull request.
+| function | description | variables | returns |
+| ---- | ----- | ------ | ----- |
+| Photo.add_photos_to_album() | Add photos to an album, you will need to provide a list of UIDs of the photos you want to add. Returns True if successfull | photos: list, album_uid: string | True if successfull  |
+| Photo.add_to_album_from_query() | Provide a search query and add all photos that are returned into an album. Provide the albumname, not the UID of the album. | query: string, albumname: string, count: int (default=1000000), offset: int (default=0), order: string (default="newest") | True if successfull |
+| Photo.check_if_album_exists() | Small function to check if an album exists | name: string, create_if_not: bool (default is False) | True if it exists, False if not (will continue to be False if the album is created) |
+| Photo.create_album() | Create an album, returns a boolean if it worked | title: string | Dict object with the album information |
+| Photo.download_album() | Download an entire album as ZIP. The file will get the same name as the title of the album, by setting the filename variable the name can be changed. | uid: string, path: string (default="."), filename: string (default=None) | True if successfull |
+| Photo.download_file() | Download a single file. The file will get the same name as in photoprism, by setting the filename variable the name can be changed. | hash: string, path: string (default="."), filename: string (default=None) | True if succesfull |
+| Photo.download_files_from_query() | Download files from a query | query: string, count: int (default=100), offset: int (default=0), order: string (default="newest") | True if succesfull | 
+| Photo.get_album() | Get all information of an album based upon the UID of the album | uid: string | Dict object with the information of the album, False if it does not exist |
+| Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
+| Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100), offset: int (default=0), order: string (default="newest") | list of uids |
+| Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
+| Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
+| Photo.search() | Create the session | query: string, count: int (default=100), offset: int (default=0), order: string (default="newest") | Dict object of the results of the search |
+| Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
+| Photo.stop_import() | Stop an import job | None | True if successfully stopped |
+| Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
+| Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
+| Photo.remove_album_uid() | Remove album based on album uid | uid: string | Dict of the removed album, False if action failed. |
+
+
+## License 
+MIT License
+
+Copyright (c) 2022 maartenvl
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
+SOFTWARE.
```

