# Comparing `tmp/acme-2.5.0.tar.gz` & `tmp/acme-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acme-2.5.0.tar", last modified: Tue Apr  4 15:07:02 2023, max compression
+gzip compressed data, was "acme-2.6.0.tar", last modified: Tue May  9 19:44:41 2023, max compression
```

## Comparing `acme-2.5.0.tar` & `acme-2.6.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 acme-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      236 2023-04-04 15:06:41.000000 acme-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)      905 2023-04-04 15:07:02.000000 acme-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       39 2023-04-04 15:06:41.000000 acme-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/acme/
--rw-r--r--   0 bmw        (501) staff       (20)      736 2023-04-04 15:06:41.000000 acme-2.5.0/acme/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/acme/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       37 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/acme/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       17 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)    18961 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/challenges_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    34794 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/client_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    13513 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/crypto_util_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     1534 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/errors_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     1719 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/fields_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     1839 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/jose_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     2082 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/jws_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    19730 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/messages_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     9671 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/standalone_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     2392 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/test_util.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/acme/_internal/tests/testdata/
--rw-r--r--   0 bmw        (501) staff       (20)      858 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/README
--rw-r--r--   0 bmw        (501) staff       (20)     2752 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert-100sans.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1866 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert-idnsans.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1289 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert-ipsans.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1310 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert-ipv6sans.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1397 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert-nocn.der
--rw-r--r--   0 bmw        (501) staff       (20)      786 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert-san.pem
--rw-r--r--   0 bmw        (501) staff       (20)      771 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert.der
--rw-r--r--   0 bmw        (501) staff       (20)      709 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/cert.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1683 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/critical-san.pem
--rw-r--r--   0 bmw        (501) staff       (20)     2577 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-100sans.pem
--rw-r--r--   0 bmw        (501) staff       (20)      676 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-6sans.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1691 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-idnsans.pem
--rw-r--r--   0 bmw        (501) staff       (20)      920 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-ipsans.pem
--rw-r--r--   0 bmw        (501) staff       (20)      952 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-ipv6sans.pem
--rw-r--r--   0 bmw        (501) staff       (20)      932 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-mixed.pem
--rw-r--r--   0 bmw        (501) staff       (20)      452 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-nosans.pem
--rw-r--r--   0 bmw        (501) staff       (20)      574 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr-san.pem
--rw-r--r--   0 bmw        (501) staff       (20)      607 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr.der
--rw-r--r--   0 bmw        (501) staff       (20)      550 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/csr.pem
--rw-r--r--   0 bmw        (501) staff       (20)      684 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/dsa512_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)      306 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/ec_secp384r1_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)      749 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa1024_cert.pem
--rw-r--r--   0 bmw        (501) staff       (20)      887 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa1024_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1294 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa2048_cert.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1704 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa2048_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)      298 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa256_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)     1814 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa4096_cert.pem
--rw-r--r--   0 bmw        (501) staff       (20)     3247 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa4096_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)      493 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/testdata/rsa512_key.pem
--rw-r--r--   0 bmw        (501) staff       (20)      396 2023-04-04 15:06:41.000000 acme-2.5.0/acme/_internal/tests/util_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    22456 2023-04-04 15:06:41.000000 acme-2.5.0/acme/challenges.py
--rw-r--r--   0 bmw        (501) staff       (20)    31163 2023-04-04 15:06:41.000000 acme-2.5.0/acme/client.py
--rw-r--r--   0 bmw        (501) staff       (20)    17799 2023-04-04 15:06:41.000000 acme-2.5.0/acme/crypto_util.py
--rw-r--r--   0 bmw        (501) staff       (20)     4315 2023-04-04 15:06:41.000000 acme-2.5.0/acme/errors.py
--rw-r--r--   0 bmw        (501) staff       (20)     1652 2023-04-04 15:06:41.000000 acme-2.5.0/acme/fields.py
--rw-r--r--   0 bmw        (501) staff       (20)     2624 2023-04-04 15:06:41.000000 acme-2.5.0/acme/jws.py
--rw-r--r--   0 bmw        (501) staff       (20)    26242 2023-04-04 15:06:41.000000 acme-2.5.0/acme/messages.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 acme-2.5.0/acme/py.typed
--rw-r--r--   0 bmw        (501) staff       (20)    12983 2023-04-04 15:06:41.000000 acme-2.5.0/acme/standalone.py
--rw-r--r--   0 bmw        (501) staff       (20)      303 2023-04-04 15:06:41.000000 acme-2.5.0/acme/util.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/acme.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)      905 2023-04-04 15:07:02.000000 acme-2.5.0/acme.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)     2514 2023-04-04 15:07:02.000000 acme-2.5.0/acme.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:02.000000 acme-2.5.0/acme.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)      204 2023-04-04 15:07:02.000000 acme-2.5.0/acme.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)        5 2023-04-04 15:07:02.000000 acme-2.5.0/acme.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 acme-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)     7434 2023-04-04 15:06:41.000000 acme-2.5.0/docs/Makefile
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/docs/_static/
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 acme-2.5.0/docs/_static/.gitignore
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/docs/_templates/
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 acme-2.5.0/docs/_templates/.gitignore
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/docs/api/
--rw-r--r--   0 bmw        (501) staff       (20)       68 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/challenges.rst
--rw-r--r--   0 bmw        (501) staff       (20)       56 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/client.rst
--rw-r--r--   0 bmw        (501) staff       (20)       56 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/errors.rst
--rw-r--r--   0 bmw        (501) staff       (20)       56 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/fields.rst
--rw-r--r--   0 bmw        (501) staff       (20)      161 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/jose.rst
--rw-r--r--   0 bmw        (501) staff       (20)       62 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/messages.rst
--rw-r--r--   0 bmw        (501) staff       (20)       68 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api/standalone.rst
--rw-r--r--   0 bmw        (501) staff       (20)       88 2023-04-04 15:06:41.000000 acme-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)    10224 2023-04-04 15:06:41.000000 acme-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      479 2023-04-04 15:06:41.000000 acme-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      156 2023-04-04 15:06:41.000000 acme-2.5.0/docs/jws-help.txt
--rw-r--r--   0 bmw        (501) staff       (20)     7259 2023-04-04 15:06:41.000000 acme-2.5.0/docs/make.bat
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/docs/man/
--rw-r--r--   0 bmw        (501) staff       (20)       46 2023-04-04 15:06:41.000000 acme-2.5.0/docs/man/jws.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:02.000000 acme-2.5.0/examples/
--rw-r--r--   0 bmw        (501) staff       (20)     7123 2023-04-04 15:06:41.000000 acme-2.5.0/examples/http01_example.py
--rw-r--r--   0 bmw        (501) staff       (20)       63 2023-04-04 15:06:41.000000 acme-2.5.0/pytest.ini
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:02.000000 acme-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     1649 2023-04-04 15:06:42.000000 acme-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 acme-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      236 2023-05-09 19:44:36.000000 acme-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)      905 2023-05-09 19:44:41.127784 acme-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       39 2023-05-09 19:44:36.000000 acme-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.123785 acme-2.6.0/acme/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      736 2023-05-09 19:44:36.000000 acme-2.6.0/acme/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.123785 acme-2.6.0/acme/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       37 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.123785 acme-2.6.0/acme/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       17 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18961 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/challenges_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    34794 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/client_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13489 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/crypto_util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1534 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/errors_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1719 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/fields_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1839 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/jose_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2082 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/jws_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    19730 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/messages_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9928 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/standalone_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2392 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/test_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.123785 acme-2.6.0/acme/_internal/tests/testdata/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      858 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/README
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2752 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert-100sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1866 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert-idnsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1289 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert-ipsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1310 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert-ipv6sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1397 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert-nocn.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      786 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert-san.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      771 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      709 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1683 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/critical-san.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2577 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-100sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      676 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-6sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1691 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-idnsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      920 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-ipsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      952 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-ipv6sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      932 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-mixed.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      452 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-nosans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      574 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr-san.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      607 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      550 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/csr.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      684 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/dsa512_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      306 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/ec_secp384r1_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      749 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa1024_cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      887 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa1024_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1294 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa2048_cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1704 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa2048_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      298 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa256_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1814 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa4096_cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3247 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa4096_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      493 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/testdata/rsa512_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      396 2023-05-09 19:44:36.000000 acme-2.6.0/acme/_internal/tests/util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22456 2023-05-09 19:44:36.000000 acme-2.6.0/acme/challenges.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    31163 2023-05-09 19:44:36.000000 acme-2.6.0/acme/client.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18051 2023-05-09 19:44:36.000000 acme-2.6.0/acme/crypto_util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4315 2023-05-09 19:44:36.000000 acme-2.6.0/acme/errors.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1652 2023-05-09 19:44:36.000000 acme-2.6.0/acme/fields.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2624 2023-05-09 19:44:36.000000 acme-2.6.0/acme/jws.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    26242 2023-05-09 19:44:36.000000 acme-2.6.0/acme/messages.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 acme-2.6.0/acme/py.typed
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12983 2023-05-09 19:44:36.000000 acme-2.6.0/acme/standalone.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      303 2023-05-09 19:44:36.000000 acme-2.6.0/acme/util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.123785 acme-2.6.0/acme.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      905 2023-05-09 19:44:41.000000 acme-2.6.0/acme.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2514 2023-05-09 19:44:41.000000 acme-2.6.0/acme.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:41.000000 acme-2.6.0/acme.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      204 2023-05-09 19:44:41.000000 acme-2.6.0/acme.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        5 2023-05-09 19:44:41.000000 acme-2.6.0/acme.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 acme-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7434 2023-05-09 19:44:36.000000 acme-2.6.0/docs/Makefile
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/docs/_static/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 acme-2.6.0/docs/_static/.gitignore
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/docs/_templates/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 acme-2.6.0/docs/_templates/.gitignore
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/docs/api/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       68 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/challenges.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       56 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/client.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       56 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/errors.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       56 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/fields.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      161 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/jose.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       62 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/messages.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       68 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api/standalone.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       88 2023-05-09 19:44:36.000000 acme-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10224 2023-05-09 19:44:36.000000 acme-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      479 2023-05-09 19:44:36.000000 acme-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      167 2023-05-09 19:44:36.000000 acme-2.6.0/docs/jws-help.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7259 2023-05-09 19:44:36.000000 acme-2.6.0/docs/make.bat
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/docs/man/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2023-05-09 19:44:36.000000 acme-2.6.0/docs/man/jws.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:41.127784 acme-2.6.0/examples/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7123 2023-05-09 19:44:36.000000 acme-2.6.0/examples/http01_example.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)       63 2023-05-09 19:44:36.000000 acme-2.6.0/pytest.ini
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:41.127784 acme-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1649 2023-05-09 19:44:37.000000 acme-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `acme-2.5.0/LICENSE.txt` & `acme-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/PKG-INFO` & `acme-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acme
-Version: 2.5.0
+Version: 2.6.0
 Summary: ACME protocol implementation in Python
 Home-page: https://github.com/letsencrypt/letsencrypt
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `acme-2.5.0/acme/__init__.py` & `acme-2.6.0/acme/__init__.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/challenges_test.py` & `acme-2.6.0/acme/_internal/tests/challenges_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/client_test.py` & `acme-2.6.0/acme/_internal/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/crypto_util_test.py` & `acme-2.6.0/acme/_internal/tests/crypto_util_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,28 @@
         key = test_util.load_pyopenssl_private_key('rsa2048_key.pem')
         # pylint: disable=protected-access
         certs = {b'foo': (key, self.cert.wrapped)}
 
         from acme.crypto_util import SSLSocket
 
         class _TestServer(socketserver.TCPServer):
