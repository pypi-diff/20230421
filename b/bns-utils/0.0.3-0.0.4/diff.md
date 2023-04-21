# Comparing `tmp/bns_utils-0.0.3.tar.gz` & `tmp/bns_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bns_utils-0.0.3.tar", last modified: Thu Apr 20 06:14:08 2023, max compression
+gzip compressed data, was "bns_utils-0.0.4.tar", last modified: Fri Apr 21 07:21:35 2023, max compression
```

## Comparing `bns_utils-0.0.3.tar` & `bns_utils-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 06:14:08.560245 bns_utils-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-02-21 06:46:37.000000 bns_utils-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3302 2023-04-20 06:14:08.558244 bns_utils-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2773 2023-02-21 13:01:48.000000 bns_utils-0.0.3/README.md
--rw-rw-rw-   0        0        0      832 2023-04-20 06:12:31.000000 bns_utils-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 06:14:08.560245 bns_utils-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 06:14:08.481239 bns_utils-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 06:14:08.539238 bns_utils-0.0.3/src/BNS_UTILS.egg-info/
--rw-rw-rw-   0        0        0     3302 2023-04-20 06:14:08.000000 bns_utils-0.0.3/src/BNS_UTILS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      589 2023-04-20 06:14:08.000000 bns_utils-0.0.3/src/BNS_UTILS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 06:14:08.000000 bns_utils-0.0.3/src/BNS_UTILS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-20 06:14:08.000000 bns_utils-0.0.3/src/BNS_UTILS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 06:14:08.000000 bns_utils-0.0.3/src/BNS_UTILS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 06:14:08.552239 bns_utils-0.0.3/src/bns_utils/
--rw-rw-rw-   0        0        0    28840 2023-04-19 13:44:28.000000 bns_utils-0.0.3/src/bns_utils/TransferFunction.py
--rw-rw-rw-   0        0        0        0 2023-02-21 06:31:53.000000 bns_utils-0.0.3/src/bns_utils/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-02-21 12:09:02.000000 bns_utils-0.0.3/src/bns_utils/data.py
--rw-rw-rw-   0        0        0    13703 2023-03-08 10:08:43.000000 bns_utils-0.0.3/src/bns_utils/fluidreports.py
--rw-rw-rw-   0        0        0     6519 2023-02-21 10:34:32.000000 bns_utils-0.0.3/src/bns_utils/general.py
--rw-rw-rw-   0        0        0     2018 2023-04-20 06:07:25.000000 bns_utils-0.0.3/src/bns_utils/monitor.py
-drwxrwxrwx   0        0        0        0 2023-04-20 06:14:08.556239 bns_utils-0.0.3/tests/
--rw-rw-rw-   0        0        0      385 2023-03-08 10:32:12.000000 bns_utils-0.0.3/tests/test_fluidreports.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:21:35.482874 bns_utils-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 06:46:37.000000 bns_utils-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3302 2023-04-21 07:21:35.481867 bns_utils-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2773 2023-02-21 13:01:48.000000 bns_utils-0.0.4/README.md
+-rw-rw-rw-   0        0        0      774 2023-04-21 07:17:03.000000 bns_utils-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 07:21:35.482874 bns_utils-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 07:21:35.429774 bns_utils-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 07:21:35.469856 bns_utils-0.0.4/src/BNS_UTILS.egg-info/
+-rw-rw-rw-   0        0        0     3302 2023-04-21 07:21:35.000000 bns_utils-0.0.4/src/BNS_UTILS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-04-21 07:21:35.000000 bns_utils-0.0.4/src/BNS_UTILS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:21:35.000000 bns_utils-0.0.4/src/BNS_UTILS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-21 07:21:35.000000 bns_utils-0.0.4/src/BNS_UTILS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 07:21:35.000000 bns_utils-0.0.4/src/BNS_UTILS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 07:21:35.476868 bns_utils-0.0.4/src/bns_utils/
+-rw-rw-rw-   0        0        0    28840 2023-04-19 13:44:28.000000 bns_utils-0.0.4/src/bns_utils/TransferFunction.py
+-rw-rw-rw-   0        0        0        0 2023-02-21 06:31:53.000000 bns_utils-0.0.4/src/bns_utils/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-02-21 12:09:02.000000 bns_utils-0.0.4/src/bns_utils/data.py
+-rw-rw-rw-   0        0        0    13703 2023-03-08 10:08:43.000000 bns_utils-0.0.4/src/bns_utils/fluidreports.py
+-rw-rw-rw-   0        0        0     6406 2023-04-20 06:51:20.000000 bns_utils-0.0.4/src/bns_utils/general.py
+-rw-rw-rw-   0        0        0     3668 2023-04-21 07:16:44.000000 bns_utils-0.0.4/src/bns_utils/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:21:35.479903 bns_utils-0.0.4/tests/
+-rw-rw-rw-   0        0        0      385 2023-03-08 10:32:12.000000 bns_utils-0.0.4/tests/test_fluidreports.py
```

### Comparing `bns_utils-0.0.3/LICENSE` & `bns_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.3/PKG-INFO` & `bns_utils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bns_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Some utilities for BNS internal use
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Dave-the-python-developer/BNS_utils
 Project-URL: PyPi, https://pypi.org/project/bns-utils/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bns_utils-0.0.3/README.md` & `bns_utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.3/pyproject.toml` & `bns_utils-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bns_utils"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Some utilities for BNS internal use"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'cycler >= 0.11.0, < 1',
     'matplotlib >= 3.5.0, < 5',
