# Comparing `tmp/pgx-0.5.1.tar.gz` & `tmp/pgx-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.5.1.tar", last modified: Sun Apr 23 03:41:09 2023, max compression
+gzip compressed data, was "pgx-0.5.2.tar", last modified: Tue Apr 25 11:29:39 2023, max compression
```

## Comparing `pgx-0.5.1.tar` & `pgx-0.5.2.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.852263 pgx-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 03:41:00.000000 pgx-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-23 03:41:09.852263 pgx-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-23 03:41:00.000000 pgx-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_mahjong/_hand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.844263 pgx-0.5.1/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.848263 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    27792 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    44159 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28910 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.848263 pgx-0.5.1/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.848263 pgx-0.5.1/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25891 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-23 03:41:00.000000 pgx-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:41:09.852263 pgx-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-23 03:41:00.000000 pgx-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.852263 pgx-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61403 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.533492 pgx-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 11:29:27.000000 pgx-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-25 11:29:39.533492 pgx-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-25 11:29:27.000000 pgx-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.493492 pgx-0.5.2/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.497492 pgx-0.5.2/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.501492 pgx-0.5.2/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.509492 pgx-0.5.2/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.513492 pgx-0.5.2/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.521492 pgx-0.5.2/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.525492 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.525492 pgx-0.5.2/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-25 11:29:27.000000 pgx-0.5.2/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.529492 pgx-0.5.2/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25972 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-04-25 11:29:28.000000 pgx-0.5.2/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.493492 pgx-0.5.2/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 11:29:39.000000 pgx-0.5.2/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-25 11:29:28.000000 pgx-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:29:39.533492 pgx-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-25 11:29:28.000000 pgx-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:39.533492 pgx-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61896 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39645 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-25 11:29:28.000000 pgx-0.5.2/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.5.1/LICENSE` & `pgx-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/PKG-INFO` & `pgx-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.1
+Version: 0.5.2
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.5.2 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.1/README.md` & `pgx-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_mahjong/_hand.py` & `pgx-0.5.2/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/api_test.py` & `pgx-0.5.2/pgx/_src/api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -145,14 +145,28 @@
     assert state.current_player.dtype == jnp.int8, state.current_player.dtype
     assert state.terminated.dtype == jnp.bool_, state.terminated.dtype
     assert state.reward.dtype == jnp.float32, state.reward.dtype
     assert (
         state.legal_action_mask.dtype == jnp.bool_
     ), state.legal_action_mask.dtype
 
+    # check public attributes
+    public_attributes = [
+        "current_player",
+        "observation",
+        "reward",
+        "terminated",
+        "truncated",
+        "legal_action_mask",
+    ]
+    for k, v in state.__dict__.items():
+        if k.startswith("_"):  # internal
+            continue
+        assert k in public_attributes
+
 
 def _validate_legal_actions(state: State):
     if state.terminated:
         # Agent can take any action at terminal state (but give no effect to the next state)
         # This is to avoid zero-division error by normalizing action probability by legal actions
         assert (
             state.legal_action_mask == jnp.ones_like(state.legal_action_mask)
```

### Comparing `pgx-0.5.1/pgx/_src/chess_utils.py` & `pgx-0.5.2/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/animalshogi.py` & `pgx-0.5.2/pgx/_src/dwg/animalshogi.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,18 @@
     #  4: GOLD
     #  5: OPP_PAWN
     #  6: OPP_ROOK
     #  7: OPP_BISHOP
     #  8: OPP_KING
     #  9: OPP_GOLD
 
-    if state.turn == 0:
-        board = state.board
+    if state._turn == 0:
+        board = state._board
     else:
-        board = state.board[::-1]
+        board = state._board[::-1]
     for xy in range(12):
         piece_type = "EMPTY"
         n = board[xy]
         if n in (0, 5):
             piece_type = "P"
         if n in (1, 6):
             piece_type = "B"
@@ -105,15 +105,15 @@
             piece_type = "K"
         if n in (4, 9):
             piece_type = "G"
 
         if piece_type == "EMPTY":
             continue
 
-        if state.turn == 0:
+        if state._turn == 0:
             is_black = 0 <= n < 5
         else:
             is_black = 5 <= n
 
         if is_black:
             pieces_g = p1_pieces_g
             x = 2 - xy // BOARD_HEIGHT  # AnimalShogiStateは右上原点
@@ -167,17 +167,17 @@
                     stroke=stroke,
                     fill=stroke,
                 )
             )
 
     # # hand
     for i, piece_num, piece_type in zip(
-        range(6), state.hand.flatten(), ["P", "R", "B", "P", "R", "B"]
+        range(6), state._hand.flatten(), ["P", "R", "B", "P", "R", "B"]
     ):
-        is_black = i < 3 if state.turn == 0 else 3 <= i  # type: ignore
+        is_black = i < 3 if state._turn == 0 else 3 <= i  # type: ignore
         _g = p1_pieces_g if is_black else p2_pieces_g
         _g.add(
             dwg.text(
                 text=f"{piece_type}:{piece_num}",
                 insert=(
                     3.1 * GRID_SIZE,
                     (3.3 + (i % 3) * 0.3) * GRID_SIZE,
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/backgammon.py` & `pgx-0.5.2/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.5.2/pgx/_src/dwg/bridge_bidding.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
     # hand
     x_offset = [235, 480, 235, -10]
     y_offset = [10, 190, 370, 190]
     area_width = 230
     area_height = 150
     for i in range(4):  # N, E, S, W
-        hand = sorted(state.hand[i * NUM_CARD_TYPE : (i + 1) * NUM_CARD_TYPE])
+        hand = sorted(state._hand[i * NUM_CARD_TYPE : (i + 1) * NUM_CARD_TYPE])
         assert len(hand) == NUM_CARD_TYPE
         # player
         pos = np.array(["North", "East", "South", "West"], dtype=object)
-        pos[state.dealer] = pos[state.dealer] + "(Dealer)"
+        pos[state._dealer] = pos[state._dealer] + "(Dealer)"
         newline_offset = 0
         over_offset = 0
 
         for j in range(4):  # spades,hearts,diamonds,clubs
             # h line
             board_g.add(
                 dwg.line(
@@ -171,15 +171,15 @@
                 font_size="20px",
                 font_family="Courier",
                 font_weight="bold",
             )
         )
 
         # vul
-        if (state.vul_NS and i % 2 == 0) or (state.vul_EW and i % 2 == 1):
+        if (state._vul_NS and i % 2 == 0) or (state._vul_EW and i % 2 == 1):
             board_g.add(
                 dwg.text(
                     text="Vul.",
                     insert=(
                         x_offset[i] + area_width + over_offset - 50,
                         y_offset[i],
                     ),
@@ -202,15 +202,15 @@
             rx="5px",
             ry="5px",
             fill="none",
             stroke=color_set.grid_color,
             stroke_width="5px",
         )
     )
-    for i, act in enumerate(state.bidding_history):
+    for i, act in enumerate(state._bidding_history):
         if act == -1:
             break
         act_str = (
             str(act // 5 + 1) + DENOMINATIONS[(act % 5)]
             if 0 <= act < 35
             else ACT[act - 35]
         )
@@ -234,15 +234,15 @@
             end=(_x + _w, _y + 30),
             stroke=color_set.grid_color,
             stroke_width="2px",
         )
     )
     # player
     pos = np.array(["N", "E", "S", "W"], dtype=object)
-    pos = np.roll(pos, -state.dealer)
+    pos = np.roll(pos, -state._dealer)
     pos[0] = pos[0] + "(D)"
     for i in range(4):
         board_g.add(
             dwg.text(
                 text=pos[i],
                 insert=(_x + 15 + 50 * (i % 4), _y + 20),
                 fill=color_set.text_color,
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/chess.py` & `pgx-0.5.2/pgx/_src/dwg/chess.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,20 +127,20 @@
                     (8.35) * GRID_SIZE,
                 ),
                 font_size="20px",
                 font_family="Serif",
             )
         )
 
-    if state.turn == 1:
+    if state._turn == 1:
         state = _flip(state)
     # pieces
     pieces_g = dwg.g()
     for i in range(64):
-        pi = int(state.board[i].item())
+        pi = int(state._board[i].item())
         if pi == 0:
             continue
         if pi < 0:
             pi *= -1
             pi += 6
         piece_type = PIECES[pi]
         xy = i
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/connect_four.py` & `pgx-0.5.2/pgx/_src/dwg/connect_four.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             ),
             fill=color_set.grid_color,
             stroke=color_set.grid_color,
         )
     )
 
     # stones
-    board = state.board
+    board = state._board
     for xy, stone in enumerate(board):
         if stone == -1:
             continue
         # ndarrayのx,yと違うことに注意
         # svgではヨコがx
         stone_y = xy // BOARD_HEIGHT * GRID_SIZE + GRID_SIZE / 2
         stone_x = xy % BOARD_WIDTH * GRID_SIZE + GRID_SIZE / 2
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/go.py` & `pgx-0.5.2/pgx/_src/dwg/go.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 r=GRID_SIZE / 10,
                 fill=color_set.grid_color,
             )
         )
     board_g.add(hoshi_g)
 
     # stones
-    board = jnp.clip(state.chain_id_board, -1, 1)
+    board = jnp.clip(state._chain_id_board, -1, 1)
     for xy, stone in enumerate(board):
         if stone == 0:
             continue
         # ndarrayのx,yと違うことに注意
         stone_y = xy // BOARD_SIZE * GRID_SIZE
         stone_x = xy % BOARD_SIZE * GRID_SIZE
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/hex.py` & `pgx-0.5.2/pgx/_src/dwg/hex.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pgx.hex import _get_abs_board
 
 r3 = jnp.sqrt(3)
 
 
 def _make_hex_dwg(dwg, state: HexState, config):
     GRID_SIZE = config["GRID_SIZE"] / 2  # 六角形の1辺
