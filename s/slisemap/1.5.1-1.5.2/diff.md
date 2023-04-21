# Comparing `tmp/slisemap-1.5.1.tar.gz` & `tmp/slisemap-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slisemap-1.5.1.tar", last modified: Fri Mar 31 13:33:44 2023, max compression
+gzip compressed data, was "slisemap-1.5.2.tar", last modified: Fri Apr 21 11:27:54 2023, max compression
```

## Comparing `slisemap-1.5.1.tar` & `slisemap-1.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:33:44.512075 slisemap-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-31 13:33:31.000000 slisemap-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-03-31 13:33:44.512075 slisemap-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-31 13:33:31.000000 slisemap-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-31 13:33:31.000000 slisemap-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 13:33:44.512075 slisemap-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:33:44.508075 slisemap-1.5.1/slisemap/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/local_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    62025 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/slisemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-03-31 13:33:31.000000 slisemap-1.5.1/slisemap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:33:44.508075 slisemap-1.5.1/slisemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-03-31 13:33:44.000000 slisemap-1.5.1/slisemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-31 13:33:44.000000 slisemap-1.5.1/slisemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:33:44.000000 slisemap-1.5.1/slisemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-31 13:33:44.000000 slisemap-1.5.1/slisemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 13:33:44.000000 slisemap-1.5.1/slisemap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:33:44.512075 slisemap-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_local_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_slisemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-31 13:33:31.000000 slisemap-1.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:27:54.668438 slisemap-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 11:27:43.000000 slisemap-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-21 11:27:54.668438 slisemap-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-21 11:27:43.000000 slisemap-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-21 11:27:43.000000 slisemap-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 11:27:54.668438 slisemap-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:27:54.668438 slisemap-1.5.2/slisemap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/local_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62118 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/slisemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-04-21 11:27:43.000000 slisemap-1.5.2/slisemap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:27:54.668438 slisemap-1.5.2/slisemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-21 11:27:54.000000 slisemap-1.5.2/slisemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-21 11:27:54.000000 slisemap-1.5.2/slisemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:27:54.000000 slisemap-1.5.2/slisemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 11:27:54.000000 slisemap-1.5.2/slisemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 11:27:54.000000 slisemap-1.5.2/slisemap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:27:54.668438 slisemap-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_local_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_slisemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-21 11:27:43.000000 slisemap-1.5.2/tests/test_utils.py
```

### Comparing `slisemap-1.5.1/LICENSE` & `slisemap-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/PKG-INFO` & `slisemap-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slisemap
-Version: 1.5.1
+Version: 1.5.2
 Summary: SLISEMAP: Combine local explanations with supervised dimensionality reduction
 Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>, Jarmo Mäkelä <jarmo.makela@helsinki.fi>, Kai Puolamäki <kai.puolamaki@helsinki.fi>
 License: MIT License
         
         Copyright (c) 2023 Anton Björklund, Jarmo Mäkelä, and Kai Puolamäki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slisemap-1.5.1/README.md` & `slisemap-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/pyproject.toml` & `slisemap-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slisemap"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
     { name = "Anton Björklund", email = "anton.bjorklund@helsinki.fi" },
     { name = "Jarmo Mäkelä", email = "jarmo.makela@helsinki.fi" },
     { name = "Kai Puolamäki", email = "kai.puolamaki@helsinki.fi" },
 ]
 description = "SLISEMAP: Combine local explanations with supervised dimensionality reduction"
 readme = "README.md"
