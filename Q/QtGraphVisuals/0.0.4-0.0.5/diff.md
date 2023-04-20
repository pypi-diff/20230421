# Comparing `tmp/qtgraphvisuals-0.0.4.tar.gz` & `tmp/qtgraphvisuals-0.0.5.tar.gz`

## Comparing `qtgraphvisuals-0.0.4.tar` & `qtgraphvisuals-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/.__main__.py.swp
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/.gitignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/__main__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/default_visual_schemes.json
--rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/widgets.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/tests/test.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/.pyproject.toml.swp
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/src/QtGraphVisuals/.gitignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/src/QtGraphVisuals/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/src/QtGraphVisuals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/src/QtGraphVisuals/__main__.py
+-rw-r--r--   0        0        0    31235 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/src/QtGraphVisuals/widgets.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/tests/.asdf.py.swp
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/tests/.test.py.swp
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/tests/test.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.5/PKG-INFO
```

### Comparing `qtgraphvisuals-0.0.4/src/QtGraphVisuals/__init__.py` & `qtgraphvisuals-0.0.5/src/QtGraphVisuals/__init__.py`

 * *Files identical despite different names*

### Comparing `qtgraphvisuals-0.0.4/src/QtGraphVisuals/__main__.py` & `qtgraphvisuals-0.0.5/src/QtGraphVisuals/__main__.py`

 * *Files identical despite different names*

### Comparing `qtgraphvisuals-0.0.4/src/QtGraphVisuals/widgets.py` & `qtgraphvisuals-0.0.5/src/QtGraphVisuals/widgets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,178 @@
 
-import sys, json, pathlib
+import sys, pathlib
 import networkx as nx
 import numpy as np
 from PySide6.QtCore import (Qt, Signal, Slot, QPoint, QPointF, QLine, QLineF,
-        QRect, QRectF)
-from PySide6.QtWidgets import (QApplication, QWidget, QLabel, QHBoxLayout,
-        QVBoxLayout, QGraphicsView, QGraphicsScene, QGraphicsRectItem,
-        QGraphicsEllipseItem, QGraphicsItem, QGraphicsTextItem, QGraphicsLineItem, QGroupBox,
+        QRect, QRectF) 
+from PySide6.QtWidgets import (QApplication, QWidget, QLabel, QHBoxLayout, QPushButton, QSizePolicy,
+        QVBoxLayout, QGraphicsView, QGraphicsScene, QGraphicsPolygonItem, QGraphicsRectItem,
+        QGraphicsEllipseItem, QGraphicsItem, QGraphicsTextItem, QGraphicsPathItem, QGraphicsLineItem, QGroupBox,
         QScrollArea, QFrame, QTabWidget, QSplitter)
-from PySide6.QtGui import QPainter, QTransform, QBrush, QPen, QColor
+from PySide6.QtGui import QPainterPath, QPainter, QTransform, QBrush, QPen, QColor, QPolygonF, QFont
 
