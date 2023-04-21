# Comparing `tmp/pynometrics-0.1.1.tar.gz` & `tmp/pynometrics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynometrics-0.1.1.tar", last modified: Sun Apr  2 10:39:03 2023, max compression
+gzip compressed data, was "pynometrics-0.1.2.tar", last modified: Fri Apr 21 08:21:08 2023, max compression
```

## Comparing `pynometrics-0.1.1.tar` & `pynometrics-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 10:39:03.141054 pynometrics-0.1.1/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1068 2023-04-01 18:56:30.000000 pynometrics-0.1.1/LICENSE.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       65 2023-04-01 18:56:30.000000 pynometrics-0.1.1/MANIFEST.in
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-02 10:39:03.140841 pynometrics-0.1.1/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      544 2023-04-01 18:56:30.000000 pynometrics-0.1.1/README.md
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 10:39:03.137895 pynometrics-0.1.1/examples/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      624 2023-04-01 18:56:30.000000 pynometrics-0.1.1/examples/example_01.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      656 2023-04-01 18:56:30.000000 pynometrics-0.1.1/examples/example_02.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-02 10:39:03.141132 pynometrics-0.1.1/setup.cfg
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1171 2023-04-02 10:38:33.000000 pynometrics-0.1.1/setup.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 10:39:03.138298 pynometrics-0.1.1/src/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     6148 2023-04-01 21:01:41.000000 pynometrics-0.1.1/src/.DS_Store
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 10:39:03.138986 pynometrics-0.1.1/src/pynometrics/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-01 18:56:30.000000 pynometrics-0.1.1/src/pynometrics/__init__.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    15919 2023-04-02 10:37:27.000000 pynometrics-0.1.1/src/pynometrics/pynometrics.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 10:39:03.140494 pynometrics-0.1.1/src/pynometrics.egg-info/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-02 10:39:03.000000 pynometrics-0.1.1/src/pynometrics.egg-info/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      393 2023-04-02 10:39:03.000000 pynometrics-0.1.1/src/pynometrics.egg-info/SOURCES.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-02 10:39:03.000000 pynometrics-0.1.1/src/pynometrics.egg-info/dependency_links.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-01 20:54:02.000000 pynometrics-0.1.1/src/pynometrics.egg-info/not-zip-safe
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       42 2023-04-02 10:39:03.000000 pynometrics-0.1.1/src/pynometrics.egg-info/requires.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       12 2023-04-02 10:39:03.000000 pynometrics-0.1.1/src/pynometrics.egg-info/top_level.txt
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.625345 pynometrics-0.1.2/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1068 2023-04-02 14:08:08.000000 pynometrics-0.1.2/LICENSE.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       65 2023-04-02 14:08:08.000000 pynometrics-0.1.2/MANIFEST.in
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 08:21:08.625134 pynometrics-0.1.2/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      544 2023-04-02 14:08:08.000000 pynometrics-0.1.2/README.md
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.622260 pynometrics-0.1.2/examples/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      624 2023-04-01 18:56:30.000000 pynometrics-0.1.2/examples/example_01.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      656 2023-04-01 18:56:30.000000 pynometrics-0.1.2/examples/example_02.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-21 08:21:08.625419 pynometrics-0.1.2/setup.cfg
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1171 2023-04-21 08:19:17.000000 pynometrics-0.1.2/setup.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.622591 pynometrics-0.1.2/src/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     6148 2023-04-01 21:01:41.000000 pynometrics-0.1.2/src/.DS_Store
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.623118 pynometrics-0.1.2/src/pynometrics/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 pynometrics-0.1.2/src/pynometrics/__init__.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16158 2023-04-21 08:19:11.000000 pynometrics-0.1.2/src/pynometrics/pynometrics.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.624850 pynometrics-0.1.2/src/pynometrics.egg-info/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      393 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-01 20:54:02.000000 pynometrics-0.1.2/src/pynometrics.egg-info/not-zip-safe
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       42 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/requires.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       12 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/top_level.txt
```

### Comparing `pynometrics-0.1.1/LICENSE.txt` & `pynometrics-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.1/PKG-INFO` & `pynometrics-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynometrics
-Version: 0.1.1
+Version: 0.1.2
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/econometric_package.git
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pynometrics-0.1.1/README.md` & `pynometrics-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.1/examples/example_01.py` & `pynometrics-0.1.2/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.1/examples/example_02.py` & `pynometrics-0.1.2/examples/example_02.py`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.1/setup.py` & `pynometrics-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("/Users/geofrey.wanyama/Desktop/wg/projects/package_dev/pyeconometrics/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     # name that will be imported, can be different from code file name
     name='pynometrics',
 
-    version='0.1.1',
+    version='0.1.2',
 
     description='Includes functions for performing econometrics tasks',
 
     # code file name without file extension
     packages=['pynometrics'],
 
     # directory in which code file is stored
```

