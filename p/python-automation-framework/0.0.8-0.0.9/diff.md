# Comparing `tmp/python-automation-framework-0.0.8.tar.gz` & `tmp/python-automation-framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.0.8.tar", last modified: Sun Apr 30 08:20:53 2023, max compression
+gzip compressed data, was "python-automation-framework-0.0.9.tar", last modified: Tue May  9 19:32:49 2023, max compression
```

## Comparing `python-automation-framework-0.0.8.tar` & `python-automation-framework-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.232520 python-automation-framework-0.0.8/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3872 2023-04-30 08:20:53.232356 python-automation-framework-0.0.8/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     3622 2023-04-29 17:41:40.000000 python-automation-framework-0.0.8/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.229737 python-automation-framework-0.0.8/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     6192 2023-04-29 17:46:30.000000 python-automation-framework-0.0.8/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.8/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2156 2023-04-29 16:20:38.000000 python-automation-framework-0.0.8/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.8/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.8/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.8/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.8/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.8/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-29 16:24:25.000000 python-automation-framework-0.0.8/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2966 2023-04-29 17:56:24.000000 python-automation-framework-0.0.8/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.8/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      265 2023-04-29 08:35:21.000000 python-automation-framework-0.0.8/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    13473 2023-04-29 17:11:48.000000 python-automation-framework-0.0.8/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6598 2023-04-29 16:11:44.000000 python-automation-framework-0.0.8/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.230637 python-automation-framework-0.0.8/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3872 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-30 08:20:53.232576 python-automation-framework-0.0.8/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-30 08:20:20.000000 python-automation-framework-0.0.8/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.232082 python-automation-framework-0.0.8/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1910 2023-04-29 16:10:05.000000 python-automation-framework-0.0.8/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.8/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1869 2023-04-28 08:20:26.000000 python-automation-framework-0.0.8/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      855 2023-04-29 12:28:05.000000 python-automation-framework-0.0.8/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.8/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     7312 2023-04-29 17:55:55.000000 python-automation-framework-0.0.8/test/test_uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.8/test/test_webdriver.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.795745 python-automation-framework-0.0.9/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-05-09 19:32:49.795584 python-automation-framework-0.0.9/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5137 2023-05-09 19:22:38.000000 python-automation-framework-0.0.9/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.793266 python-automation-framework-0.0.9/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     7037 2023-05-09 19:19:06.000000 python-automation-framework-0.0.9/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3319 2023-05-09 19:04:45.000000 python-automation-framework-0.0.9/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2114 2023-05-09 11:20:20.000000 python-automation-framework-0.0.9/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      497 2023-05-09 08:02:43.000000 python-automation-framework-0.0.9/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2473 2023-05-05 10:53:33.000000 python-automation-framework-0.0.9/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.9/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.9/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2257 2023-05-09 14:09:11.000000 python-automation-framework-0.0.9/paf/listener.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-04 17:04:40.000000 python-automation-framework-0.0.9/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4345 2023-05-09 18:44:17.000000 python-automation-framework-0.0.9/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3016 2023-05-09 19:21:48.000000 python-automation-framework-0.0.9/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2346 2023-05-04 20:56:52.000000 python-automation-framework-0.0.9/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 18:25:16.000000 python-automation-framework-0.0.9/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    14434 2023-05-09 18:27:18.000000 python-automation-framework-0.0.9/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.0.9/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.794025 python-automation-framework-0.0.9/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      668 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-09 19:32:49.795795 python-automation-framework-0.0.9/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-05-09 19:31:57.000000 python-automation-framework-0.0.9/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.795369 python-automation-framework-0.0.9/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.0.9/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1837 2023-05-09 19:20:32.000000 python-automation-framework-0.0.9/test/test_demo_mode.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:14:31.000000 python-automation-framework-0.0.9/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 11:19:43.000000 python-automation-framework-0.0.9/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3274 2023-05-09 19:15:53.000000 python-automation-framework-0.0.9/test/test_manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1563 2023-05-09 19:22:08.000000 python-automation-framework-0.0.9/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:15:46.000000 python-automation-framework-0.0.9/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     9699 2023-05-09 19:21:48.000000 python-automation-framework-0.0.9/test/test_uielement.py
```

### Comparing `python-automation-framework-0.0.8/PKG-INFO` & `python-automation-framework-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
+![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-automation-framework/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
+
+
 # PAF - Python Automation Framework
 
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
@@ -56,30 +60,34 @@
 
 ## Feature list
 
 - [UiElements](doc/uielement.md)
 - [Locators](doc/locators.md)
 - [Page objects](doc/pages.md)
 - [Components](doc/components.md)
-- [Managing WebDrivers](doc/webdriver.md)
+- [Managing WebDrivers](doc/manager.md)
 - [Execution controlling](doc/control.md)
+- [Inject listener](doc/listener.md)
 
-### Missing features (todos)
+### Missing features (tdb)
 
 - Rect assertions
 - ShadowRoot support
 - Drag & Drop over frames
 
 ## Environment variables
 
+The value behind the variable is the default value.
+
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
 * `PAF_SEQUENCE_WAIT_AFTER_FAIL=0.3`: Wait in seconds whenever a sequence action fails. 
 * `PAF_SEQUENCE_RETRY_COUNT=3`: Retry count for every sequence action.
+* `PAF_DEMO_MODE=0`: Enables the demo mode by highlighting actions and assertions.
 
 ## Examples
 
 I added two examples.
 
 1. [test_google.py](examples/test_google.py): is a regular Google search, implemented with [Page Objects](doc/pages.md) and [Components](doc/components.md). 
 2. [test_todo_mvc.py](examples/test_todo_mvc.py): are re-implemented test cases from the [Robot Framework TodoMVC](https://docs.robotframework.org/docs/examples/todo) example. It's IMHO developer friendly, better readable and less code. 
@@ -88,45 +96,66 @@
 ## Comparison
 
 Comparison of the syntax with other frameworks.
 
 **Pylenium**
 ```python
 py.get("a[href='/about']").should().have_text("About")
-```
-```python
+
 find("a[href='/about']").expect.text.be("About")
 ```
 **SeleniumBase**
 ```python
 self.assert_text_not_visible("Thanks for your purchase.", "#app .success")
-```
-```python
+
 find("#app .success").expect.text.not_be("Thanks for your purchase.")
 ```
 **Selene**
 ```python
 browser.all('#rso>div').should(have.size_greater_than(5)) \
     .first.should(have.text('Selenium automates browsers'))
-```
-```python
+
 div = find("#rso>div")
 div.expect.count.greater_than(5).be(True)
 div.first.expect.text.be("Selenium automates browsers")
 ```
 
 References: https://www.nextgenerationautomation.com/post/python-test-automation-frameworks
 
 ## Developer area
-### Run the tests
+
+### Testing
+#### Run the tests on you local machine
 ```shell
-PYTHONPATH="." pytest --numprocesses=4 --cov=paf test
+pytest --cov=paf -n=4 test
 ```
 
-### Utils
+#### Build test base container (for use in GitHub Actions)
+```shell
+podman build -f base.Dockerfile --arch=amd64 -t paf-test-base:latest
+echo $DOCKER_CONTAINER_REGISTRY_TOKEN | podman login -u mreiche --password-stdin ghcr.io
+podman push paf-test-base:latest docker://ghcr.io/mreiche/paf-test-base:latest
+```
+
+#### Build test runner container (for testing)
+```shell
+podman build -f test.Dockerfile --arch=amd64 -t paf-test:latest
+```
+Run tests within container
+```shell
+podman run paf-test:latest PAF_TEST_HEADLESS=1 PAF_TEST_CONTAINER=1 pytest --cov=paf -n=4 test
+```
+
+#### Run local selenium server
+```shell
+wget https://github.com/SeleniumHQ/selenium/releases/download/selenium-4.9.0/selenium-server-4.9.0.jar -O selenium-server.jar
+java -jar selenium-server.jar standalone --host 127.0.0.1
+```
+
+### Debug XPaths in Browser's Developer Console
 
 ```javascript
 xpath = "//dt[.//text()='Title:']/following-sibling::dd[1]"
 snapshot = document.evaluate(xpath, document.body, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE)
 snapshot.snapshotItem(0).textContent
 ```
 
@@ -136,7 +165,12 @@
     ```shell
     python setup.py sdist
     ```
 3. Publish library
     ```shell
     twine upload dist/python-automation-framework-[version].tar.gz
     ```
+
+### References
+- https://stackoverflow.com/questions/64033686/how-can-i-use-private-docker-image-in-github-actions
+- https://tecadmin.net/setup-selenium-chromedriver-on-ubuntu/
+- https://stackoverflow.com/questions/46052736/python-proxy-class
```

### Comparing `python-automation-framework-0.0.8/paf/common.py` & `python-automation-framework-0.0.9/paf/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,62 @@
 from datetime import datetime
 from enum import Enum
 
 import inject
 from selenium.webdriver.remote.webelement import WebElement
 
 from paf.locator import By
+from paf.types import Predicate
 from paf.xpath import XPath
 
 Locator = By | XPath | str
 
 
 class HasName(ABC):
     @property
     @abstractmethod
-    def name(self):
+    def name(self):  # pragma: no cover
         pass
 
 
 class HasParent(HasName, ABC):
     @property
     def _parent(self):
         return self.__parent
 
     @_parent.setter
     def _parent(self, parent: "HasParent"):
         self.__parent = parent
 
     @property
     def name_path(self):
-        path = [self]
+        from paf.component import Component
+        from paf.page import Page
+        from paf.uielement import UiElement
+        name_path = ""
+
+        def _trace(inst: HasName):
+            nonlocal name_path
+            name_path = inst.name + name_path
+            if isinstance(inst, (UiElement, Component, Page)) \
+                and isinstance(inst, HasParent) \
+                and isinstance(inst._parent, (UiElement, Component, Page)):
+                name_path = " > " + name_path
+            return True
+
+        self._trace_path(_trace)
+        return name_path
+
+    def _trace_path(self, consumer: Predicate[HasName]):
         inst = self
-        while hasattr(inst, "_parent") and inst._parent:
-            path.append(inst._parent)
-            inst = inst._parent
+        while isinstance(inst, HasName):
+            if not consumer(inst) or not isinstance(inst, HasParent):
+                break
 
-        return " > ".join(map(str, reversed(path)))
+            inst = inst._parent
 
 
 @dataclass()
 class Point:
     x: int = 0
     y: int = 0
 
@@ -79,38 +97,47 @@
 
     @property
     def bottom(self):
         return self.top + self.height
 
     def contains(self, rect: "Rect"):
         return rect.left >= self.left \
-               and rect.right <= self.right \
-               and rect.top >= self.top \
-               and rect.bottom <= self.bottom
+            and rect.right <= self.right \
+            and rect.top >= self.top \
+            and rect.bottom <= self.bottom
 
     def intersects(self, rect: "Rect"):
         return rect.left <= self.right \
-               and rect.right >= self.left \
-               and rect.top <= self.bottom \
-               and rect.bottom >= self.top
+            and rect.right >= self.left \
+            and rect.top <= self.bottom \
+            and rect.bottom >= self.top
 
 
 class Property(Enum):
     PAF_SCREENSHOTS_DIR = "screenshots"
     PAF_WINDOW_SIZE = "1920x1080"
     PAF_BROWSER_SETTING = "chrome"
     PAF_SEQUENCE_WAIT_AFTER_FAIL = 0.3
     PAF_SEQUENCE_RETRY_COUNT = 3
     PAF_SELENIUM_SERVER_URL = None
+    PAF_DEMO_MODE = "0"
 
     @staticmethod
     def env(prop: "Property") -> any:
         return os.getenv(prop.name, prop.value)
 
 
 class Formatter:
     def datetime(self, date: datetime):
         return date.strftime('%Y-%m-%d-%H:%M:%S')
 
 
+class NotFoundException(Exception):
+    pass
+
+
+class NotUniqueException(Exception):
+    pass
+
+
 def inject_config(binder: inject.Binder):
     binder.bind(Formatter, Formatter())
```

### Comparing `python-automation-framework-0.0.8/paf/component.py` & `python-automation-framework-0.0.9/paf/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Type
 
 from selenium.webdriver.support.color import Color
 
-from paf.common import HasParent, Locator, Point
+from paf.common import HasParent, Locator
 from paf.types import COMPONENT, PAGE
 from paf.uielement import UiElement, PageObject, PageObjectList, UiElementTests
 
 
 class Component(PageObject[COMPONENT], PageObjectList[COMPONENT], HasParent, UiElementTests):
 
     def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
@@ -15,15 +15,14 @@
 
     def __init__(self, ui_element: UiElement):
         self._ui_element = ui_element
         ui_element._parent = self
 
     def _find(self, by: Locator):
         ui_element = self._ui_element.find(by)
-        #ui_element._parent = self
         return ui_element
 
     @property
     def name(self):
         return f"{self.__class__.__name__}"
 
     @property
```

### Comparing `python-automation-framework-0.0.8/paf/control.py` & `python-automation-framework-0.0.9/paf/control.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass
 from time import sleep, time
 from typing import Callable
 
 import inject
 
 from paf.common import Property
+from paf.types import Consumer
 
 
 @dataclass()
 class Config:
     retry_count: int = Property.env(Property.PAF_SEQUENCE_RETRY_COUNT)
     wait_after_fail: float = Property.env(Property.PAF_SEQUENCE_WAIT_AFTER_FAIL)
 
@@ -53,15 +54,15 @@
 class Control:
 
     __global_config: Config = Config()
 
     def retry(
         self,
         action: Callable,
-        on_fail: Callable = None,
+        on_fail: Consumer[Exception] = None,
         count: int = None,
         wait_after_fail: float = None
     ):
         config_backup = Control.__global_config
         config = dataclasses.replace(config_backup)
         Control.__global_config = config
 
@@ -79,15 +80,15 @@
             try:
                 action()
                 exception = None
                 return True
             except Exception as e:
                 exception = e
                 if on_fail:
-                    on_fail()
+                    on_fail(e)
 
         sequence.run(_run)
 
         Control.__global_config = config_backup
 
         if exception:
             raise RetryException(sequence, f"{exception} after {sequence.count} retries ({round(sequence.duration, 2)} seconds)")
```

### Comparing `python-automation-framework-0.0.8/paf/javascript.py` & `python-automation-framework-0.0.9/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.8/paf/locator.py` & `python-automation-framework-0.0.9/paf/locator.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,18 @@
 
     @staticmethod
     def id(id: str):
         return By(SeleniumBy.ID, id)
 
     @staticmethod
     def xpath(xpath: str):
+        from paf.xpath import XPath
+        if isinstance(xpath, XPath):
+            xpath = str(xpath)
+
         return By(SeleniumBy.XPATH, xpath)
 
     @staticmethod
     def name(name: str):
         return By(SeleniumBy.NAME, name)
 
     @staticmethod
```

### Comparing `python-automation-framework-0.0.8/paf/manager.py` & `python-automation-framework-0.0.9/paf/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-import logging
-import os
 from datetime import datetime
 from pathlib import Path
 from typing import Type, TypeVar, Iterable
 
 import inject
 from is_empty import empty
 from selenium.webdriver import Chrome, Firefox, Edge, Safari, Remote, ChromeOptions, EdgeOptions, FirefoxOptions, WPEWebKitOptions
 from selenium.webdriver.common.options import BaseOptions
 from selenium.webdriver.remote.webdriver import WebDriver, BaseWebDriver
-
 from paf.common import Property, Formatter
 from paf.request import WebDriverRequest
 
 OPTION = TypeVar("OPTION")
 
-LOG = logging.getLogger(__name__)
-
 
 class WebDriverManager:
     def __init__(self):
         self._session_driver_map: dict[str, WebDriver] = {}
         self._thread_driver_map: dict[int, WebDriver] = {}
 
     def _get_options(self, request: WebDriverRequest, options_class: Type[OPTION]) -> OPTION:
@@ -28,89 +23,91 @@
         if not options:
             options = options_class()
         else:
             assert isinstance(options, BaseOptions)
 
         return options
 
-    def get_webdriver(self, request: WebDriverRequest = None) -> WebDriver:
-        if not request:
-            request = WebDriverRequest()
-
-        session_key = request.session
-        if session_key in self._session_driver_map:
-            return self._session_driver_map[session_key]
+    def get_webdriver(self, request: WebDriverRequest) -> WebDriver:
+        session_name = request.session_name
+        if session_name in self._session_driver_map:
+            return self._session_driver_map[session_name]
 
         webdriver = None
         webdriver_class: Type[BaseWebDriver] = None
         options: BaseOptions = None
 
-        if request.browser in ["chrome", "chromium"]:
+        if request.browser in ["chrome"]:
             options = self._get_options(request, ChromeOptions)
             webdriver_class = Chrome
         elif request.browser in ["firefox"]:
             options = self._get_options(request, FirefoxOptions)
             webdriver_class = Firefox
         elif request.browser in ["edge"]:
             options = self._get_options(request, EdgeOptions)
             webdriver_class = Edge
         elif request.browser in ["safari"]:
             options = self._get_options(request, WPEWebKitOptions)
             webdriver_class = Safari
+        else:
+            raise Exception("No browser specified")
 
         if request.browser_version:
             options.set_capability("browserVersion", request.browser_version)
-            #options.set_capability("platformName", "Windows XP")
+            # options.set_capability("platformName", "Windows XP")
 
         if request.server_url:
-            webdriver = Remote(command_executor="http://127.0.0.1:4444", options=options)
+            webdriver = Remote(command_executor=request.server_url.geturl(), options=options)
         elif webdriver_class:
             webdriver = webdriver_class(options=options)
 
-        if not webdriver:
-            raise Exception("No browser specified")
+        self.introduce_webdriver(webdriver, request)
+
+        return webdriver
 
-        self._session_driver_map[session_key] = webdriver
+    def introduce_webdriver(self, webdriver: WebDriver, request: WebDriverRequest):
+        self._session_driver_map[request.session_name] = webdriver
 
         if request.window_size:
-            LOG.info(f"Set window size: {request.window_size}")
+            #LOG.info(f"Set window size {request.window_size} on {webdriver.name}")
             webdriver.set_window_rect(0, 0, request.window_size.width, request.window_size.height)
 
-        return webdriver
+    def has_webdriver(self, session_name):
+        return session_name in self._session_driver_map
 
-    def shutdown_session(self, session_key):
-        if session_key in self._session_driver_map:
-            self.shutdown(self._session_driver_map[session_key])
+    def shutdown_session(self, session_name: str):
+        if session_name in self._session_driver_map:
+            self.shutdown(self._session_driver_map[session_name])
         else:
-            raise Exception(f"Unknown session: {session_key}")
+            raise Exception(f"Unknown session: {session_name}")
 
     def shutdown(self, webdriver: WebDriver):
         webdriver.quit()
         webdrivers = list(self._session_driver_map.values())
         index = webdrivers.index(webdriver)
 
         session_keys = list(self._session_driver_map.keys())
         key = session_keys[index]
         self._session_driver_map.pop(key)
 
     def shutdown_all(self):
         for webdriver in list(self._session_driver_map.values()):
             self.shutdown(webdriver)
 
-    def take_screenshot(self, webdriver: WebDriver) -> Path|None:
-        dir = Path(os.getenv(Property.PAF_SCREENSHOTS_DIR.name, Property.PAF_SCREENSHOTS_DIR.value))
+    def take_screenshot(self, webdriver: WebDriver) -> Path | None:
+        dir = Path(Property.env(Property.PAF_SCREENSHOTS_DIR))
         title = webdriver.title
         if empty(title):
             title = webdriver.current_url
 
         formatter = inject.instance(Formatter)
 
         file_name = f"{title}-{formatter.datetime(datetime.now())}.png"
         dir.mkdir(parents=True, exist_ok=True)
-        path = dir/file_name
+        path = dir / file_name
         if webdriver.save_screenshot(dir / file_name):
             return path
         else:
             return None
 
     @property
     def webdrivers(self) -> Iterable[WebDriver]:
```

### Comparing `python-automation-framework-0.0.8/paf/page.py` & `python-automation-framework-0.0.9/paf/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Type, TypeVar
+from typing import Type
 
 import inject
 from selenium.webdriver import ActionChains
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from paf.assertion import StringAssertion, Format
-from paf.common import HasName, Locator, Point
+from paf.common import HasName, Locator
 from paf.manager import WebDriverManager
+from paf.request import WebDriverRequest
 from paf.types import PAGE, COMPONENT
 
 
 class PageFactory:
     def create_page(self, page_class: Type[PAGE], webdriver: WebDriver = None) -> PAGE:
         if not webdriver:
-            webdriver = inject.instance(WebDriverManager).get_webdriver()
+            webdriver = inject.instance(WebDriverManager).get_webdriver(WebDriverRequest())
 
         return page_class(webdriver)
 
 
 class BasePage(HasName):
     def __init__(self, webdriver: WebDriver):
         self._webdriver = webdriver
@@ -37,14 +38,26 @@
     def name(self):
         return self.__class__.__name__
 
     @property
     def webdriver(self):
         return self._webdriver
 
+    @property
+    def expect(self):
+        return PageAssertion(self, self._webdriver)
+
+    @property
+    def wait_for(self):
+        return PageAssertion(self, self._webdriver, raise_exception=False)
+
+    def scroll_by(self, x: int = 0, y: int = 0):
+        actions = ActionChains(self._webdriver)
+        actions.scroll_by_amount(x, y).perform()
+
 
 class FinderPage(BasePage):
     def find(self, by: Locator):
         ui_element = self._find(by)
         ui_element._parent = None
         return ui_element
 
@@ -57,53 +70,40 @@
         component = component_class(ui_element)
         component._parent = self
         return component
 
     def _create_page(self, page_class: Type[PAGE]) -> PAGE:
         return page_class(self._webdriver)
 
-    @property
-    def expect(self):
-        return PageAssertion(self, self._webdriver)
-
-    @property
-    def wait_for(self):
-        return PageAssertion(self, self._webdriver, raise_exception=False)
-
-    def scroll_by(self, x: int = 0, y: int = 0):
-        actions = ActionChains(self._webdriver)
-        actions.scroll_by_amount(x, y).perform()
-
 
 class PageAssertion:
-
     def __init__(
         self,
         page: BasePage,
         webdriver: WebDriver,
         raise_exception: bool = True
     ):
         self._page = page
         self._webdriver = webdriver
         self._raise = raise_exception
 
     @property
     def title(self):
         return StringAssertion(
-            parent=None,
-            actual=lambda: self._webdriver.title,
-            subject=lambda: f"{self._page.name}.title {Format.param(self._webdriver.title)}",
+            parent=self._page,
+            actual_supplier=lambda: self._webdriver.title,
+            name_supplier=lambda: f".title {Format.param(self._webdriver.title)}",
             raise_exception=self._raise,
         )
 
     @property
     def url(self):
         return StringAssertion(
-            parent=None,
-            actual=lambda: self._webdriver.current_url,
-            subject=lambda: f"{self._page.name}.url {Format.param(self._webdriver.current_url)}",
+            parent=self._page,
+            actual_supplier=lambda: self._webdriver.current_url,
+            name_supplier=lambda: f".url {Format.param(self._webdriver.current_url)}",
             raise_exception=self._raise,
         )
 
 
 def inject_config(binder: inject.Binder):
     binder.bind(PageFactory, PageFactory())
```

### Comparing `python-automation-framework-0.0.8/paf/request.py` & `python-automation-framework-0.0.9/paf/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,17 @@
 
 from is_empty import empty
 from selenium.webdriver.common.options import BaseOptions
 
 from paf.common import Size, Property
 
 
-# import uuid
-# from is_empty import empty
-
-# O = TypeVar("O")
-
-
 class WebDriverRequest:
-    def __init__(self, session: str = "default"):
-        self._session = session
+    def __init__(self, session_name: str = "default"):
+        self._session_name = session_name
         self._window_size: Size = None
         self._browser: str = None
         self._browser_version: str = None
         self._options: BaseOptions = None
         self._server_url: ParseResult = None
         server_url = Property.env(Property.PAF_SELENIUM_SERVER_URL)
         if server_url:
@@ -41,18 +35,16 @@
     def server_url(self, url: str | ParseResult):
         if not isinstance(url, ParseResult):
             url = urlparse(url)
 
         self._server_url = url
 
     @property
-    def session(self):
-        #       if empty(self._session):
-        #           self._session = uuid.uuid4()
-        return self._session
+    def session_name(self):
+        return self._session_name
 
     def __detect_browser(self):
         match = re.search("(\w+)(?:\:(\w+))?", Property.env(Property.PAF_BROWSER_SETTING))
         if match:
             groups = match.groups()
             self._browser = groups[0]
             if not empty(groups[1]):
```

### Comparing `python-automation-framework-0.0.8/paf/uielement.py` & `python-automation-framework-0.0.9/paf/uielement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import math
-import re
 from abc import abstractmethod, ABC
 from datetime import datetime
 from pathlib import Path
 from typing import Type, TypeVar, List, Generic, Iterable, Iterator
 
 import inject
+import math
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By as SeleniumBy
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
 
 import paf.javascript as script
-from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion, RectAssertion
-from paf.common import HasParent, Locator, Point, Rect, Property, Formatter
+from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion, RectAssertion, ASSERTION
+from paf.common import HasParent, Locator, Point, Rect, Property, Formatter, NotFoundException, NotUniqueException
 from paf.control import Control
 from paf.dom import Attribute
+from paf.listener import Listener
 from paf.locator import By
 from paf.types import Mapper, Consumer, R
 from paf.xpath import XPath
 
 
 class UiElementActions:
 
     @abstractmethod
-    def click(self):
+    def click(self):   # pragma: no cover
         pass
 
     @abstractmethod
-    def hover(self):
+    def hover(self):  # pragma: no cover
         pass
 
     @abstractmethod
-    def context_click(self):
+    def context_click(self):  # pragma: no cover
         pass
 
     @abstractmethod
-    def long_click(self):
+    def long_click(self):  # pragma: no cover
         pass
 
     @abstractmethod
-    def double_click(self):
+    def double_click(self):  # pragma: no cover
         pass
 
     @abstractmethod
-    def drag_and_drop_to(self, target_ui_element: "UiElement"):
+    def drag_and_drop_to(self, target_ui_element: "UiElement"):  # pragma: no cover
         pass
 
     @abstractmethod
-    def send_keys(self, value: str):
+    def send_keys(self, value: str):  # pragma: no cover
         pass
 
     @abstractmethod
-    def type(self, value: str):
+    def type(self, value: str):  # pragma: no cover
         pass
 
     @abstractmethod
-    def clear(self):
+    def clear(self):  # pragma: no cover
         pass
 
     @abstractmethod
-    def submit(self):
+    def submit(self):  # pragma: no cover
         pass
 
 
 T = TypeVar('T')
 
 
 class PageObjectList(Generic[T], Iterable):
     @abstractmethod
-    def __getitem__(self, index: int) -> T:
+    def __getitem__(self, index: int) -> T:  # pragma: no cover
         pass
 
     @abstractmethod
-    def __iter__(self) -> Iterator[T]:
+    def __iter__(self) -> Iterator[T]:  # pragma: no cover
         pass
 
     @property
     def first(self) -> T:
         return self.__getitem__(0)
 
     @property
     def last(self) -> T:
         return self.__getitem__(-1)
 
 
 class PageObject(Generic[T]):
 
     @abstractmethod
-    def scroll_into_view(self, x: int = 0, y: int = 0):
+    def scroll_into_view(self, x: int = 0, y: int = 0):  # pragma: no cover
         pass
 
     @abstractmethod
-    def scroll_to_top(self, x: int = 0, y: int = 0):
+    def scroll_to_top(self, x: int = 0, y: int = 0):  # pragma: no cover
         pass
 
     @abstractmethod
-    def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
+    def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):  # pragma: no cover
         pass
 
 
 class UiElementTests:
     @property
     @abstractmethod
-    def expect(self) -> "UiElementAssertion":
+    def expect(self) -> "UiElementAssertion":  # pragma: no cover
         pass
 
     @property
     @abstractmethod
-    def wait_for(self) -> "UiElementAssertion":
+    def wait_for(self) -> "UiElementAssertion":  # pragma: no cover
         pass
 
 
 class TestableUiElement(PageObject["TestableUiElement"], UiElementTests, ABC):
     pass
 
 
@@ -182,43 +182,49 @@
 
             return self._ui_element.find_web_element(_handle)
         elif self._webdriver:
             self._webdriver.switch_to.default_content()
             web_elements = self._webdriver.find_elements(self._by.by, self._by.value)
             return consumer(self._filter_web_elements(web_elements))
         else:
-            raise Exception("UiElement initialized without WebDriver nor UiElement")
+            raise Exception(f"{self.name_path} initialized without WebDriver nor UiElement")
 
     def find_web_element(self, mapper: Mapper[WebElement, R]) -> R:
         def _handle(web_elements: List[WebElement]):
             count = len(web_elements)
 
             if self._by.is_unique and count != 1:
-                raise Exception(f"Not unique")
+                raise NotUniqueException(f"Not unique")
             elif count > self._index:
                 web_element = web_elements[self._index]
                 return mapper(web_element)
             else:
-                raise Exception(f"Not found")
+                raise NotFoundException(f"Not found")
 
         return self._find_web_elements(_handle)
 
-    def _action_sequence(self, consumer: Consumer[WebElement]):
+    def _action_sequence(self, consumer: Consumer[WebElement], action_name: str):
         control = inject.instance(Control)
+        listener = inject.instance(Listener)
         try:
-            control.retry(lambda: self.find_web_element(consumer))
+            control.retry(
+                action=lambda: self.find_web_element(consumer),
+                on_fail=lambda e: listener.action_failed(action_name, self, e)
+            )
+            listener.action_passed(action_name, self)
         except Exception as exception:
+            listener.action_failed_finally(action_name, self, exception)
             raise Exception(f"{self.name_path}: {exception}")
 
     def click(self):
-        self._action_sequence(lambda web_element: web_element.click())
+        self._action_sequence(lambda web_element: web_element.click(), __name__)
         return self
 
     def send_keys(self, value: str):
-        self._action_sequence(lambda web_element: web_element.send_keys(value))
+        self._action_sequence(lambda web_element: web_element.send_keys(value), __name__)
         return self
 
     def take_screenshot(self) -> Path | None:
         def _handle(web_element: WebElement):
             dir = Path(Property.env(Property.PAF_SCREENSHOTS_DIR))
             formatter = inject.instance(Formatter)
             file_name = f"{self.name}-{formatter.datetime(datetime.now())}.png"
@@ -233,82 +239,82 @@
 
     def type(self, value: str):
         def _action(web_element: WebElement):
             web_element.clear()
             web_element.send_keys(value)
             assert web_element.get_attribute("value") == value
 
-        self._action_sequence(_action)
+        self._action_sequence(_action, __name__)
         return self
 
     def hover(self):
         def _action(web_element: WebElement):
             actions = ActionChains(self._webdriver)
             actions.move_to_element(web_element).perform()
 
-        self._action_sequence(_action)
+        self._action_sequence(_action, __name__)
 
     def context_click(self):
         def _action(web_element: WebElement):
             actions = ActionChains(self._webdriver)
             actions.context_click(web_element).perform()
 
-        self._action_sequence(_action)
+        self._action_sequence(_action, __name__)
 
     def long_click(self):
         def _action(web_element: WebElement):
             actions = ActionChains(self._webdriver)
             actions.click_and_hold(web_element).perform()
 
-        self._action_sequence(_action)
+        self._action_sequence(_action, __name__)
 
     def double_click(self):
         def _action(web_element: WebElement):
             actions = ActionChains(self._webdriver)
             actions.double_click(web_element).perform()
 
-        self._action_sequence(_action)
+        self._action_sequence(_action, __name__)
 
     def drag_and_drop_to(self, target_ui_element: "UiElement"):
         def _action(source: WebElement):
             def _target_found(target: WebElement):
                 actions = ActionChains(self._webdriver)
                 actions.drag_and_drop(source, target).perform()
             target_ui_element.find_web_element(_target_found)
 
-        self._action_sequence(_action)
+        self._action_sequence(_action, __name__)
 
     @property
     def expect(self):
         return UiElementAssertion(self)
 
     @property
     def wait_for(self):
         return UiElementAssertion(self, raise_exception=False)
 
     def clear(self):
-        self._action_sequence(lambda web_element: web_element.clear())
+        self._action_sequence(lambda web_element: web_element.clear(), __name__)
         return self
 
     def submit(self):
-        self._action_sequence(lambda web_element: web_element.submit())
+        self._action_sequence(lambda web_element: web_element.submit(), __name__)
         return self
 
     def __str__(self):
         return self.name
 
     @property
     def name(self):
         return f"UiElement({self._by.__str__()})[{self._index}]"
 
     def scroll_into_view(self, x: int = 0, y: int = 0):
-        self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, Point(x, y)))
+        self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, Point(x, y)), __name__)
 
     def scroll_to_top(self, x: int = 0, y: int = 0):