-
-            def server_bind(self):  # pylint: disable=missing-docstring
-                self.socket = SSLSocket(socket.socket(),
-                        certs)
-                socketserver.TCPServer.server_bind(self)
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.socket = SSLSocket(self.socket, certs)
 
         self.server = _TestServer(('', 0), socketserver.BaseRequestHandler)
         self.port = self.server.socket.getsockname()[1]
         self.server_thread = threading.Thread(
             target=self.server.handle_request)
 
     def tearDown(self):
         if self.server_thread.is_alive():
             # The thread may have already terminated.
             self.server_thread.join()  # pragma: no cover
+        self.server.server_close()
 
     def _probe(self, name):
         from acme.crypto_util import probe_sni
         return jose.ComparableX509(probe_sni(
             name, host='127.0.0.1', port=self.port))
 
     def _start_server(self):
```

### Comparing `acme-2.5.0/acme/_internal/tests/errors_test.py` & `acme-2.6.0/acme/_internal/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/fields_test.py` & `acme-2.6.0/acme/_internal/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/jose_test.py` & `acme-2.6.0/acme/_internal/tests/jose_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/jws_test.py` & `acme-2.6.0/acme/_internal/tests/jws_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/messages_test.py` & `acme-2.6.0/acme/_internal/tests/messages_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/standalone_test.py` & `acme-2.6.0/acme/_internal/tests/standalone_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self.port = self.server.socket.getsockname()[1]
         self.thread = threading.Thread(target=self.server.serve_forever)
         self.thread.start()
 
     def tearDown(self):
         self.server.shutdown()
         self.thread.join()