-    BOARD_SIZE = int(state.size)
+    BOARD_SIZE = int(state._size)
     color_set = config["COLOR_SET"]
 
     # background
     dwg.add(
         dwg.rect(
             (0, 0),
             (BOARD_SIZE * GRID_SIZE, BOARD_SIZE * GRID_SIZE),
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.5.2/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.5.2/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.5.2/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.5.2/pgx/_src/dwg/leduc_holdem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pgx.kuhn_poker import State as KuhnPokerState
+from pgx.leduc_holdem import State as LeducHoldemState
 
 CARD = ["J", "Q", "K"]
 
 
-def _make_kuhnpoker_dwg(dwg, state: KuhnPokerState, config):
+def _make_leducHoldem_dwg(dwg, state: LeducHoldemState, config):
     GRID_SIZE = config["GRID_SIZE"]
     BOARD_SIZE = config["BOARD_WIDTH"]
     color_set = config["COLOR_SET"]
 
     # background
     dwg.add(
         dwg.rect(
@@ -16,85 +16,116 @@
             fill=color_set.background_color,
         )
     )
 
     # board
     # grid
     board_g = dwg.g()
-    board_g.add(
-        dwg.line(
-            start=(2 * GRID_SIZE, 8 * GRID_SIZE),
-            end=(6 * GRID_SIZE, 0),
-            stroke=color_set.grid_color,
-            stroke_width="2px",
-        )
-    )
 
     # card
     board_g.add(
         dwg.rect(
-            (0, 0),
+            (0, 4 * GRID_SIZE),
             (2 * GRID_SIZE, 3 * GRID_SIZE),
             fill=color_set.background_color,
             stroke=color_set.grid_color,
             stroke_width="2px",
             rx="5px",
             ry="5px",
         )
     )
     board_g.add(
         dwg.text(
-            text=CARD[state.cards[0]],
-            insert=(GRID_SIZE, GRID_SIZE),
+            text=CARD[state._cards[0]],
+            insert=(GRID_SIZE, 5 * GRID_SIZE),
             fill=color_set.text_color,
             font_size="40px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
     # chip
     board_g.add(
         dwg.text(
-            text=f"chip {state.pot[0]}",
-            insert=(0, 3.6 * GRID_SIZE),
+            text=f"chip +{state._chips[0]}",
+            insert=(0, 7.6 * GRID_SIZE),
             fill=color_set.text_color,
             font_size="18px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
 
     # card
     board_g.add(
         dwg.rect(
-            (6 * GRID_SIZE, 5 * GRID_SIZE),
+            (6 * GRID_SIZE, 4 * GRID_SIZE),
             (2 * GRID_SIZE, 3 * GRID_SIZE),
             fill=color_set.background_color,
             stroke=color_set.grid_color,
             stroke_width="2px",
             rx="5px",
             ry="5px",
         )
     )
     board_g.add(
         dwg.text(
-            text=CARD[state.cards[1]],
-            insert=(7 * GRID_SIZE, 6 * GRID_SIZE),
+            text=CARD[state._cards[1]],
+            insert=(7 * GRID_SIZE, 5 * GRID_SIZE),
             fill=color_set.text_color,
             font_size="40px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
     # chip
+    chip = f"chip +{state._chips[1]}"
     board_g.add(
         dwg.text(
-            text=f"chip {state.pot[1]}",
-            insert=(6 * GRID_SIZE, 4.6 * GRID_SIZE),
+            text=chip,
+            insert=(
+                8 * GRID_SIZE - 10 * len(chip),
+                7.6 * GRID_SIZE,
+            ),
             fill=color_set.text_color,
             font_size="18px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
 
+    # public
+    board_g.add(
+        dwg.line(
+            start=(0, 3.5 * GRID_SIZE),
+            end=(8 * GRID_SIZE, 3.5 * GRID_SIZE),
+            stroke=color_set.grid_color,
+            stroke_width="2px",
+        )
+    )
+    board_g.add(
+        dwg.rect(
+            (3 * GRID_SIZE, 0),
+            (2 * GRID_SIZE, 3 * GRID_SIZE),
+            fill=color_set.background_color,
+            stroke=color_set.p1_color
+            if state._round == 0
+            else color_set.p2_color,
+            stroke_width="2px",
+            rx="5px",
+            ry="5px",
+        )
+    )
+    board_g.add(
+        dwg.text(
+            text=CARD[state._cards[2]],
+            insert=(4 * GRID_SIZE, GRID_SIZE),
+            fill=color_set.p1_color
+            if state._round == 0
+            else color_set.p2_color,
+            font_size="40px",
+            font_family="Courier",
+            # font_weight="bold",
+        )
+    )
+
     return board_g
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.5.2/pgx/_src/dwg/kuhn_poker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pgx.leduc_holdem import State as LeducHoldemState
+from pgx.kuhn_poker import State as KuhnPokerState
 
 CARD = ["J", "Q", "K"]
 
 
-def _make_leducHoldem_dwg(dwg, state: LeducHoldemState, config):
+def _make_kuhnpoker_dwg(dwg, state: KuhnPokerState, config):
     GRID_SIZE = config["GRID_SIZE"]
     BOARD_SIZE = config["BOARD_WIDTH"]
     color_set = config["COLOR_SET"]
 
     # background
     dwg.add(
         dwg.rect(
@@ -16,116 +16,85 @@
             fill=color_set.background_color,
         )
     )
 
     # board
     # grid
     board_g = dwg.g()
+    board_g.add(
+        dwg.line(
+            start=(2 * GRID_SIZE, 8 * GRID_SIZE),
+            end=(6 * GRID_SIZE, 0),
+            stroke=color_set.grid_color,
+            stroke_width="2px",
+        )
+    )
 
     # card
     board_g.add(
         dwg.rect(
-            (0, 4 * GRID_SIZE),
+            (0, 0),
             (2 * GRID_SIZE, 3 * GRID_SIZE),
             fill=color_set.background_color,
             stroke=color_set.grid_color,
             stroke_width="2px",
             rx="5px",
             ry="5px",
         )
     )
     board_g.add(
         dwg.text(
-            text=CARD[state.cards[0]],
-            insert=(GRID_SIZE, 5 * GRID_SIZE),
+            text=CARD[state._cards[0]],
+            insert=(GRID_SIZE, GRID_SIZE),
             fill=color_set.text_color,
             font_size="40px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
     # chip
     board_g.add(
         dwg.text(
-            text=f"chip +{state.chips[0]}",
-            insert=(0, 7.6 * GRID_SIZE),
+            text=f"chip {state._pot[0]}",
+            insert=(0, 3.6 * GRID_SIZE),
             fill=color_set.text_color,
             font_size="18px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
 
     # card
     board_g.add(
         dwg.rect(
-            (6 * GRID_SIZE, 4 * GRID_SIZE),
+            (6 * GRID_SIZE, 5 * GRID_SIZE),
             (2 * GRID_SIZE, 3 * GRID_SIZE),
             fill=color_set.background_color,
             stroke=color_set.grid_color,
             stroke_width="2px",
             rx="5px",
             ry="5px",
         )
     )
     board_g.add(
         dwg.text(
-            text=CARD[state.cards[1]],
-            insert=(7 * GRID_SIZE, 5 * GRID_SIZE),
+            text=CARD[state._cards[1]],
+            insert=(7 * GRID_SIZE, 6 * GRID_SIZE),
             fill=color_set.text_color,
             font_size="40px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
     # chip
-    chip = f"chip +{state.chips[1]}"
     board_g.add(
         dwg.text(
-            text=chip,
-            insert=(
-                8 * GRID_SIZE - 10 * len(chip),
-                7.6 * GRID_SIZE,
-            ),
+            text=f"chip {state._pot[1]}",
+            insert=(6 * GRID_SIZE, 4.6 * GRID_SIZE),
             fill=color_set.text_color,
             font_size="18px",
             font_family="Courier",
             # font_weight="bold",
         )
     )
 
-    # public
-    board_g.add(
-        dwg.line(
-            start=(0, 3.5 * GRID_SIZE),
-            end=(8 * GRID_SIZE, 3.5 * GRID_SIZE),
-            stroke=color_set.grid_color,
-            stroke_width="2px",
-        )
-    )
-    board_g.add(
-        dwg.rect(
-            (3 * GRID_SIZE, 0),
-            (2 * GRID_SIZE, 3 * GRID_SIZE),
-            fill=color_set.background_color,
-            stroke=color_set.p1_color
-            if state.round == 0
-            else color_set.p2_color,
-            stroke_width="2px",
-            rx="5px",
-            ry="5px",
-        )
-    )
-    board_g.add(
-        dwg.text(
-            text=CARD[state.cards[2]],
-            insert=(4 * GRID_SIZE, GRID_SIZE),
-            fill=color_set.p1_color
-            if state.round == 0
-            else color_set.p2_color,
-            font_size="40px",
-            font_family="Courier",
-            # font_weight="bold",
-        )
-    )
-
     return board_g
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/othello.py` & `pgx-0.5.2/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/dwg/play2048.py` & `pgx-0.5.2/pgx/_src/dwg/play2048.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             fill=color_set.background_color,
         )
     )
 
     # board
     # grid
     board_g = dwg.g()
-    for i, _exp2 in enumerate(state.board):
+    for i, _exp2 in enumerate(state._board):
         exp2 = int(_exp2)
         num = 2**exp2
         if exp2 > 11:
             exp2 = 11
         x = (i % 4) * GRID_SIZE
         y = (i // 4) * GRID_SIZE
         _color = (
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/shogi.py` & `pgx-0.5.2/pgx/_src/dwg/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 
 from pgx.shogi import State as ShogiState
 
 
 def _make_shogi_dwg(dwg, state: ShogiState, config):  # noqa: C901
-    if state.turn == 1:
+    if state._turn == 1:
         from pgx.shogi import _flip
 
         state = _flip(state)
     # fmt: off
     PIECES = ["歩", "香", "桂", "銀", "角", "飛", "金", "玉", "と", "成香", "成桂", "成銀", "馬", "龍"] * 2
     NUM_TO_CHAR = ["一", "二", "三", "四", "五", "六", "七", "八", "九", "十"]
     # fmt: on
 
     def _sort_pieces(state, p1_hand, p2_hand):
         """
         ShogiStateのhandを飛、角、金、銀、桂、香、歩の順にする
         """
-        hands = state.hand.flatten()[::-1]
+        hands = state._hand.flatten()[::-1]
         tmp = hands
         hands = hands.at[0].set(tmp[1])
         hands = hands.at[1].set(tmp[2])
         hands = hands.at[2].set(tmp[0])
         hands = hands.at[7].set(tmp[8])
         hands = hands.at[8].set(tmp[9])
         hands = hands.at[9].set(tmp[7])
@@ -125,15 +125,15 @@
             )
         )
 
     # pieces
     p1_pieces_g = dwg.g()
     p2_pieces_g = dwg.g()
     one_hot_board = np.zeros((29, 81))
-    board = state.piece_board
+    board = state._board
     for i in range(81):
         piece = board[i]
         one_hot_board[piece, i] = 1
     for i, piece_pos, piece_type in zip(
         range(28),
         one_hot_board,
         PIECES,
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.5.2/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,17 @@
     # grid
     board_g = dwg.g()
     p1_g = dwg.g()
     p2_g = dwg.g()
     p3_g = dwg.g()
 
     # pieces
-    for player_id, pieces_g in zip(state.shuffled_players, [p1_g, p2_g, p3_g]):
+    for player_id, pieces_g in zip(
+        state._shuffled_players, [p1_g, p2_g, p3_g]
+    ):
         pieces_g = dwg.g()
 
         # border
         pieces_g.add(
             dwg.rect(
                 (245, 360),
                 (
@@ -103,17 +105,17 @@
         )
 
         # hands
         x = 250
         y = 370
         for type, num in zip(
             range(NUM_TILE_TYPES),
-            state.hands[player_id],
+            state._hands[player_id],
         ):
-            num_red = state.n_red_in_hands[player_id, type]
+            num_red = state._n_red_in_hands[player_id, type]
             for _ in range(num):
                 pieces_g = _set_piece(
                     x,
                     y,
                     type,
                     num_red > 0,
                     dwg,
@@ -124,15 +126,15 @@
                 num_red -= 1
 
         # river
         x = 270
         y = 220
         river_count = 0
         for type, is_red in zip(
-            state.rivers[player_id], state.is_red_in_river[player_id]
+            state._rivers[player_id], state._is_red_in_river[player_id]
         ):
             if type >= 0:
                 pieces_g = _set_piece(
                     x,
                     y,
                     type,
                     is_red,
@@ -143,20 +145,20 @@
                 x += 40
                 river_count += 1
                 if river_count > 4:
                     river_count = 0
                     x = 270
                     y += 60
 
-        if player_id == state.shuffled_players[1]:
+        if player_id == state._shuffled_players[1]:
             pieces_g.rotate(
                 angle=90, center=(BOARD_WIDTH * GRID_SIZE / 2, 100)
             )
 
-        elif player_id == state.shuffled_players[2]:
+        elif player_id == state._shuffled_players[2]:
             pieces_g.rotate(
                 angle=-90, center=(BOARD_WIDTH * GRID_SIZE / 2, 100)
             )
 
         board_g.add(pieces_g)
 
     # dora
@@ -185,27 +187,27 @@
             stroke=color_set.p2_outline,
             stroke_width="3px",
         )
     )
     board_g = _set_piece(
         BOARD_WIDTH * GRID_SIZE / 2 - 25,
         15,
-        state.dora,
+        state._dora,
         False,
         dwg,
         board_g,
         GRID_SIZE,
     )
 
     # wall
     wall_type = -1
     board_g = _set_piece(330, 120, wall_type, False, dwg, board_g, GRID_SIZE)
     board_g.add(
         dwg.text(
-            text=f"× {NUM_TILES - state.draw_ix-1}",
+            text=f"× {NUM_TILES - state._draw_ix - 1}",
             insert=(380, 150),
             fill=color_set.text_color,
             font_size="20px",
             font_family="serif",
         )
     )
     board_g.translate(0, 40)
```

### Comparing `pgx-0.5.1/pgx/_src/dwg/tictactoe.py` & `pgx-0.5.2/pgx/_src/dwg/tictactoe.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                     GRID_SIZE * x,
                     GRID_SIZE * BOARD_HEIGHT,
                 ),
                 r=GRID_SIZE * 0.014,
             )
         )
 
-    for i, mark in enumerate(state.board):
+    for i, mark in enumerate(state._board):
         x = i % BOARD_WIDTH
         y = i // BOARD_HEIGHT
         if mark == 0:  # 先手
             board_g.add(
                 dwg.line(
                     start=(
                         (x + 0.1) * GRID_SIZE,
```

### Comparing `pgx-0.5.1/pgx/_src/shogi_utils.py` & `pgx-0.5.2/pgx/_src/shogi_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     - 盤面の記入が終わったら手番（b/w）
     - 持ち駒は先手の物から順番はRBGSNLPの順
     - 最後に手数（1で固定）
 
     """
     # NOTE: input must be flipped if white turn
 
-    pb = jnp.rot90(state.piece_board.reshape((9, 9)), k=3)
+    pb = jnp.rot90(state._board.reshape((9, 9)), k=3)
     sfen = ""
     # fmt: off
     board_char_dir = ["", "P", "L", "N", "S", "B", "R", "G", "K", "+P", "+L", "+N", "+S", "+B", "+R", "p", "l", "n", "s", "b", "r", "g", "k", "+p", "+l", "+n", "+s", "+b", "+r"]
     hand_char_dir = ["P", "L", "N", "S", "B", "R", "G", "p", "l", "n", "s", "b", "r", "g"]
     hand_dir = [5, 4, 6, 3, 2, 1, 0, 12, 11, 13, 10, 9, 8, 7]
     # fmt: on
     # 盤面
@@ -203,26 +203,26 @@
         if space_length != 0:
             sfen += str(space_length)
         if i != 8:
             sfen += "/"
         else:
             sfen += " "
     # 手番
-    if state.turn == 0:
+    if state._turn == 0:
         sfen += "b "
     else:
         sfen += "w "
     # 持ち駒
-    if jnp.all(state.hand == 0):
+    if jnp.all(state._hand == 0):
         sfen += "-"
     else:
         for i in range(2):
             for j in range(7):
                 piece_type = hand_dir[i * 7 + j]
-                num_piece = state.hand.flatten()[piece_type]
+                num_piece = state._hand.flatten()[piece_type]
                 if num_piece == 0:
                     continue
                 if num_piece >= 2:
                     sfen += str(num_piece)
                 sfen += hand_char_dir[piece_type]
     sfen += f" {state._step_count + 1}"
     return sfen
```

### Comparing `pgx-0.5.1/pgx/_src/struct.py` & `pgx-0.5.2/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/_src/visualizer.py` & `pgx-0.5.2/pgx/_src/visualizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 import math
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Literal, Optional, Sequence, Union
 
+import jax
 import svgwrite  # type: ignore
 
 from pgx.v1 import State
 
 ColorTheme = Literal["light", "dark"]
 
 
@@ -336,21 +337,23 @@
                     "gray",
                 )
         elif _state.env_id in ("go-9x9", "go-19x19"):
             from pgx._src.dwg.go import _make_go_dwg
 
             self.config["GRID_SIZE"] = 25
             try:
-                self.config["BOARD_WIDTH"] = int(_state.size[0])  # type:ignore
+                self.config["BOARD_WIDTH"] = int(
+                    _state._size[0]  # type:ignore
+                )
                 self.config["BOARD_HEIGHT"] = int(
-                    _state.size[0]  # type:ignore
+                    _state._size[0]  # type:ignore
                 )
             except IndexError:
-                self.config["BOARD_WIDTH"] = int(_state.size)  # type:ignore
-                self.config["BOARD_HEIGHT"] = int(_state.size)  # type:ignore
+                self.config["BOARD_WIDTH"] = int(_state._size)  # type:ignore
+                self.config["BOARD_HEIGHT"] = int(_state._size)  # type:ignore
             self._make_dwg_group = _make_go_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
@@ -375,25 +378,25 @@
             import jax.numpy as jnp
 
             from pgx._src.dwg.hex import _make_hex_dwg, four_dig
 
             self.config["GRID_SIZE"] = 30
             try:
                 self.config["BOARD_WIDTH"] = four_dig(
-                    _state.size[0] * 1.5  # type:ignore
+                    _state._size[0] * 1.5  # type:ignore
                 )
                 self.config["BOARD_HEIGHT"] = four_dig(
-                    _state.size[0] * jnp.sqrt(3) / 2  # type:ignore
+                    _state._size[0] * jnp.sqrt(3) / 2  # type:ignore
                 )
             except IndexError:
                 self.config["BOARD_WIDTH"] = four_dig(
-                    _state.size * 1.5  # type:ignore
+                    _state._size * 1.5  # type:ignore
                 )
                 self.config["BOARD_HEIGHT"] = four_dig(
-                    _state.size * jnp.sqrt(3) / 2  # type:ignore
+                    _state._size * jnp.sqrt(3) / 2  # type:ignore
                 )
             self._make_dwg_group = _make_hex_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
@@ -611,135 +614,16 @@
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "white", "black", "lightgray", "white", "white", "black"
                 )
         else:
             assert False
 
-    # TODO: simplify me
-    def _get_nth_state(self, _states: State, _i):
-        if _states.env_id == "animal_shogi":
-            from pgx._src.dwg.animalshogi import AnimalShogiState
-
-            return AnimalShogiState(
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-                hand=_states.hand[_i],  # type:ignore
-            )
-        elif _states.env_id == "backgammon":
-            from pgx._src.dwg.backgammon import BackgammonState
-
-            return BackgammonState(
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-            )
-        elif _states.env_id == "connect_four":
-            from pgx._src.dwg.connect_four import ConnectFourState
-
-            return ConnectFourState(  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-            )
-        elif _states.env_id == "chess":
-            from pgx._src.dwg.chess import ChessState
-
-            return ChessState(
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-            )
-        elif _states.env_id == "bridge_bidding":
-            from pgx._src.dwg.bridge_bidding import BridgeBiddingState
-
-            return BridgeBiddingState(  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-                dealer=_states.dealer[_i],  # type:ignore
-                current_player=_states.current_player[_i],  # type:ignore
-                hand=_states.hand[_i],  # type:ignore
-                bidding_history=_states.bidding_history[_i],  # type:ignore
-                vul_NS=_states.vul_NS[_i],  # type:ignore
-                vul_EW=_states.vul_EW[_i],  # type:ignore
-            )
-        elif _states.env_id in ("go-9x9", "go-19x19"):
-            from pgx._src.dwg.go import GoState
-
-            return GoState(  # type:ignore
-                size=_states.size[_i],  # type:ignore
-                chain_id_board=_states.chain_id_board[_i],  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-            )
-        elif _states.env_id == "hex":
-            from pgx._src.dwg.hex import HexState
-
-            return HexState(
-                size=_states.size[_i],  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-            )
-        elif _states.env_id == "kuhn_poker":
-            from pgx._src.dwg.kuhn_poker import KuhnPokerState
-
-            return KuhnPokerState(
-                cards=_states.cards[_i], pot=_states.pot[_i]  # type:ignore
-            )
-        elif _states.env_id == "leduc_holdem":
-            from pgx._src.dwg.leduc_holdem import LeducHoldemState
-
-            return LeducHoldemState(
-                cards=_states.cards[_i],  # type:ignore
-                chips=_states.chips[_i],  # type:ignore
-                round=_states.round[_i],  # type:ignore
-            )
-        elif _states.env_id == "othello":
-            from pgx._src.dwg.othello import OthelloState
-
-            return OthelloState(
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-            )
-        elif _states.env_id == "2048":
-            from pgx._src.dwg.play2048 import Play2048State
-
-            return Play2048State(
-                board=_states.board[_i],  # type:ignore
-            )
-        elif _states.env_id == "shogi":
-            from pgx._src.dwg.shogi import ShogiState
-
-            return ShogiState(  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-                piece_board=_states.piece_board[_i],  # type:ignore
-                hand=_states.hand[_i],  # type:ignore
-            )
-        elif _states.env_id == "sparrow_mahjong":
-            from pgx._src.dwg.sparrow_mahjong import SparrowMahjongState
-
-            return SparrowMahjongState(
-                current_player=_states.current_player[_i],  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-                rivers=_states.rivers[_i],  # type:ignore
-                hands=_states.hands[_i],  # type:ignore
-                n_red_in_hands=_states.n_red_in_hands[_i],  # type:ignore
-                is_red_in_river=_states.is_red_in_river[_i],  # type:ignore
-                wall=_states.wall[_i],  # type:ignore
-                draw_ix=_states.draw_ix[_i],  # type:ignore
-                shuffled_players=_states.shuffled_players[_i],  # type:ignore
-                dora=_states.dora[_i],  # type:ignore
-            )
-        elif _states.env_id == "tic_tac_toe":
-            from pgx._src.dwg.tictactoe import TictactoeState
-
-            return TictactoeState(
-                current_player=_states.current_player[_i],  # type:ignore
-                legal_action_mask=_states.legal_action_mask[_i],  # type:ignore
-                terminated=_states.terminated[_i],  # type:ignore
-                turn=_states.turn[_i],  # type:ignore
-                board=_states.board[_i],  # type:ignore
-            )
-        else:
-            assert False
+    def _get_nth_state(self, states: State, i):
+        return jax.tree_util.tree_map(lambda x: x[i], states)
 
 
 def save_svg(
     states: State,
     filename: Union[str, Path],
     *,
     color_theme: Optional[Literal["light", "dark"]] = None,
```

### Comparing `pgx-0.5.1/pgx/animal_shogi.py` & `pgx-0.5.2/pgx/animal_shogi.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(132, dtype=jnp.bool_)  # (132,)
     observation: jnp.ndarray = jnp.zeros((4, 3, 22), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Animal Shogi specific ---
-    turn: jnp.ndarray = jnp.int8(0)
-    board: jnp.ndarray = INIT_BOARD  # (12,)
-    hand: jnp.ndarray = jnp.zeros((2, 3), dtype=jnp.int8)
+    _turn: jnp.ndarray = jnp.int8(0)
+    _board: jnp.ndarray = INIT_BOARD  # (12,)
+    _hand: jnp.ndarray = jnp.zeros((2, 3), dtype=jnp.int8)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "animal_shogi"
 
 
 @dataclass
@@ -120,15 +120,15 @@
         return 2
 
 
 def _step(state: State, action: jnp.ndarray):
     a = Action._from_label(action)
     # apply move/drop action
     state = jax.lax.cond(a.is_drop, _step_drop, _step_move, *(state, a))
-    is_try = (state.board[jnp.int8([0, 4, 8])] == KING).any()
+    is_try = (state._board[jnp.int8([0, 4, 8])] == KING).any()
 
     state = _flip(state)
 
     legal_action_mask = _legal_action_mask(state)  # TODO: fix me
     terminated = ~legal_action_mask.any() | is_try
     # fmt: off
     reward = jax.lax.select(
@@ -148,18 +148,18 @@
     state, flip_state = jax.lax.cond(
         state.current_player == player_id,
         lambda: (state, _flip(state)),
         lambda: (_flip(state), state),
     )
 
     def is_piece(p, state):
-        return state.board == p
+        return state._board == p
 
     def num_hand(p, n, state):
-        return state.hand.flatten()[p] >= n
+        return state._hand.flatten()[p] >= n
 
     # fmt: off
     piece_feat = jax.vmap(partial(is_piece, state=state))(jnp.arange(10))  # (10, 12)
     hand_feat = jax.vmap(jax.vmap(
         partial(num_hand, state=state), (None, 0)), (0, None)
     )(jnp.arange(6), jnp.arange(1, 3)).flatten().reshape(12, 1)  # (12, 1)
     hand_feat = jnp.tile(hand_feat, reps=(1, 12))  # (12, 12)
@@ -167,96 +167,96 @@
 
     obs = jnp.vstack((piece_feat, hand_feat))
     obs = obs.reshape(-1, 3, 4).transpose((2, 1, 0))
     return jnp.flip(obs, axis=1)
 
 
 def _step_move(state: State, action: Action) -> State:
-    piece = state.board[action.from_]
+    piece = state._board[action.from_]
     # remove piece from the original position
-    board = state.board.at[action.from_].set(EMPTY)
+    board = state._board.at[action.from_].set(EMPTY)
     # capture the opponent if exists
     captured = board[action.to]  # suppose >= OPP_PAWN, -1 if EMPTY
     hand = jax.lax.cond(
         captured == EMPTY,
-        lambda: state.hand,
+        lambda: state._hand,
         # add captured piece to my hand after
         #   (1) tuning opp piece into mine by % 5, and
         #   (2) filtering promoted piece by x % 4
-        lambda: state.hand.at[0, (captured % 5) % 4].add(1),
+        lambda: state._hand.at[0, (captured % 5) % 4].add(1),
     )
     # promote piece (PAWN to GOLD)
     is_promotion = (action.from_ % 4 == 1) & (piece == PAWN)
     piece = jax.lax.select(is_promotion, GOLD, piece)
     # set piece to the target position
     board = board.at[action.to].set(piece)
     # apply piece moves
-    return state.replace(board=board, hand=hand)  # type: ignore
+    return state.replace(_board=board, _hand=hand)  # type: ignore
 
 
 def _step_drop(state: State, action: Action) -> State:
     # add piece to board
-    board = state.board.at[action.to].set(action.drop_piece)
+    board = state._board.at[action.to].set(action.drop_piece)
     # remove piece from hand
-    hand = state.hand.at[0, action.drop_piece].add(-1)
-    return state.replace(board=board, hand=hand)  # type: ignore
+    hand = state._hand.at[0, action.drop_piece].add(-1)
+    return state.replace(_board=board, _hand=hand)  # type: ignore
 
 
 def _legal_action_mask(state: State):
     def is_legal(label: jnp.ndarray):
         action = Action._from_label(label)
         return jax.lax.cond(
             action.is_drop, is_legal_drop, is_legal_move, action
         )
 
     def is_legal_move(action: Action):
-        piece = state.board[action.from_]
+        piece = state._board[action.from_]
         ok = (PAWN <= piece) & (piece <= GOLD)
         ok &= action.to != -1
-        ok &= (state.board[action.to] == EMPTY) | (
-            GOLD < state.board[action.to]
+        ok &= (state._board[action.to] == EMPTY) | (
+            GOLD < state._board[action.to]
         )
         ok &= _can_move(piece, action.from_, action.to)
         ok &= ~_is_checked(_step_move(state, action))
         return ok
 
     def is_legal_drop(action: Action):
-        ok = state.board[action.to] == EMPTY
-        ok &= state.hand[0, action.drop_piece] > 0
+        ok = state._board[action.to] == EMPTY
+        ok &= state._hand[0, action.drop_piece] > 0
         ok &= (action.drop_piece != PAWN) | (action.to % 4 != 0)
         ok &= ~_is_checked(_step_drop(state, action))
         return ok
 
     return jax.vmap(is_legal)(jnp.arange(132))
 
 
 def _is_checked(state):
-    king_pos = jnp.argmin(jnp.abs(state.board - KING))
+    king_pos = jnp.argmin(jnp.abs(state._board - KING))
 
     @jax.vmap
     def can_capture_king(from_):
-        piece = state.board[from_]
+        piece = state._board[from_]
         is_opp = piece >= 5
-        return is_opp & _can_move(state.board[from_] % 5, king_pos, from_)
+        return is_opp & _can_move(state._board[from_] % 5, king_pos, from_)
 
     return can_capture_king(
         jnp.arange(12)
     ).any()  # TODO: King neighbours are enough
 
 
 def _flip(state):
-    empty_mask = state.board == EMPTY
-    board = (state.board + 5) % 10
+    empty_mask = state._board == EMPTY
+    board = (state._board + 5) % 10
     board = jnp.where(empty_mask, EMPTY, board)
     board = board[::-1]
     return state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
-        turn=(state.turn + 1) % 2,
-        board=board,
-        hand=state.hand[::-1],
+        _turn=(state._turn + 1) % 2,
+        _board=board,
+        _hand=state._hand[::-1],
     )
 
 
 def _can_move(piece, from_, to):
     def can_move(piece, from_, to):
         """Can <piece> move from <from_> to <to>?"""
         x0, y0 = from_ // 4, from_ % 4
```

### Comparing `pgx-0.5.1/pgx/backgammon.py` & `pgx-0.5.2/pgx/backgammon.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
     truncated: jnp.ndarray = FALSE
     # micro action = 6 * src + die
     legal_action_mask: jnp.ndarray = jnp.zeros(6 * 26 + 6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Backgammon specific ---
     # 各point(24) bar(2) off(2)にあるcheckerの数. 黒+, 白-
-    board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
+    _board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
     # サイコロを振るたびにrngをsplitして更新する.
-    rng: jax.random.KeyArray = jnp.zeros(2, dtype=jnp.uint16)
+    _rng: jax.random.KeyArray = jnp.zeros(2, dtype=jnp.uint16)
     # サイコロの出目 0~5: 1~6
-    dice: jnp.ndarray = jnp.zeros(2, dtype=jnp.int16)
+    _dice: jnp.ndarray = jnp.zeros(2, dtype=jnp.int16)
     # プレイできるサイコロの目
-    playable_dice: jnp.ndarray = jnp.zeros(4, dtype=jnp.int16)
+    _playable_dice: jnp.ndarray = jnp.zeros(4, dtype=jnp.int16)
     # プレイしたサイコロの目の数
-    played_dice_num: jnp.ndarray = jnp.int16(0)
+    _played_dice_num: jnp.ndarray = jnp.int16(0)
     # 黒0, 白1
-    turn: jnp.ndarray = jnp.int8(1)
+    _turn: jnp.ndarray = jnp.int8(1)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "backgammon"
 
 
 class Backgammon(v1.Env):
@@ -96,44 +96,46 @@
     dice: jnp.ndarray = _roll_init_dice(rng2)
     playable_dice: jnp.ndarray = _set_playable_dice(dice)
     played_dice_num: jnp.ndarray = jnp.int16(0)
     turn: jnp.ndarray = _init_turn(dice)
     legal_action_mask: jnp.ndarray = _legal_action_mask(board, playable_dice)
     state = State(  # type: ignore
         current_player=current_player,
-        rng=rng3,
-        board=board,
+        _rng=rng3,
+        _board=board,
         terminated=terminated,
-        dice=dice,
-        playable_dice=playable_dice,
-        played_dice_num=played_dice_num,
-        turn=turn,
+        _dice=dice,
+        _playable_dice=playable_dice,
+        _played_dice_num=played_dice_num,
+        _turn=turn,
         legal_action_mask=legal_action_mask,
     )
     return state
 
 
 def _step(state: State, action: jnp.ndarray) -> State:
     """
     terminated していない場合のstep 関数.
     """
     state = _update_by_action(state, action)
     return jax.lax.cond(
-        _is_all_off(state.board),
+        _is_all_off(state._board),
         lambda: _winning_step(state),
         lambda: _no_winning_step(state, action),
     )
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     """
     手番のplayerに対する観測を返す.
     """
-    board: jnp.ndarray = state.board
-    zero_one_dice_vec: jnp.ndarray = _to_zero_one_dice_vec(state.playable_dice)
+    board: jnp.ndarray = state._board
+    zero_one_dice_vec: jnp.ndarray = _to_zero_one_dice_vec(
+        state._playable_dice
+    )
     return jax.lax.cond(
         player_id == state.current_player,
         lambda: jnp.concatenate((board, zero_one_dice_vec), axis=None),  # type: ignore
         lambda: jnp.concatenate(
             (board, jnp.zeros(6, dtype=jnp.int8)), axis=None  # type: ignore
         ),
     )
@@ -162,15 +164,15 @@
 
 def _winning_step(
     state: State,
 ) -> State:
     """
     勝利者がいる場合のstep.
     """
-    win_score = _calc_win_score(state.board)
+    win_score = _calc_win_score(state._board)
     winner = state.current_player
     loser = 1 - winner
     reward = jnp.ones_like(state.reward)
     reward = reward.at[winner].set(win_score)
     reward = reward.at[loser].set(-win_score)
     state = state.replace(terminated=TRUE)  # type: ignore
     return state.replace(reward=reward)  # type: ignore
@@ -188,35 +190,35 @@
 
 
 def _update_by_action(state: State, action: jnp.ndarray) -> State:
     """
     行動を受け取って状態をupdate
     """
     is_no_op = action // 6 == 0
-    rng = state.rng
+    rng = state._rng
     current_player: jnp.ndarray = state.current_player
     terminated: jnp.ndarray = state.terminated
-    board: jnp.ndarray = _move(state.board, action)
-    played_dice_num: jnp.ndarray = jnp.int16(state.played_dice_num + 1)
+    board: jnp.ndarray = _move(state._board, action)
+    played_dice_num: jnp.ndarray = jnp.int16(state._played_dice_num + 1)
     playable_dice: jnp.ndarray = _update_playable_dice(
-        state.playable_dice, state.played_dice_num, state.dice, action
+        state._playable_dice, state._played_dice_num, state._dice, action
     )
     legal_action_mask: jnp.ndarray = _legal_action_mask(board, playable_dice)
     return jax.lax.cond(
         is_no_op,
         lambda: state,
         lambda: state.replace(  # type: ignore
             current_player=current_player,
-            rng=rng,
+            _rng=rng,
             terminated=terminated,
-            board=board,
-            turn=state.turn,
-            dice=state.dice,
-            playable_dice=playable_dice,
-            played_dice_num=played_dice_num,
+            _board=board,
+            _turn=state._turn,
+            _dice=state._dice,
+            _playable_dice=playable_dice,
+            _played_dice_num=played_dice_num,
             legal_action_mask=legal_action_mask,
         ),
     )  # no-opの時はupdateしない
 
 
 def _flip_board(board):
     """
@@ -237,39 +239,39 @@
     return board
 
 
 def _is_turn_end(state: State) -> bool:
     """
     play可能なサイコロ数が0の場合ないしlegal_actionがない場合交代
     """
-    return state.playable_dice.sum() == -4  # type: ignore
+    return state._playable_dice.sum() == -4  # type: ignore
 
 
 def _change_turn(state: State) -> State:
     """
     ターンを変更して新しい状態を返す.
     """
-    rng1, rng2 = jax.random.split(state.rng)
-    board: jnp.ndarray = _flip_board(state.board)  # boardを反転させて黒視点に変える
-    turn: jnp.ndarray = (state.turn + 1) % 2  # turnを変える
+    rng1, rng2 = jax.random.split(state._rng)
+    board: jnp.ndarray = _flip_board(state._board)  # boardを反転させて黒視点に変える
+    turn: jnp.ndarray = (state._turn + 1) % 2  # turnを変える
     current_player: jnp.ndarray = (state.current_player + 1) % 2
     terminated: jnp.ndarray = state.terminated
     dice: jnp.ndarray = _roll_dice(rng1)  # diceを振る
     playable_dice: jnp.ndarray = _set_playable_dice(dice)  # play可能なサイコロを初期化
     played_dice_num: jnp.ndarray = jnp.int16(0)
     legal_action_mask: jnp.ndarray = _legal_action_mask(board, dice)
     return state.replace(  # type: ignore
         current_player=current_player,
-        rng=rng2,
-        board=board,
+        _rng=rng2,
+        _board=board,
         terminated=terminated,
-        turn=turn,
-        dice=dice,
-        playable_dice=playable_dice,
-        played_dice_num=played_dice_num,
+        _turn=turn,
+        _dice=dice,
+        _playable_dice=playable_dice,
+        _played_dice_num=played_dice_num,
         legal_action_mask=legal_action_mask,
     )
 
 
 def _roll_init_dice(rng: jax.random.KeyArray) -> jnp.ndarray:
     """
     # 違う目が出るまで振り続ける.
@@ -568,10 +570,10 @@
 
 
 def _get_abs_board(state: State) -> jnp.ndarray:
     """
     visualization用
     黒ならそのまま, 白なら反転して返す.
     """
-    board: jnp.ndarray = state.board
-    turn: jnp.ndarray = state.turn
+    board: jnp.ndarray = state._board
+    turn: jnp.ndarray = state._turn
     return jax.lax.cond(turn == 0, lambda: board, lambda: _flip_board(board))
```

### Comparing `pgx-0.5.1/pgx/bridge_bidding.py` & `pgx-0.5.2/pgx/bridge_bidding.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
-from typing import Tuple
+import os
+import sys
+from typing import Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 import pgx.v1 as v1
 from pgx._src.struct import dataclass
@@ -29,80 +31,86 @@
 # 0~12 spade, 13~25 heart, 26~38 diamond, 39~51 club
 # それぞれのsuitにおいて以下の順で数字が並ぶ
 TO_CARD = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "T", "J", "Q", "K"]
 
 
 @dataclass
 class State(v1.State):
-    _step_count: jnp.ndarray = jnp.int32(0)
-    # turn 現在のターン数
-    turn: jnp.ndarray = jnp.int16(0)
-    # current_player 現在のプレイヤーid
     current_player: jnp.ndarray = jnp.int8(-1)
-    # 各プレイヤーの観測
     observation: jnp.ndarray = jnp.zeros(478, dtype=jnp.bool_)
-    # 報酬　player_id: 0, 1, 2, 3
     reward: jnp.ndarray = jnp.float32([0, 0, 0, 0])
-    # シャッフルされたプレイヤーの並び
-    shuffled_players: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
-    # 終端状態
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
+    legal_action_mask: jnp.ndarray = jnp.ones(38, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
+    _step_count: jnp.ndarray = jnp.int32(0)
+    # turn 現在のターン数
+    _turn: jnp.ndarray = jnp.int16(0)
+    # シャッフルされたプレイヤーの並び
+    _shuffled_players: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
     # hand 各プレイヤーの手札
     # index = 0 ~ 12がN, 13 ~ 25がE, 26 ~ 38がS, 39 ~ 51がWの持つ手札
     # 各要素にはカードを表す0 ~ 51の整数が格納される
-    hand: jnp.ndarray = jnp.zeros(52, dtype=jnp.int32)
+    _hand: jnp.ndarray = jnp.zeros(52, dtype=jnp.int32)
     # bidding_history 各プレイヤーのbidを時系列順に記憶
     # 最大の行動系列長 = 319
     # 各要素には、行動を表す整数が格納される
     # bidを表す0 ~ 34, passを表す35, doubleを表す36, redoubleを表す37, 行動が行われていない-1
     # 各ビッドがどのプレイヤーにより行われたかは、要素のindexから分かる（ix % 4）
-    bidding_history: jnp.ndarray = jnp.full(319, -1, dtype=jnp.int32)
+    _bidding_history: jnp.ndarray = jnp.full(319, -1, dtype=jnp.int32)
     # dealer どのプレイヤーがdealerかを表す
     # 0 = N, 1 = E, 2 = S, 3 = W
     # dealerは最初にbidを行うプレイヤー
-    dealer: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
+    _dealer: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
     # vul_NS NSチームがvulかどうかを表す
     # 0 = non vul, 1 = vul
-    vul_NS: jnp.ndarray = jnp.bool_(False)
+    _vul_NS: jnp.ndarray = jnp.bool_(False)
     # vul_EW EWチームがvulかどうかを表す
     # 0 = non vul, 1 = vul
-    vul_EW: jnp.ndarray = jnp.bool_(False)
+    _vul_EW: jnp.ndarray = jnp.bool_(False)
     # last_bid 最後にされたbid
     # last_bidder 最後にbidをしたプレイヤー
     # call_x 最後にされたbidがdoubleされているか
     # call_xx 最後にされたbidがredoubleされているか
-    last_bid: jnp.ndarray = jnp.int32(-1)
-    last_bidder: jnp.ndarray = jnp.int8(-1)
-    call_x: jnp.ndarray = jnp.bool_(False)
-    call_xx: jnp.ndarray = jnp.bool_(False)
-    # legal_actions プレイヤーの可能なbidの一覧
-    legal_action_mask: jnp.ndarray = jnp.ones(38, dtype=jnp.bool_)
+    _last_bid: jnp.ndarray = jnp.int32(-1)
+    _last_bidder: jnp.ndarray = jnp.int8(-1)
+    _call_x: jnp.ndarray = jnp.bool_(False)
+    _call_xx: jnp.ndarray = jnp.bool_(False)
     # first_denominaton_NS NSチームにおいて、各denominationをどのプレイヤー
     # が最初にbidしたかを表す
     # デノミネーションの順番は C, D, H, S, NT = 0, 1, 2, 3, 4
-    first_denomination_NS: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
+    _first_denomination_NS: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
     # first_denominaton_EW EWチームにおいて、各denominationをどのプレイヤー
     # が最初にbidしたかを表す
-    first_denomination_EW: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
+    _first_denomination_EW: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
     # passの回数
-    pass_num: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
+    _pass_num: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "bridge_bidding"
 
 
 class BridgeBidding(v1.Env):
-    def __init__(self):
+    def __init__(self, *, dds_hash_table_path: Optional[str] = None):
         super().__init__()
-        # fmt: off
-        self.hash_keys, self.hash_values = jnp.array([[19556549, 61212362, 52381660, 50424958], [53254536, 21854346, 37287883, 14009558], [44178585, 6709002, 23279217, 16304124], [36635659, 48114215, 13583653, 26208086], [44309474, 39388022, 28376136, 59735189], [61391908, 52173479, 29276467, 31670621], [34786519, 13802254, 57433417, 43152306], [48319039, 55845612, 44614774, 58169152], [47062227, 32289487, 12941848, 21338650], [36579116, 15643926, 64729756, 18678099], [62136384, 37064817, 59701038, 39188202], [13417016, 56577539, 25995845, 27248037], [61125047, 43238281, 23465183, 20030494], [7139188, 31324229, 58855042, 14296487], [2653767, 47502150, 35507905, 43823846], [31453323, 11605145, 6716808, 41061859], [21294711, 49709, 26110952, 50058629], [48130172, 3340423, 60445890, 7686579], [16041939, 27817393, 37167847, 9605779], [61154057, 17937858, 12254613, 12568801], [13796245, 46546127, 49123920, 51772041], [7195005, 45581051, 41076865, 17429796], [20635965, 14642724, 7001617, 45370595], [35616421, 19938131, 45131030, 16524847], [14559399, 15413729, 39188470, 535365], [48743216, 39672069, 60203571, 60210880], [63862780, 2462075, 23267370, 36595020], [11229980, 11616119, 20292263, 3695004], [24135854, 37532826, 54421444, 14130249], [42798085, 33026223, 2460251, 18566823], [49558558, 65537599, 14768519, 31103243], [44321156, 20075251, 42663767, 11615602], [20186726, 42678073, 11763300, 56739471], [57534601, 16703645, 6039937, 17088125], [50795278, 17350238, 11955835, 21538127], [45919621, 5520088, 27736513, 52674927], [13928720, 57324148, 28222453, 15480785], [910719, 47238830, 26345802, 56166394], [58841430, 1098476, 61890558, 26907706], [10379825, 8624220, 39701822, 29045990], [54444873, 50000486, 48563308, 55867521], [47291672, 22084522, 45484828, 32878832], [55350706, 23903891, 46142039, 11499952], [4708326, 27588734, 31010458, 11730972], [27078872, 59038086, 62842566, 51147874], [28922172, 32377861, 9109075, 10154350], [26104086, 62786977, 224865, 14335943], [20448626, 33187645, 34338784, 26382893], [29194006, 19635744, 24917755, 8532577], [64047742, 34885257, 5027048, 58399668], [27603972, 26820121, 44837703, 63748595], [60038456, 19611050, 7928914, 38555047], [13583610, 19626473, 22239272, 19888268], [28521006, 1743692, 31319264, 15168920], [64585849, 63931241, 57019799, 14189800], [2632453, 7269809, 60404342, 57986125], [1996183, 49918209, 49490468, 47760867], [6233580, 15318425, 51356120, 55074857], [15769884, 61654638, 8374039, 43685186], [44162419, 47272176, 62693156, 35359329], [36345796, 15667465, 53341561, 2978505], [1664472, 12761950, 34145519, 55197543], [37567005, 3228834, 6198166, 15646487], [63233399, 42640049, 12969011, 41620641], [22090925, 3386355, 56655568, 31631004], [16442787, 9420273, 48595545, 29770176], [49404288, 37823218, 58551818, 6772527], [36575583, 53847347, 32379432, 1630009], [9004247, 12999580, 48379959, 14252211], [25850203, 26136823, 64934025, 29362603], [10214276, 43557352, 33387586, 55512773], [45810841, 49561478, 41130845, 27034816], [34460081, 16560450, 57722793, 41007718], [53414778, 6845803, 15340368, 16647575], [30535873, 5193469, 43608154, 11391114], [20622004, 34424126, 31475211, 29619615], [10428836, 49656416, 7912677, 33427787], [57600861, 18251799, 46147432, 58946294], [6760779, 14675737, 42952146, 5480498], [46037552, 39969058, 30103468, 55330772], [64466305, 29376674, 49914839, 55269895], [36494113, 27010567, 65752150, 12395385], [49385632, 19550767, 39809394, 58806235], [20987521, 37444597, 49290126, 42326125], [37150229, 37487849, 28254397, 32949826], [9724895, 53813417, 19431235, 27438556], [42132748, 47073733, 19396568, 10026137], [3961481, 27204521, 62087205, 37602005], [22178323, 17505521, 42006207, 44143605], [12753258, 63063515, 61993175, 8920985], [10998000, 64833190, 6446892, 63676805], [66983817, 63684932, 18378359, 39946382], [63476803, 60000436, 19442420, 66417845], [38004446, 64752157, 42570179, 52844512], [1270809, 23735482, 17543294, 18795903], [4862706, 16352249, 57100612, 6219870], [63203206, 25630930, 35608240, 51357885], [59819625, 64662579, 50925335, 55670434], [29216830, 26446697, 52243336, 58475666], [43138915, 30592834, 43931516, 50628002]], dtype=jnp.int32), jnp.array([[71233, 771721, 71505, 706185], [289177, 484147, 358809, 484147], [359355, 549137, 359096, 549137], [350631, 558133, 350630, 554037], [370087, 538677, 370087, 538677], [4432, 899725, 4432, 904077], [678487, 229987, 678487, 229987], [423799, 480614, 423799, 480870], [549958, 284804, 549958, 280708], [423848, 480565, 423848, 480549], [489129, 283940, 554921, 283940], [86641, 822120, 86641, 822120], [206370, 702394, 206370, 567209], [500533, 407959, 500533, 407959], [759723, 79137, 759723, 79137], [563305, 345460, 559209, 345460], [231733, 611478, 231733, 611478], [502682, 406082, 498585, 406082], [554567, 288662, 554567, 288662], [476823, 427846, 476823, 427846], [488823, 415846, 488823, 415846], [431687, 477078, 431687, 477078], [419159, 424070, 415062, 424070], [493399, 345734, 493143, 345718], [678295, 230451, 678295, 230451], [496520, 342596, 496520, 346709], [567109, 276116, 567109, 276116], [624005, 284758, 624005, 284758], [420249, 484420, 420248, 484420], [217715, 621418, 217715, 621418], [344884, 493977, 344884, 493977], [550841, 292132, 550841, 292132], [284262, 558967, 284006, 558967], [152146, 756616, 152146, 756616], [144466, 698763, 144466, 694667], [284261, 624504, 284261, 624504], [288406, 620102, 288405, 620358], [301366, 607383, 301366, 607382], [468771, 435882, 468771, 435882], [555688, 283444, 555688, 283444], [485497, 414820, 485497, 414820], [633754, 275010, 633754, 275010], [419141, 489608, 419157, 489608], [694121, 214387, 694121, 214387], [480869, 427639, 481125, 427639], [489317, 419447, 489301, 419447], [152900, 747672, 152900, 747672], [348516, 494457, 348516, 494457], [534562, 370088, 534562, 370088], [371272, 537475, 371274, 537475], [144194, 760473, 144194, 760473], [567962, 275011, 567962, 275011], [493161, 350052, 493161, 350052], [490138, 348979, 490138, 348979], [328450, 506552, 328450, 506552], [148882, 759593, 148626, 755497], [642171, 266593, 642171, 266593], [685894, 218774, 685894, 218774], [674182, 234548, 674214, 234548], [756347, 152146, 690811, 86353], [612758, 291894, 612758, 291894], [296550, 612214, 296550, 612214], [363130, 475730, 363130, 475730], [691559, 16496, 691559, 16496], [340755, 502202, 336659, 502218], [632473, 210499, 628377, 210483], [564410, 266513, 564410, 266513], [427366, 481399, 427366, 481399], [493159, 349797, 493159, 415605], [331793, 576972, 331793, 576972], [416681, 492084, 416681, 492084], [813496, 95265, 813496, 91153], [695194, 213571, 695194, 213571], [436105, 407124, 436105, 407124], [836970, 6243, 902506, 6243], [160882, 747882, 160882, 747882], [493977, 414788, 489624, 414788], [29184, 551096, 29184, 616888], [903629, 4880, 899517, 4880], [351419, 553250, 351419, 553250], [75554, 767671, 75554, 767671], [279909, 563304, 279909, 563304], [215174, 628054, 215174, 628054], [361365, 481864, 361365, 481864], [424022, 484743, 358486, 484725], [271650, 633018, 271650, 633018], [681896, 226867, 616088, 226867], [222580, 686184, 222564, 686184], [144451, 698778, 209987, 698778], [532883, 310086, 532883, 310086], [628872, 279893, 628872, 279893], [533797, 374951, 533797, 374951], [91713, 817036, 91713, 817036], [427605, 477046, 431718, 477046], [145490, 689529, 145490, 689529], [551098, 291875, 551098, 291875], [349781, 558984, 349781, 558983], [205378, 703115, 205378, 703115], [362053, 546456, 362053, 546456], [612248, 226371, 678040, 226371]], dtype=jnp.int32)
-        # fmt: on
+        if dds_hash_table_path is None:
+            dds_hash_table_path = os.path.join(
+                os.getcwd(), "dds_hash_table.npz"
+            )
+        try:
+            self.hash_keys, self.hash_values = jnp.load(dds_hash_table_path)
+        except FileNotFoundError as e:
+            print(e)
+            print("Try the following methods")
+            print(
+                "1. Place the 'keys.npy' and 'values.npy' you created or downloaded in 'current_directry/dds_hash_table'"
+            )
+            print("2. Give the path of the dds hash table as an argument")
+            sys.exit(1)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         key1, key2, key3 = jax.random.split(key, num=3)
         return _init_by_key(jax.random.choice(key2, self.hash_keys), key3)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
@@ -141,20 +149,20 @@
     shuffled_players = _shuffle_players(rng6)
     current_player = shuffled_players[dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
     legal_actions = legal_actions.at[36].set(False)
     legal_actions = legal_actions.at[37].set(False)
     state = State(  # type: ignore
-        shuffled_players=shuffled_players,
+        _shuffled_players=shuffled_players,
         current_player=current_player,
-        hand=hand,
-        dealer=dealer,
-        vul_NS=vul_NS,
-        vul_EW=vul_EW,
+        _hand=hand,
+        _dealer=dealer,
+        _vul_NS=vul_NS,
+        _vul_EW=vul_EW,
         legal_action_mask=legal_actions,
     )
     return state
 
 
 @jax.jit
 def _init_by_key(key: jnp.ndarray, rng: jax.random.KeyArray) -> State:
@@ -168,20 +176,20 @@
     shuffled_players = _shuffle_players(rng5)
     current_player = shuffled_players[dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
     legal_actions = legal_actions.at[36].set(False)
     legal_actions = legal_actions.at[37].set(False)
     state = State(  # type: ignore
-        shuffled_players=shuffled_players,
+        _shuffled_players=shuffled_players,
         current_player=current_player,
-        hand=hand,
-        dealer=dealer,
-        vul_NS=vul_NS,
-        vul_EW=vul_EW,
+        _hand=hand,
+        _dealer=dealer,
+        _vul_NS=vul_NS,
+        _vul_EW=vul_EW,
         legal_action_mask=legal_actions,
     )
     return state
 
 
 @jax.jit
 def _shuffle_players(rng: jax.random.KeyArray) -> jnp.ndarray:
@@ -229,29 +237,29 @@
 
 
 @jax.jit
 def _player_position(player: jnp.ndarray, state: State) -> jnp.ndarray:
     return jax.lax.cond(
         player != -1,
         lambda: jnp.int8(
-            jnp.argmax(state.shuffled_players == player)
+            jnp.argmax(state._shuffled_players == player)
         ),  # playerと同じ要素のstate.shuffle_playersのindexを返す
         lambda: jnp.int8(-1),
     )
 
 
 @jax.jit
 def _step(
     state: State,
     action: int,
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> State:
     # fmt: off
-    state = state.replace(bidding_history=state.bidding_history.at[state.turn].set(action))  # type: ignore
+    state = state.replace(_bidding_history=state._bidding_history.at[state._turn].set(action))  # type: ignore
     # fmt: on
     return jax.lax.cond(
         action >= 35,
         lambda: jax.lax.switch(
             action - 35,
             [
                 lambda: jax.lax.cond(
@@ -269,60 +277,61 @@
     )
 
 
 @jax.jit
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     """Returns the observation of a given player"""
     # make vul of observation
-    vul = jnp.array([state.vul_NS, state.vul_EW], dtype=jnp.bool_)
+    vul = jnp.array([state._vul_NS, state._vul_EW], dtype=jnp.bool_)
 
     # make hand of observation
     hand = jnp.zeros(52, dtype=jnp.bool_)
     position = _player_position(player_id, state).astype(jnp.int16)
     hand = jax.lax.fori_loop(
         position * 13,
         (position + 1) * 13,
-        lambda i, hand: hand.at[state.hand[i]].set(True),
+        lambda i, hand: hand.at[state._hand[i]].set(True),
         hand,
     )
 
     # make history of observation
     obs_history = jnp.zeros(424, dtype=jnp.bool_)
     last_bid = jnp.int16(-1)
     flag = FALSE
     obs_history, last_bid, flag, state = jax.lax.fori_loop(
         0,
-        state.turn.astype(jnp.int32),
+        state._turn.astype(jnp.int32),
         _make_obs_history,
         (obs_history, last_bid, flag, state),
     )
     return jnp.concatenate((vul, obs_history, hand))
 
 
 @jax.jit
 def _make_obs_history(i, vals):
     obs_history, last_bid, flag, state = vals
-    curr_pos = ((state.dealer + i) % 4).astype(jnp.int16)
+    curr_pos = ((state._dealer + i) % 4).astype(jnp.int16)
     return jax.lax.cond(
-        (flag != jnp.bool_(True)) & (state.bidding_history[i] == 35),
+        (flag != jnp.bool_(True)) & (state._bidding_history[i] == 35),
         lambda: (obs_history.at[curr_pos].set(True), last_bid, flag, state),
         lambda: jax.lax.cond(
-            (0 <= state.bidding_history[i]) & (state.bidding_history[i] <= 34),
+            (0 <= state._bidding_history[i])
+            & (state._bidding_history[i] <= 34),
             lambda: (
                 obs_history.at[
                     4
                     + curr_pos * 35
-                    + state.bidding_history[i].astype(jnp.int16)
+                    + state._bidding_history[i].astype(jnp.int16)
                 ].set(True),
-                state.bidding_history[i].astype(jnp.int16),
+                state._bidding_history[i].astype(jnp.int16),
                 jnp.bool_(True),
                 state,
             ),
             lambda: jax.lax.switch(
-                state.bidding_history[i] - 35,
+                state._bidding_history[i] - 35,
                 [
                     lambda: (obs_history, last_bid, flag, state),
                     lambda: (
                         obs_history.at[144 + curr_pos * 35 + last_bid].set(
                             True
                         ),
                         last_bid,
@@ -347,15 +356,18 @@
 def duplicate(
     init_state: State,
 ) -> State:
     """Make duplicated state where NSplayer and EWplayer are swapped"""
     duplicated_state = copy.deepcopy(init_state)
     ix = jnp.array([1, 0, 3, 2])
     # fmt: off
-    duplicated_state = duplicated_state.replace(shuffled_players=duplicated_state.shuffled_players[ix], current_player=duplicated_state.shuffled_players[ix][duplicated_state.dealer])  # type: ignore
+    duplicated_state = duplicated_state.replace(  # type: ignore
+        _shuffled_players=duplicated_state._shuffled_players[ix],
+        current_player=duplicated_state._shuffled_players[ix][duplicated_state._dealer]
+    )
     # fmt: on
     return duplicated_state
 
 
 @jax.jit
 def _terminated_step(
     state: State,
@@ -373,29 +385,35 @@
 @jax.jit
 def _continue_step(
     state: State,
 ) -> State:
     """Return state when the game continues"""
     # fmt: off
     # 次ターンのプレイヤー、ターン数
-    state = state.replace(current_player=state.shuffled_players[(state.dealer + state.turn + 1) % 4], turn=state.turn + 1)  # type: ignore
+    state = state.replace(  # type: ignore
+        current_player=state._shuffled_players[(state._dealer + state._turn + 1) % 4],
+        _turn=state._turn + 1
+    )
     # 次のターンにX, XXが合法手か判断
     x_mask, xx_mask = _update_legal_action_X_XX(state)
-    return state.replace(legal_action_mask=state.legal_action_mask.at[36].set(x_mask).at[37].set(xx_mask), reward=jnp.zeros(4, dtype=jnp.float32))  # type: ignore
+    return state.replace(  # type: ignore
+        legal_action_mask=state.legal_action_mask.at[36].set(x_mask).at[37].set(xx_mask),
+        reward=jnp.zeros(4, dtype=jnp.float32)
+    )
     # fmt: on
 
 
 @jax.jit
 def _is_terminated(state: State) -> bool:
     """Check if the game is finished
     Four consecutive passes if not bid (pass out), otherwise three consecutive passes
     """
     return jax.lax.cond(
-        ((state.last_bid == -1) & (state.pass_num == 4))
-        | ((state.last_bid != -1) & (state.pass_num == 3)),
+        ((state._last_bid == -1) & (state._pass_num == 4))
+        | ((state._last_bid != -1) & (state._pass_num == 3)),
         lambda: True,
         lambda: False,
     )
 
 
 @jax.jit
 def _reward(
@@ -403,15 +421,15 @@
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> jnp.ndarray:
     """Return reward
     If pass out, 0 reward for everyone; if bid, calculate and return reward
     """
     return jax.lax.cond(
-        (state.last_bid == -1) & (state.pass_num == 4),
+        (state._last_bid == -1) & (state._pass_num == 4),
         lambda: jnp.zeros(4, dtype=jnp.float32),  # pass out
         lambda: _make_reward(  # caluculate reward
             state, hash_keys, hash_values
         ),
     )
 
 
@@ -433,16 +451,16 @@
     # Calculate the tricks you could have accomplished with this contraption
     dds_trick = dds_tricks[declare_position * 5 + denomination]
     # Clculate score
     score = _calc_score(
         denomination,
         level,
         vul,
-        state.call_x,
-        state.call_xx,
+        state._call_x,
+        state._call_xx,
         dds_trick,
     )
     # Make reward array in playerID order
     player_positions = jax.vmap(lambda i: _player_position(i, state))(
         jnp.arange(4)
     )
     partners = jax.vmap(lambda pos: _is_partner(pos, declare_position))(
@@ -621,73 +639,84 @@
 
 
 @jax.jit
 def _contract(
     state: State,
 ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray, jnp.ndarray]:
     """Return Contract which has position of declare ,denomination, level"""
-    denomination = state.last_bid % 5
-    level = state.last_bid // 5 + 1
+    denomination = state._last_bid % 5
+    level = state._last_bid // 5 + 1
     declare_position, vul = jax.lax.cond(
-        _position_to_team(_player_position(state.last_bidder, state)) == 0,
+        _position_to_team(_player_position(state._last_bidder, state)) == 0,
         lambda: (
-            _player_position(state.first_denomination_NS[denomination], state),
-            state.vul_NS,
+            _player_position(
+                state._first_denomination_NS[denomination], state
+            ),
+            state._vul_NS,
         ),
         lambda: (
-            _player_position(state.first_denomination_EW[denomination], state),
-            state.vul_EW,
+            _player_position(
+                state._first_denomination_EW[denomination], state
+            ),
+            state._vul_EW,
         ),
     )
     return declare_position, denomination, level, vul
 
 
 @jax.jit
 def _state_pass(
     state: State,
 ) -> State:
     """Change state if pass is taken"""
-    return state.replace(pass_num=state.pass_num + 1)  # type: ignore
+    return state.replace(_pass_num=state._pass_num + 1)  # type: ignore
 
 
 @jax.jit
 def _state_X(state: State) -> State:
     """Change state if double(X) is taken"""
-    return state.replace(call_x=jnp.bool_(True), pass_num=jnp.int32(0))  # type: ignore
+    return state.replace(_call_x=jnp.bool_(True), _pass_num=jnp.int32(0))  # type: ignore
 
 
 @jax.jit
 def _state_XX(state: State) -> State:
     """Change state if double(XX) is taken"""
-    return state.replace(call_xx=jnp.bool_(True), pass_num=jnp.int32(0))  # type: ignore
+    return state.replace(_call_xx=jnp.bool_(True), _pass_num=jnp.int32(0))  # type: ignore
 
 
 @jax.jit
 def _state_bid(state: State, action: int) -> State:
     """Change state if bid is taken"""
     # 最後のbidとそのプレイヤーを保存
     # fmt: off
-    state = state.replace(last_bid=jnp.int32(action), last_bidder=state.current_player)  # type: ignore
+    state = state.replace(_last_bid=jnp.int32(action), _last_bidder=state.current_player)  # type: ignore
     # fmt: on
     # チーム内で各denominationを最初にbidしたプレイヤー
     denomination = _bid_to_denomination(action)
-    team = _position_to_team(_player_position(state.last_bidder, state))
+    team = _position_to_team(_player_position(state._last_bidder, state))
     # fmt: off
     # team = 1ならEWチーム
-    state = jax.lax.cond(team & (state.first_denomination_EW[denomination] == -1),
-                         lambda: state.replace(first_denomination_EW=state.first_denomination_EW.at[denomination].set(state.last_bidder.astype(jnp.int8))),  # type: ignore
+    state = jax.lax.cond(team & (state._first_denomination_EW[denomination] == -1),
+                         lambda: state.replace(_first_denomination_EW=state._first_denomination_EW.at[denomination].set(state._last_bidder.astype(jnp.int8))),  # type: ignore
                          lambda: state)  # type: ignore
     # team = 0ならNSチーム
-    state = jax.lax.cond((team == 0) & (state.first_denomination_NS[denomination] == -1),
-                         lambda: state.replace(first_denomination_NS=state.first_denomination_NS.at[denomination].set(state.last_bidder.astype(jnp.int8))),  # type: ignore
+    state = jax.lax.cond((team == 0) & (state._first_denomination_NS[denomination] == -1),
+                         lambda: state.replace(_first_denomination_NS=state._first_denomination_NS.at[denomination].set(state._last_bidder.astype(jnp.int8))),  # type: ignore
                          lambda: state)  # type: ignore
     # fmt: on
     # 小さいbidを非合法手にする
     mask = jnp.arange(38) < action + 1
-    return state.replace(legal_action_mask=jnp.where(mask, jnp.bool_(0), state.legal_action_mask), call_x=jnp.bool_(False), call_xx=jnp.bool_(False), pass_num=jnp.int32(0))  # type: ignore
+    return state.replace(  # type: ignore
+        legal_action_mask=jnp.where(
+            mask, jnp.bool_(0), state.legal_action_mask
+        ),
+        _call_x=jnp.bool_(False),
+        _call_xx=jnp.bool_(False),
+        _pass_num=jnp.int32(0),
+    )
 
 
 @jax.jit
 def _bid_to_denomination(bid: int) -> int:
     """Calcularete denomination of bid"""
     return bid % 5
 
@@ -702,45 +731,45 @@
 
 @jax.jit
 def _update_legal_action_X_XX(
     state: State,
 ) -> Tuple[bool, bool]:
     """Determine if X or XX is a legal move for the next player"""
     return jax.lax.cond(
-        state.last_bidder != -1,
+        state._last_bidder != -1,
         lambda: (_is_legal_X(state), _is_legal_XX(state)),
         lambda: (False, False),
     )
 
 
 @jax.jit
 def _is_legal_X(state: State) -> bool:
     return jax.lax.cond(
-        (state.call_x == 0)
-        & (state.call_xx == 0)
+        (state._call_x == 0)
+        & (state._call_xx == 0)
         & (
             _is_partner(
-                _player_position(state.last_bidder, state),
+                _player_position(state._last_bidder, state),
                 _player_position(state.current_player, state),
             )
             == 0
         ),
         lambda: True,
         lambda: False,
     )
 
 
 @jax.jit
 def _is_legal_XX(state: State) -> bool:
     return jax.lax.cond(
-        state.call_x
-        & (state.call_xx == 0)
+        state._call_x
+        & (state._call_xx == 0)
         & (
             _is_partner(
-                _player_position(state.last_bidder, state),
+                _player_position(state._last_bidder, state),
                 _player_position(state.current_player, state),
             )
         ),
         lambda: True,
         lambda: False,
     )
 
@@ -751,15 +780,15 @@
     return (abs(position1 - position2) + 1) % 2
 
 
 def _state_to_pbn(state: State) -> str:
     """Convert state to pbn format"""
     pbn = "N:"
     for i in range(4):  # player
-        hand = jnp.sort(state.hand[i * 13 : (i + 1) * 13])
+        hand = jnp.sort(state._hand[i * 13 : (i + 1) * 13])
         for j in range(4):  # suit
             card = [
                 TO_CARD[i % 13] for i in hand if j * 13 <= i < (j + 1) * 13
             ][::-1]
             if card != [] and card[-1] == "A":
                 card = card[-1:] + card[:-1]
             pbn += "".join(card)
@@ -770,15 +799,15 @@
                 pbn += "."
     return pbn
 
 
 @jax.jit
 def _state_to_key(state: State) -> jnp.ndarray:
     """Convert state to key of dds table"""
-    hand = state.hand
+    hand = state._hand
     key = jnp.zeros(52, dtype=jnp.int8)
     for i in range(52):  # N: 0, E: 1, S: 2, W: 3
         key = key.at[hand[i]].set(i // 13)
     key = key.reshape(4, 13)
     return _to_binary(key)
```

### Comparing `pgx-0.5.1/pgx/chess.py` & `pgx-0.5.2/pgx/chess.py`

 * *Files 17% similar despite different names*

```diff
@@ -111,31 +111,31 @@
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # 64 * 73 = 4672
     observation: jnp.ndarray = jnp.zeros((8, 8, 19), dtype=jnp.float32)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Chess specific ---
-    turn: jnp.ndarray = jnp.int8(0)
-    board: jnp.ndarray = INIT_BOARD  # 左上からFENと同じ形式で埋めていく
+    _turn: jnp.ndarray = jnp.int8(0)
+    _board: jnp.ndarray = INIT_BOARD  # 左上からFENと同じ形式で埋めていく
     # (curr, opp) Flips every turn
-    can_castle_queen_side: jnp.ndarray = jnp.ones(2, dtype=jnp.bool_)
-    can_castle_king_side: jnp.ndarray = jnp.ones(2, dtype=jnp.bool_)
-    en_passant: jnp.ndarray = jnp.int8(-1)  # En passant target. Flips.
+    _can_castle_queen_side: jnp.ndarray = jnp.ones(2, dtype=jnp.bool_)
+    _can_castle_king_side: jnp.ndarray = jnp.ones(2, dtype=jnp.bool_)
+    _en_passant: jnp.ndarray = jnp.int8(-1)  # En passant target. Flips.
     # # of moves since the last piece capture or pawn move
-    halfmove_count: jnp.ndarray = jnp.int32(0)
-    fullmove_count: jnp.ndarray = jnp.int32(1)  # increase every black move
-    zobrist_hash: jnp.ndarray = jnp.uint32([1429435994, 901419182])
-    hash_history: jnp.ndarray = (
+    _halfmove_count: jnp.ndarray = jnp.int32(0)
+    _fullmove_count: jnp.ndarray = jnp.int32(1)  # increase every black move
+    _zobrist_hash: jnp.ndarray = jnp.uint32([1429435994, 901419182])
+    _hash_history: jnp.ndarray = (
         jnp.zeros((1001, 2), dtype=jnp.uint32)
         .at[0]
         .set(jnp.uint32([1429435994, 901419182]))
     )
     # index to possible piece positions for speeding up. Flips every turn.
-    possible_piece_positions: jnp.ndarray = INIT_POSSIBLE_PIECE_POSITIONS
+    _possible_piece_positions: jnp.ndarray = INIT_POSSIBLE_PIECE_POSITIONS
 
     @property
     def env_id(self) -> v1.EnvId:
         return "chess"
 
     @staticmethod
     def _from_fen(fen: str):
@@ -235,17 +235,17 @@
     )
     state = _check_termination(state)
     return state
 
 
 def _check_termination(state: State):
     has_legal_action = state.legal_action_mask.any()
-    rep = (state.hash_history == state.zobrist_hash).any(axis=1).sum() - 1
+    rep = (state._hash_history == state._zobrist_hash).any(axis=1).sum() - 1
     terminated = ~has_legal_action
-    terminated |= state.halfmove_count >= 100
+    terminated |= state._halfmove_count >= 100
     terminated |= has_insufficient_pieces(state)
     terminated |= rep >= 2
 
     is_checkmate = (~has_legal_action) & _is_checking(_flip(state))
     # fmt: off
     reward = jax.lax.select(
         is_checkmate,
@@ -258,25 +258,25 @@
         reward=reward,
     )
 
 
 def has_insufficient_pieces(state: State):
     # Uses the same condition as OpenSpiel.
     # See https://github.com/deepmind/open_spiel/blob/master/open_spiel/games/chess/chess_board.cc#L724
-    num_pieces = (state.board != EMPTY).sum()
+    num_pieces = (state._board != EMPTY).sum()
     num_pawn_rook_queen = (
-        (jnp.abs(state.board) >= ROOK) | (jnp.abs(state.board) == PAWN)
+        (jnp.abs(state._board) >= ROOK) | (jnp.abs(state._board) == PAWN)
     ).sum() - 2  # two kings
-    num_bishop = (jnp.abs(state.board) == 3).sum()
+    num_bishop = (jnp.abs(state._board) == 3).sum()
     coords = jnp.arange(64).reshape((8, 8))
     # [ 0  2  4  6 16 18 20 22 32 34 36 38 48 50 52 54 9 11 13 15 25 27 29 31 41 43 45 47 57 59 61 63]
     black_coords = jnp.hstack(
         (coords[::2, ::2].ravel(), coords[1::2, 1::2].ravel())
     )
-    num_bishop_on_black = (jnp.abs(state.board[black_coords]) == BISHOP).sum()
+    num_bishop_on_black = (jnp.abs(state._board[black_coords]) == BISHOP).sum()
     is_insufficient = FALSE
     # King vs King
     is_insufficient |= num_pieces <= 2
     # King + X vs King. X == KNIGHT or BISHOP
     is_insufficient |= (num_pieces == 3) & (num_pawn_rook_queen == 0)
     # King + Bishop* vs King + Bishop* (Bishops are on same color tile)
     is_bishop_all_on_black = num_bishop_on_black == num_bishop
@@ -286,89 +286,93 @@
     )
 
     return is_insufficient
 
 
 def _apply_move(state: State, a: Action):
     # apply move action
-    piece = state.board[a.from_]
+    piece = state._board[a.from_]
     # en passant
     is_en_passant = (
-        (state.en_passant >= 0) & (piece == PAWN) & (state.en_passant == a.to)
+        (state._en_passant >= 0)
+        & (piece == PAWN)
+        & (state._en_passant == a.to)
     )
     removed_pawn_pos = a.to - 1
     state = state.replace(  # type: ignore
-        board=state.board.at[removed_pawn_pos].set(
-            jax.lax.select(is_en_passant, EMPTY, state.board[removed_pawn_pos])
+        _board=state._board.at[removed_pawn_pos].set(
+            jax.lax.select(
+                is_en_passant, EMPTY, state._board[removed_pawn_pos]
+            )
         ),
     )
     state = state.replace(  # type: ignore
-        en_passant=jax.lax.select(
+        _en_passant=jax.lax.select(
             (piece == PAWN) & (jnp.abs(a.to - a.from_) == 2),
             jnp.int8((a.to + a.from_) // 2),
             jnp.int8(-1),
         )
     )
     # update counters
-    captured = (state.board[a.to] < 0) | (is_en_passant)
+    captured = (state._board[a.to] < 0) | (is_en_passant)
     state = state.replace(  # type: ignore
-        halfmove_count=jax.lax.select(
-            captured | (piece == PAWN), 0, state.halfmove_count + 1
+        _halfmove_count=jax.lax.select(
+            captured | (piece == PAWN), 0, state._halfmove_count + 1
         ),
-        fullmove_count=state.fullmove_count + jnp.int32(state.turn == 1),
+        _fullmove_count=state._fullmove_count + jnp.int32(state._turn == 1),
     )
     # castling
     # 可能かどうかの判断はここでは行わない。castlingがlegalでない場合はフィルタされている前提
     # left
     state = state.replace(  # type: ignore
-        board=jax.lax.cond(
+        _board=jax.lax.cond(
             (piece == KING) & (a.from_ == 32) & (a.to == 16),
-            lambda: state.board.at[0].set(EMPTY).at[24].set(ROOK),
-            lambda: state.board,
+            lambda: state._board.at[0].set(EMPTY).at[24].set(ROOK),
+            lambda: state._board,
         )
     )
     # right
     state = state.replace(  # type: ignore
-        board=jax.lax.cond(
+        _board=jax.lax.cond(
             (piece == KING) & (a.from_ == 32) & (a.to == 48),
-            lambda: state.board.at[56].set(EMPTY).at[40].set(ROOK),
-            lambda: state.board,
+            lambda: state._board.at[56].set(EMPTY).at[40].set(ROOK),
+            lambda: state._board,
         )
     )
     # update my can_castle_xxx_side
     state = state.replace(  # type: ignore
-        can_castle_queen_side=state.can_castle_queen_side.at[0].set(
+        _can_castle_queen_side=state._can_castle_queen_side.at[0].set(
             jax.lax.select(
                 (a.from_ == 32) | (a.from_ == 0),
                 FALSE,
-                state.can_castle_queen_side[0],
+                state._can_castle_queen_side[0],
             )
         ),
-        can_castle_king_side=state.can_castle_king_side.at[0].set(
+        _can_castle_king_side=state._can_castle_king_side.at[0].set(
             jax.lax.select(
                 (a.from_ == 32) | (a.from_ == 56),
                 FALSE,
-                state.can_castle_king_side[0],
+                state._can_castle_king_side[0],
             )
         ),
     )
     # update opp can_castle_xxx_side
     state = state.replace(  # type: ignore
-        can_castle_queen_side=state.can_castle_queen_side.at[1].set(
+        _can_castle_queen_side=state._can_castle_queen_side.at[1].set(
             jax.lax.select(
                 (a.to == 7),
                 FALSE,
-                state.can_castle_queen_side[1],
+                state._can_castle_queen_side[1],
             )
         ),
-        can_castle_king_side=state.can_castle_king_side.at[1].set(
+        _can_castle_king_side=state._can_castle_king_side.at[1].set(
             jax.lax.select(
                 (a.to == 63),
                 FALSE,
-                state.can_castle_king_side[1],
+                state._can_castle_king_side[1],
             )
         ),
     )
     # promotion to queen
     piece = jax.lax.select(
         piece == PAWN & (a.from_ % 8 == 6) & (a.underpromotion < 0),
         QUEEN,
@@ -378,22 +382,22 @@
     piece = jax.lax.select(
         a.underpromotion < 0,
         piece,
         jnp.int8([ROOK, BISHOP, KNIGHT])[a.underpromotion],
     )
     # actually move
     state = state.replace(  # type: ignore
-        board=state.board.at[a.from_].set(EMPTY).at[a.to].set(piece)
+        _board=state._board.at[a.from_].set(EMPTY).at[a.to].set(piece)
     )
     # update possible piece positions
-    ix = jnp.argmin(jnp.abs(state.possible_piece_positions[0, :] - a.from_))
+    ix = jnp.argmin(jnp.abs(state._possible_piece_positions[0, :] - a.from_))
     state = state.replace(  # type: ignore
-        possible_piece_positions=state.possible_piece_positions.at[0, ix].set(
-            a.to
-        )
+        _possible_piece_positions=state._possible_piece_positions.at[
+            0, ix
+        ].set(a.to)
     )
     return state
 
 
 def _flip_pos(x):
     """
     >>> _flip_pos(jnp.int8(34))
@@ -409,34 +413,34 @@
 def _rotate(board):
     return jnp.rot90(board, k=1)
 
 
 def _flip(state: State) -> State:
     return state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
-        board=-jnp.flip(state.board.reshape(8, 8), axis=1).flatten(),
-        turn=(state.turn + 1) % 2,
-        en_passant=_flip_pos(state.en_passant),
-        can_castle_queen_side=state.can_castle_queen_side[::-1],
-        can_castle_king_side=state.can_castle_king_side[::-1],
-        possible_piece_positions=state.possible_piece_positions[::-1],
+        _board=-jnp.flip(state._board.reshape(8, 8), axis=1).flatten(),
+        _turn=(state._turn + 1) % 2,
+        _en_passant=_flip_pos(state._en_passant),
+        _can_castle_queen_side=state._can_castle_queen_side[::-1],
+        _can_castle_king_side=state._can_castle_king_side[::-1],
+        _possible_piece_positions=state._possible_piece_positions[::-1],
     )
 
 
 def _legal_action_mask(state):
     def is_legal(a: Action):
         ok = _is_pseudo_legal(state, a)
         next_s = _flip(_apply_move(state, a))
         ok &= ~_is_checking(next_s)
 
         return ok
 
     @jax.vmap
     def legal_norml_moves(from_):
-        piece = state.board[from_]
+        piece = state._board[from_]
 
         @jax.vmap
         def legal_label(to):
             a = Action(from_=from_, to=to)
             return jax.lax.select(
                 (from_ >= 0) & (piece > 0) & (to >= 0) & is_legal(a),
                 a._to_label(),
@@ -455,78 +459,78 @@
         labels = make_labels(
             jnp.int32([6, 14, 22, 30, 38, 46, 54, 62])
         ).flatten()
 
         @jax.vmap
         def legal_labels(label):
             a = Action._from_label(label)
-            ok = (state.board[a.from_] == PAWN) & (a.to >= 0)
+            ok = (state._board[a.from_] == PAWN) & (a.to >= 0)
             ok &= mask[Action(from_=a.from_, to=a.to)._to_label()]
             return jax.lax.select(ok, label, -1)
 
         ok_labels = legal_labels(labels)
         return ok_labels.flatten()
 
     def legal_en_passants():
-        to = state.en_passant
+        to = state._en_passant
 
         @jax.vmap
         def legal_labels(from_):
             ok = (
                 (from_ >= 0)
                 & (from_ < 64)
                 & (to >= 0)
-                & (state.board[from_] == PAWN)
-                & (state.board[to - 1] == -PAWN)
+                & (state._board[from_] == PAWN)
+                & (state._board[to - 1] == -PAWN)
             )
             a = Action(from_=from_, to=to)
             ok &= ~_is_checking(_flip(_apply_move(state, a)))
             return jax.lax.select(ok, a._to_label(), -1)
 
         return legal_labels(jnp.int32([to - 9, to + 7]))
 
     def can_castle_king_side():
-        ok = state.board[32] == KING
-        ok &= state.board[56] == ROOK
-        ok &= state.can_castle_king_side[0]
-        ok &= state.board[40] == EMPTY
-        ok &= state.board[48] == EMPTY
+        ok = state._board[32] == KING
+        ok &= state._board[56] == ROOK
+        ok &= state._can_castle_king_side[0]
+        ok &= state._board[40] == EMPTY
+        ok &= state._board[48] == EMPTY
 
         @jax.vmap
         def is_ok(label):
             return ~_is_checking(
                 _flip(_apply_move(state, Action._from_label(label)))
             )
 
         ok &= ~_is_checking(_flip(state))
         ok &= is_ok(jnp.int32([2366, 2367])).all()
 
         return ok
 
     def can_castle_queen_side():
-        ok = state.board[32] == KING
-        ok &= state.board[0] == ROOK
-        ok &= state.can_castle_queen_side[0]
-        ok &= state.board[8] == EMPTY
-        ok &= state.board[16] == EMPTY
-        ok &= state.board[24] == EMPTY
+        ok = state._board[32] == KING
+        ok &= state._board[0] == ROOK
+        ok &= state._can_castle_queen_side[0]
+        ok &= state._board[8] == EMPTY
+        ok &= state._board[16] == EMPTY
+        ok &= state._board[24] == EMPTY
 
         @jax.vmap
         def is_ok(label):
             return ~_is_checking(
                 _flip(_apply_move(state, Action._from_label(label)))
             )
 
         ok &= ~_is_checking(_flip(state))
         ok &= is_ok(jnp.int32([2364, 2365])).all()
 
         return ok
 
     actions = legal_norml_moves(
-        state.possible_piece_positions[0]
+        state._possible_piece_positions[0]
     ).flatten()  # include -1
     # +1 is to avoid setting True to the last element
     mask = jnp.zeros(64 * 73 + 1, dtype=jnp.bool_)
     mask = mask.at[actions].set(TRUE)
 
     # castling
     mask = mask.at[2364].set(
@@ -554,42 +558,42 @@
         return (from_ != -1) & _is_pseudo_legal(state, a)
 
     return can_move(CAN_MOVE_ANY[pos, :]).any()
 
 
 def _is_checking(state: State):
     """True if possible to capture the opponent king"""
-    opp_king_pos = jnp.argmin(jnp.abs(state.board - -KING))
+    opp_king_pos = jnp.argmin(jnp.abs(state._board - -KING))
     return _is_attacking(state, opp_king_pos)
 
 
 def _is_pseudo_legal(state: State, a: Action):
-    piece = state.board[a.from_]
-    ok = (piece >= 0) & (state.board[a.to] <= 0)
+    piece = state._board[a.from_]
+    ok = (piece >= 0) & (state._board[a.to] <= 0)
     ok &= (CAN_MOVE[piece, a.from_] == a.to).any()
     between_ixs = BETWEEN[a.from_, a.to]
-    ok &= ((between_ixs < 0) | (state.board[between_ixs] == EMPTY)).all()
+    ok &= ((between_ixs < 0) | (state._board[between_ixs] == EMPTY)).all()
     # filter pawn move
     ok &= ~((piece == PAWN) & ((a.to % 8) < (a.from_ % 8)))
     ok &= ~(
         (piece == PAWN)
         & (jnp.abs(a.to - a.from_) <= 2)
-        & (state.board[a.to] < 0)
+        & (state._board[a.to] < 0)
     )
     ok &= ~(
         (piece == PAWN)
         & (jnp.abs(a.to - a.from_) > 2)
-        & (state.board[a.to] >= 0)
+        & (state._board[a.to] >= 0)
     )
     return (a.to >= 0) & ok
 
 
 def _possible_piece_positions(state):
-    my_pos = jnp.nonzero(state.board > 0, size=16, fill_value=-1)[0]
-    opp_pos = jnp.nonzero(_flip(state).board > 0, size=16, fill_value=-1)[0]
+    my_pos = jnp.nonzero(state._board > 0, size=16, fill_value=-1)[0]
+    opp_pos = jnp.nonzero(_flip(state)._board > 0, size=16, fill_value=-1)[0]
     return jnp.vstack((my_pos, opp_pos))
 
 
 def _observe(state: State):
     """Our observation design is very similar to OpenSpiel
     except two differences:
 
@@ -604,32 +608,32 @@
     - [13] 1 color
     - [14, ..., 17] 4 castling
     - [18] 1 no progress count
     """
 
     @jax.vmap
     def is_piece(piece):
-        return _rotate((state.board == piece).reshape((8, 8))).astype(
+        return _rotate((state._board == piece).reshape((8, 8))).astype(
             jnp.float32
         )
 
     ONE_PLANE = jnp.ones((1, 8, 8), dtype=jnp.float32)
 
     my_pieces = is_piece(jnp.arange(1, 7))
     opp_pieces = is_piece(-jnp.arange(1, 7))
     # See also https://github.com/LeelaChessZero/lc0/blob/f39ad6ceb62c186136fc80ad08c466217c485aa1/src/neural/encoder.cc#L290
-    rep = (state.hash_history == state.zobrist_hash).all(axis=1).sum() - 1
+    rep = (state._hash_history == state._zobrist_hash).all(axis=1).sum() - 1
     repetitions = ONE_PLANE * (rep >= 1)
-    color = ONE_PLANE * state.turn
-    my_queen_side_castling_right = ONE_PLANE * state.can_castle_queen_side[0]
-    my_king_side_castling_right = ONE_PLANE * state.can_castle_king_side[0]
-    opp_queen_side_castling_right = ONE_PLANE * state.can_castle_queen_side[1]
-    opp_king_side_castling_right = ONE_PLANE * state.can_castle_king_side[1]
+    color = ONE_PLANE * state._turn
+    my_queen_side_castling_right = ONE_PLANE * state._can_castle_queen_side[0]
+    my_king_side_castling_right = ONE_PLANE * state._can_castle_king_side[0]
+    opp_queen_side_castling_right = ONE_PLANE * state._can_castle_queen_side[1]
+    opp_king_side_castling_right = ONE_PLANE * state._can_castle_king_side[1]
     no_progress_count = (
-        ONE_PLANE * state.halfmove_count.astype(jnp.float32) / 100.0
+        ONE_PLANE * state._halfmove_count.astype(jnp.float32) / 100.0
     )
 
     return jnp.vstack(
         [
             my_pieces,
             opp_pieces,
             repetitions,
@@ -647,15 +651,15 @@
 
 def _zobrist_hash(state):
     """
     >>> state = State()
     >>> _zobrist_hash(state)
     Array([1429435994,  901419182], dtype=uint32)
     """
-    board = jax.lax.select(state.turn == 0, state.board, _flip(state).board)
+    board = jax.lax.select(state._turn == 0, state._board, _flip(state)._board)
     hash_ = jnp.uint32([0, 0])
 
     def xor(i, h):
         # 0, ..., 12 (white pawn, ..., black king)
         piece = board[i] + 6
         return h ^ HASH_TABLE[i][piece]
 
@@ -663,62 +667,62 @@
     return hash_
 
 
 def _update_zobrist_hash(state: State, action: Action):
     """
     >>> state = State()
     >>> state = _update_zobrist_hash(state, Action._from_label(jnp.int32(89)))
-    >>> state.zobrist_hash
+    >>> state._zobrist_hash
     Array([ 511492215, 1223082425], dtype=uint32)
     """
-    hash_ = state.zobrist_hash
+    hash_ = state._zobrist_hash
     # fmt: off
-    board = jax.lax.select(state.turn == 0, state.board, _flip(state).board)
-    from_ = jax.lax.select(state.turn == 0, action.from_, _flip_pos(action.from_))
-    to = jax.lax.select(state.turn == 0, action.to, _flip_pos(action.to))
+    board = jax.lax.select(state._turn == 0, state._board, _flip(state)._board)
+    from_ = jax.lax.select(state._turn == 0, action.from_, _flip_pos(action.from_))
+    to = jax.lax.select(state._turn == 0, action.to, _flip_pos(action.to))
     # fmt: on
     piece = board[from_]
     hash_ ^= HASH_TABLE[from_][piece]
     hash_ ^= HASH_TABLE[to][piece]
     return state.replace(  # type: ignore
-        zobrist_hash=hash_,
-        hash_history=state.hash_history.at[state._step_count].set(hash_),
+        _zobrist_hash=hash_,
+        _hash_history=state._hash_history.at[state._step_count].set(hash_),
     )
 
 
 def _from_fen(fen: str):
     """Restore state from FEN
 
     >>> state = _from_fen(
     ...     "rnbqkbnr/pppppppp/8/8/8/P7/1PPPPPPP/RNBQKBNR w KQkq e3 0 1"
     ... )
-    >>> _rotate(state.board.reshape(8, 8))
+    >>> _rotate(state._board.reshape(8, 8))
     Array([[-4, -2, -3, -5, -6, -3, -2, -4],
            [-1, -1, -1, -1, -1, -1, -1, -1],
            [ 0,  0,  0,  0,  0,  0,  0,  0],
            [ 0,  0,  0,  0,  0,  0,  0,  0],
            [ 0,  0,  0,  0,  0,  0,  0,  0],
            [ 1,  0,  0,  0,  0,  0,  0,  0],
            [ 0,  1,  1,  1,  1,  1,  1,  1],
            [ 4,  2,  3,  5,  6,  3,  2,  4]], dtype=int8)
-    >>> state.en_passant
+    >>> state._en_passant
     Array(34, dtype=int8)
     >>> state = _from_fen(
     ...     "rnbqkbnr/pppppppp/8/8/8/P7/1PPPPPPP/RNBQKBNR b KQkq e3 0 1"
     ... )
-    >>> _rotate(state.board.reshape(8, 8))
+    >>> _rotate(state._board.reshape(8, 8))
     Array([[-4, -2, -3, -5, -6, -3, -2, -4],
            [ 0, -1, -1, -1, -1, -1, -1, -1],
            [-1,  0,  0,  0,  0,  0,  0,  0],
            [ 0,  0,  0,  0,  0,  0,  0,  0],
            [ 0,  0,  0,  0,  0,  0,  0,  0],
            [ 0,  0,  0,  0,  0,  0,  0,  0],
            [ 1,  1,  1,  1,  1,  1,  1,  1],
            [ 4,  2,  3,  5,  6,  3,  2,  4]], dtype=int8)
-    >>> state.en_passant
+    >>> state._en_passant
     Array(37, dtype=int8)
     """
     board, turn, castling, en_passant, halfmove_cnt, fullmove_cnt = fen.split()
     arr = []
     for line in board.split("/"):
         for c in line:
             if str.isnumeric(c):
@@ -751,24 +755,24 @@
         else jnp.int8(
             "abcdefgh".index(en_passant[0]) * 8 + int(en_passant[1]) - 1
         )
     )
     if turn == "b" and ep >= 0:
         ep = _flip_pos(ep)
     state = State(  # type: ignore
-        board=jnp.rot90(mat, k=3).flatten(),
-        turn=jnp.int8(0) if turn == "w" else jnp.int8(1),
-        can_castle_queen_side=can_castle_queen_side,
-        can_castle_king_side=can_castle_king_side,
-        en_passant=ep,
-        halfmove_count=jnp.int32(halfmove_cnt),
-        fullmove_count=jnp.int32(fullmove_cnt),
+        _board=jnp.rot90(mat, k=3).flatten(),
+        _turn=jnp.int8(0) if turn == "w" else jnp.int8(1),
+        _can_castle_queen_side=can_castle_queen_side,
+        _can_castle_king_side=can_castle_king_side,
+        _en_passant=ep,
+        _halfmove_count=jnp.int32(halfmove_cnt),
+        _fullmove_count=jnp.int32(fullmove_cnt),
     )
     state = state.replace(  # type: ignore
-        possible_piece_positions=jax.jit(_possible_piece_positions)(state)
+        _possible_piece_positions=jax.jit(_possible_piece_positions)(state)
     )
     state = state.replace(  # type: ignore
         legal_action_mask=jax.jit(_legal_action_mask)(state),
     )
     state = jax.jit(_check_termination)(state)
     return state
 
@@ -782,26 +786,26 @@
     - 左上から開始して右に見ていく
     - 段が変わるときは/を挿入
     - 盤面の記入が終わったら手番（w/b）
     - キャスリングの可否。キングサイドにできる場合はK, クイーンサイドにできる場合はQを先後それぞれ書く。全部不可なら-
     - アンパッサン可能な位置。ポーンが2マス動いた場合はそのポーンが通過した位置を記録
     - 最後にポーンの移動および駒取りが発生してからの手数と通常の手数（0, 1で固定にする）
 
-    >>> s = State(en_passant=jnp.int8(34))
+    >>> s = State(_en_passant=jnp.int8(34))
     >>> _to_fen(s)
     'rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq e3 0 1'
     >>> _to_fen(
     ...     _from_fen(
     ...         "rnbqkbnr/pppppppp/8/8/8/P7/1PPPPPPP/RNBQKBNR b KQkq e3 0 1"
     ...     )
     ... )
     'rnbqkbnr/pppppppp/8/8/8/P7/1PPPPPPP/RNBQKBNR b KQkq e3 0 1'
     """
-    pb = jnp.rot90(state.board.reshape(8, 8), k=1)
-    if state.turn == 1:
+    pb = jnp.rot90(state._board.reshape(8, 8), k=1)
+    if state._turn == 1:
         pb = -jnp.flip(pb, axis=0)
     fen = ""
     # 盤面
     for i in range(8):
         space_length = 0
         for j in range(8):
             piece = pb[i, j]
@@ -818,19 +822,19 @@
         if space_length != 0:
             fen += str(space_length)
         if i != 7:
             fen += "/"
         else:
             fen += " "
     # 手番
-    fen += "w " if state.turn == 0 else "b "
+    fen += "w " if state._turn == 0 else "b "
     # キャスリング
-    can_castle_queen_side = state.can_castle_queen_side
-    can_castle_king_side = state.can_castle_king_side
-    if state.turn == 1:
+    can_castle_queen_side = state._can_castle_queen_side
+    can_castle_king_side = state._can_castle_king_side
+    if state._turn == 1:
         can_castle_queen_side = can_castle_queen_side[::-1]
         can_castle_king_side = can_castle_king_side[::-1]
     if not (can_castle_queen_side.any() | can_castle_king_side.any()):
         fen += "-"
     else:
         if can_castle_king_side[0]:
             fen += "K"
@@ -838,21 +842,21 @@
             fen += "Q"
         if can_castle_king_side[1]:
             fen += "k"
         if can_castle_queen_side[1]:
             fen += "q"
     fen += " "
     # アンパッサン
-    en_passant = state.en_passant
-    if state.turn == 1:
+    en_passant = state._en_passant
+    if state._turn == 1:
         en_passant = _flip_pos(en_passant)
     ep = int(en_passant.item())
     if ep == -1:
         fen += "-"
     else:
         fen += "abcdefgh"[ep // 8]
         fen += str(ep % 8 + 1)
     fen += " "
-    fen += str(state.halfmove_count.item())
+    fen += str(state._halfmove_count.item())
     fen += " "
-    fen += str(state.fullmove_count.item())
+    fen += str(state._fullmove_count.item())
     return fen
```

### Comparing `pgx-0.5.1/pgx/connect_four.py` & `pgx-0.5.2/pgx/connect_four.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(7, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Connect Four specific ---
-    turn: jnp.ndarray = jnp.int8(0)
+    _turn: jnp.ndarray = jnp.int8(0)
     # 6x7 board
     # [[ 0,  1,  2,  3,  4,  5,  6],
     #  [ 7,  8,  9, 10, 11, 12, 13],
     #  [14, 15, 16, 17, 18, 19, 20],
     #  [21, 22, 23, 24, 25, 26, 27],
     #  [28, 29, 30, 31, 32, 33, 34],
     #  [35, 36, 37, 38, 39, 40, 41]]
-    board: jnp.ndarray = -jnp.ones(42, jnp.int8)  # -1 (empty), 0, 1
-    blank_row: jnp.ndarray = jnp.full(7, 5)
+    _board: jnp.ndarray = -jnp.ones(42, jnp.int8)  # -1 (empty), 0, 1
+    _blank_row: jnp.ndarray = jnp.full(7, 5)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "connect_four"
 
 
 class ConnectFour(v1.Env):
@@ -110,48 +110,48 @@
 def _init(rng: jax.random.KeyArray) -> State:
     rng, subkey = jax.random.split(rng)
     current_player = jnp.int8(jax.random.bernoulli(subkey))
     return State(current_player=current_player)  # type:ignore
 
 
 def _step(state: State, action: jnp.ndarray) -> State:
-    board = state.board
-    row = state.blank_row[action]
-    blank_row = state.blank_row.at[action].set(row - 1)
-    board = board.at[_to_idx(row, action)].set(state.turn)
-    won = _win_check(board, state.turn)
+    board = state._board
+    row = state._blank_row[action]
+    blank_row = state._blank_row.at[action].set(row - 1)
+    board = board.at[_to_idx(row, action)].set(state._turn)
+    won = _win_check(board, state._turn)
     reward = jax.lax.cond(
         won,
         lambda: jnp.float32([-1, -1]).at[state.current_player].set(1),
         lambda: jnp.zeros(2, jnp.float32),
     )
     return state.replace(  # type: ignore
         current_player=1 - state.current_player,
         legal_action_mask=blank_row >= 0,
-        turn=1 - state.turn,
-        board=board,
-        blank_row=blank_row,
+        _turn=1 - state._turn,
+        _board=board,
+        _blank_row=blank_row,
         terminated=won | jnp.all(blank_row == -1),
         reward=reward,
     )
 
 
 def _to_idx(row, col):
     return row * 7 + col
 
 
 def _win_check(board, turn) -> jnp.ndarray:
     return ((board[IDX] == turn).all(axis=1)).any()
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
-    turns = jnp.int8([state.turn, 1 - state.turn])
+    turns = jnp.int8([state._turn, 1 - state._turn])
     turns = jax.lax.cond(
         player_id == state.current_player,
         lambda: turns,
         lambda: jnp.flip(turns),
     )
 
     def make(turn):
-        return state.board.reshape(6, 7) == turn
+        return state._board.reshape(6, 7) == turn
 
     return jnp.stack(jax.vmap(make)(turns), -1)
```

### Comparing `pgx-0.5.1/pgx/experimental/bridge_bidding.py` & `pgx-0.5.2/pgx/experimental/bridge_bidding.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,60 +72,60 @@
     state: State,
 ) -> State:
     """Make duplicated state where NSplayer and EWplayer are swapped
 
     >>> key = jax.random.PRNGKey(0)
     >>> state = env.init(key)
     >>> duplicate_state = _duplicate_init(state)
-    >>> duplicate_state.shuffled_players
+    >>> duplicate_state._shuffled_players
     Array([0, 2, 1, 3], dtype=int8)
-    >>> duplicate_state.dealer
+    >>> duplicate_state._dealer
     Array(1, dtype=int32)
     >>> duplicate_state.current_player
     Array(2, dtype=int8)
     >>> state = env.step(state, 35)
     >>> duplicate_state = _duplicate_init(state)
-    >>> duplicate_state.shuffled_players
+    >>> duplicate_state._shuffled_players
     Array([0, 2, 1, 3], dtype=int8)
-    >>> duplicate_state.dealer
+    >>> duplicate_state._dealer
     Array(1, dtype=int32)
     >>> duplicate_state.current_player
     Array(2, dtype=int8)
-    >>> duplicate_state.pass_num
+    >>> duplicate_state._pass_num
     Array(0, dtype=int32)
 
     >>> state = env.step(state, 0)
     >>> duplicate_state = _duplicate_init(state)
-    >>> duplicate_state.shuffled_players
+    >>> duplicate_state._shuffled_players
     Array([0, 2, 1, 3], dtype=int8)
-    >>> duplicate_state.dealer
+    >>> duplicate_state._dealer
     Array(1, dtype=int32)
     >>> duplicate_state.current_player
     Array(2, dtype=int8)
     >>> duplicate_state.legal_action_mask
     Array([ True,  True,  True,  True,  True,  True,  True,  True,  True,
             True,  True,  True,  True,  True,  True,  True,  True,  True,
             True,  True,  True,  True,  True,  True,  True,  True,  True,
             True,  True,  True,  True,  True,  True,  True,  True,  True,
            False, False], dtype=bool)
     """
     ix = jnp.array([1, 0, 3, 2])
-    shuffled_players = state.shuffled_players[ix]
-    current_player = shuffled_players[state.dealer]
+    shuffled_players = state._shuffled_players[ix]
+    current_player = shuffled_players[state._dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
     legal_actions = legal_actions.at[36].set(False)
     legal_actions = legal_actions.at[37].set(False)
     duplicated_state = State(  # type: ignore
-        shuffled_players=state.shuffled_players[ix],
+        _shuffled_players=state._shuffled_players[ix],
         current_player=current_player,
-        hand=state.hand,
-        dealer=state.dealer,
-        vul_NS=state.vul_NS,
-        vul_EW=state.vul_EW,
+        _hand=state._hand,
+        _dealer=state._dealer,
+        _vul_NS=state._vul_NS,
+        _vul_EW=state._vul_EW,
         legal_action_mask=legal_actions,
     )
     return duplicated_state
 
 
 @jax.jit
 def duplicate_step(
```

### Comparing `pgx-0.5.1/pgx/experimental/gym.py` & `pgx-0.5.2/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/experimental/pettingzoo.py` & `pgx-0.5.2/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/experimental/visualize.py` & `pgx-0.5.2/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/experimental/wrappers.py` & `pgx-0.5.2/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/go.py` & `pgx-0.5.2/pgx/go.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,35 +31,35 @@
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(19 * 19 + 1, dtype=jnp.bool_)
     observation: jnp.ndarray = jnp.zeros((19, 19, 17), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Go specific ---
-    size: jnp.ndarray = jnp.int32(19)  # NOTE: require 19 * 19 > int8
+    _size: jnp.ndarray = jnp.int32(19)  # NOTE: require 19 * 19 > int8
     # ids of representative stone id (smallest) in the connected stones
     # positive for black, negative for white, and zero for empty.
     # require at least 19 * 19 > int8, idx_squared_sum can be 361^2 > int16
-    chain_id_board: jnp.ndarray = jnp.zeros(19 * 19, dtype=jnp.int32)
-    board_history: jnp.ndarray = jnp.full((8, 19 * 19), 2, dtype=jnp.int8)
-    turn: jnp.ndarray = jnp.int8(0)  # 0 = black's turn, 1 = white's turn
-    num_captured_stones: jnp.ndarray = jnp.zeros(
+    _chain_id_board: jnp.ndarray = jnp.zeros(19 * 19, dtype=jnp.int32)
+    _board_history: jnp.ndarray = jnp.full((8, 19 * 19), 2, dtype=jnp.int8)
+    _turn: jnp.ndarray = jnp.int8(0)  # 0 = black's turn, 1 = white's turn
+    _num_captured_stones: jnp.ndarray = jnp.zeros(
         2, dtype=jnp.int32
     )  # [0]=black, [1]=white
-    passed: jnp.ndarray = FALSE  # TRUE if last action is pass
-    ko: jnp.ndarray = jnp.int32(-1)  # by SSK
-    komi: jnp.ndarray = jnp.float32(7.5)
-    black_player: jnp.ndarray = jnp.int8(0)
+    _passed: jnp.ndarray = FALSE  # TRUE if last action is pass
+    _ko: jnp.ndarray = jnp.int32(-1)  # by SSK
+    _komi: jnp.ndarray = jnp.float32(7.5)
+    _black_player: jnp.ndarray = jnp.int8(0)
 
     @property
     def env_id(self) -> v1.EnvId:
         try:
-            size = int(self.size.item())
+            size = int(self._size.item())
         except TypeError:
-            size = int(self.size[0].item())
+            size = int(self._size[0].item())
         return f"go-{size}x{size}"  # type: ignore
 
 
 class Go(v1.Env):
     def __init__(
         self,
         *,
@@ -148,90 +148,90 @@
         lambda: (current_player_color, -1 * current_player_color),
         lambda: (-1 * current_player_color, current_player_color),
     )
 
     @jax.vmap
     def _make(i):
         color = jnp.int8([1, -1])[i % 2] * my_color
-        return state.board_history[i // 2] == color
+        return state._board_history[i // 2] == color
 
     log = _make(jnp.arange(history_length * 2))
     color = jnp.full_like(log[0], my_color == 1)  # black=1, white=0
 
     return jnp.vstack([log, color]).transpose().reshape((size, size, -1))
 
 
 def _init(key: jax.random.KeyArray, size: int, komi: float = 7.5) -> State:
     black_player = jnp.int8(jax.random.bernoulli(key))
     current_player = black_player
     return State(  # type:ignore
-        size=jnp.int32(size),
-        chain_id_board=jnp.zeros(size**2, dtype=jnp.int32),
+        _size=jnp.int32(size),
+        _chain_id_board=jnp.zeros(size**2, dtype=jnp.int32),
         legal_action_mask=jnp.ones(size**2 + 1, dtype=jnp.bool_),
-        board_history=jnp.full((8, size**2), 2, dtype=jnp.int8),
+        _board_history=jnp.full((8, size**2), 2, dtype=jnp.int8),
         current_player=current_player,
-        komi=jnp.float32(komi),
-        black_player=black_player,
+        _komi=jnp.float32(komi),
+        _black_player=black_player,
     )
 
 
 def _step(state: State, action: int, size: int) -> State:
-    state = state.replace(ko=jnp.int32(-1))  # type: ignore
+    state = state.replace(_ko=jnp.int32(-1))  # type: ignore
     # update state
     state = jax.lax.cond(
         (action < size * size),
         lambda: _not_pass_move(state, action, size),
         lambda: _pass_move(state, size),
     )
 
     # increment turns
-    state = state.replace(turn=(state.turn + 1) % 2)  # type: ignore
+    state = state.replace(_turn=(state._turn + 1) % 2)  # type: ignore
     state = state.replace(current_player=(state.current_player + 1) % 2)  # type: ignore
 
     # add legal action mask
     state = state.replace(  # type:ignore
         legal_action_mask=state.legal_action_mask.at[:-1]
         .set(legal_actions(state, size))
         .at[-1]
         .set(TRUE)
     )
 
     # update board history
-    board_history = jnp.roll(state.board_history, size**2)
+    board_history = jnp.roll(state._board_history, size**2)
     board_history = board_history.at[0].set(
-        jnp.clip(state.chain_id_board, -1, 1).astype(jnp.int8)
+        jnp.clip(state._chain_id_board, -1, 1).astype(jnp.int8)
     )
-    state = state.replace(board_history=board_history)  # type:ignore
+    state = state.replace(_board_history=board_history)  # type:ignore
 
     # check PSK up to 8-steps before
     state = _check_PSK(state)
     return state
 
 
 def _pass_move(state: State, size) -> State:
     return jax.lax.cond(
-        state.passed,
+        state._passed,
         # consecutive passes results in the game end
         lambda: state.replace(terminated=TRUE, reward=_get_reward(state, size)),  # type: ignore
         # One pass continues the game
-        lambda: state.replace(passed=TRUE, reward=jnp.zeros(2, dtype=jnp.float32)),  # type: ignore
+        lambda: state.replace(_passed=TRUE, reward=jnp.zeros(2, dtype=jnp.float32)),  # type: ignore
     )
 
 
 def _not_pass_move(state: State, action, size) -> State:
-    state = state.replace(passed=FALSE)  # type: ignore
+    state = state.replace(_passed=FALSE)  # type: ignore
     xy = action
-    num_captured_stones_before = state.num_captured_stones[state.turn]
+    num_captured_stones_before = state._num_captured_stones[state._turn]
 
     ko_may_occur = _ko_may_occur(state, xy)
 
     # Remove killed stones
     adj_xy = _neighbour(xy, size)
     oppo_color = _opponent_color(state)
-    chain_id = state.chain_id_board[adj_xy]
+    chain_id = state._chain_id_board[adj_xy]
     num_pseudo, idx_sum, idx_squared_sum = _count(state, size)
     chain_ix = jnp.abs(chain_id) - 1
     is_atari = (idx_sum[chain_ix] ** 2) == idx_squared_sum[
         chain_ix
     ] * num_pseudo[chain_ix]
     single_liberty = (idx_squared_sum[chain_ix] // idx_sum[chain_ix]) - 1
     is_killed = (
@@ -256,92 +256,92 @@
     state = jax.lax.fori_loop(
         0, 4, lambda i, s: _merge_around_xy(i, s, xy, size), state
     )
 
     # Check Ko
     # fmt: off
     state = jax.lax.cond(
-        state.num_captured_stones[state.turn] - num_captured_stones_before == 1,
+        state._num_captured_stones[state._turn] - num_captured_stones_before == 1,
         lambda: state,
-        lambda: state.replace(ko=jnp.int32(-1)),  # type:ignore
+        lambda: state.replace(_ko=jnp.int32(-1)),  # type:ignore
     )
     # fmt: on
 
     return state.replace(reward=jnp.zeros(2, dtype=jnp.float32))  # type: ignore
 
 
 def _merge_around_xy(i, state: State, xy, size):
     my_color = _my_color(state)
     adj_xy = _neighbour(xy, size)[i]
     is_off = adj_xy == -1
-    is_my_chain = state.chain_id_board[adj_xy] * my_color > 0
+    is_my_chain = state._chain_id_board[adj_xy] * my_color > 0
     state = jax.lax.cond(
         ((~is_off) & is_my_chain),
         lambda: _merge_chain(state, xy, adj_xy),
         lambda: state,
     )
     return state
 
 
 def _set_stone(state: State, xy) -> State:
     my_color = _my_color(state)
     return state.replace(  # type:ignore
-        chain_id_board=state.chain_id_board.at[xy].set((xy + 1) * my_color),
+        _chain_id_board=state._chain_id_board.at[xy].set((xy + 1) * my_color),
     )
 
 
 def _merge_chain(state: State, xy, adj_xy):
     my_color = _my_color(state)
-    new_id = jnp.abs(state.chain_id_board[xy])
-    adj_chain_id = jnp.abs(state.chain_id_board[adj_xy])
+    new_id = jnp.abs(state._chain_id_board[xy])
+    adj_chain_id = jnp.abs(state._chain_id_board[adj_xy])
     small_id = jnp.minimum(new_id, adj_chain_id) * my_color
     large_id = jnp.maximum(new_id, adj_chain_id) * my_color
 
     # 大きいidの連を消し、小さいidの連と繋げる
     chain_id_board = jnp.where(
-        state.chain_id_board == large_id, small_id, state.chain_id_board
+        state._chain_id_board == large_id, small_id, state._chain_id_board
     )
 
-    return state.replace(chain_id_board=chain_id_board)  # type: ignore
+    return state.replace(_chain_id_board=chain_id_board)  # type: ignore
 
 
 def _remove_stones(
     state: State, rm_chain_id, rm_stone_xy, ko_may_occur
 ) -> State:
-    surrounded_stones = state.chain_id_board == rm_chain_id
+    surrounded_stones = state._chain_id_board == rm_chain_id
     num_captured_stones = jnp.count_nonzero(surrounded_stones)
-    chain_id_board = jnp.where(surrounded_stones, 0, state.chain_id_board)
+    chain_id_board = jnp.where(surrounded_stones, 0, state._chain_id_board)
     ko = jax.lax.cond(
         ko_may_occur & (num_captured_stones == 1),
         lambda: jnp.int32(rm_stone_xy),
-        lambda: state.ko,
+        lambda: state._ko,
     )
     return state.replace(  # type:ignore
-        chain_id_board=chain_id_board,
-        num_captured_stones=state.num_captured_stones.at[state.turn].add(
+        _chain_id_board=chain_id_board,
+        _num_captured_stones=state._num_captured_stones.at[state._turn].add(
             num_captured_stones
         ),
-        ko=ko,
+        _ko=ko,
     )
 
 
 def legal_actions(state: State, size: int) -> jnp.ndarray:
     """Logic is highly inspired by OpenSpiel's Go implementation"""
-    is_empty = state.chain_id_board == 0
+    is_empty = state._chain_id_board == 0
 
     my_color = _my_color(state)
     opp_color = _opponent_color(state)
     num_pseudo, idx_sum, idx_squared_sum = _count(state, size)
 
-    chain_ix = jnp.abs(state.chain_id_board) - 1
+    chain_ix = jnp.abs(state._chain_id_board) - 1
     # fmt: off
     in_atari = (idx_sum[chain_ix] ** 2) == idx_squared_sum[chain_ix] * num_pseudo[chain_ix]
     # fmt: on
-    has_liberty = (state.chain_id_board * my_color > 0) & ~in_atari
-    kills_opp = (state.chain_id_board * opp_color > 0) & in_atari
+    has_liberty = (state._chain_id_board * my_color > 0) & ~in_atari
+    kills_opp = (state._chain_id_board * opp_color > 0) & in_atari
 
     @jax.vmap
     def is_neighbor_ok(xy):
         neighbors = _neighbour(xy, size)
         on_board = neighbors != -1
         _has_empty = is_empty[neighbors]
         _has_liberty = has_liberty[neighbors]
@@ -352,23 +352,23 @@
             | (on_board & _has_liberty).any()
         )
 
     neighbor_ok = is_neighbor_ok(jnp.arange(size**2))
     legal_action_mask = is_empty & neighbor_ok
 
     return jax.lax.cond(
-        (state.ko == -1),
+        (state._ko == -1),
         lambda: legal_action_mask,
-        lambda: legal_action_mask.at[state.ko].set(FALSE),
+        lambda: legal_action_mask.at[state._ko].set(FALSE),
     )
 
 
 def _count(state: State, size):
     ZERO = jnp.int32(0)
-    chain_id_board = jnp.abs(state.chain_id_board)
+    chain_id_board = jnp.abs(state._chain_id_board)
     is_empty = chain_id_board == 0
     idx_sum = jnp.where(is_empty, jnp.arange(1, size**2 + 1), ZERO)
     idx_squared_sum = jnp.where(
         is_empty, jnp.arange(1, size**2 + 1) ** 2, ZERO
     )
 
     @jax.vmap
@@ -398,54 +398,54 @@
             chain_id_board == (x + 1), idx_squared_sum, ZERO
         ).sum()
 
     return _num_pseudo(idx), _idx_sum(idx), _idx_squared_sum(idx)
 
 
 def _my_color(state: State):
-    return jnp.int32([1, -1])[state.turn]
+    return jnp.int32([1, -1])[state._turn]
 
 
 def _opponent_color(state: State):
-    return jnp.int32([-1, 1])[state.turn]
+    return jnp.int32([-1, 1])[state._turn]
 
 
 def _ko_may_occur(state: State, xy: int) -> jnp.ndarray:
-    size = state.size
+    size = state._size
     x = xy // size
     y = xy % size
     oob = jnp.bool_([x - 1 < 0, x + 1 >= size, y - 1 < 0, y + 1 >= size])
     oppo_color = _opponent_color(state)
     is_occupied_by_opp = (
-        state.chain_id_board[_neighbour(xy, size)] * oppo_color > 0
+        state._chain_id_board[_neighbour(xy, size)] * oppo_color > 0
     )
     return (oob | is_occupied_by_opp).all()
 
 
 def _count_point(state, size):
     return jnp.array(
         [
             _count_ji(state, 1, size)
-            + jnp.count_nonzero(state.chain_id_board > 0),
+            + jnp.count_nonzero(state._chain_id_board > 0),
             _count_ji(state, -1, size)
-            + jnp.count_nonzero(state.chain_id_board < 0),
+            + jnp.count_nonzero(state._chain_id_board < 0),
         ],
         dtype=jnp.float32,
     )
 
 
 def _get_reward(state: State, size: int) -> jnp.ndarray:
     score = _count_point(state, size)
     reward_bw = jax.lax.cond(
-        score[0] - state.komi > score[1],
+        score[0] - state._komi > score[1],
         lambda: jnp.array([1, -1], dtype=jnp.float32),
         lambda: jnp.array([-1, 1], dtype=jnp.float32),
     )
     reward = jax.lax.cond(
-        state.black_player == 0,
+        state._black_player == 0,
         lambda: reward_bw,
         lambda: reward_bw[jnp.int8([1, 0])],
     )
     return reward
 
 
 def _neighbour(xy, size):
@@ -458,17 +458,17 @@
 
 
 def _neighbours(size):
     return jax.vmap(partial(_neighbour, size=size))(jnp.arange(size**2))
 
 
 def _count_ji(state: State, color: int, size: int):
-    board = jnp.zeros_like(state.chain_id_board)
-    board = jnp.where(state.chain_id_board * color > 0, 1, board)
-    board = jnp.where(state.chain_id_board * color < 0, -1, board)
+    board = jnp.zeros_like(state._chain_id_board)
+    board = jnp.where(state._chain_id_board * color > 0, 1, board)
+    board = jnp.where(state._chain_id_board * color < 0, -1, board)
     # 0 = empty, 1 = mine, -1 = opponent's
 
     neighbours = _neighbours(size)
 
     def is_opp_neighbours(b):
         # True if empty and any of neighbours is opponent
         return (b == 0) & (
@@ -512,15 +512,15 @@
     - Pgx employs SSK for legal actions, PSK is approximated by up to 8-steps before board, and approximate PSK action leads to immediate lose
       - Pros: Agent may be able to avoid PSK (as it observes board history up to 8-steps in AlphaGo Zero feature)
       - Cons: Ignoring the old same boards
 
     Anyway, we believe it's effect is very small as PSK rarely happens, especially in 19x19 board.
     """
     # fmt: off
-    is_psk = ~state.passed & (jnp.abs(state.board_history[0] - state.board_history[1:]).sum(axis=1) == 0).any()
+    is_psk = ~state._passed & (jnp.abs(state._board_history[0] - state._board_history[1:]).sum(axis=1) == 0).any()
     winner = state.current_player
     state = jax.lax.cond(
         is_psk,
         lambda: state.replace(  # type: ignore
             terminated=TRUE,
             reward=jnp.float32([-1, -1]).at[winner].set(1.0),
         ),
@@ -532,17 +532,17 @@
 
 # only for debug
 def _show(state: State) -> None:
     BLACK_CHAR = "@"
     WHITE_CHAR = "O"
     POINT_CHAR = "+"
     print("===========")
-    for xy in range(state.size * state.size):
-        if state.chain_id_board[xy] > 0:
+    for xy in range(state._size * state._size):
+        if state._chain_id_board[xy] > 0:
             print(" " + BLACK_CHAR, end="")
-        elif state.chain_id_board[xy] < 0:
+        elif state._chain_id_board[xy] < 0:
             print(" " + WHITE_CHAR, end="")
         else:
             print(" " + POINT_CHAR, end="")
 
-        if xy % state.size == state.size - 1:
+        if xy % state._size == state._size - 1:
             print()
```

### Comparing `pgx-0.5.1/pgx/hex.py` & `pgx-0.5.2/pgx/hex.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(11 * 11, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Hex specific ---
-    size: jnp.ndarray = jnp.int8(11)
+    _size: jnp.ndarray = jnp.int8(11)
     # 0(black), 1(white)
-    turn: jnp.ndarray = jnp.int8(0)
+    _turn: jnp.ndarray = jnp.int8(0)
     # 11x11 board
     # [[  0,  1,  2,  ...,  8,  9, 10],
     #  [ 11,  12, 13, ..., 19, 20, 21],
     #  .
     #  .
     #  .
     #  [110, 111, 112, ...,  119, 120]]
-    board: jnp.ndarray = -jnp.zeros(
+    _board: jnp.ndarray = -jnp.zeros(
         11 * 11, jnp.int32
     )  # <0(oppo), 0(empty), 0<(self)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "hex"
 
@@ -87,56 +87,56 @@
     def num_players(self) -> int:
         return 2
 
 
 def _init(rng: jax.random.KeyArray, size: int) -> State:
     rng, subkey = jax.random.split(rng)
     current_player = jnp.int8(jax.random.bernoulli(subkey))
-    return State(size=size, current_player=current_player)  # type:ignore
+    return State(_size=size, current_player=current_player)  # type:ignore
 
 
 def _step(state: State, action: jnp.ndarray, size: int) -> State:
     set_place_id = action + 1
-    board = state.board.at[action].set(set_place_id)
+    board = state._board.at[action].set(set_place_id)
     neighbour = _neighbour(action, size)
 
     def merge(i, b):
         adj_pos = neighbour[i]
         return jax.lax.cond(
             (adj_pos >= 0) & (b[adj_pos] > 0),
             lambda: jnp.where(b == b[adj_pos], set_place_id, b),
             lambda: b,
         )
 
     board = jax.lax.fori_loop(0, 6, merge, board)
-    won = _is_game_end(board, size, state.turn)
+    won = _is_game_end(board, size, state._turn)
     reward = jax.lax.cond(
         won,
         lambda: jnp.float32([-1, -1]).at[state.current_player].set(1),
         lambda: jnp.zeros(2, jnp.float32),
     )
 
     legal_action_mask = board == 0
     state = state.replace(  # type:ignore
         current_player=1 - state.current_player,
-        turn=1 - state.turn,
-        board=board * -1,
+        _turn=1 - state._turn,
+        _board=board * -1,
         reward=reward,
         terminated=won,
         legal_action_mask=legal_action_mask,
     )
 
     return state
 
 
 def _observe(state: State, player_id: jnp.ndarray, size) -> jnp.ndarray:
     board = jax.lax.cond(
         player_id == state.current_player,
-        lambda: state.board.reshape((size, size)),
-        lambda: (state.board * -1).reshape((size, size)),
+        lambda: state._board.reshape((size, size)),
+        lambda: (state._board * -1).reshape((size, size)),
     )
 
     def make(color):
         return board * color > 0
 
     return jnp.stack(jax.vmap(make)(jnp.int8([1, -1])), 2)
 
@@ -166,9 +166,9 @@
         return (_id > 0) & (_id == bottom).any()
 
     return jax.vmap(check_same_id_exist)(top).any()
 
 
 def _get_abs_board(state):
     return jax.lax.cond(
-        state.turn == 0, lambda: state.board, lambda: state.board * -1
+        state._turn == 0, lambda: state._board, lambda: state._board * -1
     )
```

### Comparing `pgx-0.5.1/pgx/kuhn_poker.py` & `pgx-0.5.2/pgx/kuhn_poker.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Kuhn poker specific ---
-    cards: jnp.ndarray = jnp.int8([-1, -1])
+    _cards: jnp.ndarray = jnp.int8([-1, -1])
     # [(player 0),(player 1)]
-    last_action: jnp.ndarray = jnp.int8(-1)
+    _last_action: jnp.ndarray = jnp.int8(-1)
     # 0(Call)  1(Bet)  2(Fold)  3(Check)
-    pot: jnp.ndarray = jnp.int8([0, 0])
+    _pot: jnp.ndarray = jnp.int8([0, 0])
 
     @property
     def env_id(self) -> v1.EnvId:
         return "kuhn_poker"
 
 
 class KuhnPoker(v1.Env):
@@ -82,42 +82,42 @@
     rng1, rng2 = jax.random.split(rng)
     current_player = jnp.int8(jax.random.bernoulli(rng1))
     init_card = jax.random.choice(
         rng2, jnp.int8([[0, 1], [0, 2], [1, 0], [1, 2], [2, 0], [2, 1]])
     )
     return State(  # type:ignore
         current_player=current_player,
-        cards=init_card,
+        _cards=init_card,
         legal_action_mask=jnp.bool_([0, 1, 0, 1]),
     )
 
 
 def _step(state: State, action):
     action = jnp.int8(action)
     pot = jax.lax.cond(
         (action == BET) | (action == CALL),
-        lambda: state.pot.at[state.current_player].add(1),
-        lambda: state.pot,
+        lambda: state._pot.at[state.current_player].add(1),
+        lambda: state._pot,
     )
 
     terminated, reward = jax.lax.cond(
         action == FOLD,
         lambda: (
             TRUE,
             jnp.float32([-1, -1]).at[1 - state.current_player].set(1),
         ),
         lambda: (FALSE, jnp.float32([0, 0])),
     )
     terminated, reward = jax.lax.cond(
-        (state.last_action == BET) & (action == CALL),
+        (state._last_action == BET) & (action == CALL),
         lambda: (TRUE, _get_unit_reward(state) * 2),
         lambda: (terminated, reward),
     )
     terminated, reward = jax.lax.cond(
-        (state.last_action == CHECK) & (action == CHECK),
+        (state._last_action == CHECK) & (action == CHECK),
         lambda: (TRUE, _get_unit_reward(state)),
         lambda: (terminated, reward),
     )
 
     legal_action = jax.lax.switch(
         action,
         [
@@ -126,37 +126,37 @@
             lambda: jnp.bool_([0, 0, 0, 0]),  # FOLD
             lambda: jnp.bool_([0, 1, 0, 1]),  # CHECK
         ],
     )
 
     return state.replace(  # type:ignore
         current_player=1 - state.current_player,
-        last_action=action,
+        _last_action=action,
         legal_action_mask=legal_action,
         terminated=terminated,
         reward=reward,
-        pot=pot,
+        _pot=pot,
     )
 
 
 def _get_unit_reward(state: State):
     return jax.lax.cond(
-        state.cards[state.current_player]
-        > state.cards[1 - state.current_player],
+        state._cards[state.current_player]
+        > state._cards[1 - state.current_player],
         lambda: jnp.float32([-1, -1]).at[state.current_player].set(1),
         lambda: jnp.float32([-1, -1]).at[1 - state.current_player].set(1),
     )
 
 
 def _observe(state: State, player_id) -> jnp.ndarray:
     """
     Index   Meaning
     0~2     J ~ K in hand
     3~4     0~1 chips for the current player
     5~6     0~1 chips for the opponent
     """
     obs = jnp.zeros(7, dtype=jnp.bool_)
-    obs = obs.at[state.cards[player_id]].set(TRUE)
-    obs = obs.at[3 + state.pot[player_id]].set(TRUE)
-    obs = obs.at[5 + state.pot[1 - player_id]].set(TRUE)
+    obs = obs.at[state._cards[player_id]].set(TRUE)
+    obs = obs.at[3 + state._pot[player_id]].set(TRUE)
+    obs = obs.at[5 + state._pot[1 - player_id]].set(TRUE)
 
     return obs
```

### Comparing `pgx-0.5.1/pgx/leduc_holdem.py` & `pgx-0.5.2/pgx/leduc_holdem.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,22 @@
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Leduc Hold'Em specific ---
-    first_player: jnp.ndarray = jnp.int8(0)
-
+    _first_player: jnp.ndarray = jnp.int8(0)
     # [(player 0), (player 1), (public)]
-    cards: jnp.ndarray = jnp.int8([-1, -1, -1])
-
+    _cards: jnp.ndarray = jnp.int8([-1, -1, -1])
     # 0(Call)  1(Bet)  2(Fold)  3(Check)
-    last_action: jnp.ndarray = INVALID_ACTION
-
-    chips: jnp.ndarray = jnp.ones(2, dtype=jnp.int8)
-    round: jnp.ndarray = jnp.int8(0)
-    raise_count: jnp.ndarray = jnp.int8(0)
+    _last_action: jnp.ndarray = INVALID_ACTION
+    _chips: jnp.ndarray = jnp.ones(2, dtype=jnp.int8)
+    _round: jnp.ndarray = jnp.int8(0)
+    _raise_count: jnp.ndarray = jnp.int8(0)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "leduc_holdem"
 
 
 class LeducHoldem(v1.Env):
@@ -91,44 +88,44 @@
     rng1, rng2, rng3 = jax.random.split(rng, 3)
     current_player = jnp.int8(jax.random.bernoulli(rng1))
     init_card = jax.random.permutation(
         rng2, jnp.int8([0, 0, 1, 1, 2, 2]), independent=True
     )
     return State(  # type:ignore
         _rng_key=rng3,
-        first_player=current_player,
+        _first_player=current_player,
         current_player=current_player,
-        cards=init_card[:3],
+        _cards=init_card[:3],
         legal_action_mask=jnp.bool_([1, 1, 0]),
-        chips=jnp.ones(2, dtype=jnp.int8),
+        _chips=jnp.ones(2, dtype=jnp.int8),
     )
 
 
 def _step(state: State, action):
     action = jnp.int8(action)
     chips = jax.lax.switch(
         action,
         [
-            lambda: state.chips.at[state.current_player].set(
-                state.chips[1 - state.current_player]
+            lambda: state._chips.at[state.current_player].set(
+                state._chips[1 - state.current_player]
             ),  # CALL
-            lambda: state.chips.at[state.current_player].set(
-                jnp.max(state.chips) + _raise_chips(state)
+            lambda: state._chips.at[state.current_player].set(
+                jnp.max(state._chips) + _raise_chips(state)
             ),  # RAISE
-            lambda: state.chips,  # FOLD
+            lambda: state._chips,  # FOLD
         ],
     )
 
     round_over, terminated, reward = _check_round_over(state, action)
     last_action = jax.lax.select(round_over, INVALID_ACTION, action)
     current_player = jax.lax.select(
-        round_over, state.first_player, 1 - state.current_player
+        round_over, state._first_player, 1 - state.current_player
     )
     raise_count = jax.lax.select(
-        round_over, jnp.int8(0), state.raise_count + jnp.int8(action == RAISE)
+        round_over, jnp.int8(0), state._raise_count + jnp.int8(action == RAISE)
     )
 
     reward *= jnp.min(chips)
 
     legal_action = jax.lax.switch(
         action,
         [
@@ -137,29 +134,29 @@
             lambda: jnp.bool_([0, 0, 0]),  # FOLD
         ],
     )
     legal_action = legal_action.at[RAISE].set(raise_count < MAX_RAISE)
 
     return state.replace(  # type:ignore
         current_player=current_player,
-        last_action=last_action,
+        _last_action=last_action,
         legal_action_mask=legal_action,
         terminated=terminated,
         reward=reward,
-        round=state.round + jnp.int8(round_over),
-        chips=chips,
-        raise_count=raise_count,
+        _round=state._round + jnp.int8(round_over),
+        _chips=chips,
+        _raise_count=raise_count,
     )
 
 
 def _check_round_over(state, action):
     round_over = (action == FOLD) | (
-        (state.last_action != INVALID_ACTION) & (action == CALL)
+        (state._last_action != INVALID_ACTION) & (action == CALL)
     )
-    terminated = round_over & (state.round == 1)
+    terminated = round_over & (state._round == 1)
 
     reward = jax.lax.select(
         terminated & (action == FOLD),
         jnp.float32([-1, -1]).at[1 - state.current_player].set(1),
         jnp.float32([0, 0]),
     )
     reward = jax.lax.select(
@@ -167,51 +164,53 @@
         _get_unit_reward(state),
         reward,
     )
     return round_over, terminated, reward
 
 
 def _get_unit_reward(state: State):
-    win_by_one_pair = state.cards[state.current_player] == state.cards[2]
-    lose_by_one_pair = state.cards[1 - state.current_player] == state.cards[2]
+    win_by_one_pair = state._cards[state.current_player] == state._cards[2]
+    lose_by_one_pair = (
+        state._cards[1 - state.current_player] == state._cards[2]
+    )
     win = win_by_one_pair | (
         ~lose_by_one_pair
         & (
-            state.cards[state.current_player]
-            > state.cards[1 - state.current_player]
+            state._cards[state.current_player]
+            > state._cards[1 - state.current_player]
         )
     )
     reward = jax.lax.select(
         win,
         jnp.float32([-1, -1]).at[state.current_player].set(1),
         jnp.float32([-1, -1]).at[1 - state.current_player].set(1),
     )
     return jax.lax.select(
-        state.cards[state.current_player]
-        == state.cards[1 - state.current_player],  # Draw
+        state._cards[state.current_player]
+        == state._cards[1 - state.current_player],  # Draw
         jnp.float32([0, 0]),
         reward,
     )
 
 
 def _raise_chips(state):
     """raise amounts is 2 in the first round and 4 in the second round."""
-    return (state.round + 1) * 2
+    return (state._round + 1) * 2
 
 
 def _observe(state: State, player_id) -> jnp.ndarray:
     """
     Index   Meaning
     0~2     J ~ K in hand
     3~5     J ~ K as public card
     6~19    0 ~ 13 chips for the current player
     20~33   0 ~ 13 chips for the opponent
     """
     obs = jnp.zeros(34, dtype=jnp.bool_)
-    obs = obs.at[state.cards[player_id]].set(TRUE)
+    obs = obs.at[state._cards[player_id]].set(TRUE)
     obs = jax.lax.select(
-        state.round == 1, obs.at[3 + state.cards[2]].set(TRUE), obs
+        state._round == 1, obs.at[3 + state._cards[2]].set(TRUE), obs
     )
-    obs = obs.at[6 + state.chips[player_id]].set(TRUE)
-    obs = obs.at[20 + state.chips[1 - player_id]].set(TRUE)
+    obs = obs.at[6 + state._chips[player_id]].set(TRUE)
+    obs = obs.at[20 + state._chips[1 - player_id]].set(TRUE)
 
     return obs
```

### Comparing `pgx-0.5.1/pgx/minatar/asterix.py` & `pgx-0.5.2/pgx/minatar/asterix.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,26 @@
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Asterix specific ---
-    player_x: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
-    player_y: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
-    entities: jnp.ndarray = jnp.ones((8, 4), dtype=jnp.int32) * INF
-    shot_timer: jnp.ndarray = jnp.ones(0, dtype=jnp.int32)
-    spawn_speed: jnp.ndarray = init_spawn_speed
-    spawn_timer: jnp.ndarray = init_spawn_speed
-    move_speed: jnp.ndarray = init_move_interval
-    move_timer: jnp.ndarray = init_move_interval
-    ramp_timer: jnp.ndarray = ramp_interval
-    ramp_index: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
-    terminal: jnp.ndarray = FALSE  # duplicated but necessary for checking the consistency to the original MinAtar
-    last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
+    _player_x: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
+    _player_y: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
+    _entities: jnp.ndarray = jnp.ones((8, 4), dtype=jnp.int32) * INF
+    _shot_timer: jnp.ndarray = jnp.ones(0, dtype=jnp.int32)
+    _spawn_speed: jnp.ndarray = init_spawn_speed
+    _spawn_timer: jnp.ndarray = init_spawn_speed
+    _move_speed: jnp.ndarray = init_move_interval
+    _move_timer: jnp.ndarray = init_move_interval
+    _ramp_timer: jnp.ndarray = ramp_interval
+    _ramp_index: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
+    _terminal: jnp.ndarray = FALSE  # duplicated but necessary for checking the consistency to the original MinAtar
+    _last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "minatar/asterix"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
@@ -89,15 +89,15 @@
         return State(_rng_key=key)  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
-        return state.replace(terminated=state.terminal)  # type: ignore
+        return state.replace(terminated=state._terminal)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -120,28 +120,28 @@
     action = jnp.int32(action)
     rng_key, rng0, rng1, rng2, rng3 = jax.random.split(state._rng_key, 5)
     state = state.replace(_rng_key=rng_key)  # type: ignore
 
     # sticky action
     action = jax.lax.cond(
         jax.random.uniform(rng0) < sticky_action_prob,
-        lambda: state.last_action,
+        lambda: state._last_action,
         lambda: action,
     )
 
     lr = jax.random.choice(rng1, jnp.array([True, False]))
     is_gold = jax.random.choice(
         rng2, jnp.array([True, False]), p=jnp.array([1 / 3, 2 / 3])
     )
     slots = jnp.zeros((8))
     slots = jax.lax.fori_loop(
         0,
         8,
         lambda i, x: jax.lax.cond(
-            state.entities[i, 0] == INF,
+            state._entities[i, 0] == INF,
             lambda: x.at[i].set(1),
             lambda: x,
         ),
         slots,
     )
     slots = jax.lax.cond(
         slots.sum() == 0, lambda: slots.at[0].set(1), lambda: slots
@@ -161,16 +161,16 @@
     state: State,
     action: jnp.ndarray,
     lr,
     is_gold,
     slot,
 ):
     return jax.lax.cond(
-        state.terminal,
-        lambda: state.replace(last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
+        state._terminal,
+        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
         lambda: _step_det_at_non_terminal(state, action, lr, is_gold, slot),
     )
 
 
 def _step_det_at_non_terminal(
     state: State,
     action: jnp.ndarray,
@@ -179,100 +179,106 @@
     slot: int,
 ):
     ramping: bool = True
     r = jnp.float32(0)
 
     # Spawn enemy if timer is up
     entities, spawn_timer = jax.lax.cond(
-        state.spawn_timer == 0,
+        state._spawn_timer == 0,
         lambda: (
-            _spawn_entity(state.entities, lr, is_gold, slot),
-            state.spawn_speed,
+            _spawn_entity(state._entities, lr, is_gold, slot),
+            state._spawn_speed,
         ),
-        lambda: (state.entities, state.spawn_timer),
+        lambda: (state._entities, state._spawn_timer),
     )
-    state = state.replace(entities=entities, spawn_timer=spawn_timer)  # type: ignore
+    state = state.replace(_entities=entities, _spawn_timer=spawn_timer)  # type: ignore
 
     # Resolve player action
     player_x, player_y = jax.lax.switch(
         action,
         [
-            lambda: (state.player_x, state.player_y),  # 0
+            lambda: (state._player_x, state._player_y),  # 0
             lambda: (
-                jax.lax.max(ZERO, state.player_x - 1),
-                state.player_y,
+                jax.lax.max(ZERO, state._player_x - 1),
+                state._player_y,
             ),  # 1
             lambda: (
-                state.player_x,
-                jax.lax.max(ONE, state.player_y - 1),
+                state._player_x,
+                jax.lax.max(ONE, state._player_y - 1),
             ),  # 2
             lambda: (
-                jax.lax.min(NINE, state.player_x + 1),
-                state.player_y,
+                jax.lax.min(NINE, state._player_x + 1),
+                state._player_y,
             ),  # 3
             lambda: (
-                state.player_x,
-                jax.lax.min(EIGHT, state.player_y + 1),
+                state._player_x,
+                jax.lax.min(EIGHT, state._player_y + 1),
             ),  # 4
-            lambda: (state.player_x, state.player_y),  # 5
+            lambda: (state._player_x, state._player_y),  # 5
         ],
     )
-    state = state.replace(player_x=player_x, player_y=player_y)  # type: ignore
+    state = state.replace(_player_x=player_x, _player_y=player_y)  # type: ignore
 
     # Update entities
     entities, player_x, player_y, r, terminal = jax.lax.fori_loop(
         0,
         8,
         lambda i, x: jax.lax.cond(
             entities[i, 0] == INF,
             lambda: x,
             lambda: _update_entities(x[0], x[1], x[2], x[3], x[4], i),
         ),
-        (state.entities, state.player_x, state.player_y, r, state.terminal),
+        (
+            state._entities,
+            state._player_x,
+            state._player_y,
+            r,
+            state._terminal,
+        ),
     )
-    state = state.replace(entities=entities, player_x=player_x, player_y=player_y, terminal=terminal)  # type: ignore
+    state = state.replace(_entities=entities, _player_x=player_x, _player_y=player_y, _terminal=terminal)  # type: ignore
 
     entities, r, terminal = jax.lax.cond(
-        state.move_timer == 0,
+        state._move_timer == 0,
         lambda: _update_entities_by_timer(
             entities, r, terminal, player_x, player_y
         ),
-        lambda: (state.entities, r, state.terminal),
+        lambda: (state._entities, r, state._terminal),
     )
-    state = state.replace(entities=entities, terminal=terminal)  # type: ignore
+    state = state.replace(_entities=entities, _terminal=terminal)  # type: ignore
     move_timer = jax.lax.cond(
-        state.move_timer == 0,
-        lambda: state.move_speed,
-        lambda: state.move_timer,
+        state._move_timer == 0,
+        lambda: state._move_speed,
+        lambda: state._move_timer,
     )
-    state = state.replace(move_timer=move_timer)  # type: ignore
+    state = state.replace(_move_timer=move_timer)  # type: ignore
 
     # Update various timers
-    state = state.replace(move_timer=state.move_timer - 1, spawn_timer=state.spawn_timer - 1)  # type: ignore
+    state = state.replace(_move_timer=state._move_timer - 1, _spawn_timer=state._spawn_timer - 1)  # type: ignore
 
     # Ramp difficulty if interval has elapsed
     spawn_speed, move_speed, ramp_timer, ramp_index = jax.lax.cond(
         ramping,
         lambda: _update_ramp(
-            state.spawn_speed,
-            state.move_speed,
-            state.ramp_timer,
-            state.ramp_index,
+            state._spawn_speed,
+            state._move_speed,
+            state._ramp_timer,
+            state._ramp_index,
         ),
         lambda: (
-            state.spawn_speed,
-            state.move_speed,
-            state.ramp_timer,
-            state.ramp_index,
+            state._spawn_speed,
+            state._move_speed,
+            state._ramp_timer,
+            state._ramp_index,
         ),
     )
-    state = state.replace(spawn_speed=spawn_speed, move_speed=move_speed, ramp_timer=ramp_timer, ramp_index=ramp_index)  # type: ignore
+    state = state.replace(_spawn_speed=spawn_speed, _move_speed=move_speed, _ramp_timer=ramp_timer, _ramp_index=ramp_index)  # type: ignore
 
     state = state.replace(  # type: ignore
-        reward=r[jnp.newaxis], last_action=action  # 1-d array
+        reward=r[jnp.newaxis], _last_action=action  # 1-d array
     )  # type: ignore
     return state
 
 
 # Spawn a new enemy or treasure at a random location with random direction (if all rows are filled do nothing)
 def _spawn_entity(entities, lr, is_gold, slot):
     x = jax.lax.cond(lr == 1, lambda: 0, lambda: 9)
@@ -362,35 +368,35 @@
     ramp_index += 1
     ramp_timer = ramp_interval
     return spawn_speed, move_speed, ramp_timer, ramp_index
 
 
 def _observe(state: State) -> jnp.ndarray:
     obs = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
-    obs = obs.at[state.player_y, state.player_x, 0].set(True)
+    obs = obs.at[state._player_y, state._player_x, 0].set(True)
     obs = jax.lax.fori_loop(
         0,
         8,
         lambda i, _obs: jax.lax.cond(
-            state.entities[i, 0] != INF,
+            state._entities[i, 0] != INF,
             lambda: _update_obs_by_entity(_obs, state, i),
             lambda: _obs,
         ),
         obs,
     )
     return obs
 
 
 def _update_obs_by_entity(obs, state, i):
-    c = jax.lax.cond(state.entities[i, 3], lambda: 3, lambda: 1)
-    obs = obs.at[state.entities[i, 1], state.entities[i, 0], c].set(True)
+    c = jax.lax.cond(state._entities[i, 3], lambda: 3, lambda: 1)
+    obs = obs.at[state._entities[i, 1], state._entities[i, 0], c].set(True)
     back_x = jax.lax.cond(
-        state.entities[i, 2],
-        lambda: state.entities[i, 0] - 1,
-        lambda: state.entities[i, 0] + 1,
+        state._entities[i, 2],
+        lambda: state._entities[i, 0] - 1,
+        lambda: state._entities[i, 0] + 1,
     )
     obs = jax.lax.cond(
         (0 <= back_x) & (back_x <= 9),
-        lambda: obs.at[state.entities[i, 1], back_x, 2].set(True),
+        lambda: obs.at[state._entities[i, 1], back_x, 2].set(True),
         lambda: obs,
     )
     return obs
```

### Comparing `pgx-0.5.1/pgx/minatar/breakout.py` & `pgx-0.5.2/pgx/minatar/breakout.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,26 +37,26 @@
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Breakout specific ---
-    ball_y: jnp.ndarray = THREE
-    ball_x: jnp.ndarray = ZERO
-    ball_dir: jnp.ndarray = TWO
-    pos: jnp.ndarray = FOUR
-    brick_map: jnp.ndarray = (
+    _ball_y: jnp.ndarray = THREE
+    _ball_x: jnp.ndarray = ZERO
+    _ball_dir: jnp.ndarray = TWO
+    _pos: jnp.ndarray = FOUR
+    _brick_map: jnp.ndarray = (
         jnp.zeros((10, 10), dtype=jnp.bool_).at[1:4, :].set(True)
     )
-    strike: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
-    last_x: jnp.ndarray = ZERO
-    last_y: jnp.ndarray = THREE
-    terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
-    last_action: jnp.ndarray = ZERO
+    _strike: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
+    _last_x: jnp.ndarray = ZERO
+    _last_y: jnp.ndarray = THREE
+    _terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
+    _last_action: jnp.ndarray = ZERO
 
     @property
     def env_id(self) -> v1.EnvId:
         return "minatar/breakout"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
@@ -90,15 +90,15 @@
         return _init(key)  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
-        return state.replace(terminated=state.terminal)  # type: ignore
+        return state.replace(terminated=state._terminal)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -119,41 +119,41 @@
     sticky_action_prob,
 ):
     action = jnp.int32(action)
     key, subkey = jax.random.split(state._rng_key)
     state = state.replace(_rng_key=key)  # type: ignore
     action = jax.lax.cond(
         jax.random.uniform(subkey) < sticky_action_prob,
-        lambda: state.last_action,
+        lambda: state._last_action,
         lambda: action,
     )
     return _step_det(state, action)
 
 
 def _init(rng: jnp.ndarray) -> State:
     ball_start = jax.random.choice(rng, 2)
     return _init_det(ball_start=ball_start)
 
 
 def _step_det(state: State, action: jnp.ndarray):
     return jax.lax.cond(
-        state.terminal,
-        lambda: state.replace(last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
+        state._terminal,
+        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
         lambda: _step_det_at_non_terminal(state, action),
     )
 
 
 def _step_det_at_non_terminal(state: State, action: jnp.ndarray):
-    ball_y = state.ball_y
-    ball_x = state.ball_x
-    ball_dir = state.ball_dir
-    pos = state.pos
-    brick_map = state.brick_map
-    strike = state.strike
-    terminal = state.terminal
+    ball_y = state._ball_y
+    ball_x = state._ball_x
+    ball_dir = state._ball_dir
+    pos = state._pos
+    brick_map = state._brick_map
+    strike = state._strike
+    terminal = state._terminal
 
     r = jnp.array(0, dtype=jnp.float32)
 
     pos = _apply_action(pos, action)
 
     # Update ball position
     last_x = ball_x
@@ -191,24 +191,24 @@
     )
 
     strike = jax.lax.cond(
         ~strike_toggle, lambda: jnp.zeros_like(strike), lambda: strike
     )
 
     state = state.replace(  # type: ignore
-        ball_y=new_y,
-        ball_x=new_x,
-        ball_dir=ball_dir,
-        pos=pos,
-        brick_map=brick_map,
-        strike=strike,
-        last_x=last_x,
-        last_y=last_y,
-        terminal=terminal,
-        last_action=action,
+        _ball_y=new_y,
+        _ball_x=new_x,
+        _ball_dir=ball_dir,
+        _pos=pos,
+        _brick_map=brick_map,
+        _strike=strike,
+        _last_x=last_x,
+        _last_y=last_y,
+        _terminal=terminal,
+        _last_action=action,
         reward=r[jnp.newaxis],
     )
     return state
 
 
 def _apply_action(pos, action):
     pos = jax.lax.cond(
@@ -282,18 +282,18 @@
 def _init_det(ball_start: jnp.ndarray) -> State:
     ball_x, ball_dir = jax.lax.switch(
         ball_start,
         [lambda: (ZERO, TWO), lambda: (NINE, THREE)],
     )
     last_x = ball_x
     return State(
-        ball_x=ball_x, ball_dir=ball_dir, last_x=last_x
+        _ball_x=ball_x, _ball_dir=ball_dir, _last_x=last_x
     )  # type: ignore
 
 
 def _observe(state: State) -> jnp.ndarray:
     obs = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
-    obs = obs.at[state.ball_y, state.ball_x, 1].set(True)
-    obs = obs.at[9, state.pos, 0].set(True)
-    obs = obs.at[state.last_y, state.last_x, 2].set(True)
-    obs = obs.at[:, :, 3].set(state.brick_map)
+    obs = obs.at[state._ball_y, state._ball_x, 1].set(True)
+    obs = obs.at[9, state._pos, 0].set(True)
+    obs = obs.at[state._last_y, state._last_x, 2].set(True)
+    obs = obs.at[:, :, 3].set(state._brick_map)
     return obs
```

### Comparing `pgx-0.5.1/pgx/minatar/freeway.py` & `pgx-0.5.2/pgx/minatar/freeway.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Freeway specific ---
-    cars: jnp.ndarray = jnp.zeros((8, 4), dtype=jnp.int32)
-    pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
-    move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
-    terminate_timer: jnp.ndarray = jnp.array(time_limit, dtype=jnp.int32)
-    terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
-    last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
+    _cars: jnp.ndarray = jnp.zeros((8, 4), dtype=jnp.int32)
+    _pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
+    _move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
+    _terminate_timer: jnp.ndarray = jnp.array(time_limit, dtype=jnp.int32)
+    _terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
+    _last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "minatar/freeway"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
@@ -80,15 +80,15 @@
         return _init(key)  # type: ignore
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
-        return state.replace(terminated=state.terminal)  # type: ignore
+        return state.replace(terminated=state._terminal)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -109,15 +109,15 @@
     sticky_action_prob,
 ):
     action = jnp.int32(action)
     key, subkey0, subkey1 = jax.random.split(state._rng_key, 3)
     state = state.replace(_rng_key=key)  # type: ignore
     action = jax.lax.cond(
         jax.random.uniform(subkey0) < sticky_action_prob,
-        lambda: state.last_action,
+        lambda: state._last_action,
         lambda: action,
     )
     speeds, directions = _random_speed_directions(subkey1)
     return _step_det(state, action, speeds=speeds, directions=directions)
 
 
 def _init(rng: jnp.ndarray) -> State:
@@ -128,32 +128,32 @@
 def _step_det(
     state: State,
     action: jnp.ndarray,
     speeds: jnp.ndarray,
     directions: jnp.ndarray,
 ):
     return jax.lax.cond(
-        state.terminal,
-        lambda: state.replace(last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
+        state._terminal,
+        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
         lambda: _step_det_at_non_terminal(state, action, speeds, directions),
     )
 
 
 def _step_det_at_non_terminal(
     state: State,
     action: jnp.ndarray,
     speeds: jnp.ndarray,
     directions: jnp.ndarray,
 ):
 
-    cars = state.cars
-    pos = state.pos
-    move_timer = state.move_timer
-    terminate_timer = state.terminate_timer
-    terminal = state.terminal
+    cars = state._cars
+    pos = state._pos
+    move_timer = state._move_timer
+    terminate_timer = state._terminate_timer
+    terminal = state._terminal
     last_action = action
 
     r = jnp.array(0, dtype=jnp.float32)
 
     move_timer, pos = jax.lax.cond(
         (action == 2) & (move_timer == 0),
         lambda: (player_speed, jax.lax.max(ZERO, pos - ONE)),
@@ -182,20 +182,20 @@
     move_timer = jax.lax.cond(
         move_timer > 0, lambda: move_timer - 1, lambda: move_timer
     )
     terminate_timer -= ONE
     terminal = terminate_timer < 0
 
     next_state = state.replace(  # type: ignore
-        cars=cars,
-        pos=pos,
-        move_timer=move_timer,
-        terminate_timer=terminate_timer,
-        terminal=terminal,
-        last_action=last_action,
+        _cars=cars,
+        _pos=pos,
+        _move_timer=move_timer,
+        _terminate_timer=terminate_timer,
+        _terminal=terminal,
+        _last_action=last_action,
         reward=r[jnp.newaxis],
     )
 
     return next_state
 
 
 def _update_cars(pos, cars):
@@ -225,15 +225,15 @@
     pos, cars = jax.lax.scan(_update_car, pos, cars)
 
     return pos, cars
 
 
 def _init_det(speeds: jnp.ndarray, directions: jnp.ndarray) -> State:
     cars = _randomize_cars(speeds, directions, initialize=True)
-    return State(cars=cars)  # type: ignore
+    return State(_cars=cars)  # type: ignore
 
 
 def _randomize_cars(
     speeds: jnp.ndarray,
     directions: jnp.ndarray,
     cars: jnp.ndarray = jnp.zeros((8, 4), dtype=int),
     initialize: bool = False,
@@ -262,18 +262,18 @@
         rng2, jnp.array([-1, 1], dtype=jnp.int32), [8]
     )
     return speeds, directions
 
 
 def _observe(state: State) -> jnp.ndarray:
     obs = jnp.zeros((10, 10, 7), dtype=jnp.bool_)
-    obs = obs.at[state.pos, 4, 0].set(TRUE)
+    obs = obs.at[state._pos, 4, 0].set(TRUE)
 
     def _update_obs(i, _obs):
-        car = state.cars[i]
+        car = state._cars[i]
         _obs = _obs.at[car[1], car[0], 1].set(TRUE)
         back_x = jax.lax.cond(
             car[3] > 0, lambda: car[0] - 1, lambda: car[0] + 1
         )
         back_x = jax.lax.cond(back_x < 0, lambda: NINE, lambda: back_x)
         back_x = jax.lax.cond(back_x > 9, lambda: ZERO, lambda: back_x)
         trail = jax.lax.abs(car[3]) + 1
```

### Comparing `pgx-0.5.1/pgx/minatar/seaquest.py` & `pgx-0.5.2/pgx/minatar/seaquest.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,35 +39,35 @@
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Seaquest specific ---
-    oxygen: jnp.ndarray = MAX_OXYGEN
-    diver_count: jnp.ndarray = ZERO
-    sub_x: jnp.ndarray = jnp.int32(5)
-    sub_y: jnp.ndarray = ZERO
-    sub_or: jnp.ndarray = FALSE
-    f_bullets: jnp.ndarray = -jnp.ones((5, 3), dtype=jnp.int32)
-    e_bullets: jnp.ndarray = -jnp.ones(
+    _oxygen: jnp.ndarray = MAX_OXYGEN
+    _diver_count: jnp.ndarray = ZERO
+    _sub_x: jnp.ndarray = jnp.int32(5)
+    _sub_y: jnp.ndarray = ZERO
+    _sub_or: jnp.ndarray = FALSE
+    _f_bullets: jnp.ndarray = -jnp.ones((5, 3), dtype=jnp.int32)
+    _e_bullets: jnp.ndarray = -jnp.ones(
         (25, 3), dtype=jnp.int32
     )  # <= 1 per each sub
-    e_fish: jnp.ndarray = -jnp.ones((25, 4), dtype=jnp.int32)  # <= 19
-    e_subs: jnp.ndarray = -jnp.ones((25, 5), dtype=jnp.int32)  # <= 19
-    divers: jnp.ndarray = -jnp.ones((5, 4), dtype=jnp.int32)  # <= 2
-    e_spawn_speed: jnp.ndarray = INIT_SPAWN_SPEED
-    e_spawn_timer: jnp.ndarray = INIT_SPAWN_SPEED
-    d_spawn_timer: jnp.ndarray = DIVER_SPAWN_SPEED
-    move_speed: jnp.ndarray = INIT_MOVE_INTERVAL
-    ramp_index: jnp.ndarray = ZERO
-    shot_timer: jnp.ndarray = ZERO
-    surface: jnp.ndarray = TRUE
-    terminal: jnp.ndarray = FALSE
-    last_action: jnp.ndarray = ZERO
+    _e_fish: jnp.ndarray = -jnp.ones((25, 4), dtype=jnp.int32)  # <= 19
+    _e_subs: jnp.ndarray = -jnp.ones((25, 5), dtype=jnp.int32)  # <= 19
+    _divers: jnp.ndarray = -jnp.ones((5, 4), dtype=jnp.int32)  # <= 2
+    _e_spawn_speed: jnp.ndarray = INIT_SPAWN_SPEED
+    _e_spawn_timer: jnp.ndarray = INIT_SPAWN_SPEED
+    _d_spawn_timer: jnp.ndarray = DIVER_SPAWN_SPEED
+    _move_speed: jnp.ndarray = INIT_MOVE_INTERVAL
+    _ramp_index: jnp.ndarray = ZERO
+    _shot_timer: jnp.ndarray = ZERO
+    _surface: jnp.ndarray = TRUE
+    _terminal: jnp.ndarray = FALSE
+    _last_action: jnp.ndarray = ZERO
 
     @property
     def env_id(self) -> v1.EnvId:
         return "minatar/seaquest"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
@@ -101,15 +101,15 @@
         return _init_det()
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
-        return state.replace(terminated=state.terminal)  # type: ignore
+        return state.replace(terminated=state._terminal)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -132,15 +132,15 @@
     key, subkey = jax.random.split(state._rng_key)
     state = state.replace(_rng_key=key)  # type: ignore
     rngs = jax.random.split(subkey, 6)
     action = jnp.int32(action)
     # sticky action
     action = jax.lax.cond(
         jax.random.uniform(rngs[0]) < sticky_action_prob,
-        lambda: state.last_action,
+        lambda: state._last_action,
         lambda: action,
     )
     enemy_lr = jax.random.choice(rngs[1], jnp.array([True, False]))
     is_sub = jax.random.choice(
         rngs[2], jnp.array([True, False]), p=jnp.array([1 / 3, 2 / 3])
     )
     enemy_y = jax.random.choice(rngs[3], jnp.arange(1, 9))
@@ -157,16 +157,16 @@
     enemy_lr,
     is_sub,
     enemy_y,
     diver_lr,
     diver_y,
 ):
     return lax.cond(
-        state.terminal,
-        lambda: state.replace(last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
+        state._terminal,
+        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
         lambda: _step_det_at_non_terminal(
             state, action, enemy_lr, is_sub, enemy_y, diver_lr, diver_y
         ),
     )
 
 
 def _step_det_at_non_terminal(
@@ -176,32 +176,32 @@
     is_sub,
     enemy_y,
     diver_lr,
     diver_y,
 ):
     ramping = TRUE
 
-    oxygen = state.oxygen
-    diver_count = state.diver_count
-    sub_x = state.sub_x
-    sub_y = state.sub_y
-    sub_or = state.sub_or
-    f_bullets = state.f_bullets
-    e_bullets = state.e_bullets
-    e_fish = state.e_fish
-    e_subs = state.e_subs
-    divers = state.divers
-    e_spawn_speed = state.e_spawn_speed
-    e_spawn_timer = state.e_spawn_timer
-    d_spawn_timer = state.d_spawn_timer
-    move_speed = state.move_speed
-    ramp_index = state.ramp_index
-    shot_timer = state.shot_timer
-    surface = state.surface
-    terminal = state.terminal
+    oxygen = state._oxygen
+    diver_count = state._diver_count
+    sub_x = state._sub_x
+    sub_y = state._sub_y
+    sub_or = state._sub_or
+    f_bullets = state._f_bullets
+    e_bullets = state._e_bullets
+    e_fish = state._e_fish
+    e_subs = state._e_subs
+    divers = state._divers
+    e_spawn_speed = state._e_spawn_speed
+    e_spawn_timer = state._e_spawn_timer
+    d_spawn_timer = state._d_spawn_timer
+    move_speed = state._move_speed
+    ramp_index = state._ramp_index
+    shot_timer = state._shot_timer
+    surface = state._surface
+    terminal = state._terminal
 
     r = jnp.float32(0)
 
     # Spawn enemy if timer is up
     e_subs, e_fish = lax.cond(
         e_spawn_timer == 0,
         lambda: _spawn_enemy(
@@ -281,33 +281,33 @@
             e_spawn_speed,
             ramp_index,
         ),
     )
     r += _r
 
     state = state.replace(  # type: ignore
-        oxygen=oxygen,
-        diver_count=diver_count,
-        sub_x=sub_x,
-        sub_y=sub_y,
-        sub_or=sub_or,
-        f_bullets=f_bullets,
-        e_bullets=e_bullets,
-        e_fish=e_fish,
-        e_subs=e_subs,
-        divers=divers,
-        e_spawn_speed=e_spawn_speed,
-        e_spawn_timer=e_spawn_timer,
-        d_spawn_timer=d_spawn_timer,
-        move_speed=move_speed,
-        ramp_index=ramp_index,
-        shot_timer=shot_timer,
-        surface=surface,
-        terminal=terminal,
-        last_action=action,
+        _oxygen=oxygen,
+        _diver_count=diver_count,
+        _sub_x=sub_x,
+        _sub_y=sub_y,
+        _sub_or=sub_or,
+        _f_bullets=f_bullets,
+        _e_bullets=e_bullets,
+        _e_fish=e_fish,
+        _e_subs=e_subs,
+        _divers=divers,
+        _e_spawn_speed=e_spawn_speed,
+        _e_spawn_timer=e_spawn_timer,
+        _d_spawn_timer=d_spawn_timer,
+        _move_speed=move_speed,
+        _ramp_index=ramp_index,
+        _shot_timer=shot_timer,
+        _surface=surface,
+        _terminal=terminal,
+        _last_action=action,
         reward=r[jnp.newaxis],
     )
     return state
 
 
 def find_ix(arr):
     ix = lax.while_loop(lambda i: arr[i][0] != -1, lambda i: i + 1, 0)
@@ -735,55 +735,55 @@
         jnp.array([x, diver_y, diver_lr, DIVER_MOVE_INTERVAL], dtype=jnp.int32)
     )
     return divers
 
 
 def _observe(state: State) -> jnp.ndarray:
     obs = jnp.zeros((10, 10, 10), dtype=jnp.bool_)
-    obs = obs.at[state.sub_y, state.sub_x, 0].set(TRUE)
+    obs = obs.at[state._sub_y, state._sub_x, 0].set(TRUE)
     back_x = lax.cond(
-        state.sub_or, lambda: state.sub_x - 1, lambda: state.sub_x + 1
+        state._sub_or, lambda: state._sub_x - 1, lambda: state._sub_x + 1
     )
-    obs = obs.at[state.sub_y, back_x, 1].set(TRUE)
-    oxygen_guage = state.oxygen * 10 // MAX_OXYGEN
+    obs = obs.at[state._sub_y, back_x, 1].set(TRUE)
+    oxygen_guage = state._oxygen * 10 // MAX_OXYGEN
     # hotfix to align to original minatar
     oxygen_guage = lax.cond(
-        state.oxygen < 0, lambda: jnp.int32(9), lambda: oxygen_guage
+        state._oxygen < 0, lambda: jnp.int32(9), lambda: oxygen_guage
     )
     obs = lax.fori_loop(
         jnp.int32(0),
         oxygen_guage,
         lambda i, _obs: _obs.at[9, i, 7].set(TRUE),
         obs,
     )
     obs = lax.fori_loop(
-        9 - state.diver_count,
+        9 - state._diver_count,
         jnp.int32(9),
         lambda i, _obs: _obs.at[9, i, 8].set(TRUE),
         obs,
     )
     obs = lax.fori_loop(
         0,
         5,
         lambda i, _obs: lax.cond(
-            state.f_bullets[i][0] >= 0,
+            state._f_bullets[i][0] >= 0,
             lambda: _obs.at[
-                state.f_bullets[i][1], state.f_bullets[i][0], 2
+                state._f_bullets[i][1], state._f_bullets[i][0], 2
             ].set(TRUE),
             lambda: _obs,
         ),
         obs,
     )
     obs = lax.fori_loop(
         0,
         25,
         lambda i, _obs: lax.cond(
-            state.e_bullets[i][0] >= 0,
+            state._e_bullets[i][0] >= 0,
             lambda: _obs.at[
-                state.e_bullets[i][1], state.e_bullets[i][0], 4
+                state._e_bullets[i][1], state._e_bullets[i][0], 4
             ].set(TRUE),
             lambda: _obs,
         ),
         obs,
     )
 
     def set_e_fish(_obs, fish):
@@ -796,16 +796,16 @@
         )
         return _obs
 
     obs = lax.fori_loop(
         0,
         25,
         lambda i, _obs: lax.cond(
-            state.e_fish[i][0] >= 0,
-            lambda: set_e_fish(_obs, state.e_fish[i]),
+            state._e_fish[i][0] >= 0,
+            lambda: set_e_fish(_obs, state._e_fish[i]),
             lambda: _obs,
         ),
         obs,
     )
 
     def set_e_subs(_obs, sub):
         _obs = _obs.at[sub[1], sub[0], 6].set(TRUE)
@@ -817,16 +817,16 @@
         )
         return _obs
 
     obs = lax.fori_loop(
         0,
         25,
         lambda i, _obs: lax.cond(
-            state.e_subs[i][0] >= 0,
-            lambda: set_e_subs(_obs, state.e_subs[i]),
+            state._e_subs[i][0] >= 0,
+            lambda: set_e_subs(_obs, state._e_subs[i]),
             lambda: _obs,
         ),
         obs,
     )
 
     def set_divers(_obs, diver):
         _obs = _obs.at[diver[1], diver[0], 9].set(TRUE)
@@ -838,16 +838,16 @@
         )
         return _obs
 
     obs = lax.fori_loop(
         0,
         5,
         lambda i, _obs: lax.cond(
-            state.divers[i][0] >= 0,
-            lambda: set_divers(_obs, state.divers[i]),
+            state._divers[i][0] >= 0,
+            lambda: set_divers(_obs, state._divers[i]),
             lambda: _obs,
         ),
         obs,
     )
 
     return obs
```

### Comparing `pgx-0.5.1/pgx/minatar/space_invaders.py` & `pgx-0.5.2/pgx/minatar/space_invaders.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,28 +35,28 @@
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar SpaceInvaders specific ---
-    pos: jnp.ndarray = jnp.int32(5)
-    f_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
-    e_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
-    alien_map: jnp.ndarray = (
+    _pos: jnp.ndarray = jnp.int32(5)
+    _f_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
+    _e_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
+    _alien_map: jnp.ndarray = (
         jnp.zeros((10, 10), dtype=jnp.bool_).at[0:4, 2:8].set(TRUE)
     )
-    alien_dir: jnp.ndarray = jnp.int32(-1)
-    enemy_move_interval: jnp.ndarray = ENEMY_MOVE_INTERVAL
-    alien_move_timer: jnp.ndarray = ENEMY_MOVE_INTERVAL
-    alien_shot_timer: jnp.ndarray = ENEMY_SHOT_INTERVAL
-    ramp_index: jnp.ndarray = jnp.int32(0)
-    shot_timer: jnp.ndarray = jnp.int32(0)
-    terminal: jnp.ndarray = FALSE
-    last_action: jnp.ndarray = jnp.int32(0)
+    _alien_dir: jnp.ndarray = jnp.int32(-1)
+    _enemy_move_interval: jnp.ndarray = ENEMY_MOVE_INTERVAL
+    _alien_move_timer: jnp.ndarray = ENEMY_MOVE_INTERVAL
+    _alien_shot_timer: jnp.ndarray = ENEMY_SHOT_INTERVAL
+    _ramp_index: jnp.ndarray = jnp.int32(0)
+    _shot_timer: jnp.ndarray = jnp.int32(0)
+    _terminal: jnp.ndarray = FALSE
+    _last_action: jnp.ndarray = jnp.int32(0)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "minatar/space_invaders"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
@@ -90,15 +90,15 @@
         return _init_det()
 
     def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
-        return state.replace(terminated=state.terminal)  # type: ignore
+        return state.replace(terminated=state._terminal)  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
     def id(self) -> v1.EnvId:
@@ -119,71 +119,71 @@
     sticky_action_prob,
 ):
     action = jnp.int32(action)
     key, subkey = jax.random.split(state._rng_key)
     state = state.replace(_rng_key=key)  # type: ignore
     action = jax.lax.cond(
         jax.random.uniform(subkey) < sticky_action_prob,
-        lambda: state.last_action,
+        lambda: state._last_action,
         lambda: action,
     )
     return _step_det(state, action)
 
 
 def _observe(state: State) -> jnp.ndarray:
     obs = jnp.zeros((10, 10, 6), dtype=jnp.bool_)
-    obs = obs.at[9, state.pos, 0].set(TRUE)
-    obs = obs.at[:, :, 1].set(state.alien_map)
+    obs = obs.at[9, state._pos, 0].set(TRUE)
+    obs = obs.at[:, :, 1].set(state._alien_map)
     obs = obs.at[:, :, 2].set(
         lax.cond(
-            state.alien_dir < 0,
-            lambda: state.alien_map,
-            lambda: jnp.zeros_like(state.alien_map),
+            state._alien_dir < 0,
+            lambda: state._alien_map,
+            lambda: jnp.zeros_like(state._alien_map),
         )
     )
     obs = obs.at[:, :, 3].set(
         lax.cond(
-            state.alien_dir < 0,
-            lambda: jnp.zeros_like(state.alien_map),
-            lambda: state.alien_map,
+            state._alien_dir < 0,
+            lambda: jnp.zeros_like(state._alien_map),
+            lambda: state._alien_map,
         )
     )
-    obs = obs.at[:, :, 4].set(state.f_bullet_map)
-    obs = obs.at[:, :, 5].set(state.e_bullet_map)
+    obs = obs.at[:, :, 4].set(state._f_bullet_map)
+    obs = obs.at[:, :, 5].set(state._e_bullet_map)
     return obs
 
 
 def _step_det(
     state: State,
     action: jnp.ndarray,
 ):
     return lax.cond(
-        state.terminal,
-        lambda: state.replace(last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
+        state._terminal,
+        lambda: state.replace(_last_action=action, reward=jnp.zeros_like(state.reward)),  # type: ignore
         lambda: _step_det_at_non_terminal(state, action),
     )
 
 
 def _step_det_at_non_terminal(
     state: State,
     action: jnp.ndarray,
 ):
     r = jnp.float32(0)
 
-    pos = state.pos
-    f_bullet_map = state.f_bullet_map
-    e_bullet_map = state.e_bullet_map
-    alien_map = state.alien_map
-    alien_dir = state.alien_dir
-    enemy_move_interval = state.enemy_move_interval
-    alien_move_timer = state.alien_move_timer
-    alien_shot_timer = state.alien_shot_timer
-    ramp_index = state.ramp_index
-    shot_timer = state.shot_timer
-    terminal = state.terminal
+    pos = state._pos
+    f_bullet_map = state._f_bullet_map
+    e_bullet_map = state._e_bullet_map
+    alien_map = state._alien_map
+    alien_dir = state._alien_dir
+    enemy_move_interval = state._enemy_move_interval
+    alien_move_timer = state._alien_move_timer
+    alien_shot_timer = state._alien_shot_timer
+    ramp_index = state._ramp_index
+    shot_timer = state._shot_timer
+    terminal = state._terminal
 
     # Resolve player action
     # action_map = ['n','l','u','r','d','f']
     pos, f_bullet_map, shot_timer = _resole_action(
         pos, f_bullet_map, shot_timer, action
     )
 
@@ -240,26 +240,26 @@
     alien_map = lax.cond(
         is_enemy_zero,
         lambda: alien_map.at[0:4, 2:8].set(TRUE),
         lambda: alien_map,
     )
 
     return state.replace(  # type: ignore
-        pos=pos,
-        f_bullet_map=f_bullet_map,
-        e_bullet_map=e_bullet_map,
-        alien_map=alien_map,
-        alien_dir=alien_dir,
-        enemy_move_interval=enemy_move_interval,
-        alien_move_timer=alien_move_timer,
-        alien_shot_timer=alien_shot_timer,
-        ramp_index=ramp_index,
-        shot_timer=shot_timer,
-        terminal=terminal,
-        last_action=action,
+        _pos=pos,
+        _f_bullet_map=f_bullet_map,
+        _e_bullet_map=e_bullet_map,
+        _alien_map=alien_map,
+        _alien_dir=alien_dir,
+        _enemy_move_interval=enemy_move_interval,
+        _alien_move_timer=alien_move_timer,
+        _alien_shot_timer=alien_shot_timer,
+        _ramp_index=ramp_index,
+        _shot_timer=shot_timer,
+        _terminal=terminal,
+        _last_action=action,
         reward=r[jnp.newaxis],
     )
 
 
 def _resole_action(pos, f_bullet_map, shot_timer, action):
     f_bullet_map = lax.cond(
         (action == 5) & (shot_timer == 0),
```

### Comparing `pgx-0.5.1/pgx/minatar/utils.py` & `pgx-0.5.2/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/pgx/othello.py` & `pgx-0.5.2/pgx/othello.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,26 +29,26 @@
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(64 + 1, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Othello specific ---
-    turn: jnp.ndarray = jnp.int8(0)
+    _turn: jnp.ndarray = jnp.int8(0)
     # 8x8 board
     # [[ 0,  1,  2,  3,  4,  5,  6,  7],
     #  [ 8,  9, 10, 11, 12, 13, 14, 15],
     #  [16, 17, 18, 19, 20, 21, 22, 23],
     #  [24, 25, 26, 27, 28, 29, 30, 31],
     #  [32, 33, 34, 35, 36, 37, 38, 39],
     #  [40, 41, 42, 43, 44, 45, 46, 47],
     #  [48, 49, 50, 51, 52, 53, 54, 55],
     #  [56, 57, 58, 59, 60, 61, 62, 63]]
-    board: jnp.ndarray = jnp.zeros(64, jnp.int8)  # -1(opp), 0(empty), 1(self)
-    passed: jnp.ndarray = FALSE
+    _board: jnp.ndarray = jnp.zeros(64, jnp.int8)  # -1(opp), 0(empty), 1(self)
+    _passed: jnp.ndarray = FALSE
 
     @property
     def env_id(self) -> v1.EnvId:
         return "othello"
 
 
 class Othello(v1.Env):
@@ -105,15 +105,15 @@
 
 
 def _init(rng: jax.random.KeyArray) -> State:
     rng, subkey = jax.random.split(rng)
     current_player = jnp.int8(jax.random.bernoulli(subkey))
     return State(
         current_player=current_player,
-        board=jnp.zeros(64, dtype=jnp.int8)
+        _board=jnp.zeros(64, dtype=jnp.int8)
         .at[28]
         .set(1)
         .at[35]
         .set(1)
         .at[27]
         .set(-1)
         .at[36]
@@ -127,15 +127,15 @@
         .set(TRUE)
         .at[44]
         .set(TRUE),
     )  # type:ignore
 
 
 def _step(state, action):
-    board = state.board
+    board = state._board
     my = board > 0
     opp = board < 0
 
     # updates at out-of-bounds indices will be skipped:
     # https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#out-of-bounds-indexing
     # Therefore, there is no need to ignore the path action
     pos = jnp.zeros(64, dtype=jnp.bool_).at[action].set(TRUE)
@@ -178,31 +178,31 @@
         0, 8, _make_legal, jnp.zeros(64, dtype=jnp.bool_)
     )
 
     reward, terminated = jax.lax.cond(
         (
             (jnp.count_nonzero(my | opp) == 64)
             | ~opp.any()
-            | (state.passed & (action == 64))
+            | (state._passed & (action == 64))
         ),
         lambda: (_get_reward(my, opp, state.current_player), TRUE),
         lambda: (jnp.zeros(2, jnp.float32), FALSE),
     )
 
     return state.replace(
         current_player=1 - state.current_player,
-        turn=1 - state.turn,
+        _turn=1 - state._turn,
         legal_action_mask=state.legal_action_mask.at[:64]
         .set(legal_action)
         .at[64]
         .set(~legal_action.any()),
         reward=reward,
         terminated=terminated,
-        board=-jnp.where(jnp.int8(opp), -1, jnp.int8(my)),
-        passed=action == 64,
+        _board=-jnp.where(jnp.int8(opp), -1, jnp.int8(my)),
+        _passed=action == 64,
     )
 
 
 def _check_line(pos, opp, shift, mask):
     _opp = opp & mask
     result = _opp & jnp.roll(pos, shift)
     result |= _opp & jnp.roll(result, shift)
@@ -225,21 +225,21 @@
         lambda: jnp.float32([-1, -1]).at[winner].set(1),
     )
 
 
 def _observe(state, player_id) -> jnp.ndarray:
     board = jax.lax.cond(
         player_id == state.current_player,
-        lambda: state.board.reshape((8, 8)),
-        lambda: (state.board * -1).reshape((8, 8)),
+        lambda: state._board.reshape((8, 8)),
+        lambda: (state._board * -1).reshape((8, 8)),
     )
 
     def make(color):
         return board * color > 0
 
     return jnp.stack(jax.vmap(make)(jnp.int8([1, -1])), -1)
 
 
 def _get_abs_board(state):
     return jax.lax.cond(
-        state.turn == 0, lambda: state.board, lambda: state.board * -1
+        state._turn == 0, lambda: state._board, lambda: state._board * -1
     )
```

### Comparing `pgx-0.5.1/pgx/play2048.py` & `pgx-0.5.2/pgx/play2048.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     reward: jnp.ndarray = jnp.float32([0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- 2048 specific ---
-    turn: jnp.ndarray = jnp.int8(0)
+    _turn: jnp.ndarray = jnp.int8(0)
     # 4x4 board
     # [[ 0,  1,  2,  3],
     #  [ 4,  5,  6,  7],
     #  [ 8,  9, 10, 11],
     #  [12, 13, 14, 15]]
-    board: jnp.ndarray = jnp.zeros(16, jnp.int8)
+    _board: jnp.ndarray = jnp.zeros(16, jnp.int8)
     #  Board is expressed as a power of 2.
     # e.g.
     # [[ 0,  0,  1,  1],
     #  [ 1,  0,  1,  2],
     #  [ 3,  3,  6,  7],
     #  [ 3,  6,  7,  9]]
     # means
@@ -89,20 +89,20 @@
         return 1
 
 
 def _init(rng: jax.random.KeyArray) -> State:
     rng1, rng2 = jax.random.split(rng)
     board = _add_random_num(jnp.zeros((4, 4), jnp.int8), rng1)
     board = _add_random_num(board, rng2)
-    return State(board=board.ravel())  # type:ignore
+    return State(_board=board.ravel())  # type:ignore
 
 
 def _step(state: State, action):
     """action: 0(left), 1(up), 2(right), 3(down)"""
-    board_2d = state.board.reshape((4, 4))
+    board_2d = state._board.reshape((4, 4))
     board_2d = jax.lax.switch(
         action,
         [
             lambda: board_2d,
             lambda: jnp.rot90(board_2d, 1),
             lambda: jnp.rot90(board_2d, 2),
             lambda: jnp.rot90(board_2d, 3),
@@ -131,25 +131,25 @@
                 jnp.rot90(board_2d, 3),
             ]
         )
     )
 
     return state.replace(  # type:ignore
         _rng_key=_rng_key,
-        board=board_2d.ravel(),
+        _board=board_2d.ravel(),
         reward=jnp.float32([reward.sum()]),
         legal_action_mask=legal_action.ravel(),
         terminated=~legal_action.any(),
     )
 
 
 def _observe(state: State, player_id) -> jnp.ndarray:
     obs = jnp.zeros((16, 31), dtype=jnp.bool_)
     obs = jax.lax.fori_loop(
-        0, 16, lambda i, obs: obs.at[i, state.board[i]].set(TRUE), obs
+        0, 16, lambda i, obs: obs.at[i, state._board[i]].set(TRUE), obs
     )
     return obs.reshape((4, 4, 31))
 
 
 def _add_random_num(board_2d, key):
     """Add 2 or 4 to the empty space on the board.
     2 appears 90% of the time, and 4 appears 10% of the time.
@@ -233,9 +233,9 @@
 
     can_slide = jax.vmap(_can_slide)(board_2d).any()
     return can_slide
 
 
 # only for debug
 def show(state):
-    board = jnp.array([0 if i == 0 else 2**i for i in state.board])
+    board = jnp.array([0 if i == 0 else 2**i for i in state._board])
     print(board.reshape((4, 4)))
```

### Comparing `pgx-0.5.1/pgx/shogi.py` & `pgx-0.5.2/pgx/shogi.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,45 +76,45 @@
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # (27 * 81,)
     observation: jnp.ndarray = jnp.zeros((119, 9, 9), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Shogi specific ---
-    turn: jnp.ndarray = jnp.int8(0)  # 0 or 1
-    piece_board: jnp.ndarray = INIT_PIECE_BOARD  # (81,) 後手のときにはflipする
-    hand: jnp.ndarray = jnp.zeros((2, 7), dtype=jnp.int8)  # 後手のときにはflipする
+    _turn: jnp.ndarray = jnp.int8(0)  # 0 or 1
+    _board: jnp.ndarray = INIT_PIECE_BOARD  # (81,) 後手のときにはflipする
+    _hand: jnp.ndarray = jnp.zeros((2, 7), dtype=jnp.int8)  # 後手のときにはflipする
     # cache
     # Redundant information used only in _is_checked for speeding-up
-    cache_m2b: jnp.ndarray = -jnp.ones(8, dtype=jnp.int8)
-    cache_king: jnp.ndarray = jnp.int32(44)
+    _cache_m2b: jnp.ndarray = -jnp.ones(8, dtype=jnp.int8)
+    _cache_king: jnp.ndarray = jnp.int32(44)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "shogi"
 
     @staticmethod
     def _from_board(turn, piece_board: jnp.ndarray, hand: jnp.ndarray):
         """Mainly for debugging purpose.
         terminated, reward, and current_player are not changed"""
-        state = State(turn=turn, piece_board=piece_board, hand=hand)  # type: ignore
+        state = State(_turn=turn, _board=piece_board, _hand=hand)  # type: ignore
         # fmt: off
         state = jax.lax.cond(turn % 2 == 1, lambda: _flip(state), lambda: state)
         # fmt: on
         return state.replace(legal_action_mask=_legal_action_mask(state))  # type: ignore
 
     @staticmethod
     def _from_sfen(sfen):
         turn, pb, hand, step_count = _from_sfen(sfen)
         return jax.jit(State._from_board)(turn, pb, hand).replace(  # type: ignore
             _step_count=jnp.int32(step_count)
         )
 
     def _to_sfen(self):
-        state = self if self.turn % 2 == 0 else _flip(self)
+        state = self if self._turn % 2 == 0 else _flip(self)
         return _to_sfen(state)
 
 
 class Shogi(v1.Env):
     def __init__(self, max_termination_steps: int = 1000):
         super().__init__()
         self.max_termination_steps = max_termination_steps
@@ -212,25 +212,23 @@
         """
         action = jnp.int32(action)
         direction, to = jnp.int8(action // 81), jnp.int8(action % 81)
         is_drop = direction >= 20
         is_promotion = (10 <= direction) & (direction < 20)
         # LEGAL_FROM_IDX[UP, 19] = [20, 21, ... -1]
         legal_from_idx = LEGAL_FROM_IDX[direction % 10, to]  # (81,)
-        from_cand = state.piece_board[legal_from_idx]  # (8,)
+        from_cand = state._board[legal_from_idx]  # (8,)
         mask = (
             (legal_from_idx >= 0)
             & (PAWN <= from_cand)
             & (from_cand < OPP_PAWN)
         )
         i = jnp.argmax(mask)
         from_ = jax.lax.select(is_drop, 0, legal_from_idx[i])
-        piece = jax.lax.select(
-            is_drop, direction - 20, state.piece_board[from_]
-        )
+        piece = jax.lax.select(is_drop, direction - 20, state._board[from_])
         return Action(is_drop=is_drop, piece=piece, to=to, from_=from_, is_promotion=is_promotion)  # type: ignore
 
 
 def _init_board():
     """Initialize Shogi State."""
     return State()
 
@@ -239,15 +237,15 @@
     a = Action._from_dlshogi_action(state, action)
     # apply move/drop action
     state = jax.lax.cond(a.is_drop, _step_drop, _step_move, *(state, a))
     # flip state
     state = _flip(state)
     state = state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
-        turn=(state.turn + 1) % 2,
+        _turn=(state._turn + 1) % 2,
     )
     legal_action_mask = _legal_action_mask(state)
     terminated = ~legal_action_mask.any()
     # fmt: off
     reward = jax.lax.select(
         terminated,
         jnp.ones(2, dtype=jnp.float32).at[state.current_player].set(-1),
@@ -258,49 +256,49 @@
         legal_action_mask=legal_action_mask,
         terminated=terminated,
         reward=reward,
     )
 
 
 def _step_move(state: State, action: Action) -> State:
-    pb = state.piece_board
+    pb = state._board
     # remove piece from the original position
     pb = pb.at[action.from_].set(EMPTY)
     # capture the opponent if exists
     captured = pb[action.to]  # suppose >= OPP_PAWN, -1 if EMPTY
     hand = jax.lax.cond(
         captured == EMPTY,
-        lambda: state.hand,
+        lambda: state._hand,
         # add captured piece to my hand after
         #   (1) tuning opp piece into mine by (x + 14) % 28, and
         #   (2) filtering promoted piece by x % 8
-        lambda: state.hand.at[0, ((captured + 14) % 28) % 8].add(1),
+        lambda: state._hand.at[0, ((captured + 14) % 28) % 8].add(1),
     )
     # promote piece
     piece = jax.lax.select(action.is_promotion, action.piece + 8, action.piece)
     # set piece to the target position
     pb = pb.at[action.to].set(piece)
     # apply piece moves
-    return state.replace(piece_board=pb, hand=hand)  # type: ignore
+    return state.replace(_board=pb, _hand=hand)  # type: ignore
 
 
 def _step_drop(state: State, action: Action) -> State:
     # add piece to board
-    pb = state.piece_board.at[action.to].set(action.piece)
+    pb = state._board.at[action.to].set(action.piece)
     # remove piece from hand
-    hand = state.hand.at[0, action.piece].add(-1)
-    return state.replace(piece_board=pb, hand=hand)  # type: ignore
+    hand = state._hand.at[0, action.piece].add(-1)
+    return state.replace(_board=pb, _hand=hand)  # type: ignore
 
 
 def _set_cache(state: State):
     return state.replace(  # type: ignore
-        cache_m2b=jnp.nonzero(
-            jax.vmap(_is_major_piece)(state.piece_board), size=8, fill_value=-1
+        _cache_m2b=jnp.nonzero(
+            jax.vmap(_is_major_piece)(state._board), size=8, fill_value=-1
         )[0],
-        cache_king=jnp.argmin(jnp.abs(state.piece_board - KING)),
+        _cache_king=jnp.argmin(jnp.abs(state._board - KING)),
     )
 
 
 def _legal_action_mask(state: State):
     # update cache
     state = _set_cache(state)
 
@@ -351,18 +349,18 @@
     )
 
     return legal_action_mask
 
 
 def _is_drop_pawn_mate(state: State):
     # check pawn drop mate
-    opp_king_pos = jnp.argmin(jnp.abs(state.piece_board - OPP_KING))
+    opp_king_pos = jnp.argmin(jnp.abs(state._board - OPP_KING))
     to = opp_king_pos + 1
     flip_state = _flip(
-        state.replace(piece_board=state.piece_board.at[to].set(PAWN))  # type: ignore
+        state.replace(_board=state._board.at[to].set(PAWN))  # type: ignore
     )
     # 玉頭の歩を取るか玉が逃げられれば詰みでない
     # fmt: off
     flipped_to = 80 - to
     flip_state = _set_cache(flip_state)
     can_capture_pawn = jax.vmap(partial(
         _is_legal_move_wo_pro, to=flipped_to, state=flip_state
@@ -373,30 +371,30 @@
     )(to=AROUND_IX[from_]).any()
     is_pawn_mate = ~(can_capture_pawn | can_king_escape)
     # fmt: on
     return is_pawn_mate, to
 
 
 def _is_legal_drop_wo_piece(to: jnp.ndarray, state: State):
-    is_illegal = state.piece_board[to] != EMPTY
+    is_illegal = state._board[to] != EMPTY
     is_illegal |= _is_checked(
-        state.replace(piece_board=state.piece_board.at[to].set(PAWN))  # type: ignore
+        state.replace(_board=state._board.at[to].set(PAWN))  # type: ignore
     )
     return ~is_illegal
 
 
 def _is_legal_drop_wo_ignoring_check(
     piece: jnp.ndarray, to: jnp.ndarray, state: State
 ):
-    is_illegal = state.piece_board[to] != EMPTY
+    is_illegal = state._board[to] != EMPTY
     # don't have the piece
-    is_illegal |= state.hand[0, piece] <= 0
+    is_illegal |= state._hand[0, piece] <= 0
     # double pawn
     is_illegal |= (piece == PAWN) & (
-        (state.piece_board == PAWN).reshape(9, 9).sum(axis=1) > 0
+        (state._board == PAWN).reshape(9, 9).sum(axis=1) > 0
     )[to // 9]
     # get stuck
     is_illegal |= ((piece == PAWN) | (piece == LANCE)) & (to % 9 == 0)
     is_illegal |= (piece == KNIGHT) & (to % 9 < 2)
     return ~is_illegal
 
 
@@ -404,49 +402,49 @@
     from_: jnp.ndarray,
     to: jnp.ndarray,
     state: State,
 ):
     ok = _is_pseudo_legal_move(from_, to, state)
     ok &= ~_is_checked(
         state.replace(  # type: ignore
-            piece_board=state.piece_board.at[from_]
+            _board=state._board.at[from_]
             .set(EMPTY)
             .at[to]
-            .set(state.piece_board[from_]),
-            cache_king=jax.lax.select(  # update cache
-                state.piece_board[from_] == KING,
+            .set(state._board[from_]),
+            _cache_king=jax.lax.select(  # update cache
+                state._board[from_] == KING,
                 jnp.int32(to),
-                state.cache_king,
+                state._cache_king,
             ),
         )
     )
     return ok
 
 
 def _is_pseudo_legal_move(
     from_: jnp.ndarray,
     to: jnp.ndarray,
     state: State,
 ):
     ok = _is_pseudo_legal_move_wo_obstacles(from_, to, state)
     # there is an obstacle between from_ and to
-    i = _major_piece_ix(state.piece_board[from_])
+    i = _major_piece_ix(state._board[from_])
     between_ix = BETWEEN_IX[i, from_, to, :]
     is_illegal = (i >= 0) & (
-        (between_ix >= 0) & (state.piece_board[between_ix] != EMPTY)
+        (between_ix >= 0) & (state._board[between_ix] != EMPTY)
     ).any()
     return ok & ~is_illegal
 
 
 def _is_pseudo_legal_move_wo_obstacles(
     from_: jnp.ndarray,
     to: jnp.ndarray,
     state: State,
 ):
-    board = state.piece_board
+    board = state._board
     # source is not my piece
     piece = board[from_]
     is_illegal = (from_ < 0) | ~((PAWN <= piece) & (piece < OPP_PAWN))
     # destination is my piece
     is_illegal |= (PAWN <= board[to]) & (board[to] < OPP_PAWN)
     # piece cannot move like that
     is_illegal |= ~CAN_MOVE[piece, from_, to]
@@ -455,38 +453,38 @@
 
 def _is_no_promotion_legal(
     from_: jnp.ndarray,
     to: jnp.ndarray,
     state: State,
 ):
     # source is not my piece
-    piece = state.piece_board[from_]
+    piece = state._board[from_]
     # promotion
     is_illegal = ((piece == PAWN) | (piece == LANCE)) & (to % 9 == 0)  # 必ず成る
     is_illegal |= (piece == KNIGHT) & (to % 9 < 2)  # 必ず成る
     return ~is_illegal
 
 
 def _is_promotion_legal(
     from_: jnp.ndarray,
     to: jnp.ndarray,
     state: State,
 ):
     # source is not my piece
-    piece = state.piece_board[from_]
+    piece = state._board[from_]
     # promotion
     is_illegal = (GOLD <= piece) & (piece <= DRAGON)  # 成れない駒
     is_illegal |= (from_ % 9 >= 3) & (to % 9 >= 3)  # 相手陣地と関係がない
     return ~is_illegal
 
 
 def _is_checked(state):
     # Use cached king position, simpler implementation is:
     # jnp.argmin(jnp.abs(state.piece_board - KING))
-    king_pos = state.cache_king
+    king_pos = state._cache_king
     flipped_king_pos = 80 - king_pos
 
     @jax.vmap
     def can_capture_king(from_):
         return _is_pseudo_legal_move(
             from_=from_, to=flipped_king_pos, state=_flip(state)
         )
@@ -496,15 +494,15 @@
         return _is_pseudo_legal_move_wo_obstacles(
             from_=from_, to=flipped_king_pos, state=_flip(state)
         )
 
     # Simpler implementation without cache of major piece places
     # from_ = CAN_MOVE_ANY[flipped_king_pos]
     # return can_capture_king(from_).any()
-    from_ = 80 - state.cache_m2b
+    from_ = 80 - state._cache_m2b
     from_ = jnp.where(from_ == 81, -1, from_)
     neighbours = NEIGHBOUR_IX[flipped_king_pos]
     return (
         can_capture_king(from_).any()
         | can_capture_king_local(neighbours).any()
     )
 
@@ -514,21 +512,21 @@
 
 
 def _rotate(board: jnp.ndarray) -> jnp.ndarray:
     return jnp.rot90(board.reshape(9, 9), k=3)
 
 
 def _flip(state):
-    empty_mask = state.piece_board == EMPTY
-    pb = (state.piece_board + 14) % 28
+    empty_mask = state._board == EMPTY
+    pb = (state._board + 14) % 28
     pb = jnp.where(empty_mask, EMPTY, pb)
     pb = pb[::-1]
     return state.replace(  # type: ignore
-        piece_board=pb,
-        hand=state.hand[jnp.int8((1, 0))],
+        _board=pb,
+        _hand=state._hand[jnp.int8((1, 0))],
     )
 
 
 def _is_major_piece(piece):
     return (
         (piece == LANCE)
         | (piece == BISHOP)
@@ -566,46 +564,45 @@
         lambda: (state, _flip(state)),
         lambda: (_flip(state), state),
     )
 
     def pieces(state):
         # 駒の場所
         my_pieces = jnp.arange(OPP_PAWN)
-        my_piece_feat = jax.vmap(lambda p: state.piece_board == p)(my_pieces)
+        my_piece_feat = jax.vmap(lambda p: state._board == p)(my_pieces)
         return my_piece_feat
 
     def effect_all(state):
         def effect(from_, to):
-            piece = state.piece_board[from_]
+            piece = state._board[from_]
             can_move = CAN_MOVE[piece, from_, to]
             major_piece_ix = _major_piece_ix(piece)
             between_ix = BETWEEN_IX[major_piece_ix, from_, to, :]
             has_obstacles = jax.lax.select(
                 major_piece_ix >= 0,
                 (
-                    (between_ix >= 0)
-                    & (state.piece_board[between_ix] != EMPTY)
+                    (between_ix >= 0) & (state._board[between_ix] != EMPTY)
                 ).any(),
                 FALSE,
             )
             return can_move & ~has_obstacles
 
         effects = jax.vmap(jax.vmap(effect, (None, 0)), (0, None))(
             ALL_SQ, ALL_SQ
         )
-        mine = (PAWN <= state.piece_board) & (state.piece_board < OPP_PAWN)
+        mine = (PAWN <= state._board) & (state._board < OPP_PAWN)
         return jnp.where(mine.reshape(81, 1), effects, FALSE)
 
     def piece_and_effect(state):
         my_pieces = jnp.arange(OPP_PAWN)
         my_effect = effect_all(state)
 
         @jax.vmap
         def filter_effect(p):
-            mask = state.piece_board == p
+            mask = state._board == p
             return jnp.where(mask.reshape(81, 1), my_effect, FALSE).any(axis=0)
 
         my_effect_feat = filter_effect(my_pieces)
         my_effect_sum = my_effect.sum(axis=0)
 
         @jax.vmap
         def effect_sum(n) -> jnp.ndarray:
@@ -632,16 +629,16 @@
     my_piece_feat = pieces(state)
     my_effect_feat, my_effect_sum_feat = piece_and_effect(state)
     opp_piece_feat = pieces(flip_state)
     opp_effect_feat, opp_effect_sum_feat = piece_and_effect(flip_state)
     opp_piece_feat = opp_piece_feat[:, ::-1]
     opp_effect_feat = opp_effect_feat[:, ::-1]
     opp_effect_sum_feat = opp_effect_sum_feat[:, ::-1]
-    my_hand_feat = hand_feat(state.hand[0])
-    opp_hand_feat = hand_feat(state.hand[1])
+    my_hand_feat = hand_feat(state._hand[0])
+    opp_hand_feat = hand_feat(state._hand[1])
     # NOTE: update cache
     checked = jnp.tile(_is_checked(_set_cache(state)), reps=(1, 9, 9))
     feat1 = [
         my_piece_feat.reshape(14, 9, 9),
         my_effect_feat.reshape(14, 9, 9),
         my_effect_sum_feat.reshape(3, 9, 9),
         opp_piece_feat.reshape(14, 9, 9),
```

### Comparing `pgx-0.5.1/pgx/sparrow_mahjong.py` & `pgx-0.5.2/pgx/sparrow_mahjong.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,37 +60,37 @@
     reward: jnp.ndarray = jnp.zeros(3, dtype=jnp.float32)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Sparrow Mahjong specific ---
-    turn: jnp.ndarray = jnp.int32(0)  # 0 = dealer
-    rivers: jnp.ndarray = -jnp.ones(
+    _turn: jnp.ndarray = jnp.int32(0)  # 0 = dealer
+    _rivers: jnp.ndarray = -jnp.ones(
         (N_PLAYER, MAX_RIVER_LENGTH), dtype=jnp.int32
     )  # tile type (0~10) is set
-    last_discard: jnp.ndarray = jnp.int32(-1)  # tile type (0~10) is set
-    hands: jnp.ndarray = jnp.zeros(
+    _last_discard: jnp.ndarray = jnp.int32(-1)  # tile type (0~10) is set
+    _hands: jnp.ndarray = jnp.zeros(
         (N_PLAYER, NUM_TILE_TYPES), dtype=jnp.int32
     )  # tile type (0~10) is set
-    n_red_in_hands: jnp.ndarray = jnp.zeros(
+    _n_red_in_hands: jnp.ndarray = jnp.zeros(
         (N_PLAYER, NUM_TILE_TYPES), dtype=jnp.int32
     )
-    is_red_in_river: jnp.ndarray = jnp.zeros(
+    _is_red_in_river: jnp.ndarray = jnp.zeros(
         (N_PLAYER, MAX_RIVER_LENGTH), dtype=jnp.bool_
     )
-    wall: jnp.ndarray = jnp.zeros(
+    _wall: jnp.ndarray = jnp.zeros(
         NUM_TILES, dtype=jnp.int32
     )  # tile id (0~43) is set
-    draw_ix: jnp.ndarray = jnp.int32(N_PLAYER * 5)
-    shuffled_players: jnp.ndarray = jnp.zeros(
+    _draw_ix: jnp.ndarray = jnp.int32(N_PLAYER * 5)
+    _shuffled_players: jnp.ndarray = jnp.zeros(
         N_PLAYER, dtype=jnp.int8
     )  # 0: dealer, ...
-    dora: jnp.ndarray = jnp.int32(0)  # tile type (0~10) is set
-    scores: jnp.ndarray = jnp.zeros(3, dtype=jnp.int32)  # 0 = dealer
+    _dora: jnp.ndarray = jnp.int32(0)  # tile type (0~10) is set
+    _scores: jnp.ndarray = jnp.zeros(3, dtype=jnp.int32)  # 0 = dealer
 
     @property
     def env_id(self) -> v1.EnvId:
         return "sparrow_mahjong"
 
 
 class SparrowMahjong(v1.Env):
@@ -113,44 +113,44 @@
             lambda x: x[-1].terminated, f, (key, state)
         )
         return state
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         # discard tile
-        hands = state.hands.at[state.turn % N_PLAYER, action].add(-1)
+        hands = state._hands.at[state._turn % N_PLAYER, action].add(-1)
         is_red_discarded = (
-            hands[state.turn % N_PLAYER, action]
-            < state.n_red_in_hands[state.turn % N_PLAYER, action]
+            hands[state._turn % N_PLAYER, action]
+            < state._n_red_in_hands[state._turn % N_PLAYER, action]
         )
-        n_red_in_hands = state.n_red_in_hands.at[
-            state.turn % N_PLAYER, action
+        n_red_in_hands = state._n_red_in_hands.at[
+            state._turn % N_PLAYER, action
         ].add(-is_red_discarded.astype(jnp.int32))
-        rivers = state.rivers.at[
-            state.turn % N_PLAYER, state.turn // N_PLAYER
+        rivers = state._rivers.at[
+            state._turn % N_PLAYER, state._turn // N_PLAYER
         ].set(action)
-        is_red_in_river = state.is_red_in_river.at[
-            state.turn % N_PLAYER, state.turn // N_PLAYER
+        is_red_in_river = state._is_red_in_river.at[
+            state._turn % N_PLAYER, state._turn // N_PLAYER
         ].set(is_red_discarded)
         last_discard = action
         state = state.replace(  # type: ignore
-            hands=hands,
-            n_red_in_hands=n_red_in_hands,
-            rivers=rivers,
-            is_red_in_river=is_red_in_river,
-            last_discard=last_discard,
+            _hands=hands,
+            _n_red_in_hands=n_red_in_hands,
+            _rivers=rivers,
+            _is_red_in_river=is_red_in_river,
+            _last_discard=last_discard,
         )
 
         scores = _hands_to_score(state)  # type: ignore
         winning_players = _check_ron(state, scores)  # type: ignore
         return lax.cond(
             jnp.any(winning_players),
             lambda: _step_by_ron(state, scores, winning_players),  # type: ignore
             lambda: lax.cond(
-                jnp.bool_(NUM_TILES - 1 <= state.draw_ix),  # type: ignore
+                jnp.bool_(NUM_TILES - 1 <= state._draw_ix),  # type: ignore
                 lambda: _step_by_tie(state),
                 lambda: _step_non_tied(state, scores),  # type: ignore
             ),
         )
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
@@ -198,20 +198,20 @@
     draw_ix = jnp.int32(N_PLAYER * 5)
     hands = hands.at[0, wall[draw_ix] // 4].add(1)
     draw_ix += 1
     legal_action_mask = hands[0] > 0
     state = State(
         current_player=current_player,
         legal_action_mask=legal_action_mask,
-        hands=hands,
-        n_red_in_hands=n_red_in_hands,
-        wall=wall,
-        draw_ix=draw_ix,
-        shuffled_players=shuffled_players,
-        dora=dora,
+        _hands=hands,
+        _n_red_in_hands=n_red_in_hands,
+        _wall=wall,
+        _draw_ix=draw_ix,
+        _shuffled_players=shuffled_players,
+        _dora=dora,
     )  # type: ignore
 
     # check tenhou
     scores = _hands_to_score(state)
     is_tsumo = _check_tsumo(state, scores)
     state = lax.cond(
         is_tsumo,
@@ -238,23 +238,23 @@
     ix = jnp.argmin(jnp.abs(WIN_HANDS - _to_base5(hand)))
     return BASE_SCORES[ix], YAKU_SCORES[ix]
 
 
 def _hands_to_score(state: State) -> jnp.ndarray:
     scores = jnp.zeros(3, dtype=jnp.int32)
     for i in range(N_PLAYER):
-        hand = state.hands[i]
+        hand = state._hands[i]
         hand = jax.lax.cond(
             hand.sum() == 5,
-            lambda: hand.at[state.last_discard].add(1),
+            lambda: hand.at[state._last_discard].add(1),
             lambda: hand,
         )
         bs, ys = _hand_to_score(hand)
-        n_doras = hand[state.dora]
-        n_red_doras = state.n_red_in_hands[i].sum().astype(jnp.int32)
+        n_doras = hand[state._dora]
+        n_red_doras = state._n_red_in_hands[i].sum().astype(jnp.int32)
         is_super_red = n_red_doras >= 6
         ys = lax.cond(is_super_red, lambda: jnp.int32(20), lambda: ys)
         s = lax.cond(
             ys >= 10,  # yakuman
             lambda: bs + ys,
             lambda: bs + ys + n_doras + n_red_doras,
         )
@@ -263,70 +263,72 @@
 
 
 def _check_ron(state: State, scores) -> jnp.ndarray:
     winning_players = jax.lax.fori_loop(
         0,
         N_PLAYER,
         lambda i, x: x.at[i].set(
-            _is_completed(state.hands.at[i, state.last_discard].add(1)[i])
+            _is_completed(state._hands.at[i, state._last_discard].add(1)[i])
         ),
         jnp.zeros(N_PLAYER, dtype=jnp.bool_),
     )
-    winning_players = winning_players.at[state.turn].set(False)
-    is_furiten = (state.rivers == state.last_discard).sum(axis=1) > 0
+    winning_players = winning_players.at[state._turn].set(False)
+    is_furiten = (state._rivers == state._last_discard).sum(axis=1) > 0
     winning_players = winning_players & jnp.logical_not(is_furiten)
     winning_players = winning_players & (scores >= 5)
     return winning_players
 
 
 def _check_tsumo(state: State, scores) -> jnp.ndarray:
-    return _is_completed(state.hands[state.turn]) & (scores[state.turn] >= 0)
+    return _is_completed(state._hands[state._turn]) & (
+        scores[state._turn] >= 0
+    )
 
 
 def _order_by_player_idx(x, shuffled_players):
     return lax.fori_loop(
         0,
         N_PLAYER,
         lambda i, e: e.at[shuffled_players[i]].set(x[i]),
         jnp.zeros_like(x),
     )
 
 
 def _step_by_ron(state: State, scores, winning_players):
     scores = scores.at[0].add(2)
     scores = scores * winning_players
-    scores = scores.at[state.turn % N_PLAYER].set(-scores.sum())
+    scores = scores.at[state._turn % N_PLAYER].set(-scores.sum())
     state = state.replace(  # type: ignore
         terminated=jnp.bool_(True),
         legal_action_mask=jnp.zeros_like(state.legal_action_mask),
-        scores=scores,
+        _scores=scores,
     )
     r = (
-        _order_by_player_idx(scores, state.shuffled_players).astype(
+        _order_by_player_idx(scores, state._shuffled_players).astype(
             jnp.float32
         )
         / MAX_SCORE
     )
     return state.replace(reward=r)  # type: ignore
 
 
 def _step_by_tsumo(state: State, scores):
     scores = scores.at[0].add(2)
-    winner_score = scores[state.turn]
+    winner_score = scores[state._turn]
     loser_score = jnp.ceil(winner_score / (N_PLAYER - 1)).astype(jnp.int32)
     winner_score = loser_score * (N_PLAYER - 1)
     scores = -jnp.ones(N_PLAYER, dtype=jnp.int32) * loser_score
-    scores = scores.at[state.turn % N_PLAYER].set(winner_score)
+    scores = scores.at[state._turn % N_PLAYER].set(winner_score)
     state = state.replace(  # type: ignore
         terminated=jnp.bool_(True),
         legal_action_mask=jnp.zeros_like(state.legal_action_mask),
-        scores=scores,
+        _scores=scores,
     )
     r = (
-        _order_by_player_idx(scores, state.shuffled_players).astype(
+        _order_by_player_idx(scores, state._shuffled_players).astype(
             jnp.float32
         )
         / MAX_SCORE
     )
     return state.replace(reward=r)  # type: ignore
 
 
@@ -335,34 +337,34 @@
         terminated=jnp.bool_(True),
         legal_action_mask=jnp.zeros_like(state.legal_action_mask),
     )
     return state.replace(reward=jnp.zeros(3, dtype=jnp.float32))  # type: ignore
 
 
 def _draw_tile(state: State) -> State:
-    turn = state.turn + 1
-    current_player = state.shuffled_players[turn % N_PLAYER]
-    tile_id = state.wall[state.draw_ix]
+    turn = state._turn + 1
+    current_player = state._shuffled_players[turn % N_PLAYER]
+    tile_id = state._wall[state._draw_ix]
     tile_type = tile_id // 4
     # gd=[36,37,38,39], rd=[40,41,42,43]
     is_red = ((tile_id % 4 == 0) & (tile_id != 36)) | (tile_id >= 40)
-    hands = state.hands.at[turn % N_PLAYER, tile_type].add(1)
-    n_red_in_hands = state.n_red_in_hands.at[turn % N_PLAYER, tile_type].add(
+    hands = state._hands.at[turn % N_PLAYER, tile_type].add(1)
+    n_red_in_hands = state._n_red_in_hands.at[turn % N_PLAYER, tile_type].add(
         is_red
     )
-    draw_ix = state.draw_ix + 1
+    draw_ix = state._draw_ix + 1
     legal_action_mask = hands[turn % N_PLAYER] > 0
     state = state.replace(  # type: ignore
-        turn=turn,
         current_player=current_player,
-        hands=hands,
-        n_red_in_hands=n_red_in_hands,
-        draw_ix=draw_ix,
         legal_action_mask=legal_action_mask,
         terminated=jnp.bool_(False),
+        _turn=turn,
+        _hands=hands,
+        _n_red_in_hands=n_red_in_hands,
+        _draw_ix=draw_ix,
     )
     return state
 
 
 def _step_non_terminal(state: State):
     r = jnp.zeros(3, dtype=jnp.float32)
     return state.replace(reward=r)  # type: ignore
@@ -385,113 +387,117 @@
     * [binary 1x11] has red doras
     * [binary 1x11] dora
     * [binary 3x11] all discarded tiles by (self, next, after the next)
     * [binary 3x2x11] discarded tiles in the last 3 steps (next, after the next)
     """
     N = 3
     n_feat = 4 + 1 + 1 + 3 + N * 2
-    turn = jnp.abs(state.shuffled_players - player_id).argmin()
+    turn = jnp.abs(state._shuffled_players - player_id).argmin()
     obs = jnp.zeros((n_feat, NUM_TILE_TYPES), dtype=jnp.bool_)
     zeros = jnp.zeros(NUM_TILE_TYPES, dtype=jnp.bool_)
     ones = jnp.ones(NUM_TILE_TYPES, dtype=jnp.bool_)
     # hand
-    obs = obs.at[0].set(jnp.where(state.hands[turn] >= 1, ones, zeros))
-    obs = obs.at[1].set(jnp.where(state.hands[turn] >= 2, ones, zeros))
-    obs = obs.at[2].set(jnp.where(state.hands[turn] >= 3, ones, zeros))
-    obs = obs.at[3].set(jnp.where(state.hands[turn] >= 4, ones, zeros))
+    obs = obs.at[0].set(jnp.where(state._hands[turn] >= 1, ones, zeros))
+    obs = obs.at[1].set(jnp.where(state._hands[turn] >= 2, ones, zeros))
+    obs = obs.at[2].set(jnp.where(state._hands[turn] >= 3, ones, zeros))
+    obs = obs.at[3].set(jnp.where(state._hands[turn] >= 4, ones, zeros))
     # red dora
     obs = obs.at[4].set(
-        jnp.where(state.n_red_in_hands[turn] >= 1, ones, zeros)
+        jnp.where(state._n_red_in_hands[turn] >= 1, ones, zeros)
     )
     # dora
-    obs = obs.at[5, state.dora].set(True)
+    obs = obs.at[5, state._dora].set(True)
     # all discards
     obs = obs.at[6].set(
         lax.fori_loop(
             0,
             MAX_RIVER_LENGTH,
             lambda i, x: lax.cond(
-                state.rivers[turn, i] >= 0,
-                lambda: x.at[state.rivers[turn, i]].set(True),
+                state._rivers[turn, i] >= 0,
+                lambda: x.at[state._rivers[turn, i]].set(True),
                 lambda: x,
             ),
             zeros,
         )
     )
     obs = obs.at[7].set(
         lax.fori_loop(
             0,
             MAX_RIVER_LENGTH,
             lambda i, x: lax.cond(
-                state.rivers[(turn + 1) % N_PLAYER, i] >= 0,
-                lambda: x.at[state.rivers[(turn + 1) % N_PLAYER, i]].set(True),
+                state._rivers[(turn + 1) % N_PLAYER, i] >= 0,
+                lambda: x.at[state._rivers[(turn + 1) % N_PLAYER, i]].set(
+                    True
+                ),
                 lambda: x,
             ),
             zeros,
         )
     )
     obs = obs.at[8].set(
         lax.fori_loop(
             0,
             MAX_RIVER_LENGTH,
             lambda i, x: lax.cond(
-                state.rivers[(turn + 2) % N_PLAYER, i] >= 0,
-                lambda: x.at[state.rivers[(turn + 2) % N_PLAYER, i]].set(True),
+                state._rivers[(turn + 2) % N_PLAYER, i] >= 0,
+                lambda: x.at[state._rivers[(turn + 2) % N_PLAYER, i]].set(
+                    True
+                ),
                 lambda: x,
             ),
             zeros,
         )
     )
     # last N discards (N=3)
     zeros = jnp.zeros(MAX_RIVER_LENGTH, dtype=jnp.bool_)
     ones = jnp.ones(MAX_RIVER_LENGTH, dtype=jnp.bool_)
     ix = (
-        jnp.where(state.rivers[(turn + 1) % N_PLAYER] >= 0, ones, zeros)
+        jnp.where(state._rivers[(turn + 1) % N_PLAYER] >= 0, ones, zeros)
     ).sum()
     obs = lax.cond(
         ix - 1 >= 0,
-        lambda: obs.at[9, state.rivers[(turn + 1) % N_PLAYER, ix - 1]].set(
+        lambda: obs.at[9, state._rivers[(turn + 1) % N_PLAYER, ix - 1]].set(
             True
         ),
         lambda: obs,
     )
     obs = lax.cond(
         ix - 2 >= 0,
-        lambda: obs.at[10, state.rivers[(turn + 1) % N_PLAYER, ix - 2]].set(
+        lambda: obs.at[10, state._rivers[(turn + 1) % N_PLAYER, ix - 2]].set(
             True
         ),
         lambda: obs,
     )
     obs = lax.cond(
         ix - 3 >= 0,
-        lambda: obs.at[11, state.rivers[(turn + 1) % N_PLAYER, ix - 3]].set(
+        lambda: obs.at[11, state._rivers[(turn + 1) % N_PLAYER, ix - 3]].set(
             True
         ),
         lambda: obs,
     )
     ix = (
-        jnp.where(state.rivers[(turn + 2) % N_PLAYER] >= 0, ones, zeros)
+        jnp.where(state._rivers[(turn + 2) % N_PLAYER] >= 0, ones, zeros)
     ).sum()
     obs = lax.cond(
         ix - 1 >= 0,
-        lambda: obs.at[12, state.rivers[(turn + 2) % N_PLAYER, ix - 1]].set(
+        lambda: obs.at[12, state._rivers[(turn + 2) % N_PLAYER, ix - 1]].set(
             True
         ),
         lambda: obs,
     )
     obs = lax.cond(
         ix - 2 >= 0,
-        lambda: obs.at[13, state.rivers[(turn + 2) % N_PLAYER, ix - 2]].set(
+        lambda: obs.at[13, state._rivers[(turn + 2) % N_PLAYER, ix - 2]].set(
             True
         ),
         lambda: obs,
     )
     obs = lax.cond(
         ix - 3 >= 0,
-        lambda: obs.at[14, state.rivers[(turn + 2) % N_PLAYER, ix - 3]].set(
+        lambda: obs.at[14, state._rivers[(turn + 2) % N_PLAYER, ix - 3]].set(
             True
         ),
         lambda: obs,
     )
     return obs
 
 
@@ -526,60 +532,60 @@
             s += "*" if is_red_in_river[i] else " "
         else:
             s += "_ "
     return s.ljust(20)
 
 
 def _to_str(state: State):
-    s = f"{'[terminated]' if state. terminated else ''} dora: {_tile_type_to_str(state.dora)}\n"
+    s = f"{'[terminated]' if state. terminated else ''} dora: {_tile_type_to_str(state._dora)}\n"
     for i in range(N_PLAYER):
-        s += f"{'*' if not state.terminated and state.turn % N_PLAYER == i else ' '}[{state.shuffled_players[i]}] "
-        s += f"{_hand_to_str(state.hands[i], state.n_red_in_hands[i])}: "
-        s += f"{_river_to_str(state.rivers[i], state.is_red_in_river[i])} "
+        s += f"{'*' if not state.terminated and state._turn % N_PLAYER == i else ' '}[{state._shuffled_players[i]}] "
+        s += f"{_hand_to_str(state._hands[i], state._n_red_in_hands[i])}: "
+        s += f"{_river_to_str(state._rivers[i], state._is_red_in_river[i])} "
         s += "\n"
     return s
 
 
 def _validate(state: State) -> bool:
-    if state.dora < 0 or 10 < state.dora:
+    if state._dora < 0 or 10 < state._dora:
         assert False
-    if 10 < state.last_discard:
+    if 10 < state._last_discard:
         assert False
-    if state.last_discard < 0 and state.rivers[0, 0] >= 0:
+    if state._last_discard < 0 and state._rivers[0, 0] >= 0:
         assert False
-    if jnp.any(state.hands < 0):
+    if jnp.any(state._hands < 0):
         assert False
-    counts = state.hands.sum(axis=0)
+    counts = state._hands.sum(axis=0)
     for i in range(N_PLAYER):
         for j in range(MAX_RIVER_LENGTH):
-            if state.rivers[i, j] >= 0:
-                counts = counts.at[state.rivers[i, j]].add(1)
+            if state._rivers[i, j] >= 0:
+                counts = counts.at[state._rivers[i, j]].add(1)
     if jnp.any(counts > 4):
         assert False
 
     # check legal_action_mask
     if not state.terminated:
         for i in range(NUM_TILE_TYPES):
             if (
                 state.legal_action_mask[i]
-                and state.hands[state.turn % N_PLAYER, i] <= 0
+                and state._hands[state._turn % N_PLAYER, i] <= 0
             ):
                 assert (
                     False
-                ), f"\n{state.legal_action_mask[i]}\n{state.hands[state.turn % N_PLAYER, i]}\n{_to_str(state)}"
+                ), f"\n{state.legal_action_mask[i]}\n{state._hands[state._turn % N_PLAYER, i]}\n{_to_str(state)}"
             if (
                 not state.legal_action_mask[i]
-                and state.hands[state.turn % N_PLAYER, i] > 0
+                and state._hands[state._turn % N_PLAYER, i] > 0
             ):
                 assert (
                     False
-                ), f"\n{state.legal_action_mask}\n{state.hands[state.turn % N_PLAYER]}\n{_to_str(state)}"
+                ), f"\n{state.legal_action_mask}\n{state._hands[state._turn % N_PLAYER]}\n{_to_str(state)}"
 
-    if not jnp.all(state.n_red_in_hands[:, :-2] <= 1):
+    if not jnp.all(state._n_red_in_hands[:, :-2] <= 1):
         assert False
-    if (state.n_red_in_hands.sum() + state.is_red_in_river.sum()) > 14:
+    if (state._n_red_in_hands.sum() + state._is_red_in_river.sum()) > 14:
         assert (
             False
-        ), f"\n{state.n_red_in_hands}\n{state.is_red_in_river}\n{_to_str(state)}"
+        ), f"\n{state._n_red_in_hands}\n{state._is_red_in_river}\n{_to_str(state)}"
 
-    assert state.scores.sum() == 0, f"\n{state.scores}\n{_to_str(state)}"
+    assert state._scores.sum() == 0, f"\n{state._scores}\n{_to_str(state)}"
     return True
```

### Comparing `pgx-0.5.1/pgx/tic_tac_toe.py` & `pgx-0.5.2/pgx/tic_tac_toe.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Tic-tac-toe specific ---
-    turn: jnp.ndarray = jnp.int8(0)
+    _turn: jnp.ndarray = jnp.int8(0)
     # 0 1 2
     # 3 4 5
     # 6 7 8
-    board: jnp.ndarray = -jnp.ones(9, jnp.int8)  # -1 (empty), 0, 1
+    _board: jnp.ndarray = -jnp.ones(9, jnp.int8)  # -1 (empty), 0, 1
 
     @property
     def env_id(self) -> v1.EnvId:
         return "tic_tac_toe"
 
 
 class TicTacToe(v1.Env):
@@ -77,41 +77,41 @@
 def _init(rng: jax.random.KeyArray) -> State:
     rng, subkey = jax.random.split(rng)
     current_player = jnp.int8(jax.random.bernoulli(subkey))
     return State(current_player=current_player)  # type:ignore
 
 
 def _step(state: State, action: jnp.ndarray) -> State:
-    state = state.replace(board=state.board.at[action].set(state.turn))  # type: ignore
-    won = _win_check(state.board, state.turn)
+    state = state.replace(_board=state._board.at[action].set(state._turn))  # type: ignore
+    won = _win_check(state._board, state._turn)
     reward = jax.lax.cond(
         won,
         lambda: jnp.float32([-1, -1]).at[state.current_player].set(1),
         lambda: jnp.zeros(2, jnp.float32),
     )
     return state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
-        legal_action_mask=state.board < 0,
+        legal_action_mask=state._board < 0,
         reward=reward,
-        terminated=won | jnp.all(state.board != -1),
-        turn=(state.turn + 1) % 2,
+        terminated=won | jnp.all(state._board != -1),
+        _turn=(state._turn + 1) % 2,
     )
 
 
 def _win_check(board, turn) -> jnp.ndarray:
     idx = jnp.int8([[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]])  # type: ignore
     return ((board[idx] == turn).all(axis=1)).any()
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     @jax.vmap
     def plane(i):
-        return (state.board == i).reshape((3, 3))
+        return (state._board == i).reshape((3, 3))
 
     # flip if player_id is opposite
     x = jax.lax.cond(
         state.current_player == player_id,
-        lambda: jnp.int8([state.turn, 1 - state.turn]),
-        lambda: jnp.int8([1 - state.turn, state.turn]),
+        lambda: jnp.int8([state._turn, 1 - state._turn]),
+        lambda: jnp.int8([1 - state._turn, state._turn]),
     )
 
     return jnp.stack(plane(x), -1)
```

### Comparing `pgx-0.5.1/pgx/v1.py` & `pgx-0.5.2/pgx/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
     elif env_id == "backgammon":
         from pgx.backgammon import Backgammon
 
         return Backgammon()
     elif env_id == "bridge_bidding":
         from pgx.bridge_bidding import BridgeBidding
 
-        return BridgeBidding()
+        return BridgeBidding(dds_hash_table_path=None)
     elif env_id == "chess":
         from pgx.chess import Chess
 
         return Chess()
     elif env_id == "connect_four":
         from pgx.connect_four import ConnectFour
```

### Comparing `pgx-0.5.1/pgx.egg-info/PKG-INFO` & `pgx-0.5.2/pgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.1
+Version: 0.5.2
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.5.2 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.1/pgx.egg-info/SOURCES.txt` & `pgx-0.5.2/pgx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 pgx.egg-info/SOURCES.txt
 pgx.egg-info/dependency_links.txt
 pgx.egg-info/requires.txt
 pgx.egg-info/top_level.txt
 pgx/_mahjong/__init__.py
 pgx/_mahjong/_action.py
 pgx/_mahjong/_hand.py
+pgx/_mahjong/_meld.py
+pgx/_mahjong/_shanten.py
+pgx/_mahjong/_yaku.py
 pgx/_src/__init__.py
 pgx/_src/api_test.py
 pgx/_src/chess_utils.py
 pgx/_src/shogi_utils.py
 pgx/_src/struct.py
 pgx/_src/visualizer.py
 pgx/_src/dwg/__init__.py
```

### Comparing `pgx-0.5.1/setup.py` & `pgx-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.5.1",
+    version="0.5.2",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
```

### Comparing `pgx-0.5.1/tests/minatar_utils.py` & `pgx-0.5.2/tests/minatar_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 state1[key], state2[key]
             ), f"{key}, {state1[key]}, {state2[key]}\n{state1}\n{state2}"
 
 
 def pgx2minatar(state, keys) -> Dict[str, Any]:
     d = {}
     for key in keys:
-        d[key] = copy.deepcopy(getattr(state, key))
+        d[key] = copy.deepcopy(getattr(state, "_" + key))
         if isinstance(d[key], jnp.ndarray):
             d[key] = np.array(d[key])
         if key == "entities":
             val = [None] * 8
             for i in range(8):
                 if d[key][i][0] != INF:
                     e = [d[key][i][j] for j in range(4)]
@@ -92,9 +92,10 @@
 
         if key in ["terminal", "sub_or", "surface"]:
             val = jnp.array(val, dtype=jnp.bool_)
         else:
             val = jnp.array(val, dtype=jnp.int32)
         d[key] = val
 
+    d = {"_" + k: v for k, v in d.items()}
     s = state_cls(**d)
     return s
```

### Comparing `pgx-0.5.1/tests/test_animal_shogi.py` & `pgx-0.5.2/tests/test_animal_shogi.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,42 +12,42 @@
     state.save_svg(fname, color_theme="dark")
 
 
 def test_step():
     state = init(jax.random.PRNGKey(0))
     visualize(state, "tests/assets/animal_shogi/test_step_000.svg")
     assert not state.terminated
-    assert state.turn == 0
+    assert state._turn == 0
 
     state = step(state, 3 * 12 + 6)  # Up PAWN
     visualize(state, "tests/assets/animal_shogi/test_step_001.svg")
     assert not state.terminated
-    assert state.turn == 1
-    assert state.board[6] == 5
-    assert state.hand[0, 0] == 0
-    assert state.hand[1, 0] == 1
-    assert state.hand.sum() == 1
+    assert state._turn == 1
+    assert state._board[6] == 5
+    assert state._hand[0, 0] == 0
+    assert state._hand[1, 0] == 1
+    assert state._hand.sum() == 1
 
     state = step(state, 0 * 12 + 11)  # Right Up Bishop
     visualize(state, "tests/assets/animal_shogi/test_step_002.svg")
     assert not state.terminated
-    assert state.turn == 0
-    assert state.board[5] == 6
-    assert state.hand[0, 0] == 1
-    assert state.hand[1, 0] == 1
-    assert state.hand.sum() == 2
+    assert state._turn == 0
+    assert state._board[5] == 6
+    assert state._hand[0, 0] == 1
+    assert state._hand[1, 0] == 1
+    assert state._hand.sum() == 2
 
     state = step(state, 8 * 12 + 6)  # Drop PAWN to 6
     visualize(state, "tests/assets/animal_shogi/test_step_003.svg")
     assert not state.terminated
-    assert state.turn == 1
-    assert state.board[5] == 5
-    assert state.hand[0, 0] == 1
-    assert state.hand[1, 0] == 0
-    assert state.hand.sum() == 1
+    assert state._turn == 1
+    assert state._board[5] == 5
+    assert state._hand[0, 0] == 1
+    assert state._hand[1, 0] == 0
+    assert state._hand.sum() == 1
 
 
 def test_observe():
     state = init(jax.random.PRNGKey(0))
     assert state.observation.shape == (4, 3, 22)
 
     # my pawn
@@ -74,19 +74,19 @@
          [False, False, False],
          [False, False, False],
          [False, False, False]]
     )
     assert (state.observation[:, :, 8] == expected).all()
 
     state = State(
-        board=jnp.int8([
+        _board=jnp.int8([
              8, -1, -1, -1,
             -1, -1, -1,  3,
             -1, -1, -1,  0]),
-        hand=jnp.int8([[2, 0, 0], [0, 1, 0]])
+        _hand=jnp.int8([[2, 0, 0], [0, 1, 0]])
     )
     state = state.replace(observation=_observe(state, state.current_player))
     expected = jnp.bool_(
         [[False, False, False],
          [False, False, False],
          [False, False, False],
          [True, False, False]]
```

### Comparing `pgx-0.5.1/tests/test_asterix.py` & `pgx-0.5.2/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/tests/test_backgammon.py` & `pgx-0.5.2/tests/test_backgammon.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,20 @@
     dice: jnp.ndarray,
     playable_dice: jnp.ndarray,
     played_dice_num: jnp.ndarray,
     legal_action_mask=jnp.zeros(6 * 26 + 6, dtype=jnp.bool_),
 ):
     return State(
         current_player=current_player,
-        rng=rng,
-        board=board,
-        turn=turn,
-        dice=dice,
-        playable_dice=playable_dice,
-        played_dice_num=played_dice_num,
+        _rng=rng,
+        _board=board,
+        _turn=turn,
+        _dice=dice,
+        _playable_dice=playable_dice,
+        _played_dice_num=played_dice_num,
         legal_action_mask=legal_action_mask,
     )
 
 
 def test_flip_board():
     test_board = make_test_boad()
     board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
@@ -115,15 +115,15 @@
     print(_flip_board, test_board)
     assert  (flipped_board == board).all()
 
 
 
 def test_init():
     state = init(rng)
-    assert state.turn == 0 or state.turn == 1
+    assert state._turn == 0 or state._turn == 1
 
 
 def test_init_roll():
     a = _roll_init_dice(rng)
     assert len(a) == 2
     assert a[0] != a[1]
 
@@ -157,17 +157,17 @@
         played_dice_num=jnp.int16(2),
     )
     assert _is_turn_end(state)
 
 
 def test_change_turn():
     state = init(rng)
-    _turn = state.turn
+    _turn = state._turn
     state = _change_turn(state)
-    assert state.turn == (_turn + 1) % 2
+    assert state._turn == (_turn + 1) % 2
 
     test_board: jnp.ndarray = make_test_boad()
     board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
     board = board.at[4].set(-5)
     board = board.at[3].set(-1)
     board = board.at[2].set(-2)
     board = board.at[27].set(-7)
@@ -182,17 +182,17 @@
         board=test_board,
         turn=jnp.int8(0),
         dice=jnp.array([2, 2], dtype=jnp.int16),
         playable_dice=jnp.array([-1, -1, -1, -1], dtype=jnp.int16),
         played_dice_num=jnp.int16(2),
     )
     state = _change_turn(state)
-    print(state.board, board)
-    assert state.turn == jnp.int8(1)  # ターンが変わっている.
-    assert (state.board == board).all()  # 反転している.
+    print(state._board, board)
+    assert state._turn == jnp.int8(1)  # ターンが変わっている.
+    assert (state._board == board).all()  # 反転している.
 
 def test_no_op():
     board: jnp.ndarray = make_test_boad()
     legal_action_mask = _legal_action_mask(
         board, jnp.array([0, 1, -1, -1], dtype=jnp.int16)
     )
     state = make_test_state(
@@ -202,15 +202,15 @@
         turn=jnp.int8(1),
         dice=jnp.array([0, 1], dtype=jnp.int16),
         playable_dice=jnp.array([0, 1, -1, -1], dtype=jnp.int16),
         played_dice_num=jnp.int16(0),
         legal_action_mask=legal_action_mask,
     )
     state = step(state, 0)  # execute no-op action
-    assert state.turn == jnp.int8(0)  # no-opの後はturnが変わっていることを確認.
+    assert state._turn == jnp.int8(0)  # no-opの後はturnが変わっていることを確認.
 
 
 def test_step():
     # 白
     board: jnp.ndarray = make_test_boad()
     board = _flip_board(board)  # 反転
     legal_action_mask = _legal_action_mask(
@@ -240,33 +240,33 @@
         True
     )  # 24(bar)->1
     assert (expected_legal_action_mask == state.legal_action_mask).all()  # legal_actionが正しいかtest
 
     # 白がサイコロ2をplay 24(bar)->1
     state = step(state=state, action=(1) * 6 + 1)
     assert (
-        state.playable_dice == jnp.array([0, -1, -1, -1], dtype=jnp.int16)
+            state._playable_dice == jnp.array([0, -1, -1, -1], dtype=jnp.int16)
     ).all()  # playable diceが正しく更新されているか
-    assert state.played_dice_num == 1  # played diceが増えているか.
-    assert state.turn == 1  # turnが変わっていないか.
-    assert state.board.at[1].get() == 4 and state.board.at[24].get() == 3
+    assert state._played_dice_num == 1  # played diceが増えているか.
+    assert state._turn == 1  # turnが変わっていないか.
+    assert state._board.at[1].get() == 4 and state._board.at[24].get() == 3
     expected_legal_action_mask: jnp.ndarray = jnp.zeros(
         6 * 26 + 6, dtype=jnp.bool_
     )
     expected_legal_action_mask = expected_legal_action_mask.at[
         6 * (1) + 0
     ].set(
         True
     )  # 24(bar)->0
     assert (expected_legal_action_mask == state.legal_action_mask).all()  # legal_actionが正しく更新されているか
     # 白がサイコロ1をplay 24(off)->0
     state = step(state=state, action=(1) * 6 + 0)
-    assert state.played_dice_num == 0
-    assert state.turn == 0  # turn が黒に変わっているか.
-    assert state.board.at[23].get() == -1 and state.board.at[25].get() == -2
+    assert state._played_dice_num == 0
+    assert state._turn == 0  # turn が黒に変わっているか.
+    assert state._board.at[23].get() == -1 and state._board.at[25].get() == -2
     
     # 黒
     board: jnp.ndarray = make_test_boad()
     legal_action_mask = _legal_action_mask(
         board, jnp.array([4, 5, -1, -1], dtype=jnp.int16)
     )
     state = make_test_state(
```

### Comparing `pgx-0.5.1/tests/test_breakout.py` & `pgx-0.5.2/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/tests/test_bridge_bidding.py` & `pgx-0.5.2/tests/test_bridge_bidding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import csv
+import os
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from pgx.bridge_bidding import (
@@ -21,15 +22,18 @@
     _state_to_pbn,
     _to_binary,
     _value_to_dds_tricks,
     duplicate,
     init,
 )
 
-env = BridgeBidding()
+
+DDS_HASH_TABLE_PATH = os.path.join(os.path.dirname(__file__), "assets/dds_hash_table.npy")
+env = BridgeBidding(dds_hash_table_path=DDS_HASH_TABLE_PATH )
+
 init_by_key = jax.jit(env.init)
 step = jax.jit(env.step)
 observe = jax.jit(env.observe)
 
 
 def test_shuffle_players():
     key = jax.random.PRNGKey(0)
@@ -39,49 +43,49 @@
         assert (shuffled_players[0] - shuffled_players[2]) % 2
         assert (shuffled_players[1] - shuffled_players[3]) % 2
 
 
 def test_init():
     key = jax.random.PRNGKey(0)
     state = init(key)
-    assert state.last_bid == -1
-    assert state.last_bidder == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert not state.pass_num
-    assert _player_position(state.current_player, state) == state.dealer
+    assert state._last_bid == -1
+    assert state._last_bidder == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert not state._pass_num
+    assert _player_position(state.current_player, state) == state._dealer
     assert state.legal_action_mask[:-2].all()
     assert not state.legal_action_mask[-2:].all()
 
 
 def test_duplicate():
     key = jax.random.PRNGKey(0)
     for i in range(1000):
         key, subkey = jax.random.split(key)
         init_state = init(subkey)
         duplicated_state = duplicate(init_state)
         assert (
             duplicated_state.current_player
-            == duplicated_state.shuffled_players[duplicated_state.dealer]
+            == duplicated_state._shuffled_players[duplicated_state._dealer]
         )
         assert (
-            init_state.shuffled_players[0]
-            == duplicated_state.shuffled_players[1]
+            init_state._shuffled_players[0]
+            == duplicated_state._shuffled_players[1]
         )
         assert (
-            init_state.shuffled_players[1]
-            == duplicated_state.shuffled_players[0]
+            init_state._shuffled_players[1]
+            == duplicated_state._shuffled_players[0]
         )
         assert (
-            init_state.shuffled_players[2]
-            == duplicated_state.shuffled_players[3]
+            init_state._shuffled_players[2]
+            == duplicated_state._shuffled_players[3]
         )
         assert (
-            init_state.shuffled_players[3]
-            == duplicated_state.shuffled_players[2]
+            init_state._shuffled_players[3]
+            == duplicated_state._shuffled_players[2]
         )
 
 
 def test_illegal_action_penalty():
     key = jax.random.PRNGKey(0)
     state = init(key)
     state = step(state, 36)
@@ -101,19 +105,19 @@
     #  XX  P 7C  P
     #   P  P
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     # state = init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(0),
-        vul_EW=jnp.bool_(0),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(0),
+        _vul_EW=jnp.bool_(0),
     )
     bidding_history = jnp.full(319, -1, dtype=jnp.int8)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     first_denomination_NS = jnp.full(5, -1, dtype=jnp.int8)
     first_denomination_EW = jnp.full(5, -1, dtype=jnp.int8)
@@ -121,463 +125,463 @@
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P
 
-    assert state.turn == 1
+    assert state._turn == 1
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
     bidding_history = bidding_history.at[0].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == np.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
 
-    assert state.turn == 2
+    assert state._turn == 2
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
     bidding_history = bidding_history.at[1].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 2
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
 
-    assert state.turn == 3
+    assert state._turn == 3
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
     bidding_history = bidding_history.at[2].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 3
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 3
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 0)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, -1, -1])
 
-    assert state.turn == 4
+    assert state._turn == 4
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
     bidding_history = bidding_history.at[3].set(0)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = legal_action_mask.at[0].set(False)
     legal_action_mask = legal_action_mask.at[36].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 0
-    assert _player_position(state.last_bidder, state) == 0
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 0
+    assert _player_position(state._last_bidder, state) == 0
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 8)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
-    assert state.turn == 5
+    assert state._turn == 5
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
     bidding_history = bidding_history.at[4].set(8)
-    assert np.all(state.bidding_history == bidding_history)
+    assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 9, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 8
-    assert _player_position(state.last_bidder, state) == 1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 8
+    assert _player_position(state._last_bidder, state) == 1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 36)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
-    assert state.turn == 6
+    assert state._turn == 6
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
     bidding_history = bidding_history.at[5].set(36)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 9, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 8
-    assert _player_position(state.last_bidder, state) == 1
-    assert state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 8
+    assert _player_position(state._last_bidder, state) == 1
+    assert state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
-    assert state.turn == 7
+    assert state._turn == 7
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
     bidding_history = bidding_history.at[6].set(35)
-    assert np.all(state.bidding_history == bidding_history)
+    assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 9, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 8
-    assert _player_position(state.last_bidder, state) == 1
-    assert state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == 8
+    assert _player_position(state._last_bidder, state) == 1
+    assert state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
-    assert state.turn == 8
+    assert state._turn == 8
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
     bidding_history = bidding_history.at[7].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 9, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 8
-    assert _player_position(state.last_bidder, state) == 1
-    assert state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 2
+    assert state._last_bid == 8
+    assert _player_position(state._last_bidder, state) == 1
+    assert state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 37)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
-    assert state.turn == 9
+    assert state._turn == 9
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
     bidding_history = bidding_history.at[8].set(37)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 9, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 8
-    assert _player_position(state.last_bidder, state) == 1
-    assert state.call_x
-    assert state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 8
+    assert _player_position(state._last_bidder, state) == 1
+    assert state._call_x
+    assert state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
-    assert state.turn == 10
+    assert state._turn == 10
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
     bidding_history = bidding_history.at[9].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 9, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 8
-    assert _player_position(state.last_bidder, state) == 1
-    assert state.call_x
-    assert state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == 8
+    assert _player_position(state._last_bidder, state) == 1
+    assert state._call_x
+    assert state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 22)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 11
+    assert state._turn == 11
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
     bidding_history = bidding_history.at[10].set(22)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 23, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(True)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 22
-    assert _player_position(state.last_bidder, state) == 3
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 22
+    assert _player_position(state._last_bidder, state) == 3
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 23)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 12
+    assert state._turn == 12
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
     bidding_history = bidding_history.at[11].set(23)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 24, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(True)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 23
-    assert _player_position(state.last_bidder, state) == 0
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 23
+    assert _player_position(state._last_bidder, state) == 0
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 13
+    assert state._turn == 13
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
     bidding_history = bidding_history.at[12].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 24, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 23
-    assert _player_position(state.last_bidder, state) == 0
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == 23
+    assert _player_position(state._last_bidder, state) == 0
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 25)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 14
+    assert state._turn == 14
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
     bidding_history = bidding_history.at[13].set(25)
-    assert np.all(state.bidding_history == bidding_history)
+    assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 26, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(True)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 25
-    assert _player_position(state.last_bidder, state) == 2
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 25
+    assert _player_position(state._last_bidder, state) == 2
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 36)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 15
+    assert state._turn == 15
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
     bidding_history = bidding_history.at[14].set(36)
-    assert np.all(state.bidding_history == bidding_history)
+    assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 26, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(True)
     assert np.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 25
-    assert _player_position(state.last_bidder, state) == 2
-    assert state.call_x
-    assert not state.call_xx
-    assert np.all(state.first_denomination_NS == first_denomination_NS)
-    assert np.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 25
+    assert _player_position(state._last_bidder, state) == 2
+    assert state._call_x
+    assert not state._call_xx
+    assert np.all(state._first_denomination_NS == first_denomination_NS)
+    assert np.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert np.all(state.reward == np.zeros(4))
 
     state = step(state, 37)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -585,34 +589,34 @@
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 16
+    assert state._turn == 16
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
     bidding_history = bidding_history.at[15].set(37)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 26, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 25
-    assert _player_position(state.last_bidder, state) == 2
-    assert state.call_x
-    assert state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 25
+    assert _player_position(state._last_bidder, state) == 2
+    assert state._call_x
+    assert state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -620,34 +624,34 @@
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 17
+    assert state._turn == 17
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
     bidding_history = bidding_history.at[16].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 26, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert np.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 25
-    assert _player_position(state.last_bidder, state) == 2
-    assert state.call_x
-    assert state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == 25
+    assert _player_position(state._last_bidder, state) == 2
+    assert state._call_x
+    assert state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 30)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -655,34 +659,34 @@
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 18
+    assert state._turn == 18
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
     bidding_history = bidding_history.at[17].set(30)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 31, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(True)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 30
-    assert _player_position(state.last_bidder, state) == 2
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 0
+    assert state._last_bid == 30
+    assert _player_position(state._last_bidder, state) == 2
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -690,34 +694,34 @@
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 19
+    assert state._turn == 19
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
     bidding_history = bidding_history.at[18].set(35)
-    assert np.all(state.bidding_history == bidding_history)
+    assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 31, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 30
-    assert _player_position(state.last_bidder, state) == 2
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == 30
+    assert _player_position(state._last_bidder, state) == 2
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -726,34 +730,34 @@
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   P
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 20
+    assert state._turn == 20
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
     bidding_history = bidding_history.at[19].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 31, False, state.legal_action_mask
     )
     legal_action_mask = legal_action_mask.at[36].set(True)
     legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 30
-    assert _player_position(state.last_bidder, state) == 2
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 2
+    assert state._last_bid == 30
+    assert _player_position(state._last_bidder, state) == 2
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -764,55 +768,55 @@
     #  XX  P 7C  P
     #   P  P
     # Passが3回続いたので終了
     assert state.terminated == True
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
-    assert state.turn == 20
+    assert state._turn == 20
     assert state.terminated
     bidding_history = bidding_history.at[20].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 31, False, state.legal_action_mask
     )
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     # legal_action_mask = legal_action_mask.at[36].set(True)
     # legal_action_mask = legal_action_mask.at[37].set(False)s
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == 30
-    assert _player_position(state.last_bidder, state) == 2
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 3
+    assert state._last_bid == 30
+    assert _player_position(state._last_bidder, state) == 2
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 3
     assert state.reward.shape == (4,)
     assert jnp.all(
         state.reward == jnp.array([-600, -600, 600, 600], dtype=jnp.int16)
     )
     declare_position, denomination, level, vul = _contract(state)
     assert declare_position == 0
     assert denomination == 0
     assert level == 7
     assert vul == 0
 
 
 def max_action_length_agent(state: State) -> int:
-    if (state.last_bid == -1 and state.pass_num != 3) or (
-        state.last_bid != -1 and state.pass_num != 2
+    if (state._last_bid == -1 and state._pass_num != 3) or (
+            state._last_bid != -1 and state._pass_num != 2
     ):
         return 35
     elif state.legal_action_mask[36]:
         return 36
     elif state.legal_action_mask[37]:
         return 37
     else:
-        return int(state.last_bid) + 1
+        return int(state._last_bid) + 1
 
 
 def test_max_action():
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
 
@@ -833,19 +837,19 @@
     #      P  P  P
     #   P
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     # state = init_by_key(HASH_TABLE_SAMPLE_KEYS[1], key)
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(0),
-        vul_EW=jnp.bool_(0),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(0),
+        _vul_EW=jnp.bool_(0),
     )
 
     bidding_history = jnp.full(319, -1, dtype=jnp.int8)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     first_denomination_NS = jnp.full(5, -1, dtype=jnp.int8)
@@ -854,96 +858,96 @@
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P
 
-    assert state.turn == 1
+    assert state._turn == 1
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
     bidding_history = bidding_history.at[0].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 1
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
 
-    assert state.turn == 2
+    assert state._turn == 2
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
     bidding_history = bidding_history.at[1].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 2
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
 
-    assert state.turn == 3
+    assert state._turn == 3
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
     bidding_history = bidding_history.at[2].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 3
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 3
     assert jnp.all(state.reward == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #   P
 
     assert state.terminated == True
-    assert state.turn == 3
+    assert state._turn == 3
     bidding_history = bidding_history.at[3].set(35)
-    assert jnp.all(state.bidding_history == bidding_history)
+    assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == jnp.ones(38, dtype=jnp.bool_))
-    assert state.last_bid == -1
-    assert _player_position(state.last_bidder, state) == -1
-    assert not state.call_x
-    assert not state.call_xx
-    assert jnp.all(state.first_denomination_NS == first_denomination_NS)
-    assert jnp.all(state.first_denomination_EW == first_denomination_EW)
-    assert state.pass_num == 4
+    assert state._last_bid == -1
+    assert _player_position(state._last_bidder, state) == -1
+    assert not state._call_x
+    assert not state._call_xx
+    assert jnp.all(state._first_denomination_NS == first_denomination_NS)
+    assert jnp.all(state._first_denomination_EW == first_denomination_EW)
+    assert state._pass_num == 4
     assert jnp.all(state.reward == jnp.zeros(4))
 
 
 def test_observe():
     # test init_obs
     # hand
     # hand: N:J92.J76.K72.9432 AKQ6.84.J863.T65 87543.KQ9532..K7 T.AT.AQT954.AQJ8
@@ -967,19 +971,19 @@
         .at[jnp.array([0, 5, 11, 12, 16, 20, 28, 31, 33, 36, 43, 44, 48])]
         .set(True)
     )
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(0),
-        vul_EW=jnp.bool_(0),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(0),
+        _vul_EW=jnp.bool_(0),
     )
 
     init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
     obs = observe(state, 0)
     print(_state_to_pbn(state))
     assert jnp.all(obs == init_obs)
 
@@ -993,50 +997,50 @@
 
     init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player3_hand))
     obs = observe(state, 3)
     assert jnp.all(obs == init_obs)
 
     # vul
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(1),
-        vul_EW=jnp.bool_(0),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(1),
+        _vul_EW=jnp.bool_(0),
     )
     init_obs = (
         jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
         .at[0]
         .set(True)
     )
     obs = observe(state, 0)
     assert jnp.all(obs == init_obs)
 
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(0),
-        vul_EW=jnp.bool_(1),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(0),
+        _vul_EW=jnp.bool_(1),
     )
     init_obs = (
         jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
         .at[1]
         .set(True)
     )
     obs = observe(state, 0)
 
     assert jnp.all(obs == init_obs)
 
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(1),
-        vul_EW=jnp.bool_(1),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(1),
+        _vul_EW=jnp.bool_(1),
     )
     init_obs = (
         jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
         .at[0]
         .set(True)
         .at[1]
         .set(True)
@@ -1057,19 +1061,19 @@
     #  XX  P 7C  P
     #   P  P
     #
 
     vul_history = jnp.zeros(426, dtype=jnp.bool_)
 
     state = state.replace(
-        dealer=jnp.int8(1),
+        _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
-        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
-        vul_NS=jnp.bool_(0),
-        vul_EW=jnp.bool_(0),
+        _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        _vul_NS=jnp.bool_(0),
+        _vul_EW=jnp.bool_(0),
     )
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -1578,71 +1582,71 @@
         y == jnp.array([67108863, 44739242, 22369621, 0], dtype=jnp.int32)
     )
 
 
 def test_state_to_pbn():
     key = jax.random.PRNGKey(0)
     state = init(key)