-        self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, Point(x, y)))
+        self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, Point(x, y)), __name__)
 
     def _count_elements(self):
         count = 0
 
         def _count(web_elements: List[WebElement]):
             nonlocal count
             count = len(web_elements)
@@ -332,66 +338,61 @@
             webdriver=self._webdriver,
             by=self._by,
             parent=self._parent,
             index=index
         )
 
 
-A = TypeVar('A')
-
 class UiElementAssertion:
 
     def __init__(
         self,
         ui_element: UiElement,
         raise_exception: bool = True,
     ):
         self._ui_element = ui_element
         self._raise = raise_exception
 
     def _map_web_element_property(
         self,
-        assertion_class: Type[A],
+        assertion_class: Type[ASSERTION],
         mapper: Mapper[WebElement, any],
         property_name: str
-    ) -> A:
+    ) -> ASSERTION:
         return assertion_class(
-            parent=None,
-            actual=lambda: self._ui_element.find_web_element(mapper),
-            subject=lambda: f"{self._ui_element.name_path}.{property_name} {Format.param(self._ui_element.find_web_element(mapper))}",
+            parent=self._ui_element,
+            actual_supplier=lambda: self._ui_element.find_web_element(mapper),
+            name_supplier=lambda: f".{property_name} {Format.param(self._ui_element.find_web_element(mapper))}",
             raise_exception=self._raise,
         )
 
     @property
     def text(self):
         def _map(web_element: WebElement):
             return web_element.text
 
         return self._map_web_element_property(StringAssertion, _map, "text")
 