-# Load default visual schemes 
-default_visual_schemes = {}
-path = pathlib.Path(__file__).parent
-with open(path / 'default_visual_schemes.json', 'r') as f:
-    default_visual_schemes = json.loads(f.read())
+def onnxToMultiDiGraph(model):
+    import onnx 
+    def setVisualScheme(graph):
+        # Set Visual Schemes
+        for node_name,data in graph.nodes(data=True):
+            node = data['node']
+            vs = {'boundaySize': 2, 'size': 50, 'label':node_name}
+            if isinstance(node, onnx.ValueInfoProto):
+                graph.nodes[node_name]['visual_scheme'] = vs
+                continue
+
+            vs['label'] = node.op_type.lower()
+            if 'conv' in node.op_type.lower():
+                vs['fillColor'] = 'darkBlue'
+            elif 'pool' in node.op_type.lower():
+                vs['fillColor'] = 'darkgraphreen'
+            elif 'elu' in node.op_type.lower():
+                vs['fillColor'] = 'darkRed'
+                vs['size'] = [50,25]
+            graph.nodes[node_name]['visual_scheme'] = vs
+
+            graph.nodes[node_name]['properties'] = {}
+            graph.nodes[node_name]['properties']['name'] = node_name
+            graph.nodes[node_name]['properties']['inbound'] = list(graph.predecessors(node_name))
+            graph.nodes[node_name]['properties']['outbound'] = list(graph.successors(node_name))
+            graph.nodes[node_name]['properties'].update({attr.name: onnx.helper.get_attribute_value(attr) for attr in list(node.attribute)})
+
+        for u,v,key,data in graph.edges(keys=True, data=True):
+            txt = onnx.helper.printable_value_info(data['value'])
+            graph.edges[u,v,key]['properties'] = {'info': txt}
+
+    # Initialize a NetworkX MultiDiGraph
+    graph = nx.MultiDiGraph(name=model.graph.name)
+
+    # Add nodes to the graph
+    for node in model.graph.node:
+        graph.add_node(node.name, node=node)
+
+    # Add initializer data to the nodes
+    for init in model.graph.initializer:
+        for node in model.graph.node:
+            if init.name in node.input:
+                graph.nodes[node.name][init.name] = init
+    
+    # Add edges to the graph
+    for value in model.graph.value_info:
+        u, v = None, None 
+        in_index, out_index = 0, 0
+        for node in model.graph.node :
+            if value.name in node.output:
+                u = node.name
+                out_index = list(node.output).index(value.name)
+            if value.name in node.input:
+                v = node.name
+                in_index = list(node.input).index(value.name)
+        if u and v:
+            graph.add_edge(u, v, in_index=in_index, out_index=out_index, value=value)
+
+    # Add input / output nodes (and edges) to the graph
+    for inout in list(model.graph.input) + list(model.graph.output):
+        for node in model.graph.node:
+
+            # Add output node
+            if inout.name in node.output:
+                index = list(node.output).index(inout.name)
+                graph.add_node(inout.name, node=inout)
+                graph.add_edge(node.name, inout.name, in_index=index, out_index=0, value=inout)
+                break
+
+            # Add input node
+            if inout.name in node.input:
+                index = list(node.input).index(inout.name)
+                graph.add_node(inout.name, node=inout)
+                graph.add_edge(inout.name, node.name, in_index=0, out_index=index, value=inout)
+                break
+
+    # Adds auxillary information to the graph for visualization purposes
+    setVisualScheme(graph)
+    return graph
+
+def kerasToMultiDiGraph(model):
+    def setVisualScheme(graph):
+        # Set Visual Schemes
+        for node in graph.nodes():
+            ntype = type(node).__name__
+            vs = {'boundaySize': 2, 'size': 50, 'label': ntype}
+
+            if 'conv' in ntype.lower():
+                vs['fillColor'] = 'darkBlue'
+            elif 'pool' in ntype.lower():
+                vs['fillColor'] = 'darkGreen'
+            elif 'elu' in ntype.lower() or 'activation' in ntype.lower():
+                vs['fillColor'] = 'darkRed'
+                vs['size'] = [50,25]
+            elif 'normalization' in ntype.lower():
+                vs['fillColor'] = 'darkMagenta'
+                vs['size'] = [50,25]
+            elif graph.in_degree(node) > 1:
+                vs['fillColor'] = 'black'
+                vs['size'] = [50,25]
+
+            graph.nodes[node]['visual_scheme'] = vs
+            graph.nodes[node]['properties'] = {}
+            graph.nodes[node]['properties']['name'] = node
+            graph.nodes[node]['properties']['inbound'] = list([n.name for n in graph.predecessors(node)])
+            graph.nodes[node]['properties']['outbound'] = list([n.name for n in graph.successors(node)])
+            graph.nodes[node]['properties'].update(node.get_config())
+
+        for u,v,key,data in graph.edges(keys=True, data=True):
+            graph.edges[u,v,key]['properties'] = {'shape': v.output_shape}
+
+    graph = nx.MultiDiGraph()
+
+    # Add all 'Layers' (aka nodes) to the graph
+    graph.add_nodes_from(model.layers)
+
+    # Get a set of all 'Nodes' (aka edges) in the keras graph
+    keras_nodes = []
+    for layer in model.layers:
+        for node in layer.outbound_nodes:
+            keras_nodes.append(node)
+    keras_nodes = set(keras_nodes)
+
+    # Add the edges to the graph
+    for kn in keras_nodes:
+        input_layers = kn.inbound_layers
+        if not isinstance(input_layers, list): 
+            input_layers = [input_layers]
+        output_layer = kn.outbound_layer
+
+        for index, input_layer in enumerate(input_layers):
+            shape = input_layer.output_shape
+            graph.add_edge(input_layer, output_layer,
+                        in_index=0, out_index=index, shape=shape)
+
+    # Adds auxillary information to the graph for visualization purposes
+    setVisualScheme(graph)
+    return graph
 
 ## Application
 class GraphViewer(QWidget):
     def __init__(self, views, parent=None):
         super().__init__(parent)
 
         # Children
         self._tabs = QTabWidget(parent=self)
         self._properties_viewer = PropertiesViewer(parent=self)