-    state = state.replace(hand=jnp.arange(52, dtype=jnp.int8))
+    state = state.replace(_hand=jnp.arange(52, dtype=jnp.int8))
     pbn = _state_to_pbn(state)
     assert (
         pbn
         == "N:AKQJT98765432... .AKQJT98765432.. ..AKQJT98765432. ...AKQJT98765432"
     )
 
-    state = state.replace(hand=jnp.arange(52, dtype=jnp.int8)[::-1])
+    state = state.replace(_hand=jnp.arange(52, dtype=jnp.int8)[::-1])
     pbn = _state_to_pbn(state)
     assert (
         pbn
         == "N:...AKQJT98765432 ..AKQJT98765432. .AKQJT98765432.. AKQJT98765432..."
     )
     # fmt: off
     hand = jnp.array([
         12,9,8,6,3,2,13,24,22,16,15,36,45,
         10,7,4,21,37,31,51,50,49,47,43,41,40,
         11,1,25,23,19,18,17,35,34,33,48,44,42,
         0,5,20,14,26,38,32,30,29,28,27,39,46,
         ]
     )
     # fmt: on
-    state = state.replace(hand=hand)
+    state = state.replace(_hand=hand)
     pbn = _state_to_pbn(state)
     print(pbn)
     assert (
         pbn
         == "N:KT9743.AQT43.J.7 J85.9.Q6.KQJ9532 Q2.KJ765.T98.T64 A6.82.AK75432.A8"
     )
 
 
 def test_state_to_key():
     rng = jax.random.PRNGKey(0)
     state = init(rng)
 