### Comparing `pynometrics-0.1.1/src/.DS_Store` & `pynometrics-0.1.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.1/src/pynometrics/pynometrics.py` & `pynometrics-0.1.2/src/pynometrics/pynometrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,53 +198,60 @@
                 leverage = self.mdl.get_influence().hat_matrix_diag,
                 cooks_distance = self.mdl.get_influence().cooks_distance[0])
         )
         
         self.df_params = (
             
             pd.DataFrame(self.mdl.params.reset_index())
-            
             .rename(columns={"index":"var", 0:"coef"})
-            
             .assign(
                 errors = lambda X: X['coef'] - self.mdl.conf_int().iloc[:,0].values,
                 pvalues = self.mdl.pvalues.values,
                 Significant = lambda X: X['pvalues'] < 0.05)
+            .query("var != 'Intercept'")
         )
 
         
-    def plot(self):
+    def plot(self, figsize=None):
         """
         Function to generate plot for chosen diagnostic check for linear regression
         
         Args:
             None
         
         Returns
             Matplotlib plot: Plot of chosen diagnostic check
         """
         
         sns.set_style('whitegrid')
         
+        if not figsize:
+            figsize = (12,5)
+        
         params = {
-            "figure.figsize":(8,5),
+            "figure.figsize":figsize,
+            "text.color":"#162871",
             "axes.titlesize":16,
             "axes.labelsize":14,
+            "axes.labelcolor": "#162871",
+            "axes.edgecolor": "#162871",
+            "xtick.color": "#162871",
+            "ytick.color": "#162871",
             "xtick.labelsize":10,
             "ytick.labelsize":10,
             "legend.fontsize":12, 
-#             "axes.grid.axis":"y",
+            "axes.grid.axis":"y",
             "axes.spines.left":False,
             "axes.spines.top":False,
-            "axes.spines.right":False
+            "axes.spines.right":False,
+
         }
         
         plt.rcParams.update(params)
-#         plt.rcParams['axes.grid.axis'] = 'x'
-#         plt.rcParams['axes.grid'] = False
+
         
         fig, ax = plt.subplots()
         
         if self.n == 1:
             
             # rows with top residuals 
             top3 = abs(self.res_df['residuals']).sort_values(ascending = False)[:3]
@@ -454,16 +461,19 @@
             ax.axvline(x = 0, linestyle = '--', color = '#F08080', linewidth = 1)
 
             plt.title('95% confidence intervals')
 
             ax.set_ylabel('Coefficients')
 
             ax.set_xlabel('estimates')
+            
+            ax.xaxis.grid(False)
+
+            
 
-        return fig
 
 def repr_table(models, model_number=False):
     """
     Function for displaying models from statsmodels in one table
     
     Args:
         models (list) list of models to display
```

### Comparing `pynometrics-0.1.1/src/pynometrics.egg-info/PKG-INFO` & `pynometrics-0.1.2/src/pynometrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynometrics
-Version: 0.1.1
+Version: 0.1.2
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/econometric_package.git
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

