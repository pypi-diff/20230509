# Comparing `tmp/insta-tweet-2.1.3.tar.gz` & `tmp/insta-tweet-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insta-tweet-2.1.3.tar", last modified: Thu Apr 27 10:31:42 2023, max compression
+gzip compressed data, was "insta-tweet-2.2.0.tar", last modified: Tue May  9 03:37:56 2023, max compression
```

## Comparing `insta-tweet-2.1.3.tar` & `insta-tweet-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 10:31:42.685035 insta-tweet-2.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-27 10:31:42.669416 insta-tweet-2.1.3/InstaTweet/
--rw-rw-rw-   0        0        0      349 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/__init__.py
--rw-rw-rw-   0        0        0     5070 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/db.py
--rw-rw-rw-   0        0        0     4516 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/instaclient.py
--rw-rw-rw-   0        0        0     4494 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/instapost.py
--rw-rw-rw-   0        0        0     5831 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/instatweet.py
--rw-rw-rw-   0        0        0     2833 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/instauser.py
--rw-rw-rw-   0        0        0    17255 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/profile.py
--rw-rw-rw-   0        0        0     7454 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/tweetclient.py
--rw-rw-rw-   0        0        0     1695 2023-04-27 09:44:14.000000 insta-tweet-2.1.3/InstaTweet/utils.py
--rw-rw-rw-   0        0        0     1084 2023-04-27 09:24:17.000000 insta-tweet-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     7529 2023-04-27 10:31:42.685035 insta-tweet-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6547 2023-04-27 10:15:34.000000 insta-tweet-2.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-27 10:31:42.685035 insta-tweet-2.1.3/insta_tweet.egg-info/
--rw-rw-rw-   0        0        0     7529 2023-04-27 10:31:42.000000 insta-tweet-2.1.3/insta_tweet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-04-27 10:31:42.000000 insta-tweet-2.1.3/insta_tweet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 10:31:42.000000 insta-tweet-2.1.3/insta_tweet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-27 10:31:42.000000 insta-tweet-2.1.3/insta_tweet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 10:31:42.000000 insta-tweet-2.1.3/insta_tweet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 10:31:42.685035 insta-tweet-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-04-27 10:31:06.000000 insta-tweet-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/
+drwxrwxrwx   0        0        0        0 2023-05-09 03:37:56.869286 insta-tweet-2.2.0/InstaTweet/
+-rw-rw-rw-   0        0        0      325 2023-05-09 03:33:58.000000 insta-tweet-2.2.0/InstaTweet/__init__.py
+-rw-rw-rw-   0        0        0     5070 2023-05-09 03:04:05.000000 insta-tweet-2.2.0/InstaTweet/db.py
+-rw-rw-rw-   0        0        0     6775 2023-05-09 03:18:47.000000 insta-tweet-2.2.0/InstaTweet/instaclient.py
+-rw-rw-rw-   0        0        0     6257 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/instapage.py
+-rw-rw-rw-   0        0        0     4852 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/instapost.py
+-rw-rw-rw-   0        0        0     6084 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/instatweet.py
+-rw-rw-rw-   0        0        0    15926 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/profile.py
+-rw-rw-rw-   0        0        0     7454 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/tweetclient.py
+-rw-rw-rw-   0        0        0     1695 2023-05-04 08:44:04.000000 insta-tweet-2.2.0/InstaTweet/utils.py
+-rw-rw-rw-   0        0        0     1084 2023-04-27 09:24:17.000000 insta-tweet-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0     7764 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6812 2023-05-09 03:36:31.000000 insta-tweet-2.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/insta_tweet.egg-info/
+-rw-rw-rw-   0        0        0     7764 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-05-09 03:32:35.000000 insta-tweet-2.2.0/setup.py
```

### Comparing `insta-tweet-2.1.3/InstaTweet/db.py` & `insta-tweet-2.2.0/InstaTweet/db.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.1.3/InstaTweet/instapost.py` & `insta-tweet-2.2.0/InstaTweet/instapost.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+from __future__ import annotations
 import os
-from functools import cached_property
-from typing import Union, List
 from datetime import datetime
 from tweepy.models import Status
+from functools import cached_property
+from typing import Union, List, Optional, Dict
 
 
 class InstaPost:
 
     """Minimalistic API response wrapper for an Instagram post"""
 
-    def __init__(self, post_data: dict):
+    def __init__(self, data: dict, client: Optional["InstaClient"] = None):
         """Initialize an :class:`~InstaPost`
 
-        :param post_data: the JSON response data of a single Instagram post, found within the :attr:`~.InstaUser.user_data`
+        :param data: the JSON response data of a single Instagram post, found within the :attr:`~.InstaUser.user_data`
         """
         #: Source data from API response
-        self.json = post_data
+        self.json = data
+        self.client = client
         #: The post id
-        self.id = post_data['id']
-        self.dimensions: dict = post_data.get('dimensions', {})
-        self.is_video: bool = post_data.get('is_video', False)
-        self.video_url = post_data.get('video_url', '')
+        self.id = data['id']
+        self.dimensions: dict = data.get('dimensions', {})
+        self.is_video: bool = data.get('is_video', False)
+        self.video_url = data.get('video_url', '')
         #: Path of downloaded media, set by :meth:`~.InstaClient.download_post`
         self.filepath: str = ''
         #: Limited data from a successful tweet based off this post, set by :meth:`~.TweetClient.send_tweet`
         self.tweet_data: dict = {}
 
     def __str__(self):
         return f'Post {self.id} by @{self.owner["username"]} on {self.timestamp}'
 
     @cached_property
-    def children(self) -> List["InstaPost"]:
+    def children(self) -> List[InstaPost]:
         """If the post is a carousel, returns a list of child :class:`InstaPost`'s"""
         if self.is_carousel:
             edges = self.json['edge_sidecar_to_children']['edges']
             return [InstaPost(edge['node']) for edge in edges]
         return []
 
     @property
@@ -48,14 +50,18 @@
     @property
     def caption(self) -> str:
         if caption_edge := self.json.get('edge_media_to_caption', {}).get('edges', []):
             return caption_edge[0].get('node', {}).get('text', '')
         return ''
 
     @property
+    def likes(self) -> Optional[int]:
+        return self.json.get('edge_liked_by', {}).get('count')
+
+    @property
     def media_url(self) -> str:
         """The direct URL to the actual post content
 
         :returns: the :attr:`~.video_url` if the post is a video, otherwise the :attr:`~.thumbnail_url`
         """
         return self.video_url if self.is_video else self.thumbnail_url
 
@@ -92,16 +98,19 @@
 
     @property
     def filetype(self) -> str:
         """Filetype of the post, based on the value of :attr:`~is_video`"""
         return '.mp4' if self.is_video else '.jpg'
 
     @property
-    def owner(self) -> dict:
-        if owner := self.json.get('owner', self.json.get('user', {})):
+    def owner(self) -> Dict:
+        if owner := self.json.get('owner', {}):
+            if not owner.get('username'):
+                if self.client and (uid := owner.get('id')):
+                    owner['username'] = self.client.get_username(uid)
             return owner
         return dict.fromkeys(['id', 'username'])
 
     @property
     def timestamp(self) -> Union[datetime, str]:
         if timestamp := self.json.get('taken_at_timestamp', self.json.get('taken_at', '')):
             return datetime.utcfromtimestamp(timestamp)
