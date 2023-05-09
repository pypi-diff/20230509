# Comparing `tmp/tumfl-0.1.6.tar.gz` & `tmp/tumfl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumfl-0.1.6.tar", last modified: Tue May  9 15:22:36 2023, max compression
+gzip compressed data, was "tumfl-0.1.7.tar", last modified: Tue May  9 19:07:22 2023, max compression
```

## Comparing `tumfl-0.1.6.tar` & `tumfl-0.1.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.590404 tumfl-0.1.6/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-09 15:22:36.590404 tumfl-0.1.6/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      403 2023-05-07 16:04:09.000000 tumfl-0.1.6/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1075 2023-05-09 15:21:42.000000 tumfl-0.1.6/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      175 2023-05-09 15:22:36.591404 tumfl-0.1.6/setup.cfg
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.584404 tumfl-0.1.6/test/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     5428 2023-05-09 15:21:53.000000 tumfl-0.1.6/test/test_formatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    12040 2023-05-07 15:43:26.000000 tumfl-0.1.6/test/test_lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    37047 2023-05-07 17:12:29.000000 tumfl-0.1.6/test/test_parser.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.585404 tumfl-0.1.6/tumfl/
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.586404 tumfl-0.1.6/tumfl/AST/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1783 2023-05-09 06:19:55.000000 tumfl-0.1.6/tumfl/AST/ASTNode.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      656 2023-05-07 15:47:19.000000 tumfl-0.1.6/tumfl/AST/BaseFunctionDefinition.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.588404 tumfl-0.1.6/tumfl/AST/Expression/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2375 2023-05-08 20:24:18.000000 tumfl-0.1.6/tumfl/AST/Expression/BinOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/Expression/Boolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:44:48.000000 tumfl-0.1.6/tumfl/AST/Expression/ExpFunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      809 2023-05-07 15:44:44.000000 tumfl-0.1.6/tumfl/AST/Expression/ExpFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 15:44:56.000000 tumfl-0.1.6/tumfl/AST/Expression/ExpMethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.6/tumfl/AST/Expression/Expression.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      419 2023-05-07 17:13:35.000000 tumfl-0.1.6/tumfl/AST/Expression/Index.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 21:14:24.000000 tumfl-0.1.6/tumfl/AST/Expression/Name.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      444 2023-05-07 17:13:17.000000 tumfl-0.1.6/tumfl/AST/Expression/NamedIndex.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/Expression/Nil.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2172 2023-05-07 20:16:49.000000 tumfl-0.1.6/tumfl/AST/Expression/Number.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/Expression/String.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      373 2023-05-07 15:45:28.000000 tumfl-0.1.6/tumfl/AST/Expression/Table.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1066 2023-05-07 15:59:18.000000 tumfl-0.1.6/tumfl/AST/Expression/TableField.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      694 2023-05-07 15:45:38.000000 tumfl-0.1.6/tumfl/AST/Expression/UnOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/Expression/Vararg.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      171 2023-05-07 15:59:24.000000 tumfl-0.1.6/tumfl/AST/Expression/Variable.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-09 15:21:53.000000 tumfl-0.1.6/tumfl/AST/Expression/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.590404 tumfl-0.1.6/tumfl/AST/Statement/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      519 2023-05-07 15:45:49.000000 tumfl-0.1.6/tumfl/AST/Statement/Assign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:45:53.000000 tumfl-0.1.6/tumfl/AST/Statement/Block.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      250 2023-05-07 15:45:58.000000 tumfl-0.1.6/tumfl/AST/Statement/Break.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.6/tumfl/AST/Statement/Chunk.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      537 2023-05-07 15:46:04.000000 tumfl-0.1.6/tumfl/AST/Statement/FunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1123 2023-05-07 15:46:10.000000 tumfl-0.1.6/tumfl/AST/Statement/FunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      337 2023-05-07 15:46:15.000000 tumfl-0.1.6/tumfl/AST/Statement/Goto.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 15:46:20.000000 tumfl-0.1.6/tumfl/AST/Statement/If.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 15:46:25.000000 tumfl-0.1.6/tumfl/AST/Statement/IterativeFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      349 2023-05-07 15:46:29.000000 tumfl-0.1.6/tumfl/AST/Statement/Label.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1302 2023-05-07 21:05:56.000000 tumfl-0.1.6/tumfl/AST/Statement/LocalAssign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      977 2023-05-07 15:46:40.000000 tumfl-0.1.6/tumfl/AST/Statement/LocalFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      653 2023-05-07 15:46:47.000000 tumfl-0.1.6/tumfl/AST/Statement/MethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      780 2023-05-07 15:46:51.000000 tumfl-0.1.6/tumfl/AST/Statement/NumericFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      439 2023-05-07 15:46:55.000000 tumfl-0.1.6/tumfl/AST/Statement/Repeat.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      236 2023-05-07 15:47:00.000000 tumfl-0.1.6/tumfl/AST/Statement/Semicolon.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/Statement/Statement.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      426 2023-05-07 15:47:09.000000 tumfl-0.1.6/tumfl/AST/Statement/While.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/Statement/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/AST/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/Token.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      150 2023-05-07 22:06:47.000000 tumfl-0.1.6/tumfl/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     6867 2023-05-09 15:21:23.000000 tumfl-0.1.6/tumfl/basic_walker.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.6/tumfl/error.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    16534 2023-05-09 12:41:26.000000 tumfl-0.1.6/tumfl/formatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    14367 2023-05-09 11:45:54.000000 tumfl-0.1.6/tumfl/lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    32663 2023-05-09 14:55:41.000000 tumfl-0.1.6/tumfl/parser.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.6/tumfl/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 15:22:36.586404 tumfl-0.1.6/tumfl.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-09 15:22:36.000000 tumfl-0.1.6/tumfl.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1683 2023-05-09 15:22:36.000000 tumfl-0.1.6/tumfl.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-09 15:22:36.000000 tumfl-0.1.6/tumfl.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-09 15:22:36.000000 tumfl-0.1.6/tumfl.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-09 15:22:36.000000 tumfl-0.1.6/tumfl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.493871 tumfl-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-09 19:07:22.497871 tumfl-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 19:07:09.000000 tumfl-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-09 19:07:09.000000 tumfl-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 19:07:22.497871 tumfl-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.485871 tumfl-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-05-09 19:07:09.000000 tumfl-0.1.7/test/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-09 19:07:09.000000 tumfl-0.1.7/test/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37047 2023-05-09 19:07:09.000000 tumfl-0.1.7/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.489871 tumfl-0.1.7/tumfl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.489871 tumfl-0.1.7/tumfl/AST/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/ASTNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/BaseFunctionDefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.493871 tumfl-0.1.7/tumfl/AST/Expression/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/BinOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/ExpFunctionCall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/ExpFunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/ExpMethodInvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/NamedIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Nil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/String.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/TableField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/UnOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Vararg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.493871 tumfl-0.1.7/tumfl/AST/Statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/FunctionCall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/FunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Goto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/IterativeFor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/LocalAssign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/LocalFunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/MethodInvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/NumericFor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Semicolon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/While.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/basic_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32663 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.489871 tumfl-0.1.7/tumfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/top_level.txt
```

### Comparing `tumfl-0.1.6/PKG-INFO` & `tumfl-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.6/pyproject.toml` & `tumfl-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tumfl"
-version = "0.1.6"
+version = "0.1.7"
 description = "The Ultimate Minimizer For Lua: minimize your lua scripts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["lua", "minimizer", "ast"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `tumfl-0.1.6/test/test_lexer.py` & `tumfl-0.1.7/test/test_lexer.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/test/test_parser.py` & `tumfl-0.1.7/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/ASTNode.py` & `tumfl-0.1.7/tumfl/AST/ASTNode.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/BaseFunctionDefinition.py` & `tumfl-0.1.7/tumfl/AST/BaseFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/ExpFunctionDefinition.py` & `tumfl-0.1.7/tumfl/AST/Expression/ExpFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/ExpMethodInvocation.py` & `tumfl-0.1.7/tumfl/AST/Expression/ExpMethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/Name.py` & `tumfl-0.1.7/tumfl/AST/Expression/Name.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/Number.py` & `tumfl-0.1.7/tumfl/AST/Expression/Number.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/String.py` & `tumfl-0.1.7/tumfl/AST/Expression/String.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/TableField.py` & `tumfl-0.1.7/tumfl/AST/Expression/TableField.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/UnOp.py` & `tumfl-0.1.7/tumfl/AST/Expression/UnOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Expression/__init__.py` & `tumfl-0.1.7/tumfl/AST/Expression/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/Assign.py` & `tumfl-0.1.7/tumfl/AST/Statement/Assign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/FunctionCall.py` & `tumfl-0.1.7/tumfl/AST/Statement/FunctionCall.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/FunctionDefinition.py` & `tumfl-0.1.7/tumfl/AST/Statement/FunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/If.py` & `tumfl-0.1.7/tumfl/AST/Statement/If.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/IterativeFor.py` & `tumfl-0.1.7/tumfl/AST/Statement/IterativeFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/LocalAssign.py` & `tumfl-0.1.7/tumfl/AST/Statement/LocalAssign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/LocalFunctionDefinition.py` & `tumfl-0.1.7/tumfl/AST/Statement/LocalFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/MethodInvocation.py` & `tumfl-0.1.7/tumfl/AST/Statement/MethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/NumericFor.py` & `tumfl-0.1.7/tumfl/AST/Statement/NumericFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/AST/Statement/__init__.py` & `tumfl-0.1.7/tumfl/AST/Statement/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/Token.py` & `tumfl-0.1.7/tumfl/Token.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/basic_walker.py` & `tumfl-0.1.7/tumfl/basic_walker.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/error.py` & `tumfl-0.1.7/tumfl/error.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/formatter.py` & `tumfl-0.1.7/tumfl/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     USE_CALL_SHORTHAND: bool = False
     # Remove all characters that are not strictly required
     REMOVE_UNNECESSARY_CHARS: bool = False
     # Add brackets to arithmetic expressions no matter the use
     ADD_ALL_BRACKETS: bool = False
     # Add brackets to arithmetic expressions if the order is potentially confusing
     ADD_CLOSE_BRACKETS: bool = True
