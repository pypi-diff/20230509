# Comparing `tmp/hotkeynet-0.1.3.tar.gz` & `tmp/hotkeynet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotkeynet-0.1.3.tar", last modified: Tue May  9 04:39:08 2023, max compression
+gzip compressed data, was "hotkeynet-0.1.4.tar", last modified: Tue May  9 04:52:44 2023, max compression
```

## Comparing `hotkeynet-0.1.3.tar` & `hotkeynet-0.1.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.221039 hotkeynet-0.1.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1119 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      341 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-09 04:39:08.220758 hotkeynet-0.1.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4408 2023-05-08 17:26:41.000000 hotkeynet-0.1.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.208766 hotkeynet-0.1.3/hotkeynet/
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-05-08 16:09:52.000000 hotkeynet-0.1.3/hotkeynet/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.211869 hotkeynet-0.1.3/hotkeynet/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      455 2023-05-08 16:10:53.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-05-09 04:36:28.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1447 2023-05-09 04:34:42.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/api.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)    18692 2023-05-09 04:34:42.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/canned.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)    17103 2023-05-09 04:34:42.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/keyname.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     3805 2023-05-08 16:59:43.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/maker.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)    55824 2023-05-08 16:57:58.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/script.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     2299 2023-05-08 06:38:52.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-09 04:36:27.000000 hotkeynet-0.1.3/hotkeynet/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1031 2023-05-09 04:30:59.000000 hotkeynet-0.1.3/hotkeynet/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    26168 2023-05-09 04:34:36.000000 hotkeynet-0.1.3/hotkeynet/canned.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.212191 hotkeynet-0.1.3/hotkeynet/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/docs/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.212467 hotkeynet-0.1.3/hotkeynet/docs/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-05-08 13:10:35.000000 hotkeynet-0.1.3/hotkeynet/docs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)    21156 2023-05-09 04:33:49.000000 hotkeynet-0.1.3/hotkeynet/keyname.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2911 2023-05-08 16:59:22.000000 hotkeynet-0.1.3/hotkeynet/maker.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    43493 2023-05-08 16:55:31.000000 hotkeynet-0.1.3/hotkeynet/script.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.213235 hotkeynet-0.1.3/hotkeynet/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/tests/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.213993 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      211 2023-05-08 04:44:05.000000 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      585 2023-05-08 16:40:41.000000 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/helper.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      299 2023-05-08 04:44:05.000000 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/paths.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      459 2023-05-08 16:17:16.000000 hotkeynet-0.1.3/hotkeynet/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      160 2023-05-08 04:41:11.000000 hotkeynet-0.1.3/hotkeynet/tests/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.214769 hotkeynet-0.1.3/hotkeynet/tpl/
--rw-r--r--   0 sanhehu    (501) staff       (20)      125 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/tpl/Block.tpl
--rw-r--r--   0 sanhehu    (501) staff       (20)       91 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/tpl/Script.tpl
--rw-r--r--   0 sanhehu    (501) staff       (20)      307 2023-05-08 16:56:31.000000 hotkeynet-0.1.3/hotkeynet/tpl/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.215034 hotkeynet-0.1.3/hotkeynet/tpl/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      449 2023-05-08 16:57:58.000000 hotkeynet-0.1.3/hotkeynet/tpl/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1491 2023-05-08 06:38:43.000000 hotkeynet-0.1.3/hotkeynet/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.215676 hotkeynet-0.1.3/hotkeynet/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-05-08 06:45:45.000000 hotkeynet-0.1.3/hotkeynet/vendor/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.216570 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-05-08 06:56:39.000000 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     5683 2023-05-08 06:56:39.000000 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     3534 2023-05-08 16:18:00.000000 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 hotkeynet-0.1.3/hotkeynet/vendor/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-08 04:40:02.000000 hotkeynet-0.1.3/hotkeynet/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.209501 hotkeynet-0.1.3/hotkeynet.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1871 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      229 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      774 2023-05-09 04:36:17.000000 hotkeynet-0.1.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      289 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-ground-truth.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       53 2023-05-08 18:00:23.000000 hotkeynet-0.1.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-09 04:39:08.221106 hotkeynet-0.1.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7698 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.220393 hotkeynet-0.1.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1418 2023-05-08 16:09:28.000000 hotkeynet-0.1.3/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1062 2023-05-09 04:34:51.000000 hotkeynet-0.1.3/tests/test_canned.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-08 06:17:59.000000 hotkeynet-0.1.3/tests/test_keyname.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      872 2023-05-08 13:49:25.000000 hotkeynet-0.1.3/tests/test_script_command.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1852 2023-05-08 13:49:38.000000 hotkeynet-0.1.3/tests/test_script_context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      826 2023-05-08 13:49:44.000000 hotkeynet-0.1.3/tests/test_script_hotkey.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      361 2023-05-08 13:49:50.000000 hotkeynet-0.1.3/tests/test_script_key.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      407 2023-05-08 13:49:58.000000 hotkeynet-0.1.3/tests/test_script_label.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1289 2023-05-08 16:14:49.000000 hotkeynet-0.1.3/tests/test_script_mouse.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      954 2023-05-08 16:51:24.000000 hotkeynet-0.1.3/tests/test_script_script.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      792 2023-05-08 13:50:22.000000 hotkeynet-0.1.3/tests/test_script_send_label.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1154 2023-05-08 13:50:55.000000 hotkeynet-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.668609 hotkeynet-0.1.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1119 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      341 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-09 04:52:44.668367 hotkeynet-0.1.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4408 2023-05-08 17:26:41.000000 hotkeynet-0.1.4/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.655548 hotkeynet-0.1.4/hotkeynet/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-05-08 16:09:52.000000 hotkeynet-0.1.4/hotkeynet/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.659574 hotkeynet-0.1.4/hotkeynet/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      455 2023-05-08 16:10:53.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-05-09 04:52:43.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1447 2023-05-09 04:34:42.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/api.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    18356 2023-05-09 04:51:31.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/canned.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16767 2023-05-09 04:51:31.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/keyname.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3805 2023-05-08 16:59:43.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/maker.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    55824 2023-05-08 16:57:58.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/script.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2299 2023-05-08 06:38:52.000000 hotkeynet-0.1.4/hotkeynet/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-09 04:51:34.000000 hotkeynet-0.1.4/hotkeynet/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1031 2023-05-09 04:30:59.000000 hotkeynet-0.1.4/hotkeynet/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    25832 2023-05-09 04:50:21.000000 hotkeynet-0.1.4/hotkeynet/canned.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.659894 hotkeynet-0.1.4/hotkeynet/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/hotkeynet/docs/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.660166 hotkeynet-0.1.4/hotkeynet/docs/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-05-08 13:10:35.000000 hotkeynet-0.1.4/hotkeynet/docs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    20820 2023-05-09 04:49:14.000000 hotkeynet-0.1.4/hotkeynet/keyname.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2911 2023-05-08 16:59:22.000000 hotkeynet-0.1.4/hotkeynet/maker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    43493 2023-05-08 16:55:31.000000 hotkeynet-0.1.4/hotkeynet/script.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.660911 hotkeynet-0.1.4/hotkeynet/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/hotkeynet/tests/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.661791 hotkeynet-0.1.4/hotkeynet/tests/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      211 2023-05-08 04:44:05.000000 hotkeynet-0.1.4/hotkeynet/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      585 2023-05-08 16:40:41.000000 hotkeynet-0.1.4/hotkeynet/tests/__pycache__/helper.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      299 2023-05-08 04:44:05.000000 hotkeynet-0.1.4/hotkeynet/tests/__pycache__/paths.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      459 2023-05-08 16:17:16.000000 hotkeynet-0.1.4/hotkeynet/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      160 2023-05-08 04:41:11.000000 hotkeynet-0.1.4/hotkeynet/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.662746 hotkeynet-0.1.4/hotkeynet/tpl/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      125 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/hotkeynet/tpl/Block.tpl
+-rw-r--r--   0 sanhehu    (501) staff       (20)       91 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/hotkeynet/tpl/Script.tpl
+-rw-r--r--   0 sanhehu    (501) staff       (20)      307 2023-05-08 16:56:31.000000 hotkeynet-0.1.4/hotkeynet/tpl/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.663037 hotkeynet-0.1.4/hotkeynet/tpl/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      449 2023-05-08 16:57:58.000000 hotkeynet-0.1.4/hotkeynet/tpl/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1491 2023-05-08 06:38:43.000000 hotkeynet-0.1.4/hotkeynet/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.663811 hotkeynet-0.1.4/hotkeynet/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-05-08 06:45:45.000000 hotkeynet-0.1.4/hotkeynet/vendor/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.664790 hotkeynet-0.1.4/hotkeynet/vendor/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-05-08 06:56:39.000000 hotkeynet-0.1.4/hotkeynet/vendor/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5683 2023-05-08 06:56:39.000000 hotkeynet-0.1.4/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3534 2023-05-08 16:18:00.000000 hotkeynet-0.1.4/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 hotkeynet-0.1.4/hotkeynet/vendor/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-08 04:40:02.000000 hotkeynet-0.1.4/hotkeynet/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.656359 hotkeynet-0.1.4/hotkeynet.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-09 04:52:44.000000 hotkeynet-0.1.4/hotkeynet.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1871 2023-05-09 04:52:44.000000 hotkeynet-0.1.4/hotkeynet.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-09 04:52:44.000000 hotkeynet-0.1.4/hotkeynet.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      229 2023-05-09 04:52:44.000000 hotkeynet-0.1.4/hotkeynet.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-05-09 04:52:44.000000 hotkeynet-0.1.4/hotkeynet.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      970 2023-05-09 04:52:13.000000 hotkeynet-0.1.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      289 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/requirements-ground-truth.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       53 2023-05-08 18:00:23.000000 hotkeynet-0.1.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-09 04:52:44.668652 hotkeynet-0.1.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7698 2023-05-08 04:33:13.000000 hotkeynet-0.1.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:52:44.668013 hotkeynet-0.1.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1418 2023-05-08 16:09:28.000000 hotkeynet-0.1.4/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1062 2023-05-09 04:34:51.000000 hotkeynet-0.1.4/tests/test_canned.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-08 06:17:59.000000 hotkeynet-0.1.4/tests/test_keyname.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      872 2023-05-08 13:49:25.000000 hotkeynet-0.1.4/tests/test_script_command.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1852 2023-05-08 13:49:38.000000 hotkeynet-0.1.4/tests/test_script_context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      826 2023-05-08 13:49:44.000000 hotkeynet-0.1.4/tests/test_script_hotkey.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      361 2023-05-08 13:49:50.000000 hotkeynet-0.1.4/tests/test_script_key.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      407 2023-05-08 13:49:58.000000 hotkeynet-0.1.4/tests/test_script_label.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1289 2023-05-08 16:14:49.000000 hotkeynet-0.1.4/tests/test_script_mouse.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      954 2023-05-08 16:51:24.000000 hotkeynet-0.1.4/tests/test_script_script.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      792 2023-05-08 13:50:22.000000 hotkeynet-0.1.4/tests/test_script_send_label.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1154 2023-05-08 13:50:55.000000 hotkeynet-0.1.4/tests/test_utils.py
```

### Comparing `hotkeynet-0.1.3/LICENSE.txt` & `hotkeynet-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/PKG-INFO` & `hotkeynet-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hotkeynet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Write hotkeynet script in Python.
 Home-page: https://github.com/MacHu-GWU/hotkeynet-project
-Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.3#downloads
+Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `hotkeynet-0.1.3/README.rst` & `hotkeynet-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/__pycache__/api.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/__pycache__/api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/__pycache__/canned.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/__pycache__/canned.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May  9 04:34:36 2023 UTC, .py size: 26168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5ccd 5964 3866 0000  U.......\.Yd8f..
+00000000: 550d 0d0a 0000 0000 0dd1 5964 e864 0000  U.........Yd.d..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 4a1b 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6403 6404 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a05 0100 6403 6405 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
 00000050: 6d09 5a0a 6d0b 5a0c 0100 6508 6505 6a0d  m.Z.m.Z...e.e.j.
 00000060: 8301 5a0d 6508 6505 6a0e 8301 5a0e 6508  ..Z.e.e.j...Z.e.
 00000070: 6505 6a0f 8301 5a0f 6508 6505 6a10 8301  e.j...Z.e.e.j...
@@ -672,498 +672,477 @@
 000029f0: da07 4354 524c 5f46 34da 0743 5452 4c5f  ..CTRL_F4..CTRL_
 00002a00: 4635 da07 4354 524c 5f46 36da 0743 5452  F5..CTRL_F6..CTR
 00002a10: 4c5f 4637 da07 4354 524c 5f46 38da 0743  L_F7..CTRL_F8..C
 00002a20: 5452 4c5f 4639 da08 4354 524c 5f46 3130  TRL_F9..CTRL_F10
 00002a30: da08 4354 524c 5f46 3131 da08 4354 524c  ..CTRL_F11..CTRL
 00002a40: 5f46 3132 da1c 4354 524c 5f4f 454d 335f  _F12..CTRL_OEM3_
 00002a50: 5741 5645 5f4f 525f 4241 434b 5f51 554f  WAVE_OR_BACK_QUO
-00002a60: 5445 da0a 4354 524c 5f4b 4559 5f31 da0a  TE..CTRL_KEY_1..
-00002a70: 4354 524c 5f4b 4559 5f32 da0a 4354 524c  CTRL_KEY_2..CTRL
-00002a80: 5f4b 4559 5f33 da0a 4354 524c 5f4b 4559  _KEY_3..CTRL_KEY
-00002a90: 5f34 da0a 4354 524c 5f4b 4559 5f35 da0a  _4..CTRL_KEY_5..
-00002aa0: 4354 524c 5f4b 4559 5f36 da0a 4354 524c  CTRL_KEY_6..CTRL
-00002ab0: 5f4b 4559 5f37 da0a 4354 524c 5f4b 4559  _KEY_7..CTRL_KEY
-00002ac0: 5f38 da0a 4354 524c 5f4b 4559 5f39 da0a  _8..CTRL_KEY_9..
-00002ad0: 4354 524c 5f4b 4559 5f30 da11 4354 524c  CTRL_KEY_0..CTRL
-00002ae0: 5f4b 4559 5f31 315f 4d49 4e55 53da 1043  _KEY_11_MINUS..C
-00002af0: 5452 4c5f 4b45 595f 3132 5f50 4c55 53da  TRL_KEY_12_PLUS.
-00002b00: 0e43 5452 4c5f 4241 434b 5350 4143 45da  .CTRL_BACKSPACE.
-00002b10: 0d43 5452 4c5f 4e55 4d50 4144 5f31 da0d  .CTRL_NUMPAD_1..
-00002b20: 4354 524c 5f4e 554d 5041 445f 32da 0d43  CTRL_NUMPAD_2..C
-00002b30: 5452 4c5f 4e55 4d50 4144 5f33 da0d 4354  TRL_NUMPAD_3..CT
-00002b40: 524c 5f4e 554d 5041 445f 34da 0d43 5452  RL_NUMPAD_4..CTR
-00002b50: 4c5f 4e55 4d50 4144 5f35 da0d 4354 524c  L_NUMPAD_5..CTRL
-00002b60: 5f4e 554d 5041 445f 36da 0d43 5452 4c5f  _NUMPAD_6..CTRL_
-00002b70: 4e55 4d50 4144 5f37 da0d 4354 524c 5f4e  NUMPAD_7..CTRL_N
-00002b80: 554d 5041 445f 38da 0d43 5452 4c5f 4e55  UMPAD_8..CTRL_NU
-00002b90: 4d50 4144 5f39 da0d 4354 524c 5f4e 554d  MPAD_9..CTRL_NUM
-00002ba0: 5041 445f 30da 1543 5452 4c5f 4e55 4d50  PAD_0..CTRL_NUMP
-00002bb0: 4144 5f31 315f 4449 5649 4445 da17 4354  AD_11_DIVIDE..CT
-00002bc0: 524c 5f4e 554d 5041 445f 3132 5f4d 554c  RL_NUMPAD_12_MUL
-00002bd0: 5449 504c 59da 0643 5452 4c5f 41da 0643  TIPLY..CTRL_A..C
-00002be0: 5452 4c5f 42da 0643 5452 4c5f 43da 0643  TRL_B..CTRL_C..C
-00002bf0: 5452 4c5f 44da 0643 5452 4c5f 45da 0643  TRL_D..CTRL_E..C
-00002c00: 5452 4c5f 46da 0643 5452 4c5f 47da 0643  TRL_F..CTRL_G..C
-00002c10: 5452 4c5f 48da 0643 5452 4c5f 49da 0643  TRL_H..CTRL_I..C
-00002c20: 5452 4c5f 4ada 0643 5452 4c5f 4bda 0643  TRL_J..CTRL_K..C
-00002c30: 5452 4c5f 4cda 0643 5452 4c5f 4dda 0643  TRL_L..CTRL_M..C
-00002c40: 5452 4c5f 4eda 0643 5452 4c5f 4fda 0643  TRL_N..CTRL_O..C
-00002c50: 5452 4c5f 50da 0643 5452 4c5f 51da 0643  TRL_P..CTRL_Q..C
-00002c60: 5452 4c5f 52da 0643 5452 4c5f 53da 0643  TRL_R..CTRL_S..C
-00002c70: 5452 4c5f 54da 0643 5452 4c5f 55da 0643  TRL_T..CTRL_U..C
-00002c80: 5452 4c5f 56da 0643 5452 4c5f 57da 0643  TRL_V..CTRL_W..C
-00002c90: 5452 4c5f 58da 0643 5452 4c5f 59da 0643  TRL_X..CTRL_Y..C
-00002ca0: 5452 4c5f 5ada 0953 4849 4654 5f54 4142  TRL_Z..SHIFT_TAB
-00002cb0: da08 5348 4946 545f 4631 da08 5348 4946  ..SHIFT_F1..SHIF
-00002cc0: 545f 4632 da08 5348 4946 545f 4633 da08  T_F2..SHIFT_F3..
-00002cd0: 5348 4946 545f 4634 da08 5348 4946 545f  SHIFT_F4..SHIFT_
-00002ce0: 4635 da08 5348 4946 545f 4636 da08 5348  F5..SHIFT_F6..SH
-00002cf0: 4946 545f 4637 da08 5348 4946 545f 4638  IFT_F7..SHIFT_F8
-00002d00: da08 5348 4946 545f 4639 da09 5348 4946  ..SHIFT_F9..SHIF
-00002d10: 545f 4631 30da 0953 4849 4654 5f46 3131  T_F10..SHIFT_F11
-00002d20: da09 5348 4946 545f 4631 32da 1d53 4849  ..SHIFT_F12..SHI
-00002d30: 4654 5f4f 454d 335f 5741 5645 5f4f 525f  FT_OEM3_WAVE_OR_
-00002d40: 4241 434b 5f51 554f 5445 da0b 5348 4946  BACK_QUOTE..SHIF
-00002d50: 545f 4b45 595f 31da 0b53 4849 4654 5f4b  T_KEY_1..SHIFT_K
-00002d60: 4559 5f32 da0b 5348 4946 545f 4b45 595f  EY_2..SHIFT_KEY_
-00002d70: 33da 0b53 4849 4654 5f4b 4559 5f34 da0b  3..SHIFT_KEY_4..
-00002d80: 5348 4946 545f 4b45 595f 35da 0b53 4849  SHIFT_KEY_5..SHI
-00002d90: 4654 5f4b 4559 5f36 da0b 5348 4946 545f  FT_KEY_6..SHIFT_
-00002da0: 4b45 595f 37da 0b53 4849 4654 5f4b 4559  KEY_7..SHIFT_KEY
-00002db0: 5f38 da0b 5348 4946 545f 4b45 595f 39da  _8..SHIFT_KEY_9.
-00002dc0: 0b53 4849 4654 5f4b 4559 5f30 da12 5348  .SHIFT_KEY_0..SH
-00002dd0: 4946 545f 4b45 595f 3131 5f4d 494e 5553  IFT_KEY_11_MINUS
-00002de0: da11 5348 4946 545f 4b45 595f 3132 5f50  ..SHIFT_KEY_12_P
-00002df0: 4c55 53da 0f53 4849 4654 5f42 4143 4b53  LUS..SHIFT_BACKS
-00002e00: 5041 4345 da0e 5348 4946 545f 4e55 4d50  PACE..SHIFT_NUMP
-00002e10: 4144 5f31 da0e 5348 4946 545f 4e55 4d50  AD_1..SHIFT_NUMP
-00002e20: 4144 5f32 da0e 5348 4946 545f 4e55 4d50  AD_2..SHIFT_NUMP
-00002e30: 4144 5f33 da0e 5348 4946 545f 4e55 4d50  AD_3..SHIFT_NUMP
-00002e40: 4144 5f34 da0e 5348 4946 545f 4e55 4d50  AD_4..SHIFT_NUMP
-00002e50: 4144 5f35 da0e 5348 4946 545f 4e55 4d50  AD_5..SHIFT_NUMP
-00002e60: 4144 5f36 da0e 5348 4946 545f 4e55 4d50  AD_6..SHIFT_NUMP
-00002e70: 4144 5f37 da0e 5348 4946 545f 4e55 4d50  AD_7..SHIFT_NUMP
-00002e80: 4144 5f38 da0e 5348 4946 545f 4e55 4d50  AD_8..SHIFT_NUMP
-00002e90: 4144 5f39 da0e 5348 4946 545f 4e55 4d50  AD_9..SHIFT_NUMP
-00002ea0: 4144 5f30 da16 5348 4946 545f 4e55 4d50  AD_0..SHIFT_NUMP
-00002eb0: 4144 5f31 315f 4449 5649 4445 da18 5348  AD_11_DIVIDE..SH
-00002ec0: 4946 545f 4e55 4d50 4144 5f31 325f 4d55  IFT_NUMPAD_12_MU
-00002ed0: 4c54 4950 4c59 da07 5348 4946 545f 41da  LTIPLY..SHIFT_A.
-00002ee0: 0753 4849 4654 5f42 da07 5348 4946 545f  .SHIFT_B..SHIFT_
-00002ef0: 43da 0753 4849 4654 5f44 da07 5348 4946  C..SHIFT_D..SHIF
-00002f00: 545f 45da 0753 4849 4654 5f46 da07 5348  T_E..SHIFT_F..SH
-00002f10: 4946 545f 47da 0753 4849 4654 5f48 da07  IFT_G..SHIFT_H..
-00002f20: 5348 4946 545f 49da 0753 4849 4654 5f4a  SHIFT_I..SHIFT_J
-00002f30: da07 5348 4946 545f 4bda 0753 4849 4654  ..SHIFT_K..SHIFT
-00002f40: 5f4c da07 5348 4946 545f 4dda 0753 4849  _L..SHIFT_M..SHI
-00002f50: 4654 5f4e da07 5348 4946 545f 4fda 0753  FT_N..SHIFT_O..S
-00002f60: 4849 4654 5f50 da07 5348 4946 545f 51da  HIFT_P..SHIFT_Q.
-00002f70: 0753 4849 4654 5f52 da07 5348 4946 545f  .SHIFT_R..SHIFT_
-00002f80: 53da 0753 4849 4654 5f54 da07 5348 4946  S..SHIFT_T..SHIF
-00002f90: 545f 55da 0753 4849 4654 5f56 da07 5348  T_U..SHIFT_V..SH
-00002fa0: 4946 545f 57da 0753 4849 4654 5f58 da07  IFT_W..SHIFT_X..
-00002fb0: 5348 4946 545f 59da 0753 4849 4654 5f5a  SHIFT_Y..SHIFT_Z
-00002fc0: da07 414c 545f 5441 42da 0641 4c54 5f46  ..ALT_TAB..ALT_F
-00002fd0: 31da 0641 4c54 5f46 32da 0641 4c54 5f46  1..ALT_F2..ALT_F
-00002fe0: 33da 0641 4c54 5f46 34da 0641 4c54 5f46  3..ALT_F4..ALT_F
-00002ff0: 35da 0641 4c54 5f46 36da 0641 4c54 5f46  5..ALT_F6..ALT_F
-00003000: 37da 0641 4c54 5f46 38da 0641 4c54 5f46  7..ALT_F8..ALT_F
-00003010: 39da 0741 4c54 5f46 3130 da07 414c 545f  9..ALT_F10..ALT_
-00003020: 4631 31da 0741 4c54 5f46 3132 da1b 414c  F11..ALT_F12..AL
-00003030: 545f 4f45 4d33 5f57 4156 455f 4f52 5f42  T_OEM3_WAVE_OR_B
-00003040: 4143 4b5f 5155 4f54 45da 0941 4c54 5f4b  ACK_QUOTE..ALT_K
-00003050: 4559 5f31 da09 414c 545f 4b45 595f 32da  EY_1..ALT_KEY_2.
-00003060: 0941 4c54 5f4b 4559 5f33 da09 414c 545f  .ALT_KEY_3..ALT_
-00003070: 4b45 595f 34da 0941 4c54 5f4b 4559 5f35  KEY_4..ALT_KEY_5
-00003080: da09 414c 545f 4b45 595f 36da 0941 4c54  ..ALT_KEY_6..ALT
-00003090: 5f4b 4559 5f37 da09 414c 545f 4b45 595f  _KEY_7..ALT_KEY_
-000030a0: 38da 0941 4c54 5f4b 4559 5f39 da09 414c  8..ALT_KEY_9..AL
-000030b0: 545f 4b45 595f 30da 1041 4c54 5f4b 4559  T_KEY_0..ALT_KEY
-000030c0: 5f31 315f 4d49 4e55 53da 0f41 4c54 5f4b  _11_MINUS..ALT_K
-000030d0: 4559 5f31 325f 504c 5553 da0d 414c 545f  EY_12_PLUS..ALT_
-000030e0: 4241 434b 5350 4143 45da 0c41 4c54 5f4e  BACKSPACE..ALT_N
-000030f0: 554d 5041 445f 31da 0c41 4c54 5f4e 554d  UMPAD_1..ALT_NUM
-00003100: 5041 445f 32da 0c41 4c54 5f4e 554d 5041  PAD_2..ALT_NUMPA
-00003110: 445f 33da 0c41 4c54 5f4e 554d 5041 445f  D_3..ALT_NUMPAD_
-00003120: 34da 0c41 4c54 5f4e 554d 5041 445f 35da  4..ALT_NUMPAD_5.
-00003130: 0c41 4c54 5f4e 554d 5041 445f 36da 0c41  .ALT_NUMPAD_6..A
-00003140: 4c54 5f4e 554d 5041 445f 37da 0c41 4c54  LT_NUMPAD_7..ALT
-00003150: 5f4e 554d 5041 445f 38da 0c41 4c54 5f4e  _NUMPAD_8..ALT_N
-00003160: 554d 5041 445f 39da 0c41 4c54 5f4e 554d  UMPAD_9..ALT_NUM
-00003170: 5041 445f 30da 1441 4c54 5f4e 554d 5041  PAD_0..ALT_NUMPA
-00003180: 445f 3131 5f44 4956 4944 45da 1641 4c54  D_11_DIVIDE..ALT
-00003190: 5f4e 554d 5041 445f 3132 5f4d 554c 5449  _NUMPAD_12_MULTI
-000031a0: 504c 59da 0541 4c54 5f41 da05 414c 545f  PLY..ALT_A..ALT_
-000031b0: 42da 0541 4c54 5f43 da05 414c 545f 44da  B..ALT_C..ALT_D.
-000031c0: 0541 4c54 5f45 da05 414c 545f 46da 0541  .ALT_E..ALT_F..A
-000031d0: 4c54 5f47 da05 414c 545f 48da 0541 4c54  LT_G..ALT_H..ALT
-000031e0: 5f49 da05 414c 545f 4ada 0541 4c54 5f4b  _I..ALT_J..ALT_K
-000031f0: da05 414c 545f 4cda 0541 4c54 5f4d da05  ..ALT_L..ALT_M..
-00003200: 414c 545f 4eda 0541 4c54 5f4f da05 414c  ALT_N..ALT_O..AL
-00003210: 545f 50da 0541 4c54 5f51 da05 414c 545f  T_P..ALT_Q..ALT_
-00003220: 52da 0541 4c54 5f53 da05 414c 545f 54da  R..ALT_S..ALT_T.
-00003230: 0541 4c54 5f55 da05 414c 545f 56da 0541  .ALT_U..ALT_V..A
-00003240: 4c54 5f57 da05 414c 545f 58da 0541 4c54  LT_W..ALT_X..ALT
-00003250: 5f59 da05 414c 545f 5ada 0b43 5452 4c5f  _Y..ALT_Z..CTRL_
-00003260: 414c 545f 4631 da0b 4354 524c 5f41 4c54  ALT_F1..CTRL_ALT
-00003270: 5f46 32da 0b43 5452 4c5f 414c 545f 4633  _F2..CTRL_ALT_F3
-00003280: da0b 4354 524c 5f41 4c54 5f46 34da 0b43  ..CTRL_ALT_F4..C
-00003290: 5452 4c5f 414c 545f 4635 da0b 4354 524c  TRL_ALT_F5..CTRL
-000032a0: 5f41 4c54 5f46 36da 0b43 5452 4c5f 414c  _ALT_F6..CTRL_AL
-000032b0: 545f 4637 da0b 4354 524c 5f41 4c54 5f46  T_F7..CTRL_ALT_F
-000032c0: 38da 0b43 5452 4c5f 414c 545f 4639 da0c  8..CTRL_ALT_F9..
-000032d0: 4354 524c 5f41 4c54 5f46 3130 da0c 4354  CTRL_ALT_F10..CT
-000032e0: 524c 5f41 4c54 5f46 3131 da0c 4354 524c  RL_ALT_F11..CTRL
-000032f0: 5f41 4c54 5f46 3132 da20 4354 524c 5f41  _ALT_F12. CTRL_A
-00003300: 4c54 5f4f 454d 335f 5741 5645 5f4f 525f  LT_OEM3_WAVE_OR_
-00003310: 4241 434b 5f51 554f 5445 da0e 4354 524c  BACK_QUOTE..CTRL
-00003320: 5f41 4c54 5f4b 4559 5f31 da0e 4354 524c  _ALT_KEY_1..CTRL
-00003330: 5f41 4c54 5f4b 4559 5f32 da0e 4354 524c  _ALT_KEY_2..CTRL
-00003340: 5f41 4c54 5f4b 4559 5f33 da0e 4354 524c  _ALT_KEY_3..CTRL
-00003350: 5f41 4c54 5f4b 4559 5f34 da0e 4354 524c  _ALT_KEY_4..CTRL
-00003360: 5f41 4c54 5f4b 4559 5f35 da0e 4354 524c  _ALT_KEY_5..CTRL
-00003370: 5f41 4c54 5f4b 4559 5f36 da0e 4354 524c  _ALT_KEY_6..CTRL
-00003380: 5f41 4c54 5f4b 4559 5f37 da0e 4354 524c  _ALT_KEY_7..CTRL
-00003390: 5f41 4c54 5f4b 4559 5f38 da0e 4354 524c  _ALT_KEY_8..CTRL
-000033a0: 5f41 4c54 5f4b 4559 5f39 da0e 4354 524c  _ALT_KEY_9..CTRL
-000033b0: 5f41 4c54 5f4b 4559 5f30 da15 4354 524c  _ALT_KEY_0..CTRL
-000033c0: 5f41 4c54 5f4b 4559 5f31 315f 4d49 4e55  _ALT_KEY_11_MINU
-000033d0: 53da 1443 5452 4c5f 414c 545f 4b45 595f  S..CTRL_ALT_KEY_
-000033e0: 3132 5f50 4c55 53da 1243 5452 4c5f 414c  12_PLUS..CTRL_AL
-000033f0: 545f 4241 434b 5350 4143 45da 1143 5452  T_BACKSPACE..CTR
-00003400: 4c5f 414c 545f 4e55 4d50 4144 5f31 da11  L_ALT_NUMPAD_1..
-00003410: 4354 524c 5f41 4c54 5f4e 554d 5041 445f  CTRL_ALT_NUMPAD_
-00003420: 32da 1143 5452 4c5f 414c 545f 4e55 4d50  2..CTRL_ALT_NUMP
-00003430: 4144 5f33 da11 4354 524c 5f41 4c54 5f4e  AD_3..CTRL_ALT_N
-00003440: 554d 5041 445f 34da 1143 5452 4c5f 414c  UMPAD_4..CTRL_AL
-00003450: 545f 4e55 4d50 4144 5f35 da11 4354 524c  T_NUMPAD_5..CTRL
-00003460: 5f41 4c54 5f4e 554d 5041 445f 36da 1143  _ALT_NUMPAD_6..C
-00003470: 5452 4c5f 414c 545f 4e55 4d50 4144 5f37  TRL_ALT_NUMPAD_7
-00003480: da11 4354 524c 5f41 4c54 5f4e 554d 5041  ..CTRL_ALT_NUMPA
-00003490: 445f 38da 1143 5452 4c5f 414c 545f 4e55  D_8..CTRL_ALT_NU
-000034a0: 4d50 4144 5f39 da11 4354 524c 5f41 4c54  MPAD_9..CTRL_ALT
-000034b0: 5f4e 554d 5041 445f 30da 1943 5452 4c5f  _NUMPAD_0..CTRL_
-000034c0: 414c 545f 4e55 4d50 4144 5f31 315f 4449  ALT_NUMPAD_11_DI
-000034d0: 5649 4445 da1b 4354 524c 5f41 4c54 5f4e  VIDE..CTRL_ALT_N
-000034e0: 554d 5041 445f 3132 5f4d 554c 5449 504c  UMPAD_12_MULTIPL
-000034f0: 59da 0a43 5452 4c5f 414c 545f 41da 0a43  Y..CTRL_ALT_A..C
-00003500: 5452 4c5f 414c 545f 42da 0a43 5452 4c5f  TRL_ALT_B..CTRL_
-00003510: 414c 545f 43da 0a43 5452 4c5f 414c 545f  ALT_C..CTRL_ALT_
-00003520: 44da 0a43 5452 4c5f 414c 545f 45da 0a43  D..CTRL_ALT_E..C
-00003530: 5452 4c5f 414c 545f 46da 0a43 5452 4c5f  TRL_ALT_F..CTRL_
-00003540: 414c 545f 47da 0a43 5452 4c5f 414c 545f  ALT_G..CTRL_ALT_
-00003550: 48da 0a43 5452 4c5f 414c 545f 49da 0a43  H..CTRL_ALT_I..C
-00003560: 5452 4c5f 414c 545f 4ada 0a43 5452 4c5f  TRL_ALT_J..CTRL_
-00003570: 414c 545f 4bda 0a43 5452 4c5f 414c 545f  ALT_K..CTRL_ALT_
-00003580: 4cda 0a43 5452 4c5f 414c 545f 4dda 0a43  L..CTRL_ALT_M..C
-00003590: 5452 4c5f 414c 545f 4eda 0a43 5452 4c5f  TRL_ALT_N..CTRL_
-000035a0: 414c 545f 4fda 0a43 5452 4c5f 414c 545f  ALT_O..CTRL_ALT_
-000035b0: 50da 0a43 5452 4c5f 414c 545f 51da 0a43  P..CTRL_ALT_Q..C
-000035c0: 5452 4c5f 414c 545f 52da 0a43 5452 4c5f  TRL_ALT_R..CTRL_
-000035d0: 414c 545f 53da 0a43 5452 4c5f 414c 545f  ALT_S..CTRL_ALT_
-000035e0: 54da 0a43 5452 4c5f 414c 545f 55da 0a43  T..CTRL_ALT_U..C
-000035f0: 5452 4c5f 414c 545f 56da 0a43 5452 4c5f  TRL_ALT_V..CTRL_
-00003600: 414c 545f 57da 0a43 5452 4c5f 414c 545f  ALT_W..CTRL_ALT_
-00003610: 58da 0a43 5452 4c5f 414c 545f 59da 0a43  X..CTRL_ALT_Y..C
-00003620: 5452 4c5f 414c 545f 5ada 0d43 5452 4c5f  TRL_ALT_Z..CTRL_
-00003630: 5348 4946 545f 4631 da0d 4354 524c 5f53  SHIFT_F1..CTRL_S
-00003640: 4849 4654 5f46 32da 0d43 5452 4c5f 5348  HIFT_F2..CTRL_SH
-00003650: 4946 545f 4633 da0d 4354 524c 5f53 4849  IFT_F3..CTRL_SHI
-00003660: 4654 5f46 34da 0d43 5452 4c5f 5348 4946  FT_F4..CTRL_SHIF
-00003670: 545f 4635 da0d 4354 524c 5f53 4849 4654  T_F5..CTRL_SHIFT
-00003680: 5f46 36da 0d43 5452 4c5f 5348 4946 545f  _F6..CTRL_SHIFT_
-00003690: 4637 da0d 4354 524c 5f53 4849 4654 5f46  F7..CTRL_SHIFT_F
-000036a0: 38da 0d43 5452 4c5f 5348 4946 545f 4639  8..CTRL_SHIFT_F9
-000036b0: da0e 4354 524c 5f53 4849 4654 5f46 3130  ..CTRL_SHIFT_F10
-000036c0: da0e 4354 524c 5f53 4849 4654 5f46 3131  ..CTRL_SHIFT_F11
-000036d0: da0e 4354 524c 5f53 4849 4654 5f46 3132  ..CTRL_SHIFT_F12
-000036e0: da22 4354 524c 5f53 4849 4654 5f4f 454d  ."CTRL_SHIFT_OEM
-000036f0: 335f 5741 5645 5f4f 525f 4241 434b 5f51  3_WAVE_OR_BACK_Q
-00003700: 554f 5445 da10 4354 524c 5f53 4849 4654  UOTE..CTRL_SHIFT
-00003710: 5f4b 4559 5f31 da10 4354 524c 5f53 4849  _KEY_1..CTRL_SHI
-00003720: 4654 5f4b 4559 5f32 da10 4354 524c 5f53  FT_KEY_2..CTRL_S
-00003730: 4849 4654 5f4b 4559 5f33 da10 4354 524c  HIFT_KEY_3..CTRL
-00003740: 5f53 4849 4654 5f4b 4559 5f34 da10 4354  _SHIFT_KEY_4..CT
-00003750: 524c 5f53 4849 4654 5f4b 4559 5f35 da10  RL_SHIFT_KEY_5..
-00003760: 4354 524c 5f53 4849 4654 5f4b 4559 5f36  CTRL_SHIFT_KEY_6
-00003770: da10 4354 524c 5f53 4849 4654 5f4b 4559  ..CTRL_SHIFT_KEY
-00003780: 5f37 da10 4354 524c 5f53 4849 4654 5f4b  _7..CTRL_SHIFT_K
-00003790: 4559 5f38 da10 4354 524c 5f53 4849 4654  EY_8..CTRL_SHIFT
-000037a0: 5f4b 4559 5f39 da10 4354 524c 5f53 4849  _KEY_9..CTRL_SHI
-000037b0: 4654 5f4b 4559 5f30 da17 4354 524c 5f53  FT_KEY_0..CTRL_S
-000037c0: 4849 4654 5f4b 4559 5f31 315f 4d49 4e55  HIFT_KEY_11_MINU
-000037d0: 53da 1643 5452 4c5f 5348 4946 545f 4b45  S..CTRL_SHIFT_KE
-000037e0: 595f 3132 5f50 4c55 53da 1443 5452 4c5f  Y_12_PLUS..CTRL_
-000037f0: 5348 4946 545f 4241 434b 5350 4143 45da  SHIFT_BACKSPACE.
-00003800: 1343 5452 4c5f 5348 4946 545f 4e55 4d50  .CTRL_SHIFT_NUMP
-00003810: 4144 5f31 da13 4354 524c 5f53 4849 4654  AD_1..CTRL_SHIFT
-00003820: 5f4e 554d 5041 445f 32da 1343 5452 4c5f  _NUMPAD_2..CTRL_
-00003830: 5348 4946 545f 4e55 4d50 4144 5f33 da13  SHIFT_NUMPAD_3..
-00003840: 4354 524c 5f53 4849 4654 5f4e 554d 5041  CTRL_SHIFT_NUMPA
-00003850: 445f 34da 1343 5452 4c5f 5348 4946 545f  D_4..CTRL_SHIFT_
-00003860: 4e55 4d50 4144 5f35 da13 4354 524c 5f53  NUMPAD_5..CTRL_S
-00003870: 4849 4654 5f4e 554d 5041 445f 36da 1343  HIFT_NUMPAD_6..C
-00003880: 5452 4c5f 5348 4946 545f 4e55 4d50 4144  TRL_SHIFT_NUMPAD
-00003890: 5f37 da13 4354 524c 5f53 4849 4654 5f4e  _7..CTRL_SHIFT_N
-000038a0: 554d 5041 445f 38da 1343 5452 4c5f 5348  UMPAD_8..CTRL_SH
-000038b0: 4946 545f 4e55 4d50 4144 5f39 da13 4354  IFT_NUMPAD_9..CT
-000038c0: 524c 5f53 4849 4654 5f4e 554d 5041 445f  RL_SHIFT_NUMPAD_
-000038d0: 30da 1b43 5452 4c5f 5348 4946 545f 4e55  0..CTRL_SHIFT_NU
-000038e0: 4d50 4144 5f31 315f 4449 5649 4445 da1d  MPAD_11_DIVIDE..
-000038f0: 4354 524c 5f53 4849 4654 5f4e 554d 5041  CTRL_SHIFT_NUMPA
-00003900: 445f 3132 5f4d 554c 5449 504c 59da 0c43  D_12_MULTIPLY..C
-00003910: 5452 4c5f 5348 4946 545f 41da 0c43 5452  TRL_SHIFT_A..CTR
-00003920: 4c5f 5348 4946 545f 42da 0c43 5452 4c5f  L_SHIFT_B..CTRL_
-00003930: 5348 4946 545f 43da 0c43 5452 4c5f 5348  SHIFT_C..CTRL_SH
-00003940: 4946 545f 44da 0c43 5452 4c5f 5348 4946  IFT_D..CTRL_SHIF
-00003950: 545f 45da 0c43 5452 4c5f 5348 4946 545f  T_E..CTRL_SHIFT_
-00003960: 46da 0c43 5452 4c5f 5348 4946 545f 47da  F..CTRL_SHIFT_G.
-00003970: 0c43 5452 4c5f 5348 4946 545f 48da 0c43  .CTRL_SHIFT_H..C
-00003980: 5452 4c5f 5348 4946 545f 49da 0c43 5452  TRL_SHIFT_I..CTR
-00003990: 4c5f 5348 4946 545f 4ada 0c43 5452 4c5f  L_SHIFT_J..CTRL_
-000039a0: 5348 4946 545f 4bda 0c43 5452 4c5f 5348  SHIFT_K..CTRL_SH
-000039b0: 4946 545f 4cda 0c43 5452 4c5f 5348 4946  IFT_L..CTRL_SHIF
-000039c0: 545f 4dda 0c43 5452 4c5f 5348 4946 545f  T_M..CTRL_SHIFT_
-000039d0: 4eda 0c43 5452 4c5f 5348 4946 545f 4fda  N..CTRL_SHIFT_O.
-000039e0: 0c43 5452 4c5f 5348 4946 545f 50da 0c43  .CTRL_SHIFT_P..C
-000039f0: 5452 4c5f 5348 4946 545f 51da 0c43 5452  TRL_SHIFT_Q..CTR
-00003a00: 4c5f 5348 4946 545f 52da 0c43 5452 4c5f  L_SHIFT_R..CTRL_
-00003a10: 5348 4946 545f 53da 0c43 5452 4c5f 5348  SHIFT_S..CTRL_SH
-00003a20: 4946 545f 54da 0c43 5452 4c5f 5348 4946  IFT_T..CTRL_SHIF
-00003a30: 545f 55da 0c43 5452 4c5f 5348 4946 545f  T_U..CTRL_SHIFT_
-00003a40: 56da 0c43 5452 4c5f 5348 4946 545f 57da  V..CTRL_SHIFT_W.
-00003a50: 0c43 5452 4c5f 5348 4946 545f 58da 0c43  .CTRL_SHIFT_X..C
-00003a60: 5452 4c5f 5348 4946 545f 59da 0c43 5452  TRL_SHIFT_Y..CTR
-00003a70: 4c5f 5348 4946 545f 5ada 0c41 4c54 5f53  L_SHIFT_Z..ALT_S
-00003a80: 4849 4654 5f46 31da 0c41 4c54 5f53 4849  HIFT_F1..ALT_SHI
-00003a90: 4654 5f46 32da 0c41 4c54 5f53 4849 4654  FT_F2..ALT_SHIFT
-00003aa0: 5f46 33da 0c41 4c54 5f53 4849 4654 5f46  _F3..ALT_SHIFT_F
-00003ab0: 34da 0c41 4c54 5f53 4849 4654 5f46 35da  4..ALT_SHIFT_F5.
-00003ac0: 0c41 4c54 5f53 4849 4654 5f46 36da 0c41  .ALT_SHIFT_F6..A
-00003ad0: 4c54 5f53 4849 4654 5f46 37da 0c41 4c54  LT_SHIFT_F7..ALT
-00003ae0: 5f53 4849 4654 5f46 38da 0c41 4c54 5f53  _SHIFT_F8..ALT_S
-00003af0: 4849 4654 5f46 39da 0d41 4c54 5f53 4849  HIFT_F9..ALT_SHI
-00003b00: 4654 5f46 3130 da0d 414c 545f 5348 4946  FT_F10..ALT_SHIF
-00003b10: 545f 4631 31da 0d41 4c54 5f53 4849 4654  T_F11..ALT_SHIFT
-00003b20: 5f46 3132 da21 414c 545f 5348 4946 545f  _F12.!ALT_SHIFT_
-00003b30: 4f45 4d33 5f57 4156 455f 4f52 5f42 4143  OEM3_WAVE_OR_BAC
-00003b40: 4b5f 5155 4f54 45da 0f41 4c54 5f53 4849  K_QUOTE..ALT_SHI
-00003b50: 4654 5f4b 4559 5f31 da0f 414c 545f 5348  FT_KEY_1..ALT_SH
-00003b60: 4946 545f 4b45 595f 32da 0f41 4c54 5f53  IFT_KEY_2..ALT_S
-00003b70: 4849 4654 5f4b 4559 5f33 da0f 414c 545f  HIFT_KEY_3..ALT_
-00003b80: 5348 4946 545f 4b45 595f 34da 0f41 4c54  SHIFT_KEY_4..ALT
-00003b90: 5f53 4849 4654 5f4b 4559 5f35 da0f 414c  _SHIFT_KEY_5..AL
-00003ba0: 545f 5348 4946 545f 4b45 595f 36da 0f41  T_SHIFT_KEY_6..A
-00003bb0: 4c54 5f53 4849 4654 5f4b 4559 5f37 da0f  LT_SHIFT_KEY_7..
-00003bc0: 414c 545f 5348 4946 545f 4b45 595f 38da  ALT_SHIFT_KEY_8.
-00003bd0: 0f41 4c54 5f53 4849 4654 5f4b 4559 5f39  .ALT_SHIFT_KEY_9
-00003be0: da0f 414c 545f 5348 4946 545f 4b45 595f  ..ALT_SHIFT_KEY_
-00003bf0: 30da 1641 4c54 5f53 4849 4654 5f4b 4559  0..ALT_SHIFT_KEY
-00003c00: 5f31 315f 4d49 4e55 53da 1541 4c54 5f53  _11_MINUS..ALT_S
-00003c10: 4849 4654 5f4b 4559 5f31 325f 504c 5553  HIFT_KEY_12_PLUS
-00003c20: da13 414c 545f 5348 4946 545f 4241 434b  ..ALT_SHIFT_BACK
-00003c30: 5350 4143 45da 1241 4c54 5f53 4849 4654  SPACE..ALT_SHIFT
-00003c40: 5f4e 554d 5041 445f 31da 1241 4c54 5f53  _NUMPAD_1..ALT_S
-00003c50: 4849 4654 5f4e 554d 5041 445f 32da 1241  HIFT_NUMPAD_2..A
-00003c60: 4c54 5f53 4849 4654 5f4e 554d 5041 445f  LT_SHIFT_NUMPAD_
-00003c70: 33da 1241 4c54 5f53 4849 4654 5f4e 554d  3..ALT_SHIFT_NUM
-00003c80: 5041 445f 34da 1241 4c54 5f53 4849 4654  PAD_4..ALT_SHIFT
-00003c90: 5f4e 554d 5041 445f 35da 1241 4c54 5f53  _NUMPAD_5..ALT_S
-00003ca0: 4849 4654 5f4e 554d 5041 445f 36da 1241  HIFT_NUMPAD_6..A
-00003cb0: 4c54 5f53 4849 4654 5f4e 554d 5041 445f  LT_SHIFT_NUMPAD_
-00003cc0: 37da 1241 4c54 5f53 4849 4654 5f4e 554d  7..ALT_SHIFT_NUM
-00003cd0: 5041 445f 38da 1241 4c54 5f53 4849 4654  PAD_8..ALT_SHIFT
-00003ce0: 5f4e 554d 5041 445f 39da 1241 4c54 5f53  _NUMPAD_9..ALT_S
-00003cf0: 4849 4654 5f4e 554d 5041 445f 30da 1a41  HIFT_NUMPAD_0..A
-00003d00: 4c54 5f53 4849 4654 5f4e 554d 5041 445f  LT_SHIFT_NUMPAD_
-00003d10: 3131 5f44 4956 4944 45da 1c41 4c54 5f53  11_DIVIDE..ALT_S
-00003d20: 4849 4654 5f4e 554d 5041 445f 3132 5f4d  HIFT_NUMPAD_12_M
-00003d30: 554c 5449 504c 59da 0b41 4c54 5f53 4849  ULTIPLY..ALT_SHI
-00003d40: 4654 5f41 da0b 414c 545f 5348 4946 545f  FT_A..ALT_SHIFT_
-00003d50: 42da 0b41 4c54 5f53 4849 4654 5f43 da0b  B..ALT_SHIFT_C..
-00003d60: 414c 545f 5348 4946 545f 44da 0b41 4c54  ALT_SHIFT_D..ALT
-00003d70: 5f53 4849 4654 5f45 da0b 414c 545f 5348  _SHIFT_E..ALT_SH
-00003d80: 4946 545f 46da 0b41 4c54 5f53 4849 4654  IFT_F..ALT_SHIFT
-00003d90: 5f47 da0b 414c 545f 5348 4946 545f 48da  _G..ALT_SHIFT_H.
-00003da0: 0b41 4c54 5f53 4849 4654 5f49 da0b 414c  .ALT_SHIFT_I..AL
-00003db0: 545f 5348 4946 545f 4ada 0b41 4c54 5f53  T_SHIFT_J..ALT_S
-00003dc0: 4849 4654 5f4b da0b 414c 545f 5348 4946  HIFT_K..ALT_SHIF
-00003dd0: 545f 4cda 0b41 4c54 5f53 4849 4654 5f4d  T_L..ALT_SHIFT_M
-00003de0: da0b 414c 545f 5348 4946 545f 4eda 0b41  ..ALT_SHIFT_N..A
-00003df0: 4c54 5f53 4849 4654 5f4f da0b 414c 545f  LT_SHIFT_O..ALT_
-00003e00: 5348 4946 545f 50da 0b41 4c54 5f53 4849  SHIFT_P..ALT_SHI
-00003e10: 4654 5f51 da0b 414c 545f 5348 4946 545f  FT_Q..ALT_SHIFT_
-00003e20: 52da 0b41 4c54 5f53 4849 4654 5f53 da0b  R..ALT_SHIFT_S..
-00003e30: 414c 545f 5348 4946 545f 54da 0b41 4c54  ALT_SHIFT_T..ALT
-00003e40: 5f53 4849 4654 5f55 da0b 414c 545f 5348  _SHIFT_U..ALT_SH
-00003e50: 4946 545f 56da 0b41 4c54 5f53 4849 4654  IFT_V..ALT_SHIFT
-00003e60: 5f57 da0b 414c 545f 5348 4946 545f 58da  _W..ALT_SHIFT_X.
-00003e70: 0b41 4c54 5f53 4849 4654 5f59 da0b 414c  .ALT_SHIFT_Y..AL
-00003e80: 545f 5348 4946 545f 5ada 1143 5452 4c5f  T_SHIFT_Z..CTRL_
-00003e90: 5348 4946 545f 414c 545f 4631 da11 4354  SHIFT_ALT_F1..CT
-00003ea0: 524c 5f53 4849 4654 5f41 4c54 5f46 32da  RL_SHIFT_ALT_F2.
-00003eb0: 1143 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-00003ec0: 4633 da11 4354 524c 5f53 4849 4654 5f41  F3..CTRL_SHIFT_A
-00003ed0: 4c54 5f46 34da 1143 5452 4c5f 5348 4946  LT_F4..CTRL_SHIF
-00003ee0: 545f 414c 545f 4635 da11 4354 524c 5f53  T_ALT_F5..CTRL_S
-00003ef0: 4849 4654 5f41 4c54 5f46 36da 1143 5452  HIFT_ALT_F6..CTR
-00003f00: 4c5f 5348 4946 545f 414c 545f 4637 da11  L_SHIFT_ALT_F7..
-00003f10: 4354 524c 5f53 4849 4654 5f41 4c54 5f46  CTRL_SHIFT_ALT_F
-00003f20: 38da 1143 5452 4c5f 5348 4946 545f 414c  8..CTRL_SHIFT_AL
-00003f30: 545f 4639 da12 4354 524c 5f53 4849 4654  T_F9..CTRL_SHIFT
-00003f40: 5f41 4c54 5f46 3130 da12 4354 524c 5f53  _ALT_F10..CTRL_S
-00003f50: 4849 4654 5f41 4c54 5f46 3131 da12 4354  HIFT_ALT_F11..CT
-00003f60: 524c 5f53 4849 4654 5f41 4c54 5f46 3132  RL_SHIFT_ALT_F12
-00003f70: da26 4354 524c 5f53 4849 4654 5f41 4c54  .&CTRL_SHIFT_ALT
-00003f80: 5f4f 454d 335f 5741 5645 5f4f 525f 4241  _OEM3_WAVE_OR_BA
-00003f90: 434b 5f51 554f 5445 da14 4354 524c 5f53  CK_QUOTE..CTRL_S
-00003fa0: 4849 4654 5f41 4c54 5f4b 4559 5f31 da14  HIFT_ALT_KEY_1..
-00003fb0: 4354 524c 5f53 4849 4654 5f41 4c54 5f4b  CTRL_SHIFT_ALT_K
-00003fc0: 4559 5f32 da14 4354 524c 5f53 4849 4654  EY_2..CTRL_SHIFT
-00003fd0: 5f41 4c54 5f4b 4559 5f33 da14 4354 524c  _ALT_KEY_3..CTRL
-00003fe0: 5f53 4849 4654 5f41 4c54 5f4b 4559 5f34  _SHIFT_ALT_KEY_4
-00003ff0: da14 4354 524c 5f53 4849 4654 5f41 4c54  ..CTRL_SHIFT_ALT
-00004000: 5f4b 4559 5f35 da14 4354 524c 5f53 4849  _KEY_5..CTRL_SHI
-00004010: 4654 5f41 4c54 5f4b 4559 5f36 da14 4354  FT_ALT_KEY_6..CT
-00004020: 524c 5f53 4849 4654 5f41 4c54 5f4b 4559  RL_SHIFT_ALT_KEY
-00004030: 5f37 da14 4354 524c 5f53 4849 4654 5f41  _7..CTRL_SHIFT_A
-00004040: 4c54 5f4b 4559 5f38 da14 4354 524c 5f53  LT_KEY_8..CTRL_S
-00004050: 4849 4654 5f41 4c54 5f4b 4559 5f39 da14  HIFT_ALT_KEY_9..
-00004060: 4354 524c 5f53 4849 4654 5f41 4c54 5f4b  CTRL_SHIFT_ALT_K
-00004070: 4559 5f30 da1b 4354 524c 5f53 4849 4654  EY_0..CTRL_SHIFT
-00004080: 5f41 4c54 5f4b 4559 5f31 315f 4d49 4e55  _ALT_KEY_11_MINU
-00004090: 53da 1a43 5452 4c5f 5348 4946 545f 414c  S..CTRL_SHIFT_AL
-000040a0: 545f 4b45 595f 3132 5f50 4c55 53da 1843  T_KEY_12_PLUS..C
-000040b0: 5452 4c5f 5348 4946 545f 414c 545f 4241  TRL_SHIFT_ALT_BA
-000040c0: 434b 5350 4143 45da 1743 5452 4c5f 5348  CKSPACE..CTRL_SH
-000040d0: 4946 545f 414c 545f 4e55 4d50 4144 5f31  IFT_ALT_NUMPAD_1
-000040e0: da17 4354 524c 5f53 4849 4654 5f41 4c54  ..CTRL_SHIFT_ALT
-000040f0: 5f4e 554d 5041 445f 32da 1743 5452 4c5f  _NUMPAD_2..CTRL_
-00004100: 5348 4946 545f 414c 545f 4e55 4d50 4144  SHIFT_ALT_NUMPAD
-00004110: 5f33 da17 4354 524c 5f53 4849 4654 5f41  _3..CTRL_SHIFT_A
-00004120: 4c54 5f4e 554d 5041 445f 34da 1743 5452  LT_NUMPAD_4..CTR
-00004130: 4c5f 5348 4946 545f 414c 545f 4e55 4d50  L_SHIFT_ALT_NUMP
-00004140: 4144 5f35 da17 4354 524c 5f53 4849 4654  AD_5..CTRL_SHIFT
-00004150: 5f41 4c54 5f4e 554d 5041 445f 36da 1743  _ALT_NUMPAD_6..C
-00004160: 5452 4c5f 5348 4946 545f 414c 545f 4e55  TRL_SHIFT_ALT_NU
-00004170: 4d50 4144 5f37 da17 4354 524c 5f53 4849  MPAD_7..CTRL_SHI
-00004180: 4654 5f41 4c54 5f4e 554d 5041 445f 38da  FT_ALT_NUMPAD_8.
-00004190: 1743 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-000041a0: 4e55 4d50 4144 5f39 da17 4354 524c 5f53  NUMPAD_9..CTRL_S
-000041b0: 4849 4654 5f41 4c54 5f4e 554d 5041 445f  HIFT_ALT_NUMPAD_
-000041c0: 30da 1f43 5452 4c5f 5348 4946 545f 414c  0..CTRL_SHIFT_AL
-000041d0: 545f 4e55 4d50 4144 5f31 315f 4449 5649  T_NUMPAD_11_DIVI
-000041e0: 4445 da21 4354 524c 5f53 4849 4654 5f41  DE.!CTRL_SHIFT_A
-000041f0: 4c54 5f4e 554d 5041 445f 3132 5f4d 554c  LT_NUMPAD_12_MUL
-00004200: 5449 504c 59da 1043 5452 4c5f 5348 4946  TIPLY..CTRL_SHIF
-00004210: 545f 414c 545f 41da 1043 5452 4c5f 5348  T_ALT_A..CTRL_SH
-00004220: 4946 545f 414c 545f 42da 1043 5452 4c5f  IFT_ALT_B..CTRL_
-00004230: 5348 4946 545f 414c 545f 43da 1043 5452  SHIFT_ALT_C..CTR
-00004240: 4c5f 5348 4946 545f 414c 545f 44da 1043  L_SHIFT_ALT_D..C
-00004250: 5452 4c5f 5348 4946 545f 414c 545f 45da  TRL_SHIFT_ALT_E.
-00004260: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-00004270: 46da 1043 5452 4c5f 5348 4946 545f 414c  F..CTRL_SHIFT_AL
-00004280: 545f 47da 1043 5452 4c5f 5348 4946 545f  T_G..CTRL_SHIFT_
-00004290: 414c 545f 48da 1043 5452 4c5f 5348 4946  ALT_H..CTRL_SHIF
-000042a0: 545f 414c 545f 49da 1043 5452 4c5f 5348  T_ALT_I..CTRL_SH
-000042b0: 4946 545f 414c 545f 4ada 1043 5452 4c5f  IFT_ALT_J..CTRL_
-000042c0: 5348 4946 545f 414c 545f 4bda 1043 5452  SHIFT_ALT_K..CTR
-000042d0: 4c5f 5348 4946 545f 414c 545f 4cda 1043  L_SHIFT_ALT_L..C
-000042e0: 5452 4c5f 5348 4946 545f 414c 545f 4dda  TRL_SHIFT_ALT_M.
-000042f0: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-00004300: 4eda 1043 5452 4c5f 5348 4946 545f 414c  N..CTRL_SHIFT_AL
-00004310: 545f 4fda 1043 5452 4c5f 5348 4946 545f  T_O..CTRL_SHIFT_
-00004320: 414c 545f 50da 1043 5452 4c5f 5348 4946  ALT_P..CTRL_SHIF
-00004330: 545f 414c 545f 51da 1043 5452 4c5f 5348  T_ALT_Q..CTRL_SH
-00004340: 4946 545f 414c 545f 52da 1043 5452 4c5f  IFT_ALT_R..CTRL_
-00004350: 5348 4946 545f 414c 545f 53da 1043 5452  SHIFT_ALT_S..CTR
-00004360: 4c5f 5348 4946 545f 414c 545f 54da 1043  L_SHIFT_ALT_T..C
-00004370: 5452 4c5f 5348 4946 545f 414c 545f 55da  TRL_SHIFT_ALT_U.
-00004380: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-00004390: 56da 1043 5452 4c5f 5348 4946 545f 414c  V..CTRL_SHIFT_AL
-000043a0: 545f 57da 1043 5452 4c5f 5348 4946 545f  T_W..CTRL_SHIFT_
-000043b0: 414c 545f 58da 1043 5452 4c5f 5348 4946  ALT_X..CTRL_SHIF
-000043c0: 545f 414c 545f 59da 1043 5452 4c5f 5348  T_ALT_Y..CTRL_SH
-000043d0: 4946 545f 414c 545f 5a72 0d00 0000 720d  IFT_ALT_Zr....r.
-000043e0: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
-000043f0: 6d6f 6475 6c65 3e03 0000 0073 0405 0000  module>....s....
-00004400: 040c 0801 0c01 1406 0a01 0a05 0a01 0a01  ................
-00004410: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004420: 0a01 0a05 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004430: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a05  ................
+00002a60: 5445 da06 4354 524c 5f31 da06 4354 524c  TE..CTRL_1..CTRL
+00002a70: 5f32 da06 4354 524c 5f33 da06 4354 524c  _2..CTRL_3..CTRL
+00002a80: 5f34 da06 4354 524c 5f35 da06 4354 524c  _4..CTRL_5..CTRL
+00002a90: 5f36 da06 4354 524c 5f37 da06 4354 524c  _6..CTRL_7..CTRL
+00002aa0: 5f38 da06 4354 524c 5f39 da06 4354 524c  _8..CTRL_9..CTRL
+00002ab0: 5f30 da0d 4354 524c 5f31 315f 4d49 4e55  _0..CTRL_11_MINU
+00002ac0: 53da 0c43 5452 4c5f 3132 5f50 4c55 53da  S..CTRL_12_PLUS.
+00002ad0: 0e43 5452 4c5f 4241 434b 5350 4143 45da  .CTRL_BACKSPACE.
+00002ae0: 0d43 5452 4c5f 4e55 4d50 4144 5f31 da0d  .CTRL_NUMPAD_1..
+00002af0: 4354 524c 5f4e 554d 5041 445f 32da 0d43  CTRL_NUMPAD_2..C
+00002b00: 5452 4c5f 4e55 4d50 4144 5f33 da0d 4354  TRL_NUMPAD_3..CT
+00002b10: 524c 5f4e 554d 5041 445f 34da 0d43 5452  RL_NUMPAD_4..CTR
+00002b20: 4c5f 4e55 4d50 4144 5f35 da0d 4354 524c  L_NUMPAD_5..CTRL
+00002b30: 5f4e 554d 5041 445f 36da 0d43 5452 4c5f  _NUMPAD_6..CTRL_
+00002b40: 4e55 4d50 4144 5f37 da0d 4354 524c 5f4e  NUMPAD_7..CTRL_N
+00002b50: 554d 5041 445f 38da 0d43 5452 4c5f 4e55  UMPAD_8..CTRL_NU
+00002b60: 4d50 4144 5f39 da0d 4354 524c 5f4e 554d  MPAD_9..CTRL_NUM
+00002b70: 5041 445f 30da 1543 5452 4c5f 4e55 4d50  PAD_0..CTRL_NUMP
+00002b80: 4144 5f31 315f 4449 5649 4445 da17 4354  AD_11_DIVIDE..CT
+00002b90: 524c 5f4e 554d 5041 445f 3132 5f4d 554c  RL_NUMPAD_12_MUL
+00002ba0: 5449 504c 59da 0643 5452 4c5f 41da 0643  TIPLY..CTRL_A..C
+00002bb0: 5452 4c5f 42da 0643 5452 4c5f 43da 0643  TRL_B..CTRL_C..C
+00002bc0: 5452 4c5f 44da 0643 5452 4c5f 45da 0643  TRL_D..CTRL_E..C
+00002bd0: 5452 4c5f 46da 0643 5452 4c5f 47da 0643  TRL_F..CTRL_G..C
+00002be0: 5452 4c5f 48da 0643 5452 4c5f 49da 0643  TRL_H..CTRL_I..C
+00002bf0: 5452 4c5f 4ada 0643 5452 4c5f 4bda 0643  TRL_J..CTRL_K..C
+00002c00: 5452 4c5f 4cda 0643 5452 4c5f 4dda 0643  TRL_L..CTRL_M..C
+00002c10: 5452 4c5f 4eda 0643 5452 4c5f 4fda 0643  TRL_N..CTRL_O..C
+00002c20: 5452 4c5f 50da 0643 5452 4c5f 51da 0643  TRL_P..CTRL_Q..C
+00002c30: 5452 4c5f 52da 0643 5452 4c5f 53da 0643  TRL_R..CTRL_S..C
+00002c40: 5452 4c5f 54da 0643 5452 4c5f 55da 0643  TRL_T..CTRL_U..C
+00002c50: 5452 4c5f 56da 0643 5452 4c5f 57da 0643  TRL_V..CTRL_W..C
+00002c60: 5452 4c5f 58da 0643 5452 4c5f 59da 0643  TRL_X..CTRL_Y..C
+00002c70: 5452 4c5f 5ada 0953 4849 4654 5f54 4142  TRL_Z..SHIFT_TAB
+00002c80: da08 5348 4946 545f 4631 da08 5348 4946  ..SHIFT_F1..SHIF
+00002c90: 545f 4632 da08 5348 4946 545f 4633 da08  T_F2..SHIFT_F3..
+00002ca0: 5348 4946 545f 4634 da08 5348 4946 545f  SHIFT_F4..SHIFT_
+00002cb0: 4635 da08 5348 4946 545f 4636 da08 5348  F5..SHIFT_F6..SH
+00002cc0: 4946 545f 4637 da08 5348 4946 545f 4638  IFT_F7..SHIFT_F8
+00002cd0: da08 5348 4946 545f 4639 da09 5348 4946  ..SHIFT_F9..SHIF
+00002ce0: 545f 4631 30da 0953 4849 4654 5f46 3131  T_F10..SHIFT_F11
+00002cf0: da09 5348 4946 545f 4631 32da 1d53 4849  ..SHIFT_F12..SHI
+00002d00: 4654 5f4f 454d 335f 5741 5645 5f4f 525f  FT_OEM3_WAVE_OR_
+00002d10: 4241 434b 5f51 554f 5445 da07 5348 4946  BACK_QUOTE..SHIF
+00002d20: 545f 31da 0753 4849 4654 5f32 da07 5348  T_1..SHIFT_2..SH
+00002d30: 4946 545f 33da 0753 4849 4654 5f34 da07  IFT_3..SHIFT_4..
+00002d40: 5348 4946 545f 35da 0753 4849 4654 5f36  SHIFT_5..SHIFT_6
+00002d50: da07 5348 4946 545f 37da 0753 4849 4654  ..SHIFT_7..SHIFT
+00002d60: 5f38 da07 5348 4946 545f 39da 0753 4849  _8..SHIFT_9..SHI
+00002d70: 4654 5f30 da0e 5348 4946 545f 3131 5f4d  FT_0..SHIFT_11_M
+00002d80: 494e 5553 da0d 5348 4946 545f 3132 5f50  INUS..SHIFT_12_P
+00002d90: 4c55 53da 0f53 4849 4654 5f42 4143 4b53  LUS..SHIFT_BACKS
+00002da0: 5041 4345 da0e 5348 4946 545f 4e55 4d50  PACE..SHIFT_NUMP
+00002db0: 4144 5f31 da0e 5348 4946 545f 4e55 4d50  AD_1..SHIFT_NUMP
+00002dc0: 4144 5f32 da0e 5348 4946 545f 4e55 4d50  AD_2..SHIFT_NUMP
+00002dd0: 4144 5f33 da0e 5348 4946 545f 4e55 4d50  AD_3..SHIFT_NUMP
+00002de0: 4144 5f34 da0e 5348 4946 545f 4e55 4d50  AD_4..SHIFT_NUMP
+00002df0: 4144 5f35 da0e 5348 4946 545f 4e55 4d50  AD_5..SHIFT_NUMP
+00002e00: 4144 5f36 da0e 5348 4946 545f 4e55 4d50  AD_6..SHIFT_NUMP
+00002e10: 4144 5f37 da0e 5348 4946 545f 4e55 4d50  AD_7..SHIFT_NUMP
+00002e20: 4144 5f38 da0e 5348 4946 545f 4e55 4d50  AD_8..SHIFT_NUMP
+00002e30: 4144 5f39 da0e 5348 4946 545f 4e55 4d50  AD_9..SHIFT_NUMP
+00002e40: 4144 5f30 da16 5348 4946 545f 4e55 4d50  AD_0..SHIFT_NUMP
+00002e50: 4144 5f31 315f 4449 5649 4445 da18 5348  AD_11_DIVIDE..SH
+00002e60: 4946 545f 4e55 4d50 4144 5f31 325f 4d55  IFT_NUMPAD_12_MU
+00002e70: 4c54 4950 4c59 da07 5348 4946 545f 41da  LTIPLY..SHIFT_A.
+00002e80: 0753 4849 4654 5f42 da07 5348 4946 545f  .SHIFT_B..SHIFT_
+00002e90: 43da 0753 4849 4654 5f44 da07 5348 4946  C..SHIFT_D..SHIF
+00002ea0: 545f 45da 0753 4849 4654 5f46 da07 5348  T_E..SHIFT_F..SH
+00002eb0: 4946 545f 47da 0753 4849 4654 5f48 da07  IFT_G..SHIFT_H..
+00002ec0: 5348 4946 545f 49da 0753 4849 4654 5f4a  SHIFT_I..SHIFT_J
+00002ed0: da07 5348 4946 545f 4bda 0753 4849 4654  ..SHIFT_K..SHIFT
+00002ee0: 5f4c da07 5348 4946 545f 4dda 0753 4849  _L..SHIFT_M..SHI
+00002ef0: 4654 5f4e da07 5348 4946 545f 4fda 0753  FT_N..SHIFT_O..S
+00002f00: 4849 4654 5f50 da07 5348 4946 545f 51da  HIFT_P..SHIFT_Q.
+00002f10: 0753 4849 4654 5f52 da07 5348 4946 545f  .SHIFT_R..SHIFT_
+00002f20: 53da 0753 4849 4654 5f54 da07 5348 4946  S..SHIFT_T..SHIF
+00002f30: 545f 55da 0753 4849 4654 5f56 da07 5348  T_U..SHIFT_V..SH
+00002f40: 4946 545f 57da 0753 4849 4654 5f58 da07  IFT_W..SHIFT_X..
+00002f50: 5348 4946 545f 59da 0753 4849 4654 5f5a  SHIFT_Y..SHIFT_Z
+00002f60: da07 414c 545f 5441 42da 0641 4c54 5f46  ..ALT_TAB..ALT_F
+00002f70: 31da 0641 4c54 5f46 32da 0641 4c54 5f46  1..ALT_F2..ALT_F
+00002f80: 33da 0641 4c54 5f46 34da 0641 4c54 5f46  3..ALT_F4..ALT_F
+00002f90: 35da 0641 4c54 5f46 36da 0641 4c54 5f46  5..ALT_F6..ALT_F
+00002fa0: 37da 0641 4c54 5f46 38da 0641 4c54 5f46  7..ALT_F8..ALT_F
+00002fb0: 39da 0741 4c54 5f46 3130 da07 414c 545f  9..ALT_F10..ALT_
+00002fc0: 4631 31da 0741 4c54 5f46 3132 da1b 414c  F11..ALT_F12..AL
+00002fd0: 545f 4f45 4d33 5f57 4156 455f 4f52 5f42  T_OEM3_WAVE_OR_B
+00002fe0: 4143 4b5f 5155 4f54 45da 0541 4c54 5f31  ACK_QUOTE..ALT_1
+00002ff0: da05 414c 545f 32da 0541 4c54 5f33 da05  ..ALT_2..ALT_3..
+00003000: 414c 545f 34da 0541 4c54 5f35 da05 414c  ALT_4..ALT_5..AL
+00003010: 545f 36da 0541 4c54 5f37 da05 414c 545f  T_6..ALT_7..ALT_
+00003020: 38da 0541 4c54 5f39 da05 414c 545f 30da  8..ALT_9..ALT_0.
+00003030: 0c41 4c54 5f31 315f 4d49 4e55 53da 0b41  .ALT_11_MINUS..A
+00003040: 4c54 5f31 325f 504c 5553 da0d 414c 545f  LT_12_PLUS..ALT_
+00003050: 4241 434b 5350 4143 45da 0c41 4c54 5f4e  BACKSPACE..ALT_N
+00003060: 554d 5041 445f 31da 0c41 4c54 5f4e 554d  UMPAD_1..ALT_NUM
+00003070: 5041 445f 32da 0c41 4c54 5f4e 554d 5041  PAD_2..ALT_NUMPA
+00003080: 445f 33da 0c41 4c54 5f4e 554d 5041 445f  D_3..ALT_NUMPAD_
+00003090: 34da 0c41 4c54 5f4e 554d 5041 445f 35da  4..ALT_NUMPAD_5.
+000030a0: 0c41 4c54 5f4e 554d 5041 445f 36da 0c41  .ALT_NUMPAD_6..A
+000030b0: 4c54 5f4e 554d 5041 445f 37da 0c41 4c54  LT_NUMPAD_7..ALT
+000030c0: 5f4e 554d 5041 445f 38da 0c41 4c54 5f4e  _NUMPAD_8..ALT_N
+000030d0: 554d 5041 445f 39da 0c41 4c54 5f4e 554d  UMPAD_9..ALT_NUM
+000030e0: 5041 445f 30da 1441 4c54 5f4e 554d 5041  PAD_0..ALT_NUMPA
+000030f0: 445f 3131 5f44 4956 4944 45da 1641 4c54  D_11_DIVIDE..ALT
+00003100: 5f4e 554d 5041 445f 3132 5f4d 554c 5449  _NUMPAD_12_MULTI
+00003110: 504c 59da 0541 4c54 5f41 da05 414c 545f  PLY..ALT_A..ALT_
+00003120: 42da 0541 4c54 5f43 da05 414c 545f 44da  B..ALT_C..ALT_D.
+00003130: 0541 4c54 5f45 da05 414c 545f 46da 0541  .ALT_E..ALT_F..A
+00003140: 4c54 5f47 da05 414c 545f 48da 0541 4c54  LT_G..ALT_H..ALT
+00003150: 5f49 da05 414c 545f 4ada 0541 4c54 5f4b  _I..ALT_J..ALT_K
+00003160: da05 414c 545f 4cda 0541 4c54 5f4d da05  ..ALT_L..ALT_M..
+00003170: 414c 545f 4eda 0541 4c54 5f4f da05 414c  ALT_N..ALT_O..AL
+00003180: 545f 50da 0541 4c54 5f51 da05 414c 545f  T_P..ALT_Q..ALT_
+00003190: 52da 0541 4c54 5f53 da05 414c 545f 54da  R..ALT_S..ALT_T.
+000031a0: 0541 4c54 5f55 da05 414c 545f 56da 0541  .ALT_U..ALT_V..A
+000031b0: 4c54 5f57 da05 414c 545f 58da 0541 4c54  LT_W..ALT_X..ALT
+000031c0: 5f59 da05 414c 545f 5ada 0b43 5452 4c5f  _Y..ALT_Z..CTRL_
+000031d0: 414c 545f 4631 da0b 4354 524c 5f41 4c54  ALT_F1..CTRL_ALT
+000031e0: 5f46 32da 0b43 5452 4c5f 414c 545f 4633  _F2..CTRL_ALT_F3
+000031f0: da0b 4354 524c 5f41 4c54 5f46 34da 0b43  ..CTRL_ALT_F4..C
+00003200: 5452 4c5f 414c 545f 4635 da0b 4354 524c  TRL_ALT_F5..CTRL
+00003210: 5f41 4c54 5f46 36da 0b43 5452 4c5f 414c  _ALT_F6..CTRL_AL
+00003220: 545f 4637 da0b 4354 524c 5f41 4c54 5f46  T_F7..CTRL_ALT_F
+00003230: 38da 0b43 5452 4c5f 414c 545f 4639 da0c  8..CTRL_ALT_F9..
+00003240: 4354 524c 5f41 4c54 5f46 3130 da0c 4354  CTRL_ALT_F10..CT
+00003250: 524c 5f41 4c54 5f46 3131 da0c 4354 524c  RL_ALT_F11..CTRL
+00003260: 5f41 4c54 5f46 3132 da20 4354 524c 5f41  _ALT_F12. CTRL_A
+00003270: 4c54 5f4f 454d 335f 5741 5645 5f4f 525f  LT_OEM3_WAVE_OR_
+00003280: 4241 434b 5f51 554f 5445 da0a 4354 524c  BACK_QUOTE..CTRL
+00003290: 5f41 4c54 5f31 da0a 4354 524c 5f41 4c54  _ALT_1..CTRL_ALT
+000032a0: 5f32 da0a 4354 524c 5f41 4c54 5f33 da0a  _2..CTRL_ALT_3..
+000032b0: 4354 524c 5f41 4c54 5f34 da0a 4354 524c  CTRL_ALT_4..CTRL
+000032c0: 5f41 4c54 5f35 da0a 4354 524c 5f41 4c54  _ALT_5..CTRL_ALT
+000032d0: 5f36 da0a 4354 524c 5f41 4c54 5f37 da0a  _6..CTRL_ALT_7..
+000032e0: 4354 524c 5f41 4c54 5f38 da0a 4354 524c  CTRL_ALT_8..CTRL
+000032f0: 5f41 4c54 5f39 da0a 4354 524c 5f41 4c54  _ALT_9..CTRL_ALT
+00003300: 5f30 da11 4354 524c 5f41 4c54 5f31 315f  _0..CTRL_ALT_11_
+00003310: 4d49 4e55 53da 1043 5452 4c5f 414c 545f  MINUS..CTRL_ALT_
+00003320: 3132 5f50 4c55 53da 1243 5452 4c5f 414c  12_PLUS..CTRL_AL
+00003330: 545f 4241 434b 5350 4143 45da 1143 5452  T_BACKSPACE..CTR
+00003340: 4c5f 414c 545f 4e55 4d50 4144 5f31 da11  L_ALT_NUMPAD_1..
+00003350: 4354 524c 5f41 4c54 5f4e 554d 5041 445f  CTRL_ALT_NUMPAD_
+00003360: 32da 1143 5452 4c5f 414c 545f 4e55 4d50  2..CTRL_ALT_NUMP
+00003370: 4144 5f33 da11 4354 524c 5f41 4c54 5f4e  AD_3..CTRL_ALT_N
+00003380: 554d 5041 445f 34da 1143 5452 4c5f 414c  UMPAD_4..CTRL_AL
+00003390: 545f 4e55 4d50 4144 5f35 da11 4354 524c  T_NUMPAD_5..CTRL
+000033a0: 5f41 4c54 5f4e 554d 5041 445f 36da 1143  _ALT_NUMPAD_6..C
+000033b0: 5452 4c5f 414c 545f 4e55 4d50 4144 5f37  TRL_ALT_NUMPAD_7
+000033c0: da11 4354 524c 5f41 4c54 5f4e 554d 5041  ..CTRL_ALT_NUMPA
+000033d0: 445f 38da 1143 5452 4c5f 414c 545f 4e55  D_8..CTRL_ALT_NU
+000033e0: 4d50 4144 5f39 da11 4354 524c 5f41 4c54  MPAD_9..CTRL_ALT
+000033f0: 5f4e 554d 5041 445f 30da 1943 5452 4c5f  _NUMPAD_0..CTRL_
+00003400: 414c 545f 4e55 4d50 4144 5f31 315f 4449  ALT_NUMPAD_11_DI
+00003410: 5649 4445 da1b 4354 524c 5f41 4c54 5f4e  VIDE..CTRL_ALT_N
+00003420: 554d 5041 445f 3132 5f4d 554c 5449 504c  UMPAD_12_MULTIPL
+00003430: 59da 0a43 5452 4c5f 414c 545f 41da 0a43  Y..CTRL_ALT_A..C
+00003440: 5452 4c5f 414c 545f 42da 0a43 5452 4c5f  TRL_ALT_B..CTRL_
+00003450: 414c 545f 43da 0a43 5452 4c5f 414c 545f  ALT_C..CTRL_ALT_
+00003460: 44da 0a43 5452 4c5f 414c 545f 45da 0a43  D..CTRL_ALT_E..C
+00003470: 5452 4c5f 414c 545f 46da 0a43 5452 4c5f  TRL_ALT_F..CTRL_
+00003480: 414c 545f 47da 0a43 5452 4c5f 414c 545f  ALT_G..CTRL_ALT_
+00003490: 48da 0a43 5452 4c5f 414c 545f 49da 0a43  H..CTRL_ALT_I..C
+000034a0: 5452 4c5f 414c 545f 4ada 0a43 5452 4c5f  TRL_ALT_J..CTRL_
+000034b0: 414c 545f 4bda 0a43 5452 4c5f 414c 545f  ALT_K..CTRL_ALT_
+000034c0: 4cda 0a43 5452 4c5f 414c 545f 4dda 0a43  L..CTRL_ALT_M..C
+000034d0: 5452 4c5f 414c 545f 4eda 0a43 5452 4c5f  TRL_ALT_N..CTRL_
+000034e0: 414c 545f 4fda 0a43 5452 4c5f 414c 545f  ALT_O..CTRL_ALT_
+000034f0: 50da 0a43 5452 4c5f 414c 545f 51da 0a43  P..CTRL_ALT_Q..C
+00003500: 5452 4c5f 414c 545f 52da 0a43 5452 4c5f  TRL_ALT_R..CTRL_
+00003510: 414c 545f 53da 0a43 5452 4c5f 414c 545f  ALT_S..CTRL_ALT_
+00003520: 54da 0a43 5452 4c5f 414c 545f 55da 0a43  T..CTRL_ALT_U..C
+00003530: 5452 4c5f 414c 545f 56da 0a43 5452 4c5f  TRL_ALT_V..CTRL_
+00003540: 414c 545f 57da 0a43 5452 4c5f 414c 545f  ALT_W..CTRL_ALT_
+00003550: 58da 0a43 5452 4c5f 414c 545f 59da 0a43  X..CTRL_ALT_Y..C
+00003560: 5452 4c5f 414c 545f 5ada 0d43 5452 4c5f  TRL_ALT_Z..CTRL_
+00003570: 5348 4946 545f 4631 da0d 4354 524c 5f53  SHIFT_F1..CTRL_S
+00003580: 4849 4654 5f46 32da 0d43 5452 4c5f 5348  HIFT_F2..CTRL_SH
+00003590: 4946 545f 4633 da0d 4354 524c 5f53 4849  IFT_F3..CTRL_SHI
+000035a0: 4654 5f46 34da 0d43 5452 4c5f 5348 4946  FT_F4..CTRL_SHIF
+000035b0: 545f 4635 da0d 4354 524c 5f53 4849 4654  T_F5..CTRL_SHIFT
+000035c0: 5f46 36da 0d43 5452 4c5f 5348 4946 545f  _F6..CTRL_SHIFT_
+000035d0: 4637 da0d 4354 524c 5f53 4849 4654 5f46  F7..CTRL_SHIFT_F
+000035e0: 38da 0d43 5452 4c5f 5348 4946 545f 4639  8..CTRL_SHIFT_F9
+000035f0: da0e 4354 524c 5f53 4849 4654 5f46 3130  ..CTRL_SHIFT_F10
+00003600: da0e 4354 524c 5f53 4849 4654 5f46 3131  ..CTRL_SHIFT_F11
+00003610: da0e 4354 524c 5f53 4849 4654 5f46 3132  ..CTRL_SHIFT_F12
+00003620: da22 4354 524c 5f53 4849 4654 5f4f 454d  ."CTRL_SHIFT_OEM
+00003630: 335f 5741 5645 5f4f 525f 4241 434b 5f51  3_WAVE_OR_BACK_Q
+00003640: 554f 5445 da0c 4354 524c 5f53 4849 4654  UOTE..CTRL_SHIFT
+00003650: 5f31 da0c 4354 524c 5f53 4849 4654 5f32  _1..CTRL_SHIFT_2
+00003660: da0c 4354 524c 5f53 4849 4654 5f33 da0c  ..CTRL_SHIFT_3..
+00003670: 4354 524c 5f53 4849 4654 5f34 da0c 4354  CTRL_SHIFT_4..CT
+00003680: 524c 5f53 4849 4654 5f35 da0c 4354 524c  RL_SHIFT_5..CTRL
+00003690: 5f53 4849 4654 5f36 da0c 4354 524c 5f53  _SHIFT_6..CTRL_S
+000036a0: 4849 4654 5f37 da0c 4354 524c 5f53 4849  HIFT_7..CTRL_SHI
+000036b0: 4654 5f38 da0c 4354 524c 5f53 4849 4654  FT_8..CTRL_SHIFT
+000036c0: 5f39 da0c 4354 524c 5f53 4849 4654 5f30  _9..CTRL_SHIFT_0
+000036d0: da13 4354 524c 5f53 4849 4654 5f31 315f  ..CTRL_SHIFT_11_
+000036e0: 4d49 4e55 53da 1243 5452 4c5f 5348 4946  MINUS..CTRL_SHIF
+000036f0: 545f 3132 5f50 4c55 53da 1443 5452 4c5f  T_12_PLUS..CTRL_
+00003700: 5348 4946 545f 4241 434b 5350 4143 45da  SHIFT_BACKSPACE.
+00003710: 1343 5452 4c5f 5348 4946 545f 4e55 4d50  .CTRL_SHIFT_NUMP
+00003720: 4144 5f31 da13 4354 524c 5f53 4849 4654  AD_1..CTRL_SHIFT
+00003730: 5f4e 554d 5041 445f 32da 1343 5452 4c5f  _NUMPAD_2..CTRL_
+00003740: 5348 4946 545f 4e55 4d50 4144 5f33 da13  SHIFT_NUMPAD_3..
+00003750: 4354 524c 5f53 4849 4654 5f4e 554d 5041  CTRL_SHIFT_NUMPA
+00003760: 445f 34da 1343 5452 4c5f 5348 4946 545f  D_4..CTRL_SHIFT_
+00003770: 4e55 4d50 4144 5f35 da13 4354 524c 5f53  NUMPAD_5..CTRL_S
+00003780: 4849 4654 5f4e 554d 5041 445f 36da 1343  HIFT_NUMPAD_6..C
+00003790: 5452 4c5f 5348 4946 545f 4e55 4d50 4144  TRL_SHIFT_NUMPAD
+000037a0: 5f37 da13 4354 524c 5f53 4849 4654 5f4e  _7..CTRL_SHIFT_N
+000037b0: 554d 5041 445f 38da 1343 5452 4c5f 5348  UMPAD_8..CTRL_SH
+000037c0: 4946 545f 4e55 4d50 4144 5f39 da13 4354  IFT_NUMPAD_9..CT
+000037d0: 524c 5f53 4849 4654 5f4e 554d 5041 445f  RL_SHIFT_NUMPAD_
+000037e0: 30da 1b43 5452 4c5f 5348 4946 545f 4e55  0..CTRL_SHIFT_NU
+000037f0: 4d50 4144 5f31 315f 4449 5649 4445 da1d  MPAD_11_DIVIDE..
+00003800: 4354 524c 5f53 4849 4654 5f4e 554d 5041  CTRL_SHIFT_NUMPA
+00003810: 445f 3132 5f4d 554c 5449 504c 59da 0c43  D_12_MULTIPLY..C
+00003820: 5452 4c5f 5348 4946 545f 41da 0c43 5452  TRL_SHIFT_A..CTR
+00003830: 4c5f 5348 4946 545f 42da 0c43 5452 4c5f  L_SHIFT_B..CTRL_
+00003840: 5348 4946 545f 43da 0c43 5452 4c5f 5348  SHIFT_C..CTRL_SH
+00003850: 4946 545f 44da 0c43 5452 4c5f 5348 4946  IFT_D..CTRL_SHIF
+00003860: 545f 45da 0c43 5452 4c5f 5348 4946 545f  T_E..CTRL_SHIFT_
+00003870: 46da 0c43 5452 4c5f 5348 4946 545f 47da  F..CTRL_SHIFT_G.
+00003880: 0c43 5452 4c5f 5348 4946 545f 48da 0c43  .CTRL_SHIFT_H..C
+00003890: 5452 4c5f 5348 4946 545f 49da 0c43 5452  TRL_SHIFT_I..CTR
+000038a0: 4c5f 5348 4946 545f 4ada 0c43 5452 4c5f  L_SHIFT_J..CTRL_
+000038b0: 5348 4946 545f 4bda 0c43 5452 4c5f 5348  SHIFT_K..CTRL_SH
+000038c0: 4946 545f 4cda 0c43 5452 4c5f 5348 4946  IFT_L..CTRL_SHIF
+000038d0: 545f 4dda 0c43 5452 4c5f 5348 4946 545f  T_M..CTRL_SHIFT_
+000038e0: 4eda 0c43 5452 4c5f 5348 4946 545f 4fda  N..CTRL_SHIFT_O.
+000038f0: 0c43 5452 4c5f 5348 4946 545f 50da 0c43  .CTRL_SHIFT_P..C
+00003900: 5452 4c5f 5348 4946 545f 51da 0c43 5452  TRL_SHIFT_Q..CTR
+00003910: 4c5f 5348 4946 545f 52da 0c43 5452 4c5f  L_SHIFT_R..CTRL_
+00003920: 5348 4946 545f 53da 0c43 5452 4c5f 5348  SHIFT_S..CTRL_SH
+00003930: 4946 545f 54da 0c43 5452 4c5f 5348 4946  IFT_T..CTRL_SHIF
+00003940: 545f 55da 0c43 5452 4c5f 5348 4946 545f  T_U..CTRL_SHIFT_
+00003950: 56da 0c43 5452 4c5f 5348 4946 545f 57da  V..CTRL_SHIFT_W.
+00003960: 0c43 5452 4c5f 5348 4946 545f 58da 0c43  .CTRL_SHIFT_X..C
+00003970: 5452 4c5f 5348 4946 545f 59da 0c43 5452  TRL_SHIFT_Y..CTR
+00003980: 4c5f 5348 4946 545f 5ada 0c41 4c54 5f53  L_SHIFT_Z..ALT_S
+00003990: 4849 4654 5f46 31da 0c41 4c54 5f53 4849  HIFT_F1..ALT_SHI
+000039a0: 4654 5f46 32da 0c41 4c54 5f53 4849 4654  FT_F2..ALT_SHIFT
+000039b0: 5f46 33da 0c41 4c54 5f53 4849 4654 5f46  _F3..ALT_SHIFT_F
+000039c0: 34da 0c41 4c54 5f53 4849 4654 5f46 35da  4..ALT_SHIFT_F5.
+000039d0: 0c41 4c54 5f53 4849 4654 5f46 36da 0c41  .ALT_SHIFT_F6..A
+000039e0: 4c54 5f53 4849 4654 5f46 37da 0c41 4c54  LT_SHIFT_F7..ALT
+000039f0: 5f53 4849 4654 5f46 38da 0c41 4c54 5f53  _SHIFT_F8..ALT_S
+00003a00: 4849 4654 5f46 39da 0d41 4c54 5f53 4849  HIFT_F9..ALT_SHI
+00003a10: 4654 5f46 3130 da0d 414c 545f 5348 4946  FT_F10..ALT_SHIF
+00003a20: 545f 4631 31da 0d41 4c54 5f53 4849 4654  T_F11..ALT_SHIFT
+00003a30: 5f46 3132 da21 414c 545f 5348 4946 545f  _F12.!ALT_SHIFT_
+00003a40: 4f45 4d33 5f57 4156 455f 4f52 5f42 4143  OEM3_WAVE_OR_BAC
+00003a50: 4b5f 5155 4f54 45da 0b41 4c54 5f53 4849  K_QUOTE..ALT_SHI
+00003a60: 4654 5f31 da0b 414c 545f 5348 4946 545f  FT_1..ALT_SHIFT_
+00003a70: 32da 0b41 4c54 5f53 4849 4654 5f33 da0b  2..ALT_SHIFT_3..
+00003a80: 414c 545f 5348 4946 545f 34da 0b41 4c54  ALT_SHIFT_4..ALT
+00003a90: 5f53 4849 4654 5f35 da0b 414c 545f 5348  _SHIFT_5..ALT_SH
+00003aa0: 4946 545f 36da 0b41 4c54 5f53 4849 4654  IFT_6..ALT_SHIFT
+00003ab0: 5f37 da0b 414c 545f 5348 4946 545f 38da  _7..ALT_SHIFT_8.
+00003ac0: 0b41 4c54 5f53 4849 4654 5f39 da0b 414c  .ALT_SHIFT_9..AL
+00003ad0: 545f 5348 4946 545f 30da 1241 4c54 5f53  T_SHIFT_0..ALT_S
+00003ae0: 4849 4654 5f31 315f 4d49 4e55 53da 1141  HIFT_11_MINUS..A
+00003af0: 4c54 5f53 4849 4654 5f31 325f 504c 5553  LT_SHIFT_12_PLUS
+00003b00: da13 414c 545f 5348 4946 545f 4241 434b  ..ALT_SHIFT_BACK
+00003b10: 5350 4143 45da 1241 4c54 5f53 4849 4654  SPACE..ALT_SHIFT
+00003b20: 5f4e 554d 5041 445f 31da 1241 4c54 5f53  _NUMPAD_1..ALT_S
+00003b30: 4849 4654 5f4e 554d 5041 445f 32da 1241  HIFT_NUMPAD_2..A
+00003b40: 4c54 5f53 4849 4654 5f4e 554d 5041 445f  LT_SHIFT_NUMPAD_
+00003b50: 33da 1241 4c54 5f53 4849 4654 5f4e 554d  3..ALT_SHIFT_NUM
+00003b60: 5041 445f 34da 1241 4c54 5f53 4849 4654  PAD_4..ALT_SHIFT
+00003b70: 5f4e 554d 5041 445f 35da 1241 4c54 5f53  _NUMPAD_5..ALT_S
+00003b80: 4849 4654 5f4e 554d 5041 445f 36da 1241  HIFT_NUMPAD_6..A
+00003b90: 4c54 5f53 4849 4654 5f4e 554d 5041 445f  LT_SHIFT_NUMPAD_
+00003ba0: 37da 1241 4c54 5f53 4849 4654 5f4e 554d  7..ALT_SHIFT_NUM
+00003bb0: 5041 445f 38da 1241 4c54 5f53 4849 4654  PAD_8..ALT_SHIFT
+00003bc0: 5f4e 554d 5041 445f 39da 1241 4c54 5f53  _NUMPAD_9..ALT_S
+00003bd0: 4849 4654 5f4e 554d 5041 445f 30da 1a41  HIFT_NUMPAD_0..A
+00003be0: 4c54 5f53 4849 4654 5f4e 554d 5041 445f  LT_SHIFT_NUMPAD_
+00003bf0: 3131 5f44 4956 4944 45da 1c41 4c54 5f53  11_DIVIDE..ALT_S
+00003c00: 4849 4654 5f4e 554d 5041 445f 3132 5f4d  HIFT_NUMPAD_12_M
+00003c10: 554c 5449 504c 59da 0b41 4c54 5f53 4849  ULTIPLY..ALT_SHI
+00003c20: 4654 5f41 da0b 414c 545f 5348 4946 545f  FT_A..ALT_SHIFT_
+00003c30: 42da 0b41 4c54 5f53 4849 4654 5f43 da0b  B..ALT_SHIFT_C..
+00003c40: 414c 545f 5348 4946 545f 44da 0b41 4c54  ALT_SHIFT_D..ALT
+00003c50: 5f53 4849 4654 5f45 da0b 414c 545f 5348  _SHIFT_E..ALT_SH
+00003c60: 4946 545f 46da 0b41 4c54 5f53 4849 4654  IFT_F..ALT_SHIFT
+00003c70: 5f47 da0b 414c 545f 5348 4946 545f 48da  _G..ALT_SHIFT_H.
+00003c80: 0b41 4c54 5f53 4849 4654 5f49 da0b 414c  .ALT_SHIFT_I..AL
+00003c90: 545f 5348 4946 545f 4ada 0b41 4c54 5f53  T_SHIFT_J..ALT_S
+00003ca0: 4849 4654 5f4b da0b 414c 545f 5348 4946  HIFT_K..ALT_SHIF
+00003cb0: 545f 4cda 0b41 4c54 5f53 4849 4654 5f4d  T_L..ALT_SHIFT_M
+00003cc0: da0b 414c 545f 5348 4946 545f 4eda 0b41  ..ALT_SHIFT_N..A
+00003cd0: 4c54 5f53 4849 4654 5f4f da0b 414c 545f  LT_SHIFT_O..ALT_
+00003ce0: 5348 4946 545f 50da 0b41 4c54 5f53 4849  SHIFT_P..ALT_SHI
+00003cf0: 4654 5f51 da0b 414c 545f 5348 4946 545f  FT_Q..ALT_SHIFT_
+00003d00: 52da 0b41 4c54 5f53 4849 4654 5f53 da0b  R..ALT_SHIFT_S..
+00003d10: 414c 545f 5348 4946 545f 54da 0b41 4c54  ALT_SHIFT_T..ALT
+00003d20: 5f53 4849 4654 5f55 da0b 414c 545f 5348  _SHIFT_U..ALT_SH
+00003d30: 4946 545f 56da 0b41 4c54 5f53 4849 4654  IFT_V..ALT_SHIFT
+00003d40: 5f57 da0b 414c 545f 5348 4946 545f 58da  _W..ALT_SHIFT_X.
+00003d50: 0b41 4c54 5f53 4849 4654 5f59 da0b 414c  .ALT_SHIFT_Y..AL
+00003d60: 545f 5348 4946 545f 5ada 1143 5452 4c5f  T_SHIFT_Z..CTRL_
+00003d70: 5348 4946 545f 414c 545f 4631 da11 4354  SHIFT_ALT_F1..CT
+00003d80: 524c 5f53 4849 4654 5f41 4c54 5f46 32da  RL_SHIFT_ALT_F2.
+00003d90: 1143 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+00003da0: 4633 da11 4354 524c 5f53 4849 4654 5f41  F3..CTRL_SHIFT_A
+00003db0: 4c54 5f46 34da 1143 5452 4c5f 5348 4946  LT_F4..CTRL_SHIF
+00003dc0: 545f 414c 545f 4635 da11 4354 524c 5f53  T_ALT_F5..CTRL_S
+00003dd0: 4849 4654 5f41 4c54 5f46 36da 1143 5452  HIFT_ALT_F6..CTR
+00003de0: 4c5f 5348 4946 545f 414c 545f 4637 da11  L_SHIFT_ALT_F7..
+00003df0: 4354 524c 5f53 4849 4654 5f41 4c54 5f46  CTRL_SHIFT_ALT_F
+00003e00: 38da 1143 5452 4c5f 5348 4946 545f 414c  8..CTRL_SHIFT_AL
+00003e10: 545f 4639 da12 4354 524c 5f53 4849 4654  T_F9..CTRL_SHIFT
+00003e20: 5f41 4c54 5f46 3130 da12 4354 524c 5f53  _ALT_F10..CTRL_S
+00003e30: 4849 4654 5f41 4c54 5f46 3131 da12 4354  HIFT_ALT_F11..CT
+00003e40: 524c 5f53 4849 4654 5f41 4c54 5f46 3132  RL_SHIFT_ALT_F12
+00003e50: da26 4354 524c 5f53 4849 4654 5f41 4c54  .&CTRL_SHIFT_ALT
+00003e60: 5f4f 454d 335f 5741 5645 5f4f 525f 4241  _OEM3_WAVE_OR_BA
+00003e70: 434b 5f51 554f 5445 da10 4354 524c 5f53  CK_QUOTE..CTRL_S
+00003e80: 4849 4654 5f41 4c54 5f31 da10 4354 524c  HIFT_ALT_1..CTRL
+00003e90: 5f53 4849 4654 5f41 4c54 5f32 da10 4354  _SHIFT_ALT_2..CT
+00003ea0: 524c 5f53 4849 4654 5f41 4c54 5f33 da10  RL_SHIFT_ALT_3..
+00003eb0: 4354 524c 5f53 4849 4654 5f41 4c54 5f34  CTRL_SHIFT_ALT_4
+00003ec0: da10 4354 524c 5f53 4849 4654 5f41 4c54  ..CTRL_SHIFT_ALT
+00003ed0: 5f35 da10 4354 524c 5f53 4849 4654 5f41  _5..CTRL_SHIFT_A
+00003ee0: 4c54 5f36 da10 4354 524c 5f53 4849 4654  LT_6..CTRL_SHIFT
+00003ef0: 5f41 4c54 5f37 da10 4354 524c 5f53 4849  _ALT_7..CTRL_SHI
+00003f00: 4654 5f41 4c54 5f38 da10 4354 524c 5f53  FT_ALT_8..CTRL_S
+00003f10: 4849 4654 5f41 4c54 5f39 da10 4354 524c  HIFT_ALT_9..CTRL
+00003f20: 5f53 4849 4654 5f41 4c54 5f30 da17 4354  _SHIFT_ALT_0..CT
+00003f30: 524c 5f53 4849 4654 5f41 4c54 5f31 315f  RL_SHIFT_ALT_11_
+00003f40: 4d49 4e55 53da 1643 5452 4c5f 5348 4946  MINUS..CTRL_SHIF
+00003f50: 545f 414c 545f 3132 5f50 4c55 53da 1843  T_ALT_12_PLUS..C
+00003f60: 5452 4c5f 5348 4946 545f 414c 545f 4241  TRL_SHIFT_ALT_BA
+00003f70: 434b 5350 4143 45da 1743 5452 4c5f 5348  CKSPACE..CTRL_SH
+00003f80: 4946 545f 414c 545f 4e55 4d50 4144 5f31  IFT_ALT_NUMPAD_1
+00003f90: da17 4354 524c 5f53 4849 4654 5f41 4c54  ..CTRL_SHIFT_ALT
+00003fa0: 5f4e 554d 5041 445f 32da 1743 5452 4c5f  _NUMPAD_2..CTRL_
+00003fb0: 5348 4946 545f 414c 545f 4e55 4d50 4144  SHIFT_ALT_NUMPAD
+00003fc0: 5f33 da17 4354 524c 5f53 4849 4654 5f41  _3..CTRL_SHIFT_A
+00003fd0: 4c54 5f4e 554d 5041 445f 34da 1743 5452  LT_NUMPAD_4..CTR
+00003fe0: 4c5f 5348 4946 545f 414c 545f 4e55 4d50  L_SHIFT_ALT_NUMP
+00003ff0: 4144 5f35 da17 4354 524c 5f53 4849 4654  AD_5..CTRL_SHIFT
+00004000: 5f41 4c54 5f4e 554d 5041 445f 36da 1743  _ALT_NUMPAD_6..C
+00004010: 5452 4c5f 5348 4946 545f 414c 545f 4e55  TRL_SHIFT_ALT_NU
+00004020: 4d50 4144 5f37 da17 4354 524c 5f53 4849  MPAD_7..CTRL_SHI
+00004030: 4654 5f41 4c54 5f4e 554d 5041 445f 38da  FT_ALT_NUMPAD_8.
+00004040: 1743 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+00004050: 4e55 4d50 4144 5f39 da17 4354 524c 5f53  NUMPAD_9..CTRL_S
+00004060: 4849 4654 5f41 4c54 5f4e 554d 5041 445f  HIFT_ALT_NUMPAD_
+00004070: 30da 1f43 5452 4c5f 5348 4946 545f 414c  0..CTRL_SHIFT_AL
+00004080: 545f 4e55 4d50 4144 5f31 315f 4449 5649  T_NUMPAD_11_DIVI
+00004090: 4445 da21 4354 524c 5f53 4849 4654 5f41  DE.!CTRL_SHIFT_A
+000040a0: 4c54 5f4e 554d 5041 445f 3132 5f4d 554c  LT_NUMPAD_12_MUL
+000040b0: 5449 504c 59da 1043 5452 4c5f 5348 4946  TIPLY..CTRL_SHIF
+000040c0: 545f 414c 545f 41da 1043 5452 4c5f 5348  T_ALT_A..CTRL_SH
+000040d0: 4946 545f 414c 545f 42da 1043 5452 4c5f  IFT_ALT_B..CTRL_
+000040e0: 5348 4946 545f 414c 545f 43da 1043 5452  SHIFT_ALT_C..CTR
+000040f0: 4c5f 5348 4946 545f 414c 545f 44da 1043  L_SHIFT_ALT_D..C
+00004100: 5452 4c5f 5348 4946 545f 414c 545f 45da  TRL_SHIFT_ALT_E.
+00004110: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+00004120: 46da 1043 5452 4c5f 5348 4946 545f 414c  F..CTRL_SHIFT_AL
+00004130: 545f 47da 1043 5452 4c5f 5348 4946 545f  T_G..CTRL_SHIFT_
+00004140: 414c 545f 48da 1043 5452 4c5f 5348 4946  ALT_H..CTRL_SHIF
+00004150: 545f 414c 545f 49da 1043 5452 4c5f 5348  T_ALT_I..CTRL_SH
+00004160: 4946 545f 414c 545f 4ada 1043 5452 4c5f  IFT_ALT_J..CTRL_
+00004170: 5348 4946 545f 414c 545f 4bda 1043 5452  SHIFT_ALT_K..CTR
+00004180: 4c5f 5348 4946 545f 414c 545f 4cda 1043  L_SHIFT_ALT_L..C
+00004190: 5452 4c5f 5348 4946 545f 414c 545f 4dda  TRL_SHIFT_ALT_M.
+000041a0: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+000041b0: 4eda 1043 5452 4c5f 5348 4946 545f 414c  N..CTRL_SHIFT_AL
+000041c0: 545f 4fda 1043 5452 4c5f 5348 4946 545f  T_O..CTRL_SHIFT_
+000041d0: 414c 545f 50da 1043 5452 4c5f 5348 4946  ALT_P..CTRL_SHIF
+000041e0: 545f 414c 545f 51da 1043 5452 4c5f 5348  T_ALT_Q..CTRL_SH
+000041f0: 4946 545f 414c 545f 52da 1043 5452 4c5f  IFT_ALT_R..CTRL_
+00004200: 5348 4946 545f 414c 545f 53da 1043 5452  SHIFT_ALT_S..CTR
+00004210: 4c5f 5348 4946 545f 414c 545f 54da 1043  L_SHIFT_ALT_T..C
+00004220: 5452 4c5f 5348 4946 545f 414c 545f 55da  TRL_SHIFT_ALT_U.
+00004230: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+00004240: 56da 1043 5452 4c5f 5348 4946 545f 414c  V..CTRL_SHIFT_AL
+00004250: 545f 57da 1043 5452 4c5f 5348 4946 545f  T_W..CTRL_SHIFT_
+00004260: 414c 545f 58da 1043 5452 4c5f 5348 4946  ALT_X..CTRL_SHIF
+00004270: 545f 414c 545f 59da 1043 5452 4c5f 5348  T_ALT_Y..CTRL_SH
+00004280: 4946 545f 414c 545f 5a72 0d00 0000 720d  IFT_ALT_Zr....r.
+00004290: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
+000042a0: 6d6f 6475 6c65 3e03 0000 0073 0405 0000  module>....s....
+000042b0: 040c 0801 0c01 1406 0a01 0a05 0a01 0a01  ................
+000042c0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000042d0: 0a01 0a05 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000042e0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a05  ................
+000042f0: 0a01 0a01 0a01 0a01 0a02 0a01 0a01 0a01  ................
+00004300: 0a01 0a01 0a02 0a02 0a01 0a05 0a01 0a01  ................
+00004310: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00004320: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00004330: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a05  ................
+00004340: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00004350: 0a05 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00004360: 0a01 0a01 0a05 0a02 0a01 0a01 0a01 0a01  ................
+00004370: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a02  ................
+00004380: 0a01 0a01 0a01 0a02 0a01 0a01 0a01 0a01  ................
+00004390: 0a01 0a01 0a01 0a01 0a02 0a05 0a01 0a01  ................
+000043a0: 0a01 0a01 0a02 0401 0401 0402 0e01 0e01  ................
+000043b0: 0e01 0e01 0e01 0e01 0e01 0e01 0e06 0201  ................
+000043c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000043d0: 0201 0201 02f4 0410 0201 0201 0201 0201  ................
+000043e0: 0201 02fa 040a 0201 0201 0201 0201 0201  ................
+000043f0: 0201 0201 0201 0201 0201 0201 02f4 0410  ................
+00004400: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00004410: 0201 0201 0201 02f4 0413 1a09 1c06 1a04  ................
+00004420: 1a04 1a07 1a04 1a04 1a07 1a07 1a07 1a0b  ................
+00004430: 0a02 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00004440: 0a01 0a01 0a01 0a01 0a02 0a01 0a01 0a01  ................
-00004450: 0a01 0a01 0a02 0a02 0a01 0a05 0a01 0a01  ................
-00004460: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004470: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004480: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a05  ................
+00004450: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00004460: 0a01 0a01 0a02 0a01 0a01 0a01 0a01 0a01  ................
+00004470: 0a01 0a01 0a01 0a01 0a01 0a01 0a02 0a01  ................
+00004480: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00004490: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-000044a0: 0a05 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-000044b0: 0a01 0a01 0a05 0a02 0a01 0a01 0a01 0a01  ................
-000044c0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a02  ................
-000044d0: 0a01 0a01 0a01 0a02 0a01 0a01 0a01 0a01  ................
-000044e0: 0a01 0a01 0a01 0a01 0a02 0a05 0a01 0a01  ................
-000044f0: 0a01 0a01 0a02 0401 0401 0402 0e01 0e01  ................
-00004500: 0e01 0e01 0e01 0e01 0e01 0e01 0e06 0201  ................
-00004510: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00004520: 0201 0201 02f4 0410 0201 0201 0201 0201  ................
-00004530: 0201 02fa 040a 0201 0201 0201 0201 0201  ................
-00004540: 0201 0201 0201 0201 0201 0201 02f4 0410  ................
-00004550: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00004560: 0201 0201 0201 02f4 0413 1a09 1c06 1a04  ................
-00004570: 1a04 1a07 1a04 1a04 1a07 1a07 1a07 1a0b  ................
-00004580: 0a02 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004590: 0a01 0a01 0a01 0a01 0a02 0a01 0a01 0a01  ................
-000045a0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-000045b0: 0a01 0a01 0a02 0a01 0a01 0a01 0a01 0a01  ................
-000045c0: 0a01 0a01 0a01 0a01 0a01 0a01 0a02 0a01  ................
-000045d0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-000045e0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-000045f0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004600: 0a03 0a02 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004610: 0a01 0a01 0a01 0a01 0a01 0a02 0a01 0a01  ................
-00004620: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00004630: 0a01 0a01 0a01 0a02 0a01 0a01 0a01 0c01  ................
-00004640: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c02  ................
+000044a0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000044b0: 0a03 0a02 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000044c0: 0a01 0a01 0a01 0a01 0a01 0a02 0a01 0a01  ................
+000044d0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000044e0: 0a01 0a01 0a01 0a02 0a01 0a01 0a01 0c01  ................
+000044f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c02  ................
+00004500: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004510: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004520: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004530: 0c01 0c03 0c02 0c01 0c01 0c01 0c01 0c01  ................
+00004540: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+00004550: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004560: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
+00004570: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004580: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004590: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000045a0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000045b0: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
+000045c0: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+000045d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000045e0: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
+000045f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004600: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004610: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004620: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004630: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
+00004640: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
 00004650: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004660: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004660: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
 00004670: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004680: 0c01 0c03 0c02 0c01 0c01 0c01 0c01 0c01  ................
-00004690: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+00004680: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004690: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
 000046a0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000046b0: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
-000046c0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000046d0: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000046e0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000046b0: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
+000046c0: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+000046d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000046e0: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
 000046f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004700: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
-00004710: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+00004700: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004710: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
 00004720: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004730: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
-00004740: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004750: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004760: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004730: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
+00004740: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+00004750: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004760: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
 00004770: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004780: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
-00004790: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
+00004780: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00004790: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
 000047a0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000047b0: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
-000047c0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000047d0: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000047e0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000047f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004800: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
-00004810: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
-00004820: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004830: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
-00004840: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004850: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004860: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004870: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004880: 0c01 0c01 0c03 0c01 0c01 0c01 0c01 0c01  ................
-00004890: 0c01 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
-000048a0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000048b0: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 0c01  ................
-000048c0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000048d0: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000048e0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000048f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00004900: 0c01 0c01                                ....
+000047b0: 0c01 0c01                                ....
```

