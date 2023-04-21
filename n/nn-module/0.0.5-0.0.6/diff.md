# Comparing `tmp/nn-module-0.0.5.tar.gz` & `tmp/nn-module-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn-module-0.0.5.tar", last modified: Fri Oct 14 07:35:52 2022, max compression
+gzip compressed data, was "nn-module-0.0.6.tar", last modified: Fri Apr 21 09:31:36 2023, max compression
```

## Comparing `nn-module-0.0.5.tar` & `nn-module-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2022-10-14 07:35:52.877057 nn-module-0.0.5/
--rw-r--r--   0 khanh      (501) staff       (20)     1069 2022-04-19 17:28:25.000000 nn-module-0.0.5/LICENSE
--rw-r--r--   0 khanh      (501) staff       (20)      465 2022-10-14 07:35:52.876935 nn-module-0.0.5/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)      219 2022-10-14 07:35:41.000000 nn-module-0.0.5/README.md
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2022-10-14 07:35:52.876217 nn-module-0.0.5/nn_module/
--rw-r--r--   0 khanh      (501) staff       (20)      440 2022-10-14 07:29:52.000000 nn-module-0.0.5/nn_module/__init__.py
--rw-r--r--   0 khanh      (501) staff       (20)     5199 2022-10-14 07:29:35.000000 nn-module-0.0.5/nn_module/attention.py
--rw-r--r--   0 khanh      (501) staff       (20)      903 2022-10-14 07:29:35.000000 nn-module-0.0.5/nn_module/feedforward.py
--rw-r--r--   0 khanh      (501) staff       (20)      532 2022-10-14 07:29:52.000000 nn-module-0.0.5/nn_module/functional.py
--rw-r--r--   0 khanh      (501) staff       (20)     3051 2022-10-14 07:30:40.000000 nn-module-0.0.5/nn_module/grand.py
--rw-r--r--   0 khanh      (501) staff       (20)      823 2022-10-14 07:29:35.000000 nn-module-0.0.5/nn_module/index.py
--rw-r--r--   0 khanh      (501) staff       (20)     1431 2022-10-14 07:29:35.000000 nn-module-0.0.5/nn_module/neuralode.py
--rw-r--r--   0 khanh      (501) staff       (20)      466 2022-10-14 07:29:35.000000 nn-module-0.0.5/nn_module/resnet.py
--rw-r--r--   0 khanh      (501) staff       (20)      369 2022-10-14 07:29:52.000000 nn-module-0.0.5/nn_module/rf.py
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2022-10-14 07:35:52.876778 nn-module-0.0.5/nn_module.egg-info/
--rw-r--r--   0 khanh      (501) staff       (20)      465 2022-10-14 07:35:52.000000 nn-module-0.0.5/nn_module.egg-info/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)      349 2022-10-14 07:35:52.000000 nn-module-0.0.5/nn_module.egg-info/SOURCES.txt
--rw-r--r--   0 khanh      (501) staff       (20)        1 2022-10-14 07:35:52.000000 nn-module-0.0.5/nn_module.egg-info/dependency_links.txt
--rw-r--r--   0 khanh      (501) staff       (20)       10 2022-10-14 07:35:52.000000 nn-module-0.0.5/nn_module.egg-info/top_level.txt
--rw-r--r--   0 khanh      (501) staff       (20)       38 2022-10-14 07:35:52.877098 nn-module-0.0.5/setup.cfg
--rw-r--r--   0 khanh      (501) staff       (20)      491 2022-10-14 07:35:31.000000 nn-module-0.0.5/setup.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:31:36.434209 nn-module-0.0.6/
+-rw-r--r--   0 khanh      (501) staff       (20)     1069 2022-11-17 03:27:36.000000 nn-module-0.0.6/LICENSE
+-rw-r--r--   0 khanh      (501) staff       (20)      456 2023-04-21 09:31:36.434039 nn-module-0.0.6/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)      219 2022-11-17 03:27:36.000000 nn-module-0.0.6/README.md
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:31:36.432840 nn-module-0.0.6/nn_module/
+-rw-r--r--   0 khanh      (501) staff       (20)      440 2022-11-17 03:27:36.000000 nn-module-0.0.6/nn_module/__init__.py
+-rw-r--r--   0 khanh      (501) staff       (20)     5197 2023-04-21 09:30:01.000000 nn-module-0.0.6/nn_module/attention.py
+-rw-r--r--   0 khanh      (501) staff       (20)      903 2022-11-17 03:27:36.000000 nn-module-0.0.6/nn_module/feedforward.py
+-rw-r--r--   0 khanh      (501) staff       (20)      532 2022-11-17 03:27:36.000000 nn-module-0.0.6/nn_module/functional.py
+-rw-r--r--   0 khanh      (501) staff       (20)     3234 2022-11-21 08:03:59.000000 nn-module-0.0.6/nn_module/grand.py
+-rw-r--r--   0 khanh      (501) staff       (20)     1431 2022-11-17 03:27:36.000000 nn-module-0.0.6/nn_module/neuralode.py
+-rw-r--r--   0 khanh      (501) staff       (20)      466 2022-11-17 03:27:36.000000 nn-module-0.0.6/nn_module/resnet.py
+-rw-r--r--   0 khanh      (501) staff       (20)      448 2022-11-21 03:12:12.000000 nn-module-0.0.6/nn_module/rf.py
+-rw-r--r--   0 khanh      (501) staff       (20)      978 2022-11-21 04:53:47.000000 nn-module-0.0.6/nn_module/table.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:31:36.433759 nn-module-0.0.6/nn_module.egg-info/
+-rw-r--r--   0 khanh      (501) staff       (20)      456 2023-04-21 09:31:36.000000 nn-module-0.0.6/nn_module.egg-info/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)      349 2023-04-21 09:31:36.000000 nn-module-0.0.6/nn_module.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh      (501) staff       (20)        1 2023-04-21 09:31:36.000000 nn-module-0.0.6/nn_module.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       10 2023-04-21 09:31:36.000000 nn-module-0.0.6/nn_module.egg-info/top_level.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       38 2023-04-21 09:31:36.434284 nn-module-0.0.6/setup.cfg
+-rw-r--r--   0 khanh      (501) staff       (20)      482 2023-04-21 09:31:13.000000 nn-module-0.0.6/setup.py
```

### Comparing `nn-module-0.0.5/LICENSE` & `nn-module-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nn-module-0.0.5/nn_module/attention.py` & `nn-module-0.0.6/nn_module/attention.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+from __future__ import annotations
+
 import math
 import random
 
 import torch
 from torch_scatter import scatter_sum
 
 from nn_module import Module
 
