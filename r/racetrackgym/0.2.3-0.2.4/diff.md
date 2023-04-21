# Comparing `tmp/racetrackgym-0.2.3.tar.gz` & `tmp/racetrackgym-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racetrackgym-0.2.3.tar", max compression
+gzip compressed data, was "racetrackgym-0.2.4.tar", max compression
```

## Comparing `racetrackgym-0.2.3.tar` & `racetrackgym-0.2.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0       13 2021-12-14 09:58:20.666537 racetrackgym-0.2.3/README.md
--rw-r--r--   0        0        0      845 2022-06-23 12:31:32.602261 racetrackgym-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       22 2021-12-14 09:58:20.667966 racetrackgym-0.2.3/racetrackgym/__init__.py
--rw-r--r--   0        0        0     2993 2022-06-17 11:33:14.851828 racetrackgym-0.2.3/racetrackgym/argument_parser.py
--rw-r--r--   0        0        0    25555 2022-06-23 12:29:18.375440 racetrackgym-0.2.3/racetrackgym/environment.py
--rw-r--r--   0        0        0     9082 2021-12-14 09:58:20.668411 racetrackgym-0.2.3/racetrackgym/evaluator.py
--rw-r--r--   0        0        0     5594 2021-12-14 09:58:20.668582 racetrackgym-0.2.3/racetrackgym/graphic.py
--rw-r--r--   0        0        0     1034 2021-12-14 09:58:20.668794 racetrackgym-0.2.3/racetrackgym/maps/barto-big.track
--rw-r--r--   0        0        0    99343 2021-12-14 09:58:20.669071 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_10.track
--rw-r--r--   0        0        0     4037 2021-12-14 09:58:20.669181 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_2.track
--rw-r--r--   0        0        0     9020 2021-12-14 09:58:20.669325 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_3.track
--rw-r--r--   0        0        0    15985 2021-12-14 09:58:20.669447 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_4.track
--rw-r--r--   0        0        0    24928 2021-12-14 09:58:20.669672 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_5.track
--rw-r--r--   0        0        0    35851 2021-12-14 09:58:20.669808 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_6.track
--rw-r--r--   0        0        0    48754 2021-12-14 09:58:20.670076 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_7.track
--rw-r--r--   0        0        0    63637 2021-12-14 09:58:20.670320 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_8.track
--rw-r--r--   0        0        0    80500 2021-12-14 09:58:20.670570 racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_9.track
--rw-r--r--   0        0        0      442 2021-12-14 09:58:20.670766 racetrackgym-0.2.3/racetrackgym/maps/barto-small.track
--rw-r--r--   0        0        0     1715 2021-12-14 09:58:20.671067 racetrackgym-0.2.3/racetrackgym/maps/barto-small_scales/barto-small_scaled_2.track
--rw-r--r--   0        0        0     6780 2021-12-14 09:58:20.671259 racetrackgym-0.2.3/racetrackgym/maps/barto-small_scales/barto-small_scaled_4.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.671499 racetrackgym-0.2.3/racetrackgym/maps/corner/1-2-3.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.671672 racetrackgym-0.2.3/racetrackgym/maps/corner/1-4-3.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.671884 racetrackgym-0.2.3/racetrackgym/maps/corner/2-1-4.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.671970 racetrackgym-0.2.3/racetrackgym/maps/corner/2-3-4.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.672055 racetrackgym-0.2.3/racetrackgym/maps/corner/3-2-1.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.672237 racetrackgym-0.2.3/racetrackgym/maps/corner/3-4-1.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.672411 racetrackgym-0.2.3/racetrackgym/maps/corner/4-1-2.track
--rw-r--r--   0        0        0      660 2021-12-14 09:58:20.672522 racetrackgym-0.2.3/racetrackgym/maps/corner/4-3-2.track
--rw-r--r--   0        0        0      470 2021-12-14 09:58:20.672707 racetrackgym-0.2.3/racetrackgym/maps/diverse/barrier.txt
--rw-r--r--   0        0        0      430 2021-12-14 09:58:20.672791 racetrackgym-0.2.3/racetrackgym/maps/diverse/bottleneck.txt
--rw-r--r--   0        0        0      550 2021-12-14 09:58:20.672897 racetrackgym-0.2.3/racetrackgym/maps/diverse/corner.txt
--rw-r--r--   0        0        0      550 2021-12-14 09:58:20.672994 racetrackgym-0.2.3/racetrackgym/maps/diverse/diagonal.txt
--rw-r--r--   0        0        0      310 2021-12-14 09:58:20.673099 racetrackgym-0.2.3/racetrackgym/maps/diverse/pyramid.txt
--rw-r--r--   0        0        0      295 2021-12-14 09:58:20.673305 racetrackgym-0.2.3/racetrackgym/maps/diverse/ring.txt
--rw-r--r--   0        0        0      520 2021-12-14 09:58:20.673442 racetrackgym-0.2.3/racetrackgym/maps/diverse/spiral.txt
--rw-r--r--   0        0        0      550 2021-12-14 09:58:20.673527 racetrackgym-0.2.3/racetrackgym/maps/diverse/straighton.txt
--rw-r--r--   0        0        0      586 2021-12-14 09:58:20.673612 racetrackgym-0.2.3/racetrackgym/maps/diverse/uturn.txt
--rw-r--r--   0        0        0      582 2021-12-14 09:58:20.673702 racetrackgym-0.2.3/racetrackgym/maps/diverse/wavy.txt
--rw-r--r--   0        0        0      955 2021-12-14 09:58:20.673786 racetrackgym-0.2.3/racetrackgym/maps/double-track.track
--rw-r--r--   0        0        0     2321 2021-12-14 09:58:20.673901 racetrackgym-0.2.3/racetrackgym/maps/hansen-bigger.track
--rw-r--r--   0        0        0     1306 2021-12-14 09:58:20.673993 racetrackgym-0.2.3/racetrackgym/maps/large_curves.track
--rw-r--r--   0        0        0      822 2021-12-14 09:58:20.674075 racetrackgym-0.2.3/racetrackgym/maps/maze-small.track
--rw-r--r--   0        0        0      909 2021-12-14 09:58:20.674239 racetrackgym-0.2.3/racetrackgym/maps/maze.track
--rw-r--r--   0        0        0      972 2021-12-14 09:58:20.674369 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_1.potentials
--rw-r--r--   0        0        0      442 2021-12-14 09:58:20.674489 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_1.track
--rw-r--r--   0        0        0    10973 2021-12-14 09:58:20.674707 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_10.potentials
--rw-r--r--   0        0        0     4574 2021-12-14 09:58:20.674855 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_10.track
--rw-r--r--   0        0        0     5029 2021-12-14 09:58:20.675094 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_11.track
--rw-r--r--   0        0        0     5484 2021-12-14 09:58:20.675333 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_12.track
--rw-r--r--   0        0        0     5939 2021-12-14 09:58:20.675425 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_13.track
--rw-r--r--   0        0        0     6394 2021-12-14 09:58:20.675585 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_14.track
--rw-r--r--   0        0        0     6849 2021-12-14 09:58:20.675702 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_15.track
--rw-r--r--   0        0        0     7304 2021-12-14 09:58:20.675813 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_16.track
--rw-r--r--   0        0        0     7759 2021-12-14 09:58:20.675925 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_17.track
--rw-r--r--   0        0        0     8214 2021-12-14 09:58:20.676006 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_18.track
--rw-r--r--   0        0        0     8669 2021-12-14 09:58:20.676115 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_19.track
--rw-r--r--   0        0        0      933 2021-12-14 09:58:20.676243 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_2.track
--rw-r--r--   0        0        0    21873 2021-12-14 09:58:20.676380 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_20.potentials
--rw-r--r--   0        0        0     9124 2021-12-14 09:58:20.676570 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_20.track
--rw-r--r--   0        0        0     9579 2021-12-14 09:58:20.676679 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_21.track
--rw-r--r--   0        0        0    10034 2021-12-14 09:58:20.676777 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_22.track
--rw-r--r--   0        0        0    10489 2021-12-14 09:58:20.676866 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_23.track
--rw-r--r--   0        0        0    10944 2021-12-14 09:58:20.676965 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_24.track
--rw-r--r--   0        0        0    11399 2021-12-14 09:58:20.677047 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_25.track
--rw-r--r--   0        0        0    11854 2021-12-14 09:58:20.677129 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_26.track
--rw-r--r--   0        0        0    12309 2021-12-14 09:58:20.677222 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_27.track
--rw-r--r--   0        0        0    12764 2021-12-14 09:58:20.677348 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_28.track
--rw-r--r--   0        0        0    13220 2021-12-14 09:58:20.677484 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_29.track
--rw-r--r--   0        0        0     1389 2021-12-14 09:58:20.677570 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_3.track
--rw-r--r--   0        0        0    32806 2021-12-14 09:58:20.677678 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_30.potentials
--rw-r--r--   0        0        0    13675 2021-12-14 09:58:20.677777 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_30.track
--rw-r--r--   0        0        0     1844 2021-12-14 09:58:20.677855 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_4.track
--rw-r--r--   0        0        0     2299 2021-12-14 09:58:20.677933 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_5.track
--rw-r--r--   0        0        0     2754 2021-12-14 09:58:20.678018 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_6.track
--rw-r--r--   0        0        0     3209 2021-12-14 09:58:20.678107 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_7.track
--rw-r--r--   0        0        0     3664 2021-12-14 09:58:20.678263 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_8.track
--rw-r--r--   0        0        0     4119 2021-12-14 09:58:20.678453 racetrackgym-0.2.3/racetrackgym/maps/nook/nook_9.track
--rw-r--r--   0        0        0     2642 2021-12-14 09:58:20.678666 racetrackgym-0.2.3/racetrackgym/maps/potentials/barto-big.potentials
--rw-r--r--   0        0        0      966 2021-12-14 09:58:20.678789 racetrackgym-0.2.3/racetrackgym/maps/potentials/barto-small.potentials
--rw-r--r--   0        0        0     6562 2021-12-14 09:58:20.678909 racetrackgym-0.2.3/racetrackgym/maps/potentials/hansen-bigger.potentials
--rw-r--r--   0        0        0     2306 2021-12-14 09:58:20.679085 racetrackgym-0.2.3/racetrackgym/maps/ring/ring-4.track
--rw-r--r--   0        0        0     2306 2021-12-14 09:58:20.679212 racetrackgym-0.2.3/racetrackgym/maps/ring/ring.track
--rw-r--r--   0        0        0     1802 2021-12-14 09:58:20.679376 racetrackgym-0.2.3/racetrackgym/maps/river/river-deadend-narrow.track
--rw-r--r--   0        0        0     1802 2021-12-14 09:58:20.679463 racetrackgym-0.2.3/racetrackgym/maps/river/river-deadend.track
--rw-r--r--   0        0        0     1802 2021-12-14 09:58:20.679545 racetrackgym-0.2.3/racetrackgym/maps/river/river.track
--rw-r--r--   0        0        0     1802 2021-12-14 09:58:20.679620 racetrackgym-0.2.3/racetrackgym/maps/river/river_narrow.track
--rw-r--r--   0        0        0      955 2021-12-14 09:58:20.679702 racetrackgym-0.2.3/racetrackgym/maps/shortcut-big.track
--rw-r--r--   0        0        0      478 2021-12-14 09:58:20.679827 racetrackgym-0.2.3/racetrackgym/maps/templates/nook.track
--rw-r--r--   0        0        0     1103 2021-12-14 09:58:20.679914 racetrackgym-0.2.3/racetrackgym/maps/templates/nook_creator.py
--rw-r--r--   0        0        0      467 2021-12-14 09:58:20.679991 racetrackgym-0.2.3/racetrackgym/maps/templates/nook_empty.track
--rw-r--r--   0        0        0      467 2021-12-14 09:58:20.680113 racetrackgym-0.2.3/racetrackgym/maps/templates/nook_end.track
--rw-r--r--   0        0        0      467 2021-12-14 09:58:20.680194 racetrackgym-0.2.3/racetrackgym/maps/templates/nook_start.track
--rw-r--r--   0        0        0      282 2021-12-14 09:58:20.680280 racetrackgym-0.2.3/racetrackgym/maps/templates/square.track
--rw-r--r--   0        0        0     1422 2022-06-23 12:29:41.041748 racetrackgym-0.2.3/racetrackgym/parser.py
--rw-r--r--   0        0        0     1214 2022-06-23 12:31:41.320174 racetrackgym-0.2.3/setup.py
--rw-r--r--   0        0        0      789 2022-06-23 12:31:41.320398 racetrackgym-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-04-20 09:10:05.953292 racetrackgym-0.2.4/README.md
+-rw-r--r--   0        0        0      867 2023-04-20 15:55:13.545286 racetrackgym-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-20 09:10:05.954789 racetrackgym-0.2.4/racetrackgym/__init__.py
+-rw-r--r--   0        0        0     2993 2023-04-20 09:10:05.954912 racetrackgym-0.2.4/racetrackgym/argument_parser.py
+-rw-r--r--   0        0        0    25555 2023-04-20 09:10:05.955109 racetrackgym-0.2.4/racetrackgym/environment.py
+-rw-r--r--   0        0        0     9082 2023-04-20 09:10:05.955262 racetrackgym-0.2.4/racetrackgym/evaluator.py
+-rw-r--r--   0        0        0     5341 2023-04-20 09:10:05.955381 racetrackgym-0.2.4/racetrackgym/graphic.py
+-rw-r--r--   0        0        0     1034 2023-04-20 09:10:05.955551 racetrackgym-0.2.4/racetrackgym/maps/barto-big.track
+-rw-r--r--   0        0        0    99343 2023-04-20 09:10:05.955898 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_10.track
+-rw-r--r--   0        0        0     4037 2023-04-20 09:10:05.956017 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_2.track
+-rw-r--r--   0        0        0     9020 2023-04-20 09:10:05.956169 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_3.track
+-rw-r--r--   0        0        0    15985 2023-04-20 09:10:05.956308 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_4.track
+-rw-r--r--   0        0        0    24928 2023-04-20 09:10:05.956435 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_5.track
+-rw-r--r--   0        0        0    35851 2023-04-20 09:10:05.956616 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_6.track
+-rw-r--r--   0        0        0    48754 2023-04-20 09:10:05.956752 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_7.track
+-rw-r--r--   0        0        0    63637 2023-04-20 09:10:05.956951 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_8.track
+-rw-r--r--   0        0        0    80500 2023-04-20 09:10:05.957149 racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_9.track
+-rw-r--r--   0        0        0      442 2023-04-20 09:10:05.957290 racetrackgym-0.2.4/racetrackgym/maps/barto-small.track
+-rw-r--r--   0        0        0     1715 2023-04-20 09:10:05.957461 racetrackgym-0.2.4/racetrackgym/maps/barto-small_scales/barto-small_scaled_2.track
+-rw-r--r--   0        0        0     6780 2023-04-20 09:10:05.957549 racetrackgym-0.2.4/racetrackgym/maps/barto-small_scales/barto-small_scaled_4.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.957691 racetrackgym-0.2.4/racetrackgym/maps/corner/1-2-3.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.957786 racetrackgym-0.2.4/racetrackgym/maps/corner/1-4-3.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.957866 racetrackgym-0.2.4/racetrackgym/maps/corner/2-1-4.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.957931 racetrackgym-0.2.4/racetrackgym/maps/corner/2-3-4.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.958015 racetrackgym-0.2.4/racetrackgym/maps/corner/3-2-1.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.958096 racetrackgym-0.2.4/racetrackgym/maps/corner/3-4-1.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.958175 racetrackgym-0.2.4/racetrackgym/maps/corner/4-1-2.track
+-rw-r--r--   0        0        0      660 2023-04-20 09:10:05.958246 racetrackgym-0.2.4/racetrackgym/maps/corner/4-3-2.track
+-rw-r--r--   0        0        0      470 2023-04-20 09:10:05.958357 racetrackgym-0.2.4/racetrackgym/maps/diverse/barrier.txt
+-rw-r--r--   0        0        0      430 2023-04-20 09:10:05.958435 racetrackgym-0.2.4/racetrackgym/maps/diverse/bottleneck.txt
+-rw-r--r--   0        0        0      550 2023-04-20 09:10:05.958507 racetrackgym-0.2.4/racetrackgym/maps/diverse/corner.txt
+-rw-r--r--   0        0        0      550 2023-04-20 09:10:05.958579 racetrackgym-0.2.4/racetrackgym/maps/diverse/diagonal.txt
+-rw-r--r--   0        0        0      310 2023-04-20 09:10:05.958651 racetrackgym-0.2.4/racetrackgym/maps/diverse/pyramid.txt
+-rw-r--r--   0        0        0      295 2023-04-20 09:10:05.958723 racetrackgym-0.2.4/racetrackgym/maps/diverse/ring.txt
+-rw-r--r--   0        0        0      520 2023-04-20 09:10:05.958791 racetrackgym-0.2.4/racetrackgym/maps/diverse/spiral.txt
+-rw-r--r--   0        0        0      550 2023-04-20 09:10:05.958857 racetrackgym-0.2.4/racetrackgym/maps/diverse/straighton.txt
+-rw-r--r--   0        0        0      586 2023-04-20 09:10:05.958922 racetrackgym-0.2.4/racetrackgym/maps/diverse/uturn.txt
+-rw-r--r--   0        0        0      582 2023-04-20 09:10:05.958995 racetrackgym-0.2.4/racetrackgym/maps/diverse/wavy.txt
+-rw-r--r--   0        0        0      955 2023-04-20 09:10:05.959076 racetrackgym-0.2.4/racetrackgym/maps/double-track.track
+-rw-r--r--   0        0        0     2321 2023-04-20 09:10:05.959199 racetrackgym-0.2.4/racetrackgym/maps/hansen-bigger.track
+-rw-r--r--   0        0        0     1306 2023-04-20 09:10:05.959263 racetrackgym-0.2.4/racetrackgym/maps/large_curves.track
+-rw-r--r--   0        0        0      822 2023-04-20 09:10:05.959332 racetrackgym-0.2.4/racetrackgym/maps/maze-small.track
+-rw-r--r--   0        0        0      909 2023-04-20 11:20:51.029605 racetrackgym-0.2.4/racetrackgym/maps/maze.track
+-rw-r--r--   0        0        0     1054 2023-04-20 11:23:24.980865 racetrackgym-0.2.4/racetrackgym/maps/maze_and_shortcuts.track
+-rw-r--r--   0        0        0      972 2023-04-20 09:10:05.959520 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_1.potentials
+-rw-r--r--   0        0        0      442 2023-04-20 09:10:05.959597 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_1.track
+-rw-r--r--   0        0        0    10973 2023-04-20 09:10:05.959748 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_10.potentials
+-rw-r--r--   0        0        0     4574 2023-04-20 09:10:05.959819 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_10.track
+-rw-r--r--   0        0        0     5029 2023-04-20 09:10:05.959917 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_11.track
+-rw-r--r--   0        0        0     5484 2023-04-20 09:10:05.960003 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_12.track
+-rw-r--r--   0        0        0     5939 2023-04-20 09:10:05.960074 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_13.track
+-rw-r--r--   0        0        0     6394 2023-04-20 09:10:05.960162 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_14.track
+-rw-r--r--   0        0        0     6849 2023-04-20 09:10:05.960235 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_15.track
+-rw-r--r--   0        0        0     7304 2023-04-20 09:10:05.960305 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_16.track
+-rw-r--r--   0        0        0     7759 2023-04-20 09:10:05.960378 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_17.track
+-rw-r--r--   0        0        0     8214 2023-04-20 09:10:05.960449 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_18.track
+-rw-r--r--   0        0        0     8669 2023-04-20 09:10:05.960535 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_19.track
+-rw-r--r--   0        0        0      933 2023-04-20 09:10:05.960625 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_2.track
+-rw-r--r--   0        0        0    21873 2023-04-20 09:10:05.960765 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_20.potentials
+-rw-r--r--   0        0        0     9124 2023-04-20 09:10:05.960856 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_20.track
+-rw-r--r--   0        0        0     9579 2023-04-20 09:10:05.960929 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_21.track
+-rw-r--r--   0        0        0    10034 2023-04-20 09:10:05.961008 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_22.track
+-rw-r--r--   0        0        0    10489 2023-04-20 09:10:05.961087 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_23.track
+-rw-r--r--   0        0        0    10944 2023-04-20 09:10:05.961159 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_24.track
+-rw-r--r--   0        0        0    11399 2023-04-20 09:10:05.961229 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_25.track
+-rw-r--r--   0        0        0    11854 2023-04-20 09:10:05.961305 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_26.track
+-rw-r--r--   0        0        0    12309 2023-04-20 09:10:05.961381 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_27.track
+-rw-r--r--   0        0        0    12764 2023-04-20 09:10:05.961459 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_28.track
+-rw-r--r--   0        0        0    13220 2023-04-20 09:10:05.961526 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_29.track
+-rw-r--r--   0        0        0     1389 2023-04-20 09:10:05.961611 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_3.track
+-rw-r--r--   0        0        0    32806 2023-04-20 09:10:05.961700 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_30.potentials
+-rw-r--r--   0        0        0    13675 2023-04-20 09:10:05.961791 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_30.track
+-rw-r--r--   0        0        0     1844 2023-04-20 09:10:05.961871 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_4.track
+-rw-r--r--   0        0        0     2299 2023-04-20 09:10:05.961945 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_5.track
+-rw-r--r--   0        0        0     2754 2023-04-20 09:10:05.962012 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_6.track
+-rw-r--r--   0        0        0     3209 2023-04-20 09:10:05.962090 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_7.track
+-rw-r--r--   0        0        0     3664 2023-04-20 09:10:05.962160 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_8.track
+-rw-r--r--   0        0        0     4119 2023-04-20 09:10:05.962232 racetrackgym-0.2.4/racetrackgym/maps/nook/nook_9.track
+-rw-r--r--   0        0        0     2642 2023-04-20 09:10:05.962362 racetrackgym-0.2.4/racetrackgym/maps/potentials/barto-big.potentials
+-rw-r--r--   0        0        0      966 2023-04-20 09:10:05.962433 racetrackgym-0.2.4/racetrackgym/maps/potentials/barto-small.potentials
+-rw-r--r--   0        0        0     6562 2023-04-20 09:10:05.962498 racetrackgym-0.2.4/racetrackgym/maps/potentials/hansen-bigger.potentials
+-rw-r--r--   0        0        0     2306 2023-04-20 09:10:05.962623 racetrackgym-0.2.4/racetrackgym/maps/ring/ring-4.track
+-rw-r--r--   0        0        0     2306 2023-04-20 09:10:05.962710 racetrackgym-0.2.4/racetrackgym/maps/ring/ring.track
+-rw-r--r--   0        0        0     1802 2023-04-20 09:10:05.962836 racetrackgym-0.2.4/racetrackgym/maps/river/river-deadend-narrow.track
+-rw-r--r--   0        0        0     1802 2023-04-20 09:10:05.962920 racetrackgym-0.2.4/racetrackgym/maps/river/river-deadend.track
+-rw-r--r--   0        0        0     1802 2023-04-20 09:10:05.963001 racetrackgym-0.2.4/racetrackgym/maps/river/river.track
+-rw-r--r--   0        0        0     1802 2023-04-20 09:10:05.963071 racetrackgym-0.2.4/racetrackgym/maps/river/river_narrow.track
+-rw-r--r--   0        0        0      955 2023-04-20 09:10:05.963141 racetrackgym-0.2.4/racetrackgym/maps/shortcut-big.track
+-rw-r--r--   0        0        0      478 2023-04-20 09:10:05.963260 racetrackgym-0.2.4/racetrackgym/maps/templates/nook.track
+-rw-r--r--   0        0        0     1103 2023-04-20 09:10:05.963345 racetrackgym-0.2.4/racetrackgym/maps/templates/nook_creator.py
+-rw-r--r--   0        0        0      467 2023-04-20 09:10:05.963412 racetrackgym-0.2.4/racetrackgym/maps/templates/nook_empty.track
+-rw-r--r--   0        0        0      467 2023-04-20 09:10:05.963480 racetrackgym-0.2.4/racetrackgym/maps/templates/nook_end.track
+-rw-r--r--   0        0        0      467 2023-04-20 09:10:05.963546 racetrackgym-0.2.4/racetrackgym/maps/templates/nook_start.track
+-rw-r--r--   0        0        0      282 2023-04-20 09:10:05.963616 racetrackgym-0.2.4/racetrackgym/maps/templates/square.track
+-rw-r--r--   0        0        0     1422 2023-04-20 09:10:05.963713 racetrackgym-0.2.4/racetrackgym/parser.py
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 racetrackgym-0.2.4/PKG-INFO
```

### Comparing `racetrackgym-0.2.3/pyproject.toml` & `racetrackgym-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Operating System :: OS Independent",
 ]
 description = "Python Simulation of the Racetrack game. This implementation is compatible with the OpenAI Gym API, and comes with additional extensions"
 name = "racetrackgym"
 readme = "README.md"
