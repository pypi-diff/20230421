# Comparing `tmp/CoLT5-attention-0.2.3.tar.gz` & `tmp/CoLT5-attention-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.2.3.tar", last modified: Wed Apr 19 22:48:13 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.2.4.tar", last modified: Fri Apr 21 14:30:56 2023, max compression
```

## Comparing `CoLT5-attention-0.2.3.tar` & `CoLT5-attention-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:30:56.544388 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 14:30:56.000000 CoLT5-attention-0.2.4/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:30:56.548388 CoLT5-attention-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-21 14:30:43.000000 CoLT5-attention-0.2.4/setup.py
```

### Comparing `CoLT5-attention-0.2.3/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.2.4/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.3
+Version: 0.2.4
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.3/LICENSE` & `CoLT5-attention-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.3/PKG-INFO` & `CoLT5-attention-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.3
+Version: 0.2.4
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.3/README.md` & `CoLT5-attention-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.3/colt5_attention/coor_descent.py` & `CoLT5-attention-0.2.4/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.3/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.2.4/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.3/colt5_attention/transformer_block.py` & `CoLT5-attention-0.2.4/colt5_attention/transformer_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,32 +55,36 @@
     )
 
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
-        heads = 8
+        heads = 8,
+        multiply_keys_by_score = False
     ):
         super().__init__()
         self.heads = heads
         self.scale = dim_head ** -0.5
         dim_hidden = dim_head * heads
 
+        self.multiply_keys_by_score = multiply_keys_by_score
+
         self.norm = RMSNorm(dim)
         self.to_q = nn.Linear(dim, dim_hidden, bias = False)
         self.to_kv = nn.Linear(dim, dim_hidden * 2, bias = False)
         self.to_out = nn.Linear(dim_hidden, dim, bias = False)
 
     def forward(
         self,
         x,
         context = None,
         mask = None,
-        normalized_scores_kv = None
+        normalized_scores_kv = None,
+        normalized_scores_q = None
     ):
         """
         einops:
         b - batch
         h - heads, or number of heads per route
         r - routing dimension, for routing different sets of key / values - should be more expressive
         n - sequence dimension
@@ -111,28 +115,34 @@
         num_kv_routes = context.shape[1]
 
         # get queries
 
         q = self.to_q(x)
         q = rearrange(q, 'b n (h d) -> b h n d', h = h)
 
+        if exists(normalized_scores_q):
+            q = q * rearrange(normalized_scores_q, 'b n -> b 1 n 1')
+
         # handle key / values, with the routing dimension, dividing the number of heads in between the routes
 
         assert divisible_by(h, num_kv_routes), 'number of heads must be divisible by the number of key / value routes'
         heads_per_route = h // num_kv_routes
 
         kv_weight = rearrange(self.to_kv.weight, '(r h d) i -> r h d i', h = heads_per_route, r = num_kv_routes)
 
         kv = einsum('r h d i, b r n i -> b r h n d', kv_weight, context)
         k, v = kv.chunk(2, dim = -1)
 
         if exists(normalized_scores_kv):
             # in paper, not sure how they passed back the signal from heavy attention to normalized scores for key/values. just multiply the values by the normalized kv scores for now
             v = v * normalized_scores_kv
 
+            if self.multiply_keys_by_score:
+                k = k * normalized_scores_kv
+
         k, v = map(lambda t: rearrange(t, 'b r h n d -> b (r h) n d'), (k, v))
 
         # scale and get similarity
 
         q = q * self.scale
         sim = einsum('b h i d, b h j d -> b h i j', q, k)
 
@@ -490,26 +500,30 @@
         light_dim_head = 64,
         light_heads = 8,
         light_window_size = 128,        # each token would see ~ 64 tokens either way to left or right
         heavy_dim_head = 64,
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
-        router_kwargs: dict = {}
+        router_kwargs: dict = {},
+        multiply_keys_by_score = False,
+        multiply_queries_by_score = False
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
 
         self.num_heavy_tokens_q = num_heavy_tokens_q
         self.num_heavy_tokens_kv = num_heavy_tokens_kv
 
+        self.multiply_queries_by_score = multiply_queries_by_score
+
         self.light_attn = LocalMHA(
             dim = dim,
             dim_head = light_dim_head,
             heads = light_heads,
             window_size = light_window_size // 2,
             prenorm = True,
             causal = False,
@@ -530,15 +544,16 @@
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = heavy_dim_head,
-            heads = heavy_heads
+            heads = heavy_heads,
+            multiply_keys_by_score = multiply_keys_by_score
         )
 
     def forward(
         self,
         x,
         *,
         num_heavy_tokens_q = None,
@@ -575,15 +590,16 @@
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
-            normalized_scores_kv = normalized_scores_kv
+            normalized_scores_kv = normalized_scores_kv,
+            normalized_scores_q = normalized_scores_q if self.multiply_queries_by_score else None
         )
 
         routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
 
         # scatter back the output of the heavy branch
 
         heavy_out = torch.zeros_like(x)
@@ -608,15 +624,16 @@
         num_tokens_kv,
         num_sets_kv = 1,                # setting this greater than 1 would route multiple sets of key / values, each of size num_tokens_kv, using this many routing tokens
         dim_head = 64,
         heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
-        kv_routing_tokens = 1
+        kv_routing_tokens = 1,
+        multiply_keys_by_score = False
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -636,15 +653,16 @@
             num_routing_tokens = kv_routing_tokens,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = dim_head,
-            heads = heads
+            heads = heads,
+            multiply_keys_by_score = multiply_keys_by_score
         )
 
     def forward(
         self,
         x,
         context,
         *,
@@ -735,15 +753,17 @@
         light_window_size = 128,
         heavy_dim_head = 64,
         heavy_heads = 8,
         light_ff_mult = 0.5,
         heavy_ff_mult = 4,
         router_straight_through = True,
         router_type = 'coor_descent',
-        router_kwargs: dict = {}
+        router_kwargs: dict = {},
+        multiply_keys_by_score = False,
+        multiply_queries_by_score = False
     ):
         super().__init__()
         self.conditional_ff = ConditionalRoutedFeedForward(
             dim,
             num_heavy_tokens = num_heavy_ff_tokens,
             light_ff_mult = light_ff_mult,
             heavy_ff_mult = heavy_ff_mult,
@@ -760,15 +780,17 @@
             heavy_dim_head = heavy_dim_head,
             heavy_heads = heavy_heads,
             num_heavy_tokens_q = num_heavy_attn_tokens_q,
             num_heavy_tokens_kv = num_heavy_attn_tokens_kv,
             num_routed_kv = num_routed_kv,
             router_straight_through = router_straight_through,
             router_type = router_type,
-            router_kwargs = router_kwargs
+            router_kwargs = router_kwargs,
+            multiply_keys_by_score = multiply_keys_by_score,
+            multiply_queries_by_score = multiply_queries_by_score
         )
 
     def forward(
         self,
         x,
         mask = None,
         num_heavy_attn_tokens_q = None,
```

### Comparing `CoLT5-attention-0.2.3/setup.py` & `CoLT5-attention-0.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.2.3',
+  version = '0.2.4',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