```

### Comparing `slisemap-1.5.1/slisemap/__init__.py` & `slisemap-1.5.2/slisemap/__init__.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/diagnostics.py` & `slisemap-1.5.2/slisemap/diagnostics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/escape.py` & `slisemap-1.5.2/slisemap/escape.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/local_models.py` & `slisemap-1.5.2/slisemap/local_models.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/loss.py` & `slisemap-1.5.2/slisemap/loss.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/metrics.py` & `slisemap-1.5.2/slisemap/metrics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/plot.py` & `slisemap-1.5.2/slisemap/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,14 +246,15 @@
 def plot_embedding_facet(
     Z: np.ndarray,
     dimensions: Sequence[str],
     data: np.ndarray,
     names: Sequence[str],
     legend_title: str = "Value",
     jitter: Union[float, np.ndarray] = 0.0,
+    share_hue: bool = True,
     **kwargs: Any,
 ) -> sns.FacetGrid:
     """Plot (multiple) embeddings.
 
     Args:
         Z: Embeddings.
         dimensions: Dimension names.
@@ -274,23 +275,43 @@
             legend_title: data[:, i],
             dimensions[0]: Z[:, 0],
             dimensions[1]: Z[:, 1],
         }
         for i, n in enumerate(names)
     )
     kwargs.setdefault("palette", "rocket")
-    kwargs.setdefault("kind", "scatter")
-    g = sns.relplot(
-        data=df,
-        x=dimensions[0],
-        y=dimensions[1],
-        hue=legend_title,
-        col="var",
-        **kwargs,
-    )
+    if share_hue:
+        kwargs.setdefault("kind", "scatter")
+        g = sns.relplot(
+            data=df,
+            x=dimensions[0],
+            y=dimensions[1],
+            hue=legend_title,
+            col="var",
+            **kwargs,
+        )
+    else:
+        fgkws = kwargs.pop("facet_kws", {})
+        fgkws.setdefault("height", 5)
+        for k in ("height", "aspect", "col_wrap"):
+            if k in kwargs:
+                fgkws[k] = kwargs.pop(k)
+        fgkws.setdefault("legend_out", False)
+        g = sns.FacetGrid(data=df, col="var", hue=legend_title, **fgkws)
+        for key, ax in g.axes_dict.items():
+            mask = df["var"] == key
+            df2 = {k: v[mask] for k, v in df.items()}
+            sns.scatterplot(
+                data=df2,
+                hue=legend_title,
+                x=dimensions[0],
+                y=dimensions[1],
+                ax=ax,
+                **kwargs,
+            )
     g.set_titles("{col_name}")
     return g
 
 
 def plot_position_legend(
     g: sns.FacetGrid,
     index: Optional[Sequence[int]],
```

### Comparing `slisemap-1.5.1/slisemap/slisemap.py` & `slisemap-1.5.2/slisemap/slisemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1370,15 +1370,15 @@
             _deprecated(
                 "Parameter 'targets' in 'Slisemap.plot'",
                 "'Slisemap.metadata.set_targets'",
             )
 
         kwargs.setdefault("figsize", (12, 6))
         fig, (ax1, ax2) = plt.subplots(1, 2, **kwargs)
-        if clusters is None:
+        if not np.iterable(clusters) and not clusters:
             _assert(not bars, "`bars!=False` requires `clusters`", Slisemap.plot)
             if Z.shape[0] == self._Z.shape[0]:
                 yhat = self.predict(numpy=False)
                 L = tonp(self.local_loss(yhat, self._Y, self._B)).ravel()
             else:
                 L = None
             plot_embedding(
@@ -1590,16 +1590,18 @@
             g = plot_embedding_facet(
                 self.get_Z(rotate=True),
                 self.metadata.get_dimensions(long=True),
                 data,
                 labels,
                 jitter=jitter,
                 col_wrap=col_wrap,
+                share_hue=False,
                 **kwargs,
             )
+            legend_inside = False
         else:
             if isinstance(clusters, int):
                 clusters, _ = self.get_model_clusters(clusters, B)
             elif clusters is None:
                 legend_inside = False
             g = plot_density_facet(
                 data, labels, clusters=clusters, col_wrap=col_wrap, **kwargs
```

### Comparing `slisemap-1.5.1/slisemap/tuning.py` & `slisemap-1.5.2/slisemap/tuning.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap/utils.py` & `slisemap-1.5.2/slisemap/utils.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/slisemap.egg-info/PKG-INFO` & `slisemap-1.5.2/slisemap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slisemap
-Version: 1.5.1
+Version: 1.5.2
 Summary: SLISEMAP: Combine local explanations with supervised dimensionality reduction
 Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>, Jarmo Mäkelä <jarmo.makela@helsinki.fi>, Kai Puolamäki <kai.puolamaki@helsinki.fi>
 License: MIT License
         
         Copyright (c) 2023 Anton Björklund, Jarmo Mäkelä, and Kai Puolamäki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slisemap-1.5.1/slisemap.egg-info/SOURCES.txt` & `slisemap-1.5.2/slisemap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_diagnostics.py` & `slisemap-1.5.2/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_escape.py` & `slisemap-1.5.2/tests/test_escape.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_local_models.py` & `slisemap-1.5.2/tests/test_local_models.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_metrics.py` & `slisemap-1.5.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_plot.py` & `slisemap-1.5.2/tests/test_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 def test_plot():
     try:
         sm, cl = get_slisemap2(30, 4, randomB=True)
         sm.plot(title="ASD", clusters=4, show=False)
         sm.plot(title="ASD", clusters=4, bars=True, show=False)
         sm.plot(title="ASD", clusters=4, bars=-1, show=False)
+        sm.plot(title="ASD", clusters=0, show=False)
         sm.plot(clusters=cl, bars=False, show=False)
         sm.plot(clusters=cl, bars=True, show=False)
         cl2 = np.asarray([f"A{9-i}" for i in np.unique(cl)])[cl]
         sm.plot(clusters=cl2, bars=False, show=False)
         sm.plot(clusters=cl2, bars=True, show=False)
         sm.plot(jitter=1, figsize=(2, 2), show=False)
         sm.metadata.set_variables(range(4), add_intercept=True)
```

### Comparing `slisemap-1.5.1/tests/test_save.py` & `slisemap-1.5.2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_slisemap.py` & `slisemap-1.5.2/tests/test_slisemap.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_tuning.py` & `slisemap-1.5.2/tests/test_tuning.py`

 * *Files identical despite different names*

### Comparing `slisemap-1.5.1/tests/test_utils.py` & `slisemap-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