-    @property
-    def displayed(self):
+    def displayed(self, expected: bool):
         def _map(web_element: WebElement):
             return web_element.is_displayed()
 
-        return self._map_web_element_property(BinaryAssertion, _map, "displayed")
+        return self._map_web_element_property(BinaryAssertion, _map, "displayed").be(expected)
 
-    @property
-    def enabled(self):
+    def enabled(self, expected: bool):
         def _map(web_element: WebElement):
             return web_element.is_enabled()
 
-        return self._map_web_element_property(BinaryAssertion, _map, "enabled")
+        return self._map_web_element_property(BinaryAssertion, _map, "enabled").be(expected)
 
-    @property
-    def selected(self):
+    def selected(self, expected: bool):
         def _map(web_element: WebElement):
             return web_element.is_selected()
 
-        return self._map_web_element_property(BinaryAssertion, _map, "selected")
+        return self._map_web_element_property(BinaryAssertion, _map, "selected").be(expected)
 
     @property
     def tag_name(self):
         def _map(web_element: WebElement):
             return web_element.tag_name
 
         return self._map_web_element_property(StringAssertion, _map, "tag name")
@@ -410,47 +411,45 @@
             return web_element.value_of_css_property(property_name)
 
         return self._map_web_element_property(StringAssertion, _map, f"css({property_name}")
 
     def classes(self, *classes):
         return self.attribute(Attribute.CLASS).has_words(*classes)
 
