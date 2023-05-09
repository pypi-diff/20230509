# Comparing `tmp/mastoposter-0.tar.gz` & `tmp/mastoposter-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastoposter-0.tar", last modified: Mon May  8 14:39:24 2023, max compression
+gzip compressed data, was "mastoposter-0.1.tar", last modified: Tue May  9 15:46:50 2023, max compression
```

## Comparing `mastoposter-0.tar` & `mastoposter-0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       42 2022-10-11 06:28:03.114718 mastoposter-0/.dockerignore
--rw-r--r--   0        0        0       70 2023-05-08 14:36:21.120748 mastoposter-0/.gitignore
--rw-r--r--   0        0        0      219 2022-10-11 06:28:03.114718 mastoposter-0/Dockerfile
--rw-r--r--   0        0        0    35149 2023-05-08 06:11:58.353055 mastoposter-0/LICENSE
--rw-r--r--   0        0        0     9394 2022-11-02 17:33:52.424775 mastoposter-0/README.md
--rw-r--r--   0        0        0     5096 2023-03-05 06:02:37.750142 mastoposter-0/config.ini
--rw-r--r--   0        0        0     3072 2023-05-08 14:26:31.327193 mastoposter-0/mastoposter/__init__.py
--rw-r--r--   0        0        0     4468 2023-05-08 14:26:31.327193 mastoposter-0/mastoposter/__main__.py
--rw-r--r--   0        0        0     1798 2023-05-08 06:42:00.510026 mastoposter-0/mastoposter/filters/__init__.py
--rw-r--r--   0        0        0     2676 2023-05-08 06:42:00.503360 mastoposter-0/mastoposter/filters/base.py
--rw-r--r--   0        0        0     1661 2023-05-08 06:42:00.470026 mastoposter-0/mastoposter/filters/boost.py
--rw-r--r--   0        0        0     2431 2023-05-08 06:42:00.450026 mastoposter-0/mastoposter/filters/combined.py
--rw-r--r--   0        0        0     2090 2023-05-08 06:42:00.463360 mastoposter-0/mastoposter/filters/media.py
--rw-r--r--   0        0        0     1946 2023-05-08 06:42:00.480026 mastoposter-0/mastoposter/filters/mention.py
--rw-r--r--   0        0        0     1411 2023-05-08 06:42:00.456693 mastoposter-0/mastoposter/filters/spoiler.py
--rw-r--r--   0        0        0     2493 2023-05-08 06:42:00.486693 mastoposter-0/mastoposter/filters/text.py
--rw-r--r--   0        0        0     1266 2023-05-08 06:42:00.496693 mastoposter-0/mastoposter/filters/visibility.py
--rw-r--r--   0        0        0      967 2023-05-08 06:42:00.416693 mastoposter-0/mastoposter/integrations/__init__.py
--rw-r--r--   0        0        0     1113 2023-05-08 06:42:00.403360 mastoposter-0/mastoposter/integrations/base.py
--rw-r--r--   0        0        0     4021 2023-05-08 06:42:00.390026 mastoposter-0/mastoposter/integrations/discord/__init__.py
--rw-r--r--   0        0        0     2535 2023-05-08 06:42:00.396693 mastoposter-0/mastoposter/integrations/discord/types.py
--rw-r--r--   0        0        0     9834 2023-05-08 06:42:00.410026 mastoposter-0/mastoposter/integrations/telegram.py
--rw-r--r--   0        0        0     2236 2023-05-08 06:42:00.423359 mastoposter-0/mastoposter/sources.py
--rw-r--r--   0        0        0    10407 2023-05-08 14:35:13.060296 mastoposter-0/mastoposter/types.py
--rw-r--r--   0        0        0     8032 2023-05-08 10:18:26.016056 mastoposter-0/mastoposter/utils.py
--rw-r--r--   0        0        0      882 2023-05-08 14:26:31.327193 mastoposter-0/pyproject.toml
--rw-r--r--   0        0        0      246 2022-11-05 08:05:19.598221 mastoposter-0/requirements.txt
--rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 mastoposter-0/PKG-INFO
+-rw-r--r--   0        0        0       42 2022-10-11 06:28:03.114718 mastoposter-0.1/.dockerignore
+-rw-r--r--   0        0        0       70 2023-05-08 15:04:53.166981 mastoposter-0.1/.gitignore
+-rw-r--r--   0        0        0      219 2022-10-11 06:28:03.114718 mastoposter-0.1/Dockerfile
+-rw-r--r--   0        0        0    35149 2023-05-08 15:04:53.166981 mastoposter-0.1/LICENSE
+-rw-r--r--   0        0        0    10101 2023-05-08 15:04:53.166981 mastoposter-0.1/README.md
+-rw-r--r--   0        0        0     5096 2023-03-05 06:02:37.750142 mastoposter-0.1/config.ini
+-rw-r--r--   0        0        0     3074 2023-05-09 15:46:11.877142 mastoposter-0.1/mastoposter/__init__.py
+-rw-r--r--   0        0        0     4468 2023-05-08 15:04:53.166981 mastoposter-0.1/mastoposter/__main__.py
+-rw-r--r--   0        0        0     1798 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/__init__.py
+-rw-r--r--   0        0        0     2676 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/base.py
+-rw-r--r--   0        0        0     1661 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/boost.py
+-rw-r--r--   0        0        0     2431 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/combined.py
+-rw-r--r--   0        0        0     2090 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/media.py
+-rw-r--r--   0        0        0     1946 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/mention.py
+-rw-r--r--   0        0        0     1411 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/spoiler.py
+-rw-r--r--   0        0        0     2493 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/text.py
+-rw-r--r--   0        0        0     1266 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/visibility.py
+-rw-r--r--   0        0        0      967 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/__init__.py
+-rw-r--r--   0        0        0     1113 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/base.py
+-rw-r--r--   0        0        0     4021 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/discord/__init__.py
+-rw-r--r--   0        0        0     2535 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/discord/types.py
+-rw-r--r--   0        0        0     9834 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/telegram.py
+-rw-r--r--   0        0        0     2236 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/sources.py
+-rw-r--r--   0        0        0    10407 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/types.py
+-rw-r--r--   0        0        0     8486 2023-05-09 15:42:36.239241 mastoposter-0.1/mastoposter/utils.py
+-rw-r--r--   0        0        0      882 2023-05-08 15:04:53.170314 mastoposter-0.1/pyproject.toml
+-rw-r--r--   0        0        0      246 2022-11-05 08:05:19.598221 mastoposter-0.1/requirements.txt
+-rw-r--r--   0        0        0    10842 1970-01-01 00:00:00.000000 mastoposter-0.1/PKG-INFO
```

### Comparing `mastoposter-0/LICENSE` & `mastoposter-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mastoposter-0/README.md` & `mastoposter-0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,48 @@
-# mastoposter - easy-to-use mastodon-to-[everything] reposter!
+# mastoposter - easy-to-use mastodon-to-[everything] reposter
 
 Mastoposter is a simple zero-headache* service that forwards your toots from any
