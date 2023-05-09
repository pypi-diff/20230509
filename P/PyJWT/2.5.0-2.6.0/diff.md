# Comparing `tmp/PyJWT-2.5.0.tar.gz` & `tmp/PyJWT-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyJWT-2.5.0.tar", last modified: Sat Sep 17 14:01:40 2022, max compression
+gzip compressed data, was "dist/PyJWT-2.6.0.tar", last modified: Thu Oct 20 01:08:45 2022, max compression
```

## Comparing `PyJWT-2.5.0.tar` & `PyJWT-2.6.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.141144 PyJWT-2.5.0/
--rw-r--r--   0 jpadilla   (501) staff       (20)      907 2022-09-16 20:01:01.000000 PyJWT-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0 jpadilla   (501) staff       (20)      322 2020-11-02 12:48:30.000000 PyJWT-2.5.0/AUTHORS.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)    27807 2022-09-17 13:52:33.000000 PyJWT-2.5.0/CHANGELOG.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     3272 2019-10-20 23:19:00.000000 PyJWT-2.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jpadilla   (501) staff       (20)     1085 2022-05-12 18:31:26.000000 PyJWT-2.5.0/LICENSE
--rw-r--r--   0 jpadilla   (501) staff       (20)      309 2021-01-12 03:01:03.000000 PyJWT-2.5.0/MANIFEST.in
--rw-r--r--   0 jpadilla   (501) staff       (20)     3836 2022-09-17 14:01:40.141296 PyJWT-2.5.0/PKG-INFO
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.111389 PyJWT-2.5.0/PyJWT.egg-info/
--rw-r--r--   0 jpadilla   (501) staff       (20)     3836 2022-09-17 14:01:39.000000 PyJWT-2.5.0/PyJWT.egg-info/PKG-INFO
--rw-r--r--   0 jpadilla   (501) staff       (20)     1858 2022-09-17 14:01:39.000000 PyJWT-2.5.0/PyJWT.egg-info/SOURCES.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-09-17 14:01:39.000000 PyJWT-2.5.0/PyJWT.egg-info/dependency_links.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-09-17 14:01:39.000000 PyJWT-2.5.0/PyJWT.egg-info/not-zip-safe
--rw-r--r--   0 jpadilla   (501) staff       (20)      331 2022-09-17 14:01:39.000000 PyJWT-2.5.0/PyJWT.egg-info/requires.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)        4 2022-09-17 14:01:39.000000 PyJWT-2.5.0/PyJWT.egg-info/top_level.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)     2336 2022-09-16 20:01:01.000000 PyJWT-2.5.0/README.rst
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.114975 PyJWT-2.5.0/docs/
--rw-r--r--   0 jpadilla   (501) staff       (20)     7405 2018-11-26 03:04:17.000000 PyJWT-2.5.0/docs/Makefile
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.115471 PyJWT-2.5.0/docs/_static/
--rw-r--r--   0 jpadilla   (501) staff       (20)      363 2018-11-26 03:04:17.000000 PyJWT-2.5.0/docs/_static/theme_overrides.css
--rw-r--r--   0 jpadilla   (501) staff       (20)     3538 2022-07-19 02:16:21.000000 PyJWT-2.5.0/docs/algorithms.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     7518 2022-09-16 20:01:01.000000 PyJWT-2.5.0/docs/api.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)       30 2021-01-12 03:01:03.000000 PyJWT-2.5.0/docs/changelog.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     3914 2022-05-12 18:31:26.000000 PyJWT-2.5.0/docs/conf.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      621 2020-12-20 00:01:37.000000 PyJWT-2.5.0/docs/faq.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)     2018 2022-09-16 20:01:01.000000 PyJWT-2.5.0/docs/index.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)      791 2021-08-08 19:55:24.000000 PyJWT-2.5.0/docs/installation.rst
--rw-r--r--   0 jpadilla   (501) staff       (20)       24 2020-06-19 14:24:04.000000 PyJWT-2.5.0/docs/requirements-docs.txt
--rw-r--r--   0 jpadilla   (501) staff       (20)    11752 2022-05-12 18:31:26.000000 PyJWT-2.5.0/docs/usage.rst
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.121034 PyJWT-2.5.0/jwt/
--rw-r--r--   0 jpadilla   (501) staff       (20)     1604 2022-09-17 13:52:33.000000 PyJWT-2.5.0/jwt/__init__.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    23688 2022-07-19 02:01:25.000000 PyJWT-2.5.0/jwt/algorithms.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     3653 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/api_jwk.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    10653 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/api_jws.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     9930 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/api_jwt.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      963 2022-05-12 18:31:26.000000 PyJWT-2.5.0/jwt/exceptions.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     1692 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/help.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      944 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/jwk_set_cache.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     3553 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/jwks_client.py
--rw-r--r--   0 jpadilla   (501) staff       (20)        0 2020-12-20 00:01:37.000000 PyJWT-2.5.0/jwt/py.typed
--rw-r--r--   0 jpadilla   (501) staff       (20)     3973 2022-09-16 20:01:01.000000 PyJWT-2.5.0/jwt/utils.py
--rw-r--r--   0 jpadilla   (501) staff       (20)       59 2022-07-19 02:01:25.000000 PyJWT-2.5.0/jwt/warnings.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     1440 2022-09-17 14:01:40.141958 PyJWT-2.5.0/setup.cfg
--rwxr-xr-x   0 jpadilla   (501) staff       (20)       62 2020-06-19 15:14:56.000000 PyJWT-2.5.0/setup.py
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.126048 PyJWT-2.5.0/tests/
--rw-r--r--   0 jpadilla   (501) staff       (20)        0 2018-11-26 03:04:17.000000 PyJWT-2.5.0/tests/__init__.py
-drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-09-17 14:01:40.140926 PyJWT-2.5.0/tests/keys/
--rw-r--r--   0 jpadilla   (501) staff       (20)     1488 2020-12-21 16:55:46.000000 PyJWT-2.5.0/tests/keys/__init__.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      245 2021-04-28 11:23:40.000000 PyJWT-2.5.0/tests/keys/jwk_ec_key_P-256.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      308 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/jwk_ec_key_P-384.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      380 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/jwk_ec_key_P-521.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      250 2021-04-28 11:23:40.000000 PyJWT-2.5.0/tests/keys/jwk_ec_key_secp256k1.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      191 2021-04-28 11:23:40.000000 PyJWT-2.5.0/tests/keys/jwk_ec_pub_P-256.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      233 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/jwk_ec_pub_P-384.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      281 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/jwk_ec_pub_P-521.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      196 2021-04-28 11:23:40.000000 PyJWT-2.5.0/tests/keys/jwk_ec_pub_secp256k1.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)      171 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/jwk_hmac.json
--rw-r--r--   0 jpadilla   (501) staff       (20)     1470 2022-07-19 02:01:25.000000 PyJWT-2.5.0/tests/keys/jwk_keyset_only_unknown_alg.json
--rw-r--r--   0 jpadilla   (501) staff       (20)     2926 2022-07-19 02:01:25.000000 PyJWT-2.5.0/tests/keys/jwk_keyset_with_unknown_alg.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      143 2021-04-28 11:23:40.000000 PyJWT-2.5.0/tests/keys/jwk_okp_key_Ed25519.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      270 2021-10-06 10:37:16.000000 PyJWT-2.5.0/tests/keys/jwk_okp_key_Ed448.json
--rw-r--r--   0 jpadilla   (501) staff       (20)       90 2021-04-28 11:23:40.000000 PyJWT-2.5.0/tests/keys/jwk_okp_pub_Ed25519.json
--rw-r--r--   0 jpadilla   (501) staff       (20)      183 2021-10-06 10:37:16.000000 PyJWT-2.5.0/tests/keys/jwk_okp_pub_Ed448.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)     1745 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/jwk_rsa_key.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)      461 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/jwk_rsa_pub.json
--rw-rw-r--   0 jpadilla   (501) staff       (20)      451 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/testkey2_rsa.pub.pem
--rw-r--r--   0 jpadilla   (501) staff       (20)      241 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/testkey_ec.priv
--rw-r--r--   0 jpadilla   (501) staff       (20)      178 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/testkey_ec.pub
--rw-r--r--   0 jpadilla   (501) staff       (20)      209 2022-07-19 02:01:25.000000 PyJWT-2.5.0/tests/keys/testkey_ec_secp192r1.priv
--rw-r--r--   0 jpadilla   (501) staff       (20)      161 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/testkey_ec_ssh.pub
--rw-r--r--   0 jpadilla   (501) staff       (20)      119 2020-08-24 14:15:08.000000 PyJWT-2.5.0/tests/keys/testkey_ed25519
--rw-r--r--   0 jpadilla   (501) staff       (20)       81 2020-08-24 14:15:07.000000 PyJWT-2.5.0/tests/keys/testkey_ed25519.pub
--rw-rw-r--   0 jpadilla   (501) staff       (20)      247 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/testkey_pkcs1.pub.pem
--rw-rw-r--   0 jpadilla   (501) staff       (20)     1281 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/testkey_rsa.cer
--rw-r--r--   0 jpadilla   (501) staff       (20)     1679 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/keys/testkey_rsa.priv
--rw-rw-r--   0 jpadilla   (501) staff       (20)      401 2020-04-08 13:53:03.000000 PyJWT-2.5.0/tests/keys/testkey_rsa.pub
--rw-r--r--   0 jpadilla   (501) staff       (20)     5022 2022-05-15 19:17:57.000000 PyJWT-2.5.0/tests/test_advisory.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    38285 2022-07-19 02:01:25.000000 PyJWT-2.5.0/tests/test_algorithms.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     9699 2022-09-16 20:01:01.000000 PyJWT-2.5.0/tests/test_api_jwk.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    29203 2022-07-19 02:01:25.000000 PyJWT-2.5.0/tests/test_api_jws.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    24770 2022-09-16 20:01:01.000000 PyJWT-2.5.0/tests/test_api_jwt.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      213 2019-10-22 15:57:44.000000 PyJWT-2.5.0/tests/test_exceptions.py
--rw-r--r--   0 jpadilla   (501) staff       (20)    12895 2022-09-16 20:01:01.000000 PyJWT-2.5.0/tests/test_jwks_client.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      625 2020-08-24 16:22:55.000000 PyJWT-2.5.0/tests/test_jwt.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      897 2020-12-20 00:01:37.000000 PyJWT-2.5.0/tests/test_utils.py
--rw-r--r--   0 jpadilla   (501) staff       (20)      722 2021-10-06 10:37:16.000000 PyJWT-2.5.0/tests/utils.py
--rw-r--r--   0 jpadilla   (501) staff       (20)     1427 2022-09-16 20:01:01.000000 PyJWT-2.5.0/tox.ini
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.271692 PyJWT-2.6.0/
+-rw-r--r--   0 jpadilla   (501) staff       (20)      908 2022-10-20 00:40:43.000000 PyJWT-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 jpadilla   (501) staff       (20)      322 2020-11-02 12:48:30.000000 PyJWT-2.6.0/AUTHORS.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)    28577 2022-10-20 01:08:19.000000 PyJWT-2.6.0/CHANGELOG.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3272 2019-10-20 23:19:00.000000 PyJWT-2.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1085 2022-05-12 18:31:26.000000 PyJWT-2.6.0/LICENSE
+-rw-r--r--   0 jpadilla   (501) staff       (20)      309 2021-01-12 03:01:03.000000 PyJWT-2.6.0/MANIFEST.in
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3836 2022-10-20 01:08:45.272015 PyJWT-2.6.0/PKG-INFO
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.209050 PyJWT-2.6.0/PyJWT.egg-info/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3836 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/PKG-INFO
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1873 2022-10-20 01:08:45.000000 PyJWT-2.6.0/PyJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)        1 2022-09-17 14:01:39.000000 PyJWT-2.6.0/PyJWT.egg-info/not-zip-safe
+-rw-r--r--   0 jpadilla   (501) staff       (20)      277 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/requires.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)        4 2022-10-20 01:08:44.000000 PyJWT-2.6.0/PyJWT.egg-info/top_level.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)     2336 2022-09-20 10:55:34.000000 PyJWT-2.6.0/README.rst
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.219760 PyJWT-2.6.0/docs/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     7405 2018-11-26 03:04:17.000000 PyJWT-2.6.0/docs/Makefile
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.220723 PyJWT-2.6.0/docs/_static/
+-rw-r--r--   0 jpadilla   (501) staff       (20)      363 2018-11-26 03:04:17.000000 PyJWT-2.6.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3538 2022-07-19 02:16:21.000000 PyJWT-2.6.0/docs/algorithms.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     7518 2022-09-20 10:55:34.000000 PyJWT-2.6.0/docs/api.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)       30 2021-01-12 03:01:03.000000 PyJWT-2.6.0/docs/changelog.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3914 2022-05-12 18:31:26.000000 PyJWT-2.6.0/docs/conf.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      621 2020-12-20 00:01:37.000000 PyJWT-2.6.0/docs/faq.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)     2018 2022-09-20 10:55:34.000000 PyJWT-2.6.0/docs/index.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)      791 2021-08-08 19:55:24.000000 PyJWT-2.6.0/docs/installation.rst
+-rw-r--r--   0 jpadilla   (501) staff       (20)       24 2020-06-19 14:24:04.000000 PyJWT-2.6.0/docs/requirements-docs.txt
+-rw-r--r--   0 jpadilla   (501) staff       (20)    11752 2022-05-12 18:31:26.000000 PyJWT-2.6.0/docs/usage.rst
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.230894 PyJWT-2.6.0/jwt/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1604 2022-10-20 01:08:19.000000 PyJWT-2.6.0/jwt/__init__.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    23688 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/algorithms.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3653 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/api_jwk.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    10653 2022-09-20 11:00:07.000000 PyJWT-2.6.0/jwt/api_jws.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    10059 2022-10-20 00:40:19.000000 PyJWT-2.6.0/jwt/api_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      963 2022-05-12 18:31:26.000000 PyJWT-2.6.0/jwt/exceptions.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1692 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/help.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      944 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/jwk_set_cache.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3553 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/jwks_client.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)        0 2020-12-20 00:01:37.000000 PyJWT-2.6.0/jwt/py.typed
+-rw-r--r--   0 jpadilla   (501) staff       (20)     3973 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/utils.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)       59 2022-09-20 10:55:34.000000 PyJWT-2.6.0/jwt/warnings.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      448 2022-09-20 10:55:34.000000 PyJWT-2.6.0/pyproject.toml
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1384 2022-10-20 01:08:45.273726 PyJWT-2.6.0/setup.cfg
+-rwxr-xr-x   0 jpadilla   (501) staff       (20)       62 2020-06-19 15:14:56.000000 PyJWT-2.6.0/setup.py
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.243403 PyJWT-2.6.0/tests/
+-rw-r--r--   0 jpadilla   (501) staff       (20)        0 2018-11-26 03:04:17.000000 PyJWT-2.6.0/tests/__init__.py
+drwxr-xr-x   0 jpadilla   (501) staff       (20)        0 2022-10-20 01:08:45.270980 PyJWT-2.6.0/tests/keys/
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1488 2020-12-21 16:55:46.000000 PyJWT-2.6.0/tests/keys/__init__.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      245 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_P-256.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      308 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_P-384.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      380 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_P-521.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      250 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_key_secp256k1.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      191 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_P-256.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      233 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_P-384.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      281 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_P-521.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      196 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_ec_pub_secp256k1.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      171 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/jwk_hmac.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1470 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/keys/jwk_keyset_only_unknown_alg.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)     2926 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/keys/jwk_keyset_with_unknown_alg.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      143 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_okp_key_Ed25519.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      270 2021-10-06 10:37:16.000000 PyJWT-2.6.0/tests/keys/jwk_okp_key_Ed448.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)       90 2021-04-28 11:23:40.000000 PyJWT-2.6.0/tests/keys/jwk_okp_pub_Ed25519.json
+-rw-r--r--   0 jpadilla   (501) staff       (20)      183 2021-10-06 10:37:16.000000 PyJWT-2.6.0/tests/keys/jwk_okp_pub_Ed448.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)     1745 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/jwk_rsa_key.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      461 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/jwk_rsa_pub.json
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      451 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey2_rsa.pub.pem
+-rw-r--r--   0 jpadilla   (501) staff       (20)      241 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_ec.priv
+-rw-r--r--   0 jpadilla   (501) staff       (20)      178 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_ec.pub
+-rw-r--r--   0 jpadilla   (501) staff       (20)      209 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/keys/testkey_ec_secp192r1.priv
+-rw-r--r--   0 jpadilla   (501) staff       (20)      161 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_ec_ssh.pub
+-rw-r--r--   0 jpadilla   (501) staff       (20)      119 2020-08-24 14:15:08.000000 PyJWT-2.6.0/tests/keys/testkey_ed25519
+-rw-r--r--   0 jpadilla   (501) staff       (20)       81 2020-08-24 14:15:07.000000 PyJWT-2.6.0/tests/keys/testkey_ed25519.pub
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      247 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey_pkcs1.pub.pem
+-rw-rw-r--   0 jpadilla   (501) staff       (20)     1281 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey_rsa.cer
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1679 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/keys/testkey_rsa.priv
+-rw-rw-r--   0 jpadilla   (501) staff       (20)      401 2020-04-08 13:53:03.000000 PyJWT-2.6.0/tests/keys/testkey_rsa.pub
+-rw-r--r--   0 jpadilla   (501) staff       (20)     5022 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_advisory.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    38285 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_algorithms.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     9699 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_api_jwk.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    29203 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_api_jws.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    25097 2022-10-20 00:40:19.000000 PyJWT-2.6.0/tests/test_api_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      213 2019-10-22 15:57:44.000000 PyJWT-2.6.0/tests/test_exceptions.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)    12895 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tests/test_jwks_client.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      625 2020-08-24 16:22:55.000000 PyJWT-2.6.0/tests/test_jwt.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      897 2020-12-20 00:01:37.000000 PyJWT-2.6.0/tests/test_utils.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)      722 2021-10-06 10:37:16.000000 PyJWT-2.6.0/tests/utils.py
+-rw-r--r--   0 jpadilla   (501) staff       (20)     1427 2022-09-20 10:55:34.000000 PyJWT-2.6.0/tox.ini
```

### Comparing `PyJWT-2.5.0/.pre-commit-config.yaml` & `PyJWT-2.6.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 22.10.0
     hooks:
       - id: black
         args: ["--target-version=py37"]
 
   - repo: https://github.com/asottile/blacken-docs
     rev: v1.12.1
     hooks:
@@ -32,10 +32,10 @@
   - repo: https://github.com/mgedmin/check-manifest
     rev: "0.48"
     hooks:
       - id: check-manifest
         args: [--no-build-isolation]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v0.971"
+    rev: "v0.982"
     hooks:
       - id: mypy
```

### Comparing `PyJWT-2.5.0/CHANGELOG.rst` & `PyJWT-2.6.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,45 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.
 This project adheres to `Semantic Versioning <https://semver.org/>`__.
 
-`Unreleased <https://github.com/jpadilla/pyjwt/compare/2.5.0...HEAD>`__
+`Unreleased <https://github.com/jpadilla/pyjwt/compare/2.6.0...HEAD>`__
 -----------------------------------------------------------------------
 
 Changed
 ~~~~~~~
 
 Fixed
 ~~~~~
 
 Added
 ~~~~~
 
-`v2.4.0 <https://github.com/jpadilla/pyjwt/compare/2.4.0...2.5.0>`__
+`v2.6.0 <https://github.com/jpadilla/pyjwt/compare/2.5.0...2.6.0>`__
+-----------------------------------------------------------------------
+
+Changed
+~~~~~~~
+
+- bump up cryptography >= 3.4.0 by @jpadilla in `#807 <https://github.com/jpadilla/pyjwt/pull/807>`_
+- Remove `types-cryptography` from `crypto` extra by @lautat in `#805 <https://github.com/jpadilla/pyjwt/pull/805>`_
+
+Fixed
+~~~~~
+
+- Invalidate token on the exact second the token expires `#797 <https://github.com/jpadilla/pyjwt/pull/797>`_
+- fix: version 2.5.0 heading typo by @c0state in `#803 <https://github.com/jpadilla/pyjwt/pull/803>`_
+
+Added
+~~~~~
+- Adding validation for `issued_at` when `iat > (now + leeway)` as `ImmatureSignatureError` by @sriharan16 in https://github.com/jpadilla/pyjwt/pull/794
+
+`v2.5.0 <https://github.com/jpadilla/pyjwt/compare/2.4.0...2.5.0>`__
 -----------------------------------------------------------------------
 
 Changed
 ~~~~~~~
 
 - Skip keys with incompatible alg when loading JWKSet by @DaGuich in `#762 <https://github.com/jpadilla/pyjwt/pull/762>`__
 - Remove support for python3.6 by @sirosen in `#777 <https://github.com/jpadilla/pyjwt/pull/777>`__