-    @property
-    def visible(self):
-        return self._visible(False)
+    def visible(self, expected: bool):
+        return self._visible(expected, False)
 
-    @property
-    def fully_visible(self):
-        return self._visible(True)
+    def fully_visible(self, expected: bool):
+        return self._visible(expected, True)
 
-    def _visible(self, fully: bool = False):
+    def _visible(self, expected: bool, fully: bool = False):
         def _map(web_element: WebElement):
             viewport = script.get_viewport(self._ui_element._webdriver)
             bounds = Rect.from_web_element(web_element)
             if fully:
                 return viewport.contains(bounds)
             else:
                 return viewport.intersects(bounds)
 
         name = "visible"
         if fully:
             name = f"fully {name}"
 
-        return self._map_web_element_property(BinaryAssertion, _map, name)
+        return self._map_web_element_property(BinaryAssertion, _map, name).be(expected)
 
     @property
     def value(self):
         return self.attribute("value")
 
     @property
     def count(self):
         return QuantityAssertion[int](
-            parent=None,
-            actual=lambda: self._ui_element._count_elements(),
-            subject=lambda: f"{self._ui_element.name_path} count {Format.param(self._ui_element._count_elements())}",
+            parent=self._ui_element,
+            actual_supplier=lambda: self._ui_element._count_elements(),
+            name_supplier=lambda: f" count {Format.param(self._ui_element._count_elements())}",
             raise_exception=self._raise,
         )
 
     @property
     def bounds(self):
         def _map(web_element: WebElement):
             return Rect.from_web_element(web_element)
