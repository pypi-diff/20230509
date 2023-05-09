# Comparing `tmp/nonebot_plugin_spark_gpt-0.1.0.tar.gz` & `tmp/nonebot_plugin_spark_gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-0.1.0.tar` & `nonebot_plugin_spark_gpt-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1407 2023-05-09 11:22:02.751582 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0       14 2023-05-07 04:23:37.338492 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
--rw-r--r--   0        0        0     8227 2023-05-08 17:28:00.134982 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/config.py
--rw-r--r--   0        0        0    27202 2023-05-08 17:35:02.026220 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/main.py
--rw-r--r--   0        0        0     6129 2023-05-08 17:20:52.155727 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
--rw-r--r--   0        0        0       14 2023-05-07 04:37:03.529698 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-07 16:21:14.595978 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/common_func.py
--rw-r--r--   0        0        0     6152 2023-05-08 15:02:15.181030 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     4877 2023-05-09 05:04:52.272343 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/main.py
--rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
--rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/render.py
--rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
--rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
--rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
--rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
--rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
--rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/text.css
--rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/text.html
--rw-r--r--   0        0        0     4215 2023-05-08 15:55:10.287665 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/newbing/config.py
--rw-r--r--   0        0        0    18565 2023-05-08 16:56:38.171949 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/newbing/main.py
--rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/newbing/newbing_func.py
--rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/__init__.py
--rw-r--r--   0        0        0     9719 2023-05-08 16:42:46.394179 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/config.py
--rw-r--r--   0        0        0    29776 2023-05-08 17:01:51.461667 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/main.py
--rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/poe_api.py
--rw-r--r--   0        0        0     7374 2023-05-08 03:59:50.889224 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/poe_func.py
--rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/pwframework.py
--rw-r--r--   0        0        0      910 2023-05-09 13:31:03.518513 nonebot_plugin_spark_gpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2891 2023-05-09 13:15:44.636412 nonebot_plugin_spark_gpt-0.1.0/README.md
--rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1743 2023-05-09 13:58:29.200887 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0       14 2023-05-07 04:23:37.338492 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-08 16:53:49.475522 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py
+-rw-r--r--   0        0        0     8227 2023-05-08 17:28:00.134982 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/config.py
+-rw-r--r--   0        0        0    27202 2023-05-08 17:35:02.026220 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/main.py
+-rw-r--r--   0        0        0     6129 2023-05-08 17:20:52.155727 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py
+-rw-r--r--   0        0        0       14 2023-05-07 04:37:03.529698 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-07 16:21:14.595978 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/common_func.py
+-rw-r--r--   0        0        0     6152 2023-05-08 15:02:15.181030 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     4877 2023-05-09 05:04:52.272343 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/main.py
+-rw-r--r--   0        0        0     3936 2023-05-09 11:11:17.903494 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc
+-rw-r--r--   0        0        0     4066 2023-05-09 11:11:11.036002 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/render.py
+-rw-r--r--   0        0        0    18464 2023-05-09 08:51:42.987873 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2023-04-22 14:17:13.496635 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-04-22 14:17:13.497555 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-04-22 14:17:13.498611 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      670 2023-05-09 08:51:13.189256 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown.html
+-rw-r--r--   0        0        0     1253 2023-05-09 05:07:59.973080 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html
+-rw-r--r--   0        0        0     4625 2023-05-09 09:23:49.857905 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/background.png
+-rw-r--r--   0        0        0     1137 2023-04-22 05:34:37.774678 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png
+-rw-r--r--   0        0        0    86342 2023-04-22 05:34:37.775678 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png
+-rw-r--r--   0        0        0      125 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-04-22 14:17:13.500554 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/text.html
+-rw-r--r--   0        0        0     4215 2023-05-08 15:55:10.287665 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/config.py
+-rw-r--r--   0        0        0    18565 2023-05-08 16:56:38.171949 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/main.py
+-rw-r--r--   0        0        0     3068 2023-05-08 16:16:37.378665 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/newbing_func.py
+-rw-r--r--   0        0        0       16 2023-05-08 03:59:58.447201 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/__init__.py
+-rw-r--r--   0        0        0     9719 2023-05-08 16:42:46.394179 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/config.py
+-rw-r--r--   0        0        0    29776 2023-05-08 17:01:51.461667 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/main.py
+-rw-r--r--   0        0        0    10706 2023-05-08 03:59:52.713874 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_api.py
+-rw-r--r--   0        0        0     7374 2023-05-08 03:59:50.889224 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_func.py
+-rw-r--r--   0        0        0     2147 2023-05-08 03:59:48.875662 nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/pwframework.py
+-rw-r--r--   0        0        0      897 2023-05-09 14:00:56.802173 nonebot_plugin_spark_gpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2889 2023-05-09 14:04:08.408306 nonebot_plugin_spark_gpt-0.1.1/README.md
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import nonebot
 
 from .poe import main
 from .newbing import main
 from .chatgpt_web import main
 from .common import main
 from nonebot.matcher import Matcher