```

### Comparing `insta-tweet-2.1.3/InstaTweet/instatweet.py` & `insta-tweet-2.2.0/InstaTweet/instatweet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, List
+from typing import Optional, List, Dict
 from . import utils, TweetClient, InstaClient, InstaPost, Profile
 
 
 class InstaTweet:
 
     """Uses the settings from a Profile to do the actual InstaTweeting
 
     You might be wondering, what's InstaTweeting? According to TDK Dictionary:
 
         .. admonition:: **InstaTweet** (`verb`):
            :class: instatweet
 
-           To load a :class:`~.Profile` 🠖 scrape :attr:`~.posts` from its Instagram users
+           To load a :class:`~.Profile` 🠖 scrape :attr:`~.posts` from its Instagram pages
            🠖 :meth:`~.download_post` & :meth:`~.send_tweet` for any new content
-           🠖 update the :attr:`~.user_map`
+           🠖 update the :attr:`~.page_map`
            🠖 :meth:`~.save` the profile if it :attr:`~.exists`
 
             .. admonition:: **Example Sentence**
                :class: example
 
                Oh, you lost 700 Twitter followers after you shared your IG post? Well maybe if people actually saw the
                picture and not just the caption your tweet would've been less creepy. You should've InstaTweeted it.
@@ -40,19 +40,18 @@
 
     @classmethod
     def load(cls, profile_name: str, local: bool = True) -> "InstaTweet":
         """Loads a profile by name
 
         :param profile_name: name of the Profile to load
         :param local: whether the profile is saved locally (default) or remotely on a database
-
         """
         return cls(profile=Profile.load(name=profile_name, local=local))
 
-    def get_proxies(self) -> Optional[dict]:
+    def get_proxies(self) -> Optional[Dict]:
         """Retrieve proxies using the loaded Profile's :attr:`~Profile.proxy_key`"""
         return utils.get_proxies(
             env_key=self.profile.proxy_key
         )
 
     def get_insta_client(self) -> InstaClient:
         """Initializes an :class:`~.InstaClient` using the loaded :class:`~.Profile` settings"""
@@ -65,79 +64,85 @@
     def get_tweet_client(self) -> TweetClient:
         """Initializes an :class:`~.TweetClient` using the loaded :class:`~.Profile` settings"""
         return TweetClient(
             profile=self.profile,
             proxies=self.proxies
         )
 
-    def start(self) -> None:
-        """InstaTweets all users that have been added to the loaded :class:`~.Profile`
+    def start(self, max_posts: int = 12) -> None:
+        """InstaTweets all pages that have been added to the loaded :class:`~.Profile`
+
+        The most recent posts from each page will be scraped, then compared to the ``scraped``
+        list in the :attr:`~.PAGE_MAPPING` to determine which are new.
 
-        Each user's IG page will be scraped and compared to the ``scraped`` list in their :attr:`~.USER_MAPPING`.
-        Posts that weren't previously scraped will be downloaded and tweeted
+        Up to ``max_posts`` new posts from each page will then be downloaded and tweeted
 
         .. note:: If ``InstaTweet`` fails to :meth:`~.download_post` or :meth:`~.send_tweet`,
-           the :attr:`~.USER_MAPPING` won't be updated
+           the :attr:`~.PAGE_MAPPING` won't be updated
 
            * This ensures that failed repost attempts are retried in the next call to :meth:`~start`
 
            If a save file for the Profile already :attr:`~.exists`, successful reposts
            will trigger a call to :meth:`~.save`
+
+        :param max_posts: the maximum number of new posts to download and tweet per page
         """
         profile = self.profile
         profile.validate()
 
         print(f'Starting InstaTweet for Profile: {profile.name}')
 
-        for user in profile.user_map:
-            new_posts = self.get_new_posts(user)
-            if not new_posts:
-                print(f'No posts to tweet for @{user}')
+        for page in profile.page_map:
+            page_name = page if page.startswith("#") else "@" + page
+
+            if not (new_posts := self.get_new_posts(page)):
+                print(f'No posts to tweet for {page_name}')
                 continue
 
-            print(f'There are {len(new_posts)} posts to tweet for @{user}')
-            hashtags = profile.get_hashtags_for(user)
+            print(f'There are {len(new_posts)} posts to tweet for {page_name}')
+            hashtags = profile.get_hashtags_for(page)
 
-            for post in new_posts:
+            for post in new_posts[:max_posts]:
                 self.insta.download_post(post)
                 if not post.is_downloaded:
                     continue
 
                 tweeted = self.twitter.send_tweet(post, hashtags)
                 if not tweeted:
                     continue
 
-                profile.get_scraped_from(user).append(post.id)
-                profile.get_tweets_for(user).append(post.tweet_data)
+                profile.get_scraped_from(page).append(post.id)
+                profile.get_tweets_for(page).append(post.tweet_data)
 
                 if profile.exists:
                     profile.save(alert=False)
 
-            print(f'Finished insta-tweeting for @{user}')
+            print(f'Finished insta-tweeting for {page_name}')
+
+        print(f'All pages have been insta-tweeted')
 
-        print(f'All users have been insta-tweeted')
+    def get_new_posts(self, insta_page: str) -> Optional[List[InstaPost]]:
+        """Scrapes recent posts from an Instagram page and returns all posts that haven't been tweeted yet
 
-    def get_new_posts(self, username) -> Optional[List[InstaPost]]:
-        """Scrapes recent posts from an Instagram user and returns all posts that haven't been tweeted yet
+        **NOTE:**  If a page's ``scraped`` list is empty, no posts will be returned.
 
-        **NOTE:**  If a user's ``scraped`` list is empty, no posts will be returned.
+        Instead, the page is "initialized" as follows:
 
-        Instead, the user is "initialized" as follows:
-          * Their ``scraped`` list will be populated with the ID's from the most recent posts
-          * These IDs are then used in future calls to the method to determine which posts to tweet
+        * The ``scraped`` list will be populated with the ID's from the most recent posts
+        * These IDs are then used in future method calls to determine which posts to tweet
 
-        :param username: the IG username to scrape posts from
-        :return: a list of posts that haven't been tweeted yet, or nothing at all (if user is only initialized)
+        :param insta_page: the Instagram page to scrape posts from
+        :return: a list of posts that haven't been tweeted yet, or nothing at all (if page is only initialized)
 
         """
-        print(f'Checking posts from @{username}')
-        scraped_posts = self.profile.get_scraped_from(username)
-        user = self.insta.get_user(username)
+        print(f'Checking posts from {insta_page}')
+        scraped_posts = self.profile.get_scraped_from(insta_page)
+        page = self.insta.scrape(insta_page)
 
         if scraped_posts:
-            new_posts = [post for post in user.posts if post.id not in scraped_posts]
+            new_posts = [post for post in page.posts if post.id not in scraped_posts]
             return sorted(new_posts, key=lambda post: post.timestamp)
         else:
-            scraped_posts.extend(post.id for post in user.posts)
-            print(f'Initialized User: @{username}')
+            scraped_posts.extend(post.id for post in page.posts)
+            print(f'Initialized {page}')
             return None
```

### Comparing `insta-tweet-2.1.3/InstaTweet/profile.py` & `insta-tweet-2.2.0/InstaTweet/profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,129 +1,94 @@
 from __future__ import annotations
-
 import os
 import copy
 import json
 import pickle
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Dict
 from . import TweetClient, DBConnection, USER_AGENT
 
 
 class Profile:
 
     """The :class:`Profile` is a configuration class used extensively throughout the package
 
-    It consists of a :attr:`~user_map` and an associated collection of API/web scraping :ref:`settings <settings>`
+    It consists of a :attr:`~page_map` and an associated collection of API/web scraping :ref:`settings <settings>`
 
     ...
 
-    .. admonition:: About the User Map
+    .. admonition:: About the Page Map
         :class: instatweet
 
-        The :attr:`~user_map` is a dict containing info about the users added to a :class:`Profile`
+        **The** :attr:`~.page_map` **is a dict containing info about the pages added to a** :class:`~.Profile`
 
-        * It's used to help detect new posts and compose tweets on a per-user basis
-        * Entries are created when you :meth:`add_users`, which map the user to a :attr:`~USER_MAPPING`
-        * The :attr:`~USER_MAPPING` maintains lists of hashtags, scraped posts, and sent tweets
-        * The mapping is updated when you :meth:`add_hashtags` and successfully :meth:`~.send_tweet`
-
-        You can access entries in the :attr:`~user_map` as follows:
-
-        * :meth:`~get_user` allows you to retrieve a full entry by username
-        * :meth:`~get_hashtags_for`, :meth:`get_scraped_from`, :meth:`get_tweets_for` provide access
-          to lists
+        * It's used to help detect new posts and compose tweets on a per-page basis
+        * Entries are created when you :meth:`~.add_pages`, which map the page to a :attr:`~.PAGE_MAPPING`
+        * The :attr:`~.PAGE_MAPPING` maintains lists of hashtags, scraped posts, and sent tweets
+        * The mapping is updated when you :meth:`~.add_hashtags` and successfully :meth:`~.send_tweet`
 
     ...
 
     **[Optional]**
 
-    A unique, identifying :attr:`~name` can be assigned to the Profile, which
-    may then be used to :meth:`~save` and, in turn, :meth:`~load` its settings
+    A unique, identifying :attr:`~name` can optionally be assigned to the Profile,
+    which may then be used to :meth:`~save` and :meth:`~load` its settings
 
-    * This makes it extremely easy to switch between Profiles and create templates
+    The save location is determined by the value of :attr:`Profile.local` as follows:
 
-    Saving isn't a requirement to :meth:`~.start` InstaTweet, but...
+    * If ``True``, saves are made locally to the :attr:`~LOCAL_DIR` as .pickle files
+    * If ``False``, saves are made remotely to a database as pickle bytes
 
-    * To :meth:`~.get_new_posts`, InstaTweet makes comparisons
-      with the ``scraped`` list in the :attr:`~.user_map`
-    * Saving this list ensures you don't :meth:`~.send_tweet`
-      for a post more than once
+    See :ref:`save-profile` for more information
 
     ...
-
-    .. admonition:: Important
-       :class: important-af
-
-       If you do :meth:`~save` your profile, the save location is determined by the value of :attr:`Profile.local`
-
-       * Local saves are made to the :attr:`~LOCAL_DIR`, as pickle files
-       * Remote saves are made to a database (via the :mod:`~.db` module) as pickle bytes
-
-       **You MUST configure the** :attr:`~InstaTweet.db.DATABASE_URL` **environment variable to save/load remotely**
-
-       * InstaTweet uses ``SQLAlchemy`` to create a :class:`~.DBConnection` -- any db it supports is compatible
-       * See the :mod:`~.db` module for more information
-
     """
-
-    USER_MAPPING = {'hashtags': [], 'scraped': [], 'tweets': []}  #: Template for an entry in the ``user_map``
-    LOCAL_DIR = Path(__file__).parent.parent.joinpath("profiles") #: Directory where local profiles are saved
+    #: Template for an entry in the :attr:`~page_map`
+    PAGE_MAPPING: Dict = {'hashtags': [], 'scraped': [], 'tweets': []}
+    #: Directory where local profiles are saved
+    LOCAL_DIR: str = Path(__file__).parent.parent.joinpath("profiles")
 
     def __init__(self, name: str = 'default', local: bool = True, **kwargs):
         """Create a new :class:`Profile`
 
-        .. note:: :class:`Profile` creation is mandatory to use the ``InstaTweet`` package
-
-           * Required as a parameter to initialize an :class:`~.InstaTweet` object
-           * Naming and saving it is ideal, but not necessary to :meth:`~.start` InstaTweet
-
         :param name: unique profile name
         :param local: indicates if profile is being saved locally or on a remote database
         :param kwargs: see below
 
         :Keyword Arguments:
             * *session_id* (``str``)
                 Instagram ``sessionid`` cookie, obtained by logging in through browser
             * *twitter_keys* (``dict``)
                 Twitter API Keys with v1.1 endpoint access
                 (see :attr:`~.TweetClient.DEFAULT_KEYS` for a template)
             * *user_agent* (``str``) -- Optional
-                The user agent to use for requests; uses a currently working hardcoded agent if not provided
+                The user agent to use for requests
             * *proxy_key* (``str``) -- Optional
                 Environment variable to retrieve proxies from
-            * .. autoattribute:: user_map
-                 :annotation:
-                 :noindex:
-
-        .. admonition:: **Profile Creation Tips**
-           :class: instatweet
-
-           * All attributes can be passed as arguments at initialization or set directly afterwards
-           * Property setters validate data types for the :ref:`mandatory-settings`
-           * The :class:`~Profile` as a whole is validated by :meth:`~validate`
-
-
         """
         self.local = local
         self.name = name    # Will raise Exception if name is already used
 
-        self.session_id = kwargs.get('session_id', '')
-        self.twitter_keys = kwargs.get('twitter_keys', TweetClient.DEFAULT_KEYS)
-        self.user_agent = kwargs.get('user_agent', USER_AGENT)
-        self.proxy_key = kwargs.get('proxy_key', None)
-        self.user_map = kwargs.get('user_map', {})  #: ``dict``: Mapping of added Instagram users and their :attr:`~USER_MAPPING`
+        #: Instagram ``sessionid`` cookie, obtained by logging in through browser
+        self.session_id: str = kwargs.get('session_id', '')
+        #: Twitter API Keys with v1.1 endpoint access (see :attr:`~.DEFAULT_KEYS` for a template)
+        self.twitter_keys: Dict = kwargs.get('twitter_keys', TweetClient.DEFAULT_KEYS)
+        #: The user agent to use for requests
+        self.user_agent: str = kwargs.get('user_agent', USER_AGENT)
+        #: Environment variable to retrieve proxies from
+        self.proxy_key: str = kwargs.get('proxy_key', None)
+        #: Mapping of added Instagram pages and their :attr:`~PAGE_MAPPING`
+        self.page_map: Dict[str, Dict] = kwargs.get('page_map', {})
 
     @classmethod
     def load(cls, name: str, local: bool = True) -> Profile:
         """Loads an existing profile from a locally saved pickle file or remotely stored pickle bytes
 
         :param name: the name of the :class:`Profile` to load
         :param local: whether the profile is saved locally (default, ``True``) or remotely on a database
-
         """
         if not cls.profile_exists(name, local):
             raise LookupError(
                 f'No {"local" if local else "database"} profile found with the name "{name}"'
             )
         if local:
             with open(cls.get_local_path(name), 'rb') as f:
@@ -134,15 +99,15 @@
 
     @classmethod
     def from_json(cls, json_str: str) -> Profile:
         """Creates a profile from a JSON formatted string of config settings"""
         return cls.from_dict(json.loads(json_str))
 
     @classmethod
-    def from_dict(cls, d: dict) -> Profile:
+    def from_dict(cls, d: Dict) -> Profile:
         """Creates a profile from a dictionary of config settings"""
         return cls(**d)
 
     @staticmethod
     def profile_exists(name: str, local: bool = True) -> bool:
         """Checks locally/remotely to see if a :class:`~Profile` with the specified name has an existing save file
 
@@ -160,63 +125,66 @@
                 return bool(db.query_profile(name).first())
 
     @staticmethod
     def get_local_path(name: str) -> str:
         """Returns filepath of where a local profile would be saved"""
         return os.path.join(Profile.LOCAL_DIR, name) + '.pickle'
 
-    def add_users(self, users: Iterable, send_tweet: bool = False):
-        """Add Instagram user(s) to the :attr:`~.user_map` for subsequent monitoring
+    def add_pages(self, pages: Iterable, send_tweet: bool = False) -> None:
+        """Add Instagram page(s) to the :attr:`~.page_map` for subsequent monitoring
 
-        .. note:: By default, newly added users won't have their posts tweeted the first time they're scraped
+        * An Instagram profile can be added as ``"@username"`` or ``"username"``
+        * A hashtag must be added as ``"#hashtag"``
 
-           * The IDs of the ~12 most recent posts are stored in the ``scraped`` list
+
+        .. note:: By default, newly added pages won't have their posts tweeted the first time they're scraped
+
+           * The IDs of the most recent posts are stored in the ``scraped`` list
            * Any new posts from that point forward will be tweeted
 
-           You can override this by setting ``send_tweet=True``
+           You can scrape AND tweet posts on the first run by setting ``send_tweet=True``
 
-           * This causes their ~12 most recent posts to be scraped AND tweeted
 
-        :param users: Instagram username(s) to automatically scrape and tweet content from
+        :param pages: Instagram pages to automatically scrape and tweet content from
         :param send_tweet: choose if tweets should be sent on the first scrape, or only for new posts going forward
         """
-        if not isinstance(users, Iterable):
-            raise TypeError(f'Invalid type provided. `users` must be an Iterable')
-        if isinstance(users, str):
-            users = [users]
-
-        for user in users:
-            mapping = copy.deepcopy(Profile.USER_MAPPING)
-            self.user_map.setdefault(user, mapping)
+        if not isinstance(pages, Iterable):
+            raise TypeError(f'Invalid type provided. `pages` must be an Iterable')
+        if isinstance(pages, str):
+            pages = [pages]
+
+        for page in pages:
+            mapping = copy.deepcopy(Profile.PAGE_MAPPING)
+            self.page_map.setdefault(page.lstrip("@"), mapping)
 
             if send_tweet:  # Non-empty scraped list will trigger Tweets to send
-                self.get_scraped_from(user).append(-1)
+                self.get_scraped_from(page).append(-1)
 
-            print(f'Added Instagram user @{user} to the user map')
+            print(f'Added Instagram page {page} to the page map')
 
         if self.exists:
             self._save_profile(alert=False)
 
-    def add_hashtags(self, user: str, hashtags: Iterable):
-        """Add hashtag(s) to a user in the :attr:`~.user_map`, which will be randomly chosen from when composing Tweets
+    def add_hashtags(self, page: str, hashtags: Iterable):
+        """Add hashtag(s) to a page in the :attr:`~.page_map`, which will be randomly chosen from when composing Tweets
 
-        :param user: the user in the user map to add hashtags to
-        :param hashtags: hashtags to choose from and include in any Tweets where content comes from this user
+        :param page: the page in the page map to add hashtags to
+        :param hashtags: hashtags to choose from and include in any Tweets where content comes from this page
         """
         if not isinstance(hashtags, Iterable):
             raise TypeError("Hashtags must be provided as a string or iterable of strings")
         if isinstance(hashtags, str):
             hashtags = [hashtags]
 
-        tags = self.get_hashtags_for(user)  # Retrieve the current hashtag list
+        tags = self.get_hashtags_for(page)  # Retrieve the current hashtag list
         tags.extend(set(hashtags) - set(tags))  # Add new ones (case-sensitive)
 
         if self.exists:
             self._save_profile(alert=False)
-        print(f'Added hashtags for @{user}')
+        print(f'Added hashtags for {page}')
 
     def save(self, name: str = None, alert: bool = True) -> bool:
         """Pickles and saves the :class:`Profile` using the specified or currently set name.
 
         :param name: name to save the :class:`Profile` under; replaces the current :attr:`~.name`
         :param alert: set to ``True`` to print a message upon successful save
         """
@@ -238,24 +206,24 @@
         else:
             with DBConnection() as db:
                 return db.save_profile(profile=self, alert=alert)
 
     def validate(self) -> None:
         """Checks to see if the Profile is fully configured for InstaTweeting
 
