# Comparing `tmp/mmk_updater-0.13.1.tar.gz` & `tmp/mmk_updater-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmk_updater-0.13.1.tar", last modified: Fri Jan 13 12:08:51 2023, max compression
+gzip compressed data, was "mmk_updater-0.14.tar", last modified: Tue May  9 06:35:45 2023, max compression
```

## Comparing `mmk_updater-0.13.1.tar` & `mmk_updater-0.14.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 melianmiko  (1000) melianmiko  (1000)        0 2023-01-13 12:08:51.682621 mmk_updater-0.13.1/
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)     1067 2023-01-04 06:54:40.000000 mmk_updater-0.13.1/LICENSE
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)      217 2023-01-13 12:08:51.682621 mmk_updater-0.13.1/PKG-INFO
--rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)       80 2023-01-04 06:55:46.000000 mmk_updater-0.13.1/README.md
-drwxrwxr-x   0 melianmiko  (1000) melianmiko  (1000)        0 2023-01-13 12:08:51.682621 mmk_updater-0.13.1/mmk_updater/
--rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      102 2022-09-06 15:07:09.000000 mmk_updater-0.13.1/mmk_updater/__init__.py
--rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      325 2023-01-13 12:00:22.000000 mmk_updater-0.13.1/mmk_updater/__main__.py
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)     9012 2023-01-13 12:01:26.000000 mmk_updater-0.13.1/mmk_updater/_base.py
--rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)     1850 2022-09-06 15:07:09.000000 mmk_updater-0.13.1/mmk_updater/_lc.py
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)      230 2022-12-22 14:47:48.000000 mmk_updater-0.13.1/mmk_updater/_tools.py
--rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)     7138 2023-01-13 12:03:44.000000 mmk_updater-0.13.1/mmk_updater/ui_tkinter.py
-drwxrwxr-x   0 melianmiko  (1000) melianmiko  (1000)        0 2023-01-13 12:08:51.682621 mmk_updater-0.13.1/mmk_updater.egg-info/
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)      217 2023-01-13 12:08:51.000000 mmk_updater-0.13.1/mmk_updater.egg-info/PKG-INFO
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)      351 2023-01-13 12:08:51.000000 mmk_updater-0.13.1/mmk_updater.egg-info/SOURCES.txt
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)        1 2023-01-13 12:08:51.000000 mmk_updater-0.13.1/mmk_updater.egg-info/dependency_links.txt
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)       14 2023-01-13 12:08:51.000000 mmk_updater-0.13.1/mmk_updater.egg-info/requires.txt
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)       12 2023-01-13 12:08:51.000000 mmk_updater-0.13.1/mmk_updater.egg-info/top_level.txt
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)      386 2023-01-13 12:08:15.000000 mmk_updater-0.13.1/pyproject.toml
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)       38 2023-01-13 12:08:51.682621 mmk_updater-0.13.1/setup.cfg
--rw-rw-r--   0 melianmiko  (1000) melianmiko  (1000)       38 2023-01-13 11:51:57.000000 mmk_updater-0.13.1/setup.py
+drwxr-xr-x   0 melianmiko  (1000) melianmiko  (1000)        0 2023-05-09 06:35:45.893521 mmk_updater-0.14/
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)     1067 2023-05-09 06:01:08.000000 mmk_updater-0.14/LICENSE
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      215 2023-05-09 06:35:45.893521 mmk_updater-0.14/PKG-INFO
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)       80 2023-05-09 06:33:54.000000 mmk_updater-0.14/README.md
+drwxr-xr-x   0 melianmiko  (1000) melianmiko  (1000)        0 2023-05-09 06:35:45.893521 mmk_updater-0.14/mmk_updater/
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      102 2023-05-09 06:01:08.000000 mmk_updater-0.14/mmk_updater/__init__.py
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      328 2023-05-09 06:06:45.000000 mmk_updater-0.14/mmk_updater/__main__.py
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)     9246 2023-05-09 06:33:19.000000 mmk_updater-0.14/mmk_updater/_base.py
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)     2774 2023-05-09 06:18:33.000000 mmk_updater-0.14/mmk_updater/_lc.py
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      230 2023-05-09 06:01:08.000000 mmk_updater-0.14/mmk_updater/_tools.py
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)     7607 2023-05-09 06:22:32.000000 mmk_updater-0.14/mmk_updater/ui_tkinter.py
+drwxr-xr-x   0 melianmiko  (1000) melianmiko  (1000)        0 2023-05-09 06:35:45.893521 mmk_updater-0.14/mmk_updater.egg-info/
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      215 2023-05-09 06:35:45.000000 mmk_updater-0.14/mmk_updater.egg-info/PKG-INFO
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      351 2023-05-09 06:35:45.000000 mmk_updater-0.14/mmk_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)        1 2023-05-09 06:35:45.000000 mmk_updater-0.14/mmk_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)       14 2023-05-09 06:35:45.000000 mmk_updater-0.14/mmk_updater.egg-info/requires.txt
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)       12 2023-05-09 06:35:45.000000 mmk_updater-0.14/mmk_updater.egg-info/top_level.txt
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)      384 2023-05-09 06:33:50.000000 mmk_updater-0.14/pyproject.toml
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)       38 2023-05-09 06:35:45.893521 mmk_updater-0.14/setup.cfg
+-rw-r--r--   0 melianmiko  (1000) melianmiko  (1000)       38 2023-05-09 06:01:08.000000 mmk_updater-0.14/setup.py
```

### Comparing `mmk_updater-0.13.1/LICENSE` & `mmk_updater-0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `mmk_updater-0.13.1/mmk_updater/_base.py` & `mmk_updater-0.14/mmk_updater/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,40 +50,46 @@
 class UpdaterTool:
     def __init__(self, release_url: str, current_version: str, ui_mod: DummyUiModule):
         self.release_url = release_url
         self.current_version = current_version
         self.release_data = {}
         self.file_path = Path.home()
         self.selected_asset = None
-        self.ppa_glob = "/etc/apt/sources.list.d/melianmiko-ubuntu-software-*"
+        self.ppa_glob = "/etc/apt/sources.list.d/melianmiko-repo*"
+        self.old_ppa_glob = "/etc/apt/sources.list.d/melianmiko-ubuntu-software-*"
 
-        self.ignore_ppa = True
+        self.ignore_ppa = False
+        self.force_show = False
 
         self.ui_mod = ui_mod
         self.ui_mod.on_bind(self)
 
         self._ui_result = False
         self._on_result = threading.Event()
 
     # overridable
     def should_show_update_ui(self):
-        if self._has_ppa() and not self.ignore_ppa:
+        if self._has_ppa() and not self.ignore_ppa and not self.force_show:
             log.debug("has ppa, don't show update ui")
             return False
 
         return self.release_data["version"] != self.current_version
 
     # overridable
     def on_release_data(self):
         pass
 
     def _has_ppa(self):
         g = glob.glob(self.ppa_glob)
         return len(g) > 0
 
+    def has_old_ppa(self):
+        g = glob.glob(self.old_ppa_glob)
+        return len(g) > 0
+
     @staticmethod
     def _has_external_updater():
         return os.path.isfile("/usr/local/bin/yay") or os.path.isfile("/usr/bin/yay")
 
     def show_update_dialog(self):
         threading.Thread(target=self._run_updater_ui).start()
 
@@ -121,15 +127,15 @@
 
     # noinspection PyBroadException
     def _process(self):
         UpdaterTool.cleanup()
 
         log.debug("fetching update info...")
         try:
-            release_info = urllib.request.urlopen(self.release_url).read()
+            release_info = urllib.request.urlopen(self.release_url, timeout=5).read()
             release_info = release_info.decode("utf8")
         except Exception:
             log.exception("can't fetch release info")
             return
 
         self.release_data = json.loads(release_info)
         log.debug("latest release: " + self.release_data["version"])
```

