# Comparing `tmp/geneagrapher-1.0.tar.gz` & `tmp/geneagrapher-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geneagrapher-1.0.tar", last modified: Sat Oct  6 06:23:29 2018, max compression
+gzip compressed data, was "geneagrapher-2.0.0.tar", max compression
```

## Comparing `geneagrapher-1.0.tar` & `geneagrapher-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,9 @@
-drwxr-xr-x   0 davidalber   (502) staff       (20)        0 2018-10-06 06:23:29.000000 geneagrapher-1.0/
--rw-r--r--   0 davidalber   (502) staff       (20)     7042 2018-10-06 06:23:29.000000 geneagrapher-1.0/PKG-INFO
-drwxr-xr-x   0 davidalber   (502) staff       (20)        0 2018-10-06 06:23:29.000000 geneagrapher-1.0/tests/
--rw-r--r--   0 davidalber   (502) staff       (20)        0 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/__init__.py
-drwxr-xr-x   0 davidalber   (502) staff       (20)        0 2018-10-06 06:23:29.000000 geneagrapher-1.0/tests/geneagrapher/
--rw-r--r--   0 davidalber   (502) staff       (20)    14401 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/test_graph_methods.py
--rw-r--r--   0 davidalber   (502) staff       (20)     4705 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/test_record_methods.py
--rw-r--r--   0 davidalber   (502) staff       (20)    18334 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/test_geneagrapher_methods.py
--rw-r--r--   0 davidalber   (502) staff       (20)     8264 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/test_grabber_methods.py
--rw-r--r--   0 davidalber   (502) staff       (20)        0 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/__init__.py
--rw-r--r--   0 davidalber   (502) staff       (20)      992 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/local_data_grabber.py
--rw-r--r--   0 davidalber   (502) staff       (20)     4216 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/test_node_methods.py
--rw-r--r--   0 davidalber   (502) staff       (20)    11166 2018-10-04 06:25:07.000000 geneagrapher-1.0/tests/geneagrapher/test_cache_grabber.py
--rw-r--r--   0 davidalber   (502) staff       (20)     5206 2018-10-06 05:49:24.000000 geneagrapher-1.0/README.md
--rw-r--r--   0 davidalber   (502) staff       (20)     1013 2018-10-06 06:18:50.000000 geneagrapher-1.0/setup.py
--rw-r--r--   0 davidalber   (502) staff       (20)       38 2018-10-06 06:23:29.000000 geneagrapher-1.0/setup.cfg
-drwxr-xr-x   0 davidalber   (502) staff       (20)        0 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher/
--rw-r--r--   0 davidalber   (502) staff       (20)     3681 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/grabber.py
--rw-r--r--   0 davidalber   (502) staff       (20)     6713 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/geneagrapher.py
-drwxr-xr-x   0 davidalber   (502) staff       (20)        0 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher/graph/
--rw-r--r--   0 davidalber   (502) staff       (20)     5793 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/graph/graph.py
--rw-r--r--   0 davidalber   (502) staff       (20)       92 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/graph/__init__.py
--rw-r--r--   0 davidalber   (502) staff       (20)     2447 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/graph/record.py
--rw-r--r--   0 davidalber   (502) staff       (20)     1981 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/graph/node.py
--rw-r--r--   0 davidalber   (502) staff       (20)        0 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/__init__.py
--rw-r--r--   0 davidalber   (502) staff       (20)     1787 2018-10-04 06:25:07.000000 geneagrapher-1.0/geneagrapher/cache_grabber.py
-drwxr-xr-x   0 davidalber   (502) staff       (20)        0 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/
--rw-r--r--   0 davidalber   (502) staff       (20)     7042 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/PKG-INFO
--rw-r--r--   0 davidalber   (502) staff       (20)      804 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/SOURCES.txt
--rw-r--r--   0 davidalber   (502) staff       (20)       65 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/entry_points.txt
--rw-r--r--   0 davidalber   (502) staff       (20)       34 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/requires.txt
--rw-r--r--   0 davidalber   (502) staff       (20)       19 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/top_level.txt
--rw-r--r--   0 davidalber   (502) staff       (20)        1 2018-10-06 06:23:29.000000 geneagrapher-1.0/geneagrapher.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0     1075 2023-04-07 19:15:48.028940 geneagrapher-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     6547 2023-04-20 22:50:15.135719 geneagrapher-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-01-28 00:21:39.412670 geneagrapher-2.0.0/geneagrapher/__init__.py
+-rw-r--r--   0        0        0     7631 2023-04-18 22:23:51.344258 geneagrapher-2.0.0/geneagrapher/geneagrapher.py
+-rw-r--r--   0        0        0     2103 2023-04-07 23:37:31.253969 geneagrapher-2.0.0/geneagrapher/output/dot.py
+-rw-r--r--   0        0        0      402 2023-04-07 19:15:48.033513 geneagrapher-2.0.0/geneagrapher/output/identity.py
+-rw-r--r--   0        0        0      530 2023-04-07 19:15:48.034385 geneagrapher-2.0.0/geneagrapher/types.py
+-rw-r--r--   0        0        0      542 2023-04-20 23:03:47.883853 geneagrapher-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7079 1970-01-01 00:00:00.000000 geneagrapher-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `geneagrapher-1.0/PKG-INFO` & `geneagrapher-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,162 @@
-Metadata-Version: 2.1
-Name: geneagrapher
-Version: 1.0
-Summary: Mathematical genealogy grapher.
-Home-page: https://github.com/davidalber/geneagrapher
-Author: David Alber
-Author-email: alber.david@gmail.com
-License: UNKNOWN
-Description: # Geneagrapher
-        Geneagrapher is a tool for extracting information from the
-        [Mathematics Geanealogy
-        Project](https://www.genealogy.math.ndsu.nodak.edu/) to form a
-        geneagraphy. The output is a dot file, which can be used by
-        [Graphviz](https://graphviz.org/) to visualize the tree.
-        
-        ## Basic Concepts
-        The input to the Geneagrapher is a set of starting nodes. If you want
-        to build the ancestor graph of C. Felix Klein, then C. Felix Klein is
-        the starting node for that graph. Multiple starting nodes may be
-        provided (to produce the combined ancestor graph for an academic
-        department, for instance).
-        
-        Each individual stored in the Mathematics Genealogy Project's website
-        has a unique integer as an identifier, and this identifier is what is
-        passed to the Geneagrapher for starting nodes. The identifier is
-        embedded in the URL for records in the Mathematics Genealogy Project
-        website. For example, [Carl
-        Gauß](https://genealogy.math.ndsu.nodak.edu/id.php?id=18231) is ID
-        18231 and [Leonhard
-        Euler](https://genealogy.math.ndsu.nodak.edu/id.php?id=38586) is ID
-        38586.
-        
-        Before running the Geneagrapher, go to the [Mathematics Genealogy
-        Project](https://genealogy.math.ndsu.nodak.edu/) and gather the
-        identifiers of the starting nodes for the graph you have in mind.
-        
-        ## Installation
-        Geneagrapher is installed by pip. If your system does not have pip,
-        see the instructions
-        [here](https://pip.pypa.io/en/stable/installing/).
-        
-        Once pip is available on your system, install Geneagrapher with:
-        ```
-        pip install geneagrapher
-        ```
-        
-        ## Usage
-        After installing the Geneagrapher, running
-        
-        ```
-        ggrapher --help
-        ```
-        
-        should produce
-        
-        ```
-        usage: ggrapher [-h] [--version] [-f FILE] [-a] [-d] [--disable-cache]
-                        [--cache-file FILE] [-v]
-                        ID [ID ...]
-        
-        Create a Graphviz "dot" file for a mathematics genealogy, where ID is a record
-        identifier from the Mathematics Genealogy Project. Multiple IDs may be passed.
-        
-        positional arguments:
-          ID                    mathematician record ID
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --version             show program's version number and exit
-          -f FILE, --file FILE  write output to FILE [default: stdout]
-          -a, --with-ancestors  retrieve ancestors of IDs and include in graph
-          -d, --with-descendants
-                                retrieve descendants of IDs and include in graph
-          --disable-cache       do not store records in local cache
-          --cache-file FILE     write cache to FILE [default: geneacache]
-          -v, --verbose         list nodes being retrieved
-        ```
-        
-        Explanations of some of the options are given below, followed by
-        examples.
-        
-        **-f FILE, --file=FILE**
-        
-        By default, the Geneagrapher writes the data it generates to standard
-        output. If you want the data written to file, you need to redirect the
-        output or use the `-f` or `--file` switch. When one of these switches
-        is used, the data is saved in the file name provided.
-        
-        **-a, --with-ancestors**
-        
-        When one of these switches is provided to the Geneagrapher, an
-        ancestor graph is generated. An ancestor graph starts with the
-        starting nodes and the works up to their advisors, their advisors'
-        advisors, and so on.
-        
-        **-d, --with-descendants**
-        
-        These switches instruct the Geneagrapher to extract information about
-        the descendants of the starting nodes (i.e., their advisees, their
-        advisees' advisees, and so on).
-        
-        ## Processing the Dot File
-        To process the generated dot file,
-        [Graphviz](https://www.graphviz.org/) is needed. Graphviz installs
-        several programs for processing dot files. For the Geneagrapher, I use
-        the dot program. Let's look at an example.
-        
-        If the Geneagrapher has generated a file named "graph.dot", we can do
-        
-        ```
-        dot -Tpng graph.dot > graph.png
-        ```
-        
-        This command produces a PNG file containing the graph. That's really
-        all there is to it. Almost.
-        
-        By default, `dot` renders an image with 96dpi. This can look a little
-        blurry at 100% on high-resolution displays. You might want to increase
-        the resolution. You can do this with the `-Gdpi` flag. For instance,
-        to produce a PNG with 150dpi, you can do
-        
-        ```
-        dot -Tpng -Gdpi=150 graph.dot > graph.png
-        ```
-        
-        ## Examples
-        _Note: the Mathematics Genealogy Project has added new data since the
-        examples below were constructed, so if re-run, the results will look
-        different. The commands, however, all remain correct._
-        
-        ### Single Node Ancestry: Carl Gau&szlig;
-        To produce the ancestry dot file for Carl Gauß and save it in the file
-        'gauss.dot', run the command
-        
-        ```
-        ggrapher -f gauss.dot -a 18231
-        ```
-        
-        ![Gauss math genealogy](https://github.com/davidalber/geneagrapher/raw/master/images/gauss-geneagraph.png)
-        
-        ### Multiple Node Ancestry: Friedrich Bessel and Christian Gerling
-        To produce the combined ancestry dot file for Friedrich Bessel and
-        Christian Gerling and save it in the file 'bessel_gerling.dot', run
-        the command
-        
-        ```
-        ggrapher -f bessel_gerling.dot -a 18603 29642
-        ```
-        
-        ![Bessel-Gerling math genealogy](https://github.com/davidalber/geneagrapher/raw/master/images/bessel-gerling-geneagraph.png)
-        
-        ### Single Node Descendant Graph: Haskell Curry
-        To produce the descendant dot file for Haskell Curry and save it in
-        the file 'curry.dot', run the command
-        
-        ```
-        ggrapher -f curry.dot -d 7398
-        ```
-        
-        ![Curry math genealogy descendants](https://github.com/davidalber/geneagrapher/raw/master/images/curry-geneagraph.png)
-        
-        Note that descendant graphs often have a lot of "fan out".
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# Geneagrapher [![Continuous Integration Status](https://github.com/davidalber/geneagrapher/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/davidalber/geneagrapher/actions/workflows/ci.yaml/badge.svg?branch=main)
+
+Geneagrapher is a tool for building mathematician advisor-advisee
+genealogies using information from the [Mathematics Genealogy
+Project](https://www.mathgenealogy.org/). The output is either a DOT
+file, which can be used by [Graphviz](https://graphviz.org/) to
+visualize the graph, or a JSON structure that you can consume with
+other software tools. Here's an example of a genealogy built by
+Geneagrapher and visualized using Graphviz:
+
+<img src="https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/chioniadis-geneagraph.png" alt="Chioniadis math
+genealogy" width="480px">
+
+To use this package, you will need to have a Python interpreter on
+your system and install this package. Additionally, if you want to
+generate the graph visualization you will need another tool (e.g.,
+[Graphviz](https://www.graphviz.org/)).
+
+If you want to build a math genealogy more easily, you may want to
+look at the [Geneagrapher
+notebook](https://observablehq.com/@davidalber/geneagrapher). That
+Observable notebook creates geneagraphs in your browser.
+
+If you want to consume records from the Math Genealogy Project in your
+own software, you may be interested in
+[geneagrapher-core](https://github.com/davidalber/geneagrapher-core).
+
+## Basic Concepts
+The input to the Geneagrapher is a set of starting nodes and traversal
+directions. Multiple starting nodes may be provided (to produce the
+combined graph for an academic department's students and professors,
+for instance).
+
+### Starting Nodes
+Each individual stored in the Mathematics Genealogy Project's website
+has a unique integer as an identifier, and this identifier is what is
+passed to the Geneagrapher to specify a starting node. The identifier
+is contained in the URL for records in the Mathematics Genealogy
+Project website. For example, [Carl
+Gauß](https://www.mathgenealogy.org/id.php?id=18231) is ID 18231 and
+[Leonhard Euler](https://www.mathgenealogy.org/id.php?id=38586) is ID
+38586.
+
+Before running the Geneagrapher, go to the [Mathematics Genealogy
+Project](https://www.mathgenealogy.org/) and gather the identifiers of
+the starting nodes for the graph you want to build.
+
+### Traversal Directions
+For each starting node, you instruct Geneagrapher to traverse in the
+advisor direction, the descendant (i.e., student) direction, or
+both. For example, if you want to build the graph of a mathematician
+and all of their students, you would specify the descendant traversal
+direction for that starting node.
+
+### Syntax
+When running Geneagrapher, you provide starting nodes on the command
+line. The syntax for doing this is `NODE_ID:TRAVERSAL_DIRECTION`,
+where `TRAVERSAL_DIRECTION` is `a | d`, and `a` and `d` indicate
+advisor and descendant traversal, respectively. Here are some
+examples:
+
+- Carl Gauß and his advisor graph: `18231:a`.
+- Carl Gauß and his descendant graph: `18231:d`.
+- Carl Gauß and his advisor and descendant graphs: `18231:ad`.
+
+## Installation
+To install Geneagrapher, you must have Python >= 3.8.1. Geneagrapher
+is installed by pip. If your system does not have pip, see the
+instructions [here](https://pip.pypa.io/en/stable/installing/).
+
+Once pip is available on your system, install Geneagrapher with:
+```
+pip install geneagrapher
+```
+
+## Usage
+You can get help by doing
+
+```
+ggrapher --help
+```
+
+## Processing the DOT File
+To process the generated DOT file,
+[Graphviz](https://www.graphviz.org/) is needed. Graphviz installs
+several programs for processing DOT files. For the Geneagrapher, use
+the `dot` program. Let's look at an example.
+
+If the Geneagrapher has generated a file named "graph.dot", a PNG file
+containing the graph can be created with the following command.
+
+```
+dot -Tpng graph.dot > graph.png
+```
+
+That's really all there is to it. Almost.
+
+By default, `dot` renders an image with 96dpi. This may not look great
+on high-resolution displays, so you might want to increase the
+resolution. You can do this with the `-Gdpi` flag. For instance, to
+produce a PNG with 150dpi, you can do
+
+```
+dot -Tpng -Gdpi=150 graph.dot > graph.png
+```
+
+Graphviz can also generate other formats, such as PDF and SVG.
+
+## Examples
+Note: the Mathematics Genealogy Project data changes over time, so if
+the examples below are re-run, the results may look different. The
+commands, however, will be the same.
+
+### Single Node Ancestry: Theodor Zwinger
+To produce the ancestry DOT file for Theodor Zwinger and save it in
+the file zwinger.dot, run the command
+
+```
+ggrapher -o zwinger.dot 125148:a
+```
+
+![Zwinger math genealogy](https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/zwinger-geneagraph.png)
+
+### Multiple Node Ancestry: Petrus Ryff and Theodor Zwinger
+To produce the combined ancestry DOT file for Petrus Ryff and Theodor
+Zwinger and save it in the file ryff_zwinger.dot, run the command
+
+```
+ggrapher -o ryff_zwinger.dot 125148:a 130248:a
+```
+
+![Ryff-Zwinger math genealogy](https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/ryff-zwinger-geneagraph.png)
+
+### Single Node Descendant Graph: Haskell Curry
+To produce the descendant DOT file for Haskell Curry and save it in
+the file curry.dot, run the command
+
+```
+ggrapher -o curry.dot 7398:d
+```
+
+![Curry math genealogy descendants](https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/curry-geneagraph.png)
+
+Note that descendant graphs often have a lot of "fan out".
+
+## Technical Details
+Previous versions of Geneagrapher made requests directly to the
+Mathematics Genealogy Project and built the graph in the
+application. The current version of Geneagrapher, however, makes
+requests to an intermediate service that is built using
+[geneagrapher-core](https://github.com/davidalber/geneagrapher-core). This
+backend service assembles requested graphs and maintains a cache of
+records.
+
+While the shared cache substantially reduces the number of requests
+from individuals running Geneagrapher (or the [Geneagrapher
+notebook](https://observablehq.com/@davidalber/geneagrapher)) and
+speeds up the graph-building process, it also creates an opportunity
+for inconsistency between information in the Mathematics Genealogy
+Project and the cache. This can happen when records are updated in the
+Mathematics Genealogy Project. Such inconsistencies will automatically
+be resolved when cached values expire.
```

