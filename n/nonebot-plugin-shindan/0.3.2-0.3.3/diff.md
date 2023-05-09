# Comparing `tmp/nonebot_plugin_shindan-0.3.2.tar.gz` & `tmp/nonebot_plugin_shindan-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_shindan-0.3.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_shindan-0.3.3.tar", max compression
```

## Comparing `nonebot_plugin_shindan-0.3.2.tar` & `nonebot_plugin_shindan-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/LICENSE
--rw-r--r--   0        0        0     1626 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/README.md
--rw-r--r--   0        0        0     8442 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/__init__.py
--rw-r--r--   0        0        0      119 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/config.py
--rw-r--r--   0        0        0     2374 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/manager.py
--rw-r--r--   0        0        0     3393 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
--rw-r--r--   0        0        0      530 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/model.py
--rw-r--r--   0        0        0     4518 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/shindanmaker.py
--rw-r--r--   0        0        0   180778 2023-04-13 02:47:47.087900 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.css
--rw-r--r--   0        0        0   247324 2023-04-13 02:47:47.091901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.js
--rw-r--r--   0        0        0   477118 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/chart.js
--rw-r--r--   0        0        0      339 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/shindan.html
--rw-r--r--   0        0        0     1965 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/shindan_list.html
--rw-r--r--   0        0        0      843 2023-04-13 02:47:47.095901 nonebot_plugin_shindan-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1626 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/README.md
+-rw-r--r--   0        0        0     8442 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/config.py
+-rw-r--r--   0        0        0     2374 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/manager.py
+-rw-r--r--   0        0        0     3393 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
+-rw-r--r--   0        0        0      530 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/model.py
+-rw-r--r--   0        0        0     4526 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/shindanmaker.py
+-rw-r--r--   0        0        0   180778 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.css
+-rw-r--r--   0        0        0   247324 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.js
+-rw-r--r--   0        0        0   477118 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/chart.js
+-rw-r--r--   0        0        0      339 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/shindan.html
+-rw-r--r--   0        0        0     1965 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/shindan_list.html
+-rw-r--r--   0        0        0      843 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_shindan-0.3.2/LICENSE` & `nonebot_plugin_shindan-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/README.md` & `nonebot_plugin_shindan-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/__init__.py` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     description="使用ShindanMaker网站的趣味占卜",
     usage="发送“占卜列表”查看可用占卜\n发送“{占卜名} {名字}”使用占卜",
     config=Config,
     extra={
         "unique_name": "shindan",
         "example": "人设生成 小Q",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.3.2",
+        "version": "0.3.3",
     },
 )
 
 add_usage = """Usage:
 添加占卜 {id} {指令}
 如：添加占卜 917962 人设生成"""
```

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/manager.py` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/model.py` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/shindanmaker.py` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/shindanmaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         if noscript := tag.find_next("noscript"):
             noscript.replace_with_children()
             tag.extract()
 
 
 async def render_html(content: str) -> Tuple[str, bool]:
     dom = BeautifulSoup(content, "lxml")
-    result_js = str(dom.find("script", string=re.compile(r"saveResult")))
+    result_js = str(dom.find("script", string=re.compile(r"savedShindanResult")))
     title = str(dom.find("h1", {"id": "shindanResultAbove"}))
     result = dom.find("div", {"id": "shindanResultBlock"})
     assert isinstance(result, Tag)
     remove_shindan_effects(result, "ef_shuffle")
     remove_shindan_effects(result, "ef_typing")
     result = str(result)
     has_chart = "chart.js" in content
```

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.css` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/app.js` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/chart.js` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/chart.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/nonebot_plugin_shindan/templates/shindan_list.html` & `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/shindan_list.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.2/pyproject.toml` & `nonebot_plugin_shindan-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_shindan"
-version = "0.3.2"
+version = "0.3.3"
 description = "Nonebot2 plugin for using ShindanMaker"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-shindan"
 repository = "https://github.com/noneplugin/nonebot-plugin-shindan"
```

### Comparing `nonebot_plugin_shindan-0.3.2/PKG-INFO` & `nonebot_plugin_shindan-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-shindan
-Version: 0.3.2
+Version: 0.3.3
 Summary: Nonebot2 plugin for using ShindanMaker
 Home-page: https://github.com/noneplugin/nonebot-plugin-shindan
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