### Comparing `hotkeynet-0.1.3/hotkeynet/__pycache__/keyname.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/__pycache__/keyname.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May  9 04:33:49 2023 UTC, .py size: 21156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2dcd 5964 a452 0000  U.......-.Yd.R..
+00000000: 550d 0d0a 0000 0000 cad0 5964 5451 0000  U.........YdTQ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 a613 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6409 5a09 640a 5a0a 640b 5a0b 640c  Z.d.Z.d.Z.d.Z.d.
 00000060: 5a0c 640d 5a0d 640e 5a0e 640f 5a0f 6410  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a10 6411 5a11 6412 5a12 6413 5a13 6414  Z.d.Z.d.Z.d.Z.d.
@@ -574,496 +574,475 @@
 000023d0: 5a07 4354 524c 5f46 335a 0743 5452 4c5f  Z.CTRL_F3Z.CTRL_
 000023e0: 4634 5a07 4354 524c 5f46 355a 0743 5452  F4Z.CTRL_F5Z.CTR
 000023f0: 4c5f 4636 5a07 4354 524c 5f46 375a 0743  L_F6Z.CTRL_F7Z.C
 00002400: 5452 4c5f 4638 5a07 4354 524c 5f46 395a  TRL_F8Z.CTRL_F9Z
 00002410: 0843 5452 4c5f 4631 305a 0843 5452 4c5f  .CTRL_F10Z.CTRL_
 00002420: 4631 315a 0843 5452 4c5f 4631 325a 1c43  F11Z.CTRL_F12Z.C
 00002430: 5452 4c5f 4f45 4d33 5f57 4156 455f 4f52  TRL_OEM3_WAVE_OR
