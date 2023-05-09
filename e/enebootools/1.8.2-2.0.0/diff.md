# Comparing `tmp/enebootools-1.8.2.tar.gz` & `tmp/enebootools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-1.8.2.tar", last modified: Tue Apr 18 07:12:10 2023, max compression
+gzip compressed data, was "enebootools-2.0.0.tar", last modified: Tue May  9 13:18:26 2023, max compression
```

## Comparing `enebootools-1.8.2.tar` & `enebootools-2.0.0.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.851783 enebootools-1.8.2/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-1.8.2/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-1.8.2/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-04-18 07:12:10.847783 enebootools-1.8.2/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-1.8.2/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-04-18 07:10:33.000000 enebootools-1.8.2/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-1.8.2/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6000 2022-12-07 09:30:25.000000 enebootools-1.8.2/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29507 2022-12-01 09:57:04.000000 enebootools-1.8.2/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-1.8.2/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23152 2023-04-18 07:09:46.000000 enebootools-1.8.2/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-1.8.2/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-1.8.2/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-1.8.2/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-1.8.2/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-1.8.2/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-1.8.2/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26266 2022-04-29 09:06:06.000000 enebootools-1.8.2/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31100 2023-03-08 13:14:00.000000 enebootools-1.8.2/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-1.8.2/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-1.8.2/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76823 2022-09-28 07:55:10.000000 enebootools-1.8.2/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-1.8.2/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-1.8.2/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-1.8.2/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-1.8.2/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-1.8.2/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-1.8.2/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-1.8.2/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-1.8.2/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-1.8.2/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-1.8.2/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2836 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-04-18 07:12:10.851783 enebootools-1.8.2/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-1.8.2/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.0/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.0/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-09 13:18:26.113034 enebootools-2.0.0/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.0/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-09 13:16:06.000000 enebootools-2.0.0/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.0/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6000 2022-12-07 09:30:25.000000 enebootools-2.0.0/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29507 2022-12-01 09:57:04.000000 enebootools-2.0.0/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.0/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23182 2023-05-09 13:12:22.000000 enebootools-2.0.0/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.0/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.0/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.0/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.0/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.0/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.0/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.0/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76864 2023-05-09 12:45:28.000000 enebootools-2.0.0/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31272 2023-05-09 12:42:28.000000 enebootools-2.0.0/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-2.0.0/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.0/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.0/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-2.0.0/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.0/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-2.0.0/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.0/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.0/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.0/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.0/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.0/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.0/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.0/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-09 13:18:26.000000 enebootools-2.0.0/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-09 13:18:26.113034 enebootools-2.0.0/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.0/setup.py
```

### Comparing `enebootools-1.8.2/LICENSE.gplv3` & `enebootools-2.0.0/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/PKG-INFO` & `enebootools-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 1.8.2
+Version: 2.0.0
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-1.8.2/README.rst` & `enebootools-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/__init__.py` & `enebootools-2.0.0/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "1.8.2"
+__VERSION__ = "2.0.0"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-1.8.2/enebootools/__init__.pyc` & `enebootools-2.0.0/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/__init__.py` & `enebootools-2.0.0/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/config.py` & `enebootools-2.0.0/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/database.py` & `enebootools-2.0.0/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/databasemodels.py` & `enebootools-2.0.0/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/featureconfig.py` & `enebootools-2.0.0/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/kobjects.py` & `enebootools-2.0.0/enebootools/assembler/kobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,30 +103,32 @@
         self.all_required_features = self._get_full_required_features()
 
         for featname in self.all_required_features:
             obj = FeatureObject.find(featname)
             if obj is None:
                 self.iface.info("Funcionalidad con nombre %s no encontrada" % featname)
                 continue
+
             new_reqs = [
                 modulename
                 for modulename in obj._get_full_required_modules()
-                if modulename not in req
+                if modulename not in req and modulename not in myreq
             ]
             if self.type == "prj":
                 for n in new_reqs:
                     if n in self.required_modules:
                         continue
                     self.iface.debug(
                         "Proyecto %s, se agrega modulo %s solicitado por funcionalidad %s"
                         % (self.formal_name(), n, featname)
                     )
             req += new_reqs
 
         req += [modulename for modulename in myreq if modulename not in req]
+
         self.all_required_modules = req
         return req
 
     def _get_full_required_features(self):
         if self.all_required_features:
             return self.all_required_features
         req = []
```

### Comparing `enebootools-1.8.2/enebootools/assembler/mypeewee.py` & `enebootools-2.0.0/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/assembler/save_auto.py` & `enebootools-2.0.0/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/autoconfig/autoconfig.py` & `enebootools-2.0.0/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/autoconfig/parsers.py` & `enebootools-2.0.0/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/__init__.py` & `enebootools-2.0.0/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.0.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.0.0/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.0.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/certificates/README.txt` & `enebootools-2.0.0/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/crypto/main.py` & `enebootools-2.0.0/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.0.0/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/entry_points.py` & `enebootools-2.0.0/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/extracttool/__init__.py` & `enebootools-2.0.0/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/extracttool/extractfunctions.py` & `enebootools-2.0.0/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.0.0/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/lib/etree/ElementPath.py` & `enebootools-2.0.0/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/lib/etree/ElementTree.py` & `enebootools-2.0.0/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/lib/etree/__init__.py` & `enebootools-2.0.0/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/lib/peewee.py` & `enebootools-2.0.0/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/lib/utils.py` & `enebootools-2.0.0/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/__init__.py` & `enebootools-2.0.0/enebootools/mergetool/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # encoding: UTF-8
 import enebootools
 from enebootools import EnebooToolsInterface
 import traceback
 
 