+from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import (
     Event,
     Bot,
     MessageSegment,
 )
 
 from .common.render.render import md_to_pic
 
+__version__ = "0.1.1"
+__plugin_meta__ = PluginMetadata(
+    "Spark-GPT",
+    "将多来源的gpt接入qq及更多平台，使用便捷，管理完善，功能强大",
+    "通过/help /帮助 /说明 /使用说明  命令来获取详细使用说明",
+    {"Author": "canxin121"},
+)
+
+
 poe_help = nonebot.on_command(
     "help", aliases={"帮助", "使用说明", "说明"}, priority=4, block=False
 )
 
 
 @poe_help.handle()
 async def __poe_help__(bot: Bot, matcher: Matcher, event: Event):
```

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/chatgpt_web_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/config.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/main.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/chatgpt_web/web_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/common_func.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/common_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/main.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/__pycache__/render.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/render.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/markdown.html` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/markdown_.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/source/background.png` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/common/render/templates/source/mi_background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/newbing/config.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/newbing/main.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/newbing/newbing_func.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/newbing/newbing_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/config.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/main.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/poe_api.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/poe_func.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/poe_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/nonebot_plugin_spark_gpt/poe/pwframework.py` & `nonebot_plugin_spark_gpt-0.1.1/nonebot_plugin_spark_gpt/poe/pwframework.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-0.1.0/pyproject.toml` & `nonebot_plugin_spark_gpt-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "0.1.0"
-description = "Spark-GPT,提供完善预设管理系统，便捷对话，成熟控制的对接多个来源的机器人"
+version = "0.1.1"
+description = "Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_spark_gpt"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebot2 = "^2.0.0-beta.1"
```

### Comparing `nonebot_plugin_spark_gpt-0.1.0/README.md` & `nonebot_plugin_spark_gpt-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
   <a href="https://github.com/canxin121">
-    <img src="https://socialify.git.ci/canxin121/Spark-GPT/image?forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=auto" width="700" height="350">
+    <img src="https://socialify.git.ci/canxin121/Spark-GPT/image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto" width="700" height="350">
   </a>
   <h1>Spark-GPT</h1>
   <p><em>Spark-GPT</em></p>
 </div>
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/nonebot-plugin-spark-gpt">
@@ -12,22 +12,22 @@
     </a>
     <img src="https://img.shields.io/pypi/pyversions/nonebot-plugin-spark-gpt" alt="python">
     <img src="https://img.shields.io/pypi/dm/nonebot-plugin-spark-gpt" alt="pypi">
     <br />
     <a href="https://onebot.dev/">
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
-    <img src="https://img.shields.io/github/last-commit/canxin121/nonebot_poe_chat" alt="github">
+    <img src="https://img.shields.io/github/last-commit/canxin121/Spark-GPT" alt="github">
     </a>
 </p>
 <div align="left">
 
 ---
 
