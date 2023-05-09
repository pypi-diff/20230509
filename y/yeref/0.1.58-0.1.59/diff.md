# Comparing `tmp/yeref-0.1.58.tar.gz` & `tmp/yeref-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.58.tar", last modified: Mon May  8 11:57:34 2023, max compression
+gzip compressed data, was "yeref-0.1.59.tar", last modified: Tue May  9 14:14:57 2023, max compression
```

## Comparing `yeref-0.1.58.tar` & `yeref-0.1.59.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 11:57:34.528570 yeref-0.1.58/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 11:57:34.528793 yeref-0.1.58/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-08 11:57:34.529463 yeref-0.1.58/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-08 11:57:19.000000 yeref-0.1.58/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 11:57:34.522898 yeref-0.1.58/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.58/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   508331 2023-05-08 11:56:43.000000 yeref-0.1.58/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   198722 2023-05-08 10:48:49.000000 yeref-0.1.58/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 11:57:34.528005 yeref-0.1.58/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-08 11:57:34.000000 yeref-0.1.58/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-09 14:14:57.916965 yeref-0.1.59/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-09 14:14:57.917146 yeref-0.1.59/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-09 14:14:57.917894 yeref-0.1.59/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-09 14:14:54.000000 yeref-0.1.59/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-09 14:14:57.910486 yeref-0.1.59/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.59/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   509642 2023-05-09 14:01:03.000000 yeref-0.1.59/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   198893 2023-05-08 17:51:39.000000 yeref-0.1.59/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-09 14:14:57.916303 yeref-0.1.59/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-09 14:14:57.000000 yeref-0.1.59/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-09 14:14:57.000000 yeref-0.1.59/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-09 14:14:57.000000 yeref-0.1.59/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-09 14:14:57.000000 yeref-0.1.59/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.58/setup.py` & `yeref-0.1.59/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.58',
+      version='0.1.59',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.58-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.59-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.58/yeref/l_.py` & `yeref-0.1.59/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1333,14 +1333,30 @@
     'ru': "🏞️ jpg",
     'en': "🏞️ jpg",
     'es': "🏞️ jpg",
     'fr': "🏞️jpg",
     'zh': "🏞️ jpg",
     'ar': "🏞️ jpg",
 }
+l_image_png = {
+    'ru': "🌁 png",
+    'en': "🌁 png",
+    'es': "🌁 png",
+    'fr': "🌁 png",
+    'zh': "🌁 png",
+    'ar': "🌁 png",
+}
+l_image_rbg = {
+    'ru': "🙌🏽 удалить фон",
+    'en': "🙌🏽 png",
+    'es': "🙌🏽 png",
+    'fr': "🙌🏽 png",
+    'zh': "🙌🏽 png",
+    'ar': "🙌🏽 png",
+}
 l_image_mp4 = {
     'ru': "🎥 mp4",
     'en': "🎥 mp4",
     'es': "🎥 mp4",
     'fr': "🎥 mp4",
     'zh': "🎥 mp4",
     'ar': "🎥 mp4",
@@ -1350,15 +1366,15 @@
     'en': "9️⃣ album⁹",
     'es': "9️⃣ álbum⁹",
     'fr': "9️⃣album⁹",
     'zh': "9️⃣专辑⁹",
     'ar': "9️⃣ البوم⁹",
 }
 l_image_thumb = {
-    'ru': "🖼️ thumb-nail",
+    'ru': "🖼️ thumb",
     'en': "🖼️ thumb-nail",
     'es': "🖼️ miniatura",
     'fr': "🖼️ ongle du pouce",
     'zh': "🖼️ 缩略图",
     'ar': "🖼️ الإبهام",
 }
 l_image_descpic = {
@@ -1381,14 +1397,30 @@
     'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в jpg",
     'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to jpg",
     'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a jpg",
     'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en jpg",
     'zh': "👩🏽‍💻<b>附上</b>照片以转换为jpg",
     'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى jpg",
 }
+l_image_png_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в png",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to jpg",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a jpg",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en jpg",
+    'zh': "👩🏽‍💻<b>附上</b>照片以转换为jpg",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى jpg",
+}
+l_image_rbg_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для удаления фона",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to jpg",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a jpg",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en jpg",
+    'zh': "👩🏽‍💻<b>附上</b>照片以转换为jpg",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى jpg",
+}
 l_image_mp4_attach = {
     'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в mp4 (Telegram-аватарку)",
     'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to mp4 (Telegram avatar)",
     'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a mp4 (Avatar de Telegram)",
     'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en mp4 (avatar Telegram)",
     'zh': "👩🏽‍💻<b>附上</b>要转换为mp4的照片（电报头像）",
     'ar': "👩🏽‍💻 <b>إرفاق</b> صورة لتحويلها إلى mp4 (Telegram avatar)",
```

### Comparing `yeref-0.1.58/yeref/yeref.py` & `yeref-0.1.59/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 lkjhgfdsa_channel_id = -1001657854832
 lkjhgfdsa_channel_un = "lkjhgfdsa_channel"
 tg_ch_ads_un = 'kiejakn3_djdjn4m_ads'
 tg_ch_ads_id = -1001921910898
 price_one = 200
 price_all = 500
 passwd = 'lost9'
+bin_empty = b'\xe2\x81\xa0\xe2\x81\xa0'  # .encode("utf-8")
+hex_empty = 'e281a0e281a0'  # .encode("utf-8").hex()  || bytes.fromhex()
+str_empty = bin_empty.decode('utf-8')
 
 TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
 TGPH_TOKENS = {
     'https://telegra.ph/pst-FereyDemoBot-05-08': 'f8c69d50846e8d55e08f8e3de514f41266e0150434219059f2c91fb4d75f',
     'https://telegra.ph/pst-FereyBotBot-05-08': 'e7f943fcc98bac07ad6aaf6e570d0f51abadf02567938c997dbc1ad1923b',
     'https://telegra.ph/pst-FereyPostBot-05-08': '14085be3058c0a25616d094f4bb65c73dc61f783468f01da41d99fb6ace1',
     'https://telegra.ph/pst-FereyMediaBot-05-08': 'cf71a596b7ecdc96d30ddffdbf1e26863dd39755f47b4fc343fc3867f373',
```