```

### Comparing `PyJWT-2.5.0/CODE_OF_CONDUCT.md` & `PyJWT-2.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/LICENSE` & `PyJWT-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/PKG-INFO` & `PyJWT-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJWT
-Version: 2.5.0
+Version: 2.6.0
 Summary: JSON Web Token implementation in Python
 Home-page: https://github.com/jpadilla/pyjwt
 Author: Jose Padilla
 Author-email: hello@jpadilla.com
 License: MIT
 Description: PyJWT
         =====
@@ -81,11 +81,11 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: docs
+Provides-Extra: crypto
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: tests
-Provides-Extra: crypto
```

### Comparing `PyJWT-2.5.0/PyJWT.egg-info/PKG-INFO` & `PyJWT-2.6.0/PyJWT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJWT
-Version: 2.5.0
+Version: 2.6.0
 Summary: JSON Web Token implementation in Python
 Home-page: https://github.com/jpadilla/pyjwt
 Author: Jose Padilla
 Author-email: hello@jpadilla.com
 License: MIT
 Description: PyJWT
         =====
@@ -81,11 +81,11 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: docs
+Provides-Extra: crypto
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: tests
-Provides-Extra: crypto
```

### Comparing `PyJWT-2.5.0/PyJWT.egg-info/SOURCES.txt` & `PyJWT-2.6.0/PyJWT.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 PyJWT.egg-info/PKG-INFO
 PyJWT.egg-info/SOURCES.txt
 PyJWT.egg-info/dependency_links.txt
 PyJWT.egg-info/not-zip-safe