+        #self._controls = ControlButtons(parent=self)
 
         # Create views
         self._views = {}
         [self.addView(name, graph) for name,graph in views.items()]
 
         # Layout
-        self.setLayout(QVBoxLayout())
+        self.setLayout(QHBoxLayout())
         self._splitter = QSplitter(Qt.Horizontal)
         self._splitter.addWidget(self._tabs)
         self._splitter.addWidget(self._properties_viewer)
+        #self.layout().addWidget(self._controls)
         self.layout().addWidget(self._splitter)
 
         # Connect
         self._tabs.currentChanged.connect(self.tabChanged)
 
     @Slot(int)
     def tabChanged(self, idx):
@@ -53,18 +188,18 @@
     def removeView(self, view_name):
         if view_name not in self._views:
             raise ValueError(f"{view_name} is not a view")
         gv = self._views.pop(view_name)
         self._tabs.removeTab(self._tabs.indexOf(gv))
         gv.deleteLater()
 
-    def addView(self, view_name, graph, visual_scheme=None):
+    def addView(self, view_name, graph):
         if view_name in self._views:
             raise ValueError(f"{view_name} already exsists")
-        gv = GraphViewerWindow(graph, visual_scheme, parent=self)
+        gv = GraphViewerWindow(graph, parent=self)
         self._views[view_name] = gv
         gv.clicked.connect(self._properties_viewer.setConfig)
         self._tabs.addTab(gv, view_name)
 
     def setView(self, view_name, graph):
         self._views[view_name].setGraph(graph)
 
@@ -134,19 +269,59 @@
         layout.setContentsMargins(0,0,0,0)
         self.setLayout(layout)
 
     def set(self, name, value):
         self._name.setText(f"{name}")
         self._value.setText(f"{value}")
 
+class ControlButtons(QWidget):
+    class SwitchButton(QWidget):
+        def __init__(self, states, parent=None):
+            super().__init__(parent)
+            self.states = states
+            self.state_idx = 0
+
+            self.button = QPushButton(self.states[self.state_idx], parent=self) 
+            self.button.setFont(QFont(self.button.font().family(), 24))
+            self.button.setFixedWidth(self.button.height()+2)
+            self.button.setStyleSheet("QPushButton {padding: 0px; border-width: 0px;}")
+            self.button.clicked.connect(self.click)
+
+            self.setLayout(QVBoxLayout())
+            self.layout().addWidget(self.button)
+            self.layout().setContentsMargins(0,0,0,0)
+
+        @Slot()
+        def click(self, e):
+            print('Click')
+            self.state_idx += 1
+            if self.state_idx >= len(self.states):
+                self.state_idx = 0
+            self.button.setText(self.states[self.state_idx])
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        #self.frame = QFrame(self)
+        #self.frame.setLayout(QVBoxLayout())
+
+        self.setLayout(QVBoxLayout())
+        self.layout().setAlignment(Qt.AlignTop)
+
+        self.button1 = ControlButtons.SwitchButton(list("➡⬇"), parent=self)
+        self.button2 = ControlButtons.SwitchButton(list("◼⚫"), parent=self)
+
+        self.layout().addWidget(self.button1)
+        self.layout().addWidget(self.button2)
+        self.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Maximum)
+
 # Graph Viewer
 class GraphViewerWindow(QGraphicsView):
     clicked = Signal(tuple)
 
