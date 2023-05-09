# Comparing `tmp/aioinsta-1.4.tar.gz` & `tmp/aioinsta-1.5.tar.gz`

## Comparing `aioinsta-1.4.tar` & `aioinsta-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/challenge.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/client.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/enums.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/exceptions.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/extractors.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/helpers.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/idcodec.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/login.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/media.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/parametrs.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/password.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/request.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/user.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/types/media.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 aioinsta-1.4/aioinsta/types/user.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aioinsta-1.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aioinsta-1.4/LICENSE
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aioinsta-1.4/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aioinsta-1.4/pyproject.toml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 aioinsta-1.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/challenge.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/client.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/enums.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/exceptions.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/extractors.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/helpers.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/idcodec.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/login.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/media.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/parametrs.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/password.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/request.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/user.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/types/media.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 aioinsta-1.5/aioinsta/types/user.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aioinsta-1.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aioinsta-1.5/LICENSE
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aioinsta-1.5/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aioinsta-1.5/pyproject.toml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 aioinsta-1.5/PKG-INFO
```

### Comparing `aioinsta-1.4/aioinsta/challenge.py` & `aioinsta-1.5/aioinsta/challenge.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/extractors.py` & `aioinsta-1.5/aioinsta/extractors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from aioinsta.types.media import Media, MediaType, Photo, Resource, Video
 from aioinsta.types.user import User, UserShort
 
 MEDIA_TYPES_GQL = {
     "GraphImage": MediaType.Photo,
     "GraphVideo": MediaType.Video,
     "GraphSidecar": MediaType.Album,
@@ -28,16 +30,31 @@
 
 def extract_user_short(data: dict) -> UserShort:
     return UserShort(pk=data.get("id", data.get("pk")), **data)
 
 
 def extract_resource_gql(data: dict) -> Resource:
     media_type = MEDIA_TYPES_GQL[data.get("__typename")]
+    display_url = data.get("display_url")
+    if data.get("is_video", False):
+        photo = None
+        video = Video(
+            url=data.get("video_url"),
+            preview=display_url,
+            view_count=data.get("video_view_count"),
+            duration=data.get("video_duration"),
+        )
+    else:
+        video = None
+        photo = Photo(url=display_url)
     return Resource(
-        pk=data.get("id"), media_type=media_type, url=data.get("display_url")
+        pk=data.get("id"),
+        media_type=media_type,
+        video=video,
+        photo=photo
     )
 
 
 def extract_caption(data: dict) -> str | None:
     try:
         caption = (
             data.get("edge_media_to_caption", {})
```

### Comparing `aioinsta-1.4/aioinsta/helpers.py` & `aioinsta-1.5/aioinsta/helpers.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/idcodec.py` & `aioinsta-1.5/aioinsta/idcodec.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/login.py` & `aioinsta-1.5/aioinsta/login.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/media.py` & `aioinsta-1.5/aioinsta/media.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/parametrs.py` & `aioinsta-1.5/aioinsta/parametrs.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/password.py` & `aioinsta-1.5/aioinsta/password.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/request.py` & `aioinsta-1.5/aioinsta/request.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/user.py` & `aioinsta-1.5/aioinsta/user.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/aioinsta/types/media.py` & `aioinsta-1.5/aioinsta/types/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 
 class MediaType(str, Enum):
     Video = "video"
     Photo = "photo"
     Album = "album"
 
 
-class Resource(BaseModel):
-    pk: str
-    media_type: MediaType
-    url: HttpUrl
-
-
 class Video(BaseModel):
     url: HttpUrl
     preview: HttpUrl
     view_count: int
-    duration: float
+    duration: float | None = 0.0
 
 
 class Photo(BaseModel):
     url: HttpUrl
 
 
+class Resource(BaseModel):
+    pk: str
+    media_type: MediaType
+    photo: Photo | None = None
+    video: Video | None = None
+
+
 class Media(BaseModel):
     pk: str
     id: str
     code: str
     user: UserShort
     caption: str | None
     taken_at: datetime
```

### Comparing `aioinsta-1.4/aioinsta/types/user.py` & `aioinsta-1.5/aioinsta/types/user.py`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/.gitignore` & `aioinsta-1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/LICENSE` & `aioinsta-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/pyproject.toml` & `aioinsta-1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aioinsta-1.4/PKG-INFO` & `aioinsta-1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioinsta
-Version: 1.4
+Version: 1.5
 Summary: Tool for parse instagram data
 Project-URL: Homepage, https://github.com/sheldygg/aioinsta
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

