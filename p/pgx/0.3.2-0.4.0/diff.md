# Comparing `tmp/pgx-0.3.2.tar.gz` & `tmp/pgx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.3.2.tar", last modified: Thu Apr 20 11:48:47 2023, max compression
+gzip compressed data, was "pgx-0.4.0.tar", last modified: Fri Apr 21 06:04:10 2023, max compression
```

## Comparing `pgx-0.3.2.tar` & `pgx-0.4.0.tar`

### file list

```diff
@@ -1,139 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.836676 pgx-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 11:48:35.000000 pgx-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 11:48:47.836676 pgx-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-20 11:48:35.000000 pgx-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.820675 pgx-0.3.2/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.824675 pgx-0.3.2/pgx/_dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.824675 pgx-0.3.2/pgx/_dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.824675 pgx-0.3.2/pgx/_dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.828676 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_dwg/tictactoe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.828676 pgx-0.3.2/pgx/_flax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_flax/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.828676 pgx-0.3.2/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    44184 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28934 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.832676 pgx-0.3.2/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.832676 pgx-0.3.2/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25917 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-20 11:48:35.000000 pgx-0.3.2/pgx/tic_tac_toe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.820675 pgx-0.3.2/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 11:48:47.000000 pgx-0.3.2/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-20 11:48:35.000000 pgx-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:48:47.836676 pgx-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 11:48:35.000000 pgx-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:47.836676 pgx-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61403 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-20 11:48:35.000000 pgx-0.3.2/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.436420 pgx-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 06:04:00.000000 pgx-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-21 06:04:10.436420 pgx-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-21 06:04:00.000000 pgx-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.420420 pgx-0.4.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.424420 pgx-0.4.0/pgx/_dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.424420 pgx-0.4.0/pgx/_dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.424420 pgx-0.4.0/pgx/_dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.428420 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_dwg/tictactoe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.428420 pgx-0.4.0/pgx/_flax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_flax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_flax/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.428420 pgx-0.4.0/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-21 06:04:00.000000 pgx-0.4.0/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/_shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28922 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.432420 pgx-0.4.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.432420 pgx-0.4.0/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-21 06:04:01.000000 pgx-0.4.0/pgx/tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.420420 pgx-0.4.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-21 06:04:10.000000 pgx-0.4.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-21 06:04:10.000000 pgx-0.4.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:04:10.000000 pgx-0.4.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 06:04:10.000000 pgx-0.4.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 06:04:10.000000 pgx-0.4.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-21 06:04:01.000000 pgx-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:04:10.436420 pgx-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-21 06:04:01.000000 pgx-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:10.436420 pgx-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61403 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-21 06:04:01.000000 pgx-0.4.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.3.2/LICENSE` & `pgx-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/README.md` & `pgx-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_cache.py` & `pgx-0.4.0/pgx/_cache.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_chess_utils.py` & `pgx-0.4.0/pgx/_chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/animalshogi.py` & `pgx-0.4.0/pgx/_dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/backgammon.py` & `pgx-0.4.0/pgx/_dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/bridge_bidding.py` & `pgx-0.4.0/pgx/_dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/chess.py` & `pgx-0.4.0/pgx/_dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/connect_four.py` & `pgx-0.4.0/pgx/_dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/go.py` & `pgx-0.4.0/pgx/_dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/hex.py` & `pgx-0.4.0/pgx/_dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/LICENSE` & `pgx-0.4.0/pgx/_dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/bBishop.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/bKing.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/bKnight.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/bPawn.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/bQueen.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/bRook.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/wBishop.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/wKing.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/wKnight.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/wPawn.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/wQueen.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/chess/wRook.svg` & `pgx-0.4.0/pgx/_dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/b.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.4.0/pgx/_dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/kuhn_poker.py` & `pgx-0.4.0/pgx/_dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/leduc_holdem.py` & `pgx-0.4.0/pgx/_dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/othello.py` & `pgx-0.4.0/pgx/_dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/play2048.py` & `pgx-0.4.0/pgx/_dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/shogi.py` & `pgx-0.4.0/pgx/_dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/sparrow_mahjong.py` & `pgx-0.4.0/pgx/_dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_dwg/tictactoe.py` & `pgx-0.4.0/pgx/_dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_flax/serialization.py` & `pgx-0.4.0/pgx/_flax/serialization.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_mahjong/_hand.py` & `pgx-0.4.0/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_shogi_utils.py` & `pgx-0.4.0/pgx/_shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/_test.py` & `pgx-0.4.0/pgx/_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     prev_state = state
     if not state.terminated:
         return
     action = 0
     state = step_fn(state, action)
     assert (state.reward == 0).all()
     for field in fields(state):
