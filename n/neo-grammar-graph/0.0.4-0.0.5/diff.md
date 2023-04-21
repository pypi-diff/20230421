# Comparing `tmp/neo_grammar_graph-0.0.4.tar.gz` & `tmp/neo_grammar_graph-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo_grammar_graph-0.0.4.tar", last modified: Wed Apr 19 10:19:24 2023, max compression
+gzip compressed data, was "neo_grammar_graph-0.0.5.tar", last modified: Fri Apr 21 14:09:56 2023, max compression
```

## Comparing `neo_grammar_graph-0.0.4.tar` & `neo_grammar_graph-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.255835 neo_grammar_graph-0.0.4/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.0.4/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44490 2023-04-19 10:19:24.256153 neo_grammar_graph-0.0.4/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     3150 2023-04-19 10:18:28.000000 neo_grammar_graph-0.0.4/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-04-19 10:17:33.000000 neo_grammar_graph-0.0.4/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1088 2023-04-19 10:19:24.257107 neo_grammar_graph-0.0.4/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.0.4/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.248058 neo_grammar_graph-0.0.4/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.252315 neo_grammar_graph-0.0.4/src/neo_grammar_graph/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       80 2023-04-19 10:17:29.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    24306 2023-04-19 10:16:21.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/gg.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      208 2023-04-18 10:01:08.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/helpers.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       96 2023-04-18 10:11:26.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph/type_defs.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.254882 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44490 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      428 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      237 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-04-19 10:19:24.000000 neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/top_level.txt
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-19 10:19:24.255159 neo_grammar_graph-0.0.4/tests/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      277 2023-04-18 09:30:38.000000 neo_grammar_graph-0.0.4/tests/test_doctests.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 14:09:56.916948 neo_grammar_graph-0.0.5/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 neo_grammar_graph-0.0.5/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44488 2023-04-21 14:09:56.917168 neo_grammar_graph-0.0.5/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     3148 2023-04-21 13:08:50.000000 neo_grammar_graph-0.0.5/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      775 2023-04-21 13:08:21.000000 neo_grammar_graph-0.0.5/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1088 2023-04-21 14:09:56.917648 neo_grammar_graph-0.0.5/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 neo_grammar_graph-0.0.5/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 14:09:56.911542 neo_grammar_graph-0.0.5/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 14:09:56.914972 neo_grammar_graph-0.0.5/src/neo_grammar_graph/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       80 2023-04-21 13:08:32.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    46430 2023-04-21 14:07:48.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph/gg.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2917 2023-04-19 14:21:50.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph/helpers.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       96 2023-04-18 10:11:26.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph/type_defs.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 14:09:56.916431 neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    44488 2023-04-21 14:09:56.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      428 2023-04-21 14:09:56.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-21 14:09:56.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      237 2023-04-21 14:09:56.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       18 2023-04-21 14:09:56.000000 neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 14:09:56.916743 neo_grammar_graph-0.0.5/tests/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      417 2023-04-21 12:53:37.000000 neo_grammar_graph-0.0.5/tests/test_doctests.py
```

### Comparing `neo_grammar_graph-0.0.4/LICENSE` & `neo_grammar_graph-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neo_grammar_graph-0.0.4/PKG-INFO` & `neo_grammar_graph-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo_grammar_graph
-Version: 0.0.4
+Version: 0.0.5
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -707,26 +707,26 @@
 This project is a re-implementation of [GrammarGraph](https://github.com/rindPHI/GrammarGraph/)
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
+* Creating sub graphs
+* Filter abstraction
 * Reachability of grammar symbols.
 * Computing the shortest path or all paths between two grammar symbols.
+* Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a
+  k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of
+  derivation trees based on that.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
-* Creating sub graphs
-* Filter abstraction
 * Checking whether a (sub) graph represents a tree
-* Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a 
-  k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of 
-  derivation trees based on that.
 
 ## Install
 
 NeoGrammarGraph requires at least Python 3.10 and a working installation of graph-tool.
 We refer to the graph-tool homepage (https://graph-tool.skewed.de/) for instructions
 on how to obtain graph-tool. On a MacOS system, we recommend the installation using
 `homebrew`; on Debian/Ubuntu, there's a custom APT repository to be used with `apt-get`.
```

### Comparing `neo_grammar_graph-0.0.4/README.md` & `neo_grammar_graph-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 This project is a re-implementation of [GrammarGraph](https://github.com/rindPHI/GrammarGraph/)
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
+* Creating sub graphs
+* Filter abstraction
 * Reachability of grammar symbols.
 * Computing the shortest path or all paths between two grammar symbols.
+* Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a
+  k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of
+  derivation trees based on that.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
-* Creating sub graphs
-* Filter abstraction
 * Checking whether a (sub) graph represents a tree
-* Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a 
-  k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of 
-  derivation trees based on that.
 
 ## Install
 
 NeoGrammarGraph requires at least Python 3.10 and a working installation of graph-tool.
 We refer to the graph-tool homepage (https://graph-tool.skewed.de/) for instructions
 on how to obtain graph-tool. On a MacOS system, we recommend the installation using
 `homebrew`; on Debian/Ubuntu, there's a custom APT repository to be used with `apt-get`.
```

### Comparing `neo_grammar_graph-0.0.4/pyproject.toml` & `neo_grammar_graph-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neo_grammar_graph"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "Graphs from Context-Free Grammars."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `neo_grammar_graph-0.0.4/setup.cfg` & `neo_grammar_graph-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	numpy>=1.24.2
-	proxyorderedset>=0.3.0
+	proxyorderedset>=0.3.2
 	scipy>=1.10.1
 
 [options.extras_require]
 test = 
 	pytest-pycharm>=0.7.0
 	pytest-xdist==2.5.0
 	pytest>=6.2.5
```

### Comparing `neo_grammar_graph-0.0.4/src/neo_grammar_graph/gg.py` & `neo_grammar_graph-0.0.5/src/neo_grammar_graph/gg.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,58 +11,202 @@
 # NeoGrammarGraph is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NeoGrammarGraph.  If not, see <http://www.gnu.org/licenses/>.
-
 import os.path
-from typing import Dict, List, Callable, Optional, Tuple
+from functools import lru_cache
+from typing import Dict, List, Callable, Optional, Tuple, Any
 
-from graph_tool import Graph, Vertex, Edge
+from graph_tool import Graph, Vertex, Edge, GraphView
 from graph_tool.search import bfs_search, BFSVisitor, StopSearch
 from graph_tool.topology import transitive_closure, all_paths
 from orderedset import OrderedSet
 
-from neo_grammar_graph.helpers import split_expansion
+from neo_grammar_graph.helpers import split_expansion, grammar_terminals
 from neo_grammar_graph.type_defs import Grammar
 
 
 class NeoGrammarGraph:
-    def __init__(self, grammar: Grammar):
+    def __init__(
+        self,
+        grammar: Grammar,
+        _graph: Optional[Graph] = None,
+        _closure: Optional[Graph] = None,
+        _choice_nodes: Optional[OrderedSet[str]] = None,
+        _nonterminal_vertex_map: Optional[Dict[str, Vertex]] = None,
+    ):
         """
         Constructs a :class:`~grammar_graph.NeoGrammarGraph` from the given
         :class:`~grammar_graph.type_defs.Grammar`.
 
         :param grammar: The grammar to construct the
             :class:`~grammar_graph.NeoGrammarGraph` object from.
+        :param _graph: An optional graph object. For internal purposes.
+        :param _closure: An optional transitive closure of the passed graph object.
+            For internal purposes.
+        :param _choice_nodes: The choice nodes in the graph object. For internal
+            purposes.
+        :param _nonterminal_vertex_map: An optional mapping from grammar symbols to
+            the corresponding vertex objects. For internal purposes.
+        """
+
+        # Either none or all of the optional arguments (but :code:`_closure`) should
+        # be provided.
+        assert (
+            _graph is None
+            and _closure is None
+            and _choice_nodes is None
+            and _nonterminal_vertex_map is None
+            or _graph is not None
+            and _choice_nodes is not None
+            and _nonterminal_vertex_map is not None
+        )
+
+        self.grammar: Grammar = grammar
+        self.graph: Graph = _graph or Graph()
+        self.closure: Optional[Graph] = _closure
+        self.choice_nodes: OrderedSet[str] = _choice_nodes or OrderedSet()
+        self.nonterminal_vertex_map: Dict[str, Vertex] = _nonterminal_vertex_map or {}
+
+        # Cache
+        self.__hash: Optional[int] = None
+
+        if _graph is None:
+            self.initialize_graph()
+
+    def __eq__(self, other: Any) -> bool:
+        """
+        Returns True if the other object is a NeoGrammarGraph object with the same
+        grammar.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        A graph equals itself.
+
+        >>> graph == graph
+        True
+
+        Two different graph objects are equal if they have the same grammar.
+
+        >>> NeoGrammarGraph(grammar) == NeoGrammarGraph(grammar)
+        True
+
+        But it is different from a proper subgraph of itself.
+
+        >>> NeoGrammarGraph(grammar) == NeoGrammarGraph(grammar).subgraph("<assgn>")
+        False
+
+        :param other: The object to compare.
+        :return: True if the other object is a NeoGrammarGraph object with the same
+            grammar.
+        """
+
+        return isinstance(other, NeoGrammarGraph) and self.grammar == other.grammar
+
+    def __hash__(self):
+        """
+        Computes the hash of this grammar graph object based on the grammar. The hash
+        is cached.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        The hashes of graph objects with the same grammar are equal.
+
+        >>> hash(NeoGrammarGraph(grammar)) == hash(NeoGrammarGraph(grammar))
+        True
+
+        The hash of a sub graph is (in this example!) different.
+
+        >>> hash(NeoGrammarGraph(grammar)) == \
+                hash(NeoGrammarGraph(grammar).subgraph("<assgn>"))
+        False
+
+        The sub graph for :code:`<start>` is the same as the original graph, so the
+        hashes are also identical.
+
+        >>> hash(NeoGrammarGraph(grammar)) == \
+                hash(NeoGrammarGraph(grammar).subgraph("<start>"))
+        True
+
+        :return: A has value for this graph.
+        """
+
+        if self.__hash is None:
+            self.__hash = hash(
+                tuple(
+                    [
+                        (nonterminal, tuple(expansions))
+                        for nonterminal, expansions in self.grammar.items()
+                    ]
+                )
+            )
+
+        return self.__hash
+
+    def initialize_graph(self):
         """
-        self.grammar = grammar
-        self.graph = Graph()
-        self.closure = None
+        Initializes the graph: Adds vertices and edges according to the grammar,
+        registers choice nodes, sets the vertex labels to the corresponding grammar
+        symbols, and populates the map from grammar symbols to vertices.
 
-        edges = []
+        :return: Nothing. Writes to :code:`self.choice_nodes`, :code:`self.graph`,
+            and resets :code:`self.nonterminal_vertex_map`.
+        """
 
+        edges: List[Tuple[str, str, int]] = []
         for nonterminal in self.grammar:
             for nr, alternative in enumerate(self.grammar[nonterminal]):
                 choice_node_name = f"{nonterminal}-choice-{nr + 1}"
+                self.choice_nodes.add(choice_node_name)
                 edges.append((nonterminal, choice_node_name, 1))
                 edges.extend(
                     [
                         (choice_node_name, expansion_element, 1)
                         for expansion_element in split_expansion(alternative)
                     ]
                 )
 
-        self.edge_weights = self.graph.new_ep("double")
+        edge_weights = self.graph.new_ep("double")
         self.graph.vp.label = self.graph.add_edge_list(
-            edges, hashed=True, eprops=[self.edge_weights]
+            edges, hashed=True, eprops=[edge_weights]
         )
-        self.nonterminal_vertex_map: Dict[str, Vertex] = {
+        self.nonterminal_vertex_map = {
             self.graph.vp.label[v]: v for v in self.graph.vertices()
         }
 
     def vertex_idx(self, symbol: str) -> Optional[int]:
         """
         Returns the vertex index for the given grammar symbol.
 
@@ -148,14 +292,92 @@
         :param symbol: The grammar symbol.
         :return: The vertex object for the given grammar symbol in the graph, or None
             if the symbol does not exist in the graph.
         """
 
         return self.nonterminal_vertex_map.get(symbol, None)
 
+    def nodes(self) -> List[str]:
+        """
+        Returns a list of all graph nodes, including the artificial choice nodes.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        Including terminal symbols and choice nodes, there are 86 nodes in the graph:
+
+        >>> len(graph.nodes())
+        86
+
+        These are the first ten nodes:
+
+        >>> graph.nodes()[:6]
+        ['<start>', '<start>-choice-1', '<stmt>', '<stmt>-choice-1', '<assgn>', ' ; ']
+
+        :return: All nodes in this grammar graph.
+        """
+
+        return [self.symbol(v) for v in self.graph.vertices()]
+
+    def edges(self) -> List[Tuple[str, str]]:
+        """
+        Returns a list of all edges in this graph.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        >>> print("\\n".join(map(str, graph.edges()[:10])))
+        ('<start>', '<start>-choice-1')
+        ('<start>-choice-1', '<stmt>')
+        ('<stmt>', '<stmt>-choice-1')
+        ('<stmt>', '<stmt>-choice-2')
+        ('<stmt>-choice-1', '<assgn>')
+        ('<stmt>-choice-1', ' ; ')
+        ('<stmt>-choice-1', '<stmt>')
+        ('<assgn>', '<assgn>-choice-1')
+        ('<stmt>-choice-2', '<assgn>')
+        ('<assgn>-choice-1', '<var>')
+
+        :return: All edges in the grammar graph. Contains edges to artificial
+            "choice nodes."
+        """
+
+        return [
+            (self.symbol(edge.source()), self.symbol(edge.target()))
+            for edge in self.graph.edges()
+        ]
+
     def symbol(self, vertex: Vertex) -> str:
         """
         Returns the symbol (terminal or nonterminal symbols from the grammar or choice
         node identifiers) for the given graph vertex.
 
         >>> import string
         >>> grammar = {
@@ -222,14 +444,251 @@
 
         vertex = self.vertex(symbol)
         if vertex is None:
             return None
 
         return [self.symbol(child_vertex) for child_vertex in vertex.out_neighbors()]
 
+    def subgraph(self, start_nonterminal: str) -> "NeoGrammarGraph":
+        """
+        Computes a sub graph for that part of the grammar starting with
+        :code:`start_nonterminal`. The resulting grammar will still start with
+        "<start>", but this initial nonterminal will be connected to
+        :code:`start_nonterminal`.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        The nonterminals of the sub graph correspond to those reachable from the chosen
+        start nonterminal. In particular, :code:`<stmt>` is missing in the below
+        example:
+
+        >>> subgraph = graph.subgraph("<assgn>")
+        >>> list(subgraph.grammar.keys())
+        ['<start>', '<assgn>', '<rhs>', '<var>', '<digit>']
+
+        The :code:`<start>` nonterminal is connected to :code:`start_nonterminal`:
+
+        >>> [(s, t) for s, t in subgraph.edges() if s == "<start>" or t == "<assgn>"]
+        [('<start>', '<start>-choice-1'), ('<start>-choice-1', '<assgn>')]
+
+        The only edge of a sub graph not contained in the original graph is part of
+        the connection of :code:`<start>` to the :code:`start_nonterminal` (via the
+        corresponding choice node):
+
+        >>> set(subgraph.edges()).difference(set(graph.edges()))
+        {('<start>-choice-1', '<assgn>')}
+
+        Two arbitrary nodes in the subgraph are connected if, and only if, they are
+        connected in the original graph:
+
+        >>> for n_1 in subgraph.nodes():
+        ...     for n_2 in subgraph.nodes():
+        ...         assert (
+        ...             not graph.reachable(n_1, n_2) and
+        ...             not subgraph.reachable(n_1, n_2) or
+        ...             graph.reachable(n_1, n_2) and
+        ...             subgraph.reachable(n_1, n_2))
+
+        The "sub graph" for the nonterminal symbol :code:`<start>` itself is the
+        original graph:
+
+        >>> graph is graph.subgraph("<start>")
+        True
+
+        :param start_nonterminal: The nonterminal symbol determining the sub grammar
+            of the sub graph to be computed.
+        :return: A sub graph for the grammar starting with :code:`start_nonterminal`.
+            The resulting graph/grammar satisfy the convention that the grammar starts
+            with the initial symbol :code:`<start>`, which is connected to
+            :code:`start_nonterminal`.
+        """
+
+        # We always assume the start nonterminal of a grammar to be :code:`<start>`.
+        # If this nonterminal is given, we return the original NeoGrammarGraph object.
+        # Note that we do not copy the object, it will literally be the same one.
+        if start_nonterminal == "<start>":
+            return self
+
+        start_vertex = self.vertex(start_nonterminal)
+        assert start_vertex is not None
+
+        # Create the new grammar using graph reachability
+        new_grammar = {"<start>": [start_nonterminal]} | {
+            nonterminal: list(expansion)
+            for nonterminal, expansion in self.grammar.items()
+            if nonterminal == start_nonterminal
+            or self.reachable(start_nonterminal, nonterminal)
+        }
+
+        # Construct the reachability property used for filtering
+        reachable = self.graph.new_vertex_property("bool")
+
+        for vertex in self.graph.vertices():
+            reachable[vertex] = vertex == start_vertex or self.reachable(
+                start_nonterminal, self.graph.vp.label[vertex]
+            )
+
+        # Create the new graph-tool graph as a filtered version of the original one.
+        new_graph = Graph(g=GraphView(self.graph, vfilt=reachable))
+        # We make the view irreversible. Otherwise, we experience problems with some
+        # functionality, such as DOT export.
+        new_graph.purge_vertices()
+
+        # We update the choice nodes set; all unreachable nodes are removed.
+        new_choice_nodes = OrderedSet(
+            [symbol for symbol in self.choice_nodes if reachable[self.vertex(symbol)]]
+        )
+
+        # We create a new "<start>" vertex with a single choice node pointing to
+        # the chosen `start_nonterminal`. This is required since "<start>" needs to
+        # be the start nonterminal by convention.
+        new_start_vertex = new_graph.add_vertex()
+        new_graph.vp.label[new_start_vertex] = "<start>"
+        new_choice_vertex = new_graph.add_vertex()
+        new_choice_label = "<start>-choice-1"
+        new_graph.vp.label[new_choice_vertex] = new_choice_label
+        new_choice_nodes.add(new_choice_label)
+
+        # Since IDs might have changed, we update the nonterminal vertex map.
+        new_nonterminal_vertex_map = {
+            new_graph.vp.label[v]: v for v in new_graph.vertices()
+        }
+
+        # With the new vertex information, we add the edges connecting the new
+        # initial nonterminal and the chosen start node.
+        new_graph.add_edge(new_start_vertex, new_choice_vertex)
+        new_graph.add_edge(
+            new_choice_vertex, new_nonterminal_vertex_map[start_nonterminal]
+        )
+
+        return NeoGrammarGraph(
+            new_grammar, new_graph, None, new_choice_nodes, new_nonterminal_vertex_map
+        )
+
+    def is_tree(self) -> bool:
+        """
+        Checks whether this graph is a tree, i.e., each node has exactly one parent.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        The assignment language grammar is recursive, so it cannot be a tree.
+
+        >>> graph.is_tree()
+        False
+
+        Though assignments are not recursive, they are no trees: The :code:`<var>` node
+        is reachable from an assignment or a :code:`<rhs>` nonterminal. The subgraph
+        for :code:`<assgn>` is a directed, acyclic graph (DAG).
+
+        >>> graph.subgraph("<assgn>").is_tree()
+        False
+
+        >>> graph.subgraph("<rhs>").is_tree()
+        True
+
+        :return:
+        """
+
+        class TreeVisitor(BFSVisitor):
+            def __init__(self):
+                self.result = True
+
+            def non_tree_edge(self, e):
+                self.result = False
+                raise StopSearch()
+
+        v = TreeVisitor()
+        bfs_search(self.graph, source=self.vertex("<start>"), visitor=v)
+
+        return v.result
+
+    def filter(self, filter_function: Callable[[str], bool]) -> OrderedSet[str]:
+        """
+        Computes the set of graph nodes satisfying the criterion determined by
+        :code:`filter_function`.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        Filtering out all choice nodes and all terminal symbols (nodes without children)
+        yields all grammar nonterminals.
+
+        >>> list(graph.filter(
+        ...     lambda symbol:
+        ...         symbol not in graph.choice_nodes
+        ...         and graph.children(symbol)))
+        ['<start>', '<stmt>', '<assgn>', '<var>', '<rhs>', '<digit>']
+
+        On the other hand, we can also specifically ask for all symbols whose nodes
+        don't have children, i.e., the terminal symbols:
+
+        >>> list(graph.filter(lambda symbol: not graph.children(symbol)))[:14]
+        [' ; ', ' := ', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l']
+
+        :param filter_function: A function taking a grammar symbol (nonterminals,
+            terminals, or choice nodes) and deciding whether it should be filtered out
+            (return False) or kept (return True).
+        :return: All grammar symbols (potentially including choice nodes) satisfying
+            the given filter criterion.
+        """
+
+        prop = self.graph.new_vertex_property("bool")
+
+        for vertex in self.graph.vertices():
+            prop[vertex] = filter_function(self.symbol(vertex))
+
+        # Create the new graph-tool graph as a filtered version of the original one.
+        return OrderedSet(
+            map(self.symbol, Graph(g=GraphView(self.graph, vfilt=prop)).vertices())
+        )
+
     def reachable(self, from_nonterminal: str, to_nonterminal: str) -> bool:
         """
         Checks whether the nonterminal symbol :code:`to_nonterminal` is reachable
         in the graph from the nonterminal symbol :code:`from_nonterminal`. Note that
         reachability is not reflexive; a nonterminal is only reachable from itself if
         there is an actual path starting and ending at that nonterminal.
 
@@ -521,15 +980,16 @@
 
         # Filter out empty paths (from which the target is not reachable).
         paths = [path for path in paths if path]
 
         if not paths:
             return []
 
-        sorted(paths, key=len)
+        # We sort paths by increasing length since we're interested in the shortest one.
+        paths = sorted(paths, key=len)
 
         result: List[str]
 
         if not node_filter(0, source_nonterminal):
             # If the start node itself should not be included in the result, we can
             # take the path as-is (it was constructed with a choice node as starting
             # vertex).
@@ -547,15 +1007,15 @@
 
     def paths_between(
         self,
         start_symbol: str,
         target_symbol: str,
         node_filter: Callable[[int, str], bool] = lambda idx, _: idx % 2 == 0,
     ) -> Optional[OrderedSet[Tuple[str, ...]]]:
-        """
+        r"""
         Returns a list of all paths between the given grammar symbols.
 
         Example:
 
         >>> import string
         >>> grammar = {
         ...     "<start>":
@@ -570,27 +1030,34 @@
         ...     "<digit>": list(string.digits)
         ... }
         >>> graph = NeoGrammarGraph(grammar)
 
         There are two paths from :code:`<stmt>` to :code:`digit` if we omit the
         filtering of intermediate choice nodes:
 
-        >>> str(graph.paths_between("<stmt>", "<digit>", lambda idx, sym: True))
-        "{('<stmt>', '<stmt>-choice-1', '<assgn>', '<assgn>-choice-1', '<rhs>', '<rhs>-choice-2', '<digit>'), ('<stmt>', '<stmt>-choice-2', '<assgn>', '<assgn>-choice-1', '<rhs>', '<rhs>-choice-2', '<digit>')}"
+        >>> print("\n".join(map(
+        ...     str, graph.paths_between("<stmt>", "<digit>", lambda idx, sym: True))))
+        ('<stmt>', '<stmt>-choice-1', '<assgn>', '<assgn>-choice-1', '<rhs>', '<rhs>-choice-2', '<digit>')
+        ('<stmt>', '<stmt>-choice-2', '<assgn>', '<assgn>-choice-1', '<rhs>', '<rhs>-choice-2', '<digit>')
 
         With the default node filter, those paths collapse to a single one:
 
         >>> str(graph.paths_between("<stmt>", "<digit>"))
         "{('<stmt>', '<assgn>', '<rhs>', '<digit>')}"
 
         There is no path from :code:`<digit>` to itself:
 
         >>> str(graph.paths_between("<digit>", "<digit>"))
         '{}'
 
+        Path computation for self-reachable symbols works as expected.
+
+        >>> str(graph.paths_between("<stmt>", "<stmt>"))
+        "{('<stmt>', '<stmt>')}"
+
         If a symbol does not exist, we obtain :code:`None`:
 
         >>> graph.paths_between("<some-digit>", "<digit>") is None
         True
 
         :param start_symbol: The start symbol of the desired paths.
         :param target_symbol: The target symbol of the desired paths.
@@ -604,22 +1071,158 @@
 
         start_vertex = self.vertex(start_symbol)
         target_vertex = self.vertex(target_symbol)
 
         if start_vertex is None or target_vertex is None:
             return None
 
-        return OrderedSet([
-            tuple([
-                self.symbol(self.graph.vertex(vid))
-                for idx, vid in enumerate(path)
-                if node_filter(idx, self.symbol(self.graph.vertex(vid)))
-            ])
-            for path in all_paths(self.graph, start_vertex, target_vertex)
-        ])
+        return OrderedSet(
+            [
+                tuple(
+                    [
+                        self.symbol(self.graph.vertex(vid))
+                        for idx, vid in enumerate(path)
+                        if node_filter(idx, self.symbol(self.graph.vertex(vid)))
+                    ]
+                )
+                for path in all_paths(self.graph, start_vertex, target_vertex)
+            ]
+        )
+
+    @lru_cache(maxsize=None)
+    def k_paths(
+        self,
+        k: int,
+        up_to: bool = False,
+        start_nonterminal: Optional[str] = None,
+        include_terminals=True,
+    ) -> OrderedSet[Tuple[str, ...]]:
+        """
+        This function computes all paths of length k in the graph, optionally restricted
+        to those reachable from the nonterminal :code:`start_nonterminal`. If up_to
+        is True, also smaller paths are considered. The artificial "choice nodes" are
+        not considered in the length computation and will not be contained in the
+        returned results. k-paths ending in terminal symbols are included if, and only
+        if, include_nonterminals is True.
+
+        Example:
+
+        >>> import string
+        >>> grammar = {
+        ...     "<start>":
+        ...         ["<stmt>"],
+        ...     "<stmt>":
+        ...         ["<assgn> ; <stmt>", "<assgn>"],
+        ...     "<assgn>":
+        ...         ["<var> := <rhs>"],
+        ...     "<rhs>":
+        ...         ["<var>", "<digit>"],
+        ...     "<var>": list(string.ascii_lowercase),
+        ...     "<digit>": list(string.digits)
+        ... }
+        >>> graph = NeoGrammarGraph(grammar)
+
+        The 1-paths in the graph correspond to the nonterminal symbols (dictionary
+        keys) in the underlying grammar.
+
+        >>> str(graph.k_paths(1, include_terminals=False))
+        "{('<start>',), ('<stmt>',), ('<assgn>',), ('<var>',), ('<rhs>',), ('<digit>',)}"
+
+        We can ask for paths starting at a particular nonterminal.
+
+        >>> str(graph.k_paths(2, start_nonterminal="<digit>"))
+        "{('<digit>', '0'), ('<digit>', '1'), ('<digit>', '2'), ('<digit>', '3'), ('<digit>', '4'), ('<digit>', '5'), ('<digit>', '6'), ('<digit>', '7'), ('<digit>', '8'), ('<digit>', '9')}"
+
+        Paths ending in terminal symbols can be excluded on demand.
+
+        >>> str(graph.k_paths(
+        ...     3,
+        ...     start_nonterminal="<assgn>",
+        ...     include_terminals=False))
+        "{('<assgn>', '<rhs>', '<var>'), ('<assgn>', '<rhs>', '<digit>')}"
+
+        If up_to is set to True, we also obtain paths shorter than the set k.
+
+        >>> str(graph.k_paths(
+        ...     3,
+        ...     start_nonterminal="<assgn>",
+        ...     up_to=True,
+        ...     include_terminals=False))
+        "{('<assgn>',), ('<assgn>', '<var>'), ('<var>',), ('<rhs>', '<var>'), ('<assgn>', '<rhs>', '<var>'), ('<assgn>', '<rhs>'), ('<rhs>',), ('<rhs>', '<digit>'), ('<assgn>', '<rhs>', '<digit>'), ('<digit>',)}"
+
+        For certain configurations, we might obtain an empty set of paths.
+
+        >>> str(graph.k_paths(
+        ...     4,
+        ...     start_nonterminal="<assgn>",
+        ...     include_terminals=False))
+        '{}'
+
+        :param k: The length of the paths to return. Maximal length if up_to is True,
+            otherwise the exact lenght.
+        :param up_to: Set to True iff you are interested also in paths shorter than k.
+        :param start_nonterminal: If present, only k-paths in the part of the grammar
+            reachable from this nonterminal will be considered.
+        :param include_terminals: Set to True iff you are interested in paths ending
+            in terminal symbols.
+        :return: The set of paths according to the chosen parameters.
+        """
+
+        # Each path of k terminal/nonterminal nodes includes k-1 choice nodes
+        k += k - 1
+
+        path_map: Dict[Vertex, List[Tuple[Vertex, ...]]] = {}
+
+        class PathVisitor(BFSVisitor):
+            def examine_edge(self, e: Edge):
+                path_map.setdefault(e.source(), []).append((e.source(),))
+                path_map.setdefault(e.target(), []).append((e.source(), e.target()))
+
+                prefixes = [
+                    path for path in path_map.get(e.source(), []) if len(path) < k
+                ]
+                if not prefixes:
+                    return
+
+                path_map[e.target()].extend(
+                    [prefix + (e.target(),) for prefix in prefixes]
+                )
+
+        bfs_search(
+            self.graph,
+            self.vertex(start_nonterminal) if start_nonterminal is not None else None,
+            PathVisitor(),
+        )
+
+        all_terminals = OrderedSet()
+        if not include_terminals:
+            all_terminals = grammar_terminals(self.grammar)
+
+        # We collect all the paths from `path_map` that do not start or end
+        # in a choice node and have a suitable length. Furthermore, we eliminate
+        # paths ending in terminal symbols if the corresponding flag is set.
+        paths = [
+            path
+            for path_set in path_map.values()
+            for path in path_set
+            if self.symbol(path[0]) not in self.choice_nodes
+            and self.symbol(path[-1]) not in self.choice_nodes
+            and (up_to or len(path) == k)
+            and self.symbol(path[-1]) not in all_terminals
+        ]
+
+        # For the final result, we remove choice nodes and convert vertex objects
+        # to grammar string symbols.
+
+        return OrderedSet(
+            [
+                tuple([self.symbol(v) for idx, v in enumerate(path) if idx % 2 == 0])
+                for path in paths
+            ]
+        )
 
     def save_to_dot(self, file_name: str) -> None:
         """
         Saves the graph as a DOT digraph that can be, e.g., exported to a PNG file
         using :code:`dot -Tpng dot_file_name.dot -o out.png`. If the given file name
         does not end in :code:`.dot`, this ending is appended to the file name.
```

### Comparing `neo_grammar_graph-0.0.4/src/neo_grammar_graph.egg-info/PKG-INFO` & `neo_grammar_graph-0.0.5/src/neo_grammar_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-grammar-graph
-Version: 0.0.4
+Version: 0.0.5
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/NeoGrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -707,26 +707,26 @@
 This project is a re-implementation of [GrammarGraph](https://github.com/rindPHI/GrammarGraph/)
 based on the efficient [graph-tool](https://graph-tool.skewed.de/) library. As of now,
 it does not support the full set of features supported by GrammarGraph; however, all
 implemented features should work significantly more efficiently thanks to graph-tool.
 
 ## Supported Features
 
+* Creating sub graphs
+* Filter abstraction
 * Reachability of grammar symbols.
 * Computing the shortest path or all paths between two grammar symbols.
+* Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a
+  k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of
+  derivation trees based on that.
 * Export to GraphViz DOT files.
 
 ## Planned Features
 
-* Creating sub graphs
-* Filter abstraction
 * Checking whether a (sub) graph represents a tree
-* Computing k-paths (paths of exactly length k) in grammars and derivation trees, and a 
-  k-path coverage measure ([see this paper](https://ieeexplore.ieee.org/document/8952419)) of 
-  derivation trees based on that.
 
 ## Install
 
 NeoGrammarGraph requires at least Python 3.10 and a working installation of graph-tool.
 We refer to the graph-tool homepage (https://graph-tool.skewed.de/) for instructions
 on how to obtain graph-tool. On a MacOS system, we recommend the installation using
 `homebrew`; on Debian/Ubuntu, there's a custom APT repository to be used with `apt-get`.
```

