# Comparing `tmp/python-chess-bughouse-0.27.3.tar.gz` & `tmp/python-chess-bughouse-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-chess-bughouse-0.27.3.tar", last modified: Tue May  2 00:31:42 2023, max compression
+gzip compressed data, was "python-chess-bughouse-0.28.0.tar", last modified: Mon May  8 23:08:57 2023, max compression
```

## Comparing `python-chess-bughouse-0.27.3.tar` & `python-chess-bughouse-0.28.0.tar`

### file list

```diff
@@ -1,22 +1,178 @@
-drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-02 00:31:42.065547 python-chess-bughouse-0.27.3/
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    50737 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/CHANGELOG.rst
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    35147 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/LICENSE.txt
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)       61 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/MANIFEST.in
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    11656 2023-05-02 00:31:42.065547 python-chess-bughouse-0.27.3/PKG-INFO
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    10428 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/README.rst
-drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-02 00:31:42.065547 python-chess-bughouse-0.27.3/chess/
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)   133163 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/chess/__init__.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    97381 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/chess/engine.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    63647 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/chess/gaviota.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    45528 2023-04-30 23:12:48.000000 python-chess-bughouse-0.27.3/chess/pgn.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    27446 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/chess/polyglot.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    26629 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/chess/svg.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    68333 2023-04-29 22:06:45.000000 python-chess-bughouse-0.27.3/chess/syzygy.py
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    48011 2023-04-30 22:27:05.000000 python-chess-bughouse-0.27.3/chess/variant.py
-drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-02 00:31:42.065547 python-chess-bughouse-0.27.3/python_chess_bughouse.egg-info/
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)    11656 2023-05-02 00:31:42.000000 python-chess-bughouse-0.27.3/python_chess_bughouse.egg-info/PKG-INFO
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)      365 2023-05-02 00:31:42.000000 python-chess-bughouse-0.27.3/python_chess_bughouse.egg-info/SOURCES.txt
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)        1 2023-05-02 00:31:42.000000 python-chess-bughouse-0.27.3/python_chess_bughouse.egg-info/dependency_links.txt
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)        6 2023-05-02 00:31:42.000000 python-chess-bughouse-0.27.3/python_chess_bughouse.egg-info/top_level.txt
--rw-r--r--   0 bouanto   (1000) bouanto   (1000)       38 2023-05-02 00:31:42.065547 python-chess-bughouse-0.27.3/setup.cfg
--rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     3789 2023-05-02 00:14:16.000000 python-chess-bughouse-0.27.3/setup.py
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.339903 python-chess-bughouse-0.28.0/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      151 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/.editorconfig
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      294 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/.gitignore
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     5006 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/.travis.yml
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    50737 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/CHANGELOG.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    35147 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/LICENSE.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       61 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/MANIFEST.in
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    11656 2023-05-08 23:08:57.339903 python-chess-bughouse-0.28.0/PKG-INFO
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    10428 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/README.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      418 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/appveyor.yml
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.326570 python-chess-bughouse-0.28.0/chess/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   133273 2023-05-08 23:08:44.000000 python-chess-bughouse-0.28.0/chess/__init__.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    97381 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/chess/engine.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    63647 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/chess/gaviota.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    45528 2023-04-30 23:12:48.000000 python-chess-bughouse-0.28.0/chess/pgn.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    27446 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/chess/polyglot.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    26629 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/chess/svg.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    68333 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/chess/syzygy.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    48011 2023-04-30 22:27:05.000000 python-chess-bughouse-0.28.0/chess/variant.py
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.326570 python-chess-bughouse-0.28.0/data/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1844 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/endgame-dm-4.epd
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1610 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/endgame-dm-5.epd
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    11432 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/endgame.epd
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.326570 python-chess-bughouse-0.28.0/data/gaviota/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     6920 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/MD5SUMS.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     7065 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/SOURCE.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2273 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/TEST-SOURCE.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2021 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/kbk.gtb.cp4
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1754 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/knk.gtb.cp4
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    27435 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/kpk.gtb.cp4
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     9443 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/kqk.gtb.cp4
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    10824 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/gaviota/krk.gtb.cp4
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.326570 python-chess-bughouse-0.28.0/data/pgn/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      745 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/anastasian-lewis.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      832 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/antichess-programfox.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    10280 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/cutechess-fischerrandom.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     4288 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/kasparov-deep-blue-1997.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     3571 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/knightvuillaume-jannlee-zh-lichess.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      241 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/molinari-bordais-1979.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1144 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/saturs-jannlee-zh-lichess.pgn
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     3666 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/pgn/stockfish-learning.pgn
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.326570 python-chess-bughouse-0.28.0/data/polyglot/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       61 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/polyglot/SOURCE.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      112 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/polyglot/lasker-trap.bin
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)  1487264 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/polyglot/performance.bin
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1784 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/suicide-dtm.epd
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      413 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/suicide-dtz.epd
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   232426 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/suicide-stats.epd
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.323237 python-chess-bughouse-0.28.0/data/syzygy/
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.329903 python-chess-bughouse-0.28.0/data/syzygy/atomic/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    15000 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/atomic/SOURCE-5.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    19345 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/atomic/SOURCE-6-DTZ.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    19345 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/atomic/SOURCE-6-WDL.txt
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.329903 python-chess-bughouse-0.28.0/data/syzygy/giveaway/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   176624 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/giveaway/SOURCE-5.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   406392 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/giveaway/SOURCE-6.txt
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.336570 python-chess-bughouse-0.28.0/data/syzygy/regular/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    58000 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBBvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   136272 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBBvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     7632 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBNvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   461840 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBNvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    81424 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBPvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    75792 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBPvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1232 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvKB.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvKB.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2256 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvKN.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvKN.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   107472 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvKP.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     5968 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KBvKP.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1360 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNNvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNNvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    93200 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNPvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   111056 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNPvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1168 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNvKN.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       80 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNvKN.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   148048 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNvKP.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    10640 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KNvKP.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    25104 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KPPvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     8656 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KPPvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     7824 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KPvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     4176 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KPvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   245328 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KPvKP.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    54480 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KPvKP.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     4944 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQBvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   139088 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQBvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     3600 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQNvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   156432 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQNvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    12496 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQPvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    32208 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQPvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     7056 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQQvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    25936 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQQvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     4560 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQRvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    44112 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQRvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      272 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     5328 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     6672 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKB.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   195216 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKB.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    10064 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKN.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   162640 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKN.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    58064 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKP.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   205776 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKP.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    16528 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKQ.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     6736 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKQ.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    20496 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKR.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   309008 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KQvKR.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2832 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRBvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   261776 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRBvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2320 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRNvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   295632 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRNvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     5136 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRPvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    12944 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRPvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1936 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRRvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    53520 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRRvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      208 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvK.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     8272 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvK.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    32912 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKB.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     9936 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKB.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   100048 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKN.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    93200 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKN.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   179408 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKP.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   193424 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKP.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    12944 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKR.rtbw
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     3408 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/KRvKR.rtbz
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    15000 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/SOURCE-5.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    38690 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/SOURCE-6.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      158 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/regular/SOURCE.txt
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.336570 python-chess-bughouse-0.28.0/data/syzygy/suicide/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   325836 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/suicide/SOURCE-5.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)   272580 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/suicide/SOURCE-6-PAWNLESS.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    86996 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/data/syzygy/suicide/TEST-SOURCE.txt
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.336570 python-chess-bughouse-0.28.0/docs/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     6786 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/Makefile
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    17990 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/Ne4.svg
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       30 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/changelog.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2499 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/conf.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     5814 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/core.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    11087 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/engine.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      806 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/gaviota.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      282 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/index.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     6713 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/make.bat
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     3812 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/pgn.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      940 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/polyglot.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      593 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/svg.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      379 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/syzygy.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2691 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/variant.rst
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      537 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/docs/wR.svg
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.336570 python-chess-bughouse-0.28.0/examples/
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.336570 python-chess-bughouse-0.28.0/examples/bratko_kopec/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1866 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/bratko_kopec/bratko-kopec.epd
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     4886 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/bratko_kopec/bratko_kopec.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     2967 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/bratko_kopec/giveaway-puzzles.epd
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)      589 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/chess960_pos_list.py
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.339903 python-chess-bughouse-0.28.0/examples/perft/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      772 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/atomic.perft
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      333 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/crazyhouse.perft
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      428 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/giveaway.perft
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      139 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/horde.perft
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     4020 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/perft.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      113 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/racingkings.perft
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)  1054418 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/random.perft
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     1410 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/perft/tricky.perft
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     1091 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/polyglot_tree.py
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     2011 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/push_san.py
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     2213 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/examples/xray_attacks.py
+drwxr-xr-x   0 bouanto   (1000) bouanto   (1000)        0 2023-05-08 23:08:57.339903 python-chess-bughouse-0.28.0/python_chess_bughouse.egg-info/
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)    11656 2023-05-08 23:08:57.000000 python-chess-bughouse-0.28.0/python_chess_bughouse.egg-info/PKG-INFO
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)     4364 2023-05-08 23:08:57.000000 python-chess-bughouse-0.28.0/python_chess_bughouse.egg-info/SOURCES.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)        1 2023-05-08 23:08:57.000000 python-chess-bughouse-0.28.0/python_chess_bughouse.egg-info/dependency_links.txt
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)        6 2023-05-08 23:08:57.000000 python-chess-bughouse-0.28.0/python_chess_bughouse.egg-info/top_level.txt
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     3706 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/release.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)       38 2023-05-08 23:08:57.339903 python-chess-bughouse-0.28.0/setup.cfg
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)     3789 2023-05-02 00:14:16.000000 python-chess-bughouse-0.28.0/setup.py
+-rwxr-xr-x   0 bouanto   (1000) bouanto   (1000)   162165 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/test.py
+-rw-r--r--   0 bouanto   (1000) bouanto   (1000)      472 2023-04-29 22:06:45.000000 python-chess-bughouse-0.28.0/tox.ini
```

### Comparing `python-chess-bughouse-0.27.3/CHANGELOG.rst` & `python-chess-bughouse-0.28.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/LICENSE.txt` & `python-chess-bughouse-0.28.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/PKG-INFO` & `python-chess-bughouse-0.28.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-chess-bughouse
-Version: 0.27.3
+Version: 0.28.0
 Summary: A pure Python chess library with move generation and validation, Polyglot opening book probing, PGN reading and writing, Gaviota tablebase probing, Syzygy tablebase probing and XBoard/UCI engine communication.
 Home-page: https://github.com/niklasf/python-chess
 Author: Niklas Fiekas
 Author-email: niklas.fiekas@backscattering.de
 License: GPL-3.0+
 Keywords: chess fen epd pgn polyglot syzygy gaviota uci xboard bughouse
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,28 +23,28 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 python-chess: a pure Python chess library
 =========================================
 