-    state = state.replace(hand=jnp.arange(52, dtype=jnp.int8))
+    state = state.replace(_hand=jnp.arange(52, dtype=jnp.int8))
     key = _state_to_key(state)
     assert jnp.all(
         key == jnp.array([0, 22369621, 44739242, 67108863], dtype=jnp.int32)
     )
 
-    state = state.replace(hand=jnp.arange(52, dtype=jnp.int8)[::-1])
+    state = state.replace(_hand=jnp.arange(52, dtype=jnp.int8)[::-1])
     key = _state_to_key(state)
     assert jnp.all(
         key == jnp.array([67108863, 44739242, 22369621, 0], dtype=jnp.int32)
     )
 
     # fmt: off
     hand = jnp.array([
         12,9,8,6,3,2,13,24,22,16,15,36,45,
         10,7,4,21,37,31,51,50,49,47,43,41,40,
         11,1,25,23,19,18,17,35,34,33,48,44,42,
         0,5,20,14,26,38,32,30,29,28,27,39,46,
         ]
     )
     # fmt: on
-    state = state.replace(hand=hand)
+    state = state.replace(_hand=hand)
     key = _state_to_key(state)
     assert jnp.all(
         key
         == jnp.array([58835992, 12758306, 67074695, 56200597], dtype=jnp.int32)
     )
 
 
