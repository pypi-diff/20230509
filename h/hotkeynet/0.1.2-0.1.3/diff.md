# Comparing `tmp/hotkeynet-0.1.2.tar.gz` & `tmp/hotkeynet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotkeynet-0.1.2.tar", last modified: Mon May  8 18:03:39 2023, max compression
+gzip compressed data, was "hotkeynet-0.1.3.tar", last modified: Tue May  9 04:39:08 2023, max compression
```

## Comparing `hotkeynet-0.1.2.tar` & `hotkeynet-0.1.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.081825 hotkeynet-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1119 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      341 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-08 18:03:39.081571 hotkeynet-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4408 2023-05-08 17:26:41.000000 hotkeynet-0.1.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.071322 hotkeynet-0.1.2/hotkeynet/
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-05-08 16:09:52.000000 hotkeynet-0.1.2/hotkeynet/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.073737 hotkeynet-0.1.2/hotkeynet/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      455 2023-05-08 16:10:53.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-05-08 18:03:38.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1359 2023-05-08 16:55:27.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/api.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     5837 2023-05-08 15:49:17.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/canned.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     5258 2023-05-08 15:21:42.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/keyname.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     3805 2023-05-08 16:59:43.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/maker.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)    55824 2023-05-08 16:57:58.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/script.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     2299 2023-05-08 06:38:52.000000 hotkeynet-0.1.2/hotkeynet/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-08 18:01:25.000000 hotkeynet-0.1.2/hotkeynet/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      954 2023-05-08 16:55:15.000000 hotkeynet-0.1.2/hotkeynet/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9740 2023-05-08 15:49:16.000000 hotkeynet-0.1.2/hotkeynet/canned.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.074043 hotkeynet-0.1.2/hotkeynet/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/hotkeynet/docs/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.074320 hotkeynet-0.1.2/hotkeynet/docs/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-05-08 13:10:35.000000 hotkeynet-0.1.2/hotkeynet/docs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     6682 2023-05-08 15:21:32.000000 hotkeynet-0.1.2/hotkeynet/keyname.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2911 2023-05-08 16:59:22.000000 hotkeynet-0.1.2/hotkeynet/maker.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    43493 2023-05-08 16:55:31.000000 hotkeynet-0.1.2/hotkeynet/script.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.075179 hotkeynet-0.1.2/hotkeynet/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/hotkeynet/tests/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.076109 hotkeynet-0.1.2/hotkeynet/tests/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      211 2023-05-08 04:44:05.000000 hotkeynet-0.1.2/hotkeynet/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      585 2023-05-08 16:40:41.000000 hotkeynet-0.1.2/hotkeynet/tests/__pycache__/helper.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      299 2023-05-08 04:44:05.000000 hotkeynet-0.1.2/hotkeynet/tests/__pycache__/paths.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      459 2023-05-08 16:17:16.000000 hotkeynet-0.1.2/hotkeynet/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      160 2023-05-08 04:41:11.000000 hotkeynet-0.1.2/hotkeynet/tests/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.076789 hotkeynet-0.1.2/hotkeynet/tpl/
--rw-r--r--   0 sanhehu    (501) staff       (20)      125 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/hotkeynet/tpl/Block.tpl
--rw-r--r--   0 sanhehu    (501) staff       (20)       91 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/hotkeynet/tpl/Script.tpl
--rw-r--r--   0 sanhehu    (501) staff       (20)      307 2023-05-08 16:56:31.000000 hotkeynet-0.1.2/hotkeynet/tpl/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.076990 hotkeynet-0.1.2/hotkeynet/tpl/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      449 2023-05-08 16:57:58.000000 hotkeynet-0.1.2/hotkeynet/tpl/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1491 2023-05-08 06:38:43.000000 hotkeynet-0.1.2/hotkeynet/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.077587 hotkeynet-0.1.2/hotkeynet/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-05-08 06:45:45.000000 hotkeynet-0.1.2/hotkeynet/vendor/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.078299 hotkeynet-0.1.2/hotkeynet/vendor/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-05-08 06:56:39.000000 hotkeynet-0.1.2/hotkeynet/vendor/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     5683 2023-05-08 06:56:39.000000 hotkeynet-0.1.2/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     3534 2023-05-08 16:18:00.000000 hotkeynet-0.1.2/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 hotkeynet-0.1.2/hotkeynet/vendor/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-08 04:40:02.000000 hotkeynet-0.1.2/hotkeynet/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.072011 hotkeynet-0.1.2/hotkeynet.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-08 18:03:39.000000 hotkeynet-0.1.2/hotkeynet.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1871 2023-05-08 18:03:39.000000 hotkeynet-0.1.2/hotkeynet.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-08 18:03:39.000000 hotkeynet-0.1.2/hotkeynet.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      229 2023-05-08 18:03:39.000000 hotkeynet-0.1.2/hotkeynet.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-05-08 18:03:39.000000 hotkeynet-0.1.2/hotkeynet.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      612 2023-05-08 18:02:31.000000 hotkeynet-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      289 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/requirements-ground-truth.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       53 2023-05-08 18:00:23.000000 hotkeynet-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-08 18:03:39.081869 hotkeynet-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7698 2023-05-08 04:33:13.000000 hotkeynet-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-08 18:03:39.081263 hotkeynet-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1418 2023-05-08 16:09:28.000000 hotkeynet-0.1.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1061 2023-05-08 15:46:05.000000 hotkeynet-0.1.2/tests/test_canned.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-08 06:17:59.000000 hotkeynet-0.1.2/tests/test_keyname.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      872 2023-05-08 13:49:25.000000 hotkeynet-0.1.2/tests/test_script_command.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1852 2023-05-08 13:49:38.000000 hotkeynet-0.1.2/tests/test_script_context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      826 2023-05-08 13:49:44.000000 hotkeynet-0.1.2/tests/test_script_hotkey.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      361 2023-05-08 13:49:50.000000 hotkeynet-0.1.2/tests/test_script_key.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      407 2023-05-08 13:49:58.000000 hotkeynet-0.1.2/tests/test_script_label.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1289 2023-05-08 16:14:49.000000 hotkeynet-0.1.2/tests/test_script_mouse.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      954 2023-05-08 16:51:24.000000 hotkeynet-0.1.2/tests/test_script_script.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      792 2023-05-08 13:50:22.000000 hotkeynet-0.1.2/tests/test_script_send_label.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1154 2023-05-08 13:50:55.000000 hotkeynet-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.221039 hotkeynet-0.1.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1119 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      341 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-09 04:39:08.220758 hotkeynet-0.1.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4408 2023-05-08 17:26:41.000000 hotkeynet-0.1.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.208766 hotkeynet-0.1.3/hotkeynet/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-05-08 16:09:52.000000 hotkeynet-0.1.3/hotkeynet/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.211869 hotkeynet-0.1.3/hotkeynet/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      455 2023-05-08 16:10:53.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-05-09 04:36:28.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1447 2023-05-09 04:34:42.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/api.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    18692 2023-05-09 04:34:42.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/canned.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17103 2023-05-09 04:34:42.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/keyname.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3805 2023-05-08 16:59:43.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/maker.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    55824 2023-05-08 16:57:58.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/script.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2299 2023-05-08 06:38:52.000000 hotkeynet-0.1.3/hotkeynet/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-09 04:36:27.000000 hotkeynet-0.1.3/hotkeynet/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1031 2023-05-09 04:30:59.000000 hotkeynet-0.1.3/hotkeynet/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    26168 2023-05-09 04:34:36.000000 hotkeynet-0.1.3/hotkeynet/canned.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.212191 hotkeynet-0.1.3/hotkeynet/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/docs/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.212467 hotkeynet-0.1.3/hotkeynet/docs/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-05-08 13:10:35.000000 hotkeynet-0.1.3/hotkeynet/docs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    21156 2023-05-09 04:33:49.000000 hotkeynet-0.1.3/hotkeynet/keyname.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2911 2023-05-08 16:59:22.000000 hotkeynet-0.1.3/hotkeynet/maker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    43493 2023-05-08 16:55:31.000000 hotkeynet-0.1.3/hotkeynet/script.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.213235 hotkeynet-0.1.3/hotkeynet/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/tests/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.213993 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      211 2023-05-08 04:44:05.000000 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      585 2023-05-08 16:40:41.000000 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/helper.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      299 2023-05-08 04:44:05.000000 hotkeynet-0.1.3/hotkeynet/tests/__pycache__/paths.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      459 2023-05-08 16:17:16.000000 hotkeynet-0.1.3/hotkeynet/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      160 2023-05-08 04:41:11.000000 hotkeynet-0.1.3/hotkeynet/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.214769 hotkeynet-0.1.3/hotkeynet/tpl/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      125 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/tpl/Block.tpl
+-rw-r--r--   0 sanhehu    (501) staff       (20)       91 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/hotkeynet/tpl/Script.tpl
+-rw-r--r--   0 sanhehu    (501) staff       (20)      307 2023-05-08 16:56:31.000000 hotkeynet-0.1.3/hotkeynet/tpl/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.215034 hotkeynet-0.1.3/hotkeynet/tpl/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      449 2023-05-08 16:57:58.000000 hotkeynet-0.1.3/hotkeynet/tpl/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1491 2023-05-08 06:38:43.000000 hotkeynet-0.1.3/hotkeynet/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.215676 hotkeynet-0.1.3/hotkeynet/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-05-08 06:45:45.000000 hotkeynet-0.1.3/hotkeynet/vendor/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.216570 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-05-08 06:56:39.000000 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5683 2023-05-08 06:56:39.000000 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3534 2023-05-08 16:18:00.000000 hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 hotkeynet-0.1.3/hotkeynet/vendor/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-08 04:40:02.000000 hotkeynet-0.1.3/hotkeynet/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.209501 hotkeynet-0.1.3/hotkeynet.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5509 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1871 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      229 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-05-09 04:39:08.000000 hotkeynet-0.1.3/hotkeynet.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      774 2023-05-09 04:36:17.000000 hotkeynet-0.1.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      289 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-ground-truth.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       53 2023-05-08 18:00:23.000000 hotkeynet-0.1.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-09 04:39:08.221106 hotkeynet-0.1.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7698 2023-05-08 04:33:13.000000 hotkeynet-0.1.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 04:39:08.220393 hotkeynet-0.1.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1418 2023-05-08 16:09:28.000000 hotkeynet-0.1.3/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1062 2023-05-09 04:34:51.000000 hotkeynet-0.1.3/tests/test_canned.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-08 06:17:59.000000 hotkeynet-0.1.3/tests/test_keyname.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      872 2023-05-08 13:49:25.000000 hotkeynet-0.1.3/tests/test_script_command.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1852 2023-05-08 13:49:38.000000 hotkeynet-0.1.3/tests/test_script_context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      826 2023-05-08 13:49:44.000000 hotkeynet-0.1.3/tests/test_script_hotkey.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      361 2023-05-08 13:49:50.000000 hotkeynet-0.1.3/tests/test_script_key.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      407 2023-05-08 13:49:58.000000 hotkeynet-0.1.3/tests/test_script_label.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1289 2023-05-08 16:14:49.000000 hotkeynet-0.1.3/tests/test_script_mouse.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      954 2023-05-08 16:51:24.000000 hotkeynet-0.1.3/tests/test_script_script.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      792 2023-05-08 13:50:22.000000 hotkeynet-0.1.3/tests/test_script_send_label.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1154 2023-05-08 13:50:55.000000 hotkeynet-0.1.3/tests/test_utils.py
```

### Comparing `hotkeynet-0.1.2/LICENSE.txt` & `hotkeynet-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/PKG-INFO` & `hotkeynet-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hotkeynet
-Version: 0.1.2
+Version: 0.1.3
 Summary: Write hotkeynet script in Python.
 Home-page: https://github.com/MacHu-GWU/hotkeynet-project
-Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `hotkeynet-0.1.2/README.rst` & `hotkeynet-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/__pycache__/api.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/__pycache__/api.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May  8 16:55:15 2023 UTC, .py size: 954 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,91 @@
-00000000: 550d 0d0a 0000 0000 7329 5964 ba03 0000  U.......s)Yd....
+00000000: 550d 0d0a 0000 0000 83cc 5964 0704 0000  U.........Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c06  d.l.m.Z...d.d.l.
-00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
-00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
-00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d13 5a13 6d14 5a14 6d15 5a15 6d16 5a16  m.Z.m.Z.m.Z.m.Z.
-00000090: 6d17 5a17 6d18 5a18 6d19 5a19 6d1a 5a1a  m.Z.m.Z.m.Z.m.Z.
-000000a0: 6d1b 5a1b 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e  m.Z.m.Z.m.Z.m.Z.
-000000b0: 6d1f 5a1f 6d20 5a20 6d21 5a21 6d22 5a22  m.Z.m Z m!Z!m"Z"
-000000c0: 6d23 5a23 6d24 5a24 6d25 5a25 6d26 5a26  m#Z#m$Z$m%Z%m&Z&
-000000d0: 6d27 5a27 6d28 5a28 6d29 5a29 6d2a 5a2a  m'Z'm(Z(m)Z)m*Z*
-000000e0: 6d2b 5a2b 6d2c 5a2c 6d2d 5a2d 6d2e 5a2e  m+Z+m,Z,m-Z-m.Z.
-000000f0: 6d2f 5a2f 6d30 5a30 6d31 5a31 6d32 5a32  m/Z/m0Z0m1Z1m2Z2
-00000100: 6d33 5a33 6d34 5a34 6d35 5a35 6d36 5a36  m3Z3m4Z4m5Z5m6Z6
-00000110: 6d37 5a37 6d38 5a38 6d39 5a39 0100 6405  m7Z7m8Z8m9Z9..d.
-00000120: 5300 2906 7a0d 0a53 7461 626c 6520 4150  S.).z..Stable AP
-00000130: 492e 0ae9 0100 0000 2901 da07 6b65 796e  I.......)...keyn
-00000140: 616d 6529 01da 0663 616e 6e65 6429 33da  ame)...canned)3.
-00000150: 0763 6f6e 7465 7874 da05 426c 6f63 6bda  .context..Block.
-00000160: 0653 6372 6970 74da 0c53 656e 644d 6f64  .Script..SendMod
-00000170: 6545 6e75 6dda 054c 6162 656c da07 436f  eEnum..Label..Co
-00000180: 6d6d 616e 64da 0e43 6f6d 6d61 6e64 4172  mmand..CommandAr
-00000190: 6745 6e75 6dda 0b43 616c 6c43 6f6d 6d61  gEnum..CallComma
-000001a0: 6e64 da06 5365 6e64 5043 da03 5275 6eda  nd..SendPC..Run.
-000001b0: 0648 6f74 6b65 79da 0e4d 6f76 656d 656e  .Hotkey..Movemen
-000001c0: 7448 6f74 6b65 79da 034b 6579 da05 4b65  tHotkey..Key..Ke
-000001d0: 7955 70da 074b 6579 446f 776e da09 5365  yUp..KeyDown..Se
-000001e0: 6e64 4c61 6265 6cda 0f4d 6f75 7365 4275  ndLabel..MouseBu
-000001f0: 7474 6f6e 456e 756d da0f 4d6f 7573 6553  ttonEnum..MouseS
-00000200: 7472 6f6b 6545 6e75 6dda 0f4d 6f75 7365  trokeEnum..Mouse
-00000210: 5461 7267 6574 456e 756d da0d 4d6f 7573  TargetEnum..Mous
-00000220: 654d 6f64 6545 6e75 6dda 0a43 6c69 636b  eModeEnum..Click
-00000230: 4d6f 7573 65da 094d 6f76 654d 6f75 7365  Mouse..MoveMouse
-00000240: da09 5265 6e61 6d65 5769 6eda 0954 6172  ..RenameWin..Tar
-00000250: 6765 7457 696e da04 5761 6974 da0a 5761  getWin..Wait..Wa
-00000260: 6974 466f 7257 696e da11 5761 6974 466f  itForWin..WaitFo
-00000270: 7257 696e 456e 6162 6c65 64da 1053 6574  rWinEnabled..Set
-00000280: 466f 7265 6772 6f75 6e64 5769 6eda 0c53  ForegroundWin..S
-00000290: 6574 4163 7469 7665 5769 6eda 0654 6f67  etActiveWin..Tog
-000002a0: 676c 65da 0d54 6f67 676c 6548 6f74 6b65  gle..ToggleHotke
-000002b0: 7973 da09 546f 6767 6c65 5769 6eda 0753  ys..ToggleWin..S
-000002c0: 656e 6457 696e da08 5365 6e64 5769 6e4d  endWin..SendWinM
-000002d0: da09 5365 6e64 5769 6e4d 46da 0853 656e  ..SendWinMF..Sen
-000002e0: 6457 696e 53da 0953 656e 6457 696e 5346  dWinS..SendWinSF
-000002f0: da0c 5365 6e64 466f 6375 7357 696e da09  ..SendFocusWin..
-00000300: 5365 7457 696e 506f 73da 0a53 6574 5769  SetWinPos..SetWi
-00000310: 6e53 697a 65da 0a53 6574 5769 6e52 6563  nSize..SetWinRec
-00000320: 74da 0454 6578 74da 0b43 7265 6174 6550  t..Text..CreateP
-00000330: 616e 656c da0c 4372 6561 7465 4275 7474  anel..CreateButt
-00000340: 6f6e da13 4372 6561 7465 5069 6374 7572  on..CreatePictur
-00000350: 6542 7574 746f 6eda 1343 7265 6174 6543  eButton..CreateC
-00000360: 6f6c 6f72 6564 4275 7474 6f6e da10 4164  oloredButton..Ad
-00000370: 6442 7574 746f 6e54 6f50 616e 656c da0f  dButtonToPanel..
-00000380: 5365 7442 7574 746f 6e48 6f74 6b65 79da  SetButtonHotkey.
-00000390: 1053 6574 4275 7474 6f6e 436f 6d6d 616e  .SetButtonComman
-000003a0: 64da 0b41 6c77 6179 734f 6e54 6f70 da0e  d..AlwaysOnTop..
-000003b0: 5365 7450 616e 656c 4c61 796f 7574 4e29  SetPanelLayoutN)
-000003c0: 3ada 075f 5f64 6f63 5f5f da00 7202 0000  :..__doc__..r...
-000003d0: 005a 024b 4e72 0300 0000 5a03 4341 4eda  .Z.KNr....Z.CAN.
-000003e0: 0673 6372 6970 7472 0400 0000 7205 0000  .scriptr....r...
-000003f0: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000400: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000410: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
-00000420: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00000430: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000440: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000450: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000460: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00000470: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
-00000480: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
-00000490: 0072 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
-000004a0: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-000004b0: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
-000004c0: 0000 0072 3000 0000 7231 0000 0072 3200  ...r0...r1...r2.
-000004d0: 0000 7233 0000 0072 3400 0000 7235 0000  ..r3...r4...r5..
-000004e0: 0072 3600 0000 a900 723a 0000 0072 3a00  .r6.....r:...r:.
-000004f0: 0000 fa42 2f55 7365 7273 2f73 616e 6865  ...B/Users/sanhe
-00000500: 6875 2f44 6f63 756d 656e 7473 2f47 6974  hu/Documents/Git
-00000510: 4875 622f 686f 746b 6579 6e65 742d 7072  Hub/hotkeynet-pr
-00000520: 6f6a 6563 742f 686f 746b 6579 6e65 742f  oject/hotkeynet/
-00000530: 6170 692e 7079 da08 3c6d 6f64 756c 653e  api.py..<module>
-00000540: 0300 0000 7306 0000 0004 040c 010c 02    ....s..........
+00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6401  m.Z.m.Z.m.Z...d.
+00000060: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
+00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
+00000080: 6d12 5a12 6d13 5a13 6d14 5a14 6d15 5a15  m.Z.m.Z.m.Z.m.Z.
+00000090: 6d16 5a16 6d17 5a17 6d18 5a18 6d19 5a19  m.Z.m.Z.m.Z.m.Z.
+000000a0: 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c 6d1d 5a1d  m.Z.m.Z.m.Z.m.Z.
+000000b0: 6d1e 5a1e 6d1f 5a1f 6d20 5a20 6d21 5a21  m.Z.m.Z.m Z m!Z!
+000000c0: 6d22 5a22 6d23 5a23 6d24 5a24 6d25 5a25  m"Z"m#Z#m$Z$m%Z%
+000000d0: 6d26 5a26 6d27 5a27 6d28 5a28 6d29 5a29  m&Z&m'Z'm(Z(m)Z)
+000000e0: 6d2a 5a2a 6d2b 5a2b 6d2c 5a2c 6d2d 5a2d  m*Z*m+Z+m,Z,m-Z-
+000000f0: 6d2e 5a2e 6d2f 5a2f 6d30 5a30 6d31 5a31  m.Z.m/Z/m0Z0m1Z1
+00000100: 6d32 5a32 6d33 5a33 6d34 5a34 6d35 5a35  m2Z2m3Z3m4Z4m5Z5
+00000110: 6d36 5a36 6d37 5a37 6d38 5a38 6d39 5a39  m6Z6m7Z7m8Z8m9Z9
+00000120: 6d3a 5a3a 6d3b 5a3b 6d3c 5a3c 6d3d 5a3d  m:Z:m;Z;m<Z<m=Z=
+00000130: 0100 6406 5300 2907 7a0d 0a53 7461 626c  ..d.S.).z..Stabl
+00000140: 6520 4150 492e 0ae9 0100 0000 2901 da07  e API.......)...
+00000150: 6b65 796e 616d 6529 01da 0663 616e 6e65  keyname)...canne
+00000160: 6429 03da 084b 6579 4d61 6b65 72da 0a43  d)...KeyMaker..C
+00000170: 6c69 636b 4d61 6b65 72da 124d 6f64 6966  lickMaker..Modif
+00000180: 6965 6443 6c69 636b 4d61 6b65 7229 33da  iedClickMaker)3.
+00000190: 0763 6f6e 7465 7874 da05 426c 6f63 6bda  .context..Block.
+000001a0: 0653 6372 6970 74da 0c53 656e 644d 6f64  .Script..SendMod
+000001b0: 6545 6e75 6dda 054c 6162 656c da07 436f  eEnum..Label..Co
+000001c0: 6d6d 616e 64da 0e43 6f6d 6d61 6e64 4172  mmand..CommandAr
+000001d0: 6745 6e75 6dda 0b43 616c 6c43 6f6d 6d61  gEnum..CallComma
+000001e0: 6e64 da06 5365 6e64 5043 da03 5275 6eda  nd..SendPC..Run.
+000001f0: 0648 6f74 6b65 79da 0e4d 6f76 656d 656e  .Hotkey..Movemen
+00000200: 7448 6f74 6b65 79da 034b 6579 da05 4b65  tHotkey..Key..Ke
+00000210: 7955 70da 074b 6579 446f 776e da09 5365  yUp..KeyDown..Se
+00000220: 6e64 4c61 6265 6cda 0f4d 6f75 7365 4275  ndLabel..MouseBu
+00000230: 7474 6f6e 456e 756d da0f 4d6f 7573 6553  ttonEnum..MouseS
+00000240: 7472 6f6b 6545 6e75 6dda 0f4d 6f75 7365  trokeEnum..Mouse
+00000250: 5461 7267 6574 456e 756d da0d 4d6f 7573  TargetEnum..Mous
+00000260: 654d 6f64 6545 6e75 6dda 0a43 6c69 636b  eModeEnum..Click
+00000270: 4d6f 7573 65da 094d 6f76 654d 6f75 7365  Mouse..MoveMouse
+00000280: da09 5265 6e61 6d65 5769 6eda 0954 6172  ..RenameWin..Tar
+00000290: 6765 7457 696e da04 5761 6974 da0a 5761  getWin..Wait..Wa
+000002a0: 6974 466f 7257 696e da11 5761 6974 466f  itForWin..WaitFo
+000002b0: 7257 696e 456e 6162 6c65 64da 1053 6574  rWinEnabled..Set
+000002c0: 466f 7265 6772 6f75 6e64 5769 6eda 0c53  ForegroundWin..S
+000002d0: 6574 4163 7469 7665 5769 6eda 0654 6f67  etActiveWin..Tog
+000002e0: 676c 65da 0d54 6f67 676c 6548 6f74 6b65  gle..ToggleHotke
+000002f0: 7973 da09 546f 6767 6c65 5769 6eda 0753  ys..ToggleWin..S
+00000300: 656e 6457 696e da08 5365 6e64 5769 6e4d  endWin..SendWinM
+00000310: da09 5365 6e64 5769 6e4d 46da 0853 656e  ..SendWinMF..Sen
+00000320: 6457 696e 53da 0953 656e 6457 696e 5346  dWinS..SendWinSF
+00000330: da0c 5365 6e64 466f 6375 7357 696e da09  ..SendFocusWin..
+00000340: 5365 7457 696e 506f 73da 0a53 6574 5769  SetWinPos..SetWi
+00000350: 6e53 697a 65da 0a53 6574 5769 6e52 6563  nSize..SetWinRec
+00000360: 74da 0454 6578 74da 0b43 7265 6174 6550  t..Text..CreateP
+00000370: 616e 656c da0c 4372 6561 7465 4275 7474  anel..CreateButt
+00000380: 6f6e da13 4372 6561 7465 5069 6374 7572  on..CreatePictur
+00000390: 6542 7574 746f 6eda 1343 7265 6174 6543  eButton..CreateC
+000003a0: 6f6c 6f72 6564 4275 7474 6f6e da10 4164  oloredButton..Ad
+000003b0: 6442 7574 746f 6e54 6f50 616e 656c da0f  dButtonToPanel..
+000003c0: 5365 7442 7574 746f 6e48 6f74 6b65 79da  SetButtonHotkey.
+000003d0: 1053 6574 4275 7474 6f6e 436f 6d6d 616e  .SetButtonComman
+000003e0: 64da 0b41 6c77 6179 734f 6e54 6f70 da0e  d..AlwaysOnTop..
+000003f0: 5365 7450 616e 656c 4c61 796f 7574 4e29  SetPanelLayoutN)
+00000400: 3eda 075f 5f64 6f63 5f5f da00 7202 0000  >..__doc__..r...
+00000410: 00da 024b 4e72 0300 0000 da03 4341 4eda  ...KNr......CAN.
+00000420: 056d 616b 6572 7204 0000 0072 0500 0000  .makerr....r....
+00000430: 7206 0000 00da 0673 6372 6970 7472 0700  r......scriptr..
+00000440: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000450: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000460: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000470: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00000480: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
+00000490: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
+000004a0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+000004b0: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+000004c0: 2100 0000 7222 0000 0072 2300 0000 7224  !...r"...r#...r$
+000004d0: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
+000004e0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+000004f0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000500: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00000510: 3100 0000 7232 0000 0072 3300 0000 7234  1...r2...r3...r4
+00000520: 0000 0072 3500 0000 7236 0000 0072 3700  ...r5...r6...r7.
+00000530: 0000 7238 0000 0072 3900 0000 a900 7240  ..r8...r9.....r@
+00000540: 0000 0072 4000 0000 fa42 2f55 7365 7273  ...r@....B/Users
+00000550: 2f73 616e 6865 6875 2f44 6f63 756d 656e  /sanhehu/Documen
+00000560: 7473 2f47 6974 4875 622f 686f 746b 6579  ts/GitHub/hotkey
+00000570: 6e65 742d 7072 6f6a 6563 742f 686f 746b  net-project/hotk
+00000580: 6579 6e65 742f 6170 692e 7079 da08 3c6d  eynet/api.py..<m
+00000590: 6f64 756c 653e 0300 0000 7308 0000 0004  odule>....s.....
+000005a0: 040c 010c 0114 06                        .......
```

