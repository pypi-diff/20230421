# Comparing `tmp/mcts_solver-0.0.3.tar.gz` & `tmp/mcts_solver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcts_solver-0.0.3.tar", last modified: Sun Nov 20 13:12:45 2022, max compression
+gzip compressed data, was "mcts_solver-0.0.4.tar", last modified: Fri Apr 21 06:31:28 2023, max compression
```

## Comparing `mcts_solver-0.0.3.tar` & `mcts_solver-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-20 13:12:45.219288 mcts_solver-0.0.3/
--rw-rw-r--   0 root         (0) root         (0)    35149 2022-08-10 12:06:43.000000 mcts_solver-0.0.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       46 2022-08-10 13:01:54.000000 mcts_solver-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-11-20 13:12:45.219288 mcts_solver-0.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      406 2022-08-11 08:42:20.000000 mcts_solver-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-20 13:12:45.135288 mcts_solver-0.0.3/mcts_solver/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-11 08:28:31.000000 mcts_solver-0.0.3/mcts_solver/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3864 2022-11-10 11:46:27.000000 mcts_solver-0.0.3/mcts_solver/mcts_solver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-20 13:12:45.215288 mcts_solver-0.0.3/mcts_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-11-20 13:12:44.000000 mcts_solver-0.0.3/mcts_solver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2022-11-20 13:12:44.000000 mcts_solver-0.0.3/mcts_solver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-20 13:12:44.000000 mcts_solver-0.0.3/mcts_solver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-20 13:12:44.000000 mcts_solver-0.0.3/mcts_solver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2022-11-20 13:12:44.000000 mcts_solver-0.0.3/mcts_solver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-11-20 13:12:44.000000 mcts_solver-0.0.3/mcts_solver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-20 13:12:45.219288 mcts_solver-0.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1674 2022-11-19 11:06:38.000000 mcts_solver-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/
+-rw-rw-r--   0 root         (0) root         (0)    35149 2022-08-10 12:06:43.000000 mcts_solver-0.0.4/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       46 2022-08-10 13:01:54.000000 mcts_solver-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      406 2022-08-11 08:42:20.000000 mcts_solver-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:31:28.059349 mcts_solver-0.0.4/mcts_solver/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-11 08:28:31.000000 mcts_solver-0.0.4/mcts_solver/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4783 2023-04-19 11:16:11.000000 mcts_solver-0.0.4/mcts_solver/mcts_solver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/mcts_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1674 2023-04-19 12:25:15.000000 mcts_solver-0.0.4/setup.py
```

### Comparing `mcts_solver-0.0.3/LICENSE` & `mcts_solver-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcts_solver-0.0.3/PKG-INFO` & `mcts_solver-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcts_solver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Monte-Carlo tree search solver for chess-ant
 Home-page: https://github.com/akuroiwa/mcts-solver
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: mcts,monte,carlo,tree,search,solver
 Platform: any
```

### Comparing `mcts_solver-0.0.3/mcts_solver/mcts_solver.py` & `mcts_solver-0.0.4/mcts_solver/mcts_solver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from mcts import mcts, treeNode
+import multiprocessing
 
 class AntLionTreeNode(treeNode):
 
     def __init__(self, state, parent):
         super().__init__(state, parent)
         self.value = None
 
@@ -18,14 +19,15 @@
         '''
         pass
 
     def mctsSolver(self, node):
         '''This is based on pseudocode from the following paper:
         `Winands, Mark & Björnsson, Yngvi & Saito, Jahn-Takeshi. (2008). Monte-Carlo Tree Search Solver. 25-36. 10.1007/978-3-540-87608-3_3.
         <https://www.researchgate.net/publication/220962507_Monte-Carlo_Tree_Search_Solver>`__
+        Parallel processing is possible thanks to OpenAI's ChatGPT advice.
         '''
         if node.isTerminal:
             if  node.state.getReward() == 1:
                 node.value = float("inf")
             elif node.state.getReward() == -1:
                 node.value = float("-inf")
             else:
@@ -34,18 +36,31 @@
         bestChild = node
 
         if bestChild.value != float("-inf") and bestChild.value != float("inf"):
             if bestChild.numVisits == 0:
                 if self.dl:
                     reward = self.dl_method(bestChild.state)
                 else:
-                    reward = bestChild.state.getCurrentPlayer() * -self.rollout(bestChild.state)
+                    # reward = bestChild.state.getCurrentPlayer() * -self.rollout(bestChild.state)
+                    with multiprocessing.Pool() as pool:
+                        num_processes = multiprocessing.cpu_count()
+                        multiple_results = [pool.apply_async(self.rollout, args=(bestChild.state,)) for i in range(num_processes)]
+                        pool.close()
+                        pool.join()
+                        results = [res for res in multiple_results if res.ready() and res.successful()]
+                        if results:
+                            reward = bestChild.state.getCurrentPlayer() * -max([res.get() for res in results])
+                        else:
+                            reward = 0
                 return reward
             else:
-                reward = -self.mctsSolver(bestChild)
+                with multiprocessing.Pool() as pool:
+                    m = pool.apply_async(-self.mctsSolver, args=(bestChild,))
+                    reward = m.get()
+                # reward = -self.mctsSolver(bestChild)
         else:
             reward = bestChild.value
 
         if reward == float("inf"):
             node.parent.value = float("-inf")
             return reward
         else:
```

### Comparing `mcts_solver-0.0.3/mcts_solver.egg-info/PKG-INFO` & `mcts_solver-0.0.4/mcts_solver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcts-solver
-Version: 0.0.3
+Version: 0.0.4
 Summary: Monte-Carlo tree search solver for chess-ant
 Home-page: https://github.com/akuroiwa/mcts-solver
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: mcts,monte,carlo,tree,search,solver
 Platform: any
```

### Comparing `mcts_solver-0.0.3/setup.py` & `mcts_solver-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import glob
 from setuptools import setup, find_packages
 
 setup(
     name='mcts_solver',
-    version='0.0.3',
+    version='0.0.4',
     url='https://github.com/akuroiwa/mcts-solver',
     # # PyPI url
     # download_url='',
     license='GNU/GPLv3+',
     author='Akihiro Kuroiwa',
     author_email='akuroiwa@env-reform.com',
     description='Monte-Carlo tree search solver for chess-ant',
```