-[![残心小站-文档库](https://github.com/canxin121/nonebot_poe_chat/blob/main/source/spark/cx.png )](https://canxin121.github.io/docs/docs/Spark_GPT.html )
+[![残心小站-文档库](https://github.com/canxin121/Spark-GPT/blob/main/source/display.png )](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 
 > 详细教程（必看，否则不会使用） 点击链接跳转👇 点击图片跳转☝️
   
 > 详细教程（必看，否则不会使用） 点击链接跳转👇 点击图片跳转☝️
 
 >
 ## [必看教程-残心小站-文档库](https://canxin121.github.io/docs/docs/Spark_GPT.html )
@@ -37,9 +37,9 @@
 ---
 
 - 目前支持将Poe,NewBing,Dalle,ChatGPT (session token)接入qq
 
 | Image 1 | Image 2 |
 |:-------:|:-------:|
 | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) |
-| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |
-| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) |                                   |
+| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) |
+| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |                                   |
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
                 [https://socialify.git.ci/canxin121/Spark-GPT/
-image?forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=auto]
+image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                             ****** Spark-GPT ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
---- [![æ®å¿å°ç«-ææ¡£åº](https://github.com/canxin121/nonebot_poe_chat/
-blob/main/source/spark/cx.png )](https://canxin121.github.io/docs/docs/
-Spark_GPT.html ) > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
-ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ >
-è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼ ç¹å»é¾æ¥è·³è½¬ð
-ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-æ®å¿å°ç«-ææ¡£åº](https://
-canxin121.github.io/docs/docs/Spark_GPT.html ) > ç¨æ·äº¤æµç¾¤:[610948446]
-(http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=KHGqjjbiz6fpRr-
+--- [![æ®å¿å°ç«-ææ¡£åº](https://github.com/canxin121/Spark-GPT/blob/
+main/source/display.png )](https://canxin121.github.io/docs/docs/Spark_GPT.html
+) > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼ ç¹å»é¾æ¥è·³è½¬ð
+ç¹å»å¾çè·³è½¬âï¸ > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
+ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-
+æ®å¿å°ç«-ææ¡£åº](https://canxin121.github.io/docs/docs/Spark_GPT.html )
+> ç¨æ·äº¤æµç¾¤:[610948446](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=KHGqjjbiz6fpRr-
 W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 ) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token)æ¥å¥qq |
 Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://github.com/canxin121/
 Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/
 canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | | ![3](https://
 github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4]
