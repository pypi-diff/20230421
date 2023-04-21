# Comparing `tmp/bacteria-0.0.8.tar.gz` & `tmp/bacteria-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.0.8.tar", last modified: Fri Apr 21 14:12:56 2023, max compression
+gzip compressed data, was "bacteria-0.0.9.tar", last modified: Fri Apr 21 14:48:14 2023, max compression
```

## Comparing `bacteria-0.0.8.tar` & `bacteria-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:12:56.335000 bacteria-0.0.8/
--rw-rw-rw-   0        0        0      606 2023-04-21 14:12:56.259000 bacteria-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:12:55.976000 bacteria-0.0.8/bacteria/
--rw-rw-rw-   0        0        0      721 2023-04-21 11:26:10.000000 bacteria-0.0.8/bacteria/__init__.py
--rw-rw-rw-   0        0        0   140541 2023-04-21 14:12:44.000000 bacteria-0.0.8/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.0.8/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:12:56.210000 bacteria-0.0.8/bacteria.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 14:12:55.000000 bacteria-0.0.8/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:12:56.306000 bacteria-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-04-21 14:12:50.000000 bacteria-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:48:14.669000 bacteria-0.0.9/
+-rw-rw-rw-   0        0        0      606 2023-04-21 14:48:14.537000 bacteria-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:48:13.748000 bacteria-0.0.9/bacteria/
+-rw-rw-rw-   0        0        0      721 2023-04-21 11:26:10.000000 bacteria-0.0.9/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   140140 2023-04-21 14:40:24.000000 bacteria-0.0.9/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.0.9/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:48:14.377000 bacteria-0.0.9/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-21 14:48:12.000000 bacteria-0.0.9/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-21 14:48:12.000000 bacteria-0.0.9/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:48:12.000000 bacteria-0.0.9/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 14:48:12.000000 bacteria-0.0.9/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 14:48:12.000000 bacteria-0.0.9/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:48:14.632000 bacteria-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-04-21 14:47:55.000000 bacteria-0.0.9/setup.py
```

### Comparing `bacteria-0.0.8/PKG-INFO` & `bacteria-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.8
+Version: 0.0.9
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.8/bacteria/__init__.py` & `bacteria-0.0.9/bacteria/__init__.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.8/bacteria/functions.py` & `bacteria-0.0.9/bacteria/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2442,15 +2442,15 @@
         Dictionary with the order used in each cell
     """	
     if len(df_3d[df_3d['Cell ID']==reverse_lineage[-1]]) == 0:
         keys = natsorted(reverse_lineage[:-1])
     else:
         keys = natsorted(reverse_lineage)
 
-    df_deriv,_ = derivative(df_3d[df_3d['Cell ID'].isin(keys)],column=column)
+    df_deriv,_ = derivative(df_3d[df_3d['Cell ID'].isin(keys)],column=column,bar = False)
 
     x_vol_sep,x_vol_order,cell_cycle = {},{},{}
 
     count = 0
     order_dict = {}
 
     for idx,cell in enumerate(keys):
@@ -2761,15 +2761,15 @@
 					filtered_lineage.append(reverse_lineages[cell])
 		else:
 			if cell in natsorted(set(lineages_corr)):
 					filtered_lineage.append(reverse_lineages[cell])
 	
 	return filtered_lineage
 
-def plot_lineage_derivative(df_lineage,peaks,plot_params = None,x_axis = 'Smoothed Volume',ax = None):
+def plot_lineage_derivative(df_lineage,peaks,column = 'Fluor1 sum',derivative_column = 'Derivative',x_axis = 'Smoothed Volume',ax = None):
     """
     Plot a single lineages derivative with the
     local minima and local maxmia. The input parameters
     are the output of 'lineage_derivative()'. This 
     function can receive both volume ('Smoothed Volume')
     and time ('Time (fps)') as the X axis.
 
@@ -2779,18 +2779,14 @@
         DataFrame output of 'lineage_derivative()' with all
         data necesseary to plot the lineages.
     peaks : dict
         Dictionary data with the indexes of local minima and
         local maxima related to 'Smoothed Volume','Smoothed 
         Derivative' and 'Time (fps)'. Output of 
         'lineage_derivative()'
-    plot_params : dict (optional)
-        Dict with the parameters used to estimate the derivative
-        of the lineage (column name, norm, log). Output of 
-        'lineage_derivative()'
     x_axis : str (optional)
         Column to use as X axis in the plot. Should be 'Smoothed 
         Volume' (default) or 'Time (fps)'.
     ax : nd.array (optional)
         Pass the ax for subplot.
             
     Returns