+        self.server.server_close()
 
     def test_index(self):
         response = requests.get(
             'http://localhost:{0}'.format(self.port), verify=False)
         assert response.text == 'ACME client standalone challenge solver'
         assert response.ok
 
@@ -84,33 +85,33 @@
         assert self._test_http01(add=True)
 
     def test_http01_not_found(self):
         assert not self._test_http01(add=False)
 
     def test_timely_shutdown(self):
         from acme.standalone import HTTP01Server
-        server = HTTP01Server(('', 0), resources=set(), timeout=0.05)
-        server_thread = threading.Thread(target=server.serve_forever)
-        server_thread.start()
-
-        client = socket.socket()
-        client.connect(('localhost', server.socket.getsockname()[1]))
-
-        stop_thread = threading.Thread(target=server.shutdown)
-        stop_thread.start()
-        server_thread.join(5.)
-
-        is_hung = server_thread.is_alive()
-        try:
-            client.shutdown(socket.SHUT_RDWR)
-        except: # pragma: no cover, pylint: disable=bare-except
-            # may raise error because socket could already be closed
-            pass
+        with HTTP01Server(('', 0), resources=set(), timeout=0.05) as server:
+            server_thread = threading.Thread(target=server.serve_forever)
+            server_thread.start()
+
+            with socket.socket() as client:
+                client.connect(('localhost', server.socket.getsockname()[1]))
+
+                stop_thread = threading.Thread(target=server.shutdown)
+                stop_thread.start()
+                server_thread.join(5.)
 