-00002440: 5f42 4143 4b5f 5155 4f54 455a 0a43 5452  _BACK_QUOTEZ.CTR
-00002450: 4c5f 4b45 595f 315a 0a43 5452 4c5f 4b45  L_KEY_1Z.CTRL_KE
-00002460: 595f 325a 0a43 5452 4c5f 4b45 595f 335a  Y_2Z.CTRL_KEY_3Z
-00002470: 0a43 5452 4c5f 4b45 595f 345a 0a43 5452  .CTRL_KEY_4Z.CTR
-00002480: 4c5f 4b45 595f 355a 0a43 5452 4c5f 4b45  L_KEY_5Z.CTRL_KE
-00002490: 595f 365a 0a43 5452 4c5f 4b45 595f 375a  Y_6Z.CTRL_KEY_7Z
-000024a0: 0a43 5452 4c5f 4b45 595f 385a 0a43 5452  .CTRL_KEY_8Z.CTR
-000024b0: 4c5f 4b45 595f 395a 0a43 5452 4c5f 4b45  L_KEY_9Z.CTRL_KE
-000024c0: 595f 305a 1143 5452 4c5f 4b45 595f 3131  Y_0Z.CTRL_KEY_11
-000024d0: 5f4d 494e 5553 5a10 4354 524c 5f4b 4559  _MINUSZ.CTRL_KEY
-000024e0: 5f31 325f 504c 5553 5a0e 4354 524c 5f42  _12_PLUSZ.CTRL_B
-000024f0: 4143 4b53 5041 4345 5a0d 4354 524c 5f4e  ACKSPACEZ.CTRL_N
-00002500: 554d 5041 445f 315a 0d43 5452 4c5f 4e55  UMPAD_1Z.CTRL_NU
-00002510: 4d50 4144 5f32 5a0d 4354 524c 5f4e 554d  MPAD_2Z.CTRL_NUM
-00002520: 5041 445f 335a 0d43 5452 4c5f 4e55 4d50  PAD_3Z.CTRL_NUMP
-00002530: 4144 5f34 5a0d 4354 524c 5f4e 554d 5041  AD_4Z.CTRL_NUMPA
-00002540: 445f 355a 0d43 5452 4c5f 4e55 4d50 4144  D_5Z.CTRL_NUMPAD
-00002550: 5f36 5a0d 4354 524c 5f4e 554d 5041 445f  _6Z.CTRL_NUMPAD_
-00002560: 375a 0d43 5452 4c5f 4e55 4d50 4144 5f38  7Z.CTRL_NUMPAD_8
-00002570: 5a0d 4354 524c 5f4e 554d 5041 445f 395a  Z.CTRL_NUMPAD_9Z
-00002580: 0d43 5452 4c5f 4e55 4d50 4144 5f30 5a15  .CTRL_NUMPAD_0Z.
-00002590: 4354 524c 5f4e 554d 5041 445f 3131 5f44  CTRL_NUMPAD_11_D
-000025a0: 4956 4944 455a 1743 5452 4c5f 4e55 4d50  IVIDEZ.CTRL_NUMP
-000025b0: 4144 5f31 325f 4d55 4c54 4950 4c59 5a06  AD_12_MULTIPLYZ.
-000025c0: 4354 524c 5f41 5a06 4354 524c 5f42 5a06  CTRL_AZ.CTRL_BZ.
-000025d0: 4354 524c 5f43 5a06 4354 524c 5f44 5a06  CTRL_CZ.CTRL_DZ.
-000025e0: 4354 524c 5f45 5a06 4354 524c 5f46 5a06  CTRL_EZ.CTRL_FZ.
-000025f0: 4354 524c 5f47 5a06 4354 524c 5f48 5a06  CTRL_GZ.CTRL_HZ.
-00002600: 4354 524c 5f49 5a06 4354 524c 5f4a 5a06  CTRL_IZ.CTRL_JZ.
-00002610: 4354 524c 5f4b 5a06 4354 524c 5f4c 5a06  CTRL_KZ.CTRL_LZ.
-00002620: 4354 524c 5f4d 5a06 4354 524c 5f4e 5a06  CTRL_MZ.CTRL_NZ.
-00002630: 4354 524c 5f4f 5a06 4354 524c 5f50 5a06  CTRL_OZ.CTRL_PZ.
-00002640: 4354 524c 5f51 5a06 4354 524c 5f52 5a06  CTRL_QZ.CTRL_RZ.
-00002650: 4354 524c 5f53 5a06 4354 524c 5f54 5a06  CTRL_SZ.CTRL_TZ.
-00002660: 4354 524c 5f55 5a06 4354 524c 5f56 5a06  CTRL_UZ.CTRL_VZ.
-00002670: 4354 524c 5f57 5a06 4354 524c 5f58 5a06  CTRL_WZ.CTRL_XZ.
-00002680: 4354 524c 5f59 5a06 4354 524c 5f5a 5a09  CTRL_YZ.CTRL_ZZ.
-00002690: 5348 4946 545f 5441 425a 0853 4849 4654  SHIFT_TABZ.SHIFT
-000026a0: 5f46 315a 0853 4849 4654 5f46 325a 0853  _F1Z.SHIFT_F2Z.S
-000026b0: 4849 4654 5f46 335a 0853 4849 4654 5f46  HIFT_F3Z.SHIFT_F
-000026c0: 345a 0853 4849 4654 5f46 355a 0853 4849  4Z.SHIFT_F5Z.SHI
-000026d0: 4654 5f46 365a 0853 4849 4654 5f46 375a  FT_F6Z.SHIFT_F7Z
-000026e0: 0853 4849 4654 5f46 385a 0853 4849 4654  .SHIFT_F8Z.SHIFT
-000026f0: 5f46 395a 0953 4849 4654 5f46 3130 5a09  _F9Z.SHIFT_F10Z.
-00002700: 5348 4946 545f 4631 315a 0953 4849 4654  SHIFT_F11Z.SHIFT
-00002710: 5f46 3132 5a1d 5348 4946 545f 4f45 4d33  _F12Z.SHIFT_OEM3
-00002720: 5f57 4156 455f 4f52 5f42 4143 4b5f 5155  _WAVE_OR_BACK_QU
-00002730: 4f54 455a 0b53 4849 4654 5f4b 4559 5f31  OTEZ.SHIFT_KEY_1
-00002740: 5a0b 5348 4946 545f 4b45 595f 325a 0b53  Z.SHIFT_KEY_2Z.S
-00002750: 4849 4654 5f4b 4559 5f33 5a0b 5348 4946  HIFT_KEY_3Z.SHIF
-00002760: 545f 4b45 595f 345a 0b53 4849 4654 5f4b  T_KEY_4Z.SHIFT_K
-00002770: 4559 5f35 5a0b 5348 4946 545f 4b45 595f  EY_5Z.SHIFT_KEY_
-00002780: 365a 0b53 4849 4654 5f4b 4559 5f37 5a0b  6Z.SHIFT_KEY_7Z.
-00002790: 5348 4946 545f 4b45 595f 385a 0b53 4849  SHIFT_KEY_8Z.SHI
-000027a0: 4654 5f4b 4559 5f39 5a0b 5348 4946 545f  FT_KEY_9Z.SHIFT_
-000027b0: 4b45 595f 305a 1253 4849 4654 5f4b 4559  KEY_0Z.SHIFT_KEY
-000027c0: 5f31 315f 4d49 4e55 535a 1153 4849 4654  _11_MINUSZ.SHIFT
-000027d0: 5f4b 4559 5f31 325f 504c 5553 5a0f 5348  _KEY_12_PLUSZ.SH
-000027e0: 4946 545f 4241 434b 5350 4143 455a 0e53  IFT_BACKSPACEZ.S
-000027f0: 4849 4654 5f4e 554d 5041 445f 315a 0e53  HIFT_NUMPAD_1Z.S
-00002800: 4849 4654 5f4e 554d 5041 445f 325a 0e53  HIFT_NUMPAD_2Z.S
-00002810: 4849 4654 5f4e 554d 5041 445f 335a 0e53  HIFT_NUMPAD_3Z.S
-00002820: 4849 4654 5f4e 554d 5041 445f 345a 0e53  HIFT_NUMPAD_4Z.S
-00002830: 4849 4654 5f4e 554d 5041 445f 355a 0e53  HIFT_NUMPAD_5Z.S
-00002840: 4849 4654 5f4e 554d 5041 445f 365a 0e53  HIFT_NUMPAD_6Z.S
-00002850: 4849 4654 5f4e 554d 5041 445f 375a 0e53  HIFT_NUMPAD_7Z.S
-00002860: 4849 4654 5f4e 554d 5041 445f 385a 0e53  HIFT_NUMPAD_8Z.S
-00002870: 4849 4654 5f4e 554d 5041 445f 395a 0e53  HIFT_NUMPAD_9Z.S
-00002880: 4849 4654 5f4e 554d 5041 445f 305a 1653  HIFT_NUMPAD_0Z.S
-00002890: 4849 4654 5f4e 554d 5041 445f 3131 5f44  HIFT_NUMPAD_11_D
-000028a0: 4956 4944 455a 1853 4849 4654 5f4e 554d  IVIDEZ.SHIFT_NUM
-000028b0: 5041 445f 3132 5f4d 554c 5449 504c 595a  PAD_12_MULTIPLYZ
-000028c0: 0753 4849 4654 5f41 5a07 5348 4946 545f  .SHIFT_AZ.SHIFT_
-000028d0: 425a 0753 4849 4654 5f43 5a07 5348 4946  BZ.SHIFT_CZ.SHIF
-000028e0: 545f 445a 0753 4849 4654 5f45 5a07 5348  T_DZ.SHIFT_EZ.SH
-000028f0: 4946 545f 465a 0753 4849 4654 5f47 5a07  IFT_FZ.SHIFT_GZ.
-00002900: 5348 4946 545f 485a 0753 4849 4654 5f49  SHIFT_HZ.SHIFT_I
-00002910: 5a07 5348 4946 545f 4a5a 0753 4849 4654  Z.SHIFT_JZ.SHIFT
-00002920: 5f4b 5a07 5348 4946 545f 4c5a 0753 4849  _KZ.SHIFT_LZ.SHI
-00002930: 4654 5f4d 5a07 5348 4946 545f 4e5a 0753  FT_MZ.SHIFT_NZ.S
-00002940: 4849 4654 5f4f 5a07 5348 4946 545f 505a  HIFT_OZ.SHIFT_PZ
-00002950: 0753 4849 4654 5f51 5a07 5348 4946 545f  .SHIFT_QZ.SHIFT_
-00002960: 525a 0753 4849 4654 5f53 5a07 5348 4946  RZ.SHIFT_SZ.SHIF
-00002970: 545f 545a 0753 4849 4654 5f55 5a07 5348  T_TZ.SHIFT_UZ.SH
-00002980: 4946 545f 565a 0753 4849 4654 5f57 5a07  IFT_VZ.SHIFT_WZ.
-00002990: 5348 4946 545f 585a 0753 4849 4654 5f59  SHIFT_XZ.SHIFT_Y
-000029a0: 5a07 5348 4946 545f 5a5a 0741 4c54 5f54  Z.SHIFT_ZZ.ALT_T
-000029b0: 4142 5a06 414c 545f 4631 5a06 414c 545f  ABZ.ALT_F1Z.ALT_
-000029c0: 4632 5a06 414c 545f 4633 5a06 414c 545f  F2Z.ALT_F3Z.ALT_
-000029d0: 4634 5a06 414c 545f 4635 5a06 414c 545f  F4Z.ALT_F5Z.ALT_
-000029e0: 4636 5a06 414c 545f 4637 5a06 414c 545f  F6Z.ALT_F7Z.ALT_
-000029f0: 4638 5a06 414c 545f 4639 5a07 414c 545f  F8Z.ALT_F9Z.ALT_
-00002a00: 4631 305a 0741 4c54 5f46 3131 5a07 414c  F10Z.ALT_F11Z.AL
-00002a10: 545f 4631 325a 1b41 4c54 5f4f 454d 335f  T_F12Z.ALT_OEM3_
-00002a20: 5741 5645 5f4f 525f 4241 434b 5f51 554f  WAVE_OR_BACK_QUO
-00002a30: 5445 5a09 414c 545f 4b45 595f 315a 0941  TEZ.ALT_KEY_1Z.A
-00002a40: 4c54 5f4b 4559 5f32 5a09 414c 545f 4b45  LT_KEY_2Z.ALT_KE
-00002a50: 595f 335a 0941 4c54 5f4b 4559 5f34 5a09  Y_3Z.ALT_KEY_4Z.
-00002a60: 414c 545f 4b45 595f 355a 0941 4c54 5f4b  ALT_KEY_5Z.ALT_K
-00002a70: 4559 5f36 5a09 414c 545f 4b45 595f 375a  EY_6Z.ALT_KEY_7Z
-00002a80: 0941 4c54 5f4b 4559 5f38 5a09 414c 545f  .ALT_KEY_8Z.ALT_
-00002a90: 4b45 595f 395a 0941 4c54 5f4b 4559 5f30  KEY_9Z.ALT_KEY_0
-00002aa0: 5a10 414c 545f 4b45 595f 3131 5f4d 494e  Z.ALT_KEY_11_MIN
-00002ab0: 5553 5a0f 414c 545f 4b45 595f 3132 5f50  USZ.ALT_KEY_12_P
-00002ac0: 4c55 535a 0d41 4c54 5f42 4143 4b53 5041  LUSZ.ALT_BACKSPA
-00002ad0: 4345 5a0c 414c 545f 4e55 4d50 4144 5f31  CEZ.ALT_NUMPAD_1
-00002ae0: 5a0c 414c 545f 4e55 4d50 4144 5f32 5a0c  Z.ALT_NUMPAD_2Z.
-00002af0: 414c 545f 4e55 4d50 4144 5f33 5a0c 414c  ALT_NUMPAD_3Z.AL
-00002b00: 545f 4e55 4d50 4144 5f34 5a0c 414c 545f  T_NUMPAD_4Z.ALT_
-00002b10: 4e55 4d50 4144 5f35 5a0c 414c 545f 4e55  NUMPAD_5Z.ALT_NU
-00002b20: 4d50 4144 5f36 5a0c 414c 545f 4e55 4d50  MPAD_6Z.ALT_NUMP
-00002b30: 4144 5f37 5a0c 414c 545f 4e55 4d50 4144  AD_7Z.ALT_NUMPAD
-00002b40: 5f38 5a0c 414c 545f 4e55 4d50 4144 5f39  _8Z.ALT_NUMPAD_9
-00002b50: 5a0c 414c 545f 4e55 4d50 4144 5f30 5a14  Z.ALT_NUMPAD_0Z.
-00002b60: 414c 545f 4e55 4d50 4144 5f31 315f 4449  ALT_NUMPAD_11_DI
-00002b70: 5649 4445 5a16 414c 545f 4e55 4d50 4144  VIDEZ.ALT_NUMPAD
-00002b80: 5f31 325f 4d55 4c54 4950 4c59 5a05 414c  _12_MULTIPLYZ.AL
-00002b90: 545f 415a 0541 4c54 5f42 5a05 414c 545f  T_AZ.ALT_BZ.ALT_
-00002ba0: 435a 0541 4c54 5f44 5a05 414c 545f 455a  CZ.ALT_DZ.ALT_EZ
-00002bb0: 0541 4c54 5f46 5a05 414c 545f 475a 0541  .ALT_FZ.ALT_GZ.A
-00002bc0: 4c54 5f48 5a05 414c 545f 495a 0541 4c54  LT_HZ.ALT_IZ.ALT
-00002bd0: 5f4a 5a05 414c 545f 4b5a 0541 4c54 5f4c  _JZ.ALT_KZ.ALT_L
-00002be0: 5a05 414c 545f 4d5a 0541 4c54 5f4e 5a05  Z.ALT_MZ.ALT_NZ.
-00002bf0: 414c 545f 4f5a 0541 4c54 5f50 5a05 414c  ALT_OZ.ALT_PZ.AL
-00002c00: 545f 515a 0541 4c54 5f52 5a05 414c 545f  T_QZ.ALT_RZ.ALT_
-00002c10: 535a 0541 4c54 5f54 5a05 414c 545f 555a  SZ.ALT_TZ.ALT_UZ
-00002c20: 0541 4c54 5f56 5a05 414c 545f 575a 0541  .ALT_VZ.ALT_WZ.A
-00002c30: 4c54 5f58 5a05 414c 545f 595a 0541 4c54  LT_XZ.ALT_YZ.ALT
-00002c40: 5f5a 5a0b 4354 524c 5f41 4c54 5f46 315a  _ZZ.CTRL_ALT_F1Z
-00002c50: 0b43 5452 4c5f 414c 545f 4632 5a0b 4354  .CTRL_ALT_F2Z.CT
-00002c60: 524c 5f41 4c54 5f46 335a 0b43 5452 4c5f  RL_ALT_F3Z.CTRL_
-00002c70: 414c 545f 4634 5a0b 4354 524c 5f41 4c54  ALT_F4Z.CTRL_ALT
-00002c80: 5f46 355a 0b43 5452 4c5f 414c 545f 4636  _F5Z.CTRL_ALT_F6
-00002c90: 5a0b 4354 524c 5f41 4c54 5f46 375a 0b43  Z.CTRL_ALT_F7Z.C
-00002ca0: 5452 4c5f 414c 545f 4638 5a0b 4354 524c  TRL_ALT_F8Z.CTRL
-00002cb0: 5f41 4c54 5f46 395a 0c43 5452 4c5f 414c  _ALT_F9Z.CTRL_AL
-00002cc0: 545f 4631 305a 0c43 5452 4c5f 414c 545f  T_F10Z.CTRL_ALT_
-00002cd0: 4631 315a 0c43 5452 4c5f 414c 545f 4631  F11Z.CTRL_ALT_F1
-00002ce0: 325a 2043 5452 4c5f 414c 545f 4f45 4d33  2Z CTRL_ALT_OEM3
-00002cf0: 5f57 4156 455f 4f52 5f42 4143 4b5f 5155  _WAVE_OR_BACK_QU
-00002d00: 4f54 455a 0e43 5452 4c5f 414c 545f 4b45  OTEZ.CTRL_ALT_KE
-00002d10: 595f 315a 0e43 5452 4c5f 414c 545f 4b45  Y_1Z.CTRL_ALT_KE
-00002d20: 595f 325a 0e43 5452 4c5f 414c 545f 4b45  Y_2Z.CTRL_ALT_KE
-00002d30: 595f 335a 0e43 5452 4c5f 414c 545f 4b45  Y_3Z.CTRL_ALT_KE
-00002d40: 595f 345a 0e43 5452 4c5f 414c 545f 4b45  Y_4Z.CTRL_ALT_KE
-00002d50: 595f 355a 0e43 5452 4c5f 414c 545f 4b45  Y_5Z.CTRL_ALT_KE
-00002d60: 595f 365a 0e43 5452 4c5f 414c 545f 4b45  Y_6Z.CTRL_ALT_KE
-00002d70: 595f 375a 0e43 5452 4c5f 414c 545f 4b45  Y_7Z.CTRL_ALT_KE
-00002d80: 595f 385a 0e43 5452 4c5f 414c 545f 4b45  Y_8Z.CTRL_ALT_KE
-00002d90: 595f 395a 0e43 5452 4c5f 414c 545f 4b45  Y_9Z.CTRL_ALT_KE
-00002da0: 595f 305a 1543 5452 4c5f 414c 545f 4b45  Y_0Z.CTRL_ALT_KE
-00002db0: 595f 3131 5f4d 494e 5553 5a14 4354 524c  Y_11_MINUSZ.CTRL
-00002dc0: 5f41 4c54 5f4b 4559 5f31 325f 504c 5553  _ALT_KEY_12_PLUS
-00002dd0: 5a12 4354 524c 5f41 4c54 5f42 4143 4b53  Z.CTRL_ALT_BACKS
-00002de0: 5041 4345 5a11 4354 524c 5f41 4c54 5f4e  PACEZ.CTRL_ALT_N
-00002df0: 554d 5041 445f 315a 1143 5452 4c5f 414c  UMPAD_1Z.CTRL_AL
-00002e00: 545f 4e55 4d50 4144 5f32 5a11 4354 524c  T_NUMPAD_2Z.CTRL
-00002e10: 5f41 4c54 5f4e 554d 5041 445f 335a 1143  _ALT_NUMPAD_3Z.C
-00002e20: 5452 4c5f 414c 545f 4e55 4d50 4144 5f34  TRL_ALT_NUMPAD_4
-00002e30: 5a11 4354 524c 5f41 4c54 5f4e 554d 5041  Z.CTRL_ALT_NUMPA
-00002e40: 445f 355a 1143 5452 4c5f 414c 545f 4e55  D_5Z.CTRL_ALT_NU
-00002e50: 4d50 4144 5f36 5a11 4354 524c 5f41 4c54  MPAD_6Z.CTRL_ALT
-00002e60: 5f4e 554d 5041 445f 375a 1143 5452 4c5f  _NUMPAD_7Z.CTRL_
-00002e70: 414c 545f 4e55 4d50 4144 5f38 5a11 4354  ALT_NUMPAD_8Z.CT
-00002e80: 524c 5f41 4c54 5f4e 554d 5041 445f 395a  RL_ALT_NUMPAD_9Z
-00002e90: 1143 5452 4c5f 414c 545f 4e55 4d50 4144  .CTRL_ALT_NUMPAD
-00002ea0: 5f30 5a19 4354 524c 5f41 4c54 5f4e 554d  _0Z.CTRL_ALT_NUM
-00002eb0: 5041 445f 3131 5f44 4956 4944 455a 1b43  PAD_11_DIVIDEZ.C
-00002ec0: 5452 4c5f 414c 545f 4e55 4d50 4144 5f31  TRL_ALT_NUMPAD_1
-00002ed0: 325f 4d55 4c54 4950 4c59 5a0a 4354 524c  2_MULTIPLYZ.CTRL
-00002ee0: 5f41 4c54 5f41 5a0a 4354 524c 5f41 4c54  _ALT_AZ.CTRL_ALT
-00002ef0: 5f42 5a0a 4354 524c 5f41 4c54 5f43 5a0a  _BZ.CTRL_ALT_CZ.
-00002f00: 4354 524c 5f41 4c54 5f44 5a0a 4354 524c  CTRL_ALT_DZ.CTRL
-00002f10: 5f41 4c54 5f45 5a0a 4354 524c 5f41 4c54  _ALT_EZ.CTRL_ALT
-00002f20: 5f46 5a0a 4354 524c 5f41 4c54 5f47 5a0a  _FZ.CTRL_ALT_GZ.
-00002f30: 4354 524c 5f41 4c54 5f48 5a0a 4354 524c  CTRL_ALT_HZ.CTRL
-00002f40: 5f41 4c54 5f49 5a0a 4354 524c 5f41 4c54  _ALT_IZ.CTRL_ALT
-00002f50: 5f4a 5a0a 4354 524c 5f41 4c54 5f4b 5a0a  _JZ.CTRL_ALT_KZ.
-00002f60: 4354 524c 5f41 4c54 5f4c 5a0a 4354 524c  CTRL_ALT_LZ.CTRL
-00002f70: 5f41 4c54 5f4d 5a0a 4354 524c 5f41 4c54  _ALT_MZ.CTRL_ALT
-00002f80: 5f4e 5a0a 4354 524c 5f41 4c54 5f4f 5a0a  _NZ.CTRL_ALT_OZ.
-00002f90: 4354 524c 5f41 4c54 5f50 5a0a 4354 524c  CTRL_ALT_PZ.CTRL
-00002fa0: 5f41 4c54 5f51 5a0a 4354 524c 5f41 4c54  _ALT_QZ.CTRL_ALT
-00002fb0: 5f52 5a0a 4354 524c 5f41 4c54 5f53 5a0a  _RZ.CTRL_ALT_SZ.
-00002fc0: 4354 524c 5f41 4c54 5f54 5a0a 4354 524c  CTRL_ALT_TZ.CTRL
-00002fd0: 5f41 4c54 5f55 5a0a 4354 524c 5f41 4c54  _ALT_UZ.CTRL_ALT
-00002fe0: 5f56 5a0a 4354 524c 5f41 4c54 5f57 5a0a  _VZ.CTRL_ALT_WZ.
-00002ff0: 4354 524c 5f41 4c54 5f58 5a0a 4354 524c  CTRL_ALT_XZ.CTRL
-00003000: 5f41 4c54 5f59 5a0a 4354 524c 5f41 4c54  _ALT_YZ.CTRL_ALT
-00003010: 5f5a 5a0d 4354 524c 5f53 4849 4654 5f46  _ZZ.CTRL_SHIFT_F
-00003020: 315a 0d43 5452 4c5f 5348 4946 545f 4632  1Z.CTRL_SHIFT_F2
-00003030: 5a0d 4354 524c 5f53 4849 4654 5f46 335a  Z.CTRL_SHIFT_F3Z
-00003040: 0d43 5452 4c5f 5348 4946 545f 4634 5a0d  .CTRL_SHIFT_F4Z.
-00003050: 4354 524c 5f53 4849 4654 5f46 355a 0d43  CTRL_SHIFT_F5Z.C
-00003060: 5452 4c5f 5348 4946 545f 4636 5a0d 4354  TRL_SHIFT_F6Z.CT
-00003070: 524c 5f53 4849 4654 5f46 375a 0d43 5452  RL_SHIFT_F7Z.CTR
-00003080: 4c5f 5348 4946 545f 4638 5a0d 4354 524c  L_SHIFT_F8Z.CTRL
-00003090: 5f53 4849 4654 5f46 395a 0e43 5452 4c5f  _SHIFT_F9Z.CTRL_
-000030a0: 5348 4946 545f 4631 305a 0e43 5452 4c5f  SHIFT_F10Z.CTRL_
-000030b0: 5348 4946 545f 4631 315a 0e43 5452 4c5f  SHIFT_F11Z.CTRL_
-000030c0: 5348 4946 545f 4631 325a 2243 5452 4c5f  SHIFT_F12Z"CTRL_
-000030d0: 5348 4946 545f 4f45 4d33 5f57 4156 455f  SHIFT_OEM3_WAVE_
-000030e0: 4f52 5f42 4143 4b5f 5155 4f54 455a 1043  OR_BACK_QUOTEZ.C
-000030f0: 5452 4c5f 5348 4946 545f 4b45 595f 315a  TRL_SHIFT_KEY_1Z
-00003100: 1043 5452 4c5f 5348 4946 545f 4b45 595f  .CTRL_SHIFT_KEY_
-00003110: 325a 1043 5452 4c5f 5348 4946 545f 4b45  2Z.CTRL_SHIFT_KE
-00003120: 595f 335a 1043 5452 4c5f 5348 4946 545f  Y_3Z.CTRL_SHIFT_
-00003130: 4b45 595f 345a 1043 5452 4c5f 5348 4946  KEY_4Z.CTRL_SHIF
-00003140: 545f 4b45 595f 355a 1043 5452 4c5f 5348  T_KEY_5Z.CTRL_SH
-00003150: 4946 545f 4b45 595f 365a 1043 5452 4c5f  IFT_KEY_6Z.CTRL_
-00003160: 5348 4946 545f 4b45 595f 375a 1043 5452  SHIFT_KEY_7Z.CTR
-00003170: 4c5f 5348 4946 545f 4b45 595f 385a 1043  L_SHIFT_KEY_8Z.C
-00003180: 5452 4c5f 5348 4946 545f 4b45 595f 395a  TRL_SHIFT_KEY_9Z
-00003190: 1043 5452 4c5f 5348 4946 545f 4b45 595f  .CTRL_SHIFT_KEY_
-000031a0: 305a 1743 5452 4c5f 5348 4946 545f 4b45  0Z.CTRL_SHIFT_KE
-000031b0: 595f 3131 5f4d 494e 5553 5a16 4354 524c  Y_11_MINUSZ.CTRL
-000031c0: 5f53 4849 4654 5f4b 4559 5f31 325f 504c  _SHIFT_KEY_12_PL
-000031d0: 5553 5a14 4354 524c 5f53 4849 4654 5f42  USZ.CTRL_SHIFT_B
-000031e0: 4143 4b53 5041 4345 5a13 4354 524c 5f53  ACKSPACEZ.CTRL_S
-000031f0: 4849 4654 5f4e 554d 5041 445f 315a 1343  HIFT_NUMPAD_1Z.C
-00003200: 5452 4c5f 5348 4946 545f 4e55 4d50 4144  TRL_SHIFT_NUMPAD
-00003210: 5f32 5a13 4354 524c 5f53 4849 4654 5f4e  _2Z.CTRL_SHIFT_N
-00003220: 554d 5041 445f 335a 1343 5452 4c5f 5348  UMPAD_3Z.CTRL_SH
-00003230: 4946 545f 4e55 4d50 4144 5f34 5a13 4354  IFT_NUMPAD_4Z.CT
-00003240: 524c 5f53 4849 4654 5f4e 554d 5041 445f  RL_SHIFT_NUMPAD_
-00003250: 355a 1343 5452 4c5f 5348 4946 545f 4e55  5Z.CTRL_SHIFT_NU
-00003260: 4d50 4144 5f36 5a13 4354 524c 5f53 4849  MPAD_6Z.CTRL_SHI
-00003270: 4654 5f4e 554d 5041 445f 375a 1343 5452  FT_NUMPAD_7Z.CTR
-00003280: 4c5f 5348 4946 545f 4e55 4d50 4144 5f38  L_SHIFT_NUMPAD_8
-00003290: 5a13 4354 524c 5f53 4849 4654 5f4e 554d  Z.CTRL_SHIFT_NUM
-000032a0: 5041 445f 395a 1343 5452 4c5f 5348 4946  PAD_9Z.CTRL_SHIF
-000032b0: 545f 4e55 4d50 4144 5f30 5a1b 4354 524c  T_NUMPAD_0Z.CTRL
-000032c0: 5f53 4849 4654 5f4e 554d 5041 445f 3131  _SHIFT_NUMPAD_11
-000032d0: 5f44 4956 4944 455a 1d43 5452 4c5f 5348  _DIVIDEZ.CTRL_SH
-000032e0: 4946 545f 4e55 4d50 4144 5f31 325f 4d55  IFT_NUMPAD_12_MU
-000032f0: 4c54 4950 4c59 5a0c 4354 524c 5f53 4849  LTIPLYZ.CTRL_SHI
-00003300: 4654 5f41 5a0c 4354 524c 5f53 4849 4654  FT_AZ.CTRL_SHIFT
-00003310: 5f42 5a0c 4354 524c 5f53 4849 4654 5f43  _BZ.CTRL_SHIFT_C
-00003320: 5a0c 4354 524c 5f53 4849 4654 5f44 5a0c  Z.CTRL_SHIFT_DZ.
-00003330: 4354 524c 5f53 4849 4654 5f45 5a0c 4354  CTRL_SHIFT_EZ.CT
-00003340: 524c 5f53 4849 4654 5f46 5a0c 4354 524c  RL_SHIFT_FZ.CTRL
-00003350: 5f53 4849 4654 5f47 5a0c 4354 524c 5f53  _SHIFT_GZ.CTRL_S
-00003360: 4849 4654 5f48 5a0c 4354 524c 5f53 4849  HIFT_HZ.CTRL_SHI
-00003370: 4654 5f49 5a0c 4354 524c 5f53 4849 4654  FT_IZ.CTRL_SHIFT
-00003380: 5f4a 5a0c 4354 524c 5f53 4849 4654 5f4b  _JZ.CTRL_SHIFT_K
-00003390: 5a0c 4354 524c 5f53 4849 4654 5f4c 5a0c  Z.CTRL_SHIFT_LZ.
-000033a0: 4354 524c 5f53 4849 4654 5f4d 5a0c 4354  CTRL_SHIFT_MZ.CT
-000033b0: 524c 5f53 4849 4654 5f4e 5a0c 4354 524c  RL_SHIFT_NZ.CTRL
-000033c0: 5f53 4849 4654 5f4f 5a0c 4354 524c 5f53  _SHIFT_OZ.CTRL_S
-000033d0: 4849 4654 5f50 5a0c 4354 524c 5f53 4849  HIFT_PZ.CTRL_SHI
-000033e0: 4654 5f51 5a0c 4354 524c 5f53 4849 4654  FT_QZ.CTRL_SHIFT
-000033f0: 5f52 5a0c 4354 524c 5f53 4849 4654 5f53  _RZ.CTRL_SHIFT_S
-00003400: 5a0c 4354 524c 5f53 4849 4654 5f54 5a0c  Z.CTRL_SHIFT_TZ.
-00003410: 4354 524c 5f53 4849 4654 5f55 5a0c 4354  CTRL_SHIFT_UZ.CT
-00003420: 524c 5f53 4849 4654 5f56 5a0c 4354 524c  RL_SHIFT_VZ.CTRL
-00003430: 5f53 4849 4654 5f57 5a0c 4354 524c 5f53  _SHIFT_WZ.CTRL_S
-00003440: 4849 4654 5f58 5a0c 4354 524c 5f53 4849  HIFT_XZ.CTRL_SHI
-00003450: 4654 5f59 5a0c 4354 524c 5f53 4849 4654  FT_YZ.CTRL_SHIFT
-00003460: 5f5a 5a0c 414c 545f 5348 4946 545f 4631  _ZZ.ALT_SHIFT_F1
-00003470: 5a0c 414c 545f 5348 4946 545f 4632 5a0c  Z.ALT_SHIFT_F2Z.
-00003480: 414c 545f 5348 4946 545f 4633 5a0c 414c  ALT_SHIFT_F3Z.AL
-00003490: 545f 5348 4946 545f 4634 5a0c 414c 545f  T_SHIFT_F4Z.ALT_
-000034a0: 5348 4946 545f 4635 5a0c 414c 545f 5348  SHIFT_F5Z.ALT_SH
-000034b0: 4946 545f 4636 5a0c 414c 545f 5348 4946  IFT_F6Z.ALT_SHIF
-000034c0: 545f 4637 5a0c 414c 545f 5348 4946 545f  T_F7Z.ALT_SHIFT_
-000034d0: 4638 5a0c 414c 545f 5348 4946 545f 4639  F8Z.ALT_SHIFT_F9
-000034e0: 5a0d 414c 545f 5348 4946 545f 4631 305a  Z.ALT_SHIFT_F10Z
-000034f0: 0d41 4c54 5f53 4849 4654 5f46 3131 5a0d  .ALT_SHIFT_F11Z.
-00003500: 414c 545f 5348 4946 545f 4631 325a 2141  ALT_SHIFT_F12Z!A
-00003510: 4c54 5f53 4849 4654 5f4f 454d 335f 5741  LT_SHIFT_OEM3_WA
-00003520: 5645 5f4f 525f 4241 434b 5f51 554f 5445  VE_OR_BACK_QUOTE
-00003530: 5a0f 414c 545f 5348 4946 545f 4b45 595f  Z.ALT_SHIFT_KEY_
-00003540: 315a 0f41 4c54 5f53 4849 4654 5f4b 4559  1Z.ALT_SHIFT_KEY
-00003550: 5f32 5a0f 414c 545f 5348 4946 545f 4b45  _2Z.ALT_SHIFT_KE
-00003560: 595f 335a 0f41 4c54 5f53 4849 4654 5f4b  Y_3Z.ALT_SHIFT_K
-00003570: 4559 5f34 5a0f 414c 545f 5348 4946 545f  EY_4Z.ALT_SHIFT_
-00003580: 4b45 595f 355a 0f41 4c54 5f53 4849 4654  KEY_5Z.ALT_SHIFT
-00003590: 5f4b 4559 5f36 5a0f 414c 545f 5348 4946  _KEY_6Z.ALT_SHIF
-000035a0: 545f 4b45 595f 375a 0f41 4c54 5f53 4849  T_KEY_7Z.ALT_SHI
-000035b0: 4654 5f4b 4559 5f38 5a0f 414c 545f 5348  FT_KEY_8Z.ALT_SH
-000035c0: 4946 545f 4b45 595f 395a 0f41 4c54 5f53  IFT_KEY_9Z.ALT_S
-000035d0: 4849 4654 5f4b 4559 5f30 5a16 414c 545f  HIFT_KEY_0Z.ALT_
-000035e0: 5348 4946 545f 4b45 595f 3131 5f4d 494e  SHIFT_KEY_11_MIN
-000035f0: 5553 5a15 414c 545f 5348 4946 545f 4b45  USZ.ALT_SHIFT_KE
-00003600: 595f 3132 5f50 4c55 535a 1341 4c54 5f53  Y_12_PLUSZ.ALT_S
-00003610: 4849 4654 5f42 4143 4b53 5041 4345 5a12  HIFT_BACKSPACEZ.
-00003620: 414c 545f 5348 4946 545f 4e55 4d50 4144  ALT_SHIFT_NUMPAD
-00003630: 5f31 5a12 414c 545f 5348 4946 545f 4e55  _1Z.ALT_SHIFT_NU
-00003640: 4d50 4144 5f32 5a12 414c 545f 5348 4946  MPAD_2Z.ALT_SHIF
-00003650: 545f 4e55 4d50 4144 5f33 5a12 414c 545f  T_NUMPAD_3Z.ALT_
-00003660: 5348 4946 545f 4e55 4d50 4144 5f34 5a12  SHIFT_NUMPAD_4Z.
-00003670: 414c 545f 5348 4946 545f 4e55 4d50 4144  ALT_SHIFT_NUMPAD
-00003680: 5f35 5a12 414c 545f 5348 4946 545f 4e55  _5Z.ALT_SHIFT_NU
-00003690: 4d50 4144 5f36 5a12 414c 545f 5348 4946  MPAD_6Z.ALT_SHIF
-000036a0: 545f 4e55 4d50 4144 5f37 5a12 414c 545f  T_NUMPAD_7Z.ALT_
-000036b0: 5348 4946 545f 4e55 4d50 4144 5f38 5a12  SHIFT_NUMPAD_8Z.
-000036c0: 414c 545f 5348 4946 545f 4e55 4d50 4144  ALT_SHIFT_NUMPAD
-000036d0: 5f39 5a12 414c 545f 5348 4946 545f 4e55  _9Z.ALT_SHIFT_NU
-000036e0: 4d50 4144 5f30 5a1a 414c 545f 5348 4946  MPAD_0Z.ALT_SHIF
-000036f0: 545f 4e55 4d50 4144 5f31 315f 4449 5649  T_NUMPAD_11_DIVI
-00003700: 4445 5a1c 414c 545f 5348 4946 545f 4e55  DEZ.ALT_SHIFT_NU
-00003710: 4d50 4144 5f31 325f 4d55 4c54 4950 4c59  MPAD_12_MULTIPLY
-00003720: 5a0b 414c 545f 5348 4946 545f 415a 0b41  Z.ALT_SHIFT_AZ.A
-00003730: 4c54 5f53 4849 4654 5f42 5a0b 414c 545f  LT_SHIFT_BZ.ALT_
-00003740: 5348 4946 545f 435a 0b41 4c54 5f53 4849  SHIFT_CZ.ALT_SHI
-00003750: 4654 5f44 5a0b 414c 545f 5348 4946 545f  FT_DZ.ALT_SHIFT_
-00003760: 455a 0b41 4c54 5f53 4849 4654 5f46 5a0b  EZ.ALT_SHIFT_FZ.
-00003770: 414c 545f 5348 4946 545f 475a 0b41 4c54  ALT_SHIFT_GZ.ALT
-00003780: 5f53 4849 4654 5f48 5a0b 414c 545f 5348  _SHIFT_HZ.ALT_SH
-00003790: 4946 545f 495a 0b41 4c54 5f53 4849 4654  IFT_IZ.ALT_SHIFT
-000037a0: 5f4a 5a0b 414c 545f 5348 4946 545f 4b5a  _JZ.ALT_SHIFT_KZ
-000037b0: 0b41 4c54 5f53 4849 4654 5f4c 5a0b 414c  .ALT_SHIFT_LZ.AL
-000037c0: 545f 5348 4946 545f 4d5a 0b41 4c54 5f53  T_SHIFT_MZ.ALT_S
-000037d0: 4849 4654 5f4e 5a0b 414c 545f 5348 4946  HIFT_NZ.ALT_SHIF
-000037e0: 545f 4f5a 0b41 4c54 5f53 4849 4654 5f50  T_OZ.ALT_SHIFT_P
-000037f0: 5a0b 414c 545f 5348 4946 545f 515a 0b41  Z.ALT_SHIFT_QZ.A
-00003800: 4c54 5f53 4849 4654 5f52 5a0b 414c 545f  LT_SHIFT_RZ.ALT_
-00003810: 5348 4946 545f 535a 0b41 4c54 5f53 4849  SHIFT_SZ.ALT_SHI
-00003820: 4654 5f54 5a0b 414c 545f 5348 4946 545f  FT_TZ.ALT_SHIFT_
-00003830: 555a 0b41 4c54 5f53 4849 4654 5f56 5a0b  UZ.ALT_SHIFT_VZ.
-00003840: 414c 545f 5348 4946 545f 575a 0b41 4c54  ALT_SHIFT_WZ.ALT
-00003850: 5f53 4849 4654 5f58 5a0b 414c 545f 5348  _SHIFT_XZ.ALT_SH
-00003860: 4946 545f 595a 0b41 4c54 5f53 4849 4654  IFT_YZ.ALT_SHIFT
-00003870: 5f5a 5a11 4354 524c 5f53 4849 4654 5f41  _ZZ.CTRL_SHIFT_A
-00003880: 4c54 5f46 315a 1143 5452 4c5f 5348 4946  LT_F1Z.CTRL_SHIF
-00003890: 545f 414c 545f 4632 5a11 4354 524c 5f53  T_ALT_F2Z.CTRL_S
-000038a0: 4849 4654 5f41 4c54 5f46 335a 1143 5452  HIFT_ALT_F3Z.CTR
-000038b0: 4c5f 5348 4946 545f 414c 545f 4634 5a11  L_SHIFT_ALT_F4Z.
-000038c0: 4354 524c 5f53 4849 4654 5f41 4c54 5f46  CTRL_SHIFT_ALT_F
-000038d0: 355a 1143 5452 4c5f 5348 4946 545f 414c  5Z.CTRL_SHIFT_AL
-000038e0: 545f 4636 5a11 4354 524c 5f53 4849 4654  T_F6Z.CTRL_SHIFT
-000038f0: 5f41 4c54 5f46 375a 1143 5452 4c5f 5348  _ALT_F7Z.CTRL_SH
-00003900: 4946 545f 414c 545f 4638 5a11 4354 524c  IFT_ALT_F8Z.CTRL
-00003910: 5f53 4849 4654 5f41 4c54 5f46 395a 1243  _SHIFT_ALT_F9Z.C
-00003920: 5452 4c5f 5348 4946 545f 414c 545f 4631  TRL_SHIFT_ALT_F1
-00003930: 305a 1243 5452 4c5f 5348 4946 545f 414c  0Z.CTRL_SHIFT_AL
-00003940: 545f 4631 315a 1243 5452 4c5f 5348 4946  T_F11Z.CTRL_SHIF
-00003950: 545f 414c 545f 4631 325a 2643 5452 4c5f  T_ALT_F12Z&CTRL_
-00003960: 5348 4946 545f 414c 545f 4f45 4d33 5f57  SHIFT_ALT_OEM3_W
-00003970: 4156 455f 4f52 5f42 4143 4b5f 5155 4f54  AVE_OR_BACK_QUOT
-00003980: 455a 1443 5452 4c5f 5348 4946 545f 414c  EZ.CTRL_SHIFT_AL
-00003990: 545f 4b45 595f 315a 1443 5452 4c5f 5348  T_KEY_1Z.CTRL_SH
-000039a0: 4946 545f 414c 545f 4b45 595f 325a 1443  IFT_ALT_KEY_2Z.C
-000039b0: 5452 4c5f 5348 4946 545f 414c 545f 4b45  TRL_SHIFT_ALT_KE
-000039c0: 595f 335a 1443 5452 4c5f 5348 4946 545f  Y_3Z.CTRL_SHIFT_
-000039d0: 414c 545f 4b45 595f 345a 1443 5452 4c5f  ALT_KEY_4Z.CTRL_
-000039e0: 5348 4946 545f 414c 545f 4b45 595f 355a  SHIFT_ALT_KEY_5Z
-000039f0: 1443 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-00003a00: 4b45 595f 365a 1443 5452 4c5f 5348 4946  KEY_6Z.CTRL_SHIF
-00003a10: 545f 414c 545f 4b45 595f 375a 1443 5452  T_ALT_KEY_7Z.CTR
-00003a20: 4c5f 5348 4946 545f 414c 545f 4b45 595f  L_SHIFT_ALT_KEY_
-00003a30: 385a 1443 5452 4c5f 5348 4946 545f 414c  8Z.CTRL_SHIFT_AL
-00003a40: 545f 4b45 595f 395a 1443 5452 4c5f 5348  T_KEY_9Z.CTRL_SH
-00003a50: 4946 545f 414c 545f 4b45 595f 305a 1b43  IFT_ALT_KEY_0Z.C
-00003a60: 5452 4c5f 5348 4946 545f 414c 545f 4b45  TRL_SHIFT_ALT_KE
-00003a70: 595f 3131 5f4d 494e 5553 5a1a 4354 524c  Y_11_MINUSZ.CTRL
-00003a80: 5f53 4849 4654 5f41 4c54 5f4b 4559 5f31  _SHIFT_ALT_KEY_1
-00003a90: 325f 504c 5553 5a18 4354 524c 5f53 4849  2_PLUSZ.CTRL_SHI
-00003aa0: 4654 5f41 4c54 5f42 4143 4b53 5041 4345  FT_ALT_BACKSPACE
-00003ab0: 5a17 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
-00003ac0: 5f4e 554d 5041 445f 315a 1743 5452 4c5f  _NUMPAD_1Z.CTRL_
-00003ad0: 5348 4946 545f 414c 545f 4e55 4d50 4144  SHIFT_ALT_NUMPAD
-00003ae0: 5f32 5a17 4354 524c 5f53 4849 4654 5f41  _2Z.CTRL_SHIFT_A
-00003af0: 4c54 5f4e 554d 5041 445f 335a 1743 5452  LT_NUMPAD_3Z.CTR
-00003b00: 4c5f 5348 4946 545f 414c 545f 4e55 4d50  L_SHIFT_ALT_NUMP
-00003b10: 4144 5f34 5a17 4354 524c 5f53 4849 4654  AD_4Z.CTRL_SHIFT
-00003b20: 5f41 4c54 5f4e 554d 5041 445f 355a 1743  _ALT_NUMPAD_5Z.C
-00003b30: 5452 4c5f 5348 4946 545f 414c 545f 4e55  TRL_SHIFT_ALT_NU
-00003b40: 4d50 4144 5f36 5a17 4354 524c 5f53 4849  MPAD_6Z.CTRL_SHI
-00003b50: 4654 5f41 4c54 5f4e 554d 5041 445f 375a  FT_ALT_NUMPAD_7Z
-00003b60: 1743 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
-00003b70: 4e55 4d50 4144 5f38 5a17 4354 524c 5f53  NUMPAD_8Z.CTRL_S
-00003b80: 4849 4654 5f41 4c54 5f4e 554d 5041 445f  HIFT_ALT_NUMPAD_
-00003b90: 395a 1743 5452 4c5f 5348 4946 545f 414c  9Z.CTRL_SHIFT_AL
-00003ba0: 545f 4e55 4d50 4144 5f30 5a1f 4354 524c  T_NUMPAD_0Z.CTRL
-00003bb0: 5f53 4849 4654 5f41 4c54 5f4e 554d 5041  _SHIFT_ALT_NUMPA
-00003bc0: 445f 3131 5f44 4956 4944 455a 2143 5452  D_11_DIVIDEZ!CTR
-00003bd0: 4c5f 5348 4946 545f 414c 545f 4e55 4d50  L_SHIFT_ALT_NUMP
-00003be0: 4144 5f31 325f 4d55 4c54 4950 4c59 5a10  AD_12_MULTIPLYZ.
-00003bf0: 4354 524c 5f53 4849 4654 5f41 4c54 5f41  CTRL_SHIFT_ALT_A
-00003c00: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
-00003c10: 5f42 5a10 4354 524c 5f53 4849 4654 5f41  _BZ.CTRL_SHIFT_A
-00003c20: 4c54 5f43 5a10 4354 524c 5f53 4849 4654  LT_CZ.CTRL_SHIFT
-00003c30: 5f41 4c54 5f44 5a10 4354 524c 5f53 4849  _ALT_DZ.CTRL_SHI
-00003c40: 4654 5f41 4c54 5f45 5a10 4354 524c 5f53  FT_ALT_EZ.CTRL_S
-00003c50: 4849 4654 5f41 4c54 5f46 5a10 4354 524c  HIFT_ALT_FZ.CTRL
-00003c60: 5f53 4849 4654 5f41 4c54 5f47 5a10 4354  _SHIFT_ALT_GZ.CT
-00003c70: 524c 5f53 4849 4654 5f41 4c54 5f48 5a10  RL_SHIFT_ALT_HZ.
-00003c80: 4354 524c 5f53 4849 4654 5f41 4c54 5f49  CTRL_SHIFT_ALT_I
-00003c90: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
-00003ca0: 5f4a 5a10 4354 524c 5f53 4849 4654 5f41  _JZ.CTRL_SHIFT_A
-00003cb0: 4c54 5f4b 5a10 4354 524c 5f53 4849 4654  LT_KZ.CTRL_SHIFT
-00003cc0: 5f41 4c54 5f4c 5a10 4354 524c 5f53 4849  _ALT_LZ.CTRL_SHI
-00003cd0: 4654 5f41 4c54 5f4d 5a10 4354 524c 5f53  FT_ALT_MZ.CTRL_S
-00003ce0: 4849 4654 5f41 4c54 5f4e 5a10 4354 524c  HIFT_ALT_NZ.CTRL
-00003cf0: 5f53 4849 4654 5f41 4c54 5f4f 5a10 4354  _SHIFT_ALT_OZ.CT
-00003d00: 524c 5f53 4849 4654 5f41 4c54 5f50 5a10  RL_SHIFT_ALT_PZ.
-00003d10: 4354 524c 5f53 4849 4654 5f41 4c54 5f51  CTRL_SHIFT_ALT_Q
-00003d20: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
-00003d30: 5f52 5a10 4354 524c 5f53 4849 4654 5f41  _RZ.CTRL_SHIFT_A
-00003d40: 4c54 5f53 5a10 4354 524c 5f53 4849 4654  LT_SZ.CTRL_SHIFT
-00003d50: 5f41 4c54 5f54 5a10 4354 524c 5f53 4849  _ALT_TZ.CTRL_SHI
-00003d60: 4654 5f41 4c54 5f55 5a10 4354 524c 5f53  FT_ALT_UZ.CTRL_S
-00003d70: 4849 4654 5f41 4c54 5f56 5a10 4354 524c  HIFT_ALT_VZ.CTRL
-00003d80: 5f53 4849 4654 5f41 4c54 5f57 5a10 4354  _SHIFT_ALT_WZ.CT
-00003d90: 524c 5f53 4849 4654 5f41 4c54 5f58 5a10  RL_SHIFT_ALT_XZ.
-00003da0: 4354 524c 5f53 4849 4654 5f41 4c54 5f59  CTRL_SHIFT_ALT_Y
-00003db0: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
-00003dc0: 5f5a 7240 0000 0072 4000 0000 7240 0000  _Zr@...r@...r@..
-00003dd0: 0072 4100 0000 da08 3c6d 6f64 756c 653e  .rA.....<module>
-00003de0: 0300 0000 73e6 0400 0004 1104 0104 0504  ....s...........
-00003df0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00003e00: 0104 0104 0104 0504 0104 0104 0104 0104  ................
-00003e10: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00003e20: 0104 0504 0104 0104 0104 0104 0204 0104  ................
-00003e30: 0104 0104 0104 0104 0204 0204 0104 0504  ................
-00003e40: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00003e50: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00003e60: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00003e70: 0104 0504 0104 0104 0104 0104 0104 0104  ................
-00003e80: 0104 0104 0504 0104 0104 0104 0104 0104  ................
-00003e90: 0204 0104 0104 0104 0504 0204 0104 0104  ................
-00003ea0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00003eb0: 0104 0204 0104 0104 0104 0204 0104 0104  ................
-00003ec0: 0104 0104 0104 0104 0104 0104 0204 0504  ................
-00003ed0: 0104 0104 0104 0104 0602 0102 0102 0102  ................
-00003ee0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00003ef0: f404 1002 0102 0102 0102 0102 0102 fa04  ................
-00003f00: 0a02 0102 0102 0102 0102 0102 0102 0102  ................
-00003f10: 0102 0102 0102 0102 f404 1002 0102 0102  ................
-00003f20: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00003f30: 0102 f404 1310 0410 0410 0710 0410 0410  ................
-00003f40: 0710 0710 0410 0410 0710 0b08 0208 0108  ................
-00003f50: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003f60: 0108 0108 0208 0108 0108 0108 0108 0108  ................
-00003f70: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003f80: 0208 0108 0108 0108 0108 0108 0108 0108  ................
-00003f90: 0108 0108 0108 0108 0208 0108 0108 0108  ................
-00003fa0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003fb0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003fc0: 0108 0108 0108 0108 0108 0108 0308 0208  ................
-00003fd0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003fe0: 0108 0108 0108 0208 0108 0108 0108 0108  ................
-00003ff0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00004000: 0108 0208 0108 0108 0108 0108 0108 0108  ................
-00004010: 0108 0108 0108 0108 0108 0208 0108 0108  ................
-00004020: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00004030: 0108 0108 0108 0108 0108 010a 010a 010a  ................
-00004040: 010a 010a 010a 010a 010a 010a 010a 030a  ................
-00004050: 020a 010a 010a 010a 010a 010a 010a 010a  ................
-00004060: 010a 010a 010a 010a 020a 010a 010a 010a  ................
+00002440: 5f42 4143 4b5f 5155 4f54 455a 0643 5452  _BACK_QUOTEZ.CTR
+00002450: 4c5f 315a 0643 5452 4c5f 325a 0643 5452  L_1Z.CTRL_2Z.CTR
+00002460: 4c5f 335a 0643 5452 4c5f 345a 0643 5452  L_3Z.CTRL_4Z.CTR
+00002470: 4c5f 355a 0643 5452 4c5f 365a 0643 5452  L_5Z.CTRL_6Z.CTR
+00002480: 4c5f 375a 0643 5452 4c5f 385a 0643 5452  L_7Z.CTRL_8Z.CTR
+00002490: 4c5f 395a 0643 5452 4c5f 305a 0d43 5452  L_9Z.CTRL_0Z.CTR
+000024a0: 4c5f 3131 5f4d 494e 5553 5a0c 4354 524c  L_11_MINUSZ.CTRL
+000024b0: 5f31 325f 504c 5553 5a0e 4354 524c 5f42  _12_PLUSZ.CTRL_B
+000024c0: 4143 4b53 5041 4345 5a0d 4354 524c 5f4e  ACKSPACEZ.CTRL_N
+000024d0: 554d 5041 445f 315a 0d43 5452 4c5f 4e55  UMPAD_1Z.CTRL_NU
+000024e0: 4d50 4144 5f32 5a0d 4354 524c 5f4e 554d  MPAD_2Z.CTRL_NUM
+000024f0: 5041 445f 335a 0d43 5452 4c5f 4e55 4d50  PAD_3Z.CTRL_NUMP
+00002500: 4144 5f34 5a0d 4354 524c 5f4e 554d 5041  AD_4Z.CTRL_NUMPA
+00002510: 445f 355a 0d43 5452 4c5f 4e55 4d50 4144  D_5Z.CTRL_NUMPAD
+00002520: 5f36 5a0d 4354 524c 5f4e 554d 5041 445f  _6Z.CTRL_NUMPAD_
+00002530: 375a 0d43 5452 4c5f 4e55 4d50 4144 5f38  7Z.CTRL_NUMPAD_8
+00002540: 5a0d 4354 524c 5f4e 554d 5041 445f 395a  Z.CTRL_NUMPAD_9Z
+00002550: 0d43 5452 4c5f 4e55 4d50 4144 5f30 5a15  .CTRL_NUMPAD_0Z.
+00002560: 4354 524c 5f4e 554d 5041 445f 3131 5f44  CTRL_NUMPAD_11_D
+00002570: 4956 4944 455a 1743 5452 4c5f 4e55 4d50  IVIDEZ.CTRL_NUMP
+00002580: 4144 5f31 325f 4d55 4c54 4950 4c59 5a06  AD_12_MULTIPLYZ.
+00002590: 4354 524c 5f41 5a06 4354 524c 5f42 5a06  CTRL_AZ.CTRL_BZ.
+000025a0: 4354 524c 5f43 5a06 4354 524c 5f44 5a06  CTRL_CZ.CTRL_DZ.
+000025b0: 4354 524c 5f45 5a06 4354 524c 5f46 5a06  CTRL_EZ.CTRL_FZ.
+000025c0: 4354 524c 5f47 5a06 4354 524c 5f48 5a06  CTRL_GZ.CTRL_HZ.
+000025d0: 4354 524c 5f49 5a06 4354 524c 5f4a 5a06  CTRL_IZ.CTRL_JZ.
+000025e0: 4354 524c 5f4b 5a06 4354 524c 5f4c 5a06  CTRL_KZ.CTRL_LZ.
+000025f0: 4354 524c 5f4d 5a06 4354 524c 5f4e 5a06  CTRL_MZ.CTRL_NZ.
+00002600: 4354 524c 5f4f 5a06 4354 524c 5f50 5a06  CTRL_OZ.CTRL_PZ.
+00002610: 4354 524c 5f51 5a06 4354 524c 5f52 5a06  CTRL_QZ.CTRL_RZ.
+00002620: 4354 524c 5f53 5a06 4354 524c 5f54 5a06  CTRL_SZ.CTRL_TZ.
+00002630: 4354 524c 5f55 5a06 4354 524c 5f56 5a06  CTRL_UZ.CTRL_VZ.
+00002640: 4354 524c 5f57 5a06 4354 524c 5f58 5a06  CTRL_WZ.CTRL_XZ.
+00002650: 4354 524c 5f59 5a06 4354 524c 5f5a 5a09  CTRL_YZ.CTRL_ZZ.
+00002660: 5348 4946 545f 5441 425a 0853 4849 4654  SHIFT_TABZ.SHIFT
+00002670: 5f46 315a 0853 4849 4654 5f46 325a 0853  _F1Z.SHIFT_F2Z.S
+00002680: 4849 4654 5f46 335a 0853 4849 4654 5f46  HIFT_F3Z.SHIFT_F
+00002690: 345a 0853 4849 4654 5f46 355a 0853 4849  4Z.SHIFT_F5Z.SHI
+000026a0: 4654 5f46 365a 0853 4849 4654 5f46 375a  FT_F6Z.SHIFT_F7Z
+000026b0: 0853 4849 4654 5f46 385a 0853 4849 4654  .SHIFT_F8Z.SHIFT
+000026c0: 5f46 395a 0953 4849 4654 5f46 3130 5a09  _F9Z.SHIFT_F10Z.
+000026d0: 5348 4946 545f 4631 315a 0953 4849 4654  SHIFT_F11Z.SHIFT
+000026e0: 5f46 3132 5a1d 5348 4946 545f 4f45 4d33  _F12Z.SHIFT_OEM3
+000026f0: 5f57 4156 455f 4f52 5f42 4143 4b5f 5155  _WAVE_OR_BACK_QU
+00002700: 4f54 455a 0753 4849 4654 5f31 5a07 5348  OTEZ.SHIFT_1Z.SH
+00002710: 4946 545f 325a 0753 4849 4654 5f33 5a07  IFT_2Z.SHIFT_3Z.
+00002720: 5348 4946 545f 345a 0753 4849 4654 5f35  SHIFT_4Z.SHIFT_5
+00002730: 5a07 5348 4946 545f 365a 0753 4849 4654  Z.SHIFT_6Z.SHIFT
+00002740: 5f37 5a07 5348 4946 545f 385a 0753 4849  _7Z.SHIFT_8Z.SHI
+00002750: 4654 5f39 5a07 5348 4946 545f 305a 0e53  FT_9Z.SHIFT_0Z.S
+00002760: 4849 4654 5f31 315f 4d49 4e55 535a 0d53  HIFT_11_MINUSZ.S
+00002770: 4849 4654 5f31 325f 504c 5553 5a0f 5348  HIFT_12_PLUSZ.SH
+00002780: 4946 545f 4241 434b 5350 4143 455a 0e53  IFT_BACKSPACEZ.S
+00002790: 4849 4654 5f4e 554d 5041 445f 315a 0e53  HIFT_NUMPAD_1Z.S
+000027a0: 4849 4654 5f4e 554d 5041 445f 325a 0e53  HIFT_NUMPAD_2Z.S
+000027b0: 4849 4654 5f4e 554d 5041 445f 335a 0e53  HIFT_NUMPAD_3Z.S
+000027c0: 4849 4654 5f4e 554d 5041 445f 345a 0e53  HIFT_NUMPAD_4Z.S
+000027d0: 4849 4654 5f4e 554d 5041 445f 355a 0e53  HIFT_NUMPAD_5Z.S
+000027e0: 4849 4654 5f4e 554d 5041 445f 365a 0e53  HIFT_NUMPAD_6Z.S
+000027f0: 4849 4654 5f4e 554d 5041 445f 375a 0e53  HIFT_NUMPAD_7Z.S
+00002800: 4849 4654 5f4e 554d 5041 445f 385a 0e53  HIFT_NUMPAD_8Z.S
+00002810: 4849 4654 5f4e 554d 5041 445f 395a 0e53  HIFT_NUMPAD_9Z.S
+00002820: 4849 4654 5f4e 554d 5041 445f 305a 1653  HIFT_NUMPAD_0Z.S
+00002830: 4849 4654 5f4e 554d 5041 445f 3131 5f44  HIFT_NUMPAD_11_D
+00002840: 4956 4944 455a 1853 4849 4654 5f4e 554d  IVIDEZ.SHIFT_NUM
+00002850: 5041 445f 3132 5f4d 554c 5449 504c 595a  PAD_12_MULTIPLYZ
+00002860: 0753 4849 4654 5f41 5a07 5348 4946 545f  .SHIFT_AZ.SHIFT_
+00002870: 425a 0753 4849 4654 5f43 5a07 5348 4946  BZ.SHIFT_CZ.SHIF
+00002880: 545f 445a 0753 4849 4654 5f45 5a07 5348  T_DZ.SHIFT_EZ.SH
+00002890: 4946 545f 465a 0753 4849 4654 5f47 5a07  IFT_FZ.SHIFT_GZ.
+000028a0: 5348 4946 545f 485a 0753 4849 4654 5f49  SHIFT_HZ.SHIFT_I
+000028b0: 5a07 5348 4946 545f 4a5a 0753 4849 4654  Z.SHIFT_JZ.SHIFT
+000028c0: 5f4b 5a07 5348 4946 545f 4c5a 0753 4849  _KZ.SHIFT_LZ.SHI
+000028d0: 4654 5f4d 5a07 5348 4946 545f 4e5a 0753  FT_MZ.SHIFT_NZ.S
+000028e0: 4849 4654 5f4f 5a07 5348 4946 545f 505a  HIFT_OZ.SHIFT_PZ
+000028f0: 0753 4849 4654 5f51 5a07 5348 4946 545f  .SHIFT_QZ.SHIFT_
+00002900: 525a 0753 4849 4654 5f53 5a07 5348 4946  RZ.SHIFT_SZ.SHIF
+00002910: 545f 545a 0753 4849 4654 5f55 5a07 5348  T_TZ.SHIFT_UZ.SH
+00002920: 4946 545f 565a 0753 4849 4654 5f57 5a07  IFT_VZ.SHIFT_WZ.
+00002930: 5348 4946 545f 585a 0753 4849 4654 5f59  SHIFT_XZ.SHIFT_Y
+00002940: 5a07 5348 4946 545f 5a5a 0741 4c54 5f54  Z.SHIFT_ZZ.ALT_T
+00002950: 4142 5a06 414c 545f 4631 5a06 414c 545f  ABZ.ALT_F1Z.ALT_
+00002960: 4632 5a06 414c 545f 4633 5a06 414c 545f  F2Z.ALT_F3Z.ALT_
+00002970: 4634 5a06 414c 545f 4635 5a06 414c 545f  F4Z.ALT_F5Z.ALT_
+00002980: 4636 5a06 414c 545f 4637 5a06 414c 545f  F6Z.ALT_F7Z.ALT_
+00002990: 4638 5a06 414c 545f 4639 5a07 414c 545f  F8Z.ALT_F9Z.ALT_
+000029a0: 4631 305a 0741 4c54 5f46 3131 5a07 414c  F10Z.ALT_F11Z.AL
+000029b0: 545f 4631 325a 1b41 4c54 5f4f 454d 335f  T_F12Z.ALT_OEM3_
+000029c0: 5741 5645 5f4f 525f 4241 434b 5f51 554f  WAVE_OR_BACK_QUO
+000029d0: 5445 5a05 414c 545f 315a 0541 4c54 5f32  TEZ.ALT_1Z.ALT_2
+000029e0: 5a05 414c 545f 335a 0541 4c54 5f34 5a05  Z.ALT_3Z.ALT_4Z.
+000029f0: 414c 545f 355a 0541 4c54 5f36 5a05 414c  ALT_5Z.ALT_6Z.AL
+00002a00: 545f 375a 0541 4c54 5f38 5a05 414c 545f  T_7Z.ALT_8Z.ALT_
+00002a10: 395a 0541 4c54 5f30 5a0c 414c 545f 3131  9Z.ALT_0Z.ALT_11
+00002a20: 5f4d 494e 5553 5a0b 414c 545f 3132 5f50  _MINUSZ.ALT_12_P
+00002a30: 4c55 535a 0d41 4c54 5f42 4143 4b53 5041  LUSZ.ALT_BACKSPA
+00002a40: 4345 5a0c 414c 545f 4e55 4d50 4144 5f31  CEZ.ALT_NUMPAD_1
+00002a50: 5a0c 414c 545f 4e55 4d50 4144 5f32 5a0c  Z.ALT_NUMPAD_2Z.
+00002a60: 414c 545f 4e55 4d50 4144 5f33 5a0c 414c  ALT_NUMPAD_3Z.AL
+00002a70: 545f 4e55 4d50 4144 5f34 5a0c 414c 545f  T_NUMPAD_4Z.ALT_
+00002a80: 4e55 4d50 4144 5f35 5a0c 414c 545f 4e55  NUMPAD_5Z.ALT_NU
+00002a90: 4d50 4144 5f36 5a0c 414c 545f 4e55 4d50  MPAD_6Z.ALT_NUMP
+00002aa0: 4144 5f37 5a0c 414c 545f 4e55 4d50 4144  AD_7Z.ALT_NUMPAD
+00002ab0: 5f38 5a0c 414c 545f 4e55 4d50 4144 5f39  _8Z.ALT_NUMPAD_9
+00002ac0: 5a0c 414c 545f 4e55 4d50 4144 5f30 5a14  Z.ALT_NUMPAD_0Z.
+00002ad0: 414c 545f 4e55 4d50 4144 5f31 315f 4449  ALT_NUMPAD_11_DI
+00002ae0: 5649 4445 5a16 414c 545f 4e55 4d50 4144  VIDEZ.ALT_NUMPAD
+00002af0: 5f31 325f 4d55 4c54 4950 4c59 5a05 414c  _12_MULTIPLYZ.AL
+00002b00: 545f 415a 0541 4c54 5f42 5a05 414c 545f  T_AZ.ALT_BZ.ALT_
+00002b10: 435a 0541 4c54 5f44 5a05 414c 545f 455a  CZ.ALT_DZ.ALT_EZ
+00002b20: 0541 4c54 5f46 5a05 414c 545f 475a 0541  .ALT_FZ.ALT_GZ.A
+00002b30: 4c54 5f48 5a05 414c 545f 495a 0541 4c54  LT_HZ.ALT_IZ.ALT
+00002b40: 5f4a 5a05 414c 545f 4b5a 0541 4c54 5f4c  _JZ.ALT_KZ.ALT_L
+00002b50: 5a05 414c 545f 4d5a 0541 4c54 5f4e 5a05  Z.ALT_MZ.ALT_NZ.
+00002b60: 414c 545f 4f5a 0541 4c54 5f50 5a05 414c  ALT_OZ.ALT_PZ.AL
+00002b70: 545f 515a 0541 4c54 5f52 5a05 414c 545f  T_QZ.ALT_RZ.ALT_
+00002b80: 535a 0541 4c54 5f54 5a05 414c 545f 555a  SZ.ALT_TZ.ALT_UZ
+00002b90: 0541 4c54 5f56 5a05 414c 545f 575a 0541  .ALT_VZ.ALT_WZ.A
+00002ba0: 4c54 5f58 5a05 414c 545f 595a 0541 4c54  LT_XZ.ALT_YZ.ALT
+00002bb0: 5f5a 5a0b 4354 524c 5f41 4c54 5f46 315a  _ZZ.CTRL_ALT_F1Z
+00002bc0: 0b43 5452 4c5f 414c 545f 4632 5a0b 4354  .CTRL_ALT_F2Z.CT
+00002bd0: 524c 5f41 4c54 5f46 335a 0b43 5452 4c5f  RL_ALT_F3Z.CTRL_
+00002be0: 414c 545f 4634 5a0b 4354 524c 5f41 4c54  ALT_F4Z.CTRL_ALT
+00002bf0: 5f46 355a 0b43 5452 4c5f 414c 545f 4636  _F5Z.CTRL_ALT_F6
+00002c00: 5a0b 4354 524c 5f41 4c54 5f46 375a 0b43  Z.CTRL_ALT_F7Z.C
+00002c10: 5452 4c5f 414c 545f 4638 5a0b 4354 524c  TRL_ALT_F8Z.CTRL
+00002c20: 5f41 4c54 5f46 395a 0c43 5452 4c5f 414c  _ALT_F9Z.CTRL_AL
+00002c30: 545f 4631 305a 0c43 5452 4c5f 414c 545f  T_F10Z.CTRL_ALT_
+00002c40: 4631 315a 0c43 5452 4c5f 414c 545f 4631  F11Z.CTRL_ALT_F1
+00002c50: 325a 2043 5452 4c5f 414c 545f 4f45 4d33  2Z CTRL_ALT_OEM3
+00002c60: 5f57 4156 455f 4f52 5f42 4143 4b5f 5155  _WAVE_OR_BACK_QU
+00002c70: 4f54 455a 0a43 5452 4c5f 414c 545f 315a  OTEZ.CTRL_ALT_1Z
+00002c80: 0a43 5452 4c5f 414c 545f 325a 0a43 5452  .CTRL_ALT_2Z.CTR
+00002c90: 4c5f 414c 545f 335a 0a43 5452 4c5f 414c  L_ALT_3Z.CTRL_AL
+00002ca0: 545f 345a 0a43 5452 4c5f 414c 545f 355a  T_4Z.CTRL_ALT_5Z
+00002cb0: 0a43 5452 4c5f 414c 545f 365a 0a43 5452  .CTRL_ALT_6Z.CTR
+00002cc0: 4c5f 414c 545f 375a 0a43 5452 4c5f 414c  L_ALT_7Z.CTRL_AL
+00002cd0: 545f 385a 0a43 5452 4c5f 414c 545f 395a  T_8Z.CTRL_ALT_9Z
+00002ce0: 0a43 5452 4c5f 414c 545f 305a 1143 5452  .CTRL_ALT_0Z.CTR
+00002cf0: 4c5f 414c 545f 3131 5f4d 494e 5553 5a10  L_ALT_11_MINUSZ.
+00002d00: 4354 524c 5f41 4c54 5f31 325f 504c 5553  CTRL_ALT_12_PLUS
+00002d10: 5a12 4354 524c 5f41 4c54 5f42 4143 4b53  Z.CTRL_ALT_BACKS
+00002d20: 5041 4345 5a11 4354 524c 5f41 4c54 5f4e  PACEZ.CTRL_ALT_N
+00002d30: 554d 5041 445f 315a 1143 5452 4c5f 414c  UMPAD_1Z.CTRL_AL
+00002d40: 545f 4e55 4d50 4144 5f32 5a11 4354 524c  T_NUMPAD_2Z.CTRL
+00002d50: 5f41 4c54 5f4e 554d 5041 445f 335a 1143  _ALT_NUMPAD_3Z.C
+00002d60: 5452 4c5f 414c 545f 4e55 4d50 4144 5f34  TRL_ALT_NUMPAD_4
+00002d70: 5a11 4354 524c 5f41 4c54 5f4e 554d 5041  Z.CTRL_ALT_NUMPA
+00002d80: 445f 355a 1143 5452 4c5f 414c 545f 4e55  D_5Z.CTRL_ALT_NU
+00002d90: 4d50 4144 5f36 5a11 4354 524c 5f41 4c54  MPAD_6Z.CTRL_ALT
+00002da0: 5f4e 554d 5041 445f 375a 1143 5452 4c5f  _NUMPAD_7Z.CTRL_
+00002db0: 414c 545f 4e55 4d50 4144 5f38 5a11 4354  ALT_NUMPAD_8Z.CT
+00002dc0: 524c 5f41 4c54 5f4e 554d 5041 445f 395a  RL_ALT_NUMPAD_9Z
+00002dd0: 1143 5452 4c5f 414c 545f 4e55 4d50 4144  .CTRL_ALT_NUMPAD
+00002de0: 5f30 5a19 4354 524c 5f41 4c54 5f4e 554d  _0Z.CTRL_ALT_NUM
+00002df0: 5041 445f 3131 5f44 4956 4944 455a 1b43  PAD_11_DIVIDEZ.C
+00002e00: 5452 4c5f 414c 545f 4e55 4d50 4144 5f31  TRL_ALT_NUMPAD_1
+00002e10: 325f 4d55 4c54 4950 4c59 5a0a 4354 524c  2_MULTIPLYZ.CTRL
+00002e20: 5f41 4c54 5f41 5a0a 4354 524c 5f41 4c54  _ALT_AZ.CTRL_ALT
+00002e30: 5f42 5a0a 4354 524c 5f41 4c54 5f43 5a0a  _BZ.CTRL_ALT_CZ.
+00002e40: 4354 524c 5f41 4c54 5f44 5a0a 4354 524c  CTRL_ALT_DZ.CTRL
+00002e50: 5f41 4c54 5f45 5a0a 4354 524c 5f41 4c54  _ALT_EZ.CTRL_ALT
+00002e60: 5f46 5a0a 4354 524c 5f41 4c54 5f47 5a0a  _FZ.CTRL_ALT_GZ.
+00002e70: 4354 524c 5f41 4c54 5f48 5a0a 4354 524c  CTRL_ALT_HZ.CTRL
+00002e80: 5f41 4c54 5f49 5a0a 4354 524c 5f41 4c54  _ALT_IZ.CTRL_ALT
+00002e90: 5f4a 5a0a 4354 524c 5f41 4c54 5f4b 5a0a  _JZ.CTRL_ALT_KZ.
+00002ea0: 4354 524c 5f41 4c54 5f4c 5a0a 4354 524c  CTRL_ALT_LZ.CTRL
+00002eb0: 5f41 4c54 5f4d 5a0a 4354 524c 5f41 4c54  _ALT_MZ.CTRL_ALT
+00002ec0: 5f4e 5a0a 4354 524c 5f41 4c54 5f4f 5a0a  _NZ.CTRL_ALT_OZ.
+00002ed0: 4354 524c 5f41 4c54 5f50 5a0a 4354 524c  CTRL_ALT_PZ.CTRL
+00002ee0: 5f41 4c54 5f51 5a0a 4354 524c 5f41 4c54  _ALT_QZ.CTRL_ALT
+00002ef0: 5f52 5a0a 4354 524c 5f41 4c54 5f53 5a0a  _RZ.CTRL_ALT_SZ.
+00002f00: 4354 524c 5f41 4c54 5f54 5a0a 4354 524c  CTRL_ALT_TZ.CTRL
+00002f10: 5f41 4c54 5f55 5a0a 4354 524c 5f41 4c54  _ALT_UZ.CTRL_ALT
+00002f20: 5f56 5a0a 4354 524c 5f41 4c54 5f57 5a0a  _VZ.CTRL_ALT_WZ.
+00002f30: 4354 524c 5f41 4c54 5f58 5a0a 4354 524c  CTRL_ALT_XZ.CTRL
+00002f40: 5f41 4c54 5f59 5a0a 4354 524c 5f41 4c54  _ALT_YZ.CTRL_ALT
+00002f50: 5f5a 5a0d 4354 524c 5f53 4849 4654 5f46  _ZZ.CTRL_SHIFT_F
+00002f60: 315a 0d43 5452 4c5f 5348 4946 545f 4632  1Z.CTRL_SHIFT_F2
+00002f70: 5a0d 4354 524c 5f53 4849 4654 5f46 335a  Z.CTRL_SHIFT_F3Z
+00002f80: 0d43 5452 4c5f 5348 4946 545f 4634 5a0d  .CTRL_SHIFT_F4Z.
+00002f90: 4354 524c 5f53 4849 4654 5f46 355a 0d43  CTRL_SHIFT_F5Z.C
+00002fa0: 5452 4c5f 5348 4946 545f 4636 5a0d 4354  TRL_SHIFT_F6Z.CT
+00002fb0: 524c 5f53 4849 4654 5f46 375a 0d43 5452  RL_SHIFT_F7Z.CTR
+00002fc0: 4c5f 5348 4946 545f 4638 5a0d 4354 524c  L_SHIFT_F8Z.CTRL
+00002fd0: 5f53 4849 4654 5f46 395a 0e43 5452 4c5f  _SHIFT_F9Z.CTRL_
+00002fe0: 5348 4946 545f 4631 305a 0e43 5452 4c5f  SHIFT_F10Z.CTRL_
+00002ff0: 5348 4946 545f 4631 315a 0e43 5452 4c5f  SHIFT_F11Z.CTRL_
+00003000: 5348 4946 545f 4631 325a 2243 5452 4c5f  SHIFT_F12Z"CTRL_
+00003010: 5348 4946 545f 4f45 4d33 5f57 4156 455f  SHIFT_OEM3_WAVE_
+00003020: 4f52 5f42 4143 4b5f 5155 4f54 455a 0c43  OR_BACK_QUOTEZ.C
+00003030: 5452 4c5f 5348 4946 545f 315a 0c43 5452  TRL_SHIFT_1Z.CTR
+00003040: 4c5f 5348 4946 545f 325a 0c43 5452 4c5f  L_SHIFT_2Z.CTRL_
+00003050: 5348 4946 545f 335a 0c43 5452 4c5f 5348  SHIFT_3Z.CTRL_SH
+00003060: 4946 545f 345a 0c43 5452 4c5f 5348 4946  IFT_4Z.CTRL_SHIF
+00003070: 545f 355a 0c43 5452 4c5f 5348 4946 545f  T_5Z.CTRL_SHIFT_
+00003080: 365a 0c43 5452 4c5f 5348 4946 545f 375a  6Z.CTRL_SHIFT_7Z
+00003090: 0c43 5452 4c5f 5348 4946 545f 385a 0c43  .CTRL_SHIFT_8Z.C
+000030a0: 5452 4c5f 5348 4946 545f 395a 0c43 5452  TRL_SHIFT_9Z.CTR
+000030b0: 4c5f 5348 4946 545f 305a 1343 5452 4c5f  L_SHIFT_0Z.CTRL_
+000030c0: 5348 4946 545f 3131 5f4d 494e 5553 5a12  SHIFT_11_MINUSZ.
+000030d0: 4354 524c 5f53 4849 4654 5f31 325f 504c  CTRL_SHIFT_12_PL
+000030e0: 5553 5a14 4354 524c 5f53 4849 4654 5f42  USZ.CTRL_SHIFT_B
+000030f0: 4143 4b53 5041 4345 5a13 4354 524c 5f53  ACKSPACEZ.CTRL_S
+00003100: 4849 4654 5f4e 554d 5041 445f 315a 1343  HIFT_NUMPAD_1Z.C
+00003110: 5452 4c5f 5348 4946 545f 4e55 4d50 4144  TRL_SHIFT_NUMPAD
+00003120: 5f32 5a13 4354 524c 5f53 4849 4654 5f4e  _2Z.CTRL_SHIFT_N
+00003130: 554d 5041 445f 335a 1343 5452 4c5f 5348  UMPAD_3Z.CTRL_SH
+00003140: 4946 545f 4e55 4d50 4144 5f34 5a13 4354  IFT_NUMPAD_4Z.CT
+00003150: 524c 5f53 4849 4654 5f4e 554d 5041 445f  RL_SHIFT_NUMPAD_
+00003160: 355a 1343 5452 4c5f 5348 4946 545f 4e55  5Z.CTRL_SHIFT_NU
+00003170: 4d50 4144 5f36 5a13 4354 524c 5f53 4849  MPAD_6Z.CTRL_SHI
+00003180: 4654 5f4e 554d 5041 445f 375a 1343 5452  FT_NUMPAD_7Z.CTR
+00003190: 4c5f 5348 4946 545f 4e55 4d50 4144 5f38  L_SHIFT_NUMPAD_8
+000031a0: 5a13 4354 524c 5f53 4849 4654 5f4e 554d  Z.CTRL_SHIFT_NUM
+000031b0: 5041 445f 395a 1343 5452 4c5f 5348 4946  PAD_9Z.CTRL_SHIF
+000031c0: 545f 4e55 4d50 4144 5f30 5a1b 4354 524c  T_NUMPAD_0Z.CTRL
+000031d0: 5f53 4849 4654 5f4e 554d 5041 445f 3131  _SHIFT_NUMPAD_11
+000031e0: 5f44 4956 4944 455a 1d43 5452 4c5f 5348  _DIVIDEZ.CTRL_SH
+000031f0: 4946 545f 4e55 4d50 4144 5f31 325f 4d55  IFT_NUMPAD_12_MU
+00003200: 4c54 4950 4c59 5a0c 4354 524c 5f53 4849  LTIPLYZ.CTRL_SHI
+00003210: 4654 5f41 5a0c 4354 524c 5f53 4849 4654  FT_AZ.CTRL_SHIFT
+00003220: 5f42 5a0c 4354 524c 5f53 4849 4654 5f43  _BZ.CTRL_SHIFT_C
+00003230: 5a0c 4354 524c 5f53 4849 4654 5f44 5a0c  Z.CTRL_SHIFT_DZ.
+00003240: 4354 524c 5f53 4849 4654 5f45 5a0c 4354  CTRL_SHIFT_EZ.CT
+00003250: 524c 5f53 4849 4654 5f46 5a0c 4354 524c  RL_SHIFT_FZ.CTRL
+00003260: 5f53 4849 4654 5f47 5a0c 4354 524c 5f53  _SHIFT_GZ.CTRL_S
+00003270: 4849 4654 5f48 5a0c 4354 524c 5f53 4849  HIFT_HZ.CTRL_SHI
+00003280: 4654 5f49 5a0c 4354 524c 5f53 4849 4654  FT_IZ.CTRL_SHIFT
+00003290: 5f4a 5a0c 4354 524c 5f53 4849 4654 5f4b  _JZ.CTRL_SHIFT_K
+000032a0: 5a0c 4354 524c 5f53 4849 4654 5f4c 5a0c  Z.CTRL_SHIFT_LZ.
+000032b0: 4354 524c 5f53 4849 4654 5f4d 5a0c 4354  CTRL_SHIFT_MZ.CT
+000032c0: 524c 5f53 4849 4654 5f4e 5a0c 4354 524c  RL_SHIFT_NZ.CTRL
+000032d0: 5f53 4849 4654 5f4f 5a0c 4354 524c 5f53  _SHIFT_OZ.CTRL_S
+000032e0: 4849 4654 5f50 5a0c 4354 524c 5f53 4849  HIFT_PZ.CTRL_SHI
+000032f0: 4654 5f51 5a0c 4354 524c 5f53 4849 4654  FT_QZ.CTRL_SHIFT
+00003300: 5f52 5a0c 4354 524c 5f53 4849 4654 5f53  _RZ.CTRL_SHIFT_S
+00003310: 5a0c 4354 524c 5f53 4849 4654 5f54 5a0c  Z.CTRL_SHIFT_TZ.
+00003320: 4354 524c 5f53 4849 4654 5f55 5a0c 4354  CTRL_SHIFT_UZ.CT
+00003330: 524c 5f53 4849 4654 5f56 5a0c 4354 524c  RL_SHIFT_VZ.CTRL
+00003340: 5f53 4849 4654 5f57 5a0c 4354 524c 5f53  _SHIFT_WZ.CTRL_S
+00003350: 4849 4654 5f58 5a0c 4354 524c 5f53 4849  HIFT_XZ.CTRL_SHI
+00003360: 4654 5f59 5a0c 4354 524c 5f53 4849 4654  FT_YZ.CTRL_SHIFT
+00003370: 5f5a 5a0c 414c 545f 5348 4946 545f 4631  _ZZ.ALT_SHIFT_F1
+00003380: 5a0c 414c 545f 5348 4946 545f 4632 5a0c  Z.ALT_SHIFT_F2Z.
+00003390: 414c 545f 5348 4946 545f 4633 5a0c 414c  ALT_SHIFT_F3Z.AL
+000033a0: 545f 5348 4946 545f 4634 5a0c 414c 545f  T_SHIFT_F4Z.ALT_
+000033b0: 5348 4946 545f 4635 5a0c 414c 545f 5348  SHIFT_F5Z.ALT_SH
+000033c0: 4946 545f 4636 5a0c 414c 545f 5348 4946  IFT_F6Z.ALT_SHIF
+000033d0: 545f 4637 5a0c 414c 545f 5348 4946 545f  T_F7Z.ALT_SHIFT_
+000033e0: 4638 5a0c 414c 545f 5348 4946 545f 4639  F8Z.ALT_SHIFT_F9
+000033f0: 5a0d 414c 545f 5348 4946 545f 4631 305a  Z.ALT_SHIFT_F10Z
+00003400: 0d41 4c54 5f53 4849 4654 5f46 3131 5a0d  .ALT_SHIFT_F11Z.
+00003410: 414c 545f 5348 4946 545f 4631 325a 2141  ALT_SHIFT_F12Z!A
+00003420: 4c54 5f53 4849 4654 5f4f 454d 335f 5741  LT_SHIFT_OEM3_WA
+00003430: 5645 5f4f 525f 4241 434b 5f51 554f 5445  VE_OR_BACK_QUOTE
+00003440: 5a0b 414c 545f 5348 4946 545f 315a 0b41  Z.ALT_SHIFT_1Z.A
+00003450: 4c54 5f53 4849 4654 5f32 5a0b 414c 545f  LT_SHIFT_2Z.ALT_
+00003460: 5348 4946 545f 335a 0b41 4c54 5f53 4849  SHIFT_3Z.ALT_SHI
+00003470: 4654 5f34 5a0b 414c 545f 5348 4946 545f  FT_4Z.ALT_SHIFT_
+00003480: 355a 0b41 4c54 5f53 4849 4654 5f36 5a0b  5Z.ALT_SHIFT_6Z.
+00003490: 414c 545f 5348 4946 545f 375a 0b41 4c54  ALT_SHIFT_7Z.ALT
+000034a0: 5f53 4849 4654 5f38 5a0b 414c 545f 5348  _SHIFT_8Z.ALT_SH
+000034b0: 4946 545f 395a 0b41 4c54 5f53 4849 4654  IFT_9Z.ALT_SHIFT
+000034c0: 5f30 5a12 414c 545f 5348 4946 545f 3131  _0Z.ALT_SHIFT_11
+000034d0: 5f4d 494e 5553 5a11 414c 545f 5348 4946  _MINUSZ.ALT_SHIF
+000034e0: 545f 3132 5f50 4c55 535a 1341 4c54 5f53  T_12_PLUSZ.ALT_S
+000034f0: 4849 4654 5f42 4143 4b53 5041 4345 5a12  HIFT_BACKSPACEZ.
+00003500: 414c 545f 5348 4946 545f 4e55 4d50 4144  ALT_SHIFT_NUMPAD
+00003510: 5f31 5a12 414c 545f 5348 4946 545f 4e55  _1Z.ALT_SHIFT_NU
+00003520: 4d50 4144 5f32 5a12 414c 545f 5348 4946  MPAD_2Z.ALT_SHIF
+00003530: 545f 4e55 4d50 4144 5f33 5a12 414c 545f  T_NUMPAD_3Z.ALT_
+00003540: 5348 4946 545f 4e55 4d50 4144 5f34 5a12  SHIFT_NUMPAD_4Z.
+00003550: 414c 545f 5348 4946 545f 4e55 4d50 4144  ALT_SHIFT_NUMPAD
+00003560: 5f35 5a12 414c 545f 5348 4946 545f 4e55  _5Z.ALT_SHIFT_NU
+00003570: 4d50 4144 5f36 5a12 414c 545f 5348 4946  MPAD_6Z.ALT_SHIF
+00003580: 545f 4e55 4d50 4144 5f37 5a12 414c 545f  T_NUMPAD_7Z.ALT_
+00003590: 5348 4946 545f 4e55 4d50 4144 5f38 5a12  SHIFT_NUMPAD_8Z.
+000035a0: 414c 545f 5348 4946 545f 4e55 4d50 4144  ALT_SHIFT_NUMPAD
+000035b0: 5f39 5a12 414c 545f 5348 4946 545f 4e55  _9Z.ALT_SHIFT_NU
+000035c0: 4d50 4144 5f30 5a1a 414c 545f 5348 4946  MPAD_0Z.ALT_SHIF
+000035d0: 545f 4e55 4d50 4144 5f31 315f 4449 5649  T_NUMPAD_11_DIVI
+000035e0: 4445 5a1c 414c 545f 5348 4946 545f 4e55  DEZ.ALT_SHIFT_NU
+000035f0: 4d50 4144 5f31 325f 4d55 4c54 4950 4c59  MPAD_12_MULTIPLY
+00003600: 5a0b 414c 545f 5348 4946 545f 415a 0b41  Z.ALT_SHIFT_AZ.A
+00003610: 4c54 5f53 4849 4654 5f42 5a0b 414c 545f  LT_SHIFT_BZ.ALT_
+00003620: 5348 4946 545f 435a 0b41 4c54 5f53 4849  SHIFT_CZ.ALT_SHI
+00003630: 4654 5f44 5a0b 414c 545f 5348 4946 545f  FT_DZ.ALT_SHIFT_
+00003640: 455a 0b41 4c54 5f53 4849 4654 5f46 5a0b  EZ.ALT_SHIFT_FZ.
+00003650: 414c 545f 5348 4946 545f 475a 0b41 4c54  ALT_SHIFT_GZ.ALT
+00003660: 5f53 4849 4654 5f48 5a0b 414c 545f 5348  _SHIFT_HZ.ALT_SH
+00003670: 4946 545f 495a 0b41 4c54 5f53 4849 4654  IFT_IZ.ALT_SHIFT
+00003680: 5f4a 5a0b 414c 545f 5348 4946 545f 4b5a  _JZ.ALT_SHIFT_KZ
+00003690: 0b41 4c54 5f53 4849 4654 5f4c 5a0b 414c  .ALT_SHIFT_LZ.AL
+000036a0: 545f 5348 4946 545f 4d5a 0b41 4c54 5f53  T_SHIFT_MZ.ALT_S
+000036b0: 4849 4654 5f4e 5a0b 414c 545f 5348 4946  HIFT_NZ.ALT_SHIF
+000036c0: 545f 4f5a 0b41 4c54 5f53 4849 4654 5f50  T_OZ.ALT_SHIFT_P
+000036d0: 5a0b 414c 545f 5348 4946 545f 515a 0b41  Z.ALT_SHIFT_QZ.A
+000036e0: 4c54 5f53 4849 4654 5f52 5a0b 414c 545f  LT_SHIFT_RZ.ALT_
+000036f0: 5348 4946 545f 535a 0b41 4c54 5f53 4849  SHIFT_SZ.ALT_SHI
+00003700: 4654 5f54 5a0b 414c 545f 5348 4946 545f  FT_TZ.ALT_SHIFT_
+00003710: 555a 0b41 4c54 5f53 4849 4654 5f56 5a0b  UZ.ALT_SHIFT_VZ.
+00003720: 414c 545f 5348 4946 545f 575a 0b41 4c54  ALT_SHIFT_WZ.ALT
+00003730: 5f53 4849 4654 5f58 5a0b 414c 545f 5348  _SHIFT_XZ.ALT_SH
+00003740: 4946 545f 595a 0b41 4c54 5f53 4849 4654  IFT_YZ.ALT_SHIFT
+00003750: 5f5a 5a11 4354 524c 5f53 4849 4654 5f41  _ZZ.CTRL_SHIFT_A
+00003760: 4c54 5f46 315a 1143 5452 4c5f 5348 4946  LT_F1Z.CTRL_SHIF
+00003770: 545f 414c 545f 4632 5a11 4354 524c 5f53  T_ALT_F2Z.CTRL_S
+00003780: 4849 4654 5f41 4c54 5f46 335a 1143 5452  HIFT_ALT_F3Z.CTR
+00003790: 4c5f 5348 4946 545f 414c 545f 4634 5a11  L_SHIFT_ALT_F4Z.
+000037a0: 4354 524c 5f53 4849 4654 5f41 4c54 5f46  CTRL_SHIFT_ALT_F
+000037b0: 355a 1143 5452 4c5f 5348 4946 545f 414c  5Z.CTRL_SHIFT_AL
+000037c0: 545f 4636 5a11 4354 524c 5f53 4849 4654  T_F6Z.CTRL_SHIFT
+000037d0: 5f41 4c54 5f46 375a 1143 5452 4c5f 5348  _ALT_F7Z.CTRL_SH
+000037e0: 4946 545f 414c 545f 4638 5a11 4354 524c  IFT_ALT_F8Z.CTRL
+000037f0: 5f53 4849 4654 5f41 4c54 5f46 395a 1243  _SHIFT_ALT_F9Z.C
+00003800: 5452 4c5f 5348 4946 545f 414c 545f 4631  TRL_SHIFT_ALT_F1
+00003810: 305a 1243 5452 4c5f 5348 4946 545f 414c  0Z.CTRL_SHIFT_AL
+00003820: 545f 4631 315a 1243 5452 4c5f 5348 4946  T_F11Z.CTRL_SHIF
+00003830: 545f 414c 545f 4631 325a 2643 5452 4c5f  T_ALT_F12Z&CTRL_
+00003840: 5348 4946 545f 414c 545f 4f45 4d33 5f57  SHIFT_ALT_OEM3_W
+00003850: 4156 455f 4f52 5f42 4143 4b5f 5155 4f54  AVE_OR_BACK_QUOT
+00003860: 455a 1043 5452 4c5f 5348 4946 545f 414c  EZ.CTRL_SHIFT_AL
+00003870: 545f 315a 1043 5452 4c5f 5348 4946 545f  T_1Z.CTRL_SHIFT_
+00003880: 414c 545f 325a 1043 5452 4c5f 5348 4946  ALT_2Z.CTRL_SHIF
+00003890: 545f 414c 545f 335a 1043 5452 4c5f 5348  T_ALT_3Z.CTRL_SH
+000038a0: 4946 545f 414c 545f 345a 1043 5452 4c5f  IFT_ALT_4Z.CTRL_
+000038b0: 5348 4946 545f 414c 545f 355a 1043 5452  SHIFT_ALT_5Z.CTR
+000038c0: 4c5f 5348 4946 545f 414c 545f 365a 1043  L_SHIFT_ALT_6Z.C
+000038d0: 5452 4c5f 5348 4946 545f 414c 545f 375a  TRL_SHIFT_ALT_7Z
+000038e0: 1043 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+000038f0: 385a 1043 5452 4c5f 5348 4946 545f 414c  8Z.CTRL_SHIFT_AL
+00003900: 545f 395a 1043 5452 4c5f 5348 4946 545f  T_9Z.CTRL_SHIFT_
+00003910: 414c 545f 305a 1743 5452 4c5f 5348 4946  ALT_0Z.CTRL_SHIF
+00003920: 545f 414c 545f 3131 5f4d 494e 5553 5a16  T_ALT_11_MINUSZ.
+00003930: 4354 524c 5f53 4849 4654 5f41 4c54 5f31  CTRL_SHIFT_ALT_1
+00003940: 325f 504c 5553 5a18 4354 524c 5f53 4849  2_PLUSZ.CTRL_SHI
+00003950: 4654 5f41 4c54 5f42 4143 4b53 5041 4345  FT_ALT_BACKSPACE
+00003960: 5a17 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
+00003970: 5f4e 554d 5041 445f 315a 1743 5452 4c5f  _NUMPAD_1Z.CTRL_
+00003980: 5348 4946 545f 414c 545f 4e55 4d50 4144  SHIFT_ALT_NUMPAD
+00003990: 5f32 5a17 4354 524c 5f53 4849 4654 5f41  _2Z.CTRL_SHIFT_A
+000039a0: 4c54 5f4e 554d 5041 445f 335a 1743 5452  LT_NUMPAD_3Z.CTR
+000039b0: 4c5f 5348 4946 545f 414c 545f 4e55 4d50  L_SHIFT_ALT_NUMP
+000039c0: 4144 5f34 5a17 4354 524c 5f53 4849 4654  AD_4Z.CTRL_SHIFT
+000039d0: 5f41 4c54 5f4e 554d 5041 445f 355a 1743  _ALT_NUMPAD_5Z.C
+000039e0: 5452 4c5f 5348 4946 545f 414c 545f 4e55  TRL_SHIFT_ALT_NU
+000039f0: 4d50 4144 5f36 5a17 4354 524c 5f53 4849  MPAD_6Z.CTRL_SHI
+00003a00: 4654 5f41 4c54 5f4e 554d 5041 445f 375a  FT_ALT_NUMPAD_7Z
+00003a10: 1743 5452 4c5f 5348 4946 545f 414c 545f  .CTRL_SHIFT_ALT_
+00003a20: 4e55 4d50 4144 5f38 5a17 4354 524c 5f53  NUMPAD_8Z.CTRL_S
+00003a30: 4849 4654 5f41 4c54 5f4e 554d 5041 445f  HIFT_ALT_NUMPAD_
+00003a40: 395a 1743 5452 4c5f 5348 4946 545f 414c  9Z.CTRL_SHIFT_AL
+00003a50: 545f 4e55 4d50 4144 5f30 5a1f 4354 524c  T_NUMPAD_0Z.CTRL
+00003a60: 5f53 4849 4654 5f41 4c54 5f4e 554d 5041  _SHIFT_ALT_NUMPA
+00003a70: 445f 3131 5f44 4956 4944 455a 2143 5452  D_11_DIVIDEZ!CTR
+00003a80: 4c5f 5348 4946 545f 414c 545f 4e55 4d50  L_SHIFT_ALT_NUMP
+00003a90: 4144 5f31 325f 4d55 4c54 4950 4c59 5a10  AD_12_MULTIPLYZ.
+00003aa0: 4354 524c 5f53 4849 4654 5f41 4c54 5f41  CTRL_SHIFT_ALT_A
+00003ab0: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
+00003ac0: 5f42 5a10 4354 524c 5f53 4849 4654 5f41  _BZ.CTRL_SHIFT_A
+00003ad0: 4c54 5f43 5a10 4354 524c 5f53 4849 4654  LT_CZ.CTRL_SHIFT
+00003ae0: 5f41 4c54 5f44 5a10 4354 524c 5f53 4849  _ALT_DZ.CTRL_SHI
+00003af0: 4654 5f41 4c54 5f45 5a10 4354 524c 5f53  FT_ALT_EZ.CTRL_S
+00003b00: 4849 4654 5f41 4c54 5f46 5a10 4354 524c  HIFT_ALT_FZ.CTRL
+00003b10: 5f53 4849 4654 5f41 4c54 5f47 5a10 4354  _SHIFT_ALT_GZ.CT
+00003b20: 524c 5f53 4849 4654 5f41 4c54 5f48 5a10  RL_SHIFT_ALT_HZ.
+00003b30: 4354 524c 5f53 4849 4654 5f41 4c54 5f49  CTRL_SHIFT_ALT_I
+00003b40: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
+00003b50: 5f4a 5a10 4354 524c 5f53 4849 4654 5f41  _JZ.CTRL_SHIFT_A
+00003b60: 4c54 5f4b 5a10 4354 524c 5f53 4849 4654  LT_KZ.CTRL_SHIFT
+00003b70: 5f41 4c54 5f4c 5a10 4354 524c 5f53 4849  _ALT_LZ.CTRL_SHI
+00003b80: 4654 5f41 4c54 5f4d 5a10 4354 524c 5f53  FT_ALT_MZ.CTRL_S
+00003b90: 4849 4654 5f41 4c54 5f4e 5a10 4354 524c  HIFT_ALT_NZ.CTRL
+00003ba0: 5f53 4849 4654 5f41 4c54 5f4f 5a10 4354  _SHIFT_ALT_OZ.CT
+00003bb0: 524c 5f53 4849 4654 5f41 4c54 5f50 5a10  RL_SHIFT_ALT_PZ.
+00003bc0: 4354 524c 5f53 4849 4654 5f41 4c54 5f51  CTRL_SHIFT_ALT_Q
+00003bd0: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
+00003be0: 5f52 5a10 4354 524c 5f53 4849 4654 5f41  _RZ.CTRL_SHIFT_A
+00003bf0: 4c54 5f53 5a10 4354 524c 5f53 4849 4654  LT_SZ.CTRL_SHIFT
+00003c00: 5f41 4c54 5f54 5a10 4354 524c 5f53 4849  _ALT_TZ.CTRL_SHI
+00003c10: 4654 5f41 4c54 5f55 5a10 4354 524c 5f53  FT_ALT_UZ.CTRL_S
+00003c20: 4849 4654 5f41 4c54 5f56 5a10 4354 524c  HIFT_ALT_VZ.CTRL
+00003c30: 5f53 4849 4654 5f41 4c54 5f57 5a10 4354  _SHIFT_ALT_WZ.CT
+00003c40: 524c 5f53 4849 4654 5f41 4c54 5f58 5a10  RL_SHIFT_ALT_XZ.
+00003c50: 4354 524c 5f53 4849 4654 5f41 4c54 5f59  CTRL_SHIFT_ALT_Y
+00003c60: 5a10 4354 524c 5f53 4849 4654 5f41 4c54  Z.CTRL_SHIFT_ALT
+00003c70: 5f5a 7240 0000 0072 4000 0000 7240 0000  _Zr@...r@...r@..
+00003c80: 0072 4100 0000 da08 3c6d 6f64 756c 653e  .rA.....<module>
+00003c90: 0300 0000 73e6 0400 0004 1104 0104 0504  ....s...........
+00003ca0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003cb0: 0104 0104 0104 0504 0104 0104 0104 0104  ................
+00003cc0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003cd0: 0104 0504 0104 0104 0104 0104 0204 0104  ................
+00003ce0: 0104 0104 0104 0104 0204 0204 0104 0504  ................
+00003cf0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003d00: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003d10: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003d20: 0104 0504 0104 0104 0104 0104 0104 0104  ................
+00003d30: 0104 0104 0504 0104 0104 0104 0104 0104  ................
+00003d40: 0204 0104 0104 0104 0504 0204 0104 0104  ................
+00003d50: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00003d60: 0104 0204 0104 0104 0104 0204 0104 0104  ................
+00003d70: 0104 0104 0104 0104 0104 0104 0204 0504  ................
+00003d80: 0104 0104 0104 0104 0602 0102 0102 0102  ................
+00003d90: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00003da0: f404 1002 0102 0102 0102 0102 0102 fa04  ................
+00003db0: 0a02 0102 0102 0102 0102 0102 0102 0102  ................
+00003dc0: 0102 0102 0102 0102 f404 1002 0102 0102  ................
+00003dd0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00003de0: 0102 f404 1310 0410 0410 0710 0410 0410  ................
+00003df0: 0710 0710 0410 0410 0710 0b08 0208 0108  ................
+00003e00: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003e10: 0108 0108 0208 0108 0108 0108 0108 0108  ................
+00003e20: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003e30: 0208 0108 0108 0108 0108 0108 0108 0108  ................
+00003e40: 0108 0108 0108 0108 0208 0108 0108 0108  ................
+00003e50: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003e60: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003e70: 0108 0108 0108 0108 0108 0108 0308 0208  ................
+00003e80: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003e90: 0108 0108 0108 0208 0108 0108 0108 0108  ................
+00003ea0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003eb0: 0108 0208 0108 0108 0108 0108 0108 0108  ................
+00003ec0: 0108 0108 0108 0108 0108 0208 0108 0108  ................
+00003ed0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003ee0: 0108 0108 0108 0108 0108 010a 010a 010a  ................
+00003ef0: 010a 010a 010a 010a 010a 010a 010a 030a  ................
+00003f00: 020a 010a 010a 010a 010a 010a 010a 010a  ................
+00003f10: 010a 010a 010a 010a 020a 010a 010a 010a  ................
+00003f20: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003f30: 010a 010a 020a 010a 010a 010a 010a 010a  ................
+00003f40: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00003f50: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003f60: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003f70: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003f80: 030a 010a 010a 010a 010a 010a 010a 010a  ................
+00003f90: 010a 010a 010a 010a 020a 010a 010a 010a  ................
+00003fa0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003fb0: 010a 010a 020a 010a 010a 010a 010a 010a  ................
+00003fc0: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00003fd0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003fe0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003ff0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00004000: 030a 010a 010a 010a 010a 010a 010a 010a  ................
+00004010: 010a 010a 010a 010a 020a 010a 010a 010a  ................
+00004020: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00004030: 010a 010a 020a 010a 010a 010a 010a 010a  ................
+00004040: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00004050: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00004060: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00004070: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004080: 010a 010a 020a 010a 010a 010a 010a 010a  ................
-00004090: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00004080: 030a 010a 010a 010a 010a 010a 010a 010a  ................
+00004090: 010a 010a 010a 010a 020a 010a 010a 010a  ................
 000040a0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000040b0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000040c0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000040d0: 030a 010a 010a 010a 010a 010a 010a 010a  ................