-Mastodon-compatible Fediverse software (Pleroma also works!) to any of your
+Mastodon-compatible Fediverse software (Pleroma also works\*\*!) to any of your
 other services! For now it supports only Discord webhooks and Telegram, but it
 can be easily extended to support pretty much anything!
 
 ## Installation
 
+### Via pip
+
+Since recently we have package published to pip (thanks to
+[@cybertailor@deadinsi.de](https://deadinsi.de/@cybertailor) for adding
+pyproject file), so now you can just do the following:
+
+```sh
+pip install mastoposter
+```
+
+Note that you would still have to clone repository to build a Docker image.
+
+### Old way
+
 You can run it either on your host machine, or inside a Docker container.
 In any case, you have to clone that repo first in order to do anything:
+
 ```sh
 git clone https://github.com/hatkidchan/mastoposter && cd mastoposter
 ```
 
 After that, you can either run it in Docker, set up a standalone systemd
 service, or just run it as it is!
 
-### Docker:
+### Docker
 
 ```sh
 docker build -t mastoposter .
-docker run --restart=always -dv /path/to/config.ini:/config.ini:ro --name mastoposter mastoposter
+docker run -d \
+    --restart=unless-stopped \
+    -v /path/to/config.ini:/config.ini:ro \
+    --name mastoposter mastoposter
 ```
 
 And you should be good to go
 
 ### Systemd
 
 Let's say that you've cloned that repo to the `$MASTOPOSTER_ROOT`, then
@@ -42,205 +60,233 @@
 WorkingDirectory=$MASTOPOSTER_ROOT
 Restart=on-failure
 
 [Install]
 WantedBy=network.target
 ```
 
-Before running it though, don't forget to install dependencies from the 
+Before running it though, don't forget to install dependencies from the
 ./requirements.txt, but it's a good idea to use a virtual environment for that.
 Though, that's outside of the scope of that, so I won't cover it here.
 
 ### Running manually
+
 Just be in the folder with it, have dependencies installed and run:
+
+```sh
 python3 -m mastoposter config.ini
+```
 
 ## Configuration
 
 Configuration file is just a regular INI file with a couple sections.
 
+Configuration wizard is still in progress, but we have a couple examples for
+common use-cases. If you have troubles configuring it yourself, you could
+either use discussions feature, or ask me on Fedi directly (links on profile).
+
 ### [main]
+
 Section `main` contains settings of your account (ie, your instance, list ID,
 user ID, access token), as well as list of modules to load.
 
 #### instance
+
 This is your instance. It should be written without the `https://` part, so,
 for example, `mastodon.social`.
 
 #### token
+
 This is your access token.
 
 On Mastodon, you can acquire it by creating an application with the minimum of
 `read:statuses` and `read:lists` permissions.
 
 On Pleroma you're out of luck and have to manually lure your token out of the
 frontend you're using. For example, in Pleroma FE you can look in the "Network"
 tab of the devtools and look for `chats` request. Inside the request headers,
 there should be `Authorization: Bearer XXXXXXXXXXX` header. That's your token.
 
 #### user
+
 It's still not properly tested, but you could just leave it as `auto` for now.
 
 In case it fails, on Mastodon you can get your user ID by looking at your
 profile picture URL. The part between "/avatars/" and "original/" without all of
 the slashes is your user ID.
 
 On Pleroma you're out of luck again, I don't remember how I got mine. Just hope
 that "auto" will work, lol.
 
 #### list
+
 That's the main problem of this crossposter: it requires a list to be created
 to function properly. Both Pleroma and Mastodon support them, so it shouldn't be
 a big deal. Just create a list, add yourself into it and copy its ID (it should
 be in the address bar).
 
 List is required to filter incoming events. You can't just listen for home
 timeline 'cause some events are not guaranteed to be there (boosts at least).
 
 #### auto-reconnect
+
 You can set it to either `yes` or `no`. When set to `yes`, it will reconnect
 on any websocket error, but not on any error related to modules (even if it's a
 connection error!!!)
 
 #### modules
+
 More about them later
 
 #### loglevel
+
 Self-explanatory, logging level. Can be either `DEBUG`, `INFO`, `WARNING` or
 `ERROR`. Defaults to `INFO`
 
 ### Modules
+
 There's two types of modules supported at this point: `telegram` and `discord`.
 Both of them are self-explanatory, but we'll go over them real quick.
 
 Each module should contain at least `type` property and its name should start
 with the `module/`. `filters` field is also can be specified. Check the
 corresponding section to learn more about them.
 
 To use module, add it to the `modules` field in the `main` section. It should
 not have the `module/` prefix since it's always there. You can use multiple
 modules and separate them using spaces.
 
 #### `type = telegram`
+
 Module with that type will work in Telegram mode.
 It requires your Bot token to be set in the `token` field, as well as `chat`
 to be set with your chat ID. You can use `@username` if the chat is public.
 Also there's a `silent` field, when it's set to `true`, it'll set
 `disable_notification` flag on every post sent.
 
 `template` field contains your template for the message. It's pretty much
 Jinja2 template. Since we use `parse_mode=html`, your `template` should be
 formatted appropriately. Template itself has only `status` variable exposed,
 which contains the status/post/toot itself. There's also some handy properties
 such as `reblog_or_status` which points to either reblog, or status itself. Or
 `name_emojiless` which contains the name without emojis. Or `name` which
 contains either `display_name` or `username`, if first one is empty.
 
-
 #### `type = discord`
+
 Module for Discord webhooks. The only required parameter (besides the `type`) is
 `webhook`. It **should** have `wait=true` set. You can also use `thread_id` as a
 GET parameter to that. You also can use filters, nothing special about that.
 
 ### Filters
+
 Filters are the most powerful feature of this crossposter. They allow you to...
 
 Filter out where posts should and shouldn't go! It's that easy!
 
 There's a couple of filters with different types and options, but all of them
 should be contained in sections with names starting with `filter/`, as well
 as have a `type` field with filter type.
 
 Also, you can specify multiple filters and they'll be chained together using
 AND operator. You can also prefix filter name with either `~` or `!` to invert
 its behavior.
 
 #### `type = boost`
+
 Simple filter that passes through posts that are boosted from someone.
 
 It also has an optional `list` property where you can specify the list of
 accounts to check from. You can use globbing, but be aware, that it uses
 `fnmatch` function to glob stuff, so `@*` doesn't mean "any local user", but
 rather it means "any user". NOTE that his behavior is not intended and may be
 changed to more appropriate one later. If `list` is empty, any boost will
 trigger that filter. If list is not empty, it will allow only users from that
 list.
 
 #### `type = mention`
+
 This filter is kinda similar to the `boost` one, but works with mentions.
 Also has `list` property, yada yada you got the idea, same deal with fnmatch.
 
 #### `type = spoiler`
+
 Matches posts with spoilers/content-warnings.
 
 Has an optional `regexp` parameter that will allow you to specify regular
 expression to match your spoiler text.
 
 #### `type = content`
+
 Filter to match post content against either a regular expression, or a list of
 tags. Matching is done on the plaintext version of the post.
 
 You can have one of two properties (but not both because fuck you): `tags` or
 `regexp`. It's obvious what does what: if you have `regexp` set, plaintext
 version of status is checked against that regular expression, and if you have
 `tags` set, then only statuses that have those tags will be allowed.
 
 Please note that in case of tags, you should NOT use `#` symbol in front of
 them.
 
 #### `type = visibility`
+
 Simple filter that just checks for post visibility.
 Has a single property `options` that is a space-separated list of allowed
 visibility levels. Note that `direct` visibility is always ignored so cannot
 be used here.
 
 #### `type = media`
+
 Filter that allows only some media types to be posted.
 
 `valid_media` is a space-separated list of media types from Mastodon API
 (`image`, `gifv`, `video`, `audio` or `unknown`). If your Fedi software has
 support for other types, they also should work.
 
 `mode` option defines the mode of operation: it can be either `include`,
 `exclude` or `only`. In case of `include`, filter will trigger when post
 has media with that type, but others are allowed as well. `exclude` is the
 opposite: if status has media with that type, filter won't trigger. `only`
 allows statuses with either no media, or listed types only.
 
 #### `type = combined`
+
 The most powerful filter 'cause it allows you to combine multiple filters using
 different operations.
 
 `filters` option should contain space-separated list of filters. You also can
 negate them using `!` or `~` prefixes.
 
 `operator` is a type of operation to be used. Can be either `all`, `any` or
 `single`. `all` means that all of the filters should be used. `any` means
 that if any filter is triggered, this one will also trigger. `single` means
 that only one filter should be triggered. Think of it as an XOR operation of
 some sort.
 
 ## Sample configurations
 
-### For Telegram:
+### For Telegram
+
 ```ini
 [main]
 modules = tg
 instance = expired.mentality.rip
 token = haha-no
 list = 42
 user = auto
 
 [module/tg]
 type = telegram
 token = 12345:blahblahblah
 chat = 12345
 ```
 
-### For Telegram with a separate shitpost channel:
+### For Telegram with a separate shitpost channel
+
 ```ini
 [main]
 modules = tg tg-shitpost
 instance = expired.mentality.rip
 token = haha-no
 list = 42
 user = auto
@@ -249,16 +295,21 @@
 type = telegram
 token = 12345:blahblahblah
 chat = 12345
 filters = !shitpost
 
 [module/tg-shitpost]
 type = telegram
-token = 12345:blahblahblah
+token = ${module/tg:token}
 chat = @shitposting
 filters = shitpost
 
 [filters/shitpost]
 type = content
 mode = tag
 tags = shitpost
 ```
+
+## Asterisks
+
+1. Well, most of the time that is.
+2. Works only when it has lists support.
```

### Comparing `mastoposter-0/config.ini` & `mastoposter-0.1/config.ini`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/__init__.py` & `mastoposter-0.1/mastoposter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from mastoposter.integrations import (
     DiscordIntegration,
     FilteredIntegration,
     TelegramIntegration,
 )
 from mastoposter.types import Status
 
-__version__ = "0"
+__version__ = "0.1"
 __description__ = "Mastodon to [anything] reposter"
 
 logger = getLogger()
 
 
 def load_integrations_from(config: ConfigParser) -> List[FilteredIntegration]:
     modules: List[FilteredIntegration] = []
```

### Comparing `mastoposter-0/mastoposter/__main__.py` & `mastoposter-0.1/mastoposter/__main__.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/__init__.py` & `mastoposter-0.1/mastoposter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/base.py` & `mastoposter-0.1/mastoposter/filters/base.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/boost.py` & `mastoposter-0.1/mastoposter/filters/boost.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/combined.py` & `mastoposter-0.1/mastoposter/filters/combined.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/media.py` & `mastoposter-0.1/mastoposter/filters/media.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/mention.py` & `mastoposter-0.1/mastoposter/filters/mention.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/spoiler.py` & `mastoposter-0.1/mastoposter/filters/spoiler.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/text.py` & `mastoposter-0.1/mastoposter/filters/text.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/filters/visibility.py` & `mastoposter-0.1/mastoposter/filters/visibility.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/integrations/__init__.py` & `mastoposter-0.1/mastoposter/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/integrations/base.py` & `mastoposter-0.1/mastoposter/integrations/base.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/integrations/discord/__init__.py` & `mastoposter-0.1/mastoposter/integrations/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/integrations/discord/types.py` & `mastoposter-0.1/mastoposter/integrations/discord/types.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/integrations/telegram.py` & `mastoposter-0.1/mastoposter/integrations/telegram.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/sources.py` & `mastoposter-0.1/mastoposter/sources.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/types.py` & `mastoposter-0.1/mastoposter/types.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0/mastoposter/utils.py` & `mastoposter-0.1/mastoposter/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,22 @@
         ),
         "pre": lambda tag: (
             "\n<pre>%s</pre>\n" % str.join("", map(node_to_html, tag.children))
         ),
         "code": lambda tag: (
             "<code>%s</code>" % str.join("", map(node_to_html, tag.children))
         ),