-    def __init__(self, graph=None, visual_scheme=None, parent=None):
+    def __init__(self, graph=None, parent=None):
         super().__init__(parent)
         self._graph = graph
 
         # Configure QGraphicsView
         self.setTransformationAnchor(QGraphicsView.NoAnchor)
         self.setResizeAnchor(QGraphicsView.NoAnchor)
         self.setHorizontalScrollBarPolicy( Qt.ScrollBarAlwaysOff )
@@ -154,15 +329,15 @@
         self.setRenderHints(QPainter.Antialiasing)
 
         # Create/Configure the Scene
         self._scene = QGraphicsScene(self)
         self.setScene(self._scene)
 
         self._vgraph = None
-        self.setGraph(self._graph, visual_scheme)
+        self.setGraph(self._graph)
 
         # Set scene bounding rect
         self.setSceneRect()
 
         # State
         self._dragging = False
         self._selected = None
@@ -191,15 +366,15 @@
         super().mousePressEvent(e)
 
     def mouseReleaseEvent(self, e):
         if e.button() == Qt.LeftButton:
             self._dragging = False
             self.setCursor(Qt.ArrowCursor)
             if self._selected:
-                self.clicked.emit(self._selected.get_properties())
+                self.clicked.emit(self._selected.getProperties())
                 #self.scene().setSceneRect(self.scene().itemsBoundingRect())
         super().mouseReleaseEvent(e)
 
     def _checkHovering(self, e):
         item = self.itemAt(e.position().toPoint())
         if not item and not self._hovering:
             pass
@@ -252,68 +427,38 @@
     def centerScene(self):
         p0 = self.mapToScene(*self.centerOfView()) 
         self.setTransform(QTransform().translate(p0.x(), p0.y()), combine=True)
 
     def centerOfView(self):
         return (self.size().width()-1)/2, (self.size().height()-1)/2
 
-    def setGraph(self, graph, visual_scheme=None):
+    def setGraph(self, graph):
         self.scene().clear()
         
-        # Convert graph (if not already a DiGraph) and set visual scheme (if not specified)
+        # Convert graph (if not already a MultiDiGraph)
         if isinstance(graph, nx.MultiDiGraph):
             self._graph = graph
-            if visual_scheme is None:
-                visual_scheme = default_visual_schemes['default']
         elif 'keras' in graph.__module__:
-            self._graph = self.kerasToMultiDiGraph(graph)
-            if visual_scheme is None:
-                visual_scheme = default_visual_schemes['keras']
+            self._graph = kerasToMultiDiGraph(graph)
+        elif 'onnx' in graph.__module__:
+            self._graph = onnxToMultiDiGraph(graph)
 
-        self._vgraph = VisualGraph(self._graph, visual_scheme=visual_scheme)
+        self._vgraph = VisualGraph(self._graph)
         self.scene().addItem(self._vgraph)
         self.setSceneRect()
 
         # reset-state
         self._dragging = False
         self._selected = None
 
-    def kerasToMultiDiGraph(self, model):
-        from tensorflow import keras
-        graph = nx.MultiDiGraph()
-
-        # Add all 'Layers' (aka nodes) to the graph
-        graph.add_nodes_from(model.layers)
-
-        # Get a set of all 'Nodes' (aka edges) in the keras graph
-        keras_nodes = []
-        for layer in model.layers:
-            for node in layer.outbound_nodes:
-                keras_nodes.append(node)
-        keras_nodes = set(keras_nodes)
-
-        # Add the edges to the graph
-        for kn in keras_nodes:
-            input_layers = kn.inbound_layers
-            if not isinstance(input_layers, list): 
-                input_layers = [input_layers]
-            output_layer = kn.outbound_layer
-
-            for index, input_layer in enumerate(input_layers):
-                shape = input_layer.output_shape
-                graph.add_edge(input_layer, output_layer,
-                            in_index=0, out_index=index, shape=shape)
-        return graph
-
 class VisualGraph(QGraphicsItem):