-000040e0: 010a 010a 010a 010a 020a 010a 010a 010a  ................
+000040b0: 010a 010a 020a 010a 010a 010a 010a 010a  ................
+000040c0: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+000040d0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+000040e0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 000040f0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004100: 010a 010a 020a 010a 010a 010a 010a 010a  ................
-00004110: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00004100: 030a 010a 010a 010a 010a 010a 010a 010a  ................
+00004110: 010a 010a 010a 010a 020a 010a 010a 010a  ................
 00004120: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004130: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004140: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004150: 030a 010a 010a 010a 010a 010a 010a 010a  ................
-00004160: 010a 010a 010a 010a 020a 010a 010a 010a  ................
-00004170: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004180: 010a 010a 020a 010a 010a 010a 010a 010a  ................
-00004190: 010a 010a 010a 010a 010a 010a 020a 010a  ................
-000041a0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000041b0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000041c0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000041d0: 030a 010a 010a 010a 010a 010a 010a 010a  ................
-000041e0: 010a 010a 010a 010a 020a 010a 010a 010a  ................
-000041f0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004200: 010a 010a 020a 010a 010a 010a 010a 010a  ................
-00004210: 010a 010a 010a 010a 010a 010a 020a 010a  ................
-00004220: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004230: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004240: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004250: 030a 010a 010a 010a 010a 010a 010a 010a  ................
-00004260: 010a 010a 010a 010a 020a 010a 010a 010a  ................
-00004270: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00004280: 010a 010a 020a 010a 010a 010a 010a 010a  ................
-00004290: 010a 010a 010a 010a 010a 010a 020a 010a  ................
-000042a0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000042b0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000042c0: 010a 010a 010a 010a 010a 010a 010a 01    ...............
+00004130: 010a 010a 020a 010a 010a 010a 010a 010a  ................
+00004140: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00004150: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00004160: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00004170: 010a 010a 010a 010a 010a 010a 010a 01    ...............
```

### Comparing `hotkeynet-0.1.3/hotkeynet/__pycache__/maker.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/__pycache__/maker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/__pycache__/script.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/__pycache__/script.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/__pycache__/utils.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/api.py` & `hotkeynet-0.1.4/hotkeynet/api.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/canned.py` & `hotkeynet-0.1.4/hotkeynet/canned.py`

 * *Files 15% similar despite different names*

```diff
@@ -336,26 +336,26 @@
 CTRL_F8 = CTRL_(_KN.F8)
 CTRL_F9 = CTRL_(_KN.F9)
 CTRL_F10 = CTRL_(_KN.F10)
 CTRL_F11 = CTRL_(_KN.F11)
 CTRL_F12 = CTRL_(_KN.F12)
 
 CTRL_OEM3_WAVE_OR_BACK_QUOTE = CTRL_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_KEY_1 = CTRL_(_KN.KEY_1)