```

### Comparing `python-automation-framework-0.0.8/paf/xpath.py` & `python-automation-framework-0.0.9/paf/xpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
             return self._xpath
 
         def contains(self, value: any):
             self._attribute_matches("contains", self._attribute, value)
             return self._xpath
 
         def has_words(self, *words: any):
-            if not isinstance(words, Iterable):
-                words = [words]
+            # if not isinstance(words, Iterable):
+            #     words = [words]
             self._attribute_contains_words(self._attribute, words)
             return self._xpath
 
         def starts_with(self, value: any):
             self._attribute_matches("starts-with", self._attribute, value)
             return self._xpath
 
@@ -104,28 +104,31 @@
         self._encloses.append(xpath)
         return xpath
 
     @staticmethod
     def _is_function(attribute: str):
         return attribute.strip().endswith(")")
 
-    def attribute(self, attribute: str):
+    def attribute(self, attribute: str | Attribute):
+        if isinstance(attribute, Attribute):
+            attribute = attribute.value
+
         if not XPath._is_function(attribute):
             attribute = f"@{attribute}"
 
         return XPath.Test(self, attribute)
 
     def id(self, value: str):
-        return self.attribute(Attribute.ID.value).be(value)
+        return self.attribute(Attribute.ID).be(value)
 
     def name(self, value: str):