### Comparing `geneagrapher-1.0/README.md` & `geneagrapher-2.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,154 +1,179 @@
-# Geneagrapher
-Geneagrapher is a tool for extracting information from the
-[Mathematics Geanealogy
-Project](https://www.genealogy.math.ndsu.nodak.edu/) to form a
-geneagraphy. The output is a dot file, which can be used by
-[Graphviz](https://graphviz.org/) to visualize the tree.
+Metadata-Version: 2.1
+Name: geneagrapher
+Version: 2.0.0
+Summary: Mathematical genealogy grapher.
+License: MIT
+Author: David Alber
+Author-email: alber.david@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: websockets (>=10.4,<11.0)
+Description-Content-Type: text/markdown
+
+# Geneagrapher [![Continuous Integration Status](https://github.com/davidalber/geneagrapher/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/davidalber/geneagrapher/actions/workflows/ci.yaml/badge.svg?branch=main)
+
+Geneagrapher is a tool for building mathematician advisor-advisee
+genealogies using information from the [Mathematics Genealogy
+Project](https://www.mathgenealogy.org/). The output is either a DOT
+file, which can be used by [Graphviz](https://graphviz.org/) to
+visualize the graph, or a JSON structure that you can consume with
+other software tools. Here's an example of a genealogy built by
+Geneagrapher and visualized using Graphviz:
+
+<img src="https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/chioniadis-geneagraph.png" alt="Chioniadis math
+genealogy" width="480px">
+
+To use this package, you will need to have a Python interpreter on
+your system and install this package. Additionally, if you want to
+generate the graph visualization you will need another tool (e.g.,
+[Graphviz](https://www.graphviz.org/)).
+
+If you want to build a math genealogy more easily, you may want to
+look at the [Geneagrapher
+notebook](https://observablehq.com/@davidalber/geneagrapher). That
+Observable notebook creates geneagraphs in your browser.
+
+If you want to consume records from the Math Genealogy Project in your
+own software, you may be interested in
+[geneagrapher-core](https://github.com/davidalber/geneagrapher-core).
 
 ## Basic Concepts
-The input to the Geneagrapher is a set of starting nodes. If you want
-to build the ancestor graph of C. Felix Klein, then C. Felix Klein is
-the starting node for that graph. Multiple starting nodes may be
-provided (to produce the combined ancestor graph for an academic
-department, for instance).
+The input to the Geneagrapher is a set of starting nodes and traversal
+directions. Multiple starting nodes may be provided (to produce the
+combined graph for an academic department's students and professors,
+for instance).
 
+### Starting Nodes
 Each individual stored in the Mathematics Genealogy Project's website
 has a unique integer as an identifier, and this identifier is what is
-passed to the Geneagrapher for starting nodes. The identifier is
-embedded in the URL for records in the Mathematics Genealogy Project
-website. For example, [Carl
-Gauß](https://genealogy.math.ndsu.nodak.edu/id.php?id=18231) is ID
-18231 and [Leonhard
-Euler](https://genealogy.math.ndsu.nodak.edu/id.php?id=38586) is ID
+passed to the Geneagrapher to specify a starting node. The identifier
+is contained in the URL for records in the Mathematics Genealogy
+Project website. For example, [Carl
+Gauß](https://www.mathgenealogy.org/id.php?id=18231) is ID 18231 and
+[Leonhard Euler](https://www.mathgenealogy.org/id.php?id=38586) is ID
 38586.
 
 Before running the Geneagrapher, go to the [Mathematics Genealogy
-Project](https://genealogy.math.ndsu.nodak.edu/) and gather the
-identifiers of the starting nodes for the graph you have in mind.
+Project](https://www.mathgenealogy.org/) and gather the identifiers of
+the starting nodes for the graph you want to build.
+
+### Traversal Directions
+For each starting node, you instruct Geneagrapher to traverse in the
+advisor direction, the descendant (i.e., student) direction, or
+both. For example, if you want to build the graph of a mathematician
+and all of their students, you would specify the descendant traversal
+direction for that starting node.
+
+### Syntax
+When running Geneagrapher, you provide starting nodes on the command
+line. The syntax for doing this is `NODE_ID:TRAVERSAL_DIRECTION`,
+where `TRAVERSAL_DIRECTION` is `a | d`, and `a` and `d` indicate
+advisor and descendant traversal, respectively. Here are some
+examples:
+
+- Carl Gauß and his advisor graph: `18231:a`.
+- Carl Gauß and his descendant graph: `18231:d`.
+- Carl Gauß and his advisor and descendant graphs: `18231:ad`.
 
 ## Installation
-Geneagrapher is installed by pip. If your system does not have pip,
-see the instructions
-[here](https://pip.pypa.io/en/stable/installing/).
+To install Geneagrapher, you must have Python >= 3.8.1. Geneagrapher
+is installed by pip. If your system does not have pip, see the
+instructions [here](https://pip.pypa.io/en/stable/installing/).
 
 Once pip is available on your system, install Geneagrapher with:
 ```
 pip install geneagrapher
 ```
 
 ## Usage
-After installing the Geneagrapher, running
+You can get help by doing
 
 ```
 ggrapher --help
 ```
 
-should produce
-
-```
-usage: ggrapher [-h] [--version] [-f FILE] [-a] [-d] [--disable-cache]
-                [--cache-file FILE] [-v]
-                ID [ID ...]
-
-Create a Graphviz "dot" file for a mathematics genealogy, where ID is a record
-identifier from the Mathematics Genealogy Project. Multiple IDs may be passed.
-
-positional arguments:
-  ID                    mathematician record ID
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --version             show program's version number and exit
-  -f FILE, --file FILE  write output to FILE [default: stdout]
-  -a, --with-ancestors  retrieve ancestors of IDs and include in graph
-  -d, --with-descendants
-                        retrieve descendants of IDs and include in graph
-  --disable-cache       do not store records in local cache
-  --cache-file FILE     write cache to FILE [default: geneacache]
-  -v, --verbose         list nodes being retrieved
-```
-
-Explanations of some of the options are given below, followed by
-examples.
-
-**-f FILE, --file=FILE**
-
-By default, the Geneagrapher writes the data it generates to standard
-output. If you want the data written to file, you need to redirect the
-output or use the `-f` or `--file` switch. When one of these switches
-is used, the data is saved in the file name provided.
-
-**-a, --with-ancestors**
-
-When one of these switches is provided to the Geneagrapher, an
-ancestor graph is generated. An ancestor graph starts with the
-starting nodes and the works up to their advisors, their advisors'
-advisors, and so on.
-
-**-d, --with-descendants**
-
-These switches instruct the Geneagrapher to extract information about
-the descendants of the starting nodes (i.e., their advisees, their
-advisees' advisees, and so on).
-
-## Processing the Dot File
-To process the generated dot file,
+## Processing the DOT File
+To process the generated DOT file,
 [Graphviz](https://www.graphviz.org/) is needed. Graphviz installs
-several programs for processing dot files. For the Geneagrapher, I use
-the dot program. Let's look at an example.
+several programs for processing DOT files. For the Geneagrapher, use
+the `dot` program. Let's look at an example.
 
-If the Geneagrapher has generated a file named "graph.dot", we can do
+If the Geneagrapher has generated a file named "graph.dot", a PNG file
+containing the graph can be created with the following command.
 
 ```
 dot -Tpng graph.dot > graph.png
 ```
 
-This command produces a PNG file containing the graph. That's really
-all there is to it. Almost.
+That's really all there is to it. Almost.
 
-By default, `dot` renders an image with 96dpi. This can look a little
-blurry at 100% on high-resolution displays. You might want to increase
-the resolution. You can do this with the `-Gdpi` flag. For instance,
-to produce a PNG with 150dpi, you can do
+By default, `dot` renders an image with 96dpi. This may not look great
+on high-resolution displays, so you might want to increase the
+resolution. You can do this with the `-Gdpi` flag. For instance, to
+produce a PNG with 150dpi, you can do
 
 ```
 dot -Tpng -Gdpi=150 graph.dot > graph.png
 ```
 
+Graphviz can also generate other formats, such as PDF and SVG.
+
 ## Examples
-_Note: the Mathematics Genealogy Project has added new data since the
-examples below were constructed, so if re-run, the results will look
-different. The commands, however, all remain correct._
+Note: the Mathematics Genealogy Project data changes over time, so if
+the examples below are re-run, the results may look different. The
+commands, however, will be the same.
 
-### Single Node Ancestry: Carl Gau&szlig;
-To produce the ancestry dot file for Carl Gauß and save it in the file
-'gauss.dot', run the command
+### Single Node Ancestry: Theodor Zwinger
+To produce the ancestry DOT file for Theodor Zwinger and save it in
+the file zwinger.dot, run the command
 
 ```
-ggrapher -f gauss.dot -a 18231
+ggrapher -o zwinger.dot 125148:a
 ```
 
-![Gauss math genealogy](images/gauss-geneagraph.png)
+![Zwinger math genealogy](https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/zwinger-geneagraph.png)
 
-### Multiple Node Ancestry: Friedrich Bessel and Christian Gerling
-To produce the combined ancestry dot file for Friedrich Bessel and
-Christian Gerling and save it in the file 'bessel_gerling.dot', run
-the command
+### Multiple Node Ancestry: Petrus Ryff and Theodor Zwinger
+To produce the combined ancestry DOT file for Petrus Ryff and Theodor
+Zwinger and save it in the file ryff_zwinger.dot, run the command
 
 ```
-ggrapher -f bessel_gerling.dot -a 18603 29642
+ggrapher -o ryff_zwinger.dot 125148:a 130248:a
 ```
 
-![Bessel-Gerling math genealogy](images/bessel-gerling-geneagraph.png)
+![Ryff-Zwinger math genealogy](https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/ryff-zwinger-geneagraph.png)
 
 ### Single Node Descendant Graph: Haskell Curry
-To produce the descendant dot file for Haskell Curry and save it in
-the file 'curry.dot', run the command
+To produce the descendant DOT file for Haskell Curry and save it in
+the file curry.dot, run the command
 
 ```
-ggrapher -f curry.dot -d 7398
+ggrapher -o curry.dot 7398:d
 ```
 
-![Curry math genealogy descendants](images/curry-geneagraph.png)
+![Curry math genealogy descendants](https://raw.githubusercontent.com/davidalber/geneagrapher/v2.0.0/images/curry-geneagraph.png)
 
 Note that descendant graphs often have a lot of "fan out".
+
+## Technical Details
+Previous versions of Geneagrapher made requests directly to the
+Mathematics Genealogy Project and built the graph in the
+application. The current version of Geneagrapher, however, makes
+requests to an intermediate service that is built using
+[geneagrapher-core](https://github.com/davidalber/geneagrapher-core). This
+backend service assembles requested graphs and maintains a cache of
+records.
+
+While the shared cache substantially reduces the number of requests
+from individuals running Geneagrapher (or the [Geneagrapher
+notebook](https://observablehq.com/@davidalber/geneagrapher)) and
+speeds up the graph-building process, it also creates an opportunity
+for inconsistency between information in the Mathematics Genealogy
+Project and the cache. This can happen when records are updated in the
+Mathematics Genealogy Project. Such inconsistencies will automatically
+be resolved when cached values expire.
+
```