-from enebootools.mergetool import flpatchqs, flpatchpy, flpatchtest, flpatchmodel, flpatchxml, flpatchlxml, flpatchdir, projectbuilder
+from enebootools.mergetool import (
+    flpatchqs,
+    flpatchpy,
+    flpatchtest,
+    flpatchmodel,
+    flpatchxml,
+    flpatchlxml,
+    flpatchdir,
+    projectbuilder,
+    flpatchapipy,
+)
 
 """
     El receptor de las llamadas del parser es una clase. Cada opción
     activada, genera una llamada en una función de la clase y así va 
     configurando la clase con cada llamada consecutiva.
     
     Esta clase está a nivel de módulo (mergetool) y es la interfaz
@@ -56,276 +66,292 @@
         existe, argumentos no válidos... etc)
     
 """
 
 
 class MergeToolInterface(EnebooToolsInterface):
     module_description = "Herramientas para la ayuda de resolución de conflictos de mezcla"
-    def __init__(self, setup_parser = True):
+
+    def __init__(self, setup_parser=True):
         EnebooToolsInterface.__init__(self, False)
         self.patch_qs_rewrite = "warn"
         self.patch_py_rewrite = "warn"
         self.patch_test_rewrite = "warn"
         self.patch_model_rewrite = "warn"
         self.patch_xml_style_name = "legacy1"
         self.patch_qs_style_name = "legacy"
         self.patch_py_style_name = "legacy"
         self.patch_test_style_name = "legacy"
         self.patch_model_style_name = "legacy"
         self.diff_xml_search_move = False
         self.patch_name = None
         self.patch_dest = None
         self.clean_patch = False