-.. image:: https://travis-ci.org/niklasf/python-chess.svg?branch=v0.27.3
+.. image:: https://travis-ci.org/niklasf/python-chess.svg?branch=v0.28.0
     :target: https://travis-ci.org/niklasf/python-chess
 
-.. image:: https://ci.appveyor.com/api/projects/status/y9k3hdbm0f0nbum9/branch/v0.27.3?svg=true
+.. image:: https://ci.appveyor.com/api/projects/status/y9k3hdbm0f0nbum9/branch/v0.28.0?svg=true
     :target: https://ci.appveyor.com/project/niklasf/python-chess
 
 .. image:: https://coveralls.io/repos/github/niklasf/python-chess/badge.svg?branch=master
    :target: https://coveralls.io/github/niklasf/python-chess?branch=master
 
 .. image:: https://badge.fury.io/py/python-chess.svg
     :target: https://pypi.python.org/pypi/python-chess
 
-.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v0.27.3
-    :target: https://python-chess.readthedocs.io/en/v0.27.3/
+.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v0.28.0
+    :target: https://python-chess.readthedocs.io/en/v0.28.0/
 
 Introduction
 ------------
 
 python-chess is a pure Python chess library with move generation, move
 validation and support for common formats. This is the Scholar's mate in
 python-chess:
