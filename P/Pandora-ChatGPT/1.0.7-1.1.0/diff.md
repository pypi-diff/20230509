# Comparing `tmp/Pandora-ChatGPT-1.0.7.tar.gz` & `tmp/Pandora-ChatGPT-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-mv85qnud/Pandora-ChatGPT-1.0.7.tar", last modified: Tue Apr 25 08:50:13 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-xca5n3cu/Pandora-ChatGPT-1.1.0.tar", last modified: Tue May  9 07:51:20 2023, max compression
```

## Comparing `Pandora-ChatGPT-1.0.7.tar` & `Pandora-ChatGPT-1.1.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:50:13.000000 Pandora-ChatGPT-1.0.7/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-04-25 08:50:00.000000 Pandora-ChatGPT-1.0.7/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/exts/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:51:20.000000 Pandora-ChatGPT-1.1.0/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-09 07:51:05.000000 Pandora-ChatGPT-1.1.0/src/pandora/turbo/chat.py
```

### Comparing `Pandora-ChatGPT-1.0.7/LICENSE` & `Pandora-ChatGPT-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/PKG-INFO` & `Pandora-ChatGPT-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.0.7
+Version: 1.1.0
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
@@ -50,26 +50,28 @@
 [![Downloads](https://static.pepy.tech/badge/pandora-chatgpt)](https://pypi.python.org/pypi/pandora-chatgpt)
 [![PyPi workflow](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml)
 [![Docker workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml)
 [![Discord](https://img.shields.io/discord/1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa)
 
 ## 体验地址
 * 点击 <a href="https://chat.zhile.io" target="_blank" title="Pandora Cloud体验地址">https://chat.zhile.io</a>
-* 登录获取 `Access Token` 需要梯子。不过对IP无讲究，国家支持就行。
+* 可以访问 [这里](http://ai.fakeopen.com/auth) 拿 `Access Token`
+* 也可以官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
 * `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。
 * 这个页面上还包含一个共享账号的链接，**没有账号**的可以点进去体验一下。
  
 ## ChatGPT使用时可能会遇到：
 
 ### 1. Please stand by, while we are checking your browser... 
 ### &nbsp;&nbsp;&nbsp;动不动来一下，有时候还不动或者出人机验证。痛！
 ![t0](https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png)
 
 ### 2. Access denied. You do not have access to chat.openai.com. 
 ### &nbsp;&nbsp;&nbsp;经典问题，只能到处找可用VPN，费时费力，更费钱。移动端访问更难。痛！
+![t1.1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.1.png)
 ![t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png)
 
 ### 3. ChatGPT is at capacity right now 
 ### &nbsp;&nbsp;&nbsp;系统负载高，白嫖用户不给用。痛！
 ![t2](https://github.com/pengzhile/pandora/raw/master/doc/images/t2.png)
 
 ### 4. This content may violate our <u>content policy</u>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.0.7 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.1.0 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
@@ -30,27 +30,29 @@
 pypi.python.org/pypi/pandora-chatgpt) [![PyPi workflow](https://github.com/
 pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://
 github.com/pengzhile/pandora/actions/workflows/python-publish.yml) [![Docker
 workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-
 publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/
 docker-publish.yml) [![Discord](https://img.shields.io/discord/
 1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa) ##
-ä½éªå°å * ç¹å» https://chat.zhile.io * ç»å½è·å `Access Token`
-éè¦æ¢¯å­ãä¸è¿å¯¹IPæ è®²ç©¶ï¼å½å®¶æ¯æå°±è¡ã * `Access Token`
-æææ `14`
+ä½éªå°å * ç¹å» https://chat.zhile.io * å¯ä»¥è®¿é® [è¿é](http://
+ai.fakeopen.com/auth) æ¿ `Access Token` * ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é®
+[è¿é](http://chat.openai.com/api/auth/session) æ¿ `Access Token` * `Access
+Token` æææ `14`
 å¤©ï¼æé´è®¿é®**ä¸éè¦æ¢¯å­**ãè¿æå³çä½ å¨ææºä¸ä¹å¯éæä½¿ç¨ã
 *
 è¿ä¸ªé¡µé¢ä¸è¿åå«ä¸ä¸ªå±äº«è´¦å·çé¾æ¥ï¼**æ²¡æè´¦å·**çå¯ä»¥ç¹è¿å»ä½éªä¸ä¸ã
 ## ChatGPTä½¿ç¨æ¶å¯è½ä¼éå°ï¼ ### 1. Please stand by, while we are
 checking your browser... ###
    å¨ä¸å¨æ¥ä¸ä¸ï¼ææ¶åè¿ä¸å¨æèåºäººæºéªè¯ãçï¼ ![t0]
 (https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png) ### 2.
 Access denied. You do not have access to chat.openai.com. ###
    ç»å¸é®é¢ï¼åªè½å°å¤æ¾å¯ç¨VPNï¼è´¹æ¶è´¹åï¼æ´è´¹é±ãç§»å¨ç«¯è®¿é®æ´é¾ãçï¼
-![t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png) ### 3.
+![t1.1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.1.png) !
+[t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png) ### 3.
 ChatGPT is at capacity right now ###
    ç³»ç»è´è½½é«ï¼ç½å«ç¨æ·ä¸ç»ç¨ãçï¼ ![t2](https://github.com/
 pengzhile/pandora/raw/master/doc/images/t2.png) ### 4. This content may violate
 our content_policy. ###
    éå¾·å®¡æ¥ï¼å¤è§¦åå æ¬¡å¯è½å°±å°å·äºãçï¼ï¼ï¼ ![t3](https:
 //github.com/pengzhile/pandora/raw/master/doc/images/t3.png) ### 5. Something
 went wrong. ###    åçç«éå±çæ­ï¼çªç¶å°±åºæéäºãçï¼ ![t4]
```

### Comparing `Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/PKG-INFO` & `Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.0.7
+Version: 1.1.0
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
@@ -50,26 +50,28 @@
 [![Downloads](https://static.pepy.tech/badge/pandora-chatgpt)](https://pypi.python.org/pypi/pandora-chatgpt)
 [![PyPi workflow](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml)
 [![Docker workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml)
 [![Discord](https://img.shields.io/discord/1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa)
 
 ## 体验地址
 * 点击 <a href="https://chat.zhile.io" target="_blank" title="Pandora Cloud体验地址">https://chat.zhile.io</a>
-* 登录获取 `Access Token` 需要梯子。不过对IP无讲究，国家支持就行。
+* 可以访问 [这里](http://ai.fakeopen.com/auth) 拿 `Access Token`
+* 也可以官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
 * `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。
 * 这个页面上还包含一个共享账号的链接，**没有账号**的可以点进去体验一下。
  
 ## ChatGPT使用时可能会遇到：
 
 ### 1. Please stand by, while we are checking your browser... 
 ### &nbsp;&nbsp;&nbsp;动不动来一下，有时候还不动或者出人机验证。痛！
 ![t0](https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png)
 
 ### 2. Access denied. You do not have access to chat.openai.com. 
 ### &nbsp;&nbsp;&nbsp;经典问题，只能到处找可用VPN，费时费力，更费钱。移动端访问更难。痛！
+![t1.1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.1.png)
 ![t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png)
 
 ### 3. ChatGPT is at capacity right now 
 ### &nbsp;&nbsp;&nbsp;系统负载高，白嫖用户不给用。痛！
 ![t2](https://github.com/pengzhile/pandora/raw/master/doc/images/t2.png)
 
 ### 4. This content may violate our <u>content policy</u>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.0.7 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.1.0 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
@@ -30,27 +30,29 @@
 pypi.python.org/pypi/pandora-chatgpt) [![PyPi workflow](https://github.com/
 pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://
 github.com/pengzhile/pandora/actions/workflows/python-publish.yml) [![Docker
 workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-
 publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/
 docker-publish.yml) [![Discord](https://img.shields.io/discord/
 1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa) ##
-ä½éªå°å * ç¹å» https://chat.zhile.io * ç»å½è·å `Access Token`
-éè¦æ¢¯å­ãä¸è¿å¯¹IPæ è®²ç©¶ï¼å½å®¶æ¯æå°±è¡ã * `Access Token`
-æææ `14`
+ä½éªå°å * ç¹å» https://chat.zhile.io * å¯ä»¥è®¿é® [è¿é](http://
+ai.fakeopen.com/auth) æ¿ `Access Token` * ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é®
+[è¿é](http://chat.openai.com/api/auth/session) æ¿ `Access Token` * `Access
+Token` æææ `14`
 å¤©ï¼æé´è®¿é®**ä¸éè¦æ¢¯å­**ãè¿æå³çä½ å¨ææºä¸ä¹å¯éæä½¿ç¨ã
 *
 è¿ä¸ªé¡µé¢ä¸è¿åå«ä¸ä¸ªå±äº«è´¦å·çé¾æ¥ï¼**æ²¡æè´¦å·**çå¯ä»¥ç¹è¿å»ä½éªä¸ä¸ã
 ## ChatGPTä½¿ç¨æ¶å¯è½ä¼éå°ï¼ ### 1. Please stand by, while we are
 checking your browser... ###
    å¨ä¸å¨æ¥ä¸ä¸ï¼ææ¶åè¿ä¸å¨æèåºäººæºéªè¯ãçï¼ ![t0]
 (https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png) ### 2.
 Access denied. You do not have access to chat.openai.com. ###
    ç»å¸é®é¢ï¼åªè½å°å¤æ¾å¯ç¨VPNï¼è´¹æ¶è´¹åï¼æ´è´¹é±ãç§»å¨ç«¯è®¿é®æ´é¾ãçï¼
-![t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png) ### 3.
+![t1.1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.1.png) !
+[t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png) ### 3.
 ChatGPT is at capacity right now ###
    ç³»ç»è´è½½é«ï¼ç½å«ç¨æ·ä¸ç»ç¨ãçï¼ ![t2](https://github.com/
 pengzhile/pandora/raw/master/doc/images/t2.png) ### 4. This content may violate
 our content_policy. ###
    éå¾·å®¡æ¥ï¼å¤è§¦åå æ¬¡å¯è½å°±å°å·äºãçï¼ï¼ï¼ ![t3](https:
 //github.com/pengzhile/pandora/raw/master/doc/images/t3.png) ### 5. Something
 went wrong. ###    åçç«éå±çæ­ï¼çªç¶å°±åºæéäºãçï¼ ![t4]
```

### Comparing `Pandora-ChatGPT-1.0.7/Pandora_ChatGPT.egg-info/SOURCES.txt` & `Pandora-ChatGPT-1.1.0/Pandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/README.md` & `Pandora-ChatGPT-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 [![Downloads](https://static.pepy.tech/badge/pandora-chatgpt)](https://pypi.python.org/pypi/pandora-chatgpt)
 [![PyPi workflow](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml)
 [![Docker workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml)
 [![Discord](https://img.shields.io/discord/1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa)
 
 ## 体验地址
 * 点击 <a href="https://chat.zhile.io" target="_blank" title="Pandora Cloud体验地址">https://chat.zhile.io</a>
-* 登录获取 `Access Token` 需要梯子。不过对IP无讲究，国家支持就行。
+* 可以访问 [这里](http://ai.fakeopen.com/auth) 拿 `Access Token`
+* 也可以官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
 * `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。
 * 这个页面上还包含一个共享账号的链接，**没有账号**的可以点进去体验一下。
  
 ## ChatGPT使用时可能会遇到：
 
 ### 1. Please stand by, while we are checking your browser... 
 ### &nbsp;&nbsp;&nbsp;动不动来一下，有时候还不动或者出人机验证。痛！
 ![t0](https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png)
 
 ### 2. Access denied. You do not have access to chat.openai.com. 
 ### &nbsp;&nbsp;&nbsp;经典问题，只能到处找可用VPN，费时费力，更费钱。移动端访问更难。痛！
+![t1.1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.1.png)
 ![t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png)
 
 ### 3. ChatGPT is at capacity right now 
 ### &nbsp;&nbsp;&nbsp;系统负载高，白嫖用户不给用。痛！
 ![t2](https://github.com/pengzhile/pandora/raw/master/doc/images/t2.png)
 
 ### 4. This content may violate our <u>content policy</u>.
```

#### html2text {}

```diff
@@ -10,27 +10,29 @@
 pypi.python.org/pypi/pandora-chatgpt) [![PyPi workflow](https://github.com/
 pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://
 github.com/pengzhile/pandora/actions/workflows/python-publish.yml) [![Docker
 workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-
 publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/
 docker-publish.yml) [![Discord](https://img.shields.io/discord/
 1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa) ##
-ä½éªå°å * ç¹å» https://chat.zhile.io * ç»å½è·å `Access Token`
-éè¦æ¢¯å­ãä¸è¿å¯¹IPæ è®²ç©¶ï¼å½å®¶æ¯æå°±è¡ã * `Access Token`
-æææ `14`
+ä½éªå°å * ç¹å» https://chat.zhile.io * å¯ä»¥è®¿é® [è¿é](http://
+ai.fakeopen.com/auth) æ¿ `Access Token` * ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é®
+[è¿é](http://chat.openai.com/api/auth/session) æ¿ `Access Token` * `Access
+Token` æææ `14`
 å¤©ï¼æé´è®¿é®**ä¸éè¦æ¢¯å­**ãè¿æå³çä½ å¨ææºä¸ä¹å¯éæä½¿ç¨ã
 *
 è¿ä¸ªé¡µé¢ä¸è¿åå«ä¸ä¸ªå±äº«è´¦å·çé¾æ¥ï¼**æ²¡æè´¦å·**çå¯ä»¥ç¹è¿å»ä½éªä¸ä¸ã
 ## ChatGPTä½¿ç¨æ¶å¯è½ä¼éå°ï¼ ### 1. Please stand by, while we are
 checking your browser... ###
    å¨ä¸å¨æ¥ä¸ä¸ï¼ææ¶åè¿ä¸å¨æèåºäººæºéªè¯ãçï¼ ![t0]
 (https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png) ### 2.
 Access denied. You do not have access to chat.openai.com. ###
    ç»å¸é®é¢ï¼åªè½å°å¤æ¾å¯ç¨VPNï¼è´¹æ¶è´¹åï¼æ´è´¹é±ãç§»å¨ç«¯è®¿é®æ´é¾ãçï¼
-![t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png) ### 3.
+![t1.1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.1.png) !
+[t1](https://github.com/pengzhile/pandora/raw/master/doc/images/t1.png) ### 3.
 ChatGPT is at capacity right now ###
    ç³»ç»è´è½½é«ï¼ç½å«ç¨æ·ä¸ç»ç¨ãçï¼ ![t2](https://github.com/
 pengzhile/pandora/raw/master/doc/images/t2.png) ### 4. This content may violate
 our content_policy. ###
    éå¾·å®¡æ¥ï¼å¤è§¦åå æ¬¡å¯è½å°±å°å·äºãçï¼ï¼ï¼ ![t3](https:
 //github.com/pengzhile/pandora/raw/master/doc/images/t3.png) ### 5. Something
 went wrong. ###    åçç«éå±çæ­ï¼çªç¶å°±åºæéäºãçï¼ ![t4]
```

### Comparing `Pandora-ChatGPT-1.0.7/setup.py` & `Pandora-ChatGPT-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/pengzhile/pandora',
     packages=find_packages('src'),
     package_dir={'pandora': 'src/pandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['pandora-cloud~=0.0.7'],
+        'cloud': ['pandora-cloud~=0.1.0'],
     },
     entry_points={
         'console_scripts': [
             'pandora = pandora.launcher:run',
             'pandora-cloud = pandora.cloud_launcher:run',
         ]
     },
```

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/bots/legacy.py` & `Pandora-ChatGPT-1.1.0/src/pandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/bots/server.py` & `Pandora-ChatGPT-1.1.0/src/pandora/bots/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
         return jsonify(ret)
 
     def list_models(self):
         return self.__proxy_result(self.chatgpt.list_models(True, self.__get_token_key()))
 
     def list_conversations(self):
-        offset = request.args.get('offset', '1')
+        offset = request.args.get('offset', '0')
         limit = request.args.get('limit', '20')
 
         return self.__proxy_result(self.chatgpt.list_conversations(offset, limit, True, self.__get_token_key()))
 
     def get_conversation(self, conversation_id):
         return self.__proxy_result(self.chatgpt.get_conversation(conversation_id, True, self.__get_token_key()))
```

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/cloud_launcher.py` & `Pandora-ChatGPT-1.1.0/src/pandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/exts/hooks.py` & `Pandora-ChatGPT-1.1.0/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/exts/token.py` & `Pandora-ChatGPT-1.1.0/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/apple-touch-icon.png` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/favicon-16x16.png` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/favicon-32x32.png` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/flask/templates/chat.html` & `Pandora-ChatGPT-1.1.0/src/pandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/launcher.py` & `Pandora-ChatGPT-1.1.0/src/pandora/launcher.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/migrations/migrate.py` & `Pandora-ChatGPT-1.1.0/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/migrations/models.py` & `Pandora-ChatGPT-1.1.0/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Pandora-ChatGPT-1.1.0/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/openai/api.py` & `Pandora-ChatGPT-1.1.0/src/pandora/openai/api.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/openai/auth.py` & `Pandora-ChatGPT-1.1.0/src/pandora/openai/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import re
 from datetime import datetime as dt
 from os import getenv
 from urllib.parse import urlparse, parse_qs
 
 import requests
 from certifi import where
-from requests.exceptions import SSLError
 
 
 class Auth0:
     def __init__(self, email: str, password: str, proxy: str = None, use_cache: bool = True):
         self.session_token = None
         self.email = email
         self.password = password
@@ -43,30 +42,34 @@
 
         if not self.__check_email(self.email) or not self.password:
             raise Exception('invalid email or password.')
 
         return self.__part_two() if login_local else self.get_access_token_proxy()
 
     def __part_two(self) -> str:
-        url = '{}/auth/endpoint'.format(self.api_prefix)
+        url = '{}/auth/endpoint1'.format(self.api_prefix)
         headers = {
             'User-Agent': self.user_agent,
         }
-        resp = self.session.get(url, headers=headers, allow_redirects=False, **self.req_kwargs)
+        data = {
+            'g-recaptcha-response': 'Pandora is so cool!',
+        }
+
+        resp = self.session.post(url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs)
 
         if resp.status_code == 200:
             json = resp.json()
             return self.__part_three(json['state'], json['url'])
         else:
             raise Exception(resp.text)
 
     def __part_three(self, state1: str, url: str) -> str:
         headers = {
             'User-Agent': self.user_agent,
-            'Referer': 'https://explorer.api.openai.com/',
+            'Referer': 'https://chat.openai.com/',
         }
         resp = self.session.get(url, headers=headers, allow_redirects=True, **self.req_kwargs)
 
         if resp.status_code == 200:
             try:
                 url_params = parse_qs(urlparse(resp.url).query)
                 state = url_params['state'][0]
@@ -109,29 +112,46 @@
         data = {
             'state': state,
             'username': self.email,
             'password': self.password,
             'action': 'default',
         }
 
-        try:
-            resp = self.session.post(url, headers=headers, data=data, allow_redirects=True, **self.req_kwargs)
-        except SSLError as e:
-            if not hasattr(e.request, 'url') or not e.request.url:
-                raise Exception('Error login')
+        resp = self.session.post(url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs)
+        if resp.status_code == 302:
+            location = resp.headers['Location']
+            if not location.startswith('/authorize/resume?'):
+                raise Exception('Login failed.')
 
-            return self.get_access_token(state1, e.request.url)
+            return self.__part_six(state1, location, url)
 
         if resp.status_code == 400:
             raise Exception('Wrong email or password.')
         else:
             raise Exception('Error login.')
 
+    def __part_six(self, state1: str, location: str, ref: str) -> str:
+        url = 'https://auth0.openai.com' + location
+        headers = {
+            'User-Agent': self.user_agent,
+            'Referer': ref,
+        }
+
+        resp = self.session.get(url, headers=headers, allow_redirects=False, **self.req_kwargs)
+        if resp.status_code == 302:
+            location = resp.headers['Location']
+            if not location.startswith('https://chat.openai.com/api/auth/callback/auth0?'):
+                raise Exception('Login callback failed.')
+
+            return self.get_access_token(state1, resp.headers['Location'])
+
+        raise Exception('Error login.')
+
     def get_access_token(self, state1: str, callback_url: str) -> str:
-        url = '{}/auth/token'.format(self.api_prefix)
+        url = '{}/auth/token1'.format(self.api_prefix)
         headers = {
             'User-Agent': self.user_agent,
         }
         data = {
             'state': state1,
             'callbackUrl': callback_url,
         }
```

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/openai/utils.py` & `Pandora-ChatGPT-1.1.0/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/turbo/base.py` & `Pandora-ChatGPT-1.1.0/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.0.7/src/pandora/turbo/chat.py` & `Pandora-ChatGPT-1.1.0/src/pandora/turbo/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 
 
 class TurboGPT:
     DEFAULT_SYSTEM_PROMPT = 'You are ChatGPT, a large language model trained by OpenAI. ' \
                             'Answer as concisely as possible.\nKnowledge cutoff: 2021-09-01\n' \
                             'Current date: {}'.format(dt.now().strftime('%Y-%m-%d'))
     TITLE_PROMPT = 'Generate a brief title for our conversation.'
-    MAX_TOKENS = 4096
+    MAX_TOKENS = {
+        'gpt-3.5-turbo': 4096,
+        'gpt-4': 8192,
+        'gpt-4-32k': 32768,
+    }
 
     def __init__(self, api_keys: dict, proxy=None):
         self.api_keys = api_keys
         self.api_keys_key_list = list(api_keys)
         self.default_api_keys_key = self.api_keys_key_list[0]
 
         self.api = ChatCompletion(proxy)
@@ -40,21 +44,37 @@
         return self.api_keys[token_key or self.default_api_keys_key]
 
     def list_token_keys(self):
         return self.api_keys_key_list
 
     def list_models(self, raw=False, token=None):
         models = {
-            'models': [{
-                'slug': 'gpt-3.5-turbo',
-                'max_tokens': 4096,
-                'title': 'Default',
-                'description': 'Turbo is the api model that powers ChatGPT',
-                'tags': []
-            }]
+            'models': [
+                {
+                    'slug': 'gpt-3.5-turbo',
+                    'max_tokens': self.MAX_TOKENS['gpt-3.5-turbo'],
+                    'title': 'GPT-3.5',
+                    'description': 'Turbo is the api model that powers ChatGPT',
+                    'tags': []
+                },
+                {
+                    'slug': 'gpt-4',
+                    'max_tokens': self.MAX_TOKENS['gpt-4'],
+                    'title': 'GPT-4',
+                    'description': 'More capable than any GPT-3.5, able to do complex tasks, and optimized for chat',
+                    'tags': []
+                },
+                {
+                    'slug': 'gpt-4-32k',
+                    'max_tokens': self.MAX_TOKENS['gpt-4-32k'],
+                    'title': 'GPT-4 32K',
+                    'description': 'Same capabilities as the base gpt-4 mode but with 4x the context length',
+                    'tags': []
+                }
+            ]
         }
 
         if raw:
             return self.__wrap_response(models)
 
         return models['models']
 
@@ -258,15 +278,15 @@
         def __out_generator():
             for line in generator:
                 yield self.__map_conversation(status, conversation, gpt_prompt, line)
 
         return status, headers, __out_generator()
 
     def __reduce_messages(self, messages, model):
-        while gpt_num_tokens(messages, model) > self.MAX_TOKENS - 200:
+        while gpt_num_tokens(messages) > self.MAX_TOKENS[model] - 200:
             if len(messages) < 2:
                 raise Exception('prompt too long')
 
             messages.pop(1)
 
         return messages
```