-        if setup_parser: self.setup_parser()
-        
+        if setup_parser:
+            self.setup_parser()
+
     def setup_parser(self):
         EnebooToolsInterface.setup_parser(self)
         self.parser.declare_option(
-            name = "patch-qs-rewrite",
-            description = "indica si al aplicar un parche de QS se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
-            level = "action",
-            variable = "VALUE", 
-            call_function = self.set_patch_qs_rewrite
-            )
-        self.parser.declare_option(
-            name = "patch-py-rewrite",
-            description = "indica si al aplicar un parche de PY se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
-            level = "action",
-            variable = "VALUE", 
-            call_function = self.set_patch_py_rewrite
-            )
-        self.parser.declare_option(
-            name = "patch-test-rewrite",
-            description = "indica si al aplicar un parche de PY_test se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
-            level = "action",
-            variable = "VALUE", 
-            call_function = self.set_patch_test_rewrite
-            )
-        self.parser.declare_option(
-            name = "patch-model-rewrite",
-            description = "indica si al aplicar un parche de PY_model se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
-            level = "action",
-            variable = "VALUE", 
-            call_function = self.set_patch_model_rewrite
-            )
-        self.parser.declare_option(
-            name = "patch-name",
-            description = "Indica el nombre del parche que se usará en lugar de autodetectarlo.",
-            level = "action",
-            variable = "NAME", 
-            call_function = self.set_patch_name
-            )
-        self.parser.declare_option(
-            name = "patch-dest",
-            description = "Donde guardar un fichero de parche",
-            level = "action",
-            variable = "FILENAME", 
-            call_function = self.set_patch_dest
-            )
-        self.parser.declare_option(
-            name = "enable-diff-xml-search-move",
-            description = "Activa la búsqueda de movimientos de bloques XML. Puede ser un poco más lento y puede generar parches incompatibles con otras herramientas.",
-            level = "action",
-            call_function = self.enable_diff_xml_search_move
-            )
-        self.parser.declare_option(
-            name = "patch-xml-style",
-            description = "Usar otro estilo para generar parches XML (ver mergetools/etc/patch-styles/)",
-            variable = "NAME", 
-            level = "action",
-            call_function = self.set_patch_xml_style
-            )
-        self.parser.declare_option(
-            name = "patch-qs-style",
-            description = "Usar otro estilo para generar parches QS (legacy|qsdir)",
-            variable = "NAME", 
-            level = "action",
-            call_function = self.set_patch_qs_style
-            )
-        self.parser.declare_option(
-            name = "patch-py-style",
-            description = "Usar otro estilo para generar parches PY (legacy|pydir)",
-            variable = "NAME", 
-            level = "action",
-            call_function = self.set_patch_py_style
-            )
-        self.parser.declare_option(
-            name = "patch-test-style",
-            description = "Usar otro estilo para generar parches PY_test (legacy|testdir)",
-            variable = "NAME", 
-            level = "action",
-            call_function = self.set_patch_test_style
-            )
-        self.parser.declare_option(
-            name = "patch-model-style",
-            description = "Usar otro estilo para generar parches PY_model (legacy|modeldir)",
-            variable = "NAME", 
-            level = "action",
-            call_function = self.set_patch_model_style
-            )
-        self.parser.declare_option(
-            name = "clean-patch",
-            description = "provoca que el parche generado sea de tipo limpieza",
-            level = "action", # ( action | parser )
-            variable = None, 
-            call_function = self.set_clean_patch
-            )
-            
+            name="patch-qs-rewrite",
+            description="indica si al aplicar un parche de QS se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
+            level="action",
+            variable="VALUE",
+            call_function=self.set_patch_qs_rewrite,
+        )
+        self.parser.declare_option(
+            name="patch-py-rewrite",
+            description="indica si al aplicar un parche de PY se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
+            level="action",
+            variable="VALUE",
+            call_function=self.set_patch_py_rewrite,
+        )
+        self.parser.declare_option(
+            name="patch-test-rewrite",
+            description="indica si al aplicar un parche de PY_test se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
+            level="action",
+            variable="VALUE",
+            call_function=self.set_patch_test_rewrite,
+        )
+        self.parser.declare_option(
+            name="patch-model-rewrite",
+            description="indica si al aplicar un parche de PY_model se debe sobreescribir o no las clases existentes ( reverse / predelete / yes / warn / no / abort ) ",
+            level="action",
+            variable="VALUE",
+            call_function=self.set_patch_model_rewrite,
+        )
+        self.parser.declare_option(
+            name="patch-name",
+            description="Indica el nombre del parche que se usará en lugar de autodetectarlo.",
+            level="action",
+            variable="NAME",
+            call_function=self.set_patch_name,
+        )
+        self.parser.declare_option(
+            name="patch-dest",
+            description="Donde guardar un fichero de parche",
+            level="action",
+            variable="FILENAME",
+            call_function=self.set_patch_dest,
+        )
+        self.parser.declare_option(
+            name="enable-diff-xml-search-move",
+            description="Activa la búsqueda de movimientos de bloques XML. Puede ser un poco más lento y puede generar parches incompatibles con otras herramientas.",
+            level="action",
+            call_function=self.enable_diff_xml_search_move,
+        )
+        self.parser.declare_option(
+            name="patch-xml-style",
+            description="Usar otro estilo para generar parches XML (ver mergetools/etc/patch-styles/)",
+            variable="NAME",
+            level="action",
+            call_function=self.set_patch_xml_style,
+        )
+        self.parser.declare_option(
+            name="patch-qs-style",
+            description="Usar otro estilo para generar parches QS (legacy|qsdir)",
+            variable="NAME",
+            level="action",
+            call_function=self.set_patch_qs_style,
+        )
+        self.parser.declare_option(
+            name="patch-py-style",
+            description="Usar otro estilo para generar parches PY (legacy|pydir)",
+            variable="NAME",
+            level="action",
+            call_function=self.set_patch_py_style,
+        )
+        self.parser.declare_option(
+            name="patch-test-style",
+            description="Usar otro estilo para generar parches PY_test (legacy|testdir)",
+            variable="NAME",
+            level="action",
+            call_function=self.set_patch_test_style,
+        )
+        self.parser.declare_option(
+            name="patch-model-style",
+            description="Usar otro estilo para generar parches PY_model (legacy|modeldir)",
+            variable="NAME",
+            level="action",
+            call_function=self.set_patch_model_style,
+        )
+        self.parser.declare_option(
+            name="clean-patch",
+            description="provoca que el parche generado sea de tipo limpieza",
+            level="action",  # ( action | parser )
+            variable=None,
+            call_function=self.set_clean_patch,
+        )
+
         self.build_project_action = self.parser.declare_action(
-            name = "build-project",
-            args = ["buildxml"],
-            options = [],
-            description = "Lee el fichero $buildxml y realiza las operaciones que se determinan",
-            call_function = self.do_build_project,
-            )
+            name="build-project",
+            args=["buildxml"],
+            options=[],
+            description="Lee el fichero $buildxml y realiza las operaciones que se determinan",
+            call_function=self.do_build_project,
+        )
         self.build_project_action.set_help_arg(
-            buildxml = "Fichero del que leer las instrucciones",
-            )                
-            
+            buildxml="Fichero del que leer las instrucciones",
+        )
+
         self.folder_diff_action = self.parser.declare_action(
-            name = "folder-diff",
-            args = ["patchdir","basedir","finaldir"],
-            options = ["patch-name", "patch-qs-style", "patch-xml-style"],
-            description = "Genera en $patchdir una colección de parches de la diferencia entre las carpetas $basedir y $finaldir",
-            call_function = self.do_folder_diff,
-            )                
-            
+            name="folder-diff",
+            args=["patchdir", "basedir", "finaldir"],
+            options=["patch-name", "patch-qs-style", "patch-xml-style"],
+            description="Genera en $patchdir una colección de parches de la diferencia entre las carpetas $basedir y $finaldir",
+            call_function=self.do_folder_diff,
+        )
+
         self.folder_diff_action = self.parser.declare_action(
-            name = "folder-diff",
-            args = ["patchdir","basedir","finaldir"],
-            options = ["patch-name", "patch-py-style", "patch-test-style", "patch-xml-style"],
-            description = "Genera en $patchdir una colección de parches de la diferencia entre las carpetas $basedir y $finaldir",
-            call_function = self.do_folder_diff,
-            )          
-            
+            name="folder-diff",
+            args=["patchdir", "basedir", "finaldir"],
+            options=["patch-name", "patch-py-style", "patch-test-style", "patch-xml-style"],
+            description="Genera en $patchdir una colección de parches de la diferencia entre las carpetas $basedir y $finaldir",
+            call_function=self.do_folder_diff,
+        )
+
         self.folder_diff_action = self.parser.declare_action(
-            name = "folder-diff",
-            args = ["patchdir","basedir","finaldir"],
-            options = ["patch-name", "patch-py-style", "patch-model-style", "patch-xml-style"],
-            description = "Genera en $patchdir una colección de parches de la diferencia entre las carpetas $basedir y $finaldir",
-            call_function = self.do_folder_diff,
-            )
+            name="folder-diff",
+            args=["patchdir", "basedir", "finaldir"],
+            options=["patch-name", "patch-py-style", "patch-model-style", "patch-xml-style"],
+            description="Genera en $patchdir una colección de parches de la diferencia entre las carpetas $basedir y $finaldir",
+            call_function=self.do_folder_diff,
+        )
         self.folder_diff_action.set_help_arg(
-            patchdir = "Carpeta donde guardar las diferencias",
-            basedir = "Carpeta a leer como referencia",
-            finaldir = "Carpeta a comparar",
-            )                
-            
+            patchdir="Carpeta donde guardar las diferencias",
+            basedir="Carpeta a leer como referencia",
+            finaldir="Carpeta a comparar",
+        )
+
         self.folder_patch_action = self.parser.declare_action(
-            name = "folder-patch",
-            args = ["patchdir","basedir","finaldir"],
-            options = ["patch-name"],
-            description = "Aplica los parches en $patchdir a la carpeta $basedir y genera $finaldir",
-            call_function = self.do_folder_patch,
-            )
+            name="folder-patch",
+            args=["patchdir", "basedir", "finaldir"],
+            options=["patch-name"],
+            description="Aplica los parches en $patchdir a la carpeta $basedir y genera $finaldir",
+            call_function=self.do_folder_patch,
+        )
         self.folder_patch_action.set_help_arg(
-            patchdir = "Carpeta donde leer las diferencias",
-            basedir = "Carpeta a leer como referencia",
-            finaldir = "Carpeta a aplicar los cambios",
-            )                
+            patchdir="Carpeta donde leer las diferencias",
+            basedir="Carpeta a leer como referencia",
+            finaldir="Carpeta a aplicar los cambios",
+        )
 
         self.file_diff_action = self.parser.declare_action(
-            name = "file-diff",
-            args = ["ext","base","final"],
-            description = "Genera un parche de fichero $ext de la diferencia entre el fichero $base y $final",
-            options = ['output-file','clean-patch'],
-            call_function = self.do_file_diff,
-            min_file_list = 0, # por defecto es 0
-            max_file_list = 0, # por defecto es 0, -1 indica sin límite.
-            min_argcount = -1  # cantidad de argumentos obligatorios. por defecto -1
-            )
+            name="file-diff",
+            args=["ext", "base", "final"],
+            description="Genera un parche de fichero $ext de la diferencia entre el fichero $base y $final",
+            options=["output-file", "clean-patch"],
+            call_function=self.do_file_diff,
+            min_file_list=0,  # por defecto es 0
+            max_file_list=0,  # por defecto es 0, -1 indica sin límite.
+            min_argcount=-1,  # cantidad de argumentos obligatorios. por defecto -1
+        )
         self.file_diff_action.set_help_arg(
-            ext = "Tipo de fichero a procesar: QS / XML / PY / PY_test",
-            base = "Fichero original",
-            final = "Fichero final",
-            )                
-        self.file_patch_action = self.parser.declare_action( 
-            name = "file-patch",
-            args = ["ext","base","patch"],
-            description = "Aplica un parche de fichero $ext especificado por $patch al fichero $base",
-            options = ['output-file','patch-qs-rewrite','patch-py-rewrite','patch-test-rewrite',"enable-diff-xml-search-move","patch-xml-style"],
-            call_function = self.do_file_patch,
-            )
+            ext="Tipo de fichero a procesar: QS / XML / PY / PY_test",
+            base="Fichero original",
+            final="Fichero final",
+        )
+        self.file_patch_action = self.parser.declare_action(
+            name="file-patch",
+            args=["ext", "base", "patch"],
+            description="Aplica un parche de fichero $ext especificado por $patch al fichero $base",
+            options=[
+                "output-file",
+                "patch-qs-rewrite",
+                "patch-py-rewrite",
+                "patch-test-rewrite",
+                "enable-diff-xml-search-move",
+                "patch-xml-style",
+            ],
+            call_function=self.do_file_patch,
+        )
         self.file_patch_action.set_help_arg(
-            ext = "Tipo de fichero a procesar: QS / XML / PY / PY_test",
-            base = "Fichero original",
-            patch = "Parche a aplicar sobre $base",
-            )
+            ext="Tipo de fichero a procesar: QS / XML / PY / PY_test",
+            base="Fichero original",
+            patch="Parche a aplicar sobre $base",
+        )
         self.file_diff_action.set_help_arg(
-            ext = "Tipo de fichero a procesar: QS / XML / PY / PY_model",
-            base = "Fichero original",
-            final = "Fichero final",
-            )                
-        self.file_patch_action = self.parser.declare_action( 
-            name = "file-patch",
-            args = ["ext","base","patch"],
-            description = "Aplica un parche de fichero $ext especificado por $patch al fichero $base",
-            options = ['output-file','patch-qs-rewrite','patch-py-rewrite','patch-model-rewrite',"enable-diff-xml-search-move","patch-xml-style"],
-            call_function = self.do_file_patch,
-            )
+            ext="Tipo de fichero a procesar: QS / XML / PY / PY_model",
+            base="Fichero original",
+            final="Fichero final",
+        )
+        self.file_patch_action = self.parser.declare_action(
+            name="file-patch",
+            args=["ext", "base", "patch"],
+            description="Aplica un parche de fichero $ext especificado por $patch al fichero $base",
+            options=[
+                "output-file",
+                "patch-qs-rewrite",
+                "patch-py-rewrite",
+                "patch-model-rewrite",
+                "enable-diff-xml-search-move",
+                "patch-xml-style",
+            ],
+            call_function=self.do_file_patch,
+        )
         self.file_patch_action.set_help_arg(
-            ext = "Tipo de fichero a procesar: QS / XML / PY / PY_model",
-            base = "Fichero original",
-            patch = "Parche a aplicar sobre $base",
-            )
-        self.file_check_action = self.parser.declare_action( 
-            name = "file-check",
-            args = ["check","filename"],
-            description = "Analiza un fichero $filename en busca de errores usando el algoritmo de comprobación $check",
-            options = ['patch-dest'],
-            call_function = self.do_file_check,
-            )
+            ext="Tipo de fichero a procesar: QS / XML / PY / PY_model",
+            base="Fichero original",
+            patch="Parche a aplicar sobre $base",
+        )
+        self.file_check_action = self.parser.declare_action(
+            name="file-check",
+            args=["check", "filename"],
+            description="Analiza un fichero $filename en busca de errores usando el algoritmo de comprobación $check",
+            options=["patch-dest"],
+            call_function=self.do_file_check,
+        )
         self.file_check_action.set_help_arg(
-            check = "Tipo de análisis a realizar: qs-classes / ...",
-            filename = "Fichero a analizar",
-            )
+            check="Tipo de análisis a realizar: qs-classes / ...",
+            filename="Fichero a analizar",
+        )
         self.qs_extract_action = self.parser.declare_action(
-            name = "qs-extract",
-            args = ["final","classlist"],
-            description = "Extrae del fichero $final las clases indicadas en $classlist",
-            options = ['output-file'],
-            call_function = self.do_qs_extract,
-            )
+            name="qs-extract",
+            args=["final", "classlist"],
+            description="Extrae del fichero $final las clases indicadas en $classlist",
+            options=["output-file"],
+            call_function=self.do_qs_extract,
+        )
         self.py_extract_action = self.parser.declare_action(
-            name = "py-extract",
-            args = ["final","classlist"],
-            description = "Extrae del fichero $final las clases indicadas en $classlist",
-            options = ['output-file'],
-            call_function = self.do_py_extract,
-            )
+            name="py-extract",
+            args=["final", "classlist"],
+            description="Extrae del fichero $final las clases indicadas en $classlist",
+            options=["output-file"],
+            call_function=self.do_py_extract,
+        )
         self.test_extract_action = self.parser.declare_action(
-            name = "test-extract",
-            args = ["final","classlist"],
-            description = "Extrae del fichero $final las clases indicadas en $classlist",
-            options = ['output-file'],
-            call_function = self.do_test_extract,
-            )
+            name="test-extract",
+            args=["final", "classlist"],
+            description="Extrae del fichero $final las clases indicadas en $classlist",
+            options=["output-file"],
+            call_function=self.do_test_extract,
+        )
         self.model_extract_action = self.parser.declare_action(
-            name = "model-extract",
-            args = ["final","classlist"],
-            description = "Extrae del fichero $final las clases indicadas en $classlist",
-            options = ['output-file'],
-            call_function = self.do_model_extract,
-            )
+            name="model-extract",
+            args=["final", "classlist"],
+            description="Extrae del fichero $final las clases indicadas en $classlist",
+            options=["output-file"],
+            call_function=self.do_model_extract,
+        )
         self.qs_extract_action.set_help_arg(
-            final = "Fichero QS que contiene las clases a extraer",
-            classlist = "Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
-            )   
+            final="Fichero QS que contiene las clases a extraer",
+            classlist="Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
+        )
         self.py_extract_action.set_help_arg(
-            final = "Fichero PY que contiene las clases a extraer",
-            classlist = "Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
-            )
+            final="Fichero PY que contiene las clases a extraer",
+            classlist="Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
+        )
         self.test_extract_action.set_help_arg(
-            final = "Fichero PY_test que contiene las clases a extraer",
-            classlist = "Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
-            ) 
+            final="Fichero PY_test que contiene las clases a extraer",
+            classlist="Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
+        )
         self.model_extract_action.set_help_arg(
-            final = "Fichero PY_model que contiene las clases a extraer",
-            classlist = "Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
-            )                
+            final="Fichero PY_model que contiene las clases a extraer",
+            classlist="Lista de clases a extraer, separadas por coma y sin espacios: class1,class2,...",
+        )
 
         self.qs_split_action = self.parser.declare_action(
             name="qs-split",
             args=["final"],
             description="Separa el fichero $final en subficheros en una carpeta",
             options=[],
             call_function=self.do_qs_split,
@@ -404,203 +430,216 @@
             call_function=self.do_model_join,
         )
         self.model_join_action.set_help_arg(
             folder="Carpeta con los subficheros PY_model",
         )
 
     def set_patch_name(self, name):