@@ -77,43 +77,43 @@
 
     >>> board.is_checkmate()
     True
 
     >>> board
     Board('r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR b KQkq - 0 4')
 
-`Documentation <https://python-chess.readthedocs.io/en/v0.27.3/>`__
+`Documentation <https://python-chess.readthedocs.io/en/v0.28.0/>`__
 --------------------------------------------------------------------
 
-* `Core <https://python-chess.readthedocs.io/en/v0.27.3/core.html>`_
-* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v0.27.3/pgn.html>`_
-* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v0.27.3/polyglot.html>`_
-* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.27.3/gaviota.html>`_
-* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.27.3/syzygy.html>`_
-* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v0.27.3/engine.html>`_
-* `Variants <https://python-chess.readthedocs.io/en/v0.27.3/variant.html>`_
-* `Changelog <https://python-chess.readthedocs.io/en/v0.27.3/changelog.html>`_
+* `Core <https://python-chess.readthedocs.io/en/v0.28.0/core.html>`_
+* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v0.28.0/pgn.html>`_
+* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v0.28.0/polyglot.html>`_
+* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.28.0/gaviota.html>`_
+* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.28.0/syzygy.html>`_
+* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v0.28.0/engine.html>`_
+* `Variants <https://python-chess.readthedocs.io/en/v0.28.0/variant.html>`_
+* `Changelog <https://python-chess.readthedocs.io/en/v0.28.0/changelog.html>`_
 
 Features
 --------
 
 * Supports Python 3.5+ and PyPy3.
 
 * IPython/Jupyter Notebook integration.