-CTRL_KEY_2 = CTRL_(_KN.KEY_2)
-CTRL_KEY_3 = CTRL_(_KN.KEY_3)
-CTRL_KEY_4 = CTRL_(_KN.KEY_4)
-CTRL_KEY_5 = CTRL_(_KN.KEY_5)
-CTRL_KEY_6 = CTRL_(_KN.KEY_6)
-CTRL_KEY_7 = CTRL_(_KN.KEY_7)
-CTRL_KEY_8 = CTRL_(_KN.KEY_8)
-CTRL_KEY_9 = CTRL_(_KN.KEY_9)
-CTRL_KEY_0 = CTRL_(_KN.KEY_0)
-CTRL_KEY_11_MINUS = CTRL_(_KN.KEY_11_MINUS)
-CTRL_KEY_12_PLUS = CTRL_(_KN.KEY_12_PLUS)
+CTRL_1 = CTRL_(_KN.KEY_1)
+CTRL_2 = CTRL_(_KN.KEY_2)
+CTRL_3 = CTRL_(_KN.KEY_3)
+CTRL_4 = CTRL_(_KN.KEY_4)
+CTRL_5 = CTRL_(_KN.KEY_5)
+CTRL_6 = CTRL_(_KN.KEY_6)
+CTRL_7 = CTRL_(_KN.KEY_7)
+CTRL_8 = CTRL_(_KN.KEY_8)
+CTRL_9 = CTRL_(_KN.KEY_9)
+CTRL_0 = CTRL_(_KN.KEY_0)
+CTRL_11_MINUS = CTRL_(_KN.KEY_11_MINUS)
+CTRL_12_PLUS = CTRL_(_KN.KEY_12_PLUS)
 CTRL_BACKSPACE = CTRL_(_KN.BACKSPACE)
 
 CTRL_NUMPAD_1 = CTRL_(_KN.NUMPAD_1)
 CTRL_NUMPAD_2 = CTRL_(_KN.NUMPAD_2)
 CTRL_NUMPAD_3 = CTRL_(_KN.NUMPAD_3)
 CTRL_NUMPAD_4 = CTRL_(_KN.NUMPAD_4)
 CTRL_NUMPAD_5 = CTRL_(_KN.NUMPAD_5)
