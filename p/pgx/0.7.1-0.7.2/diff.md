# Comparing `tmp/pgx-0.7.1.tar.gz` & `tmp/pgx-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.7.1.tar", last modified: Fri Apr 28 07:30:18 2023, max compression
+gzip compressed data, was "pgx-0.7.2.tar", last modified: Tue May  9 16:54:35 2023, max compression
```

## Comparing `pgx-0.7.1.tar` & `pgx-0.7.2.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.966359 pgx-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 07:30:07.000000 pgx-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-04-28 07:30:18.966359 pgx-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-04-28 07:30:07.000000 pgx-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.946360 pgx-0.7.1/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.950360 pgx-0.7.1/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.950360 pgx-0.7.1/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.954360 pgx-0.7.1/pgx/_src/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/assets/between.npy
--rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/assets/can_move.npy
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.954360 pgx-0.7.1/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.954360 pgx-0.7.1/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.958360 pgx-0.7.1/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.958360 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    37353 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.962360 pgx-0.7.1/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.962360 pgx-0.7.1/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-28 07:30:07.000000 pgx-0.7.1/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.950360 pgx-0.7.1/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-04-28 07:30:18.000000 pgx-0.7.1/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-28 07:30:18.000000 pgx-0.7.1/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:30:18.000000 pgx-0.7.1/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 07:30:18.000000 pgx-0.7.1/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 07:30:18.000000 pgx-0.7.1/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 07:30:07.000000 pgx-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:30:18.966359 pgx-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 07:30:07.000000 pgx-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:18.966359 pgx-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61927 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29776 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-28 07:30:07.000000 pgx-0.7.1/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.517311 pgx-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 16:54:26.000000 pgx-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-09 16:54:35.517311 pgx-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-05-09 16:54:26.000000 pgx-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.501311 pgx-0.7.2/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.501311 pgx-0.7.2/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.501311 pgx-0.7.2/pgx/_mahjong/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_mahjong/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.501311 pgx-0.7.2/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.505311 pgx-0.7.2/pgx/_src/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/assets/between.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/assets/can_move.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.509311 pgx-0.7.2/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.509311 pgx-0.7.2/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.509311 pgx-0.7.2/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.513311 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37353 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.513311 pgx-0.7.2/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.513311 pgx-0.7.2/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-09 16:54:26.000000 pgx-0.7.2/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-09 16:54:27.000000 pgx-0.7.2/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.501311 pgx-0.7.2/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-09 16:54:35.000000 pgx-0.7.2/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-09 16:54:35.000000 pgx-0.7.2/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:54:35.000000 pgx-0.7.2/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 16:54:35.000000 pgx-0.7.2/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 16:54:35.000000 pgx-0.7.2/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-09 16:54:27.000000 pgx-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:54:35.517311 pgx-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-09 16:54:27.000000 pgx-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:35.517311 pgx-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61927 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29776 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-09 16:54:27.000000 pgx-0.7.2/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.7.1/LICENSE` & `pgx-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/PKG-INFO` & `pgx-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.7.1
+Version: 0.7.2
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -63,15 +63,15 @@
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
 while not (state.terminated | state.terminated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
-> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in April 2023. Opinions and comments are more than welcome!
+> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in May 2023. Opinions and comments are more than welcome!
 
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.7.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.7.2 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -31,15 +31,15 @@
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
 # vectorized states while not (state.terminated | state.terminated).all():
 action = model(state.current_player, state.observation,
 state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
 â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
-change without notice. We aim to release v1.0.0 in April 2023. Opinions and
+change without notice. We aim to release v1.0.0 in May 2023. Opinions and
 comments are more than welcome!  ## Supported games | Backgammon | Chess |
 Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
 sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
 raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
 sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
 raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
```

### Comparing `pgx-0.7.1/README.md` & `pgx-0.7.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
 while not (state.terminated | state.terminated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
-> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in April 2023. Opinions and comments are more than welcome!
+> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in May 2023. Opinions and comments are more than welcome!
 
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
 # vectorized states while not (state.terminated | state.terminated).all():
 action = model(state.current_player, state.observation,
 state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
 â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
-change without notice. We aim to release v1.0.0 in April 2023. Opinions and
+change without notice. We aim to release v1.0.0 in May 2023. Opinions and
 comments are more than welcome!  ## Supported games | Backgammon | Chess |
 Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
 sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
 raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
 sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
 raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
```

### Comparing `pgx-0.7.1/pgx/_mahjong/_hand.py` & `pgx-0.7.2/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_mahjong/_meld.py` & `pgx-0.7.2/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_mahjong/_shanten.py` & `pgx-0.7.2/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_mahjong/_yaku.py` & `pgx-0.7.2/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/api_test.py` & `pgx-0.7.2/pgx/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/assets/between.npy` & `pgx-0.7.2/pgx/_src/assets/between.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/assets/can_move.npy` & `pgx-0.7.2/pgx/_src/assets/can_move.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/chess_utils.py` & `pgx-0.7.2/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/animalshogi.py` & `pgx-0.7.2/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/backgammon.py` & `pgx-0.7.2/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.7.2/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/chess.py` & `pgx-0.7.2/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/connect_four.py` & `pgx-0.7.2/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/go.py` & `pgx-0.7.2/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/hex.py` & `pgx-0.7.2/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.7.2/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.7.2/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.7.2/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.7.2/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.7.2/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/othello.py` & `pgx-0.7.2/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/play2048.py` & `pgx-0.7.2/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/shogi.py` & `pgx-0.7.2/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.7.2/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/dwg/tictactoe.py` & `pgx-0.7.2/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/shogi_utils.py` & `pgx-0.7.2/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/struct.py` & `pgx-0.7.2/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/_src/visualizer.py` & `pgx-0.7.2/pgx/_src/visualizer.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/animal_shogi.py` & `pgx-0.7.2/pgx/animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/backgammon.py` & `pgx-0.7.2/pgx/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/bridge_bidding.py` & `pgx-0.7.2/pgx/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/chess.py` & `pgx-0.7.2/pgx/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/connect_four.py` & `pgx-0.7.2/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/experimental/bridge_bidding.py` & `pgx-0.7.2/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/experimental/gym.py` & `pgx-0.7.2/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/experimental/pettingzoo.py` & `pgx-0.7.2/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/experimental/visualize.py` & `pgx-0.7.2/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/go.py` & `pgx-0.7.2/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/hex.py` & `pgx-0.7.2/pgx/hex.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     # 11x11 board
     # [[  0,  1,  2,  ...,  8,  9, 10],
     #  [ 11,  12, 13, ..., 19, 20, 21],
     #  .
     #  .
     #  .
     #  [110, 111, 112, ...,  119, 120]]
-    _board: jnp.ndarray = -jnp.zeros(
+    _board: jnp.ndarray = jnp.zeros(
         11 * 11, jnp.int32
     )  # <0(oppo), 0(empty), 0<(self)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "hex"
 
@@ -121,24 +121,27 @@
         legal_action_mask=legal_action_mask,
     )
 
     return state
 
 
 def _observe(state: State, player_id: jnp.ndarray, size) -> jnp.ndarray:
-    board = jax.lax.cond(
+    board = jax.lax.select(
         player_id == state.current_player,
-        lambda: state._board.reshape((size, size)),
-        lambda: (state._board * -1).reshape((size, size)),
+        state._board.reshape((size, size)),
+        -state._board.reshape((size, size)),
     )
 
-    def make(color):
-        return board * color > 0
+    my_board = board * 1 > 0
+    opp_board = board * -1 > 0
+    my_color = jax.lax.select(
+        player_id == state.current_player, state._turn, 1 - state._turn
+    ) * jnp.ones_like(my_board)
 
-    return jnp.stack(jax.vmap(make)(jnp.int8([1, -1])), 2)
+    return jnp.stack([my_board, opp_board, my_color], 2, dtype=jnp.bool_)
 
 
 def _neighbour(xy, size):
     """
         (x,y-1)   (x+1,y-1)
     (x-1,y)    (x,y)    (x+1,y)
        (x-1,y+1)   (x,y+1)
```

### Comparing `pgx-0.7.1/pgx/kuhn_poker.py` & `pgx-0.7.2/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/leduc_holdem.py` & `pgx-0.7.2/pgx/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/minatar/asterix.py` & `pgx-0.7.2/pgx/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/minatar/breakout.py` & `pgx-0.7.2/pgx/minatar/breakout.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
-        return "minatar-asterix"
+        return "minatar-breakout"
 
     @property
     def version(self) -> str:
         return "beta"
 
     @property
     def num_players(self):
```

### Comparing `pgx-0.7.1/pgx/minatar/freeway.py` & `pgx-0.7.2/pgx/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/minatar/seaquest.py` & `pgx-0.7.2/pgx/minatar/seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/minatar/space_invaders.py` & `pgx-0.7.2/pgx/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/minatar/utils.py` & `pgx-0.7.2/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/othello.py` & `pgx-0.7.2/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/play2048.py` & `pgx-0.7.2/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/shogi.py` & `pgx-0.7.2/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/sparrow_mahjong.py` & `pgx-0.7.2/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/tic_tac_toe.py` & `pgx-0.7.2/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx/v1.py` & `pgx-0.7.2/pgx/v1.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/pgx.egg-info/PKG-INFO` & `pgx-0.7.2/pgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.7.1
+Version: 0.7.2
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -63,15 +63,15 @@
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
 while not (state.terminated | state.terminated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
-> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in April 2023. Opinions and comments are more than welcome!
+> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in May 2023. Opinions and comments are more than welcome!
 
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.7.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.7.2 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -31,15 +31,15 @@
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
 # vectorized states while not (state.terminated | state.terminated).all():
 action = model(state.current_player, state.observation,
 state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
 â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
-change without notice. We aim to release v1.0.0 in April 2023. Opinions and
+change without notice. We aim to release v1.0.0 in May 2023. Opinions and
 comments are more than welcome!  ## Supported games | Backgammon | Chess |
 Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
 sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
 raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
 sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
 raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
```

### Comparing `pgx-0.7.1/pgx.egg-info/SOURCES.txt` & `pgx-0.7.2/pgx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pgx.egg-info/top_level.txt
 pgx/_mahjong/__init__.py
 pgx/_mahjong/_action.py
 pgx/_mahjong/_hand.py
 pgx/_mahjong/_meld.py
 pgx/_mahjong/_shanten.py
 pgx/_mahjong/_yaku.py
+pgx/_mahjong/cache/__init__.py
 pgx/_src/__init__.py
 pgx/_src/api_test.py
 pgx/_src/chess_utils.py
 pgx/_src/shogi_utils.py
 pgx/_src/struct.py
 pgx/_src/visualizer.py
 pgx/_src/assets/between.npy
```

### Comparing `pgx-0.7.1/setup.py` & `pgx-0.7.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.7.1",
+    version="0.7.2",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
-    package_data={"": ["LICENSE", "*.svg", "_src/assets/*.npy"]},
+    package_data={
+        "": ["LICENSE", "*.svg", "_src/assets/*.npy", "_mahjong/*.json"]
+    },
     include_package_data=True,
     install_requires=[
         "jax>=0.3.25",  # JAX version on Colab (TPU)
         "svgwrite",
-        "typing_extensions"
+        "typing_extensions",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `pgx-0.7.1/tests/minatar_utils.py` & `pgx-0.7.2/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_animal_shogi.py` & `pgx-0.7.2/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_asterix.py` & `pgx-0.7.2/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_backgammon.py` & `pgx-0.7.2/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_breakout.py` & `pgx-0.7.2/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_bridge_bidding.py` & `pgx-0.7.2/tests/test_bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_chess.py` & `pgx-0.7.2/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_connect_four.py` & `pgx-0.7.2/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_freeway.py` & `pgx-0.7.2/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_go.py` & `pgx-0.7.2/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_hex.py` & `pgx-0.7.2/tests/test_hex.py`

 * *Files 15% similar despite different names*

```diff
@@ -93,23 +93,25 @@
     @ O . . .
      . . . . .
       . . . . .
     """
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     assert state.current_player == 0
-    assert (jnp.zeros((11, 11, 2)) == observe(state, 0)).all()
+    assert (jnp.zeros((11, 11, 3)) == observe(state, 0)).all()
     state = step(state, 0)
+    assert (observe(state, 0)[:, :, 2] == 0).all()
+    assert (observe(state, 1)[:, :, 2] == 1).all()
     state = step(state, 1)
     assert (
-        jnp.zeros((11, 11, 2)).at[0, 0, 0].set(1).at[0, 1, 1].set(1)
+        jnp.zeros((11, 11, 3), dtype=jnp.bool_).at[0, 0, 0].set(True).at[0, 1, 1].set(True)
         == observe(state, 0)
     ).all()
     assert (
-        jnp.zeros((11, 11, 2)).at[0, 1, 0].set(1).at[0, 0, 1].set(1)
+            jnp.zeros((11, 11, 3), dtype=jnp.bool_).at[0, 1, 0].set(True).at[0, 0, 1].set(True).at[:, :, 2].set(True)
         == observe(state, 1)
     ).all()
 
 
 def test_random_play():
     key = jax.random.PRNGKey(0)
     done = jnp.bool_(False)
```

### Comparing `pgx-0.7.1/tests/test_kuhn_poker.py` & `pgx-0.7.2/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_leduc_holdem.py` & `pgx-0.7.2/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_mahjong.py` & `pgx-0.7.2/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_othello.py` & `pgx-0.7.2/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_play2048.py` & `pgx-0.7.2/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_seaquest.py` & `pgx-0.7.2/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_shogi.py` & `pgx-0.7.2/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_space_invaders.py` & `pgx-0.7.2/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_sparrow_mahjong.py` & `pgx-0.7.2/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.1/tests/test_tic_tac_toe.py` & `pgx-0.7.2/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

