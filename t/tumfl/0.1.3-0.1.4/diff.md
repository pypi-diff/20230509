# Comparing `tmp/tumfl-0.1.3.tar.gz` & `tmp/tumfl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumfl-0.1.3.tar", last modified: Mon May  8 20:45:01 2023, max compression
+gzip compressed data, was "tumfl-0.1.4.tar", last modified: Tue May  9 06:20:30 2023, max compression
```

## Comparing `tumfl-0.1.3.tar` & `tumfl-0.1.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.332873 tumfl-0.1.3/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-08 20:45:01.332873 tumfl-0.1.3/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      403 2023-05-07 16:04:09.000000 tumfl-0.1.3/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1075 2023-05-08 20:44:25.000000 tumfl-0.1.3/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      175 2023-05-08 20:45:01.332873 tumfl-0.1.3/setup.cfg
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.326873 tumfl-0.1.3/test/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    12040 2023-05-07 15:43:26.000000 tumfl-0.1.3/test/test_lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    37047 2023-05-07 17:12:29.000000 tumfl-0.1.3/test/test_parser.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.327873 tumfl-0.1.3/tumfl/
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.328873 tumfl-0.1.3/tumfl/AST/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1303 2023-05-07 15:59:04.000000 tumfl-0.1.3/tumfl/AST/ASTNode.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      656 2023-05-07 15:47:19.000000 tumfl-0.1.3/tumfl/AST/BaseFunctionDefinition.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.330873 tumfl-0.1.3/tumfl/AST/Expression/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2375 2023-05-08 20:24:18.000000 tumfl-0.1.3/tumfl/AST/Expression/BinOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/Expression/Boolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:44:48.000000 tumfl-0.1.3/tumfl/AST/Expression/ExpFunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      809 2023-05-07 15:44:44.000000 tumfl-0.1.3/tumfl/AST/Expression/ExpFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 15:44:56.000000 tumfl-0.1.3/tumfl/AST/Expression/ExpMethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.3/tumfl/AST/Expression/Expression.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      419 2023-05-07 17:13:35.000000 tumfl-0.1.3/tumfl/AST/Expression/Index.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 21:14:24.000000 tumfl-0.1.3/tumfl/AST/Expression/Name.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      444 2023-05-07 17:13:17.000000 tumfl-0.1.3/tumfl/AST/Expression/NamedIndex.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/Expression/Nil.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2172 2023-05-07 20:16:49.000000 tumfl-0.1.3/tumfl/AST/Expression/Number.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/Expression/String.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      373 2023-05-07 15:45:28.000000 tumfl-0.1.3/tumfl/AST/Expression/Table.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1066 2023-05-07 15:59:18.000000 tumfl-0.1.3/tumfl/AST/Expression/TableField.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      694 2023-05-07 15:45:38.000000 tumfl-0.1.3/tumfl/AST/Expression/UnOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/Expression/Vararg.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      171 2023-05-07 15:59:24.000000 tumfl-0.1.3/tumfl/AST/Expression/Variable.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-08 20:41:45.000000 tumfl-0.1.3/tumfl/AST/Expression/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.332873 tumfl-0.1.3/tumfl/AST/Statement/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      519 2023-05-07 15:45:49.000000 tumfl-0.1.3/tumfl/AST/Statement/Assign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:45:53.000000 tumfl-0.1.3/tumfl/AST/Statement/Block.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      250 2023-05-07 15:45:58.000000 tumfl-0.1.3/tumfl/AST/Statement/Break.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.3/tumfl/AST/Statement/Chunk.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      537 2023-05-07 15:46:04.000000 tumfl-0.1.3/tumfl/AST/Statement/FunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1123 2023-05-07 15:46:10.000000 tumfl-0.1.3/tumfl/AST/Statement/FunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      337 2023-05-07 15:46:15.000000 tumfl-0.1.3/tumfl/AST/Statement/Goto.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 15:46:20.000000 tumfl-0.1.3/tumfl/AST/Statement/If.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 15:46:25.000000 tumfl-0.1.3/tumfl/AST/Statement/IterativeFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      349 2023-05-07 15:46:29.000000 tumfl-0.1.3/tumfl/AST/Statement/Label.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1302 2023-05-07 21:05:56.000000 tumfl-0.1.3/tumfl/AST/Statement/LocalAssign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      977 2023-05-07 15:46:40.000000 tumfl-0.1.3/tumfl/AST/Statement/LocalFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      653 2023-05-07 15:46:47.000000 tumfl-0.1.3/tumfl/AST/Statement/MethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      780 2023-05-07 15:46:51.000000 tumfl-0.1.3/tumfl/AST/Statement/NumericFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      439 2023-05-07 15:46:55.000000 tumfl-0.1.3/tumfl/AST/Statement/Repeat.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      236 2023-05-07 15:47:00.000000 tumfl-0.1.3/tumfl/AST/Statement/Semicolon.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/Statement/Statement.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      426 2023-05-07 15:47:09.000000 tumfl-0.1.3/tumfl/AST/Statement/While.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/Statement/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/AST/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/Token.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      150 2023-05-07 22:06:47.000000 tumfl-0.1.3/tumfl/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     5481 2023-05-07 21:31:57.000000 tumfl-0.1.3/tumfl/basic_walker.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.3/tumfl/error.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    16490 2023-05-08 20:41:41.000000 tumfl-0.1.3/tumfl/formatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    14367 2023-05-07 15:55:19.000000 tumfl-0.1.3/tumfl/lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    32621 2023-05-07 17:45:47.000000 tumfl-0.1.3/tumfl/parser.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.3/tumfl/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-08 20:45:01.328873 tumfl-0.1.3/tumfl.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-08 20:45:01.000000 tumfl-0.1.3/tumfl.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1660 2023-05-08 20:45:01.000000 tumfl-0.1.3/tumfl.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-08 20:45:01.000000 tumfl-0.1.3/tumfl.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-08 20:45:01.000000 tumfl-0.1.3/tumfl.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-08 20:45:01.000000 tumfl-0.1.3/tumfl.egg-info/top_level.txt
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.036494 tumfl-0.1.4/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-09 06:20:30.036494 tumfl-0.1.4/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      403 2023-05-07 16:04:09.000000 tumfl-0.1.4/README.md
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1075 2023-05-09 06:18:47.000000 tumfl-0.1.4/pyproject.toml
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      175 2023-05-09 06:20:30.036494 tumfl-0.1.4/setup.cfg
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.030493 tumfl-0.1.4/test/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    12040 2023-05-07 15:43:26.000000 tumfl-0.1.4/test/test_lexer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    37047 2023-05-07 17:12:29.000000 tumfl-0.1.4/test/test_parser.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.031494 tumfl-0.1.4/tumfl/
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.032493 tumfl-0.1.4/tumfl/AST/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1783 2023-05-09 06:19:55.000000 tumfl-0.1.4/tumfl/AST/ASTNode.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      656 2023-05-07 15:47:19.000000 tumfl-0.1.4/tumfl/AST/BaseFunctionDefinition.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.034494 tumfl-0.1.4/tumfl/AST/Expression/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2375 2023-05-08 20:24:18.000000 tumfl-0.1.4/tumfl/AST/Expression/BinOp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/Expression/Boolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:44:48.000000 tumfl-0.1.4/tumfl/AST/Expression/ExpFunctionCall.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      809 2023-05-07 15:44:44.000000 tumfl-0.1.4/tumfl/AST/Expression/ExpFunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 15:44:56.000000 tumfl-0.1.4/tumfl/AST/Expression/ExpMethodInvocation.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.4/tumfl/AST/Expression/Expression.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      419 2023-05-07 17:13:35.000000 tumfl-0.1.4/tumfl/AST/Expression/Index.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 21:14:24.000000 tumfl-0.1.4/tumfl/AST/Expression/Name.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      444 2023-05-07 17:13:17.000000 tumfl-0.1.4/tumfl/AST/Expression/NamedIndex.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/Expression/Nil.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2172 2023-05-07 20:16:49.000000 tumfl-0.1.4/tumfl/AST/Expression/Number.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/Expression/String.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      373 2023-05-07 15:45:28.000000 tumfl-0.1.4/tumfl/AST/Expression/Table.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1066 2023-05-07 15:59:18.000000 tumfl-0.1.4/tumfl/AST/Expression/TableField.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      694 2023-05-07 15:45:38.000000 tumfl-0.1.4/tumfl/AST/Expression/UnOp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/Expression/Vararg.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      171 2023-05-07 15:59:24.000000 tumfl-0.1.4/tumfl/AST/Expression/Variable.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-09 06:20:00.000000 tumfl-0.1.4/tumfl/AST/Expression/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.036494 tumfl-0.1.4/tumfl/AST/Statement/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      519 2023-05-07 15:45:49.000000 tumfl-0.1.4/tumfl/AST/Statement/Assign.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:45:53.000000 tumfl-0.1.4/tumfl/AST/Statement/Block.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      250 2023-05-07 15:45:58.000000 tumfl-0.1.4/tumfl/AST/Statement/Break.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.4/tumfl/AST/Statement/Chunk.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      537 2023-05-07 15:46:04.000000 tumfl-0.1.4/tumfl/AST/Statement/FunctionCall.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1123 2023-05-07 15:46:10.000000 tumfl-0.1.4/tumfl/AST/Statement/FunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      337 2023-05-07 15:46:15.000000 tumfl-0.1.4/tumfl/AST/Statement/Goto.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 15:46:20.000000 tumfl-0.1.4/tumfl/AST/Statement/If.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 15:46:25.000000 tumfl-0.1.4/tumfl/AST/Statement/IterativeFor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      349 2023-05-07 15:46:29.000000 tumfl-0.1.4/tumfl/AST/Statement/Label.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1302 2023-05-07 21:05:56.000000 tumfl-0.1.4/tumfl/AST/Statement/LocalAssign.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      977 2023-05-07 15:46:40.000000 tumfl-0.1.4/tumfl/AST/Statement/LocalFunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      653 2023-05-07 15:46:47.000000 tumfl-0.1.4/tumfl/AST/Statement/MethodInvocation.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      780 2023-05-07 15:46:51.000000 tumfl-0.1.4/tumfl/AST/Statement/NumericFor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      439 2023-05-07 15:46:55.000000 tumfl-0.1.4/tumfl/AST/Statement/Repeat.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      236 2023-05-07 15:47:00.000000 tumfl-0.1.4/tumfl/AST/Statement/Semicolon.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/Statement/Statement.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      426 2023-05-07 15:47:09.000000 tumfl-0.1.4/tumfl/AST/Statement/While.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/Statement/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/AST/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/Token.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      150 2023-05-07 22:06:47.000000 tumfl-0.1.4/tumfl/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     5481 2023-05-07 21:31:57.000000 tumfl-0.1.4/tumfl/basic_walker.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.4/tumfl/error.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    16490 2023-05-08 20:41:41.000000 tumfl-0.1.4/tumfl/formatter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    14367 2023-05-07 15:55:19.000000 tumfl-0.1.4/tumfl/lexer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    32621 2023-05-07 17:45:47.000000 tumfl-0.1.4/tumfl/parser.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.4/tumfl/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-09 06:20:30.031494 tumfl-0.1.4/tumfl.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-09 06:20:30.000000 tumfl-0.1.4/tumfl.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1660 2023-05-09 06:20:30.000000 tumfl-0.1.4/tumfl.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-09 06:20:30.000000 tumfl-0.1.4/tumfl.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-09 06:20:30.000000 tumfl-0.1.4/tumfl.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-09 06:20:30.000000 tumfl-0.1.4/tumfl.egg-info/top_level.txt
```

### Comparing `tumfl-0.1.3/PKG-INFO` & `tumfl-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.3/pyproject.toml` & `tumfl-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tumfl"
-version = "0.1.3"
+version = "0.1.4"
 description = "The Ultimate Minimizer For Lua: minimize your lua scripts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["lua", "minimizer", "ast"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `tumfl-0.1.3/test/test_lexer.py` & `tumfl-0.1.4/test/test_lexer.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/test/test_parser.py` & `tumfl-0.1.4/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/ASTNode.py` & `tumfl-0.1.4/tumfl/AST/ASTNode.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,13 +31,25 @@
             i
             for i in dir(self)
             if not i.startswith("__")
             # ignore "token" for comparison (and parent check)
             and i not in ["replace", "parent", "parent_class", "var", "token"]
         )
 