+    # Add a space around `=` in table constructors
+    SPACE_IN_TABLE: bool = True
 
 
 class MinifiedStyle(FormattingStyle):
     # pylint: disable=too-few-public-methods
 
     STATEMENT_SEPARATOR = ";"
     INDENTATION = ""
@@ -157,15 +159,15 @@
         result += ["end"]
         return result
 
     def visit_Index(self, node: Index) -> Retype:
         return [*self.visit(node.lhs), "[", *self.visit(node.variable_name), "]"]
 
     def visit_Label(self, node: Label) -> Retype:
-        return ["::", self.visit(node.label_name), "::"]
+        return ["::", *self.visit(node.label_name), "::"]
 
     def visit_Name(self, node: Name) -> Retype:
         return [node.variable_name]
 
     def visit_Nil(self, _node: Nil) -> Retype:
         return ["nil"]
 
@@ -186,16 +188,16 @@
         return [";"]
 
     def visit_String(self, node: String) -> Retype:
         if "\n" in node.value:
             level: int = self._find_level(node.value)
             return [f"[{'=' * level}[{node.value}]{'=' * level}]"]
         if self.s.USE_SINGLE_QUOTE and node.value.count("'") < node.value.count('"'):
-            return ["'" + node.value.replace('"', '\\"') + "'"]
-        return ['"' + node.value.replace("'", "\\'") + '"']
+            return ["'" + node.value.replace("'", "\\'") + "'"]
+        return ['"' + node.value.replace('"', '\\"') + '"']
 
     def visit_Table(self, node: Table) -> Retype:
         return ["{", *self._format_args(node.fields), "}"]
 
     def visit_Vararg(self, _node: Vararg) -> Retype:
         return ["..."]
 