```

### Comparing `PyJWT-2.5.0/README.rst` & `PyJWT-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/Makefile` & `PyJWT-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/algorithms.rst` & `PyJWT-2.6.0/docs/algorithms.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/api.rst` & `PyJWT-2.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/conf.py` & `PyJWT-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/faq.rst` & `PyJWT-2.6.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/index.rst` & `PyJWT-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/installation.rst` & `PyJWT-2.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/docs/usage.rst` & `PyJWT-2.6.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/__init__.py` & `PyJWT-2.6.0/jwt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     PyJWKClientError,
     PyJWKError,
     PyJWKSetError,
     PyJWTError,
 )
 from .jwks_client import PyJWKClient
 
-__version__ = "2.5.0"
+__version__ = "2.6.0"
 
 __title__ = "PyJWT"
 __description__ = "JSON Web Token implementation in Python"
 __url__ = "https://pyjwt.readthedocs.io"
 __uri__ = __url__
 __doc__ = f"{__description__} <{__uri__}>"
```

### Comparing `PyJWT-2.5.0/jwt/algorithms.py` & `PyJWT-2.6.0/jwt/algorithms.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/api_jwk.py` & `PyJWT-2.6.0/jwt/api_jwk.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/api_jws.py` & `PyJWT-2.6.0/jwt/api_jws.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/api_jwt.py` & `PyJWT-2.6.0/jwt/api_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,21 @@
 
     def _validate_required_claims(self, payload, options):
         for claim in options["require"]:
             if payload.get(claim) is None:
                 raise MissingRequiredClaimError(claim)
 
     def _validate_iat(self, payload, now, leeway):