-        if name == "": name = None
+        if name == "":
+            name = None
         self.patch_name = name
 
     def set_patch_dest(self, filename):
-        if filename == "": filename = None
+        if filename == "":
+            filename = None
         self.patch_dest = filename
-        
+
     def set_patch_xml_style(self, name):
         self.patch_xml_style_name = name
-        
+
     def set_patch_qs_style(self, name):
         self.patch_qs_style_name = name
-        
+
     def set_patch_qs_rewrite(self, value):
-        if value not in ['reverse','predelete','yes','no','warn','abort']: raise ValueError
+        if value not in ["reverse", "predelete", "yes", "no", "warn", "abort"]:
+            raise ValueError
         self.patch_qs_rewrite = value
-        
+
     def set_patch_py_style(self, name):
         self.patch_py_style_name = name
-        
+
     def set_patch_test_style(self, name):
         self.patch_test_style_name = name
-        
+
     def set_patch_model_style(self, name):
         self.patch_model_style_name = name
-        
+
     def set_patch_py_rewrite(self, value):
-        if value not in ['reverse','predelete','yes','no','warn','abort']: raise ValueError
+        if value not in ["reverse", "predelete", "yes", "no", "warn", "abort"]:
+            raise ValueError
         self.patch_py_rewrite = value
-        
+
     def set_patch_test_rewrite(self, value):