### Comparing `mmk_updater-0.13.1/mmk_updater/_lc.py` & `mmk_updater-0.14/mmk_updater/_lc.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     "has_update_title": "New version of {} is available",
     "file_pattern": "File: {} ({})",
     "downloading": "Downloading file {}...",
     "downloading_run_after": "Installation will be started automatically after download",
     "download_btn": "Update now",
     "dl_error": "ERROR: Download failed",
     "close_btn": "Close",
+    "ppa_migration": "This application migrated from Ubuntu PPA to self-hosted Debian/Ubuntu repository.\n\n"
+                     "To receive this and other updates, you must run repository migration.\n"
+                     "This will make less than one minute, click here to get instructions.\n"
+                     "Sorry for wasting time...",
     "site_btn": "View in web browser",
     "repo_install": "Install it via system package manager.",
     "manual_install": "Update downloaded, but we can't install it automatically.\nFile "
                       "was saved to {}.\nPlease install it after app close."
 }
 
 L18N = {
@@ -20,23 +24,27 @@
         "file_pattern": "Будет загружен: {} ({})",
         "downloading": "Загружаем файл {}...",
         "downloading_run_after": "Установка начнётся сразу после загрузки",
         "download_btn": "Обновить",
         "dl_error": "ОШИБКА: Не удалось скачать файл",
         "site_btn": "Перейти на веб-сайт программы",
         "close_btn": "Закрыть",
+        "ppa_migration": "Это приложение было перенесено с Ubuntu PPA на собственный репозиторий.\n\n"
+                         "Чтобы получить это и последующие обновления, выполните замену подключенного\n"
+                         "репозитория. Это займёт одну минуту, нажмите сюда для получения инструкций..\n"
+                         "Извините за потраченное время...",
         "repo_install": "Установите обновление ч-з системный пакетный менеджер",
         "manual_install": "Обновление загружено, но мы не можем установить его автоматически.\nФайл "
                           "сохранён по пути {}. \nУстановите его, когда будет возможность."
     }
 }
 
 
 def t(k):