-    'tqdm >= 4.64.0, < 5',
     'pandas >= 1.5.0, < 2',
     'scipy >= 1.9.0, < 2'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Dave-the-python-developer/BNS_utils"
 "PyPi" = "https://pypi.org/project/bns-utils/"
```

### Comparing `bns_utils-0.0.3/src/BNS_UTILS.egg-info/PKG-INFO` & `bns_utils-0.0.4/src/BNS_UTILS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bns-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Some utilities for BNS internal use
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Dave-the-python-developer/BNS_utils
 Project-URL: PyPi, https://pypi.org/project/bns-utils/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bns_utils-0.0.3/src/BNS_UTILS.egg-info/SOURCES.txt` & `bns_utils-0.0.4/src/BNS_UTILS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.3/src/bns_utils/TransferFunction.py` & `bns_utils-0.0.4/src/bns_utils/TransferFunction.py`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.3/src/bns_utils/data.py` & `bns_utils-0.0.4/src/bns_utils/data.py`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.3/src/bns_utils/fluidreports.py` & `bns_utils-0.0.4/src/bns_utils/fluidreports.py`

 * *Files identical despite different names*

### Comparing `bns_utils-0.0.3/src/bns_utils/general.py` & `bns_utils-0.0.4/src/bns_utils/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import matplotlib.pyplot as plt 
-from cycler import cycler
 import matplotlib
-from tqdm import tqdm
 import ipywidgets as widgets
 from ipywidgets import interact
 import glob
 import pandas as pd
 import os
 from scipy.signal import butter, filtfilt
 
@@ -14,15 +12,17 @@
 #setting the figure paramters 
 plt.rcParams['figure.figsize'] = [10, 6]
 plt.rcParams['figure.dpi'] = 100 # 200 e.g. is really fine, but slower
 plt.rcParams['font.size'] = 14
 plt.rcParams['font.family'] = 'Trebuchet MS'
 
 #setting the color parameters