+def fully_connected_graph(n: int) -> torch.Tensor:
+    e = torch.tensor([
+        n * list(range(n)),
+        sum([[i] * n for i in range(n)], [])
+    ], dtype=torch.int64)
+    return e
+
 
 def sparse_multihead_softmax(values: torch.Tensor, index: torch.Tensor, eps: float = 1e-16) -> torch.Tensor:
     """
     :param values: (b, m, h)
     :param index: (m,)
     :param eps:
     :return: (b, m, h)
@@ -22,88 +31,93 @@
     values = values - values.max()  # shift does not change softmax, use this to avoid overflow and reduce numerical err
     exp_logits = torch.exp(values)
     exp_logits_sum = scatter_sum(src=exp_logits, index=index, dim=1)[:, index, :]
     return exp_logits / (exp_logits_sum + eps)
 
 
 def sparse_multihead_attention(
-        q: torch.Tensor, k: torch.Tensor, edge_index: torch.Tensor, head_index: torch.Tensor,
+        q: torch.Tensor, k: torch.Tensor, e: torch.Tensor, h: torch.Tensor,
 ):
     """
     :param q: (b, n, d) - (batch, node, dim)
     :param k: (b, n, d) - (batch, node, dim)
-    :param edge_index: (2, m) - (2, edge)
-    :param head_index: (d,) - (dim,)
+    :param e: (2, m) - (2, edge)
+    :param h: (d,) - (dim,)
     :return: (b, m, h) - (batch, edge, head)
     """
     assert len(q.shape) == 3
     assert len(k.shape) == 3
     assert q.shape == k.shape
 
-    assert len(edge_index.shape) == 2
-    assert edge_index.shape[0] == 2
-    assert edge_index.dtype == torch.int64
+    assert len(e.shape) == 2
+    assert e.shape[0] == 2
+    assert e.dtype == torch.int64
 
-    assert len(head_index.shape) == 1
-    assert head_index.shape[0] == q.shape[2]
+    assert len(h.shape) == 1
+    assert h.shape[0] == q.shape[2]
 
-    src_q = q[:, edge_index[0, :], :]  # (b, m, d)
-    dst_k = k[:, edge_index[1, :], :]  # (b, m, d)
+    src_q = q[:, e[0, :], :]  # (b, m, d)
+    dst_k = k[:, e[1, :], :]  # (b, m, d)
     a_e = src_q * dst_k  # (b, m, d)
-    a_e_sum = scatter_sum(src=a_e, index=head_index, dim=2)  # (b, m, h)
+    a_e_sum = scatter_sum(src=a_e, index=h, dim=2)  # (b, m, h)
     return a_e_sum
 
 
 class SparseMultiheadAttention(Module):
     def __init__(self,
                  key_dim: int,
                  hidden_dim: int,
-                 edge_index: torch.Tensor,
                  num_heads: int = 1,
                  ):
-        """
-        :param edge_index: (2, m)
-        """
         assert hidden_dim % num_heads == 0
-        assert len(edge_index.shape) == 2
-        assert edge_index.shape[0] == 2
-        assert edge_index.dtype == torch.int64
 
         super().__init__()
 
         self.num_heads = num_heads
         self.key_dim = key_dim
         self.hidden_dim = hidden_dim
 
-        self.register_buffer("edge_index", edge_index)
-        self.register_buffer("head_index", torch.tensor(
+        self.register_buffer("h", torch.tensor(
             [i // (hidden_dim // num_heads) for i in range(hidden_dim)]
             , dtype=torch.int64,
         ))
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(key_dim={self.key_dim}, hidden_dim={self.hidden_dim}, num_heads={self.num_heads})"
 
-    def forward(self, q: torch.Tensor, k: torch.Tensor, reduce_dim: int = 1) -> torch.Tensor:
+    def forward(self, q: torch.Tensor, k: torch.Tensor, e: torch.Tensor | None = None, r: torch.Tensor | None = None) -> torch.Tensor:
         """
         :param q: (b, n, d)
         :param k: (b, n, d)
