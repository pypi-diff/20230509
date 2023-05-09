# Comparing `tmp/aioinsta-1.1.tar.gz` & `tmp/aioinsta-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioinsta-1.1.tar", last modified: Sat Jan 28 21:13:11 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aioinsta-1.1.tar` & `aioinsta-1.2.tar`

### file list

```diff
@@ -1,34 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-28 21:13:11.733208 aioinsta-1.1/
--rw-rw-rw-   0        0        0     1084 2023-01-17 21:05:37.000000 aioinsta-1.1/LICENSE
--rw-rw-rw-   0        0        0      353 2023-01-28 21:13:11.732212 aioinsta-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-01-19 13:29:15.000000 aioinsta-1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-28 21:13:11.683458 aioinsta-1.1/aioinsta/
--rw-rw-rw-   0        0        0      100 2023-01-20 13:28:07.000000 aioinsta-1.1/aioinsta/__init__.py
--rw-rw-rw-   0        0        0      270 2023-01-21 22:21:47.000000 aioinsta-1.1/aioinsta/client.py
--rw-rw-rw-   0        0        0      673 2023-01-22 14:12:18.000000 aioinsta-1.1/aioinsta/config.py
--rw-rw-rw-   0        0        0      157 2023-01-18 14:46:19.000000 aioinsta-1.1/aioinsta/enums.py
--rw-rw-rw-   0        0        0       47 2023-01-22 14:53:33.000000 aioinsta-1.1/aioinsta/exceptions.py
--rw-rw-rw-   0        0        0     3298 2023-01-22 16:31:27.000000 aioinsta-1.1/aioinsta/extractors.py
-drwxrwxrwx   0        0        0        0 2023-01-28 21:13:11.723234 aioinsta-1.1/aioinsta/methods/
--rw-rw-rw-   0        0        0       92 2023-01-21 22:21:41.000000 aioinsta-1.1/aioinsta/methods/__init__.py
--rw-rw-rw-   0        0        0    16873 2023-01-22 13:28:12.000000 aioinsta-1.1/aioinsta/methods/login.py
--rw-rw-rw-   0        0        0      942 2023-01-21 21:58:33.000000 aioinsta-1.1/aioinsta/methods/media.py
--rw-rw-rw-   0        0        0     1498 2023-01-28 20:45:23.000000 aioinsta-1.1/aioinsta/methods/user.py
--rw-rw-rw-   0        0        0     2266 2023-01-22 14:58:10.000000 aioinsta-1.1/aioinsta/request.py
-drwxrwxrwx   0        0        0        0 2023-01-28 21:13:11.731215 aioinsta-1.1/aioinsta/types/
--rw-rw-rw-   0        0        0      168 2023-01-22 16:27:15.000000 aioinsta-1.1/aioinsta/types/__init__.py
--rw-rw-rw-   0        0        0      540 2023-01-19 21:05:32.000000 aioinsta-1.1/aioinsta/types/media.py
--rw-rw-rw-   0        0        0      202 2023-01-19 21:05:32.000000 aioinsta-1.1/aioinsta/types/photo.py
--rw-rw-rw-   0        0        0     1159 2023-01-22 16:21:20.000000 aioinsta-1.1/aioinsta/types/story.py
--rw-rw-rw-   0        0        0     1045 2023-01-22 14:21:27.000000 aioinsta-1.1/aioinsta/types/user.py
--rw-rw-rw-   0        0        0      344 2023-01-18 21:28:50.000000 aioinsta-1.1/aioinsta/types/usershort.py
--rw-rw-rw-   0        0        0      304 2023-01-19 21:05:32.000000 aioinsta-1.1/aioinsta/types/video.py
--rw-rw-rw-   0        0        0      112 2023-01-20 22:02:49.000000 aioinsta-1.1/aioinsta/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-28 21:13:11.710187 aioinsta-1.1/aioinsta.egg-info/
--rw-rw-rw-   0        0        0      353 2023-01-28 21:13:11.000000 aioinsta-1.1/aioinsta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-01-28 21:13:11.000000 aioinsta-1.1/aioinsta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-28 21:13:11.000000 aioinsta-1.1/aioinsta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-01-28 21:13:11.000000 aioinsta-1.1/aioinsta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-28 21:13:11.000000 aioinsta-1.1/aioinsta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-28 21:13:11.733208 aioinsta-1.1/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-01-28 21:12:54.000000 aioinsta-1.1/setup.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/challenge.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/client.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/enums.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/exceptions.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/extractors.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/helpers.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/idcodec.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/login.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/media.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/password.py
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/request.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/user.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/types/media.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 aioinsta-1.2/aioinsta/types/user.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 aioinsta-1.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aioinsta-1.2/LICENSE
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aioinsta-1.2/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aioinsta-1.2/pyproject.toml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 aioinsta-1.2/PKG-INFO
```

