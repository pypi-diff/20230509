# Comparing `tmp/glamconv-0.3.0.tar.gz` & `tmp/glamconv-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glamconv-0.3.0.tar", last modified: Wed Feb 15 12:45:39 2023, max compression
+gzip compressed data, was "glamconv-0.3.1.tar", last modified: Tue May  9 17:56:16 2023, max compression
```

## Comparing `glamconv-0.3.0.tar` & `glamconv-0.3.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.775109 glamconv-0.3.0/
--rw-rw-r--   0 katia     (1000) katia     (1000)      329 2023-02-15 12:44:09.000000 glamconv-0.3.0/MANIFEST.in
--rw-rw-r--   0 katia     (1000) katia     (1000)      409 2023-02-15 12:45:39.775109 glamconv-0.3.0/PKG-INFO
--rw-rw-r--   0 katia     (1000) katia     (1000)      261 2021-04-15 12:24:08.000000 glamconv-0.3.0/README.rst
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.759109 glamconv-0.3.0/examples/
--rw-rw-r--   0 katia     (1000) katia     (1000)     3158 2022-08-01 09:26:40.000000 glamconv-0.3.0/examples/ead-transform.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     5046 2021-04-15 12:24:08.000000 glamconv-0.3.0/examples/generic-ead-transformation.json
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.759109 glamconv-0.3.0/glamconv/
--rw-rw-r--   0 katia     (1000) katia     (1000)      176 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/__init__.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.763109 glamconv-0.3.0/glamconv/cli/
--rw-rw-r--   0 katia     (1000) katia     (1000)       87 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/cli/__init__.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    11353 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/cli/commands.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.763109 glamconv-0.3.0/glamconv/eac/
--rw-rw-r--   0 katia     (1000) katia     (1000)      695 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/__init__.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     6562 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/adjusters.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.763109 glamconv-0.3.0/glamconv/eac/ape-eac-schema/
--rw-rw-r--   0 katia     (1000) katia     (1000)    60710 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/ape-eac-schema/apeEAC-CPF.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)     3180 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/ape-eac-schema/xlink.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)     5695 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/ape-eac-schema/xml.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)    12610 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/cleaners.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2737 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/default-eac-cpf-to-ape-settings.json
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.763109 glamconv-0.3.0/glamconv/eac/eac-cpf-schema/
--rw-rw-r--   0 katia     (1000) katia     (1000)    46012 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/eac-cpf-schema/cpf.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)     3180 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/eac-cpf-schema/xlink.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)     5695 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/eac-cpf-schema/xml.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)     1171 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/formats.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2524 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/namespacers.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      904 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/registration.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     6488 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/required_elts_adders.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1365 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/supplementers.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     8530 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/text_data.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1509 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/utils.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2659 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/eac/validators.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.767109 glamconv-0.3.0/glamconv/ead/
--rw-rw-r--   0 katia     (1000) katia     (1000)      692 2021-08-30 14:13:55.000000 glamconv-0.3.0/glamconv/ead/__init__.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    12891 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/adjusters.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.767109 glamconv-0.3.0/glamconv/ead/ape-ead-schema/
--rw-rw-r--   0 katia     (1000) katia     (1000)    76857 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ape-ead-schema/apeEAD.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)     3180 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ape-ead-schema/xlink.xsd
--rw-rw-r--   0 katia     (1000) katia     (1000)    15380 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/arch_data.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    18492 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/cleaners.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     7663 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/default-ead2-to-ape-settings.json
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.771109 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/
--rw-rw-r--   0 katia     (1000) katia     (1000)   186679 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/ead.dtd
--rw-rw-r--   0 katia     (1000) katia     (1000)    38830 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/eadlocal.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     5910 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-cyr1.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     3513 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-cyr2.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     2433 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-dia.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     4598 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk1.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     3334 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk2.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     4159 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk3.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     4257 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk4.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     6160 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-lat1.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)    10378 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-lat2.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     5671 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-num.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     6182 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-pub.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)     4498 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-tech.ent
--rw-rw-r--   0 katia     (1000) katia     (1000)    23328 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/ead_2002_correcters.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1172 2022-08-01 09:26:40.000000 glamconv-0.3.0/glamconv/ead/formats.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    14362 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/header.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    21258 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/link_managers.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2457 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/namespacers.py
--rw-rw-r--   0 katia     (1000) katia     (1000)      972 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/registration.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1358 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/supplementers.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    27816 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/text_data.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1588 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/ead/utils.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2528 2022-08-01 09:26:40.000000 glamconv-0.3.0/glamconv/ead/validators.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.771109 glamconv-0.3.0/glamconv/transformer/
--rw-rw-r--   0 katia     (1000) katia     (1000)      327 2021-04-15 12:24:08.000000 glamconv-0.3.0/glamconv/transformer/__init__.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     5601 2022-08-01 09:26:40.000000 glamconv-0.3.0/glamconv/transformer/actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1010 2022-08-01 09:26:40.000000 glamconv-0.3.0/glamconv/transformer/formats.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2827 2022-08-01 09:26:40.000000 glamconv-0.3.0/glamconv/transformer/libraries.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     4723 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/transformer/logger.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     4361 2022-08-01 10:02:26.000000 glamconv-0.3.0/glamconv/transformer/parameters.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     7728 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/transformer/processes.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1760 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/transformer/rw_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     3535 2023-02-15 12:44:09.000000 glamconv-0.3.0/glamconv/utils.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.763109 glamconv-0.3.0/glamconv.egg-info/
--rw-rw-r--   0 katia     (1000) katia     (1000)      409 2023-02-15 12:45:39.000000 glamconv-0.3.0/glamconv.egg-info/PKG-INFO
--rw-rw-r--   0 katia     (1000) katia     (1000)     2916 2023-02-15 12:45:39.000000 glamconv-0.3.0/glamconv.egg-info/SOURCES.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)        1 2023-02-15 12:45:39.000000 glamconv-0.3.0/glamconv.egg-info/dependency_links.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)        1 2021-04-15 12:24:51.000000 glamconv-0.3.0/glamconv.egg-info/not-zip-safe
--rw-rw-r--   0 katia     (1000) katia     (1000)        5 2023-02-15 12:45:39.000000 glamconv-0.3.0/glamconv.egg-info/requires.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)        9 2023-02-15 12:45:39.000000 glamconv-0.3.0/glamconv.egg-info/top_level.txt
--rw-rw-r--   0 katia     (1000) katia     (1000)       38 2023-02-15 12:45:39.775109 glamconv-0.3.0/setup.cfg
--rw-rw-r--   0 katia     (1000) katia     (1000)     1200 2023-02-15 12:44:09.000000 glamconv-0.3.0/setup.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.775109 glamconv-0.3.0/test/
--rw-rw-r--   0 katia     (1000) katia     (1000)      613 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/__init__.py
-drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-02-15 12:45:39.775109 glamconv-0.3.0/test/data/
--rw-rw-r--   0 katia     (1000) katia     (1000)     1089 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/data/simple-eac.xml
--rw-rw-r--   0 katia     (1000) katia     (1000)      239 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/data/simple-ead.xml
--rw-rw-r--   0 katia     (1000) katia     (1000)    21088 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_adjusters_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    66311 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_cleaners_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     5482 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_namespacers_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    10637 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_required_elts_adders_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1790 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_supplementers_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    30504 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_text_data_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     3814 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_eac_validators_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    14333 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_adjusters_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    15398 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_arch_data_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    72836 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_cleaners_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    35415 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_ead_2002_correctors_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)    20845 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_header_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     4873 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_namespacers_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     1455 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_supplementers_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     3195 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_ead_validators_actions.py
--rw-rw-r--   0 katia     (1000) katia     (1000)     2974 2023-02-15 12:44:09.000000 glamconv-0.3.0/test/test_transformer_rw_actions.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.157559 glamconv-0.3.1/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      329 2023-05-05 09:17:54.000000 glamconv-0.3.1/MANIFEST.in
+-rw-rw-r--   0 katia     (1000) katia     (1000)      409 2023-05-09 17:56:16.157559 glamconv-0.3.1/PKG-INFO
+-rw-rw-r--   0 katia     (1000) katia     (1000)      261 2021-04-15 12:24:08.000000 glamconv-0.3.1/README.rst
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.141559 glamconv-0.3.1/examples/
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3158 2023-03-19 19:24:49.000000 glamconv-0.3.1/examples/ead-transform.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5046 2021-04-15 12:24:08.000000 glamconv-0.3.1/examples/generic-ead-transformation.json
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.141559 glamconv-0.3.1/glamconv/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      176 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/__init__.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.141559 glamconv-0.3.1/glamconv/cli/
+-rw-rw-r--   0 katia     (1000) katia     (1000)       87 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/cli/__init__.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    11353 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/cli/commands.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.145559 glamconv-0.3.1/glamconv/eac/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      695 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/__init__.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     6562 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/adjusters.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.145559 glamconv-0.3.1/glamconv/eac/ape-eac-schema/
+-rw-rw-r--   0 katia     (1000) katia     (1000)    60710 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/ape-eac-schema/apeEAC-CPF.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3180 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/ape-eac-schema/xlink.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5695 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/ape-eac-schema/xml.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)    13772 2023-05-09 17:51:11.000000 glamconv-0.3.1/glamconv/eac/cleaners.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2859 2023-05-09 17:51:11.000000 glamconv-0.3.1/glamconv/eac/default-eac-cpf-to-ape-settings.json
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.145559 glamconv-0.3.1/glamconv/eac/eac-cpf-schema/
+-rw-rw-r--   0 katia     (1000) katia     (1000)    46012 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/eac-cpf-schema/cpf.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3180 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/eac-cpf-schema/xlink.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5695 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/eac-cpf-schema/xml.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1171 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/formats.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2524 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/namespacers.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)      904 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/registration.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     6488 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/required_elts_adders.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1365 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/supplementers.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     8530 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/text_data.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1509 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/utils.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2659 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/eac/validators.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.145559 glamconv-0.3.1/glamconv/ead/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      692 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/ead/__init__.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    12891 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/adjusters.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.149559 glamconv-0.3.1/glamconv/ead/ape-ead-schema/
+-rw-rw-r--   0 katia     (1000) katia     (1000)    76857 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ape-ead-schema/apeEAD.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3180 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ape-ead-schema/xlink.xsd
+-rw-rw-r--   0 katia     (1000) katia     (1000)    15380 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/arch_data.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    18492 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/cleaners.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     7663 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/default-ead2-to-ape-settings.json
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.153559 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/
+-rw-rw-r--   0 katia     (1000) katia     (1000)   186679 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/ead.dtd
+-rw-rw-r--   0 katia     (1000) katia     (1000)    38830 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/eadlocal.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5910 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-cyr1.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3513 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-cyr2.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2433 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-dia.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4598 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk1.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3334 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk2.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4159 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk3.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4257 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk4.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     6160 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-lat1.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)    10378 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-lat2.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5671 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-num.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     6182 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-pub.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4498 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-tech.ent
+-rw-rw-r--   0 katia     (1000) katia     (1000)    23328 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/ead_2002_correcters.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1172 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/ead/formats.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    14362 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/header.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    21258 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/link_managers.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2457 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/namespacers.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)      972 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/registration.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1358 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/supplementers.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    27816 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/text_data.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1588 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/ead/utils.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2528 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/ead/validators.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.153559 glamconv-0.3.1/glamconv/transformer/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      327 2021-04-15 12:24:08.000000 glamconv-0.3.1/glamconv/transformer/__init__.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5601 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/transformer/actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1010 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/transformer/formats.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2827 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/transformer/libraries.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4723 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/transformer/logger.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4361 2023-03-19 19:24:49.000000 glamconv-0.3.1/glamconv/transformer/parameters.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     7728 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/transformer/processes.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1760 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/transformer/rw_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3535 2023-05-05 09:17:54.000000 glamconv-0.3.1/glamconv/utils.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.141559 glamconv-0.3.1/glamconv.egg-info/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      409 2023-05-09 17:56:15.000000 glamconv-0.3.1/glamconv.egg-info/PKG-INFO
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2916 2023-05-09 17:56:16.000000 glamconv-0.3.1/glamconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 katia     (1000) katia     (1000)        1 2023-05-09 17:56:15.000000 glamconv-0.3.1/glamconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 katia     (1000) katia     (1000)        1 2021-04-15 12:24:51.000000 glamconv-0.3.1/glamconv.egg-info/not-zip-safe
+-rw-rw-r--   0 katia     (1000) katia     (1000)        5 2023-05-09 17:56:15.000000 glamconv-0.3.1/glamconv.egg-info/requires.txt
+-rw-rw-r--   0 katia     (1000) katia     (1000)        9 2023-05-09 17:56:15.000000 glamconv-0.3.1/glamconv.egg-info/top_level.txt
+-rw-rw-r--   0 katia     (1000) katia     (1000)       38 2023-05-09 17:56:16.157559 glamconv-0.3.1/setup.cfg
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1200 2023-05-09 17:51:11.000000 glamconv-0.3.1/setup.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.157559 glamconv-0.3.1/test/
+-rw-rw-r--   0 katia     (1000) katia     (1000)      613 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/__init__.py
+drwxrwxr-x   0 katia     (1000) katia     (1000)        0 2023-05-09 17:56:16.157559 glamconv-0.3.1/test/data/
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1089 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/data/simple-eac.xml
+-rw-rw-r--   0 katia     (1000) katia     (1000)      239 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/data/simple-ead.xml
+-rw-rw-r--   0 katia     (1000) katia     (1000)    21088 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_eac_adjusters_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    67466 2023-05-09 17:51:11.000000 glamconv-0.3.1/test/test_eac_cleaners_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     5482 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_eac_namespacers_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    10637 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_eac_required_elts_adders_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1790 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_eac_supplementers_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    30504 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_eac_text_data_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3814 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_eac_validators_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    14333 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_adjusters_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    15398 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_arch_data_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    72836 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_cleaners_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    35415 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_ead_2002_correctors_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)    20845 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_header_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     4873 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_namespacers_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     1455 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_supplementers_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     3195 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_ead_validators_actions.py
+-rw-rw-r--   0 katia     (1000) katia     (1000)     2974 2023-05-05 09:17:54.000000 glamconv-0.3.1/test/test_transformer_rw_actions.py
```

### Comparing `glamconv-0.3.0/examples/ead-transform.py` & `glamconv-0.3.1/examples/ead-transform.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/examples/generic-ead-transformation.json` & `glamconv-0.3.1/examples/generic-ead-transformation.json`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/cli/commands.py` & `glamconv-0.3.1/glamconv/cli/commands.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/__init__.py` & `glamconv-0.3.1/glamconv/eac/__init__.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/adjusters.py` & `glamconv-0.3.1/glamconv/eac/adjusters.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/ape-eac-schema/apeEAC-CPF.xsd` & `glamconv-0.3.1/glamconv/eac/ape-eac-schema/apeEAC-CPF.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/ape-eac-schema/xlink.xsd` & `glamconv-0.3.1/glamconv/eac/ape-eac-schema/xlink.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/ape-eac-schema/xml.xsd` & `glamconv-0.3.1/glamconv/eac/ape-eac-schema/xml.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/cleaners.py` & `glamconv-0.3.1/glamconv/eac/cleaners.py`

 * *Files 6% similar despite different names*