-    def __init__(self, graph=None, visual_scheme=None, parent=None):
+    def __init__(self, graph=None, horizontal=False, parent=None):
         super().__init__(parent=parent)
 
         # Drawing Config
-        self.visual_scheme = visual_scheme
         self.node_size = 75
         self.y_spacing = 1.25*self.node_size
         self.x_spacing = 1.25*self.node_size
 
         self.brush = QBrush(Qt.darkGreen)
         self.pen = QPen(Qt.black, 2)
 
@@ -359,19 +504,24 @@
                             ideal_x[j] += (self.x_spacing - xdelta)
 
             for i,node in enumerate(generation):
                 positions[node][0] = ideal_x[i]
 
         return positions
 
-    def create_visual_nodes(self, positions):
+    def create_visual_nodes(self, positions, horizontal=False):
         for node,pos in positions.items():
-            l,t = pos[0]-self.node_size/2, pos[1]-self.node_size/2
+            if horizontal:
+                l,t = pos[1]-self.node_size/2, pos[0]-self.node_size/2
+            else:
+                l,t = pos[0]-self.node_size/2, pos[1]-self.node_size/2
+
+            visual_scheme = self._graph.nodes[node].get('visual_scheme', {})
             self._node_to_vnode_map[node] = VisualNode(node, QPointF(l,t),
-                    self.visual_scheme, parent=self)
+                    visual_scheme, parent=self)
 
     def create_visual_edges(self):
         self._edge_to_vedge_map.clear()
         for u,v,key,data in self._graph.edges(keys=True, data=True):
             self._edge_to_vedge_map[(u,v,key)] = VisualEdge((u,v,key,data), parent=self)
 
     def paint(self, painter, option, widget=None):
@@ -428,176 +578,283 @@
     def update_adjacent_edges(self, node):
         for u,v,idx in self._graph.in_edges(node, keys=True):
             self._edge_to_vedge_map[(u,v,idx)].updatePath()
 
         for u,v,idx in self._graph.out_edges(node, keys=True):
             self._edge_to_vedge_map[(u,v,idx)].updatePath()
 
-    def setGraph(self, graph):
+    def setGraph(self, graph, horizontal=False):
         self._graph = nx.MultiDiGraph(graph)
         positions = self.calculate_positions()
-        self.create_visual_nodes(positions)
+        self.create_visual_nodes(positions, horizontal)
         self.create_visual_edges()
         self._bounding_rect = self.childrenBoundingRect()
 
 class VisualEdge(QGraphicsItem):