-        if value not in ['reverse','predelete','yes','no','warn','abort']: raise ValueError
+        if value not in ["reverse", "predelete", "yes", "no", "warn", "abort"]:
+            raise ValueError
         self.patch_test_rewrite = value
-        
+
     def set_patch_model_rewrite(self, value):
-        if value not in ['reverse','predelete','yes','no','warn','abort']: raise ValueError
+        if value not in ["reverse", "predelete", "yes", "no", "warn", "abort"]:
+            raise ValueError
         self.patch_model_rewrite = value
 
     def enable_diff_xml_search_move(self):
         self.diff_xml_search_move = True
 
     def set_clean_patch(self):
         self.clean_patch = True
-        
-    
+
     # :::: ACTIONS ::::
     def do_build_project(self, buildxml):
         try:
             return projectbuilder.build_xml_file(self, buildxml)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-    
+            self.exception(type(e).__name__, str(e))
+
     def do_folder_diff(self, basedir, finaldir, patchdir):
         try:
             return flpatchdir.diff_folder(self, basedir, finaldir, patchdir)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
+            self.exception(type(e).__name__, str(e))
 
     def do_folder_patch(self, basedir, finaldir, patchdir):
         try:
             return flpatchdir.patch_folder(self, basedir, finaldir, patchdir)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
