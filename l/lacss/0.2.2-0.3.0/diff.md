# Comparing `tmp/lacss-0.2.2.tar.gz` & `tmp/lacss-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.2.2.tar", max compression
+gzip compressed data, was "lacss-0.3.0.tar", max compression
```

## Comparing `lacss-0.2.2.tar` & `lacss-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1062 2023-03-07 20:26:01.088077 lacss-0.2.2/LICENSE
--rw-r--r--   0        0        0      978 2023-03-07 23:33:18.261072 lacss-0.2.2/README.md
--rw-r--r--   0        0        0       65 2023-03-15 14:04:31.091599 lacss-0.2.2/lacss/__init__.py
--rw-r--r--   0        0        0       47 2023-03-08 13:25:26.759293 lacss-0.2.2/lacss/data/__init__.py
--rw-r--r--   0        0        0     6063 2023-03-08 13:25:26.771841 lacss-0.2.2/lacss/data/generator.py
--rw-r--r--   0        0        0     9160 2023-03-31 20:18:30.795450 lacss-0.2.2/lacss/data/parser.py
--rw-r--r--   0        0        0     3289 2023-04-07 12:37:03.716465 lacss-0.2.2/lacss/deploy.py
--rw-r--r--   0        0        0       74 2023-03-08 13:25:26.788189 lacss-0.2.2/lacss/losses/__init__.py
--rw-r--r--   0        0        0     5275 2023-04-08 12:43:30.562328 lacss-0.2.2/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0     3189 2023-04-04 13:41:26.676796 lacss-0.2.2/lacss/losses/detection.py
--rw-r--r--   0        0        0     7309 2023-04-08 12:43:30.571689 lacss-0.2.2/lacss/losses/instance.py
--rw-r--r--   0        0        0       56 2023-03-17 14:54:37.040008 lacss-0.2.2/lacss/metrics/__init__.py
--rw-r--r--   0        0        0     5547 2023-04-04 20:03:39.259309 lacss-0.2.2/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      216 2023-04-06 13:32:26.472769 lacss-0.2.2/lacss/modules/__init__.py
--rw-r--r--   0        0        0     3171 2023-04-08 12:43:30.580990 lacss-0.2.2/lacss/modules/auxiliary.py
--rw-r--r--   0        0        0     2270 2023-03-17 14:54:37.064947 lacss-0.2.2/lacss/modules/common.py
--rw-r--r--   0        0        0     6394 2023-03-25 15:35:28.361632 lacss-0.2.2/lacss/modules/convnext.py
--rw-r--r--   0        0        0     6270 2023-04-04 12:56:43.303932 lacss-0.2.2/lacss/modules/detector.py
--rw-r--r--   0        0        0     3813 2023-04-06 15:08:48.257135 lacss-0.2.2/lacss/modules/lacss.py
--rw-r--r--   0        0        0     2934 2023-04-04 13:17:46.979593 lacss-0.2.2/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3771 2023-03-29 20:09:14.758729 lacss-0.2.2/lacss/modules/resnet.py
--rw-r--r--   0        0        0     4595 2023-03-24 12:44:29.815442 lacss-0.2.2/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     1979 2023-04-08 12:43:30.590920 lacss-0.2.2/lacss/modules/unet.py
--rw-r--r--   0        0        0      155 2023-03-08 13:25:26.937574 lacss-0.2.2/lacss/ops/__init__.py
--rw-r--r--   0        0        0     2175 2023-03-29 19:14:12.283632 lacss-0.2.2/lacss/ops/boxes.py
--rw-r--r--   0        0        0     2218 2023-03-29 20:11:51.333783 lacss-0.2.2/lacss/ops/image.py
--rw-r--r--   0        0        0     2739 2023-03-08 13:25:24.882290 lacss-0.2.2/lacss/ops/locations.py
--rw-r--r--   0        0        0     5967 2023-03-08 13:25:26.971031 lacss-0.2.2/lacss/ops/masks.py
--rw-r--r--   0        0        0     4704 2023-03-08 13:25:26.979821 lacss-0.2.2/lacss/ops/nms.py
--rw-r--r--   0        0        0     9245 2023-03-31 20:18:30.816558 lacss-0.2.2/lacss/ops/patches.py
--rw-r--r--   0        0        0       19 2023-03-07 23:30:16.150024 lacss-0.2.2/lacss/tracking/__init__.py
--rw-r--r--   0        0        0    13086 2023-04-05 14:50:34.337479 lacss-0.2.2/lacss/tracking/smc.py
--rw-r--r--   0        0        0       99 2023-03-17 14:54:37.111420 lacss-0.2.2/lacss/train/__init__.py
--rw-r--r--   0        0        0      718 2023-03-08 13:25:27.022221 lacss-0.2.2/lacss/train/data/__init__.py
--rw-r--r--   0        0        0     4076 2023-03-08 13:25:25.475969 lacss-0.2.2/lacss/train/data/array_adapter.py
--rw-r--r--   0        0        0     5529 2023-03-08 13:25:25.535533 lacss-0.2.2/lacss/train/data/data_adapter.py
--rw-r--r--   0        0        0     6287 2023-03-07 20:25:59.686559 lacss-0.2.2/lacss/train/data/data_handler.py
--rw-r--r--   0        0        0    10656 2023-03-07 23:30:16.170915 lacss-0.2.2/lacss/train/data/dataset.py
--rw-r--r--   0        0        0     2599 2023-03-07 20:26:00.050854 lacss-0.2.2/lacss/train/data/generator_adapter.py
--rw-r--r--   0        0        0     2105 2023-03-07 20:26:00.044184 lacss-0.2.2/lacss/train/data/list_adapter.py
--rw-r--r--   0        0        0     3440 2023-03-07 20:25:59.695064 lacss-0.2.2/lacss/train/data/tf_dataset_adapter.py
--rw-r--r--   0        0        0     2566 2023-03-07 20:25:59.999227 lacss-0.2.2/lacss/train/data/torch_dataloader_adapter.py
--rw-r--r--   0        0        0     6394 2023-03-08 13:25:25.861971 lacss-0.2.2/lacss/train/data/utils.py
--rw-r--r--   0        0        0     6859 2023-04-02 20:23:18.129096 lacss-0.2.2/lacss/train/loss.py
--rw-r--r--   0        0        0      222 2023-03-17 14:54:37.123202 lacss-0.2.2/lacss/train/metric.py
--rw-r--r--   0        0        0     4303 2023-04-07 15:15:01.848289 lacss-0.2.2/lacss/train/strategy.py
--rw-r--r--   0        0        0     5793 2023-04-05 20:33:38.500440 lacss-0.2.2/lacss/train/trainer.py
--rw-r--r--   0        0        0     4571 2023-04-04 13:04:53.871986 lacss-0.2.2/lacss/utils.py
--rw-r--r--   0        0        0      810 2023-04-08 14:07:44.893006 lacss-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 lacss-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-03-07 20:26:01.088077 lacss-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1140 2023-04-14 14:17:40.520445 lacss-0.3.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-20 16:47:25.199622 lacss-0.3.0/lacss/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-08 13:25:26.759293 lacss-0.3.0/lacss/data/__init__.py
+-rw-r--r--   0        0        0     6063 2023-03-08 13:25:26.771841 lacss-0.3.0/lacss/data/generator.py
+-rw-r--r--   0        0        0     9160 2023-04-09 15:45:08.107465 lacss-0.3.0/lacss/data/parser.py
+-rw-r--r--   0        0        0     3107 2023-04-20 16:47:25.195421 lacss-0.3.0/lacss/deploy.py
+-rw-r--r--   0        0        0       74 2023-03-08 13:25:26.788189 lacss-0.3.0/lacss/losses/__init__.py
+-rw-r--r--   0        0        0     5524 2023-04-17 17:58:59.215796 lacss-0.3.0/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0     3189 2023-04-09 15:45:08.834799 lacss-0.3.0/lacss/losses/detection.py
+-rw-r--r--   0        0        0     8278 2023-04-19 18:55:57.265740 lacss-0.3.0/lacss/losses/instance.py
+-rw-r--r--   0        0        0       56 2023-04-09 15:43:25.895964 lacss-0.3.0/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0     5547 2023-04-09 15:45:08.243066 lacss-0.3.0/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      216 2023-04-09 15:45:09.203039 lacss-0.3.0/lacss/modules/__init__.py
+-rw-r--r--   0        0        0     3171 2023-04-10 12:50:28.921730 lacss-0.3.0/lacss/modules/auxiliary.py
+-rw-r--r--   0        0        0     2270 2023-04-09 15:43:26.027653 lacss-0.3.0/lacss/modules/common.py
+-rw-r--r--   0        0        0     6557 2023-04-17 17:58:06.955449 lacss-0.3.0/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     6270 2023-04-09 15:43:26.072837 lacss-0.3.0/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3813 2023-04-09 15:45:08.267826 lacss-0.3.0/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     2934 2023-04-09 15:45:08.286815 lacss-0.3.0/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3771 2023-04-09 15:45:07.023954 lacss-0.3.0/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     4595 2023-04-09 15:45:07.056520 lacss-0.3.0/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     1979 2023-04-10 12:50:41.257622 lacss-0.3.0/lacss/modules/unet.py
+-rw-r--r--   0        0        0      155 2023-03-08 13:25:26.937574 lacss-0.3.0/lacss/ops/__init__.py
+-rw-r--r--   0        0        0     2175 2023-04-09 15:43:24.529427 lacss-0.3.0/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     2218 2023-04-09 15:45:07.073615 lacss-0.3.0/lacss/ops/image.py
+-rw-r--r--   0        0        0     2739 2023-03-08 13:25:24.882290 lacss-0.3.0/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5967 2023-03-08 13:25:26.971031 lacss-0.3.0/lacss/ops/masks.py
+-rw-r--r--   0        0        0     4704 2023-03-08 13:25:26.979821 lacss-0.3.0/lacss/ops/nms.py
+-rw-r--r--   0        0        0     9245 2023-04-09 15:45:08.363814 lacss-0.3.0/lacss/ops/patches.py
+-rw-r--r--   0        0        0       19 2023-03-07 23:30:16.150024 lacss-0.3.0/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0    13086 2023-04-09 15:41:06.218121 lacss-0.3.0/lacss/tracking/smc.py
+-rw-r--r--   0        0        0       99 2023-04-09 15:43:27.268348 lacss-0.3.0/lacss/train/__init__.py
+-rw-r--r--   0        0        0      718 2023-03-08 13:25:27.022221 lacss-0.3.0/lacss/train/data/__init__.py
+-rw-r--r--   0        0        0     4076 2023-03-08 13:25:25.475969 lacss-0.3.0/lacss/train/data/array_adapter.py
+-rw-r--r--   0        0        0     5529 2023-03-08 13:25:25.535533 lacss-0.3.0/lacss/train/data/data_adapter.py
+-rw-r--r--   0        0        0     6287 2023-03-07 20:25:59.686559 lacss-0.3.0/lacss/train/data/data_handler.py
+-rw-r--r--   0        0        0    10656 2023-03-07 23:30:16.170915 lacss-0.3.0/lacss/train/data/dataset.py
+-rw-r--r--   0        0        0     2599 2023-03-07 20:26:00.050854 lacss-0.3.0/lacss/train/data/generator_adapter.py
+-rw-r--r--   0        0        0     2105 2023-03-07 20:26:00.044184 lacss-0.3.0/lacss/train/data/list_adapter.py
+-rw-r--r--   0        0        0     3440 2023-03-07 20:25:59.695064 lacss-0.3.0/lacss/train/data/tf_dataset_adapter.py
+-rw-r--r--   0        0        0     2566 2023-03-07 20:25:59.999227 lacss-0.3.0/lacss/train/data/torch_dataloader_adapter.py
+-rw-r--r--   0        0        0     6394 2023-03-08 13:25:25.861971 lacss-0.3.0/lacss/train/data/utils.py
+-rw-r--r--   0        0        0     6826 2023-04-09 15:45:10.891402 lacss-0.3.0/lacss/train/loss.py
+-rw-r--r--   0        0        0      222 2023-04-09 15:43:26.263916 lacss-0.3.0/lacss/train/metric.py
+-rw-r--r--   0        0        0     4018 2023-04-09 15:45:10.909855 lacss-0.3.0/lacss/train/strategy.py
+-rw-r--r--   0        0        0     7437 2023-04-14 17:55:24.096524 lacss-0.3.0/lacss/train/trainer.py
+-rw-r--r--   0        0        0     4571 2023-04-20 16:47:25.237210 lacss-0.3.0/lacss/utils.py
+-rw-r--r--   0        0        0      810 2023-04-21 18:21:08.516980 lacss-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 lacss-0.3.0/PKG-INFO
```

### Comparing `lacss-0.2.2/LICENSE` & `lacss-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/data/generator.py` & `lacss-0.3.0/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/data/parser.py` & `lacss-0.3.0/lacss/data/parser.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/deploy.py` & `lacss-0.3.0/lacss/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,19 @@
         cfg = dataclasses.asdict(cfg)
 
     module = lacss.modules.Lacss(**cfg)
 
     return module, freeze(params)
 
 
