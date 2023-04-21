# Comparing `tmp/bacteria-0.0.7.tar.gz` & `tmp/bacteria-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.0.7.tar", last modified: Fri Apr 21 14:10:37 2023, max compression
+gzip compressed data, was "bacteria-0.0.8.tar", last modified: Fri Apr 21 14:12:56 2023, max compression
```

## Comparing `bacteria-0.0.7.tar` & `bacteria-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:36.919000 bacteria-0.0.7/
--rw-rw-rw-   0        0        0      606 2023-04-21 14:10:36.693000 bacteria-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:36.253000 bacteria-0.0.7/bacteria/
--rw-rw-rw-   0        0        0      721 2023-04-21 11:26:10.000000 bacteria-0.0.7/bacteria/__init__.py
--rw-rw-rw-   0        0        0   140531 2023-04-21 14:10:24.000000 bacteria-0.0.7/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.0.7/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:36.652000 bacteria-0.0.7/bacteria.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-21 14:10:35.000000 bacteria-0.0.7/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-21 14:10:35.000000 bacteria-0.0.7/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:10:35.000000 bacteria-0.0.7/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 14:10:35.000000 bacteria-0.0.7/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 14:10:35.000000 bacteria-0.0.7/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:10:36.883000 bacteria-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-04-21 14:10:30.000000 bacteria-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:12:56.335000 bacteria-0.0.8/
+-rw-rw-rw-   0        0        0      606 2023-04-21 14:12:56.259000 bacteria-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:12:55.976000 bacteria-0.0.8/bacteria/
+-rw-rw-rw-   0        0        0      721 2023-04-21 11:26:10.000000 bacteria-0.0.8/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   140541 2023-04-21 14:12:44.000000 bacteria-0.0.8/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.0.8/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:12:56.210000 bacteria-0.0.8/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:12:56.306000 bacteria-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-04-21 14:12:50.000000 bacteria-0.0.8/setup.py
```

### Comparing `bacteria-0.0.7/PKG-INFO` & `bacteria-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.7
+Version: 0.0.8
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.7/bacteria/__init__.py` & `bacteria-0.0.8/bacteria/__init__.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.7/bacteria/functions.py` & `bacteria-0.0.8/bacteria/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1394,20 +1394,21 @@
     plus : int (optional)
         value to change the window to the convolution
         to adapt the range for the loop 
         (e.g, default = i in range(1,len(x)-2))
         
     Returns
     --------------
+    df_derivative : DataFrame
+        DataFrame with the deravtives data alongside with 
+        the time and volume 
     dict_derivative : dict
         A dict with other dicts that contains the 
         [volume,fluor,time,F/V and all derivatives] 
-        of each cell at the slide window (cell number = key),
-    df_derivative : DataFrame
-        DataFrame with the deravtive data alongside with the time and volume 
+        of each cell at the slide window (cell number = key).
     """
     if column == 'Volume':
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
     else:
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V','Volume'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
     
     dict_derivative,vol_dict,time_dict,bin_dict,ratio_dict = {},{},{},{},{}
@@ -1500,15 +1501,15 @@
                                     columns=['Cell ID','Time (fps)','F/V','Volume','Derivative','Derivative/V','Derivative Log','Derivative Log/V','Cell Cycle']))
         
     df_derivative = pd.concat(df_temp, ignore_index=True)
     dict_derivative['Volume'],dict_derivative['Time (fps)'],dict_derivative['F/V'] = vol_dict,time_dict,ratio_dict
     dict_derivative['Cell Cycle'],dict_derivative['Derivative'],dict_derivative['Derivative/V'] = bin_dict,dev_dict,dev_dict_norm
     dict_derivative['Derivative Log'], dict_derivative['Derivative Log/V'] = dev_dict_log,dev_dict_log_norm
 
-    return dict_derivative,df_derivative
+    return df_derivative,dict_derivative
 
 def column_mean(df,column,conf = .95, method = np.mean, plot_hist = False):
 	"""
 	Estimate the column mean for all cells using
 	the 'pd.melt()' method, sorting by time.
 
 	Parameters
@@ -2441,15 +2442,15 @@
         Dictionary with the order used in each cell
     """	
     if len(df_3d[df_3d['Cell ID']==reverse_lineage[-1]]) == 0:
         keys = natsorted(reverse_lineage[:-1])
     else:
         keys = natsorted(reverse_lineage)
 
-    _,df_deriv = derivative(df_3d[df_3d['Cell ID'].isin(keys)],column=column)
+    df_deriv,_ = derivative(df_3d[df_3d['Cell ID'].isin(keys)],column=column)
 
     x_vol_sep,x_vol_order,cell_cycle = {},{},{}
 
     count = 0
     order_dict = {}
 
     for idx,cell in enumerate(keys):
```

### Comparing `bacteria-0.0.7/bacteria/pipeline.py` & `bacteria-0.0.8/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.7/bacteria.egg-info/PKG-INFO` & `bacteria-0.0.8/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.7
+Version: 0.0.8
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.7/setup.py` & `bacteria-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.0.7',      
+    version = '0.0.8',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/markdown",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