+    class ArrowHead(QGraphicsItem):
+        def __init__(self, parent=None):
+            super().__init__(parent=parent)
+            line = QLineF(QPointF(-3,0), QPointF(3,0))
+            line.setAngle(30)
+            self.arrow_up = QGraphicsLineItem (line, parent=self)
+            self.arrow_up.setPen(QPen(Qt.white))
+
+            line = QLineF(QPointF(-3,0), QPointF(3,0))
+            line.setAngle(-30)
+            self.arrow_down = QGraphicsLineItem (line, parent=self)
+            self.arrow_down.setPen(QPen(Qt.white))
+
+            self.arrow_up.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+            self.arrow_down.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+
+        def setHovering(self, state):
+            if state:
+                self.parentItem().path.setPen(QPen(Qt.red))
+                self.parentItem().text.setVisible(True)
+                self.setPen(QPen(Qt.red))
+            else:
+                self.parentItem().path.setPen(QPen(Qt.white))
+                self.parentItem().text.setVisible(False)
+                self.setPen(QPen(Qt.white))
+            self.parentItem().update()
+
+        def setPen(self, pen):
+            self.arrow_up.setPen(pen)
+            self.arrow_down.setPen(pen)
+
+        def paint(self, painter, option, widget=None):
+            pass
+
+        def boundingRect(self):
+            return self.childrenBoundingRect()
+
+    class Arc(QGraphicsItem):
+        def __init__(self, parent=None):
+            super().__init__(parent=parent)
+            self.rect = QRectF()
+            self.pen = QPen()
+            self.orientation = True
+
+        def setOrientation(self, ori):
+            self.orientation = ori
+
+        def setRect(self, rect):
+            self.rect = rect
+
+        def setPen(self, pen):
+            self.pen = pen 
+
+        def paint(self, painter, option, widget=None):
+            painter.setPen(self.pen)
+            if self.orientation:
+                start, span = 0, 180*16
+            else:
+                start, span = 0, -180*16
+            painter.drawArc(self.rect, start, span)
+
+        def boundingRect(self):
+            return self.rect
+
+
     def __init__(self, edge, parent=None):
         super().__init__(parent=parent)
 
         # Unpack the edge
+        self.graph = self.parentItem()._graph
         self.edge = edge
         self.in_node, self.out_node, self.key, self.data = edge
         self.in_vnode = self.parentItem()._node_to_vnode_map[self.in_node]
         self.out_vnode = self.parentItem()._node_to_vnode_map[self.out_node]
 
         # Create the graphics items
-        self.path = QGraphicsLineItem(parent=self)
-        self.arrow_left = QGraphicsLineItem(parent=self)
-        self.arrow_right = QGraphicsLineItem(parent=self)
+        self.path = VisualEdge.Arc(parent=self)
+        self.arrow = VisualEdge.ArrowHead(parent=self)
         self.text = QGraphicsTextItem(str(self.data), parent=self)#str(self.data))
+        self.setEdgeText()
 
         self.path.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
-        self.arrow_left.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
-        self.arrow_right.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        #self.arrow.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
         self.text.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
         self.text.setVisible(False)
 
         # Colorize
         self.path.setPen(QPen(Qt.white))
-        self.arrow_left.setPen(QPen(Qt.white))
-        self.arrow_right.setPen(QPen(Qt.white))
+        self.arrow.setPen(QPen(Qt.white))
         self.text.setDefaultTextColor(Qt.lightGray)
 
         # Calculate graphic items positions
         self.setZValue(-1)
         self.calculatePath()
-        self.calculateArrowHead()
         self.calculateText()
 
+    def setEdgeText(self):
+        properties = self.data.get('properties', {})
+        if properties:
+            txt = "\n".join([f"{k}: {v}" for k,v in properties.items()])
+        else:
+            txt = ""
+        self.text.setPlainText(txt)
+
+    def lineIntersects(self, line):
+        def orientation(p1,p2,p3): 
+            val = (float(p2.y() - p1.y()) * (p3.x() - p2.x())) - (float(p2.x() - p1.x()) * (p3.y() - p2.y()))
+            return val > 0
+
+        path = QPainterPath(line.p1())
+        path.lineTo(line.p2())
+        for vnode in self.parentItem()._node_to_vnode_map.values():
+            if vnode is self.in_vnode or vnode is self.out_vnode:
+                continue
+            shape = vnode.mapToScene(vnode.shape())
+            if shape.intersects(path):
+                return True, orientation(self.in_vnode.center(), self.out_vnode.center(), vnode.center())
+        return False, False
+
     def calculatePath(self):
+
+        # If a straight path intersects other nodes, make the line arc instead
+        line = QLineF(self.out_vnode.center(), self.in_vnode.center())
+        intersected, orientation = self.lineIntersects(line)
+        if intersected: 
+            h = 80 if orientation else -80
+        else:
+            h = 0
+
+        rect = QRectF(QPointF(0,h/2), QPointF(line.length(), -h/2))
+        self.path.setOrientation(orientation)
+        self.path.setRect(rect)
+        self.path.setRotation(-line.angle())
+
+        pos = line.p1()
+
+        # For multi-edge nodes draw an offset on the edge so its more visible
         delta = 0
         if isinstance(self.key, int):
             if self.key != 0:
                 delta = 8 if self.key % 2 else -8
