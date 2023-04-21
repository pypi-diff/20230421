# Comparing `tmp/structout-0.1.8.tar.gz` & `tmp/structout-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/structout-0.1.8.tar", last modified: Fri May 17 15:50:43 2019, max compression
+gzip compressed data, was "dist/structout-0.1.9.tar", last modified: Fri May 17 16:09:54 2019, max compression
```

## Comparing `structout-0.1.8.tar` & `structout-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2019-05-17 15:50:43.000000 structout-0.1.8/
-drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2019-05-17 15:50:43.000000 structout-0.1.8/structout.egg-info/
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      234 2019-05-17 15:50:43.000000 structout-0.1.8/structout.egg-info/SOURCES.txt
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      284 2019-05-17 15:50:43.000000 structout-0.1.8/structout.egg-info/PKG-INFO
--rw-rw-r--   0 ikea      (1000) ikea      (1000)        1 2019-05-17 15:50:43.000000 structout-0.1.8/structout.egg-info/dependency_links.txt
--rw-rw-r--   0 ikea      (1000) ikea      (1000)       10 2019-05-17 15:50:43.000000 structout-0.1.8/structout.egg-info/top_level.txt
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      437 2018-11-17 00:12:44.000000 structout-0.1.8/README.md
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      284 2019-05-17 15:50:43.000000 structout-0.1.8/PKG-INFO
--rw-rw-r--   0 ikea      (1000) ikea      (1000)     3265 2018-11-17 00:12:44.000000 structout-0.1.8/setup.py
-drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2019-05-17 15:50:43.000000 structout-0.1.8/structout/
--rw-rw-r--   0 ikea      (1000) ikea      (1000)     6456 2018-11-17 00:12:44.000000 structout-0.1.8/structout/graph.py
--rw-rw-r--   0 ikea      (1000) ikea      (1000)     2634 2018-11-17 00:13:01.000000 structout-0.1.8/structout/intlist.py
--rw-rw-r--   0 ikea      (1000) ikea      (1000)      178 2019-05-17 15:50:43.000000 structout-0.1.8/structout/_version.py
--rw-rw-r--   0 ikea      (1000) ikea      (1000)       81 2018-11-17 00:12:44.000000 structout-0.1.8/structout/__init__.py
--rw-rw-r--   0 ikea      (1000) ikea      (1000)       38 2019-05-17 15:50:43.000000 structout-0.1.8/setup.cfg
+drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2019-05-17 16:09:54.000000 structout-0.1.9/
+drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2019-05-17 16:09:54.000000 structout-0.1.9/structout.egg-info/
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)      234 2019-05-17 16:09:54.000000 structout-0.1.9/structout.egg-info/SOURCES.txt
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)      284 2019-05-17 16:09:54.000000 structout-0.1.9/structout.egg-info/PKG-INFO
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)        1 2019-05-17 16:09:54.000000 structout-0.1.9/structout.egg-info/dependency_links.txt
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)       10 2019-05-17 16:09:54.000000 structout-0.1.9/structout.egg-info/top_level.txt
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)      437 2018-11-17 00:12:44.000000 structout-0.1.9/README.md
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)      284 2019-05-17 16:09:54.000000 structout-0.1.9/PKG-INFO
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)     3265 2018-11-17 00:12:44.000000 structout-0.1.9/setup.py
+drwxrwxr-x   0 ikea      (1000) ikea      (1000)        0 2019-05-17 16:09:54.000000 structout-0.1.9/structout/
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)     6459 2019-05-17 16:08:42.000000 structout-0.1.9/structout/graph.py
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)     2634 2018-11-17 00:13:01.000000 structout-0.1.9/structout/intlist.py
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)      178 2019-05-17 16:09:54.000000 structout-0.1.9/structout/_version.py
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)       81 2018-11-17 00:12:44.000000 structout-0.1.9/structout/__init__.py
+-rw-rw-r--   0 ikea      (1000) ikea      (1000)       38 2019-05-17 16:09:54.000000 structout-0.1.9/setup.cfg
```

### Comparing `structout-0.1.8/setup.py` & `structout-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `structout-0.1.8/structout/graph.py` & `structout-0.1.9/structout/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,44 +22,39 @@
 def set_print_symbol(g, colorstyle='normal', nodelabel='label', edgelabel='label'):
 
 
     if type(colorstyle) == str:
         if colorstyle == "bw": # white
 
             for n, d in g.nodes(data=True):
-               d['asciisymbol'] = d.get(nodelabel,str(n))
+               d['asciisymbol'] = str(d.get(nodelabel,n))
 
             if edgelabel != None:
                 for a,b,d in g.edges(data=True):
                     if d.get(edgelabel,None):
                         d['asciisymbol'] = d[edgelabel]
 
         else: # default color
 
             for n, d in g.nodes(data=True):
-               d['asciisymbol'] = color(d.get(nodelabel, str(n)), 'red')
+               d['asciisymbol'] = color( str(d.get(nodelabel, n)), 'red')
 
             if edgelabel != None:
                 for a,b,d in g.edges(data=True):
                     if d.get(edgelabel,None):
                         d['asciisymbol'] = color(d[edgelabel], 'blue')
 
 
     else: # colorlists
         for nodes, col in zip (colorstyle, ["magenta", "cyan", "yellow", "red", "blue", "green"]):
            for n in nodes:
-               g.node[n]['asciisymbol'] = color(g.node[n].get(nodelabel,str(n)), col)
+               g.node[n]['asciisymbol'] = color(str(   g.node[n].get(nodelabel,n)), col)
         for n,d in g.nodes(data=True):
             if "asciisymbol" not in d:
-                g.node[n]['asciisymbol'] = color(g.node[n].get(nodelabel,str(n)), 'black')
-
-
-
-
-
+                g.node[n]['asciisymbol'] = color(  str( g.node[n].get(nodelabel,n)), 'black')
     return g
 
 
 ####
 # coordinate setter
 ###
 
@@ -231,8 +226,8 @@
 
 ''' 
 getting coordinates of molecules...  the molecule thing should be in the eden package afair
 import molecule
 chem=molecule.nx_to_rdkit(graph)
 m.GetConformer().GetAtomPosition(0)
 transform coordinates
-'''
+'''
```

### Comparing `structout-0.1.8/structout/intlist.py` & `structout-0.1.9/structout/intlist.py`

 * *Files identical despite different names*