### Comparing `hotkeynet-0.1.2/hotkeynet/__pycache__/maker.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/__pycache__/maker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/__pycache__/script.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/__pycache__/script.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/__pycache__/utils.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/api.py` & `hotkeynet-0.1.3/hotkeynet/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 """
 Stable API.
 """
 
 from . import keyname as KN
 from . import canned as CAN
+from .maker import (
+    KeyMaker,
+    ClickMaker,
+    ModifiedClickMaker,
+)
 
 from .script import (
     context,
     Block,
     Script,
     SendModeEnum,
     Label,
```

### Comparing `hotkeynet-0.1.2/hotkeynet/maker.py` & `hotkeynet-0.1.3/hotkeynet/maker.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/script.py` & `hotkeynet-0.1.3/hotkeynet/script.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/tests/__pycache__/helper.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/tests/__pycache__/helper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/utils.py` & `hotkeynet-0.1.3/hotkeynet/utils.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/better_enum.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc` & `hotkeynet-0.1.3/hotkeynet/vendor/__pycache__/pytest_cov_helper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/vendor/better_enum.py` & `hotkeynet-0.1.3/hotkeynet/vendor/better_enum.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet/vendor/pytest_cov_helper.py` & `hotkeynet-0.1.3/hotkeynet/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/hotkeynet.egg-info/PKG-INFO` & `hotkeynet-0.1.3/hotkeynet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hotkeynet
-Version: 0.1.2
+Version: 0.1.3
 Summary: Write hotkeynet script in Python.
 Home-page: https://github.com/MacHu-GWU/hotkeynet-project
-Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/hotkeynet/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `hotkeynet-0.1.2/hotkeynet.egg-info/SOURCES.txt` & `hotkeynet-0.1.3/hotkeynet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/release-history.rst` & `hotkeynet-0.1.3/release-history.rst`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.3 (2023-05-09)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- Add lots of keyname and canned key enum.
+
+
 0.1.2 (2023-05-08)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
 - remove unnecessary dependencies.
```

### Comparing `hotkeynet-0.1.2/requirements-doc.txt` & `hotkeynet-0.1.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/setup.py` & `hotkeynet-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_api.py` & `hotkeynet-0.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_canned.py` & `hotkeynet-0.1.3/tests/test_canned.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     assert canned._resolve_key_liked_arg(canned.KEY_1) == "1"
     assert canned._resolve_key_liked_arg(KN.KEY_1) == "1"
 
 
 def test_key_with_modifier():
     assert canned.CTRL_(canned.KEY_1, KN.KEY_2)().key == "Ctrl 1, 2"
     assert canned.CTRL_ALT_(canned.KEY_1, KN.KEY_2)().key == "Ctrl Alt 1, 2"
-    assert canned.CTRL_SHIFT_ALT(canned.KEY_1, KN.KEY_2)().key == "Ctrl Shift Alt 1, 2"
+    assert canned.CTRL_SHIFT_ALT_(canned.KEY_1, KN.KEY_2)().key == "Ctrl Shift Alt 1, 2"
     assert canned.LWIN_(canned.KEY_1)().key == "LWin 1"
     assert canned.RWIN_(KN.KEY_1)().key == "RWin 1"
 
 def test_modified_mouse_click():
     assert canned.MOUSE_LButton().button == "LButton"
 
     actions = canned.SHIFT_LEFT_CLICK()
```

### Comparing `hotkeynet-0.1.2/tests/test_keyname.py` & `hotkeynet-0.1.3/tests/test_keyname.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_script_command.py` & `hotkeynet-0.1.3/tests/test_script_command.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_script_context.py` & `hotkeynet-0.1.3/tests/test_script_context.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_script_hotkey.py` & `hotkeynet-0.1.3/tests/test_script_hotkey.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_script_mouse.py` & `hotkeynet-0.1.3/tests/test_script_mouse.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_script_script.py` & `hotkeynet-0.1.3/tests/test_script_script.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_script_send_label.py` & `hotkeynet-0.1.3/tests/test_script_send_label.py`

 * *Files identical despite different names*

### Comparing `hotkeynet-0.1.2/tests/test_utils.py` & `hotkeynet-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