+            self.exception(type(e).__name__, str(e))
 
-    
     def do_file_diff(self, ext, base, final):
         try:
             ext = str(ext).upper()
-            if ext == 'QS':
+            if ext == "QS":
                 return flpatchqs.diff_qs(self, base, final)
-            if ext == 'QSDIR':
+            if ext == "QSDIR":
                 return flpatchqs.diff_qs_dir(self, base, final)
-            if ext == 'PY':
+            if ext == "PY":
                 aBase = base.split("/")
                 nom = aBase[-1:][0]
                 if nom.startswith("test_"):
                     return flpatchtest.diff_test(self, base, final)
-                elif nom.endswith("_ut.py"):
-                    return flpatchpy.diff_py(self, base, final)
-                elif nom.endswith("_def.py"):
-                    return flpatchpy.diff_py(self, base, final)
+
+                elif nom.endswith("_api.py"):
+                    return flpatchapipy.diff_py(self, base, final)
                 elif "models" in base or "pruebasqs" in base:
                     return flpatchmodel.diff_model(self, base, final)
                 else:
                     return flpatchpy.diff_py(self, base, final)
-            #if ext == 'XML': return flpatchxml.diff_xml(self,base,final)
-            if ext == 'XML': return flpatchlxml.diff_lxml(self,base,final)
+            # if ext == 'XML': return flpatchxml.diff_xml(self,base,final)
+            if ext == "XML":
+                return flpatchlxml.diff_lxml(self, base, final)
             print("Unknown $ext %s" % (repr(ext)))
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
+            self.exception(type(e).__name__, str(e))
 
     def do_file_patch(self, ext, base, patch):
         try:
             ext = str(ext).upper()
-            if ext == 'QS': return flpatchqs.patch_qs(self,base,patch)
-            if ext == 'QSDIR': return flpatchqs.patch_qs_dir(self,base,patch)
-            if ext == 'PY':
+            if ext == "QS":
+                return flpatchqs.patch_qs(self, base, patch)
+            if ext == "QSDIR":
+                return flpatchqs.patch_qs_dir(self, base, patch)
+            if ext == "PY":
                 aBase = base.split("/")
                 nom = aBase[-1:][0]
                 if nom.startswith("test_"):
                     return flpatchtest.patch_test(self, base, patch)
                 elif nom.endswith("_ut.py"):
                     return flpatchpy.patch_py(self, base, patch)
                 elif nom.endswith("_def.py"):
                     return flpatchpy.patch_py(self, base, patch)
+                elif nom.endswith(("_api.py", "_schema.py", "_model.py")):
+                    return flpatchapipy.patch_py(self, base, patch)
                 elif "models" in base or "pruebasqs" in base:
                     return flpatchmodel.patch_model(self, base, patch)
                 else:
                     return flpatchpy.patch_py(self, base, patch)