-matplotlib.rcParams['axes.prop_cycle'] = cycler('color', ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf'])
+colors = ["#1f77b4", "#ff7f0e", "#2ca02c", "#d62728", "#9467bd","#8c564b", "#e377c2", "#7f7f7f", "#bcbd22", "#17becf"]
+prop_cycle = [("color", color) for color in colors]
+matplotlib.rcParams['axes.prop_cycle'] = prop_cycle
 
 
 def concat_csv_IP21_data(path):
 
     '''
     Documentation:
 
@@ -48,15 +48,15 @@
     DF = BNS.concat_csv_IP21_data(path)
 
     '''
     extension = 'csv'
     all_files = [i for i in glob.glob('*.{}'.format(extension))]
     DF = pd.DataFrame()
     os.chdir(path)
-    for file in tqdm(all_files):
+    for file in all_files:
         #read and concatenate the data
         col_name = file[:-4]
         df = pd.read_csv(file)
         df['TS'] = pd.to_datetime(df['TS'])
         df.rename(columns = {'Value':col_name},inplace=True)
         df.set_index('TS',inplace=True)
         DF = pd.concat([DF,df],axis=1)
@@ -139,16 +139,16 @@
     BNS.plot_x_y_data(data, widget = False, start_date = None, end_date = None)
 
     '''
 
     matplotlib.rcParams['figure.figsize'] = [16, 6]
     matplotlib.rcParams['figure.dpi'] = 100 # 200 e.g. is really fine, but slower
     matplotlib.rcParams['font.size'] = 14
-    matplotlib.rcParams['font.family'] = 'Trebuchet MS'
-    matplotlib.rcParams['axes.prop_cycle'] = cycler('color', ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf'])
+    matplotlib.rcParams['font.family'] = 'Trebuchet MS'    
+    matplotlib.rcParams['axes.prop_cycle'] = prop_cycle
     #if the widget is not specified then I will create a widget for the user to select the columns to plot
     if widget == False:
         widget = widgets.SelectMultiple(
             options=data.columns,
             value=[data.columns[0]],
             #rows=10,
             description='Columns',
```

### Comparing `bns_utils-0.0.3/src/bns_utils/monitor.py` & `bns_utils-0.0.4/src/bns_utils/monitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import subprocess
 import requests
 import time
 from socket import gethostname,gethostbyname
+import smtplib
+from email.message import EmailMessage
 
 # You can find the bot token and chat id on: https://bluenickel.sharepoint.com/:x:/r/_layouts/15/Doc.aspx?sourcedoc=%7B4B85D1DB-87C0-472F-91C9-27EA70195A71%7D&file=BNS_Telegram_Bots_and_Groups.xlsx&action=default&mobileredirect=true
-class QuickMonitor:
+class QuickMonitorTelegram:
     def __init__(self,telegram_bot_token,telegram_chat_id,service_list,freq):
         # Telegram Bot token and chat ID
         self.token = telegram_bot_token
         self.chat_id = telegram_chat_id
         # Service names to monitor
         self.services = service_list        
         self.machine_ip = gethostbyname(gethostname())
@@ -35,8 +37,45 @@
                 # Run the command to check if the service is running
                 result = subprocess.check_output(f'sc query "{service}"', shell=True, text=True)
                 # If the service is not active, append it to the list
                 if not "RUNNING" in result:
                     stopped_services.append(service)                
             except:
                 pass
-        return stopped_services
+        return stopped_services
+    
+class QuickMonitorTeams:
+    def __init__(self,smtp_server, smtp_port, smtp_user, smtp_password,service_list,freq):
+        # SMTP server details
+        self.smtp_server = smtp_server
+        self.smtp_port = smtp_port
+        self.smptp_user = smtp_user
+        self.smtp_password = smtp_password
+        #user with power automate flow
+        self.to = "james@bluenickel.co.za"
+        #subject that tirggers outlook rule
+        self.subject = "Power Automate Service Monitor Mail"
+        # Service names to monitor
+        self.services = service_list        
+        self.machine_ip = gethostbyname(gethostname())
+        # Command to check if the service is running
+        while True:
+            stopped = self.check_services()
+            if len(stopped) > 0:
+               service_str = ", ".join(str(x) for x in stopped)
+               body = f"The following services have stopped on machine {self.machine_ip}:\n" + service_str
+               self.send_email(body)
+            time.sleep(freq)  # Execute the task every freq seconds  
+
+    def send_email(self,body):
+        msg = EmailMessage()
+        msg.set_content(body)
+        msg['Subject'] = self.subject
+        msg['From'] = self.smptp_user
+        msg['To'] = self.to
+        try:
+            with smtplib.SMTP(self.smtp_server, self.smtp_port) as server:
+                server.login(self.smtp_user, self.smtp_password)
+                server.send_message(msg)            
+        except Exception as e:
+            #maybe write the error to a log??
+            pass
```