-        :param reduce_dim: reduce_dim=1, sum of each row is 1
+        :param e: (2, m)
+        :param r: (m, )
         :return: (b, m, h)
         """
         assert len(q.shape) == 3
         assert len(k.shape) == 3
         assert q.shape == k.shape
+        if e is None: # fully connected graph - normal multiheaded attention
+            n = q.shape[1]
+            e = fully_connected_graph(n).to(self.device) 
+
+        assert len(e.shape) == 2
+        assert e.shape[0] == 2
+        assert e.dtype == torch.int64
+        if r is None:
+            r = e[0, :]
+        assert len(r.shape) == 1
+        assert r.shape[0] == e.shape[1]
+
         a_values = sparse_multihead_attention(
             q=q,
             k=k,
-            edge_index=self.edge_index,
-            head_index=self.head_index,
+            e=e,
+            h=self.h,
         ) / math.sqrt(self.key_dim)  # (b, m, h)
-        a_values = sparse_multihead_softmax(values=a_values, index=self.edge_index[1 - reduce_dim, :])
+        a_values = sparse_multihead_softmax(values=a_values, index=r)
         return a_values
 
 
 if __name__ == "__main__":
     def _attention(q: torch.Tensor, k: torch.Tensor):
         """
         :param q: (b, n, d)
@@ -114,45 +128,45 @@
         assert len(k.shape) == 3
         assert q.shape == k.shape
         a_sum = torch.bmm(q, k.transpose(1, 2))
         return a_sum
 
 
     def _sparse_multihead_attention_elementwise(
-            q: torch.Tensor, k: torch.Tensor, edge_index: torch.Tensor, head_index: torch.Tensor,
+            q: torch.Tensor, k: torch.Tensor, e: torch.Tensor, h: torch.Tensor,
     ):
         """
         :param q: (b, n, d) - (batch, node, dim)
         :param k: (b, n, d) - (batch, node, dim)
-        :param edge_index: (2, m) - (2, edge)
-        :param head_index: (d,) - (dim,)
+        :param e: (2, m) - (2, edge)
+        :param h: (d,) - (dim,)
         :return: (b, m, h) - (batch, edge, head)
         """
         a_sum_list = []
-        for i in head_index.unique():
-            q_i = q[:, :, head_index == i]
-            k_i = k[:, :, head_index == i]
+        for i in h.unique():
+            q_i = q[:, :, h == i]
+            k_i = k[:, :, h == i]
             a_sum_i = _attention(q_i, k_i)
             a_sum_list.append(a_sum_i)
         a_sum = torch.stack(a_sum_list, dim=3)  # (b, n, n, h)
         a_e_sum_list = []