-
-        line = QLineF(self.out_vnode.center(), self.in_vnode.center())
         if delta:
             offset = (line.normalVector().unitVector().p2() - line.p1()) * delta
-            line.translate(offset)
-        self.path.setLine(line)
-
-    def calculateArrowHead(self):
-        c = self.path.line().center()
-        u = self.path.line().unitVector().p1() - self.path.line().unitVector().p2()
-        angle = self.path.line().angle()
-
-        # Arrow head
-        arrow_right = QLineF(c+3*u, c-3*u)
-        arrow_right.setAngle(angle+30)
+            pos = offset + line.p1()
+        else:
+            offset = QPointF(0,0)
+        self.path.setPos(pos)
 
-        arrow_left = QLineF(c+3*u, c-3*u)
-        arrow_left.setAngle(angle-30)
+        curve_offset = (line.normalVector().unitVector().p2() - line.p1()) * h/2
+        self.arrow.setRotation(-line.angle())
+        self.arrow.setPos(line.center() + curve_offset + offset)
 
-        self.arrow_left.setLine(arrow_left)
-        self.arrow_right.setLine(arrow_right)
+    def getLine(self):
+        return QLineF(self.out_vnode.center(), self.in_vnode.center())
 
     def calculateText(self):
-        self.text.setPos(self.path.line().center())
+        self.text.setPos(self.getLine().center())
 
     def updatePath(self):
+        self.prepareGeometryChange()
         self.calculatePath()
-        self.calculateArrowHead()
         self.calculateText()
-
-    def setHovering(self, state):
-        if state:
-            self.path.setPen(QPen(Qt.red))
-            self.arrow_left.setPen(QPen(Qt.red))
-            self.arrow_right.setPen(QPen(Qt.red))
-            self.text.setVisible(True)
-        else:
-            self.path.setPen(QPen(Qt.white))
-            self.arrow_left.setPen(QPen(Qt.white))
-            self.arrow_right.setPen(QPen(Qt.white))
-            self.text.setVisible(False)
         self.update()
 
+    #def setHovering(self, state):
+    #    if state:
+    #        self.path.setPen(QPen(Qt.red))
+    #        self.arrow.setPen(QPen(Qt.red))
+    #        self.text.setVisible(True)
+    #    else:
+    #        self.path.setPen(QPen(Qt.white))
+    #        self.arrow.setPen(QPen(Qt.white))
+    #        self.text.setVisible(False)
+    #    self.update()
+
     def paint(self, painter, option, widget=None):
         pass
+        #painter.drawRect(self.boundingRect())
 
     def boundingRect(self):
-        return QRectF(self.arrow_left.boundingRect()).united(self.arrow_right.boundingRect())
+        return self.childrenBoundingRect()
 
 class VisualNode(QGraphicsItem):
+    class Background(QGraphicsItem):
+        def __init__(self, brush, pen, parent=None):
+            super().__init__(parent=parent)
+            self._boundary = None
+            self.brush = brush
+            self.pen = pen
+
+        def setBoundingRect(self, boundary):
+            self._boundary = boundary
+
+        def boundingRect(self):
+            return self._boundary
+
+        def paint(self, painter, option, widget=None):
+            painter.setBrush(self.brush)
+            painter.drawRoundedRect(self.boundingRect(), 5, 5)
+
     def __init__(self, node, pos, visual_scheme, parent=None):
         super().__init__(parent)
         # Keep reference to node
-        self.visual_scheme = visual_scheme
+        self.graph = self.parentItem()._graph
         self.node = node
 
         # set node config