-    lang = locale.getdefaultlocale()[0]
+    lang = locale.getlocale()[0]
     if lang in L18N:
         if k in L18N[lang]:
             return L18N[lang][k]
 
     if k in BASE_LOCALE:
         return BASE_LOCALE[k]
     return k
```

### Comparing `mmk_updater-0.13.1/mmk_updater/ui_tkinter.py` & `mmk_updater-0.14/mmk_updater/ui_tkinter.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,24 @@
             root.wm_title("Updater")
 
             frame = ttk.Frame(root)
             frame.grid()
 
             self._add_base_update_info(frame, 1)
 
-            ttk.Label(frame, text=t("repo_install"), justify=tkinter.LEFT) \
-                .grid(column=0, row=4, columnspan=3, padx=16, pady=4, sticky=tkinter.NW)
+            if self.updater.has_old_ppa():
+                link = ttk.Label(frame, text=t("ppa_migration"),
+                                 foreground="#FF5500",
+                                 cursor="hand2")
+                link.bind("<Button-1>", self._open_old_ppa_guide)
+                link.grid(column=0, row=4, padx=16, pady=4, columnspan=3, sticky=tkinter.NW)
+            else:
+                ttk.Label(frame, text=t("repo_install"), justify=tkinter.LEFT) \
+                    .grid(column=0, row=4, columnspan=3, padx=16, pady=4, sticky=tkinter.NW)
+
             ttk.Button(frame, text=t("close_btn"), command=root.destroy) \
                 .grid(column=0, row=5, padx=4, pady=4, sticky=tkinter.NW)
 
         self.init_tk().after_idle(_internal)
 
     def show_download_progress(self):
         ready = threading.Event()
@@ -190,10 +198,12 @@
             link.grid(column=0, row=3, padx=16, pady=4, columnspan=columns, sticky=tkinter.NW)
 
     def _close_download_bar(self):
         self.init_tk().after_idle(self.tk_dl_root.destroy)
         self.tk_dl_root = None
         self.tk_progress = None
 
-    # noinspection PyUnusedLocal
-    def _open_site(self, ev):
+    def _open_old_ppa_guide(self, _):
+        webbrowser.open("https://melianmiko.ru/en/ppa_migration")
+
+    def _open_site(self, _):
         webbrowser.open(self.updater.release_data["website"])
```