-        :raises ValueError: if the :attr:`~.session_id`, :attr:`~.twitter_keys`, or :attr:`~.user_map` are invalid
+        :raises ValueError: if the :attr:`~.session_id`, :attr:`~.twitter_keys`, or :attr:`~.page_map` are invalid
         """
         if not self.session_id:
             raise ValueError('Instagram sessionid cookie is required to scrape posts')
 
         if bad_keys := [key for key, value in self.twitter_keys.items() if value == 'string']:
             raise ValueError(f'Values not set for the following Twitter keys: {bad_keys}')
 
-        if not self.user_map:
-            raise ValueError('You must add at least one Instagram user to auto-tweet from')
+        if not self.page_map:
+            raise ValueError('You must add at least one Instagram page to auto-tweet from')
 
     def to_pickle(self) -> bytes:
         """Serializes profile to a pickled byte string"""
         return pickle.dumps(self)
 
     def to_json(self) -> str:
         """Serializes profile to a JSON formatted string"""
@@ -276,15 +244,15 @@
         return {
             'name': self.name,
             'local': self.local,
             'session_id': self.session_id,
             'twitter_keys': self.twitter_keys,
             'user_agent': self.user_agent,
             'proxy_key': self.proxy_key,
-            'user_map': self.user_map,
+            'page_map': self.page_map,
         }
 
     @property
     def exists(self) -> bool:
         """Returns True if a local save file or database record exists for the currently set profile name"""
         return self.profile_exists(name=self.name, local=self.local)
 
@@ -296,36 +264,34 @@
     @property
     def profile_path(self) -> str:
         """If :attr:`~.local` is ``True``, returns the file path for where this profile would be/is saved"""
         if self.local and not self.is_default:
             return Profile.get_local_path(self.name)
         return ''
 
-    def get_user(self, user: str) -> dict:
-        """Returns the specified user's dict entry in the :attr:`user_map`"""
-        return self.user_map[user]
-
-    def get_scraped_from(self, user: str) -> list:
-        """Returns a list of posts that have been scraped from the specified user"""
-        return self.user_map[user]['scraped']
-
-    def get_tweets_for(self, user: str) -> list:
-        """Returns a list of tweets that use the specified user's scraped content"""
-        return self.user_map[user]['tweets']
-
-    def get_hashtags_for(self, user: str) -> list:
-        """Returns the hashtag list for the specified user"""
-        return self.user_map[user]['hashtags']
+    def get_page(self, page: str) -> dict:
+        """Returns the specified page's dict entry in the :attr:`page_map`"""
+        return self.page_map[page.lstrip('@')]
+
+    def get_scraped_from(self, page: str) -> list:
+        """Returns a list of posts that have been scraped from the specified page"""
+        return self.get_page(page)['scraped']
+
+    def get_tweets_for(self, page: str) -> list:
+        """Returns a list of tweets that use the specified page's scraped content"""
+        return self.get_page(page)['tweets']
+
+    def get_hashtags_for(self, page: str) -> list:
+        """Returns the hashtag list for the specified page"""
+        return self.get_page(page)['hashtags']
 
     @property
     def local(self) -> bool:
         """Indicates if saves should be made locally (``True``) or on a remote database (``False``)
-
-         :rtype: bool
-         """
+        """
         return self._local
 
     @local.setter
     def local(self, local: bool):
         if local:
             if not os.path.exists(self.LOCAL_DIR):
                 os.mkdir(self.LOCAL_DIR)
@@ -355,15 +321,15 @@
 
         :raises FileExistsError: if :attr:`~local` ``==True`` and a save is found in the :attr:`~LOCAL_DIR`
         :raises ResourceWarning: if :attr:`~local` ``==False`` and a database row is found by :meth:`~.query_profile`
         """
         return self._name
 
     @name.setter
-    def name(self, profile_name):
+    def name(self, profile_name: str):
         """Sets the profile name, if a profile with that name doesn't already exist locally/remotely"""
         if profile_name != 'default' and self.profile_exists(profile_name, local=self.local):
             if self.local:
                 raise FileExistsError(
                     'Local save file already exists for profile named "{}"\n'.format(profile_name) +
                     'Please choose another name, load the profile, or delete the file.')
             else:
@@ -388,15 +354,15 @@
                 f'Session ID cookie must be of type {str}'
             )
         self._session_id = session_id
         if self.exists:
             self._save_profile(alert=False)
 
     @property
