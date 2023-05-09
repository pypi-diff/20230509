# Comparing `tmp/fastapi_amis_admin_cli-0.1.0.tar.gz` & `tmp/fastapi_amis_admin_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_cli-0.1.0.tar", last modified: Fri Jul  1 06:22:31 2022, max compression
+gzip compressed data, was "fastapi_amis_admin_cli-0.1.1.tar", last modified: Tue May  9 08:56:39 2023, max compression
```

## Comparing `fastapi_amis_admin_cli-0.1.0.tar` & `fastapi_amis_admin_cli-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0     2133 2022-05-28 14:54:13.197420 fastapi_amis_admin_cli-0.1.0/.gitignore
--rw-r--r--   0        0        0    11558 2022-01-15 16:24:21.399000 fastapi_amis_admin_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     1256 2022-05-28 15:32:35.402638 fastapi_amis_admin_cli-0.1.0/README.md
--rw-r--r--   0        0        0      100 2022-05-28 08:45:24.064128 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/cookiecutter.json
--rw-r--r--   0        0        0      246 2022-05-26 13:08:32.004411 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/__init__.py
--rw-r--r--   0        0        0      750 2022-06-10 14:16:35.813439 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py
--rw-r--r--   0        0        0      206 2022-05-26 09:10:18.482391 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/apis.py
--rw-r--r--   0        0        0        0 2022-05-27 06:19:18.767737 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/crud.py
--rw-r--r--   0        0        0      686 2022-05-26 04:36:33.170207 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py
--rw-r--r--   0        0        0      695 2022-06-10 14:16:35.771475 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/models.py
--rw-r--r--   0        0        0       68 2022-05-26 03:27:12.416572 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/schemas.py
--rw-r--r--   0        0        0       26 2022-05-23 09:29:33.512434 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/tests.py
--rw-r--r--   0        0        0      368 2022-05-28 09:03:59.195000 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/cookiecutter.json
--rw-r--r--   0        0        0      391 2022-05-30 13:59:02.924301 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/Dockerfile
--rw-r--r--   0        0        0      471 2022-06-04 08:50:13.068278 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/README.md
--rw-r--r--   0        0        0      398 2022-06-30 10:12:58.263623 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/.env
--rw-r--r--   0        0        0        0 2022-05-12 08:47:40.318000 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/apps/__init__.py
--rw-r--r--   0        0        0      110 2022-05-23 02:16:40.221000 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/__init__.py
--rw-r--r--   0        0        0      435 2022-06-10 14:16:35.825432 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/adminsite.py
--rw-r--r--   0        0        0      490 2022-06-10 14:16:35.798451 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/settings.py
--rw-r--r--   0        0        0     1897 2022-07-01 05:24:53.592696 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py
--rw-r--r--   0        0        0      275 2022-07-01 06:21:07.870970 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/requirements.txt
--rw-r--r--   0        0        0      378 2022-05-30 14:00:21.016996 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/docker-compose.yml
--rw-r--r--   0        0        0      955 2022-05-31 09:28:03.032714 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/scripts/run.sh
--rw-r--r--   0        0        0       83 2022-06-30 10:24:45.442878 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 14:40:55.873535 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/commands/__init__.py
--rw-r--r--   0        0        0     2179 2022-05-29 06:22:14.723065 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/commands/main.py
--rw-r--r--   0        0        0     1674 2022-07-01 06:13:04.760726 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/commands/project.py
--rw-r--r--   0        0        0     2288 2022-05-29 07:03:13.849707 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/commands/utils.py
--rw-r--r--   0        0        0       74 2022-05-28 12:31:29.770843 fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/main.py
--rw-r--r--   0        0        0     1458 2022-05-26 15:17:01.743294 fastapi_amis_admin_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 fastapi_amis_admin_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1256 2022-05-28 15:32:35.402638 fastapi_amis_admin_cli-0.1.1/README.md
+-rw-r--r--   0        0        0      100 2022-05-28 08:45:24.064128 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/cookiecutter.json
+-rw-r--r--   0        0        0      422 2023-05-09 01:50:53.209469 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/__init__.py
+-rw-r--r--   0        0        0      669 2023-05-09 01:50:53.220445 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py
+-rw-r--r--   0        0        0      143 2022-08-13 16:02:30.396212 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/apis.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:19:18.767737 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/crud.py
+-rw-r--r--   0        0        0      686 2022-05-26 04:36:33.170207 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py
+-rw-r--r--   0        0        0      652 2023-05-09 02:10:05.738379 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/models.py
+-rw-r--r--   0        0        0       68 2022-05-26 03:27:12.416572 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/schemas.py
+-rw-r--r--   0        0        0       26 2022-05-23 09:29:33.512434 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/tests.py
+-rw-r--r--   0        0        0      377 2023-05-09 01:22:34.362238 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/cookiecutter.json
+-rw-r--r--   0        0        0      391 2022-05-30 13:59:02.924301 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/Dockerfile
+-rw-r--r--   0        0        0      911 2023-05-09 08:55:47.865644 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/README.md
+-rw-r--r--   0        0        0      464 2023-05-09 01:39:10.888488 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/.env
+-rw-r--r--   0        0        0        0 2022-05-12 08:47:40.318000 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/apps/__init__.py
+-rw-r--r--   0        0        0      110 2022-05-23 02:16:40.221000 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/__init__.py
+-rw-r--r--   0        0        0      435 2022-06-10 14:16:35.825432 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/adminsite.py
+-rw-r--r--   0        0        0      490 2022-06-10 14:16:35.798451 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/core/settings.py
+-rw-r--r--   0        0        0     1801 2023-05-09 01:52:17.958788 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py
+-rw-r--r--   0        0        0      269 2023-05-09 08:29:07.400258 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/requirements.txt
+-rw-r--r--   0        0        0      378 2022-05-30 14:00:21.016996 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/docker-compose.yml
+-rw-r--r--   0        0        0     1815 2023-05-09 08:08:21.181729 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-05-09 08:17:24.867753 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-26 14:40:55.873535 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/__init__.py
+-rw-r--r--   0        0        0     2983 2023-05-09 08:41:28.975785 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/main.py
+-rw-r--r--   0        0        0     1674 2022-07-01 06:13:04.760726 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/project.py
+-rw-r--r--   0        0        0     2833 2023-05-09 03:37:40.520047 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/utils.py
+-rw-r--r--   0        0        0       74 2022-05-28 12:31:29.770843 fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/main.py
+-rw-r--r--   0        0        0     1494 2023-05-09 07:56:21.864863 fastapi_amis_admin_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 fastapi_amis_admin_cli-0.1.1/PKG-INFO
```

### Comparing `fastapi_amis_admin_cli-0.1.0/README.md` & `fastapi_amis_admin_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py` & `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from fastapi_amis_admin import amis,admin
+from fastapi_amis_admin import amis, admin
 from fastapi_amis_admin.admin import AdminApp
 