-        assert not is_hung, 'Server shutdown should not be hung'
+                is_hung = server_thread.is_alive()
+                try:
+                    client.shutdown(socket.SHUT_RDWR)
+                except: # pragma: no cover, pylint: disable=bare-except
+                    # may raise error because socket could already be closed
+                    pass
+
+                assert not is_hung, 'Server shutdown should not be hung'
 
 
 @unittest.skipIf(not challenges.TLSALPN01.is_supported(), "pyOpenSSL too old")
 class TLSALPN01ServerTest(unittest.TestCase):
     """Test for acme.standalone.TLSALPN01Server."""
 
     def setUp(self):
@@ -129,14 +130,15 @@
         # pylint: disable=no-member
         self.thread = threading.Thread(target=self.server.serve_forever)
         self.thread.start()
 
     def tearDown(self):
         self.server.shutdown()  # pylint: disable=no-member
         self.thread.join()
+        self.server.server_close()
 
     # TODO: This is not implemented yet, see comments in standalone.py
     # def test_certs(self):
     #    host, port = self.server.socket.getsockname()[:2]
     #    cert = crypto_util.probe_sni(
     #        b'localhost', host=host, port=port, timeout=1)
     #    # Expect normal cert when connecting without ALPN.
@@ -210,14 +212,16 @@
         prev_port = None
         # assert ports are equal
         for sockname in socknames:
             port = sockname[1]
             if prev_port:
                 assert prev_port == port
             prev_port = port
