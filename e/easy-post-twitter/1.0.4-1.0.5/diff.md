# Comparing `tmp/easy_post_twitter-1.0.4.tar.gz` & `tmp/easy_post_twitter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_post_twitter-1.0.4.tar", max compression
+gzip compressed data, was "easy_post_twitter-1.0.5.tar", max compression
```

## Comparing `easy_post_twitter-1.0.4.tar` & `easy_post_twitter-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       22 2022-09-23 19:06:20.507819 easy_post_twitter-1.0.4/easy_post_twitter/__init__.py
--rw-r--r--   0        0        0     8984 2022-09-23 19:06:20.511819 easy_post_twitter-1.0.4/easy_post_twitter/twitter.py
--rw-r--r--   0        0        0      415 2022-09-23 19:06:20.515819 easy_post_twitter-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      706 2022-09-23 19:07:29.146553 easy_post_twitter-1.0.4/setup.py
--rw-r--r--   0        0        0      523 2022-09-23 19:07:29.146691 easy_post_twitter-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.5/easy_post_twitter/__init__.py
+-rw-r--r--   0        0        0     9345 2023-05-09 13:46:49.905237 easy_post_twitter-1.0.5/easy_post_twitter/twitter.py
+-rw-r--r--   0        0        0      415 2023-05-09 21:43:16.746278 easy_post_twitter-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.5/PKG-INFO
```

### Comparing `easy_post_twitter-1.0.4/easy_post_twitter/twitter.py` & `easy_post_twitter-1.0.5/easy_post_twitter/twitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,13 +189,21 @@
             try:
                 client = self.__get_client()
                 response = client.create_tweet(text=text)
                 log.info(f'Tweet created successfully. ID: {response.data["id"]}')
             except Exception as e:
                 log.error(f'Error creating tweet. Error: {e}')
 
+    def tweetItNow(self, text):
+        '''Tweet the "text" and do not ask questions'''
+        client = self.__get_client()
+        try:
+            response = client.create_tweet(text=text)
+            log.info(f'Tweet created successfully. ID: {response.data["id"]}')
+        except Exception as e:
+            log.error(f'Error creating tweet. Error: {e}')
 
 if __name__ == '__main__':
     img = '/home/drakon/Documents/DEV/projetos/easy_post_twitter/imgs/market1.png'
     tw = Twitter(with_images=True)
     status = 'B3 interbank deposit futures: today and a month ago #FuturodoCDI #mercadofinanceiro'
     tw.tweet_to_publish_with_image(text=status, imgs=img, sequential=False)
```

### Comparing `easy_post_twitter-1.0.4/PKG-INFO` & `easy_post_twitter-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: easy-post-twitter
-Version: 1.0.4
+Version: 1.0.5
 Summary: The easy way to send posts to twitter.
 Author: Thiago Oliveira
 Author-email: thiceconelo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: tweepy (>=4.10.0,<5.0.0)
```