+        "span": lambda tag: (
+            (
+                '<span class="tg-spoiler">%s</span>'
+                if "_mfm_blur_" in tag.attrs.get("class", "")
+                else "%s"
+            )
+            % str.join("", map(node_to_html, tag.children))
+        ),
         "blockquote": lambda tag: "\n%s"
         % str.join(
             "\n",
             (
                 "| %s" % part
                 for part in str.join(
                     "", map(node_to_html, tag.children)
@@ -173,14 +181,18 @@
         ),
         "pre": lambda tag: (
             "\n``%s``\n" % str.join("", map(node_to_markdown, tag.children))
         ),
         "code": lambda tag: (
             "`%s`" % str.join("", map(node_to_markdown, tag.children))
         ),
+        "span": lambda tag: (
+            ("||%s||" if "_mfm_blur_" in tag.attrs.get("class", "") else "%s")
+            % str.join("", map(node_to_markdown, tag.children))
+        ),
         "blockquote": lambda tag: (
             "\n%s"
             % str.join(
                 "\n",
                 (
                     "▍%s" % part
                     for part in str.join(
```

### Comparing `mastoposter-0/pyproject.toml` & `mastoposter-0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mastoposter-0/PKG-INFO` & `mastoposter-0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastoposter
-Version: 0
+Version: 0.1
 Summary: mastoposter - configurable reposter from Mastodon-compatible Fediverse servers
 Keywords: mastodon,discord,telegram
 Author-email: hatkidchan <hatkidchan@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
@@ -14,37 +14,55 @@
 Requires-Dist: Jinja2
 Requires-Dist: beautifulsoup4
 Requires-Dist: emoji
 Requires-Dist: httpx
 Requires-Dist: websockets
 Project-URL: Source, https://github.com/hatkidchan/mastoposter
 
-# mastoposter - easy-to-use mastodon-to-[everything] reposter!
+# mastoposter - easy-to-use mastodon-to-[everything] reposter
 
 Mastoposter is a simple zero-headache* service that forwards your toots from any
-Mastodon-compatible Fediverse software (Pleroma also works!) to any of your
+Mastodon-compatible Fediverse software (Pleroma also works\*\*!) to any of your
 other services! For now it supports only Discord webhooks and Telegram, but it
 can be easily extended to support pretty much anything!
 
 ## Installation
 
+### Via pip
+
+Since recently we have package published to pip (thanks to
+[@cybertailor@deadinsi.de](https://deadinsi.de/@cybertailor) for adding
+pyproject file), so now you can just do the following:
+
+```sh
+pip install mastoposter
+```
+
+Note that you would still have to clone repository to build a Docker image.
+
+### Old way
+
 You can run it either on your host machine, or inside a Docker container.
 In any case, you have to clone that repo first in order to do anything:
+
 ```sh
 git clone https://github.com/hatkidchan/mastoposter && cd mastoposter
 ```
 
 After that, you can either run it in Docker, set up a standalone systemd
 service, or just run it as it is!
 
-### Docker:
+### Docker
 
 ```sh
 docker build -t mastoposter .
-docker run --restart=always -dv /path/to/config.ini:/config.ini:ro --name mastoposter mastoposter
+docker run -d \
+    --restart=unless-stopped \
+    -v /path/to/config.ini:/config.ini:ro \
+    --name mastoposter mastoposter
 ```
 
 And you should be good to go
 
 ### Systemd
 
 Let's say that you've cloned that repo to the `$MASTOPOSTER_ROOT`, then
@@ -62,205 +80,233 @@
 WorkingDirectory=$MASTOPOSTER_ROOT
 Restart=on-failure
 
 [Install]
 WantedBy=network.target
 ```
 
-Before running it though, don't forget to install dependencies from the 
+Before running it though, don't forget to install dependencies from the
 ./requirements.txt, but it's a good idea to use a virtual environment for that.
 Though, that's outside of the scope of that, so I won't cover it here.
 
 ### Running manually
+
 Just be in the folder with it, have dependencies installed and run:
+
+```sh
 python3 -m mastoposter config.ini
+```
 
 ## Configuration
 
 Configuration file is just a regular INI file with a couple sections.
 
+Configuration wizard is still in progress, but we have a couple examples for
+common use-cases. If you have troubles configuring it yourself, you could
+either use discussions feature, or ask me on Fedi directly (links on profile).
+
 ### [main]
+
 Section `main` contains settings of your account (ie, your instance, list ID,
 user ID, access token), as well as list of modules to load.
 
 #### instance
+
 This is your instance. It should be written without the `https://` part, so,
 for example, `mastodon.social`.
 
 #### token
+
 This is your access token.
 
 On Mastodon, you can acquire it by creating an application with the minimum of
 `read:statuses` and `read:lists` permissions.
 
 On Pleroma you're out of luck and have to manually lure your token out of the
 frontend you're using. For example, in Pleroma FE you can look in the "Network"
 tab of the devtools and look for `chats` request. Inside the request headers,
 there should be `Authorization: Bearer XXXXXXXXXXX` header. That's your token.
 
 #### user
+
 It's still not properly tested, but you could just leave it as `auto` for now.
 
 In case it fails, on Mastodon you can get your user ID by looking at your
 profile picture URL. The part between "/avatars/" and "original/" without all of
 the slashes is your user ID.
 
 On Pleroma you're out of luck again, I don't remember how I got mine. Just hope
 that "auto" will work, lol.
 
 #### list
+
 That's the main problem of this crossposter: it requires a list to be created
 to function properly. Both Pleroma and Mastodon support them, so it shouldn't be
 a big deal. Just create a list, add yourself into it and copy its ID (it should
 be in the address bar).
 
 List is required to filter incoming events. You can't just listen for home
 timeline 'cause some events are not guaranteed to be there (boosts at least).
 
 #### auto-reconnect
+
 You can set it to either `yes` or `no`. When set to `yes`, it will reconnect
 on any websocket error, but not on any error related to modules (even if it's a
 connection error!!!)
 
 #### modules
+
 More about them later
 
 #### loglevel
+
 Self-explanatory, logging level. Can be either `DEBUG`, `INFO`, `WARNING` or
 `ERROR`. Defaults to `INFO`
 
 ### Modules
+
 There's two types of modules supported at this point: `telegram` and `discord`.
 Both of them are self-explanatory, but we'll go over them real quick.
 
 Each module should contain at least `type` property and its name should start
 with the `module/`. `filters` field is also can be specified. Check the
 corresponding section to learn more about them.
 
 To use module, add it to the `modules` field in the `main` section. It should
 not have the `module/` prefix since it's always there. You can use multiple
 modules and separate them using spaces.
 
 #### `type = telegram`
+
 Module with that type will work in Telegram mode.
 It requires your Bot token to be set in the `token` field, as well as `chat`
 to be set with your chat ID. You can use `@username` if the chat is public.
 Also there's a `silent` field, when it's set to `true`, it'll set
 `disable_notification` flag on every post sent.
 
 `template` field contains your template for the message. It's pretty much
 Jinja2 template. Since we use `parse_mode=html`, your `template` should be
 formatted appropriately. Template itself has only `status` variable exposed,
 which contains the status/post/toot itself. There's also some handy properties
 such as `reblog_or_status` which points to either reblog, or status itself. Or
 `name_emojiless` which contains the name without emojis. Or `name` which
 contains either `display_name` or `username`, if first one is empty.
 
-
 #### `type = discord`
+
 Module for Discord webhooks. The only required parameter (besides the `type`) is
 `webhook`. It **should** have `wait=true` set. You can also use `thread_id` as a
 GET parameter to that. You also can use filters, nothing special about that.
 
 ### Filters
+
 Filters are the most powerful feature of this crossposter. They allow you to...
 
 Filter out where posts should and shouldn't go! It's that easy!
 
 There's a couple of filters with different types and options, but all of them
 should be contained in sections with names starting with `filter/`, as well
 as have a `type` field with filter type.
 
 Also, you can specify multiple filters and they'll be chained together using
 AND operator. You can also prefix filter name with either `~` or `!` to invert
 its behavior.
 
 #### `type = boost`
+
 Simple filter that passes through posts that are boosted from someone.
 
 It also has an optional `list` property where you can specify the list of
 accounts to check from. You can use globbing, but be aware, that it uses
 `fnmatch` function to glob stuff, so `@*` doesn't mean "any local user", but
 rather it means "any user". NOTE that his behavior is not intended and may be
 changed to more appropriate one later. If `list` is empty, any boost will
 trigger that filter. If list is not empty, it will allow only users from that
 list.
 
 #### `type = mention`
+
 This filter is kinda similar to the `boost` one, but works with mentions.
 Also has `list` property, yada yada you got the idea, same deal with fnmatch.
 
 #### `type = spoiler`
+
 Matches posts with spoilers/content-warnings.
 
 Has an optional `regexp` parameter that will allow you to specify regular
 expression to match your spoiler text.
 
 #### `type = content`
+
 Filter to match post content against either a regular expression, or a list of
 tags. Matching is done on the plaintext version of the post.
 
 You can have one of two properties (but not both because fuck you): `tags` or
 `regexp`. It's obvious what does what: if you have `regexp` set, plaintext
 version of status is checked against that regular expression, and if you have
 `tags` set, then only statuses that have those tags will be allowed.
 
 Please note that in case of tags, you should NOT use `#` symbol in front of
 them.
 
 #### `type = visibility`
+
 Simple filter that just checks for post visibility.
 Has a single property `options` that is a space-separated list of allowed
 visibility levels. Note that `direct` visibility is always ignored so cannot
 be used here.
 
 #### `type = media`
+
 Filter that allows only some media types to be posted.
 
 `valid_media` is a space-separated list of media types from Mastodon API
 (`image`, `gifv`, `video`, `audio` or `unknown`). If your Fedi software has
 support for other types, they also should work.
 
 `mode` option defines the mode of operation: it can be either `include`,
 `exclude` or `only`. In case of `include`, filter will trigger when post
 has media with that type, but others are allowed as well. `exclude` is the
 opposite: if status has media with that type, filter won't trigger. `only`
 allows statuses with either no media, or listed types only.
 
 #### `type = combined`
+
 The most powerful filter 'cause it allows you to combine multiple filters using
 different operations.
 
 `filters` option should contain space-separated list of filters. You also can
 negate them using `!` or `~` prefixes.
 
 `operator` is a type of operation to be used. Can be either `all`, `any` or
 `single`. `all` means that all of the filters should be used. `any` means
 that if any filter is triggered, this one will also trigger. `single` means
 that only one filter should be triggered. Think of it as an XOR operation of
 some sort.
 
 ## Sample configurations
 
-### For Telegram:
+### For Telegram
+
 ```ini
 [main]
 modules = tg
 instance = expired.mentality.rip
 token = haha-no
 list = 42
 user = auto
 
 [module/tg]
 type = telegram
 token = 12345:blahblahblah
 chat = 12345
 ```
 
-### For Telegram with a separate shitpost channel:
+### For Telegram with a separate shitpost channel
+
 ```ini
 [main]
 modules = tg tg-shitpost
 instance = expired.mentality.rip
 token = haha-no
 list = 42
 user = auto
@@ -269,17 +315,22 @@
 type = telegram
 token = 12345:blahblahblah
 chat = 12345
 filters = !shitpost
 
 [module/tg-shitpost]
 type = telegram
-token = 12345:blahblahblah
+token = ${module/tg:token}
 chat = @shitposting
 filters = shitpost
 
 [filters/shitpost]
 type = content
 mode = tag
 tags = shitpost
 ```
 
+## Asterisks
+
+1. Well, most of the time that is.
+2. Works only when it has lists support.
+
```