+        for server in servers.servers:
+            server.server_close()
 
 
 class HTTP01DualNetworkedServersTest(unittest.TestCase):
     """Tests for acme.standalone.HTTP01DualNetworkedServers."""
 
     def setUp(self):
         self.account_key = jose.JWK.load(
```

### Comparing `acme-2.5.0/acme/_internal/tests/test_util.py` & `acme-2.6.0/acme/_internal/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/README` & `acme-2.6.0/acme/_internal/tests/testdata/README`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert-100sans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/cert-100sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert-idnsans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/cert-idnsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert-ipsans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/cert-ipsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert-ipv6sans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/cert-ipv6sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert-nocn.der` & `acme-2.6.0/acme/_internal/tests/testdata/cert-nocn.der`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert-san.pem` & `acme-2.6.0/acme/_internal/tests/testdata/cert-san.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert.der` & `acme-2.6.0/acme/_internal/tests/testdata/cert.der`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/cert.pem` & `acme-2.6.0/acme/_internal/tests/testdata/cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/critical-san.pem` & `acme-2.6.0/acme/_internal/tests/testdata/critical-san.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-100sans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-100sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-6sans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-6sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-idnsans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-idnsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-ipsans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-ipsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-ipv6sans.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-ipv6sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-mixed.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-mixed.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr-san.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr-san.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr.der` & `acme-2.6.0/acme/_internal/tests/testdata/csr.der`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/csr.pem` & `acme-2.6.0/acme/_internal/tests/testdata/csr.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/dsa512_key.pem` & `acme-2.6.0/acme/_internal/tests/testdata/dsa512_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/rsa1024_cert.pem` & `acme-2.6.0/acme/_internal/tests/testdata/rsa1024_cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/rsa1024_key.pem` & `acme-2.6.0/acme/_internal/tests/testdata/rsa1024_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/rsa2048_cert.pem` & `acme-2.6.0/acme/_internal/tests/testdata/rsa2048_cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/rsa2048_key.pem` & `acme-2.6.0/acme/_internal/tests/testdata/rsa2048_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/rsa4096_cert.pem` & `acme-2.6.0/acme/_internal/tests/testdata/rsa4096_cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/_internal/tests/testdata/rsa4096_key.pem` & `acme-2.6.0/acme/_internal/tests/testdata/rsa4096_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/challenges.py` & `acme-2.6.0/acme/challenges.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/client.py` & `acme-2.6.0/acme/client.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/crypto_util.py` & `acme-2.6.0/acme/crypto_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,35 +132,41 @@
                 # used by code which expects a standard socket such as
                 # socketserver in the standard library.
                 raise socket.error(error)
 
     def accept(self) -> Tuple[FakeConnection, Any]:  # pylint: disable=missing-function-docstring
         sock, addr = self.sock.accept()
 
-        context = SSL.Context(self.method)
-        context.set_options(SSL.OP_NO_SSLv2)
-        context.set_options(SSL.OP_NO_SSLv3)
-        context.set_tlsext_servername_callback(self._pick_certificate_cb)
-        if self.alpn_selection is not None:
-            context.set_alpn_select_callback(self.alpn_selection)
-
-        ssl_sock = self.FakeConnection(SSL.Connection(context, sock))
-        ssl_sock.set_accept_state()
-
-        # This log line is especially desirable because without it requests to
-        # our standalone TLSALPN server would not be logged.
-        logger.debug("Performing handshake with %s", addr)
         try:
-            ssl_sock.do_handshake()
-        except SSL.Error as error:
-            # _pick_certificate_cb might have returned without
-            # creating SSL context (wrong server name)
-            raise socket.error(error)
+            context = SSL.Context(self.method)
+            context.set_options(SSL.OP_NO_SSLv2)
+            context.set_options(SSL.OP_NO_SSLv3)
+            context.set_tlsext_servername_callback(self._pick_certificate_cb)
+            if self.alpn_selection is not None:
+                context.set_alpn_select_callback(self.alpn_selection)
+
+            ssl_sock = self.FakeConnection(SSL.Connection(context, sock))
+            ssl_sock.set_accept_state()
+
+            # This log line is especially desirable because without it requests to
+            # our standalone TLSALPN server would not be logged.
+            logger.debug("Performing handshake with %s", addr)
+            try:
+                ssl_sock.do_handshake()
+            except SSL.Error as error:
+                # _pick_certificate_cb might have returned without
+                # creating SSL context (wrong server name)
+                raise socket.error(error)
 
-        return ssl_sock, addr
+            return ssl_sock, addr
+        except:
+            # If we encounter any error, close the new socket before reraising
+            # the exception.
+            sock.close()
+            raise
 
 
 def probe_sni(name: bytes, host: bytes, port: int = 443, timeout: int = 300,  # pylint: disable=too-many-arguments
               method: int = _DEFAULT_SSL_METHOD, source_address: Tuple[str, int] = ('', 0),
               alpn_protocols: Optional[Sequence[bytes]] = None) -> crypto.X509:
     """Probe SNI server for SSL certificate.
```

### Comparing `acme-2.5.0/acme/errors.py` & `acme-2.6.0/acme/errors.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/fields.py` & `acme-2.6.0/acme/fields.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/jws.py` & `acme-2.6.0/acme/jws.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/messages.py` & `acme-2.6.0/acme/messages.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme/standalone.py` & `acme-2.6.0/acme/standalone.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/acme.egg-info/PKG-INFO` & `acme-2.6.0/acme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acme
-Version: 2.5.0
+Version: 2.6.0
 Summary: ACME protocol implementation in Python
 Home-page: https://github.com/letsencrypt/letsencrypt
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `acme-2.5.0/acme.egg-info/SOURCES.txt` & `acme-2.6.0/acme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/docs/Makefile` & `acme-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/docs/conf.py` & `acme-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/docs/make.bat` & `acme-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/examples/http01_example.py` & `acme-2.6.0/examples/http01_example.py`

 * *Files identical despite different names*

### Comparing `acme-2.5.0/setup.py` & `acme-2.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.5.0'
+version = '2.6.0'
 
 install_requires = [
-    'cryptography>=2.5.0',
+    'cryptography>=3.2.1',
     'josepy>=1.13.0',
     # pyOpenSSL 23.1.0 is a bad release: https://github.com/pyca/pyopenssl/issues/1199
     'PyOpenSSL>=17.5.0,!=23.1.0',
     'pyrfc3339',
     'pytz>=2019.3',
     'requests>=2.20.0',
     'setuptools>=41.6.0',
```