-version = "0.2.3"
+version = "0.2.4"
 
 [tool.poetry.dependencies]
 Pillow = "^8.4.0"
 argparse = "^1.4.0"
 matplotlib = "^3.4.3"
 numpy = "^1.21.4"
 python = ">=3.9,<3.11"
 rlmate = ">=0.0.20"
+jupyterlab = "^3.6.3"
 
 [tool.poetry.dev-dependencies]
 black = {version = "*", allow-prereleases = true}
 flake8 = "^3.7.9"
 flake8-bugbear = "^20.1.2"
 pep8-naming = "^0.9.1"
 pytest = "^6.2.5"
```

### Comparing `racetrackgym-0.2.3/racetrackgym/argument_parser.py` & `racetrackgym-0.2.4/racetrackgym/argument_parser.py`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/environment.py` & `racetrackgym-0.2.4/racetrackgym/environment.py`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/evaluator.py` & `racetrackgym-0.2.4/racetrackgym/evaluator.py`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/graphic.py` & `racetrackgym-0.2.4/racetrackgym/graphic.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,36 +65,33 @@
             0,
             0,
         ),
     )
     for i, line in enumerate(env.map.map):
         for j, sign in enumerate(line):
             if sign == "x":
-                result.paste(wall, (j * size, i * size), mask=wall)
-                continue
-            if sign == "s":
+                current = wall
+            elif sign == "s":
                 if hide_start_line:
-                    result.paste(empty, (j * size, i * size), mask=empty)
+                    current = empty
                 else:
-                    result.paste(start, (j * size, i * size), mask=start)
-                continue
-            if sign == "g":
-                result.paste(goal, (j * size, i * size), mask=goal)
-                continue
-            if sign == ".":
+                    current = start
+            elif sign == "g":
+                current = goal
+            elif sign == ".":
                 if show_landmarks:
                     rgb_value = int(255 - env.potentials[i][j] * 10)
                     landmark_color = (0, 0, rgb_value)
                     landmark = Image.new("RGBA", (size, size), landmark_color)
                     draw = ImageDraw.Draw(landmark)
                     draw.rectangle(((0, 0), (size - 1, size - 1)), outline=(0, 0, 0))
-                    result.paste(landmark, (j * size, i * size), mask=landmark)
+                    current = landmark
                 else:
-                    result.paste(empty, (j * size, i * size), mask=empty)
-                continue
+                    current = empty
+            result.paste(current, (j * size, i * size), mask=current)
 
     path = copy.copy(env.path)
     path.append(path[-1])
     color = line_colors[0]
     o = 0.5
 
     if show_path:
```

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_10.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_10.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_2.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_2.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_3.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_3.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_4.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_4.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_5.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_5.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_6.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_6.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_7.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_7.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_8.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_8.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-big_scales/barto-big_scaled_9.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-big_scales/barto-big_scaled_9.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/barto-small_scales/barto-small_scaled_2.track` & `racetrackgym-0.2.4/racetrackgym/maps/barto-small_scales/barto-small_scaled_2.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/1-2-3.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/1-2-3.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/2-1-4.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/2-1-4.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/2-3-4.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/2-3-4.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/3-2-1.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/3-2-1.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/3-4-1.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/3-4-1.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/4-1-2.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/4-1-2.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/corner/4-3-2.track` & `racetrackgym-0.2.4/racetrackgym/maps/corner/4-3-2.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/diverse/corner.txt` & `racetrackgym-0.2.4/racetrackgym/maps/diverse/corner.txt`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/diverse/diagonal.txt` & `racetrackgym-0.2.4/racetrackgym/maps/diverse/diagonal.txt`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/diverse/spiral.txt` & `racetrackgym-0.2.4/racetrackgym/maps/diverse/spiral.txt`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/diverse/wavy.txt` & `racetrackgym-0.2.4/racetrackgym/maps/diverse/wavy.txt`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/double-track.track` & `racetrackgym-0.2.4/racetrackgym/maps/double-track.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/hansen-bigger.track` & `racetrackgym-0.2.4/racetrackgym/maps/hansen-bigger.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/maze-small.track` & `racetrackgym-0.2.4/racetrackgym/maps/maze-small.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/maze.track` & `racetrackgym-0.2.4/racetrackgym/maps/maze.track`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-d.m: 29 30
+dim: 29 30
 g..x...........x........x.....
 g..x...........x........x.....
 x..x..xxxx..x..x..xxxx..x..xxx
 x..x..x.....x.....x.....x.....
 x..x..x.....x.....x.....x.....
 x..xxxx..xxxxxxxxxx..xxxxxxx..
 x........x........x...........
```

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_1.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_1.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_10.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_10.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_10.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_10.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_11.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_11.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_12.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_12.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_13.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_13.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_14.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_14.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_16.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_16.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_17.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_17.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_2.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_2.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_20.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_20.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_21.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_21.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_22.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_22.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_23.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_23.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_24.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_24.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_25.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_25.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_26.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_26.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_27.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_27.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_28.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_28.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_29.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_29.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_3.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_3.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_30.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_30.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_30.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_30.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_4.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_4.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_5.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_5.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_6.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_6.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_7.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_7.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/nook/nook_9.track` & `racetrackgym-0.2.4/racetrackgym/maps/nook/nook_9.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/potentials/barto-big.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/potentials/barto-big.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/potentials/barto-small.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/potentials/barto-small.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/potentials/hansen-bigger.potentials` & `racetrackgym-0.2.4/racetrackgym/maps/potentials/hansen-bigger.potentials`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/ring/ring-4.track` & `racetrackgym-0.2.4/racetrackgym/maps/ring/ring-4.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/ring/ring.track` & `racetrackgym-0.2.4/racetrackgym/maps/ring/ring.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/river/river-deadend-narrow.track` & `racetrackgym-0.2.4/racetrackgym/maps/river/river-deadend-narrow.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/river/river-deadend.track` & `racetrackgym-0.2.4/racetrackgym/maps/river/river-deadend.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/river/river.track` & `racetrackgym-0.2.4/racetrackgym/maps/river/river.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/river/river_narrow.track` & `racetrackgym-0.2.4/racetrackgym/maps/river/river_narrow.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/shortcut-big.track` & `racetrackgym-0.2.4/racetrackgym/maps/shortcut-big.track`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/maps/templates/nook_creator.py` & `racetrackgym-0.2.4/racetrackgym/maps/templates/nook_creator.py`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/racetrackgym/parser.py` & `racetrackgym-0.2.4/racetrackgym/parser.py`

 * *Files identical despite different names*

### Comparing `racetrackgym-0.2.3/PKG-INFO` & `racetrackgym-0.2.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: racetrackgym
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Simulation of the Racetrack game. This implementation is compatible with the OpenAI Gym API, and comes with additional extensions
 Author: Timo P. Gros
 Author-email: timopgros@cs.uni-saarland.de
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=8.4.0,<9.0.0)
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Requires-Dist: jupyterlab (>=3.6.3,<4.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: numpy (>=1.21.4,<2.0.0)
 Requires-Dist: rlmate (>=0.0.20)
 Description-Content-Type: text/markdown
 
 # racetrack
```