```diff
@@ -329,7 +329,39 @@
             )
             if log_details:
                 logger.warning(
                     "The following elements have been deleted:\n"
                     + "\n".join(deleted_elts)
                 )
         return xml_root
+
+
+class EmptySourcesEraser(TransformAction):
+    applicable_for = (EAC_CPF,)
+    uid = "empty-sources-eraser"
+    name = "Erasing the <sources> element if it doesn't contain any <source> elements"
+    category = "Cleansing"
+    desc = (
+        "Ape-EAC only allow a <sources> element in <control> if it contains, "
+        "at least, one <source> child element. This action deletes all the "
+        "empty <sources> elements."
+    )
+
+    def _execute(self, xml_root, logger, log_details):
+        count = 0
+        deleted_elts = []
+        for xml_elt in xml_root.xpath("control/sources[not(source)]"):
+            count += 1
+            if log_details:
+                deleted_elts.append(log_element(xml_elt))
+            xml_elt.getparent().remove(xml_elt)
+        if count > 0:
+            logger.warning(
+                "Deleting empty <sources> elements in <control>. {count} "
+                "elements have been deleted."
+            )
+            if log_details:
+                logger.warning(
+                    "The following elements have been deleted:\n"
+                    + "\n".join(deleted_elts)
+                )
+        return xml_root
```