-    def twitter_keys(self) -> dict:
+    def twitter_keys(self) -> Dict:
         """Twitter developer API keys with v1.1 endpoint access. See :attr:`~.DEFAULT_KEYS`"""
         return self._twitter_keys
 
     @twitter_keys.setter
     def twitter_keys(self, api_keys: dict):
         if not isinstance(api_keys, dict):
             raise TypeError(
```

### Comparing `insta-tweet-2.1.3/InstaTweet/tweetclient.py` & `insta-tweet-2.2.0/InstaTweet/tweetclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     def build_tweet(self, post: InstaPost, hashtags: Optional[list[str]] = None) -> str:
         """Uses an :class:`~.InstaPost` to build the body text of a tweet
 
         .. admonition:: How Tweets are Composed
            :class: instatweet
 
            - The :attr:`~.InstaPost.caption` is used as a starting point
-           - If you :meth:`~.add_hashtags` for the user, it will randomly :meth:`~pick_hashtags` to include
+           - If you :meth:`~.add_hashtags` for the page, it will randomly :meth:`~pick_hashtags` to include
            - Lastly, the post's :attr:`~.InstaPost.permalink` is added to the end
 
         **Example**::
 
          >> post = instatweet.insta.get_user("dailykittenig").posts[0]
          >> tweet = instatweet.twitter.build_tweet(post)
          >> print(tweet)
```

### Comparing `insta-tweet-2.1.3/InstaTweet/utils.py` & `insta-tweet-2.2.0/InstaTweet/utils.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.1.3/LICENSE` & `insta-tweet-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.1.3/PKG-INFO` & `insta-tweet-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insta-tweet
-Version: 2.1.3
+Version: 2.2.0
 Summary: Automatically Repost Content From Instagram to Twitter
 Home-page: https://www.github.com/TDKorn/insta-tweet/
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT
 Download-URL: https://github.com/TDKorn/insta-tweet/tarball/master/
 Keywords: instagram,twitter,api,instagram api,twitter api,repost,instagram repost,reposter
@@ -12,24 +12,24 @@
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. meta::
    :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
    :description: A Python package to automatically repost content from Instagram to Twitter
 
-.. |.InstaTweet| replace:: ``InstaTweet``
-.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L5-L142
-.. |.add_users| replace:: ``add_users()``
-.. _.add_users: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L167-L197
-.. |.Profile| replace:: ``Profile``
-.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L12-L416
-.. |.start| replace:: ``start()``
-.. _.start: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L72-L117
-.. |.InstaClient| replace:: ``InstaClient``
-.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instaclient.py#L14-L108
+.. |.InstaTweet| replace:: InstaTweet
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-L147
+.. |.add_pages| replace:: add_pages()
+.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165
+.. |.Profile| replace:: Profile
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382
+.. |.start| replace:: start()
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L71-L121
+.. |.InstaClient| replace:: InstaClient
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instaclient.py#L16-L159
 .. |mandatory-settings| replace:: mandatory settings
 .. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
 
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
@@ -86,30 +86,30 @@
 What's InstaTweet?
 ~~~~~~~~~~~~~~~~~~~~~
 
 |.InstaTweet|_ is a customizable tool to automatically repost content from Instagram to Twitter.
 
 
 
-Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_users|_ to repost from
+Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_pages|_ to repost from
 
 
 .. code-block:: python
 
     from InstaTweet import Profile
 
     # Create a new (local) Profile
     >>> profile = Profile('myProfile')
 
     # Configure the mandatory settings (at minimum)
     >>> profile.twitter_keys = twitter_api_keys
     >>> profile.session_id = '6011991A'
 
-    # Add at least one Instagram account to repost from
-    >>> profile.add_users('the.dailykitten')
+    # Add at least one Instagram page (user/hashtag) to repost from
+    >>> profile.add_pages(['the.dailykitten', '#thedailykitten'])
 
     # Save the Profile [optional]
     >>> profile.save()
 
     Saved Local Profile myProfile
 
 
@@ -127,27 +127,30 @@
 
     # Run InstaTweet by calling start()
     >>> insta_tweet.start()
 
 
 |
 
-.. image:: https://user-images.githubusercontent.com/96394652/232274766-71e87fb2-f402-466d-9624-f775d8e985ac.png
+.. image:: https://user-images.githubusercontent.com/96394652/236979506-83d12d6f-114d-43ce-b4db-b062f8d0ed3a.png
+   :width: 700px
 
 |
 
 As ``InstaTweet`` runs, its progress will be logged to console:
 
 .. code-block:: python
 
     Starting InstaTweet for Profile: myProfile
     Checking posts from @the.dailykitten
-    
-    Finished insta-tweeting for @the.dailykitten
-    All users have been insta-tweeted
+    ...
+    Checking posts from #thedailykitten
+    ...
+    Finished insta-tweeting for #thedailykitten
+    All pages have been insta-tweeted
 
 ...
 
 Okay... But Why? 😟
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
@@ -176,24 +179,30 @@
 The package's custom |.InstaClient|_ can also be used as a standalone Instagram scraper
 
 .. code-block:: python
 
    from InstaTweet import InstaClient
 
    >>> ig = InstaClient(session_id="kjfdn309wredsfl")
+
+   # Scrape Instagram user or hashtag
    >>> user = ig.get_user('dailykittenig')
-   >>> print(user)
+   >>> hashtag = ig.get_hashtag('#dailykitten')
+   >>> print(user, hashtag, sep='\n')
 
-   <InstaTweet.instauser.InstaUser object at 0x000002B9A1101330>
+   Instagram User: @dailykittenig
+   Instagram Hashtag: #dailykitten
 
-   >>> print(user.posts)
-   >>> ig.download_post(user.posts[0])
+   # Download most recent post
+   >>> post = user.posts[0]
+   >>> print(post)
+   >>> ig.download_post(post)
 
-   [<InstaTweet.instapost.InstaPost object at 0x000002B9A250F5E0>, ...]
-   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\\path\\to\\insta-tweet\\downloads\\2981866202934977614.mp4
+   Post 2981866202934977614 by @dailykittenig on 2022-11-29 01:44:37
+   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\path\to\insta-tweet\downloads\2981866202934977614.mp4
 
 ...
 
 Installation
 ~~~~~~~~~~~~~~
 
 To install using pip:
```

### Comparing `insta-tweet-2.1.3/README.rst` & `insta-tweet-2.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .. meta::
    :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
    :description: A Python package to automatically repost content from Instagram to Twitter
 
 .. |.InstaTweet| replace:: ``InstaTweet``
-.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L5-L142
-.. |.add_users| replace:: ``add_users()``
-.. _.add_users: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L167-L197
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-L147
+.. |.add_pages| replace:: ``add_pages()``
+.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165
 .. |.Profile| replace:: ``Profile``
-.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L12-L416
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382
 .. |.start| replace:: ``start()``
-.. _.start: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L72-L117
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L71-L121
 .. |.InstaClient| replace:: ``InstaClient``
-.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instaclient.py#L14-L108
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instaclient.py#L16-L159
 .. |mandatory-settings| replace:: mandatory settings
 .. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
 
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
@@ -82,32 +82,32 @@
 What's InstaTweet?
 ~~~~~~~~~~~~~~~~~~~~~
 
 |.InstaTweet|_ is a customizable tool to automatically repost content from Instagram to Twitter.
 
 
 
-Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_users|_ to repost from
+Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_pages|_ to repost from
 
 
 .. code-block:: python
 
     from InstaTweet import Profile
 
     # Create a new (local) Profile
     >>> profile = Profile('myProfile')
 
     # Configure the mandatory settings (at minimum)
     >>> profile.twitter_keys = twitter_api_keys
     >>> profile.session_id = '6011991A'
 
-    # Add at least one Instagram account to repost from
-    >>> profile.add_users('the.dailykitten')
+    # Add at least one Instagram page (user/hashtag) to repost from
+    >>> profile.add_pages(['the.dailykitten', '#thedailykitten'])
 
-    # Save the Profile [optional]
+     # Save the Profile [optional]
     >>> profile.save()
 
     Saved Local Profile myProfile
 
 
 Once configured, the |.Profile|_ can be used to initialize and |.start|_ InstaTweet:
 
@@ -123,27 +123,30 @@
 
     # Run InstaTweet by calling start()
     >>> insta_tweet.start()
 
 
 |
 
-.. image:: https://user-images.githubusercontent.com/96394652/232274766-71e87fb2-f402-466d-9624-f775d8e985ac.png
+.. image:: https://user-images.githubusercontent.com/96394652/236979506-83d12d6f-114d-43ce-b4db-b062f8d0ed3a.png
+   :width: 700px
 
 |
 
 As ``InstaTweet`` runs, its progress will be logged to console:
 
 .. code-block:: python
 
     Starting InstaTweet for Profile: myProfile
     Checking posts from @the.dailykitten
-    
-    Finished insta-tweeting for @the.dailykitten
-    All users have been insta-tweeted
+    ...
+    Checking posts from #thedailykitten
+    ...
+    Finished insta-tweeting for #thedailykitten
+    All pages have been insta-tweeted
 
 ...
 
 Okay... But Why? 😟
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 .. raw:: html
@@ -154,17 +157,17 @@
       </tr>
       <tr>
          <td>
 
 **InstaTweet has two main use cases:**
 
 * To automatically share your own Instagram posts to Twitter
-* To automatically tweet new content from other Instagram users
+* To automatically tweet new content from other Instagram users/hashtags
 
-Regardless of your intention, InstaTweet will detect new posts from the users you specify,
+Regardless of your intention, InstaTweet will detect new posts from the pages you specify,
 download them, and repost them to Twitter.
 
 .. raw:: html
 
    </td></tr>
    </table>
 
@@ -178,24 +181,30 @@
 The package's custom |.InstaClient|_ can also be used as a standalone Instagram scraper
 
 .. code-block:: python
 
    from InstaTweet import InstaClient
 
    >>> ig = InstaClient(session_id="kjfdn309wredsfl")
+
+   # Scrape Instagram user or hashtag
    >>> user = ig.get_user('dailykittenig')
-   >>> print(user)
+   >>> hashtag = ig.get_hashtag('#dailykitten')
+   >>> print(user, hashtag, sep='\n')
 
-   <InstaTweet.instauser.InstaUser object at 0x000002B9A1101330>
+   Instagram User: @dailykittenig
+   Instagram Hashtag: #dailykitten
 
-   >>> print(user.posts)
-   >>> ig.download_post(user.posts[0])
+   # Download most recent post
+   >>> post = user.posts[0]
+   >>> print(post)
+   >>> ig.download_post(post)
 
-   [<InstaTweet.instapost.InstaPost object at 0x000002B9A250F5E0>, ...]
-   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\\path\\to\\insta-tweet\\downloads\\2981866202934977614.mp4
+   Post 2981866202934977614 by @dailykittenig on 2022-11-29 01:44:37
+   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\path\to\insta-tweet\downloads\2981866202934977614.mp4
 
 ...
 
 Installation
 ~~~~~~~~~~~~~~
 
 To install using pip:
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 .. meta:: :title: InstaTweet - Automatically Repost Content From Instagram to
 Twitter :description: A Python package to automatically repost content from
 Instagram to Twitter .. |.InstaTweet| replace:: ``InstaTweet`` .. _.InstaTweet:
-https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L5-
-L142 .. |.add_users| replace:: ``add_users()`` .. _.add_users: https://
-github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L167-L197 ..
+https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-
+L147 .. |.add_pages| replace:: ``add_pages()`` .. _.add_pages: https://
+github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165 ..
 |.Profile| replace:: ``Profile`` .. _.Profile: https://github.com/tdkorn/insta-
-tweet/blob/master/InstaTweet/profile.py#L12-L416 .. |.start| replace:: ``start
-()`` .. _.start: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/
-instatweet.py#L72-L117 .. |.InstaClient| replace:: ``InstaClient`` ..
-_.InstaClient: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/
-instaclient.py#L14-L108 .. |mandatory-settings| replace:: mandatory settings ..
+tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382 .. |.start| replace:: ``start
+()`` .. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/
+instatweet.py#L71-L121 .. |.InstaClient| replace:: ``InstaClient`` ..
+_.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/
+instaclient.py#L16-L159 .. |mandatory-settings| replace:: mandatory settings ..
 _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/
 getting-started.html#mandatory-settings .. _about-insta-tweet: â¨ð¥
 InstaTweet ð¤â¨ ----------------------- .. image:: https://img.shields.io/
 pypi/v/insta-tweet :target: https://pypi.org/project/insta-tweet/ :alt: PyPI
 Version .. image:: https://img.shields.io/badge/GitHub-insta--tweet-4f1abc :
 target: https://github.com/tdkorn/insta-tweet :alt: GitHub Repository ..
 image:: https://static.pepy.tech/personalized-badge/insta-
@@ -35,47 +35,50 @@
 share_with_instatweet.png :alt: Sharing an Instagram post to Twitter using
 InstaTweet. The actual photo or video appears in the tweet. It's a thicc cat,
 very handsome. Nobody will click the link, but they'll definitely see this bad
 boy. With ``InstaTweet``, you can rest easy knowing that, although nobody will
 click the link, they'll at least see what you posted. ... What's InstaTweet?
 ~~~~~~~~~~~~~~~~~~~~~ |.InstaTweet|_ is a customizable tool to automatically
 repost content from Instagram to Twitter. Simply create a |.Profile|_,
-configure the |mandatory-settings|_, and |.add_users|_ to repost from .. code-
+configure the |mandatory-settings|_, and |.add_pages|_ to repost from .. code-
 block:: python from InstaTweet import Profile # Create a new (local) Profile
 >>> profile = Profile('myProfile') # Configure the mandatory settings (at
 minimum) >>> profile.twitter_keys = twitter_api_keys >>> profile.session_id =
-'6011991A' # Add at least one Instagram account to repost from >>>
-profile.add_users('the.dailykitten') # Save the Profile [optional] >>>
-profile.save() Saved Local Profile myProfile Once configured, the |.Profile|_
-can be used to initialize and |.start|_ InstaTweet: .. code-block:: python from
-InstaTweet import InstaTweet # Directly initialize with a Profile object >>>
-insta_tweet = InstaTweet(profile) # Or load a saved Profile by name >>>
-insta_tweet = InstaTweet.load("myProfile") # Run InstaTweet by calling start()
->>> insta_tweet.start() | .. image:: https://user-images.githubusercontent.com/
-96394652/232274766-71e87fb2-f402-466d-9624-f775d8e985ac.png | As ``InstaTweet``
-runs, its progress will be logged to console: .. code-block:: python Starting
-InstaTweet for Profile: myProfile Checking posts from @the.dailykitten Finished
-insta-tweeting for @the.dailykitten All users have been insta-tweeted ...
-Okay... But Why? ð ~~~~~~~~~~~~~~~~~~~~~~~ .. raw:: html
+'6011991A' # Add at least one Instagram page (user/hashtag) to repost from >>>
+profile.add_pages(['the.dailykitten', '#thedailykitten']) # Save the Profile
+[optional] >>> profile.save() Saved Local Profile myProfile Once configured,
+the |.Profile|_ can be used to initialize and |.start|_ InstaTweet: .. code-
+block:: python from InstaTweet import InstaTweet # Directly initialize with a
+Profile object >>> insta_tweet = InstaTweet(profile) # Or load a saved Profile
+by name >>> insta_tweet = InstaTweet.load("myProfile") # Run InstaTweet by
+calling start() >>> insta_tweet.start() | .. image:: https://user-
+images.githubusercontent.com/96394652/236979506-83d12d6f-114d-43ce-b4db-
+b062f8d0ed3a.png :width: 700px | As ``InstaTweet`` runs, its progress will be
+logged to console: .. code-block:: python Starting InstaTweet for Profile:
+myProfile Checking posts from @the.dailykitten ... Checking posts from
+#thedailykitten ... Finished insta-tweeting for #thedailykitten All pages have
+been insta-tweeted ... Okay... But Why? ð ~~~~~~~~~~~~~~~~~~~~~~~ .. raw::
+html
 ð¥ But Why? ð¤¨
 **InstaTweet has two main use cases:** * To automatically share your own
 Instagram posts to Twitter * To automatically tweet new content from other
-Instagram users Regardless of your intention, InstaTweet will detect new posts
-from the users you specify, download them, and repost them to Twitter. .. raw::
-html
+Instagram users/hashtags Regardless of your intention, InstaTweet will detect
+new posts from the pages you specify, download them, and repost them to
+Twitter. .. raw:: html
 ... Other Use Case: The |.InstaClient|_ ======================================
 The package's custom |.InstaClient|_ can also be used as a standalone Instagram
 scraper .. code-block:: python from InstaTweet import InstaClient >>> ig =
-InstaClient(session_id="kjfdn309wredsfl") >>> user = ig.get_user
-('dailykittenig') >>> print(user)
-instauser.InstaUser object at 0x000002B9A1101330> >>> print(user.posts) >>>
-ig.download_post(user.posts[0]) [
-instapost.InstaPost object at 0x000002B9A250F5E0>, ...] Downloaded post https:/
-/www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\\path\\to\\insta-
-tweet\\downloads\\2981866202934977614.mp4 ... Installation ~~~~~~~~~~~~~~ To
+InstaClient(session_id="kjfdn309wredsfl") # Scrape Instagram user or hashtag
+>>> user = ig.get_user('dailykittenig') >>> hashtag = ig.get_hashtag
+('#dailykitten') >>> print(user, hashtag, sep='\n') Instagram User:
+@dailykittenig Instagram Hashtag: #dailykitten # Download most recent post >>>
+post = user.posts[0] >>> print(post) >>> ig.download_post(post) Post
+2981866202934977614 by @dailykittenig on 2022-11-29 01:44:37 Downloaded post
+https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\path\to\insta-
+tweet\downloads\2981866202934977614.mp4 ... Installation ~~~~~~~~~~~~~~ To
 install using pip: .. code-block:: shell pip install insta-tweet Please note
 that ``InstaTweet`` requires ``Python >= 3.8`` ... Documentation
 ~~~~~~~~~~~~~~~~~ The rest of this `README
 instatweet.readthedocs.io/en/latest/_readme/getting-started.html>`_, the `API
 documentation
 instatweet.readthedocs.io/en/latest/modules.html>`_, and `snippets
 instatweet.readthedocs.io/en/latest/snippets.html>`_ can all be found on `Read
```

### Comparing `insta-tweet-2.1.3/insta_tweet.egg-info/PKG-INFO` & `insta-tweet-2.2.0/insta_tweet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insta-tweet
-Version: 2.1.3
+Version: 2.2.0
 Summary: Automatically Repost Content From Instagram to Twitter
 Home-page: https://www.github.com/TDKorn/insta-tweet/
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT
 Download-URL: https://github.com/TDKorn/insta-tweet/tarball/master/
 Keywords: instagram,twitter,api,instagram api,twitter api,repost,instagram repost,reposter
@@ -12,24 +12,24 @@
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. meta::
    :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
    :description: A Python package to automatically repost content from Instagram to Twitter
 
-.. |.InstaTweet| replace:: ``InstaTweet``
-.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L5-L142
-.. |.add_users| replace:: ``add_users()``
-.. _.add_users: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L167-L197
-.. |.Profile| replace:: ``Profile``
-.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L12-L416
-.. |.start| replace:: ``start()``
-.. _.start: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L72-L117
-.. |.InstaClient| replace:: ``InstaClient``
-.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instaclient.py#L14-L108
+.. |.InstaTweet| replace:: InstaTweet
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-L147
+.. |.add_pages| replace:: add_pages()
+.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165
+.. |.Profile| replace:: Profile
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382
+.. |.start| replace:: start()
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L71-L121
+.. |.InstaClient| replace:: InstaClient
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instaclient.py#L16-L159
 .. |mandatory-settings| replace:: mandatory settings
 .. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
 
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
@@ -86,30 +86,30 @@
 What's InstaTweet?
 ~~~~~~~~~~~~~~~~~~~~~
 
 |.InstaTweet|_ is a customizable tool to automatically repost content from Instagram to Twitter.
 
 
 
-Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_users|_ to repost from
+Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_pages|_ to repost from
 
 
 .. code-block:: python
 
     from InstaTweet import Profile
 
     # Create a new (local) Profile
     >>> profile = Profile('myProfile')
 
     # Configure the mandatory settings (at minimum)
     >>> profile.twitter_keys = twitter_api_keys
     >>> profile.session_id = '6011991A'
 
-    # Add at least one Instagram account to repost from
-    >>> profile.add_users('the.dailykitten')
+    # Add at least one Instagram page (user/hashtag) to repost from
+    >>> profile.add_pages(['the.dailykitten', '#thedailykitten'])
 
     # Save the Profile [optional]
     >>> profile.save()
 
     Saved Local Profile myProfile
 
 
@@ -127,27 +127,30 @@
 
     # Run InstaTweet by calling start()
     >>> insta_tweet.start()
 
 
 |
 
-.. image:: https://user-images.githubusercontent.com/96394652/232274766-71e87fb2-f402-466d-9624-f775d8e985ac.png
+.. image:: https://user-images.githubusercontent.com/96394652/236979506-83d12d6f-114d-43ce-b4db-b062f8d0ed3a.png
+   :width: 700px
 
 |
 
 As ``InstaTweet`` runs, its progress will be logged to console:
 
 .. code-block:: python
 
     Starting InstaTweet for Profile: myProfile
     Checking posts from @the.dailykitten
-    
-    Finished insta-tweeting for @the.dailykitten
-    All users have been insta-tweeted
+    ...
+    Checking posts from #thedailykitten
+    ...
+    Finished insta-tweeting for #thedailykitten
+    All pages have been insta-tweeted
 
 ...
 
 Okay... But Why? 😟
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
@@ -176,24 +179,30 @@
 The package's custom |.InstaClient|_ can also be used as a standalone Instagram scraper
 
 .. code-block:: python
 
    from InstaTweet import InstaClient
 
    >>> ig = InstaClient(session_id="kjfdn309wredsfl")
+
+   # Scrape Instagram user or hashtag
    >>> user = ig.get_user('dailykittenig')
-   >>> print(user)
+   >>> hashtag = ig.get_hashtag('#dailykitten')
+   >>> print(user, hashtag, sep='\n')
 
-   <InstaTweet.instauser.InstaUser object at 0x000002B9A1101330>
+   Instagram User: @dailykittenig
+   Instagram Hashtag: #dailykitten
 
-   >>> print(user.posts)
-   >>> ig.download_post(user.posts[0])
+   # Download most recent post
+   >>> post = user.posts[0]
+   >>> print(post)
+   >>> ig.download_post(post)
 
-   [<InstaTweet.instapost.InstaPost object at 0x000002B9A250F5E0>, ...]
-   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\\path\\to\\insta-tweet\\downloads\\2981866202934977614.mp4
+   Post 2981866202934977614 by @dailykittenig on 2022-11-29 01:44:37
+   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\path\to\insta-tweet\downloads\2981866202934977614.mp4
 
 ...
 
 Installation
 ~~~~~~~~~~~~~~
 
 To install using pip:
```

### Comparing `insta-tweet-2.1.3/setup.py` & `insta-tweet-2.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 import os
-import re
+from pathlib import Path
 from setuptools import setup
 
-
 LONG_DESCRIPTION_SRC = 'README_PyPi.rst'
 
 
 def read(file):
     with open(os.path.abspath(file), 'r', encoding='utf-8') as f:
         return f.read()
 
 
-def get_pypi_desc(rst_file=LONG_DESCRIPTION_SRC):
-    rst = read(rst_file)
-    # Replace the "From the Docs..." rst admonition with a screenshot of it
-    docs_admonition_regex = r'.. admonition:: From the Docs\.\.\.[\w\W]+https.+\n{3}'
-    docs_admonition_img = ".. image:: {}".format(
-        "https://user-images.githubusercontent.com/96394652/187158617-f45761ab-3aa9-472f-a6fb-a99cd0ce900c.png\n\n\n"
-    )
-    return re.sub(
-        pattern=docs_admonition_regex,
-        repl=docs_admonition_img,
-        string=rst
-    )
+# Parse version
+init = Path(__file__).parent.joinpath("InstaTweet", "__init__.py")
+for line in init.read_text().split("\n"):
+    if line.startswith("__version__ ="):
+        break
+version = line.split(" = ")[-1].strip('"')
 
 
 setup(
     name='insta-tweet',
     packages=['InstaTweet'],
-    version='2.1.3',
+    version=version,
     license='MIT',
     description='Automatically Repost Content From Instagram to Twitter',
-    long_description=get_pypi_desc(LONG_DESCRIPTION_SRC),
+    long_description=read(LONG_DESCRIPTION_SRC),
     long_description_content_type="text/x-rst; charset=UTF-8",
     author='Adam Korn',
     author_email='hello@dailykitten.net',
     url='https://www.github.com/TDKorn/insta-tweet/',
     download_url=f"https://github.com/TDKorn/insta-tweet/tarball/master/",
     keywords=['instagram', 'twitter', 'api', 'instagram api', 'twitter api', 'repost', 'instagram repost', 'reposter'],
     install_requires=[
```