@@ -1691,18 +1695,18 @@
     rng = jax.random.PRNGKey(0)
     # state => key => st
     for _ in range(1000):
         rng1, rng2 = jax.random.split(rng)
         state = init(rng2)
         sorted_hand = jnp.concatenate(
             [
-                jnp.sort(state.hand[:13]),
-                jnp.sort(state.hand[13:26]),
-                jnp.sort(state.hand[26:39]),
-                jnp.sort(state.hand[39:]),
+                jnp.sort(state._hand[:13]),
+                jnp.sort(state._hand[13:26]),
+                jnp.sort(state._hand[26:39]),
+                jnp.sort(state._hand[39:]),
             ]
         ).reshape(-1)
         key = _state_to_key(state)
         reconst_hand = _key_to_hand(key)
         assert jnp.all(sorted_hand == reconst_hand)
 
 
@@ -1713,15 +1717,15 @@
         reader = csv.reader(f, delimiter=",")
         for i in reader:
             samples.append([i[0], np.array(i[1:]).astype(np.int8)])
     key = jax.random.PRNGKey(0)
     for i in range(len(HASH_TABLE_SAMPLE_KEYS)):
         key, subkey = jax.random.split(key)
         state = init(subkey)
-        state = state.replace(hand=_key_to_hand(HASH_TABLE_SAMPLE_KEYS[i]))
+        state = state.replace(_hand=_key_to_hand(HASH_TABLE_SAMPLE_KEYS[i]))
         dds_tricks = _calculate_dds_tricks(
             state, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES
         )
         # sample dataから、作成したhash tableを用いて、ddsの結果を計算
         # その結果とsample dataが一致しているか確認
         assert jnp.all(dds_tricks == samples[i][1])
 