-        self.node_label, self.pen, self.brush, self.size = None, None, None, None
-        self.setNodeConfig()
+        self.node_label, self.pen = None, None
+        self.brush, self.size = None, None
+        self.setVisualScheme()
 
-        # set node shell
         self.shell = QGraphicsEllipseItem(0, 0, self.size[0], self.size[1], parent=self)
-        self.shell.setBrush(self.brush)
         self.shell.setPen(self.pen)
-        self.shell.setEnabled(False)
+        self.shell.setBrush(self.brush)
         self.shell.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        self.shell.setEnabled(False)
+
+        #self.background = VisualNode.Background(self.brush, self.pen, parent=self)
+        #self.background.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        #self.background.setEnabled(False)
 
         # set text
         self.text = QGraphicsTextItem(self.label_text, parent=self)
         self.text.setPos(self.shell.boundingRect().center() - self.text.boundingRect().center())
+        self.text.setDefaultTextColor(Qt.white)
         self.text.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
         self.text.setEnabled(False)
-        self.text.setDefaultTextColor(Qt.white)
 
+        # set node shell
+        #self.background.setBoundingRect(self.boundingRect())
         super().setPos(pos - self.boundingRect().center())
 
-    def setNodeConfig(self):
-        ntype = type(self.node).__name__
-        default_config = self.visual_scheme['nodes'].get('default', {})
-        config = self.visual_scheme['nodes'].get(ntype, default_config)
+    def setVisualScheme(self):
+        config = self.graph.nodes[self.node].get('visual_scheme', {})
 
         # Pen
-        self.pen = QPen(Qt.black, int(config.get("boundarySize", 0)))
+        self.pen = QPen(Qt.black, int(config.get("boundarySize", 2)))
         
         # Brush
         color = config.get("fillColor", 'darkGray')
         self.brush = QBrush(getattr(Qt, color))
 
         # Size
-        size = config.get('size', [20,20])
+        size = config.get('size', [50,50])
         if not isinstance(size, list):
             size = [size, size]
         self.size = [int(s) for s in size]
 
         # Node Label
-        label_attr = config.get('label_attr', None) 
-        if label_attr:
-            attr = getattr(self.node, label_attr)
-            if callable(attr):
-                txt = attr()
-            else:
-                txt = attr
-        else:
-            txt = type(self.node).__name__
-        self.label_text = txt
+        self.label_text = config.get('label', type(self.node).__name__) 
 
-    def get_properties(self):
-        if hasattr(self.node, 'get_config'):
-            return self.node.get_config()
-        elif hasattr(self.node, '__dict__'):
-            return self.node.__dict__
-        else:
-            return {'type': type(self.node).__name__, 'name': self.node}
+    def getProperties(self):
+        defaults = {'type': type(self.node).__name__, 'name': self.node}
+        return self.graph.nodes[self.node].get('properties', defaults) 
 
     def paint(self, painter, option, widget=None):
         pass
+        #painter.setBrush(self.brush)
+        #painter.drawRoundedRect(self.boundingRect(), 5, 5)
+        #super().paint(painter, option, widget=None)
+        #pass
 
     def boundingRect(self):
         return self.childrenBoundingRect() 
 
     def center(self):
         return self.pos() + self.childrenBoundingRect().center()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtgraphvisuals-0.0.4/LICENSE` & `qtgraphvisuals-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgraphvisuals-0.0.4/pyproject.toml` & `qtgraphvisuals-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 exclude = [
     "env/"
 ]
 
 [project]
 name = "QtGraphVisuals"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jacob Botimer", email="botimerj@gmail.com" },
 ]
 description = "A qt-widget to visualize directed graphs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qtgraphvisuals-0.0.4/PKG-INFO` & `qtgraphvisuals-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtGraphVisuals
-Version: 0.0.4
+Version: 0.0.5
 Summary: A qt-widget to visualize directed graphs
 Project-URL: Homepage, https://github.com/jake987654321/QtGraphVisuals
 Project-URL: Bug Tracker, https://github.com/jake987654321/QtGraphVisuals/issues
 Author-email: Jacob Botimer <botimerj@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