-        if field.name in ["reward", "steps", "_info"]:
+        if field.name in ["reward", "steps"]:
             continue
         assert (
             getattr(state, field.name) == getattr(prev_state, field.name)
         ).all(), f"{field.name} : \n{getattr(state, field.name)}\n{getattr(prev_state, field.name)}"
 
 
 def _validate_init_reward(state: State):
```

### Comparing `pgx-0.3.2/pgx/_visualizer.py` & `pgx-0.4.0/pgx/_visualizer.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/animal_shogi.py` & `pgx-0.4.0/pgx/animal_shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from functools import partial
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 EMPTY = jnp.int8(-1)
 PAWN = jnp.int8(0)
```

### Comparing `pgx-0.3.2/pgx/backgammon.py` & `pgx-0.4.0/pgx/backgammon.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 @dataclass
 class State(core.State):
```

### Comparing `pgx-0.3.2/pgx/bridge_bidding.py` & `pgx-0.4.0/pgx/bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 import copy
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 # カードと数字の対応
 # 0~12 spade, 13~25 heart, 26~38 diamond, 39~51 club
 # それぞれのsuitにおいて以下の順で数字が並ぶ
```

### Comparing `pgx-0.3.2/pgx/chess.py` & `pgx-0.4.0/pgx/chess.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
 from pgx._chess_utils import (  # type: ignore
     BETWEEN,
     CAN_MOVE,
     CAN_MOVE_ANY,
     HASH_TABLE,
     INIT_LEGAL_ACTION_MASK,
     INIT_POSSIBLE_PIECE_POSITIONS,
     PLANE_MAP,
     TO_MAP,
 )
-from pgx._flax.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 EMPTY = jnp.int8(0)
 PAWN = jnp.int8(1)
 KNIGHT = jnp.int8(2)
```

### Comparing `pgx-0.3.2/pgx/connect_four.py` & `pgx-0.4.0/pgx/connect_four.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(core.State):
```

### Comparing `pgx-0.3.2/pgx/core.py` & `pgx-0.4.0/pgx/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
-from typing import Any, Dict, Literal, Optional, Tuple, get_args
+from typing import Literal, Optional, Tuple, get_args
 
 import jax
 import jax.numpy as jnp
-
-from pgx._flax.struct import dataclass, field
+from chex import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 # Pgx environments are versioned like OpenAI Gym or Brax.
 # OpenAI Gym forces user to specify version (e.g., `MountainCar-v0`); while Brax does not (e.g., `ant`)
@@ -55,67 +54,142 @@
     "sparrow_mahjong",
     "tic_tac_toe",
 ]
 
 
 @dataclass
 class State(abc.ABC):
+    """Base state class of all Pgx game environments. Basically an immutable (frozen) dataclass.
+    A basic usage is generating via `Env.init`:
+
+        state = env.init(jax.random.PRNGKey(0))
+
+    and `Env.step` receives and returns this state class:
+
+        state = env.step(state, action)
+
+    There are 6 common attributes over all games:
+
+    Attributes:
+        current_player (jnp.ndarray): id of agent to play.
+            Note that this does NOT represent the turn (e.g., black/white in Go).
+            This ID is consistent over the parallel vmapped states.
+        observation (jnp.ndarray): observation for the current state.
+            `Env.observe` is called to compute.
+        reward (jnp.ndarray): the `i`-th element indicates the intermediate reward for
+            the agent with player-id `i`. If `Env.step` is called for a terminal state,
+            the following `state.reward` is zero for all players.
+        terminated (jnp.ndarray): denotes that the state is termianl state. Note that
+            some environments (e.g., Go) have an `max_termination_steps` parameter inside
+            and will terminates within a limited number of states (following AlphaGo).
+        truncated (jnp.ndarray): so far, not used as all Pgx environments are finite horizon
+        legal_action_mask (jnp.ndarray): Boolean array of legal actions. If illegal action is taken,
+            the game will terminate immediately with the penalty to the palyer.
+    """
+
     current_player: jnp.ndarray
     observation: jnp.ndarray
     reward: jnp.ndarray
     terminated: jnp.ndarray
     truncated: jnp.ndarray  # so far, not used as all Pgx environments are finite horizon
     legal_action_mask: jnp.ndarray
     # NOTE: _rng_key is
     #   - used for stochastic env and auto reset
     #   - updated only when actually used
     #   - supposed NOT to be used by agent
     _rng_key: jax.random.KeyArray
     _step_count: jnp.ndarray