-    def parent(self, parent: ASTNode) -> None:
+    def parent(self, parent: Optional[ASTNode]) -> None:
         self.parent_class = parent
         for i in self.__dir():
             node: Any = getattr(self, i)
             if isinstance(node, ASTNode):
                 node.parent(self)
+
+    def replace_child(self, to_replace: ASTNode, replacement: ASTNode) -> None:
+        for i in self.__dir():
+            node: Any = getattr(self, i)
+            if node is to_replace:
+                setattr(self, i, replacement)
+                return
+            if isinstance(node, list):
+                for j, element in enumerate(node):
+                    if element is to_replace:
+                        node[j] = replacement
+                        return
```

### Comparing `tumfl-0.1.3/tumfl/AST/BaseFunctionDefinition.py` & `tumfl-0.1.4/tumfl/AST/BaseFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/BinOp.py` & `tumfl-0.1.4/tumfl/AST/Expression/BinOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/ExpFunctionDefinition.py` & `tumfl-0.1.4/tumfl/AST/Expression/ExpFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/ExpMethodInvocation.py` & `tumfl-0.1.4/tumfl/AST/Expression/ExpMethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/Name.py` & `tumfl-0.1.4/tumfl/AST/Expression/Name.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/Number.py` & `tumfl-0.1.4/tumfl/AST/Expression/Number.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/String.py` & `tumfl-0.1.4/tumfl/AST/Expression/String.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/TableField.py` & `tumfl-0.1.4/tumfl/AST/Expression/TableField.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/UnOp.py` & `tumfl-0.1.4/tumfl/AST/Expression/UnOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Expression/__init__.py` & `tumfl-0.1.4/tumfl/AST/Expression/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/Assign.py` & `tumfl-0.1.4/tumfl/AST/Statement/Assign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/FunctionCall.py` & `tumfl-0.1.4/tumfl/AST/Statement/FunctionCall.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/FunctionDefinition.py` & `tumfl-0.1.4/tumfl/AST/Statement/FunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/If.py` & `tumfl-0.1.4/tumfl/AST/Statement/If.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/IterativeFor.py` & `tumfl-0.1.4/tumfl/AST/Statement/IterativeFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/LocalAssign.py` & `tumfl-0.1.4/tumfl/AST/Statement/LocalAssign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/LocalFunctionDefinition.py` & `tumfl-0.1.4/tumfl/AST/Statement/LocalFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/MethodInvocation.py` & `tumfl-0.1.4/tumfl/AST/Statement/MethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/NumericFor.py` & `tumfl-0.1.4/tumfl/AST/Statement/NumericFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/AST/Statement/__init__.py` & `tumfl-0.1.4/tumfl/AST/Statement/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/Token.py` & `tumfl-0.1.4/tumfl/Token.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/basic_walker.py` & `tumfl-0.1.4/tumfl/basic_walker.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/error.py` & `tumfl-0.1.4/tumfl/error.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/formatter.py` & `tumfl-0.1.4/tumfl/formatter.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/lexer.py` & `tumfl-0.1.4/tumfl/lexer.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/parser.py` & `tumfl-0.1.4/tumfl/parser.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl/utils.py` & `tumfl-0.1.4/tumfl/utils.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.3/tumfl.egg-info/PKG-INFO` & `tumfl-0.1.4/tumfl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.3/tumfl.egg-info/SOURCES.txt` & `tumfl-0.1.4/tumfl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