+@partial(jax.jit, static_argnums=0)
+def _predict(apply_fn, params, image):
+    return apply_fn(dict(params=params), image)
+
+
 class Predictor:
     def __init__(self, url, precompile_shape=None):
 
         self.model = load_from_pretrained(url)
 
         if precompile_shape is not None:
 
@@ -93,35 +98,23 @@
                 iter(precompile_shape[0])
             except:
                 precompile_shape = [precompile_shape]
             for shape in precompile_shape:
                 x = np.zeros(shape)
                 _ = self.predict(x)
 
-    def _predict(self, image, apply_fn, strategy):
-        _, params = self.model
-
-        predict_fn = strategy.predict
-
-        state = TrainState.create(
-            params=params,
-            apply_fn=apply_fn,
-        )
-
-        return predict_fn(state, image)
-
-    def predict(self, image, *, strategy=strategy.Core, **kwargs):
+    def predict(self, image, **kwargs):
 
         module, params = self.model
 
         if len(kwargs) > 0:
-            apply_fn = _cached_partial(module.apply_fn, **kwargs)
+            apply_fn = _cached_partial(module.apply, **kwargs)
         else:
-            apply_fn = module.apply_fn
+            apply_fn = module.apply
 
-        return self._predict(image, strategy, apply_fn)
+        return _predict(apply_fn, params, image)
 
     def predict_label(self, image, **kwargs):
 
         preds = self.predict(image, **kwargs)
 
         return patches_to_label(preds, input_size=image.shape[:2])
