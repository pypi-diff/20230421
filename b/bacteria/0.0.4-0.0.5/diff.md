# Comparing `tmp/bacteria-0.0.4.tar.gz` & `tmp/bacteria-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.0.4.tar", last modified: Fri Apr 21 11:22:19 2023, max compression
+gzip compressed data, was "bacteria-0.0.5.tar", last modified: Fri Apr 21 11:26:43 2023, max compression
```

## Comparing `bacteria-0.0.4.tar` & `bacteria-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:22:19.539000 bacteria-0.0.4/
--rw-rw-rw-   0        0        0      606 2023-04-21 11:22:19.456000 bacteria-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:22:19.179000 bacteria-0.0.4/bacteria/
--rw-rw-rw-   0        0        0      681 2023-04-21 11:22:10.000000 bacteria-0.0.4/bacteria/__init__.py
--rw-rw-rw-   0        0        0   147595 2023-04-21 11:22:10.000000 bacteria-0.0.4/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 11:22:09.000000 bacteria-0.0.4/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:22:19.439000 bacteria-0.0.4/bacteria.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 11:22:18.000000 bacteria-0.0.4/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:22:19.512000 bacteria-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-04-21 11:22:08.000000 bacteria-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:26:43.709000 bacteria-0.0.5/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:26:43.627000 bacteria-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:26:43.231000 bacteria-0.0.5/bacteria/
+-rw-rw-rw-   0        0        0      721 2023-04-21 11:26:10.000000 bacteria-0.0.5/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   148191 2023-04-21 11:26:24.000000 bacteria-0.0.5/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 11:26:24.000000 bacteria-0.0.5/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:26:43.608000 bacteria-0.0.5/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:26:42.000000 bacteria-0.0.5/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-21 11:26:42.000000 bacteria-0.0.5/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:26:42.000000 bacteria-0.0.5/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 11:26:42.000000 bacteria-0.0.5/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 11:26:42.000000 bacteria-0.0.5/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:26:43.679000 bacteria-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-04-21 11:26:39.000000 bacteria-0.0.5/setup.py
```

### Comparing `bacteria-0.0.4/PKG-INFO` & `bacteria-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.4
+Version: 0.0.5
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.4/bacteria/__init__.py` & `bacteria-0.0.5/bacteria/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os
-import sys
-import time
-import shutil
-import graphviz
-import scipy.io
-# import matlab.engine
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-from IPython import display
-from scipy.stats import sem
-from natsort import natsorted # pip install natsort
+# import os
+# import sys
+# import time
+# import shutil
+# import graphviz
+# import scipy.io
+# # import matlab.engine
+# import numpy as np
+# import pandas as pd
+# import seaborn as sns
+# import matplotlib.pyplot as plt
+# from IPython import display
+# from scipy.stats import sem
+# from natsort import natsorted # pip install natsort
 from bacteria.functions import *
 from bacteria.pipeline import *
-from datetime import date,timedelta
-from matplotlib.lines import Line2D
-from sklearn import preprocessing as pre
-from sklearn.linear_model import LinearRegression
-from scipy.signal import savgol_filter, argrelextrema
-from anytree import Node, RenderTree, PostOrderIter # pip install anytree
+# from datetime import date,timedelta
+# from matplotlib.lines import Line2D
+# from sklearn import preprocessing as pre
+# from sklearn.linear_model import LinearRegression
+# from scipy.signal import savgol_filter, argrelextrema
+# from anytree import Node, RenderTree, PostOrderIter # pip install anytree
```

### Comparing `bacteria-0.0.4/bacteria/functions.py` & `bacteria-0.0.5/bacteria/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+import os
+import sys
+import time
+import shutil
+import graphviz
+import scipy.io
+# import matlab.engine
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
+from IPython import display
+from scipy.stats import sem
+from natsort import natsorted # pip install natsort
+from datetime import date,timedelta
+from matplotlib.lines import Line2D
+from sklearn import preprocessing as pre
+from sklearn.linear_model import LinearRegression
+from scipy.signal import savgol_filter, argrelextrema
+from anytree import Node, RenderTree, PostOrderIter # pip install anytree
+
+
 def interactive_table(df_list, cell = None, labels = None):
     """
     Creates an interactive table with statistics using a DataFrame as input. 
     
     Parameters
     --------------
     df_list: list
```

### Comparing `bacteria-0.0.4/bacteria/pipeline.py` & `bacteria-0.0.5/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.4/bacteria.egg-info/PKG-INFO` & `bacteria-0.0.5/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.4
+Version: 0.0.5
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.4/setup.py` & `bacteria-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.0.4',      
+    version = '0.0.5',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/markdown",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