-        for e in range(edge_index.shape[1]):
-            i, j = edge_index[:, e]
+        for k in range(e.shape[1]):
+            i, j = e[:, k]
             a_e_sum_list.append(a_sum[:, i, j, :])
         a_e_sum = torch.stack(a_e_sum_list, dim=1)  # (b, m, h)
         return a_e_sum
 
 
     # test sparse_multi_headed_attention
     b, n, d = 3, 5, 4
     q = torch.rand(b, n, d)
     k = torch.rand(b, n, d)
-    edge_index = []
+    e = []
     for i in range(n):
         for j in range(n):
             if random.random() < 0.5:
-                edge_index.append((i, j))
-    edge_index = torch.tensor(edge_index).T
-    head_index = torch.tensor([0, 0, 1, 1])
-    expected = _sparse_multihead_attention_elementwise(q, k, edge_index, head_index)
-    actual = sparse_multihead_attention(q, k, edge_index, head_index)
+                e.append((i, j))
+    e = torch.tensor(e).T
+    h = torch.tensor([0, 0, 1, 1])
+    expected = _sparse_multihead_attention_elementwise(q, k, e, h)
+    actual = sparse_multihead_attention(q, k, e, h)
     assert torch.isclose(expected, actual).all()
```

### Comparing `nn-module-0.0.5/nn_module/feedforward.py` & `nn-module-0.0.6/nn_module/feedforward.py`

 * *Files identical despite different names*

### Comparing `nn-module-0.0.5/nn_module/functional.py` & `nn-module-0.0.6/nn_module/functional.py`

 * *Files identical despite different names*

### Comparing `nn-module-0.0.5/nn_module/grand.py` & `nn-module-0.0.6/nn_module/grand.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple
 
 import torch
 import torch_scatter
 import torch_sparse
 from torch import Tensor, nn
 
-from nn_module.attention import SparseMultiheadAttention
+from nn_module.attention import SparseMultiheadAttention, fully_connected_graph
 from nn_module.neuralode import ODEFunc
 
 
 def sparse_batch_matmul(values: torch.Tensor, edge: torch.Tensor, dim: Tuple[int, int],
                         dense: torch.Tensor) -> torch.Tensor:
     """
     :param values: (*, m)
@@ -30,33 +30,35 @@
 
 
 class LinearGRAND(ODEFunc):
     def __init__(self,
                  num_nodes: int,
                  diffusion_dim: int,
                  attention_dim: int,
-                 edge_index: torch.Tensor,
+                 edge_index: torch.Tensor | None = None,
                  num_heads: int = 1,
                  softmax_dim: int = 1,
                  bias: bool = False,
                  ):
         """
         :param edge_index: (2, m)
         """
         super().__init__()
 
+        if edge_index is None: # fully connected graph - normal multiheaded attention
+            edge_index = fully_connected_graph(num_nodes)
+
         self.num_nodes = num_nodes
         self.register_buffer("edge_index", edge_index)
         self.register_parameter("w_q", nn.Parameter(torch.empty(diffusion_dim, attention_dim, dtype=torch.float32)))
         self.register_parameter("w_k", nn.Parameter(torch.empty(diffusion_dim, attention_dim, dtype=torch.float32)))
 
         self.add_module("attention", SparseMultiheadAttention(
             key_dim=diffusion_dim,
             hidden_dim=attention_dim,
-            edge_index=edge_index,
             num_heads=num_heads,
         ))
 
         self.attention_values = None
         self.reduce_operator = None
         self.radius2 = None
 
@@ -71,21 +73,22 @@
     def on_before_integration(self, x0: torch.Tensor, t_list: torch.Tensor):
         """
         call before every integration
         """
         self.attention_values = self.attention.forward(
             q=x0 @ self.w_q,
             k=x0 @ self.w_k,
-            reduce_dim=self.softmax_dim,
+            e=self.edge_index,
+            r=self.edge_index[1 - self.softmax_dim, :],
         ).mean(dim=-1)  # average over all heads
 
         b, n, _ = x0.shape
         self.reduce_operator = torch_scatter.scatter_sum(
             src=self.attention_values,
-            index=self.attention.edge_index[1 - self.softmax_dim, :],
+            index=self.edge_index[1 - self.softmax_dim, :],
         ).view(b, n, 1)
 
     def forward(self, t: float, x: Tensor):
         """
         :param t:
         :param x: (b, n, d)
         """
```

### Comparing `nn-module-0.0.5/nn_module/neuralode.py` & `nn-module-0.0.6/nn_module/neuralode.py`

 * *Files identical despite different names*