-        return self.attribute(Attribute.NAME.value).be(value)
+        return self.attribute(Attribute.NAME).be(value)
 
     def classes(self, *classes: any):
-        return self.attribute(Attribute.CLASS.value).has_words(*classes)
+        return self.attribute(Attribute.CLASS).has_words(*classes)
 
     @property
     def text(self):
         return XPath.Test(self, ".//text()")
 
     @staticmethod
     def _translate_sub_selection(selector: str):
@@ -163,20 +166,20 @@
     def _something_contains_word(something: str, string: any):
         return f"contains(concat(' ', normalize-space({something}), ' '), ' {string} ')"
 
     @staticmethod
     def _something_is(something: str, value: any):
         return f"{something}='{value}'"
 
-    @staticmethod
-    def _something_is_not(something: str, value: any):
-        return f"{something}!='{value}'"
+    # @staticmethod
+    # def _something_is_not(something: str, value: any):
+    #     return f"{something}!='{value}'"
 
     @staticmethod
-    def _something_matches(operation:str, something: str, value: any):
+    def _something_matches(operation: str, something: str, value: any):
         return f"{operation}({something},'{value}')"
 
     def _build(self):
         xpath = self._selector
         attributes = self._attributes.copy()
         for encloses in self._encloses:
             attributes.append(encloses._build())
