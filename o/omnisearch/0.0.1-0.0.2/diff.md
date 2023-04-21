# Comparing `tmp/omnisearch-0.0.1.tar.gz` & `tmp/omnisearch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnisearch-0.0.1.tar", last modified: Tue Apr 18 14:22:47 2023, max compression
+gzip compressed data, was "omnisearch-0.0.2.tar", last modified: Fri Apr 21 11:41:58 2023, max compression
```

## Comparing `omnisearch-0.0.1.tar` & `omnisearch-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:22:47.702943 omnisearch-0.0.1/
--rw-rw-rw-   0        0        0       57 2023-04-18 14:22:47.702943 omnisearch-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 14:22:47.679938 omnisearch-0.0.1/omnisearch/
--rw-rw-rw-   0        0        0        0 2023-04-18 14:21:18.000000 omnisearch-0.0.1/omnisearch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:22:47.700943 omnisearch-0.0.1/omnisearch.egg-info/
--rw-rw-rw-   0        0        0       57 2023-04-18 14:22:47.000000 omnisearch-0.0.1/omnisearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-04-18 14:22:47.000000 omnisearch-0.0.1/omnisearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:22:47.000000 omnisearch-0.0.1/omnisearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-18 14:22:47.000000 omnisearch-0.0.1/omnisearch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 14:22:47.703944 omnisearch-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       87 2023-04-18 14:22:31.000000 omnisearch-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:41:58.675647 omnisearch-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-04-18 14:26:53.000000 omnisearch-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      616 2023-04-21 11:41:58.675647 omnisearch-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3296 2023-04-21 11:39:49.000000 omnisearch-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:41:58.648642 omnisearch-0.0.2/algorithms/
+-rw-rw-rw-   0        0        0      382 2023-04-08 14:47:28.000000 omnisearch-0.0.2/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2406 2023-04-17 16:15:55.000000 omnisearch-0.0.2/algorithms/a_star.py
+-rw-rw-rw-   0        0        0     2138 2023-04-17 16:15:55.000000 omnisearch-0.0.2/algorithms/best_first.py
+-rw-rw-rw-   0        0        0     1934 2023-04-17 16:15:55.000000 omnisearch-0.0.2/algorithms/branch_and_bound.py
+-rw-rw-rw-   0        0        0     1718 2023-04-17 16:15:55.000000 omnisearch-0.0.2/algorithms/breadth_first.py
+-rw-rw-rw-   0        0        0     1702 2023-04-17 16:15:55.000000 omnisearch-0.0.2/algorithms/depth_first.py
+-rw-rw-rw-   0        0        0     3047 2023-04-16 18:47:52.000000 omnisearch-0.0.2/algorithms/hill_climbing.py
+-rw-rw-rw-   0        0        0     2746 2023-04-16 18:47:52.000000 omnisearch-0.0.2/algorithms/iterative_deepening.py
+-rw-rw-rw-   0        0        0     1799 2023-04-17 16:15:55.000000 omnisearch-0.0.2/algorithms/uniform_cost.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:41:58.652643 omnisearch-0.0.2/data_structures/
+-rw-rw-rw-   0        0        0       93 2023-04-18 13:51:25.000000 omnisearch-0.0.2/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     1435 2023-04-18 14:26:53.000000 omnisearch-0.0.2/data_structures/priority_queue.py
+-rw-rw-rw-   0        0        0     1028 2023-04-18 14:26:53.000000 omnisearch-0.0.2/data_structures/queue.py
+-rw-rw-rw-   0        0        0     1021 2023-04-18 14:26:53.000000 omnisearch-0.0.2/data_structures/stack.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:41:58.654644 omnisearch-0.0.2/interfaces/
+-rw-rw-rw-   0        0        0       52 2023-03-22 13:45:41.000000 omnisearch-0.0.2/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1746 2023-04-07 15:40:00.000000 omnisearch-0.0.2/interfaces/state_space_problem.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:41:58.670647 omnisearch-0.0.2/omnisearch.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-04-21 11:41:58.000000 omnisearch-0.0.2/omnisearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-04-21 11:41:58.000000 omnisearch-0.0.2/omnisearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:41:58.000000 omnisearch-0.0.2/omnisearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-21 11:41:58.000000 omnisearch-0.0.2/omnisearch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 11:41:58.674648 omnisearch-0.0.2/problems/
+-rw-rw-rw-   0        0        0      142 2023-04-01 17:36:13.000000 omnisearch-0.0.2/problems/__init__.py
+-rw-rw-rw-   0        0        0     2159 2023-04-08 13:18:21.000000 omnisearch-0.0.2/problems/maze.py
+-rw-rw-rw-   0        0        0     2806 2023-04-19 10:31:02.000000 omnisearch-0.0.2/problems/missionaries_and_cannibals.py
+-rw-rw-rw-   0        0        0     1521 2023-04-08 12:12:09.000000 omnisearch-0.0.2/problems/n_queens.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:41:58.675647 omnisearch-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-04-21 11:39:49.000000 omnisearch-0.0.2/setup.py
```