-(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) | |
-![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png)
+(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | |
+![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png)
 | |
```

### Comparing `nonebot_plugin_spark_gpt-0.1.0/PKG-INFO` & `nonebot_plugin_spark_gpt-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 0.1.0
-Summary: Spark-GPT,提供完善预设管理系统，便捷对话，成熟控制的对接多个来源的机器人
+Version: 0.1.1
+Summary: Spark-GPT,将多来源的gpt接入qq及更多平台,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot
@@ -24,15 +24,15 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pymdown-extensions (>=9.11,<10.0)
 Requires-Dist: python-markdown-math (>=0.8,<0.9)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://github.com/canxin121">
-    <img src="https://socialify.git.ci/canxin121/Spark-GPT/image?forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=auto" width="700" height="350">
+    <img src="https://socialify.git.ci/canxin121/Spark-GPT/image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto" width="700" height="350">
   </a>
   <h1>Spark-GPT</h1>
   <p><em>Spark-GPT</em></p>
 </div>
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/nonebot-plugin-spark-gpt">
@@ -40,22 +40,22 @@
     </a>
     <img src="https://img.shields.io/pypi/pyversions/nonebot-plugin-spark-gpt" alt="python">
     <img src="https://img.shields.io/pypi/dm/nonebot-plugin-spark-gpt" alt="pypi">
     <br />
     <a href="https://onebot.dev/">
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
-    <img src="https://img.shields.io/github/last-commit/canxin121/nonebot_poe_chat" alt="github">
+    <img src="https://img.shields.io/github/last-commit/canxin121/Spark-GPT" alt="github">
     </a>
 </p>
 <div align="left">
 
 ---
 
-[![残心小站-文档库](https://github.com/canxin121/nonebot_poe_chat/blob/main/source/spark/cx.png )](https://canxin121.github.io/docs/docs/Spark_GPT.html )
+[![残心小站-文档库](https://github.com/canxin121/Spark-GPT/blob/main/source/display.png )](https://canxin121.github.io/docs/docs/Spark_GPT.html )
 
 > 详细教程（必看，否则不会使用） 点击链接跳转👇 点击图片跳转☝️
   
 > 详细教程（必看，否则不会使用） 点击链接跳转👇 点击图片跳转☝️
 
 >
 ## [必看教程-残心小站-文档库](https://canxin121.github.io/docs/docs/Spark_GPT.html )
@@ -65,10 +65,10 @@
 ---
 
 - 目前支持将Poe,NewBing,Dalle,ChatGPT (session token)接入qq
 
 | Image 1 | Image 2 |
 |:-------:|:-------:|
 | ![1](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) |
-| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |
-| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) |                                   |
+| ![3](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) |
+| ![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) |                                   |
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 0.1.1 Summary:
 Spark-
-GPT,æä¾å®åé¢è®¾ç®¡çç³»ç»ï¼ä¾¿æ·å¯¹è¯ï¼æçæ§å¶çå¯¹æ¥å¤ä¸ªæ¥æºçæºå¨äºº
+GPT,å°å¤æ¥æºçgptæ¥å¥qqåæ´å¤å¹³å°,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: bidict (>=0.22.1,<0.23.0)
 Requires-Dist: edgegpt (>=0.3.6,<0.4.0) Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: imagegen (>=0.2,<0.3) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: markdown (>=3.4.3,<4.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.0.0-beta.1,<3.0.0) ; extra == "onebot" Requires-Dist: nonebot-plugin-
 guild-patch Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0) Requires-Dist:
 playwright (>=1.33.0,<2.0.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pymdown-extensions (>=9.11,<10.0) Requires-Dist: python-
 markdown-math (>=0.8,<0.9) Description-Content-Type: text/markdown
                 [https://socialify.git.ci/canxin121/Spark-GPT/
-image?forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=auto]
+image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                             ****** Spark-GPT ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
---- [![æ®å¿å°ç«-ææ¡£åº](https://github.com/canxin121/nonebot_poe_chat/
-blob/main/source/spark/cx.png )](https://canxin121.github.io/docs/docs/
-Spark_GPT.html ) > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
-ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ >
-è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼ ç¹å»é¾æ¥è·³è½¬ð
-ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-æ®å¿å°ç«-ææ¡£åº](https://
-canxin121.github.io/docs/docs/Spark_GPT.html ) > ç¨æ·äº¤æµç¾¤:[610948446]
-(http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=KHGqjjbiz6fpRr-
+--- [![æ®å¿å°ç«-ææ¡£åº](https://github.com/canxin121/Spark-GPT/blob/
+main/source/display.png )](https://canxin121.github.io/docs/docs/Spark_GPT.html
+) > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼ ç¹å»é¾æ¥è·³è½¬ð
+ç¹å»å¾çè·³è½¬âï¸ > è¯¦ç»æç¨ï¼å¿çï¼å¦åä¸ä¼ä½¿ç¨ï¼
+ç¹å»é¾æ¥è·³è½¬ð ç¹å»å¾çè·³è½¬âï¸ > ## [å¿çæç¨-
+æ®å¿å°ç«-ææ¡£åº](https://canxin121.github.io/docs/docs/Spark_GPT.html )
+> ç¨æ·äº¤æµç¾¤:[610948446](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=KHGqjjbiz6fpRr-
 W2X9SugTXThKFiprJ&authKey=LhpClaGtc4%2Ff3EL7f4IIIt7F94vLHJj4HSS8c2YCE55nRBRBtftzla%2Bgj7pa0fWX&noverify=0&group_code=610948446
 ) --- - ç®åæ¯æå°Poe,NewBing,Dalle,ChatGPT (session token)æ¥å¥qq |
 Image 1 | Image 2 | |:-------:|:-------:| | ![1](https://github.com/canxin121/
 Spark-GPT/blob/main/source/spark/demo(1).png) | ![2](https://github.com/
 canxin121/Spark-GPT/blob/main/source/spark/demo(2).png) | | ![3](https://
 github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(3).png) | ![4]
-(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png) | |
-![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png)
+(https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(5).png) | |
+![5](https://github.com/canxin121/Spark-GPT/blob/main/source/spark/demo(4).png)
 | |
```