+        iat = payload["iat"]
         try:
-            int(payload["iat"])
+            int(iat)
         except ValueError:
             raise InvalidIssuedAtError("Issued At claim (iat) must be an integer.")
+        if iat > (now + leeway):
+            raise ImmatureSignatureError("The token is not yet valid (iat)")
 
     def _validate_nbf(self, payload, now, leeway):
         try:
             nbf = int(payload["nbf"])
         except ValueError:
             raise DecodeError("Not Before claim (nbf) must be an integer.")
 
@@ -226,15 +229,15 @@
 
     def _validate_exp(self, payload, now, leeway):
         try:
             exp = int(payload["exp"])
         except ValueError:
             raise DecodeError("Expiration Time claim (exp) must be an" " integer.")
 
-        if exp < (now - leeway):
+        if exp <= (now - leeway):
             raise ExpiredSignatureError("Signature has expired")
 
     def _validate_aud(self, payload, audience):
         if audience is None:
             if "aud" not in payload or not payload["aud"]:
                 return
             # Application did not specify an audience, but
```

### Comparing `PyJWT-2.5.0/jwt/exceptions.py` & `PyJWT-2.6.0/jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/help.py` & `PyJWT-2.6.0/jwt/help.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/jwk_set_cache.py` & `PyJWT-2.6.0/jwt/jwk_set_cache.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/jwks_client.py` & `PyJWT-2.6.0/jwt/jwks_client.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/jwt/utils.py` & `PyJWT-2.6.0/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/setup.cfg` & `PyJWT-2.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,23 @@
 
 [options.extras_require]
 docs = 
 	sphinx>=4.5.0,<5.0.0
 	sphinx-rtd-theme
 	zope.interface
 crypto = 