@@ -211,27 +213,27 @@
             "end",
         ]
 
     def _need_brackets(
         self, own_node: BinOp, other_node: Expression, care_unop: bool
     ) -> bool:
         own_precedence: int = own_node.op.get_precedence()
-        close_precedence: int = own_precedence + (
-            1 if self.s.ADD_CLOSE_BRACKETS else -1
-        )
         return (
             self.s.ADD_ALL_BRACKETS
             or isinstance(other_node, BinOp)
             and (
-                other_node.op.get_precedence() < own_precedence
-                or other_node.op.get_precedence() == close_precedence
+                own_precedence > other_node.op.get_precedence()
+                or self.s.ADD_CLOSE_BRACKETS
+                and other_node.op in own_node.op.get_optional_brackets()
             )
             or (care_unop or self.s.ADD_CLOSE_BRACKETS)
             and isinstance(other_node, UnOp)
-            and (10 < own_precedence or 10 == close_precedence)
+            and (
+                own_precedence > 10 or self.s.ADD_CLOSE_BRACKETS and own_precedence >= 9
+            )
         )
 
     def visit_BinOp(self, node: BinOp) -> Retype:
         result: Retype = []
         if self._need_brackets(node, node.left, True):
             result += ["(", *self.visit(node.left), ")"]
         else:
```

### Comparing `tumfl-0.1.6/tumfl/lexer.py` & `tumfl-0.1.7/tumfl/lexer.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/parser.py` & `tumfl-0.1.7/tumfl/parser.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl/utils.py` & `tumfl-0.1.7/tumfl/utils.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.6/tumfl.egg-info/PKG-INFO` & `tumfl-0.1.7/tumfl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.6/tumfl.egg-info/SOURCES.txt` & `tumfl-0.1.7/tumfl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