-  `SVG rendering docs <https://python-chess.readthedocs.io/en/v0.27.3/svg.html>`_.
+  `SVG rendering docs <https://python-chess.readthedocs.io/en/v0.28.0/svg.html>`_.
 
   .. code:: python
 
       >>> board
 
   .. image:: https://backscattering.de/web-boardimage/board.png?fen=r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR&lastmove=h5f7&check=e8
 
 * Chess variants: Standard, Chess960, Suicide, Giveaway, Atomic,
   King of the Hill, Racing Kings, Horde, Three-check, Crazyhouse.
-  `Variant docs <https://python-chess.readthedocs.io/en/v0.27.3/variant.html>`_.
+  `Variant docs <https://python-chess.readthedocs.io/en/v0.28.0/variant.html>`_.
 
 * Make and unmake moves.
 
   .. code:: python
 
       >>> Nf3 = chess.Move.from_uci("g1f3")
       >>> board.push(Nf3)  # Make the move
@@ -227,18 +227,18 @@
       >>> board.epd(bm=board.parse_uci("d2d4"))
       'rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - bm d4;'
 
       >>> ops = board.set_epd("1k1r4/pp1b1R2/3q2pp/4p3/2B5/4Q3/PPP2B2/2K5 b - - bm Qd1+; id \"BK.01\";")
       >>> ops == {'bm': [chess.Move.from_uci('d6d1')], 'id': 'BK.01'}
       True
 
-* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v0.27.3/core.html#chess.Board.pin>`_.
+* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v0.28.0/core.html#chess.Board.pin>`_.
 
 * Reads Polyglot opening books.
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/polyglot.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/polyglot.html>`__.
 
   .. code:: python
 
       >>> import chess.polyglot
 
       >>> book = chess.polyglot.open_reader("data/polyglot/performance.bin")
 
@@ -249,15 +249,15 @@
       >>> main_entry.weight
       1
 
       >>> book.close()
 
 * Reads and writes PGNs. Supports headers, comments, NAGs and a tree of
   variations.
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/pgn.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/pgn.html>`__.
 
   .. code:: python
 
       >>> import chess.pgn
 
       >>> with open("data/pgn/molinari-bordais-1979.pgn") as pgn:
       ...     first_game = chess.pgn.read_game(pgn)