@@ -407,26 +407,26 @@
 SHIFT_F8 = SHIFT_(_KN.F8)
 SHIFT_F9 = SHIFT_(_KN.F9)
 SHIFT_F10 = SHIFT_(_KN.F10)
 SHIFT_F11 = SHIFT_(_KN.F11)
 SHIFT_F12 = SHIFT_(_KN.F12)
 
 SHIFT_OEM3_WAVE_OR_BACK_QUOTE = SHIFT_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-SHIFT_KEY_1 = SHIFT_(_KN.KEY_1)
-SHIFT_KEY_2 = SHIFT_(_KN.KEY_2)
-SHIFT_KEY_3 = SHIFT_(_KN.KEY_3)
-SHIFT_KEY_4 = SHIFT_(_KN.KEY_4)
-SHIFT_KEY_5 = SHIFT_(_KN.KEY_5)
-SHIFT_KEY_6 = SHIFT_(_KN.KEY_6)
-SHIFT_KEY_7 = SHIFT_(_KN.KEY_7)
-SHIFT_KEY_8 = SHIFT_(_KN.KEY_8)
-SHIFT_KEY_9 = SHIFT_(_KN.KEY_9)
-SHIFT_KEY_0 = SHIFT_(_KN.KEY_0)
-SHIFT_KEY_11_MINUS = SHIFT_(_KN.KEY_11_MINUS)
-SHIFT_KEY_12_PLUS = SHIFT_(_KN.KEY_12_PLUS)
+SHIFT_1 = SHIFT_(_KN.KEY_1)
+SHIFT_2 = SHIFT_(_KN.KEY_2)
+SHIFT_3 = SHIFT_(_KN.KEY_3)
+SHIFT_4 = SHIFT_(_KN.KEY_4)
+SHIFT_5 = SHIFT_(_KN.KEY_5)
+SHIFT_6 = SHIFT_(_KN.KEY_6)
+SHIFT_7 = SHIFT_(_KN.KEY_7)
+SHIFT_8 = SHIFT_(_KN.KEY_8)
+SHIFT_9 = SHIFT_(_KN.KEY_9)
+SHIFT_0 = SHIFT_(_KN.KEY_0)
+SHIFT_11_MINUS = SHIFT_(_KN.KEY_11_MINUS)
+SHIFT_12_PLUS = SHIFT_(_KN.KEY_12_PLUS)
 SHIFT_BACKSPACE = SHIFT_(_KN.BACKSPACE)
 
 SHIFT_NUMPAD_1 = SHIFT_(_KN.NUMPAD_1)
 SHIFT_NUMPAD_2 = SHIFT_(_KN.NUMPAD_2)
 SHIFT_NUMPAD_3 = SHIFT_(_KN.NUMPAD_3)
 SHIFT_NUMPAD_4 = SHIFT_(_KN.NUMPAD_4)
 SHIFT_NUMPAD_5 = SHIFT_(_KN.NUMPAD_5)
@@ -478,26 +478,26 @@
 ALT_F8 = ALT_(_KN.F8)
 ALT_F9 = ALT_(_KN.F9)
 ALT_F10 = ALT_(_KN.F10)
 ALT_F11 = ALT_(_KN.F11)
 ALT_F12 = ALT_(_KN.F12)
 
 ALT_OEM3_WAVE_OR_BACK_QUOTE = ALT_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-ALT_KEY_1 = ALT_(_KN.KEY_1)
-ALT_KEY_2 = ALT_(_KN.KEY_2)
-ALT_KEY_3 = ALT_(_KN.KEY_3)
-ALT_KEY_4 = ALT_(_KN.KEY_4)
-ALT_KEY_5 = ALT_(_KN.KEY_5)
-ALT_KEY_6 = ALT_(_KN.KEY_6)
-ALT_KEY_7 = ALT_(_KN.KEY_7)
-ALT_KEY_8 = ALT_(_KN.KEY_8)
-ALT_KEY_9 = ALT_(_KN.KEY_9)
-ALT_KEY_0 = ALT_(_KN.KEY_0)
-ALT_KEY_11_MINUS = ALT_(_KN.KEY_11_MINUS)
-ALT_KEY_12_PLUS = ALT_(_KN.KEY_12_PLUS)
+ALT_1 = ALT_(_KN.KEY_1)
+ALT_2 = ALT_(_KN.KEY_2)
+ALT_3 = ALT_(_KN.KEY_3)
+ALT_4 = ALT_(_KN.KEY_4)
+ALT_5 = ALT_(_KN.KEY_5)
+ALT_6 = ALT_(_KN.KEY_6)
+ALT_7 = ALT_(_KN.KEY_7)
+ALT_8 = ALT_(_KN.KEY_8)
+ALT_9 = ALT_(_KN.KEY_9)
+ALT_0 = ALT_(_KN.KEY_0)
+ALT_11_MINUS = ALT_(_KN.KEY_11_MINUS)
+ALT_12_PLUS = ALT_(_KN.KEY_12_PLUS)
 ALT_BACKSPACE = ALT_(_KN.BACKSPACE)
 
 ALT_NUMPAD_1 = ALT_(_KN.NUMPAD_1)
 ALT_NUMPAD_2 = ALT_(_KN.NUMPAD_2)
 ALT_NUMPAD_3 = ALT_(_KN.NUMPAD_3)
 ALT_NUMPAD_4 = ALT_(_KN.NUMPAD_4)
 ALT_NUMPAD_5 = ALT_(_KN.NUMPAD_5)
@@ -547,26 +547,26 @@
 CTRL_ALT_F8 = CTRL_ALT_(_KN.F8)
 CTRL_ALT_F9 = CTRL_ALT_(_KN.F9)
 CTRL_ALT_F10 = CTRL_ALT_(_KN.F10)
 CTRL_ALT_F11 = CTRL_ALT_(_KN.F11)
 CTRL_ALT_F12 = CTRL_ALT_(_KN.F12)
 
 CTRL_ALT_OEM3_WAVE_OR_BACK_QUOTE = CTRL_ALT_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_ALT_KEY_1 = CTRL_ALT_(_KN.KEY_1)
-CTRL_ALT_KEY_2 = CTRL_ALT_(_KN.KEY_2)
-CTRL_ALT_KEY_3 = CTRL_ALT_(_KN.KEY_3)
-CTRL_ALT_KEY_4 = CTRL_ALT_(_KN.KEY_4)
-CTRL_ALT_KEY_5 = CTRL_ALT_(_KN.KEY_5)
-CTRL_ALT_KEY_6 = CTRL_ALT_(_KN.KEY_6)
-CTRL_ALT_KEY_7 = CTRL_ALT_(_KN.KEY_7)
-CTRL_ALT_KEY_8 = CTRL_ALT_(_KN.KEY_8)
-CTRL_ALT_KEY_9 = CTRL_ALT_(_KN.KEY_9)
-CTRL_ALT_KEY_0 = CTRL_ALT_(_KN.KEY_0)
-CTRL_ALT_KEY_11_MINUS = CTRL_ALT_(_KN.KEY_11_MINUS)
-CTRL_ALT_KEY_12_PLUS = CTRL_ALT_(_KN.KEY_12_PLUS)
+CTRL_ALT_1 = CTRL_ALT_(_KN.KEY_1)
+CTRL_ALT_2 = CTRL_ALT_(_KN.KEY_2)
+CTRL_ALT_3 = CTRL_ALT_(_KN.KEY_3)
+CTRL_ALT_4 = CTRL_ALT_(_KN.KEY_4)
+CTRL_ALT_5 = CTRL_ALT_(_KN.KEY_5)
+CTRL_ALT_6 = CTRL_ALT_(_KN.KEY_6)
+CTRL_ALT_7 = CTRL_ALT_(_KN.KEY_7)
+CTRL_ALT_8 = CTRL_ALT_(_KN.KEY_8)
+CTRL_ALT_9 = CTRL_ALT_(_KN.KEY_9)
+CTRL_ALT_0 = CTRL_ALT_(_KN.KEY_0)
+CTRL_ALT_11_MINUS = CTRL_ALT_(_KN.KEY_11_MINUS)
+CTRL_ALT_12_PLUS = CTRL_ALT_(_KN.KEY_12_PLUS)
 CTRL_ALT_BACKSPACE = CTRL_ALT_(_KN.BACKSPACE)
 
 CTRL_ALT_NUMPAD_1 = CTRL_ALT_(_KN.NUMPAD_1)
 CTRL_ALT_NUMPAD_2 = CTRL_ALT_(_KN.NUMPAD_2)
 CTRL_ALT_NUMPAD_3 = CTRL_ALT_(_KN.NUMPAD_3)
 CTRL_ALT_NUMPAD_4 = CTRL_ALT_(_KN.NUMPAD_4)
 CTRL_ALT_NUMPAD_5 = CTRL_ALT_(_KN.NUMPAD_5)
@@ -616,26 +616,26 @@
 CTRL_SHIFT_F8 = CTRL_SHIFT_(_KN.F8)
 CTRL_SHIFT_F9 = CTRL_SHIFT_(_KN.F9)
 CTRL_SHIFT_F10 = CTRL_SHIFT_(_KN.F10)
 CTRL_SHIFT_F11 = CTRL_SHIFT_(_KN.F11)
 CTRL_SHIFT_F12 = CTRL_SHIFT_(_KN.F12)
 
 CTRL_SHIFT_OEM3_WAVE_OR_BACK_QUOTE = CTRL_SHIFT_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_SHIFT_KEY_1 = CTRL_SHIFT_(_KN.KEY_1)