-    _info: Dict[str, Any] = field(default_factory=dict)  # experimental
 
     @property
     @abc.abstractmethod
     def env_id(self) -> EnvId:
+        """Environment id (e.g. "go-19x19")"""
         ...
 
     def _repr_html_(self) -> str:
+        return self.to_svg()
+
+    def to_svg(
+        self,
+        *,
+        color_theme: Optional[Literal["light", "dark"]] = None,
+        scale: Optional[float] = None,
+    ) -> str:
+        """Return SVG string. Useful for visualization in notebook.
+
+        Args:
+            color_theme (Optional[Literal["light", "dark"]]): xxx see also global config.
+            scale (Optional[float]): change image size. Default(None) is 1.0
+
+        Returns:
+            str: SVG string
+        """
         from pgx._visualizer import Visualizer
 
-        v = Visualizer()
+        v = Visualizer(color_theme=color_theme, scale=scale)
         return v.get_dwg(states=self).tostring()
 
     def save_svg(
         self,
         filename,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
-        """
-        color_theme: Default(None) is "light"
-        scale: change image size. Default(None) is 1.0
+        """Save the entire state (not observation) to a file.
+        The filename must end with `.svg`
+
+        Args:
+            color_theme (Optional[Literal["light", "dark"]]): xxx see also global config.
+            scale (Optional[float]): change image size. Default(None) is 1.0
+
+        Returns:
+            None
         """
         from pgx._visualizer import save_svg
 
         save_svg(self, filename, color_theme=color_theme, scale=scale)
 
 
 class Env(abc.ABC):
+    """Environment class API.
+
+    !!! example "Example usage"
+
+        ```py
+        env: Env = pgx.make("tic_tac_toe")
+        state = env.init(jax.random.PRNGKey(0))
+        action = jax.random.int32(4)
+        state = env.step(state, action)
+        ```
+
+    """
+
     def __init__(self):
         ...
 
     def init(self, key: jax.random.KeyArray) -> State:
+        """Return the initial state. Note that no internal state of
+        environment changes.
+
+        Args:
+            key: pseudo-random generator key in JAX
+
+        Returns:
+            State: initial state of environment
+
+        """
         key, subkey = jax.random.split(key)
         state = self._init(subkey)
         state = state.replace(_rng_key=key)  # type: ignore
         observation = self.observe(state, state.current_player)
         return state.replace(observation=observation)  # type: ignore
 
     def step(self, state: State, action: jnp.ndarray) -> State:
+        """Step function."""
         is_illegal = ~state.legal_action_mask[action]
         current_player = state.current_player
 
         # If the state is already terminated or truncated, environment does not take usual step,
         # but return the same state with zero-rewards for all players
         state = jax.lax.cond(
             (state.terminated | state.truncated),
@@ -141,14 +215,15 @@
             lambda: state,
         )
 
         observation = self.observe(state, state.current_player)
         return state.replace(observation=observation)  # type: ignore
 
     def observe(self, state: State, player_id: jnp.ndarray) -> jnp.ndarray:
+        """Observation function."""
         obs = self._observe(state, player_id)
         return jax.lax.stop_gradient(obs)
 
     @abc.abstractmethod
     def _init(self, key: jax.random.KeyArray) -> State:
         """Implement game-specific init function here."""
         ...
@@ -167,35 +242,39 @@
     @abc.abstractmethod
     def name(self) -> str:
         ...
 
     @property
     @abc.abstractmethod
     def version(self) -> str:
+        """Environment version. Updated when behavior, parameter, or API is changed.
+        Refactoring or speeding up without any expected behavior changes will NOT update the version number.
+        """
         ...
 
     @property
     @abc.abstractmethod
     def num_players(self) -> int:
+        """Number of players (e.g., 2 in Tic-tac-toe)"""
         ...
 
     @property
+    def num_actions(self) -> int:
+        """Return the size of action space (e.g., 9 in Tic-tac-toe)"""
+        state = self.init(jax.random.PRNGKey(0))
+        return int(state.legal_action_mask.shape[0])
+
+    @property
     def observation_shape(self) -> Tuple[int, ...]:
         """Return the matrix shape of observation"""
         state = self.init(jax.random.PRNGKey(0))
         obs = self._observe(state, state.current_player)
         return obs.shape
 
     @property
-    def action_shape(self) -> Tuple[int, ...]:
-        """Return the matrix shape of legal_action_mask"""
-        state = self.init(jax.random.PRNGKey(0))
-        return state.legal_action_mask.shape
-
-    @property
     def _illegal_action_penalty(self) -> float:
         """Negative reward given when illegal action is selected."""
         return -1.0
 
     def _step_with_illegal_action(
         self, state: State, loser: jnp.ndarray
     ) -> State:
```

### Comparing `pgx-0.3.2/pgx/experimental/bridge_bidding.py` & `pgx-0.4.0/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/experimental/gym.py` & `pgx-0.4.0/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/experimental/pettingzoo.py` & `pgx-0.4.0/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/experimental/visualize.py` & `pgx-0.4.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/experimental/wrappers.py` & `pgx-0.4.0/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/go.py` & `pgx-0.4.0/pgx/go.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from functools import partial
 
 import jax
+from chex import dataclass
 from jax import numpy as jnp
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(core.State):
```

### Comparing `pgx-0.3.2/pgx/hex.py` & `pgx-0.4.0/pgx/hex.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(core.State):
```

### Comparing `pgx-0.3.2/pgx/kuhn_poker.py` & `pgx-0.4.0/pgx/kuhn_poker.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 CALL = jnp.int8(0)
 BET = jnp.int8(1)
 FOLD = jnp.int8(2)
 CHECK = jnp.int8(3)
```

### Comparing `pgx-0.3.2/pgx/leduc_holdem.py` & `pgx-0.4.0/pgx/leduc_holdem.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 INVALID_ACTION = jnp.int8(-1)
 CALL = jnp.int8(0)
 RAISE = jnp.int8(1)
```

### Comparing `pgx-0.3.2/pgx/minatar/asterix.py` & `pgx-0.4.0/pgx/minatar/asterix.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     * Tian Tian (ttian@ualberta.ca)
 The original MinAtar implementation is distributed under GNU General Public License v3.0
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
+from chex import dataclass
 from jax import numpy as jnp
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 ramp_interval: jnp.ndarray = jnp.array(100, dtype=jnp.int32)
 init_spawn_speed: jnp.ndarray = jnp.array(10, dtype=jnp.int32)
 init_move_interval: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
 shot_cool_down: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
 INF: jnp.ndarray = jnp.array(99, dtype=jnp.int32)
```

### Comparing `pgx-0.3.2/pgx/minatar/breakout.py` & `pgx-0.4.0/pgx/minatar/breakout.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     * Tian Tian (ttian@ualberta.ca)
 The original MinAtar implementation is distributed under GNU General Public License v3.0
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
+from chex import dataclass
 from jax import numpy as jnp
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 ZERO = jnp.array(0, dtype=jnp.int32)
 ONE = jnp.array(1, dtype=jnp.int32)
 TWO = jnp.array(2, dtype=jnp.int32)
 THREE = jnp.array(3, dtype=jnp.int32)
```

### Comparing `pgx-0.3.2/pgx/minatar/freeway.py` & `pgx-0.4.0/pgx/minatar/freeway.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     * Tian Tian (ttian@ualberta.ca)
 The original MinAtar implementation is distributed under GNU General Public License v3.0
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
+from chex import dataclass
 from jax import numpy as jnp
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 player_speed = jnp.array(3, dtype=jnp.int32)
 time_limit = jnp.array(2500, dtype=jnp.int32)
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 ZERO = jnp.array(0, dtype=jnp.int32)
```

### Comparing `pgx-0.3.2/pgx/minatar/seaquest.py` & `pgx-0.4.0/pgx/minatar/seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 The original MinAtar implementation is distributed under GNU General Public License v3.0
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
 import jax.lax as lax
+from chex import dataclass
 from jax import numpy as jnp
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 RAMP_INTERVAL: jnp.ndarray = jnp.int32(100)
 MAX_OXYGEN: jnp.ndarray = jnp.int32(200)
 INIT_SPAWN_SPEED: jnp.ndarray = jnp.int32(20)
 DIVER_SPAWN_SPEED: jnp.ndarray = jnp.int32(30)
 INIT_MOVE_INTERVAL: jnp.ndarray = jnp.int32(5)
 SHOT_COOL_DOWN: jnp.ndarray = jnp.int32(5)
```

### Comparing `pgx-0.3.2/pgx/minatar/space_invaders.py` & `pgx-0.4.0/pgx/minatar/space_invaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 The original MinAtar implementation is distributed under GNU General Public License v3.0
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
 import jax.lax as lax
+from chex import dataclass
 from jax import numpy as jnp
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 SHOT_COOL_DOWN = jnp.int32(5)
 ENEMY_MOVE_INTERVAL = jnp.int32(12)
 ENEMY_SHOT_INTERVAL = jnp.int32(10)
```

### Comparing `pgx-0.3.2/pgx/minatar/utils.py` & `pgx-0.4.0/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/pgx/othello.py` & `pgx-0.4.0/pgx/othello.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(core.State):
```

### Comparing `pgx-0.3.2/pgx/play2048.py` & `pgx-0.4.0/pgx/play2048.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 ZERO = jnp.int8(0)
 
 
 @dataclass
```

### Comparing `pgx-0.3.2/pgx/shogi.py` & `pgx-0.4.0/pgx/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 from pgx._shogi_utils import (
     AROUND_IX,
     BETWEEN_IX,
     CAN_MOVE,
     CAN_MOVE_ANY,
     INIT_LEGAL_ACTION_MASK,
     INIT_PIECE_BOARD,
```

### Comparing `pgx-0.3.2/pgx/sparrow_mahjong.py` & `pgx-0.4.0/pgx/sparrow_mahjong.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     * ロン・ツモは自動判定
   * 誰も一つも行動を取らずにエピソードが終わるのを避けるため、親の第一ツモでの和了の場合は配牌し直し（天和を避けている）
 """
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 NUM_TILES = 44
 NUM_TILE_TYPES = 11
 N_PLAYER = 3
 MAX_RIVER_LENGTH = 10
```

### Comparing `pgx-0.3.2/pgx/tic_tac_toe.py` & `pgx-0.4.0/pgx/tic_tac_toe.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
+from chex import dataclass
 
 import pgx.core as core
-from pgx._flax.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(core.State):
     current_player: jnp.ndarray = jnp.int8(0)
-    observation: jnp.ndarray = jnp.zeros(27, dtype=jnp.bool_)
+    observation: jnp.ndarray = jnp.zeros((3, 3, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Tic-tac-toe specific ---
@@ -101,18 +101,19 @@
 
 def _win_check(board, turn) -> jnp.ndarray:
     idx = jnp.int8([[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]])  # type: ignore
     return ((board[idx] == turn).all(axis=1)).any()
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
-    empty_board = state.board == -1
-    my_board, opp_obard = jax.lax.cond(
-        state.current_player
-        == player_id,  # flip board if player_id is opposite
-        lambda: (state.turn == state.board, (1 - state.turn) == state.board),
-        lambda: ((1 - state.turn) == state.board, state.turn == state.board),
-    )
-    return jnp.concatenate(
-        [empty_board, my_board, opp_obard],
-        dtype=jnp.bool_,
+    @jax.vmap
+    def plane(i):
+        return (state.board == i).reshape((3, 3))
+
+    # flip if player_id is opposite
+    x = jax.lax.cond(
+        state.current_player == player_id,
+        lambda: jnp.int8([state.turn, 1 - state.turn]),
+        lambda: jnp.int8([1 - state.turn, state.turn]),
     )
+
+    return jnp.stack(plane(x), -1)
```

### Comparing `pgx-0.3.2/pgx.egg-info/SOURCES.txt` & `pgx-0.4.0/pgx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 pgx/_dwg/images/sparrow_mahjong/__init__.py
 pgx/_dwg/images/sparrow_mahjong/b.svg
 pgx/_dwg/images/sparrow_mahjong/gd.svg
 pgx/_dwg/images/sparrow_mahjong/oya.svg
 pgx/_dwg/images/sparrow_mahjong/rd.svg
 pgx/_flax/__init__.py
 pgx/_flax/serialization.py
-pgx/_flax/struct.py
 pgx/_mahjong/__init__.py
 pgx/_mahjong/_action.py
 pgx/_mahjong/_hand.py
 pgx/experimental/__init__.py
 pgx/experimental/bridge_bidding.py
 pgx/experimental/gym.py
 pgx/experimental/pettingzoo.py
```

### Comparing `pgx-0.3.2/setup.py` & `pgx-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pgx",
-    version="0.3.2",
+    version="0.4.0",
     long_description_content_type="text/markdown",
     description="",
     url="",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
     package_data={"": ["LICENSE", "*.svg"]},
     include_package_data=True,
-    install_requires=["jax", "svgwrite", "ipywidgets", "msgpack"],
+    install_requires=[
+        "jax>=0.3.25",  # JAX version on Colab (TPU)
+        "chex>=0.1.6",
+        "svgwrite",
+        "msgpack",
+        "typing_extensions"
+    ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `pgx-0.3.2/tests/minatar_utils.py` & `pgx-0.4.0/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_animal_shogi.py` & `pgx-0.4.0/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_asterix.py` & `pgx-0.4.0/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_backgammon.py` & `pgx-0.4.0/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_breakout.py` & `pgx-0.4.0/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_bridge_bidding.py` & `pgx-0.4.0/tests/test_bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_chess.py` & `pgx-0.4.0/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_connect_four.py` & `pgx-0.4.0/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_freeway.py` & `pgx-0.4.0/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_go.py` & `pgx-0.4.0/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_hex.py` & `pgx-0.4.0/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_kuhn_poker.py` & `pgx-0.4.0/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_leduc_holdem.py` & `pgx-0.4.0/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_mahjong.py` & `pgx-0.4.0/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_othello.py` & `pgx-0.4.0/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_play2048.py` & `pgx-0.4.0/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_seaquest.py` & `pgx-0.4.0/tests/test_seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,14 @@
     N = 100
     for _ in range(N):
         env.reset()
         s = extract_state(env, state_keys)
         s_pgx = _init_det()
         s_pgx2 = minatar2pgx(s, seaquest.State)
         for field in fields(s_pgx):
-            if field.name == '_info':
-                continue
             assert jnp.allclose(getattr(s_pgx, field.name), getattr(s_pgx2, field.name))
 
 
 def test_observe():
     env = Environment("seaquest", sticky_action_prob=0.0)
     num_actions = env.num_actions()
```

### Comparing `pgx-0.3.2/tests/test_shogi.py` & `pgx-0.4.0/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_space_invaders.py` & `pgx-0.4.0/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_sparrow_mahjong.py` & `pgx-0.4.0/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.3.2/tests/test_tic_tac_toe.py` & `pgx-0.4.0/tests/test_tic_tac_toe.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,22 +173,23 @@
     turn = jnp.int8(0)
     assert _win_check(board, turn)
 
 
 def test_observe():
     state = init(jax.random.PRNGKey(1))
     obs = observe(state, state.current_player)
-    init_obs = jnp.zeros(27).at[:9].set(1)
+    init_obs = jnp.zeros([3, 3, 2])
     assert (obs == init_obs).all()
 
-    state = step(state, 0)
+    state = step(state, 1)
+    assert state.current_player == 0
     obs = observe(state, 0)
-    assert (obs == init_obs.at[0].set(0).at[18].set(1)).all(), obs
+    assert (obs == init_obs.at[0, 1, 1].set(1)).all(), obs
     obs = observe(state, 1)
-    assert (obs == init_obs.at[0].set(0).at[9].set(1)).all(), obs
+    assert (obs == init_obs.at[0, 1, 0].set(1)).all(), obs
 
 
 
 def test_api():
     import pgx
     env = pgx.make("tic_tac_toe")
     pgx.api_test(env, 10)
```