```

### Comparing `lacss-0.2.2/lacss/losses/auxiliary.py` & `lacss-0.3.0/lacss/losses/auxiliary.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             & (preds["instance_xc"] < width)
         )
 
         areas = jnp.sum(
             preds["instance_output"], axis=(-1, -2), where=valid_locs, keepdims=True
         )
         areas = jnp.clip(areas, EPS, 1e6)
-        loss = jax.lax.rsqrt(areas) * self.a
+        loss = jax.lax.rsqrt(areas) * preds["instance_output"].shape[-1] * self.a
 
         mask = preds["instance_mask"]
         n_instances = jnp.count_nonzero(mask) + EPS
         loss = loss.sum(where=mask) / n_instances
 
         return loss
 
@@ -160,21 +160,24 @@
             logit += offset
 
             label = label.at[yc + ps // 2, xc + ps // 2].max(logit)
             label = label[ps // 2 : -ps // 2, ps // 2 : -ps // 2]
 
             return label
 
-        fg_pred = jax.nn.tanh(preds["fg_pred"])
-        fg_label = jax.nn.tanh(_max_merge(preds))
+        # fg_pred = jax.nn.tanh(preds["fg_pred"] / 2)
+        # fg_label = jax.nn.tanh(_max_merge(preds) / 2)
+        fg_pred = jax.nn.sigmoid(preds["fg_pred"])
+        fg_label = jax.lax.stop_gradient(jax.nn.sigmoid(_max_merge(preds)))
 
         locs = jnp.floor(inputs["gt_locations"] + 0.5)
         locs = locs.astype(int)
         fg_label = fg_label.at[locs[:, 0], locs[:, 1]].set(1.0)
 
         assert fg_pred.shape == fg_label.shape
 
-        loss = 1.0 - fg_pred * jax.lax.stop_gradient(fg_label)
+        # loss = 1.0 - fg_pred * jax.lax.stop_gradient(fg_label)
+        loss = (1.0 - fg_label) * fg_pred + fg_label * (1.0 - fg_pred)
 
         loss = loss.mean()
 
         return loss
```

### Comparing `lacss-0.2.2/lacss/losses/detection.py` & `lacss-0.3.0/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/losses/instance.py` & `lacss-0.3.0/lacss/losses/instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -156,15 +156,19 @@
 class SupervisedInstanceLoss(Loss):
     def call(self, preds: dict, labels: dict, **kwargs):
 
         instance_mask = preds["instance_mask"]
         instance_logit = preds["instance_logit"]
         yc = preds["instance_yc"]
         xc = preds["instance_xc"]
-        gt_labels = labels["gt_labels"].astype("int32")
+
+        if isinstance(labels, dict):
+            gt_labels = labels["gt_labels"].astype("int32")
+        else:
+            gt_labels = labels.astype("int32")
 
         n_patches, ps, _ = yc.shape
 
         gt_labels = jnp.pad(gt_labels, ps // 2)
         gt_patches = gt_labels[yc + ps // 2, xc + ps // 2] == (
             jnp.arange(n_patches)[:, None, None] + 1
         )
@@ -172,37 +176,60 @@
 
         loss = optax.sigmoid_binary_cross_entropy(instance_logit, gt_patches)
 
         return _mean_over_boolean_mask(loss, instance_mask)
 
 
 class SelfSupervisedInstanceLoss(Loss):
+    def __init__(self, soft_label: bool = True, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.soft_label = soft_label
+
     def call(self, preds: dict, **kwargs):
 
         instance_mask = preds["instance_mask"]
         instances = preds["instance_output"]
+        instance_logit = preds["instance_logit"]
         yc = preds["instance_yc"]
         xc = preds["instance_xc"]
 
         patch_size = instances.shape[-1]
         padding_size = patch_size // 2 + 2
         yc += padding_size
         xc += padding_size
 
         binary_mask = jax.lax.stop_gradient(jax.nn.sigmoid(preds["fg_pred"]))
+        # binary_mask = jax.lax.stop_gradient(preds["fg_pred"])
         seg = jnp.pad(binary_mask, padding_size)
 
-        seg_patch = seg[yc, xc]
-        loss = (1.0 - seg_patch) * instances + seg_patch * (1.0 - instances)
+        if self.soft_label:
+
+            seg_patch = seg[yc, xc]
+
+            loss = (1.0 - seg_patch) * instances + seg_patch * (1.0 - instances)
+
+            instance_sum = jnp.zeros_like(seg)
+            instance_sum = instance_sum.at[yc, xc].add(instances)
+            instance_sum_i = instance_sum[yc, xc] - instances
+
+            loss = loss + instances * instance_sum_i
+
+        else:
+
+            seg = (seg > 0.5).astype(instances.dtype)
+            seg_patch = seg[yc, xc]
+
+            loss = (1.0 - seg_patch) * instances + seg_patch * (1.0 - instances)
 
-        instance_sum = jnp.zeros_like(seg)
-        instance_sum = instance_sum.at[yc, xc].add(instances)
-        instance_sum_i = instance_sum[yc, xc] - instances
+            log_yi_sum = jnp.zeros_like(seg)
+            log_yi = -jax.nn.log_sigmoid(-instance_logit)
+            log_yi_sum = log_yi_sum.at[yc, xc].add(log_yi)
+            log_yi = log_yi_sum[yc, xc] - log_yi
 
-        loss = loss + instances * instance_sum_i
+            loss = loss + (instances * log_yi)
 
         return _mean_over_boolean_mask(loss, instance_mask)
 
 
 class WeaklySupervisedInstanceLoss(Loss):
     def __init__(self, ignore_mask: bool = False, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -222,27 +249,30 @@
         xc += padding_size
 
         if self.ignore_mask:
             seg = jnp.zeros(inputs["image"].shape[:-1])
             seg = jnp.pad(seg, padding_size)
             loss = jnp.zeros_like(instances)
         else:
-            seg = labels["gt_mask"].astype("float32")
+            if isinstance(labels, dict):
+                seg = labels["gt_mask"].astype("float32")
+            else:
+                seg = labels.astype("float32")
             seg = jnp.pad(seg, padding_size)
             seg_patch = seg[yc, xc]
             loss = (1.0 - seg_patch) * instances + seg_patch * (1.0 - instances)
 
-        # log_yi_sum = jnp.zeros_like(seg)
+        log_yi_sum = jnp.zeros_like(seg)
 
-        # log_yi = - jax.nn.log_sigmoid( - instance_logit)
-        # log_yi_sum = log_yi_sum.at[yc, xc].add(log_yi)
-        # log_yi = log_yi_sum[yc, xc] - log_yi
+        log_yi = -jax.nn.log_sigmoid(-instance_logit)
+        log_yi_sum = log_yi_sum.at[yc, xc].add(log_yi)
+        log_yi = log_yi_sum[yc, xc] - log_yi
 
-        # loss = loss + (instances * log_yi)
+        loss = loss + (instances * log_yi)
 
-        instance_sum = jnp.zeros_like(seg)
-        instance_sum = instance_sum.at[yc, xc].add(instances)
-        instance_sum_i = instance_sum[yc, xc] - instances
+        # instance_sum = jnp.zeros_like(seg)
+        # instance_sum = instance_sum.at[yc, xc].add(instances)
+        # instance_sum_i = instance_sum[yc, xc] - instances
 
-        loss = loss + (instances * instance_sum_i)
+        # loss = loss + (instances * instance_sum_i)
 
         return _mean_over_boolean_mask(loss, instance_mask)
```

### Comparing `lacss-0.2.2/lacss/metrics/ranked.py` & `lacss-0.3.0/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/auxiliary.py` & `lacss-0.3.0/lacss/modules/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/common.py` & `lacss-0.3.0/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/convnext.py` & `lacss-0.3.0/lacss/modules/convnext.py`

 * *Files 18% similar despite different names*

```diff
@@ -105,59 +105,71 @@
     "convnext_tiny_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_tiny_22k_224.pth",
     "convnext_small_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_small_22k_224.pth",
     "convnext_base_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_base_22k_224.pth",
     "convnext_large_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_large_22k_224.pth",
     "convnext_xlarge_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_xlarge_22k_224.pth",
 }
 
-# def load_weight(jax_model, url):
-#     ''' Load pretrained convnext models
-#     specs for pretrained models are:
-#         tiny: dims=(96, 192, 384, 768), depths=(3,3,9,3)
-#         small: dims=(96, 192, 384, 768), depths=(3,3,27,3)
-#         base: dims=(128, 256, 512, 1024), depths=(3,3,27,3)
-#         large: dims=(192, 384, 768, 1536), depths=(3,3,27,3)
-#         X-large: dims=(256, 512, 1024, 2048), depths=(3,3,27,3)
-#     '''
-#     import torch
-
-#     def t(m, k, new_value):
-#         new_value = jnp.array(new_value)
-#         assert vars(m)[k].shape == new_value.shape
-#         vars(m)[k] = new_value
-
-#     checkpoint = torch.hub.load_state_dict_from_url(url=url, map_location="cpu")
-#     params = checkpoint['model']
-
-#     cnt = 1
-#     for i in range(4):
-#         for k in range(jax_model.depths[i]):
-#             block = vars(jax_model)[f'block{cnt}' if cnt > 1 else 'block']
-#             t(block, 'gamma', params[f'stages.{i}.{k}.gamma'])
-#             t(block.conv, 'bias', params[f'stages.{i}.{k}.dwconv.bias'])
-#             t(block.conv, 'kernel', params[f'stages.{i}.{k}.dwconv.weight'].permute(2,3,1,0))
-#             t(block.layer_norm, 'bias', params[f'stages.{i}.{k}.norm.bias'])
-#             t(block.layer_norm, 'scale', params[f'stages.{i}.{k}.norm.weight'])
-#             t(block.linear, 'bias', params[f'stages.{i}.{k}.pwconv1.bias'])
-#             t(block.linear, 'kernel', params[f'stages.{i}.{k}.pwconv1.weight'].transpose(0,1))
-#             t(block.linear2, 'bias', params[f'stages.{i}.{k}.pwconv2.bias'])
-#             t(block.linear2, 'kernel', params[f'stages.{i}.{k}.pwconv2.weight'].transpose(0,1))
-
-#             cnt += 1
-
-#     norm = jax_model.layer_norm
-#     t(norm, 'bias', params['downsample_layers.0.1.bias'])
-#     t(norm, 'scale', params['downsample_layers.0.1.weight'])
-
-#     conv = jax_model.conv
-#     t(conv, 'bias', params['downsample_layers.0.0.bias'])
-#     t(conv, 'kernel', params['downsample_layers.0.0.weight'].permute(2,3,1,0))
-
-#     for i in range(1,4):
-#         norm = vars(jax_model)[f'layer_norm{i+1}']
-#         t(norm, 'bias', params[f'downsample_layers.{i}.0.bias'])
-#         t(norm, 'scale', params[f'downsample_layers.{i}.0.weight'])
-#         conv = vars(jax_model)[f'conv{i+1}']
-#         t(conv, 'bias', params[f'downsample_layers.{i}.1.bias'])
-#         t(conv, 'kernel', params[f'downsample_layers.{i}.1.weight'].permute(2,3,1,0))
 
-#     return jax_model
+def load_weight(jax_model, jax_params, url):
+    """Load pretrained convnext models
+    specs for pretrained models are:
+        tiny: dims=(96, 192, 384, 768), depths=(3,3,9,3)
+        small: dims=(96, 192, 384, 768), depths=(3,3,27,3)
+        base: dims=(128, 256, 512, 1024), depths=(3,3,27,3)
+        large: dims=(192, 384, 768, 1536), depths=(3,3,27,3)
+        X-large: dims=(256, 512, 1024, 2048), depths=(3,3,27,3)
+    """
+    import torch
+    from flax.core.frozen_dict import freeze, unfreeze
+
+    def t(m, new_value):
+        new_value = jnp.array(new_value)
+        assert m.shape == new_value.shape
+        m = new_value
+
+    checkpoint = torch.hub.load_state_dict_from_url(url=url, map_location="cpu")
+    params = checkpoint["model"]
+    jax_params = unfreeze(jax_params)
+
+    cnt = 0
+    for i in range(4):
+        for k in range(jax_model.depths[i]):
+            block = jax_params[f"_Block_{cnt}"]
+            t(block["gamma"], params[f"stages.{i}.{k}.gamma"])
+            t(block["Conv_0"]["bias"], params[f"stages.{i}.{k}.dwconv.bias"])
+            t(
+                block["Conv_0"]["kernel"],
+                params[f"stages.{i}.{k}.dwconv.weight"].permute(2, 3, 1, 0),
+            )
+            t(block["LayerNorm_0"]["bias"], params[f"stages.{i}.{k}.norm.bias"])
+            t(block["LayerNorm_0"]["scale"], params[f"stages.{i}.{k}.norm.weight"])
+            t(block["Dense_0"]["bias"], params[f"stages.{i}.{k}.pwconv1.bias"])
+            t(
+                block["Dense_0"]["kernel"],
+                params[f"stages.{i}.{k}.pwconv1.weight"].transpose(0, 1),
+            )
+            t(block["Dense_1"]["bias"], params[f"stages.{i}.{k}.pwconv2.bias"])
+            t(
+                block["Dense_1"]["kernel"],
+                params[f"stages.{i}.{k}.pwconv2.weight"].transpose(0, 1),
+            )
+
+            cnt += 1
+
+    norm = jax_params[f"LayerNorm_0"]
+    t(norm["bias"], params["downsample_layers.0.1.bias"])
+    t(norm["scale"], params["downsample_layers.0.1.weight"])
+
+    conv = jax_params[f"Conv_0"]
+    t(conv["bias"], params["downsample_layers.0.0.bias"])
+    t(conv["kernel"], params["downsample_layers.0.0.weight"].permute(2, 3, 1, 0))
+
+    for i in range(1, 4):
+        norm = jax_params[f"LayerNorm_{i}"]
+        t(norm["bias"], params[f"downsample_layers.{i}.0.bias"])
+        t(norm["scale"], params[f"downsample_layers.{i}.0.weight"])
+        conv = jax_params[f"Conv_{i}"]
+        t(conv["bias"], params[f"downsample_layers.{i}.1.bias"])
+        t(conv["kernel"], params[f"downsample_layers.{i}.1.weight"].permute(2, 3, 1, 0))
+
+    return freeze(jax_params)
```

### Comparing `lacss-0.2.2/lacss/modules/detector.py` & `lacss-0.3.0/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/lacss.py` & `lacss-0.3.0/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/lpn.py` & `lacss-0.3.0/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/resnet.py` & `lacss-0.3.0/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/segmentor.py` & `lacss-0.3.0/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/modules/unet.py` & `lacss-0.3.0/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/ops/boxes.py` & `lacss-0.3.0/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/ops/image.py` & `lacss-0.3.0/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/ops/locations.py` & `lacss-0.3.0/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/ops/masks.py` & `lacss-0.3.0/lacss/ops/masks.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/ops/nms.py` & `lacss-0.3.0/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/ops/patches.py` & `lacss-0.3.0/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/tracking/smc.py` & `lacss-0.3.0/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/__init__.py` & `lacss-0.3.0/lacss/train/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/array_adapter.py` & `lacss-0.3.0/lacss/train/data/array_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/data_adapter.py` & `lacss-0.3.0/lacss/train/data/data_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/data_handler.py` & `lacss-0.3.0/lacss/train/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/dataset.py` & `lacss-0.3.0/lacss/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/generator_adapter.py` & `lacss-0.3.0/lacss/train/data/generator_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/list_adapter.py` & `lacss-0.3.0/lacss/train/data/list_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/tf_dataset_adapter.py` & `lacss-0.3.0/lacss/train/data/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/torch_dataloader_adapter.py` & `lacss-0.3.0/lacss/train/data/torch_dataloader_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/data/utils.py` & `lacss-0.3.0/lacss/train/data/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/lacss/train/loss.py` & `lacss-0.3.0/lacss/train/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,17 @@
         raise ValueError(f"Invalid reduction '{reduction}'")
 
     return loss * weight
 
 
 class LossLog(struct.PyTreeNode):
     loss_fn: Loss = struct.field(pytree_node=False)
-    weight: jnp.ndarray = jnp.array(1.0)
-    cnt: jnp.ndarray = jnp.array(0.0)
-    sum: jnp.ndarray = jnp.array(0.0)
+    weight: jnp.ndarray = 1.0
+    cnt: jnp.ndarray = 0.0
+    sum: jnp.ndarray = 0.0
 
     def update(self, **kwargs):
         loss = self.loss_fn(**kwargs) * self.weight
         new_log = self.replace(cnt=self.cnt + 1, sum=self.sum + loss)
         return loss, new_log
 
     def compute(self):
```

### Comparing `lacss-0.2.2/lacss/train/strategy.py` & `lacss-0.3.0/lacss/train/strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,29 +29,20 @@
 
         losses, loss_logs = zip(*[loss_fn.update(**args) for loss_fn in loss_logs])
         total_loss = sum(losses)
 
         return total_loss, (state, loss_logs, preds)
 
     @classmethod
-    def init_fn(cls, key, model, inputs, tx):
+    def init_fn(cls, key, model, inputs):
         inputs_obj = Inputs.from_value(inputs)
 
-        # mode is not bound
-        if model.scope is None:
-            variables = model.init(key, *inputs_obj.args, **inputs_obj.kwargs)
-        else:
-            model, variables = model.unbind()
-
-        state = TrainState.create(
-            apply_fn=model.apply,
-            params=variables["params"],
-            tx=tx,
-        )
-        return state, model
+        state = model.init(key, *inputs_obj.args, **inputs_obj.kwargs)
+
+        return state
 
     @classmethod
     def predict(cls, state, inputs):  # only if model is immutable
         # print("JIT Predict")
         inputs_obj = Inputs.from_value(inputs)
         preds = state.apply_fn(
             {"params": state.params}, *inputs_obj.args, **inputs_obj.kwargs
@@ -123,17 +114,17 @@
 
         #         # sync batch statistics
         #         model.map(partial(jax.lax.pmean, axis_name="mapped"), tx.BatchStat, inplace=True)
 
         return state, loss_logs, preds
 
     @classmethod
-    def init_fn(cls, key, model, inputs, tx):
+    def init_fn(cls, key, model, inputs):
         inputs = jax.tree_map(lambda v: v[0], inputs)
-        return Eager.init_fn(key, model, inputs, tx)
+        return Eager.init_fn(key, model, inputs)
 
 
 class Distributed(_Distributed):
     train_step = jax.pmap(
         _Distributed._train_step,
         axis_name="mapped",
         in_axes=(None, None, 0, 0, None),
```

### Comparing `lacss-0.2.2/lacss/train/trainer.py` & `lacss-0.3.0/lacss/train/trainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,44 +26,88 @@
         self,
         model: nn.Module,
         losses: tp.Optional[tp.Union[tp.Sequence[Loss], Loss]] = None,
         optimizer: GradientTransformation = None,
         seed: int = 42,
         strategy: type = strategy.JIT,
     ):
+
         self.model = model
-        self.losses = (losses,) if isinstance(losses, Loss) else losses
+        self.losses = losses
+        self._loss_weights = None
+
         self.seed = seed if isinstance(seed, jnp.ndarray) else jax.random.PRNGKey(seed)
-        self.optimizer = optimizer
+        self._optimizer = optimizer
 
         self._strategy = strategy
         self._initialized = False
 
-        self.reset()
+        # self.reset()
+
+    def reset(self, loss_weights=None):
+
+        if self.losses is None:
+            raise ValueError(f"No loss functions provided")
+
+        losses = self.losses
+        try:
+            iter(losses)
+        except:
+            losses = (losses,)
+
+        if loss_weights is not None:
+            self._loss_weights = loss_weights
+        else:
+            loss_weights = self._loss_weights
+
+        if loss_weights is None:
+            loss_weights = (1.0,) * len(losses)
+
+        if len(loss_weights) != len(self.losses):
+            raise ValueError(
+                f"Loss weights supplied {loss_weights} does not match the number of loss functions ({len(losses)})"
+            )
 
-    def reset(self):
-        self.loss_logs = tuple(LossLog(loss) for loss in self.losses)
+        self.loss_logs = tuple(
+            LossLog(loss, w) for loss, w in zip(self.losses, loss_weights)
+        )
 
     @property
     def initialized(self):
         return self._initialized
 
     def initialize(self, dataset, tx: GradientTransformation = None):
 
         if tx is None:
             tx = self.optimizer
 
         if not self._initialized:
-            peek = next(dataset())
-            inputs, _, _ = unpack_x_y_sample_weight(peek)
 
-            self.seed, key = jax.random.split(self.seed)
-            self.state, self.model = self._strategy.init_fn(key, self.model, inputs, tx)
+            if self.model.scope is None:
+
+                peek = next(dataset())
+                inputs, _, _ = unpack_x_y_sample_weight(peek)
+
+                self.seed, key = jax.random.split(self.seed)
+                variables = self._strategy.init_fn(key, self.model, inputs)
+
+            else:
+
+                self.model, variables = self.model.unbind()
+
+            self.state = TrainState.create(
+                apply_fn=self.model.apply,
+                params=variables["params"],
+                tx=tx,
+            )
+
+        else:
+
+            raise ValueError("Calling initialize() on already initialized Trainer")
 
-        self.reset()
         self._initialized = True
 
     def __call__(self, inputs, *, strategy=None, **kwargs):
         if strategy is None:
             strategy = self._strategy
 
         predict_fn = strategy.predict
@@ -119,15 +163,15 @@
 
     def save_model(self, path, sub_module: tp.Optional[str] = None):
         module = self.model
         params = self.params
 
         if sub_module is not None:
             module = module.bind(dict(params=params))
-            module = module[sub_module]
+            module = getattr(module, sub_module)
             module, params = module.unbind()
             params = params["params"]
 
         if isinstance(path, str):
             path = pathlib.Path(path)
 
         path.parent.mkdir(parents=True, exist_ok=True)
@@ -151,15 +195,20 @@
             path = pathlib.Path(path)
 
         try:
             _bytes = path.read_bytes()
         except BaseException as e:
             raise OSError(f"Could not load the checkpoint. Got exception: {e}")
 
-        return cloudpickle.loads(_bytes)
+        trainer = cloudpickle.loads(_bytes)
+
+        if not isinstance(trainer, Trainer):
+            raise TypeError("The saved obj is not a Trainer checkpoint")
+
+        return trainer
 
     def test(self, dataset, metrics, strategy=None):
         if strategy is None:
             strategy = self._strategy
 
         try:
             iter(metrics)
@@ -186,7 +235,24 @@
         for metrics in self.test(*args, **kwargs):
             pass
         return {_get_name(m): m.compute() for m in metrics}
 
     @property
     def params(self):
         return self.state.params
+
+    @property
+    def optimizer(self):
+        return self._optimizer
+
+    @optimizer.setter
+    def optimizer(self, tx):
+
+        self._optimizer = tx
+
+        if self._initialized:
+
+            self.state = TrainState.create(
+                apply_fn=self.model.apply,
+                params=self.params,
+                tx=tx,
+            )
```

### Comparing `lacss-0.2.2/lacss/utils.py` & `lacss-0.3.0/lacss/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.2.2/pyproject.toml` & `lacss-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacss"
-version = "0.2.2"
+version = "0.3.0"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