### Comparing `glamconv-0.3.0/glamconv/eac/default-eac-cpf-to-ape-settings.json` & `glamconv-0.3.1/glamconv/eac/default-eac-cpf-to-ape-settings.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9943181818181819%*

 * *Differences: {"'steps'": "{insert: [(17, OrderedDict([('id', 'empty-sources-eraser'), ('log_details', False), "*

 * *            "('params', OrderedDict())]))]}"}*

```diff
@@ -85,14 +85,19 @@
         },
         {
             "id": "description-children-text-elements-converter",
             "log_details": false,
             "params": {}
         },
         {
+            "id": "empty-sources-eraser",
+            "log_details": false,
+            "params": {}
+        },
+        {
             "id": "eac-cpf-namespace-adder",
             "log_details": false,
             "params": {}
         },
         {
             "id": "eac-ape-validator",
             "log_details": true,
```

### Comparing `glamconv-0.3.0/glamconv/eac/eac-cpf-schema/cpf.xsd` & `glamconv-0.3.1/glamconv/eac/eac-cpf-schema/cpf.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/eac-cpf-schema/xlink.xsd` & `glamconv-0.3.1/glamconv/eac/eac-cpf-schema/xlink.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/eac-cpf-schema/xml.xsd` & `glamconv-0.3.1/glamconv/eac/eac-cpf-schema/xml.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/formats.py` & `glamconv-0.3.1/glamconv/eac/formats.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/namespacers.py` & `glamconv-0.3.1/glamconv/eac/namespacers.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/registration.py` & `glamconv-0.3.1/glamconv/eac/registration.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/required_elts_adders.py` & `glamconv-0.3.1/glamconv/eac/required_elts_adders.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/supplementers.py` & `glamconv-0.3.1/glamconv/eac/supplementers.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/text_data.py` & `glamconv-0.3.1/glamconv/eac/text_data.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/utils.py` & `glamconv-0.3.1/glamconv/eac/utils.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/eac/validators.py` & `glamconv-0.3.1/glamconv/eac/validators.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/__init__.py` & `glamconv-0.3.1/glamconv/ead/__init__.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/adjusters.py` & `glamconv-0.3.1/glamconv/ead/adjusters.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ape-ead-schema/apeEAD.xsd` & `glamconv-0.3.1/glamconv/ead/ape-ead-schema/apeEAD.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ape-ead-schema/xlink.xsd` & `glamconv-0.3.1/glamconv/ead/ape-ead-schema/xlink.xsd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/arch_data.py` & `glamconv-0.3.1/glamconv/ead/arch_data.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/cleaners.py` & `glamconv-0.3.1/glamconv/ead/cleaners.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/default-ead2-to-ape-settings.json` & `glamconv-0.3.1/glamconv/ead/default-ead2-to-ape-settings.json`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/ead.dtd` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/ead.dtd`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/eadlocal.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/eadlocal.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-cyr1.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-cyr1.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-cyr2.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-cyr2.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-dia.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-dia.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk1.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk1.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk2.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk2.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk3.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk3.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-grk4.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-grk4.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-lat1.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-lat1.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-lat2.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-lat2.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-num.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-num.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-pub.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-pub.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead-2002-dtd/iso-tech.ent` & `glamconv-0.3.1/glamconv/ead/ead-2002-dtd/iso-tech.ent`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/ead_2002_correcters.py` & `glamconv-0.3.1/glamconv/ead/ead_2002_correcters.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/formats.py` & `glamconv-0.3.1/glamconv/ead/formats.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/header.py` & `glamconv-0.3.1/glamconv/ead/header.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/link_managers.py` & `glamconv-0.3.1/glamconv/ead/link_managers.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/namespacers.py` & `glamconv-0.3.1/glamconv/ead/namespacers.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/registration.py` & `glamconv-0.3.1/glamconv/ead/registration.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/supplementers.py` & `glamconv-0.3.1/glamconv/ead/supplementers.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/text_data.py` & `glamconv-0.3.1/glamconv/ead/text_data.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/utils.py` & `glamconv-0.3.1/glamconv/ead/utils.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/ead/validators.py` & `glamconv-0.3.1/glamconv/ead/validators.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/actions.py` & `glamconv-0.3.1/glamconv/transformer/actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/formats.py` & `glamconv-0.3.1/glamconv/transformer/formats.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/libraries.py` & `glamconv-0.3.1/glamconv/transformer/libraries.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/logger.py` & `glamconv-0.3.1/glamconv/transformer/logger.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/parameters.py` & `glamconv-0.3.1/glamconv/transformer/parameters.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/processes.py` & `glamconv-0.3.1/glamconv/transformer/processes.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/transformer/rw_actions.py` & `glamconv-0.3.1/glamconv/transformer/rw_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv/utils.py` & `glamconv-0.3.1/glamconv/utils.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/glamconv.egg-info/SOURCES.txt` & `glamconv-0.3.1/glamconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/setup.py` & `glamconv-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 with open(osp.join(osp.dirname(__file__), "README.rst")) as f:
     long_description = f.read()
 
 
 setup(
     name="glamconv",
-    version="0.3.0",
+    version="0.3.1",
     license="LGPL",
     description=description,
     long_description=description,
     author="Logilab S.A. (Paris, FRANCE)",
     author_email="contact@logilab.fr",
     url="http://www.logilab.org/project/glamconv",
     classifiers=[
```

### Comparing `glamconv-0.3.0/test/__init__.py` & `glamconv-0.3.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/data/simple-eac.xml` & `glamconv-0.3.1/test/data/simple-eac.xml`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_eac_adjusters_actions.py` & `glamconv-0.3.1/test/test_eac_adjusters_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_eac_cleaners_actions.py` & `glamconv-0.3.1/test/test_eac_cleaners_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from glamconv.utils import NS
 from glamconv.eac.cleaners import (
     AttributesEraser,
     MultipleIdentitiesEraser,
     AdditionalLanguageDeclarationEraser,
     AdditionalNameOrEntryEraser,
     WrappingObjectsEraser,
+    EmptySourcesEraser,
 )
 
 
 DATA_EAC_CPF = """
 <eac-cpf xmlns:xlink="http://www.w3.org/1999/xlink">
   <control>
     <recordId>TEST01</recordId>
@@ -45,14 +46,43 @@
 
 def build_qname(prefixed_name):
     prefix, *local_name = prefixed_name.split(":", 1)
     qname = f"{{{NS[prefix]}}}{local_name[0]}" if len(local_name) > 0 else prefixed_name
     return qname
 
 
+class TestEmptySourcesEraser(ActionTestCase):
+    action_class = EmptySourcesEraser
+
+    def test_non_empty_sources(self):
+        inp_root = etree.fromstring(DATA_EAC_CPF)
+        inp_root[0].append(
+            etree.fromstring(
+                "<sources>"
+                '<source lastDateTimeVerified="2023-05-09T19:26:00Z">'
+                "<sourceEntry>TEST10</sourceEntry></source>"
+                "</sources>"
+            )
+        )
+        out_root = self.run_action(inp_root)
+        self.assertEqual(len(out_root[0]), 5)
+        self.assertEqual(out_root[0][4].tag, "sources")
+        self.assertEqual(len(out_root[0][4]), 1)
+        self.assertEqual(out_root[0][4][0].tag, "source")
+        self.assertEqual(out_root[0][4][0][0].tag, "sourceEntry")
+        self.assertEqual(out_root[0][4][0][0].text, "TEST10")
+
+    def test_empty_sources(self):
+        inp_root = etree.fromstring(DATA_EAC_CPF)
+        inp_root[0].append(etree.fromstring("<sources/>"))
+        out_root = self.run_action(inp_root)
+        self.assertEqual(len(out_root[0]), 4)
+        self.assertEqual(out_root[0][-1].tag, "maintenanceHistory")
+
+
 class TestWrappingObjectsEraser(ActionTestCase):
     action_class = WrappingObjectsEraser
 
     def test_wrapping_objects_in_relations_children(self):
         for prt_name in ("cpfRelation", "resourceRelation", "functionRelation"):
             with self.subTest(parent_name=prt_name):
                 inp_root = etree.fromstring(DATA_EAC_CPF)
```

### Comparing `glamconv-0.3.0/test/test_eac_namespacers_actions.py` & `glamconv-0.3.1/test/test_eac_namespacers_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_eac_required_elts_adders_actions.py` & `glamconv-0.3.1/test/test_eac_required_elts_adders_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_eac_supplementers_actions.py` & `glamconv-0.3.1/test/test_eac_supplementers_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_eac_text_data_actions.py` & `glamconv-0.3.1/test/test_eac_text_data_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_eac_validators_actions.py` & `glamconv-0.3.1/test/test_eac_validators_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_adjusters_actions.py` & `glamconv-0.3.1/test/test_ead_adjusters_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_arch_data_actions.py` & `glamconv-0.3.1/test/test_ead_arch_data_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_cleaners_actions.py` & `glamconv-0.3.1/test/test_ead_cleaners_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_ead_2002_correctors_actions.py` & `glamconv-0.3.1/test/test_ead_ead_2002_correctors_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_header_actions.py` & `glamconv-0.3.1/test/test_ead_header_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_namespacers_actions.py` & `glamconv-0.3.1/test/test_ead_namespacers_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_supplementers_actions.py` & `glamconv-0.3.1/test/test_ead_supplementers_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_ead_validators_actions.py` & `glamconv-0.3.1/test/test_ead_validators_actions.py`

 * *Files identical despite different names*

### Comparing `glamconv-0.3.0/test/test_transformer_rw_actions.py` & `glamconv-0.3.1/test/test_transformer_rw_actions.py`

 * *Files identical despite different names*