-            if ext == 'XML': return flpatchlxml.patch_lxml(self,patch,base)
+            if ext == "XML":
+                return flpatchlxml.patch_lxml(self, patch, base)
             print("Unknown $ext %s" % (repr(ext)))
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
+            self.exception(type(e).__name__, str(e))
 
     def do_file_check(self, check, filename):
         try:
-            check = str(check).lower() 
-            if check == 'qs-classes': return flpatchqs.check_qs_classes(self,filename)
-            if check == 'py-classes': return flpatchpy.check_py_classes(self,filename)
-            if check == 'test-classes': return flpatchtest.check_test_classes(self,filename)
-            if check == 'model-classes': return flpatchmodel.check_model_classes(self,filename)
+            check = str(check).lower()
+            if check == "qs-classes":
+                return flpatchqs.check_qs_classes(self, filename)
+            if check == "py-classes":
+                return flpatchpy.check_py_classes(self, filename)
+            if check == "test-classes":
+                return flpatchtest.check_test_classes(self, filename)
+            if check == "model-classes":
+                return flpatchmodel.check_model_classes(self, filename)
             print("Unknown $check %s" % (repr(check)))
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_qs_extract(self, final, classlist):
         try:
-            return flpatchqs.extract_classes_qs(self,final, classlist)
+            return flpatchqs.extract_classes_qs(self, final, classlist)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_qs_split(self, final):
         try:
-            return flpatchqs.split_qs(self,final)
+            return flpatchqs.split_qs(self, final)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_qs_join(self, folder):
         try:
-            return flpatchqs.join_qs(self,folder)
+            return flpatchqs.join_qs(self, folder)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_py_extract(self, final, classlist):
         try:
-            return flpatchpy.extract_classes_py(self,final, classlist)
+            return flpatchpy.extract_classes_py(self, final, classlist)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_py_split(self, final):
         try:
-            return flpatchpy.split_py(self,final)
+            return flpatchpy.split_py(self, final)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_py_join(self, folder):
         try:
-            return flpatchpy.join_py(self,folder)
+            return flpatchpy.join_py(self, folder)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_test_extract(self, final, classlist):
         try:
-            return flpatchtest.extract_classes_test(self,final, classlist)
+            return flpatchtest.extract_classes_test(self, final, classlist)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_test_split(self, final):
         try:
-            return flpatchtest.split_test(self,final)
+            return flpatchtest.split_test(self, final)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_test_join(self, folder):
         try:
-            return flpatchtest.join_test(self,folder)
+            return flpatchtest.join_test(self, folder)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_model_extract(self, final, classlist):
         try:
-            return flpatchmodel.extract_classes_model(self,final, classlist)
+            return flpatchmodel.extract_classes_model(self, final, classlist)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_model_split(self, final):
         try:
-            return flpatchmodel.split_model(self,final)
+            return flpatchmodel.split_model(self, final)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
-            
+            self.exception(type(e).__name__, str(e))
+
     def do_model_join(self, folder):
         try:
-            return flpatchmodel.join_model(self,folder)
+            return flpatchmodel.join_model(self, folder)
         except Exception as e:
-            self.exception(type(e).__name__,str(e))
+            self.exception(type(e).__name__, str(e))
```

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/index.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchdir.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchdir.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os.path
 import shutil
 import difflib
 import time
 import hashlib
 import fnmatch
 
-from enebootools.mergetool import flpatchqs, flpatchlxml, flpatchpy
+from enebootools.mergetool import flpatchqs, flpatchlxml, flpatchpy, flpatchapipy
 
 
 def filepath():
     return os.path.abspath(os.path.dirname(__file__))
 
 
 def filedir(x):
@@ -95,15 +95,14 @@
             self.root = None
             iface.error("No se pudo leer el parche: " + str(e))
 
     def patch_folder(self, folder):
         if self.root is None:
             return
         for action in self.root:
-
             actionname = action.tag
             if not isinstance(actionname, str):
                 continue
             if actionname.startswith("{"):
                 actionname = action.tag.split("}")[1]
             actionname = actionname.lower()
             if actionname.startswith("flpatch:"):
@@ -313,15 +312,18 @@
         old_verbosity = self.iface.verbosity
         self.iface.verbosity -= 2
         if self.iface.verbosity < 0:
             self.iface.verbosity = 0
         old_style, self.iface.patch_py_style_name = self.iface.patch_py_style_name, style
         self.iface.set_output_file(dst + ".patched")
         if style in ["legacy"]:
-            ret = flpatchpy.patch_py(self.iface, dst, src)
+            if filename.endswith(("_api.py", "_schema.py", "_model.py")):
+                ret = flpatchapipy.patch_py(self.iface, dst, src)
+            else:
+                ret = flpatchpy.patch_py(self.iface, dst, src)
         elif style in ["qsdir"]:
             ret = flpatchpy.patch_py_dir(self.iface, dst, src)
         else:
             raise ValueError("Estilo de parche PY desconocido: %s" % style)
         self.iface.output = old_output
         self.iface.verbosity = old_verbosity
         self.iface.patch_qs_style_name = old_style
@@ -409,15 +411,14 @@
         self.deleted_files = basedir_files - finaldir_files
         self.common_files = finaldir_files & basedir_files
         # iface.info("+ %s" % self.added_files)
         # iface.info("- %s" % self.deleted_files)
         # print("=", self.common_files)
 
         if basedir and finaldir:
-
             iface.info("Calculando diferencias . . . ")
 
             file_actions = []
             file_actions += [(os.path.dirname(f), f, "add") for f in self.added_files]
             file_actions += [(os.path.dirname(f), f, "common") for f in self.common_files]
             file_actions += [(os.path.dirname(f), f, "delete") for f in self.deleted_files]
             # Intentar guardarlos de forma ordenada, para minimizar las diferencias entre parches.
@@ -687,21 +688,19 @@
             shutil.copytree(src, dst)
 
     fpatch = FolderApplyPatch(iface, patchdir)
     fpatch.patch_folder(finaldir)
 
 
 def update_patch_folder(iface, finaldir, srcdir, patchdir, path):
-
     basedir = os.path.join(path, "build/base")
     mod_files = []
 
     fpatch = FolderCreatePatch(iface, finaldir, srcdir, patchdir)
     for action in fpatch.root:
-
         src_file = os.path.join(srcdir, action.get("path"), action.get("name"))
         final_file = os.path.join(finaldir, action.get("path"), action.get("name"))
         base_file = os.path.join(basedir, action.get("path"), action.get("name"))
         src_time = os.path.getmtime(src_file) if os.path.exists(src_file) else 0
         final_time = os.path.getmtime(final_file) if os.path.exists(final_file) else 0
         if src_time and final_time and src_time <= final_time:
             fpatch.root.remove(action)
```

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchpy.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchapipy.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     
     
     Aunque pueda parecer información excesiva, es normal, porque genera un 
     arbol 1->N y da la información exacta de la extensión/mezcla al usuario
     final.
     
 """
+# PARA: _model, _schema y _api.py
 
 import re, os.path, difflib, math, itertools, shutil, sys, io
 import pprint, subprocess
 
 pp = pprint.PrettyPrinter(indent=4)
 
 
@@ -1125,15 +1126,14 @@
 
         new_block = []
         add_buffer_a = []
         add_buffer_b = []
         last_a_diff = 0
         last_b_diff = 0
         while True:
-
             if a_diffs and a_diffs[0][0] == base_pos:
                 f_a_diff = a_diffs.pop(0)
                 if f_a_diff[1] == "+ ":
                     a_offset += 1
                     add_buffer_a.append(f_a_diff[3])
                     last_a_diff = 0
                 if f_a_diff[1] == "- ":
@@ -1774,30 +1774,30 @@
             else:
                 # Si no había clase posterior, entonces marcamos como posición
                 # de inserción el próximo bloque.
                 child_class = parent_class + 1
 
             # Si la clase que vamos a heredar es la que está en el iface, entonces
             #   en el iface habrá que cambiarlo por la nuestra.
-            if clbase["iface"]:  # -> primero comprobar que tenemos iface.
+            """ if clbase["iface"]:  # -> primero comprobar que tenemos iface.
                 iface.debug2r(iface=clbase["iface"])
                 if clbase["iface"]["classname"] == extending:
                     iface.debug(
                         "La clase que estamos extendiendo (%s) es el "
                         "tipo de dato usado por iface, por lo tanto actualizamos"
                         " el tipo de dato usado por iface a %s" % (extending, newclass)
                     )
                     todo.append("fix-iface newclass")
                     new_iface_class = newclass
             else:
                 iface.warn(
                     "No existe declaración de iface en el código (aplicando patch para clase %s)"
                     % newclass
                 )
-                todo.append("create-iface")
+                todo.append("create-iface") """
 
             # Si la clase del parche que estamos aplicando pasa a extender otra
             # clase con nombre distinto, actualizaremos también los constructores.
             if cdpatch[newclass]["extends"] != extending:
                 iface.debug(
                     "La clase %s extendía %s en el parche, pasará a"
                     " heredar a la clase %s" % (newclass, cdpatch[newclass]["extends"], extending)
```

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchqs.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchtest.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/flpatchxml.py` & `enebootools-2.0.0/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/projectbuilder.py` & `enebootools-2.0.0/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/test/__init__.py` & `enebootools-2.0.0/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.0.0/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/packager/__init__.py` & `enebootools-2.0.0/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/packager/pkgjoiner.py` & `enebootools-2.0.0/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/packager/pkgsplitter.py` & `enebootools-2.0.0/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/parseargs.py` & `enebootools-2.0.0/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools/parseargs.pyc` & `enebootools-2.0.0/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.2/enebootools.egg-info/PKG-INFO` & `enebootools-2.0.0/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 1.8.2
+Version: 2.0.0
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-1.8.2/enebootools.egg-info/SOURCES.txt` & `enebootools-2.0.0/enebootools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 enebootools/lib/utils.py
 enebootools/lib/etree/ElementInclude.py
 enebootools/lib/etree/ElementPath.py
 enebootools/lib/etree/ElementTree.py
 enebootools/lib/etree/__init__.py
 enebootools/lib/etree/cElementTree.py
 enebootools/mergetool/__init__.py
+enebootools/mergetool/flpatchapipy.py
 enebootools/mergetool/flpatchdir.py
 enebootools/mergetool/flpatchlxml.py
 enebootools/mergetool/flpatchmodel.py
 enebootools/mergetool/flpatchpy.py
 enebootools/mergetool/flpatchqs.py
 enebootools/mergetool/flpatchtest.py
 enebootools/mergetool/flpatchxml.py
```

### Comparing `enebootools-1.8.2/setup.py` & `enebootools-2.0.0/setup.py`

 * *Files identical despite different names*