@@ -1739,15 +1743,17 @@
     )
     # fmt: on
 
 
 def test_api():
     import pgx
 
-    env = pgx.make("bridge_bidding")
+    env = pgx.bridge_bidding.BridgeBidding(
+        dds_hash_table_path=DDS_HASH_TABLE_PATH
+    )
     pgx.api_test(env, 10)
 
 
 def to_value(sample: list) -> jnp.ndarray:
     """Convert sample to value
     >>> sample = ['0', '1', '0', '4', '0', '13', '12', '13', '9', '13', '0', '1', '0', '4', '0', '13', '12', '13', '9', '13']
     >>> to_value(sample)
```

### Comparing `pgx-0.5.1/tests/test_chess.py` & `pgx-0.5.2/tests/test_chess.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,66 +127,66 @@
     # TODO: black underpromotion
 
 
 def test_step():
     # normal step
     state = State._from_fen("1k6/8/8/8/8/8/1Q6/7K w - - 0 1")
     state.save_svg("tests/assets/chess/step_001.svg")
-    assert state.board[p("b1")] == EMPTY
+    assert state._board[p("b1")] == EMPTY
     state = step(state, jnp.int32(672))
     state.save_svg("tests/assets/chess/step_002.svg")
-    assert state.board[p("b1", True)] == -QUEEN
+    assert state._board[p("b1", True)] == -QUEEN
 
     # promotion
     state = State._from_fen("r1r4k/1P6/8/8/8/8/P7/7K w - - 0 1")
     state.save_svg("tests/assets/chess/step_002.svg")
-    assert state.board[p("b8")] == EMPTY
+    assert state._board[p("b8")] == EMPTY
     # underpromotion
     next_state = step(state, jnp.int32(1022))
     next_state.save_svg("tests/assets/chess/step_003.svg")
-    assert next_state.board[p("b8", True)] == -ROOK
+    assert next_state._board[p("b8", True)] == -ROOK
     # promotion to queen
     next_state = step(state, jnp.int32(p("b7") * 73 + 16))
     next_state.save_svg("tests/assets/chess/step_004.svg")
-    assert next_state.board[p("b8", True)] == -QUEEN
+    assert next_state._board[p("b8", True)] == -QUEEN
 
     # castling
     state = State._from_fen("1k6/8/8/8/8/8/8/R3K2R w KQ - 0 1")
     state.save_svg("tests/assets/chess/step_005.svg")
     # left
     next_state = step(state, jnp.int32(p("e1") * 73 + 28))
     next_state.save_svg("tests/assets/chess/step_006.svg")
-    assert next_state.board[p("c1", True)] == -KING
-    assert next_state.board[p("d1", True)] == -ROOK  # castling
-    assert next_state.board[p("a1", True)] == EMPTY  # castling
+    assert next_state._board[p("c1", True)] == -KING
+    assert next_state._board[p("d1", True)] == -ROOK  # castling
+    assert next_state._board[p("a1", True)] == EMPTY  # castling
     # right
     next_state = step(state, jnp.int32(p("e1") * 73 + 31))
     next_state.save_svg("tests/assets/chess/step_007.svg")
-    assert next_state.board[p("g1", True)] == -KING
-    assert next_state.board[p("f1", True)] == -ROOK  # castling
-    assert next_state.board[p("h1", True)] == EMPTY  # castling
+    assert next_state._board[p("g1", True)] == -KING
+    assert next_state._board[p("f1", True)] == -ROOK  # castling
+    assert next_state._board[p("h1", True)] == EMPTY  # castling
 
     # en passant
     state = State._from_fen("1k6/8/8/8/3pP3/8/8/R3K2R b KQ e3 0 1")
     state.save_svg("tests/assets/chess/step_008.svg")
-    assert state.board[p("e4", True)] == -PAWN
+    assert state._board[p("e4", True)] == -PAWN
     next_state = step(state, jnp.int32(p("d4", True) * 73 + 44))
     next_state.save_svg("tests/assets/chess/step_009.svg")
-    assert next_state.board[p("e3")] == -PAWN
-    assert next_state.board[p("e4")] == EMPTY
+    assert next_state._board[p("e3")] == -PAWN
+    assert next_state._board[p("e4")] == EMPTY
     state = State._from_fen("1k6/8/8/8/3p4/8/4P3/R3K2R w KQ - 0 1")
     state.save_svg("tests/assets/chess/step_010.svg")
     next_state = step(state, jnp.int32(p("e2") * 73 + 17))  # UP 2
     next_state.save_svg("tests/assets/chess/step_011.svg")
-    assert next_state.en_passant == p("e3", True)
+    assert next_state._en_passant == p("e3", True)
     state = State._from_fen("1k6/p7/8/8/3p4/8/4P3/R3K2R b KQ - 0 1")
     state.save_svg("tests/assets/chess/step_012.svg")
     next_state = step(state, jnp.int32(p("a7", True) * 73 + 17))  # UP 2
     next_state.save_svg("tests/assets/chess/step_013.svg")
-    assert next_state.en_passant == p("a6")  # en passant is always white view
+    assert next_state._en_passant == p("a6")  # en passant is always white view
 
 
 def test_legal_action_mask():
     # init board
     state = State._from_fen("rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - 0 1")
     state.save_svg("tests/assets/chess/legal_action_mask_001.svg")
     assert state.legal_action_mask.sum() == 20
@@ -349,45 +349,45 @@
     assert state.legal_action_mask.sum() == 24
 
     # en passant
     state = State._from_fen("7k/7p/8/6P1/8/8/8/K7 b - - 0 1")
     state.save_svg("tests/assets/chess/legal_action_mask_028.svg")
     state = step(state, jnp.int32(4178))  # BPawn: h7 -> h5
     state.save_svg("tests/assets/chess/legal_action_mask_029.svg")
-    print(state.en_passant)
+    print(state._en_passant)
     print(state._to_fen())
     print(jnp.nonzero(state.legal_action_mask))
     assert state.legal_action_mask.sum() == 5
 
     # en passant (black)
     state = State._from_fen("7k/8/8/8/1p6/8/P7/K7 w - - 0 1")
     state.save_svg("tests/assets/chess/legal_action_mask_030.svg")
     state = step(state, jnp.int32(90))  # WPawn: a2 -> a4
     state.save_svg("tests/assets/chess/legal_action_mask_031.svg")
-    print(state.en_passant)
+    print(state._en_passant)
     print(state._to_fen())
     print(jnp.nonzero(state.legal_action_mask))
     assert state.legal_action_mask.sum() == 5
 
     # en passant
     state = State._from_fen("7k/4p3/8/3P1P2/8/8/8/K7 b - - 0 1")
     state.save_svg("tests/assets/chess/legal_action_mask_032.svg")
     state = step(state, jnp.int32(2426))  # BPawn: e7 -> e5
     state.save_svg("tests/assets/chess/legal_action_mask_033.svg")
-    print(state.en_passant)
+    print(state._en_passant)
     print(state._to_fen())
     print(jnp.nonzero(state.legal_action_mask))
     assert state.legal_action_mask.sum() == 7
 
     # en passant (black)
     state = State._from_fen("7k/8/8/8/2p1p3/8/3P4/K7 w - - 0 1")
     state.save_svg("tests/assets/chess/legal_action_mask_034.svg")
     state = step(state, jnp.int32(1842))  # WPawn: d2 -> d4
     state.save_svg("tests/assets/chess/legal_action_mask_035.svg")
-    print(state.en_passant)
+    print(state._en_passant)
     print(state._to_fen())
     print(jnp.nonzero(state.legal_action_mask))
     assert state.legal_action_mask.sum() == 7
 
     # pinned
     state = State._from_fen("7k/8/8/8/8/8/8/KR5q w - - 0 1")
     state.save_svg("tests/assets/chess/legal_action_mask_036.svg")
@@ -621,15 +621,15 @@
     state.save_svg("tests/assets/chess/buggy_samples_009.svg")
     state = step(state, 3986)
     state.save_svg("tests/assets/chess/buggy_samples_010.svg")
     assert state._to_fen() == "rn1qkbr1/2pp1pp1/p3pn1p/PQ6/1P6/6P1/2PP1P1P/R1BNKBNb w Qq - 0 11"
 
     # wrong en passant by pinned pawn
     state = State._from_fen("rn6/1b6/8/p1Br1k1p/PPp1pPpP/NRp3P1/2B4R/2K5 b - f3 0 54")
-    print(state.en_passant)
+    print(state._en_passant)
     state.save_svg("tests/assets/chess/buggy_samples_011.svg")
     expected_legal_actions = [16, 17, 263, 652, 654, 656, 701, 714, 715, 1517, 1984, 1985, 1986, 1987, 1988, 1989, 1990, 2000, 2001, 3154, 3182, 3197, 3853]
     assert state.legal_action_mask.sum() == len(expected_legal_actions), f"\nactual:{jnp.nonzero(state.legal_action_mask)[0]}\nexpected\n{expected_legal_actions}"
 
 
 def test_observe():
     state = init(jax.random.PRNGKey(0))
```

### Comparing `pgx-0.5.1/tests/test_connect_four.py` & `pgx-0.5.2/tests/test_connect_four.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     @@.....
     OO.....
     @@.....
     OO.....
     @@.....
     """
     # fmt: off