-CTRL_SHIFT_KEY_2 = CTRL_SHIFT_(_KN.KEY_2)
-CTRL_SHIFT_KEY_3 = CTRL_SHIFT_(_KN.KEY_3)
-CTRL_SHIFT_KEY_4 = CTRL_SHIFT_(_KN.KEY_4)
-CTRL_SHIFT_KEY_5 = CTRL_SHIFT_(_KN.KEY_5)
-CTRL_SHIFT_KEY_6 = CTRL_SHIFT_(_KN.KEY_6)
-CTRL_SHIFT_KEY_7 = CTRL_SHIFT_(_KN.KEY_7)
-CTRL_SHIFT_KEY_8 = CTRL_SHIFT_(_KN.KEY_8)
-CTRL_SHIFT_KEY_9 = CTRL_SHIFT_(_KN.KEY_9)
-CTRL_SHIFT_KEY_0 = CTRL_SHIFT_(_KN.KEY_0)
-CTRL_SHIFT_KEY_11_MINUS = CTRL_SHIFT_(_KN.KEY_11_MINUS)
-CTRL_SHIFT_KEY_12_PLUS = CTRL_SHIFT_(_KN.KEY_12_PLUS)
+CTRL_SHIFT_1 = CTRL_SHIFT_(_KN.KEY_1)
+CTRL_SHIFT_2 = CTRL_SHIFT_(_KN.KEY_2)
+CTRL_SHIFT_3 = CTRL_SHIFT_(_KN.KEY_3)
+CTRL_SHIFT_4 = CTRL_SHIFT_(_KN.KEY_4)
+CTRL_SHIFT_5 = CTRL_SHIFT_(_KN.KEY_5)
+CTRL_SHIFT_6 = CTRL_SHIFT_(_KN.KEY_6)
+CTRL_SHIFT_7 = CTRL_SHIFT_(_KN.KEY_7)
+CTRL_SHIFT_8 = CTRL_SHIFT_(_KN.KEY_8)
+CTRL_SHIFT_9 = CTRL_SHIFT_(_KN.KEY_9)
+CTRL_SHIFT_0 = CTRL_SHIFT_(_KN.KEY_0)
+CTRL_SHIFT_11_MINUS = CTRL_SHIFT_(_KN.KEY_11_MINUS)
+CTRL_SHIFT_12_PLUS = CTRL_SHIFT_(_KN.KEY_12_PLUS)
 CTRL_SHIFT_BACKSPACE = CTRL_SHIFT_(_KN.BACKSPACE)
 
 CTRL_SHIFT_NUMPAD_1 = CTRL_SHIFT_(_KN.NUMPAD_1)
 CTRL_SHIFT_NUMPAD_2 = CTRL_SHIFT_(_KN.NUMPAD_2)
 CTRL_SHIFT_NUMPAD_3 = CTRL_SHIFT_(_KN.NUMPAD_3)
 CTRL_SHIFT_NUMPAD_4 = CTRL_SHIFT_(_KN.NUMPAD_4)
 CTRL_SHIFT_NUMPAD_5 = CTRL_SHIFT_(_KN.NUMPAD_5)
@@ -685,26 +685,26 @@
 ALT_SHIFT_F8 = ALT_SHIFT_(_KN.F8)
 ALT_SHIFT_F9 = ALT_SHIFT_(_KN.F9)
 ALT_SHIFT_F10 = ALT_SHIFT_(_KN.F10)
 ALT_SHIFT_F11 = ALT_SHIFT_(_KN.F11)
 ALT_SHIFT_F12 = ALT_SHIFT_(_KN.F12)
 
 ALT_SHIFT_OEM3_WAVE_OR_BACK_QUOTE = ALT_SHIFT_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-ALT_SHIFT_KEY_1 = ALT_SHIFT_(_KN.KEY_1)
-ALT_SHIFT_KEY_2 = ALT_SHIFT_(_KN.KEY_2)
-ALT_SHIFT_KEY_3 = ALT_SHIFT_(_KN.KEY_3)
-ALT_SHIFT_KEY_4 = ALT_SHIFT_(_KN.KEY_4)
-ALT_SHIFT_KEY_5 = ALT_SHIFT_(_KN.KEY_5)
-ALT_SHIFT_KEY_6 = ALT_SHIFT_(_KN.KEY_6)
-ALT_SHIFT_KEY_7 = ALT_SHIFT_(_KN.KEY_7)
-ALT_SHIFT_KEY_8 = ALT_SHIFT_(_KN.KEY_8)
-ALT_SHIFT_KEY_9 = ALT_SHIFT_(_KN.KEY_9)
-ALT_SHIFT_KEY_0 = ALT_SHIFT_(_KN.KEY_0)
-ALT_SHIFT_KEY_11_MINUS = ALT_SHIFT_(_KN.KEY_11_MINUS)
-ALT_SHIFT_KEY_12_PLUS = ALT_SHIFT_(_KN.KEY_12_PLUS)
+ALT_SHIFT_1 = ALT_SHIFT_(_KN.KEY_1)
+ALT_SHIFT_2 = ALT_SHIFT_(_KN.KEY_2)
+ALT_SHIFT_3 = ALT_SHIFT_(_KN.KEY_3)
+ALT_SHIFT_4 = ALT_SHIFT_(_KN.KEY_4)
+ALT_SHIFT_5 = ALT_SHIFT_(_KN.KEY_5)
+ALT_SHIFT_6 = ALT_SHIFT_(_KN.KEY_6)
+ALT_SHIFT_7 = ALT_SHIFT_(_KN.KEY_7)
+ALT_SHIFT_8 = ALT_SHIFT_(_KN.KEY_8)
+ALT_SHIFT_9 = ALT_SHIFT_(_KN.KEY_9)
+ALT_SHIFT_0 = ALT_SHIFT_(_KN.KEY_0)
+ALT_SHIFT_11_MINUS = ALT_SHIFT_(_KN.KEY_11_MINUS)
+ALT_SHIFT_12_PLUS = ALT_SHIFT_(_KN.KEY_12_PLUS)
 ALT_SHIFT_BACKSPACE = ALT_SHIFT_(_KN.BACKSPACE)
 
 ALT_SHIFT_NUMPAD_1 = ALT_SHIFT_(_KN.NUMPAD_1)
 ALT_SHIFT_NUMPAD_2 = ALT_SHIFT_(_KN.NUMPAD_2)
 ALT_SHIFT_NUMPAD_3 = ALT_SHIFT_(_KN.NUMPAD_3)
 ALT_SHIFT_NUMPAD_4 = ALT_SHIFT_(_KN.NUMPAD_4)
 ALT_SHIFT_NUMPAD_5 = ALT_SHIFT_(_KN.NUMPAD_5)
@@ -754,26 +754,26 @@
 CTRL_SHIFT_ALT_F8 = CTRL_SHIFT_ALT_(_KN.F8)
 CTRL_SHIFT_ALT_F9 = CTRL_SHIFT_ALT_(_KN.F9)
 CTRL_SHIFT_ALT_F10 = CTRL_SHIFT_ALT_(_KN.F10)
 CTRL_SHIFT_ALT_F11 = CTRL_SHIFT_ALT_(_KN.F11)
 CTRL_SHIFT_ALT_F12 = CTRL_SHIFT_ALT_(_KN.F12)
 
 CTRL_SHIFT_ALT_OEM3_WAVE_OR_BACK_QUOTE = CTRL_SHIFT_ALT_(_KN.OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_SHIFT_ALT_KEY_1 = CTRL_SHIFT_ALT_(_KN.KEY_1)
-CTRL_SHIFT_ALT_KEY_2 = CTRL_SHIFT_ALT_(_KN.KEY_2)
-CTRL_SHIFT_ALT_KEY_3 = CTRL_SHIFT_ALT_(_KN.KEY_3)
-CTRL_SHIFT_ALT_KEY_4 = CTRL_SHIFT_ALT_(_KN.KEY_4)
-CTRL_SHIFT_ALT_KEY_5 = CTRL_SHIFT_ALT_(_KN.KEY_5)
-CTRL_SHIFT_ALT_KEY_6 = CTRL_SHIFT_ALT_(_KN.KEY_6)
-CTRL_SHIFT_ALT_KEY_7 = CTRL_SHIFT_ALT_(_KN.KEY_7)
-CTRL_SHIFT_ALT_KEY_8 = CTRL_SHIFT_ALT_(_KN.KEY_8)
-CTRL_SHIFT_ALT_KEY_9 = CTRL_SHIFT_ALT_(_KN.KEY_9)
-CTRL_SHIFT_ALT_KEY_0 = CTRL_SHIFT_ALT_(_KN.KEY_0)
-CTRL_SHIFT_ALT_KEY_11_MINUS = CTRL_SHIFT_ALT_(_KN.KEY_11_MINUS)
-CTRL_SHIFT_ALT_KEY_12_PLUS = CTRL_SHIFT_ALT_(_KN.KEY_12_PLUS)
+CTRL_SHIFT_ALT_1 = CTRL_SHIFT_ALT_(_KN.KEY_1)
+CTRL_SHIFT_ALT_2 = CTRL_SHIFT_ALT_(_KN.KEY_2)
+CTRL_SHIFT_ALT_3 = CTRL_SHIFT_ALT_(_KN.KEY_3)
+CTRL_SHIFT_ALT_4 = CTRL_SHIFT_ALT_(_KN.KEY_4)
+CTRL_SHIFT_ALT_5 = CTRL_SHIFT_ALT_(_KN.KEY_5)
+CTRL_SHIFT_ALT_6 = CTRL_SHIFT_ALT_(_KN.KEY_6)
+CTRL_SHIFT_ALT_7 = CTRL_SHIFT_ALT_(_KN.KEY_7)
+CTRL_SHIFT_ALT_8 = CTRL_SHIFT_ALT_(_KN.KEY_8)
+CTRL_SHIFT_ALT_9 = CTRL_SHIFT_ALT_(_KN.KEY_9)
+CTRL_SHIFT_ALT_0 = CTRL_SHIFT_ALT_(_KN.KEY_0)
+CTRL_SHIFT_ALT_11_MINUS = CTRL_SHIFT_ALT_(_KN.KEY_11_MINUS)
+CTRL_SHIFT_ALT_12_PLUS = CTRL_SHIFT_ALT_(_KN.KEY_12_PLUS)
 CTRL_SHIFT_ALT_BACKSPACE = CTRL_SHIFT_ALT_(_KN.BACKSPACE)
 
 CTRL_SHIFT_ALT_NUMPAD_1 = CTRL_SHIFT_ALT_(_KN.NUMPAD_1)
 CTRL_SHIFT_ALT_NUMPAD_2 = CTRL_SHIFT_ALT_(_KN.NUMPAD_2)
 CTRL_SHIFT_ALT_NUMPAD_3 = CTRL_SHIFT_ALT_(_KN.NUMPAD_3)
 CTRL_SHIFT_ALT_NUMPAD_4 = CTRL_SHIFT_ALT_(_KN.NUMPAD_4)
 CTRL_SHIFT_ALT_NUMPAD_5 = CTRL_SHIFT_ALT_(_KN.NUMPAD_5)
```

### Comparing `hotkeynet-0.1.3/hotkeynet/keyname.py` & `hotkeynet-0.1.4/hotkeynet/keyname.py`

 * *Files 3% similar despite different names*

```diff
@@ -313,26 +313,26 @@
 CTRL_F8 = CTRL_(F8)
 CTRL_F9 = CTRL_(F9)
 CTRL_F10 = CTRL_(F10)
 CTRL_F11 = CTRL_(F11)
 CTRL_F12 = CTRL_(F12)
 
 CTRL_OEM3_WAVE_OR_BACK_QUOTE = CTRL_(OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_KEY_1 = CTRL_(KEY_1)
-CTRL_KEY_2 = CTRL_(KEY_2)
-CTRL_KEY_3 = CTRL_(KEY_3)
-CTRL_KEY_4 = CTRL_(KEY_4)
-CTRL_KEY_5 = CTRL_(KEY_5)
-CTRL_KEY_6 = CTRL_(KEY_6)
-CTRL_KEY_7 = CTRL_(KEY_7)
-CTRL_KEY_8 = CTRL_(KEY_8)
-CTRL_KEY_9 = CTRL_(KEY_9)
-CTRL_KEY_0 = CTRL_(KEY_0)
-CTRL_KEY_11_MINUS = CTRL_(KEY_11_MINUS)
-CTRL_KEY_12_PLUS = CTRL_(KEY_12_PLUS)
+CTRL_1 = CTRL_(KEY_1)
+CTRL_2 = CTRL_(KEY_2)
+CTRL_3 = CTRL_(KEY_3)
+CTRL_4 = CTRL_(KEY_4)
+CTRL_5 = CTRL_(KEY_5)
+CTRL_6 = CTRL_(KEY_6)
+CTRL_7 = CTRL_(KEY_7)
+CTRL_8 = CTRL_(KEY_8)
+CTRL_9 = CTRL_(KEY_9)
+CTRL_0 = CTRL_(KEY_0)
+CTRL_11_MINUS = CTRL_(KEY_11_MINUS)
+CTRL_12_PLUS = CTRL_(KEY_12_PLUS)
 CTRL_BACKSPACE = CTRL_(BACKSPACE)
 
 CTRL_NUMPAD_1 = CTRL_(NUMPAD_1)
 CTRL_NUMPAD_2 = CTRL_(NUMPAD_2)
 CTRL_NUMPAD_3 = CTRL_(NUMPAD_3)
 CTRL_NUMPAD_4 = CTRL_(NUMPAD_4)
 CTRL_NUMPAD_5 = CTRL_(NUMPAD_5)
@@ -384,26 +384,26 @@
 SHIFT_F8 = SHIFT_(F8)
 SHIFT_F9 = SHIFT_(F9)
 SHIFT_F10 = SHIFT_(F10)
 SHIFT_F11 = SHIFT_(F11)
 SHIFT_F12 = SHIFT_(F12)
 
 SHIFT_OEM3_WAVE_OR_BACK_QUOTE = SHIFT_(OEM3_WAVE_OR_BACK_QUOTE)
-SHIFT_KEY_1 = SHIFT_(KEY_1)
-SHIFT_KEY_2 = SHIFT_(KEY_2)
-SHIFT_KEY_3 = SHIFT_(KEY_3)
-SHIFT_KEY_4 = SHIFT_(KEY_4)
-SHIFT_KEY_5 = SHIFT_(KEY_5)
-SHIFT_KEY_6 = SHIFT_(KEY_6)
-SHIFT_KEY_7 = SHIFT_(KEY_7)
-SHIFT_KEY_8 = SHIFT_(KEY_8)
-SHIFT_KEY_9 = SHIFT_(KEY_9)
-SHIFT_KEY_0 = SHIFT_(KEY_0)
-SHIFT_KEY_11_MINUS = SHIFT_(KEY_11_MINUS)
-SHIFT_KEY_12_PLUS = SHIFT_(KEY_12_PLUS)
+SHIFT_1 = SHIFT_(KEY_1)
+SHIFT_2 = SHIFT_(KEY_2)
+SHIFT_3 = SHIFT_(KEY_3)
+SHIFT_4 = SHIFT_(KEY_4)
+SHIFT_5 = SHIFT_(KEY_5)
+SHIFT_6 = SHIFT_(KEY_6)
+SHIFT_7 = SHIFT_(KEY_7)
+SHIFT_8 = SHIFT_(KEY_8)
+SHIFT_9 = SHIFT_(KEY_9)
+SHIFT_0 = SHIFT_(KEY_0)
+SHIFT_11_MINUS = SHIFT_(KEY_11_MINUS)
+SHIFT_12_PLUS = SHIFT_(KEY_12_PLUS)
 SHIFT_BACKSPACE = SHIFT_(BACKSPACE)
 
 SHIFT_NUMPAD_1 = SHIFT_(NUMPAD_1)
 SHIFT_NUMPAD_2 = SHIFT_(NUMPAD_2)
 SHIFT_NUMPAD_3 = SHIFT_(NUMPAD_3)
 SHIFT_NUMPAD_4 = SHIFT_(NUMPAD_4)
 SHIFT_NUMPAD_5 = SHIFT_(NUMPAD_5)
@@ -455,26 +455,26 @@
 ALT_F8 = ALT_(F8)
 ALT_F9 = ALT_(F9)
 ALT_F10 = ALT_(F10)
 ALT_F11 = ALT_(F11)
 ALT_F12 = ALT_(F12)
 
 ALT_OEM3_WAVE_OR_BACK_QUOTE = ALT_(OEM3_WAVE_OR_BACK_QUOTE)
-ALT_KEY_1 = ALT_(KEY_1)
-ALT_KEY_2 = ALT_(KEY_2)
-ALT_KEY_3 = ALT_(KEY_3)
-ALT_KEY_4 = ALT_(KEY_4)
-ALT_KEY_5 = ALT_(KEY_5)
-ALT_KEY_6 = ALT_(KEY_6)
-ALT_KEY_7 = ALT_(KEY_7)
-ALT_KEY_8 = ALT_(KEY_8)
-ALT_KEY_9 = ALT_(KEY_9)
-ALT_KEY_0 = ALT_(KEY_0)
-ALT_KEY_11_MINUS = ALT_(KEY_11_MINUS)
-ALT_KEY_12_PLUS = ALT_(KEY_12_PLUS)
+ALT_1 = ALT_(KEY_1)
+ALT_2 = ALT_(KEY_2)
+ALT_3 = ALT_(KEY_3)
+ALT_4 = ALT_(KEY_4)
+ALT_5 = ALT_(KEY_5)
+ALT_6 = ALT_(KEY_6)
+ALT_7 = ALT_(KEY_7)
+ALT_8 = ALT_(KEY_8)
+ALT_9 = ALT_(KEY_9)
+ALT_0 = ALT_(KEY_0)
+ALT_11_MINUS = ALT_(KEY_11_MINUS)
+ALT_12_PLUS = ALT_(KEY_12_PLUS)
 ALT_BACKSPACE = ALT_(BACKSPACE)
 
 ALT_NUMPAD_1 = ALT_(NUMPAD_1)
 ALT_NUMPAD_2 = ALT_(NUMPAD_2)
 ALT_NUMPAD_3 = ALT_(NUMPAD_3)
 ALT_NUMPAD_4 = ALT_(NUMPAD_4)
 ALT_NUMPAD_5 = ALT_(NUMPAD_5)
@@ -524,26 +524,26 @@
 CTRL_ALT_F8 = CTRL_ALT_(F8)
 CTRL_ALT_F9 = CTRL_ALT_(F9)
 CTRL_ALT_F10 = CTRL_ALT_(F10)
 CTRL_ALT_F11 = CTRL_ALT_(F11)
 CTRL_ALT_F12 = CTRL_ALT_(F12)
 
 CTRL_ALT_OEM3_WAVE_OR_BACK_QUOTE = CTRL_ALT_(OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_ALT_KEY_1 = CTRL_ALT_(KEY_1)
-CTRL_ALT_KEY_2 = CTRL_ALT_(KEY_2)
-CTRL_ALT_KEY_3 = CTRL_ALT_(KEY_3)
-CTRL_ALT_KEY_4 = CTRL_ALT_(KEY_4)
-CTRL_ALT_KEY_5 = CTRL_ALT_(KEY_5)
-CTRL_ALT_KEY_6 = CTRL_ALT_(KEY_6)
-CTRL_ALT_KEY_7 = CTRL_ALT_(KEY_7)
-CTRL_ALT_KEY_8 = CTRL_ALT_(KEY_8)
-CTRL_ALT_KEY_9 = CTRL_ALT_(KEY_9)
-CTRL_ALT_KEY_0 = CTRL_ALT_(KEY_0)
-CTRL_ALT_KEY_11_MINUS = CTRL_ALT_(KEY_11_MINUS)
-CTRL_ALT_KEY_12_PLUS = CTRL_ALT_(KEY_12_PLUS)
+CTRL_ALT_1 = CTRL_ALT_(KEY_1)
+CTRL_ALT_2 = CTRL_ALT_(KEY_2)
+CTRL_ALT_3 = CTRL_ALT_(KEY_3)
+CTRL_ALT_4 = CTRL_ALT_(KEY_4)
+CTRL_ALT_5 = CTRL_ALT_(KEY_5)
+CTRL_ALT_6 = CTRL_ALT_(KEY_6)
+CTRL_ALT_7 = CTRL_ALT_(KEY_7)
+CTRL_ALT_8 = CTRL_ALT_(KEY_8)
+CTRL_ALT_9 = CTRL_ALT_(KEY_9)
+CTRL_ALT_0 = CTRL_ALT_(KEY_0)
+CTRL_ALT_11_MINUS = CTRL_ALT_(KEY_11_MINUS)
+CTRL_ALT_12_PLUS = CTRL_ALT_(KEY_12_PLUS)
 CTRL_ALT_BACKSPACE = CTRL_ALT_(BACKSPACE)
 
 CTRL_ALT_NUMPAD_1 = CTRL_ALT_(NUMPAD_1)
 CTRL_ALT_NUMPAD_2 = CTRL_ALT_(NUMPAD_2)
 CTRL_ALT_NUMPAD_3 = CTRL_ALT_(NUMPAD_3)
 CTRL_ALT_NUMPAD_4 = CTRL_ALT_(NUMPAD_4)
 CTRL_ALT_NUMPAD_5 = CTRL_ALT_(NUMPAD_5)
@@ -593,26 +593,26 @@
 CTRL_SHIFT_F8 = CTRL_SHIFT_(F8)
 CTRL_SHIFT_F9 = CTRL_SHIFT_(F9)
 CTRL_SHIFT_F10 = CTRL_SHIFT_(F10)
 CTRL_SHIFT_F11 = CTRL_SHIFT_(F11)
 CTRL_SHIFT_F12 = CTRL_SHIFT_(F12)
 
 CTRL_SHIFT_OEM3_WAVE_OR_BACK_QUOTE = CTRL_SHIFT_(OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_SHIFT_KEY_1 = CTRL_SHIFT_(KEY_1)
-CTRL_SHIFT_KEY_2 = CTRL_SHIFT_(KEY_2)
-CTRL_SHIFT_KEY_3 = CTRL_SHIFT_(KEY_3)
-CTRL_SHIFT_KEY_4 = CTRL_SHIFT_(KEY_4)
-CTRL_SHIFT_KEY_5 = CTRL_SHIFT_(KEY_5)
-CTRL_SHIFT_KEY_6 = CTRL_SHIFT_(KEY_6)
-CTRL_SHIFT_KEY_7 = CTRL_SHIFT_(KEY_7)
-CTRL_SHIFT_KEY_8 = CTRL_SHIFT_(KEY_8)
-CTRL_SHIFT_KEY_9 = CTRL_SHIFT_(KEY_9)
-CTRL_SHIFT_KEY_0 = CTRL_SHIFT_(KEY_0)
-CTRL_SHIFT_KEY_11_MINUS = CTRL_SHIFT_(KEY_11_MINUS)
-CTRL_SHIFT_KEY_12_PLUS = CTRL_SHIFT_(KEY_12_PLUS)
+CTRL_SHIFT_1 = CTRL_SHIFT_(KEY_1)
+CTRL_SHIFT_2 = CTRL_SHIFT_(KEY_2)
+CTRL_SHIFT_3 = CTRL_SHIFT_(KEY_3)
+CTRL_SHIFT_4 = CTRL_SHIFT_(KEY_4)
+CTRL_SHIFT_5 = CTRL_SHIFT_(KEY_5)
+CTRL_SHIFT_6 = CTRL_SHIFT_(KEY_6)
+CTRL_SHIFT_7 = CTRL_SHIFT_(KEY_7)
+CTRL_SHIFT_8 = CTRL_SHIFT_(KEY_8)
+CTRL_SHIFT_9 = CTRL_SHIFT_(KEY_9)
+CTRL_SHIFT_0 = CTRL_SHIFT_(KEY_0)
+CTRL_SHIFT_11_MINUS = CTRL_SHIFT_(KEY_11_MINUS)
+CTRL_SHIFT_12_PLUS = CTRL_SHIFT_(KEY_12_PLUS)
 CTRL_SHIFT_BACKSPACE = CTRL_SHIFT_(BACKSPACE)
 
 CTRL_SHIFT_NUMPAD_1 = CTRL_SHIFT_(NUMPAD_1)
 CTRL_SHIFT_NUMPAD_2 = CTRL_SHIFT_(NUMPAD_2)
 CTRL_SHIFT_NUMPAD_3 = CTRL_SHIFT_(NUMPAD_3)
 CTRL_SHIFT_NUMPAD_4 = CTRL_SHIFT_(NUMPAD_4)
 CTRL_SHIFT_NUMPAD_5 = CTRL_SHIFT_(NUMPAD_5)
@@ -662,26 +662,26 @@
 ALT_SHIFT_F8 = ALT_SHIFT_(F8)
 ALT_SHIFT_F9 = ALT_SHIFT_(F9)
 ALT_SHIFT_F10 = ALT_SHIFT_(F10)
 ALT_SHIFT_F11 = ALT_SHIFT_(F11)
 ALT_SHIFT_F12 = ALT_SHIFT_(F12)
 
 ALT_SHIFT_OEM3_WAVE_OR_BACK_QUOTE = ALT_SHIFT_(OEM3_WAVE_OR_BACK_QUOTE)
-ALT_SHIFT_KEY_1 = ALT_SHIFT_(KEY_1)
-ALT_SHIFT_KEY_2 = ALT_SHIFT_(KEY_2)
-ALT_SHIFT_KEY_3 = ALT_SHIFT_(KEY_3)
-ALT_SHIFT_KEY_4 = ALT_SHIFT_(KEY_4)
-ALT_SHIFT_KEY_5 = ALT_SHIFT_(KEY_5)
-ALT_SHIFT_KEY_6 = ALT_SHIFT_(KEY_6)
-ALT_SHIFT_KEY_7 = ALT_SHIFT_(KEY_7)
-ALT_SHIFT_KEY_8 = ALT_SHIFT_(KEY_8)
-ALT_SHIFT_KEY_9 = ALT_SHIFT_(KEY_9)
-ALT_SHIFT_KEY_0 = ALT_SHIFT_(KEY_0)
-ALT_SHIFT_KEY_11_MINUS = ALT_SHIFT_(KEY_11_MINUS)
-ALT_SHIFT_KEY_12_PLUS = ALT_SHIFT_(KEY_12_PLUS)
+ALT_SHIFT_1 = ALT_SHIFT_(KEY_1)
+ALT_SHIFT_2 = ALT_SHIFT_(KEY_2)
+ALT_SHIFT_3 = ALT_SHIFT_(KEY_3)
+ALT_SHIFT_4 = ALT_SHIFT_(KEY_4)
+ALT_SHIFT_5 = ALT_SHIFT_(KEY_5)
+ALT_SHIFT_6 = ALT_SHIFT_(KEY_6)
+ALT_SHIFT_7 = ALT_SHIFT_(KEY_7)
+ALT_SHIFT_8 = ALT_SHIFT_(KEY_8)
+ALT_SHIFT_9 = ALT_SHIFT_(KEY_9)
+ALT_SHIFT_0 = ALT_SHIFT_(KEY_0)
+ALT_SHIFT_11_MINUS = ALT_SHIFT_(KEY_11_MINUS)
+ALT_SHIFT_12_PLUS = ALT_SHIFT_(KEY_12_PLUS)
 ALT_SHIFT_BACKSPACE = ALT_SHIFT_(BACKSPACE)
 
 ALT_SHIFT_NUMPAD_1 = ALT_SHIFT_(NUMPAD_1)
 ALT_SHIFT_NUMPAD_2 = ALT_SHIFT_(NUMPAD_2)
 ALT_SHIFT_NUMPAD_3 = ALT_SHIFT_(NUMPAD_3)
 ALT_SHIFT_NUMPAD_4 = ALT_SHIFT_(NUMPAD_4)
 ALT_SHIFT_NUMPAD_5 = ALT_SHIFT_(NUMPAD_5)
@@ -731,26 +731,26 @@
 CTRL_SHIFT_ALT_F8 = CTRL_SHIFT_ALT(F8)
 CTRL_SHIFT_ALT_F9 = CTRL_SHIFT_ALT(F9)
 CTRL_SHIFT_ALT_F10 = CTRL_SHIFT_ALT(F10)
 CTRL_SHIFT_ALT_F11 = CTRL_SHIFT_ALT(F11)
 CTRL_SHIFT_ALT_F12 = CTRL_SHIFT_ALT(F12)
 
 CTRL_SHIFT_ALT_OEM3_WAVE_OR_BACK_QUOTE = CTRL_SHIFT_ALT(OEM3_WAVE_OR_BACK_QUOTE)
-CTRL_SHIFT_ALT_KEY_1 = CTRL_SHIFT_ALT(KEY_1)
-CTRL_SHIFT_ALT_KEY_2 = CTRL_SHIFT_ALT(KEY_2)
-CTRL_SHIFT_ALT_KEY_3 = CTRL_SHIFT_ALT(KEY_3)
-CTRL_SHIFT_ALT_KEY_4 = CTRL_SHIFT_ALT(KEY_4)
-CTRL_SHIFT_ALT_KEY_5 = CTRL_SHIFT_ALT(KEY_5)
-CTRL_SHIFT_ALT_KEY_6 = CTRL_SHIFT_ALT(KEY_6)
-CTRL_SHIFT_ALT_KEY_7 = CTRL_SHIFT_ALT(KEY_7)
-CTRL_SHIFT_ALT_KEY_8 = CTRL_SHIFT_ALT(KEY_8)
-CTRL_SHIFT_ALT_KEY_9 = CTRL_SHIFT_ALT(KEY_9)
-CTRL_SHIFT_ALT_KEY_0 = CTRL_SHIFT_ALT(KEY_0)
-CTRL_SHIFT_ALT_KEY_11_MINUS = CTRL_SHIFT_ALT(KEY_11_MINUS)
-CTRL_SHIFT_ALT_KEY_12_PLUS = CTRL_SHIFT_ALT(KEY_12_PLUS)
+CTRL_SHIFT_ALT_1 = CTRL_SHIFT_ALT(KEY_1)
+CTRL_SHIFT_ALT_2 = CTRL_SHIFT_ALT(KEY_2)
+CTRL_SHIFT_ALT_3 = CTRL_SHIFT_ALT(KEY_3)
+CTRL_SHIFT_ALT_4 = CTRL_SHIFT_ALT(KEY_4)
+CTRL_SHIFT_ALT_5 = CTRL_SHIFT_ALT(KEY_5)
+CTRL_SHIFT_ALT_6 = CTRL_SHIFT_ALT(KEY_6)
+CTRL_SHIFT_ALT_7 = CTRL_SHIFT_ALT(KEY_7)
+CTRL_SHIFT_ALT_8 = CTRL_SHIFT_ALT(KEY_8)
+CTRL_SHIFT_ALT_9 = CTRL_SHIFT_ALT(KEY_9)
+CTRL_SHIFT_ALT_0 = CTRL_SHIFT_ALT(KEY_0)
+CTRL_SHIFT_ALT_11_MINUS = CTRL_SHIFT_ALT(KEY_11_MINUS)
+CTRL_SHIFT_ALT_12_PLUS = CTRL_SHIFT_ALT(KEY_12_PLUS)
 CTRL_SHIFT_ALT_BACKSPACE = CTRL_SHIFT_ALT(BACKSPACE)
 
 CTRL_SHIFT_ALT_NUMPAD_1 = CTRL_SHIFT_ALT(NUMPAD_1)
 CTRL_SHIFT_ALT_NUMPAD_2 = CTRL_SHIFT_ALT(NUMPAD_2)
 CTRL_SHIFT_ALT_NUMPAD_3 = CTRL_SHIFT_ALT(NUMPAD_3)
 CTRL_SHIFT_ALT_NUMPAD_4 = CTRL_SHIFT_ALT(NUMPAD_4)
 CTRL_SHIFT_ALT_NUMPAD_5 = CTRL_SHIFT_ALT(NUMPAD_5)
```

### Comparing `hotkeynet-0.1.3/hotkeynet/maker.py` & `hotkeynet-0.1.4/hotkeynet/maker.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/script.py` & `hotkeynet-0.1.4/hotkeynet/script.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/tests/__pycache__/helper.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/tests/__pycache__/helper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/utils.py` & `hotkeynet-0.1.4/hotkeynet/utils.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc` & `hotkeynet-0.1.4/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/vendor/better_enum.py` & `hotkeynet-0.1.4/hotkeynet/vendor/better_enum.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet/vendor/pytest_cov_helper.py` & `hotkeynet-0.1.4/hotkeynet/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/hotkeynet.egg-info/PKG-INFO` & `hotkeynet-0.1.4/hotkeynet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hotkeynet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Write hotkeynet script in Python.
 Home-page: https://github.com/MacHu-GWU/hotkeynet-project
-Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.3#downloads
+Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `hotkeynet-0.1.3/hotkeynet.egg-info/SOURCES.txt` & `hotkeynet-0.1.4/hotkeynet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/release-history.rst` & `hotkeynet-0.1.4/release-history.rst`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.4 (2023-05-09)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- rename ``CTRL_KEY_1`` -> ``CTRL_1``, and also for ``SHIFT_`` and ``ALT_``.
+
+
 0.1.3 (2023-05-09)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
 - Add lots of keyname and canned key enum.
```

### Comparing `hotkeynet-0.1.3/requirements-doc.txt` & `hotkeynet-0.1.4/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/setup.py` & `hotkeynet-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_api.py` & `hotkeynet-0.1.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_canned.py` & `hotkeynet-0.1.4/tests/test_canned.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_keyname.py` & `hotkeynet-0.1.4/tests/test_keyname.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_script_command.py` & `hotkeynet-0.1.4/tests/test_script_command.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_script_context.py` & `hotkeynet-0.1.4/tests/test_script_context.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_script_hotkey.py` & `hotkeynet-0.1.4/tests/test_script_hotkey.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_script_mouse.py` & `hotkeynet-0.1.4/tests/test_script_mouse.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_script_script.py` & `hotkeynet-0.1.4/tests/test_script_script.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_script_send_label.py` & `hotkeynet-0.1.4/tests/test_script_send_label.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.3/tests/test_utils.py` & `hotkeynet-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