-	cryptography>=3.3.1
-	types-cryptography>=3.3.21
+	cryptography>=3.4.0
 tests = 
 	pytest>=6.0.0,<7.0.0
 	coverage[toml]==5.0.4
 dev = 
 	sphinx>=4.5.0,<5.0.0
 	sphinx-rtd-theme
 	zope.interface
-	cryptography>=3.3.1
-	types-cryptography>=3.3.21
+	cryptography>=3.4.0
 	pytest>=6.0.0,<7.0.0
 	coverage[toml]==5.0.4
 	pre-commit
 
 [options.packages.find]
 exclude = 
 	tests
```

### Comparing `PyJWT-2.5.0/tests/keys/__init__.py` & `PyJWT-2.6.0/tests/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/keys/jwk_keyset_only_unknown_alg.json` & `PyJWT-2.6.0/tests/keys/jwk_keyset_only_unknown_alg.json`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/keys/jwk_keyset_with_unknown_alg.json` & `PyJWT-2.6.0/tests/keys/jwk_keyset_with_unknown_alg.json`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/keys/jwk_rsa_key.json` & `PyJWT-2.6.0/tests/keys/jwk_rsa_key.json`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/keys/testkey_rsa.cer` & `PyJWT-2.6.0/tests/keys/testkey_rsa.cer`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/keys/testkey_rsa.priv` & `PyJWT-2.6.0/tests/keys/testkey_rsa.priv`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_advisory.py` & `PyJWT-2.6.0/tests/test_advisory.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_algorithms.py` & `PyJWT-2.6.0/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_api_jwk.py` & `PyJWT-2.6.0/tests/test_api_jwk.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_api_jws.py` & `PyJWT-2.6.0/tests/test_api_jws.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_api_jwt.py` & `PyJWT-2.6.0/tests/test_api_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,22 @@
             "eyJpYXQiOiJub3QtYW4taW50In0."
             "H1GmcQgSySa5LOKYbzGm--b1OmRbHFkyk8pq811FzZM"
         )
 
         with pytest.raises(InvalidIssuedAtError):
             jwt.decode(example_jwt, "secret", algorithms=["HS256"])
 
+    def test_decode_raises_exception_if_iat_is_greater_than_now(self, jwt, payload):
+        payload["iat"] = utc_timestamp() + 10
+        secret = "secret"
+        jwt_message = jwt.encode(payload, secret)
+
+        with pytest.raises(ImmatureSignatureError):
+            jwt.decode(jwt_message, secret, algorithms=["HS256"])
+
     def test_decode_raises_exception_if_nbf_is_not_int(self, jwt):
         # >>> jwt.encode({'nbf': 'not-an-int'}, 'secret')
         example_jwt = (
             "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9."
             "eyJuYmYiOiJub3QtYW4taW50In0."
             "c25hldC8G2ZamC8uKpax9sYMTgdZo3cxrmzFHaAAluw"
         )
```

### Comparing `PyJWT-2.5.0/tests/test_jwks_client.py` & `PyJWT-2.6.0/tests/test_jwks_client.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_jwt.py` & `PyJWT-2.6.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/test_utils.py` & `PyJWT-2.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tests/utils.py` & `PyJWT-2.6.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `PyJWT-2.5.0/tox.ini` & `PyJWT-2.6.0/tox.ini`

 * *Files identical despite different names*