-    assert (state.board == jnp.array(
+    assert (state._board == jnp.array(
         [1, 1, -1, -1, -1, -1, -1,
          0, 0, -1, -1, -1, -1, -1,
          1, 1, -1, -1, -1, -1, -1,
          0, 0, -1, -1, -1, -1, -1,
          1, 1, -1, -1, -1, -1, -1,
          0, 0, -1, -1, -1, -1, -1])).all()
     # fmt:on
```

### Comparing `pgx-0.5.1/tests/test_freeway.py` & `pgx-0.5.2/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/tests/test_go.py` & `pgx-0.5.2/tests/test_go.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 
 def test_end_by_pass():
     key = jax.random.PRNGKey(0)
 
     state = init(key=key)
     state = step(state=state, action=25)
-    assert state.passed
+    assert state._passed
     assert not state.terminated
     state = step(state=state, action=0)
-    assert not state.passed
+    assert not state._passed
     assert not state.terminated
     state = step(state=state, action=25)
-    assert state.passed
+    assert state._passed
     assert not state.terminated
     state = step(state=state, action=25)
-    assert state.passed
+    assert state._passed
     assert state.terminated
 
 
 def test_step():
     """
     https://www.cosumi.net/replay/?b=You&w=COSUMI&k=0&r=0&bs=5&gr=ccbccdcbdbbadabdbecaacabecaddeaettceedbetttt
     """
@@ -80,15 +80,15 @@
       [ 0 1 2 3 4 ]
     [0] + O O @ +
     [1] O + O @ +
     [2] + O @ + @
     [3] O O @ + @
     [4] O O O @ +
     """
-    assert (jnp.clip(state.chain_id_board, -1, 1) == expected_board.ravel()).all()
+    assert (jnp.clip(state._chain_id_board, -1, 1) == expected_board.ravel()).all()
     assert state.terminated
 
     # 同点なのでコミの分 黒 == player_1 の負け
     assert (state.reward == jnp.array([1, -1])).all()
 
 
 def test_ko():
@@ -115,29 +115,29 @@
     ===========
     + + @ + +
     + @ O @ +
     + O + O +
     + + O + +
     + + + + +
     """
-    assert state.ko == 12
+    assert state._ko == 12
 
     loser = state.current_player
     state1: State = step(
         state=state, action=12
     )  # BLACK
     # ルール違反により黒 = player_id=1 の負け
     assert state1.terminated
     assert state1.reward[loser] == -1.
     assert state1.reward.sum() == 0.
 
     state2: State = step(state=state, action=0)  # BLACK
     # 回避した場合
     assert not state2.terminated
-    assert state2.ko == -1
+    assert state2._ko == -1
 
     # see #468
     state: State = init(key=key)
     state = step(state, action=2)
     state = step(state, action=9)
     state = step(state, action=18)
     state = step(state, action=5)
@@ -164,15 +164,15 @@
     state = step(state, action=17)
     state = step(state, action=25)
     state = step(state, action=13)
     state = step(state, action=4)
     state = step(state, action=14)
     state = step(state, action=23)
     state = step(state, action=0)
-    assert state.ko == -1
+    assert state._ko == -1
 
     # see #468
     state: State = init(key=key)
     state = step(state, action=1)
     state = step(state, action=16)
     state = step(state, action=9)
     state = step(state, action=11)
@@ -196,15 +196,15 @@
     state = step(state, action=25)
     state = step(state, action=12)
     state = step(state, action=10)
     state = step(state, action=2)
     state = step(state, action=25)
     state = step(state, action=3)
     state = step(state, action=20)
-    assert state.ko == -1
+    assert state._ko == -1
 
     # Ko after pass
     state: State = init(key=key)
     state = step(state, action=17)
     state = step(state, action=25)
     state = step(state, action=20)
     state = step(state, action=24)
@@ -238,15 +238,15 @@
     state = step(state, action=19)
     state = step(state, action=7)
     state = step(state, action=23)
     state = step(state, action=18)
     state = step(state, action=13)
     state = step(state, action=24)
     state = step(state, action=25)  # pass
-    assert state.ko == -1
+    assert state._ko == -1
 
     # see #479
     actions = [107, 11, 56, 41, 300, 19, 228, 231, 344, 257, 35, 32, 57, 276, 0, 277, 164, 15, 187, 179, 357, 255, 150, 211, 256,
      190, 297, 303, 358, 189, 322, 3, 129, 64, 13, 336, 22, 286, 264, 192, 55, 360, 23, 31, 113, 119, 195, 98, 208, 294,
      240, 241, 149, 280, 118, 296, 245, 99, 335, 226, 29, 287, 84, 248, 225, 351, 202, 20, 137, 274, 232, 85, 36, 141,
      108, 95, 282, 93, 337, 216, 58, 131, 283, 10, 106, 243, 318, 220, 136, 34, 127, 293, 80, 165, 125, 83, 114, 105,
      30, 61, 147, 71, 109, 173, 87, 233, 76, 361, 66, 115, 212, 200, 346, 197, 54, 326, 298, 167, 347, 4, 354, 16, 140,
@@ -264,15 +264,15 @@
      117, 112, 5, 81, 118, 135, 82, 92, 140, 123, 97, 278, 47, 361, 137, 230, 220]
     env = Go(size=19)
     env.init = jax.jit(env.init)
     env.step = jax.jit(env.step)
     state = env.init(jax.random.PRNGKey(0))
     for a in actions:
         state = env.step(state, a)
-    assert state.ko == -1
+    assert state._ko == -1
     assert state.legal_action_mask[231]
 
 def test_observe():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     assert state.current_player == 1
     # player 0 is white, player 1 is black
@@ -297,15 +297,15 @@
          [-1,  1, -1,  0, 0],
          [ 0,  0,  0,  0, 0],
          [ 0,  0,  0,  0, 0],
          [ 0,  0,  0,  0, 0]]
     )
     # fmt: on
     assert state.current_player == 1