### Comparing `aioinsta-1.1/LICENSE` & `aioinsta-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinsta-1.1/aioinsta/extractors.py` & `aioinsta-1.2/aioinsta/extractors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,78 @@
-from urllib.parse import urlparse
+import json
 
-from .enums import MediaType
-from .types import Media, Photo, UserShort, Video, Story, StoryMedia
+from aioinsta.types.media import Media, MediaType, Photo, Resource, Video
+from aioinsta.types.user import User, UserShort
 
 MEDIA_TYPES_GQL = {
-    "GraphImage": MediaType.PHOTO,
-    "GraphVideo": MediaType.VIDEO,
-    "GraphSidecar": MediaType.ALBUM,
-    "StoryVideo": MediaType.VIDEO,
+    "GraphImage": MediaType.Photo,
+    "GraphVideo": MediaType.Video,
+    "GraphSidecar": MediaType.Album,
+    "StoryVideo": MediaType.Video,
 }
 
-MEDIA_TYPES_V1 = {
-    1: MediaType.PHOTO,
-    2: MediaType.VIDEO
-}
 
-def excract_url_code(url: str):
-    path = urlparse(url).path
-    parts = [p for p in path.split("/") if p]
-    return parts.pop()
-
-
-def extract_user_short(data):
-    data["pk"] = data.get("id", data.get("pk", None))
-    return UserShort(**data)
-
-
-def exctract_album(data):
-    album = []
-    for album_media in data:
-        media_data = album_media["node"]
-        media_type = MEDIA_TYPES_GQL[media_data["__typename"]]
-        if media_type == MediaType.PHOTO:
-            album.append(Photo(photo_url=media_data.get("display_url")))
-        elif media_type == MediaType.VIDEO:
-            album.append(
-                Video(
-                    preview_url=media_data.get("display_url"),
-                    video_url=media_data.get("video_url"),
-                    view_count=media_data.get("video_view_count"),
-                )
-            )
-    return album
-
-
-def extract_media_gql(data):
-    if data.get("edge_media_to_caption")["edges"] != []:
-        caption = data.get("edge_media_to_caption")["edges"][0]["node"]["text"]
-    else:
-        caption = None
-    resources = data.get("edge_sidecar_to_children")
-    if resources:
-        album = exctract_album(resources.get("edges"))
-    else:
-        album = None
-    return Media(
-        media_type=MEDIA_TYPES_GQL[data["__typename"]],
-        user=extract_user_short(data["owner"]),
-        thumbnail_url=data.get("display_resources")[-1]["src"],
-        taken_at=data.get("taken_at_timestamp"),
-        photo=Photo(photo_url=data.get("display_resources")[-1]["src"]),
-        video=Video(
-            video_url=data.get("video_url"),
-            video_duration=data.get("video_duration"),
-            view_count=data.get("video_view_count"),
-            preview_url=data.get("display_resources")[-1]["src"],
-        ),
-        caption=caption,
-        like_count=data.get("edge_media_preview_like")["count"],
-        album=album,
+def extract_user_graphql(data: dict) -> User:
+    return User(
+        pk=data.get("id"),
+        media_count=data.get("edge_owner_to_timeline_media", {}).get("count", 0),
+        follower_count=data.get("edge_followed_by", {}).get("count", 0),
+        following_count=data.get("edge_follow", {}).get("count", 0),
+        **data,
     )
 
-def extract_story_v1(data):
-    thumbnail_url = data.get("image_versions2").get("candidates")[0]["url"]
-    if "video_versions" in data:
-        video_url = data.get("video_versions")[0]["url"]
-        video = Video(preview_url=thumbnail_url, video_url=video_url)
-        video_duration = data["video_duration"]
+
+def extract_user_v1(data: dict) -> User:
+    return User(
+        profile_pic_url_hd=data.get("hd_profile_pic_url_info").get("url"),
+        **data,
+    )
+
+
+def extract_user_short(data: dict) -> UserShort:
+    return UserShort(pk=data.get("id", data.get("pk")), **data)
+
+
+def extract_resource_gql(data: dict) -> Resource:
+    media_type = MEDIA_TYPES_GQL[data.get("__typename")]
+    return Resource(
+        pk=data.get("id"), media_type=media_type, url=data.get("display_url")
+    )
+
+
+def extract_media_gql(data: dict):
+    user = extract_user_short(data.get("owner"))
+    media_type = MEDIA_TYPES_GQL[data.get("__typename")]
+    media_id = data.get("id")
+    display_url = data.get("display_url")
+    caption = (
+        data.get("edge_media_to_caption", {})
+        .get("edges", [])[0]
+        .get("node", {})
+        .get("text")
+    )
+    if data.get("is_video", False):
+        photo = None
+        video = Video(
+            url=data.get("video_url"),
+            preview=display_url,
+            view_count=data.get("video_view_count"),
+            duration=data.get("video_duration"),
+        )
     else:
         video = None
-        video_duration = None
-    feed_medias = []
-    story_feed_medias = data.get('story_feed_media') or []
-    for feed_media in story_feed_medias:
-        feed_media["media_pk"] = int(feed_media["media_id"])
-        feed_medias.append(StoryMedia(**feed_media))
-    return Story(
-        pk=data["pk"],
-        id=data["id"],
-        code=data["code"],
+        photo = Photo(url=display_url)
+    return Media(
+        id=media_id,
+        code=data.get("shortcode"),
+        pk=media_id,
+        taken_at=data.get("taken_at_timestamp"),
+        user=user,
+        caption=caption or "",
+        media_type=media_type,
         video=video,
-        video_duration=video_duration,
-        media_type=MEDIA_TYPES_V1[data["media_type"]],
-        taken_at=data["taken_at"],
-        user=extract_user_short(data["user"]),
-        medias=feed_medias
+        photo=photo,
+        resource=[
+            extract_resource_gql(edge.get("node"))
+            for edge in data.get("edge_sidecar_to_children", {}).get("edges", [])
+        ],
     )
```

### Comparing `aioinsta-1.1/aioinsta/methods/user.py` & `aioinsta-1.2/aioinsta/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-import json
+from aioinsta import login
+from aioinsta.extractors import extract_user_graphql, extract_user_v1
+from aioinsta.types.user import User
 
-from typing import List
-from ..request import RequestClient
-from ..types import User, Story
-from .. import config
-from ..extractors import extract_story_v1
-
-class UserClient(RequestClient):
-    async def user_info_private(self, username: str):
-        info = await self.private_request(method="GET", path=f"users/{username}/usernameinfo/")
-        return info["json"]["user"]
-
-    async def user_stories_private(self, user_id: int) -> List[Story]:
-        params = {
-            "supported_capabilities_new": json.dumps(config.SUPPORTED_CAPABILITIES)
-        }
-        reel = (await self.private_request(method="GET", path=f"feed/user/{user_id}/story/", params=params))["json"].get("reel")
-        stories = []
-        for item in reel.get("items", []):
-            stories.append(extract_story_v1(item))
-        return stories
-    
-    async def user_medias_public(self, user_id: int) -> None:
-        pass
-        
-
-    async def user_stories(self, username: str) -> List[Story]:
-        user_id = (await self.user_info(username)).pk
-        return await self.user_stories_private(user_id)
-    
-    async def user_info(self, username: str) -> User:
-        username = username.lower()
-        user_info = await self.user_info_private(username)
-        return User(**user_info)
-    
-    async def user_medias(self, username: str) -> None:
-        username = username.lower()
-        user_id = (await self.user_info(username)).pk
-                
+
+class UserClient:
+    def __init__(self, login_client: "login.Login"):
+        self.login_client = login_client
+
+    async def user_info_by_username_gql(self, username: str) -> User:
+        response = await self.login_client.public_a1_request(
+            method="GET", path=f"/{username!s}/"
+        )
+        user = extract_user_graphql(response.get("user"))
+        return user
+
+    async def user_info_by_username_v1(self, username: str) -> User:
+        response = (
+            await self.login_client.private_request(
+                method="GET", path=f"users/{username}/usernameinfo"
+            )
+        ).get("response")
+        return extract_user_v1(response.get("user"))
+
+    async def user_info_from_username(self, username: str) -> User | None:
+        username = str(username).lower()
+        try:
+            return await self.user_info_by_username_gql(username)
+        except ValueError:
+            return await self.user_info_by_username_v1(username)
+
+    async def user_id_from_username(self, username: str):
+        return (await self.user_info_from_username(username)).pk
```