```

### Comparing `python-automation-framework-0.0.8/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.0.9/python_automation_framework.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
+![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-automation-framework/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
+
+
 # PAF - Python Automation Framework
 
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
@@ -56,30 +60,34 @@
 
 ## Feature list
 
 - [UiElements](doc/uielement.md)
 - [Locators](doc/locators.md)
 - [Page objects](doc/pages.md)
 - [Components](doc/components.md)
-- [Managing WebDrivers](doc/webdriver.md)
+- [Managing WebDrivers](doc/manager.md)
 - [Execution controlling](doc/control.md)
+- [Inject listener](doc/listener.md)
 
-### Missing features (todos)
+### Missing features (tdb)
 
 - Rect assertions
 - ShadowRoot support
 - Drag & Drop over frames
 
 ## Environment variables
 
+The value behind the variable is the default value.
+
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
 * `PAF_SEQUENCE_WAIT_AFTER_FAIL=0.3`: Wait in seconds whenever a sequence action fails. 
 * `PAF_SEQUENCE_RETRY_COUNT=3`: Retry count for every sequence action.
+* `PAF_DEMO_MODE=0`: Enables the demo mode by highlighting actions and assertions.
 
 ## Examples
 
 I added two examples.
 
 1. [test_google.py](examples/test_google.py): is a regular Google search, implemented with [Page Objects](doc/pages.md) and [Components](doc/components.md). 
 2. [test_todo_mvc.py](examples/test_todo_mvc.py): are re-implemented test cases from the [Robot Framework TodoMVC](https://docs.robotframework.org/docs/examples/todo) example. It's IMHO developer friendly, better readable and less code. 
@@ -88,45 +96,66 @@
 ## Comparison
 
 Comparison of the syntax with other frameworks.
 
 **Pylenium**
 ```python
 py.get("a[href='/about']").should().have_text("About")
-```
-```python
+
 find("a[href='/about']").expect.text.be("About")
 ```
 **SeleniumBase**
 ```python
 self.assert_text_not_visible("Thanks for your purchase.", "#app .success")
-```
-```python
+
 find("#app .success").expect.text.not_be("Thanks for your purchase.")
 ```
 **Selene**
 ```python
 browser.all('#rso>div').should(have.size_greater_than(5)) \
     .first.should(have.text('Selenium automates browsers'))
-```
-```python
+
 div = find("#rso>div")
 div.expect.count.greater_than(5).be(True)
 div.first.expect.text.be("Selenium automates browsers")
 ```
 
 References: https://www.nextgenerationautomation.com/post/python-test-automation-frameworks
 
 ## Developer area
-### Run the tests
+
+### Testing
+#### Run the tests on you local machine
 ```shell
-PYTHONPATH="." pytest --numprocesses=4 --cov=paf test
+pytest --cov=paf -n=4 test
 ```
 
-### Utils
+#### Build test base container (for use in GitHub Actions)
+```shell
+podman build -f base.Dockerfile --arch=amd64 -t paf-test-base:latest
+echo $DOCKER_CONTAINER_REGISTRY_TOKEN | podman login -u mreiche --password-stdin ghcr.io
+podman push paf-test-base:latest docker://ghcr.io/mreiche/paf-test-base:latest
+```
+
+#### Build test runner container (for testing)
+```shell
+podman build -f test.Dockerfile --arch=amd64 -t paf-test:latest
+```
+Run tests within container
+```shell
+podman run paf-test:latest PAF_TEST_HEADLESS=1 PAF_TEST_CONTAINER=1 pytest --cov=paf -n=4 test
+```
+
+#### Run local selenium server
+```shell
+wget https://github.com/SeleniumHQ/selenium/releases/download/selenium-4.9.0/selenium-server-4.9.0.jar -O selenium-server.jar
+java -jar selenium-server.jar standalone --host 127.0.0.1
+```
+
+### Debug XPaths in Browser's Developer Console
 
 ```javascript
 xpath = "//dt[.//text()='Title:']/following-sibling::dd[1]"
 snapshot = document.evaluate(xpath, document.body, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE)
 snapshot.snapshotItem(0).textContent
 ```
 
@@ -136,7 +165,12 @@
     ```shell
     python setup.py sdist
     ```
 3. Publish library
     ```shell
     twine upload dist/python-automation-framework-[version].tar.gz
     ```
+
+### References
+- https://stackoverflow.com/questions/64033686/how-can-i-use-private-docker-image-in-github-actions
+- https://tecadmin.net/setup-selenium-chromedriver-on-ubuntu/
+- https://stackoverflow.com/questions/46052736/python-proxy-class
```

### Comparing `python-automation-framework-0.0.8/setup.py` & `python-automation-framework-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.8",
+    version="0.0.9",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.0.8/test/test_component.py` & `python-automation-framework-0.0.9/test/test_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import pytest
 
 from paf.component import Component
 from paf.locator import By
 from paf.manager import WebDriverManager
 from paf.page import Page, PageFactory
 from paf.xpath import XPath
+from test import create_webdriver
 
 
 @pytest.fixture
 def components_page():
-    yield inject.instance(PageFactory).create_page(ComponentsPage)
+    yield inject.instance(PageFactory).create_page(ComponentsPage, create_webdriver())
 
 
 class ComponentsPage(Page):
     @property
     @cache
     def custom_component(self):
         return self._create_component(MyComponent, self._find(By.tag_name("body")))
@@ -45,19 +46,19 @@
 def test_component_list_name(components_page: ComponentsPage):
     assert components_page.custom_component.last.name_path == "ComponentsPage > MyComponent > UiElement(By.tag name(body))[-1]"
 
 
 def test_component_list(components_page: ComponentsPage):
     components_page.open("https://testpages.herokuapp.com/styled/tag/dynamic-table.html")
     rows = components_page.table_row
-    assert rows.name_path == "ComponentsPage > TableRow > UiElement(By.xpath(//table[@ID='dynamictable']//tr))[0]"
+    assert rows.name_path == "ComponentsPage > TableRow > UiElement(By.xpath(//table[@id='dynamictable']//tr))[0]"
     rows.expect.count.be(3)
     rows.first.col.first.expect.text.be("name")
     rows.first.col.last.expect.text.be("age")
-
+    assert rows.last.col.first.wait_for.text.be("George")
     rows.last.col.last.expect.text.be("42")
 
     for row in rows:
         row.highlight()
 
 
 def teardown_module():
```

### Comparing `python-automation-framework-0.0.8/test/test_request.py` & `python-automation-framework-0.0.9/test/test_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from urllib.parse import ParseResult
 
+import inject
+
 from paf.manager import WebDriverManager
 from paf.request import WebDriverRequest
-from selenium.webdriver import ChromeOptions, Remote
-import inject
 
 
 def test_browser(monkeypatch):
     monkeypatch.setenv('PAF_BROWSER_SETTING', 'firefox')
     request = WebDriverRequest()
     assert request.browser == "firefox"
 
@@ -25,31 +25,16 @@
 def test_window_size(monkeypatch):
     monkeypatch.setenv('PAF_WINDOW_SIZE', '1024x768')
     request = WebDriverRequest()
     assert request.window_size.width == 1024
     assert request.window_size.height == 768
 
 
-def test_chrome_options():
-    request = WebDriverRequest()
-    request.browser = "chrome"
-    request.options = ChromeOptions()
-    manager = inject.instance(WebDriverManager)
-    webdriver = manager.get_webdriver(request)
-    assert webdriver.name == request.browser
-
-
-def test_remote_webdriver(monkeypatch):
-    server_url = "http://127.0.0.1:4444"
-    monkeypatch.setenv('PAF_SELENIUM_SERVER_URL', server_url)
-    request = WebDriverRequest()
+def test_server_url(monkeypatch):
+    monkeypatch.setenv('PAF_SELENIUM_SERVER_URL', "http://127.0.0.1:4444")
+    request = WebDriverRequest("remote")
     request.browser = "chrome"
-    request.options = ChromeOptions()
     assert isinstance(request.server_url, ParseResult)
-    manager = inject.instance(WebDriverManager)
-    webdriver = manager.get_webdriver(request)
-    assert webdriver.name == request.browser
 
 
 def teardown_module():
-    manager = inject.instance(WebDriverManager)
-    manager.shutdown_all()
+    inject.instance(WebDriverManager).shutdown_all()
```

### Comparing `python-automation-framework-0.0.8/test/test_uielement.py` & `python-automation-framework-0.0.9/test/test_uielement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import inject
 import pytest
-from selenium.webdriver.remote.webdriver import WebDriver, BaseWebDriver
 from selenium.webdriver.support.color import Color
 
 from paf.control import Control
 from paf.locator import By
 from paf.manager import WebDriverManager
 from paf.page import PageFactory, FinderPage
+from paf.uielement import UiElement
 from paf.xpath import XPath
 from test import create_webdriver
 
-page_factory: PageFactory = None
-
-
-def setup_module():
-    global page_factory
-    page_factory = inject.instance(PageFactory)
-
 
 @pytest.fixture
 def finder():
+    page_factory = inject.instance(PageFactory)
     finder = page_factory.create_page(FinderPage, create_webdriver())
     yield finder
 
 
-def test_finder_page(finder: FinderPage):
+def test_basics(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     assert p.name_path == 'UiElement(By.id(para1))[0]'
     assert p.name == p.name_path
-    assert isinstance(finder.webdriver, BaseWebDriver)
+    assert str(p) == p.name
+    assert finder.webdriver == p.webdriver
+
+    centered = finder.find(".centered")
+    p2 = centered.find("#para2")
+
+    assert p2.name == "UiElement(By.css selector(#para2))[0]"
+    assert p2.name_path == "UiElement(By.css selector(.centered))[0] > " + p2.name
 
 
 # def test_rect():
 #     finder = page_factory.create_page(FinderPage, create_webdriver())
 #     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 #
 #     p = finder.find(By.id("para1"))
@@ -57,14 +58,15 @@
 
     text = p.expect.text
     text.be("A paragraph of text")
     text.map(str.upper).be("A PARAGRAPH OF TEXT")
     text.not_be("Bla")
     text.contains("paragraph").be(True)
     text.has_words("paragraph", "text").be(True)
+    text.has_words("bla").be(False)
     text.starts_with("A").be(True)
     text.ends_with("text").be(True)
     text.matches("hello").be(False)
     assert text.actual == "A paragraph of text"
 
     length = p.expect.text.length
     length.be(19)
@@ -72,14 +74,29 @@
     length.greater_equal_than(10).be(True)
     length.lower_than(20).be(True)
     length.lower_equal_than(30).be(True)
     length.between(18, 20).be(True)
     length.not_be(30)
 
 
+def test_text_assertion_fails(finder: FinderPage):
+    with pytest.raises(AssertionError) as e:
+        finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
+        p = finder.find("#para1")
+        p.expect.attribute("data").be("null")
+
+    assert "Expected UiElement(By.css selector(#para1))[0].attribute(data) *undefined* to be [null] after 3 retries" in \
+           e.value.args[0]
+
+
+def test_untested_assertion_raises(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
+    title = finder.expect.title
+
+
 def test_wait(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find("#para1")
 
     assert p.wait_for.tag_name.be("p") is True
     assert p.wait_for.tag_name.be("b") is False
@@ -93,39 +110,38 @@
     p.expect.css("outline").be("rgb(0, 255, 0) solid 5px")
 
 
 def test_scroll_to_visible(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
 
     p = finder.find(By.id("pre1").unique)
-    p.expect.visible.be(False)
+    p.expect.visible(False)
     p.scroll_into_view()
-    p.expect.visible.be(True)
-    p.expect.fully_visible.be(True)
+    p.expect.visible(True)
+    p.expect.fully_visible(True)
 
     first = finder.find("#p1")
-    first.expect.visible.be(False)
+    first.expect.visible(False)
     first.scroll_to_top()
-    first.expect.visible.be(True)
-    p.expect.visible.be(False)
+    first.expect.visible(True)
+    p.expect.visible(False)
 
 
 def test_find_sub_elements_list(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
 
     # Sub elements
     div = finder.find("#div1")
     p = div.find("p")
     p.expect.attribute("name").be("pName1")
 
     # Find sub element by XPath
     p2 = div.find(XPath.at("p"))
     p2.expect.attribute("name").be("pName1")
 
-
     # Correct XPAth
     div.find(By.xpath("//p")).expect.attribute("name").be("pName1")
     div.find(By.xpath("./p")).expect.attribute("name").be("pName1")
 
     # List
     p.first.expect.attribute("name").be("pName1")
     p[1].expect.attribute("name").be("pName2")
@@ -136,28 +152,34 @@
         break
 
 
 def test_form(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-html-form-test.html")
 
     checkbox = finder.find(XPath.at("input").name("checkboxes[]").attribute("value").be("cb3"))
-    checkbox.expect.selected.be(True)
+    checkbox.expect.selected(True)
 
     textarea = finder.find(By.name("comments"))
     textarea.expect.value.be("Comments...")
     textarea.type("Hello World")
     textarea.expect.value.be("Hello World")
 
     username = finder.find(By.name("username"))
-    username.expect.enabled.be(True)
+    username.expect.enabled(True)
     username.send_keys("My Name")
     username.expect.value.be("My Name")
     username.clear()
     username.expect.value.be("")
 
+    form = finder.find("#HTMLFormElements")
+    form.submit()
+
+    # From Textarea
+    finder.find("#_valuecomments").expect.text.be("Hello World")
+
 
 def test_screenshot(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
     p = finder.find(By.id("pre1").unique)
     path = p.take_screenshot()
     assert path
 
@@ -165,43 +187,54 @@
 def test_retry(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/key-click-display-test.html")
     btn = finder.find(By.id("button").unique)
     clicks = finder.find(XPath.at("div").id("events").select("p"))
 
     control = inject.instance(Control)
     btn.click()
-    control.retry(lambda: clicks.expect.count.be(3), lambda: btn.click(), wait_after_fail=0, count=3)
+    control.retry(
+        action=lambda: clicks.expect.count.be(3),
+        on_fail=lambda e: btn.click(),
+        wait_after_fail=0,
+        count=3
+    )
 
 
 def test_actions(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/events/javascript-events.html")
 
     click_btn = finder.find("#onclick")
     click_status = finder.find("#onclickstatus")
-    click_status.expect.displayed.be(False)
+    click_status.expect.displayed(False)
     click_btn.click()
-    click_status.expect.displayed.be(True)
+    click_status.expect.displayed(True)
 
     hover_btn = finder.find("#onmouseover")
     hover_status = finder.find("#onmouseoverstatus")
-    hover_status.expect.displayed.be(False)
+    hover_status.expect.displayed(False)
     hover_btn.hover()
-    hover_status.expect.displayed.be(True)
+    hover_status.expect.displayed(True)
 
     context_btn = finder.find("#oncontextmenu")
     context_status = finder.find("#oncontextmenustatus")
-    context_status.expect.displayed.be(False)
+    context_status.expect.displayed(False)
     context_btn.context_click()
-    context_status.expect.displayed.be(True)
+    context_status.expect.displayed(True)
 
     double_click_btn = finder.find("#ondoubleclick")
     double_click_status = finder.find("#ondoubleclickstatus")
-    double_click_status.expect.displayed.be(False)
+    double_click_status.expect.displayed(False)
     double_click_btn.double_click()
-    double_click_status.expect.displayed.be(True)
+    double_click_status.expect.displayed(True)
+
+    mouse_down_btn = finder.find("#onmousedown")
+    mouse_down_status = finder.find("#onmousedownstatus")
+    mouse_down_status.expect.displayed(False)
+    mouse_down_btn.long_click()
+    mouse_down_status.expect.displayed(True)
 
 
 def test_drag_and_drop(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/drag-drop-javascript.html")
 
     drag = finder.find(".drag.left")
     drop = finder.find("#droppable1")
@@ -228,9 +261,49 @@
     btn = finder.find("#fakealert")
 
     ok.expect.count.be(0)
     btn.click()
     ok.expect.count.be(1)
 
 
+def test_uninitialized_ui_element_fails(finder: FinderPage):
+    with pytest.raises(Exception) as e:
+        ui_element = UiElement(By.id("id"))
+        ui_element.click()
+
+    assert "initialized without WebDriver nor UiElement" in e.value.args[0]
+
+
+def test_action_on_non_interactable_fails(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/alerts/fake-alert-test.html")
+    ok = finder.find("#dialog-ok")
+    with pytest.raises(Exception) as e:
+        ok.click()
+
+    assert "Message: element not interactable" in e.value.args[0]
+
+
+def test_not_unique_fails(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/key-click-display-test.html")
+    btn = finder.find(By.id("button").unique)
+    btn.click()
+    btn.click()
+
+    events = finder.find("#events")
+    with pytest.raises(Exception) as e:
+        p = events.find(By.tag_name("p").unique)
+        p.expect.text.be("click")
+
+    assert "Not unique" in e.value.args[0]
+
+
+def test_not_found_fails(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
+    with pytest.raises(Exception) as e:
+        unknown = finder.find("#unkown")
+        unknown.highlight()
+
+    assert "Not found" in e.value.args[0]
+
+
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