@@ -2813,29 +2809,26 @@
         for cell in cells:
             plt.axvline(df_lineage[df_lineage['Cell ID']==cell][x_axis].values[-1],linestyle='--',color="darkgray", zorder=1, label=for_label)
             for_label = "_nolegend_"
         plt.title('Lineage {}-{}'.format(cells[0],cells[-1]), fontsize = 17)
         plt.axhline(np.mean(df_lineage['Smoothed Derivative'].values),linestyle=':',color="gray",label='Mean')
         if x_axis == 'Time (fps)':
             plt.xlabel('Time (min)', fontsize = 15)
-        elif x_axis == 'Smoothed Volume':
+        elif x_axis == 'Smoothed Volume' or x_axis == 'Volume':
             plt.xlabel(r'Volume [$\mu m^3$]', fontsize = 15)
         else:
             plt.xlabel(x_axis, fontsize = 15)
-        if plot_params is not None:
-            if plot_params['norm'] and plot_params['log']:
-                plt.ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(plot_params['column']), fontsize = 17)
-            elif plot_params['norm']:
-                plt.ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(plot_params['column']), fontsize = 17)
-            elif plot_params['log']:
-                plt.ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(plot_params['column']), fontsize = 17)
-            else:
-                plt.ylabel(r'$\frac{\partial %s}{\partial t}$'%(plot_params['column']), fontsize = 17)
-        else:
-            plt.ylabel('Derivative', fontsize = 17)
+        if derivative_column == 'Log Derivative/V':
+            plt.ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15)
+        elif derivative_column == 'Derivative/V':
+            plt.ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15)
+        elif derivative_column == 'Log Derivative':
+            plt.ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(column), fontsize = 15)
+        elif derivative_column == 'Derivative':
+            plt.ylabel(r'$\frac{\partial %s}{\partial t}$'%(column), fontsize = 15)
         plt.legend(bbox_to_anchor=(1.05, 1),loc="upper left", borderaxespad=0.,ncol=1)
         plt.show()
     else:
         out = []
         for cell in cells:
             out.append(ax.plot(df_lineage[df_lineage['Cell ID']==cell][x_axis],df_lineage[df_lineage['Cell ID']==cell]['Derivative'],'.',label = 'Cell {}'.format(cell)))
         out.append(ax.plot(df_lineage[x_axis].values,df_lineage['Smoothed Derivative'].values,'k',label = 'Smoothed Derivative'))
@@ -2850,25 +2843,22 @@
         out.append(ax.axhline(np.mean(df_lineage['Smoothed Derivative'].values),linestyle=':',color="gray",label='Mean'))
         if x_axis == 'Time (fps)':
             out.append(ax.set_xlabel('Time (min)', fontsize = 15))
         elif x_axis == 'Smoothed Volume':
             out.append(ax.set_xlabel(r'Volume [$\mu m^3$]', fontsize = 15))
         else:
             out.append(ax.set_xlabel(x_axis, fontsize = 15))
-        if plot_params is not None:
-            if plot_params['norm'] and plot_params['log']:
-                out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(plot_params['column']), fontsize = 17))
-            elif plot_params['norm']:
-                out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(plot_params['column']), fontsize = 17))
-            elif plot_params['log']:
-                out.append(ax.set_ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(plot_params['column']), fontsize = 17))
-            else:
-                out.append(ax.set_ylabel(r'$\frac{\partial %s}{\partial t}$'%(plot_params['column']), fontsize = 17))
-        else:
-            out.append(ax.set_ylabel('Derivative', fontsize = 17))        
+        if derivative_column == 'Log Derivative/V':
+           out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
+        elif derivative_column == 'Derivative/V':
+           out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
+        elif derivative_column == 'Log Derivative':
+            out.append(ax.set_ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(column), fontsize = 15))
+        elif derivative_column == 'Derivative':
+            out.append(ax.set_ylabel(r'$\frac{\partial %s}{\partial t}$'%(column), fontsize = 15))
         out.append(ax.legend(bbox_to_anchor=(1.05, 1),loc="upper left", borderaxespad=0.,ncol=1))
 
         return out
 
 def plot_lineage_ratio(df_lineage,x_axis = 'Smoothed Volume',ax = None):
     """
     Plot a single lineages F/V ratio. The input parameters
```

### Comparing `bacteria-0.0.8/bacteria/pipeline.py` & `bacteria-0.0.9/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.8/bacteria.egg-info/PKG-INFO` & `bacteria-0.0.9/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.8
+Version: 0.0.9
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.8/setup.py` & `bacteria-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.0.8',      
+    version = '0.0.9',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/markdown",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