@@ -270,18 +270,18 @@
       >>> first_game.mainline()
       <Mainline at ... (1. e4 c5 2. c4 Nc6 3. Ne2 Nf6 4. Nbc3 Nb4 5. g3 Nd3#)>
 
       >>> first_game.headers["Result"]
       '0-1'
 
 * Probe Gaviota endgame tablebases (DTM, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/gaviota.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/gaviota.html>`__.
 
 * Probe Syzygy endgame tablebases (DTZ, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/syzygy.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/syzygy.html>`__.
 
   .. code:: python
 
       >>> import chess.syzygy
 
       >>> tablebase = chess.syzygy.open_tablebase("data/syzygy/regular")
 
@@ -290,15 +290,15 @@
       >>> board = chess.Board("8/2K5/4B3/3N4/8/8/4k3/8 b - - 0 1")
       >>> tablebase.probe_dtz(board)
       -53
 
       >>> tablebase.close()
 
 * Communicate with UCI/XBoard engines. Based on ``asyncio``.
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/engine.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/engine.html>`__.
 
   .. code:: python
 
       >>> import chess.engine
 
       >>> engine = chess.engine.SimpleEngine.popen_uci("stockfish")
       >>> engine.id.get("name")
```

### Comparing `python-chess-bughouse-0.27.3/README.rst` & `python-chess-bughouse-0.28.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/__init__.py` & `python-chess-bughouse-0.28.0/chess/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 """
 from typing import Counter
 
 __author__ = "Niklas Fiekas"
 
 __email__ = "niklas.fiekas@backscattering.de"
 
-__version__ = "0.27.3"
+__version__ = "0.28.0"
 
 import collections
 import copy
 import enum
 import re
 import itertools
 import typing
@@ -2548,15 +2548,18 @@
         self.push(move)
         is_check = self.is_check()
         is_checkmate = (is_check and self.is_checkmate()) or self.is_variant_loss() or self.is_variant_win()
         self.pop()
 
         # Drops.
         if move.drop:
-            san = "@" + SQUARE_NAMES[move.to_square]
+            san = ""
+            if move.drop != PAWN:
+                san = piece_symbol(move.drop).upper()
+            san += "@" + SQUARE_NAMES[move.to_square]
 
         # Castling.
         if self.is_castling(move):
             if square_file(move.to_square) < square_file(move.from_square):
                 san = "O-O-O"
             else:
                 san = "O-O"
```

### Comparing `python-chess-bughouse-0.27.3/chess/engine.py` & `python-chess-bughouse-0.28.0/chess/engine.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/gaviota.py` & `python-chess-bughouse-0.28.0/chess/gaviota.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/pgn.py` & `python-chess-bughouse-0.28.0/chess/pgn.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/polyglot.py` & `python-chess-bughouse-0.28.0/chess/polyglot.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/svg.py` & `python-chess-bughouse-0.28.0/chess/svg.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/syzygy.py` & `python-chess-bughouse-0.28.0/chess/syzygy.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/chess/variant.py` & `python-chess-bughouse-0.28.0/chess/variant.py`

 * *Files identical despite different names*

### Comparing `python-chess-bughouse-0.27.3/python_chess_bughouse.egg-info/PKG-INFO` & `python-chess-bughouse-0.28.0/python_chess_bughouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-chess-bughouse
-Version: 0.27.3
+Version: 0.28.0
 Summary: A pure Python chess library with move generation and validation, Polyglot opening book probing, PGN reading and writing, Gaviota tablebase probing, Syzygy tablebase probing and XBoard/UCI engine communication.
 Home-page: https://github.com/niklasf/python-chess
 Author: Niklas Fiekas
 Author-email: niklas.fiekas@backscattering.de
 License: GPL-3.0+
 Keywords: chess fen epd pgn polyglot syzygy gaviota uci xboard bughouse
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,28 +23,28 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 python-chess: a pure Python chess library
 =========================================
 
-.. image:: https://travis-ci.org/niklasf/python-chess.svg?branch=v0.27.3
+.. image:: https://travis-ci.org/niklasf/python-chess.svg?branch=v0.28.0
     :target: https://travis-ci.org/niklasf/python-chess
 
-.. image:: https://ci.appveyor.com/api/projects/status/y9k3hdbm0f0nbum9/branch/v0.27.3?svg=true
+.. image:: https://ci.appveyor.com/api/projects/status/y9k3hdbm0f0nbum9/branch/v0.28.0?svg=true
     :target: https://ci.appveyor.com/project/niklasf/python-chess
 
 .. image:: https://coveralls.io/repos/github/niklasf/python-chess/badge.svg?branch=master
    :target: https://coveralls.io/github/niklasf/python-chess?branch=master
 
 .. image:: https://badge.fury.io/py/python-chess.svg
     :target: https://pypi.python.org/pypi/python-chess
 
-.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v0.27.3
-    :target: https://python-chess.readthedocs.io/en/v0.27.3/
+.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v0.28.0
+    :target: https://python-chess.readthedocs.io/en/v0.28.0/
 
 Introduction
 ------------
 
 python-chess is a pure Python chess library with move generation, move
 validation and support for common formats. This is the Scholar's mate in
 python-chess:
@@ -77,43 +77,43 @@
 
     >>> board.is_checkmate()
     True
 
     >>> board
     Board('r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR b KQkq - 0 4')
 
-`Documentation <https://python-chess.readthedocs.io/en/v0.27.3/>`__
+`Documentation <https://python-chess.readthedocs.io/en/v0.28.0/>`__
 --------------------------------------------------------------------
 
-* `Core <https://python-chess.readthedocs.io/en/v0.27.3/core.html>`_
-* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v0.27.3/pgn.html>`_
-* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v0.27.3/polyglot.html>`_
-* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.27.3/gaviota.html>`_
-* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.27.3/syzygy.html>`_
-* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v0.27.3/engine.html>`_
-* `Variants <https://python-chess.readthedocs.io/en/v0.27.3/variant.html>`_
-* `Changelog <https://python-chess.readthedocs.io/en/v0.27.3/changelog.html>`_
+* `Core <https://python-chess.readthedocs.io/en/v0.28.0/core.html>`_
+* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v0.28.0/pgn.html>`_
+* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v0.28.0/polyglot.html>`_
+* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.28.0/gaviota.html>`_
+* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v0.28.0/syzygy.html>`_
+* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v0.28.0/engine.html>`_
+* `Variants <https://python-chess.readthedocs.io/en/v0.28.0/variant.html>`_
+* `Changelog <https://python-chess.readthedocs.io/en/v0.28.0/changelog.html>`_
 
 Features
 --------
 
 * Supports Python 3.5+ and PyPy3.
 
 * IPython/Jupyter Notebook integration.
-  `SVG rendering docs <https://python-chess.readthedocs.io/en/v0.27.3/svg.html>`_.
+  `SVG rendering docs <https://python-chess.readthedocs.io/en/v0.28.0/svg.html>`_.
 
   .. code:: python
 
       >>> board
 
   .. image:: https://backscattering.de/web-boardimage/board.png?fen=r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR&lastmove=h5f7&check=e8
 
 * Chess variants: Standard, Chess960, Suicide, Giveaway, Atomic,
   King of the Hill, Racing Kings, Horde, Three-check, Crazyhouse.
-  `Variant docs <https://python-chess.readthedocs.io/en/v0.27.3/variant.html>`_.
+  `Variant docs <https://python-chess.readthedocs.io/en/v0.28.0/variant.html>`_.
 
 * Make and unmake moves.
 
   .. code:: python
 
       >>> Nf3 = chess.Move.from_uci("g1f3")
       >>> board.push(Nf3)  # Make the move
@@ -227,18 +227,18 @@
       >>> board.epd(bm=board.parse_uci("d2d4"))
       'rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - bm d4;'
 
       >>> ops = board.set_epd("1k1r4/pp1b1R2/3q2pp/4p3/2B5/4Q3/PPP2B2/2K5 b - - bm Qd1+; id \"BK.01\";")
       >>> ops == {'bm': [chess.Move.from_uci('d6d1')], 'id': 'BK.01'}
       True
 
-* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v0.27.3/core.html#chess.Board.pin>`_.
+* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v0.28.0/core.html#chess.Board.pin>`_.
 
 * Reads Polyglot opening books.
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/polyglot.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/polyglot.html>`__.
 
   .. code:: python
 
       >>> import chess.polyglot
 
       >>> book = chess.polyglot.open_reader("data/polyglot/performance.bin")
 
@@ -249,15 +249,15 @@
       >>> main_entry.weight
       1
 
       >>> book.close()
 
 * Reads and writes PGNs. Supports headers, comments, NAGs and a tree of
   variations.
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/pgn.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/pgn.html>`__.
 
   .. code:: python
 
       >>> import chess.pgn
 
       >>> with open("data/pgn/molinari-bordais-1979.pgn") as pgn:
       ...     first_game = chess.pgn.read_game(pgn)
@@ -270,18 +270,18 @@
       >>> first_game.mainline()
       <Mainline at ... (1. e4 c5 2. c4 Nc6 3. Ne2 Nf6 4. Nbc3 Nb4 5. g3 Nd3#)>
 
       >>> first_game.headers["Result"]
       '0-1'
 
 * Probe Gaviota endgame tablebases (DTM, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/gaviota.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/gaviota.html>`__.
 
 * Probe Syzygy endgame tablebases (DTZ, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/syzygy.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/syzygy.html>`__.
 
   .. code:: python
 
       >>> import chess.syzygy
 
       >>> tablebase = chess.syzygy.open_tablebase("data/syzygy/regular")
 
@@ -290,15 +290,15 @@
       >>> board = chess.Board("8/2K5/4B3/3N4/8/8/4k3/8 b - - 0 1")
       >>> tablebase.probe_dtz(board)
       -53
 
       >>> tablebase.close()
 
 * Communicate with UCI/XBoard engines. Based on ``asyncio``.
-  `Docs <https://python-chess.readthedocs.io/en/v0.27.3/engine.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v0.28.0/engine.html>`__.
 
   .. code:: python
 
       >>> import chess.engine
 
       >>> engine = chess.engine.SimpleEngine.popen_uci("stockfish")
       >>> engine.id.get("name")
```

### Comparing `python-chess-bughouse-0.27.3/setup.py` & `python-chess-bughouse-0.28.0/setup.py`

 * *Files identical despite different names*