-from core.adminsite import site
 # from .models import Category
 
 
-@site.register_admin
 class {{cookiecutter.slug|capitalize}}App(admin.AdminApp):
     page_schema = amis.PageSchema(label='{{cookiecutter.name|capitalize}}', icon='fa fa-bolt')
     router_prefix = '/{{cookiecutter.slug}}'
 
     def __init__(self, app: "AdminApp"):
         super().__init__(app)
         # self.register_admin(CategoryAdmin)
 
 
 # Register your models here.
 
 # class CategoryAdmin(admin.ModelAdmin):
-#     group_schema = None
 #     page_schema = amis.PageSchema(label='Category', icon='fa fa-folder')
 #     model = Category
 #     search_fields = [Category.name]
```

### Comparing `fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py` & `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/App/{{cookiecutter.slug}}/jobs.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py` & `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/Project/{{cookiecutter.slug}}/backend/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from core.adminsite import site
 from core.settings import settings
 
 app = FastAPI(debug=settings.debug)
 
 # 安装应用
 from apps import {{ cookiecutter.app_slug }}
-{{ cookiecutter.app_slug }}.setup(app)
+{{ cookiecutter.app_slug }}.setup(app.router,site)
 
 # 挂载后台管理系统
 site.mount_app(app)
 
 
 @app.on_event("startup")
 async def startup():
 {% if cookiecutter.use_user_auth == "True" %}
     from core.adminsite import auth
     await site.db.async_run_sync(SQLModel.metadata.create_all, is_session=False)
-    await auth.create_role_user(role_key='admin')
-    await auth.create_role_user(role_key='vip')
-    await auth.create_role_user(role_key='test')
+    await auth.create_role_user('admin')
 {% endif %}
 {% if cookiecutter.use_scheduler == "True" %}
     from core.adminsite import scheduler
     scheduler.start()
 {% else %}
     pass
 {% endif %}
```

### Comparing `fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/commands/project.py` & `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_cli-0.1.0/fastapi_amis_admin_cli/commands/utils.py` & `fastapi_amis_admin_cli-0.1.1/fastapi_amis_admin_cli/commands/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 from typing import Optional, List, TypeVar, Dict, Any, Union
 
 import typer
 from click import Choice
 
 
 def get_language() -> str:
-    language = os.getenv('LANGUAGE') or os.getenv('LANG') or locale.getdefaultlocale()[0]
-    return 'zh_CN' if language.lower().startswith('zh') else 'en_US'
+    language = os.getenv('LANGUAGE') or os.getenv('LANG') or locale.getdefaultlocale()[0] or "en_US"
+    return 'zh_CN' if language.lower().startswith('zh') else language
 
 
+@functools.lru_cache()
 def get_settings() -> Dict[str, Any]:
     backend = get_backend_path(must=True)
-    sys.path.append(str(backend.resolve()))
+    sys.path.append(str(backend))
+    os.chdir(backend)  # 切换到backend目录
     try:
-        settings = importlib.import_module('core.settings')
+        module = importlib.import_module('core.settings')
     except ImportError as e:
         return {}
-    return settings.settings.dict()
+    return module.settings.dict()
+
+
+def get_setting_value(key: str, default: Any = None) -> Any:
+    return get_settings().get(key, default)
 
 
 _VT = TypeVar("_VT")
 
 
 def list_prompt(text: str, lst: List[_VT], default: _VT = None, **kwargs) -> _VT:
     if not lst:
@@ -42,33 +48,46 @@
     return lst[int(index)]
 
 
 @functools.lru_cache()
 def get_backend_path(must: bool = False) -> Optional[Path]:
     path = Path('.')
     if (path / "core/__init__.py").is_file() and str(path.resolve()).endswith('backend'):
-        return path
+        return path.resolve()
     lst = [
         p.parent.parent for p in path.glob("**/backend/core/__init__.py")
         if p.is_file() and '{{cookiecutter.slug}}' not in str(p)
     ]
     path = list_prompt("Where is the backend path?", lst)
     if not path and must:
         while True:
             path: Path = typer.prompt("Where is the backend path?", type=Path)
             if (path / "core/__init__.py").is_file():
                 break
             else:
                 typer.secho("Cannot find backend in current folder!", fg=typer.colors.RED)
-    return path
+    return path.resolve() if path else None
 
 
 def check_requirement(name: str, install: Union[str, bool] = False) -> bool:
     try:
         importlib.import_module(name)
         return True
     except ImportError:
         if install:
             name = name if install is True else install
             os.system(f'pip install {name}')
             return True
         return False
+
+
+def kill_port(port):
+    import psutil
+
+    for proc in psutil.process_iter():
+        if proc.name().find("python") == -1:
+            continue
+        for conns in proc.connections(kind="inet"):
+            if conns.laddr.port == port:
+                proc.kill()
+                return proc
+    return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastapi_amis_admin_cli-0.1.0/pyproject.toml` & `fastapi_amis_admin_cli-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,22 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "typer",
-    "cookiecutter",
+    "typer>=0.9.0",
+    "cookiecutter>=2.1.1",
+    "psutil>=5.9.5",
 ]
 
 [project.urls]
-Source = "https://github.com/amisadmin/fastapi_amis_admin_cli"
-FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi_amis_admin"
+Source = "https://github.com/amisadmin/fastapi-amis-admin-cli"
+FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi-amis-admin"
 
 [project.optional-dependencies]
 test = [
     "pytest >=6.2.4,<7.0.0",
 ]
 [project.scripts]
 faa = "fastapi_amis_admin_cli.main:app"
```

### Comparing `fastapi_amis_admin_cli-0.1.0/PKG-INFO` & `fastapi_amis_admin_cli-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI-Amis-Admin-Cli is an extended library for quickly building `FastAPI-Amis-Admin` projects.
 Keywords: fastapi-amis-admin-cli,fastapi-amis-admin,fastapi-user-auth,fastapi-APScheduler
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
@@ -14,19 +14,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: typer
-Requires-Dist: cookiecutter
+Requires-Dist: typer>=0.9.0
+Requires-Dist: cookiecutter>=2.1.1
+Requires-Dist: psutil>=5.9.5
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
-Project-URL: FastAPI-Amis-Admin, https://github.com/amisadmin/fastapi_amis_admin
-Project-URL: Source, https://github.com/amisadmin/fastapi_amis_admin_cli
+Project-URL: FastAPI-Amis-Admin, https://github.com/amisadmin/fastapi-amis-admin
+Project-URL: Source, https://github.com/amisadmin/fastapi-amis-admin-cli
 Provides-Extra: test
 
 <h2 align="center">
   FastAPI-Amis-Admin-Cli
 </h2>
 
 ## 项目介绍
```