-    assert state.turn % 2 == 0  # black turn
+    assert state._turn % 2 == 0  # black turn
     obs = observe(state, 0)   # white
     assert obs.shape == (5, 5, 17)
     assert (obs[:, :, 0] == (curr_board == -1)).all()
     assert (obs[:, :, 1] == (curr_board == 1)).all()
     assert (obs[:, :, -1] == 0).all()
 
     obs = observe(state, 1)  # black
@@ -1102,15 +1102,15 @@
     state = env.step(state, 1)  # WHITE
     #  O O + @ O
     #  @ @ @ O O
     #  @ @ @ O +
     #  + @ O O O
     #  @ @ @ O +
     assert state.terminated
-    assert state.black_player == 1
+    assert state._black_player == 1
     assert (state.reward == jnp.float32([-1, 1])).all()  # black wins
 
 
 def test_random_play_5():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     while not state.terminated:
@@ -1120,17 +1120,17 @@
         else:
             key = jax.random.PRNGKey(0)
             key, subkey = jax.random.split(key)
             a = jax.random.choice(subkey, actions[0])
 
         state = step(state=state, action=a)
 
-        if state.turn > 100:
+        if state._turn > 100:
             break
-    assert state.passed or state.turn > 100
+    assert state._passed or state._turn > 100
 
 
 def test_api():
     import pgx
     env = pgx.make("go-9x9")
     pgx.api_test(env, 10)
     env = pgx.make("go-19x19")
```

### Comparing `pgx-0.5.1/tests/test_hex.py` & `pgx-0.5.2/tests/test_hex.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
           0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
           0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
           0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
           0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
           0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0])
     # fmt:on
-    assert jnp.all(state.board == expected)
+    assert jnp.all(state._board == expected)
 
 
 def test_terminated():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     assert not state.terminated
     for i in range(11):
```

### Comparing `pgx-0.5.1/tests/test_kuhn_poker.py` & `pgx-0.5.2/tests/test_kuhn_poker.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 step = jax.jit(env.step)
 observe = jax.jit(env.observe)
 
 
 def test_init():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
-    assert state.cards[0] != state.cards[1]
+    assert state._cards[0] != state._cards[1]
     assert (state.legal_action_mask == jnp.bool_([0, 1, 0, 1])).all()
 
 
 def test_step():
     key = jax.random.PRNGKey(0)
     # cards = [2, 0]
     state = init(key)
```

### Comparing `pgx-0.5.1/tests/test_leduc_holdem.py` & `pgx-0.5.2/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/tests/test_othello.py` & `pgx-0.5.2/tests/test_othello.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         0, -1, -1, -1, -1, -1, 0, 0,
         0, 0, 1, 1, -1, 0, 0, 0,
         0, 0, 1, 1, 1, 0, 0, 0,
         0, 0, 0, 0, 0, 0, 0, 0,
         0, 0, 0, 0, 0, 0, 0, 0,
         0, 0, 0, 0, 0, 0, 0, 0])
     # fmt:on
-    assert jnp.all(state.board == expected)
+    assert jnp.all(state._board == expected)
 
 
 def test_terminated():
     # wipe out
     key = jax.random.PRNGKey(0)
     state = init(key)
     for i in [37, 43, 34, 29, 52, 45, 38, 44]:
```

### Comparing `pgx-0.5.1/tests/test_play2048.py` & `pgx-0.5.2/tests/test_play2048.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 observe = jax.jit(env.observe)
 slide_and_merge = jax.jit(_slide_and_merge)
 
 
 def test_init():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
-    assert jnp.count_nonzero(state.board == 1) == 2
+    assert jnp.count_nonzero(state._board == 1) == 2
 
 
 def test_slide_and_merge():
     line = jnp.int8([0, 2, 0, 2])
     assert (slide_and_merge(line)[0] == jnp.int8([3, 0, 0, 0])).all()
 
     line = jnp.int8([0, 2, 0, 1])
@@ -46,48 +46,48 @@
     """
     [[0 0 0 0]
      [0 0 2 0]
      [0 0 0 0]
      [0 0 2 0]]
     """
     assert (
-        state.board
+        state._board
         == jnp.int8([0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1, 0])
     ).all()
 
     state = step(state, 3)  # down
     """
     [[0 0 0 0]
      [0 0 0 0]
      [0 0 0 2]
      [0 0 4 0]]
     """
     assert (
-        state.board
+        state._board
         == jnp.int8([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 2, 0])
     ).all()
 
 
 def test_legal_action():
     board = jnp.int8([0, 1, 2, 3, 2, 3, 4, 5, 3, 4, 5, 6, 4, 5, 6, 0])
-    state = State(board=board)
+    state = State(_board=board)
     state = step(state, 0)
     """
     [[ 2  4  8  2]
      [ 4  8 16 32]
      [ 8 16 32 64]
      [16 32 64  0]]
     """
     assert (state.legal_action_mask == jnp.bool_([0, 0, 1, 1])).all()
     assert not state.terminated
 
 
 def test_terminated():
     board = jnp.int8([1, 2, 3, 4, 2, 3, 4, 5, 3, 4, 5, 6, 0, 4, 5, 6])
-    state = State(board=board)
+    state = State(_board=board)
     state = step(state, 0)
     """
     [[ 2  4  8 16]
      [ 4  8 16 32]
      [ 8 16 32 64]
      [16 32 64  2]]
     """
```

### Comparing `pgx-0.5.1/tests/test_seaquest.py` & `pgx-0.5.2/tests/test_seaquest.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,71 +134,71 @@
     import pgx
     env = pgx.make("minatar/seaquest")
     pgx.api_test(env)
 
 
 def test_buggy_sample():
     state = seaquest.State(
-        oxygen=jnp.int32(187),
-        diver_count=jnp.int32(0),
-        sub_x=jnp.int32(0),
-        sub_y=jnp.int32(3),
-        sub_or=jnp.bool_(False),
-        f_bullets= -jnp.ones(
+        _oxygen=jnp.int32(187),
+        _diver_count=jnp.int32(0),
+        _sub_x=jnp.int32(0),
+        _sub_y=jnp.int32(3),
+        _sub_or=jnp.bool_(False),
+        _f_bullets=-jnp.ones(
             (5, 3), dtype=jnp.int32
         ),  #.at[0, :].set(jnp.int32([6, 6, 0])),
-        e_bullets=-jnp.ones(
+        _e_bullets=-jnp.ones(
             (25, 3), dtype=jnp.int32
         ),
-        e_fish = (-jnp.ones(
+        _e_fish=(-jnp.ones(
             (25, 4), dtype=jnp.int32
         )).at[:2, :].set(
             [[3, 8, 0, 2],
              [0, 4, 1, 4]]
         ),
-        e_subs = (-jnp.ones(
+        _e_subs=(-jnp.ones(
             (25, 5), dtype=jnp.int32
         )).at[:2, :].set(
             jnp.int32(
                 [[9, 1, 1, 0, 6],
                  [6, 6, 0, 3, 1]]
             )
         ),
-        divers = (-jnp.ones(
+        _divers=(-jnp.ones(
             (5, 4), dtype=jnp.int32
         )).at[:2, :].set(
             [[3, 3, 0, 2],
              [1, 7, 1, 2]]
         ),
-        e_spawn_speed=jnp.int32(19),
-        e_spawn_timer=jnp.int32(18),
-        d_spawn_timer=jnp.int32(21),
-        move_speed=jnp.int32(5),
-        ramp_index=jnp.int32(1),
-        shot_timer=jnp.int32(0),
-        surface=jnp.bool_(False),
-        terminal=jnp.bool_(False),
-        last_action=jnp.int32(4)
+        _e_spawn_speed=jnp.int32(19),
+        _e_spawn_timer=jnp.int32(18),
+        _d_spawn_timer=jnp.int32(21),
+        _move_speed=jnp.int32(5),
+        _ramp_index=jnp.int32(1),
+        _shot_timer=jnp.int32(0),
+        _surface=jnp.bool_(False),
+        _terminal=jnp.bool_(False),
+        _last_action=jnp.int32(4)
     )
     state = state.replace(observation=observe(state))
     # state.save_svg("tmp.svg")
     state = _step_det(state, 0,
                       enemy_lr=True,
                       is_sub=False,
                       enemy_y=4,
                       diver_lr=True,
                       diver_y=7
                       )
     # print(state.f_bullets)
     print("e_bullets")
-    print(state.e_bullets)
+    print(state._e_bullets)
     # print(state.e_fish)
     print("e_subs")
-    print(state.e_subs)
-    assert (state.e_bullets[0] == jnp.int32([-1, -1, -1])).all()
-    assert (state.e_subs[0] == jnp.int32([6, 6, 0, 2, 0])).all()
+    print(state._e_subs)
+    assert (state._e_bullets[0] == jnp.int32([-1, -1, -1])).all()
+    assert (state._e_subs[0] == jnp.int32([6, 6, 0, 2, 0])).all()
 
 
 def test_api():
     import pgx
     env = pgx.make("minatar/seaquest")
     pgx.api_test(env, 10)
```

### Comparing `pgx-0.5.1/tests/test_shogi.py` & `pgx-0.5.2/tests/test_shogi.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         state = state.replace(hand=hand)
     return state
 
 
 def test_init():
     key = jax.random.PRNGKey(0)
     s = init(key)
-    assert jnp.unique(s.piece_board).shape[0] == 1 + 8 + 8
+    assert jnp.unique(s._board).shape[0] == 1 + 8 + 8
     assert s.legal_action_mask.sum() != 0
     legal_actions = jnp.int32([5, 7, 14, 23, 25, 32, 34, 41, 43, 50, 52, 59, 61, 68, 77, 79, 115, 124, 133, 142, 187, 196, 205, 214, 268, 277, 286, 295, 304, 331])
     assert (jnp.nonzero(s.legal_action_mask)[0] == legal_actions).all(), jnp.nonzero(s.legal_action_mask)[0]
 
 
 def test_is_legal_drop():
     # 打ち歩詰
@@ -111,15 +111,15 @@
     visualize(state, "tests/assets/shogi/buggy_samples_005.svg")
     dlshogi_action = 846
     state = step(state, dlshogi_action)
     visualize(state, "tests/assets/shogi/buggy_samples_006.svg")
     sfen = "4+R4/9/9/9/9/9/9/9/9 w 2r2b4g3s4n4l7p 1"
     expected_state = State._from_sfen(sfen)
     visualize(expected_state, "tests/assets/shogi/buggy_samples_006.svg")
-    assert (state.piece_board == expected_state.piece_board).all()
+    assert (state._board == expected_state._board).all()
 
     # #603
     state = State._from_sfen("8k/9/9/5b3/9/3B5/9/9/K8 b 2r4g4s4n4l18p 1")
     visualize(state, "tests/assets/shogi/buggy_samples_007.svg")
     dlshogi_action = 202
     a = Action._from_dlshogi_action(state, dlshogi_action)
     assert a.from_ == xy2i(6, 6)
@@ -129,36 +129,36 @@
     visualize(state, "tests/assets/shogi/buggy_samples_008.svg")
     dlshogi_action = 225
     a = Action._from_dlshogi_action(state, dlshogi_action)
     assert a.from_ == xy2i(9, 2)
     assert a.piece == HORSE
     state = step(state, dlshogi_action)
     expected_state = State._from_sfen("+P+BGg1p2+P/2+Pgp+N1sp/1+N5l1/P3kP1pL/3P1r3/B2KP3L/4L1SP+s/+r2+p2pgP/2P2+n+p2 w Snp 1")
-    assert (state.piece_board == expected_state.piece_board).all()
+    assert (state._board == expected_state._board).all()
 
     # #613
     state = State._from_sfen("1+N3s1n1/5k2l/l+P2g1bp1/2pP1p2p/p2ppNS2/LB6P/1pS1g2PL/3KPR2S/1R1G1NG2 b P4p 1")
     visualize(state, "tests/assets/shogi/buggy_samples_009.svg")
     dlshogi_action = 42
     a = Action._from_dlshogi_action(state, dlshogi_action)
     assert a.from_ == xy2i(5, 8)
     assert a.piece == PAWN
     state = step(state, dlshogi_action)
     expected_state = State._from_sfen("1+N3s1n1/5k2l/l+P2g1bp1/2pP1p2p/p2ppNS2/LB6P/1pS1P2PL/3K1R2S/1R1G1NG2 w GP4p 1")
-    assert (state.piece_board == expected_state.piece_board).all()
+    assert (state._board == expected_state._board).all()
 
     # #618
     state = State._from_sfen("2+P+P2G1+S/1P2+P+P1+Pn/+S1GK2P2/1b2PP3/1nl4PP/3k2lRL/1pg+s3L1/p2R2p2/P+n+B+p+ng1+s+p w P 1")
     visualize(state, "tests/assets/shogi/buggy_samples_010.svg")
     dlshogi_action = 28
     a = Action._from_dlshogi_action(state, dlshogi_action)
     assert a.from_ == xy2i(4, 3)
     state = step(state, dlshogi_action)
     expected_state = State._from_sfen("2+P+P2G1+S/1P2+P+P1+Pn/+S1GK2P2/1b2PP3/1nl4PP/3k2lRL/1pg4L1/p2+s2p2/P+n+B+p+ng1+s+p b Pr 1")
-    assert (state.piece_board == expected_state.piece_board).all()
+    assert (state._board == expected_state._board).all()
 
     # 629
     state = State._from_sfen("1ns6/+S1p+Ng1p1l/+P2pg1nNS/4k2G1/2L2R2s/p1G2+BPR1/3Pp2+p1/1+p3B1P1/1LPK2+l1+p b P4p 1")
     visualize(state, "tests/assets/shogi/buggy_samples_011.svg")
     dlshogi_action = 1660  # 歩打
     state = step(state, dlshogi_action)
     visualize(state, "tests/assets/shogi/buggy_samples_012.svg")
```

### Comparing `pgx-0.5.1/tests/test_space_invaders.py` & `pgx-0.5.2/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/tests/test_sparrow_mahjong.py` & `pgx-0.5.2/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.1/tests/test_tic_tac_toe.py` & `pgx-0.5.2/tests/test_tic_tac_toe.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,98 +15,98 @@
     assert state.current_player == 1
 
 
 def test_step():
     key = jax.random.PRNGKey(1)
     state = init(key=key)
     assert state.current_player == 1
-    assert state.turn == 0
+    assert state._turn == 0
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([1, 1, 1, 1, 1, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(
-        state.board == jnp.int8([-1, -1, -1, -1, -1, -1, -1, -1, -1])
+        state._board == jnp.int8([-1, -1, -1, -1, -1, -1, -1, -1, -1])
     )
     assert not state.terminated
     # -1 -1 -1
     # -1 -1 -1
     # -1 -1 -1
 
     action = jnp.int8(4)
     state = step(state, action)
     assert state.current_player == 0
-    assert state.turn == 1
+    assert state._turn == 1
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([1, 1, 1, 1, 0, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(
-        state.board == jnp.int8([-1, -1, -1, -1, 0, -1, -1, -1, -1])
+        state._board == jnp.int8([-1, -1, -1, -1, 0, -1, -1, -1, -1])
     )
     assert jnp.all(state.reward == 0)  # fmt: ignore
     assert not state.terminated
     # -1 -1 -1
     # -1  0 -1
     # -1 -1 -1
 
     action = jnp.int8(0)
     state = step(state, action)
     assert state.current_player == 1
-    assert state.turn == 0
+    assert state._turn == 0
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([0, 1, 1, 1, 0, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
-    assert jnp.all(state.board == jnp.int8([1, -1, -1, -1, 0, -1, -1, -1, -1]))
+    assert jnp.all(state._board == jnp.int8([1, -1, -1, -1, 0, -1, -1, -1, -1]))
     assert jnp.all(state.reward == 0)  # fmt: ignore
     assert not state.terminated
     #  1 -1 -1
     # -1  0 -1
     # -1 -1 -1
 
     action = jnp.int8(1)
     state = step(state, action)
     assert state.current_player == 0
-    assert state.turn == 1
+    assert state._turn == 1
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([0, 0, 1, 1, 0, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
-    assert jnp.all(state.board == jnp.int8([1, 0, -1, -1, 0, -1, -1, -1, -1]))
+    assert jnp.all(state._board == jnp.int8([1, 0, -1, -1, 0, -1, -1, -1, -1]))
     assert jnp.all(state.reward == 0)  # fmt: ignore
     assert not state.terminated
     #  1  0 -1
     # -1  0 -1
     # -1 -1 -1
 
     action = jnp.int8(8)
     state = step(state, action)
     assert state.current_player == 1
-    assert state.turn == 0
+    assert state._turn == 0
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([0, 0, 1, 1, 0, 1, 1, 1, 0], jnp.bool_)
     )  # fmt: ignore
-    assert jnp.all(state.board == jnp.int8([1, 0, -1, -1, 0, -1, -1, -1, 1]))
+    assert jnp.all(state._board == jnp.int8([1, 0, -1, -1, 0, -1, -1, -1, 1]))
     assert jnp.all(state.reward == 0)  # fmt: ignore
     assert not state.terminated
     #  1  0 -1
     # -1  0 -1
     # -1 -1  1
 
     action = jnp.int8(7)
     state = step(state, action)
     assert state.current_player == 0
-    assert state.turn == 1
+    assert state._turn == 1
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([1, 1, 1, 1, 1, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
-    assert jnp.all(state.board == jnp.int8([1, 0, -1, -1, 0, -1, -1, 0, 1]))
+    assert jnp.all(state._board == jnp.int8([1, 0, -1, -1, 0, -1, -1, 0, 1]))
     assert jnp.all(state.reward == jnp.int16([-1, 1]))  # fmt: ignore
     assert state.terminated
     #  1  0 -1
     # -1  0 -1
     # -1  0  1
 
 
@@ -115,15 +115,15 @@
     key = jax.random.PRNGKey(0)
     for i in range(N):
         done = jnp.bool_(False)
         key, sub_key = jax.random.split(key)
         state = init(sub_key)
         rewards = jnp.int16([0.0, 0.0])
         while not done:
-            assert jnp.all(rewards == 0), state.board
+            assert jnp.all(rewards == 0), state._board
             legal_actions = jnp.where(state.legal_action_mask)[0]
             key, sub_key = jax.random.split(key)
             action = jax.random.choice(sub_key, legal_actions)
             state = step(state, action)
             done = state.terminated
             rewards += state.reward
```

